# KinesisVideoMediaClient

> [Index](../README.md) > [KinesisVideoMedia](./README.md) > KinesisVideoMediaClient

!!! note ""

    Auto-generated documentation for [KinesisVideoMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#kinesisvideomedia)
    type annotations stubs module [types-aiobotocore-kinesis-video-media](https://pypi.org/project/types-aiobotocore-kinesis-video-media/).

## KinesisVideoMediaClient

Type annotations and code completion for `#!python session.create_client("kinesis-video-media")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

```python
# KinesisVideoMediaClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_kinesis_video_media.client import KinesisVideoMediaClient

session = get_session()
async with session.create_client("kinesis-video-media") as client:
    client: KinesisVideoMediaClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("kinesis-video-media").exceptions` structure.

```python
# KinesisVideoMediaClient.exceptions usage example

async with session.create_client("kinesis-video-media") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ClientLimitExceededException,
        client.ConnectionLimitExceededException,
        client.InvalidArgumentException,
        client.InvalidEndpointException,
        client.NotAuthorizedException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
# KinesisVideoMediaClient usage type checking example

from types_aiobotocore_kinesis_video_media.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("kinesis-video-media").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("kinesis-video-media").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_media

Use this API to retrieve media content from a Kinesis video stream.

Type annotations and code completion for `#!python session.create_client("kinesis-video-media").get_media` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media/client/get_media.html)

```python
# get_media method definition

await def get_media(
    self,
    *,
    StartSelector: StartSelectorTypeDef,  # (1)
    StreamName: str = ...,
    StreamARN: str = ...,
) -> GetMediaOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartSelectorTypeDef](./type_defs.md#startselectortypedef) 
2. See [:material-code-braces: GetMediaOutputTypeDef](./type_defs.md#getmediaoutputtypedef) 


```python
# get_media method usage example with argument unpacking

kwargs: GetMediaInputTypeDef = {  # (1)
    "StartSelector": ...,
}

parent.get_media(**kwargs)
```

1. See [:material-code-braces: GetMediaInputTypeDef](./type_defs.md#getmediainputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("kinesis-video-media").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("kinesis-video-media").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```





