<a id="iotdataplaneclient-for-aiobotocore-iotdataplane-module"></a>

# IoTDataPlaneClient for aiobotocore IoTDataPlane module

> [Index](../README.md) > [IoTDataPlane](./README.md) > IoTDataPlaneClient

Auto-generated documentation for
[IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
type annotations stubs module
[types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

- [IoTDataPlaneClient for aiobotocore IoTDataPlane module](#iotdataplaneclient-for-aiobotocore-iotdataplane-module)
  - [IoTDataPlaneClient](#iotdataplaneclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [delete_thing_shadow](#delete_thing_shadow)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_retained_message](#get_retained_message)
    - [get_thing_shadow](#get_thing_shadow)
    - [list_named_shadows_for_thing](#list_named_shadows_for_thing)
    - [list_retained_messages](#list_retained_messages)
    - [publish](#publish)
    - [update_thing_shadow](#update_thing_shadow)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="iotdataplaneclient"></a>

## IoTDataPlaneClient

Type annotations for `session.create_client("iot-data")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_iot_data.client import IoTDataPlaneClient

session = get_session()
async with session.create_client("iot-data") as client:
    client: IoTDataPlaneClient
```

Boto3 documentation:
[IoTDataPlane.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_iot_data.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalFailureException`
- `Exceptions.InvalidRequestException`
- `Exceptions.MethodNotAllowedException`
- `Exceptions.RequestEntityTooLargeException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.ThrottlingException`
- `Exceptions.UnauthorizedException`
- `Exceptions.UnsupportedDocumentEncodingException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

IoTDataPlaneClient exceptions.

Type annotations for `session.create_client("iot-data").exceptions` method.

Boto3 documentation:
[IoTDataPlane.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("iot-data").can_paginate` method.

Boto3 documentation:
[IoTDataPlane.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="delete\_thing\_shadow"></a>

### delete_thing_shadow

Deletes the shadow for the specified thing.

Type annotations for `session.create_client("iot-data").delete_thing_shadow`
method.

Boto3 documentation:
[IoTDataPlane.Client.delete_thing_shadow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.delete_thing_shadow)

Asynchronous method. Use `await delete_thing_shadow(...)` for a synchronous
call.

Arguments mapping described in
[DeleteThingShadowRequestRequestTypeDef](./type_defs.md#deletethingshadowrequestrequesttypedef).

Keyword-only arguments:

- `thingName`: `str` *(required)*
- `shadowName`: `str`

Returns a `Coroutine` for
[DeleteThingShadowResponseTypeDef](./type_defs.md#deletethingshadowresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("iot-data").generate_presigned_url`
method.

Boto3 documentation:
[IoTDataPlane.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_retained\_message"></a>

### get_retained_message

Gets the details of a single retained message for the specified topic.

Type annotations for `session.create_client("iot-data").get_retained_message`
method.

Boto3 documentation:
[IoTDataPlane.Client.get_retained_message](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.get_retained_message)

Asynchronous method. Use `await get_retained_message(...)` for a synchronous
call.

Arguments mapping described in
[GetRetainedMessageRequestRequestTypeDef](./type_defs.md#getretainedmessagerequestrequesttypedef).

Keyword-only arguments:

- `topic`: `str` *(required)*

Returns a `Coroutine` for
[GetRetainedMessageResponseTypeDef](./type_defs.md#getretainedmessageresponsetypedef).

<a id="get\_thing\_shadow"></a>

### get_thing_shadow

Gets the shadow for the specified thing.

Type annotations for `session.create_client("iot-data").get_thing_shadow`
method.

Boto3 documentation:
[IoTDataPlane.Client.get_thing_shadow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.get_thing_shadow)

Asynchronous method. Use `await get_thing_shadow(...)` for a synchronous call.

Arguments mapping described in
[GetThingShadowRequestRequestTypeDef](./type_defs.md#getthingshadowrequestrequesttypedef).

Keyword-only arguments:

- `thingName`: `str` *(required)*
- `shadowName`: `str`

Returns a `Coroutine` for
[GetThingShadowResponseTypeDef](./type_defs.md#getthingshadowresponsetypedef).

<a id="list\_named\_shadows\_for\_thing"></a>

### list_named_shadows_for_thing

Lists the shadows for the specified thing.

Type annotations for
`session.create_client("iot-data").list_named_shadows_for_thing` method.

Boto3 documentation:
[IoTDataPlane.Client.list_named_shadows_for_thing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.list_named_shadows_for_thing)

Asynchronous method. Use `await list_named_shadows_for_thing(...)` for a
synchronous call.

Arguments mapping described in
[ListNamedShadowsForThingRequestRequestTypeDef](./type_defs.md#listnamedshadowsforthingrequestrequesttypedef).

Keyword-only arguments:

- `thingName`: `str` *(required)*
- `nextToken`: `str`
- `pageSize`: `int`

Returns a `Coroutine` for
[ListNamedShadowsForThingResponseTypeDef](./type_defs.md#listnamedshadowsforthingresponsetypedef).

<a id="list\_retained\_messages"></a>

### list_retained_messages

Lists summary information about the retained messages stored for the account.

Type annotations for `session.create_client("iot-data").list_retained_messages`
method.

Boto3 documentation:
[IoTDataPlane.Client.list_retained_messages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.list_retained_messages)

Asynchronous method. Use `await list_retained_messages(...)` for a synchronous
call.

Arguments mapping described in
[ListRetainedMessagesRequestRequestTypeDef](./type_defs.md#listretainedmessagesrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef).

<a id="publish"></a>

### publish

Publishes an MQTT message.

Type annotations for `session.create_client("iot-data").publish` method.

Boto3 documentation:
[IoTDataPlane.Client.publish](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.publish)

Asynchronous method. Use `await publish(...)` for a synchronous call.

Arguments mapping described in
[PublishRequestRequestTypeDef](./type_defs.md#publishrequestrequesttypedef).

Keyword-only arguments:

- `topic`: `str` *(required)*
- `qos`: `int`
- `retain`: `bool`
- `payload`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]

<a id="update\_thing\_shadow"></a>

### update_thing_shadow

Updates the shadow for the specified thing.

Type annotations for `session.create_client("iot-data").update_thing_shadow`
method.

Boto3 documentation:
[IoTDataPlane.Client.update_thing_shadow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.update_thing_shadow)

Asynchronous method. Use `await update_thing_shadow(...)` for a synchronous
call.

Arguments mapping described in
[UpdateThingShadowRequestRequestTypeDef](./type_defs.md#updatethingshadowrequestrequesttypedef).

Keyword-only arguments:

- `thingName`: `str` *(required)*
- `payload`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\] *(required)*
- `shadowName`: `str`

Returns a `Coroutine` for
[UpdateThingShadowResponseTypeDef](./type_defs.md#updatethingshadowresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("iot-data").__aenter__` method.

Boto3 documentation:
[IoTDataPlane.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [IoTDataPlaneClient](#iotdataplaneclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("iot-data").__aexit__` method.

Boto3 documentation:
[IoTDataPlane.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("iot-data").get_paginator` method
with overloads.

- `client.get_paginator("list_retained_messages")` ->
  [ListRetainedMessagesPaginator](./paginators.md#listretainedmessagespaginator)
