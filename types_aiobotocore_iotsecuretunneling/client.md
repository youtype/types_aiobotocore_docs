<a id="iotsecuretunnelingclient-for-aiobotocore-iotsecuretunneling-module"></a>

# IoTSecureTunnelingClient for aiobotocore IoTSecureTunneling module

> [Index](..) > [IoTSecureTunneling](.) > IoTSecureTunnelingClient

Auto-generated documentation for
[IoTSecureTunneling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
type annotations stubs module
[types-aiobotocore-iotsecuretunneling](https://pypi.org/project/types-aiobotocore-iotsecuretunneling/).

- [IoTSecureTunnelingClient for aiobotocore IoTSecureTunneling module](#iotsecuretunnelingclient-for-aiobotocore-iotsecuretunneling-module)
  - [IoTSecureTunnelingClient](#iotsecuretunnelingclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [close_tunnel](#close_tunnel)
    - [describe_tunnel](#describe_tunnel)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_tunnels](#list_tunnels)
    - [open_tunnel](#open_tunnel)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)

<a id="iotsecuretunnelingclient"></a>

## IoTSecureTunnelingClient

Type annotations for `aiobotocore.create_client("iotsecuretunneling")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_iotsecuretunneling.client import IoTSecureTunnelingClient

def get_iotsecuretunneling_client() -> IoTSecureTunnelingClient:
    return Session().client("iotsecuretunneling")
```

Boto3 documentation:
[IoTSecureTunneling.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_iotsecuretunneling.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

IoTSecureTunnelingClient exceptions.

Type annotations for
`aiobotocore.create_client("iotsecuretunneling").exceptions` method.

Boto3 documentation:
[IoTSecureTunneling.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`aiobotocore.create_client("iotsecuretunneling").can_paginate` method.

Boto3 documentation:
[IoTSecureTunneling.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="close_tunnel"></a>

### close_tunnel

Closes a tunnel identified by the unique tunnel id.

Type annotations for
`aiobotocore.create_client("iotsecuretunneling").close_tunnel` method.

Boto3 documentation:
[IoTSecureTunneling.Client.close_tunnel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.close_tunnel)

Asynchronous method. Use `await close_tunnel(...)` for a synchronous call.

Arguments mapping described in
[CloseTunnelRequestRequestTypeDef](./type_defs.md#closetunnelrequestrequesttypedef).

Keyword-only arguments:

- `tunnelId`: `str` *(required)*
- `delete`: `bool`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_tunnel"></a>

### describe_tunnel

Gets information about a tunnel identified by the unique tunnel id.

Type annotations for
`aiobotocore.create_client("iotsecuretunneling").describe_tunnel` method.

Boto3 documentation:
[IoTSecureTunneling.Client.describe_tunnel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.describe_tunnel)

Asynchronous method. Use `await describe_tunnel(...)` for a synchronous call.

Arguments mapping described in
[DescribeTunnelRequestRequestTypeDef](./type_defs.md#describetunnelrequestrequesttypedef).

Keyword-only arguments:

- `tunnelId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeTunnelResponseTypeDef](./type_defs.md#describetunnelresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("iotsecuretunneling").generate_presigned_url`
method.

Boto3 documentation:
[IoTSecureTunneling.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Lists the tags for the specified resource.

Type annotations for
`aiobotocore.create_client("iotsecuretunneling").list_tags_for_resource`
method.

Boto3 documentation:
[IoTSecureTunneling.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list_tunnels"></a>

### list_tunnels

List all tunnels for an AWS account.

Type annotations for
`aiobotocore.create_client("iotsecuretunneling").list_tunnels` method.

Boto3 documentation:
[IoTSecureTunneling.Client.list_tunnels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.list_tunnels)

Asynchronous method. Use `await list_tunnels(...)` for a synchronous call.

Arguments mapping described in
[ListTunnelsRequestRequestTypeDef](./type_defs.md#listtunnelsrequestrequesttypedef).

Keyword-only arguments:

- `thingName`: `str`
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListTunnelsResponseTypeDef](./type_defs.md#listtunnelsresponsetypedef).

<a id="open_tunnel"></a>

### open_tunnel

Creates a new tunnel, and returns two client access tokens for clients to use
to connect to the AWS IoT Secure Tunneling proxy server.

Type annotations for
`aiobotocore.create_client("iotsecuretunneling").open_tunnel` method.

Boto3 documentation:
[IoTSecureTunneling.Client.open_tunnel](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.open_tunnel)

Asynchronous method. Use `await open_tunnel(...)` for a synchronous call.

Arguments mapping described in
[OpenTunnelRequestRequestTypeDef](./type_defs.md#opentunnelrequestrequesttypedef).

Keyword-only arguments:

- `description`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `destinationConfig`:
  [DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef)
- `timeoutConfig`: [TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef)

Returns a `Coroutine` for
[OpenTunnelResponseTypeDef](./type_defs.md#opentunnelresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

A resource tag.

Type annotations for
`aiobotocore.create_client("iotsecuretunneling").tag_resource` method.

Boto3 documentation:
[IoTSecureTunneling.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes a tag from a resource.

Type annotations for
`aiobotocore.create_client("iotsecuretunneling").untag_resource` method.

Boto3 documentation:
[IoTSecureTunneling.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].
