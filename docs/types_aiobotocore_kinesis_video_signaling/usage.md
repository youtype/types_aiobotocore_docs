<a id="examples-for-aiobotocore-kinesisvideosignalingchannels-module"></a>

# Examples for aiobotocore KinesisVideoSignalingChannels module

> [Index](../README.md) > [KinesisVideoSignalingChannels](./README.md) >
> Examples

- [Examples for aiobotocore KinesisVideoSignalingChannels module](#examples-for-aiobotocore-kinesisvideosignalingchannels-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[kinesis-video-signaling]` package
installed.

Write your `KinesisVideoSignalingChannels` code as usual, type checking and
code completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type KinesisVideoSignalingChannelsClient
# and provides type checking and code completion
async with session.create_client("kinesis-video-signaling") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[kinesis-video-signaling]` or a standalone
`types_aiobotocore_kinesis_video_signaling` package, you have to explicitly
specify `client: KinesisVideoSignalingChannelsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_signaling.client import KinesisVideoSignalingChannelsClient
from types_aiobotocore_kinesis_video_signaling.type_defs import bool






session = get_session()

async with session.create_client("kinesis-video-signaling") as client:
    client: KinesisVideoSignalingChannelsClient

    
    result: bool = client.can_paginate()
    

    

    
```
