# MediaTailorClient

> [Index](../README.md) > [MediaTailor](./README.md) > MediaTailorClient

!!! note ""

    Auto-generated documentation for [MediaTailor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor)
    type annotations stubs module [types-aiobotocore-mediatailor](https://pypi.org/project/types-aiobotocore-mediatailor/).

## MediaTailorClient

Type annotations and code completion for `#!python session.create_client("mediatailor")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client)

```python
# MediaTailorClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_mediatailor.client import MediaTailorClient

session = get_session()
async with session.create_client("mediatailor") as client:
    client: MediaTailorClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("mediatailor").exceptions` structure.

```python
# MediaTailorClient.exceptions usage example

async with session.create_client("mediatailor") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
    ) as e:
        print(e)
```

```python
# MediaTailorClient usage type checking example

from types_aiobotocore_mediatailor.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("mediatailor").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("mediatailor").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### configure\_logs\_for\_channel

Configures Amazon CloudWatch log settings for a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").configure_logs_for_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.configure_logs_for_channel)

```python
# configure_logs_for_channel method definition

await def configure_logs_for_channel(
    self,
    *,
    ChannelName: str,
    LogTypes: Sequence[LogTypeType],  # (1)
) -> ConfigureLogsForChannelResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-braces: ConfigureLogsForChannelResponseTypeDef](./type_defs.md#configurelogsforchannelresponsetypedef) 


```python
# configure_logs_for_channel method usage example with argument unpacking

kwargs: ConfigureLogsForChannelRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
    "LogTypes": ...,
}

parent.configure_logs_for_channel(**kwargs)
```

1. See [:material-code-braces: ConfigureLogsForChannelRequestRequestTypeDef](./type_defs.md#configurelogsforchannelrequestrequesttypedef) 

### configure\_logs\_for\_playback\_configuration

Amazon CloudWatch log settings for a playback configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").configure_logs_for_playback_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.configure_logs_for_playback_configuration)

```python
# configure_logs_for_playback_configuration method definition

