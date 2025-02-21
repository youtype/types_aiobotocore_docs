# Type definitions

> [Index](../README.md) > [CloudWatchEvidently](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#cloudwatchevidently)
    type annotations stubs module [types-aiobotocore-evidently](https://pypi.org/project/types-aiobotocore-evidently/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_evidently.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## SegmentOverrideUnionTypeDef

```python
# SegmentOverrideUnionTypeDef Union usage example

from types_aiobotocore_evidently.type_defs import SegmentOverrideUnionTypeDef


def get_value() -> SegmentOverrideUnionTypeDef:
    return ...


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
# EvaluationRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import EvaluationRequestTypeDef


def get_value() -> EvaluationRequestTypeDef:
    return {
        "entityId": ...,
    }


# EvaluationRequestTypeDef definition

class EvaluationRequestTypeDef(TypedDict):
    entityId: str,
    feature: str,
    evaluationContext: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


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
# CloudWatchLogsDestinationConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CloudWatchLogsDestinationConfigTypeDef


def get_value() -> CloudWatchLogsDestinationConfigTypeDef:
    return {
        "logGroup": ...,
    }


# CloudWatchLogsDestinationConfigTypeDef definition

class CloudWatchLogsDestinationConfigTypeDef(TypedDict):
    logGroup: NotRequired[str],
```

## CloudWatchLogsDestinationTypeDef

```python
# CloudWatchLogsDestinationTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CloudWatchLogsDestinationTypeDef


def get_value() -> CloudWatchLogsDestinationTypeDef:
    return {
        "logGroup": ...,
    }


# CloudWatchLogsDestinationTypeDef definition

class CloudWatchLogsDestinationTypeDef(TypedDict):
    logGroup: NotRequired[str],
```

## OnlineAbConfigTypeDef

```python
# OnlineAbConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import OnlineAbConfigTypeDef


def get_value() -> OnlineAbConfigTypeDef:
    return {
        "controlTreatmentName": ...,
    }


# OnlineAbConfigTypeDef definition

class OnlineAbConfigTypeDef(TypedDict):
    controlTreatmentName: NotRequired[str],
    treatmentWeights: NotRequired[Mapping[str, int]],
```

## TreatmentConfigTypeDef

```python
# TreatmentConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import TreatmentConfigTypeDef


def get_value() -> TreatmentConfigTypeDef:
    return {
        "description": ...,
    }


# TreatmentConfigTypeDef definition

class TreatmentConfigTypeDef(TypedDict):
    feature: str,
    name: str,
    variation: str,
    description: NotRequired[str],
```

## LaunchGroupConfigTypeDef

```python
# LaunchGroupConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import LaunchGroupConfigTypeDef


def get_value() -> LaunchGroupConfigTypeDef:
    return {
        "description": ...,
    }


# LaunchGroupConfigTypeDef definition

class LaunchGroupConfigTypeDef(TypedDict):
    feature: str,
    name: str,
    variation: str,
    description: NotRequired[str],
```

## ProjectAppConfigResourceConfigTypeDef

```python
# ProjectAppConfigResourceConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ProjectAppConfigResourceConfigTypeDef


def get_value() -> ProjectAppConfigResourceConfigTypeDef:
    return {
        "applicationId": ...,
    }


# ProjectAppConfigResourceConfigTypeDef definition

class ProjectAppConfigResourceConfigTypeDef(TypedDict):
    applicationId: NotRequired[str],
    environmentId: NotRequired[str],
```

## CreateSegmentRequestTypeDef

```python
# CreateSegmentRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CreateSegmentRequestTypeDef


def get_value() -> CreateSegmentRequestTypeDef:
    return {
        "name": ...,
    }


# CreateSegmentRequestTypeDef definition

class CreateSegmentRequestTypeDef(TypedDict):
    name: str,
    pattern: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## SegmentTypeDef

```python
# SegmentTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import SegmentTypeDef


def get_value() -> SegmentTypeDef:
    return {
        "arn": ...,
    }


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

## DeleteExperimentRequestTypeDef

```python
# DeleteExperimentRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import DeleteExperimentRequestTypeDef


def get_value() -> DeleteExperimentRequestTypeDef:
    return {
        "experiment": ...,
    }


# DeleteExperimentRequestTypeDef definition

class DeleteExperimentRequestTypeDef(TypedDict):
    experiment: str,
    project: str,
```

## DeleteFeatureRequestTypeDef

```python
# DeleteFeatureRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import DeleteFeatureRequestTypeDef


def get_value() -> DeleteFeatureRequestTypeDef:
    return {
        "feature": ...,
    }


# DeleteFeatureRequestTypeDef definition

class DeleteFeatureRequestTypeDef(TypedDict):
    feature: str,
    project: str,
```

## DeleteLaunchRequestTypeDef

```python
# DeleteLaunchRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import DeleteLaunchRequestTypeDef


def get_value() -> DeleteLaunchRequestTypeDef:
    return {
        "launch": ...,
    }


# DeleteLaunchRequestTypeDef definition

class DeleteLaunchRequestTypeDef(TypedDict):
    launch: str,
    project: str,
```

## DeleteProjectRequestTypeDef

```python
# DeleteProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import DeleteProjectRequestTypeDef


def get_value() -> DeleteProjectRequestTypeDef:
    return {
        "project": ...,
    }


# DeleteProjectRequestTypeDef definition

class DeleteProjectRequestTypeDef(TypedDict):
    project: str,
```

## DeleteSegmentRequestTypeDef

```python
# DeleteSegmentRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import DeleteSegmentRequestTypeDef


def get_value() -> DeleteSegmentRequestTypeDef:
    return {
        "segment": ...,
    }


# DeleteSegmentRequestTypeDef definition

class DeleteSegmentRequestTypeDef(TypedDict):
    segment: str,
```

## EvaluateFeatureRequestTypeDef

```python
# EvaluateFeatureRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import EvaluateFeatureRequestTypeDef


def get_value() -> EvaluateFeatureRequestTypeDef:
    return {
        "entityId": ...,
    }


# EvaluateFeatureRequestTypeDef definition

class EvaluateFeatureRequestTypeDef(TypedDict):
    entityId: str,
    feature: str,
    project: str,
    evaluationContext: NotRequired[str],
```

## VariableValueTypeDef

```python
# VariableValueTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import VariableValueTypeDef


def get_value() -> VariableValueTypeDef:
    return {
        "boolValue": ...,
    }


# VariableValueTypeDef definition

class VariableValueTypeDef(TypedDict):
    boolValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    longValue: NotRequired[int],
    stringValue: NotRequired[str],
```

## EvaluationRuleTypeDef

```python
# EvaluationRuleTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import EvaluationRuleTypeDef


def get_value() -> EvaluationRuleTypeDef:
    return {
        "name": ...,
    }


# EvaluationRuleTypeDef definition

class EvaluationRuleTypeDef(TypedDict):
    type: str,
    name: NotRequired[str],
```

## ExperimentExecutionTypeDef

```python
# ExperimentExecutionTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ExperimentExecutionTypeDef


def get_value() -> ExperimentExecutionTypeDef:
    return {
        "endedTime": ...,
    }


# ExperimentExecutionTypeDef definition

class ExperimentExecutionTypeDef(TypedDict):
    endedTime: NotRequired[datetime],
    startedTime: NotRequired[datetime],
```

## ExperimentReportTypeDef

```python
# ExperimentReportTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ExperimentReportTypeDef


def get_value() -> ExperimentReportTypeDef:
    return {
        "content": ...,
    }


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
# ExperimentResultsDataTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ExperimentResultsDataTypeDef


def get_value() -> ExperimentResultsDataTypeDef:
    return {
        "metricName": ...,
    }


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
# ExperimentScheduleTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ExperimentScheduleTypeDef


def get_value() -> ExperimentScheduleTypeDef:
    return {
        "analysisCompleteTime": ...,
    }


# ExperimentScheduleTypeDef definition

class ExperimentScheduleTypeDef(TypedDict):
    analysisCompleteTime: NotRequired[datetime],
```

## OnlineAbDefinitionTypeDef

```python
# OnlineAbDefinitionTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import OnlineAbDefinitionTypeDef


def get_value() -> OnlineAbDefinitionTypeDef:
    return {
        "controlTreatmentName": ...,
    }


# OnlineAbDefinitionTypeDef definition

class OnlineAbDefinitionTypeDef(TypedDict):
    controlTreatmentName: NotRequired[str],
    treatmentWeights: NotRequired[Dict[str, int]],
```

## TreatmentTypeDef

```python
# TreatmentTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import TreatmentTypeDef


def get_value() -> TreatmentTypeDef:
    return {
        "description": ...,
    }


# TreatmentTypeDef definition

class TreatmentTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    featureVariations: NotRequired[Dict[str, str]],
```

## GetExperimentRequestTypeDef

```python
# GetExperimentRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetExperimentRequestTypeDef


def get_value() -> GetExperimentRequestTypeDef:
    return {
        "experiment": ...,
    }


# GetExperimentRequestTypeDef definition

class GetExperimentRequestTypeDef(TypedDict):
    experiment: str,
    project: str,
```

## GetFeatureRequestTypeDef

```python
# GetFeatureRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetFeatureRequestTypeDef


def get_value() -> GetFeatureRequestTypeDef:
    return {
        "feature": ...,
    }


# GetFeatureRequestTypeDef definition

class GetFeatureRequestTypeDef(TypedDict):
    feature: str,
    project: str,
```

## GetLaunchRequestTypeDef

```python
# GetLaunchRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetLaunchRequestTypeDef


def get_value() -> GetLaunchRequestTypeDef:
    return {
        "launch": ...,
    }


# GetLaunchRequestTypeDef definition

class GetLaunchRequestTypeDef(TypedDict):
    launch: str,
    project: str,
```

## GetProjectRequestTypeDef

```python
# GetProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetProjectRequestTypeDef


def get_value() -> GetProjectRequestTypeDef:
    return {
        "project": ...,
    }


# GetProjectRequestTypeDef definition

class GetProjectRequestTypeDef(TypedDict):
    project: str,
```

## GetSegmentRequestTypeDef

```python
# GetSegmentRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetSegmentRequestTypeDef


def get_value() -> GetSegmentRequestTypeDef:
    return {
        "segment": ...,
    }


# GetSegmentRequestTypeDef definition

class GetSegmentRequestTypeDef(TypedDict):
    segment: str,
```

## LaunchExecutionTypeDef

```python
# LaunchExecutionTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import LaunchExecutionTypeDef


def get_value() -> LaunchExecutionTypeDef:
    return {
        "endedTime": ...,
    }


# LaunchExecutionTypeDef definition

class LaunchExecutionTypeDef(TypedDict):
    endedTime: NotRequired[datetime],
    startedTime: NotRequired[datetime],
```

## LaunchGroupTypeDef

```python
# LaunchGroupTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import LaunchGroupTypeDef


def get_value() -> LaunchGroupTypeDef:
    return {
        "description": ...,
    }


# LaunchGroupTypeDef definition

class LaunchGroupTypeDef(TypedDict):
    featureVariations: Dict[str, str],
    name: str,
    description: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListExperimentsRequestTypeDef

```python
# ListExperimentsRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListExperimentsRequestTypeDef


def get_value() -> ListExperimentsRequestTypeDef:
    return {
        "project": ...,
    }


# ListExperimentsRequestTypeDef definition

class ListExperimentsRequestTypeDef(TypedDict):
    project: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[ExperimentStatusType],  # (1)
```

1. See [:material-code-brackets: ExperimentStatusType](./literals.md#experimentstatustype) 
## ListFeaturesRequestTypeDef

```python
# ListFeaturesRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListFeaturesRequestTypeDef


def get_value() -> ListFeaturesRequestTypeDef:
    return {
        "project": ...,
    }


# ListFeaturesRequestTypeDef definition

class ListFeaturesRequestTypeDef(TypedDict):
    project: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListLaunchesRequestTypeDef

```python
# ListLaunchesRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListLaunchesRequestTypeDef


def get_value() -> ListLaunchesRequestTypeDef:
    return {
        "project": ...,
    }


# ListLaunchesRequestTypeDef definition

class ListLaunchesRequestTypeDef(TypedDict):
    project: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[LaunchStatusType],  # (1)
```

1. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
## ListProjectsRequestTypeDef

```python
# ListProjectsRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListProjectsRequestTypeDef


def get_value() -> ListProjectsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListProjectsRequestTypeDef definition

class ListProjectsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ProjectSummaryTypeDef


def get_value() -> ProjectSummaryTypeDef:
    return {
        "activeExperimentCount": ...,
    }


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
## ListSegmentReferencesRequestTypeDef

```python
# ListSegmentReferencesRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListSegmentReferencesRequestTypeDef


def get_value() -> ListSegmentReferencesRequestTypeDef:
    return {
        "segment": ...,
    }


# ListSegmentReferencesRequestTypeDef definition

class ListSegmentReferencesRequestTypeDef(TypedDict):
    segment: str,
    type: SegmentReferenceResourceTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: SegmentReferenceResourceTypeType](./literals.md#segmentreferenceresourcetypetype) 
## RefResourceTypeDef

```python
# RefResourceTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import RefResourceTypeDef


def get_value() -> RefResourceTypeDef:
    return {
        "arn": ...,
    }


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

## ListSegmentsRequestTypeDef

```python
# ListSegmentsRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListSegmentsRequestTypeDef


def get_value() -> ListSegmentsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListSegmentsRequestTypeDef definition

class ListSegmentsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## MetricDefinitionConfigTypeDef

```python
# MetricDefinitionConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import MetricDefinitionConfigTypeDef


def get_value() -> MetricDefinitionConfigTypeDef:
    return {
        "entityIdKey": ...,
    }


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
# MetricDefinitionTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import MetricDefinitionTypeDef


def get_value() -> MetricDefinitionTypeDef:
    return {
        "entityIdKey": ...,
    }


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
# ProjectAppConfigResourceTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ProjectAppConfigResourceTypeDef


def get_value() -> ProjectAppConfigResourceTypeDef:
    return {
        "applicationId": ...,
    }


# ProjectAppConfigResourceTypeDef definition

class ProjectAppConfigResourceTypeDef(TypedDict):
    applicationId: str,
    configurationProfileId: str,
    environmentId: str,
```

## S3DestinationConfigTypeDef

```python
# S3DestinationConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import S3DestinationConfigTypeDef


def get_value() -> S3DestinationConfigTypeDef:
    return {
        "bucket": ...,
    }


# S3DestinationConfigTypeDef definition

class S3DestinationConfigTypeDef(TypedDict):
    bucket: NotRequired[str],
    prefix: NotRequired[str],
```

## S3DestinationTypeDef

```python
# S3DestinationTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import S3DestinationTypeDef


def get_value() -> S3DestinationTypeDef:
    return {
        "bucket": ...,
    }


# S3DestinationTypeDef definition

class S3DestinationTypeDef(TypedDict):
    bucket: NotRequired[str],
    prefix: NotRequired[str],
```

## PutProjectEventsResultEntryTypeDef

```python
# PutProjectEventsResultEntryTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import PutProjectEventsResultEntryTypeDef


def get_value() -> PutProjectEventsResultEntryTypeDef:
    return {
        "errorCode": ...,
    }


# PutProjectEventsResultEntryTypeDef definition

class PutProjectEventsResultEntryTypeDef(TypedDict):
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
    eventId: NotRequired[str],
```

## SegmentOverrideOutputTypeDef

```python
# SegmentOverrideOutputTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import SegmentOverrideOutputTypeDef


def get_value() -> SegmentOverrideOutputTypeDef:
    return {
        "evaluationOrder": ...,
    }


# SegmentOverrideOutputTypeDef definition

class SegmentOverrideOutputTypeDef(TypedDict):
    evaluationOrder: int,
    segment: str,
    weights: Dict[str, int],
```

## SegmentOverrideTypeDef

```python
# SegmentOverrideTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import SegmentOverrideTypeDef


def get_value() -> SegmentOverrideTypeDef:
    return {
        "evaluationOrder": ...,
    }


# SegmentOverrideTypeDef definition

class SegmentOverrideTypeDef(TypedDict):
    evaluationOrder: int,
    segment: str,
    weights: Mapping[str, int],
```

## StartLaunchRequestTypeDef

```python
# StartLaunchRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import StartLaunchRequestTypeDef


def get_value() -> StartLaunchRequestTypeDef:
    return {
        "launch": ...,
    }


# StartLaunchRequestTypeDef definition

class StartLaunchRequestTypeDef(TypedDict):
    launch: str,
    project: str,
```

## StopExperimentRequestTypeDef

```python
# StopExperimentRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import StopExperimentRequestTypeDef


def get_value() -> StopExperimentRequestTypeDef:
    return {
        "experiment": ...,
    }


# StopExperimentRequestTypeDef definition

class StopExperimentRequestTypeDef(TypedDict):
    experiment: str,
    project: str,
    desiredState: NotRequired[ExperimentStopDesiredStateType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: ExperimentStopDesiredStateType](./literals.md#experimentstopdesiredstatetype) 
## StopLaunchRequestTypeDef

```python
# StopLaunchRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import StopLaunchRequestTypeDef


def get_value() -> StopLaunchRequestTypeDef:
    return {
        "launch": ...,
    }


# StopLaunchRequestTypeDef definition

class StopLaunchRequestTypeDef(TypedDict):
    launch: str,
    project: str,
    desiredState: NotRequired[LaunchStopDesiredStateType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: LaunchStopDesiredStateType](./literals.md#launchstopdesiredstatetype) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TestSegmentPatternRequestTypeDef

```python
# TestSegmentPatternRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import TestSegmentPatternRequestTypeDef


def get_value() -> TestSegmentPatternRequestTypeDef:
    return {
        "pattern": ...,
    }


# TestSegmentPatternRequestTypeDef definition

class TestSegmentPatternRequestTypeDef(TypedDict):
    pattern: str,
    payload: str,
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## BatchEvaluateFeatureRequestTypeDef

```python
# BatchEvaluateFeatureRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import BatchEvaluateFeatureRequestTypeDef


def get_value() -> BatchEvaluateFeatureRequestTypeDef:
    return {
        "project": ...,
    }


# BatchEvaluateFeatureRequestTypeDef definition

class BatchEvaluateFeatureRequestTypeDef(TypedDict):
    project: str,
    requests: Sequence[EvaluationRequestTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationRequestTypeDef](./type_defs.md#evaluationrequesttypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExperimentResponseTypeDef

```python
# StartExperimentResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import StartExperimentResponseTypeDef


def get_value() -> StartExperimentResponseTypeDef:
    return {
        "startedTime": ...,
    }


# StartExperimentResponseTypeDef definition

class StartExperimentResponseTypeDef(TypedDict):
    startedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopExperimentResponseTypeDef

```python
# StopExperimentResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import StopExperimentResponseTypeDef


def get_value() -> StopExperimentResponseTypeDef:
    return {
        "endedTime": ...,
    }


# StopExperimentResponseTypeDef definition

class StopExperimentResponseTypeDef(TypedDict):
    endedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopLaunchResponseTypeDef

```python
# StopLaunchResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import StopLaunchResponseTypeDef


def get_value() -> StopLaunchResponseTypeDef:
    return {
        "endedTime": ...,
    }


# StopLaunchResponseTypeDef definition

class StopLaunchResponseTypeDef(TypedDict):
    endedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestSegmentPatternResponseTypeDef

```python
# TestSegmentPatternResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import TestSegmentPatternResponseTypeDef


def get_value() -> TestSegmentPatternResponseTypeDef:
    return {
        "match": ...,
    }


# TestSegmentPatternResponseTypeDef definition

class TestSegmentPatternResponseTypeDef(TypedDict):
    match: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectRequestTypeDef

```python
# UpdateProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UpdateProjectRequestTypeDef


def get_value() -> UpdateProjectRequestTypeDef:
    return {
        "project": ...,
    }


# UpdateProjectRequestTypeDef definition

class UpdateProjectRequestTypeDef(TypedDict):
    project: str,
    appConfigResource: NotRequired[ProjectAppConfigResourceConfigTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: ProjectAppConfigResourceConfigTypeDef](./type_defs.md#projectappconfigresourceconfigtypedef) 
## CreateSegmentResponseTypeDef

```python
# CreateSegmentResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CreateSegmentResponseTypeDef


def get_value() -> CreateSegmentResponseTypeDef:
    return {
        "segment": ...,
    }


# CreateSegmentResponseTypeDef definition

class CreateSegmentResponseTypeDef(TypedDict):
    segment: SegmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSegmentResponseTypeDef

```python
# GetSegmentResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetSegmentResponseTypeDef


def get_value() -> GetSegmentResponseTypeDef:
    return {
        "segment": ...,
    }


# GetSegmentResponseTypeDef definition

class GetSegmentResponseTypeDef(TypedDict):
    segment: SegmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSegmentsResponseTypeDef

```python
# ListSegmentsResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListSegmentsResponseTypeDef


def get_value() -> ListSegmentsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# EvaluateFeatureResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import EvaluateFeatureResponseTypeDef


def get_value() -> EvaluateFeatureResponseTypeDef:
    return {
        "details": ...,
    }


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
# EvaluationResultTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import EvaluationResultTypeDef


def get_value() -> EvaluationResultTypeDef:
    return {
        "details": ...,
    }


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
# VariationConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import VariationConfigTypeDef


def get_value() -> VariationConfigTypeDef:
    return {
        "name": ...,
    }


# VariationConfigTypeDef definition

class VariationConfigTypeDef(TypedDict):
    name: str,
    value: VariableValueTypeDef,  # (1)
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) 
## VariationTypeDef

```python
# VariationTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import VariationTypeDef


def get_value() -> VariationTypeDef:
    return {
        "name": ...,
    }


# VariationTypeDef definition

class VariationTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[VariableValueTypeDef],  # (1)
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) 
## FeatureSummaryTypeDef

```python
# FeatureSummaryTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import FeatureSummaryTypeDef


def get_value() -> FeatureSummaryTypeDef:
    return {
        "arn": ...,
    }


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
# EventTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import EventTypeDef


def get_value() -> EventTypeDef:
    return {
        "data": ...,
    }


# EventTypeDef definition

class EventTypeDef(TypedDict):
    data: str,
    timestamp: TimestampTypeDef,
    type: EventTypeType,  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## GetExperimentResultsRequestTypeDef

```python
# GetExperimentResultsRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetExperimentResultsRequestTypeDef


def get_value() -> GetExperimentResultsRequestTypeDef:
    return {
        "experiment": ...,
    }


# GetExperimentResultsRequestTypeDef definition

class GetExperimentResultsRequestTypeDef(TypedDict):
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
## StartExperimentRequestTypeDef

```python
# StartExperimentRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import StartExperimentRequestTypeDef


def get_value() -> StartExperimentRequestTypeDef:
    return {
        "analysisCompleteTime": ...,
    }


# StartExperimentRequestTypeDef definition

class StartExperimentRequestTypeDef(TypedDict):
    analysisCompleteTime: TimestampTypeDef,
    experiment: str,
    project: str,
```

## GetExperimentResultsResponseTypeDef

```python
# GetExperimentResultsResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetExperimentResultsResponseTypeDef


def get_value() -> GetExperimentResultsResponseTypeDef:
    return {
        "details": ...,
    }


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
## ListExperimentsRequestPaginateTypeDef

```python
# ListExperimentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListExperimentsRequestPaginateTypeDef


def get_value() -> ListExperimentsRequestPaginateTypeDef:
    return {
        "project": ...,
    }


# ListExperimentsRequestPaginateTypeDef definition

class ListExperimentsRequestPaginateTypeDef(TypedDict):
    project: str,
    status: NotRequired[ExperimentStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ExperimentStatusType](./literals.md#experimentstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFeaturesRequestPaginateTypeDef

```python
# ListFeaturesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListFeaturesRequestPaginateTypeDef


def get_value() -> ListFeaturesRequestPaginateTypeDef:
    return {
        "project": ...,
    }


# ListFeaturesRequestPaginateTypeDef definition

class ListFeaturesRequestPaginateTypeDef(TypedDict):
    project: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLaunchesRequestPaginateTypeDef

```python
# ListLaunchesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListLaunchesRequestPaginateTypeDef


def get_value() -> ListLaunchesRequestPaginateTypeDef:
    return {
        "project": ...,
    }


# ListLaunchesRequestPaginateTypeDef definition

class ListLaunchesRequestPaginateTypeDef(TypedDict):
    project: str,
    status: NotRequired[LaunchStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestPaginateTypeDef

```python
# ListProjectsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListProjectsRequestPaginateTypeDef


def get_value() -> ListProjectsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListProjectsRequestPaginateTypeDef definition

class ListProjectsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSegmentReferencesRequestPaginateTypeDef

```python
# ListSegmentReferencesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListSegmentReferencesRequestPaginateTypeDef


def get_value() -> ListSegmentReferencesRequestPaginateTypeDef:
    return {
        "segment": ...,
    }


# ListSegmentReferencesRequestPaginateTypeDef definition

class ListSegmentReferencesRequestPaginateTypeDef(TypedDict):
    segment: str,
    type: SegmentReferenceResourceTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SegmentReferenceResourceTypeType](./literals.md#segmentreferenceresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSegmentsRequestPaginateTypeDef

```python
# ListSegmentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListSegmentsRequestPaginateTypeDef


def get_value() -> ListSegmentsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListSegmentsRequestPaginateTypeDef definition

class ListSegmentsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsResponseTypeDef

```python
# ListProjectsResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListProjectsResponseTypeDef


def get_value() -> ListProjectsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# ListSegmentReferencesResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListSegmentReferencesResponseTypeDef


def get_value() -> ListSegmentReferencesResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# MetricGoalConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import MetricGoalConfigTypeDef


def get_value() -> MetricGoalConfigTypeDef:
    return {
        "desiredChange": ...,
    }


# MetricGoalConfigTypeDef definition

class MetricGoalConfigTypeDef(TypedDict):
    metricDefinition: MetricDefinitionConfigTypeDef,  # (2)
    desiredChange: NotRequired[ChangeDirectionEnumType],  # (1)
```

1. See [:material-code-brackets: ChangeDirectionEnumType](./literals.md#changedirectionenumtype) 
2. See [:material-code-braces: MetricDefinitionConfigTypeDef](./type_defs.md#metricdefinitionconfigtypedef) 
## MetricMonitorConfigTypeDef

```python
# MetricMonitorConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import MetricMonitorConfigTypeDef


def get_value() -> MetricMonitorConfigTypeDef:
    return {
        "metricDefinition": ...,
    }


# MetricMonitorConfigTypeDef definition

class MetricMonitorConfigTypeDef(TypedDict):
    metricDefinition: MetricDefinitionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: MetricDefinitionConfigTypeDef](./type_defs.md#metricdefinitionconfigtypedef) 
## MetricGoalTypeDef

```python
# MetricGoalTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import MetricGoalTypeDef


def get_value() -> MetricGoalTypeDef:
    return {
        "desiredChange": ...,
    }


# MetricGoalTypeDef definition

class MetricGoalTypeDef(TypedDict):
    metricDefinition: MetricDefinitionTypeDef,  # (2)
    desiredChange: NotRequired[ChangeDirectionEnumType],  # (1)
```

1. See [:material-code-brackets: ChangeDirectionEnumType](./literals.md#changedirectionenumtype) 
2. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
## MetricMonitorTypeDef

```python
# MetricMonitorTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import MetricMonitorTypeDef


def get_value() -> MetricMonitorTypeDef:
    return {
        "metricDefinition": ...,
    }


# MetricMonitorTypeDef definition

class MetricMonitorTypeDef(TypedDict):
    metricDefinition: MetricDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
## ProjectDataDeliveryConfigTypeDef

```python
# ProjectDataDeliveryConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ProjectDataDeliveryConfigTypeDef


def get_value() -> ProjectDataDeliveryConfigTypeDef:
    return {
        "cloudWatchLogs": ...,
    }


# ProjectDataDeliveryConfigTypeDef definition

class ProjectDataDeliveryConfigTypeDef(TypedDict):
    cloudWatchLogs: NotRequired[CloudWatchLogsDestinationConfigTypeDef],  # (1)
    s3Destination: NotRequired[S3DestinationConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CloudWatchLogsDestinationConfigTypeDef](./type_defs.md#cloudwatchlogsdestinationconfigtypedef) 
2. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
## UpdateProjectDataDeliveryRequestTypeDef

```python
# UpdateProjectDataDeliveryRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UpdateProjectDataDeliveryRequestTypeDef


def get_value() -> UpdateProjectDataDeliveryRequestTypeDef:
    return {
        "project": ...,
    }


# UpdateProjectDataDeliveryRequestTypeDef definition

class UpdateProjectDataDeliveryRequestTypeDef(TypedDict):
    project: str,
    cloudWatchLogs: NotRequired[CloudWatchLogsDestinationConfigTypeDef],  # (1)
    s3Destination: NotRequired[S3DestinationConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CloudWatchLogsDestinationConfigTypeDef](./type_defs.md#cloudwatchlogsdestinationconfigtypedef) 
2. See [:material-code-braces: S3DestinationConfigTypeDef](./type_defs.md#s3destinationconfigtypedef) 
## ProjectDataDeliveryTypeDef

```python
# ProjectDataDeliveryTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ProjectDataDeliveryTypeDef


def get_value() -> ProjectDataDeliveryTypeDef:
    return {
        "cloudWatchLogs": ...,
    }


# ProjectDataDeliveryTypeDef definition

class ProjectDataDeliveryTypeDef(TypedDict):
    cloudWatchLogs: NotRequired[CloudWatchLogsDestinationTypeDef],  # (1)
    s3Destination: NotRequired[S3DestinationTypeDef],  # (2)
```

1. See [:material-code-braces: CloudWatchLogsDestinationTypeDef](./type_defs.md#cloudwatchlogsdestinationtypedef) 
2. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
## PutProjectEventsResponseTypeDef

```python
# PutProjectEventsResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import PutProjectEventsResponseTypeDef


def get_value() -> PutProjectEventsResponseTypeDef:
    return {
        "eventResults": ...,
    }


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
# ScheduledSplitTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ScheduledSplitTypeDef


def get_value() -> ScheduledSplitTypeDef:
    return {
        "groupWeights": ...,
    }


# ScheduledSplitTypeDef definition

class ScheduledSplitTypeDef(TypedDict):
    startTime: datetime,
    groupWeights: NotRequired[Dict[str, int]],
    segmentOverrides: NotRequired[List[SegmentOverrideOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: SegmentOverrideOutputTypeDef](./type_defs.md#segmentoverrideoutputtypedef) 
## BatchEvaluateFeatureResponseTypeDef

```python
# BatchEvaluateFeatureResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import BatchEvaluateFeatureResponseTypeDef


def get_value() -> BatchEvaluateFeatureResponseTypeDef:
    return {
        "results": ...,
    }


# BatchEvaluateFeatureResponseTypeDef definition

class BatchEvaluateFeatureResponseTypeDef(TypedDict):
    results: List[EvaluationResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFeatureRequestTypeDef

```python
# CreateFeatureRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CreateFeatureRequestTypeDef


def get_value() -> CreateFeatureRequestTypeDef:
    return {
        "name": ...,
    }


# CreateFeatureRequestTypeDef definition

class CreateFeatureRequestTypeDef(TypedDict):
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
## UpdateFeatureRequestTypeDef

```python
# UpdateFeatureRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UpdateFeatureRequestTypeDef


def get_value() -> UpdateFeatureRequestTypeDef:
    return {
        "feature": ...,
    }


# UpdateFeatureRequestTypeDef definition

class UpdateFeatureRequestTypeDef(TypedDict):
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
# FeatureTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import FeatureTypeDef


def get_value() -> FeatureTypeDef:
    return {
        "arn": ...,
    }


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
# ListFeaturesResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListFeaturesResponseTypeDef


def get_value() -> ListFeaturesResponseTypeDef:
    return {
        "features": ...,
    }


# ListFeaturesResponseTypeDef definition

class ListFeaturesResponseTypeDef(TypedDict):
    features: List[FeatureSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FeatureSummaryTypeDef](./type_defs.md#featuresummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProjectEventsRequestTypeDef

```python
# PutProjectEventsRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import PutProjectEventsRequestTypeDef


def get_value() -> PutProjectEventsRequestTypeDef:
    return {
        "events": ...,
    }


# PutProjectEventsRequestTypeDef definition

class PutProjectEventsRequestTypeDef(TypedDict):
    events: Sequence[EventTypeDef],  # (1)
    project: str,
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
## CreateExperimentRequestTypeDef

```python
# CreateExperimentRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CreateExperimentRequestTypeDef


def get_value() -> CreateExperimentRequestTypeDef:
    return {
        "metricGoals": ...,
    }


# CreateExperimentRequestTypeDef definition

class CreateExperimentRequestTypeDef(TypedDict):
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
## UpdateExperimentRequestTypeDef

```python
# UpdateExperimentRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UpdateExperimentRequestTypeDef


def get_value() -> UpdateExperimentRequestTypeDef:
    return {
        "experiment": ...,
    }


# UpdateExperimentRequestTypeDef definition

class UpdateExperimentRequestTypeDef(TypedDict):
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
# ExperimentTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ExperimentTypeDef


def get_value() -> ExperimentTypeDef:
    return {
        "arn": ...,
    }


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
## CreateProjectRequestTypeDef

```python
# CreateProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CreateProjectRequestTypeDef


def get_value() -> CreateProjectRequestTypeDef:
    return {
        "name": ...,
    }


# CreateProjectRequestTypeDef definition

class CreateProjectRequestTypeDef(TypedDict):
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
# ProjectTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ProjectTypeDef


def get_value() -> ProjectTypeDef:
    return {
        "activeExperimentCount": ...,
    }


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
# ScheduledSplitsLaunchDefinitionTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ScheduledSplitsLaunchDefinitionTypeDef


def get_value() -> ScheduledSplitsLaunchDefinitionTypeDef:
    return {
        "steps": ...,
    }


# ScheduledSplitsLaunchDefinitionTypeDef definition

class ScheduledSplitsLaunchDefinitionTypeDef(TypedDict):
    steps: NotRequired[List[ScheduledSplitTypeDef]],  # (1)
```

1. See [:material-code-braces: ScheduledSplitTypeDef](./type_defs.md#scheduledsplittypedef) 
## ScheduledSplitConfigTypeDef

```python
# ScheduledSplitConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ScheduledSplitConfigTypeDef


def get_value() -> ScheduledSplitConfigTypeDef:
    return {
        "groupWeights": ...,
    }


# ScheduledSplitConfigTypeDef definition

class ScheduledSplitConfigTypeDef(TypedDict):
    groupWeights: Mapping[str, int],
    startTime: TimestampTypeDef,
    segmentOverrides: NotRequired[Sequence[SegmentOverrideUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: SegmentOverrideTypeDef](./type_defs.md#segmentoverridetypedef) [:material-code-braces: SegmentOverrideOutputTypeDef](./type_defs.md#segmentoverrideoutputtypedef) 
## CreateFeatureResponseTypeDef

```python
# CreateFeatureResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CreateFeatureResponseTypeDef


def get_value() -> CreateFeatureResponseTypeDef:
    return {
        "feature": ...,
    }


# CreateFeatureResponseTypeDef definition

class CreateFeatureResponseTypeDef(TypedDict):
    feature: FeatureTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FeatureTypeDef](./type_defs.md#featuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFeatureResponseTypeDef

```python
# GetFeatureResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetFeatureResponseTypeDef


def get_value() -> GetFeatureResponseTypeDef:
    return {
        "feature": ...,
    }


# GetFeatureResponseTypeDef definition

class GetFeatureResponseTypeDef(TypedDict):
    feature: FeatureTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FeatureTypeDef](./type_defs.md#featuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFeatureResponseTypeDef

```python
# UpdateFeatureResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UpdateFeatureResponseTypeDef


def get_value() -> UpdateFeatureResponseTypeDef:
    return {
        "feature": ...,
    }


# UpdateFeatureResponseTypeDef definition

class UpdateFeatureResponseTypeDef(TypedDict):
    feature: FeatureTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FeatureTypeDef](./type_defs.md#featuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExperimentResponseTypeDef

```python
# CreateExperimentResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CreateExperimentResponseTypeDef


def get_value() -> CreateExperimentResponseTypeDef:
    return {
        "experiment": ...,
    }


# CreateExperimentResponseTypeDef definition

class CreateExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExperimentResponseTypeDef

```python
# GetExperimentResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetExperimentResponseTypeDef


def get_value() -> GetExperimentResponseTypeDef:
    return {
        "experiment": ...,
    }


# GetExperimentResponseTypeDef definition

class GetExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExperimentsResponseTypeDef

```python
# ListExperimentsResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListExperimentsResponseTypeDef


def get_value() -> ListExperimentsResponseTypeDef:
    return {
        "experiments": ...,
    }


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
# UpdateExperimentResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UpdateExperimentResponseTypeDef


def get_value() -> UpdateExperimentResponseTypeDef:
    return {
        "experiment": ...,
    }


# UpdateExperimentResponseTypeDef definition

class UpdateExperimentResponseTypeDef(TypedDict):
    experiment: ExperimentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectResponseTypeDef

```python
# CreateProjectResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CreateProjectResponseTypeDef


def get_value() -> CreateProjectResponseTypeDef:
    return {
        "project": ...,
    }


# CreateProjectResponseTypeDef definition

class CreateProjectResponseTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProjectResponseTypeDef

```python
# GetProjectResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetProjectResponseTypeDef


def get_value() -> GetProjectResponseTypeDef:
    return {
        "project": ...,
    }


# GetProjectResponseTypeDef definition

class GetProjectResponseTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectDataDeliveryResponseTypeDef

```python
# UpdateProjectDataDeliveryResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UpdateProjectDataDeliveryResponseTypeDef


def get_value() -> UpdateProjectDataDeliveryResponseTypeDef:
    return {
        "project": ...,
    }


# UpdateProjectDataDeliveryResponseTypeDef definition

class UpdateProjectDataDeliveryResponseTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectResponseTypeDef

```python
# UpdateProjectResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UpdateProjectResponseTypeDef


def get_value() -> UpdateProjectResponseTypeDef:
    return {
        "project": ...,
    }


# UpdateProjectResponseTypeDef definition

class UpdateProjectResponseTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LaunchTypeDef

```python
# LaunchTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import LaunchTypeDef


def get_value() -> LaunchTypeDef:
    return {
        "arn": ...,
    }


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
# ScheduledSplitsLaunchConfigTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ScheduledSplitsLaunchConfigTypeDef


def get_value() -> ScheduledSplitsLaunchConfigTypeDef:
    return {
        "steps": ...,
    }


# ScheduledSplitsLaunchConfigTypeDef definition

class ScheduledSplitsLaunchConfigTypeDef(TypedDict):
    steps: Sequence[ScheduledSplitConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ScheduledSplitConfigTypeDef](./type_defs.md#scheduledsplitconfigtypedef) 
## CreateLaunchResponseTypeDef

```python
# CreateLaunchResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CreateLaunchResponseTypeDef


def get_value() -> CreateLaunchResponseTypeDef:
    return {
        "launch": ...,
    }


# CreateLaunchResponseTypeDef definition

class CreateLaunchResponseTypeDef(TypedDict):
    launch: LaunchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchTypeDef](./type_defs.md#launchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLaunchResponseTypeDef

```python
# GetLaunchResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import GetLaunchResponseTypeDef


def get_value() -> GetLaunchResponseTypeDef:
    return {
        "launch": ...,
    }


# GetLaunchResponseTypeDef definition

class GetLaunchResponseTypeDef(TypedDict):
    launch: LaunchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchTypeDef](./type_defs.md#launchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLaunchesResponseTypeDef

```python
# ListLaunchesResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import ListLaunchesResponseTypeDef


def get_value() -> ListLaunchesResponseTypeDef:
    return {
        "launches": ...,
    }


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
# StartLaunchResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import StartLaunchResponseTypeDef


def get_value() -> StartLaunchResponseTypeDef:
    return {
        "launch": ...,
    }


# StartLaunchResponseTypeDef definition

class StartLaunchResponseTypeDef(TypedDict):
    launch: LaunchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchTypeDef](./type_defs.md#launchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLaunchResponseTypeDef

```python
# UpdateLaunchResponseTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UpdateLaunchResponseTypeDef


def get_value() -> UpdateLaunchResponseTypeDef:
    return {
        "launch": ...,
    }


# UpdateLaunchResponseTypeDef definition

class UpdateLaunchResponseTypeDef(TypedDict):
    launch: LaunchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchTypeDef](./type_defs.md#launchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLaunchRequestTypeDef

```python
# CreateLaunchRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import CreateLaunchRequestTypeDef


def get_value() -> CreateLaunchRequestTypeDef:
    return {
        "groups": ...,
    }


# CreateLaunchRequestTypeDef definition

class CreateLaunchRequestTypeDef(TypedDict):
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
## UpdateLaunchRequestTypeDef

```python
# UpdateLaunchRequestTypeDef TypedDict usage example

from types_aiobotocore_evidently.type_defs import UpdateLaunchRequestTypeDef


def get_value() -> UpdateLaunchRequestTypeDef:
    return {
        "launch": ...,
    }


# UpdateLaunchRequestTypeDef definition

class UpdateLaunchRequestTypeDef(TypedDict):
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
