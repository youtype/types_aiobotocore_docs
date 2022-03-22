<a id="examples-for-aiobotocore-chimesdkmeetings-module"></a>

# Examples for aiobotocore ChimeSDKMeetings module

> [Index](../README.md) > [ChimeSDKMeetings](./README.md) > Examples

- [Examples for aiobotocore ChimeSDKMeetings module](#examples-for-aiobotocore-chimesdkmeetings-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[chime-sdk-meetings]` package installed.

Write your `ChimeSDKMeetings` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ChimeSDKMeetingsClient
# and provides type checking and code completion
async with session.create_client("chime-sdk-meetings") as client:
    
    # result has type BatchCreateAttendeeResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_create_attendee()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[chime-sdk-meetings]` or a standalone
`types_aiobotocore_chime_sdk_meetings` package, you have to explicitly specify
`client: ChimeSDKMeetingsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_meetings.client import ChimeSDKMeetingsClient
from types_aiobotocore_chime_sdk_meetings.type_defs import BatchCreateAttendeeResponseTypeDef






session = get_session()

async with session.create_client("chime-sdk-meetings") as client:
    client: ChimeSDKMeetingsClient

    
    result: BatchCreateAttendeeResponseTypeDef = client.batch_create_attendee()
    

    

    
```
