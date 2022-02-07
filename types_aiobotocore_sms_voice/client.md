<a id="pinpointsmsvoiceclient-for-aiobotocore-pinpointsmsvoice-module"></a>

# PinpointSMSVoiceClient for aiobotocore PinpointSMSVoice module

> [Index](..) > [PinpointSMSVoice](.) > PinpointSMSVoiceClient

Auto-generated documentation for
[PinpointSMSVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice)
type annotations stubs module
[types-aiobotocore-sms-voice](https://pypi.org/project/types-aiobotocore-sms-voice/).

- [PinpointSMSVoiceClient for aiobotocore PinpointSMSVoice module](#pinpointsmsvoiceclient-for-aiobotocore-pinpointsmsvoice-module)
  - [PinpointSMSVoiceClient](#pinpointsmsvoiceclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_configuration_set](#create_configuration_set)
    - [create_configuration_set_event_destination](#create_configuration_set_event_destination)
    - [delete_configuration_set](#delete_configuration_set)
    - [delete_configuration_set_event_destination](#delete_configuration_set_event_destination)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_configuration_set_event_destinations](#get_configuration_set_event_destinations)
    - [list_configuration_sets](#list_configuration_sets)
    - [send_voice_message](#send_voice_message)
    - [update_configuration_set_event_destination](#update_configuration_set_event_destination)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="pinpointsmsvoiceclient"></a>

## PinpointSMSVoiceClient

Type annotations for `session.create_client("sms-voice")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_sms_voice.client import PinpointSMSVoiceClient

session = get_session()
async with session.create_client("sms-voice") as client:
    client: PinpointSMSVoiceClient
```

Boto3 documentation:
[PinpointSMSVoice.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_sms_voice.client import Exceptions

def handle_error(exc: Exceptions.AlreadyExistsException) -> None:
    ...
```

Exceptions:

- `Exceptions.AlreadyExistsException`
- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.InternalServiceErrorException`
- `Exceptions.LimitExceededException`
- `Exceptions.NotFoundException`
- `Exceptions.TooManyRequestsException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

PinpointSMSVoiceClient exceptions.

Type annotations for `session.create_client("sms-voice").exceptions` method.

Boto3 documentation:
[PinpointSMSVoice.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("sms-voice").can_paginate` method.

Boto3 documentation:
[PinpointSMSVoice.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_configuration_set"></a>

### create_configuration_set

Create a new configuration set.

Type annotations for
`session.create_client("sms-voice").create_configuration_set` method.

Boto3 documentation:
[PinpointSMSVoice.Client.create_configuration_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.create_configuration_set)

Asynchronous method. Use `await create_configuration_set(...)` for a
synchronous call.

Arguments mapping described in
[CreateConfigurationSetRequestRequestTypeDef](./type_defs.md#createconfigurationsetrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationSetName`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create_configuration_set_event_destination"></a>

### create_configuration_set_event_destination

Create a new event destination in a configuration set.

Type annotations for
`session.create_client("sms-voice").create_configuration_set_event_destination`
method.

Boto3 documentation:
[PinpointSMSVoice.Client.create_configuration_set_event_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.create_configuration_set_event_destination)

Asynchronous method. Use
`await create_configuration_set_event_destination(...)` for a synchronous call.

Arguments mapping described in
[CreateConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#createconfigurationseteventdestinationrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationSetName`: `str` *(required)*
- `EventDestination`:
  [EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef)
- `EventDestinationName`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_configuration_set"></a>

### delete_configuration_set

Deletes an existing configuration set.

Type annotations for
`session.create_client("sms-voice").delete_configuration_set` method.

Boto3 documentation:
[PinpointSMSVoice.Client.delete_configuration_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.delete_configuration_set)

Asynchronous method. Use `await delete_configuration_set(...)` for a
synchronous call.

Arguments mapping described in
[DeleteConfigurationSetRequestRequestTypeDef](./type_defs.md#deleteconfigurationsetrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationSetName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_configuration_set_event_destination"></a>

### delete_configuration_set_event_destination

Deletes an event destination in a configuration set.

Type annotations for
`session.create_client("sms-voice").delete_configuration_set_event_destination`
method.

Boto3 documentation:
[PinpointSMSVoice.Client.delete_configuration_set_event_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.delete_configuration_set_event_destination)

Asynchronous method. Use
`await delete_configuration_set_event_destination(...)` for a synchronous call.

Arguments mapping described in
[DeleteConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#deleteconfigurationseteventdestinationrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationSetName`: `str` *(required)*
- `EventDestinationName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("sms-voice").generate_presigned_url` method.

Boto3 documentation:
[PinpointSMSVoice.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_configuration_set_event_destinations"></a>

### get_configuration_set_event_destinations

Obtain information about an event destination, including the types of events it
reports, the Amazon Resource Name (ARN) of the destination, and the name of the
event destination.

Type annotations for
`session.create_client("sms-voice").get_configuration_set_event_destinations`
method.

Boto3 documentation:
[PinpointSMSVoice.Client.get_configuration_set_event_destinations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.get_configuration_set_event_destinations)

Asynchronous method. Use `await get_configuration_set_event_destinations(...)`
for a synchronous call.

Arguments mapping described in
[GetConfigurationSetEventDestinationsRequestRequestTypeDef](./type_defs.md#getconfigurationseteventdestinationsrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationSetName`: `str` *(required)*

Returns a `Coroutine` for
[GetConfigurationSetEventDestinationsResponseTypeDef](./type_defs.md#getconfigurationseteventdestinationsresponsetypedef).

<a id="list_configuration_sets"></a>

### list_configuration_sets

List all of the configuration sets associated with your Amazon Pinpoint account
in the current region.

Type annotations for
`session.create_client("sms-voice").list_configuration_sets` method.

Boto3 documentation:
[PinpointSMSVoice.Client.list_configuration_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.list_configuration_sets)

Asynchronous method. Use `await list_configuration_sets(...)` for a synchronous
call.

Arguments mapping described in
[ListConfigurationSetsRequestRequestTypeDef](./type_defs.md#listconfigurationsetsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `PageSize`: `str`

Returns a `Coroutine` for
[ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef).

<a id="send_voice_message"></a>

### send_voice_message

Create a new voice message and send it to a recipient's phone number.

Type annotations for `session.create_client("sms-voice").send_voice_message`
method.

Boto3 documentation:
[PinpointSMSVoice.Client.send_voice_message](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.send_voice_message)

Asynchronous method. Use `await send_voice_message(...)` for a synchronous
call.

Arguments mapping described in
[SendVoiceMessageRequestRequestTypeDef](./type_defs.md#sendvoicemessagerequestrequesttypedef).

Keyword-only arguments:

- `CallerId`: `str`
- `ConfigurationSetName`: `str`
- `Content`:
  [VoiceMessageContentTypeDef](./type_defs.md#voicemessagecontenttypedef)
- `DestinationPhoneNumber`: `str`
- `OriginationPhoneNumber`: `str`

Returns a `Coroutine` for
[SendVoiceMessageResponseTypeDef](./type_defs.md#sendvoicemessageresponsetypedef).

<a id="update_configuration_set_event_destination"></a>

### update_configuration_set_event_destination

Update an event destination in a configuration set.

Type annotations for
`session.create_client("sms-voice").update_configuration_set_event_destination`
method.

Boto3 documentation:
[PinpointSMSVoice.Client.update_configuration_set_event_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.update_configuration_set_event_destination)

Asynchronous method. Use
`await update_configuration_set_event_destination(...)` for a synchronous call.

Arguments mapping described in
[UpdateConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#updateconfigurationseteventdestinationrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationSetName`: `str` *(required)*
- `EventDestinationName`: `str` *(required)*
- `EventDestination`:
  [EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("sms-voice").__aenter__` method.

Boto3 documentation:
[PinpointSMSVoice.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [PinpointSMSVoiceClient](#pinpointsmsvoiceclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("sms-voice").__aexit__` method.

Boto3 documentation:
[PinpointSMSVoice.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
