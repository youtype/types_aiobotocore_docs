# KinesisVideoWebRTCStorageClient

> [Index](../README.md) > [KinesisVideoWebRTCStorage](./README.md) > KinesisVideoWebRTCStorageClient

!!! note ""

    Auto-generated documentation for [KinesisVideoWebRTCStorage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
    type annotations stubs module [types-aiobotocore-kinesis-video-webrtc-storage](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage/).

## KinesisVideoWebRTCStorageClient

Type annotations and code completion for `#!python session.create_client("kinesis-video-webrtc-storage")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client)

```python
KinesisVideoWebRTCStorageClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_kinesis_video_webrtc_storage.client import KinesisVideoWebRTCStorageClient

session = get_session()
async with session.create_client("kinesis-video-webrtc-storage") as client:
    client: KinesisVideoWebRTCStorageClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("kinesis-video-webrtc-storage").exceptions` structure.

```python
KinesisVideoWebRTCStorageClient.exceptions usage example

async with session.create_client("kinesis-video-webrtc-storage") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ClientLimitExceededException,
        client.InvalidArgumentException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
KinesisVideoWebRTCStorageClient usage type checking example

from types_aiobotocore_kinesis_video_webrtc_storage.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("kinesis-video-webrtc-storage").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("kinesis-video-webrtc-storage").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("kinesis-video-webrtc-storage").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client.generate_presigned_url)

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


### join\_storage\_session

Join the ongoing one way-video and/or multi-way audio WebRTC session as a video
producing device for an input channel.

Type annotations and code completion for `#!python session.create_client("kinesis-video-webrtc-storage").join_storage_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client.join_storage_session)

```python
# join_storage_session method definition

await def join_storage_session(
    self,
    *,
    channelArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# join_storage_session method usage example with argument unpacking

kwargs: JoinStorageSessionInputRequestTypeDef = {  # (1)
    "channelArn": ...,
}

parent.join_storage_session(**kwargs)
```

1. See [:material-code-braces: JoinStorageSessionInputRequestTypeDef](./type_defs.md#joinstoragesessioninputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("kinesis-video-webrtc-storage").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> KinesisVideoWebRTCStorageClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("kinesis-video-webrtc-storage").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





