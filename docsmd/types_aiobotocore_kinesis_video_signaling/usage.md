# Examples

> [Index](../README.md) > [KinesisVideoSignalingChannels](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisVideoSignalingChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#kinesisvideosignalingchannels)
    type annotations stubs module [types-aiobotocore-kinesis-video-signaling](https://pypi.org/project/types-aiobotocore-kinesis-video-signaling/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kinesis-video-signaling]` package installed.

Write your `KinesisVideoSignalingChannels` code as usual,
type checking and code completion should work out of the box.



```python
# KinesisVideoSignalingChannelsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesis-video-signaling") as client:  # (1)
    result = await client.get_ice_server_config()  # (2)
```

1. client: [KinesisVideoSignalingChannelsClient](./client.md)
2. result: [:material-code-braces: GetIceServerConfigResponseTypeDef](./type_defs.md#geticeserverconfigresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[kinesis-video-signaling]`
or a standalone `types_aiobotocore_kinesis_video_signaling` package, you have to explicitly specify
`client: KinesisVideoSignalingChannelsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KinesisVideoSignalingChannelsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_signaling.client import KinesisVideoSignalingChannelsClient
from types_aiobotocore_kinesis_video_signaling.type_defs import GetIceServerConfigResponseTypeDef
from types_aiobotocore_kinesis_video_signaling.type_defs import GetIceServerConfigRequestTypeDef


session = get_session()

async with session.create_client("kinesis-video-signaling") as client:
    client: KinesisVideoSignalingChannelsClient
    kwargs: GetIceServerConfigRequestTypeDef = {...}
    result: GetIceServerConfigResponseTypeDef = await client.get_ice_server_config(**kwargs)
```




