# PinpointSMSVoiceClient

> [Index](../README.md) > [PinpointSMSVoice](./README.md) > PinpointSMSVoiceClient

!!! note ""

    Auto-generated documentation for [PinpointSMSVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice/).

## PinpointSMSVoiceClient

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_pinpoint_sms_voice.client import PinpointSMSVoiceClient

session = get_session()
async with session.create_client("pinpoint-sms-voice") as client:
    client: PinpointSMSVoiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("pinpoint-sms-voice").exceptions` structure.

```python title="Usage example"
async with session.create_client("pinpoint-sms-voice") as client:
    try:
        do_something(client)
    except (
            client.AlreadyExistsException,
        client.BadRequestException,
        client.ClientError,
        client.InternalServiceErrorException,
        client.LimitExceededException,
        client.NotFoundException,
        client.TooManyRequestsException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_pinpoint_sms_voice.client import Exceptions

def handle_error(exc: Exceptions.AlreadyExistsException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### create\_configuration\_set

Create a new configuration set.

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").create_configuration_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.create_configuration_set)

```python title="Method definition"
await def create_configuration_set(
    self,
    *,
    ConfigurationSetName: str = ...,
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: CreateConfigurationSetRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.create_configuration_set(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationSetRequestRequestTypeDef](./type_defs.md#createconfigurationsetrequestrequesttypedef) 

### create\_configuration\_set\_event\_destination

Create a new event destination in a configuration set.

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").create_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.create_configuration_set_event_destination)

```python title="Method definition"
await def create_configuration_set_event_destination(
    self,
    *,
    ConfigurationSetName: str,
    EventDestination: EventDestinationDefinitionTypeDef = ...,  # (1)
    EventDestinationName: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 


```python title="Usage example with kwargs"
kwargs: CreateConfigurationSetEventDestinationRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.create_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: CreateConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#createconfigurationseteventdestinationrequestrequesttypedef) 

### delete\_configuration\_set

Deletes an existing configuration set.

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").delete_configuration_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.delete_configuration_set)

```python title="Method definition"
await def delete_configuration_set(
    self,
    *,
    ConfigurationSetName: str,
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: DeleteConfigurationSetRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.delete_configuration_set(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationSetRequestRequestTypeDef](./type_defs.md#deleteconfigurationsetrequestrequesttypedef) 

### delete\_configuration\_set\_event\_destination

Deletes an event destination in a configuration set.

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").delete_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.delete_configuration_set_event_destination)

```python title="Method definition"
await def delete_configuration_set_event_destination(
    self,
    *,
    ConfigurationSetName: str,
    EventDestinationName: str,
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: DeleteConfigurationSetEventDestinationRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
    "EventDestinationName": ...,
}

parent.delete_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: DeleteConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#deleteconfigurationseteventdestinationrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.generate_presigned_url)

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


### get\_configuration\_set\_event\_destinations

Obtain information about an event destination, including the types of events it
reports, the Amazon Resource Name (ARN) of the destination, and the name of the
event destination.

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").get_configuration_set_event_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.get_configuration_set_event_destinations)

```python title="Method definition"
await def get_configuration_set_event_destinations(
    self,
    *,
    ConfigurationSetName: str,
) -> GetConfigurationSetEventDestinationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfigurationSetEventDestinationsResponseTypeDef](./type_defs.md#getconfigurationseteventdestinationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetConfigurationSetEventDestinationsRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
}

parent.get_configuration_set_event_destinations(**kwargs)
```

1. See [:material-code-braces: GetConfigurationSetEventDestinationsRequestRequestTypeDef](./type_defs.md#getconfigurationseteventdestinationsrequestrequesttypedef) 

### send\_voice\_message

Create a new voice message and send it to a recipient's phone number.

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").send_voice_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.send_voice_message)

```python title="Method definition"
await def send_voice_message(
    self,
    *,
    CallerId: str = ...,
    ConfigurationSetName: str = ...,
    Content: VoiceMessageContentTypeDef = ...,  # (1)
    DestinationPhoneNumber: str = ...,
    OriginationPhoneNumber: str = ...,
) -> SendVoiceMessageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VoiceMessageContentTypeDef](./type_defs.md#voicemessagecontenttypedef) 
2. See [:material-code-braces: SendVoiceMessageResponseTypeDef](./type_defs.md#sendvoicemessageresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SendVoiceMessageRequestRequestTypeDef = {  # (1)
    "CallerId": ...,
}

parent.send_voice_message(**kwargs)
```

1. See [:material-code-braces: SendVoiceMessageRequestRequestTypeDef](./type_defs.md#sendvoicemessagerequestrequesttypedef) 

### update\_configuration\_set\_event\_destination

Update an event destination in a configuration set.

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").update_configuration_set_event_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.update_configuration_set_event_destination)

```python title="Method definition"
await def update_configuration_set_event_destination(
    self,
    *,
    ConfigurationSetName: str,
    EventDestinationName: str,
    EventDestination: EventDestinationDefinitionTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EventDestinationDefinitionTypeDef](./type_defs.md#eventdestinationdefinitiontypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateConfigurationSetEventDestinationRequestRequestTypeDef = {  # (1)
    "ConfigurationSetName": ...,
    "EventDestinationName": ...,
}

parent.update_configuration_set_event_destination(**kwargs)
```

1. See [:material-code-braces: UpdateConfigurationSetEventDestinationRequestRequestTypeDef](./type_defs.md#updateconfigurationseteventdestinationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> PinpointSMSVoiceClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#PinpointSMSVoice.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





