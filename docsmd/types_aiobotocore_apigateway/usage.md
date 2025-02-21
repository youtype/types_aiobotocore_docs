# Examples

> [Index](../README.md) > [APIGateway](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [APIGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#apigateway)
    type annotations stubs module [types-aiobotocore-apigateway](https://pypi.org/project/types-aiobotocore-apigateway/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[apigateway]` package installed.

Write your `APIGateway` code as usual,
type checking and code completion should work out of the box.



```python
# APIGatewayClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("apigateway") as client:  # (1)
    result = await client.create_api_key()  # (2)
```

1. client: [APIGatewayClient](./client.md)
2. result: [:material-code-braces: ApiKeyResponseTypeDef](./type_defs.md#apikeyresponsetypedef) 



```python
# GetApiKeysPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("apigateway") as client:  # (1)
    paginator = client.get_paginator("get_api_keys")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetApiKeysPaginator](./paginators.md#getapikeyspaginator)
3. item: [:material-code-braces: ApiKeysTypeDef](./type_defs.md#apikeystypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[apigateway]`
or a standalone `types_aiobotocore_apigateway` package, you have to explicitly specify
`client: APIGatewayClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# APIGatewayClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.client import APIGatewayClient
from types_aiobotocore_apigateway.type_defs import ApiKeyResponseTypeDef
from types_aiobotocore_apigateway.type_defs import CreateApiKeyRequestTypeDef


session = get_session()

async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    kwargs: CreateApiKeyRequestTypeDef = {...}
    result: ApiKeyResponseTypeDef = await client.create_api_key(**kwargs)
```



```python
# GetApiKeysPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.client import APIGatewayClient
from types_aiobotocore_apigateway.paginator import GetApiKeysPaginator
from types_aiobotocore_apigateway.type_defs import ApiKeysTypeDef


session = get_session()

async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetApiKeysPaginator = client.get_paginator("get_api_keys")
    async for item in paginator.paginate(...):
        item: ApiKeysTypeDef
        print(item)
```


