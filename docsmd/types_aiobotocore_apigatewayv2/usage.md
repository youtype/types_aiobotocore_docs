# Examples

> [Index](../README.md) > [ApiGatewayV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ApiGatewayV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#apigatewayv2)
    type annotations stubs module [types-aiobotocore-apigatewayv2](https://pypi.org/project/types-aiobotocore-apigatewayv2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[apigatewayv2]` package installed.

Write your `ApiGatewayV2` code as usual,
type checking and code completion should work out of the box.



```python
# ApiGatewayV2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("apigatewayv2") as client:  # (1)
    result = await client.create_api()  # (2)
```

1. client: [ApiGatewayV2Client](./client.md)
2. result: [:material-code-braces: CreateApiResponseTypeDef](./type_defs.md#createapiresponsetypedef) 



```python
# GetApisPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("apigatewayv2") as client:  # (1)
    paginator = client.get_paginator("get_apis")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetApisPaginator](./paginators.md#getapispaginator)
3. item: [:material-code-braces: GetApisResponseTypeDef](./type_defs.md#getapisresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[apigatewayv2]`
or a standalone `types_aiobotocore_apigatewayv2` package, you have to explicitly specify
`client: ApiGatewayV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ApiGatewayV2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.client import ApiGatewayV2Client
from types_aiobotocore_apigatewayv2.type_defs import CreateApiResponseTypeDef
from types_aiobotocore_apigatewayv2.type_defs import CreateApiRequestTypeDef


session = get_session()

async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    kwargs: CreateApiRequestTypeDef = {...}
    result: CreateApiResponseTypeDef = await client.create_api(**kwargs)
```



```python
# GetApisPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.client import ApiGatewayV2Client
from types_aiobotocore_apigatewayv2.paginator import GetApisPaginator
from types_aiobotocore_apigatewayv2.type_defs import GetApisResponseTypeDef


session = get_session()

async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetApisPaginator = client.get_paginator("get_apis")
    async for item in paginator.paginate(...):
        item: GetApisResponseTypeDef
        print(item)
```


