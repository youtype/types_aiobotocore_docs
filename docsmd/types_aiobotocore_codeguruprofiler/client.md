# CodeGuruProfilerClient

> [Index](../README.md) > [CodeGuruProfiler](./README.md) > CodeGuruProfilerClient

!!! note ""

    Auto-generated documentation for [CodeGuruProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
    type annotations stubs module [types-aiobotocore-codeguruprofiler](https://pypi.org/project/types-aiobotocore-codeguruprofiler/).

## CodeGuruProfilerClient

Type annotations and code completion for `#!python session.create_client("codeguruprofiler")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client)

```python
# CodeGuruProfilerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_codeguruprofiler.client import CodeGuruProfilerClient

session = get_session()
async with session.create_client("codeguruprofiler") as client:
    client: CodeGuruProfilerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("codeguruprofiler").exceptions` structure.

```python
# CodeGuruProfilerClient.exceptions usage example

async with session.create_client("codeguruprofiler") as client:
    try:
        do_something(client)
    except (
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
# CodeGuruProfilerClient usage type checking example

from types_aiobotocore_codeguruprofiler.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### add\_notification\_channels

Add up to 2 anomaly notifications channels for a profiling group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").add_notification_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.add_notification_channels)

```python
# add_notification_channels method definition

await def add_notification_channels(
    self,
    *,
    channels: Sequence[ChannelUnionTypeDef],  # (1)
    profilingGroupName: str,
) -> AddNotificationChannelsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) [:material-code-braces: ChannelOutputTypeDef](./type_defs.md#channeloutputtypedef) 
2. See [:material-code-braces: AddNotificationChannelsResponseTypeDef](./type_defs.md#addnotificationchannelsresponsetypedef) 


```python
# add_notification_channels method usage example with argument unpacking

kwargs: AddNotificationChannelsRequestRequestTypeDef = {  # (1)
    "channels": ...,
    "profilingGroupName": ...,
}

parent.add_notification_channels(**kwargs)
```

1. See [:material-code-braces: AddNotificationChannelsRequestRequestTypeDef](./type_defs.md#addnotificationchannelsrequestrequesttypedef) 

### batch\_get\_frame\_metric\_data

Returns the time series of values for a requested list of frame metrics from a
time
period.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").batch_get_frame_metric_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.batch_get_frame_metric_data)

```python
# batch_get_frame_metric_data method definition

await def batch_get_frame_metric_data(
    self,
    *,
    profilingGroupName: str,
    endTime: TimestampTypeDef = ...,
    frameMetrics: Sequence[FrameMetricUnionTypeDef] = ...,  # (1)
    period: str = ...,
    startTime: TimestampTypeDef = ...,
    targetResolution: AggregationPeriodType = ...,  # (2)
) -> BatchGetFrameMetricDataResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FrameMetricTypeDef](./type_defs.md#framemetrictypedef) [:material-code-braces: FrameMetricOutputTypeDef](./type_defs.md#framemetricoutputtypedef) 
2. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
3. See [:material-code-braces: BatchGetFrameMetricDataResponseTypeDef](./type_defs.md#batchgetframemetricdataresponsetypedef) 


```python
# batch_get_frame_metric_data method usage example with argument unpacking

kwargs: BatchGetFrameMetricDataRequestRequestTypeDef = {  # (1)
    "profilingGroupName": ...,
}

parent.batch_get_frame_metric_data(**kwargs)
```

1. See [:material-code-braces: BatchGetFrameMetricDataRequestRequestTypeDef](./type_defs.md#batchgetframemetricdatarequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### configure\_agent

Used by profiler agents to report their current state and to receive remote
configuration
updates.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").configure_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.configure_agent)

```python
# configure_agent method definition

await def configure_agent(
    self,
    *,
    profilingGroupName: str,
    fleetInstanceId: str = ...,
    metadata: Mapping[MetadataFieldType, str] = ...,  # (1)
) -> ConfigureAgentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MetadataFieldType](./literals.md#metadatafieldtype) 
2. See [:material-code-braces: ConfigureAgentResponseTypeDef](./type_defs.md#configureagentresponsetypedef) 


```python
# configure_agent method usage example with argument unpacking

kwargs: ConfigureAgentRequestRequestTypeDef = {  # (1)
    "profilingGroupName": ...,
}

parent.configure_agent(**kwargs)
```

1. See [:material-code-braces: ConfigureAgentRequestRequestTypeDef](./type_defs.md#configureagentrequestrequesttypedef) 

### create\_profiling\_group

Creates a profiling group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").create_profiling_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.create_profiling_group)

```python
# create_profiling_group method definition

await def create_profiling_group(
    self,
    *,
    clientToken: str,
    profilingGroupName: str,
    agentOrchestrationConfig: AgentOrchestrationConfigTypeDef = ...,  # (1)
    computePlatform: ComputePlatformType = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> CreateProfilingGroupResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AgentOrchestrationConfigTypeDef](./type_defs.md#agentorchestrationconfigtypedef) 
2. See [:material-code-brackets: ComputePlatformType](./literals.md#computeplatformtype) 
3. See [:material-code-braces: CreateProfilingGroupResponseTypeDef](./type_defs.md#createprofilinggroupresponsetypedef) 


```python
# create_profiling_group method usage example with argument unpacking

kwargs: CreateProfilingGroupRequestRequestTypeDef = {  # (1)
    "clientToken": ...,
    "profilingGroupName": ...,
}

parent.create_profiling_group(**kwargs)
```

1. See [:material-code-braces: CreateProfilingGroupRequestRequestTypeDef](./type_defs.md#createprofilinggrouprequestrequesttypedef) 

### delete\_profiling\_group

Deletes a profiling group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").delete_profiling_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.delete_profiling_group)

```python
# delete_profiling_group method definition

await def delete_profiling_group(
    self,
    *,
    profilingGroupName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_profiling_group method usage example with argument unpacking

kwargs: DeleteProfilingGroupRequestRequestTypeDef = {  # (1)
    "profilingGroupName": ...,
}

parent.delete_profiling_group(**kwargs)
```

1. See [:material-code-braces: DeleteProfilingGroupRequestRequestTypeDef](./type_defs.md#deleteprofilinggrouprequestrequesttypedef) 

### describe\_profiling\_group

Returns a
[ProfilingGroupDescription](https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ProfilingGroupDescription.html)
object that contains information about the requested profiling
group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").describe_profiling_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.describe_profiling_group)

```python
# describe_profiling_group method definition

await def describe_profiling_group(
    self,
    *,
    profilingGroupName: str,
) -> DescribeProfilingGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProfilingGroupResponseTypeDef](./type_defs.md#describeprofilinggroupresponsetypedef) 


```python
# describe_profiling_group method usage example with argument unpacking

kwargs: DescribeProfilingGroupRequestRequestTypeDef = {  # (1)
    "profilingGroupName": ...,
}

parent.describe_profiling_group(**kwargs)
```

1. See [:material-code-braces: DescribeProfilingGroupRequestRequestTypeDef](./type_defs.md#describeprofilinggrouprequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.generate_presigned_url)

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


### get\_findings\_report\_account\_summary

Returns a list of
[FindingsReportSummary](https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_FindingsReportSummary.html)
objects that contain analysis results for all profiling groups in your AWS
account.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").get_findings_report_account_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_findings_report_account_summary)

```python
# get_findings_report_account_summary method definition

await def get_findings_report_account_summary(
    self,
    *,
    dailyReportsOnly: bool = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> GetFindingsReportAccountSummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFindingsReportAccountSummaryResponseTypeDef](./type_defs.md#getfindingsreportaccountsummaryresponsetypedef) 


```python
# get_findings_report_account_summary method usage example with argument unpacking

kwargs: GetFindingsReportAccountSummaryRequestRequestTypeDef = {  # (1)
    "dailyReportsOnly": ...,
}

parent.get_findings_report_account_summary(**kwargs)
```

1. See [:material-code-braces: GetFindingsReportAccountSummaryRequestRequestTypeDef](./type_defs.md#getfindingsreportaccountsummaryrequestrequesttypedef) 

### get\_notification\_configuration

Get the current configuration for anomaly notifications for a profiling group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").get_notification_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_notification_configuration)

```python
# get_notification_configuration method definition

await def get_notification_configuration(
    self,
    *,
    profilingGroupName: str,
) -> GetNotificationConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNotificationConfigurationResponseTypeDef](./type_defs.md#getnotificationconfigurationresponsetypedef) 


```python
# get_notification_configuration method usage example with argument unpacking

kwargs: GetNotificationConfigurationRequestRequestTypeDef = {  # (1)
    "profilingGroupName": ...,
}

parent.get_notification_configuration(**kwargs)
```

1. See [:material-code-braces: GetNotificationConfigurationRequestRequestTypeDef](./type_defs.md#getnotificationconfigurationrequestrequesttypedef) 

### get\_policy

Returns the JSON-formatted resource-based policy on a profiling group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").get_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_policy)

```python
# get_policy method definition

await def get_policy(
    self,
    *,
    profilingGroupName: str,
) -> GetPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef) 


```python
# get_policy method usage example with argument unpacking

kwargs: GetPolicyRequestRequestTypeDef = {  # (1)
    "profilingGroupName": ...,
}

parent.get_policy(**kwargs)
```

1. See [:material-code-braces: GetPolicyRequestRequestTypeDef](./type_defs.md#getpolicyrequestrequesttypedef) 

### get\_profile

Gets the aggregated profile of a profiling group for a specified time range.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").get_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_profile)

```python
# get_profile method definition

await def get_profile(
    self,
    *,
    profilingGroupName: str,
    accept: str = ...,
    endTime: TimestampTypeDef = ...,
    maxDepth: int = ...,
    period: str = ...,
    startTime: TimestampTypeDef = ...,
) -> GetProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProfileResponseTypeDef](./type_defs.md#getprofileresponsetypedef) 


```python
# get_profile method usage example with argument unpacking

kwargs: GetProfileRequestRequestTypeDef = {  # (1)
    "profilingGroupName": ...,
}

parent.get_profile(**kwargs)
```

1. See [:material-code-braces: GetProfileRequestRequestTypeDef](./type_defs.md#getprofilerequestrequesttypedef) 

### get\_recommendations

Returns a list of
[Recommendation](https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_Recommendation.html)
objects that contain recommendations for a profiling group for a given time
period.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").get_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.get_recommendations)

```python
# get_recommendations method definition

await def get_recommendations(
    self,
    *,
    endTime: TimestampTypeDef,
    profilingGroupName: str,
    startTime: TimestampTypeDef,
    locale: str = ...,
) -> GetRecommendationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRecommendationsResponseTypeDef](./type_defs.md#getrecommendationsresponsetypedef) 


```python
# get_recommendations method usage example with argument unpacking

kwargs: GetRecommendationsRequestRequestTypeDef = {  # (1)
    "endTime": ...,
    "profilingGroupName": ...,
    "startTime": ...,
}

parent.get_recommendations(**kwargs)
```

1. See [:material-code-braces: GetRecommendationsRequestRequestTypeDef](./type_defs.md#getrecommendationsrequestrequesttypedef) 

### list\_findings\_reports

List the available reports for a given profiling group and time range.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").list_findings_reports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_findings_reports)

```python
# list_findings_reports method definition

await def list_findings_reports(
    self,
    *,
    endTime: TimestampTypeDef,
    profilingGroupName: str,
    startTime: TimestampTypeDef,
    dailyReportsOnly: bool = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListFindingsReportsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFindingsReportsResponseTypeDef](./type_defs.md#listfindingsreportsresponsetypedef) 


```python
# list_findings_reports method usage example with argument unpacking

kwargs: ListFindingsReportsRequestRequestTypeDef = {  # (1)
    "endTime": ...,
    "profilingGroupName": ...,
    "startTime": ...,
}

parent.list_findings_reports(**kwargs)
```

1. See [:material-code-braces: ListFindingsReportsRequestRequestTypeDef](./type_defs.md#listfindingsreportsrequestrequesttypedef) 

### list\_profile\_times

Lists the start times of the available aggregated profiles of a profiling group
for an aggregation period within the specified time
range.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").list_profile_times` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profile_times)

```python
# list_profile_times method definition

await def list_profile_times(
    self,
    *,
    endTime: TimestampTypeDef,
    period: AggregationPeriodType,  # (1)
    profilingGroupName: str,
    startTime: TimestampTypeDef,
    maxResults: int = ...,
    nextToken: str = ...,
    orderBy: OrderByType = ...,  # (2)
) -> ListProfileTimesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
2. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
3. See [:material-code-braces: ListProfileTimesResponseTypeDef](./type_defs.md#listprofiletimesresponsetypedef) 


```python
# list_profile_times method usage example with argument unpacking

kwargs: ListProfileTimesRequestRequestTypeDef = {  # (1)
    "endTime": ...,
    "period": ...,
    "profilingGroupName": ...,
    "startTime": ...,
}

parent.list_profile_times(**kwargs)
```

1. See [:material-code-braces: ListProfileTimesRequestRequestTypeDef](./type_defs.md#listprofiletimesrequestrequesttypedef) 

### list\_profiling\_groups

Returns a list of profiling groups.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").list_profiling_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_profiling_groups)

```python
# list_profiling_groups method definition

await def list_profiling_groups(
    self,
    *,
    includeDescription: bool = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListProfilingGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProfilingGroupsResponseTypeDef](./type_defs.md#listprofilinggroupsresponsetypedef) 


```python
# list_profiling_groups method usage example with argument unpacking

kwargs: ListProfilingGroupsRequestRequestTypeDef = {  # (1)
    "includeDescription": ...,
}

parent.list_profiling_groups(**kwargs)
```

1. See [:material-code-braces: ListProfilingGroupsRequestRequestTypeDef](./type_defs.md#listprofilinggroupsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of the tags that are assigned to a specified resource.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.list_tags_for_resource)

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

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### post\_agent\_profile

Submits profiling data to an aggregated profile of a profiling group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").post_agent_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.post_agent_profile)

```python
# post_agent_profile method definition

await def post_agent_profile(
    self,
    *,
    agentProfile: BlobTypeDef,
    contentType: str,
    profilingGroupName: str,
    profileToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# post_agent_profile method usage example with argument unpacking

kwargs: PostAgentProfileRequestRequestTypeDef = {  # (1)
    "agentProfile": ...,
    "contentType": ...,
    "profilingGroupName": ...,
}

parent.post_agent_profile(**kwargs)
```

1. See [:material-code-braces: PostAgentProfileRequestRequestTypeDef](./type_defs.md#postagentprofilerequestrequesttypedef) 

### put\_permission

Adds permissions to a profiling group's resource-based policy that are provided
using an action
group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").put_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.put_permission)

```python
# put_permission method definition

await def put_permission(
    self,
    *,
    actionGroup: ActionGroupType,  # (1)
    principals: Sequence[str],
    profilingGroupName: str,
    revisionId: str = ...,
) -> PutPermissionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ActionGroupType](./literals.md#actiongrouptype) 
2. See [:material-code-braces: PutPermissionResponseTypeDef](./type_defs.md#putpermissionresponsetypedef) 


```python
# put_permission method usage example with argument unpacking

kwargs: PutPermissionRequestRequestTypeDef = {  # (1)
    "actionGroup": ...,
    "principals": ...,
    "profilingGroupName": ...,
}

parent.put_permission(**kwargs)
```

1. See [:material-code-braces: PutPermissionRequestRequestTypeDef](./type_defs.md#putpermissionrequestrequesttypedef) 

### remove\_notification\_channel

Remove one anomaly notifications channel for a profiling group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").remove_notification_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.remove_notification_channel)

```python
# remove_notification_channel method definition

await def remove_notification_channel(
    self,
    *,
    channelId: str,
    profilingGroupName: str,
) -> RemoveNotificationChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveNotificationChannelResponseTypeDef](./type_defs.md#removenotificationchannelresponsetypedef) 


```python
# remove_notification_channel method usage example with argument unpacking

kwargs: RemoveNotificationChannelRequestRequestTypeDef = {  # (1)
    "channelId": ...,
    "profilingGroupName": ...,
}

parent.remove_notification_channel(**kwargs)
```

1. See [:material-code-braces: RemoveNotificationChannelRequestRequestTypeDef](./type_defs.md#removenotificationchannelrequestrequesttypedef) 

### remove\_permission

Removes permissions from a profiling group's resource-based policy that are
provided using an action
group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").remove_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.remove_permission)

```python
# remove_permission method definition

await def remove_permission(
    self,
    *,
    actionGroup: ActionGroupType,  # (1)
    profilingGroupName: str,
    revisionId: str,
) -> RemovePermissionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ActionGroupType](./literals.md#actiongrouptype) 
2. See [:material-code-braces: RemovePermissionResponseTypeDef](./type_defs.md#removepermissionresponsetypedef) 


```python
# remove_permission method usage example with argument unpacking

kwargs: RemovePermissionRequestRequestTypeDef = {  # (1)
    "actionGroup": ...,
    "profilingGroupName": ...,
    "revisionId": ...,
}

parent.remove_permission(**kwargs)
```

1. See [:material-code-braces: RemovePermissionRequestRequestTypeDef](./type_defs.md#removepermissionrequestrequesttypedef) 

### submit\_feedback

Sends feedback to CodeGuru Profiler about whether the anomaly detected by the
analysis is useful or
not.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").submit_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.submit_feedback)

```python
# submit_feedback method definition

await def submit_feedback(
    self,
    *,
    anomalyInstanceId: str,
    profilingGroupName: str,
    type: FeedbackTypeType,  # (1)
    comment: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: FeedbackTypeType](./literals.md#feedbacktypetype) 


```python
# submit_feedback method usage example with argument unpacking

kwargs: SubmitFeedbackRequestRequestTypeDef = {  # (1)
    "anomalyInstanceId": ...,
    "profilingGroupName": ...,
    "type": ...,
}

parent.submit_feedback(**kwargs)
```

1. See [:material-code-braces: SubmitFeedbackRequestRequestTypeDef](./type_defs.md#submitfeedbackrequestrequesttypedef) 

### tag\_resource

Use to assign one or more tags to a resource.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.tag_resource)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Use to remove one or more tags from a resource.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.untag_resource)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_profiling\_group

Updates a profiling group.

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").update_profiling_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.update_profiling_group)

```python
# update_profiling_group method definition

await def update_profiling_group(
    self,
    *,
    agentOrchestrationConfig: AgentOrchestrationConfigTypeDef,  # (1)
    profilingGroupName: str,
) -> UpdateProfilingGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AgentOrchestrationConfigTypeDef](./type_defs.md#agentorchestrationconfigtypedef) 
2. See [:material-code-braces: UpdateProfilingGroupResponseTypeDef](./type_defs.md#updateprofilinggroupresponsetypedef) 


```python
# update_profiling_group method usage example with argument unpacking

kwargs: UpdateProfilingGroupRequestRequestTypeDef = {  # (1)
    "agentOrchestrationConfig": ...,
    "profilingGroupName": ...,
}

parent.update_profiling_group(**kwargs)
```

1. See [:material-code-braces: UpdateProfilingGroupRequestRequestTypeDef](./type_defs.md#updateprofilinggrouprequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("codeguruprofiler").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CodeGuruProfilerClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("codeguruprofiler").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("codeguruprofiler").get_paginator` method with overloads.

- `client.get_paginator("list_profile_times")` -> [ListProfileTimesPaginator](./paginators.md#listprofiletimespaginator)



