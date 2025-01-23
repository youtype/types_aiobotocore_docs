# Type definitions

> [Index](../README.md) > [ApplicationInsights](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ApplicationInsights](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#applicationinsights)
    type annotations stubs module [types-aiobotocore-application-insights](https://pypi.org/project/types-aiobotocore-application-insights/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## WorkloadConfigurationTypeDef

```python
# WorkloadConfigurationTypeDef definition

class WorkloadConfigurationTypeDef(TypedDict):
    WorkloadName: NotRequired[str],
    Tier: NotRequired[TierType],  # (1)
    Configuration: NotRequired[str],
```

1. See [:material-code-brackets: TierType](./literals.md#tiertype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ApplicationComponentTypeDef

```python
# ApplicationComponentTypeDef definition

class ApplicationComponentTypeDef(TypedDict):
    ComponentName: NotRequired[str],
    ComponentRemarks: NotRequired[str],
    ResourceType: NotRequired[str],
    OsType: NotRequired[OsTypeType],  # (1)
    Tier: NotRequired[TierType],  # (2)
    Monitor: NotRequired[bool],
    DetectedWorkload: NotRequired[Dict[TierType, Dict[str, str]]],  # (3)
```

1. See [:material-code-brackets: OsTypeType](./literals.md#ostypetype) 
2. See [:material-code-brackets: TierType](./literals.md#tiertype) 
3. See [:material-code-brackets: TierType](./literals.md#tiertype) 
## ApplicationInfoTypeDef

```python
# ApplicationInfoTypeDef definition

class ApplicationInfoTypeDef(TypedDict):
    AccountId: NotRequired[str],
    ResourceGroupName: NotRequired[str],
    LifeCycle: NotRequired[str],
    OpsItemSNSTopicArn: NotRequired[str],
    SNSNotificationArn: NotRequired[str],
    OpsCenterEnabled: NotRequired[bool],
    CWEMonitorEnabled: NotRequired[bool],
    Remarks: NotRequired[str],
    AutoConfigEnabled: NotRequired[bool],
    DiscoveryType: NotRequired[DiscoveryTypeType],  # (1)
    AttachMissingPermission: NotRequired[bool],
```

1. See [:material-code-brackets: DiscoveryTypeType](./literals.md#discoverytypetype) 
## ConfigurationEventTypeDef

```python
# ConfigurationEventTypeDef definition

class ConfigurationEventTypeDef(TypedDict):
    ResourceGroupName: NotRequired[str],
    AccountId: NotRequired[str],
    MonitoredResourceARN: NotRequired[str],
    EventStatus: NotRequired[ConfigurationEventStatusType],  # (1)
    EventResourceType: NotRequired[ConfigurationEventResourceTypeType],  # (2)
    EventTime: NotRequired[datetime],
    EventDetail: NotRequired[str],
    EventResourceName: NotRequired[str],
```

1. See [:material-code-brackets: ConfigurationEventStatusType](./literals.md#configurationeventstatustype) 
2. See [:material-code-brackets: ConfigurationEventResourceTypeType](./literals.md#configurationeventresourcetypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateComponentRequestRequestTypeDef

```python
# CreateComponentRequestRequestTypeDef definition

class CreateComponentRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    ResourceList: Sequence[str],
```

## CreateLogPatternRequestRequestTypeDef

```python
# CreateLogPatternRequestRequestTypeDef definition

class CreateLogPatternRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    PatternSetName: str,
    PatternName: str,
    Pattern: str,
    Rank: int,
```

## LogPatternTypeDef

```python
# LogPatternTypeDef definition

class LogPatternTypeDef(TypedDict):
    PatternSetName: NotRequired[str],
    PatternName: NotRequired[str],
    Pattern: NotRequired[str],
    Rank: NotRequired[int],
```

## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
```

## DeleteComponentRequestRequestTypeDef

```python
# DeleteComponentRequestRequestTypeDef definition

class DeleteComponentRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
```

## DeleteLogPatternRequestRequestTypeDef

```python
# DeleteLogPatternRequestRequestTypeDef definition

class DeleteLogPatternRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    PatternSetName: str,
    PatternName: str,
```

## DescribeApplicationRequestRequestTypeDef

```python
# DescribeApplicationRequestRequestTypeDef definition

class DescribeApplicationRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    AccountId: NotRequired[str],
```

## DescribeComponentConfigurationRecommendationRequestRequestTypeDef

```python
# DescribeComponentConfigurationRecommendationRequestRequestTypeDef definition

class DescribeComponentConfigurationRecommendationRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    Tier: TierType,  # (1)
    WorkloadName: NotRequired[str],
    RecommendationType: NotRequired[RecommendationTypeType],  # (2)
```

1. See [:material-code-brackets: TierType](./literals.md#tiertype) 
2. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
## DescribeComponentConfigurationRequestRequestTypeDef

```python
# DescribeComponentConfigurationRequestRequestTypeDef definition

class DescribeComponentConfigurationRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    AccountId: NotRequired[str],
```

## DescribeComponentRequestRequestTypeDef

```python
# DescribeComponentRequestRequestTypeDef definition

class DescribeComponentRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    AccountId: NotRequired[str],
```

## DescribeLogPatternRequestRequestTypeDef

```python
# DescribeLogPatternRequestRequestTypeDef definition

class DescribeLogPatternRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    PatternSetName: str,
    PatternName: str,
    AccountId: NotRequired[str],
```

## DescribeObservationRequestRequestTypeDef

```python
# DescribeObservationRequestRequestTypeDef definition

class DescribeObservationRequestRequestTypeDef(TypedDict):
    ObservationId: str,
    AccountId: NotRequired[str],
```

## ObservationTypeDef

```python
# ObservationTypeDef definition

class ObservationTypeDef(TypedDict):
    Id: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    SourceType: NotRequired[str],
    SourceARN: NotRequired[str],
    LogGroup: NotRequired[str],
    LineTime: NotRequired[datetime],
    LogText: NotRequired[str],
    LogFilter: NotRequired[LogFilterType],  # (1)
    MetricNamespace: NotRequired[str],
    MetricName: NotRequired[str],
    Unit: NotRequired[str],
    Value: NotRequired[float],
    CloudWatchEventId: NotRequired[str],
    CloudWatchEventSource: NotRequired[CloudWatchEventSourceType],  # (2)
    CloudWatchEventDetailType: NotRequired[str],
    HealthEventArn: NotRequired[str],
    HealthService: NotRequired[str],
    HealthEventTypeCode: NotRequired[str],
    HealthEventTypeCategory: NotRequired[str],
    HealthEventDescription: NotRequired[str],
    CodeDeployDeploymentId: NotRequired[str],
    CodeDeployDeploymentGroup: NotRequired[str],
    CodeDeployState: NotRequired[str],
    CodeDeployApplication: NotRequired[str],
    CodeDeployInstanceGroupId: NotRequired[str],
    Ec2State: NotRequired[str],
    RdsEventCategories: NotRequired[str],
    RdsEventMessage: NotRequired[str],
    S3EventName: NotRequired[str],
    StatesExecutionArn: NotRequired[str],
    StatesArn: NotRequired[str],
    StatesStatus: NotRequired[str],
    StatesInput: NotRequired[str],
    EbsEvent: NotRequired[str],
    EbsResult: NotRequired[str],
    EbsCause: NotRequired[str],
    EbsRequestId: NotRequired[str],
    XRayFaultPercent: NotRequired[int],
    XRayThrottlePercent: NotRequired[int],
    XRayErrorPercent: NotRequired[int],
    XRayRequestCount: NotRequired[int],
    XRayRequestAverageLatency: NotRequired[int],
    XRayNodeName: NotRequired[str],
    XRayNodeType: NotRequired[str],
```

1. See [:material-code-brackets: LogFilterType](./literals.md#logfiltertype) 
2. See [:material-code-brackets: CloudWatchEventSourceType](./literals.md#cloudwatcheventsourcetype) 
## DescribeProblemObservationsRequestRequestTypeDef

```python
# DescribeProblemObservationsRequestRequestTypeDef definition

class DescribeProblemObservationsRequestRequestTypeDef(TypedDict):
    ProblemId: str,
    AccountId: NotRequired[str],
```

## DescribeProblemRequestRequestTypeDef

```python
# DescribeProblemRequestRequestTypeDef definition

class DescribeProblemRequestRequestTypeDef(TypedDict):
    ProblemId: str,
    AccountId: NotRequired[str],
```

## ProblemTypeDef

```python
# ProblemTypeDef definition

class ProblemTypeDef(TypedDict):
    Id: NotRequired[str],
    Title: NotRequired[str],
    ShortName: NotRequired[str],
    Insights: NotRequired[str],
    Status: NotRequired[StatusType],  # (1)
    AffectedResource: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    SeverityLevel: NotRequired[SeverityLevelType],  # (2)
    AccountId: NotRequired[str],
    ResourceGroupName: NotRequired[str],
    Feedback: NotRequired[Dict[FeedbackKeyType, FeedbackValueType]],  # (3)
    RecurringCount: NotRequired[int],
    LastRecurrenceTime: NotRequired[datetime],
    Visibility: NotRequired[VisibilityType],  # (4)
    ResolutionMethod: NotRequired[ResolutionMethodType],  # (5)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: SeverityLevelType](./literals.md#severityleveltype) 
3. See [:material-code-brackets: FeedbackKeyType](./literals.md#feedbackkeytype) [:material-code-brackets: FeedbackValueType](./literals.md#feedbackvaluetype) 
4. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
5. See [:material-code-brackets: ResolutionMethodType](./literals.md#resolutionmethodtype) 
## DescribeWorkloadRequestRequestTypeDef

```python
# DescribeWorkloadRequestRequestTypeDef definition

class DescribeWorkloadRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    WorkloadId: str,
    AccountId: NotRequired[str],
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    AccountId: NotRequired[str],
```

## ListComponentsRequestRequestTypeDef

```python
# ListComponentsRequestRequestTypeDef definition

class ListComponentsRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    AccountId: NotRequired[str],
```

## ListLogPatternSetsRequestRequestTypeDef

```python
# ListLogPatternSetsRequestRequestTypeDef definition

class ListLogPatternSetsRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    AccountId: NotRequired[str],
```

## ListLogPatternsRequestRequestTypeDef

```python
# ListLogPatternsRequestRequestTypeDef definition

class ListLogPatternsRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    PatternSetName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    AccountId: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## ListWorkloadsRequestRequestTypeDef

```python
# ListWorkloadsRequestRequestTypeDef definition

class ListWorkloadsRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    AccountId: NotRequired[str],
```

## WorkloadTypeDef

```python
# WorkloadTypeDef definition

class WorkloadTypeDef(TypedDict):
    WorkloadId: NotRequired[str],
    ComponentName: NotRequired[str],
    WorkloadName: NotRequired[str],
    Tier: NotRequired[TierType],  # (1)
    WorkloadRemarks: NotRequired[str],
    MissingWorkloadConfig: NotRequired[bool],
```

1. See [:material-code-brackets: TierType](./literals.md#tiertype) 
## RemoveWorkloadRequestRequestTypeDef

```python
# RemoveWorkloadRequestRequestTypeDef definition

class RemoveWorkloadRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    WorkloadId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    OpsCenterEnabled: NotRequired[bool],
    CWEMonitorEnabled: NotRequired[bool],
    OpsItemSNSTopicArn: NotRequired[str],
    SNSNotificationArn: NotRequired[str],
    RemoveSNSTopic: NotRequired[bool],
    AutoConfigEnabled: NotRequired[bool],
    AttachMissingPermission: NotRequired[bool],
```

## UpdateComponentConfigurationRequestRequestTypeDef

```python
# UpdateComponentConfigurationRequestRequestTypeDef definition

class UpdateComponentConfigurationRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    Monitor: NotRequired[bool],
    Tier: NotRequired[TierType],  # (1)
    ComponentConfiguration: NotRequired[str],
    AutoConfigEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: TierType](./literals.md#tiertype) 
## UpdateComponentRequestRequestTypeDef

```python
# UpdateComponentRequestRequestTypeDef definition

class UpdateComponentRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    NewComponentName: NotRequired[str],
    ResourceList: NotRequired[Sequence[str]],
```

## UpdateLogPatternRequestRequestTypeDef

```python
# UpdateLogPatternRequestRequestTypeDef definition

class UpdateLogPatternRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    PatternSetName: str,
    PatternName: str,
    Pattern: NotRequired[str],
    Rank: NotRequired[int],
```

## UpdateProblemRequestRequestTypeDef

```python
# UpdateProblemRequestRequestTypeDef definition

class UpdateProblemRequestRequestTypeDef(TypedDict):
    ProblemId: str,
    UpdateStatus: NotRequired[UpdateStatusType],  # (1)
    Visibility: NotRequired[VisibilityType],  # (2)
```

1. See [:material-code-brackets: UpdateStatusType](./literals.md#updatestatustype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## AddWorkloadRequestRequestTypeDef

```python
# AddWorkloadRequestRequestTypeDef definition

class AddWorkloadRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    WorkloadConfiguration: WorkloadConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: WorkloadConfigurationTypeDef](./type_defs.md#workloadconfigurationtypedef) 
## UpdateWorkloadRequestRequestTypeDef

```python
# UpdateWorkloadRequestRequestTypeDef definition

class UpdateWorkloadRequestRequestTypeDef(TypedDict):
    ResourceGroupName: str,
    ComponentName: str,
    WorkloadConfiguration: WorkloadConfigurationTypeDef,  # (1)
    WorkloadId: NotRequired[str],
```

1. See [:material-code-braces: WorkloadConfigurationTypeDef](./type_defs.md#workloadconfigurationtypedef) 
## AddWorkloadResponseTypeDef

```python
# AddWorkloadResponseTypeDef definition

class AddWorkloadResponseTypeDef(TypedDict):
    WorkloadId: str,
    WorkloadConfiguration: WorkloadConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkloadConfigurationTypeDef](./type_defs.md#workloadconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeComponentConfigurationRecommendationResponseTypeDef

```python
# DescribeComponentConfigurationRecommendationResponseTypeDef definition

class DescribeComponentConfigurationRecommendationResponseTypeDef(TypedDict):
    ComponentConfiguration: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeComponentConfigurationResponseTypeDef

```python
# DescribeComponentConfigurationResponseTypeDef definition

class DescribeComponentConfigurationResponseTypeDef(TypedDict):
    Monitor: bool,
    Tier: TierType,  # (1)
    ComponentConfiguration: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TierType](./literals.md#tiertype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkloadResponseTypeDef

```python
# DescribeWorkloadResponseTypeDef definition

class DescribeWorkloadResponseTypeDef(TypedDict):
    WorkloadId: str,
    WorkloadRemarks: str,
    WorkloadConfiguration: WorkloadConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkloadConfigurationTypeDef](./type_defs.md#workloadconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLogPatternSetsResponseTypeDef

```python
# ListLogPatternSetsResponseTypeDef definition

class ListLogPatternSetsResponseTypeDef(TypedDict):
    ResourceGroupName: str,
    AccountId: str,
    LogPatternSets: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkloadResponseTypeDef

```python
# UpdateWorkloadResponseTypeDef definition

class UpdateWorkloadResponseTypeDef(TypedDict):
    WorkloadId: str,
    WorkloadConfiguration: WorkloadConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkloadConfigurationTypeDef](./type_defs.md#workloadconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeComponentResponseTypeDef

```python
# DescribeComponentResponseTypeDef definition

class DescribeComponentResponseTypeDef(TypedDict):
    ApplicationComponent: ApplicationComponentTypeDef,  # (1)
    ResourceList: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationComponentTypeDef](./type_defs.md#applicationcomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComponentsResponseTypeDef

```python
# ListComponentsResponseTypeDef definition

class ListComponentsResponseTypeDef(TypedDict):
    ApplicationComponentList: List[ApplicationComponentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationComponentTypeDef](./type_defs.md#applicationcomponenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    ApplicationInfo: ApplicationInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationInfoTypeDef](./type_defs.md#applicationinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicationResponseTypeDef

```python
# DescribeApplicationResponseTypeDef definition

class DescribeApplicationResponseTypeDef(TypedDict):
    ApplicationInfo: ApplicationInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationInfoTypeDef](./type_defs.md#applicationinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    ApplicationInfoList: List[ApplicationInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationInfoTypeDef](./type_defs.md#applicationinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationResponseTypeDef

```python
# UpdateApplicationResponseTypeDef definition

class UpdateApplicationResponseTypeDef(TypedDict):
    ApplicationInfo: ApplicationInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationInfoTypeDef](./type_defs.md#applicationinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationHistoryResponseTypeDef

```python
# ListConfigurationHistoryResponseTypeDef definition

class ListConfigurationHistoryResponseTypeDef(TypedDict):
    EventList: List[ConfigurationEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationEventTypeDef](./type_defs.md#configurationeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    ResourceGroupName: NotRequired[str],
    OpsCenterEnabled: NotRequired[bool],
    CWEMonitorEnabled: NotRequired[bool],
    OpsItemSNSTopicArn: NotRequired[str],
    SNSNotificationArn: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    AutoConfigEnabled: NotRequired[bool],
    AutoCreate: NotRequired[bool],
    GroupingType: NotRequired[GroupingTypeType],  # (2)
    AttachMissingPermission: NotRequired[bool],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: GroupingTypeType](./literals.md#groupingtypetype) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateLogPatternResponseTypeDef

```python
# CreateLogPatternResponseTypeDef definition

class CreateLogPatternResponseTypeDef(TypedDict):
    LogPattern: LogPatternTypeDef,  # (1)
    ResourceGroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LogPatternTypeDef](./type_defs.md#logpatterntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLogPatternResponseTypeDef

```python
# DescribeLogPatternResponseTypeDef definition

class DescribeLogPatternResponseTypeDef(TypedDict):
    ResourceGroupName: str,
    AccountId: str,
    LogPattern: LogPatternTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LogPatternTypeDef](./type_defs.md#logpatterntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLogPatternsResponseTypeDef

```python
# ListLogPatternsResponseTypeDef definition

class ListLogPatternsResponseTypeDef(TypedDict):
    ResourceGroupName: str,
    AccountId: str,
    LogPatterns: List[LogPatternTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LogPatternTypeDef](./type_defs.md#logpatterntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLogPatternResponseTypeDef

```python
# UpdateLogPatternResponseTypeDef definition

class UpdateLogPatternResponseTypeDef(TypedDict):
    ResourceGroupName: str,
    LogPattern: LogPatternTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LogPatternTypeDef](./type_defs.md#logpatterntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeObservationResponseTypeDef

```python
# DescribeObservationResponseTypeDef definition

class DescribeObservationResponseTypeDef(TypedDict):
    Observation: ObservationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ObservationTypeDef](./type_defs.md#observationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RelatedObservationsTypeDef

```python
# RelatedObservationsTypeDef definition

class RelatedObservationsTypeDef(TypedDict):
    ObservationList: NotRequired[List[ObservationTypeDef]],  # (1)
```

1. See [:material-code-braces: ObservationTypeDef](./type_defs.md#observationtypedef) 
## DescribeProblemResponseTypeDef

```python
# DescribeProblemResponseTypeDef definition

class DescribeProblemResponseTypeDef(TypedDict):
    Problem: ProblemTypeDef,  # (1)
    SNSNotificationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProblemTypeDef](./type_defs.md#problemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProblemsResponseTypeDef

```python
# ListProblemsResponseTypeDef definition

class ListProblemsResponseTypeDef(TypedDict):
    ProblemList: List[ProblemTypeDef],  # (1)
    ResourceGroupName: str,
    AccountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProblemTypeDef](./type_defs.md#problemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationHistoryRequestRequestTypeDef

```python
# ListConfigurationHistoryRequestRequestTypeDef definition

class ListConfigurationHistoryRequestRequestTypeDef(TypedDict):
    ResourceGroupName: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    EventStatus: NotRequired[ConfigurationEventStatusType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    AccountId: NotRequired[str],
```

1. See [:material-code-brackets: ConfigurationEventStatusType](./literals.md#configurationeventstatustype) 
## ListProblemsRequestRequestTypeDef

```python
# ListProblemsRequestRequestTypeDef definition

class ListProblemsRequestRequestTypeDef(TypedDict):
    AccountId: NotRequired[str],
    ResourceGroupName: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ComponentName: NotRequired[str],
    Visibility: NotRequired[VisibilityType],  # (1)
```

1. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
## ListWorkloadsResponseTypeDef

```python
# ListWorkloadsResponseTypeDef definition

class ListWorkloadsResponseTypeDef(TypedDict):
    WorkloadList: List[WorkloadTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkloadTypeDef](./type_defs.md#workloadtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProblemObservationsResponseTypeDef

```python
# DescribeProblemObservationsResponseTypeDef definition

class DescribeProblemObservationsResponseTypeDef(TypedDict):
    RelatedObservations: RelatedObservationsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RelatedObservationsTypeDef](./type_defs.md#relatedobservationstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