await def configure_logs_for_playback_configuration(
    self,
    *,
    PercentEnabled: int,
    PlaybackConfigurationName: str,
) -> ConfigureLogsForPlaybackConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ConfigureLogsForPlaybackConfigurationResponseTypeDef](./type_defs.md#configurelogsforplaybackconfigurationresponsetypedef) 


```python
# configure_logs_for_playback_configuration method usage example with argument unpacking

kwargs: ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef = {  # (1)
    "PercentEnabled": ...,
    "PlaybackConfigurationName": ...,
}

parent.configure_logs_for_playback_configuration(**kwargs)
```

1. See [:material-code-braces: ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef](./type_defs.md#configurelogsforplaybackconfigurationrequestrequesttypedef) 

### create\_channel

Creates a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").create_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_channel)

```python
# create_channel method definition

await def create_channel(
    self,
    *,
    ChannelName: str,
    Outputs: Sequence[RequestOutputItemTypeDef],  # (1)
    PlaybackMode: PlaybackModeType,  # (2)
    Audiences: Sequence[str] = ...,
    FillerSlate: SlateSourceTypeDef = ...,  # (3)
    Tags: Mapping[str, str] = ...,
    Tier: TierType = ...,  # (4)
    TimeShiftConfiguration: TimeShiftConfigurationTypeDef = ...,  # (5)
) -> CreateChannelResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: RequestOutputItemTypeDef](./type_defs.md#requestoutputitemtypedef) 
2. See [:material-code-brackets: PlaybackModeType](./literals.md#playbackmodetype) 
3. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
4. See [:material-code-brackets: TierType](./literals.md#tiertype) 
5. See [:material-code-braces: TimeShiftConfigurationTypeDef](./type_defs.md#timeshiftconfigurationtypedef) 
6. See [:material-code-braces: CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef) 


```python
# create_channel method usage example with argument unpacking

kwargs: CreateChannelRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
    "Outputs": ...,
    "PlaybackMode": ...,
}

parent.create_channel(**kwargs)
```

1. See [:material-code-braces: CreateChannelRequestRequestTypeDef](./type_defs.md#createchannelrequestrequesttypedef) 

### create\_live\_source

The live source configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").create_live_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_live_source)

```python
# create_live_source method definition

await def create_live_source(
    self,
    *,
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    LiveSourceName: str,
    SourceLocationName: str,
    Tags: Mapping[str, str] = ...,
) -> CreateLiveSourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
2. See [:material-code-braces: CreateLiveSourceResponseTypeDef](./type_defs.md#createlivesourceresponsetypedef) 


```python
# create_live_source method usage example with argument unpacking

kwargs: CreateLiveSourceRequestRequestTypeDef = {  # (1)
    "HttpPackageConfigurations": ...,
    "LiveSourceName": ...,
    "SourceLocationName": ...,
}

parent.create_live_source(**kwargs)
```

1. See [:material-code-braces: CreateLiveSourceRequestRequestTypeDef](./type_defs.md#createlivesourcerequestrequesttypedef) 

### create\_prefetch\_schedule

Creates a prefetch schedule for a playback configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").create_prefetch_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_prefetch_schedule)

```python
# create_prefetch_schedule method definition

await def create_prefetch_schedule(
    self,
    *,
    Consumption: PrefetchConsumptionTypeDef,  # (1)
    Name: str,
    PlaybackConfigurationName: str,
    Retrieval: PrefetchRetrievalTypeDef,  # (2)
    StreamId: str = ...,
) -> CreatePrefetchScheduleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PrefetchConsumptionTypeDef](./type_defs.md#prefetchconsumptiontypedef) 
2. See [:material-code-braces: PrefetchRetrievalTypeDef](./type_defs.md#prefetchretrievaltypedef) 
3. See [:material-code-braces: CreatePrefetchScheduleResponseTypeDef](./type_defs.md#createprefetchscheduleresponsetypedef) 


```python
# create_prefetch_schedule method usage example with argument unpacking

kwargs: CreatePrefetchScheduleRequestRequestTypeDef = {  # (1)
    "Consumption": ...,
    "Name": ...,
    "PlaybackConfigurationName": ...,
    "Retrieval": ...,
}

parent.create_prefetch_schedule(**kwargs)
```

1. See [:material-code-braces: CreatePrefetchScheduleRequestRequestTypeDef](./type_defs.md#createprefetchschedulerequestrequesttypedef) 

### create\_program

Creates a program within a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").create_program` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_program)

```python
# create_program method definition

await def create_program(
    self,
    *,
    ChannelName: str,
    ProgramName: str,
    ScheduleConfiguration: ScheduleConfigurationTypeDef,  # (1)
    SourceLocationName: str,
    AdBreaks: Sequence[AdBreakUnionTypeDef] = ...,  # (2)
    AudienceMedia: Sequence[AudienceMediaUnionTypeDef] = ...,  # (3)
    LiveSourceName: str = ...,
    VodSourceName: str = ...,
) -> CreateProgramResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) [:material-code-braces: AdBreakOutputTypeDef](./type_defs.md#adbreakoutputtypedef) 
3. See [:material-code-braces: AudienceMediaTypeDef](./type_defs.md#audiencemediatypedef) [:material-code-braces: AudienceMediaOutputTypeDef](./type_defs.md#audiencemediaoutputtypedef) 
4. See [:material-code-braces: CreateProgramResponseTypeDef](./type_defs.md#createprogramresponsetypedef) 


```python
# create_program method usage example with argument unpacking

kwargs: CreateProgramRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
    "ProgramName": ...,
    "ScheduleConfiguration": ...,
    "SourceLocationName": ...,
}

parent.create_program(**kwargs)
```

1. See [:material-code-braces: CreateProgramRequestRequestTypeDef](./type_defs.md#createprogramrequestrequesttypedef) 

### create\_source\_location

Creates a source location.

Type annotations and code completion for `#!python session.create_client("mediatailor").create_source_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_source_location)

```python
# create_source_location method definition

await def create_source_location(
    self,
    *,
    HttpConfiguration: HttpConfigurationTypeDef,  # (1)
    SourceLocationName: str,
    AccessConfiguration: AccessConfigurationTypeDef = ...,  # (2)
    DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,  # (3)
    SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...,  # (4)
    Tags: Mapping[str, str] = ...,
) -> CreateSourceLocationResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: HttpConfigurationTypeDef](./type_defs.md#httpconfigurationtypedef) 
2. See [:material-code-braces: AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef) 
3. See [:material-code-braces: DefaultSegmentDeliveryConfigurationTypeDef](./type_defs.md#defaultsegmentdeliveryconfigurationtypedef) 
4. See [:material-code-braces: SegmentDeliveryConfigurationTypeDef](./type_defs.md#segmentdeliveryconfigurationtypedef) 
5. See [:material-code-braces: CreateSourceLocationResponseTypeDef](./type_defs.md#createsourcelocationresponsetypedef) 


```python
# create_source_location method usage example with argument unpacking

kwargs: CreateSourceLocationRequestRequestTypeDef = {  # (1)
    "HttpConfiguration": ...,
    "SourceLocationName": ...,
}

parent.create_source_location(**kwargs)
```

1. See [:material-code-braces: CreateSourceLocationRequestRequestTypeDef](./type_defs.md#createsourcelocationrequestrequesttypedef) 

### create\_vod\_source

The VOD source configuration parameters.

Type annotations and code completion for `#!python session.create_client("mediatailor").create_vod_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_vod_source)

```python
# create_vod_source method definition

await def create_vod_source(
    self,
    *,
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    SourceLocationName: str,
    VodSourceName: str,
    Tags: Mapping[str, str] = ...,
) -> CreateVodSourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
2. See [:material-code-braces: CreateVodSourceResponseTypeDef](./type_defs.md#createvodsourceresponsetypedef) 


```python
# create_vod_source method usage example with argument unpacking

kwargs: CreateVodSourceRequestRequestTypeDef = {  # (1)
    "HttpPackageConfigurations": ...,
    "SourceLocationName": ...,
    "VodSourceName": ...,
}

parent.create_vod_source(**kwargs)
```

1. See [:material-code-braces: CreateVodSourceRequestRequestTypeDef](./type_defs.md#createvodsourcerequestrequesttypedef) 

### delete\_channel

Deletes a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").delete_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_channel)

```python
# delete_channel method definition

await def delete_channel(
    self,
    *,
    ChannelName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_channel method usage example with argument unpacking

kwargs: DeleteChannelRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.delete_channel(**kwargs)
```

1. See [:material-code-braces: DeleteChannelRequestRequestTypeDef](./type_defs.md#deletechannelrequestrequesttypedef) 

### delete\_channel\_policy

The channel policy to delete.

Type annotations and code completion for `#!python session.create_client("mediatailor").delete_channel_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_channel_policy)

```python
# delete_channel_policy method definition

await def delete_channel_policy(
    self,
    *,
    ChannelName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_channel_policy method usage example with argument unpacking

kwargs: DeleteChannelPolicyRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.delete_channel_policy(**kwargs)
```

1. See [:material-code-braces: DeleteChannelPolicyRequestRequestTypeDef](./type_defs.md#deletechannelpolicyrequestrequesttypedef) 

### delete\_live\_source

The live source to delete.

Type annotations and code completion for `#!python session.create_client("mediatailor").delete_live_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_live_source)

```python
# delete_live_source method definition

await def delete_live_source(
    self,
    *,
    LiveSourceName: str,
    SourceLocationName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_live_source method usage example with argument unpacking

kwargs: DeleteLiveSourceRequestRequestTypeDef = {  # (1)
    "LiveSourceName": ...,
    "SourceLocationName": ...,
}

parent.delete_live_source(**kwargs)
```

1. See [:material-code-braces: DeleteLiveSourceRequestRequestTypeDef](./type_defs.md#deletelivesourcerequestrequesttypedef) 

### delete\_playback\_configuration

Deletes a playback configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").delete_playback_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_playback_configuration)

```python
# delete_playback_configuration method definition

await def delete_playback_configuration(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_playback_configuration method usage example with argument unpacking

kwargs: DeletePlaybackConfigurationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_playback_configuration(**kwargs)
```

1. See [:material-code-braces: DeletePlaybackConfigurationRequestRequestTypeDef](./type_defs.md#deleteplaybackconfigurationrequestrequesttypedef) 

### delete\_prefetch\_schedule

Deletes a prefetch schedule for a specific playback configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").delete_prefetch_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_prefetch_schedule)

```python
# delete_prefetch_schedule method definition

await def delete_prefetch_schedule(
    self,
    *,
    Name: str,
    PlaybackConfigurationName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_prefetch_schedule method usage example with argument unpacking

kwargs: DeletePrefetchScheduleRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "PlaybackConfigurationName": ...,
}

parent.delete_prefetch_schedule(**kwargs)
```

1. See [:material-code-braces: DeletePrefetchScheduleRequestRequestTypeDef](./type_defs.md#deleteprefetchschedulerequestrequesttypedef) 

### delete\_program

Deletes a program within a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").delete_program` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_program)

```python
# delete_program method definition

await def delete_program(
    self,
    *,
    ChannelName: str,
    ProgramName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_program method usage example with argument unpacking

kwargs: DeleteProgramRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
    "ProgramName": ...,
}

parent.delete_program(**kwargs)
```

1. See [:material-code-braces: DeleteProgramRequestRequestTypeDef](./type_defs.md#deleteprogramrequestrequesttypedef) 

### delete\_source\_location

Deletes a source location.

Type annotations and code completion for `#!python session.create_client("mediatailor").delete_source_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_source_location)

```python
# delete_source_location method definition

await def delete_source_location(
    self,
    *,
    SourceLocationName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_source_location method usage example with argument unpacking

kwargs: DeleteSourceLocationRequestRequestTypeDef = {  # (1)
    "SourceLocationName": ...,
}

parent.delete_source_location(**kwargs)
```

1. See [:material-code-braces: DeleteSourceLocationRequestRequestTypeDef](./type_defs.md#deletesourcelocationrequestrequesttypedef) 

### delete\_vod\_source

The video on demand (VOD) source to delete.

Type annotations and code completion for `#!python session.create_client("mediatailor").delete_vod_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.delete_vod_source)

```python
# delete_vod_source method definition

await def delete_vod_source(
    self,
    *,
    SourceLocationName: str,
    VodSourceName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_vod_source method usage example with argument unpacking

kwargs: DeleteVodSourceRequestRequestTypeDef = {  # (1)
    "SourceLocationName": ...,
    "VodSourceName": ...,
}

parent.delete_vod_source(**kwargs)
```

1. See [:material-code-braces: DeleteVodSourceRequestRequestTypeDef](./type_defs.md#deletevodsourcerequestrequesttypedef) 

### describe\_channel

Describes a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").describe_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_channel)

```python
# describe_channel method definition

await def describe_channel(
    self,
    *,
    ChannelName: str,
) -> DescribeChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelResponseTypeDef](./type_defs.md#describechannelresponsetypedef) 


```python
# describe_channel method usage example with argument unpacking

kwargs: DescribeChannelRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.describe_channel(**kwargs)
```

1. See [:material-code-braces: DescribeChannelRequestRequestTypeDef](./type_defs.md#describechannelrequestrequesttypedef) 

### describe\_live\_source

The live source to describe.

Type annotations and code completion for `#!python session.create_client("mediatailor").describe_live_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_live_source)

```python
# describe_live_source method definition

await def describe_live_source(
    self,
    *,
    LiveSourceName: str,
    SourceLocationName: str,
) -> DescribeLiveSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLiveSourceResponseTypeDef](./type_defs.md#describelivesourceresponsetypedef) 


```python
# describe_live_source method usage example with argument unpacking

kwargs: DescribeLiveSourceRequestRequestTypeDef = {  # (1)
    "LiveSourceName": ...,
    "SourceLocationName": ...,
}

parent.describe_live_source(**kwargs)
```

1. See [:material-code-braces: DescribeLiveSourceRequestRequestTypeDef](./type_defs.md#describelivesourcerequestrequesttypedef) 

### describe\_program

Describes a program within a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").describe_program` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_program)

```python
# describe_program method definition

await def describe_program(
    self,
    *,
    ChannelName: str,
    ProgramName: str,
) -> DescribeProgramResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProgramResponseTypeDef](./type_defs.md#describeprogramresponsetypedef) 


```python
# describe_program method usage example with argument unpacking

kwargs: DescribeProgramRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
    "ProgramName": ...,
}

parent.describe_program(**kwargs)
```

1. See [:material-code-braces: DescribeProgramRequestRequestTypeDef](./type_defs.md#describeprogramrequestrequesttypedef) 

### describe\_source\_location

Describes a source location.

Type annotations and code completion for `#!python session.create_client("mediatailor").describe_source_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_source_location)

```python
# describe_source_location method definition

await def describe_source_location(
    self,
    *,
    SourceLocationName: str,
) -> DescribeSourceLocationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSourceLocationResponseTypeDef](./type_defs.md#describesourcelocationresponsetypedef) 


```python
# describe_source_location method usage example with argument unpacking

kwargs: DescribeSourceLocationRequestRequestTypeDef = {  # (1)
    "SourceLocationName": ...,
}

parent.describe_source_location(**kwargs)
```

1. See [:material-code-braces: DescribeSourceLocationRequestRequestTypeDef](./type_defs.md#describesourcelocationrequestrequesttypedef) 

### describe\_vod\_source

Provides details about a specific video on demand (VOD) source in a specific
source
location.

Type annotations and code completion for `#!python session.create_client("mediatailor").describe_vod_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.describe_vod_source)

```python
# describe_vod_source method definition

await def describe_vod_source(
    self,
    *,
    SourceLocationName: str,
    VodSourceName: str,
) -> DescribeVodSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVodSourceResponseTypeDef](./type_defs.md#describevodsourceresponsetypedef) 


```python
# describe_vod_source method usage example with argument unpacking

kwargs: DescribeVodSourceRequestRequestTypeDef = {  # (1)
    "SourceLocationName": ...,
    "VodSourceName": ...,
}

parent.describe_vod_source(**kwargs)
```

1. See [:material-code-braces: DescribeVodSourceRequestRequestTypeDef](./type_defs.md#describevodsourcerequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("mediatailor").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.generate_presigned_url)

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


### get\_channel\_policy

Returns the channel's IAM policy.

Type annotations and code completion for `#!python session.create_client("mediatailor").get_channel_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_policy)

```python
# get_channel_policy method definition

await def get_channel_policy(
    self,
    *,
    ChannelName: str,
) -> GetChannelPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelPolicyResponseTypeDef](./type_defs.md#getchannelpolicyresponsetypedef) 


```python
# get_channel_policy method usage example with argument unpacking

kwargs: GetChannelPolicyRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.get_channel_policy(**kwargs)
```

1. See [:material-code-braces: GetChannelPolicyRequestRequestTypeDef](./type_defs.md#getchannelpolicyrequestrequesttypedef) 

### get\_channel\_schedule

Retrieves information about your channel's schedule.

Type annotations and code completion for `#!python session.create_client("mediatailor").get_channel_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_channel_schedule)

```python
# get_channel_schedule method definition

await def get_channel_schedule(
    self,
    *,
    ChannelName: str,
    Audience: str = ...,
    DurationMinutes: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetChannelScheduleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelScheduleResponseTypeDef](./type_defs.md#getchannelscheduleresponsetypedef) 


```python
# get_channel_schedule method usage example with argument unpacking

kwargs: GetChannelScheduleRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.get_channel_schedule(**kwargs)
```

1. See [:material-code-braces: GetChannelScheduleRequestRequestTypeDef](./type_defs.md#getchannelschedulerequestrequesttypedef) 

### get\_playback\_configuration

Retrieves a playback configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").get_playback_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_playback_configuration)

```python
# get_playback_configuration method definition

await def get_playback_configuration(
    self,
    *,
    Name: str,
) -> GetPlaybackConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPlaybackConfigurationResponseTypeDef](./type_defs.md#getplaybackconfigurationresponsetypedef) 


```python
# get_playback_configuration method usage example with argument unpacking

kwargs: GetPlaybackConfigurationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_playback_configuration(**kwargs)
```

1. See [:material-code-braces: GetPlaybackConfigurationRequestRequestTypeDef](./type_defs.md#getplaybackconfigurationrequestrequesttypedef) 

### get\_prefetch\_schedule

Retrieves a prefetch schedule for a playback configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").get_prefetch_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.get_prefetch_schedule)

```python
# get_prefetch_schedule method definition

await def get_prefetch_schedule(
    self,
    *,
    Name: str,
    PlaybackConfigurationName: str,
) -> GetPrefetchScheduleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPrefetchScheduleResponseTypeDef](./type_defs.md#getprefetchscheduleresponsetypedef) 


```python
# get_prefetch_schedule method usage example with argument unpacking

kwargs: GetPrefetchScheduleRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "PlaybackConfigurationName": ...,
}

parent.get_prefetch_schedule(**kwargs)
```

1. See [:material-code-braces: GetPrefetchScheduleRequestRequestTypeDef](./type_defs.md#getprefetchschedulerequestrequesttypedef) 

### list\_alerts

Lists the alerts that are associated with a MediaTailor channel assembly
resource.

Type annotations and code completion for `#!python session.create_client("mediatailor").list_alerts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_alerts)

```python
# list_alerts method definition

await def list_alerts(
    self,
    *,
    ResourceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAlertsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAlertsResponseTypeDef](./type_defs.md#listalertsresponsetypedef) 


```python
# list_alerts method usage example with argument unpacking

kwargs: ListAlertsRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_alerts(**kwargs)
```

1. See [:material-code-braces: ListAlertsRequestRequestTypeDef](./type_defs.md#listalertsrequestrequesttypedef) 

### list\_channels

Retrieves information about the channels that are associated with the current
AWS
account.

Type annotations and code completion for `#!python session.create_client("mediatailor").list_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_channels)

```python
# list_channels method definition

await def list_channels(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# list_channels method usage example with argument unpacking

kwargs: ListChannelsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_channels(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef) 

### list\_live\_sources

Lists the live sources contained in a source location.

Type annotations and code completion for `#!python session.create_client("mediatailor").list_live_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_live_sources)

```python
# list_live_sources method definition

await def list_live_sources(
    self,
    *,
    SourceLocationName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListLiveSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLiveSourcesResponseTypeDef](./type_defs.md#listlivesourcesresponsetypedef) 


```python
# list_live_sources method usage example with argument unpacking

kwargs: ListLiveSourcesRequestRequestTypeDef = {  # (1)
    "SourceLocationName": ...,
}

parent.list_live_sources(**kwargs)
```

1. See [:material-code-braces: ListLiveSourcesRequestRequestTypeDef](./type_defs.md#listlivesourcesrequestrequesttypedef) 

### list\_playback\_configurations

Retrieves existing playback configurations.

Type annotations and code completion for `#!python session.create_client("mediatailor").list_playback_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_playback_configurations)

```python
# list_playback_configurations method definition

await def list_playback_configurations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPlaybackConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPlaybackConfigurationsResponseTypeDef](./type_defs.md#listplaybackconfigurationsresponsetypedef) 


```python
# list_playback_configurations method usage example with argument unpacking

kwargs: ListPlaybackConfigurationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_playback_configurations(**kwargs)
```

1. See [:material-code-braces: ListPlaybackConfigurationsRequestRequestTypeDef](./type_defs.md#listplaybackconfigurationsrequestrequesttypedef) 

### list\_prefetch\_schedules

Lists the prefetch schedules for a playback configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").list_prefetch_schedules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_prefetch_schedules)

```python
# list_prefetch_schedules method definition

await def list_prefetch_schedules(
    self,
    *,
    PlaybackConfigurationName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    StreamId: str = ...,
) -> ListPrefetchSchedulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPrefetchSchedulesResponseTypeDef](./type_defs.md#listprefetchschedulesresponsetypedef) 


```python
# list_prefetch_schedules method usage example with argument unpacking

kwargs: ListPrefetchSchedulesRequestRequestTypeDef = {  # (1)
    "PlaybackConfigurationName": ...,
}

parent.list_prefetch_schedules(**kwargs)
```

1. See [:material-code-braces: ListPrefetchSchedulesRequestRequestTypeDef](./type_defs.md#listprefetchschedulesrequestrequesttypedef) 

### list\_source\_locations

Lists the source locations for a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").list_source_locations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_source_locations)

```python
# list_source_locations method definition

await def list_source_locations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSourceLocationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSourceLocationsResponseTypeDef](./type_defs.md#listsourcelocationsresponsetypedef) 


```python
# list_source_locations method usage example with argument unpacking

kwargs: ListSourceLocationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_source_locations(**kwargs)
```

1. See [:material-code-braces: ListSourceLocationsRequestRequestTypeDef](./type_defs.md#listsourcelocationsrequestrequesttypedef) 

### list\_tags\_for\_resource

A list of tags that are associated with this resource.

Type annotations and code completion for `#!python session.create_client("mediatailor").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_vod\_sources

Lists the VOD sources contained in a source location.

Type annotations and code completion for `#!python session.create_client("mediatailor").list_vod_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.list_vod_sources)

```python
# list_vod_sources method definition

await def list_vod_sources(
    self,
    *,
    SourceLocationName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListVodSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVodSourcesResponseTypeDef](./type_defs.md#listvodsourcesresponsetypedef) 


```python
# list_vod_sources method usage example with argument unpacking

kwargs: ListVodSourcesRequestRequestTypeDef = {  # (1)
    "SourceLocationName": ...,
}

parent.list_vod_sources(**kwargs)
```

1. See [:material-code-braces: ListVodSourcesRequestRequestTypeDef](./type_defs.md#listvodsourcesrequestrequesttypedef) 

### put\_channel\_policy

Creates an IAM policy for the channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").put_channel_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.put_channel_policy)

```python
# put_channel_policy method definition

await def put_channel_policy(
    self,
    *,
    ChannelName: str,
    Policy: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_channel_policy method usage example with argument unpacking

kwargs: PutChannelPolicyRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
    "Policy": ...,
}

parent.put_channel_policy(**kwargs)
```

1. See [:material-code-braces: PutChannelPolicyRequestRequestTypeDef](./type_defs.md#putchannelpolicyrequestrequesttypedef) 

### put\_playback\_configuration

Creates a playback configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").put_playback_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.put_playback_configuration)

```python
# put_playback_configuration method definition

await def put_playback_configuration(
    self,
    *,
    Name: str,
    AdDecisionServerUrl: str = ...,
    AvailSuppression: AvailSuppressionTypeDef = ...,  # (1)
    Bumper: BumperTypeDef = ...,  # (2)
    CdnConfiguration: CdnConfigurationTypeDef = ...,  # (3)
    ConfigurationAliases: Mapping[str, Mapping[str, str]] = ...,
    DashConfiguration: DashConfigurationForPutTypeDef = ...,  # (4)
    InsertionMode: InsertionModeType = ...,  # (5)
    LivePreRollConfiguration: LivePreRollConfigurationTypeDef = ...,  # (6)
    ManifestProcessingRules: ManifestProcessingRulesTypeDef = ...,  # (7)
    PersonalizationThresholdSeconds: int = ...,
    SlateAdUrl: str = ...,
    Tags: Mapping[str, str] = ...,
    TranscodeProfileName: str = ...,
    VideoContentSourceUrl: str = ...,
) -> PutPlaybackConfigurationResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: AvailSuppressionTypeDef](./type_defs.md#availsuppressiontypedef) 
2. See [:material-code-braces: BumperTypeDef](./type_defs.md#bumpertypedef) 
3. See [:material-code-braces: CdnConfigurationTypeDef](./type_defs.md#cdnconfigurationtypedef) 
4. See [:material-code-braces: DashConfigurationForPutTypeDef](./type_defs.md#dashconfigurationforputtypedef) 
5. See [:material-code-brackets: InsertionModeType](./literals.md#insertionmodetype) 
6. See [:material-code-braces: LivePreRollConfigurationTypeDef](./type_defs.md#liveprerollconfigurationtypedef) 
7. See [:material-code-braces: ManifestProcessingRulesTypeDef](./type_defs.md#manifestprocessingrulestypedef) 
8. See [:material-code-braces: PutPlaybackConfigurationResponseTypeDef](./type_defs.md#putplaybackconfigurationresponsetypedef) 


```python
# put_playback_configuration method usage example with argument unpacking

kwargs: PutPlaybackConfigurationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.put_playback_configuration(**kwargs)
```

1. See [:material-code-braces: PutPlaybackConfigurationRequestRequestTypeDef](./type_defs.md#putplaybackconfigurationrequestrequesttypedef) 

### start\_channel

Starts a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").start_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.start_channel)

```python
# start_channel method definition

await def start_channel(
    self,
    *,
    ChannelName: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_channel method usage example with argument unpacking

kwargs: StartChannelRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.start_channel(**kwargs)
```

1. See [:material-code-braces: StartChannelRequestRequestTypeDef](./type_defs.md#startchannelrequestrequesttypedef) 

### stop\_channel

Stops a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").stop_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.stop_channel)

```python
# stop_channel method definition

await def stop_channel(
    self,
    *,
    ChannelName: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_channel method usage example with argument unpacking

kwargs: StopChannelRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
}

parent.stop_channel(**kwargs)
```

1. See [:material-code-braces: StopChannelRequestRequestTypeDef](./type_defs.md#stopchannelrequestrequesttypedef) 

### tag\_resource

The resource to tag.

Type annotations and code completion for `#!python session.create_client("mediatailor").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

The resource to untag.

Type annotations and code completion for `#!python session.create_client("mediatailor").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_channel

Updates a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").update_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_channel)

```python
# update_channel method definition

await def update_channel(
    self,
    *,
    ChannelName: str,
    Outputs: Sequence[RequestOutputItemTypeDef],  # (1)
    Audiences: Sequence[str] = ...,
    FillerSlate: SlateSourceTypeDef = ...,  # (2)
    TimeShiftConfiguration: TimeShiftConfigurationTypeDef = ...,  # (3)
) -> UpdateChannelResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RequestOutputItemTypeDef](./type_defs.md#requestoutputitemtypedef) 
2. See [:material-code-braces: SlateSourceTypeDef](./type_defs.md#slatesourcetypedef) 
3. See [:material-code-braces: TimeShiftConfigurationTypeDef](./type_defs.md#timeshiftconfigurationtypedef) 
4. See [:material-code-braces: UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef) 


```python
# update_channel method usage example with argument unpacking

kwargs: UpdateChannelRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
    "Outputs": ...,
}

parent.update_channel(**kwargs)
```

1. See [:material-code-braces: UpdateChannelRequestRequestTypeDef](./type_defs.md#updatechannelrequestrequesttypedef) 

### update\_live\_source

Updates a live source's configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").update_live_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_live_source)

```python
# update_live_source method definition

await def update_live_source(
    self,
    *,
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    LiveSourceName: str,
    SourceLocationName: str,
) -> UpdateLiveSourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
2. See [:material-code-braces: UpdateLiveSourceResponseTypeDef](./type_defs.md#updatelivesourceresponsetypedef) 


```python
# update_live_source method usage example with argument unpacking

kwargs: UpdateLiveSourceRequestRequestTypeDef = {  # (1)
    "HttpPackageConfigurations": ...,
    "LiveSourceName": ...,
    "SourceLocationName": ...,
}

parent.update_live_source(**kwargs)
```

1. See [:material-code-braces: UpdateLiveSourceRequestRequestTypeDef](./type_defs.md#updatelivesourcerequestrequesttypedef) 

### update\_program

Updates a program within a channel.

Type annotations and code completion for `#!python session.create_client("mediatailor").update_program` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)

```python
# update_program method definition

await def update_program(
    self,
    *,
    ChannelName: str,
    ProgramName: str,
    ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,  # (1)
    AdBreaks: Sequence[AdBreakTypeDef] = ...,  # (2)
    AudienceMedia: Sequence[AudienceMediaTypeDef] = ...,  # (3)
) -> UpdateProgramResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: UpdateProgramScheduleConfigurationTypeDef](./type_defs.md#updateprogramscheduleconfigurationtypedef) 
2. See [:material-code-braces: AdBreakTypeDef](./type_defs.md#adbreaktypedef) 
3. See [:material-code-braces: AudienceMediaTypeDef](./type_defs.md#audiencemediatypedef) 
4. See [:material-code-braces: UpdateProgramResponseTypeDef](./type_defs.md#updateprogramresponsetypedef) 


```python
# update_program method usage example with argument unpacking

kwargs: UpdateProgramRequestRequestTypeDef = {  # (1)
    "ChannelName": ...,
    "ProgramName": ...,
    "ScheduleConfiguration": ...,
}

parent.update_program(**kwargs)
```

1. See [:material-code-braces: UpdateProgramRequestRequestTypeDef](./type_defs.md#updateprogramrequestrequesttypedef) 

### update\_source\_location

Updates a source location.

Type annotations and code completion for `#!python session.create_client("mediatailor").update_source_location` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_source_location)

```python
# update_source_location method definition

await def update_source_location(
    self,
    *,
    HttpConfiguration: HttpConfigurationTypeDef,  # (1)
    SourceLocationName: str,
    AccessConfiguration: AccessConfigurationTypeDef = ...,  # (2)
    DefaultSegmentDeliveryConfiguration: DefaultSegmentDeliveryConfigurationTypeDef = ...,  # (3)
    SegmentDeliveryConfigurations: Sequence[SegmentDeliveryConfigurationTypeDef] = ...,  # (4)
) -> UpdateSourceLocationResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: HttpConfigurationTypeDef](./type_defs.md#httpconfigurationtypedef) 
2. See [:material-code-braces: AccessConfigurationTypeDef](./type_defs.md#accessconfigurationtypedef) 
3. See [:material-code-braces: DefaultSegmentDeliveryConfigurationTypeDef](./type_defs.md#defaultsegmentdeliveryconfigurationtypedef) 
4. See [:material-code-braces: SegmentDeliveryConfigurationTypeDef](./type_defs.md#segmentdeliveryconfigurationtypedef) 
5. See [:material-code-braces: UpdateSourceLocationResponseTypeDef](./type_defs.md#updatesourcelocationresponsetypedef) 


```python
# update_source_location method usage example with argument unpacking

kwargs: UpdateSourceLocationRequestRequestTypeDef = {  # (1)
    "HttpConfiguration": ...,
    "SourceLocationName": ...,
}

parent.update_source_location(**kwargs)
```

1. See [:material-code-braces: UpdateSourceLocationRequestRequestTypeDef](./type_defs.md#updatesourcelocationrequestrequesttypedef) 

### update\_vod\_source

Updates a VOD source's configuration.

Type annotations and code completion for `#!python session.create_client("mediatailor").update_vod_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_vod_source)

```python
# update_vod_source method definition

await def update_vod_source(
    self,
    *,
    HttpPackageConfigurations: Sequence[HttpPackageConfigurationTypeDef],  # (1)
    SourceLocationName: str,
    VodSourceName: str,
) -> UpdateVodSourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HttpPackageConfigurationTypeDef](./type_defs.md#httppackageconfigurationtypedef) 
2. See [:material-code-braces: UpdateVodSourceResponseTypeDef](./type_defs.md#updatevodsourceresponsetypedef) 


```python
# update_vod_source method usage example with argument unpacking

kwargs: UpdateVodSourceRequestRequestTypeDef = {  # (1)
    "HttpPackageConfigurations": ...,
    "SourceLocationName": ...,
    "VodSourceName": ...,
}

parent.update_vod_source(**kwargs)
```

1. See [:material-code-braces: UpdateVodSourceRequestRequestTypeDef](./type_defs.md#updatevodsourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("mediatailor").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "MediaTailorClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("mediatailor").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.__aexit__)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("mediatailor").get_paginator` method with overloads.

- `client.get_paginator("get_channel_schedule")` -> [GetChannelSchedulePaginator](./paginators.md#getchannelschedulepaginator)
- `client.get_paginator("list_alerts")` -> [ListAlertsPaginator](./paginators.md#listalertspaginator)
- `client.get_paginator("list_channels")` -> [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- `client.get_paginator("list_live_sources")` -> [ListLiveSourcesPaginator](./paginators.md#listlivesourcespaginator)
- `client.get_paginator("list_playback_configurations")` -> [ListPlaybackConfigurationsPaginator](./paginators.md#listplaybackconfigurationspaginator)
- `client.get_paginator("list_prefetch_schedules")` -> [ListPrefetchSchedulesPaginator](./paginators.md#listprefetchschedulespaginator)
- `client.get_paginator("list_source_locations")` -> [ListSourceLocationsPaginator](./paginators.md#listsourcelocationspaginator)
- `client.get_paginator("list_vod_sources")` -> [ListVodSourcesPaginator](./paginators.md#listvodsourcespaginator)



