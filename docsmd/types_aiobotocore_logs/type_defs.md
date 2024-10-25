# Type definitions

> [Index](../README.md) > [CloudWatchLogs](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
    type annotations stubs module [types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

## MetricTransformationUnionTypeDef

```python
# MetricTransformationUnionTypeDef definition

MetricTransformationUnionTypeDef = Union[
    MetricTransformationTypeDef,  # (1)
    MetricTransformationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricTransformationTypeDef](./type_defs.md#metrictransformationtypedef) 
2. See [:material-code-braces: MetricTransformationOutputTypeDef](./type_defs.md#metrictransformationoutputtypedef) 



## AccountPolicyTypeDef

```python
# AccountPolicyTypeDef definition

class AccountPolicyTypeDef(TypedDict):
    policyName: NotRequired[str],
    policyDocument: NotRequired[str],
    lastUpdatedTime: NotRequired[int],
    policyType: NotRequired[PolicyTypeType],  # (1)
    scope: NotRequired[ScopeType],  # (2)
    selectionCriteria: NotRequired[str],
    accountId: NotRequired[str],
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## AnomalyDetectorTypeDef

```python
# AnomalyDetectorTypeDef definition

class AnomalyDetectorTypeDef(TypedDict):
    anomalyDetectorArn: NotRequired[str],
    detectorName: NotRequired[str],
    logGroupArnList: NotRequired[List[str]],
    evaluationFrequency: NotRequired[EvaluationFrequencyType],  # (1)
    filterPattern: NotRequired[str],
    anomalyDetectorStatus: NotRequired[AnomalyDetectorStatusType],  # (2)
    kmsKeyId: NotRequired[str],
    creationTimeStamp: NotRequired[int],
    lastModifiedTimeStamp: NotRequired[int],
    anomalyVisibilityTime: NotRequired[int],
```

1. See [:material-code-brackets: EvaluationFrequencyType](./literals.md#evaluationfrequencytype) 
2. See [:material-code-brackets: AnomalyDetectorStatusType](./literals.md#anomalydetectorstatustype) 
## LogEventTypeDef

```python
# LogEventTypeDef definition

class LogEventTypeDef(TypedDict):
    timestamp: NotRequired[int],
    message: NotRequired[str],
```

## PatternTokenTypeDef

```python
# PatternTokenTypeDef definition

class PatternTokenTypeDef(TypedDict):
    dynamicTokenPosition: NotRequired[int],
    isDynamic: NotRequired[bool],
    tokenString: NotRequired[str],
    enumerations: NotRequired[Dict[str, int]],
```

## AssociateKmsKeyRequestRequestTypeDef

```python
# AssociateKmsKeyRequestRequestTypeDef definition

class AssociateKmsKeyRequestRequestTypeDef(TypedDict):
    kmsKeyId: str,
    logGroupName: NotRequired[str],
    resourceIdentifier: NotRequired[str],
```

## CancelExportTaskRequestRequestTypeDef

```python
# CancelExportTaskRequestRequestTypeDef definition

class CancelExportTaskRequestRequestTypeDef(TypedDict):
    taskId: str,
```

## S3DeliveryConfigurationTypeDef

```python
# S3DeliveryConfigurationTypeDef definition

class S3DeliveryConfigurationTypeDef(TypedDict):
    suffixPath: NotRequired[str],
    enableHiveCompatiblePath: NotRequired[bool],
```

## RecordFieldTypeDef

```python
# RecordFieldTypeDef definition

class RecordFieldTypeDef(TypedDict):
    name: NotRequired[str],
    mandatory: NotRequired[bool],
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

## CreateExportTaskRequestRequestTypeDef

```python
# CreateExportTaskRequestRequestTypeDef definition

class CreateExportTaskRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    fromTime: int,
    to: int,
    destination: str,
    taskName: NotRequired[str],
    logStreamNamePrefix: NotRequired[str],
    destinationPrefix: NotRequired[str],
```

## CreateLogAnomalyDetectorRequestRequestTypeDef

```python
# CreateLogAnomalyDetectorRequestRequestTypeDef definition

class CreateLogAnomalyDetectorRequestRequestTypeDef(TypedDict):
    logGroupArnList: Sequence[str],
    detectorName: NotRequired[str],
    evaluationFrequency: NotRequired[EvaluationFrequencyType],  # (1)
    filterPattern: NotRequired[str],
    kmsKeyId: NotRequired[str],
    anomalyVisibilityTime: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: EvaluationFrequencyType](./literals.md#evaluationfrequencytype) 
## CreateLogGroupRequestRequestTypeDef

```python
# CreateLogGroupRequestRequestTypeDef definition

class CreateLogGroupRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    kmsKeyId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    logGroupClass: NotRequired[LogGroupClassType],  # (1)
```

1. See [:material-code-brackets: LogGroupClassType](./literals.md#loggroupclasstype) 
## CreateLogStreamRequestRequestTypeDef

```python
# CreateLogStreamRequestRequestTypeDef definition

class CreateLogStreamRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    logStreamName: str,
```

## DeleteAccountPolicyRequestRequestTypeDef

```python
# DeleteAccountPolicyRequestRequestTypeDef definition

class DeleteAccountPolicyRequestRequestTypeDef(TypedDict):
    policyName: str,
    policyType: PolicyTypeType,  # (1)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
## DeleteDataProtectionPolicyRequestRequestTypeDef

```python
# DeleteDataProtectionPolicyRequestRequestTypeDef definition

class DeleteDataProtectionPolicyRequestRequestTypeDef(TypedDict):
    logGroupIdentifier: str,
```

## DeleteDeliveryDestinationPolicyRequestRequestTypeDef

```python
# DeleteDeliveryDestinationPolicyRequestRequestTypeDef definition

class DeleteDeliveryDestinationPolicyRequestRequestTypeDef(TypedDict):
    deliveryDestinationName: str,
```

## DeleteDeliveryDestinationRequestRequestTypeDef

```python
# DeleteDeliveryDestinationRequestRequestTypeDef definition

class DeleteDeliveryDestinationRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteDeliveryRequestRequestTypeDef

```python
# DeleteDeliveryRequestRequestTypeDef definition

class DeleteDeliveryRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteDeliverySourceRequestRequestTypeDef

```python
# DeleteDeliverySourceRequestRequestTypeDef definition

class DeleteDeliverySourceRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteDestinationRequestRequestTypeDef

```python
# DeleteDestinationRequestRequestTypeDef definition

class DeleteDestinationRequestRequestTypeDef(TypedDict):
    destinationName: str,
```

## DeleteLogAnomalyDetectorRequestRequestTypeDef

```python
# DeleteLogAnomalyDetectorRequestRequestTypeDef definition

class DeleteLogAnomalyDetectorRequestRequestTypeDef(TypedDict):
    anomalyDetectorArn: str,
```

## DeleteLogGroupRequestRequestTypeDef

```python
# DeleteLogGroupRequestRequestTypeDef definition

class DeleteLogGroupRequestRequestTypeDef(TypedDict):
    logGroupName: str,
```

## DeleteLogStreamRequestRequestTypeDef

```python
# DeleteLogStreamRequestRequestTypeDef definition

class DeleteLogStreamRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    logStreamName: str,
```

## DeleteMetricFilterRequestRequestTypeDef

```python
# DeleteMetricFilterRequestRequestTypeDef definition

class DeleteMetricFilterRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    filterName: str,
```

## DeleteQueryDefinitionRequestRequestTypeDef

```python
# DeleteQueryDefinitionRequestRequestTypeDef definition

class DeleteQueryDefinitionRequestRequestTypeDef(TypedDict):
    queryDefinitionId: str,
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    policyName: NotRequired[str],
```

## DeleteRetentionPolicyRequestRequestTypeDef

```python
# DeleteRetentionPolicyRequestRequestTypeDef definition

class DeleteRetentionPolicyRequestRequestTypeDef(TypedDict):
    logGroupName: str,
```

## DeleteSubscriptionFilterRequestRequestTypeDef

```python
# DeleteSubscriptionFilterRequestRequestTypeDef definition

class DeleteSubscriptionFilterRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    filterName: str,
```

## DeliveryDestinationConfigurationTypeDef

```python
# DeliveryDestinationConfigurationTypeDef definition

class DeliveryDestinationConfigurationTypeDef(TypedDict):
    destinationResourceArn: str,
```

## DeliverySourceTypeDef

```python
# DeliverySourceTypeDef definition

class DeliverySourceTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    resourceArns: NotRequired[List[str]],
    service: NotRequired[str],
    logType: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

## DescribeAccountPoliciesRequestRequestTypeDef

```python
# DescribeAccountPoliciesRequestRequestTypeDef definition

class DescribeAccountPoliciesRequestRequestTypeDef(TypedDict):
    policyType: PolicyTypeType,  # (1)
    policyName: NotRequired[str],
    accountIdentifiers: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeConfigurationTemplatesRequestRequestTypeDef

```python
# DescribeConfigurationTemplatesRequestRequestTypeDef definition

class DescribeConfigurationTemplatesRequestRequestTypeDef(TypedDict):
    service: NotRequired[str],
    logTypes: NotRequired[Sequence[str]],
    resourceTypes: NotRequired[Sequence[str]],
    deliveryDestinationTypes: NotRequired[Sequence[DeliveryDestinationTypeType]],  # (1)
    nextToken: NotRequired[str],
    limit: NotRequired[int],
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype) 
## DescribeDeliveriesRequestRequestTypeDef

```python
# DescribeDeliveriesRequestRequestTypeDef definition

class DescribeDeliveriesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    limit: NotRequired[int],
```

## DescribeDeliveryDestinationsRequestRequestTypeDef

```python
# DescribeDeliveryDestinationsRequestRequestTypeDef definition

class DescribeDeliveryDestinationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    limit: NotRequired[int],
```

## DescribeDeliverySourcesRequestRequestTypeDef

```python
# DescribeDeliverySourcesRequestRequestTypeDef definition

class DescribeDeliverySourcesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    limit: NotRequired[int],
```

## DescribeDestinationsRequestRequestTypeDef

```python
# DescribeDestinationsRequestRequestTypeDef definition

class DescribeDestinationsRequestRequestTypeDef(TypedDict):
    DestinationNamePrefix: NotRequired[str],
    nextToken: NotRequired[str],
    limit: NotRequired[int],
```

## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    destinationName: NotRequired[str],
    targetArn: NotRequired[str],
    roleArn: NotRequired[str],
    accessPolicy: NotRequired[str],
    arn: NotRequired[str],
    creationTime: NotRequired[int],
```

## DescribeExportTasksRequestRequestTypeDef

```python
# DescribeExportTasksRequestRequestTypeDef definition

class DescribeExportTasksRequestRequestTypeDef(TypedDict):
    taskId: NotRequired[str],
    statusCode: NotRequired[ExportTaskStatusCodeType],  # (1)
    nextToken: NotRequired[str],
    limit: NotRequired[int],
```

1. See [:material-code-brackets: ExportTaskStatusCodeType](./literals.md#exporttaskstatuscodetype) 
## DescribeLogGroupsRequestRequestTypeDef

```python
# DescribeLogGroupsRequestRequestTypeDef definition

class DescribeLogGroupsRequestRequestTypeDef(TypedDict):
    accountIdentifiers: NotRequired[Sequence[str]],
    logGroupNamePrefix: NotRequired[str],
    logGroupNamePattern: NotRequired[str],
    nextToken: NotRequired[str],
    limit: NotRequired[int],
    includeLinkedAccounts: NotRequired[bool],
    logGroupClass: NotRequired[LogGroupClassType],  # (1)
```

1. See [:material-code-brackets: LogGroupClassType](./literals.md#loggroupclasstype) 
## LogGroupTypeDef

```python
# LogGroupTypeDef definition

class LogGroupTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    creationTime: NotRequired[int],
    retentionInDays: NotRequired[int],
    metricFilterCount: NotRequired[int],
    arn: NotRequired[str],
    storedBytes: NotRequired[int],
    kmsKeyId: NotRequired[str],
    dataProtectionStatus: NotRequired[DataProtectionStatusType],  # (1)
    inheritedProperties: NotRequired[List[InheritedPropertyType]],  # (2)
    logGroupClass: NotRequired[LogGroupClassType],  # (3)
    logGroupArn: NotRequired[str],
```

1. See [:material-code-brackets: DataProtectionStatusType](./literals.md#dataprotectionstatustype) 
2. See [:material-code-brackets: InheritedPropertyType](./literals.md#inheritedpropertytype) 
3. See [:material-code-brackets: LogGroupClassType](./literals.md#loggroupclasstype) 
## DescribeLogStreamsRequestRequestTypeDef

```python
# DescribeLogStreamsRequestRequestTypeDef definition

class DescribeLogStreamsRequestRequestTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    logGroupIdentifier: NotRequired[str],
    logStreamNamePrefix: NotRequired[str],
    orderBy: NotRequired[OrderByType],  # (1)
    descending: NotRequired[bool],
    nextToken: NotRequired[str],
    limit: NotRequired[int],
```

1. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
## LogStreamTypeDef

```python
# LogStreamTypeDef definition

class LogStreamTypeDef(TypedDict):
    logStreamName: NotRequired[str],
    creationTime: NotRequired[int],
    firstEventTimestamp: NotRequired[int],
    lastEventTimestamp: NotRequired[int],
    lastIngestionTime: NotRequired[int],
    uploadSequenceToken: NotRequired[str],
    arn: NotRequired[str],
    storedBytes: NotRequired[int],
```

## DescribeMetricFiltersRequestRequestTypeDef

```python
# DescribeMetricFiltersRequestRequestTypeDef definition

class DescribeMetricFiltersRequestRequestTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    filterNamePrefix: NotRequired[str],
    nextToken: NotRequired[str],
    limit: NotRequired[int],
    metricName: NotRequired[str],
    metricNamespace: NotRequired[str],
```

## DescribeQueriesRequestRequestTypeDef

```python
# DescribeQueriesRequestRequestTypeDef definition

class DescribeQueriesRequestRequestTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    status: NotRequired[QueryStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
## QueryInfoTypeDef

```python
# QueryInfoTypeDef definition

class QueryInfoTypeDef(TypedDict):
    queryId: NotRequired[str],
    queryString: NotRequired[str],
    status: NotRequired[QueryStatusType],  # (1)
    createTime: NotRequired[int],
    logGroupName: NotRequired[str],
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
## DescribeQueryDefinitionsRequestRequestTypeDef

```python
# DescribeQueryDefinitionsRequestRequestTypeDef definition

class DescribeQueryDefinitionsRequestRequestTypeDef(TypedDict):
    queryDefinitionNamePrefix: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## QueryDefinitionTypeDef

```python
# QueryDefinitionTypeDef definition

class QueryDefinitionTypeDef(TypedDict):
    queryDefinitionId: NotRequired[str],
    name: NotRequired[str],
    queryString: NotRequired[str],
    lastModified: NotRequired[int],
    logGroupNames: NotRequired[List[str]],
```

## DescribeResourcePoliciesRequestRequestTypeDef

```python
# DescribeResourcePoliciesRequestRequestTypeDef definition

class DescribeResourcePoliciesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    limit: NotRequired[int],
```

## ResourcePolicyTypeDef

```python
# ResourcePolicyTypeDef definition

class ResourcePolicyTypeDef(TypedDict):
    policyName: NotRequired[str],
    policyDocument: NotRequired[str],
    lastUpdatedTime: NotRequired[int],
```

## DescribeSubscriptionFiltersRequestRequestTypeDef

```python
# DescribeSubscriptionFiltersRequestRequestTypeDef definition

class DescribeSubscriptionFiltersRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    filterNamePrefix: NotRequired[str],
    nextToken: NotRequired[str],
    limit: NotRequired[int],
```

## SubscriptionFilterTypeDef

```python
# SubscriptionFilterTypeDef definition

class SubscriptionFilterTypeDef(TypedDict):
    filterName: NotRequired[str],
    logGroupName: NotRequired[str],
    filterPattern: NotRequired[str],
    destinationArn: NotRequired[str],
    roleArn: NotRequired[str],
    distribution: NotRequired[DistributionType],  # (1)
    creationTime: NotRequired[int],
```

1. See [:material-code-brackets: DistributionType](./literals.md#distributiontype) 
## DisassociateKmsKeyRequestRequestTypeDef

```python
# DisassociateKmsKeyRequestRequestTypeDef definition

class DisassociateKmsKeyRequestRequestTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    resourceIdentifier: NotRequired[str],
```

## EntityTypeDef

```python
# EntityTypeDef definition

class EntityTypeDef(TypedDict):
    keyAttributes: NotRequired[Mapping[str, str]],
    attributes: NotRequired[Mapping[str, str]],
```

## ExportTaskExecutionInfoTypeDef

```python
# ExportTaskExecutionInfoTypeDef definition

class ExportTaskExecutionInfoTypeDef(TypedDict):
    creationTime: NotRequired[int],
    completionTime: NotRequired[int],
```

## ExportTaskStatusTypeDef

```python
# ExportTaskStatusTypeDef definition

class ExportTaskStatusTypeDef(TypedDict):
    code: NotRequired[ExportTaskStatusCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: ExportTaskStatusCodeType](./literals.md#exporttaskstatuscodetype) 
## FilterLogEventsRequestRequestTypeDef

```python
# FilterLogEventsRequestRequestTypeDef definition

class FilterLogEventsRequestRequestTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    logGroupIdentifier: NotRequired[str],
    logStreamNames: NotRequired[Sequence[str]],
    logStreamNamePrefix: NotRequired[str],
    startTime: NotRequired[int],
    endTime: NotRequired[int],
    filterPattern: NotRequired[str],
    nextToken: NotRequired[str],
    limit: NotRequired[int],
    interleaved: NotRequired[bool],
    unmask: NotRequired[bool],
```

## FilteredLogEventTypeDef

```python
# FilteredLogEventTypeDef definition

class FilteredLogEventTypeDef(TypedDict):
    logStreamName: NotRequired[str],
    timestamp: NotRequired[int],
    message: NotRequired[str],
    ingestionTime: NotRequired[int],
    eventId: NotRequired[str],
```

## SearchedLogStreamTypeDef

```python
# SearchedLogStreamTypeDef definition

class SearchedLogStreamTypeDef(TypedDict):
    logStreamName: NotRequired[str],
    searchedCompletely: NotRequired[bool],
```

## GetDataProtectionPolicyRequestRequestTypeDef

```python
# GetDataProtectionPolicyRequestRequestTypeDef definition

class GetDataProtectionPolicyRequestRequestTypeDef(TypedDict):
    logGroupIdentifier: str,
```

## GetDeliveryDestinationPolicyRequestRequestTypeDef

```python
# GetDeliveryDestinationPolicyRequestRequestTypeDef definition

class GetDeliveryDestinationPolicyRequestRequestTypeDef(TypedDict):
    deliveryDestinationName: str,
```

## PolicyTypeDef

```python
# PolicyTypeDef definition

class PolicyTypeDef(TypedDict):
    deliveryDestinationPolicy: NotRequired[str],
```

## GetDeliveryDestinationRequestRequestTypeDef

```python
# GetDeliveryDestinationRequestRequestTypeDef definition

class GetDeliveryDestinationRequestRequestTypeDef(TypedDict):
    name: str,
```

## GetDeliveryRequestRequestTypeDef

```python
# GetDeliveryRequestRequestTypeDef definition

class GetDeliveryRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetDeliverySourceRequestRequestTypeDef

```python
# GetDeliverySourceRequestRequestTypeDef definition

class GetDeliverySourceRequestRequestTypeDef(TypedDict):
    name: str,
```

## GetLogAnomalyDetectorRequestRequestTypeDef

```python
# GetLogAnomalyDetectorRequestRequestTypeDef definition

class GetLogAnomalyDetectorRequestRequestTypeDef(TypedDict):
    anomalyDetectorArn: str,
```

## GetLogEventsRequestRequestTypeDef

```python
# GetLogEventsRequestRequestTypeDef definition

class GetLogEventsRequestRequestTypeDef(TypedDict):
    logStreamName: str,
    logGroupName: NotRequired[str],
    logGroupIdentifier: NotRequired[str],
    startTime: NotRequired[int],
    endTime: NotRequired[int],
    nextToken: NotRequired[str],
    limit: NotRequired[int],
    startFromHead: NotRequired[bool],
    unmask: NotRequired[bool],
```

## OutputLogEventTypeDef

```python
# OutputLogEventTypeDef definition

class OutputLogEventTypeDef(TypedDict):
    timestamp: NotRequired[int],
    message: NotRequired[str],
    ingestionTime: NotRequired[int],
```

## GetLogGroupFieldsRequestRequestTypeDef

```python
# GetLogGroupFieldsRequestRequestTypeDef definition

class GetLogGroupFieldsRequestRequestTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    time: NotRequired[int],
    logGroupIdentifier: NotRequired[str],
```

## LogGroupFieldTypeDef

```python
# LogGroupFieldTypeDef definition

class LogGroupFieldTypeDef(TypedDict):
    name: NotRequired[str],
    percent: NotRequired[int],
```

## GetLogRecordRequestRequestTypeDef

```python
# GetLogRecordRequestRequestTypeDef definition

class GetLogRecordRequestRequestTypeDef(TypedDict):
    logRecordPointer: str,
    unmask: NotRequired[bool],
```

## GetQueryResultsRequestRequestTypeDef

```python
# GetQueryResultsRequestRequestTypeDef definition

class GetQueryResultsRequestRequestTypeDef(TypedDict):
    queryId: str,
```

## QueryStatisticsTypeDef

```python
# QueryStatisticsTypeDef definition

class QueryStatisticsTypeDef(TypedDict):
    recordsMatched: NotRequired[float],
    recordsScanned: NotRequired[float],
    bytesScanned: NotRequired[float],
```

## ResultFieldTypeDef

```python
# ResultFieldTypeDef definition

class ResultFieldTypeDef(TypedDict):
    field: NotRequired[str],
    value: NotRequired[str],
```

## InputLogEventTypeDef

```python
# InputLogEventTypeDef definition

class InputLogEventTypeDef(TypedDict):
    timestamp: int,
    message: str,
```

## ListAnomaliesRequestRequestTypeDef

```python
# ListAnomaliesRequestRequestTypeDef definition

class ListAnomaliesRequestRequestTypeDef(TypedDict):
    anomalyDetectorArn: NotRequired[str],
    suppressionState: NotRequired[SuppressionStateType],  # (1)
    limit: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: SuppressionStateType](./literals.md#suppressionstatetype) 
## ListLogAnomalyDetectorsRequestRequestTypeDef

```python
# ListLogAnomalyDetectorsRequestRequestTypeDef definition

class ListLogAnomalyDetectorsRequestRequestTypeDef(TypedDict):
    filterLogGroupArn: NotRequired[str],
    limit: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTagsLogGroupRequestRequestTypeDef

```python
# ListTagsLogGroupRequestRequestTypeDef definition

class ListTagsLogGroupRequestRequestTypeDef(TypedDict):
    logGroupName: str,
```

## LiveTailSessionLogEventTypeDef

```python
# LiveTailSessionLogEventTypeDef definition

class LiveTailSessionLogEventTypeDef(TypedDict):
    logStreamName: NotRequired[str],
    logGroupIdentifier: NotRequired[str],
    message: NotRequired[str],
    timestamp: NotRequired[int],
    ingestionTime: NotRequired[int],
```

## LiveTailSessionMetadataTypeDef

```python
# LiveTailSessionMetadataTypeDef definition

class LiveTailSessionMetadataTypeDef(TypedDict):
    sampled: NotRequired[bool],
```

## LiveTailSessionStartTypeDef

```python
# LiveTailSessionStartTypeDef definition

class LiveTailSessionStartTypeDef(TypedDict):
    requestId: NotRequired[str],
    sessionId: NotRequired[str],
    logGroupIdentifiers: NotRequired[List[str]],
    logStreamNames: NotRequired[List[str]],
    logStreamNamePrefixes: NotRequired[List[str]],
    logEventFilterPattern: NotRequired[str],
```

## MetricFilterMatchRecordTypeDef

```python
# MetricFilterMatchRecordTypeDef definition

class MetricFilterMatchRecordTypeDef(TypedDict):
    eventNumber: NotRequired[int],
    eventMessage: NotRequired[str],
    extractedValues: NotRequired[Dict[str, str]],
```

## MetricTransformationOutputTypeDef

```python
# MetricTransformationOutputTypeDef definition

class MetricTransformationOutputTypeDef(TypedDict):
    metricName: str,
    metricNamespace: str,
    metricValue: str,
    defaultValue: NotRequired[float],
    dimensions: NotRequired[Dict[str, str]],
    unit: NotRequired[StandardUnitType],  # (1)
```

1. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## MetricTransformationTypeDef

```python
# MetricTransformationTypeDef definition

class MetricTransformationTypeDef(TypedDict):
    metricName: str,
    metricNamespace: str,
    metricValue: str,
    defaultValue: NotRequired[float],
    dimensions: NotRequired[Mapping[str, str]],
    unit: NotRequired[StandardUnitType],  # (1)
```

1. See [:material-code-brackets: StandardUnitType](./literals.md#standardunittype) 
## PutAccountPolicyRequestRequestTypeDef

```python
# PutAccountPolicyRequestRequestTypeDef definition

class PutAccountPolicyRequestRequestTypeDef(TypedDict):
    policyName: str,
    policyDocument: str,
    policyType: PolicyTypeType,  # (1)
    scope: NotRequired[ScopeType],  # (2)
    selectionCriteria: NotRequired[str],
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-brackets: ScopeType](./literals.md#scopetype) 
## PutDataProtectionPolicyRequestRequestTypeDef

```python
# PutDataProtectionPolicyRequestRequestTypeDef definition

class PutDataProtectionPolicyRequestRequestTypeDef(TypedDict):
    logGroupIdentifier: str,
    policyDocument: str,
```

## PutDeliveryDestinationPolicyRequestRequestTypeDef

```python
# PutDeliveryDestinationPolicyRequestRequestTypeDef definition

class PutDeliveryDestinationPolicyRequestRequestTypeDef(TypedDict):
    deliveryDestinationName: str,
    deliveryDestinationPolicy: str,
```

## PutDeliverySourceRequestRequestTypeDef

```python
# PutDeliverySourceRequestRequestTypeDef definition

class PutDeliverySourceRequestRequestTypeDef(TypedDict):
    name: str,
    resourceArn: str,
    logType: str,
    tags: NotRequired[Mapping[str, str]],
```

## PutDestinationPolicyRequestRequestTypeDef

```python
# PutDestinationPolicyRequestRequestTypeDef definition

class PutDestinationPolicyRequestRequestTypeDef(TypedDict):
    destinationName: str,
    accessPolicy: str,
    forceUpdate: NotRequired[bool],
```

## PutDestinationRequestRequestTypeDef

```python
# PutDestinationRequestRequestTypeDef definition

class PutDestinationRequestRequestTypeDef(TypedDict):
    destinationName: str,
    targetArn: str,
    roleArn: str,
    tags: NotRequired[Mapping[str, str]],
```

## RejectedEntityInfoTypeDef

```python
# RejectedEntityInfoTypeDef definition

class RejectedEntityInfoTypeDef(TypedDict):
    errorType: EntityRejectionErrorTypeType,  # (1)
```

1. See [:material-code-brackets: EntityRejectionErrorTypeType](./literals.md#entityrejectionerrortypetype) 
## RejectedLogEventsInfoTypeDef

```python
# RejectedLogEventsInfoTypeDef definition

class RejectedLogEventsInfoTypeDef(TypedDict):
    tooNewLogEventStartIndex: NotRequired[int],
    tooOldLogEventEndIndex: NotRequired[int],
    expiredLogEventEndIndex: NotRequired[int],
```

## PutQueryDefinitionRequestRequestTypeDef

```python
# PutQueryDefinitionRequestRequestTypeDef definition

class PutQueryDefinitionRequestRequestTypeDef(TypedDict):
    name: str,
    queryString: str,
    queryDefinitionId: NotRequired[str],
    logGroupNames: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
```

## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    policyName: NotRequired[str],
    policyDocument: NotRequired[str],
```

## PutRetentionPolicyRequestRequestTypeDef

```python
# PutRetentionPolicyRequestRequestTypeDef definition

class PutRetentionPolicyRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    retentionInDays: int,
```

## PutSubscriptionFilterRequestRequestTypeDef

```python
# PutSubscriptionFilterRequestRequestTypeDef definition

class PutSubscriptionFilterRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    filterName: str,
    filterPattern: str,
    destinationArn: str,
    roleArn: NotRequired[str],
    distribution: NotRequired[DistributionType],  # (1)
```

1. See [:material-code-brackets: DistributionType](./literals.md#distributiontype) 
## SessionStreamingExceptionTypeDef

```python
# SessionStreamingExceptionTypeDef definition

class SessionStreamingExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## SessionTimeoutExceptionTypeDef

```python
# SessionTimeoutExceptionTypeDef definition

class SessionTimeoutExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## StartLiveTailRequestRequestTypeDef

```python
# StartLiveTailRequestRequestTypeDef definition

class StartLiveTailRequestRequestTypeDef(TypedDict):
    logGroupIdentifiers: Sequence[str],
    logStreamNames: NotRequired[Sequence[str]],
    logStreamNamePrefixes: NotRequired[Sequence[str]],
    logEventFilterPattern: NotRequired[str],
```

## StartQueryRequestRequestTypeDef

```python
# StartQueryRequestRequestTypeDef definition

class StartQueryRequestRequestTypeDef(TypedDict):
    startTime: int,
    endTime: int,
    queryString: str,
    logGroupName: NotRequired[str],
    logGroupNames: NotRequired[Sequence[str]],
    logGroupIdentifiers: NotRequired[Sequence[str]],
    limit: NotRequired[int],
```

## StopQueryRequestRequestTypeDef

```python
# StopQueryRequestRequestTypeDef definition

class StopQueryRequestRequestTypeDef(TypedDict):
    queryId: str,
```

## SuppressionPeriodTypeDef

```python
# SuppressionPeriodTypeDef definition

class SuppressionPeriodTypeDef(TypedDict):
    value: NotRequired[int],
    suppressionUnit: NotRequired[SuppressionUnitType],  # (1)
```

1. See [:material-code-brackets: SuppressionUnitType](./literals.md#suppressionunittype) 
## TagLogGroupRequestRequestTypeDef

```python
# TagLogGroupRequestRequestTypeDef definition

class TagLogGroupRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    tags: Mapping[str, str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TestMetricFilterRequestRequestTypeDef

```python
# TestMetricFilterRequestRequestTypeDef definition

class TestMetricFilterRequestRequestTypeDef(TypedDict):
    filterPattern: str,
    logEventMessages: Sequence[str],
```

## UntagLogGroupRequestRequestTypeDef

```python
# UntagLogGroupRequestRequestTypeDef definition

class UntagLogGroupRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    tags: Sequence[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateLogAnomalyDetectorRequestRequestTypeDef

```python
# UpdateLogAnomalyDetectorRequestRequestTypeDef definition

class UpdateLogAnomalyDetectorRequestRequestTypeDef(TypedDict):
    anomalyDetectorArn: str,
    enabled: bool,
    evaluationFrequency: NotRequired[EvaluationFrequencyType],  # (1)
    filterPattern: NotRequired[str],
    anomalyVisibilityTime: NotRequired[int],
```

1. See [:material-code-brackets: EvaluationFrequencyType](./literals.md#evaluationfrequencytype) 
## AnomalyTypeDef

```python
# AnomalyTypeDef definition

class AnomalyTypeDef(TypedDict):
    anomalyId: str,
    patternId: str,
    anomalyDetectorArn: str,
    patternString: str,
    firstSeen: int,
    lastSeen: int,
    description: str,
    active: bool,
    state: StateType,  # (1)
    histogram: Dict[str, int],
    logSamples: List[LogEventTypeDef],  # (2)
    patternTokens: List[PatternTokenTypeDef],  # (3)
    logGroupArnList: List[str],
    patternRegex: NotRequired[str],
    priority: NotRequired[str],
    suppressed: NotRequired[bool],
    suppressedDate: NotRequired[int],
    suppressedUntil: NotRequired[int],
    isPatternLevelSuppression: NotRequired[bool],
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
2. See [:material-code-braces: LogEventTypeDef](./type_defs.md#logeventtypedef) 
3. See [:material-code-braces: PatternTokenTypeDef](./type_defs.md#patterntokentypedef) 
## ConfigurationTemplateDeliveryConfigValuesTypeDef

```python
# ConfigurationTemplateDeliveryConfigValuesTypeDef definition

class ConfigurationTemplateDeliveryConfigValuesTypeDef(TypedDict):
    recordFields: NotRequired[List[str]],
    fieldDelimiter: NotRequired[str],
    s3DeliveryConfiguration: NotRequired[S3DeliveryConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: S3DeliveryConfigurationTypeDef](./type_defs.md#s3deliveryconfigurationtypedef) 
## CreateDeliveryRequestRequestTypeDef

```python
# CreateDeliveryRequestRequestTypeDef definition

class CreateDeliveryRequestRequestTypeDef(TypedDict):
    deliverySourceName: str,
    deliveryDestinationArn: str,
    recordFields: NotRequired[Sequence[str]],
    fieldDelimiter: NotRequired[str],
    s3DeliveryConfiguration: NotRequired[S3DeliveryConfigurationTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: S3DeliveryConfigurationTypeDef](./type_defs.md#s3deliveryconfigurationtypedef) 
## DeliveryTypeDef

```python
# DeliveryTypeDef definition

class DeliveryTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    deliverySourceName: NotRequired[str],
    deliveryDestinationArn: NotRequired[str],
    deliveryDestinationType: NotRequired[DeliveryDestinationTypeType],  # (1)
    recordFields: NotRequired[List[str]],
    fieldDelimiter: NotRequired[str],
    s3DeliveryConfiguration: NotRequired[S3DeliveryConfigurationTypeDef],  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype) 
2. See [:material-code-braces: S3DeliveryConfigurationTypeDef](./type_defs.md#s3deliveryconfigurationtypedef) 
## UpdateDeliveryConfigurationRequestRequestTypeDef

```python
# UpdateDeliveryConfigurationRequestRequestTypeDef definition

class UpdateDeliveryConfigurationRequestRequestTypeDef(TypedDict):
    id: str,
    recordFields: NotRequired[Sequence[str]],
    fieldDelimiter: NotRequired[str],
    s3DeliveryConfiguration: NotRequired[S3DeliveryConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: S3DeliveryConfigurationTypeDef](./type_defs.md#s3deliveryconfigurationtypedef) 
## CreateExportTaskResponseTypeDef

```python
# CreateExportTaskResponseTypeDef definition

class CreateExportTaskResponseTypeDef(TypedDict):
    taskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLogAnomalyDetectorResponseTypeDef

```python
# CreateLogAnomalyDetectorResponseTypeDef definition

class CreateLogAnomalyDetectorResponseTypeDef(TypedDict):
    anomalyDetectorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteQueryDefinitionResponseTypeDef

```python
# DeleteQueryDefinitionResponseTypeDef definition

class DeleteQueryDefinitionResponseTypeDef(TypedDict):
    success: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountPoliciesResponseTypeDef

```python
# DescribeAccountPoliciesResponseTypeDef definition

class DescribeAccountPoliciesResponseTypeDef(TypedDict):
    accountPolicies: List[AccountPolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountPolicyTypeDef](./type_defs.md#accountpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataProtectionPolicyResponseTypeDef

```python
# GetDataProtectionPolicyResponseTypeDef definition

class GetDataProtectionPolicyResponseTypeDef(TypedDict):
    logGroupIdentifier: str,
    policyDocument: str,
    lastUpdatedTime: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLogAnomalyDetectorResponseTypeDef

```python
# GetLogAnomalyDetectorResponseTypeDef definition

class GetLogAnomalyDetectorResponseTypeDef(TypedDict):
    detectorName: str,
    logGroupArnList: List[str],
    evaluationFrequency: EvaluationFrequencyType,  # (1)
    filterPattern: str,
    anomalyDetectorStatus: AnomalyDetectorStatusType,  # (2)
    kmsKeyId: str,
    creationTimeStamp: int,
    lastModifiedTimeStamp: int,
    anomalyVisibilityTime: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EvaluationFrequencyType](./literals.md#evaluationfrequencytype) 
2. See [:material-code-brackets: AnomalyDetectorStatusType](./literals.md#anomalydetectorstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLogRecordResponseTypeDef

```python
# GetLogRecordResponseTypeDef definition

class GetLogRecordResponseTypeDef(TypedDict):
    logRecord: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLogAnomalyDetectorsResponseTypeDef

```python
# ListLogAnomalyDetectorsResponseTypeDef definition

class ListLogAnomalyDetectorsResponseTypeDef(TypedDict):
    anomalyDetectors: List[AnomalyDetectorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnomalyDetectorTypeDef](./type_defs.md#anomalydetectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsLogGroupResponseTypeDef

```python
# ListTagsLogGroupResponseTypeDef definition

class ListTagsLogGroupResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAccountPolicyResponseTypeDef

```python
# PutAccountPolicyResponseTypeDef definition

class PutAccountPolicyResponseTypeDef(TypedDict):
    accountPolicy: AccountPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountPolicyTypeDef](./type_defs.md#accountpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDataProtectionPolicyResponseTypeDef

```python
# PutDataProtectionPolicyResponseTypeDef definition

class PutDataProtectionPolicyResponseTypeDef(TypedDict):
    logGroupIdentifier: str,
    policyDocument: str,
    lastUpdatedTime: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutQueryDefinitionResponseTypeDef

```python
# PutQueryDefinitionResponseTypeDef definition

class PutQueryDefinitionResponseTypeDef(TypedDict):
    queryDefinitionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartQueryResponseTypeDef

```python
# StartQueryResponseTypeDef definition

class StartQueryResponseTypeDef(TypedDict):
    queryId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopQueryResponseTypeDef

```python
# StopQueryResponseTypeDef definition

class StopQueryResponseTypeDef(TypedDict):
    success: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeliveryDestinationTypeDef

```python
# DeliveryDestinationTypeDef definition

class DeliveryDestinationTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    deliveryDestinationType: NotRequired[DeliveryDestinationTypeType],  # (1)
    outputFormat: NotRequired[OutputFormatType],  # (2)
    deliveryDestinationConfiguration: NotRequired[DeliveryDestinationConfigurationTypeDef],  # (3)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype) 
2. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
3. See [:material-code-braces: DeliveryDestinationConfigurationTypeDef](./type_defs.md#deliverydestinationconfigurationtypedef) 
## PutDeliveryDestinationRequestRequestTypeDef

```python
# PutDeliveryDestinationRequestRequestTypeDef definition

class PutDeliveryDestinationRequestRequestTypeDef(TypedDict):
    name: str,
    deliveryDestinationConfiguration: DeliveryDestinationConfigurationTypeDef,  # (1)
    outputFormat: NotRequired[OutputFormatType],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DeliveryDestinationConfigurationTypeDef](./type_defs.md#deliverydestinationconfigurationtypedef) 
2. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
## DescribeDeliverySourcesResponseTypeDef

```python
# DescribeDeliverySourcesResponseTypeDef definition

class DescribeDeliverySourcesResponseTypeDef(TypedDict):
    deliverySources: List[DeliverySourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeliverySourceTypeDef](./type_defs.md#deliverysourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeliverySourceResponseTypeDef

```python
# GetDeliverySourceResponseTypeDef definition

class GetDeliverySourceResponseTypeDef(TypedDict):
    deliverySource: DeliverySourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeliverySourceTypeDef](./type_defs.md#deliverysourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDeliverySourceResponseTypeDef

```python
# PutDeliverySourceResponseTypeDef definition

class PutDeliverySourceResponseTypeDef(TypedDict):
    deliverySource: DeliverySourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeliverySourceTypeDef](./type_defs.md#deliverysourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationTemplatesRequestDescribeConfigurationTemplatesPaginateTypeDef

```python
# DescribeConfigurationTemplatesRequestDescribeConfigurationTemplatesPaginateTypeDef definition

class DescribeConfigurationTemplatesRequestDescribeConfigurationTemplatesPaginateTypeDef(TypedDict):
    service: NotRequired[str],
    logTypes: NotRequired[Sequence[str]],
    resourceTypes: NotRequired[Sequence[str]],
    deliveryDestinationTypes: NotRequired[Sequence[DeliveryDestinationTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDeliveriesRequestDescribeDeliveriesPaginateTypeDef

```python
# DescribeDeliveriesRequestDescribeDeliveriesPaginateTypeDef definition

class DescribeDeliveriesRequestDescribeDeliveriesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDeliveryDestinationsRequestDescribeDeliveryDestinationsPaginateTypeDef

```python
# DescribeDeliveryDestinationsRequestDescribeDeliveryDestinationsPaginateTypeDef definition

class DescribeDeliveryDestinationsRequestDescribeDeliveryDestinationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDeliverySourcesRequestDescribeDeliverySourcesPaginateTypeDef

```python
# DescribeDeliverySourcesRequestDescribeDeliverySourcesPaginateTypeDef definition

class DescribeDeliverySourcesRequestDescribeDeliverySourcesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef

```python
# DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef definition

class DescribeDestinationsRequestDescribeDestinationsPaginateTypeDef(TypedDict):
    DestinationNamePrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef

```python
# DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef definition

class DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef(TypedDict):
    taskId: NotRequired[str],
    statusCode: NotRequired[ExportTaskStatusCodeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ExportTaskStatusCodeType](./literals.md#exporttaskstatuscodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef

```python
# DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef definition

class DescribeLogGroupsRequestDescribeLogGroupsPaginateTypeDef(TypedDict):
    accountIdentifiers: NotRequired[Sequence[str]],
    logGroupNamePrefix: NotRequired[str],
    logGroupNamePattern: NotRequired[str],
    includeLinkedAccounts: NotRequired[bool],
    logGroupClass: NotRequired[LogGroupClassType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LogGroupClassType](./literals.md#loggroupclasstype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef

```python
# DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef definition

class DescribeLogStreamsRequestDescribeLogStreamsPaginateTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    logGroupIdentifier: NotRequired[str],
    logStreamNamePrefix: NotRequired[str],
    orderBy: NotRequired[OrderByType],  # (1)
    descending: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef

```python
# DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef definition

class DescribeMetricFiltersRequestDescribeMetricFiltersPaginateTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    filterNamePrefix: NotRequired[str],
    metricName: NotRequired[str],
    metricNamespace: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeQueriesRequestDescribeQueriesPaginateTypeDef

```python
# DescribeQueriesRequestDescribeQueriesPaginateTypeDef definition

class DescribeQueriesRequestDescribeQueriesPaginateTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    status: NotRequired[QueryStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef

```python
# DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef definition

class DescribeResourcePoliciesRequestDescribeResourcePoliciesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef

```python
# DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef definition

class DescribeSubscriptionFiltersRequestDescribeSubscriptionFiltersPaginateTypeDef(TypedDict):
    logGroupName: str,
    filterNamePrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## FilterLogEventsRequestFilterLogEventsPaginateTypeDef

```python
# FilterLogEventsRequestFilterLogEventsPaginateTypeDef definition

class FilterLogEventsRequestFilterLogEventsPaginateTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    logGroupIdentifier: NotRequired[str],
    logStreamNames: NotRequired[Sequence[str]],
    logStreamNamePrefix: NotRequired[str],
    startTime: NotRequired[int],
    endTime: NotRequired[int],
    filterPattern: NotRequired[str],
    interleaved: NotRequired[bool],
    unmask: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAnomaliesRequestListAnomaliesPaginateTypeDef

```python
# ListAnomaliesRequestListAnomaliesPaginateTypeDef definition

class ListAnomaliesRequestListAnomaliesPaginateTypeDef(TypedDict):
    anomalyDetectorArn: NotRequired[str],
    suppressionState: NotRequired[SuppressionStateType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SuppressionStateType](./literals.md#suppressionstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLogAnomalyDetectorsRequestListLogAnomalyDetectorsPaginateTypeDef

```python
# ListLogAnomalyDetectorsRequestListLogAnomalyDetectorsPaginateTypeDef definition

class ListLogAnomalyDetectorsRequestListLogAnomalyDetectorsPaginateTypeDef(TypedDict):
    filterLogGroupArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDestinationsResponseTypeDef

```python
# DescribeDestinationsResponseTypeDef definition

class DescribeDestinationsResponseTypeDef(TypedDict):
    destinations: List[DestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDestinationResponseTypeDef

```python
# PutDestinationResponseTypeDef definition

class PutDestinationResponseTypeDef(TypedDict):
    destination: DestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLogGroupsResponseTypeDef

```python
# DescribeLogGroupsResponseTypeDef definition

class DescribeLogGroupsResponseTypeDef(TypedDict):
    logGroups: List[LogGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LogGroupTypeDef](./type_defs.md#loggrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLogStreamsResponseTypeDef

```python
# DescribeLogStreamsResponseTypeDef definition

class DescribeLogStreamsResponseTypeDef(TypedDict):
    logStreams: List[LogStreamTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LogStreamTypeDef](./type_defs.md#logstreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeQueriesResponseTypeDef

```python
# DescribeQueriesResponseTypeDef definition

class DescribeQueriesResponseTypeDef(TypedDict):
    queries: List[QueryInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QueryInfoTypeDef](./type_defs.md#queryinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeQueryDefinitionsResponseTypeDef

```python
# DescribeQueryDefinitionsResponseTypeDef definition

class DescribeQueryDefinitionsResponseTypeDef(TypedDict):
    queryDefinitions: List[QueryDefinitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: QueryDefinitionTypeDef](./type_defs.md#querydefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourcePoliciesResponseTypeDef

```python
# DescribeResourcePoliciesResponseTypeDef definition

class DescribeResourcePoliciesResponseTypeDef(TypedDict):
    resourcePolicies: List[ResourcePolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResponseTypeDef

```python
# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    resourcePolicy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSubscriptionFiltersResponseTypeDef

```python
# DescribeSubscriptionFiltersResponseTypeDef definition

class DescribeSubscriptionFiltersResponseTypeDef(TypedDict):
    subscriptionFilters: List[SubscriptionFilterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionFilterTypeDef](./type_defs.md#subscriptionfiltertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportTaskTypeDef

```python
# ExportTaskTypeDef definition

class ExportTaskTypeDef(TypedDict):
    taskId: NotRequired[str],
    taskName: NotRequired[str],
    logGroupName: NotRequired[str],
    from: NotRequired[int],
    to: NotRequired[int],
    destination: NotRequired[str],
    destinationPrefix: NotRequired[str],
    status: NotRequired[ExportTaskStatusTypeDef],  # (1)
    executionInfo: NotRequired[ExportTaskExecutionInfoTypeDef],  # (2)
```

1. See [:material-code-braces: ExportTaskStatusTypeDef](./type_defs.md#exporttaskstatustypedef) 
2. See [:material-code-braces: ExportTaskExecutionInfoTypeDef](./type_defs.md#exporttaskexecutioninfotypedef) 
## FilterLogEventsResponseTypeDef

```python
# FilterLogEventsResponseTypeDef definition

class FilterLogEventsResponseTypeDef(TypedDict):
    events: List[FilteredLogEventTypeDef],  # (1)
    searchedLogStreams: List[SearchedLogStreamTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilteredLogEventTypeDef](./type_defs.md#filteredlogeventtypedef) 
2. See [:material-code-braces: SearchedLogStreamTypeDef](./type_defs.md#searchedlogstreamtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeliveryDestinationPolicyResponseTypeDef

```python
# GetDeliveryDestinationPolicyResponseTypeDef definition

class GetDeliveryDestinationPolicyResponseTypeDef(TypedDict):
    policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDeliveryDestinationPolicyResponseTypeDef

```python
# PutDeliveryDestinationPolicyResponseTypeDef definition

class PutDeliveryDestinationPolicyResponseTypeDef(TypedDict):
    policy: PolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLogEventsResponseTypeDef

```python
# GetLogEventsResponseTypeDef definition

class GetLogEventsResponseTypeDef(TypedDict):
    events: List[OutputLogEventTypeDef],  # (1)
    nextForwardToken: str,
    nextBackwardToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutputLogEventTypeDef](./type_defs.md#outputlogeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLogGroupFieldsResponseTypeDef

```python
# GetLogGroupFieldsResponseTypeDef definition

class GetLogGroupFieldsResponseTypeDef(TypedDict):
    logGroupFields: List[LogGroupFieldTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LogGroupFieldTypeDef](./type_defs.md#loggroupfieldtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueryResultsResponseTypeDef

```python
# GetQueryResultsResponseTypeDef definition

class GetQueryResultsResponseTypeDef(TypedDict):
    results: List[List[ResultFieldTypeDef]],  # (1)
    statistics: QueryStatisticsTypeDef,  # (2)
    status: QueryStatusType,  # (3)
    encryptionKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ResultFieldTypeDef](./type_defs.md#resultfieldtypedef) 
2. See [:material-code-braces: QueryStatisticsTypeDef](./type_defs.md#querystatisticstypedef) 
3. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLogEventsRequestRequestTypeDef

```python
# PutLogEventsRequestRequestTypeDef definition

class PutLogEventsRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    logStreamName: str,
    logEvents: Sequence[InputLogEventTypeDef],  # (1)
    sequenceToken: NotRequired[str],
    entity: NotRequired[EntityTypeDef],  # (2)
```

1. See [:material-code-braces: InputLogEventTypeDef](./type_defs.md#inputlogeventtypedef) 
2. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
## LiveTailSessionUpdateTypeDef

```python
# LiveTailSessionUpdateTypeDef definition

class LiveTailSessionUpdateTypeDef(TypedDict):
    sessionMetadata: NotRequired[LiveTailSessionMetadataTypeDef],  # (1)
    sessionResults: NotRequired[List[LiveTailSessionLogEventTypeDef]],  # (2)
```

1. See [:material-code-braces: LiveTailSessionMetadataTypeDef](./type_defs.md#livetailsessionmetadatatypedef) 
2. See [:material-code-braces: LiveTailSessionLogEventTypeDef](./type_defs.md#livetailsessionlogeventtypedef) 
## TestMetricFilterResponseTypeDef

```python
# TestMetricFilterResponseTypeDef definition

class TestMetricFilterResponseTypeDef(TypedDict):
    matches: List[MetricFilterMatchRecordTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricFilterMatchRecordTypeDef](./type_defs.md#metricfiltermatchrecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricFilterTypeDef

```python
# MetricFilterTypeDef definition

class MetricFilterTypeDef(TypedDict):
    filterName: NotRequired[str],
    filterPattern: NotRequired[str],
    metricTransformations: NotRequired[List[MetricTransformationOutputTypeDef]],  # (1)
    creationTime: NotRequired[int],
    logGroupName: NotRequired[str],
```

1. See [:material-code-braces: MetricTransformationOutputTypeDef](./type_defs.md#metrictransformationoutputtypedef) 
## PutLogEventsResponseTypeDef

```python
# PutLogEventsResponseTypeDef definition

class PutLogEventsResponseTypeDef(TypedDict):
    nextSequenceToken: str,
    rejectedLogEventsInfo: RejectedLogEventsInfoTypeDef,  # (1)
    rejectedEntityInfo: RejectedEntityInfoTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RejectedLogEventsInfoTypeDef](./type_defs.md#rejectedlogeventsinfotypedef) 
2. See [:material-code-braces: RejectedEntityInfoTypeDef](./type_defs.md#rejectedentityinfotypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnomalyRequestRequestTypeDef

```python
# UpdateAnomalyRequestRequestTypeDef definition

class UpdateAnomalyRequestRequestTypeDef(TypedDict):
    anomalyDetectorArn: str,
    anomalyId: NotRequired[str],
    patternId: NotRequired[str],
    suppressionType: NotRequired[SuppressionTypeType],  # (1)
    suppressionPeriod: NotRequired[SuppressionPeriodTypeDef],  # (2)
```

1. See [:material-code-brackets: SuppressionTypeType](./literals.md#suppressiontypetype) 
2. See [:material-code-braces: SuppressionPeriodTypeDef](./type_defs.md#suppressionperiodtypedef) 
## ListAnomaliesResponseTypeDef

```python
# ListAnomaliesResponseTypeDef definition

class ListAnomaliesResponseTypeDef(TypedDict):
    anomalies: List[AnomalyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnomalyTypeDef](./type_defs.md#anomalytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigurationTemplateTypeDef

```python
# ConfigurationTemplateTypeDef definition

class ConfigurationTemplateTypeDef(TypedDict):
    service: NotRequired[str],
    logType: NotRequired[str],
    resourceType: NotRequired[str],
    deliveryDestinationType: NotRequired[DeliveryDestinationTypeType],  # (1)
    defaultDeliveryConfigValues: NotRequired[ConfigurationTemplateDeliveryConfigValuesTypeDef],  # (2)
    allowedFields: NotRequired[List[RecordFieldTypeDef]],  # (3)
    allowedOutputFormats: NotRequired[List[OutputFormatType]],  # (4)
    allowedActionForAllowVendedLogsDeliveryForResource: NotRequired[str],
    allowedFieldDelimiters: NotRequired[List[str]],
    allowedSuffixPathFields: NotRequired[List[str]],
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype) 
2. See [:material-code-braces: ConfigurationTemplateDeliveryConfigValuesTypeDef](./type_defs.md#configurationtemplatedeliveryconfigvaluestypedef) 
3. See [:material-code-braces: RecordFieldTypeDef](./type_defs.md#recordfieldtypedef) 
4. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
## CreateDeliveryResponseTypeDef

```python
# CreateDeliveryResponseTypeDef definition

class CreateDeliveryResponseTypeDef(TypedDict):
    delivery: DeliveryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeliveryTypeDef](./type_defs.md#deliverytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDeliveriesResponseTypeDef

```python
# DescribeDeliveriesResponseTypeDef definition

class DescribeDeliveriesResponseTypeDef(TypedDict):
    deliveries: List[DeliveryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeliveryTypeDef](./type_defs.md#deliverytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeliveryResponseTypeDef

```python
# GetDeliveryResponseTypeDef definition

class GetDeliveryResponseTypeDef(TypedDict):
    delivery: DeliveryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeliveryTypeDef](./type_defs.md#deliverytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDeliveryDestinationsResponseTypeDef

```python
# DescribeDeliveryDestinationsResponseTypeDef definition

class DescribeDeliveryDestinationsResponseTypeDef(TypedDict):
    deliveryDestinations: List[DeliveryDestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeliveryDestinationTypeDef](./type_defs.md#deliverydestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeliveryDestinationResponseTypeDef

```python
# GetDeliveryDestinationResponseTypeDef definition

class GetDeliveryDestinationResponseTypeDef(TypedDict):
    deliveryDestination: DeliveryDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeliveryDestinationTypeDef](./type_defs.md#deliverydestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDeliveryDestinationResponseTypeDef

```python
# PutDeliveryDestinationResponseTypeDef definition

class PutDeliveryDestinationResponseTypeDef(TypedDict):
    deliveryDestination: DeliveryDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeliveryDestinationTypeDef](./type_defs.md#deliverydestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeExportTasksResponseTypeDef

```python
# DescribeExportTasksResponseTypeDef definition

class DescribeExportTasksResponseTypeDef(TypedDict):
    exportTasks: List[ExportTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportTaskTypeDef](./type_defs.md#exporttasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartLiveTailResponseStreamTypeDef

```python
# StartLiveTailResponseStreamTypeDef definition

class StartLiveTailResponseStreamTypeDef(TypedDict):
    sessionStart: NotRequired[LiveTailSessionStartTypeDef],  # (1)
    sessionUpdate: NotRequired[LiveTailSessionUpdateTypeDef],  # (2)
    SessionTimeoutException: NotRequired[SessionTimeoutExceptionTypeDef],  # (3)
    SessionStreamingException: NotRequired[SessionStreamingExceptionTypeDef],  # (4)
```

1. See [:material-code-braces: LiveTailSessionStartTypeDef](./type_defs.md#livetailsessionstarttypedef) 
2. See [:material-code-braces: LiveTailSessionUpdateTypeDef](./type_defs.md#livetailsessionupdatetypedef) 
3. See [:material-code-braces: SessionTimeoutExceptionTypeDef](./type_defs.md#sessiontimeoutexceptiontypedef) 
4. See [:material-code-braces: SessionStreamingExceptionTypeDef](./type_defs.md#sessionstreamingexceptiontypedef) 
## DescribeMetricFiltersResponseTypeDef

```python
# DescribeMetricFiltersResponseTypeDef definition

class DescribeMetricFiltersResponseTypeDef(TypedDict):
    metricFilters: List[MetricFilterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MetricFilterTypeDef](./type_defs.md#metricfiltertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutMetricFilterRequestRequestTypeDef

```python
# PutMetricFilterRequestRequestTypeDef definition

class PutMetricFilterRequestRequestTypeDef(TypedDict):
    logGroupName: str,
    filterName: str,
    filterPattern: str,
    metricTransformations: Sequence[MetricTransformationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: MetricTransformationTypeDef](./type_defs.md#metrictransformationtypedef) [:material-code-braces: MetricTransformationOutputTypeDef](./type_defs.md#metrictransformationoutputtypedef) 
## DescribeConfigurationTemplatesResponseTypeDef

```python
# DescribeConfigurationTemplatesResponseTypeDef definition

class DescribeConfigurationTemplatesResponseTypeDef(TypedDict):
    configurationTemplates: List[ConfigurationTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationTemplateTypeDef](./type_defs.md#configurationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartLiveTailResponseTypeDef

```python
# StartLiveTailResponseTypeDef definition

class StartLiveTailResponseTypeDef(TypedDict):
    responseStream: AioEventStream[StartLiveTailResponseStreamTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StartLiveTailResponseStreamTypeDef](./type_defs.md#startlivetailresponsestreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
