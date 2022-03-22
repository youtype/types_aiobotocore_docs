<a id="examples-for-aiobotocore-apigateway-module"></a>

# Examples for aiobotocore APIGateway module

> [Index](../README.md) > [APIGateway](./README.md) > Examples

- [Examples for aiobotocore APIGateway module](#examples-for-aiobotocore-apigateway-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[apigateway]` package installed.

Write your `APIGateway` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type APIGatewayClient
# and provides type checking and code completion
async with session.create_client("apigateway") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetApiKeysPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_api_keys")
    async for item in paginator.paginate(...):
        # item has type ApiKeysTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[apigateway]` or a standalone
`types_aiobotocore_apigateway` package, you have to explicitly specify
`client: APIGatewayClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.client import APIGatewayClient
from types_aiobotocore_apigateway.type_defs import bool
from types_aiobotocore_apigateway.paginator import GetApiKeysPaginator

from types_aiobotocore_apigateway.literals import PaginatorName



session = get_session()

async with session.create_client("apigateway") as client:
    client: APIGatewayClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_api_keys"
    paginator: GetApiKeysPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ApiKeysTypeDef
        print(item)
    

    
```
