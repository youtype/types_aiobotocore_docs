<a id="examples-for-aiobotocore-voiceid-module"></a>

# Examples for aiobotocore VoiceID module

> [Index](../README.md) > [VoiceID](./README.md) > Examples

- [Examples for aiobotocore VoiceID module](#examples-for-aiobotocore-voiceid-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[voice-id]` package installed.

Write your `VoiceID` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type VoiceIDClient
# and provides type checking and code completion
async with session.create_client("voice-id") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[voice-id]` or a standalone
`types_aiobotocore_voice_id` package, you have to explicitly specify
`client: VoiceIDClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_voice_id.client import VoiceIDClient
from types_aiobotocore_voice_id.type_defs import bool






session = get_session()

async with session.create_client("voice-id") as client:
    client: VoiceIDClient

    
    result: bool = client.can_paginate()
    

    

    
```
