<a id="examples-for-aiobotocore-pinpointsmsvoice-module"></a>

# Examples for aiobotocore PinpointSMSVoice module

> [Index](../README.md) > [PinpointSMSVoice](./README.md) > Examples

- [Examples for aiobotocore PinpointSMSVoice module](#examples-for-aiobotocore-pinpointsmsvoice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sms-voice]` package installed.

Write your `PinpointSMSVoice` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type PinpointSMSVoiceClient
# and provides type checking and code completion
async with session.create_client("sms-voice") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sms-voice]` or a standalone
`types_aiobotocore_sms_voice` package, you have to explicitly specify
`client: PinpointSMSVoiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sms_voice.client import PinpointSMSVoiceClient
from types_aiobotocore_sms_voice.type_defs import bool






session = get_session()

async with session.create_client("sms-voice") as client:
    client: PinpointSMSVoiceClient

    
    result: bool = client.can_paginate()
    

    

    
```
