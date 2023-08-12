# Type definitions

> [Index](../README.md) > [CodeGuruProfiler](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeGuruProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#CodeGuruProfiler)
    type annotations stubs module [types-aiobotocore-codeguruprofiler](https://pypi.org/project/types-aiobotocore-codeguruprofiler/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## ChannelTypeDef

```python
# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    eventPublishers: Sequence[EventPublisherType],  # (1)
    uri: str,
    id: NotRequired[str],
```

1. See [:material-code-brackets: EventPublisherType](./literals.md#eventpublishertype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## AgentConfigurationTypeDef

```python
# AgentConfigurationTypeDef definition

class AgentConfigurationTypeDef(TypedDict):
    periodInSeconds: int,
    shouldProfile: bool,
    agentParameters: NotRequired[Dict[AgentParameterFieldType, str]],  # (1)
```

1. See [:material-code-brackets: AgentParameterFieldType](./literals.md#agentparameterfieldtype) 
## AgentOrchestrationConfigTypeDef

```python
# AgentOrchestrationConfigTypeDef definition

class AgentOrchestrationConfigTypeDef(TypedDict):
    profilingEnabled: bool,
```

## AggregatedProfileTimeTypeDef

```python
# AggregatedProfileTimeTypeDef definition

class AggregatedProfileTimeTypeDef(TypedDict):
    period: NotRequired[AggregationPeriodType],  # (1)
    start: NotRequired[datetime],
```

1. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
## UserFeedbackTypeDef

```python
# UserFeedbackTypeDef definition

class UserFeedbackTypeDef(TypedDict):
    type: FeedbackTypeType,  # (1)
```

1. See [:material-code-brackets: FeedbackTypeType](./literals.md#feedbacktypetype) 
## MetricTypeDef

```python
# MetricTypeDef definition

class MetricTypeDef(TypedDict):
    frameName: str,
    threadStates: List[str],
    type: MetricTypeType,  # (1)
```

1. See [:material-code-brackets: MetricTypeType](./literals.md#metrictypetype) 
## FrameMetricTypeDef

```python
# FrameMetricTypeDef definition

class FrameMetricTypeDef(TypedDict):
    frameName: str,
    threadStates: Sequence[str],
    type: MetricTypeType,  # (1)
```

1. See [:material-code-brackets: MetricTypeType](./literals.md#metrictypetype) 
## TimestampStructureTypeDef

```python
# TimestampStructureTypeDef definition

class TimestampStructureTypeDef(TypedDict):
    value: datetime,
```

## ConfigureAgentRequestRequestTypeDef

```python
# ConfigureAgentRequestRequestTypeDef definition

class ConfigureAgentRequestRequestTypeDef(TypedDict):
    profilingGroupName: str,
    fleetInstanceId: NotRequired[str],
    metadata: NotRequired[Mapping[MetadataFieldType, str]],  # (1)
```

1. See [:material-code-brackets: MetadataFieldType](./literals.md#metadatafieldtype) 
## DeleteProfilingGroupRequestRequestTypeDef

```python
# DeleteProfilingGroupRequestRequestTypeDef definition

class DeleteProfilingGroupRequestRequestTypeDef(TypedDict):
    profilingGroupName: str,
```

## DescribeProfilingGroupRequestRequestTypeDef

```python
# DescribeProfilingGroupRequestRequestTypeDef definition

class DescribeProfilingGroupRequestRequestTypeDef(TypedDict):
    profilingGroupName: str,
```

## FindingsReportSummaryTypeDef

```python
# FindingsReportSummaryTypeDef definition

class FindingsReportSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    profileEndTime: NotRequired[datetime],
    profileStartTime: NotRequired[datetime],
    profilingGroupName: NotRequired[str],
    totalNumberOfFindings: NotRequired[int],
```

## GetFindingsReportAccountSummaryRequestRequestTypeDef

```python
# GetFindingsReportAccountSummaryRequestRequestTypeDef definition

class GetFindingsReportAccountSummaryRequestRequestTypeDef(TypedDict):
    dailyReportsOnly: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetNotificationConfigurationRequestRequestTypeDef

```python
# GetNotificationConfigurationRequestRequestTypeDef definition

class GetNotificationConfigurationRequestRequestTypeDef(TypedDict):
    profilingGroupName: str,
```

## GetPolicyRequestRequestTypeDef

```python
# GetPolicyRequestRequestTypeDef definition

class GetPolicyRequestRequestTypeDef(TypedDict):
    profilingGroupName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ProfileTimeTypeDef

```python
# ProfileTimeTypeDef definition

class ProfileTimeTypeDef(TypedDict):
    start: NotRequired[datetime],
```

## ListProfilingGroupsRequestRequestTypeDef

```python
# ListProfilingGroupsRequestRequestTypeDef definition

class ListProfilingGroupsRequestRequestTypeDef(TypedDict):
    includeDescription: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## MatchTypeDef

```python
# MatchTypeDef definition

class MatchTypeDef(TypedDict):
    frameAddress: NotRequired[str],
    targetFramesIndex: NotRequired[int],
    thresholdBreachValue: NotRequired[float],
```

## PatternTypeDef

```python
# PatternTypeDef definition

class PatternTypeDef(TypedDict):
    countersToAggregate: NotRequired[List[str]],
    description: NotRequired[str],
    id: NotRequired[str],
    name: NotRequired[str],
    resolutionSteps: NotRequired[str],
    targetFrames: NotRequired[List[List[str]]],
    thresholdPercent: NotRequired[float],
```

## PutPermissionRequestRequestTypeDef

```python
# PutPermissionRequestRequestTypeDef definition

class PutPermissionRequestRequestTypeDef(TypedDict):
    actionGroup: ActionGroupType,  # (1)
    principals: Sequence[str],
    profilingGroupName: str,
    revisionId: NotRequired[str],
```

1. See [:material-code-brackets: ActionGroupType](./literals.md#actiongrouptype) 
## RemoveNotificationChannelRequestRequestTypeDef

```python
# RemoveNotificationChannelRequestRequestTypeDef definition

class RemoveNotificationChannelRequestRequestTypeDef(TypedDict):
    channelId: str,
    profilingGroupName: str,
```

## RemovePermissionRequestRequestTypeDef

```python
# RemovePermissionRequestRequestTypeDef definition

class RemovePermissionRequestRequestTypeDef(TypedDict):
    actionGroup: ActionGroupType,  # (1)
    profilingGroupName: str,
    revisionId: str,
```

1. See [:material-code-brackets: ActionGroupType](./literals.md#actiongrouptype) 
## SubmitFeedbackRequestRequestTypeDef

```python
# SubmitFeedbackRequestRequestTypeDef definition

class SubmitFeedbackRequestRequestTypeDef(TypedDict):
    anomalyInstanceId: str,
    profilingGroupName: str,
    type: FeedbackTypeType,  # (1)
    comment: NotRequired[str],
```

1. See [:material-code-brackets: FeedbackTypeType](./literals.md#feedbacktypetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AddNotificationChannelsRequestRequestTypeDef

```python
# AddNotificationChannelsRequestRequestTypeDef definition

class AddNotificationChannelsRequestRequestTypeDef(TypedDict):
    channels: Sequence[ChannelTypeDef],  # (1)
    profilingGroupName: str,
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    channels: NotRequired[List[ChannelTypeDef]],  # (1)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
## GetPolicyResponseTypeDef

```python
# GetPolicyResponseTypeDef definition

class GetPolicyResponseTypeDef(TypedDict):
    policy: str,
    revisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProfileResponseTypeDef

```python
# GetProfileResponseTypeDef definition

class GetProfileResponseTypeDef(TypedDict):
    contentEncoding: str,
    contentType: str,
    profile: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPermissionResponseTypeDef

```python
# PutPermissionResponseTypeDef definition

class PutPermissionResponseTypeDef(TypedDict):
    policy: str,
    revisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemovePermissionResponseTypeDef

```python
# RemovePermissionResponseTypeDef definition

class RemovePermissionResponseTypeDef(TypedDict):
    policy: str,
    revisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigureAgentResponseTypeDef

```python
# ConfigureAgentResponseTypeDef definition

class ConfigureAgentResponseTypeDef(TypedDict):
    configuration: AgentConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentConfigurationTypeDef](./type_defs.md#agentconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProfilingGroupRequestRequestTypeDef

```python
# CreateProfilingGroupRequestRequestTypeDef definition

class CreateProfilingGroupRequestRequestTypeDef(TypedDict):
    clientToken: str,
    profilingGroupName: str,
    agentOrchestrationConfig: NotRequired[AgentOrchestrationConfigTypeDef],  # (1)
    computePlatform: NotRequired[ComputePlatformType],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AgentOrchestrationConfigTypeDef](./type_defs.md#agentorchestrationconfigtypedef) 
2. See [:material-code-brackets: ComputePlatformType](./literals.md#computeplatformtype) 
## UpdateProfilingGroupRequestRequestTypeDef

```python
# UpdateProfilingGroupRequestRequestTypeDef definition

class UpdateProfilingGroupRequestRequestTypeDef(TypedDict):
    agentOrchestrationConfig: AgentOrchestrationConfigTypeDef,  # (1)
    profilingGroupName: str,
```

1. See [:material-code-braces: AgentOrchestrationConfigTypeDef](./type_defs.md#agentorchestrationconfigtypedef) 
## ProfilingStatusTypeDef

```python
# ProfilingStatusTypeDef definition

class ProfilingStatusTypeDef(TypedDict):
    latestAgentOrchestratedAt: NotRequired[datetime],
    latestAgentProfileReportedAt: NotRequired[datetime],
    latestAggregatedProfile: NotRequired[AggregatedProfileTimeTypeDef],  # (1)
```

1. See [:material-code-braces: AggregatedProfileTimeTypeDef](./type_defs.md#aggregatedprofiletimetypedef) 
## AnomalyInstanceTypeDef

```python
# AnomalyInstanceTypeDef definition

class AnomalyInstanceTypeDef(TypedDict):
    id: str,
    startTime: datetime,
    endTime: NotRequired[datetime],
    userFeedback: NotRequired[UserFeedbackTypeDef],  # (1)
```

1. See [:material-code-braces: UserFeedbackTypeDef](./type_defs.md#userfeedbacktypedef) 
## FrameMetricDatumTypeDef

```python
# FrameMetricDatumTypeDef definition

class FrameMetricDatumTypeDef(TypedDict):
    frameMetric: FrameMetricTypeDef,  # (1)
    values: List[float],
```

1. See [:material-code-braces: FrameMetricTypeDef](./type_defs.md#framemetrictypedef) 
## BatchGetFrameMetricDataRequestRequestTypeDef

```python
# BatchGetFrameMetricDataRequestRequestTypeDef definition

class BatchGetFrameMetricDataRequestRequestTypeDef(TypedDict):
    profilingGroupName: str,
    endTime: NotRequired[Union[datetime, str]],
    frameMetrics: NotRequired[Sequence[FrameMetricTypeDef]],  # (1)
    period: NotRequired[str],
    startTime: NotRequired[Union[datetime, str]],
    targetResolution: NotRequired[AggregationPeriodType],  # (2)
```

1. See [:material-code-braces: FrameMetricTypeDef](./type_defs.md#framemetrictypedef) 
2. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
## GetProfileRequestRequestTypeDef

```python
# GetProfileRequestRequestTypeDef definition

class GetProfileRequestRequestTypeDef(TypedDict):
    profilingGroupName: str,
    accept: NotRequired[str],
    endTime: NotRequired[Union[datetime, str]],
    maxDepth: NotRequired[int],
    period: NotRequired[str],
    startTime: NotRequired[Union[datetime, str]],
```

## GetRecommendationsRequestRequestTypeDef

```python
# GetRecommendationsRequestRequestTypeDef definition

class GetRecommendationsRequestRequestTypeDef(TypedDict):
    endTime: Union[datetime, str],
    profilingGroupName: str,
    startTime: Union[datetime, str],
    locale: NotRequired[str],
```

## ListFindingsReportsRequestRequestTypeDef

```python
# ListFindingsReportsRequestRequestTypeDef definition

class ListFindingsReportsRequestRequestTypeDef(TypedDict):
    endTime: Union[datetime, str],
    profilingGroupName: str,
    startTime: Union[datetime, str],
    dailyReportsOnly: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListProfileTimesRequestRequestTypeDef

```python
# ListProfileTimesRequestRequestTypeDef definition

class ListProfileTimesRequestRequestTypeDef(TypedDict):
    endTime: Union[datetime, str],
    period: AggregationPeriodType,  # (1)
    profilingGroupName: str,
    startTime: Union[datetime, str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    orderBy: NotRequired[OrderByType],  # (2)
```

1. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
2. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
## PostAgentProfileRequestRequestTypeDef

```python
# PostAgentProfileRequestRequestTypeDef definition

class PostAgentProfileRequestRequestTypeDef(TypedDict):
    agentProfile: Union[str, bytes, IO[Any], StreamingBody],
    contentType: str,
    profilingGroupName: str,
    profileToken: NotRequired[str],
```

## GetFindingsReportAccountSummaryResponseTypeDef

```python
# GetFindingsReportAccountSummaryResponseTypeDef definition

class GetFindingsReportAccountSummaryResponseTypeDef(TypedDict):
    nextToken: str,
    reportSummaries: List[FindingsReportSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FindingsReportSummaryTypeDef](./type_defs.md#findingsreportsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFindingsReportsResponseTypeDef

```python
# ListFindingsReportsResponseTypeDef definition

class ListFindingsReportsResponseTypeDef(TypedDict):
    findingsReportSummaries: List[FindingsReportSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FindingsReportSummaryTypeDef](./type_defs.md#findingsreportsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfileTimesRequestListProfileTimesPaginateTypeDef

```python
# ListProfileTimesRequestListProfileTimesPaginateTypeDef definition

class ListProfileTimesRequestListProfileTimesPaginateTypeDef(TypedDict):
    endTime: Union[datetime, str],
    period: AggregationPeriodType,  # (1)
    profilingGroupName: str,
    startTime: Union[datetime, str],
    orderBy: NotRequired[OrderByType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
2. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProfileTimesResponseTypeDef

```python
# ListProfileTimesResponseTypeDef definition

class ListProfileTimesResponseTypeDef(TypedDict):
    nextToken: str,
    profileTimes: List[ProfileTimeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileTimeTypeDef](./type_defs.md#profiletimetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    allMatchesCount: int,
    allMatchesSum: float,
    endTime: datetime,
    pattern: PatternTypeDef,  # (1)
    startTime: datetime,
    topMatches: List[MatchTypeDef],  # (2)
```

1. See [:material-code-braces: PatternTypeDef](./type_defs.md#patterntypedef) 
2. See [:material-code-braces: MatchTypeDef](./type_defs.md#matchtypedef) 
## AddNotificationChannelsResponseTypeDef

```python
# AddNotificationChannelsResponseTypeDef definition

class AddNotificationChannelsResponseTypeDef(TypedDict):
    notificationConfiguration: NotificationConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNotificationConfigurationResponseTypeDef

```python
# GetNotificationConfigurationResponseTypeDef definition

class GetNotificationConfigurationResponseTypeDef(TypedDict):
    notificationConfiguration: NotificationConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveNotificationChannelResponseTypeDef

```python
# RemoveNotificationChannelResponseTypeDef definition

class RemoveNotificationChannelResponseTypeDef(TypedDict):
    notificationConfiguration: NotificationConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProfilingGroupDescriptionTypeDef

```python
# ProfilingGroupDescriptionTypeDef definition

class ProfilingGroupDescriptionTypeDef(TypedDict):
    agentOrchestrationConfig: NotRequired[AgentOrchestrationConfigTypeDef],  # (1)
    arn: NotRequired[str],
    computePlatform: NotRequired[ComputePlatformType],  # (2)
    createdAt: NotRequired[datetime],
    name: NotRequired[str],
    profilingStatus: NotRequired[ProfilingStatusTypeDef],  # (3)
    tags: NotRequired[Dict[str, str]],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: AgentOrchestrationConfigTypeDef](./type_defs.md#agentorchestrationconfigtypedef) 
2. See [:material-code-brackets: ComputePlatformType](./literals.md#computeplatformtype) 
3. See [:material-code-braces: ProfilingStatusTypeDef](./type_defs.md#profilingstatustypedef) 
## AnomalyTypeDef

```python
# AnomalyTypeDef definition

class AnomalyTypeDef(TypedDict):
    instances: List[AnomalyInstanceTypeDef],  # (1)
    metric: MetricTypeDef,  # (2)
    reason: str,
```

1. See [:material-code-braces: AnomalyInstanceTypeDef](./type_defs.md#anomalyinstancetypedef) 
2. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
## BatchGetFrameMetricDataResponseTypeDef

```python
# BatchGetFrameMetricDataResponseTypeDef definition

class BatchGetFrameMetricDataResponseTypeDef(TypedDict):
    endTime: datetime,
    endTimes: List[TimestampStructureTypeDef],  # (1)
    frameMetricData: List[FrameMetricDatumTypeDef],  # (2)
    resolution: AggregationPeriodType,  # (3)
    startTime: datetime,
    unprocessedEndTimes: Dict[str, List[TimestampStructureTypeDef]],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: TimestampStructureTypeDef](./type_defs.md#timestampstructuretypedef) 
2. See [:material-code-braces: FrameMetricDatumTypeDef](./type_defs.md#framemetricdatumtypedef) 
3. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype) 
4. See [:material-code-braces: TimestampStructureTypeDef](./type_defs.md#timestampstructuretypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProfilingGroupResponseTypeDef

```python
# CreateProfilingGroupResponseTypeDef definition

class CreateProfilingGroupResponseTypeDef(TypedDict):
    profilingGroup: ProfilingGroupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfilingGroupDescriptionTypeDef](./type_defs.md#profilinggroupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProfilingGroupResponseTypeDef

```python
# DescribeProfilingGroupResponseTypeDef definition

class DescribeProfilingGroupResponseTypeDef(TypedDict):
    profilingGroup: ProfilingGroupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfilingGroupDescriptionTypeDef](./type_defs.md#profilinggroupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfilingGroupsResponseTypeDef

```python
# ListProfilingGroupsResponseTypeDef definition

class ListProfilingGroupsResponseTypeDef(TypedDict):
    nextToken: str,
    profilingGroupNames: List[str],
    profilingGroups: List[ProfilingGroupDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfilingGroupDescriptionTypeDef](./type_defs.md#profilinggroupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProfilingGroupResponseTypeDef

```python
# UpdateProfilingGroupResponseTypeDef definition

class UpdateProfilingGroupResponseTypeDef(TypedDict):
    profilingGroup: ProfilingGroupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfilingGroupDescriptionTypeDef](./type_defs.md#profilinggroupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecommendationsResponseTypeDef

```python
# GetRecommendationsResponseTypeDef definition

class GetRecommendationsResponseTypeDef(TypedDict):
    anomalies: List[AnomalyTypeDef],  # (1)
    profileEndTime: datetime,
    profileStartTime: datetime,
    profilingGroupName: str,
    recommendations: List[RecommendationTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AnomalyTypeDef](./type_defs.md#anomalytypedef) 
2. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
