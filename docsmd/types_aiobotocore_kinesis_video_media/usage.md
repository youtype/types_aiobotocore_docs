# Examples

> [Index](../README.md) > [KinesisVideoMedia](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisVideoMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#kinesisvideomedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-media](https://pypi.org/project/types-aiobotocore-kinesis-video-media/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kinesis-video-media]` package installed.

Write your `KinesisVideoMedia` code as usual,
type checking and code completion should work out of the box.



```python
# KinesisVideoMediaClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesis-video-media") as client:  # (1)
    result = await client.get_media()  # (2)
```

1. client: [KinesisVideoMediaClient](./client.md)
2. result: [:material-code-braces: GetMediaOutputTypeDef](./type_defs.md#getmediaoutputtypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[kinesis-video-media]`
or a standalone `types_aiobotocore_kinesis_video_media` package, you have to explicitly specify
`client: KinesisVideoMediaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KinesisVideoMediaClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_media.client import KinesisVideoMediaClient
from types_aiobotocore_kinesis_video_media.type_defs import GetMediaOutputTypeDef
from types_aiobotocore_kinesis_video_media.type_defs import GetMediaInputTypeDef


session = get_session()

async with session.create_client("kinesis-video-media") as client:
    client: KinesisVideoMediaClient
    kwargs: GetMediaInputTypeDef = {...}
    result: GetMediaOutputTypeDef = await client.get_media(**kwargs)
```




