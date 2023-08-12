# ChimeSDKMediaPipelinesClient

> [Index](../README.md) > [ChimeSDKMediaPipelines](./README.md) > ChimeSDKMediaPipelinesClient

!!! note ""

    Auto-generated documentation for [ChimeSDKMediaPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines)
    type annotations stubs module [types-aiobotocore-chime-sdk-media-pipelines](https://pypi.org/project/types-aiobotocore-chime-sdk-media-pipelines/).

## ChimeSDKMediaPipelinesClient

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client)

```python
ChimeSDKMediaPipelinesClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_chime_sdk_media_pipelines.client import ChimeSDKMediaPipelinesClient

session = get_session()
async with session.create_client("chime-sdk-media-pipelines") as client:
    client: ChimeSDKMediaPipelinesClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("chime-sdk-media-pipelines").exceptions` structure.

```python
ChimeSDKMediaPipelinesClient.exceptions usage example

async with session.create_client("chime-sdk-media-pipelines") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.ForbiddenException,
        client.NotFoundException,
        client.ResourceLimitExceededException,
        client.ServiceFailureException,
        client.ServiceUnavailableException,
        client.ThrottledClientException,
        client.UnauthorizedClientException,
    ) as e:
        print(e)
```

```python
ChimeSDKMediaPipelinesClient usage type checking example

from types_aiobotocore_chime_sdk_media_pipelines.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_media\_capture\_pipeline

Creates a media pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").create_media_capture_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_capture_pipeline)

```python
# create_media_capture_pipeline method definition

