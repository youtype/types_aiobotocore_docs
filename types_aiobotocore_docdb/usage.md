<a id="examples-for-aiobotocore-docdb-module"></a>

# Examples for aiobotocore DocDB module

> [Index](../README.md) > [DocDB](./README.md) > Examples

- [Examples for aiobotocore DocDB module](#examples-for-aiobotocore-docdb-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[docdb]` package installed.

Write your `DocDB` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DocDBClient
# and provides type checking and code completion
async with session.create_client("docdb") as client:
    
    # result has type AddSourceIdentifierToSubscriptionResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_source_identifier_to_subscription()
    

    
    # paginator has type DescribeCertificatesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_certificates")
    async for item in paginator.paginate(...):
        # item has type CertificateMessageTypeDef
        print(item)
    

    
    # waiter has type DBInstanceAvailableWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("db_instance_available")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[docdb]` or a standalone `types_aiobotocore_docdb`
package, you have to explicitly specify `client: DocDBClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_docdb.client import DocDBClient
from types_aiobotocore_docdb.type_defs import AddSourceIdentifierToSubscriptionResultTypeDef
from types_aiobotocore_docdb.paginator import DescribeCertificatesPaginator
from types_aiobotocore_docdb.waiter import DBInstanceAvailableWaiter
from types_aiobotocore_docdb.literals import PaginatorName
from types_aiobotocore_docdb.literals import WaiterName


session = get_session()

async with session.create_client("docdb") as client:
    client: DocDBClient

    
    result: AddSourceIdentifierToSubscriptionResultTypeDef = client.add_source_identifier_to_subscription()
    

    
    paginator_name: PaginatorName = "describe_certificates"
    paginator: DescribeCertificatesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: CertificateMessageTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "db_instance_available"
    waiter: DBInstanceAvailableWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
