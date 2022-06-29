# ApiGatewayManagementApiClient

> [Index](../README.md) > [ApiGatewayManagementApi](./README.md) > ApiGatewayManagementApiClient

!!! note ""

    Auto-generated documentation for [ApiGatewayManagementApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
    type annotations stubs module [types-aiobotocore-apigatewaymanagementapi](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi/).

## ApiGatewayManagementApiClient

Type annotations and code completion for `#!python session.create_client("apigatewaymanagementapi")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_apigatewaymanagementapi.client import ApiGatewayManagementApiClient

session = get_session()
async with session.create_client("apigatewaymanagementapi") as client:
    client: ApiGatewayManagementApiClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("apigatewaymanagementapi").exceptions` structure.

```python title="Usage example"
async with session.create_client("apigatewaymanagementapi") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ForbiddenException,
        client.GoneException,
        client.LimitExceededException,
        client.PayloadTooLargeException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_apigatewaymanagementapi.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("apigatewaymanagementapi").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("apigatewaymanagementapi").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### delete\_connection

Delete the connection with the provided id.

Type annotations and code completion for `#!python session.create_client("apigatewaymanagementapi").delete_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.delete_connection)

```python title="Method definition"
await def delete_connection(
    self,
    *,
    ConnectionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: DeleteConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionId": ...,
}

parent.delete_connection(**kwargs)
```

1. See [:material-code-braces: DeleteConnectionRequestRequestTypeDef](./type_defs.md#deleteconnectionrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("apigatewaymanagementapi").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_connection

Get information about the connection with the provided id.

Type annotations and code completion for `#!python session.create_client("apigatewaymanagementapi").get_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.get_connection)

```python title="Method definition"
await def get_connection(
    self,
    *,
    ConnectionId: str,
) -> GetConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConnectionResponseTypeDef](./type_defs.md#getconnectionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionId": ...,
}

parent.get_connection(**kwargs)
```

1. See [:material-code-braces: GetConnectionRequestRequestTypeDef](./type_defs.md#getconnectionrequestrequesttypedef) 

### post\_to\_connection

Sends the provided data to the specified connection.

Type annotations and code completion for `#!python session.create_client("apigatewaymanagementapi").post_to_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.post_to_connection)

```python title="Method definition"
await def post_to_connection(
    self,
    *,
    Data: Union[str, bytes, IO[Any], StreamingBody],
    ConnectionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python title="Usage example with kwargs"
kwargs: PostToConnectionRequestRequestTypeDef = {  # (1)
    "Data": ...,
    "ConnectionId": ...,
}

parent.post_to_connection(**kwargs)
```

1. See [:material-code-braces: PostToConnectionRequestRequestTypeDef](./type_defs.md#posttoconnectionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("apigatewaymanagementapi").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> ApiGatewayManagementApiClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("apigatewaymanagementapi").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





