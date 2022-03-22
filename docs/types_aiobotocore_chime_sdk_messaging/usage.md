<a id="examples-for-aiobotocore-chimesdkmessaging-module"></a>

# Examples for aiobotocore ChimeSDKMessaging module

> [Index](../README.md) > [ChimeSDKMessaging](./README.md) > Examples

- [Examples for aiobotocore ChimeSDKMessaging module](#examples-for-aiobotocore-chimesdkmessaging-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[chime-sdk-messaging]` package installed.

Write your `ChimeSDKMessaging` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ChimeSDKMessagingClient
# and provides type checking and code completion
async with session.create_client("chime-sdk-messaging") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_channel_flow()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[chime-sdk-messaging]` or a standalone
`types_aiobotocore_chime_sdk_messaging` package, you have to explicitly specify
`client: ChimeSDKMessagingClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_messaging.client import ChimeSDKMessagingClient
from types_aiobotocore_chime_sdk_messaging.type_defs import None






session = get_session()

async with session.create_client("chime-sdk-messaging") as client:
    client: ChimeSDKMessagingClient

    
    result: None = client.associate_channel_flow()
    

    

    
```
