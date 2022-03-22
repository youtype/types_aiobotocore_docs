<a id="examples-for-aiobotocore-simpledb-module"></a>

# Examples for aiobotocore SimpleDB module

> [Index](../README.md) > [SimpleDB](./README.md) > Examples

- [Examples for aiobotocore SimpleDB module](#examples-for-aiobotocore-simpledb-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sdb]` package installed.

Write your `SimpleDB` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SimpleDBClient
# and provides type checking and code completion
async with session.create_client("sdb") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_delete_attributes()
    

    
    # paginator has type ListDomainsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_domains")
    async for item in paginator.paginate(...):
        # item has type ListDomainsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sdb]` or a standalone `types_aiobotocore_sdb`
package, you have to explicitly specify `client: SimpleDBClient` type
annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sdb.client import SimpleDBClient
from types_aiobotocore_sdb.type_defs import None
from types_aiobotocore_sdb.paginator import ListDomainsPaginator

from types_aiobotocore_sdb.literals import PaginatorName



session = get_session()

async with session.create_client("sdb") as client:
    client: SimpleDBClient

    
    result: None = client.batch_delete_attributes()
    

    
    paginator_name: PaginatorName = "list_domains"
    paginator: ListDomainsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDomainsResultTypeDef
        print(item)
    

    
```
