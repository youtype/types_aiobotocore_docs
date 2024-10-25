# Type definitions

> [Index](../README.md) > [DevOpsGuru](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DevOpsGuru](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
    type annotations stubs module [types-aiobotocore-devops-guru](https://pypi.org/project/types-aiobotocore-devops-guru/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## CloudFormationCostEstimationResourceCollectionFilterUnionTypeDef

```python
# CloudFormationCostEstimationResourceCollectionFilterUnionTypeDef definition

CloudFormationCostEstimationResourceCollectionFilterUnionTypeDef = Union[
    CloudFormationCostEstimationResourceCollectionFilterTypeDef,  # (1)
    CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CloudFormationCostEstimationResourceCollectionFilterTypeDef](./type_defs.md#cloudformationcostestimationresourcecollectionfiltertypedef) 
2. See [:material-code-braces: CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef](./type_defs.md#cloudformationcostestimationresourcecollectionfilteroutputtypedef) 

## NotificationFilterConfigUnionTypeDef

```python
# NotificationFilterConfigUnionTypeDef definition

NotificationFilterConfigUnionTypeDef = Union[
    NotificationFilterConfigTypeDef,  # (1)
    NotificationFilterConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NotificationFilterConfigTypeDef](./type_defs.md#notificationfilterconfigtypedef) 
2. See [:material-code-braces: NotificationFilterConfigOutputTypeDef](./type_defs.md#notificationfilterconfigoutputtypedef) 

## ServiceCollectionUnionTypeDef

```python
# ServiceCollectionUnionTypeDef definition

ServiceCollectionUnionTypeDef = Union[
    ServiceCollectionTypeDef,  # (1)
    ServiceCollectionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServiceCollectionTypeDef](./type_defs.md#servicecollectiontypedef) 
2. See [:material-code-braces: ServiceCollectionOutputTypeDef](./type_defs.md#servicecollectionoutputtypedef) 

## TagCostEstimationResourceCollectionFilterUnionTypeDef

```python
# TagCostEstimationResourceCollectionFilterUnionTypeDef definition

TagCostEstimationResourceCollectionFilterUnionTypeDef = Union[
    TagCostEstimationResourceCollectionFilterTypeDef,  # (1)
    TagCostEstimationResourceCollectionFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TagCostEstimationResourceCollectionFilterTypeDef](./type_defs.md#tagcostestimationresourcecollectionfiltertypedef) 
2. See [:material-code-braces: TagCostEstimationResourceCollectionFilterOutputTypeDef](./type_defs.md#tagcostestimationresourcecollectionfilteroutputtypedef) 

## ResourceCollectionUnionTypeDef

```python
# ResourceCollectionUnionTypeDef definition

ResourceCollectionUnionTypeDef = Union[
    ResourceCollectionTypeDef,  # (1)
    ResourceCollectionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceCollectionTypeDef](./type_defs.md#resourcecollectiontypedef) 
2. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 



## AccountInsightHealthTypeDef

```python
# AccountInsightHealthTypeDef definition

class AccountInsightHealthTypeDef(TypedDict):
    OpenProactiveInsights: NotRequired[int],
    OpenReactiveInsights: NotRequired[int],
```

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

## AmazonCodeGuruProfilerIntegrationTypeDef

```python
# AmazonCodeGuruProfilerIntegrationTypeDef definition

class AmazonCodeGuruProfilerIntegrationTypeDef(TypedDict):
    Status: NotRequired[EventSourceOptInStatusType],  # (1)
```

1. See [:material-code-brackets: EventSourceOptInStatusType](./literals.md#eventsourceoptinstatustype) 
## AnomalyReportedTimeRangeTypeDef

```python
# AnomalyReportedTimeRangeTypeDef definition

class AnomalyReportedTimeRangeTypeDef(TypedDict):
    OpenTime: datetime,
    CloseTime: NotRequired[datetime],
```

## AnomalyResourceTypeDef

```python
# AnomalyResourceTypeDef definition

class AnomalyResourceTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[str],
```

## AnomalySourceMetadataTypeDef

```python
# AnomalySourceMetadataTypeDef definition

class AnomalySourceMetadataTypeDef(TypedDict):
    Source: NotRequired[str],
    SourceResourceName: NotRequired[str],
    SourceResourceType: NotRequired[str],
```

## AnomalyTimeRangeTypeDef

```python
# AnomalyTimeRangeTypeDef definition

class AnomalyTimeRangeTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: NotRequired[datetime],
```

## CloudFormationCollectionFilterTypeDef

```python
# CloudFormationCollectionFilterTypeDef definition

class CloudFormationCollectionFilterTypeDef(TypedDict):
    StackNames: NotRequired[List[str]],
```

## CloudFormationCollectionOutputTypeDef

```python
# CloudFormationCollectionOutputTypeDef definition

class CloudFormationCollectionOutputTypeDef(TypedDict):
    StackNames: NotRequired[List[str]],
```

## CloudFormationCollectionTypeDef

```python
# CloudFormationCollectionTypeDef definition

class CloudFormationCollectionTypeDef(TypedDict):
    StackNames: NotRequired[Sequence[str]],
```

## CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef

```python
# CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef definition

class CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef(TypedDict):
    StackNames: NotRequired[List[str]],
```

## CloudFormationCostEstimationResourceCollectionFilterTypeDef

```python
# CloudFormationCostEstimationResourceCollectionFilterTypeDef definition

class CloudFormationCostEstimationResourceCollectionFilterTypeDef(TypedDict):
    StackNames: NotRequired[Sequence[str]],
```

## InsightHealthTypeDef

```python
# InsightHealthTypeDef definition

class InsightHealthTypeDef(TypedDict):
    OpenProactiveInsights: NotRequired[int],
    OpenReactiveInsights: NotRequired[int],
    MeanTimeToRecoverInMilliseconds: NotRequired[int],
```

## TimestampMetricValuePairTypeDef

```python
# TimestampMetricValuePairTypeDef definition

class TimestampMetricValuePairTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
    MetricValue: NotRequired[float],
```

## CloudWatchMetricsDimensionTypeDef

```python
# CloudWatchMetricsDimensionTypeDef definition

class CloudWatchMetricsDimensionTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## TagCostEstimationResourceCollectionFilterOutputTypeDef

```python
# TagCostEstimationResourceCollectionFilterOutputTypeDef definition

class TagCostEstimationResourceCollectionFilterOutputTypeDef(TypedDict):
    AppBoundaryKey: str,
    TagValues: List[str],
```

## CostEstimationTimeRangeTypeDef

```python
# CostEstimationTimeRangeTypeDef definition

class CostEstimationTimeRangeTypeDef(TypedDict):
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

## DeleteInsightRequestRequestTypeDef

```python
# DeleteInsightRequestRequestTypeDef definition

class DeleteInsightRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DescribeAnomalyRequestRequestTypeDef

```python
# DescribeAnomalyRequestRequestTypeDef definition

class DescribeAnomalyRequestRequestTypeDef(TypedDict):
    Id: str,
    AccountId: NotRequired[str],
```

## DescribeFeedbackRequestRequestTypeDef

```python
# DescribeFeedbackRequestRequestTypeDef definition

class DescribeFeedbackRequestRequestTypeDef(TypedDict):
    InsightId: NotRequired[str],
```

## InsightFeedbackTypeDef

```python
# InsightFeedbackTypeDef definition

class InsightFeedbackTypeDef(TypedDict):
    Id: NotRequired[str],
    Feedback: NotRequired[InsightFeedbackOptionType],  # (1)
```

1. See [:material-code-brackets: InsightFeedbackOptionType](./literals.md#insightfeedbackoptiontype) 
## DescribeInsightRequestRequestTypeDef

```python
# DescribeInsightRequestRequestTypeDef definition

class DescribeInsightRequestRequestTypeDef(TypedDict):
    Id: str,
    AccountId: NotRequired[str],
```

## DescribeOrganizationHealthRequestRequestTypeDef

```python
# DescribeOrganizationHealthRequestRequestTypeDef definition

class DescribeOrganizationHealthRequestRequestTypeDef(TypedDict):
    AccountIds: NotRequired[Sequence[str]],
    OrganizationalUnitIds: NotRequired[Sequence[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef

```python
# DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef definition

class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(TypedDict):
    OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,  # (1)
    AccountIds: NotRequired[Sequence[str]],
    OrganizationalUnitIds: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: OrganizationResourceCollectionTypeType](./literals.md#organizationresourcecollectiontypetype) 
## DescribeResourceCollectionHealthRequestRequestTypeDef

```python
# DescribeResourceCollectionHealthRequestRequestTypeDef definition

class DescribeResourceCollectionHealthRequestRequestTypeDef(TypedDict):
    ResourceCollectionType: ResourceCollectionTypeType,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype) 
## EventResourceTypeDef

```python
# EventResourceTypeDef definition

class EventResourceTypeDef(TypedDict):
    Type: NotRequired[str],
    Name: NotRequired[str],
    Arn: NotRequired[str],
```

## GetCostEstimationRequestRequestTypeDef

```python
# GetCostEstimationRequestRequestTypeDef definition

class GetCostEstimationRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## ServiceResourceCostTypeDef

```python
# ServiceResourceCostTypeDef definition

class ServiceResourceCostTypeDef(TypedDict):
    Type: NotRequired[str],
    State: NotRequired[CostEstimationServiceResourceStateType],  # (1)
    Count: NotRequired[int],
    UnitCost: NotRequired[float],
    Cost: NotRequired[float],
```

1. See [:material-code-brackets: CostEstimationServiceResourceStateType](./literals.md#costestimationserviceresourcestatetype) 
## GetResourceCollectionRequestRequestTypeDef

```python
# GetResourceCollectionRequestRequestTypeDef definition

class GetResourceCollectionRequestRequestTypeDef(TypedDict):
    ResourceCollectionType: ResourceCollectionTypeType,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype) 
## InsightTimeRangeTypeDef

```python
# InsightTimeRangeTypeDef definition

class InsightTimeRangeTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: NotRequired[datetime],
```

## KMSServerSideEncryptionIntegrationConfigTypeDef

```python
# KMSServerSideEncryptionIntegrationConfigTypeDef definition

class KMSServerSideEncryptionIntegrationConfigTypeDef(TypedDict):
    KMSKeyId: NotRequired[str],
    OptInStatus: NotRequired[OptInStatusType],  # (1)
    Type: NotRequired[ServerSideEncryptionTypeType],  # (2)
```

1. See [:material-code-brackets: OptInStatusType](./literals.md#optinstatustype) 
2. See [:material-code-brackets: ServerSideEncryptionTypeType](./literals.md#serversideencryptiontypetype) 
## KMSServerSideEncryptionIntegrationTypeDef

```python
# KMSServerSideEncryptionIntegrationTypeDef definition

class KMSServerSideEncryptionIntegrationTypeDef(TypedDict):
    KMSKeyId: NotRequired[str],
    OptInStatus: NotRequired[OptInStatusType],  # (1)
    Type: NotRequired[ServerSideEncryptionTypeType],  # (2)
```

1. See [:material-code-brackets: OptInStatusType](./literals.md#optinstatustype) 
2. See [:material-code-brackets: ServerSideEncryptionTypeType](./literals.md#serversideencryptiontypetype) 
## ServiceCollectionTypeDef

```python
# ServiceCollectionTypeDef definition

class ServiceCollectionTypeDef(TypedDict):
    ServiceNames: NotRequired[Sequence[ServiceNameType]],  # (1)
```

1. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
## ListAnomalousLogGroupsRequestRequestTypeDef

```python
# ListAnomalousLogGroupsRequestRequestTypeDef definition

class ListAnomalousLogGroupsRequestRequestTypeDef(TypedDict):
    InsightId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListInsightsOngoingStatusFilterTypeDef

```python
# ListInsightsOngoingStatusFilterTypeDef definition

class ListInsightsOngoingStatusFilterTypeDef(TypedDict):
    Type: InsightTypeType,  # (1)
```

1. See [:material-code-brackets: InsightTypeType](./literals.md#insighttypetype) 
## ListMonitoredResourcesFiltersTypeDef

```python
# ListMonitoredResourcesFiltersTypeDef definition

class ListMonitoredResourcesFiltersTypeDef(TypedDict):
    ResourcePermission: ResourcePermissionType,  # (1)
    ResourceTypeFilters: Sequence[ResourceTypeFilterType],  # (2)
```

1. See [:material-code-brackets: ResourcePermissionType](./literals.md#resourcepermissiontype) 
2. See [:material-code-brackets: ResourceTypeFilterType](./literals.md#resourcetypefiltertype) 
## ListNotificationChannelsRequestRequestTypeDef

```python
# ListNotificationChannelsRequestRequestTypeDef definition

class ListNotificationChannelsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## ListRecommendationsRequestRequestTypeDef

```python
# ListRecommendationsRequestRequestTypeDef definition

class ListRecommendationsRequestRequestTypeDef(TypedDict):
    InsightId: str,
    NextToken: NotRequired[str],
    Locale: NotRequired[LocaleType],  # (1)
    AccountId: NotRequired[str],
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
## LogAnomalyClassTypeDef

```python
# LogAnomalyClassTypeDef definition

class LogAnomalyClassTypeDef(TypedDict):
    LogStreamName: NotRequired[str],
    LogAnomalyType: NotRequired[LogAnomalyTypeType],  # (1)
    LogAnomalyToken: NotRequired[str],
    LogEventId: NotRequired[str],
    Explanation: NotRequired[str],
    NumberOfLogLinesOccurrences: NotRequired[int],
    LogEventTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: LogAnomalyTypeType](./literals.md#loganomalytypetype) 
## LogsAnomalyDetectionIntegrationConfigTypeDef

```python
# LogsAnomalyDetectionIntegrationConfigTypeDef definition

class LogsAnomalyDetectionIntegrationConfigTypeDef(TypedDict):
    OptInStatus: NotRequired[OptInStatusType],  # (1)
```

1. See [:material-code-brackets: OptInStatusType](./literals.md#optinstatustype) 
## LogsAnomalyDetectionIntegrationTypeDef

```python
# LogsAnomalyDetectionIntegrationTypeDef definition

class LogsAnomalyDetectionIntegrationTypeDef(TypedDict):
    OptInStatus: NotRequired[OptInStatusType],  # (1)
```

1. See [:material-code-brackets: OptInStatusType](./literals.md#optinstatustype) 
## NotificationFilterConfigOutputTypeDef

```python
# NotificationFilterConfigOutputTypeDef definition

class NotificationFilterConfigOutputTypeDef(TypedDict):
    Severities: NotRequired[List[InsightSeverityType]],  # (1)
    MessageTypes: NotRequired[List[NotificationMessageTypeType]],  # (2)
```

1. See [:material-code-brackets: InsightSeverityType](./literals.md#insightseveritytype) 
2. See [:material-code-brackets: NotificationMessageTypeType](./literals.md#notificationmessagetypetype) 
## SnsChannelConfigTypeDef

```python
# SnsChannelConfigTypeDef definition

class SnsChannelConfigTypeDef(TypedDict):
    TopicArn: NotRequired[str],
```

## NotificationFilterConfigTypeDef

```python
# NotificationFilterConfigTypeDef definition

class NotificationFilterConfigTypeDef(TypedDict):
    Severities: NotRequired[Sequence[InsightSeverityType]],  # (1)
    MessageTypes: NotRequired[Sequence[NotificationMessageTypeType]],  # (2)
```

1. See [:material-code-brackets: InsightSeverityType](./literals.md#insightseveritytype) 
2. See [:material-code-brackets: NotificationMessageTypeType](./literals.md#notificationmessagetypetype) 
## OpsCenterIntegrationConfigTypeDef

```python
# OpsCenterIntegrationConfigTypeDef definition

class OpsCenterIntegrationConfigTypeDef(TypedDict):
    OptInStatus: NotRequired[OptInStatusType],  # (1)
```

1. See [:material-code-brackets: OptInStatusType](./literals.md#optinstatustype) 
## OpsCenterIntegrationTypeDef

```python
# OpsCenterIntegrationTypeDef definition

class OpsCenterIntegrationTypeDef(TypedDict):
    OptInStatus: NotRequired[OptInStatusType],  # (1)
```

1. See [:material-code-brackets: OptInStatusType](./literals.md#optinstatustype) 
## PerformanceInsightsMetricDimensionGroupTypeDef

```python
# PerformanceInsightsMetricDimensionGroupTypeDef definition

class PerformanceInsightsMetricDimensionGroupTypeDef(TypedDict):
    Group: NotRequired[str],
    Dimensions: NotRequired[List[str]],
    Limit: NotRequired[int],
```

## PerformanceInsightsStatTypeDef

```python
# PerformanceInsightsStatTypeDef definition

class PerformanceInsightsStatTypeDef(TypedDict):
    Type: NotRequired[str],
    Value: NotRequired[float],
```

## PerformanceInsightsReferenceScalarTypeDef

```python
# PerformanceInsightsReferenceScalarTypeDef definition

class PerformanceInsightsReferenceScalarTypeDef(TypedDict):
    Value: NotRequired[float],
```

## PredictionTimeRangeTypeDef

```python
# PredictionTimeRangeTypeDef definition

class PredictionTimeRangeTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: NotRequired[datetime],
```

## ServiceCollectionOutputTypeDef

```python
# ServiceCollectionOutputTypeDef definition

class ServiceCollectionOutputTypeDef(TypedDict):
    ServiceNames: NotRequired[List[ServiceNameType]],  # (1)
```

1. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
## RecommendationRelatedAnomalyResourceTypeDef

```python
# RecommendationRelatedAnomalyResourceTypeDef definition

class RecommendationRelatedAnomalyResourceTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[str],
```

## RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef

```python
# RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef definition

class RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
```

## RecommendationRelatedEventResourceTypeDef

```python
# RecommendationRelatedEventResourceTypeDef definition

class RecommendationRelatedEventResourceTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[str],
```

## RemoveNotificationChannelRequestRequestTypeDef

```python
# RemoveNotificationChannelRequestRequestTypeDef definition

class RemoveNotificationChannelRequestRequestTypeDef(TypedDict):
    Id: str,
```

## TagCollectionFilterTypeDef

```python
# TagCollectionFilterTypeDef definition

class TagCollectionFilterTypeDef(TypedDict):
    AppBoundaryKey: str,
    TagValues: List[str],
```

## TagCollectionOutputTypeDef

```python
# TagCollectionOutputTypeDef definition

class TagCollectionOutputTypeDef(TypedDict):
    AppBoundaryKey: str,
    TagValues: List[str],
```

## TagCollectionTypeDef

```python
# TagCollectionTypeDef definition

class TagCollectionTypeDef(TypedDict):
    AppBoundaryKey: str,
    TagValues: Sequence[str],
```

## ServiceInsightHealthTypeDef

```python
# ServiceInsightHealthTypeDef definition

class ServiceInsightHealthTypeDef(TypedDict):
    OpenProactiveInsights: NotRequired[int],
    OpenReactiveInsights: NotRequired[int],
```

## TagCostEstimationResourceCollectionFilterTypeDef

```python
# TagCostEstimationResourceCollectionFilterTypeDef definition

class TagCostEstimationResourceCollectionFilterTypeDef(TypedDict):
    AppBoundaryKey: str,
    TagValues: Sequence[str],
```

## UpdateCloudFormationCollectionFilterTypeDef

```python
# UpdateCloudFormationCollectionFilterTypeDef definition

class UpdateCloudFormationCollectionFilterTypeDef(TypedDict):
    StackNames: NotRequired[Sequence[str]],
```

## UpdateTagCollectionFilterTypeDef

```python
# UpdateTagCollectionFilterTypeDef definition

class UpdateTagCollectionFilterTypeDef(TypedDict):
    AppBoundaryKey: str,
    TagValues: Sequence[str],
```

## AccountHealthTypeDef

```python
# AccountHealthTypeDef definition

class AccountHealthTypeDef(TypedDict):
    AccountId: NotRequired[str],
    Insight: NotRequired[AccountInsightHealthTypeDef],  # (1)
```

1. See [:material-code-braces: AccountInsightHealthTypeDef](./type_defs.md#accountinsighthealthtypedef) 
## AddNotificationChannelResponseTypeDef

```python
# AddNotificationChannelResponseTypeDef definition

class AddNotificationChannelResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountHealthResponseTypeDef

```python
# DescribeAccountHealthResponseTypeDef definition

class DescribeAccountHealthResponseTypeDef(TypedDict):
    OpenReactiveInsights: int,
    OpenProactiveInsights: int,
    MetricsAnalyzed: int,
    ResourceHours: int,
    AnalyzedResourceCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountOverviewResponseTypeDef

```python
# DescribeAccountOverviewResponseTypeDef definition

class DescribeAccountOverviewResponseTypeDef(TypedDict):
    ReactiveInsights: int,
    ProactiveInsights: int,
    MeanTimeToRecoverInMilliseconds: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationHealthResponseTypeDef

```python
# DescribeOrganizationHealthResponseTypeDef definition

class DescribeOrganizationHealthResponseTypeDef(TypedDict):
    OpenReactiveInsights: int,
    OpenProactiveInsights: int,
    MetricsAnalyzed: int,
    ResourceHours: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationOverviewResponseTypeDef

```python
# DescribeOrganizationOverviewResponseTypeDef definition

class DescribeOrganizationOverviewResponseTypeDef(TypedDict):
    ReactiveInsights: int,
    ProactiveInsights: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventSourcesConfigTypeDef

```python
# EventSourcesConfigTypeDef definition

class EventSourcesConfigTypeDef(TypedDict):
    AmazonCodeGuruProfiler: NotRequired[AmazonCodeGuruProfilerIntegrationTypeDef],  # (1)
```

1. See [:material-code-braces: AmazonCodeGuruProfilerIntegrationTypeDef](./type_defs.md#amazoncodeguruprofilerintegrationtypedef) 
## CloudFormationHealthTypeDef

```python
# CloudFormationHealthTypeDef definition

class CloudFormationHealthTypeDef(TypedDict):
    StackName: NotRequired[str],
    Insight: NotRequired[InsightHealthTypeDef],  # (1)
    AnalyzedResourceCount: NotRequired[int],
```

1. See [:material-code-braces: InsightHealthTypeDef](./type_defs.md#insighthealthtypedef) 
## TagHealthTypeDef

```python
# TagHealthTypeDef definition

class TagHealthTypeDef(TypedDict):
    AppBoundaryKey: NotRequired[str],
    TagValue: NotRequired[str],
    Insight: NotRequired[InsightHealthTypeDef],  # (1)
    AnalyzedResourceCount: NotRequired[int],
```

1. See [:material-code-braces: InsightHealthTypeDef](./type_defs.md#insighthealthtypedef) 
## CloudWatchMetricsDataSummaryTypeDef

```python
# CloudWatchMetricsDataSummaryTypeDef definition

class CloudWatchMetricsDataSummaryTypeDef(TypedDict):
    TimestampMetricValuePairList: NotRequired[List[TimestampMetricValuePairTypeDef]],  # (1)
    StatusCode: NotRequired[CloudWatchMetricDataStatusCodeType],  # (2)
```

1. See [:material-code-braces: TimestampMetricValuePairTypeDef](./type_defs.md#timestampmetricvaluepairtypedef) 
2. See [:material-code-brackets: CloudWatchMetricDataStatusCodeType](./literals.md#cloudwatchmetricdatastatuscodetype) 
## CostEstimationResourceCollectionFilterOutputTypeDef

```python
# CostEstimationResourceCollectionFilterOutputTypeDef definition

class CostEstimationResourceCollectionFilterOutputTypeDef(TypedDict):
    CloudFormation: NotRequired[CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef],  # (1)
    Tags: NotRequired[List[TagCostEstimationResourceCollectionFilterOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef](./type_defs.md#cloudformationcostestimationresourcecollectionfilteroutputtypedef) 
2. See [:material-code-braces: TagCostEstimationResourceCollectionFilterOutputTypeDef](./type_defs.md#tagcostestimationresourcecollectionfilteroutputtypedef) 
## DescribeAccountOverviewRequestRequestTypeDef

```python
# DescribeAccountOverviewRequestRequestTypeDef definition

class DescribeAccountOverviewRequestRequestTypeDef(TypedDict):
    FromTime: TimestampTypeDef,
    ToTime: NotRequired[TimestampTypeDef],
```

## DescribeOrganizationOverviewRequestRequestTypeDef

```python
# DescribeOrganizationOverviewRequestRequestTypeDef definition

class DescribeOrganizationOverviewRequestRequestTypeDef(TypedDict):
    FromTime: TimestampTypeDef,
    ToTime: NotRequired[TimestampTypeDef],
    AccountIds: NotRequired[Sequence[str]],
    OrganizationalUnitIds: NotRequired[Sequence[str]],
```

## EndTimeRangeTypeDef

```python
# EndTimeRangeTypeDef definition

class EndTimeRangeTypeDef(TypedDict):
    FromTime: NotRequired[TimestampTypeDef],
    ToTime: NotRequired[TimestampTypeDef],
```

## EventTimeRangeTypeDef

```python
# EventTimeRangeTypeDef definition

class EventTimeRangeTypeDef(TypedDict):
    FromTime: TimestampTypeDef,
    ToTime: TimestampTypeDef,
```

## StartTimeRangeTypeDef

```python
# StartTimeRangeTypeDef definition

class StartTimeRangeTypeDef(TypedDict):
    FromTime: NotRequired[TimestampTypeDef],
    ToTime: NotRequired[TimestampTypeDef],
```

## DescribeFeedbackResponseTypeDef

```python
# DescribeFeedbackResponseTypeDef definition

class DescribeFeedbackResponseTypeDef(TypedDict):
    InsightFeedback: InsightFeedbackTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightFeedbackTypeDef](./type_defs.md#insightfeedbacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutFeedbackRequestRequestTypeDef

```python
# PutFeedbackRequestRequestTypeDef definition

class PutFeedbackRequestRequestTypeDef(TypedDict):
    InsightFeedback: NotRequired[InsightFeedbackTypeDef],  # (1)
```

1. See [:material-code-braces: InsightFeedbackTypeDef](./type_defs.md#insightfeedbacktypedef) 
## DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef

```python
# DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef definition

class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(TypedDict):
    OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,  # (1)
    AccountIds: NotRequired[Sequence[str]],
    OrganizationalUnitIds: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OrganizationResourceCollectionTypeType](./literals.md#organizationresourcecollectiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef

```python
# DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef definition

class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(TypedDict):
    ResourceCollectionType: ResourceCollectionTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCostEstimationRequestGetCostEstimationPaginateTypeDef

```python
# GetCostEstimationRequestGetCostEstimationPaginateTypeDef definition

class GetCostEstimationRequestGetCostEstimationPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef

```python
# GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef definition

class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(TypedDict):
    ResourceCollectionType: ResourceCollectionTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef

```python
# ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef definition

class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(TypedDict):
    InsightId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef

```python
# ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef definition

class ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecommendationsRequestListRecommendationsPaginateTypeDef

```python
# ListRecommendationsRequestListRecommendationsPaginateTypeDef definition

class ListRecommendationsRequestListRecommendationsPaginateTypeDef(TypedDict):
    InsightId: str,
    Locale: NotRequired[LocaleType],  # (1)
    AccountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAnomaliesForInsightFiltersTypeDef

```python
# ListAnomaliesForInsightFiltersTypeDef definition

class ListAnomaliesForInsightFiltersTypeDef(TypedDict):
    ServiceCollection: NotRequired[ServiceCollectionTypeDef],  # (1)
```

1. See [:material-code-braces: ServiceCollectionTypeDef](./type_defs.md#servicecollectiontypedef) 
## ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef

```python
# ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef definition

class ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef(TypedDict):
    Filters: NotRequired[ListMonitoredResourcesFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListMonitoredResourcesFiltersTypeDef](./type_defs.md#listmonitoredresourcesfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMonitoredResourcesRequestRequestTypeDef

```python
# ListMonitoredResourcesRequestRequestTypeDef definition

class ListMonitoredResourcesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[ListMonitoredResourcesFiltersTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListMonitoredResourcesFiltersTypeDef](./type_defs.md#listmonitoredresourcesfilterstypedef) 
## LogAnomalyShowcaseTypeDef

```python
# LogAnomalyShowcaseTypeDef definition

class LogAnomalyShowcaseTypeDef(TypedDict):
    LogAnomalyClasses: NotRequired[List[LogAnomalyClassTypeDef]],  # (1)
```

1. See [:material-code-braces: LogAnomalyClassTypeDef](./type_defs.md#loganomalyclasstypedef) 
## NotificationChannelConfigOutputTypeDef

```python
# NotificationChannelConfigOutputTypeDef definition

class NotificationChannelConfigOutputTypeDef(TypedDict):
    Sns: SnsChannelConfigTypeDef,  # (1)
    Filters: NotRequired[NotificationFilterConfigOutputTypeDef],  # (2)
```

1. See [:material-code-braces: SnsChannelConfigTypeDef](./type_defs.md#snschannelconfigtypedef) 
2. See [:material-code-braces: NotificationFilterConfigOutputTypeDef](./type_defs.md#notificationfilterconfigoutputtypedef) 
## UpdateServiceIntegrationConfigTypeDef

```python
# UpdateServiceIntegrationConfigTypeDef definition

class UpdateServiceIntegrationConfigTypeDef(TypedDict):
    OpsCenter: NotRequired[OpsCenterIntegrationConfigTypeDef],  # (1)
    LogsAnomalyDetection: NotRequired[LogsAnomalyDetectionIntegrationConfigTypeDef],  # (2)
    KMSServerSideEncryption: NotRequired[KMSServerSideEncryptionIntegrationConfigTypeDef],  # (3)
```

1. See [:material-code-braces: OpsCenterIntegrationConfigTypeDef](./type_defs.md#opscenterintegrationconfigtypedef) 
2. See [:material-code-braces: LogsAnomalyDetectionIntegrationConfigTypeDef](./type_defs.md#logsanomalydetectionintegrationconfigtypedef) 
3. See [:material-code-braces: KMSServerSideEncryptionIntegrationConfigTypeDef](./type_defs.md#kmsserversideencryptionintegrationconfigtypedef) 
## ServiceIntegrationConfigTypeDef

```python
# ServiceIntegrationConfigTypeDef definition

class ServiceIntegrationConfigTypeDef(TypedDict):
    OpsCenter: NotRequired[OpsCenterIntegrationTypeDef],  # (1)
    LogsAnomalyDetection: NotRequired[LogsAnomalyDetectionIntegrationTypeDef],  # (2)
    KMSServerSideEncryption: NotRequired[KMSServerSideEncryptionIntegrationTypeDef],  # (3)
```

1. See [:material-code-braces: OpsCenterIntegrationTypeDef](./type_defs.md#opscenterintegrationtypedef) 
2. See [:material-code-braces: LogsAnomalyDetectionIntegrationTypeDef](./type_defs.md#logsanomalydetectionintegrationtypedef) 
3. See [:material-code-braces: KMSServerSideEncryptionIntegrationTypeDef](./type_defs.md#kmsserversideencryptionintegrationtypedef) 
## PerformanceInsightsMetricQueryTypeDef

```python
# PerformanceInsightsMetricQueryTypeDef definition

class PerformanceInsightsMetricQueryTypeDef(TypedDict):
    Metric: NotRequired[str],
    GroupBy: NotRequired[PerformanceInsightsMetricDimensionGroupTypeDef],  # (1)
    Filter: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: PerformanceInsightsMetricDimensionGroupTypeDef](./type_defs.md#performanceinsightsmetricdimensiongrouptypedef) 
## RecommendationRelatedAnomalySourceDetailTypeDef

```python
# RecommendationRelatedAnomalySourceDetailTypeDef definition

class RecommendationRelatedAnomalySourceDetailTypeDef(TypedDict):
    CloudWatchMetrics: NotRequired[List[RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef](./type_defs.md#recommendationrelatedcloudwatchmetricssourcedetailtypedef) 
## RecommendationRelatedEventTypeDef

```python
# RecommendationRelatedEventTypeDef definition

class RecommendationRelatedEventTypeDef(TypedDict):
    Name: NotRequired[str],
    Resources: NotRequired[List[RecommendationRelatedEventResourceTypeDef]],  # (1)
```

1. See [:material-code-braces: RecommendationRelatedEventResourceTypeDef](./type_defs.md#recommendationrelatedeventresourcetypedef) 
## ResourceCollectionFilterTypeDef

```python
# ResourceCollectionFilterTypeDef definition

class ResourceCollectionFilterTypeDef(TypedDict):
    CloudFormation: NotRequired[CloudFormationCollectionFilterTypeDef],  # (1)
    Tags: NotRequired[List[TagCollectionFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: CloudFormationCollectionFilterTypeDef](./type_defs.md#cloudformationcollectionfiltertypedef) 
2. See [:material-code-braces: TagCollectionFilterTypeDef](./type_defs.md#tagcollectionfiltertypedef) 
## ResourceCollectionOutputTypeDef

```python
# ResourceCollectionOutputTypeDef definition

class ResourceCollectionOutputTypeDef(TypedDict):
    CloudFormation: NotRequired[CloudFormationCollectionOutputTypeDef],  # (1)
    Tags: NotRequired[List[TagCollectionOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: CloudFormationCollectionOutputTypeDef](./type_defs.md#cloudformationcollectionoutputtypedef) 
2. See [:material-code-braces: TagCollectionOutputTypeDef](./type_defs.md#tagcollectionoutputtypedef) 
## ResourceCollectionTypeDef

```python
# ResourceCollectionTypeDef definition

class ResourceCollectionTypeDef(TypedDict):
    CloudFormation: NotRequired[CloudFormationCollectionTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagCollectionTypeDef]],  # (2)
```

1. See [:material-code-braces: CloudFormationCollectionTypeDef](./type_defs.md#cloudformationcollectiontypedef) 
2. See [:material-code-braces: TagCollectionTypeDef](./type_defs.md#tagcollectiontypedef) 
## ServiceHealthTypeDef

```python
# ServiceHealthTypeDef definition

class ServiceHealthTypeDef(TypedDict):
    ServiceName: NotRequired[ServiceNameType],  # (1)
    Insight: NotRequired[ServiceInsightHealthTypeDef],  # (2)
    AnalyzedResourceCount: NotRequired[int],
```

1. See [:material-code-brackets: ServiceNameType](./literals.md#servicenametype) 
2. See [:material-code-braces: ServiceInsightHealthTypeDef](./type_defs.md#serviceinsighthealthtypedef) 
## UpdateResourceCollectionFilterTypeDef

```python
# UpdateResourceCollectionFilterTypeDef definition

class UpdateResourceCollectionFilterTypeDef(TypedDict):
    CloudFormation: NotRequired[UpdateCloudFormationCollectionFilterTypeDef],  # (1)
    Tags: NotRequired[Sequence[UpdateTagCollectionFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: UpdateCloudFormationCollectionFilterTypeDef](./type_defs.md#updatecloudformationcollectionfiltertypedef) 
2. See [:material-code-braces: UpdateTagCollectionFilterTypeDef](./type_defs.md#updatetagcollectionfiltertypedef) 
## DescribeEventSourcesConfigResponseTypeDef

```python
# DescribeEventSourcesConfigResponseTypeDef definition

class DescribeEventSourcesConfigResponseTypeDef(TypedDict):
    EventSources: EventSourcesConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSourcesConfigTypeDef](./type_defs.md#eventsourcesconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEventSourcesConfigRequestRequestTypeDef

```python
# UpdateEventSourcesConfigRequestRequestTypeDef definition

class UpdateEventSourcesConfigRequestRequestTypeDef(TypedDict):
    EventSources: NotRequired[EventSourcesConfigTypeDef],  # (1)
```

1. See [:material-code-braces: EventSourcesConfigTypeDef](./type_defs.md#eventsourcesconfigtypedef) 
## CloudWatchMetricsDetailTypeDef

```python
# CloudWatchMetricsDetailTypeDef definition

class CloudWatchMetricsDetailTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
    Dimensions: NotRequired[List[CloudWatchMetricsDimensionTypeDef]],  # (1)
    Stat: NotRequired[CloudWatchMetricsStatType],  # (2)
    Unit: NotRequired[str],
    Period: NotRequired[int],
    MetricDataSummary: NotRequired[CloudWatchMetricsDataSummaryTypeDef],  # (3)
```

1. See [:material-code-braces: CloudWatchMetricsDimensionTypeDef](./type_defs.md#cloudwatchmetricsdimensiontypedef) 
2. See [:material-code-brackets: CloudWatchMetricsStatType](./literals.md#cloudwatchmetricsstattype) 
3. See [:material-code-braces: CloudWatchMetricsDataSummaryTypeDef](./type_defs.md#cloudwatchmetricsdatasummarytypedef) 
## GetCostEstimationResponseTypeDef

```python
# GetCostEstimationResponseTypeDef definition

class GetCostEstimationResponseTypeDef(TypedDict):
    ResourceCollection: CostEstimationResourceCollectionFilterOutputTypeDef,  # (1)
    Status: CostEstimationStatusType,  # (2)
    Costs: List[ServiceResourceCostTypeDef],  # (3)
    TimeRange: CostEstimationTimeRangeTypeDef,  # (4)
    TotalCost: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CostEstimationResourceCollectionFilterOutputTypeDef](./type_defs.md#costestimationresourcecollectionfilteroutputtypedef) 
2. See [:material-code-brackets: CostEstimationStatusType](./literals.md#costestimationstatustype) 
3. See [:material-code-braces: ServiceResourceCostTypeDef](./type_defs.md#serviceresourcecosttypedef) 
4. See [:material-code-braces: CostEstimationTimeRangeTypeDef](./type_defs.md#costestimationtimerangetypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInsightsClosedStatusFilterTypeDef

```python
# ListInsightsClosedStatusFilterTypeDef definition

class ListInsightsClosedStatusFilterTypeDef(TypedDict):
    Type: InsightTypeType,  # (1)
    EndTimeRange: EndTimeRangeTypeDef,  # (2)
```

1. See [:material-code-brackets: InsightTypeType](./literals.md#insighttypetype) 
2. See [:material-code-braces: EndTimeRangeTypeDef](./type_defs.md#endtimerangetypedef) 
## ListInsightsAnyStatusFilterTypeDef

```python
# ListInsightsAnyStatusFilterTypeDef definition

class ListInsightsAnyStatusFilterTypeDef(TypedDict):
    Type: InsightTypeType,  # (1)
    StartTimeRange: StartTimeRangeTypeDef,  # (2)
```

1. See [:material-code-brackets: InsightTypeType](./literals.md#insighttypetype) 
2. See [:material-code-braces: StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) 
## ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef

```python
# ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef definition

class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(TypedDict):
    InsightId: str,
    StartTimeRange: NotRequired[StartTimeRangeTypeDef],  # (1)
    AccountId: NotRequired[str],
    Filters: NotRequired[ListAnomaliesForInsightFiltersTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) 
2. See [:material-code-braces: ListAnomaliesForInsightFiltersTypeDef](./type_defs.md#listanomaliesforinsightfilterstypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAnomaliesForInsightRequestRequestTypeDef

```python
# ListAnomaliesForInsightRequestRequestTypeDef definition

class ListAnomaliesForInsightRequestRequestTypeDef(TypedDict):
    InsightId: str,
    StartTimeRange: NotRequired[StartTimeRangeTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    AccountId: NotRequired[str],
    Filters: NotRequired[ListAnomaliesForInsightFiltersTypeDef],  # (2)
```

1. See [:material-code-braces: StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) 
2. See [:material-code-braces: ListAnomaliesForInsightFiltersTypeDef](./type_defs.md#listanomaliesforinsightfilterstypedef) 
## AnomalousLogGroupTypeDef

```python
# AnomalousLogGroupTypeDef definition

class AnomalousLogGroupTypeDef(TypedDict):
    LogGroupName: NotRequired[str],
    ImpactStartTime: NotRequired[datetime],
    ImpactEndTime: NotRequired[datetime],
    NumberOfLogLinesScanned: NotRequired[int],
    LogAnomalyShowcases: NotRequired[List[LogAnomalyShowcaseTypeDef]],  # (1)
```

1. See [:material-code-braces: LogAnomalyShowcaseTypeDef](./type_defs.md#loganomalyshowcasetypedef) 
## NotificationChannelTypeDef

```python
# NotificationChannelTypeDef definition

class NotificationChannelTypeDef(TypedDict):
    Id: NotRequired[str],
    Config: NotRequired[NotificationChannelConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: NotificationChannelConfigOutputTypeDef](./type_defs.md#notificationchannelconfigoutputtypedef) 
## NotificationChannelConfigTypeDef

```python
# NotificationChannelConfigTypeDef definition

class NotificationChannelConfigTypeDef(TypedDict):
    Sns: SnsChannelConfigTypeDef,  # (1)
    Filters: NotRequired[NotificationFilterConfigUnionTypeDef],  # (2)
```

1. See [:material-code-braces: SnsChannelConfigTypeDef](./type_defs.md#snschannelconfigtypedef) 
2. See [:material-code-braces: NotificationFilterConfigTypeDef](./type_defs.md#notificationfilterconfigtypedef) [:material-code-braces: NotificationFilterConfigOutputTypeDef](./type_defs.md#notificationfilterconfigoutputtypedef) 
## UpdateServiceIntegrationRequestRequestTypeDef

```python
# UpdateServiceIntegrationRequestRequestTypeDef definition

class UpdateServiceIntegrationRequestRequestTypeDef(TypedDict):
    ServiceIntegration: UpdateServiceIntegrationConfigTypeDef,  # (1)
```

1. See [:material-code-braces: UpdateServiceIntegrationConfigTypeDef](./type_defs.md#updateserviceintegrationconfigtypedef) 
## DescribeServiceIntegrationResponseTypeDef

```python
# DescribeServiceIntegrationResponseTypeDef definition

class DescribeServiceIntegrationResponseTypeDef(TypedDict):
    ServiceIntegration: ServiceIntegrationConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceIntegrationConfigTypeDef](./type_defs.md#serviceintegrationconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PerformanceInsightsReferenceMetricTypeDef

```python
# PerformanceInsightsReferenceMetricTypeDef definition

class PerformanceInsightsReferenceMetricTypeDef(TypedDict):
    MetricQuery: NotRequired[PerformanceInsightsMetricQueryTypeDef],  # (1)
```

1. See [:material-code-braces: PerformanceInsightsMetricQueryTypeDef](./type_defs.md#performanceinsightsmetricquerytypedef) 
## RecommendationRelatedAnomalyTypeDef

```python
# RecommendationRelatedAnomalyTypeDef definition

class RecommendationRelatedAnomalyTypeDef(TypedDict):
    Resources: NotRequired[List[RecommendationRelatedAnomalyResourceTypeDef]],  # (1)
    SourceDetails: NotRequired[List[RecommendationRelatedAnomalySourceDetailTypeDef]],  # (2)
    AnomalyId: NotRequired[str],
```

1. See [:material-code-braces: RecommendationRelatedAnomalyResourceTypeDef](./type_defs.md#recommendationrelatedanomalyresourcetypedef) 
2. See [:material-code-braces: RecommendationRelatedAnomalySourceDetailTypeDef](./type_defs.md#recommendationrelatedanomalysourcedetailtypedef) 
## GetResourceCollectionResponseTypeDef

```python
# GetResourceCollectionResponseTypeDef definition

class GetResourceCollectionResponseTypeDef(TypedDict):
    ResourceCollection: ResourceCollectionFilterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceCollectionFilterTypeDef](./type_defs.md#resourcecollectionfiltertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (1)
    Id: NotRequired[str],
    Time: NotRequired[datetime],
    EventSource: NotRequired[str],
    Name: NotRequired[str],
    DataSource: NotRequired[EventDataSourceType],  # (2)
    EventClass: NotRequired[EventClassType],  # (3)
    Resources: NotRequired[List[EventResourceTypeDef]],  # (4)
```

1. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
2. See [:material-code-brackets: EventDataSourceType](./literals.md#eventdatasourcetype) 
3. See [:material-code-brackets: EventClassType](./literals.md#eventclasstype) 
4. See [:material-code-braces: EventResourceTypeDef](./type_defs.md#eventresourcetypedef) 
## MonitoredResourceIdentifierTypeDef

```python
# MonitoredResourceIdentifierTypeDef definition

class MonitoredResourceIdentifierTypeDef(TypedDict):
    MonitoredResourceName: NotRequired[str],
    Type: NotRequired[str],
    ResourcePermission: NotRequired[ResourcePermissionType],  # (1)
    LastUpdated: NotRequired[datetime],
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourcePermissionType](./literals.md#resourcepermissiontype) 
2. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
## ProactiveInsightSummaryTypeDef

```python
# ProactiveInsightSummaryTypeDef definition

class ProactiveInsightSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Severity: NotRequired[InsightSeverityType],  # (1)
    Status: NotRequired[InsightStatusType],  # (2)
    InsightTimeRange: NotRequired[InsightTimeRangeTypeDef],  # (3)
    PredictionTimeRange: NotRequired[PredictionTimeRangeTypeDef],  # (4)
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (5)
    ServiceCollection: NotRequired[ServiceCollectionOutputTypeDef],  # (6)
    AssociatedResourceArns: NotRequired[List[str]],
```

1. See [:material-code-brackets: InsightSeverityType](./literals.md#insightseveritytype) 
2. See [:material-code-brackets: InsightStatusType](./literals.md#insightstatustype) 
3. See [:material-code-braces: InsightTimeRangeTypeDef](./type_defs.md#insighttimerangetypedef) 
4. See [:material-code-braces: PredictionTimeRangeTypeDef](./type_defs.md#predictiontimerangetypedef) 
5. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
6. See [:material-code-braces: ServiceCollectionOutputTypeDef](./type_defs.md#servicecollectionoutputtypedef) 
## ProactiveInsightTypeDef

```python
# ProactiveInsightTypeDef definition

class ProactiveInsightTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Severity: NotRequired[InsightSeverityType],  # (1)
    Status: NotRequired[InsightStatusType],  # (2)
    InsightTimeRange: NotRequired[InsightTimeRangeTypeDef],  # (3)
    PredictionTimeRange: NotRequired[PredictionTimeRangeTypeDef],  # (4)
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (5)
    SsmOpsItemId: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: InsightSeverityType](./literals.md#insightseveritytype) 
2. See [:material-code-brackets: InsightStatusType](./literals.md#insightstatustype) 
3. See [:material-code-braces: InsightTimeRangeTypeDef](./type_defs.md#insighttimerangetypedef) 
4. See [:material-code-braces: PredictionTimeRangeTypeDef](./type_defs.md#predictiontimerangetypedef) 
5. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
## ProactiveOrganizationInsightSummaryTypeDef

```python
# ProactiveOrganizationInsightSummaryTypeDef definition

class ProactiveOrganizationInsightSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    AccountId: NotRequired[str],
    OrganizationalUnitId: NotRequired[str],
    Name: NotRequired[str],
    Severity: NotRequired[InsightSeverityType],  # (1)
    Status: NotRequired[InsightStatusType],  # (2)
    InsightTimeRange: NotRequired[InsightTimeRangeTypeDef],  # (3)
    PredictionTimeRange: NotRequired[PredictionTimeRangeTypeDef],  # (4)
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (5)
    ServiceCollection: NotRequired[ServiceCollectionOutputTypeDef],  # (6)
```

1. See [:material-code-brackets: InsightSeverityType](./literals.md#insightseveritytype) 
2. See [:material-code-brackets: InsightStatusType](./literals.md#insightstatustype) 
3. See [:material-code-braces: InsightTimeRangeTypeDef](./type_defs.md#insighttimerangetypedef) 
4. See [:material-code-braces: PredictionTimeRangeTypeDef](./type_defs.md#predictiontimerangetypedef) 
5. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
6. See [:material-code-braces: ServiceCollectionOutputTypeDef](./type_defs.md#servicecollectionoutputtypedef) 
## ReactiveInsightSummaryTypeDef

```python
# ReactiveInsightSummaryTypeDef definition

class ReactiveInsightSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Severity: NotRequired[InsightSeverityType],  # (1)
    Status: NotRequired[InsightStatusType],  # (2)
    InsightTimeRange: NotRequired[InsightTimeRangeTypeDef],  # (3)
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (4)
    ServiceCollection: NotRequired[ServiceCollectionOutputTypeDef],  # (5)
    AssociatedResourceArns: NotRequired[List[str]],
```

1. See [:material-code-brackets: InsightSeverityType](./literals.md#insightseveritytype) 
2. See [:material-code-brackets: InsightStatusType](./literals.md#insightstatustype) 
3. See [:material-code-braces: InsightTimeRangeTypeDef](./type_defs.md#insighttimerangetypedef) 
4. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
5. See [:material-code-braces: ServiceCollectionOutputTypeDef](./type_defs.md#servicecollectionoutputtypedef) 
## ReactiveInsightTypeDef

```python
# ReactiveInsightTypeDef definition

class ReactiveInsightTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Severity: NotRequired[InsightSeverityType],  # (1)
    Status: NotRequired[InsightStatusType],  # (2)
    InsightTimeRange: NotRequired[InsightTimeRangeTypeDef],  # (3)
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (4)
    SsmOpsItemId: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: InsightSeverityType](./literals.md#insightseveritytype) 
2. See [:material-code-brackets: InsightStatusType](./literals.md#insightstatustype) 
3. See [:material-code-braces: InsightTimeRangeTypeDef](./type_defs.md#insighttimerangetypedef) 
4. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
## ReactiveOrganizationInsightSummaryTypeDef

```python
# ReactiveOrganizationInsightSummaryTypeDef definition

class ReactiveOrganizationInsightSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    AccountId: NotRequired[str],
    OrganizationalUnitId: NotRequired[str],
    Name: NotRequired[str],
    Severity: NotRequired[InsightSeverityType],  # (1)
    Status: NotRequired[InsightStatusType],  # (2)
    InsightTimeRange: NotRequired[InsightTimeRangeTypeDef],  # (3)
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (4)
    ServiceCollection: NotRequired[ServiceCollectionOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: InsightSeverityType](./literals.md#insightseveritytype) 
2. See [:material-code-brackets: InsightStatusType](./literals.md#insightstatustype) 
3. See [:material-code-braces: InsightTimeRangeTypeDef](./type_defs.md#insighttimerangetypedef) 
4. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
5. See [:material-code-braces: ServiceCollectionOutputTypeDef](./type_defs.md#servicecollectionoutputtypedef) 
## ListEventsFiltersTypeDef

```python
# ListEventsFiltersTypeDef definition

class ListEventsFiltersTypeDef(TypedDict):
    InsightId: NotRequired[str],
    EventTimeRange: NotRequired[EventTimeRangeTypeDef],  # (1)
    EventClass: NotRequired[EventClassType],  # (2)
    EventSource: NotRequired[str],
    DataSource: NotRequired[EventDataSourceType],  # (3)
    ResourceCollection: NotRequired[ResourceCollectionTypeDef],  # (4)
```

1. See [:material-code-braces: EventTimeRangeTypeDef](./type_defs.md#eventtimerangetypedef) 
2. See [:material-code-brackets: EventClassType](./literals.md#eventclasstype) 
3. See [:material-code-brackets: EventDataSourceType](./literals.md#eventdatasourcetype) 
4. See [:material-code-braces: ResourceCollectionTypeDef](./type_defs.md#resourcecollectiontypedef) 
## DescribeOrganizationResourceCollectionHealthResponseTypeDef

```python
# DescribeOrganizationResourceCollectionHealthResponseTypeDef definition

class DescribeOrganizationResourceCollectionHealthResponseTypeDef(TypedDict):
    CloudFormation: List[CloudFormationHealthTypeDef],  # (1)
    Service: List[ServiceHealthTypeDef],  # (2)
    Account: List[AccountHealthTypeDef],  # (3)
    Tags: List[TagHealthTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CloudFormationHealthTypeDef](./type_defs.md#cloudformationhealthtypedef) 
2. See [:material-code-braces: ServiceHealthTypeDef](./type_defs.md#servicehealthtypedef) 
3. See [:material-code-braces: AccountHealthTypeDef](./type_defs.md#accounthealthtypedef) 
4. See [:material-code-braces: TagHealthTypeDef](./type_defs.md#taghealthtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourceCollectionHealthResponseTypeDef

```python
# DescribeResourceCollectionHealthResponseTypeDef definition

class DescribeResourceCollectionHealthResponseTypeDef(TypedDict):
    CloudFormation: List[CloudFormationHealthTypeDef],  # (1)
    Service: List[ServiceHealthTypeDef],  # (2)
    Tags: List[TagHealthTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CloudFormationHealthTypeDef](./type_defs.md#cloudformationhealthtypedef) 
2. See [:material-code-braces: ServiceHealthTypeDef](./type_defs.md#servicehealthtypedef) 
3. See [:material-code-braces: TagHealthTypeDef](./type_defs.md#taghealthtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CostEstimationResourceCollectionFilterTypeDef

```python
# CostEstimationResourceCollectionFilterTypeDef definition

class CostEstimationResourceCollectionFilterTypeDef(TypedDict):
    CloudFormation: NotRequired[CloudFormationCostEstimationResourceCollectionFilterUnionTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagCostEstimationResourceCollectionFilterUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: CloudFormationCostEstimationResourceCollectionFilterTypeDef](./type_defs.md#cloudformationcostestimationresourcecollectionfiltertypedef) [:material-code-braces: CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef](./type_defs.md#cloudformationcostestimationresourcecollectionfilteroutputtypedef) 
2. See [:material-code-braces: TagCostEstimationResourceCollectionFilterTypeDef](./type_defs.md#tagcostestimationresourcecollectionfiltertypedef) [:material-code-braces: TagCostEstimationResourceCollectionFilterOutputTypeDef](./type_defs.md#tagcostestimationresourcecollectionfilteroutputtypedef) 
## UpdateResourceCollectionRequestRequestTypeDef

```python
# UpdateResourceCollectionRequestRequestTypeDef definition

class UpdateResourceCollectionRequestRequestTypeDef(TypedDict):
    Action: UpdateResourceCollectionActionType,  # (1)
    ResourceCollection: UpdateResourceCollectionFilterTypeDef,  # (2)
```

1. See [:material-code-brackets: UpdateResourceCollectionActionType](./literals.md#updateresourcecollectionactiontype) 
2. See [:material-code-braces: UpdateResourceCollectionFilterTypeDef](./type_defs.md#updateresourcecollectionfiltertypedef) 
## ListInsightsStatusFilterTypeDef

```python
# ListInsightsStatusFilterTypeDef definition

class ListInsightsStatusFilterTypeDef(TypedDict):
    Ongoing: NotRequired[ListInsightsOngoingStatusFilterTypeDef],  # (1)
    Closed: NotRequired[ListInsightsClosedStatusFilterTypeDef],  # (2)
    Any: NotRequired[ListInsightsAnyStatusFilterTypeDef],  # (3)
```

1. See [:material-code-braces: ListInsightsOngoingStatusFilterTypeDef](./type_defs.md#listinsightsongoingstatusfiltertypedef) 
2. See [:material-code-braces: ListInsightsClosedStatusFilterTypeDef](./type_defs.md#listinsightsclosedstatusfiltertypedef) 
3. See [:material-code-braces: ListInsightsAnyStatusFilterTypeDef](./type_defs.md#listinsightsanystatusfiltertypedef) 
## ListAnomalousLogGroupsResponseTypeDef

```python
# ListAnomalousLogGroupsResponseTypeDef definition

class ListAnomalousLogGroupsResponseTypeDef(TypedDict):
    InsightId: str,
    AnomalousLogGroups: List[AnomalousLogGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AnomalousLogGroupTypeDef](./type_defs.md#anomalousloggrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNotificationChannelsResponseTypeDef

```python
# ListNotificationChannelsResponseTypeDef definition

class ListNotificationChannelsResponseTypeDef(TypedDict):
    Channels: List[NotificationChannelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NotificationChannelTypeDef](./type_defs.md#notificationchanneltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddNotificationChannelRequestRequestTypeDef

```python
# AddNotificationChannelRequestRequestTypeDef definition

class AddNotificationChannelRequestRequestTypeDef(TypedDict):
    Config: NotificationChannelConfigTypeDef,  # (1)
```

1. See [:material-code-braces: NotificationChannelConfigTypeDef](./type_defs.md#notificationchannelconfigtypedef) 
## PerformanceInsightsReferenceComparisonValuesTypeDef

```python
# PerformanceInsightsReferenceComparisonValuesTypeDef definition

class PerformanceInsightsReferenceComparisonValuesTypeDef(TypedDict):
    ReferenceScalar: NotRequired[PerformanceInsightsReferenceScalarTypeDef],  # (1)
    ReferenceMetric: NotRequired[PerformanceInsightsReferenceMetricTypeDef],  # (2)
```

1. See [:material-code-braces: PerformanceInsightsReferenceScalarTypeDef](./type_defs.md#performanceinsightsreferencescalartypedef) 
2. See [:material-code-braces: PerformanceInsightsReferenceMetricTypeDef](./type_defs.md#performanceinsightsreferencemetrictypedef) 
## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    Description: NotRequired[str],
    Link: NotRequired[str],
    Name: NotRequired[str],
    Reason: NotRequired[str],
    RelatedEvents: NotRequired[List[RecommendationRelatedEventTypeDef]],  # (1)
    RelatedAnomalies: NotRequired[List[RecommendationRelatedAnomalyTypeDef]],  # (2)
    Category: NotRequired[str],
```

1. See [:material-code-braces: RecommendationRelatedEventTypeDef](./type_defs.md#recommendationrelatedeventtypedef) 
2. See [:material-code-braces: RecommendationRelatedAnomalyTypeDef](./type_defs.md#recommendationrelatedanomalytypedef) 
## ListEventsResponseTypeDef

```python
# ListEventsResponseTypeDef definition

class ListEventsResponseTypeDef(TypedDict):
    Events: List[EventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMonitoredResourcesResponseTypeDef

```python
# ListMonitoredResourcesResponseTypeDef definition

class ListMonitoredResourcesResponseTypeDef(TypedDict):
    MonitoredResourceIdentifiers: List[MonitoredResourceIdentifierTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MonitoredResourceIdentifierTypeDef](./type_defs.md#monitoredresourceidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInsightsResponseTypeDef

```python
# ListInsightsResponseTypeDef definition

class ListInsightsResponseTypeDef(TypedDict):
    ProactiveInsights: List[ProactiveInsightSummaryTypeDef],  # (1)
    ReactiveInsights: List[ReactiveInsightSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProactiveInsightSummaryTypeDef](./type_defs.md#proactiveinsightsummarytypedef) 
2. See [:material-code-braces: ReactiveInsightSummaryTypeDef](./type_defs.md#reactiveinsightsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchInsightsResponseTypeDef

```python
# SearchInsightsResponseTypeDef definition

class SearchInsightsResponseTypeDef(TypedDict):
    ProactiveInsights: List[ProactiveInsightSummaryTypeDef],  # (1)
    ReactiveInsights: List[ReactiveInsightSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProactiveInsightSummaryTypeDef](./type_defs.md#proactiveinsightsummarytypedef) 
2. See [:material-code-braces: ReactiveInsightSummaryTypeDef](./type_defs.md#reactiveinsightsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchOrganizationInsightsResponseTypeDef

```python
# SearchOrganizationInsightsResponseTypeDef definition

class SearchOrganizationInsightsResponseTypeDef(TypedDict):
    ProactiveInsights: List[ProactiveInsightSummaryTypeDef],  # (1)
    ReactiveInsights: List[ReactiveInsightSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProactiveInsightSummaryTypeDef](./type_defs.md#proactiveinsightsummarytypedef) 
2. See [:material-code-braces: ReactiveInsightSummaryTypeDef](./type_defs.md#reactiveinsightsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInsightResponseTypeDef

```python
# DescribeInsightResponseTypeDef definition

class DescribeInsightResponseTypeDef(TypedDict):
    ProactiveInsight: ProactiveInsightTypeDef,  # (1)
    ReactiveInsight: ReactiveInsightTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProactiveInsightTypeDef](./type_defs.md#proactiveinsighttypedef) 
2. See [:material-code-braces: ReactiveInsightTypeDef](./type_defs.md#reactiveinsighttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrganizationInsightsResponseTypeDef

```python
# ListOrganizationInsightsResponseTypeDef definition

class ListOrganizationInsightsResponseTypeDef(TypedDict):
    ProactiveInsights: List[ProactiveOrganizationInsightSummaryTypeDef],  # (1)
    ReactiveInsights: List[ReactiveOrganizationInsightSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProactiveOrganizationInsightSummaryTypeDef](./type_defs.md#proactiveorganizationinsightsummarytypedef) 
2. See [:material-code-braces: ReactiveOrganizationInsightSummaryTypeDef](./type_defs.md#reactiveorganizationinsightsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventsRequestListEventsPaginateTypeDef

```python
# ListEventsRequestListEventsPaginateTypeDef definition

class ListEventsRequestListEventsPaginateTypeDef(TypedDict):
    Filters: ListEventsFiltersTypeDef,  # (1)
    AccountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListEventsFiltersTypeDef](./type_defs.md#listeventsfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEventsRequestRequestTypeDef

```python
# ListEventsRequestRequestTypeDef definition

class ListEventsRequestRequestTypeDef(TypedDict):
    Filters: ListEventsFiltersTypeDef,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    AccountId: NotRequired[str],
```

1. See [:material-code-braces: ListEventsFiltersTypeDef](./type_defs.md#listeventsfilterstypedef) 
## SearchInsightsFiltersTypeDef

```python
# SearchInsightsFiltersTypeDef definition

class SearchInsightsFiltersTypeDef(TypedDict):
    Severities: NotRequired[Sequence[InsightSeverityType]],  # (1)
    Statuses: NotRequired[Sequence[InsightStatusType]],  # (2)
    ResourceCollection: NotRequired[ResourceCollectionUnionTypeDef],  # (3)
    ServiceCollection: NotRequired[ServiceCollectionUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: InsightSeverityType](./literals.md#insightseveritytype) 
2. See [:material-code-brackets: InsightStatusType](./literals.md#insightstatustype) 
3. See [:material-code-braces: ResourceCollectionTypeDef](./type_defs.md#resourcecollectiontypedef) [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
4. See [:material-code-braces: ServiceCollectionTypeDef](./type_defs.md#servicecollectiontypedef) [:material-code-braces: ServiceCollectionOutputTypeDef](./type_defs.md#servicecollectionoutputtypedef) 
## SearchOrganizationInsightsFiltersTypeDef

```python
# SearchOrganizationInsightsFiltersTypeDef definition

class SearchOrganizationInsightsFiltersTypeDef(TypedDict):
    Severities: NotRequired[Sequence[InsightSeverityType]],  # (1)
    Statuses: NotRequired[Sequence[InsightStatusType]],  # (2)
    ResourceCollection: NotRequired[ResourceCollectionUnionTypeDef],  # (3)
    ServiceCollection: NotRequired[ServiceCollectionUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: InsightSeverityType](./literals.md#insightseveritytype) 
2. See [:material-code-brackets: InsightStatusType](./literals.md#insightstatustype) 
3. See [:material-code-braces: ResourceCollectionTypeDef](./type_defs.md#resourcecollectiontypedef) [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
4. See [:material-code-braces: ServiceCollectionTypeDef](./type_defs.md#servicecollectiontypedef) [:material-code-braces: ServiceCollectionOutputTypeDef](./type_defs.md#servicecollectionoutputtypedef) 
## StartCostEstimationRequestRequestTypeDef

```python
# StartCostEstimationRequestRequestTypeDef definition

class StartCostEstimationRequestRequestTypeDef(TypedDict):
    ResourceCollection: CostEstimationResourceCollectionFilterTypeDef,  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: CostEstimationResourceCollectionFilterTypeDef](./type_defs.md#costestimationresourcecollectionfiltertypedef) 
## ListInsightsRequestListInsightsPaginateTypeDef

```python
# ListInsightsRequestListInsightsPaginateTypeDef definition

class ListInsightsRequestListInsightsPaginateTypeDef(TypedDict):
    StatusFilter: ListInsightsStatusFilterTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListInsightsStatusFilterTypeDef](./type_defs.md#listinsightsstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInsightsRequestRequestTypeDef

```python
# ListInsightsRequestRequestTypeDef definition

class ListInsightsRequestRequestTypeDef(TypedDict):
    StatusFilter: ListInsightsStatusFilterTypeDef,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListInsightsStatusFilterTypeDef](./type_defs.md#listinsightsstatusfiltertypedef) 
## ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef

```python
# ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef definition

class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(TypedDict):
    StatusFilter: ListInsightsStatusFilterTypeDef,  # (1)
    AccountIds: NotRequired[Sequence[str]],
    OrganizationalUnitIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListInsightsStatusFilterTypeDef](./type_defs.md#listinsightsstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationInsightsRequestRequestTypeDef

```python
# ListOrganizationInsightsRequestRequestTypeDef definition

class ListOrganizationInsightsRequestRequestTypeDef(TypedDict):
    StatusFilter: ListInsightsStatusFilterTypeDef,  # (1)
    MaxResults: NotRequired[int],
    AccountIds: NotRequired[Sequence[str]],
    OrganizationalUnitIds: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListInsightsStatusFilterTypeDef](./type_defs.md#listinsightsstatusfiltertypedef) 
## PerformanceInsightsReferenceDataTypeDef

```python
# PerformanceInsightsReferenceDataTypeDef definition

class PerformanceInsightsReferenceDataTypeDef(TypedDict):
    Name: NotRequired[str],
    ComparisonValues: NotRequired[PerformanceInsightsReferenceComparisonValuesTypeDef],  # (1)
```

1. See [:material-code-braces: PerformanceInsightsReferenceComparisonValuesTypeDef](./type_defs.md#performanceinsightsreferencecomparisonvaluestypedef) 
## ListRecommendationsResponseTypeDef

```python
# ListRecommendationsResponseTypeDef definition

class ListRecommendationsResponseTypeDef(TypedDict):
    Recommendations: List[RecommendationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchInsightsRequestRequestTypeDef

```python
# SearchInsightsRequestRequestTypeDef definition

class SearchInsightsRequestRequestTypeDef(TypedDict):
    StartTimeRange: StartTimeRangeTypeDef,  # (1)
    Type: InsightTypeType,  # (2)
    Filters: NotRequired[SearchInsightsFiltersTypeDef],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) 
2. See [:material-code-brackets: InsightTypeType](./literals.md#insighttypetype) 
3. See [:material-code-braces: SearchInsightsFiltersTypeDef](./type_defs.md#searchinsightsfilterstypedef) 
## SearchInsightsRequestSearchInsightsPaginateTypeDef

```python
# SearchInsightsRequestSearchInsightsPaginateTypeDef definition

class SearchInsightsRequestSearchInsightsPaginateTypeDef(TypedDict):
    StartTimeRange: StartTimeRangeTypeDef,  # (1)
    Type: InsightTypeType,  # (2)
    Filters: NotRequired[SearchInsightsFiltersTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) 
2. See [:material-code-brackets: InsightTypeType](./literals.md#insighttypetype) 
3. See [:material-code-braces: SearchInsightsFiltersTypeDef](./type_defs.md#searchinsightsfilterstypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchOrganizationInsightsRequestRequestTypeDef

```python
# SearchOrganizationInsightsRequestRequestTypeDef definition

class SearchOrganizationInsightsRequestRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
    StartTimeRange: StartTimeRangeTypeDef,  # (1)
    Type: InsightTypeType,  # (2)
    Filters: NotRequired[SearchOrganizationInsightsFiltersTypeDef],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) 
2. See [:material-code-brackets: InsightTypeType](./literals.md#insighttypetype) 
3. See [:material-code-braces: SearchOrganizationInsightsFiltersTypeDef](./type_defs.md#searchorganizationinsightsfilterstypedef) 
## SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef

```python
# SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef definition

class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(TypedDict):
    AccountIds: Sequence[str],
    StartTimeRange: StartTimeRangeTypeDef,  # (1)
    Type: InsightTypeType,  # (2)
    Filters: NotRequired[SearchOrganizationInsightsFiltersTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: StartTimeRangeTypeDef](./type_defs.md#starttimerangetypedef) 
2. See [:material-code-brackets: InsightTypeType](./literals.md#insighttypetype) 
3. See [:material-code-braces: SearchOrganizationInsightsFiltersTypeDef](./type_defs.md#searchorganizationinsightsfilterstypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## PerformanceInsightsMetricsDetailTypeDef

```python
# PerformanceInsightsMetricsDetailTypeDef definition

class PerformanceInsightsMetricsDetailTypeDef(TypedDict):
    MetricDisplayName: NotRequired[str],
    Unit: NotRequired[str],
    MetricQuery: NotRequired[PerformanceInsightsMetricQueryTypeDef],  # (1)
    ReferenceData: NotRequired[List[PerformanceInsightsReferenceDataTypeDef]],  # (2)
    StatsAtAnomaly: NotRequired[List[PerformanceInsightsStatTypeDef]],  # (3)
    StatsAtBaseline: NotRequired[List[PerformanceInsightsStatTypeDef]],  # (3)
```

1. See [:material-code-braces: PerformanceInsightsMetricQueryTypeDef](./type_defs.md#performanceinsightsmetricquerytypedef) 
2. See [:material-code-braces: PerformanceInsightsReferenceDataTypeDef](./type_defs.md#performanceinsightsreferencedatatypedef) 
3. See [:material-code-braces: PerformanceInsightsStatTypeDef](./type_defs.md#performanceinsightsstattypedef) 
4. See [:material-code-braces: PerformanceInsightsStatTypeDef](./type_defs.md#performanceinsightsstattypedef) 
## AnomalySourceDetailsTypeDef

```python
# AnomalySourceDetailsTypeDef definition

class AnomalySourceDetailsTypeDef(TypedDict):
    CloudWatchMetrics: NotRequired[List[CloudWatchMetricsDetailTypeDef]],  # (1)
    PerformanceInsightsMetrics: NotRequired[List[PerformanceInsightsMetricsDetailTypeDef]],  # (2)
```

1. See [:material-code-braces: CloudWatchMetricsDetailTypeDef](./type_defs.md#cloudwatchmetricsdetailtypedef) 
2. See [:material-code-braces: PerformanceInsightsMetricsDetailTypeDef](./type_defs.md#performanceinsightsmetricsdetailtypedef) 
## ProactiveAnomalySummaryTypeDef

```python
# ProactiveAnomalySummaryTypeDef definition

class ProactiveAnomalySummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Severity: NotRequired[AnomalySeverityType],  # (1)
    Status: NotRequired[AnomalyStatusType],  # (2)
    UpdateTime: NotRequired[datetime],
    AnomalyTimeRange: NotRequired[AnomalyTimeRangeTypeDef],  # (3)
    AnomalyReportedTimeRange: NotRequired[AnomalyReportedTimeRangeTypeDef],  # (4)
    PredictionTimeRange: NotRequired[PredictionTimeRangeTypeDef],  # (5)
    SourceDetails: NotRequired[AnomalySourceDetailsTypeDef],  # (6)
    AssociatedInsightId: NotRequired[str],
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (7)
    Limit: NotRequired[float],
    SourceMetadata: NotRequired[AnomalySourceMetadataTypeDef],  # (8)
    AnomalyResources: NotRequired[List[AnomalyResourceTypeDef]],  # (9)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: AnomalySeverityType](./literals.md#anomalyseveritytype) 
2. See [:material-code-brackets: AnomalyStatusType](./literals.md#anomalystatustype) 
3. See [:material-code-braces: AnomalyTimeRangeTypeDef](./type_defs.md#anomalytimerangetypedef) 
4. See [:material-code-braces: AnomalyReportedTimeRangeTypeDef](./type_defs.md#anomalyreportedtimerangetypedef) 
5. See [:material-code-braces: PredictionTimeRangeTypeDef](./type_defs.md#predictiontimerangetypedef) 
6. See [:material-code-braces: AnomalySourceDetailsTypeDef](./type_defs.md#anomalysourcedetailstypedef) 
7. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
8. See [:material-code-braces: AnomalySourceMetadataTypeDef](./type_defs.md#anomalysourcemetadatatypedef) 
9. See [:material-code-braces: AnomalyResourceTypeDef](./type_defs.md#anomalyresourcetypedef) 
## ProactiveAnomalyTypeDef

```python
# ProactiveAnomalyTypeDef definition

class ProactiveAnomalyTypeDef(TypedDict):
    Id: NotRequired[str],
    Severity: NotRequired[AnomalySeverityType],  # (1)
    Status: NotRequired[AnomalyStatusType],  # (2)
    UpdateTime: NotRequired[datetime],
    AnomalyTimeRange: NotRequired[AnomalyTimeRangeTypeDef],  # (3)
    AnomalyReportedTimeRange: NotRequired[AnomalyReportedTimeRangeTypeDef],  # (4)
    PredictionTimeRange: NotRequired[PredictionTimeRangeTypeDef],  # (5)
    SourceDetails: NotRequired[AnomalySourceDetailsTypeDef],  # (6)
    AssociatedInsightId: NotRequired[str],
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (7)
    Limit: NotRequired[float],
    SourceMetadata: NotRequired[AnomalySourceMetadataTypeDef],  # (8)
    AnomalyResources: NotRequired[List[AnomalyResourceTypeDef]],  # (9)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: AnomalySeverityType](./literals.md#anomalyseveritytype) 
2. See [:material-code-brackets: AnomalyStatusType](./literals.md#anomalystatustype) 
3. See [:material-code-braces: AnomalyTimeRangeTypeDef](./type_defs.md#anomalytimerangetypedef) 
4. See [:material-code-braces: AnomalyReportedTimeRangeTypeDef](./type_defs.md#anomalyreportedtimerangetypedef) 
5. See [:material-code-braces: PredictionTimeRangeTypeDef](./type_defs.md#predictiontimerangetypedef) 
6. See [:material-code-braces: AnomalySourceDetailsTypeDef](./type_defs.md#anomalysourcedetailstypedef) 
7. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
8. See [:material-code-braces: AnomalySourceMetadataTypeDef](./type_defs.md#anomalysourcemetadatatypedef) 
9. See [:material-code-braces: AnomalyResourceTypeDef](./type_defs.md#anomalyresourcetypedef) 
## ReactiveAnomalySummaryTypeDef

```python
# ReactiveAnomalySummaryTypeDef definition

class ReactiveAnomalySummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Severity: NotRequired[AnomalySeverityType],  # (1)
    Status: NotRequired[AnomalyStatusType],  # (2)
    AnomalyTimeRange: NotRequired[AnomalyTimeRangeTypeDef],  # (3)
    AnomalyReportedTimeRange: NotRequired[AnomalyReportedTimeRangeTypeDef],  # (4)
    SourceDetails: NotRequired[AnomalySourceDetailsTypeDef],  # (5)
    AssociatedInsightId: NotRequired[str],
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (6)
    Type: NotRequired[AnomalyTypeType],  # (7)
    Name: NotRequired[str],
    Description: NotRequired[str],
    CausalAnomalyId: NotRequired[str],
    AnomalyResources: NotRequired[List[AnomalyResourceTypeDef]],  # (8)
```

1. See [:material-code-brackets: AnomalySeverityType](./literals.md#anomalyseveritytype) 
2. See [:material-code-brackets: AnomalyStatusType](./literals.md#anomalystatustype) 
3. See [:material-code-braces: AnomalyTimeRangeTypeDef](./type_defs.md#anomalytimerangetypedef) 
4. See [:material-code-braces: AnomalyReportedTimeRangeTypeDef](./type_defs.md#anomalyreportedtimerangetypedef) 
5. See [:material-code-braces: AnomalySourceDetailsTypeDef](./type_defs.md#anomalysourcedetailstypedef) 
6. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
7. See [:material-code-brackets: AnomalyTypeType](./literals.md#anomalytypetype) 
8. See [:material-code-braces: AnomalyResourceTypeDef](./type_defs.md#anomalyresourcetypedef) 
## ReactiveAnomalyTypeDef

```python
# ReactiveAnomalyTypeDef definition

class ReactiveAnomalyTypeDef(TypedDict):
    Id: NotRequired[str],
    Severity: NotRequired[AnomalySeverityType],  # (1)
    Status: NotRequired[AnomalyStatusType],  # (2)
    AnomalyTimeRange: NotRequired[AnomalyTimeRangeTypeDef],  # (3)
    AnomalyReportedTimeRange: NotRequired[AnomalyReportedTimeRangeTypeDef],  # (4)
    SourceDetails: NotRequired[AnomalySourceDetailsTypeDef],  # (5)
    AssociatedInsightId: NotRequired[str],
    ResourceCollection: NotRequired[ResourceCollectionOutputTypeDef],  # (6)
    Type: NotRequired[AnomalyTypeType],  # (7)
    Name: NotRequired[str],
    Description: NotRequired[str],
    CausalAnomalyId: NotRequired[str],
    AnomalyResources: NotRequired[List[AnomalyResourceTypeDef]],  # (8)
```

1. See [:material-code-brackets: AnomalySeverityType](./literals.md#anomalyseveritytype) 
2. See [:material-code-brackets: AnomalyStatusType](./literals.md#anomalystatustype) 
3. See [:material-code-braces: AnomalyTimeRangeTypeDef](./type_defs.md#anomalytimerangetypedef) 
4. See [:material-code-braces: AnomalyReportedTimeRangeTypeDef](./type_defs.md#anomalyreportedtimerangetypedef) 
5. See [:material-code-braces: AnomalySourceDetailsTypeDef](./type_defs.md#anomalysourcedetailstypedef) 
6. See [:material-code-braces: ResourceCollectionOutputTypeDef](./type_defs.md#resourcecollectionoutputtypedef) 
7. See [:material-code-brackets: AnomalyTypeType](./literals.md#anomalytypetype) 
8. See [:material-code-braces: AnomalyResourceTypeDef](./type_defs.md#anomalyresourcetypedef) 
## ListAnomaliesForInsightResponseTypeDef

```python
# ListAnomaliesForInsightResponseTypeDef definition

class ListAnomaliesForInsightResponseTypeDef(TypedDict):
    ProactiveAnomalies: List[ProactiveAnomalySummaryTypeDef],  # (1)
    ReactiveAnomalies: List[ReactiveAnomalySummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProactiveAnomalySummaryTypeDef](./type_defs.md#proactiveanomalysummarytypedef) 
2. See [:material-code-braces: ReactiveAnomalySummaryTypeDef](./type_defs.md#reactiveanomalysummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAnomalyResponseTypeDef

```python
# DescribeAnomalyResponseTypeDef definition

class DescribeAnomalyResponseTypeDef(TypedDict):
    ProactiveAnomaly: ProactiveAnomalyTypeDef,  # (1)
    ReactiveAnomaly: ReactiveAnomalyTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProactiveAnomalyTypeDef](./type_defs.md#proactiveanomalytypedef) 
2. See [:material-code-braces: ReactiveAnomalyTypeDef](./type_defs.md#reactiveanomalytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
