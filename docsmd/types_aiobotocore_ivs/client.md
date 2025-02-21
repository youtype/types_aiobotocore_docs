# IVSClient

> [Index](../README.md) > [IVS](./README.md) > IVSClient

!!! note ""

    Auto-generated documentation for [IVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#ivs)
    type annotations stubs module [types-aiobotocore-ivs](https://pypi.org/project/types-aiobotocore-ivs/).

## IVSClient

Type annotations and code completion for `#!python session.create_client("ivs")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client)

```python
# IVSClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_ivs.client import IVSClient

session = get_session()
async with session.create_client("ivs") as client:
    client: IVSClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("ivs").exceptions` structure.

```python
# IVSClient.exceptions usage example

async with session.create_client("ivs") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ChannelNotBroadcasting,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.PendingVerification,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.StreamUnavailable,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# IVSClient usage type checking example

from types_aiobotocore_ivs.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("ivs").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("ivs").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/generate_presigned_url.html)

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


### batch\_get\_channel

Performs <a>GetChannel</a> on multiple ARNs simultaneously.

Type annotations and code completion for `#!python session.create_client("ivs").batch_get_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/batch_get_channel.html)

```python
# batch_get_channel method definition

await def batch_get_channel(
    self,
    *,
    arns: Sequence[str],
) -> BatchGetChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetChannelResponseTypeDef](./type_defs.md#batchgetchannelresponsetypedef) 


```python
# batch_get_channel method usage example with argument unpacking

kwargs: BatchGetChannelRequestTypeDef = {  # (1)
    "arns": ...,
}

parent.batch_get_channel(**kwargs)
```

1. See [:material-code-braces: BatchGetChannelRequestTypeDef](./type_defs.md#batchgetchannelrequesttypedef) 

### batch\_get\_stream\_key

Performs <a>GetStreamKey</a> on multiple ARNs simultaneously.

Type annotations and code completion for `#!python session.create_client("ivs").batch_get_stream_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/batch_get_stream_key.html)

```python
# batch_get_stream_key method definition

await def batch_get_stream_key(
    self,
    *,
    arns: Sequence[str],
) -> BatchGetStreamKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetStreamKeyResponseTypeDef](./type_defs.md#batchgetstreamkeyresponsetypedef) 


```python
# batch_get_stream_key method usage example with argument unpacking

kwargs: BatchGetStreamKeyRequestTypeDef = {  # (1)
    "arns": ...,
}

parent.batch_get_stream_key(**kwargs)
```

1. See [:material-code-braces: BatchGetStreamKeyRequestTypeDef](./type_defs.md#batchgetstreamkeyrequesttypedef) 

### batch\_start\_viewer\_session\_revocation

Performs <a>StartViewerSessionRevocation</a> on multiple channel ARN and viewer
ID pairs simultaneously.

Type annotations and code completion for `#!python session.create_client("ivs").batch_start_viewer_session_revocation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/batch_start_viewer_session_revocation.html)

```python
# batch_start_viewer_session_revocation method definition

await def batch_start_viewer_session_revocation(
    self,
    *,
    viewerSessions: Sequence[BatchStartViewerSessionRevocationViewerSessionTypeDef],  # (1)
) -> BatchStartViewerSessionRevocationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: BatchStartViewerSessionRevocationViewerSessionTypeDef](./type_defs.md#batchstartviewersessionrevocationviewersessiontypedef) 
2. See [:material-code-braces: BatchStartViewerSessionRevocationResponseTypeDef](./type_defs.md#batchstartviewersessionrevocationresponsetypedef) 


```python
# batch_start_viewer_session_revocation method usage example with argument unpacking

kwargs: BatchStartViewerSessionRevocationRequestTypeDef = {  # (1)
    "viewerSessions": ...,
}

parent.batch_start_viewer_session_revocation(**kwargs)
```

1. See [:material-code-braces: BatchStartViewerSessionRevocationRequestTypeDef](./type_defs.md#batchstartviewersessionrevocationrequesttypedef) 

### create\_channel

Creates a new channel and an associated stream key to start streaming.

Type annotations and code completion for `#!python session.create_client("ivs").create_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/create_channel.html)

```python
# create_channel method definition

await def create_channel(
    self,
    *,
    authorized: bool = ...,
    containerFormat: ContainerFormatType = ...,  # (1)
    insecureIngest: bool = ...,
    latencyMode: ChannelLatencyModeType = ...,  # (2)
    multitrackInputConfiguration: MultitrackInputConfigurationTypeDef = ...,  # (3)
    name: str = ...,
    playbackRestrictionPolicyArn: str = ...,
    preset: TranscodePresetType = ...,  # (4)
    recordingConfigurationArn: str = ...,
    tags: Mapping[str, str] = ...,
    type: ChannelTypeType = ...,  # (5)
) -> CreateChannelResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ContainerFormatType](./literals.md#containerformattype) 
2. See [:material-code-brackets: ChannelLatencyModeType](./literals.md#channellatencymodetype) 
3. See [:material-code-braces: MultitrackInputConfigurationTypeDef](./type_defs.md#multitrackinputconfigurationtypedef) 
4. See [:material-code-brackets: TranscodePresetType](./literals.md#transcodepresettype) 
5. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
6. See [:material-code-braces: CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef) 


```python
# create_channel method usage example with argument unpacking

kwargs: CreateChannelRequestTypeDef = {  # (1)
    "authorized": ...,
}

parent.create_channel(**kwargs)
```

1. See [:material-code-braces: CreateChannelRequestTypeDef](./type_defs.md#createchannelrequesttypedef) 

### create\_playback\_restriction\_policy

Creates a new playback restriction policy, for constraining playback by
countries and/or origins.

Type annotations and code completion for `#!python session.create_client("ivs").create_playback_restriction_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/create_playback_restriction_policy.html)

```python
# create_playback_restriction_policy method definition

await def create_playback_restriction_policy(
    self,
    *,
    allowedCountries: Sequence[str] = ...,
    allowedOrigins: Sequence[str] = ...,
    enableStrictOriginEnforcement: bool = ...,
    name: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreatePlaybackRestrictionPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePlaybackRestrictionPolicyResponseTypeDef](./type_defs.md#createplaybackrestrictionpolicyresponsetypedef) 


```python
# create_playback_restriction_policy method usage example with argument unpacking

kwargs: CreatePlaybackRestrictionPolicyRequestTypeDef = {  # (1)
    "allowedCountries": ...,
}

parent.create_playback_restriction_policy(**kwargs)
```

1. See [:material-code-braces: CreatePlaybackRestrictionPolicyRequestTypeDef](./type_defs.md#createplaybackrestrictionpolicyrequesttypedef) 

### create\_recording\_configuration

Creates a new recording configuration, used to enable recording to Amazon S3.

Type annotations and code completion for `#!python session.create_client("ivs").create_recording_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/create_recording_configuration.html)

```python
# create_recording_configuration method definition

await def create_recording_configuration(
    self,
    *,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    name: str = ...,
    recordingReconnectWindowSeconds: int = ...,
    renditionConfiguration: RenditionConfigurationUnionTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
    thumbnailConfiguration: ThumbnailConfigurationUnionTypeDef = ...,  # (3)
) -> CreateRecordingConfigurationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-braces: RenditionConfigurationTypeDef](./type_defs.md#renditionconfigurationtypedef) [:material-code-braces: RenditionConfigurationOutputTypeDef](./type_defs.md#renditionconfigurationoutputtypedef) 
3. See [:material-code-braces: ThumbnailConfigurationTypeDef](./type_defs.md#thumbnailconfigurationtypedef) [:material-code-braces: ThumbnailConfigurationOutputTypeDef](./type_defs.md#thumbnailconfigurationoutputtypedef) 
4. See [:material-code-braces: CreateRecordingConfigurationResponseTypeDef](./type_defs.md#createrecordingconfigurationresponsetypedef) 


```python
# create_recording_configuration method usage example with argument unpacking

kwargs: CreateRecordingConfigurationRequestTypeDef = {  # (1)
    "destinationConfiguration": ...,
}

parent.create_recording_configuration(**kwargs)
```

1. See [:material-code-braces: CreateRecordingConfigurationRequestTypeDef](./type_defs.md#createrecordingconfigurationrequesttypedef) 

### create\_stream\_key

Creates a stream key, used to initiate a stream, for the specified channel ARN.

Type annotations and code completion for `#!python session.create_client("ivs").create_stream_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/create_stream_key.html)

```python
# create_stream_key method definition

await def create_stream_key(
    self,
    *,
    channelArn: str,
    tags: Mapping[str, str] = ...,
) -> CreateStreamKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateStreamKeyResponseTypeDef](./type_defs.md#createstreamkeyresponsetypedef) 


```python
# create_stream_key method usage example with argument unpacking

kwargs: CreateStreamKeyRequestTypeDef = {  # (1)
    "channelArn": ...,
}

parent.create_stream_key(**kwargs)
```

1. See [:material-code-braces: CreateStreamKeyRequestTypeDef](./type_defs.md#createstreamkeyrequesttypedef) 

### delete\_channel

Deletes the specified channel and its associated stream keys.

Type annotations and code completion for `#!python session.create_client("ivs").delete_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/delete_channel.html)

```python
# delete_channel method definition

await def delete_channel(
    self,
    *,
    arn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_channel method usage example with argument unpacking

kwargs: DeleteChannelRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_channel(**kwargs)
```

1. See [:material-code-braces: DeleteChannelRequestTypeDef](./type_defs.md#deletechannelrequesttypedef) 

### delete\_playback\_key\_pair

Deletes a specified authorization key pair.

Type annotations and code completion for `#!python session.create_client("ivs").delete_playback_key_pair` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/delete_playback_key_pair.html)

```python
# delete_playback_key_pair method definition

await def delete_playback_key_pair(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_playback_key_pair method usage example with argument unpacking

kwargs: DeletePlaybackKeyPairRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_playback_key_pair(**kwargs)
```

1. See [:material-code-braces: DeletePlaybackKeyPairRequestTypeDef](./type_defs.md#deleteplaybackkeypairrequesttypedef) 

### delete\_playback\_restriction\_policy

Deletes the specified playback restriction policy.

Type annotations and code completion for `#!python session.create_client("ivs").delete_playback_restriction_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/delete_playback_restriction_policy.html)

```python
# delete_playback_restriction_policy method definition

await def delete_playback_restriction_policy(
    self,
    *,
    arn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_playback_restriction_policy method usage example with argument unpacking

kwargs: DeletePlaybackRestrictionPolicyRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_playback_restriction_policy(**kwargs)
```

1. See [:material-code-braces: DeletePlaybackRestrictionPolicyRequestTypeDef](./type_defs.md#deleteplaybackrestrictionpolicyrequesttypedef) 

### delete\_recording\_configuration

Deletes the recording configuration for the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs").delete_recording_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/delete_recording_configuration.html)

```python
# delete_recording_configuration method definition

await def delete_recording_configuration(
    self,
    *,
    arn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_recording_configuration method usage example with argument unpacking

kwargs: DeleteRecordingConfigurationRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_recording_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteRecordingConfigurationRequestTypeDef](./type_defs.md#deleterecordingconfigurationrequesttypedef) 

### delete\_stream\_key

Deletes the stream key for the specified ARN, so it can no longer be used to
stream.

Type annotations and code completion for `#!python session.create_client("ivs").delete_stream_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/delete_stream_key.html)

```python
# delete_stream_key method definition

await def delete_stream_key(
    self,
    *,
    arn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_stream_key method usage example with argument unpacking

kwargs: DeleteStreamKeyRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_stream_key(**kwargs)
```

1. See [:material-code-braces: DeleteStreamKeyRequestTypeDef](./type_defs.md#deletestreamkeyrequesttypedef) 

### get\_channel

Gets the channel configuration for the specified channel ARN.

Type annotations and code completion for `#!python session.create_client("ivs").get_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/get_channel.html)

```python
# get_channel method definition

await def get_channel(
    self,
    *,
    arn: str,
) -> GetChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelResponseTypeDef](./type_defs.md#getchannelresponsetypedef) 


```python
# get_channel method usage example with argument unpacking

kwargs: GetChannelRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_channel(**kwargs)
```

1. See [:material-code-braces: GetChannelRequestTypeDef](./type_defs.md#getchannelrequesttypedef) 

### get\_playback\_key\_pair

Gets a specified playback authorization key pair and returns the
<code>arn</code> and <code>fingerprint</code>.

Type annotations and code completion for `#!python session.create_client("ivs").get_playback_key_pair` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/get_playback_key_pair.html)

```python
# get_playback_key_pair method definition

await def get_playback_key_pair(
    self,
    *,
    arn: str,
) -> GetPlaybackKeyPairResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPlaybackKeyPairResponseTypeDef](./type_defs.md#getplaybackkeypairresponsetypedef) 


```python
# get_playback_key_pair method usage example with argument unpacking

kwargs: GetPlaybackKeyPairRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_playback_key_pair(**kwargs)
```

1. See [:material-code-braces: GetPlaybackKeyPairRequestTypeDef](./type_defs.md#getplaybackkeypairrequesttypedef) 

### get\_playback\_restriction\_policy

Gets the specified playback restriction policy.

Type annotations and code completion for `#!python session.create_client("ivs").get_playback_restriction_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/get_playback_restriction_policy.html)

```python
# get_playback_restriction_policy method definition

await def get_playback_restriction_policy(
    self,
    *,
    arn: str,
) -> GetPlaybackRestrictionPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPlaybackRestrictionPolicyResponseTypeDef](./type_defs.md#getplaybackrestrictionpolicyresponsetypedef) 


```python
# get_playback_restriction_policy method usage example with argument unpacking

kwargs: GetPlaybackRestrictionPolicyRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_playback_restriction_policy(**kwargs)
```

1. See [:material-code-braces: GetPlaybackRestrictionPolicyRequestTypeDef](./type_defs.md#getplaybackrestrictionpolicyrequesttypedef) 

### get\_recording\_configuration

Gets the recording configuration for the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs").get_recording_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/get_recording_configuration.html)

```python
# get_recording_configuration method definition

await def get_recording_configuration(
    self,
    *,
    arn: str,
) -> GetRecordingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRecordingConfigurationResponseTypeDef](./type_defs.md#getrecordingconfigurationresponsetypedef) 


```python
# get_recording_configuration method usage example with argument unpacking

kwargs: GetRecordingConfigurationRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_recording_configuration(**kwargs)
```

1. See [:material-code-braces: GetRecordingConfigurationRequestTypeDef](./type_defs.md#getrecordingconfigurationrequesttypedef) 

### get\_stream

Gets information about the active (live) stream on a specified channel.

Type annotations and code completion for `#!python session.create_client("ivs").get_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/get_stream.html)

```python
# get_stream method definition

await def get_stream(
    self,
    *,
    channelArn: str,
) -> GetStreamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStreamResponseTypeDef](./type_defs.md#getstreamresponsetypedef) 


```python
# get_stream method usage example with argument unpacking

kwargs: GetStreamRequestTypeDef = {  # (1)
    "channelArn": ...,
}

parent.get_stream(**kwargs)
```

1. See [:material-code-braces: GetStreamRequestTypeDef](./type_defs.md#getstreamrequesttypedef) 

### get\_stream\_key

Gets stream-key information for a specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs").get_stream_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/get_stream_key.html)

```python
# get_stream_key method definition

await def get_stream_key(
    self,
    *,
    arn: str,
) -> GetStreamKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStreamKeyResponseTypeDef](./type_defs.md#getstreamkeyresponsetypedef) 


```python
# get_stream_key method usage example with argument unpacking

kwargs: GetStreamKeyRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_stream_key(**kwargs)
```

1. See [:material-code-braces: GetStreamKeyRequestTypeDef](./type_defs.md#getstreamkeyrequesttypedef) 

### get\_stream\_session

Gets metadata on a specified stream.

Type annotations and code completion for `#!python session.create_client("ivs").get_stream_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/get_stream_session.html)

```python
# get_stream_session method definition

await def get_stream_session(
    self,
    *,
    channelArn: str,
    streamId: str = ...,
) -> GetStreamSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStreamSessionResponseTypeDef](./type_defs.md#getstreamsessionresponsetypedef) 


```python
# get_stream_session method usage example with argument unpacking

kwargs: GetStreamSessionRequestTypeDef = {  # (1)
    "channelArn": ...,
}

parent.get_stream_session(**kwargs)
```

1. See [:material-code-braces: GetStreamSessionRequestTypeDef](./type_defs.md#getstreamsessionrequesttypedef) 

### import\_playback\_key\_pair

Imports the public portion of a new key pair and returns its <code>arn</code>
and <code>fingerprint</code>.

Type annotations and code completion for `#!python session.create_client("ivs").import_playback_key_pair` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/import_playback_key_pair.html)

```python
# import_playback_key_pair method definition

await def import_playback_key_pair(
    self,
    *,
    publicKeyMaterial: str,
    name: str = ...,
    tags: Mapping[str, str] = ...,
) -> ImportPlaybackKeyPairResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ImportPlaybackKeyPairResponseTypeDef](./type_defs.md#importplaybackkeypairresponsetypedef) 


```python
# import_playback_key_pair method usage example with argument unpacking

kwargs: ImportPlaybackKeyPairRequestTypeDef = {  # (1)
    "publicKeyMaterial": ...,
}

parent.import_playback_key_pair(**kwargs)
```

1. See [:material-code-braces: ImportPlaybackKeyPairRequestTypeDef](./type_defs.md#importplaybackkeypairrequesttypedef) 

### list\_channels

Gets summary information about all channels in your account, in the Amazon Web
Services region where the API request is processed.

Type annotations and code completion for `#!python session.create_client("ivs").list_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/list_channels.html)

```python
# list_channels method definition

await def list_channels(
    self,
    *,
    filterByName: str = ...,
    filterByPlaybackRestrictionPolicyArn: str = ...,
    filterByRecordingConfigurationArn: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# list_channels method usage example with argument unpacking

kwargs: ListChannelsRequestTypeDef = {  # (1)
    "filterByName": ...,
}

parent.list_channels(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestTypeDef](./type_defs.md#listchannelsrequesttypedef) 

### list\_playback\_key\_pairs

Gets summary information about playback key pairs.

Type annotations and code completion for `#!python session.create_client("ivs").list_playback_key_pairs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/list_playback_key_pairs.html)

```python
# list_playback_key_pairs method definition

await def list_playback_key_pairs(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPlaybackKeyPairsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPlaybackKeyPairsResponseTypeDef](./type_defs.md#listplaybackkeypairsresponsetypedef) 


```python
# list_playback_key_pairs method usage example with argument unpacking

kwargs: ListPlaybackKeyPairsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_playback_key_pairs(**kwargs)
```

1. See [:material-code-braces: ListPlaybackKeyPairsRequestTypeDef](./type_defs.md#listplaybackkeypairsrequesttypedef) 

### list\_playback\_restriction\_policies

Gets summary information about playback restriction policies.

Type annotations and code completion for `#!python session.create_client("ivs").list_playback_restriction_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/list_playback_restriction_policies.html)

```python
# list_playback_restriction_policies method definition

await def list_playback_restriction_policies(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPlaybackRestrictionPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPlaybackRestrictionPoliciesResponseTypeDef](./type_defs.md#listplaybackrestrictionpoliciesresponsetypedef) 


```python
# list_playback_restriction_policies method usage example with argument unpacking

kwargs: ListPlaybackRestrictionPoliciesRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_playback_restriction_policies(**kwargs)
```

1. See [:material-code-braces: ListPlaybackRestrictionPoliciesRequestTypeDef](./type_defs.md#listplaybackrestrictionpoliciesrequesttypedef) 

### list\_recording\_configurations

Gets summary information about all recording configurations in your account, in
the Amazon Web Services region where the API request is processed.

Type annotations and code completion for `#!python session.create_client("ivs").list_recording_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/list_recording_configurations.html)

```python
# list_recording_configurations method definition

await def list_recording_configurations(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListRecordingConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRecordingConfigurationsResponseTypeDef](./type_defs.md#listrecordingconfigurationsresponsetypedef) 


```python
# list_recording_configurations method usage example with argument unpacking

kwargs: ListRecordingConfigurationsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_recording_configurations(**kwargs)
```

1. See [:material-code-braces: ListRecordingConfigurationsRequestTypeDef](./type_defs.md#listrecordingconfigurationsrequesttypedef) 

### list\_stream\_keys

Gets summary information about stream keys for the specified channel.

Type annotations and code completion for `#!python session.create_client("ivs").list_stream_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/list_stream_keys.html)

```python
# list_stream_keys method definition

await def list_stream_keys(
    self,
    *,
    channelArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListStreamKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStreamKeysResponseTypeDef](./type_defs.md#liststreamkeysresponsetypedef) 


```python
# list_stream_keys method usage example with argument unpacking

kwargs: ListStreamKeysRequestTypeDef = {  # (1)
    "channelArn": ...,
}

parent.list_stream_keys(**kwargs)
```

1. See [:material-code-braces: ListStreamKeysRequestTypeDef](./type_defs.md#liststreamkeysrequesttypedef) 

### list\_stream\_sessions

Gets a summary of current and previous streams for a specified channel in your
account, in the AWS region where the API request is processed.

Type annotations and code completion for `#!python session.create_client("ivs").list_stream_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/list_stream_sessions.html)

```python
# list_stream_sessions method definition

await def list_stream_sessions(
    self,
    *,
    channelArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListStreamSessionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStreamSessionsResponseTypeDef](./type_defs.md#liststreamsessionsresponsetypedef) 


```python
# list_stream_sessions method usage example with argument unpacking

kwargs: ListStreamSessionsRequestTypeDef = {  # (1)
    "channelArn": ...,
}

parent.list_stream_sessions(**kwargs)
```

1. See [:material-code-braces: ListStreamSessionsRequestTypeDef](./type_defs.md#liststreamsessionsrequesttypedef) 

### list\_streams

Gets summary information about live streams in your account, in the Amazon Web
Services region where the API request is processed.

Type annotations and code completion for `#!python session.create_client("ivs").list_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/list_streams.html)

```python
# list_streams method definition

await def list_streams(
    self,
    *,
    filterBy: StreamFiltersTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListStreamsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamFiltersTypeDef](./type_defs.md#streamfilterstypedef) 
2. See [:material-code-braces: ListStreamsResponseTypeDef](./type_defs.md#liststreamsresponsetypedef) 


```python
# list_streams method usage example with argument unpacking

kwargs: ListStreamsRequestTypeDef = {  # (1)
    "filterBy": ...,
}

parent.list_streams(**kwargs)
```

1. See [:material-code-braces: ListStreamsRequestTypeDef](./type_defs.md#liststreamsrequesttypedef) 

### list\_tags\_for\_resource

Gets information about Amazon Web Services tags for the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### put\_metadata

Inserts metadata into the active stream of the specified channel.

Type annotations and code completion for `#!python session.create_client("ivs").put_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/put_metadata.html)

```python
# put_metadata method definition

await def put_metadata(
    self,
    *,
    channelArn: str,
    metadata: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_metadata method usage example with argument unpacking

kwargs: PutMetadataRequestTypeDef = {  # (1)
    "channelArn": ...,
    "metadata": ...,
}

parent.put_metadata(**kwargs)
```

1. See [:material-code-braces: PutMetadataRequestTypeDef](./type_defs.md#putmetadatarequesttypedef) 

### start\_viewer\_session\_revocation

Starts the process of revoking the viewer session associated with a specified
channel ARN and viewer ID.

Type annotations and code completion for `#!python session.create_client("ivs").start_viewer_session_revocation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/start_viewer_session_revocation.html)

```python
# start_viewer_session_revocation method definition

await def start_viewer_session_revocation(
    self,
    *,
    channelArn: str,
    viewerId: str,
    viewerSessionVersionsLessThanOrEqualTo: int = ...,
) -> Dict[str, Any]:
    ...
```



```python
# start_viewer_session_revocation method usage example with argument unpacking

kwargs: StartViewerSessionRevocationRequestTypeDef = {  # (1)
    "channelArn": ...,
    "viewerId": ...,
}

parent.start_viewer_session_revocation(**kwargs)
```

1. See [:material-code-braces: StartViewerSessionRevocationRequestTypeDef](./type_defs.md#startviewersessionrevocationrequesttypedef) 

### stop\_stream

Disconnects the incoming RTMPS stream for the specified channel.

Type annotations and code completion for `#!python session.create_client("ivs").stop_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/stop_stream.html)

```python
# stop_stream method definition

await def stop_stream(
    self,
    *,
    channelArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_stream method usage example with argument unpacking

kwargs: StopStreamRequestTypeDef = {  # (1)
    "channelArn": ...,
}

parent.stop_stream(**kwargs)
```

1. See [:material-code-braces: StopStreamRequestTypeDef](./type_defs.md#stopstreamrequesttypedef) 

### tag\_resource

Adds or updates tags for the Amazon Web Services resource with the specified
ARN.

Type annotations and code completion for `#!python session.create_client("ivs").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes tags from the resource with the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_channel

Updates a channel's configuration.

Type annotations and code completion for `#!python session.create_client("ivs").update_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/update_channel.html)

```python
# update_channel method definition

await def update_channel(
    self,
    *,
    arn: str,
    authorized: bool = ...,
    containerFormat: ContainerFormatType = ...,  # (1)
    insecureIngest: bool = ...,
    latencyMode: ChannelLatencyModeType = ...,  # (2)
    multitrackInputConfiguration: MultitrackInputConfigurationTypeDef = ...,  # (3)
    name: str = ...,
    playbackRestrictionPolicyArn: str = ...,
    preset: TranscodePresetType = ...,  # (4)
    recordingConfigurationArn: str = ...,
    type: ChannelTypeType = ...,  # (5)
) -> UpdateChannelResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ContainerFormatType](./literals.md#containerformattype) 
2. See [:material-code-brackets: ChannelLatencyModeType](./literals.md#channellatencymodetype) 
3. See [:material-code-braces: MultitrackInputConfigurationTypeDef](./type_defs.md#multitrackinputconfigurationtypedef) 
4. See [:material-code-brackets: TranscodePresetType](./literals.md#transcodepresettype) 
5. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
6. See [:material-code-braces: UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef) 


```python
# update_channel method usage example with argument unpacking

kwargs: UpdateChannelRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_channel(**kwargs)
```

1. See [:material-code-braces: UpdateChannelRequestTypeDef](./type_defs.md#updatechannelrequesttypedef) 

### update\_playback\_restriction\_policy

Updates a specified playback restriction policy.

Type annotations and code completion for `#!python session.create_client("ivs").update_playback_restriction_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs/client/update_playback_restriction_policy.html)

```python
# update_playback_restriction_policy method definition

await def update_playback_restriction_policy(
    self,
    *,
    arn: str,
    allowedCountries: Sequence[str] = ...,
    allowedOrigins: Sequence[str] = ...,
    enableStrictOriginEnforcement: bool = ...,
    name: str = ...,
) -> UpdatePlaybackRestrictionPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdatePlaybackRestrictionPolicyResponseTypeDef](./type_defs.md#updateplaybackrestrictionpolicyresponsetypedef) 


```python
# update_playback_restriction_policy method usage example with argument unpacking

kwargs: UpdatePlaybackRestrictionPolicyRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_playback_restriction_policy(**kwargs)
```

1. See [:material-code-braces: UpdatePlaybackRestrictionPolicyRequestTypeDef](./type_defs.md#updateplaybackrestrictionpolicyrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("ivs").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("ivs").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#IVS.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("ivs").get_paginator` method with overloads.

- `client.get_paginator("list_channels")` -> [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- `client.get_paginator("list_playback_key_pairs")` -> [ListPlaybackKeyPairsPaginator](./paginators.md#listplaybackkeypairspaginator)
- `client.get_paginator("list_recording_configurations")` -> [ListRecordingConfigurationsPaginator](./paginators.md#listrecordingconfigurationspaginator)
- `client.get_paginator("list_stream_keys")` -> [ListStreamKeysPaginator](./paginators.md#liststreamkeyspaginator)
- `client.get_paginator("list_streams")` -> [ListStreamsPaginator](./paginators.md#liststreamspaginator)



