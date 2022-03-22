<a id="examples-for-aiobotocore-apigatewayv2-module"></a>

# Examples for aiobotocore ApiGatewayV2 module

> [Index](../README.md) > [ApiGatewayV2](./README.md) > Examples

- [Examples for aiobotocore ApiGatewayV2 module](#examples-for-aiobotocore-apigatewayv2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[apigatewayv2]` package installed.

Write your `ApiGatewayV2` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ApiGatewayV2Client
# and provides type checking and code completion
async with session.create_client("apigatewayv2") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetApisPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_apis")
    async for item in paginator.paginate(...):
        # item has type GetApisResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[apigatewayv2]` or a standalone
`types_aiobotocore_apigatewayv2` package, you have to explicitly specify
`client: ApiGatewayV2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.client import ApiGatewayV2Client
from types_aiobotocore_apigatewayv2.type_defs import bool
from types_aiobotocore_apigatewayv2.paginator import GetApisPaginator

from types_aiobotocore_apigatewayv2.literals import PaginatorName



session = get_session()

async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_apis"
    paginator: GetApisPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetApisResponseTypeDef
        print(item)
    

    
```
