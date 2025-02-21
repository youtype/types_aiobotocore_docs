# Examples

> [Index](../README.md) > [ChimeSDKMediaPipelines](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ChimeSDKMediaPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#chimesdkmediapipelines)
    type annotations stubs module [types-aiobotocore-chime-sdk-media-pipelines](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[chime-sdk-media-pipelines]` package installed.

Write your `ChimeSDKMediaPipelines` code as usual,
type checking and code completion should work out of the box.



```python
# ChimeSDKMediaPipelinesClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("chime-sdk-media-pipelines") as client:  # (1)
    result = await client.create_media_capture_pipeline()  # (2)
```

1. client: [ChimeSDKMediaPipelinesClient](./client.md)
2. result: [:material-code-braces: CreateMediaCapturePipelineResponseTypeDef](./type_defs.md#createmediacapturepipelineresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[chime-sdk-media-pipelines]`
or a standalone `types_aiobotocore_chime_sdk_media_pipelines` package, you have to explicitly specify
`client: ChimeSDKMediaPipelinesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ChimeSDKMediaPipelinesClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient
from types_aiobotocore_chime_sdk_media_pipelines.type_defs import CreateMediaCapturePipelineResponseTypeDef
from types_aiobotocore_chime_sdk_media_pipelines.type_defs import CreateMediaCapturePipelineRequestTypeDef


session = get_session()

async with session.create_client("chime-sdk-media-pipelines") as client:
    client: ChimeSDKMediaPipelinesClient
    kwargs: CreateMediaCapturePipelineRequestTypeDef = {...}
    result: CreateMediaCapturePipelineResponseTypeDef = await client.create_media_capture_pipeline(**kwargs)
```




