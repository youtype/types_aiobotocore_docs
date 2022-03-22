<a id="examples-for-aiobotocore-mwaa-module"></a>

# Examples for aiobotocore MWAA module

> [Index](../README.md) > [MWAA](./README.md) > Examples

- [Examples for aiobotocore MWAA module](#examples-for-aiobotocore-mwaa-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mwaa]` package installed.

Write your `MWAA` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MWAAClient
# and provides type checking and code completion
async with session.create_client("mwaa") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListEnvironmentsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_environments")
    async for item in paginator.paginate(...):
        # item has type ListEnvironmentsOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mwaa]` or a standalone `types_aiobotocore_mwaa`
package, you have to explicitly specify `client: MWAAClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mwaa.client import MWAAClient
from types_aiobotocore_mwaa.type_defs import bool
from types_aiobotocore_mwaa.paginator import ListEnvironmentsPaginator

from types_aiobotocore_mwaa.literals import PaginatorName



session = get_session()

async with session.create_client("mwaa") as client:
    client: MWAAClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_environments"
    paginator: ListEnvironmentsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListEnvironmentsOutputTypeDef
        print(item)
    

    
```
