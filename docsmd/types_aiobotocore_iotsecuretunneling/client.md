# IoTSecureTunnelingClient

> [Index](../README.md) > [IoTSecureTunneling](./README.md) > IoTSecureTunnelingClient

!!! note ""

    Auto-generated documentation for [IoTSecureTunneling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#iotsecuretunneling)
    type annotations stubs module [types-aiobotocore-iotsecuretunneling](https://pypi.org/project/types-aiobotocore-iotsecuretunneling/).

## IoTSecureTunnelingClient

Type annotations and code completion for `#!python session.create_client("iotsecuretunneling")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client)

```python
# IoTSecureTunnelingClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iotsecuretunneling.client import IoTSecureTunnelingClient

session = get_session()
async with session.create_client("iotsecuretunneling") as client:
    client: IoTSecureTunnelingClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iotsecuretunneling").exceptions` structure.

```python
# IoTSecureTunnelingClient.exceptions usage example

async with session.create_client("iotsecuretunneling") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.LimitExceededException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# IoTSecureTunnelingClient usage type checking example

from types_aiobotocore_iotsecuretunneling.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### close\_tunnel

Closes a tunnel identified by the unique tunnel id.

Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").close_tunnel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling/client/close_tunnel.html)

```python
# close_tunnel method definition

await def close_tunnel(
    self,
    *,
    tunnelId: str,
    delete: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# close_tunnel method usage example with argument unpacking

kwargs: CloseTunnelRequestTypeDef = {  # (1)
    "tunnelId": ...,
}

parent.close_tunnel(**kwargs)
```

1. See [:material-code-braces: CloseTunnelRequestTypeDef](./type_defs.md#closetunnelrequesttypedef) 

### describe\_tunnel

Gets information about a tunnel identified by the unique tunnel id.

Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").describe_tunnel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling/client/describe_tunnel.html)

```python
# describe_tunnel method definition

await def describe_tunnel(
    self,
    *,
    tunnelId: str,
) -> DescribeTunnelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTunnelResponseTypeDef](./type_defs.md#describetunnelresponsetypedef) 


```python
# describe_tunnel method usage example with argument unpacking

kwargs: DescribeTunnelRequestTypeDef = {  # (1)
    "tunnelId": ...,
}

parent.describe_tunnel(**kwargs)
```

1. See [:material-code-braces: DescribeTunnelRequestTypeDef](./type_defs.md#describetunnelrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### list\_tunnels

List all tunnels for an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").list_tunnels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling/client/list_tunnels.html)

```python
# list_tunnels method definition

await def list_tunnels(
    self,
    *,
    thingName: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListTunnelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTunnelsResponseTypeDef](./type_defs.md#listtunnelsresponsetypedef) 


```python
# list_tunnels method usage example with argument unpacking

kwargs: ListTunnelsRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.list_tunnels(**kwargs)
```

1. See [:material-code-braces: ListTunnelsRequestTypeDef](./type_defs.md#listtunnelsrequesttypedef) 

### open\_tunnel

Creates a new tunnel, and returns two client access tokens for clients to use
to connect to the IoT Secure Tunneling proxy server.

Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").open_tunnel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling/client/open_tunnel.html)

```python
# open_tunnel method definition

await def open_tunnel(
    self,
    *,
    description: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (1)
    destinationConfig: DestinationConfigUnionTypeDef = ...,  # (2)
    timeoutConfig: TimeoutConfigTypeDef = ...,  # (3)
) -> OpenTunnelResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) [:material-code-braces: DestinationConfigOutputTypeDef](./type_defs.md#destinationconfigoutputtypedef) 
3. See [:material-code-braces: TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef) 
4. See [:material-code-braces: OpenTunnelResponseTypeDef](./type_defs.md#opentunnelresponsetypedef) 


```python
# open_tunnel method usage example with argument unpacking

kwargs: OpenTunnelRequestTypeDef = {  # (1)
    "description": ...,
}

parent.open_tunnel(**kwargs)
```

1. See [:material-code-braces: OpenTunnelRequestTypeDef](./type_defs.md#opentunnelrequesttypedef) 

### rotate\_tunnel\_access\_token

Revokes the current client access token (CAT) and returns new CAT for clients
to use when reconnecting to secure tunneling to access the same tunnel.

Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").rotate_tunnel_access_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling/client/rotate_tunnel_access_token.html)

```python
# rotate_tunnel_access_token method definition

await def rotate_tunnel_access_token(
    self,
    *,
    tunnelId: str,
    clientMode: ClientModeType,  # (1)
    destinationConfig: DestinationConfigUnionTypeDef = ...,  # (2)
) -> RotateTunnelAccessTokenResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ClientModeType](./literals.md#clientmodetype) 
2. See [:material-code-braces: DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef) [:material-code-braces: DestinationConfigOutputTypeDef](./type_defs.md#destinationconfigoutputtypedef) 
3. See [:material-code-braces: RotateTunnelAccessTokenResponseTypeDef](./type_defs.md#rotatetunnelaccesstokenresponsetypedef) 


```python
# rotate_tunnel_access_token method usage example with argument unpacking

kwargs: RotateTunnelAccessTokenRequestTypeDef = {  # (1)
    "tunnelId": ...,
    "clientMode": ...,
}

parent.rotate_tunnel_access_token(**kwargs)
```

1. See [:material-code-braces: RotateTunnelAccessTokenRequestTypeDef](./type_defs.md#rotatetunnelaccesstokenrequesttypedef) 

### tag\_resource

A resource tag.

Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes a tag from a resource.

Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iotsecuretunneling").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```





