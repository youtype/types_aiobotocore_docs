<a id="examples-for-aiobotocore-lambda-module"></a>

# Examples for aiobotocore Lambda module

> [Index](../README.md) > [Lambda](./README.md) > Examples

- [Examples for aiobotocore Lambda module](#examples-for-aiobotocore-lambda-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[lambda]` package installed.

Write your `Lambda` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type LambdaClient
# and provides type checking and code completion
async with session.create_client("lambda") as client:
    
    # result has type AddLayerVersionPermissionResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_layer_version_permission()
    

    
    # paginator has type ListAliasesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_aliases")
    async for item in paginator.paginate(...):
        # item has type ListAliasesResponseTypeDef
        print(item)
    

    
    # waiter has type FunctionActiveWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("function_active")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[lambda]` or a standalone
`types_aiobotocore_lambda` package, you have to explicitly specify
`client: LambdaClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_lambda.client import LambdaClient
from types_aiobotocore_lambda.type_defs import AddLayerVersionPermissionResponseTypeDef
from types_aiobotocore_lambda.paginator import ListAliasesPaginator
from types_aiobotocore_lambda.waiter import FunctionActiveWaiter
from types_aiobotocore_lambda.literals import PaginatorName
from types_aiobotocore_lambda.literals import WaiterName


session = get_session()

async with session.create_client("lambda") as client:
    client: LambdaClient

    
    result: AddLayerVersionPermissionResponseTypeDef = client.add_layer_version_permission()
    

    
    paginator_name: PaginatorName = "list_aliases"
    paginator: ListAliasesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAliasesResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "function_active"
    waiter: FunctionActiveWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
