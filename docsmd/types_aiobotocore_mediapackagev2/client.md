# Mediapackagev2Client

> [Index](../README.md) > [Mediapackagev2](./README.md) > Mediapackagev2Client

!!! note ""

    Auto-generated documentation for [Mediapackagev2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
    type annotations stubs module [types-aiobotocore-mediapackagev2](https://pypi.org/project/types-aiobotocore-mediapackagev2/).

## Mediapackagev2Client

Type annotations and code completion for `#!python session.create_client("mediapackagev2")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#Mediapackagev2.Client)

```python
# Mediapackagev2Client usage example

from aiobotocore.session import get_session
from types_aiobotocore_mediapackagev2.client import Mediapackagev2Client

session = get_session()
async with session.create_client("mediapackagev2") as client:
    client: Mediapackagev2Client
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("mediapackagev2").exceptions` structure.

```python
# Mediapackagev2Client.exceptions usage example

async with session.create_client("mediapackagev2") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# Mediapackagev2Client usage type checking example

from types_aiobotocore_mediapackagev2.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("mediapackagev2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("mediapackagev2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("mediapackagev2").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### cancel\_harvest\_job

Cancels an in-progress harvest job.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").cancel_harvest_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/cancel_harvest_job.html)

```python
# cancel_harvest_job method definition

await def cancel_harvest_job(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    HarvestJobName: str,
    ETag: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_harvest_job method usage example with argument unpacking

kwargs: CancelHarvestJobRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
    "HarvestJobName": ...,
}

parent.cancel_harvest_job(**kwargs)
```

1. See [:material-code-braces: CancelHarvestJobRequestRequestTypeDef](./type_defs.md#cancelharvestjobrequestrequesttypedef) 

### create\_channel

Create a channel to start receiving content streams.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").create_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/create_channel.html)

```python
# create_channel method definition

await def create_channel(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    ClientToken: str = ...,
    InputType: InputTypeType = ...,  # (1)
    Description: str = ...,
    InputSwitchConfiguration: InputSwitchConfigurationTypeDef = ...,  # (2)
    OutputHeaderConfiguration: OutputHeaderConfigurationTypeDef = ...,  # (3)
    Tags: Mapping[str, str] = ...,
) -> CreateChannelResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: InputTypeType](./literals.md#inputtypetype) 
2. See [:material-code-braces: InputSwitchConfigurationTypeDef](./type_defs.md#inputswitchconfigurationtypedef) 
3. See [:material-code-braces: OutputHeaderConfigurationTypeDef](./type_defs.md#outputheaderconfigurationtypedef) 
4. See [:material-code-braces: CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef) 


```python
# create_channel method usage example with argument unpacking

kwargs: CreateChannelRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.create_channel(**kwargs)
```

1. See [:material-code-braces: CreateChannelRequestRequestTypeDef](./type_defs.md#createchannelrequestrequesttypedef) 

### create\_channel\_group

Create a channel group to group your channels and origin endpoints.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").create_channel_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/create_channel_group.html)

```python
# create_channel_group method definition

await def create_channel_group(
    self,
    *,
    ChannelGroupName: str,
    ClientToken: str = ...,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateChannelGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateChannelGroupResponseTypeDef](./type_defs.md#createchannelgroupresponsetypedef) 


```python
# create_channel_group method usage example with argument unpacking

kwargs: CreateChannelGroupRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.create_channel_group(**kwargs)
```

1. See [:material-code-braces: CreateChannelGroupRequestRequestTypeDef](./type_defs.md#createchannelgrouprequestrequesttypedef) 

### create\_harvest\_job

Creates a new harvest job to export content from a MediaPackage v2 channel to
an S3 bucket.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").create_harvest_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/create_harvest_job.html)

```python
# create_harvest_job method definition

await def create_harvest_job(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    HarvestedManifests: HarvestedManifestsTypeDef,  # (1)
    ScheduleConfiguration: HarvesterScheduleConfigurationTypeDef,  # (2)
    Destination: DestinationTypeDef,  # (3)
    Description: str = ...,
    ClientToken: str = ...,
    HarvestJobName: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateHarvestJobResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: HarvestedManifestsTypeDef](./type_defs.md#harvestedmanifeststypedef) 
2. See [:material-code-braces: HarvesterScheduleConfigurationTypeDef](./type_defs.md#harvesterscheduleconfigurationtypedef) 
3. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
4. See [:material-code-braces: CreateHarvestJobResponseTypeDef](./type_defs.md#createharvestjobresponsetypedef) 


```python
# create_harvest_job method usage example with argument unpacking

kwargs: CreateHarvestJobRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
    "HarvestedManifests": ...,
    "ScheduleConfiguration": ...,
    "Destination": ...,
}

parent.create_harvest_job(**kwargs)
```

1. See [:material-code-braces: CreateHarvestJobRequestRequestTypeDef](./type_defs.md#createharvestjobrequestrequesttypedef) 

### create\_origin\_endpoint

The endpoint is attached to a channel, and represents the output of the live
content.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").create_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/create_origin_endpoint.html)

```python
# create_origin_endpoint method definition

await def create_origin_endpoint(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    ContainerType: ContainerTypeType,  # (1)
    Segment: SegmentTypeDef = ...,  # (2)
    ClientToken: str = ...,
    Description: str = ...,
    StartoverWindowSeconds: int = ...,
    HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,  # (3)
    LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,  # (4)
    DashManifests: Sequence[CreateDashManifestConfigurationTypeDef] = ...,  # (5)
    ForceEndpointErrorConfiguration: ForceEndpointErrorConfigurationTypeDef = ...,  # (6)
    Tags: Mapping[str, str] = ...,
) -> CreateOriginEndpointResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
3. See [:material-code-braces: CreateHlsManifestConfigurationTypeDef](./type_defs.md#createhlsmanifestconfigurationtypedef) 
4. See [:material-code-braces: CreateLowLatencyHlsManifestConfigurationTypeDef](./type_defs.md#createlowlatencyhlsmanifestconfigurationtypedef) 
5. See [:material-code-braces: CreateDashManifestConfigurationTypeDef](./type_defs.md#createdashmanifestconfigurationtypedef) 
6. See [:material-code-braces: ForceEndpointErrorConfigurationTypeDef](./type_defs.md#forceendpointerrorconfigurationtypedef) 
7. See [:material-code-braces: CreateOriginEndpointResponseTypeDef](./type_defs.md#createoriginendpointresponsetypedef) 


```python
# create_origin_endpoint method usage example with argument unpacking

kwargs: CreateOriginEndpointRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
    "ContainerType": ...,
}

parent.create_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateOriginEndpointRequestRequestTypeDef](./type_defs.md#createoriginendpointrequestrequesttypedef) 

### delete\_channel

Delete a channel to stop AWS Elemental MediaPackage from receiving further
content.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").delete_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/delete_channel.html)

```python
# delete_channel method definition

await def delete_channel(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_channel method usage example with argument unpacking

kwargs: DeleteChannelRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.delete_channel(**kwargs)
```

1. See [:material-code-braces: DeleteChannelRequestRequestTypeDef](./type_defs.md#deletechannelrequestrequesttypedef) 

### delete\_channel\_group

Delete a channel group.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").delete_channel_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/delete_channel_group.html)

```python
# delete_channel_group method definition

await def delete_channel_group(
    self,
    *,
    ChannelGroupName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_channel_group method usage example with argument unpacking

kwargs: DeleteChannelGroupRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.delete_channel_group(**kwargs)
```

1. See [:material-code-braces: DeleteChannelGroupRequestRequestTypeDef](./type_defs.md#deletechannelgrouprequestrequesttypedef) 

### delete\_channel\_policy

Delete a channel policy.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").delete_channel_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/delete_channel_policy.html)

```python
# delete_channel_policy method definition

await def delete_channel_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_channel_policy method usage example with argument unpacking

kwargs: DeleteChannelPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.delete_channel_policy(**kwargs)
```

1. See [:material-code-braces: DeleteChannelPolicyRequestRequestTypeDef](./type_defs.md#deletechannelpolicyrequestrequesttypedef) 

### delete\_origin\_endpoint

Origin endpoints can serve content until they're deleted.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").delete_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/delete_origin_endpoint.html)

```python
# delete_origin_endpoint method definition

await def delete_origin_endpoint(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_origin_endpoint method usage example with argument unpacking

kwargs: DeleteOriginEndpointRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
}

parent.delete_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteOriginEndpointRequestRequestTypeDef](./type_defs.md#deleteoriginendpointrequestrequesttypedef) 

### delete\_origin\_endpoint\_policy

Delete an origin endpoint policy.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").delete_origin_endpoint_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/delete_origin_endpoint_policy.html)

```python
# delete_origin_endpoint_policy method definition

await def delete_origin_endpoint_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_origin_endpoint_policy method usage example with argument unpacking

kwargs: DeleteOriginEndpointPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
}

parent.delete_origin_endpoint_policy(**kwargs)
```

1. See [:material-code-braces: DeleteOriginEndpointPolicyRequestRequestTypeDef](./type_defs.md#deleteoriginendpointpolicyrequestrequesttypedef) 

### get\_channel

Retrieves the specified channel that's configured in AWS Elemental
MediaPackage, including the origin endpoints that are associated with it.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/get_channel.html)

```python
# get_channel method definition

await def get_channel(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
) -> GetChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelResponseTypeDef](./type_defs.md#getchannelresponsetypedef) 


```python
# get_channel method usage example with argument unpacking

kwargs: GetChannelRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.get_channel(**kwargs)
```

1. See [:material-code-braces: GetChannelRequestRequestTypeDef](./type_defs.md#getchannelrequestrequesttypedef) 

### get\_channel\_group

Retrieves the specified channel group that's configured in AWS Elemental
MediaPackage, including the channels and origin endpoints that are associated
with it.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_channel_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/get_channel_group.html)

```python
# get_channel_group method definition

await def get_channel_group(
    self,
    *,
    ChannelGroupName: str,
) -> GetChannelGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelGroupResponseTypeDef](./type_defs.md#getchannelgroupresponsetypedef) 


```python
# get_channel_group method usage example with argument unpacking

kwargs: GetChannelGroupRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.get_channel_group(**kwargs)
```

1. See [:material-code-braces: GetChannelGroupRequestRequestTypeDef](./type_defs.md#getchannelgrouprequestrequesttypedef) 

### get\_channel\_policy

Retrieves the specified channel policy that's configured in AWS Elemental
MediaPackage.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_channel_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/get_channel_policy.html)

```python
# get_channel_policy method definition

await def get_channel_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
) -> GetChannelPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelPolicyResponseTypeDef](./type_defs.md#getchannelpolicyresponsetypedef) 


```python
# get_channel_policy method usage example with argument unpacking

kwargs: GetChannelPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.get_channel_policy(**kwargs)
```

1. See [:material-code-braces: GetChannelPolicyRequestRequestTypeDef](./type_defs.md#getchannelpolicyrequestrequesttypedef) 

### get\_harvest\_job

Retrieves the details of a specific harvest job.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_harvest_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/get_harvest_job.html)

```python
# get_harvest_job method definition

await def get_harvest_job(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    HarvestJobName: str,
) -> GetHarvestJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetHarvestJobResponseTypeDef](./type_defs.md#getharvestjobresponsetypedef) 


```python
# get_harvest_job method usage example with argument unpacking

kwargs: GetHarvestJobRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
    "HarvestJobName": ...,
}

parent.get_harvest_job(**kwargs)
```

1. See [:material-code-braces: GetHarvestJobRequestRequestTypeDef](./type_defs.md#getharvestjobrequestrequesttypedef) 

### get\_origin\_endpoint

Retrieves the specified origin endpoint that's configured in AWS Elemental
MediaPackage to obtain its playback URL and to view the packaging settings that
it's currently using.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/get_origin_endpoint.html)

```python
# get_origin_endpoint method definition

await def get_origin_endpoint(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
) -> GetOriginEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOriginEndpointResponseTypeDef](./type_defs.md#getoriginendpointresponsetypedef) 


```python
# get_origin_endpoint method usage example with argument unpacking

kwargs: GetOriginEndpointRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
}

parent.get_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: GetOriginEndpointRequestRequestTypeDef](./type_defs.md#getoriginendpointrequestrequesttypedef) 

### get\_origin\_endpoint\_policy

Retrieves the specified origin endpoint policy that's configured in AWS
Elemental MediaPackage.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_origin_endpoint_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/get_origin_endpoint_policy.html)

```python
# get_origin_endpoint_policy method definition

await def get_origin_endpoint_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
) -> GetOriginEndpointPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOriginEndpointPolicyResponseTypeDef](./type_defs.md#getoriginendpointpolicyresponsetypedef) 


```python
# get_origin_endpoint_policy method usage example with argument unpacking

kwargs: GetOriginEndpointPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
}

parent.get_origin_endpoint_policy(**kwargs)
```

1. See [:material-code-braces: GetOriginEndpointPolicyRequestRequestTypeDef](./type_defs.md#getoriginendpointpolicyrequestrequesttypedef) 

### list\_channel\_groups

Retrieves all channel groups that are configured in AWS Elemental MediaPackage,
including the channels and origin endpoints that are associated with it.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").list_channel_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/list_channel_groups.html)

```python
# list_channel_groups method definition

await def list_channel_groups(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListChannelGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelGroupsResponseTypeDef](./type_defs.md#listchannelgroupsresponsetypedef) 


```python
# list_channel_groups method usage example with argument unpacking

kwargs: ListChannelGroupsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_channel_groups(**kwargs)
```

1. See [:material-code-braces: ListChannelGroupsRequestRequestTypeDef](./type_defs.md#listchannelgroupsrequestrequesttypedef) 

### list\_channels

Retrieves all channels in a specific channel group that are configured in AWS
Elemental MediaPackage, including the origin endpoints that are associated with
it.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").list_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/list_channels.html)

```python
# list_channels method definition

await def list_channels(
    self,
    *,
    ChannelGroupName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# list_channels method usage example with argument unpacking

kwargs: ListChannelsRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.list_channels(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef) 

### list\_harvest\_jobs

Retrieves a list of harvest jobs that match the specified criteria.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").list_harvest_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/list_harvest_jobs.html)

```python
# list_harvest_jobs method definition

await def list_harvest_jobs(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str = ...,
    OriginEndpointName: str = ...,
    Status: HarvestJobStatusType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListHarvestJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: HarvestJobStatusType](./literals.md#harvestjobstatustype) 
2. See [:material-code-braces: ListHarvestJobsResponseTypeDef](./type_defs.md#listharvestjobsresponsetypedef) 


```python
# list_harvest_jobs method usage example with argument unpacking

kwargs: ListHarvestJobsRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.list_harvest_jobs(**kwargs)
```

1. See [:material-code-braces: ListHarvestJobsRequestRequestTypeDef](./type_defs.md#listharvestjobsrequestrequesttypedef) 

### list\_origin\_endpoints

Retrieves all origin endpoints in a specific channel that are configured in AWS
Elemental MediaPackage.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").list_origin_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/list_origin_endpoints.html)

```python
# list_origin_endpoints method definition

await def list_origin_endpoints(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListOriginEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOriginEndpointsResponseTypeDef](./type_defs.md#listoriginendpointsresponsetypedef) 


```python
# list_origin_endpoints method usage example with argument unpacking

kwargs: ListOriginEndpointsRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.list_origin_endpoints(**kwargs)
```

1. See [:material-code-braces: ListOriginEndpointsRequestRequestTypeDef](./type_defs.md#listoriginendpointsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags assigned to a resource.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/list_tags_for_resource.html)

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

### put\_channel\_policy

Attaches an IAM policy to the specified channel.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").put_channel_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/put_channel_policy.html)

```python
# put_channel_policy method definition

await def put_channel_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    Policy: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_channel_policy method usage example with argument unpacking

kwargs: PutChannelPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "Policy": ...,
}

parent.put_channel_policy(**kwargs)
```

1. See [:material-code-braces: PutChannelPolicyRequestRequestTypeDef](./type_defs.md#putchannelpolicyrequestrequesttypedef) 

### put\_origin\_endpoint\_policy

Attaches an IAM policy to the specified origin endpoint.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").put_origin_endpoint_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/put_origin_endpoint_policy.html)

```python
# put_origin_endpoint_policy method definition

await def put_origin_endpoint_policy(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    Policy: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_origin_endpoint_policy method usage example with argument unpacking

kwargs: PutOriginEndpointPolicyRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
    "Policy": ...,
}

parent.put_origin_endpoint_policy(**kwargs)
```

1. See [:material-code-braces: PutOriginEndpointPolicyRequestRequestTypeDef](./type_defs.md#putoriginendpointpolicyrequestrequesttypedef) 

### tag\_resource

Assigns one of more tags (key-value pairs) to the specified MediaPackage
resource.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/tag_resource.html)

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

Removes one or more tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/untag_resource.html)

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

Update the specified channel.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").update_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/update_channel.html)

```python
# update_channel method definition

await def update_channel(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    ETag: str = ...,
    Description: str = ...,
    InputSwitchConfiguration: InputSwitchConfigurationTypeDef = ...,  # (1)
    OutputHeaderConfiguration: OutputHeaderConfigurationTypeDef = ...,  # (2)
) -> UpdateChannelResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InputSwitchConfigurationTypeDef](./type_defs.md#inputswitchconfigurationtypedef) 
2. See [:material-code-braces: OutputHeaderConfigurationTypeDef](./type_defs.md#outputheaderconfigurationtypedef) 
3. See [:material-code-braces: UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef) 


```python
# update_channel method usage example with argument unpacking

kwargs: UpdateChannelRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.update_channel(**kwargs)
```

1. See [:material-code-braces: UpdateChannelRequestRequestTypeDef](./type_defs.md#updatechannelrequestrequesttypedef) 

### update\_channel\_group

Update the specified channel group.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").update_channel_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/update_channel_group.html)

```python
# update_channel_group method definition

await def update_channel_group(
    self,
    *,
    ChannelGroupName: str,
    ETag: str = ...,
    Description: str = ...,
) -> UpdateChannelGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateChannelGroupResponseTypeDef](./type_defs.md#updatechannelgroupresponsetypedef) 


```python
# update_channel_group method usage example with argument unpacking

kwargs: UpdateChannelGroupRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.update_channel_group(**kwargs)
```

1. See [:material-code-braces: UpdateChannelGroupRequestRequestTypeDef](./type_defs.md#updatechannelgrouprequestrequesttypedef) 

### update\_origin\_endpoint

Update the specified origin endpoint.

Type annotations and code completion for `#!python session.create_client("mediapackagev2").update_origin_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/client/update_origin_endpoint.html)

```python
# update_origin_endpoint method definition

await def update_origin_endpoint(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    ContainerType: ContainerTypeType,  # (1)
    Segment: SegmentTypeDef = ...,  # (2)
    Description: str = ...,
    StartoverWindowSeconds: int = ...,
    HlsManifests: Sequence[CreateHlsManifestConfigurationTypeDef] = ...,  # (3)
    LowLatencyHlsManifests: Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef] = ...,  # (4)
    DashManifests: Sequence[CreateDashManifestConfigurationTypeDef] = ...,  # (5)
    ForceEndpointErrorConfiguration: ForceEndpointErrorConfigurationTypeDef = ...,  # (6)
    ETag: str = ...,
) -> UpdateOriginEndpointResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
3. See [:material-code-braces: CreateHlsManifestConfigurationTypeDef](./type_defs.md#createhlsmanifestconfigurationtypedef) 
4. See [:material-code-braces: CreateLowLatencyHlsManifestConfigurationTypeDef](./type_defs.md#createlowlatencyhlsmanifestconfigurationtypedef) 
5. See [:material-code-braces: CreateDashManifestConfigurationTypeDef](./type_defs.md#createdashmanifestconfigurationtypedef) 
6. See [:material-code-braces: ForceEndpointErrorConfigurationTypeDef](./type_defs.md#forceendpointerrorconfigurationtypedef) 
7. See [:material-code-braces: UpdateOriginEndpointResponseTypeDef](./type_defs.md#updateoriginendpointresponsetypedef) 


```python
# update_origin_endpoint method usage example with argument unpacking

kwargs: UpdateOriginEndpointRequestRequestTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
    "OriginEndpointName": ...,
    "ContainerType": ...,
}

parent.update_origin_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateOriginEndpointRequestRequestTypeDef](./type_defs.md#updateoriginendpointrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("mediapackagev2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#Mediapackagev2.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "Mediapackagev2Client":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("mediapackagev2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#Mediapackagev2.Client)

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

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_paginator` method with overloads.

- `client.get_paginator("list_channel_groups")` -> [ListChannelGroupsPaginator](./paginators.md#listchannelgroupspaginator)
- `client.get_paginator("list_channels")` -> [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- `client.get_paginator("list_harvest_jobs")` -> [ListHarvestJobsPaginator](./paginators.md#listharvestjobspaginator)
- `client.get_paginator("list_origin_endpoints")` -> [ListOriginEndpointsPaginator](./paginators.md#listoriginendpointspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_waiter` method with overloads.

- `client.get_waiter("harvest_job_finished")` -> [HarvestJobFinishedWaiter](./waiters.md#harvestjobfinishedwaiter)

