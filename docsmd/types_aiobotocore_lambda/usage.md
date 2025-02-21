# Examples

> [Index](../README.md) > [Lambda](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Lambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#lambda)
    type annotations stubs module [types-aiobotocore-lambda](https://pypi.org/project/types-aiobotocore-lambda/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[lambda]` package installed.

Write your `Lambda` code as usual,
type checking and code completion should work out of the box.



```python
# LambdaClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lambda") as client:  # (1)
    result = await client.add_layer_version_permission()  # (2)
```

1. client: [LambdaClient](./client.md)
2. result: [:material-code-braces: AddLayerVersionPermissionResponseTypeDef](./type_defs.md#addlayerversionpermissionresponsetypedef) 



```python
# ListAliasesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lambda") as client:  # (1)
    paginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LambdaClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 



```python
# FunctionActiveV2Waiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lambda") as client:  # (1)
    waiter = client.get_waiter("function_active_v2")  # (2)
    await waiter.wait()
```

1. client: [LambdaClient](./client.md)
2. waiter: [FunctionActiveV2Waiter](./waiters.md#functionactivev2waiter)


### Explicit type annotations

With `types-aiobotocore-lite[lambda]`
or a standalone `types_aiobotocore_lambda` package, you have to explicitly specify
`client: LambdaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LambdaClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lambda.client import LambdaClient
from types_aiobotocore_lambda.type_defs import AddLayerVersionPermissionResponseTypeDef
from types_aiobotocore_lambda.type_defs import AddLayerVersionPermissionRequestTypeDef


session = get_session()

async with session.create_client("lambda") as client:
    client: LambdaClient
    kwargs: AddLayerVersionPermissionRequestTypeDef = {...}
    result: AddLayerVersionPermissionResponseTypeDef = await client.add_layer_version_permission(**kwargs)
```



```python
# ListAliasesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lambda.client import LambdaClient
from types_aiobotocore_lambda.paginator import ListAliasesPaginator
from types_aiobotocore_lambda.type_defs import ListAliasesResponseTypeDef


session = get_session()

async with session.create_client("lambda") as client:
    client: LambdaClient
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
    async for item in paginator.paginate(...):
        item: ListAliasesResponseTypeDef
        print(item)
```



```python
# FunctionActiveV2Waiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lambda.client import LambdaClient
from types_aiobotocore_lambda.waiter import FunctionActiveV2Waiter


session = get_session()

async with session.create_client("lambda") as client:
    client: LambdaClient
    waiter: FunctionActiveV2Waiter = client.get_waiter("function_active_v2")
    await waiter.wait()
```
