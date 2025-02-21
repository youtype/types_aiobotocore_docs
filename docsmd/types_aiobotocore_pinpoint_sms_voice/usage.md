# Examples

> [Index](../README.md) > [PinpointSMSVoice](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PinpointSMSVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#pinpointsmsvoice)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[pinpoint-sms-voice]` package installed.

Write your `PinpointSMSVoice` code as usual,
type checking and code completion should work out of the box.



```python
# PinpointSMSVoiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pinpoint-sms-voice") as client:  # (1)
    result = await client.get_configuration_set_event_destinations()  # (2)
```

1. client: [PinpointSMSVoiceClient](./client.md)
2. result: [:material-code-braces: GetConfigurationSetEventDestinationsResponseTypeDef](./type_defs.md#getconfigurationseteventdestinationsresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[pinpoint-sms-voice]`
or a standalone `types_aiobotocore_pinpoint_sms_voice` package, you have to explicitly specify
`client: PinpointSMSVoiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PinpointSMSVoiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice.client import PinpointSMSVoiceClient
from types_aiobotocore_pinpoint_sms_voice.type_defs import GetConfigurationSetEventDestinationsResponseTypeDef
from types_aiobotocore_pinpoint_sms_voice.type_defs import GetConfigurationSetEventDestinationsRequestTypeDef


session = get_session()

async with session.create_client("pinpoint-sms-voice") as client:
    client: PinpointSMSVoiceClient
    kwargs: GetConfigurationSetEventDestinationsRequestTypeDef = {...}
    result: GetConfigurationSetEventDestinationsResponseTypeDef = await client.get_configuration_set_event_destinations(**kwargs)
```




