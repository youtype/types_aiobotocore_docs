# Examples

> [Index](../README.md) > [SMSVoice](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SMSVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#smsvoice)
    type annotations stubs module [types-aiobotocore-sms-voice](https://pypi.org/project/types-aiobotocore-sms-voice/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sms-voice]` package installed.

Write your `SMSVoice` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SMSVoiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sms-voice") as client:  # (1)
    result = await client.get_configuration_set_event_destinations()  # (2)
```

1. client: [SMSVoiceClient](./client.md)
2. result: [:material-code-braces: GetConfigurationSetEventDestinationsResponseTypeDef](./type_defs.md#getconfigurationseteventdestinationsresponsetypedef)






### Explicit type annotations

With `types-aiobotocore-lite[sms-voice]`
or a standalone `types_aiobotocore_sms_voice` package, you have to explicitly specify
`client: SMSVoiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SMSVoiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sms_voice.client import SMSVoiceClient
from types_aiobotocore_sms_voice.type_defs import GetConfigurationSetEventDestinationsResponseTypeDef
from types_aiobotocore_sms_voice.type_defs import GetConfigurationSetEventDestinationsRequestTypeDef


session = get_session()

async with session.create_client("sms-voice") as client:
    client: SMSVoiceClient
    kwargs: GetConfigurationSetEventDestinationsRequestTypeDef = {...}
    result: GetConfigurationSetEventDestinationsResponseTypeDef = await client.get_configuration_set_event_destinations(**kwargs)
```