await def create_media_capture_pipeline(
    self,
    *,
    SourceType: MediaPipelineSourceTypeType,  # (1)
    SourceArn: str,
    SinkType: MediaPipelineSinkTypeType,  # (2)
    SinkArn: str,
    ClientRequestToken: str = ...,
    ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateMediaCapturePipelineResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: MediaPipelineSourceTypeType](./literals.md#mediapipelinesourcetypetype) 
2. See [:material-code-brackets: MediaPipelineSinkTypeType](./literals.md#mediapipelinesinktypetype) 
3. See [:material-code-braces: ChimeSdkMeetingConfigurationTypeDef](./type_defs.md#chimesdkmeetingconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateMediaCapturePipelineResponseTypeDef](./type_defs.md#createmediacapturepipelineresponsetypedef) 


```python
# create_media_capture_pipeline method usage example with argument unpacking

kwargs: CreateMediaCapturePipelineRequestRequestTypeDef = {  # (1)
    "SourceType": ...,
    "SourceArn": ...,
    "SinkType": ...,
    "SinkArn": ...,
}

parent.create_media_capture_pipeline(**kwargs)
```

1. See [:material-code-braces: CreateMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#createmediacapturepipelinerequestrequesttypedef) 

### create\_media\_concatenation\_pipeline

Creates a media concatenation pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").create_media_concatenation_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_concatenation_pipeline)

```python
# create_media_concatenation_pipeline method definition

await def create_media_concatenation_pipeline(
    self,
    *,
    Sources: Sequence[ConcatenationSourceTypeDef],  # (1)
    Sinks: Sequence[ConcatenationSinkTypeDef],  # (2)
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateMediaConcatenationPipelineResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ConcatenationSourceTypeDef](./type_defs.md#concatenationsourcetypedef) 
2. See [:material-code-braces: ConcatenationSinkTypeDef](./type_defs.md#concatenationsinktypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateMediaConcatenationPipelineResponseTypeDef](./type_defs.md#createmediaconcatenationpipelineresponsetypedef) 


```python
# create_media_concatenation_pipeline method usage example with argument unpacking

kwargs: CreateMediaConcatenationPipelineRequestRequestTypeDef = {  # (1)
    "Sources": ...,
    "Sinks": ...,
}

parent.create_media_concatenation_pipeline(**kwargs)
```

1. See [:material-code-braces: CreateMediaConcatenationPipelineRequestRequestTypeDef](./type_defs.md#createmediaconcatenationpipelinerequestrequesttypedef) 

### create\_media\_insights\_pipeline

Creates a media insights pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").create_media_insights_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline)

```python
# create_media_insights_pipeline method definition

await def create_media_insights_pipeline(
    self,
    *,
    MediaInsightsPipelineConfigurationArn: str,
    KinesisVideoStreamSourceRuntimeConfiguration: KinesisVideoStreamSourceRuntimeConfigurationTypeDef = ...,  # (1)
    MediaInsightsRuntimeMetadata: Mapping[str, str] = ...,
    KinesisVideoStreamRecordingSourceRuntimeConfiguration: KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef = ...,  # (2)
    S3RecordingSinkRuntimeConfiguration: S3RecordingSinkRuntimeConfigurationTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    ClientRequestToken: str = ...,
) -> CreateMediaInsightsPipelineResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: KinesisVideoStreamSourceRuntimeConfigurationTypeDef](./type_defs.md#kinesisvideostreamsourceruntimeconfigurationtypedef) 
2. See [:material-code-braces: KinesisVideoStreamRecordingSourceRuntimeConfigurationTypeDef](./type_defs.md#kinesisvideostreamrecordingsourceruntimeconfigurationtypedef) 
3. See [:material-code-braces: S3RecordingSinkRuntimeConfigurationTypeDef](./type_defs.md#s3recordingsinkruntimeconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateMediaInsightsPipelineResponseTypeDef](./type_defs.md#createmediainsightspipelineresponsetypedef) 


```python
# create_media_insights_pipeline method usage example with argument unpacking

kwargs: CreateMediaInsightsPipelineRequestRequestTypeDef = {  # (1)
    "MediaInsightsPipelineConfigurationArn": ...,
}

parent.create_media_insights_pipeline(**kwargs)
```

1. See [:material-code-braces: CreateMediaInsightsPipelineRequestRequestTypeDef](./type_defs.md#createmediainsightspipelinerequestrequesttypedef) 

### create\_media\_insights\_pipeline\_configuration

A structure that contains the static configurations for a media insights
pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").create_media_insights_pipeline_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_insights_pipeline_configuration)

```python
# create_media_insights_pipeline_configuration method definition

await def create_media_insights_pipeline_configuration(
    self,
    *,
    MediaInsightsPipelineConfigurationName: str,
    ResourceAccessRoleArn: str,
    Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],  # (1)
    RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    ClientRequestToken: str = ...,
) -> CreateMediaInsightsPipelineConfigurationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: MediaInsightsPipelineConfigurationElementTypeDef](./type_defs.md#mediainsightspipelineconfigurationelementtypedef) 
2. See [:material-code-braces: RealTimeAlertConfigurationTypeDef](./type_defs.md#realtimealertconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateMediaInsightsPipelineConfigurationResponseTypeDef](./type_defs.md#createmediainsightspipelineconfigurationresponsetypedef) 


```python
# create_media_insights_pipeline_configuration method usage example with argument unpacking

kwargs: CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef = {  # (1)
    "MediaInsightsPipelineConfigurationName": ...,
    "ResourceAccessRoleArn": ...,
    "Elements": ...,
}

parent.create_media_insights_pipeline_configuration(**kwargs)
```

1. See [:material-code-braces: CreateMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#createmediainsightspipelineconfigurationrequestrequesttypedef) 

### create\_media\_live\_connector\_pipeline

Creates a media live connector pipeline in an Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").create_media_live_connector_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.create_media_live_connector_pipeline)

```python
# create_media_live_connector_pipeline method definition

await def create_media_live_connector_pipeline(
    self,
    *,
    Sources: Sequence[LiveConnectorSourceConfigurationTypeDef],  # (1)
    Sinks: Sequence[LiveConnectorSinkConfigurationTypeDef],  # (2)
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateMediaLiveConnectorPipelineResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: LiveConnectorSourceConfigurationTypeDef](./type_defs.md#liveconnectorsourceconfigurationtypedef) 
2. See [:material-code-braces: LiveConnectorSinkConfigurationTypeDef](./type_defs.md#liveconnectorsinkconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateMediaLiveConnectorPipelineResponseTypeDef](./type_defs.md#createmedialiveconnectorpipelineresponsetypedef) 


```python
# create_media_live_connector_pipeline method usage example with argument unpacking

kwargs: CreateMediaLiveConnectorPipelineRequestRequestTypeDef = {  # (1)
    "Sources": ...,
    "Sinks": ...,
}

parent.create_media_live_connector_pipeline(**kwargs)
```

1. See [:material-code-braces: CreateMediaLiveConnectorPipelineRequestRequestTypeDef](./type_defs.md#createmedialiveconnectorpipelinerequestrequesttypedef) 

### delete\_media\_capture\_pipeline

Deletes the media pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").delete_media_capture_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.delete_media_capture_pipeline)

```python
# delete_media_capture_pipeline method definition

await def delete_media_capture_pipeline(
    self,
    *,
    MediaPipelineId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_media_capture_pipeline method usage example with argument unpacking

kwargs: DeleteMediaCapturePipelineRequestRequestTypeDef = {  # (1)
    "MediaPipelineId": ...,
}

parent.delete_media_capture_pipeline(**kwargs)
```

1. See [:material-code-braces: DeleteMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#deletemediacapturepipelinerequestrequesttypedef) 

### delete\_media\_insights\_pipeline\_configuration

Deletes the specified configuration settings.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").delete_media_insights_pipeline_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.delete_media_insights_pipeline_configuration)

```python
# delete_media_insights_pipeline_configuration method definition

await def delete_media_insights_pipeline_configuration(
    self,
    *,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_media_insights_pipeline_configuration method usage example with argument unpacking

kwargs: DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_media_insights_pipeline_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#deletemediainsightspipelineconfigurationrequestrequesttypedef) 

### delete\_media\_pipeline

Deletes the media pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").delete_media_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.delete_media_pipeline)

```python
# delete_media_pipeline method definition

await def delete_media_pipeline(
    self,
    *,
    MediaPipelineId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_media_pipeline method usage example with argument unpacking

kwargs: DeleteMediaPipelineRequestRequestTypeDef = {  # (1)
    "MediaPipelineId": ...,
}

parent.delete_media_pipeline(**kwargs)
```

1. See [:material-code-braces: DeleteMediaPipelineRequestRequestTypeDef](./type_defs.md#deletemediapipelinerequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.generate_presigned_url)

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


### get\_media\_capture\_pipeline

Gets an existing media pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").get_media_capture_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.get_media_capture_pipeline)

```python
# get_media_capture_pipeline method definition

await def get_media_capture_pipeline(
    self,
    *,
    MediaPipelineId: str,
) -> GetMediaCapturePipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMediaCapturePipelineResponseTypeDef](./type_defs.md#getmediacapturepipelineresponsetypedef) 


```python
# get_media_capture_pipeline method usage example with argument unpacking

kwargs: GetMediaCapturePipelineRequestRequestTypeDef = {  # (1)
    "MediaPipelineId": ...,
}

parent.get_media_capture_pipeline(**kwargs)
```

1. See [:material-code-braces: GetMediaCapturePipelineRequestRequestTypeDef](./type_defs.md#getmediacapturepipelinerequestrequesttypedef) 

### get\_media\_insights\_pipeline\_configuration

Gets the configuration settings for a media insights pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").get_media_insights_pipeline_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.get_media_insights_pipeline_configuration)

```python
# get_media_insights_pipeline_configuration method definition

await def get_media_insights_pipeline_configuration(
    self,
    *,
    Identifier: str,
) -> GetMediaInsightsPipelineConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMediaInsightsPipelineConfigurationResponseTypeDef](./type_defs.md#getmediainsightspipelineconfigurationresponsetypedef) 


```python
# get_media_insights_pipeline_configuration method usage example with argument unpacking

kwargs: GetMediaInsightsPipelineConfigurationRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_media_insights_pipeline_configuration(**kwargs)
```

1. See [:material-code-braces: GetMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#getmediainsightspipelineconfigurationrequestrequesttypedef) 

### get\_media\_pipeline

Gets an existing media pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").get_media_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.get_media_pipeline)

```python
# get_media_pipeline method definition

await def get_media_pipeline(
    self,
    *,
    MediaPipelineId: str,
) -> GetMediaPipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMediaPipelineResponseTypeDef](./type_defs.md#getmediapipelineresponsetypedef) 


```python
# get_media_pipeline method usage example with argument unpacking

kwargs: GetMediaPipelineRequestRequestTypeDef = {  # (1)
    "MediaPipelineId": ...,
}

parent.get_media_pipeline(**kwargs)
```

1. See [:material-code-braces: GetMediaPipelineRequestRequestTypeDef](./type_defs.md#getmediapipelinerequestrequesttypedef) 

### list\_media\_capture\_pipelines

Returns a list of media pipelines.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").list_media_capture_pipelines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_media_capture_pipelines)

```python
# list_media_capture_pipelines method definition

await def list_media_capture_pipelines(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMediaCapturePipelinesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMediaCapturePipelinesResponseTypeDef](./type_defs.md#listmediacapturepipelinesresponsetypedef) 


```python
# list_media_capture_pipelines method usage example with argument unpacking

kwargs: ListMediaCapturePipelinesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_media_capture_pipelines(**kwargs)
```

1. See [:material-code-braces: ListMediaCapturePipelinesRequestRequestTypeDef](./type_defs.md#listmediacapturepipelinesrequestrequesttypedef) 

### list\_media\_insights\_pipeline\_configurations

Lists the available media insights pipeline configurations.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").list_media_insights_pipeline_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_media_insights_pipeline_configurations)

```python
# list_media_insights_pipeline_configurations method definition

await def list_media_insights_pipeline_configurations(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMediaInsightsPipelineConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMediaInsightsPipelineConfigurationsResponseTypeDef](./type_defs.md#listmediainsightspipelineconfigurationsresponsetypedef) 


```python
# list_media_insights_pipeline_configurations method usage example with argument unpacking

kwargs: ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_media_insights_pipeline_configurations(**kwargs)
```

1. See [:material-code-braces: ListMediaInsightsPipelineConfigurationsRequestRequestTypeDef](./type_defs.md#listmediainsightspipelineconfigurationsrequestrequesttypedef) 

### list\_media\_pipelines

Returns a list of media pipelines.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").list_media_pipelines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_media_pipelines)

```python
# list_media_pipelines method definition

await def list_media_pipelines(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMediaPipelinesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMediaPipelinesResponseTypeDef](./type_defs.md#listmediapipelinesresponsetypedef) 


```python
# list_media_pipelines method usage example with argument unpacking

kwargs: ListMediaPipelinesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_media_pipelines(**kwargs)
```

1. See [:material-code-braces: ListMediaPipelinesRequestRequestTypeDef](./type_defs.md#listmediapipelinesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags available for a media pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

The ARN of the media pipeline that you want to tag.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes any tags from a media pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_media\_insights\_pipeline\_configuration

Updates the media insights pipeline's configuration settings.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").update_media_insights_pipeline_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_configuration)

```python
# update_media_insights_pipeline_configuration method definition

await def update_media_insights_pipeline_configuration(
    self,
    *,
    Identifier: str,
    ResourceAccessRoleArn: str,
    Elements: Sequence[MediaInsightsPipelineConfigurationElementTypeDef],  # (1)
    RealTimeAlertConfiguration: RealTimeAlertConfigurationTypeDef = ...,  # (2)
) -> UpdateMediaInsightsPipelineConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MediaInsightsPipelineConfigurationElementTypeDef](./type_defs.md#mediainsightspipelineconfigurationelementtypedef) 
2. See [:material-code-braces: RealTimeAlertConfigurationTypeDef](./type_defs.md#realtimealertconfigurationtypedef) 
3. See [:material-code-braces: UpdateMediaInsightsPipelineConfigurationResponseTypeDef](./type_defs.md#updatemediainsightspipelineconfigurationresponsetypedef) 


```python
# update_media_insights_pipeline_configuration method usage example with argument unpacking

kwargs: UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
    "ResourceAccessRoleArn": ...,
    "Elements": ...,
}

parent.update_media_insights_pipeline_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateMediaInsightsPipelineConfigurationRequestRequestTypeDef](./type_defs.md#updatemediainsightspipelineconfigurationrequestrequesttypedef) 

### update\_media\_insights\_pipeline\_status

Updates the status of a media insights pipeline.

Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").update_media_insights_pipeline_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.update_media_insights_pipeline_status)

```python
# update_media_insights_pipeline_status method definition

await def update_media_insights_pipeline_status(
    self,
    *,
    Identifier: str,
    UpdateStatus: MediaPipelineStatusUpdateType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MediaPipelineStatusUpdateType](./literals.md#mediapipelinestatusupdatetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_media_insights_pipeline_status method usage example with argument unpacking

kwargs: UpdateMediaInsightsPipelineStatusRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
    "UpdateStatus": ...,
}

parent.update_media_insights_pipeline_status(**kwargs)
```

1. See [:material-code-braces: UpdateMediaInsightsPipelineStatusRequestRequestTypeDef](./type_defs.md#updatemediainsightspipelinestatusrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> ChimeSDKMediaPipelinesClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("chime-sdk-media-pipelines").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#ChimeSDKMediaPipelines.Client.__aexit__)

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





