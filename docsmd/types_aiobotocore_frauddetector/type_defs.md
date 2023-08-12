# Type definitions

> [Index](../README.md) > [FraudDetector](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [FraudDetector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#FraudDetector)
    type annotations stubs module [types-aiobotocore-frauddetector](https://pypi.org/project/types-aiobotocore-frauddetector/).

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




## ATIMetricDataPointTypeDef

```python
# ATIMetricDataPointTypeDef definition

class ATIMetricDataPointTypeDef(TypedDict):
    cr: NotRequired[float],
    adr: NotRequired[float],
    threshold: NotRequired[float],
    atodr: NotRequired[float],
```

## ATIModelPerformanceTypeDef

```python
# ATIModelPerformanceTypeDef definition

class ATIModelPerformanceTypeDef(TypedDict):
    asi: NotRequired[float],
```

## AggregatedLogOddsMetricTypeDef

```python
# AggregatedLogOddsMetricTypeDef definition

class AggregatedLogOddsMetricTypeDef(TypedDict):
    variableNames: List[str],
    aggregatedVariablesImportance: float,
```

## AggregatedVariablesImpactExplanationTypeDef

```python
# AggregatedVariablesImpactExplanationTypeDef definition

class AggregatedVariablesImpactExplanationTypeDef(TypedDict):
    eventVariableNames: NotRequired[List[str]],
    relativeImpact: NotRequired[str],
    logOddsImpact: NotRequired[float],
```

## AllowDenyListTypeDef

```python
# AllowDenyListTypeDef definition

class AllowDenyListTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    variableType: NotRequired[str],
    createdTime: NotRequired[str],
    updatedTime: NotRequired[str],
    arn: NotRequired[str],
```

## BatchCreateVariableErrorTypeDef

```python
# BatchCreateVariableErrorTypeDef definition

class BatchCreateVariableErrorTypeDef(TypedDict):
    name: NotRequired[str],
    code: NotRequired[int],
    message: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## VariableEntryTypeDef

```python
# VariableEntryTypeDef definition

class VariableEntryTypeDef(TypedDict):
    name: NotRequired[str],
    dataType: NotRequired[str],
    dataSource: NotRequired[str],
    defaultValue: NotRequired[str],
    description: NotRequired[str],
    variableType: NotRequired[str],
```

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

## BatchGetVariableErrorTypeDef

```python
# BatchGetVariableErrorTypeDef definition

class BatchGetVariableErrorTypeDef(TypedDict):
    name: NotRequired[str],
    code: NotRequired[int],
    message: NotRequired[str],
```

## BatchGetVariableRequestRequestTypeDef

```python
# BatchGetVariableRequestRequestTypeDef definition

class BatchGetVariableRequestRequestTypeDef(TypedDict):
    names: Sequence[str],
```

## VariableTypeDef

```python
# VariableTypeDef definition

class VariableTypeDef(TypedDict):
    name: NotRequired[str],
    dataType: NotRequired[DataTypeType],  # (1)
    dataSource: NotRequired[DataSourceType],  # (2)
    defaultValue: NotRequired[str],
    description: NotRequired[str],
    variableType: NotRequired[str],
    lastUpdatedTime: NotRequired[str],
    createdTime: NotRequired[str],
    arn: NotRequired[str],
```

1. See [:material-code-brackets: DataTypeType](./literals.md#datatypetype) 
2. See [:material-code-brackets: DataSourceType](./literals.md#datasourcetype) 
## BatchImportTypeDef

```python
# BatchImportTypeDef definition

class BatchImportTypeDef(TypedDict):
    jobId: NotRequired[str],
    status: NotRequired[AsyncJobStatusType],  # (1)
    failureReason: NotRequired[str],
    startTime: NotRequired[str],
    completionTime: NotRequired[str],
    inputPath: NotRequired[str],
    outputPath: NotRequired[str],
    eventTypeName: NotRequired[str],
    iamRoleArn: NotRequired[str],
    arn: NotRequired[str],
    processedRecordsCount: NotRequired[int],
    failedRecordsCount: NotRequired[int],
    totalRecordsCount: NotRequired[int],
```

1. See [:material-code-brackets: AsyncJobStatusType](./literals.md#asyncjobstatustype) 
## BatchPredictionTypeDef

```python
# BatchPredictionTypeDef definition

class BatchPredictionTypeDef(TypedDict):
    jobId: NotRequired[str],
    status: NotRequired[AsyncJobStatusType],  # (1)
    failureReason: NotRequired[str],
    startTime: NotRequired[str],
    completionTime: NotRequired[str],
    lastHeartbeatTime: NotRequired[str],
    inputPath: NotRequired[str],
    outputPath: NotRequired[str],
    eventTypeName: NotRequired[str],
    detectorName: NotRequired[str],
    detectorVersion: NotRequired[str],
    iamRoleArn: NotRequired[str],
    arn: NotRequired[str],
    processedRecordsCount: NotRequired[int],
    totalRecordsCount: NotRequired[int],
```

1. See [:material-code-brackets: AsyncJobStatusType](./literals.md#asyncjobstatustype) 
## CancelBatchImportJobRequestRequestTypeDef

```python
# CancelBatchImportJobRequestRequestTypeDef definition

class CancelBatchImportJobRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## CancelBatchPredictionJobRequestRequestTypeDef

```python
# CancelBatchPredictionJobRequestRequestTypeDef definition

class CancelBatchPredictionJobRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## ModelVersionTypeDef

```python
# ModelVersionTypeDef definition

class ModelVersionTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    modelVersionNumber: str,
    arn: NotRequired[str],
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    detectorId: str,
    ruleId: str,
    ruleVersion: str,
```

## ExternalEventsDetailTypeDef

```python
# ExternalEventsDetailTypeDef definition

class ExternalEventsDetailTypeDef(TypedDict):
    dataLocation: str,
    dataAccessRoleArn: str,
```

## FieldValidationMessageTypeDef

```python
# FieldValidationMessageTypeDef definition

class FieldValidationMessageTypeDef(TypedDict):
    fieldName: NotRequired[str],
    identifier: NotRequired[str],
    title: NotRequired[str],
    content: NotRequired[str],
    type: NotRequired[str],
```

## FileValidationMessageTypeDef

```python
# FileValidationMessageTypeDef definition

class FileValidationMessageTypeDef(TypedDict):
    title: NotRequired[str],
    content: NotRequired[str],
    type: NotRequired[str],
```

## DeleteBatchImportJobRequestRequestTypeDef

```python
# DeleteBatchImportJobRequestRequestTypeDef definition

class DeleteBatchImportJobRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## DeleteBatchPredictionJobRequestRequestTypeDef

```python
# DeleteBatchPredictionJobRequestRequestTypeDef definition

class DeleteBatchPredictionJobRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## DeleteDetectorRequestRequestTypeDef

```python
# DeleteDetectorRequestRequestTypeDef definition

class DeleteDetectorRequestRequestTypeDef(TypedDict):
    detectorId: str,
```

## DeleteDetectorVersionRequestRequestTypeDef

```python
# DeleteDetectorVersionRequestRequestTypeDef definition

class DeleteDetectorVersionRequestRequestTypeDef(TypedDict):
    detectorId: str,
    detectorVersionId: str,
```

## DeleteEntityTypeRequestRequestTypeDef

```python
# DeleteEntityTypeRequestRequestTypeDef definition

class DeleteEntityTypeRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteEventRequestRequestTypeDef

```python
# DeleteEventRequestRequestTypeDef definition

class DeleteEventRequestRequestTypeDef(TypedDict):
    eventId: str,
    eventTypeName: str,
    deleteAuditHistory: NotRequired[bool],
```

## DeleteEventTypeRequestRequestTypeDef

```python
# DeleteEventTypeRequestRequestTypeDef definition

class DeleteEventTypeRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteEventsByEventTypeRequestRequestTypeDef

```python
# DeleteEventsByEventTypeRequestRequestTypeDef definition

class DeleteEventsByEventTypeRequestRequestTypeDef(TypedDict):
    eventTypeName: str,
```

## DeleteExternalModelRequestRequestTypeDef

```python
# DeleteExternalModelRequestRequestTypeDef definition

class DeleteExternalModelRequestRequestTypeDef(TypedDict):
    modelEndpoint: str,
```

## DeleteLabelRequestRequestTypeDef

```python
# DeleteLabelRequestRequestTypeDef definition

class DeleteLabelRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteListRequestRequestTypeDef

```python
# DeleteListRequestRequestTypeDef definition

class DeleteListRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteModelRequestRequestTypeDef

```python
# DeleteModelRequestRequestTypeDef definition

class DeleteModelRequestRequestTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
## DeleteModelVersionRequestRequestTypeDef

```python
# DeleteModelVersionRequestRequestTypeDef definition

class DeleteModelVersionRequestRequestTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    modelVersionNumber: str,
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
## DeleteOutcomeRequestRequestTypeDef

```python
# DeleteOutcomeRequestRequestTypeDef definition

class DeleteOutcomeRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteVariableRequestRequestTypeDef

```python
# DeleteVariableRequestRequestTypeDef definition

class DeleteVariableRequestRequestTypeDef(TypedDict):
    name: str,
```

## DescribeDetectorRequestRequestTypeDef

```python
# DescribeDetectorRequestRequestTypeDef definition

class DescribeDetectorRequestRequestTypeDef(TypedDict):
    detectorId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## DetectorVersionSummaryTypeDef

```python
# DetectorVersionSummaryTypeDef definition

class DetectorVersionSummaryTypeDef(TypedDict):
    detectorVersionId: NotRequired[str],
    status: NotRequired[DetectorVersionStatusType],  # (1)
    description: NotRequired[str],
    lastUpdatedTime: NotRequired[str],
```

1. See [:material-code-brackets: DetectorVersionStatusType](./literals.md#detectorversionstatustype) 
## DescribeModelVersionsRequestRequestTypeDef

```python
# DescribeModelVersionsRequestRequestTypeDef definition

class DescribeModelVersionsRequestRequestTypeDef(TypedDict):
    modelId: NotRequired[str],
    modelVersionNumber: NotRequired[str],
    modelType: NotRequired[ModelTypeEnumType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
## DetectorTypeDef

```python
# DetectorTypeDef definition

class DetectorTypeDef(TypedDict):
    detectorId: NotRequired[str],
    description: NotRequired[str],
    eventTypeName: NotRequired[str],
    lastUpdatedTime: NotRequired[str],
    createdTime: NotRequired[str],
    arn: NotRequired[str],
```

## EntityTypeDef

```python
# EntityTypeDef definition

class EntityTypeDef(TypedDict):
    entityType: str,
    entityId: str,
```

## EntityTypeTypeDef

```python
# EntityTypeTypeDef definition

class EntityTypeTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    lastUpdatedTime: NotRequired[str],
    createdTime: NotRequired[str],
    arn: NotRequired[str],
```

## EvaluatedExternalModelTypeDef

```python
# EvaluatedExternalModelTypeDef definition

class EvaluatedExternalModelTypeDef(TypedDict):
    modelEndpoint: NotRequired[str],
    useEventVariables: NotRequired[bool],
    inputVariables: NotRequired[Dict[str, str]],
    outputVariables: NotRequired[Dict[str, str]],
```

## EvaluatedRuleTypeDef

```python
# EvaluatedRuleTypeDef definition

class EvaluatedRuleTypeDef(TypedDict):
    ruleId: NotRequired[str],
    ruleVersion: NotRequired[str],
    expression: NotRequired[str],
    expressionWithValues: NotRequired[str],
    outcomes: NotRequired[List[str]],
    evaluated: NotRequired[bool],
    matched: NotRequired[bool],
```

## EventOrchestrationTypeDef

```python
# EventOrchestrationTypeDef definition

class EventOrchestrationTypeDef(TypedDict):
    eventBridgeEnabled: bool,
```

## EventPredictionSummaryTypeDef

```python
# EventPredictionSummaryTypeDef definition

class EventPredictionSummaryTypeDef(TypedDict):
    eventId: NotRequired[str],
    eventTypeName: NotRequired[str],
    eventTimestamp: NotRequired[str],
    predictionTimestamp: NotRequired[str],
    detectorId: NotRequired[str],
    detectorVersionId: NotRequired[str],
```

## IngestedEventStatisticsTypeDef

```python
# IngestedEventStatisticsTypeDef definition

class IngestedEventStatisticsTypeDef(TypedDict):
    numberOfEvents: NotRequired[int],
    eventDataSizeInBytes: NotRequired[int],
    leastRecentEvent: NotRequired[str],
    mostRecentEvent: NotRequired[str],
    lastUpdatedTime: NotRequired[str],
```

## EventVariableSummaryTypeDef

```python
# EventVariableSummaryTypeDef definition

class EventVariableSummaryTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
    source: NotRequired[str],
```

## ExternalModelSummaryTypeDef

```python
# ExternalModelSummaryTypeDef definition

class ExternalModelSummaryTypeDef(TypedDict):
    modelEndpoint: NotRequired[str],
    modelSource: NotRequired[ModelSourceType],  # (1)
```

1. See [:material-code-brackets: ModelSourceType](./literals.md#modelsourcetype) 
## ModelInputConfigurationTypeDef

```python
# ModelInputConfigurationTypeDef definition

class ModelInputConfigurationTypeDef(TypedDict):
    useEventVariables: bool,
    eventTypeName: NotRequired[str],
    format: NotRequired[ModelInputDataFormatType],  # (1)
    jsonInputTemplate: NotRequired[str],
    csvInputTemplate: NotRequired[str],
```

1. See [:material-code-brackets: ModelInputDataFormatType](./literals.md#modelinputdataformattype) 
## ModelOutputConfigurationTypeDef

```python
# ModelOutputConfigurationTypeDef definition

class ModelOutputConfigurationTypeDef(TypedDict):
    format: ModelOutputDataFormatType,  # (1)
    jsonKeyToVariableMap: NotRequired[Dict[str, str]],
    csvIndexToVariableMap: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ModelOutputDataFormatType](./literals.md#modeloutputdataformattype) 
## FilterConditionTypeDef

```python
# FilterConditionTypeDef definition

class FilterConditionTypeDef(TypedDict):
    value: NotRequired[str],
```

## GetBatchImportJobsRequestRequestTypeDef

```python
# GetBatchImportJobsRequestRequestTypeDef definition

class GetBatchImportJobsRequestRequestTypeDef(TypedDict):
    jobId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetBatchPredictionJobsRequestRequestTypeDef

```python
# GetBatchPredictionJobsRequestRequestTypeDef definition

class GetBatchPredictionJobsRequestRequestTypeDef(TypedDict):
    jobId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetDeleteEventsByEventTypeStatusRequestRequestTypeDef

```python
# GetDeleteEventsByEventTypeStatusRequestRequestTypeDef definition

class GetDeleteEventsByEventTypeStatusRequestRequestTypeDef(TypedDict):
    eventTypeName: str,
```

## GetDetectorVersionRequestRequestTypeDef

```python
# GetDetectorVersionRequestRequestTypeDef definition

class GetDetectorVersionRequestRequestTypeDef(TypedDict):
    detectorId: str,
    detectorVersionId: str,
```

## GetDetectorsRequestRequestTypeDef

```python
# GetDetectorsRequestRequestTypeDef definition

class GetDetectorsRequestRequestTypeDef(TypedDict):
    detectorId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetEntityTypesRequestRequestTypeDef

```python
# GetEntityTypesRequestRequestTypeDef definition

class GetEntityTypesRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetEventPredictionMetadataRequestRequestTypeDef

```python
# GetEventPredictionMetadataRequestRequestTypeDef definition

class GetEventPredictionMetadataRequestRequestTypeDef(TypedDict):
    eventId: str,
    eventTypeName: str,
    detectorId: str,
    detectorVersionId: str,
    predictionTimestamp: str,
```

## RuleResultTypeDef

```python
# RuleResultTypeDef definition

class RuleResultTypeDef(TypedDict):
    ruleId: NotRequired[str],
    outcomes: NotRequired[List[str]],
```

## GetEventRequestRequestTypeDef

```python
# GetEventRequestRequestTypeDef definition

class GetEventRequestRequestTypeDef(TypedDict):
    eventId: str,
    eventTypeName: str,
```

## GetEventTypesRequestRequestTypeDef

```python
# GetEventTypesRequestRequestTypeDef definition

class GetEventTypesRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetExternalModelsRequestRequestTypeDef

```python
# GetExternalModelsRequestRequestTypeDef definition

class GetExternalModelsRequestRequestTypeDef(TypedDict):
    modelEndpoint: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## KMSKeyTypeDef

```python
# KMSKeyTypeDef definition

class KMSKeyTypeDef(TypedDict):
    kmsEncryptionKeyArn: NotRequired[str],
```

## GetLabelsRequestRequestTypeDef

```python
# GetLabelsRequestRequestTypeDef definition

class GetLabelsRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## LabelTypeDef

```python
# LabelTypeDef definition

class LabelTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    lastUpdatedTime: NotRequired[str],
    createdTime: NotRequired[str],
    arn: NotRequired[str],
```

## GetListElementsRequestRequestTypeDef

```python
# GetListElementsRequestRequestTypeDef definition

class GetListElementsRequestRequestTypeDef(TypedDict):
    name: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetListsMetadataRequestRequestTypeDef

```python
# GetListsMetadataRequestRequestTypeDef definition

class GetListsMetadataRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetModelVersionRequestRequestTypeDef

```python
# GetModelVersionRequestRequestTypeDef definition

class GetModelVersionRequestRequestTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    modelVersionNumber: str,
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
## GetModelsRequestRequestTypeDef

```python
# GetModelsRequestRequestTypeDef definition

class GetModelsRequestRequestTypeDef(TypedDict):
    modelId: NotRequired[str],
    modelType: NotRequired[ModelTypeEnumType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
## ModelTypeDef

```python
# ModelTypeDef definition

class ModelTypeDef(TypedDict):
    modelId: NotRequired[str],
    modelType: NotRequired[ModelTypeEnumType],  # (1)
    description: NotRequired[str],
    eventTypeName: NotRequired[str],
    createdTime: NotRequired[str],
    lastUpdatedTime: NotRequired[str],
    arn: NotRequired[str],
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
## GetOutcomesRequestRequestTypeDef

```python
# GetOutcomesRequestRequestTypeDef definition

class GetOutcomesRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## OutcomeTypeDef

```python
# OutcomeTypeDef definition

class OutcomeTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    lastUpdatedTime: NotRequired[str],
    createdTime: NotRequired[str],
    arn: NotRequired[str],
```

## GetRulesRequestRequestTypeDef

```python
# GetRulesRequestRequestTypeDef definition

class GetRulesRequestRequestTypeDef(TypedDict):
    detectorId: str,
    ruleId: NotRequired[str],
    ruleVersion: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RuleDetailTypeDef

```python
# RuleDetailTypeDef definition

class RuleDetailTypeDef(TypedDict):
    ruleId: NotRequired[str],
    description: NotRequired[str],
    detectorId: NotRequired[str],
    ruleVersion: NotRequired[str],
    expression: NotRequired[str],
    language: NotRequired[LanguageType],  # (1)
    outcomes: NotRequired[List[str]],
    lastUpdatedTime: NotRequired[str],
    createdTime: NotRequired[str],
    arn: NotRequired[str],
```

1. See [:material-code-brackets: LanguageType](./literals.md#languagetype) 
## GetVariablesRequestRequestTypeDef

```python
# GetVariablesRequestRequestTypeDef definition

class GetVariablesRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## IngestedEventsTimeWindowTypeDef

```python
# IngestedEventsTimeWindowTypeDef definition

class IngestedEventsTimeWindowTypeDef(TypedDict):
    startTime: str,
    endTime: str,
```

## LabelSchemaTypeDef

```python
# LabelSchemaTypeDef definition

class LabelSchemaTypeDef(TypedDict):
    labelMapper: NotRequired[Mapping[str, Sequence[str]]],
    unlabeledEventsTreatment: NotRequired[UnlabeledEventsTreatmentType],  # (1)
```

1. See [:material-code-brackets: UnlabeledEventsTreatmentType](./literals.md#unlabeledeventstreatmenttype) 
## PredictionTimeRangeTypeDef

```python
# PredictionTimeRangeTypeDef definition

class PredictionTimeRangeTypeDef(TypedDict):
    startTime: str,
    endTime: str,
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## LogOddsMetricTypeDef

```python
# LogOddsMetricTypeDef definition

class LogOddsMetricTypeDef(TypedDict):
    variableName: str,
    variableType: str,
    variableImportance: float,
```

## MetricDataPointTypeDef

```python
# MetricDataPointTypeDef definition

class MetricDataPointTypeDef(TypedDict):
    fpr: NotRequired[float],
    precision: NotRequired[float],
    tpr: NotRequired[float],
    threshold: NotRequired[float],
```

## OFIMetricDataPointTypeDef

```python
# OFIMetricDataPointTypeDef definition

class OFIMetricDataPointTypeDef(TypedDict):
    fpr: NotRequired[float],
    precision: NotRequired[float],
    tpr: NotRequired[float],
    threshold: NotRequired[float],
```

## UncertaintyRangeTypeDef

```python
# UncertaintyRangeTypeDef definition

class UncertaintyRangeTypeDef(TypedDict):
    lowerBoundValue: float,
    upperBoundValue: float,
```

## VariableImpactExplanationTypeDef

```python
# VariableImpactExplanationTypeDef definition

class VariableImpactExplanationTypeDef(TypedDict):
    eventVariableName: NotRequired[str],
    relativeImpact: NotRequired[str],
    logOddsImpact: NotRequired[float],
```

## PutKMSEncryptionKeyRequestRequestTypeDef

```python
# PutKMSEncryptionKeyRequestRequestTypeDef definition

class PutKMSEncryptionKeyRequestRequestTypeDef(TypedDict):
    kmsEncryptionKeyArn: str,
```

## TFIMetricDataPointTypeDef

```python
# TFIMetricDataPointTypeDef definition

class TFIMetricDataPointTypeDef(TypedDict):
    fpr: NotRequired[float],
    precision: NotRequired[float],
    tpr: NotRequired[float],
    threshold: NotRequired[float],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tagKeys: Sequence[str],
```

## UpdateDetectorVersionMetadataRequestRequestTypeDef

```python
# UpdateDetectorVersionMetadataRequestRequestTypeDef definition

class UpdateDetectorVersionMetadataRequestRequestTypeDef(TypedDict):
    detectorId: str,
    detectorVersionId: str,
    description: str,
```

## UpdateDetectorVersionStatusRequestRequestTypeDef

```python
# UpdateDetectorVersionStatusRequestRequestTypeDef definition

class UpdateDetectorVersionStatusRequestRequestTypeDef(TypedDict):
    detectorId: str,
    detectorVersionId: str,
    status: DetectorVersionStatusType,  # (1)
```

1. See [:material-code-brackets: DetectorVersionStatusType](./literals.md#detectorversionstatustype) 
## UpdateEventLabelRequestRequestTypeDef

```python
# UpdateEventLabelRequestRequestTypeDef definition

class UpdateEventLabelRequestRequestTypeDef(TypedDict):
    eventId: str,
    eventTypeName: str,
    assignedLabel: str,
    labelTimestamp: str,
```

## UpdateListRequestRequestTypeDef

```python
# UpdateListRequestRequestTypeDef definition

class UpdateListRequestRequestTypeDef(TypedDict):
    name: str,
    elements: NotRequired[Sequence[str]],
    description: NotRequired[str],
    updateMode: NotRequired[ListUpdateModeType],  # (1)
    variableType: NotRequired[str],
```

1. See [:material-code-brackets: ListUpdateModeType](./literals.md#listupdatemodetype) 
## UpdateModelRequestRequestTypeDef

```python
# UpdateModelRequestRequestTypeDef definition

class UpdateModelRequestRequestTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
## UpdateModelVersionStatusRequestRequestTypeDef

```python
# UpdateModelVersionStatusRequestRequestTypeDef definition

class UpdateModelVersionStatusRequestRequestTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    modelVersionNumber: str,
    status: ModelVersionStatusType,  # (2)
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
2. See [:material-code-brackets: ModelVersionStatusType](./literals.md#modelversionstatustype) 
## UpdateVariableRequestRequestTypeDef

```python
# UpdateVariableRequestRequestTypeDef definition

class UpdateVariableRequestRequestTypeDef(TypedDict):
    name: str,
    defaultValue: NotRequired[str],
    description: NotRequired[str],
    variableType: NotRequired[str],
```

## ATITrainingMetricsValueTypeDef

```python
# ATITrainingMetricsValueTypeDef definition

class ATITrainingMetricsValueTypeDef(TypedDict):
    metricDataPoints: NotRequired[List[ATIMetricDataPointTypeDef]],  # (1)
    modelPerformance: NotRequired[ATIModelPerformanceTypeDef],  # (2)
```

1. See [:material-code-braces: ATIMetricDataPointTypeDef](./type_defs.md#atimetricdatapointtypedef) 
2. See [:material-code-braces: ATIModelPerformanceTypeDef](./type_defs.md#atimodelperformancetypedef) 
## AggregatedVariablesImportanceMetricsTypeDef

```python
# AggregatedVariablesImportanceMetricsTypeDef definition

class AggregatedVariablesImportanceMetricsTypeDef(TypedDict):
    logOddsMetrics: NotRequired[List[AggregatedLogOddsMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: AggregatedLogOddsMetricTypeDef](./type_defs.md#aggregatedlogoddsmetrictypedef) 
## CreateBatchImportJobRequestRequestTypeDef

```python
# CreateBatchImportJobRequestRequestTypeDef definition

class CreateBatchImportJobRequestRequestTypeDef(TypedDict):
    jobId: str,
    inputPath: str,
    outputPath: str,
    eventTypeName: str,
    iamRoleArn: str,
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateBatchPredictionJobRequestRequestTypeDef

```python
# CreateBatchPredictionJobRequestRequestTypeDef definition

class CreateBatchPredictionJobRequestRequestTypeDef(TypedDict):
    jobId: str,
    inputPath: str,
    outputPath: str,
    eventTypeName: str,
    detectorName: str,
    iamRoleArn: str,
    detectorVersion: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateListRequestRequestTypeDef

```python
# CreateListRequestRequestTypeDef definition

class CreateListRequestRequestTypeDef(TypedDict):
    name: str,
    elements: NotRequired[Sequence[str]],
    variableType: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateModelRequestRequestTypeDef

```python
# CreateModelRequestRequestTypeDef definition

class CreateModelRequestRequestTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    eventTypeName: str,
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRuleRequestRequestTypeDef

```python
# CreateRuleRequestRequestTypeDef definition

class CreateRuleRequestRequestTypeDef(TypedDict):
    ruleId: str,
    detectorId: str,
    expression: str,
    language: LanguageType,  # (1)
    outcomes: Sequence[str],
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: LanguageType](./literals.md#languagetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateVariableRequestRequestTypeDef

```python
# CreateVariableRequestRequestTypeDef definition

class CreateVariableRequestRequestTypeDef(TypedDict):
    name: str,
    dataType: DataTypeType,  # (1)
    dataSource: DataSourceType,  # (2)
    defaultValue: str,
    description: NotRequired[str],
    variableType: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: DataTypeType](./literals.md#datatypetype) 
2. See [:material-code-brackets: DataSourceType](./literals.md#datasourcetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutDetectorRequestRequestTypeDef

```python
# PutDetectorRequestRequestTypeDef definition

class PutDetectorRequestRequestTypeDef(TypedDict):
    detectorId: str,
    eventTypeName: str,
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutEntityTypeRequestRequestTypeDef

```python
# PutEntityTypeRequestRequestTypeDef definition

class PutEntityTypeRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutLabelRequestRequestTypeDef

```python
# PutLabelRequestRequestTypeDef definition

class PutLabelRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutOutcomeRequestRequestTypeDef

```python
# PutOutcomeRequestRequestTypeDef definition

class PutOutcomeRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceARN: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## BatchCreateVariableRequestRequestTypeDef

```python
# BatchCreateVariableRequestRequestTypeDef definition

class BatchCreateVariableRequestRequestTypeDef(TypedDict):
    variableEntries: Sequence[VariableEntryTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: VariableEntryTypeDef](./type_defs.md#variableentrytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## BatchCreateVariableResultTypeDef

```python
# BatchCreateVariableResultTypeDef definition

class BatchCreateVariableResultTypeDef(TypedDict):
    errors: List[BatchCreateVariableErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchCreateVariableErrorTypeDef](./type_defs.md#batchcreatevariableerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDetectorVersionResultTypeDef

```python
# CreateDetectorVersionResultTypeDef definition

class CreateDetectorVersionResultTypeDef(TypedDict):
    detectorId: str,
    detectorVersionId: str,
    status: DetectorVersionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DetectorVersionStatusType](./literals.md#detectorversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelVersionResultTypeDef

```python
# CreateModelVersionResultTypeDef definition

class CreateModelVersionResultTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    modelVersionNumber: str,
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEventsByEventTypeResultTypeDef

```python
# DeleteEventsByEventTypeResultTypeDef definition

class DeleteEventsByEventTypeResultTypeDef(TypedDict):
    eventTypeName: str,
    eventsDeletionStatus: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeleteEventsByEventTypeStatusResultTypeDef

```python
# GetDeleteEventsByEventTypeStatusResultTypeDef definition

class GetDeleteEventsByEventTypeStatusResultTypeDef(TypedDict):
    eventTypeName: str,
    eventsDeletionStatus: AsyncJobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AsyncJobStatusType](./literals.md#asyncjobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetListElementsResultTypeDef

```python
# GetListElementsResultTypeDef definition

class GetListElementsResultTypeDef(TypedDict):
    elements: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetListsMetadataResultTypeDef

```python
# GetListsMetadataResultTypeDef definition

class GetListsMetadataResultTypeDef(TypedDict):
    lists: List[AllowDenyListTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AllowDenyListTypeDef](./type_defs.md#allowdenylisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateModelVersionResultTypeDef

```python
# UpdateModelVersionResultTypeDef definition

class UpdateModelVersionResultTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    modelVersionNumber: str,
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetVariableResultTypeDef

```python
# BatchGetVariableResultTypeDef definition

class BatchGetVariableResultTypeDef(TypedDict):
    variables: List[VariableTypeDef],  # (1)
    errors: List[BatchGetVariableErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: VariableTypeDef](./type_defs.md#variabletypedef) 
2. See [:material-code-braces: BatchGetVariableErrorTypeDef](./type_defs.md#batchgetvariableerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVariablesResultTypeDef

```python
# GetVariablesResultTypeDef definition

class GetVariablesResultTypeDef(TypedDict):
    variables: List[VariableTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VariableTypeDef](./type_defs.md#variabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBatchImportJobsResultTypeDef

```python
# GetBatchImportJobsResultTypeDef definition

class GetBatchImportJobsResultTypeDef(TypedDict):
    batchImports: List[BatchImportTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchImportTypeDef](./type_defs.md#batchimporttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBatchPredictionJobsResultTypeDef

```python
# GetBatchPredictionJobsResultTypeDef definition

class GetBatchPredictionJobsResultTypeDef(TypedDict):
    batchPredictions: List[BatchPredictionTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPredictionTypeDef](./type_defs.md#batchpredictiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelEndpointDataBlobTypeDef

```python
# ModelEndpointDataBlobTypeDef definition

class ModelEndpointDataBlobTypeDef(TypedDict):
    byteBuffer: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    contentType: NotRequired[str],
```

## ModelScoresTypeDef

```python
# ModelScoresTypeDef definition

class ModelScoresTypeDef(TypedDict):
    modelVersion: NotRequired[ModelVersionTypeDef],  # (1)
    scores: NotRequired[Dict[str, float]],
```

1. See [:material-code-braces: ModelVersionTypeDef](./type_defs.md#modelversiontypedef) 
## CreateDetectorVersionRequestRequestTypeDef

```python
# CreateDetectorVersionRequestRequestTypeDef definition

class CreateDetectorVersionRequestRequestTypeDef(TypedDict):
    detectorId: str,
    rules: Sequence[RuleTypeDef],  # (1)
    description: NotRequired[str],
    externalModelEndpoints: NotRequired[Sequence[str]],
    modelVersions: NotRequired[Sequence[ModelVersionTypeDef]],  # (2)
    ruleExecutionMode: NotRequired[RuleExecutionModeType],  # (3)
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ModelVersionTypeDef](./type_defs.md#modelversiontypedef) 
3. See [:material-code-brackets: RuleExecutionModeType](./literals.md#ruleexecutionmodetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRuleResultTypeDef

```python
# CreateRuleResultTypeDef definition

class CreateRuleResultTypeDef(TypedDict):
    rule: RuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRuleRequestRequestTypeDef

```python
# DeleteRuleRequestRequestTypeDef definition

class DeleteRuleRequestRequestTypeDef(TypedDict):
    rule: RuleTypeDef,  # (1)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## GetDetectorVersionResultTypeDef

```python
# GetDetectorVersionResultTypeDef definition

class GetDetectorVersionResultTypeDef(TypedDict):
    detectorId: str,
    detectorVersionId: str,
    description: str,
    externalModelEndpoints: List[str],
    modelVersions: List[ModelVersionTypeDef],  # (1)
    rules: List[RuleTypeDef],  # (2)
    status: DetectorVersionStatusType,  # (3)
    lastUpdatedTime: str,
    createdTime: str,
    ruleExecutionMode: RuleExecutionModeType,  # (4)
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ModelVersionTypeDef](./type_defs.md#modelversiontypedef) 
2. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
3. See [:material-code-brackets: DetectorVersionStatusType](./literals.md#detectorversionstatustype) 
4. See [:material-code-brackets: RuleExecutionModeType](./literals.md#ruleexecutionmodetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDetectorVersionRequestRequestTypeDef

```python
# UpdateDetectorVersionRequestRequestTypeDef definition

class UpdateDetectorVersionRequestRequestTypeDef(TypedDict):
    detectorId: str,
    detectorVersionId: str,
    externalModelEndpoints: Sequence[str],
    rules: Sequence[RuleTypeDef],  # (1)
    description: NotRequired[str],
    modelVersions: NotRequired[Sequence[ModelVersionTypeDef]],  # (2)
    ruleExecutionMode: NotRequired[RuleExecutionModeType],  # (3)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ModelVersionTypeDef](./type_defs.md#modelversiontypedef) 
3. See [:material-code-brackets: RuleExecutionModeType](./literals.md#ruleexecutionmodetype) 
## UpdateRuleMetadataRequestRequestTypeDef

```python
# UpdateRuleMetadataRequestRequestTypeDef definition

class UpdateRuleMetadataRequestRequestTypeDef(TypedDict):
    rule: RuleTypeDef,  # (1)
    description: str,
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## UpdateRuleVersionRequestRequestTypeDef

```python
# UpdateRuleVersionRequestRequestTypeDef definition

class UpdateRuleVersionRequestRequestTypeDef(TypedDict):
    rule: RuleTypeDef,  # (1)
    expression: str,
    language: LanguageType,  # (2)
    outcomes: Sequence[str],
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-brackets: LanguageType](./literals.md#languagetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateRuleVersionResultTypeDef

```python
# UpdateRuleVersionResultTypeDef definition

class UpdateRuleVersionResultTypeDef(TypedDict):
    rule: RuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataValidationMetricsTypeDef

```python
# DataValidationMetricsTypeDef definition

class DataValidationMetricsTypeDef(TypedDict):
    fileLevelMessages: NotRequired[List[FileValidationMessageTypeDef]],  # (1)
    fieldLevelMessages: NotRequired[List[FieldValidationMessageTypeDef]],  # (2)
```

1. See [:material-code-braces: FileValidationMessageTypeDef](./type_defs.md#filevalidationmessagetypedef) 
2. See [:material-code-braces: FieldValidationMessageTypeDef](./type_defs.md#fieldvalidationmessagetypedef) 
## DescribeDetectorResultTypeDef

```python
# DescribeDetectorResultTypeDef definition

class DescribeDetectorResultTypeDef(TypedDict):
    detectorId: str,
    detectorVersionSummaries: List[DetectorVersionSummaryTypeDef],  # (1)
    nextToken: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorVersionSummaryTypeDef](./type_defs.md#detectorversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDetectorsResultTypeDef

```python
# GetDetectorsResultTypeDef definition

class GetDetectorsResultTypeDef(TypedDict):
    detectors: List[DetectorTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DetectorTypeDef](./type_defs.md#detectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    eventId: NotRequired[str],
    eventTypeName: NotRequired[str],
    eventTimestamp: NotRequired[str],
    eventVariables: NotRequired[Dict[str, str]],
    currentLabel: NotRequired[str],
    labelTimestamp: NotRequired[str],
    entities: NotRequired[List[EntityTypeDef]],  # (1)
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
## SendEventRequestRequestTypeDef

```python
# SendEventRequestRequestTypeDef definition

class SendEventRequestRequestTypeDef(TypedDict):
    eventId: str,
    eventTypeName: str,
    eventTimestamp: str,
    eventVariables: Mapping[str, str],
    entities: Sequence[EntityTypeDef],  # (1)
    assignedLabel: NotRequired[str],
    labelTimestamp: NotRequired[str],
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
## GetEntityTypesResultTypeDef

```python
# GetEntityTypesResultTypeDef definition

class GetEntityTypesResultTypeDef(TypedDict):
    entityTypes: List[EntityTypeTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntityTypeTypeDef](./type_defs.md#entitytypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEventTypeRequestRequestTypeDef

```python
# PutEventTypeRequestRequestTypeDef definition

class PutEventTypeRequestRequestTypeDef(TypedDict):
    name: str,
    eventVariables: Sequence[str],
    entityTypes: Sequence[str],
    description: NotRequired[str],
    labels: NotRequired[Sequence[str]],
    eventIngestion: NotRequired[EventIngestionType],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    eventOrchestration: NotRequired[EventOrchestrationTypeDef],  # (3)
```

1. See [:material-code-brackets: EventIngestionType](./literals.md#eventingestiontype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EventOrchestrationTypeDef](./type_defs.md#eventorchestrationtypedef) 
## ListEventPredictionsResultTypeDef

```python
# ListEventPredictionsResultTypeDef definition

class ListEventPredictionsResultTypeDef(TypedDict):
    eventPredictionSummaries: List[EventPredictionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventPredictionSummaryTypeDef](./type_defs.md#eventpredictionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventTypeTypeDef

```python
# EventTypeTypeDef definition

class EventTypeTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    eventVariables: NotRequired[List[str]],
    labels: NotRequired[List[str]],
    entityTypes: NotRequired[List[str]],
    eventIngestion: NotRequired[EventIngestionType],  # (1)
    ingestedEventStatistics: NotRequired[IngestedEventStatisticsTypeDef],  # (2)
    lastUpdatedTime: NotRequired[str],
    createdTime: NotRequired[str],
    arn: NotRequired[str],
    eventOrchestration: NotRequired[EventOrchestrationTypeDef],  # (3)
```

1. See [:material-code-brackets: EventIngestionType](./literals.md#eventingestiontype) 
2. See [:material-code-braces: IngestedEventStatisticsTypeDef](./type_defs.md#ingestedeventstatisticstypedef) 
3. See [:material-code-braces: EventOrchestrationTypeDef](./type_defs.md#eventorchestrationtypedef) 
## ExternalModelOutputsTypeDef

```python
# ExternalModelOutputsTypeDef definition

class ExternalModelOutputsTypeDef(TypedDict):
    externalModel: NotRequired[ExternalModelSummaryTypeDef],  # (1)
    outputs: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ExternalModelSummaryTypeDef](./type_defs.md#externalmodelsummarytypedef) 
## ExternalModelTypeDef

```python
# ExternalModelTypeDef definition

class ExternalModelTypeDef(TypedDict):
    modelEndpoint: NotRequired[str],
    modelSource: NotRequired[ModelSourceType],  # (1)
    invokeModelEndpointRoleArn: NotRequired[str],
    inputConfiguration: NotRequired[ModelInputConfigurationTypeDef],  # (2)
    outputConfiguration: NotRequired[ModelOutputConfigurationTypeDef],  # (3)
    modelEndpointStatus: NotRequired[ModelEndpointStatusType],  # (4)
    lastUpdatedTime: NotRequired[str],
    createdTime: NotRequired[str],
    arn: NotRequired[str],
```

1. See [:material-code-brackets: ModelSourceType](./literals.md#modelsourcetype) 
2. See [:material-code-braces: ModelInputConfigurationTypeDef](./type_defs.md#modelinputconfigurationtypedef) 
3. See [:material-code-braces: ModelOutputConfigurationTypeDef](./type_defs.md#modeloutputconfigurationtypedef) 
4. See [:material-code-brackets: ModelEndpointStatusType](./literals.md#modelendpointstatustype) 
## PutExternalModelRequestRequestTypeDef

```python
# PutExternalModelRequestRequestTypeDef definition

class PutExternalModelRequestRequestTypeDef(TypedDict):
    modelEndpoint: str,
    modelSource: ModelSourceType,  # (1)
    invokeModelEndpointRoleArn: str,
    inputConfiguration: ModelInputConfigurationTypeDef,  # (2)
    outputConfiguration: ModelOutputConfigurationTypeDef,  # (3)
    modelEndpointStatus: ModelEndpointStatusType,  # (4)
    tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-brackets: ModelSourceType](./literals.md#modelsourcetype) 
2. See [:material-code-braces: ModelInputConfigurationTypeDef](./type_defs.md#modelinputconfigurationtypedef) 
3. See [:material-code-braces: ModelOutputConfigurationTypeDef](./type_defs.md#modeloutputconfigurationtypedef) 
4. See [:material-code-brackets: ModelEndpointStatusType](./literals.md#modelendpointstatustype) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetKMSEncryptionKeyResultTypeDef

```python
# GetKMSEncryptionKeyResultTypeDef definition

class GetKMSEncryptionKeyResultTypeDef(TypedDict):
    kmsKey: KMSKeyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KMSKeyTypeDef](./type_defs.md#kmskeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLabelsResultTypeDef

```python
# GetLabelsResultTypeDef definition

class GetLabelsResultTypeDef(TypedDict):
    labels: List[LabelTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LabelTypeDef](./type_defs.md#labeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetModelsResultTypeDef

```python
# GetModelsResultTypeDef definition

class GetModelsResultTypeDef(TypedDict):
    nextToken: str,
    models: List[ModelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOutcomesResultTypeDef

```python
# GetOutcomesResultTypeDef definition

class GetOutcomesResultTypeDef(TypedDict):
    outcomes: List[OutcomeTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutcomeTypeDef](./type_defs.md#outcometypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRulesResultTypeDef

```python
# GetRulesResultTypeDef definition

class GetRulesResultTypeDef(TypedDict):
    ruleDetails: List[RuleDetailTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleDetailTypeDef](./type_defs.md#ruledetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IngestedEventsDetailTypeDef

```python
# IngestedEventsDetailTypeDef definition

class IngestedEventsDetailTypeDef(TypedDict):
    ingestedEventsTimeWindow: IngestedEventsTimeWindowTypeDef,  # (1)
```

1. See [:material-code-braces: IngestedEventsTimeWindowTypeDef](./type_defs.md#ingestedeventstimewindowtypedef) 
## TrainingDataSchemaTypeDef

```python
# TrainingDataSchemaTypeDef definition

class TrainingDataSchemaTypeDef(TypedDict):
    modelVariables: Sequence[str],
    labelSchema: NotRequired[LabelSchemaTypeDef],  # (1)
```

1. See [:material-code-braces: LabelSchemaTypeDef](./type_defs.md#labelschematypedef) 
## ListEventPredictionsRequestRequestTypeDef

```python
# ListEventPredictionsRequestRequestTypeDef definition

class ListEventPredictionsRequestRequestTypeDef(TypedDict):
    eventId: NotRequired[FilterConditionTypeDef],  # (1)
    eventType: NotRequired[FilterConditionTypeDef],  # (1)
    detectorId: NotRequired[FilterConditionTypeDef],  # (1)
    detectorVersionId: NotRequired[FilterConditionTypeDef],  # (1)
    predictionTimeRange: NotRequired[PredictionTimeRangeTypeDef],  # (5)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterConditionTypeDef](./type_defs.md#filterconditiontypedef) 
2. See [:material-code-braces: FilterConditionTypeDef](./type_defs.md#filterconditiontypedef) 
3. See [:material-code-braces: FilterConditionTypeDef](./type_defs.md#filterconditiontypedef) 
4. See [:material-code-braces: FilterConditionTypeDef](./type_defs.md#filterconditiontypedef) 
5. See [:material-code-braces: PredictionTimeRangeTypeDef](./type_defs.md#predictiontimerangetypedef) 
## VariableImportanceMetricsTypeDef

```python
# VariableImportanceMetricsTypeDef definition

class VariableImportanceMetricsTypeDef(TypedDict):
    logOddsMetrics: NotRequired[List[LogOddsMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: LogOddsMetricTypeDef](./type_defs.md#logoddsmetrictypedef) 
## TrainingMetricsTypeDef

```python
# TrainingMetricsTypeDef definition

class TrainingMetricsTypeDef(TypedDict):
    auc: NotRequired[float],
    metricDataPoints: NotRequired[List[MetricDataPointTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricDataPointTypeDef](./type_defs.md#metricdatapointtypedef) 
## OFIModelPerformanceTypeDef

```python
# OFIModelPerformanceTypeDef definition

class OFIModelPerformanceTypeDef(TypedDict):
    auc: NotRequired[float],
    uncertaintyRange: NotRequired[UncertaintyRangeTypeDef],  # (1)
```

1. See [:material-code-braces: UncertaintyRangeTypeDef](./type_defs.md#uncertaintyrangetypedef) 
## TFIModelPerformanceTypeDef

```python
# TFIModelPerformanceTypeDef definition

class TFIModelPerformanceTypeDef(TypedDict):
    auc: NotRequired[float],
    uncertaintyRange: NotRequired[UncertaintyRangeTypeDef],  # (1)
```

1. See [:material-code-braces: UncertaintyRangeTypeDef](./type_defs.md#uncertaintyrangetypedef) 
## PredictionExplanationsTypeDef

```python
# PredictionExplanationsTypeDef definition

class PredictionExplanationsTypeDef(TypedDict):
    variableImpactExplanations: NotRequired[List[VariableImpactExplanationTypeDef]],  # (1)
    aggregatedVariablesImpactExplanations: NotRequired[List[AggregatedVariablesImpactExplanationTypeDef]],  # (2)
```

1. See [:material-code-braces: VariableImpactExplanationTypeDef](./type_defs.md#variableimpactexplanationtypedef) 
2. See [:material-code-braces: AggregatedVariablesImpactExplanationTypeDef](./type_defs.md#aggregatedvariablesimpactexplanationtypedef) 
## GetEventPredictionRequestRequestTypeDef

```python
# GetEventPredictionRequestRequestTypeDef definition

class GetEventPredictionRequestRequestTypeDef(TypedDict):
    detectorId: str,
    eventId: str,
    eventTypeName: str,
    entities: Sequence[EntityTypeDef],  # (1)
    eventTimestamp: str,
    eventVariables: Mapping[str, str],
    detectorVersionId: NotRequired[str],
    externalModelEndpointDataBlobs: NotRequired[Mapping[str, ModelEndpointDataBlobTypeDef]],  # (2)
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
2. See [:material-code-braces: ModelEndpointDataBlobTypeDef](./type_defs.md#modelendpointdatablobtypedef) 
## GetEventResultTypeDef

```python
# GetEventResultTypeDef definition

class GetEventResultTypeDef(TypedDict):
    event: EventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEventTypesResultTypeDef

```python
# GetEventTypesResultTypeDef definition

class GetEventTypesResultTypeDef(TypedDict):
    eventTypes: List[EventTypeTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventTypeTypeDef](./type_defs.md#eventtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEventPredictionResultTypeDef

```python
# GetEventPredictionResultTypeDef definition

class GetEventPredictionResultTypeDef(TypedDict):
    modelScores: List[ModelScoresTypeDef],  # (1)
    ruleResults: List[RuleResultTypeDef],  # (2)
    externalModelOutputs: List[ExternalModelOutputsTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ModelScoresTypeDef](./type_defs.md#modelscorestypedef) 
2. See [:material-code-braces: RuleResultTypeDef](./type_defs.md#ruleresulttypedef) 
3. See [:material-code-braces: ExternalModelOutputsTypeDef](./type_defs.md#externalmodeloutputstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExternalModelsResultTypeDef

```python
# GetExternalModelsResultTypeDef definition

class GetExternalModelsResultTypeDef(TypedDict):
    externalModels: List[ExternalModelTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExternalModelTypeDef](./type_defs.md#externalmodeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateModelVersionRequestRequestTypeDef

```python
# UpdateModelVersionRequestRequestTypeDef definition

class UpdateModelVersionRequestRequestTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    majorVersionNumber: str,
    externalEventsDetail: NotRequired[ExternalEventsDetailTypeDef],  # (2)
    ingestedEventsDetail: NotRequired[IngestedEventsDetailTypeDef],  # (3)
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
2. See [:material-code-braces: ExternalEventsDetailTypeDef](./type_defs.md#externaleventsdetailtypedef) 
3. See [:material-code-braces: IngestedEventsDetailTypeDef](./type_defs.md#ingestedeventsdetailtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateModelVersionRequestRequestTypeDef

```python
# CreateModelVersionRequestRequestTypeDef definition

class CreateModelVersionRequestRequestTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    trainingDataSource: TrainingDataSourceEnumType,  # (2)
    trainingDataSchema: TrainingDataSchemaTypeDef,  # (3)
    externalEventsDetail: NotRequired[ExternalEventsDetailTypeDef],  # (4)
    ingestedEventsDetail: NotRequired[IngestedEventsDetailTypeDef],  # (5)
    tags: NotRequired[Sequence[TagTypeDef]],  # (6)
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
2. See [:material-code-brackets: TrainingDataSourceEnumType](./literals.md#trainingdatasourceenumtype) 
3. See [:material-code-braces: TrainingDataSchemaTypeDef](./type_defs.md#trainingdataschematypedef) 
4. See [:material-code-braces: ExternalEventsDetailTypeDef](./type_defs.md#externaleventsdetailtypedef) 
5. See [:material-code-braces: IngestedEventsDetailTypeDef](./type_defs.md#ingestedeventsdetailtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetModelVersionResultTypeDef

```python
# GetModelVersionResultTypeDef definition

class GetModelVersionResultTypeDef(TypedDict):
    modelId: str,
    modelType: ModelTypeEnumType,  # (1)
    modelVersionNumber: str,
    trainingDataSource: TrainingDataSourceEnumType,  # (2)
    trainingDataSchema: TrainingDataSchemaTypeDef,  # (3)
    externalEventsDetail: ExternalEventsDetailTypeDef,  # (4)
    ingestedEventsDetail: IngestedEventsDetailTypeDef,  # (5)
    status: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
2. See [:material-code-brackets: TrainingDataSourceEnumType](./literals.md#trainingdatasourceenumtype) 
3. See [:material-code-braces: TrainingDataSchemaTypeDef](./type_defs.md#trainingdataschematypedef) 
4. See [:material-code-braces: ExternalEventsDetailTypeDef](./type_defs.md#externaleventsdetailtypedef) 
5. See [:material-code-braces: IngestedEventsDetailTypeDef](./type_defs.md#ingestedeventsdetailtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrainingResultTypeDef

```python
# TrainingResultTypeDef definition

class TrainingResultTypeDef(TypedDict):
    dataValidationMetrics: NotRequired[DataValidationMetricsTypeDef],  # (1)
    trainingMetrics: NotRequired[TrainingMetricsTypeDef],  # (2)
    variableImportanceMetrics: NotRequired[VariableImportanceMetricsTypeDef],  # (3)
```

1. See [:material-code-braces: DataValidationMetricsTypeDef](./type_defs.md#datavalidationmetricstypedef) 
2. See [:material-code-braces: TrainingMetricsTypeDef](./type_defs.md#trainingmetricstypedef) 
3. See [:material-code-braces: VariableImportanceMetricsTypeDef](./type_defs.md#variableimportancemetricstypedef) 
## OFITrainingMetricsValueTypeDef

```python
# OFITrainingMetricsValueTypeDef definition

class OFITrainingMetricsValueTypeDef(TypedDict):
    metricDataPoints: NotRequired[List[OFIMetricDataPointTypeDef]],  # (1)
    modelPerformance: NotRequired[OFIModelPerformanceTypeDef],  # (2)
```

1. See [:material-code-braces: OFIMetricDataPointTypeDef](./type_defs.md#ofimetricdatapointtypedef) 
2. See [:material-code-braces: OFIModelPerformanceTypeDef](./type_defs.md#ofimodelperformancetypedef) 
## TFITrainingMetricsValueTypeDef

```python
# TFITrainingMetricsValueTypeDef definition

class TFITrainingMetricsValueTypeDef(TypedDict):
    metricDataPoints: NotRequired[List[TFIMetricDataPointTypeDef]],  # (1)
    modelPerformance: NotRequired[TFIModelPerformanceTypeDef],  # (2)
```

1. See [:material-code-braces: TFIMetricDataPointTypeDef](./type_defs.md#tfimetricdatapointtypedef) 
2. See [:material-code-braces: TFIModelPerformanceTypeDef](./type_defs.md#tfimodelperformancetypedef) 
## ModelVersionEvaluationTypeDef

```python
# ModelVersionEvaluationTypeDef definition

class ModelVersionEvaluationTypeDef(TypedDict):
    outputVariableName: NotRequired[str],
    evaluationScore: NotRequired[str],
    predictionExplanations: NotRequired[PredictionExplanationsTypeDef],  # (1)
```

1. See [:material-code-braces: PredictionExplanationsTypeDef](./type_defs.md#predictionexplanationstypedef) 
## TrainingMetricsV2TypeDef

```python
# TrainingMetricsV2TypeDef definition

class TrainingMetricsV2TypeDef(TypedDict):
    ofi: NotRequired[OFITrainingMetricsValueTypeDef],  # (1)
    tfi: NotRequired[TFITrainingMetricsValueTypeDef],  # (2)
    ati: NotRequired[ATITrainingMetricsValueTypeDef],  # (3)
```

1. See [:material-code-braces: OFITrainingMetricsValueTypeDef](./type_defs.md#ofitrainingmetricsvaluetypedef) 
2. See [:material-code-braces: TFITrainingMetricsValueTypeDef](./type_defs.md#tfitrainingmetricsvaluetypedef) 
3. See [:material-code-braces: ATITrainingMetricsValueTypeDef](./type_defs.md#atitrainingmetricsvaluetypedef) 
## EvaluatedModelVersionTypeDef

```python
# EvaluatedModelVersionTypeDef definition

class EvaluatedModelVersionTypeDef(TypedDict):
    modelId: NotRequired[str],
    modelVersion: NotRequired[str],
    modelType: NotRequired[str],
    evaluations: NotRequired[List[ModelVersionEvaluationTypeDef]],  # (1)
```

1. See [:material-code-braces: ModelVersionEvaluationTypeDef](./type_defs.md#modelversionevaluationtypedef) 
## TrainingResultV2TypeDef

```python
# TrainingResultV2TypeDef definition

class TrainingResultV2TypeDef(TypedDict):
    dataValidationMetrics: NotRequired[DataValidationMetricsTypeDef],  # (1)
    trainingMetricsV2: NotRequired[TrainingMetricsV2TypeDef],  # (2)
    variableImportanceMetrics: NotRequired[VariableImportanceMetricsTypeDef],  # (3)
    aggregatedVariablesImportanceMetrics: NotRequired[AggregatedVariablesImportanceMetricsTypeDef],  # (4)
```

1. See [:material-code-braces: DataValidationMetricsTypeDef](./type_defs.md#datavalidationmetricstypedef) 
2. See [:material-code-braces: TrainingMetricsV2TypeDef](./type_defs.md#trainingmetricsv2typedef) 
3. See [:material-code-braces: VariableImportanceMetricsTypeDef](./type_defs.md#variableimportancemetricstypedef) 
4. See [:material-code-braces: AggregatedVariablesImportanceMetricsTypeDef](./type_defs.md#aggregatedvariablesimportancemetricstypedef) 
## GetEventPredictionMetadataResultTypeDef

```python
# GetEventPredictionMetadataResultTypeDef definition

class GetEventPredictionMetadataResultTypeDef(TypedDict):
    eventId: str,
    eventTypeName: str,
    entityId: str,
    entityType: str,
    eventTimestamp: str,
    detectorId: str,
    detectorVersionId: str,
    detectorVersionStatus: str,
    eventVariables: List[EventVariableSummaryTypeDef],  # (1)
    rules: List[EvaluatedRuleTypeDef],  # (2)
    ruleExecutionMode: RuleExecutionModeType,  # (3)
    outcomes: List[str],
    evaluatedModelVersions: List[EvaluatedModelVersionTypeDef],  # (4)
    evaluatedExternalModels: List[EvaluatedExternalModelTypeDef],  # (5)
    predictionTimestamp: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: EventVariableSummaryTypeDef](./type_defs.md#eventvariablesummarytypedef) 
2. See [:material-code-braces: EvaluatedRuleTypeDef](./type_defs.md#evaluatedruletypedef) 
3. See [:material-code-brackets: RuleExecutionModeType](./literals.md#ruleexecutionmodetype) 
4. See [:material-code-braces: EvaluatedModelVersionTypeDef](./type_defs.md#evaluatedmodelversiontypedef) 
5. See [:material-code-braces: EvaluatedExternalModelTypeDef](./type_defs.md#evaluatedexternalmodeltypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelVersionDetailTypeDef

```python
# ModelVersionDetailTypeDef definition

class ModelVersionDetailTypeDef(TypedDict):
    modelId: NotRequired[str],
    modelType: NotRequired[ModelTypeEnumType],  # (1)
    modelVersionNumber: NotRequired[str],
    status: NotRequired[str],
    trainingDataSource: NotRequired[TrainingDataSourceEnumType],  # (2)
    trainingDataSchema: NotRequired[TrainingDataSchemaTypeDef],  # (3)
    externalEventsDetail: NotRequired[ExternalEventsDetailTypeDef],  # (4)
    ingestedEventsDetail: NotRequired[IngestedEventsDetailTypeDef],  # (5)
    trainingResult: NotRequired[TrainingResultTypeDef],  # (6)
    lastUpdatedTime: NotRequired[str],
    createdTime: NotRequired[str],
    arn: NotRequired[str],
    trainingResultV2: NotRequired[TrainingResultV2TypeDef],  # (7)
```

1. See [:material-code-brackets: ModelTypeEnumType](./literals.md#modeltypeenumtype) 
2. See [:material-code-brackets: TrainingDataSourceEnumType](./literals.md#trainingdatasourceenumtype) 
3. See [:material-code-braces: TrainingDataSchemaTypeDef](./type_defs.md#trainingdataschematypedef) 
4. See [:material-code-braces: ExternalEventsDetailTypeDef](./type_defs.md#externaleventsdetailtypedef) 
5. See [:material-code-braces: IngestedEventsDetailTypeDef](./type_defs.md#ingestedeventsdetailtypedef) 
6. See [:material-code-braces: TrainingResultTypeDef](./type_defs.md#trainingresulttypedef) 
7. See [:material-code-braces: TrainingResultV2TypeDef](./type_defs.md#trainingresultv2typedef) 
## DescribeModelVersionsResultTypeDef

```python
# DescribeModelVersionsResultTypeDef definition

class DescribeModelVersionsResultTypeDef(TypedDict):
    modelVersionDetails: List[ModelVersionDetailTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelVersionDetailTypeDef](./type_defs.md#modelversiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
