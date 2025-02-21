# Examples

> [Index](../README.md) > [ApiGatewayManagementApi](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ApiGatewayManagementApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#apigatewaymanagementapi)
    type annotations stubs module [types-aiobotocore-apigatewaymanagementapi](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[apigatewaymanagementapi]` package installed.

Write your `ApiGatewayManagementApi` code as usual,
type checking and code completion should work out of the box.



```python
# ApiGatewayManagementApiClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("apigatewaymanagementapi") as client:  # (1)
    result = await client.delete_connection()  # (2)
```

1. client: [ApiGatewayManagementApiClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[apigatewaymanagementapi]`
or a standalone `types_aiobotocore_apigatewaymanagementapi` package, you have to explicitly specify
`client: ApiGatewayManagementApiClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ApiGatewayManagementApiClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_apigatewaymanagementapi.client import ApiGatewayManagementApiClient
from types_aiobotocore_apigatewaymanagementapi.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_apigatewaymanagementapi.type_defs import DeleteConnectionRequestTypeDef


session = get_session()

async with session.create_client("apigatewaymanagementapi") as client:
    client: ApiGatewayManagementApiClient
    kwargs: DeleteConnectionRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.delete_connection(**kwargs)
```




