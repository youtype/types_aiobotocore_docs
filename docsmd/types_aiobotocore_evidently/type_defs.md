# Type definitions

> [Index](../README.md) > [CloudWatchEvidently](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently)
    type annotations stubs module [types-aiobotocore-evidently](https://pypi.org/project/types-aiobotocore-evidently/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## SegmentOverrideUnionTypeDef

```python
# SegmentOverrideUnionTypeDef definition

SegmentOverrideUnionTypeDef = Union[
    SegmentOverrideTypeDef,  # (1)
    SegmentOverrideOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SegmentOverrideTypeDef](./type_defs.md#segmentoverridetypedef) 
2. See [:material-code-braces: SegmentOverrideOutputTypeDef](./type_defs.md#segmentoverrideoutputtypedef) 



## EvaluationRequestTypeDef

```python
# EvaluationRequestTypeDef definition

class EvaluationRequestTypeDef(TypedDict):
    entityId: str,
    feature: str,
    evaluationContext: NotRequired[str],
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

## CloudWatchLogsDestinationConfigTypeDef

```python
# CloudWatchLogsDestinationConfigTypeDef definition

class CloudWatchLogsDestinationConfigTypeDef(TypedDict):
    logGroup: NotRequired[str],
```

## CloudWatchLogsDestinationTypeDef

```python
# CloudWatchLogsDestinationTypeDef definition

class CloudWatchLogsDestinationTypeDef(TypedDict):
    logGroup: NotRequired[str],
```

## OnlineAbConfigTypeDef

```python
# OnlineAbConfigTypeDef definition

class OnlineAbConfigTypeDef(TypedDict):
    controlTreatmentName: NotRequired[str],
    treatmentWeights: NotRequired[Mapping[str, int]],
```

## TreatmentConfigTypeDef

```python
# TreatmentConfigTypeDef definition

class TreatmentConfigTypeDef(TypedDict):
    feature: str,
    name: str,
    variation: str,
    description: NotRequired[str],
```

## LaunchGroupConfigTypeDef

```python
# LaunchGroupConfigTypeDef definition

class LaunchGroupConfigTypeDef(TypedDict):
    feature: str,
    name: str,
    variation: str,
    description: NotRequired[str],
```

## ProjectAppConfigResourceConfigTypeDef

```python
# ProjectAppConfigResourceConfigTypeDef definition

class ProjectAppConfigResourceConfigTypeDef(TypedDict):
    applicationId: NotRequired[str],
    environmentId: NotRequired[str],
```

## CreateSegmentRequestRequestTypeDef

```python
# CreateSegmentRequestRequestTypeDef definition

class CreateSegmentRequestRequestTypeDef(TypedDict):
    name: str,
    pattern: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## SegmentTypeDef

```python
# SegmentTypeDef definition

class SegmentTypeDef(TypedDict):
    arn: str,
    createdTime: datetime,
    lastUpdatedTime: datetime,
    name: str,
    pattern: str,
    description: NotRequired[str],
    experimentCount: NotRequired[int],
    launchCount: NotRequired[int],
    tags: NotRequired[Dict[str, str]],
```

## DeleteExperimentRequestRequestTypeDef

```python
# DeleteExperimentRequestRequestTypeDef definition

class DeleteExperimentRequestRequestTypeDef(TypedDict):
    experiment: str,
    project: str,
```

## DeleteFeatureRequestRequestTypeDef

```python
# DeleteFeatureRequestRequestTypeDef definition

class DeleteFeatureRequestRequestTypeDef(TypedDict):
    feature: str,
    project: str,
```

## DeleteLaunchRequestRequestTypeDef

```python
# DeleteLaunchRequestRequestTypeDef definition

class DeleteLaunchRequestRequestTypeDef(TypedDict):
    launch: str,
    project: str,
```

## DeleteProjectRequestRequestTypeDef

```python
# DeleteProjectRequestRequestTypeDef definition

class DeleteProjectRequestRequestTypeDef(TypedDict):
    project: str,
```

## DeleteSegmentRequestRequestTypeDef

```python
# DeleteSegmentRequestRequestTypeDef definition

class DeleteSegmentRequestRequestTypeDef(TypedDict):
    segment: str,
```

## EvaluateFeatureRequestRequestTypeDef

```python
# EvaluateFeatureRequestRequestTypeDef definition

class EvaluateFeatureRequestRequestTypeDef(TypedDict):
    entityId: str,
    feature: str,
    project: str,
    evaluationContext: NotRequired[str],
```

## VariableValueTypeDef

```python
# VariableValueTypeDef definition

class VariableValueTypeDef(TypedDict):
    boolValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    longValue: NotRequired[int],
    stringValue: NotRequired[str],
```

## EvaluationRuleTypeDef

```python
# EvaluationRuleTypeDef definition

class EvaluationRuleTypeDef(TypedDict):
    type: str,
    name: NotRequired[str],
```

## ExperimentExecutionTypeDef

```python
# ExperimentExecutionTypeDef definition

class ExperimentExecutionTypeDef(TypedDict):
    endedTime: NotRequired[datetime],
    startedTime: NotRequired[datetime],
```

## ExperimentReportTypeDef

```python
# ExperimentReportTypeDef definition

class ExperimentReportTypeDef(TypedDict):
    content: NotRequired[str],
    metricName: NotRequired[str],
    reportName: NotRequired[ExperimentReportNameType],  # (1)
    treatmentName: NotRequired[str],
```

1. See [:material-code-brackets: ExperimentReportNameType](./literals.md#experimentreportnametype) 
## ExperimentResultsDataTypeDef

```python
# ExperimentResultsDataTypeDef definition

class ExperimentResultsDataTypeDef(TypedDict):
    metricName: NotRequired[str],
    resultStat: NotRequired[ExperimentResultResponseTypeType],  # (1)
    treatmentName: NotRequired[str],
    values: NotRequired[List[float]],
```

1. See [:material-code-brackets: ExperimentResultResponseTypeType](./literals.md#experimentresultresponsetypetype) 
## ExperimentScheduleTypeDef

```python
# ExperimentScheduleTypeDef definition

class ExperimentScheduleTypeDef(TypedDict):
    analysisCompleteTime: NotRequired[datetime],
```

## OnlineAbDefinitionTypeDef

```python
# OnlineAbDefinitionTypeDef definition

class OnlineAbDefinitionTypeDef(TypedDict):
    controlTreatmentName: NotRequired[str],
    treatmentWeights: NotRequired[Dict[str, int]],
```

## TreatmentTypeDef

```python
# TreatmentTypeDef definition

class TreatmentTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    featureVariations: NotRequired[Dict[str, str]],
```

## GetExperimentRequestRequestTypeDef

```python
# GetExperimentRequestRequestTypeDef definition

class GetExperimentRequestRequestTypeDef(TypedDict):
    experiment: str,
    project: str,
```

## GetFeatureRequestRequestTypeDef

```python
# GetFeatureRequestRequestTypeDef definition

class GetFeatureRequestRequestTypeDef(TypedDict):
    feature: str,
    project: str,
```

## GetLaunchRequestRequestTypeDef

```python
# GetLaunchRequestRequestTypeDef definition

class GetLaunchRequestRequestTypeDef(TypedDict):
    launch: str,
    project: str,
```

## GetProjectRequestRequestTypeDef

```python
# GetProjectRequestRequestTypeDef definition

class GetProjectRequestRequestTypeDef(TypedDict):
    project: str,
```

## GetSegmentRequestRequestTypeDef

```python
# GetSegmentRequestRequestTypeDef definition

class GetSegmentRequestRequestTypeDef(TypedDict):
    segment: str,
```

## LaunchExecutionTypeDef

```python
# LaunchExecutionTypeDef definition

class LaunchExecutionTypeDef(TypedDict):
    endedTime: NotRequired[datetime],
    startedTime: NotRequired[datetime],
```

## LaunchGroupTypeDef

```python
# LaunchGroupTypeDef definition

class LaunchGroupTypeDef(TypedDict):
    featureVariations: Dict[str, str],
    name: str,
    description: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListExperimentsRequestRequestTypeDef

```python
# ListExperimentsRequestRequestTypeDef definition

class ListExperimentsRequestRequestTypeDef(TypedDict):
    project: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[ExperimentStatusType],  # (1)
```

1. See [:material-code-brackets: ExperimentStatusType](./literals.md#experimentstatustype) 
## ListFeaturesRequestRequestTypeDef

```python
# ListFeaturesRequestRequestTypeDef definition

class ListFeaturesRequestRequestTypeDef(TypedDict):
    project: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListLaunchesRequestRequestTypeDef

```python
# ListLaunchesRequestRequestTypeDef definition

class ListLaunchesRequestRequestTypeDef(TypedDict):
    project: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[LaunchStatusType],  # (1)
```

1. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
## ListProjectsRequestRequestTypeDef

```python
# ListProjectsRequestRequestTypeDef definition

class ListProjectsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    arn: str,
    createdTime: datetime,
    lastUpdatedTime: datetime,
    name: str,
    status: ProjectStatusType,  # (1)
    activeExperimentCount: NotRequired[int],
    activeLaunchCount: NotRequired[int],
    description: NotRequired[str],
    experimentCount: NotRequired[int],
    featureCount: NotRequired[int],
    launchCount: NotRequired[int],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
## ListSegmentReferencesRequestRequestTypeDef

```python
# ListSegmentReferencesRequestRequestTypeDef definition

class ListSegmentReferencesRequestRequestTypeDef(TypedDict):
    segment: str,
    type: SegmentReferenceResourceTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: SegmentReferenceResourceTypeType](./literals.md#segmentreferenceresourcetypetype) 
## RefResourceTypeDef

```python
# RefResourceTypeDef definition

class RefResourceTypeDef(TypedDict):
    name: str,
    type: str,
    arn: NotRequired[str],
    endTime: NotRequired[str],
    lastUpdatedOn: NotRequired[str],
    startTime: NotRequired[str],
    status: NotRequired[str],
```

## ListSegmentsRequestRequestTypeDef

```python
# ListSegmentsRequestRequestTypeDef definition

class ListSegmentsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## MetricDefinitionConfigTypeDef

```python
# MetricDefinitionConfigTypeDef definition

class MetricDefinitionConfigTypeDef(TypedDict):
    entityIdKey: str,
    name: str,
    valueKey: str,
    eventPattern: NotRequired[str],
    unitLabel: NotRequired[str],
```

## MetricDefinitionTypeDef

```python
# MetricDefinitionTypeDef definition

class MetricDefinitionTypeDef(TypedDict):
    entityIdKey: NotRequired[str],
    eventPattern: NotRequired[str],
    name: NotRequired[str],
    unitLabel: NotRequired[str],
    valueKey: NotRequired[str],
```

## ProjectAppConfigResourceTypeDef

```python
# ProjectAppConfigResourceTypeDef definition

class ProjectAppConfigResourceTypeDef(TypedDict):
    applicationId: str,
    configurationProfileId: str,
    environmentId: str,
```

## S3DestinationConfigTypeDef

```python
# S3DestinationConfigTypeDef definition

class S3DestinationConfigTypeDef(TypedDict):
    bucket: NotRequired[str],
    prefix: NotRequired[str],
```

## S3DestinationTypeDef

```python
# S3DestinationTypeDef definition

class S3DestinationTypeDef(TypedDict):
    bucket: NotRequired[str],
    prefix: NotRequired[str],
```

## PutProjectEventsResultEntryTypeDef

```python
# PutProjectEventsResultEntryTypeDef definition

class PutProjectEventsResultEntryTypeDef(TypedDict):
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
    eventId: NotRequired[str],
```

## SegmentOverrideOutputTypeDef

```python
# SegmentOverrideOutputTypeDef definition

class SegmentOverrideOutputTypeDef(TypedDict):
    evaluationOrder: int,
    segment: str,
    weights: Dict[str, int],
```

## SegmentOverrideTypeDef

```python
# SegmentOverrideTypeDef definition

class SegmentOverrideTypeDef(TypedDict):
    evaluationOrder: int,
    segment: str,
    weights: Mapping[str, int],
```

## StartLaunchRequestRequestTypeDef

```python
# StartLaunchRequestRequestTypeDef definition

class StartLaunchRequestRequestTypeDef(TypedDict):
    launch: str,
    project: str,
```

## StopExperimentRequestRequestTypeDef

```python
# StopExperimentRequestRequestTypeDef definition

class StopExperimentRequestRequestTypeDef(TypedDict):
    experiment: str,
    project: str,
    desiredState: NotRequired[ExperimentStopDesiredStateType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: ExperimentStopDesiredStateType](./literals.md#experimentstopdesiredstatetype) 
## StopLaunchRequestRequestTypeDef

```python
# StopLaunchRequestRequestTypeDef definition

class StopLaunchRequestRequestTypeDef(TypedDict):
    launch: str,
    project: str,
    desiredState: NotRequired[LaunchStopDesiredStateType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: LaunchStopDesiredStateType](./literals.md#launchstopdesiredstatetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TestSegmentPatternRequestRequestTypeDef

```python
# TestSegmentPatternRequestRequestTypeDef definition

class TestSegmentPatternRequestRequestTypeDef(TypedDict):
    pattern: str,
    payload: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## BatchEvaluateFeatureRequestRequestTypeDef

```python
# BatchEvaluateFeatureRequestRequestTypeDef definition

class BatchEvaluateFeatureRequestRequestTypeDef(TypedDict):
    project: str,
    requests: Sequence[EvaluationRequestTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationRequestTypeDef](./type_defs.md#evaluationrequesttypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExperimentResponseTypeDef

```python
# StartExperimentResponseTypeDef definition

class StartExperimentResponseTypeDef(TypedDict):
    startedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopExperimentResponseTypeDef

```python
# StopExperimentResponseTypeDef definition

class StopExperimentResponseTypeDef(TypedDict):
    endedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopLaunchResponseTypeDef

```python
# StopLaunchResponseTypeDef definition

class StopLaunchResponseTypeDef(TypedDict):
    endedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestSegmentPatternResponseTypeDef

```python
# TestSegmentPatternResponseTypeDef definition

class TestSegmentPatternResponseTypeDef(TypedDict):
    match: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectRequestRequestTypeDef

```python
# UpdateProjectRequestRequestTypeDef definition

class UpdateProjectRequestRequestTypeDef(TypedDict):
    project: str,
    appConfigResource: NotRequired[ProjectAppConfigResourceConfigTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: ProjectAppConfigResourceConfigTypeDef](./type_defs.md#projectappconfigresourceconfigtypedef) 
## CreateSegmentResponseTypeDef

```python
# CreateSegmentResponseTypeDef definition

class CreateSegmentResponseTypeDef(TypedDict):
    segment: SegmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSegmentResponseTypeDef

```python
# GetSegmentResponseTypeDef definition

class GetSegmentResponseTypeDef(TypedDict):
    segment: SegmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSegmentsResponseTypeDef

```python
# ListSegmentsResponseTypeDef definition

class ListSegmentsResponseTypeDef(TypedDict):
    segments: List[SegmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EvaluateFeatureResponseTypeDef

```python
# EvaluateFeatureResponseTypeDef definition

class EvaluateFeatureResponseTypeDef(TypedDict):
    details: str,
    reason: str,
    value: VariableValueTypeDef,  # (1)
    variation: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EvaluationResultTypeDef

```python
# EvaluationResultTypeDef definition

class EvaluationResultTypeDef(TypedDict):
    entityId: str,
    feature: str,
    details: NotRequired[str],
    project: NotRequired[str],
    reason: NotRequired[str],
    value: NotRequired[VariableValueTypeDef],  # (1)
    variation: NotRequired[str],
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) 
## VariationConfigTypeDef

```python
# VariationConfigTypeDef definition

class VariationConfigTypeDef(TypedDict):
    name: str,
    value: VariableValueTypeDef,  # (1)
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) 
## VariationTypeDef

```python
# VariationTypeDef definition

class VariationTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[VariableValueTypeDef],  # (1)
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) 
## FeatureSummaryTypeDef

```python
# FeatureSummaryTypeDef definition

class FeatureSummaryTypeDef(TypedDict):
    arn: str,
    createdTime: datetime,
    evaluationStrategy: FeatureEvaluationStrategyType,  # (2)
    lastUpdatedTime: datetime,
    name: str,
    status: FeatureStatusType,  # (3)
    defaultVariation: NotRequired[str],
    evaluationRules: NotRequired[List[EvaluationRuleTypeDef]],  # (1)
    project: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: EvaluationRuleTypeDef](./type_defs.md#evaluationruletypedef) 
2. See [:material-code-brackets: FeatureEvaluationStrategyType](./literals.md#featureevaluationstrategytype) 
3. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    data: str,
    timestamp: TimestampTypeDef,
    type: EventTypeType,  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## GetExperimentResultsRequestRequestTypeDef

```python
# GetExperimentResultsRequestRequestTypeDef definition

class GetExperimentResultsRequestRequestTypeDef(TypedDict):
    experiment: str,
    metricNames: Sequence[str],
    project: str,
    treatmentNames: Sequence[str],
    baseStat: NotRequired[ExperimentBaseStatType],  # (1)
    endTime: NotRequired[TimestampTypeDef],
    period: NotRequired[int],
    reportNames: NotRequired[Sequence[ExperimentReportNameType]],  # (2)
    resultStats: NotRequired[Sequence[ExperimentResultRequestTypeType]],  # (3)
    startTime: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: ExperimentBaseStatType](./literals.md#experimentbasestattype) 
2. See [:material-code-brackets: ExperimentReportNameType](./literals.md#experimentreportnametype) 
3. See [:material-code-brackets: ExperimentResultRequestTypeType](./literals.md#experimentresultrequesttypetype) 
## StartExperimentRequestRequestTypeDef

```python
# StartExperimentRequestRequestTypeDef definition

class StartExperimentRequestRequestTypeDef(TypedDict):
    analysisCompleteTime: TimestampTypeDef,
    experiment: str,
    project: str,
```

## GetExperimentResultsResponseTypeDef

```python
# GetExperimentResultsResponseTypeDef definition

class GetExperimentResultsResponseTypeDef(TypedDict):
    details: str,
    reports: List[ExperimentReportTypeDef],  # (1)
    resultsData: List[ExperimentResultsDataTypeDef],  # (2)
    timestamps: List[datetime],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ExperimentReportTypeDef](./type_defs.md#experimentreporttypedef) 
2. See [:material-code-braces: ExperimentResultsDataTypeDef](./type_defs.md#experimentresultsdatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExperimentsRequestListExperimentsPaginateTypeDef

```python
# ListExperimentsRequestListExperimentsPaginateTypeDef definition

class ListExperimentsRequestListExperimentsPaginateTypeDef(TypedDict):
    project: str,
    status: NotRequired[ExperimentStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ExperimentStatusType](./literals.md#experimentstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFeaturesRequestListFeaturesPaginateTypeDef

```python
# ListFeaturesRequestListFeaturesPaginateTypeDef definition

class ListFeaturesRequestListFeaturesPaginateTypeDef(TypedDict):
    project: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLaunchesRequestListLaunchesPaginateTypeDef

```python
# ListLaunchesRequestListLaunchesPaginateTypeDef definition

class ListLaunchesRequestListLaunchesPaginateTypeDef(TypedDict):
    project: str,
    status: NotRequired[LaunchStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestListProjectsPaginateTypeDef

```python
# ListProjectsRequestListProjectsPaginateTypeDef definition

class ListProjectsRequestListProjectsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef

```python
# ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef definition

class ListSegmentReferencesRequestListSegmentReferencesPaginateTypeDef(TypedDict):
    segment: str,
    type: SegmentReferenceResourceTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SegmentReferenceResourceTypeType](./literals.md#segmentreferenceresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSegmentsRequestListSegmentsPaginateTypeDef

```python
# ListSegmentsRequestListSegmentsPaginateTypeDef definition

class ListSegmentsRequestListSegmentsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsResponseTypeDef

```python
# ListProjectsResponseTypeDef definition

class ListProjectsResponseTypeDef(TypedDict):
    projects: List[ProjectSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSegmentReferencesResponseTypeDef

```python
# ListSegmentReferencesResponseTypeDef definition

class ListSegmentReferencesResponseTypeDef(TypedDict):
    referencedBy: List[RefResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RefResourceTypeDef](./type_defs.md#refresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricGoalConfigTypeDef

```python
# MetricGoalConfigTypeDef definition

class MetricGoalConfigTypeDef(TypedDict):
    metricDefinition: MetricDefinitionConfigTypeDef,  # (2)
    desiredChange: NotRequired[ChangeDirectionEnumType],  # (1)
```

1. See [:material-code-brackets: ChangeDirectionEnumType](./literals.md#changedirectionenumtype) 
2. See [:material-code-braces: MetricDefinitionConfigTypeDef](./type_defs.md#metricdefinitionconfigtypedef) 
## MetricMonitorConfigTypeDef

```python
# MetricMonitorConfigTypeDef definition

class MetricMonitorConfigTypeDef(TypedDict):
    metricDefinition: MetricDefinitionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: MetricDefinitionConfigTypeDef](./type_defs.md#metricdefinitionconfigtypedef) 
## MetricGoalTypeDef

```python
# MetricGoalTypeDef definition

class MetricGoalTypeDef(TypedDict):
    metricDefinition: MetricDefinitionTypeDef,  # (2)
    desiredChange: NotRequired[ChangeDirectionEnumType],  # (1)
```

1. See [:material-code-brackets: ChangeDirectionEnumType](./literals.md#changedirectionenumtype) 
2. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
## MetricMonitorTypeDef

```python
# MetricMonitorTypeDef definition

class MetricMonitorTypeDef(TypedDict):
    metricDefinition: MetricDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
## ProjectDataDeliveryConfigTypeDef

```python
# ProjectDataDeliveryConfigTypeDef definition

class ProjectDataDeliveryConfigTypeDef(TypedDict):
    cloudWatchLogs: NotRequired[CloudWatchLogsDestinationConfigTypeDef],  # (1)
    s3Destination: NotRequired[S3DestinationConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CloudWatchLogsDestinationConfigTypeDef](./type_defs.md#cloudwatchlogsdestinationconfigtypedef) 
2. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
## UpdateProjectDataDeliveryRequestRequestTypeDef

```python
# UpdateProjectDataDeliveryRequestRequestTypeDef definition

class UpdateProjectDataDeliveryRequestRequestTypeDef(TypedDict):
    project: str,
    cloudWatchLogs: NotRequired[CloudWatchLogsDestinationConfigTypeDef],  # (1)
    s3Destination: NotRequired[S3DestinationConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CloudWatchLogsDestinationConfigTypeDef](./type_defs.md#cloudwatchlogsdestinationconfigtypedef) 
2. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
## ProjectDataDeliveryTypeDef

```python
# ProjectDataDeliveryTypeDef definition

class ProjectDataDeliveryTypeDef(TypedDict):
    cloudWatchLogs: NotRequired[CloudWatchLogsDestinationTypeDef],  # (1)
    s3Destination: NotRequired[S3DestinationTypeDef],  # (2)
```

1. See [:material-code-braces: CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef) 
2. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
## PutProjectEventsResponseTypeDef

```python
# PutProjectEventsResponseTypeDef definition

class PutProjectEventsResponseTypeDef(TypedDict):
    eventResults: List[PutProjectEventsResultEntryTypeDef],  # (1)
    failedEventCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PutProjectEventsResultEntryTypeDef](./type_defs.md#putprojecteventsresultentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduledSplitTypeDef

```python
# ScheduledSplitTypeDef definition

class ScheduledSplitTypeDef(TypedDict):
    startTime: datetime,
    groupWeights: NotRequired[Dict[str, int]],
    segmentOverrides: NotRequired[List[SegmentOverrideOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: SegmentOverrideOutputTypeDef](./type_defs.md#segmentoverrideoutputtypedef) 
## BatchEvaluateFeatureResponseTypeDef

```python
# BatchEvaluateFeatureResponseTypeDef definition

class BatchEvaluateFeatureResponseTypeDef(TypedDict):
    results: List[EvaluationResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFeatureRequestRequestTypeDef

```python
# CreateFeatureRequestRequestTypeDef definition

class CreateFeatureRequestRequestTypeDef(TypedDict):
    name: str,
    project: str,
    variations: Sequence[VariationConfigTypeDef],  # (1)
    defaultVariation: NotRequired[str],
    description: NotRequired[str],
    entityOverrides: NotRequired[Mapping[str, str]],
    evaluationStrategy: NotRequired[FeatureEvaluationStrategyType],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: VariationConfigTypeDef](./type_defs.md#variationconfigtypedef) 
2. See [:material-code-brackets: FeatureEvaluationStrategyType](./literals.md#featureevaluationstrategytype) 
## UpdateFeatureRequestRequestTypeDef

```python
# UpdateFeatureRequestRequestTypeDef definition

class UpdateFeatureRequestRequestTypeDef(TypedDict):
    feature: str,
    project: str,
    addOrUpdateVariations: NotRequired[Sequence[VariationConfigTypeDef]],  # (1)
    defaultVariation: NotRequired[str],
    description: NotRequired[str],
    entityOverrides: NotRequired[Mapping[str, str]],
    evaluationStrategy: NotRequired[FeatureEvaluationStrategyType],  # (2)
    removeVariations: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: VariationConfigTypeDef](./type_defs.md#variationconfigtypedef) 
2. See [:material-code-brackets: FeatureEvaluationStrategyType](./literals.md#featureevaluationstrategytype) 
## FeatureTypeDef

```python
# FeatureTypeDef definition

class FeatureTypeDef(TypedDict):
    arn: str,
    createdTime: datetime,
    evaluationStrategy: FeatureEvaluationStrategyType,  # (2)
    lastUpdatedTime: datetime,
    name: str,
    status: FeatureStatusType,  # (3)
    valueType: VariationValueTypeType,  # (4)
    variations: List[VariationTypeDef],  # (5)
    defaultVariation: NotRequired[str],
    description: NotRequired[str],
    entityOverrides: NotRequired[Dict[str, str]],
    evaluationRules: NotRequired[List[EvaluationRuleTypeDef]],  # (1)
    project: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: EvaluationRuleTypeDef](./type_defs.md#evaluationruletypedef) 
2. See [:material-code-brackets: FeatureEvaluationStrategyType](./literals.md#featureevaluationstrategytype) 
3. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
4. See [:material-code-brackets: VariationValueTypeType](./literals.md#variationvaluetypetype) 
5. See [:material-code-braces: VariationTypeDef](./type_defs.md#variationtypedef) 
## ListFeaturesResponseTypeDef

```python
# ListFeaturesResponseTypeDef definition

class ListFeaturesResponseTypeDef(TypedDict):
    features: List[FeatureSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FeatureSummaryTypeDef](./type_defs.md#featuresummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProjectEventsRequestRequestTypeDef

```python
# PutProjectEventsRequestRequestTypeDef definition

class PutProjectEventsRequestRequestTypeDef(TypedDict):
    events: Sequence[EventTypeDef],  # (1)
    project: str,
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
## CreateExperimentRequestRequestTypeDef

```python
# CreateExperimentRequestRequestTypeDef definition

class CreateExperimentRequestRequestTypeDef(TypedDict):
    metricGoals: Sequence[MetricGoalConfigTypeDef],  # (1)
    name: str,
    project: str,
    treatments: Sequence[TreatmentConfigTypeDef],  # (2)
    description: NotRequired[str],
    onlineAbConfig: NotRequired[OnlineAbConfigTypeDef],  # (3)
    randomizationSalt: NotRequired[str],
    samplingRate: NotRequired[int],
    segment: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MetricGoalConfigTypeDef](./type_defs.md#metricgoalconfigtypedef) 
2. See [:material-code-braces: TreatmentConfigTypeDef](./type_defs.md#treatmentconfigtypedef) 
3. See [:material-code-braces: OnlineAbConfigTypeDef](./type_defs.md#onlineabconfigtypedef) 
## UpdateExperimentRequestRequestTypeDef

```python
# UpdateExperimentRequestRequestTypeDef definition

class UpdateExperimentRequestRequestTypeDef(TypedDict):
    experiment: str,
    project: str,
    description: NotRequired[str],
    metricGoals: NotRequired[Sequence[MetricGoalConfigTypeDef]],  # (1)
    onlineAbConfig: NotRequired[OnlineAbConfigTypeDef],  # (2)
    randomizationSalt: NotRequired[str],
    removeSegment: NotRequired[bool],
    samplingRate: NotRequired[int],
    segment: NotRequired[str],
    treatments: NotRequired[Sequence[TreatmentConfigTypeDef]],  # (3)
```

1. See [:material-code-braces: MetricGoalConfigTypeDef](./type_defs.md#metricgoalconfigtypedef) 
2. See [:material-code-braces: OnlineAbConfigTypeDef](./type_defs.md#onlineabconfigtypedef) 
3. See [:material-code-braces: TreatmentConfigTypeDef](./type_defs.md#treatmentconfigtypedef) 
## ExperimentTypeDef

```python
# ExperimentTypeDef definition

class ExperimentTypeDef(TypedDict):
    arn: str,
    createdTime: datetime,
    lastUpdatedTime: datetime,
    name: str,
    status: ExperimentStatusType,  # (5)
    type: ExperimentTypeType,  # (7)
    description: NotRequired[str],
    execution: NotRequired[ExperimentExecutionTypeDef],  # (1)
    metricGoals: NotRequired[List[MetricGoalTypeDef]],  # (2)
    onlineAbDefinition: NotRequired[OnlineAbDefinitionTypeDef],  # (3)
    project: NotRequired[str],
    randomizationSalt: NotRequired[str],
    samplingRate: NotRequired[int],
    schedule: NotRequired[ExperimentScheduleTypeDef],  # (4)
    segment: NotRequired[str],
    statusReason: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    treatments: NotRequired[List[TreatmentTypeDef]],  # (6)
```

1. See [:material-code-braces: ExperimentExecutionTypeDef](./type_defs.md#experimentexecutiontypedef) 
2. See [:material-code-braces: MetricGoalTypeDef](./type_defs.md#metricgoaltypedef) 
3. See [:material-code-braces: OnlineAbDefinitionTypeDef](./type_defs.md#onlineabdefinitiontypedef) 
4. See [:material-code-braces: ExperimentScheduleTypeDef](./type_defs.md#experimentscheduletypedef) 
5. See [:material-code-brackets: ExperimentStatusType](./literals.md#experimentstatustype) 
6. See [:material-code-braces: TreatmentTypeDef](./type_defs.md#treatmenttypedef) 
7. See [:material-code-brackets: ExperimentTypeType](./literals.md#experimenttypetype) 
## CreateProjectRequestRequestTypeDef

```python
# CreateProjectRequestRequestTypeDef definition

class CreateProjectRequestRequestTypeDef(TypedDict):
    name: str,
    appConfigResource: NotRequired[ProjectAppConfigResourceConfigTypeDef],  # (1)
    dataDelivery: NotRequired[ProjectDataDeliveryConfigTypeDef],  # (2)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ProjectAppConfigResourceConfigTypeDef](./type_defs.md#projectappconfigresourceconfigtypedef) 
2. See [:material-code-braces: ProjectDataDeliveryConfigTypeDef](./type_defs.md#projectdatadeliveryconfigtypedef) 
## ProjectTypeDef

```python
# ProjectTypeDef definition

class ProjectTypeDef(TypedDict):
    arn: str,
    createdTime: datetime,
    lastUpdatedTime: datetime,
    name: str,
    status: ProjectStatusType,  # (3)
    activeExperimentCount: NotRequired[int],
    activeLaunchCount: NotRequired[int],
    appConfigResource: NotRequired[ProjectAppConfigResourceTypeDef],  # (1)
    dataDelivery: NotRequired[ProjectDataDeliveryTypeDef],  # (2)
    description: NotRequired[str],
    experimentCount: NotRequired[int],
    featureCount: NotRequired[int],
    launchCount: NotRequired[int],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ProjectAppConfigResourceTypeDef](./type_defs.md#projectappconfigresourcetypedef) 
2. See [:material-code-braces: ProjectDataDeliveryTypeDef](./type_defs.md#projectdatadeliverytypedef) 
3. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
## ScheduledSplitsLaunchDefinitionTypeDef

```python
# ScheduledSplitsLaunchDefinitionTypeDef definition

class ScheduledSplitsLaunchDefinitionTypeDef(TypedDict):
    steps: NotRequired[List[ScheduledSplitTypeDef]],  # (1)
```

1. See [:material-code-braces: ScheduledSplitTypeDef](./type_defs.md#scheduledsplittypedef) 
## ScheduledSplitConfigTypeDef

```python
# ScheduledSplitConfigTypeDef definition

class ScheduledSplitConfigTypeDef(TypedDict):
    groupWeights: Mapping[str, int],
    startTime: TimestampTypeDef,
    segmentOverrides: NotRequired[Sequence[SegmentOverrideUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: SegmentOverrideTypeDef](./type_defs.md#segmentoverridetypedef) [:material-code-braces: SegmentOverrideOutputTypeDef](./type_defs.md#segmentoverrideoutputtypedef) 
## CreateFeatureResponseTypeDef

```python
# CreateFeatureResponseTypeDef definition

class CreateFeatureResponseTypeDef(TypedDict):
    feature: FeatureTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FeatureTypeDef](./type_defs.md#featuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFeatureResponseTypeDef

```python
# GetFeatureResponseTypeDef definition

class GetFeatureResponseTypeDef(TypedDict):
    feature: FeatureTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FeatureTypeDef](./type_defs.md#featuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFeatureResponseTypeDef

```python
# UpdateFeatureResponseTypeDef definition

class UpdateFeatureResponseTypeDef(TypedDict):
    feature: FeatureTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FeatureTypeDef](./type_defs.md#featuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExperimentResponseTypeDef

```python
# CreateExperimentResponseTypeDef definition

class CreateExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExperimentResponseTypeDef

```python
# GetExperimentResponseTypeDef definition

class GetExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExperimentsResponseTypeDef

```python
# ListExperimentsResponseTypeDef definition

class ListExperimentsResponseTypeDef(TypedDict):
    experiments: List[ExperimentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateExperimentResponseTypeDef

```python
# UpdateExperimentResponseTypeDef definition

class UpdateExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectResponseTypeDef

```python
# CreateProjectResponseTypeDef definition

class CreateProjectResponseTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProjectResponseTypeDef

```python
# GetProjectResponseTypeDef definition

class GetProjectResponseTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectDataDeliveryResponseTypeDef

```python
# UpdateProjectDataDeliveryResponseTypeDef definition

class UpdateProjectDataDeliveryResponseTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectResponseTypeDef

```python
# UpdateProjectResponseTypeDef definition

class UpdateProjectResponseTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LaunchTypeDef

```python
# LaunchTypeDef definition

class LaunchTypeDef(TypedDict):
    arn: str,
    createdTime: datetime,
    lastUpdatedTime: datetime,
    name: str,
    status: LaunchStatusType,  # (5)
    type: LaunchTypeType,  # (6)
    description: NotRequired[str],
    execution: NotRequired[LaunchExecutionTypeDef],  # (1)
    groups: NotRequired[List[LaunchGroupTypeDef]],  # (2)
    metricMonitors: NotRequired[List[MetricMonitorTypeDef]],  # (3)
    project: NotRequired[str],
    randomizationSalt: NotRequired[str],
    scheduledSplitsDefinition: NotRequired[ScheduledSplitsLaunchDefinitionTypeDef],  # (4)
    statusReason: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: LaunchExecutionTypeDef](./type_defs.md#launchexecutiontypedef) 
2. See [:material-code-braces: LaunchGroupTypeDef](./type_defs.md#launchgrouptypedef) 
3. See [:material-code-braces: MetricMonitorTypeDef](./type_defs.md#metricmonitortypedef) 
4. See [:material-code-braces: ScheduledSplitsLaunchDefinitionTypeDef](./type_defs.md#scheduledsplitslaunchdefinitiontypedef) 
5. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
6. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
## ScheduledSplitsLaunchConfigTypeDef

```python
# ScheduledSplitsLaunchConfigTypeDef definition

class ScheduledSplitsLaunchConfigTypeDef(TypedDict):
    steps: Sequence[ScheduledSplitConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ScheduledSplitConfigTypeDef](./type_defs.md#scheduledsplitconfigtypedef) 
## CreateLaunchResponseTypeDef

```python
# CreateLaunchResponseTypeDef definition

class CreateLaunchResponseTypeDef(TypedDict):
    launch: LaunchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchTypeDef](./type_defs.md#launchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLaunchResponseTypeDef

```python
# GetLaunchResponseTypeDef definition

class GetLaunchResponseTypeDef(TypedDict):
    launch: LaunchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchTypeDef](./type_defs.md#launchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLaunchesResponseTypeDef

```python
# ListLaunchesResponseTypeDef definition

class ListLaunchesResponseTypeDef(TypedDict):
    launches: List[LaunchTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LaunchTypeDef](./type_defs.md#launchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartLaunchResponseTypeDef

```python
# StartLaunchResponseTypeDef definition

class StartLaunchResponseTypeDef(TypedDict):
    launch: LaunchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchTypeDef](./type_defs.md#launchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLaunchResponseTypeDef

```python
# UpdateLaunchResponseTypeDef definition

class UpdateLaunchResponseTypeDef(TypedDict):
    launch: LaunchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchTypeDef](./type_defs.md#launchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLaunchRequestRequestTypeDef

```python
# CreateLaunchRequestRequestTypeDef definition

class CreateLaunchRequestRequestTypeDef(TypedDict):
    groups: Sequence[LaunchGroupConfigTypeDef],  # (1)
    name: str,
    project: str,
    description: NotRequired[str],
    metricMonitors: NotRequired[Sequence[MetricMonitorConfigTypeDef]],  # (2)
    randomizationSalt: NotRequired[str],
    scheduledSplitsConfig: NotRequired[ScheduledSplitsLaunchConfigTypeDef],  # (3)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: LaunchGroupConfigTypeDef](./type_defs.md#launchgroupconfigtypedef) 
2. See [:material-code-braces: MetricMonitorConfigTypeDef](./type_defs.md#metricmonitorconfigtypedef) 
3. See [:material-code-braces: ScheduledSplitsLaunchConfigTypeDef](./type_defs.md#scheduledsplitslaunchconfigtypedef) 
## UpdateLaunchRequestRequestTypeDef

```python
# UpdateLaunchRequestRequestTypeDef definition

class UpdateLaunchRequestRequestTypeDef(TypedDict):
    launch: str,
    project: str,
    description: NotRequired[str],
    groups: NotRequired[Sequence[LaunchGroupConfigTypeDef]],  # (1)
    metricMonitors: NotRequired[Sequence[MetricMonitorConfigTypeDef]],  # (2)
    randomizationSalt: NotRequired[str],
    scheduledSplitsConfig: NotRequired[ScheduledSplitsLaunchConfigTypeDef],  # (3)
```

1. See [:material-code-braces: LaunchGroupConfigTypeDef](./type_defs.md#launchgroupconfigtypedef) 
2. See [:material-code-braces: MetricMonitorConfigTypeDef](./type_defs.md#metricmonitorconfigtypedef) 
3. See [:material-code-braces: ScheduledSplitsLaunchConfigTypeDef](./type_defs.md#scheduledsplitslaunchconfigtypedef) 
