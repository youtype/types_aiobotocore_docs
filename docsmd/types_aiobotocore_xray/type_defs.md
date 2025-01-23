# Type definitions

> [Index](../README.md) > [XRay](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [XRay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#xray)
    type annotations stubs module [types-aiobotocore-xray](https://pypi.org/project/types-aiobotocore-xray/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AliasTypeDef

```python
# AliasTypeDef definition

class AliasTypeDef(TypedDict):
    Name: NotRequired[str],
    Names: NotRequired[List[str]],
    Type: NotRequired[str],
```

## AnnotationValueTypeDef

```python
# AnnotationValueTypeDef definition

class AnnotationValueTypeDef(TypedDict):
    NumberValue: NotRequired[float],
    BooleanValue: NotRequired[bool],
    StringValue: NotRequired[str],
```

## ServiceIdTypeDef

```python
# ServiceIdTypeDef definition

class ServiceIdTypeDef(TypedDict):
    Name: NotRequired[str],
    Names: NotRequired[List[str]],
    AccountId: NotRequired[str],
    Type: NotRequired[str],
```

## AvailabilityZoneDetailTypeDef

```python
# AvailabilityZoneDetailTypeDef definition

class AvailabilityZoneDetailTypeDef(TypedDict):
    Name: NotRequired[str],
```

## BackendConnectionErrorsTypeDef

```python
# BackendConnectionErrorsTypeDef definition

class BackendConnectionErrorsTypeDef(TypedDict):
    TimeoutCount: NotRequired[int],
    ConnectionRefusedCount: NotRequired[int],
    HTTPCode4XXCount: NotRequired[int],
    HTTPCode5XXCount: NotRequired[int],
    UnknownHostCount: NotRequired[int],
    OtherCount: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## BatchGetTracesRequestRequestTypeDef

```python
# BatchGetTracesRequestRequestTypeDef definition

class BatchGetTracesRequestRequestTypeDef(TypedDict):
    TraceIds: Sequence[str],
    NextToken: NotRequired[str],
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

## CancelTraceRetrievalRequestRequestTypeDef

```python
# CancelTraceRetrievalRequestRequestTypeDef definition

class CancelTraceRetrievalRequestRequestTypeDef(TypedDict):
    RetrievalToken: str,
```

## InsightsConfigurationTypeDef

```python
# InsightsConfigurationTypeDef definition

class InsightsConfigurationTypeDef(TypedDict):
    InsightsEnabled: NotRequired[bool],
    NotificationsEnabled: NotRequired[bool],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## SamplingRuleTypeDef

```python
# SamplingRuleTypeDef definition

class SamplingRuleTypeDef(TypedDict):
    ResourceARN: str,
    Priority: int,
    FixedRate: float,
    ReservoirSize: int,
    ServiceName: str,
    ServiceType: str,
    Host: str,
    HTTPMethod: str,
    URLPath: str,
    Version: int,
    RuleName: NotRequired[str],
    RuleARN: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
```

## DeleteGroupRequestRequestTypeDef

```python
# DeleteGroupRequestRequestTypeDef definition

class DeleteGroupRequestRequestTypeDef(TypedDict):
    GroupName: NotRequired[str],
    GroupARN: NotRequired[str],
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    PolicyName: str,
    PolicyRevisionId: NotRequired[str],
```

## DeleteSamplingRuleRequestRequestTypeDef

```python
# DeleteSamplingRuleRequestRequestTypeDef definition

class DeleteSamplingRuleRequestRequestTypeDef(TypedDict):
    RuleName: NotRequired[str],
    RuleARN: NotRequired[str],
```

## ErrorStatisticsTypeDef

```python
# ErrorStatisticsTypeDef definition

class ErrorStatisticsTypeDef(TypedDict):
    ThrottleCount: NotRequired[int],
    OtherCount: NotRequired[int],
    TotalCount: NotRequired[int],
```

## FaultStatisticsTypeDef

```python
# FaultStatisticsTypeDef definition

class FaultStatisticsTypeDef(TypedDict):
    OtherCount: NotRequired[int],
    TotalCount: NotRequired[int],
```

## HistogramEntryTypeDef

```python
# HistogramEntryTypeDef definition

class HistogramEntryTypeDef(TypedDict):
    Value: NotRequired[float],
    Count: NotRequired[int],
```

## EncryptionConfigTypeDef

```python
# EncryptionConfigTypeDef definition

class EncryptionConfigTypeDef(TypedDict):
    KeyId: NotRequired[str],
    Status: NotRequired[EncryptionStatusType],  # (1)
    Type: NotRequired[EncryptionTypeType],  # (2)
```

1. See [:material-code-brackets: EncryptionStatusType](./literals.md#encryptionstatustype) 
2. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## RootCauseExceptionTypeDef

```python
# RootCauseExceptionTypeDef definition

class RootCauseExceptionTypeDef(TypedDict):
    Name: NotRequired[str],
    Message: NotRequired[str],
```

## ForecastStatisticsTypeDef

```python
# ForecastStatisticsTypeDef definition

class ForecastStatisticsTypeDef(TypedDict):
    FaultCountHigh: NotRequired[int],
    FaultCountLow: NotRequired[int],
```

## GetGroupRequestRequestTypeDef

```python
# GetGroupRequestRequestTypeDef definition

class GetGroupRequestRequestTypeDef(TypedDict):
    GroupName: NotRequired[str],
    GroupARN: NotRequired[str],
```

## GetGroupsRequestRequestTypeDef

```python
# GetGroupsRequestRequestTypeDef definition

class GetGroupsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## GetIndexingRulesRequestRequestTypeDef

```python
# GetIndexingRulesRequestRequestTypeDef definition

class GetIndexingRulesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## GetInsightEventsRequestRequestTypeDef

```python
# GetInsightEventsRequestRequestTypeDef definition

class GetInsightEventsRequestRequestTypeDef(TypedDict):
    InsightId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetInsightRequestRequestTypeDef

```python
# GetInsightRequestRequestTypeDef definition

class GetInsightRequestRequestTypeDef(TypedDict):
    InsightId: str,
```

## GetRetrievedTracesGraphRequestRequestTypeDef

```python
# GetRetrievedTracesGraphRequestRequestTypeDef definition

class GetRetrievedTracesGraphRequestRequestTypeDef(TypedDict):
    RetrievalToken: str,
    NextToken: NotRequired[str],
```

## GetSamplingRulesRequestRequestTypeDef

```python
# GetSamplingRulesRequestRequestTypeDef definition

class GetSamplingRulesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## GetSamplingStatisticSummariesRequestRequestTypeDef

```python
# GetSamplingStatisticSummariesRequestRequestTypeDef definition

class GetSamplingStatisticSummariesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## SamplingStatisticSummaryTypeDef

```python
# SamplingStatisticSummaryTypeDef definition

class SamplingStatisticSummaryTypeDef(TypedDict):
    RuleName: NotRequired[str],
    Timestamp: NotRequired[datetime],
    RequestCount: NotRequired[int],
    BorrowCount: NotRequired[int],
    SampledCount: NotRequired[int],
```

## SamplingTargetDocumentTypeDef

```python
# SamplingTargetDocumentTypeDef definition

class SamplingTargetDocumentTypeDef(TypedDict):
    RuleName: NotRequired[str],
    FixedRate: NotRequired[float],
    ReservoirQuota: NotRequired[int],
    ReservoirQuotaTTL: NotRequired[datetime],
    Interval: NotRequired[int],
```

## UnprocessedStatisticsTypeDef

```python
# UnprocessedStatisticsTypeDef definition

class UnprocessedStatisticsTypeDef(TypedDict):
    RuleName: NotRequired[str],
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## GetTraceGraphRequestRequestTypeDef

```python
# GetTraceGraphRequestRequestTypeDef definition

class GetTraceGraphRequestRequestTypeDef(TypedDict):
    TraceIds: Sequence[str],
    NextToken: NotRequired[str],
```

## SamplingStrategyTypeDef

```python
# SamplingStrategyTypeDef definition

class SamplingStrategyTypeDef(TypedDict):
    Name: NotRequired[SamplingStrategyNameType],  # (1)
    Value: NotRequired[float],
```

1. See [:material-code-brackets: SamplingStrategyNameType](./literals.md#samplingstrategynametype) 
## GraphLinkTypeDef

```python
# GraphLinkTypeDef definition

class GraphLinkTypeDef(TypedDict):
    ReferenceType: NotRequired[str],
    SourceTraceId: NotRequired[str],
    DestinationTraceIds: NotRequired[List[str]],
```

## HttpTypeDef

```python
# HttpTypeDef definition

class HttpTypeDef(TypedDict):
    HttpURL: NotRequired[str],
    HttpStatus: NotRequired[int],
    HttpMethod: NotRequired[str],
    UserAgent: NotRequired[str],
    ClientIp: NotRequired[str],
```

## ProbabilisticRuleValueTypeDef

```python
# ProbabilisticRuleValueTypeDef definition

class ProbabilisticRuleValueTypeDef(TypedDict):
    DesiredSamplingPercentage: float,
    ActualSamplingPercentage: NotRequired[float],
```

## ProbabilisticRuleValueUpdateTypeDef

```python
# ProbabilisticRuleValueUpdateTypeDef definition

class ProbabilisticRuleValueUpdateTypeDef(TypedDict):
    DesiredSamplingPercentage: float,
```

## RequestImpactStatisticsTypeDef

```python
# RequestImpactStatisticsTypeDef definition

class RequestImpactStatisticsTypeDef(TypedDict):
    FaultCount: NotRequired[int],
    OkCount: NotRequired[int],
    TotalCount: NotRequired[int],
```

## InsightImpactGraphEdgeTypeDef

```python
# InsightImpactGraphEdgeTypeDef definition

class InsightImpactGraphEdgeTypeDef(TypedDict):
    ReferenceId: NotRequired[int],
```

## InstanceIdDetailTypeDef

```python
# InstanceIdDetailTypeDef definition

class InstanceIdDetailTypeDef(TypedDict):
    Id: NotRequired[str],
```

## ListResourcePoliciesRequestRequestTypeDef

```python
# ListResourcePoliciesRequestRequestTypeDef definition

class ListResourcePoliciesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## ResourcePolicyTypeDef

```python
# ResourcePolicyTypeDef definition

class ResourcePolicyTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    PolicyDocument: NotRequired[str],
    PolicyRevisionId: NotRequired[str],
    LastUpdatedTime: NotRequired[datetime],
```

## ListRetrievedTracesRequestRequestTypeDef

```python
# ListRetrievedTracesRequestRequestTypeDef definition

class ListRetrievedTracesRequestRequestTypeDef(TypedDict):
    RetrievalToken: str,
    TraceFormat: NotRequired[TraceFormatTypeType],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: TraceFormatTypeType](./literals.md#traceformattypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    NextToken: NotRequired[str],
```

## PutEncryptionConfigRequestRequestTypeDef

```python
# PutEncryptionConfigRequestRequestTypeDef definition

class PutEncryptionConfigRequestRequestTypeDef(TypedDict):
    Type: EncryptionTypeType,  # (1)
    KeyId: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    PolicyName: str,
    PolicyDocument: str,
    PolicyRevisionId: NotRequired[str],
    BypassPolicyLockoutCheck: NotRequired[bool],
```

## PutTraceSegmentsRequestRequestTypeDef

```python
# PutTraceSegmentsRequestRequestTypeDef definition

class PutTraceSegmentsRequestRequestTypeDef(TypedDict):
    TraceSegmentDocuments: Sequence[str],
```

## UnprocessedTraceSegmentTypeDef

```python
# UnprocessedTraceSegmentTypeDef definition

class UnprocessedTraceSegmentTypeDef(TypedDict):
    Id: NotRequired[str],
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## ResourceARNDetailTypeDef

```python
# ResourceARNDetailTypeDef definition

class ResourceARNDetailTypeDef(TypedDict):
    ARN: NotRequired[str],
```

## ResponseTimeRootCauseEntityTypeDef

```python
# ResponseTimeRootCauseEntityTypeDef definition

class ResponseTimeRootCauseEntityTypeDef(TypedDict):
    Name: NotRequired[str],
    Coverage: NotRequired[float],
    Remote: NotRequired[bool],
```

## SpanTypeDef

```python
# SpanTypeDef definition

class SpanTypeDef(TypedDict):
    Id: NotRequired[str],
    Document: NotRequired[str],
```

## SamplingRuleOutputTypeDef

```python
# SamplingRuleOutputTypeDef definition

class SamplingRuleOutputTypeDef(TypedDict):
    ResourceARN: str,
    Priority: int,
    FixedRate: float,
    ReservoirSize: int,
    ServiceName: str,
    ServiceType: str,
    Host: str,
    HTTPMethod: str,
    URLPath: str,
    Version: int,
    RuleName: NotRequired[str],
    RuleARN: NotRequired[str],
    Attributes: NotRequired[Dict[str, str]],
```

## SamplingRuleUpdateTypeDef

```python
# SamplingRuleUpdateTypeDef definition

class SamplingRuleUpdateTypeDef(TypedDict):
    RuleName: NotRequired[str],
    RuleARN: NotRequired[str],
    ResourceARN: NotRequired[str],
    Priority: NotRequired[int],
    FixedRate: NotRequired[float],
    ReservoirSize: NotRequired[int],
    Host: NotRequired[str],
    ServiceName: NotRequired[str],
    ServiceType: NotRequired[str],
    HTTPMethod: NotRequired[str],
    URLPath: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
```

## SegmentTypeDef

```python
# SegmentTypeDef definition

class SegmentTypeDef(TypedDict):
    Id: NotRequired[str],
    Document: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateTraceSegmentDestinationRequestRequestTypeDef

```python
# UpdateTraceSegmentDestinationRequestRequestTypeDef definition

class UpdateTraceSegmentDestinationRequestRequestTypeDef(TypedDict):
    Destination: NotRequired[TraceSegmentDestinationType],  # (1)
```

1. See [:material-code-brackets: TraceSegmentDestinationType](./literals.md#tracesegmentdestinationtype) 
## AnomalousServiceTypeDef

```python
# AnomalousServiceTypeDef definition

class AnomalousServiceTypeDef(TypedDict):
    ServiceId: NotRequired[ServiceIdTypeDef],  # (1)
```

1. See [:material-code-braces: ServiceIdTypeDef](./type_defs.md#serviceidtypedef) 
## TraceUserTypeDef

```python
# TraceUserTypeDef definition

class TraceUserTypeDef(TypedDict):
    UserName: NotRequired[str],
    ServiceIds: NotRequired[List[ServiceIdTypeDef]],  # (1)
```

1. See [:material-code-braces: ServiceIdTypeDef](./type_defs.md#serviceidtypedef) 
## ValueWithServiceIdsTypeDef

```python
# ValueWithServiceIdsTypeDef definition

class ValueWithServiceIdsTypeDef(TypedDict):
    AnnotationValue: NotRequired[AnnotationValueTypeDef],  # (1)
    ServiceIds: NotRequired[List[ServiceIdTypeDef]],  # (2)
```

1. See [:material-code-braces: AnnotationValueTypeDef](./type_defs.md#annotationvaluetypedef) 
2. See [:material-code-braces: ServiceIdTypeDef](./type_defs.md#serviceidtypedef) 
## BatchGetTracesRequestPaginateTypeDef

```python
# BatchGetTracesRequestPaginateTypeDef definition

class BatchGetTracesRequestPaginateTypeDef(TypedDict):
    TraceIds: Sequence[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetGroupsRequestPaginateTypeDef

```python
# GetGroupsRequestPaginateTypeDef definition

class GetGroupsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetSamplingRulesRequestPaginateTypeDef

```python
# GetSamplingRulesRequestPaginateTypeDef definition

class GetSamplingRulesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetSamplingStatisticSummariesRequestPaginateTypeDef

```python
# GetSamplingStatisticSummariesRequestPaginateTypeDef definition

class GetSamplingStatisticSummariesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTraceGraphRequestPaginateTypeDef

```python
# GetTraceGraphRequestPaginateTypeDef definition

class GetTraceGraphRequestPaginateTypeDef(TypedDict):
    TraceIds: Sequence[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourcePoliciesRequestPaginateTypeDef

```python
# ListResourcePoliciesRequestPaginateTypeDef definition

class ListResourcePoliciesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestPaginateTypeDef

```python
# ListTagsForResourceRequestPaginateTypeDef definition

class ListTagsForResourceRequestPaginateTypeDef(TypedDict):
    ResourceARN: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTraceSegmentDestinationResultTypeDef

```python
# GetTraceSegmentDestinationResultTypeDef definition

class GetTraceSegmentDestinationResultTypeDef(TypedDict):
    Destination: TraceSegmentDestinationType,  # (1)
    Status: TraceSegmentDestinationStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TraceSegmentDestinationType](./literals.md#tracesegmentdestinationtype) 
2. See [:material-code-brackets: TraceSegmentDestinationStatusType](./literals.md#tracesegmentdestinationstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTraceRetrievalResultTypeDef

```python
# StartTraceRetrievalResultTypeDef definition

class StartTraceRetrievalResultTypeDef(TypedDict):
    RetrievalToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTraceSegmentDestinationResultTypeDef

```python
# UpdateTraceSegmentDestinationResultTypeDef definition

class UpdateTraceSegmentDestinationResultTypeDef(TypedDict):
    Destination: TraceSegmentDestinationType,  # (1)
    Status: TraceSegmentDestinationStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TraceSegmentDestinationType](./literals.md#tracesegmentdestinationtype) 
2. See [:material-code-brackets: TraceSegmentDestinationStatusType](./literals.md#tracesegmentdestinationstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GroupSummaryTypeDef

```python
# GroupSummaryTypeDef definition

class GroupSummaryTypeDef(TypedDict):
    GroupName: NotRequired[str],
    GroupARN: NotRequired[str],
    FilterExpression: NotRequired[str],
    InsightsConfiguration: NotRequired[InsightsConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: InsightsConfigurationTypeDef](./type_defs.md#insightsconfigurationtypedef) 
## GroupTypeDef

```python
# GroupTypeDef definition

class GroupTypeDef(TypedDict):
    GroupName: NotRequired[str],
    GroupARN: NotRequired[str],
    FilterExpression: NotRequired[str],
    InsightsConfiguration: NotRequired[InsightsConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: InsightsConfigurationTypeDef](./type_defs.md#insightsconfigurationtypedef) 
## UpdateGroupRequestRequestTypeDef

```python
# UpdateGroupRequestRequestTypeDef definition

class UpdateGroupRequestRequestTypeDef(TypedDict):
    GroupName: NotRequired[str],
    GroupARN: NotRequired[str],
    FilterExpression: NotRequired[str],
    InsightsConfiguration: NotRequired[InsightsConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: InsightsConfigurationTypeDef](./type_defs.md#insightsconfigurationtypedef) 
## CreateGroupRequestRequestTypeDef

```python
# CreateGroupRequestRequestTypeDef definition

class CreateGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    FilterExpression: NotRequired[str],
    InsightsConfiguration: NotRequired[InsightsConfigurationTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: InsightsConfigurationTypeDef](./type_defs.md#insightsconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
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
## CreateSamplingRuleRequestRequestTypeDef

```python
# CreateSamplingRuleRequestRequestTypeDef definition

class CreateSamplingRuleRequestRequestTypeDef(TypedDict):
    SamplingRule: SamplingRuleTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: SamplingRuleTypeDef](./type_defs.md#samplingruletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## EdgeStatisticsTypeDef

```python
# EdgeStatisticsTypeDef definition

class EdgeStatisticsTypeDef(TypedDict):
    OkCount: NotRequired[int],
    ErrorStatistics: NotRequired[ErrorStatisticsTypeDef],  # (1)
    FaultStatistics: NotRequired[FaultStatisticsTypeDef],  # (2)
    TotalCount: NotRequired[int],
    TotalResponseTime: NotRequired[float],
```

1. See [:material-code-braces: ErrorStatisticsTypeDef](./type_defs.md#errorstatisticstypedef) 
2. See [:material-code-braces: FaultStatisticsTypeDef](./type_defs.md#faultstatisticstypedef) 
## ServiceStatisticsTypeDef

```python
# ServiceStatisticsTypeDef definition

class ServiceStatisticsTypeDef(TypedDict):
    OkCount: NotRequired[int],
    ErrorStatistics: NotRequired[ErrorStatisticsTypeDef],  # (1)
    FaultStatistics: NotRequired[FaultStatisticsTypeDef],  # (2)
    TotalCount: NotRequired[int],
    TotalResponseTime: NotRequired[float],
```

1. See [:material-code-braces: ErrorStatisticsTypeDef](./type_defs.md#errorstatisticstypedef) 
2. See [:material-code-braces: FaultStatisticsTypeDef](./type_defs.md#faultstatisticstypedef) 
## GetEncryptionConfigResultTypeDef

```python
# GetEncryptionConfigResultTypeDef definition

class GetEncryptionConfigResultTypeDef(TypedDict):
    EncryptionConfig: EncryptionConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEncryptionConfigResultTypeDef

```python
# PutEncryptionConfigResultTypeDef definition

class PutEncryptionConfigResultTypeDef(TypedDict):
    EncryptionConfig: EncryptionConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ErrorRootCauseEntityTypeDef

```python
# ErrorRootCauseEntityTypeDef definition

class ErrorRootCauseEntityTypeDef(TypedDict):
    Name: NotRequired[str],
    Exceptions: NotRequired[List[RootCauseExceptionTypeDef]],  # (1)
    Remote: NotRequired[bool],
```

1. See [:material-code-braces: RootCauseExceptionTypeDef](./type_defs.md#rootcauseexceptiontypedef) 
## FaultRootCauseEntityTypeDef

```python
# FaultRootCauseEntityTypeDef definition

class FaultRootCauseEntityTypeDef(TypedDict):
    Name: NotRequired[str],
    Exceptions: NotRequired[List[RootCauseExceptionTypeDef]],  # (1)
    Remote: NotRequired[bool],
```

1. See [:material-code-braces: RootCauseExceptionTypeDef](./type_defs.md#rootcauseexceptiontypedef) 
## GetInsightImpactGraphRequestRequestTypeDef

```python
# GetInsightImpactGraphRequestRequestTypeDef definition

class GetInsightImpactGraphRequestRequestTypeDef(TypedDict):
    InsightId: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    NextToken: NotRequired[str],
```

## GetInsightSummariesRequestRequestTypeDef

```python
# GetInsightSummariesRequestRequestTypeDef definition

class GetInsightSummariesRequestRequestTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    States: NotRequired[Sequence[InsightStateType]],  # (1)
    GroupARN: NotRequired[str],
    GroupName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: InsightStateType](./literals.md#insightstatetype) 
## GetServiceGraphRequestPaginateTypeDef

```python
# GetServiceGraphRequestPaginateTypeDef definition

class GetServiceGraphRequestPaginateTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    GroupName: NotRequired[str],
    GroupARN: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetServiceGraphRequestRequestTypeDef

```python
# GetServiceGraphRequestRequestTypeDef definition

class GetServiceGraphRequestRequestTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    GroupName: NotRequired[str],
    GroupARN: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetTimeSeriesServiceStatisticsRequestPaginateTypeDef

```python
# GetTimeSeriesServiceStatisticsRequestPaginateTypeDef definition

class GetTimeSeriesServiceStatisticsRequestPaginateTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    GroupName: NotRequired[str],
    GroupARN: NotRequired[str],
    EntitySelectorExpression: NotRequired[str],
    Period: NotRequired[int],
    ForecastStatistics: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTimeSeriesServiceStatisticsRequestRequestTypeDef

```python
# GetTimeSeriesServiceStatisticsRequestRequestTypeDef definition

class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    GroupName: NotRequired[str],
    GroupARN: NotRequired[str],
    EntitySelectorExpression: NotRequired[str],
    Period: NotRequired[int],
    ForecastStatistics: NotRequired[bool],
    NextToken: NotRequired[str],
```

## SamplingStatisticsDocumentTypeDef

```python
# SamplingStatisticsDocumentTypeDef definition

class SamplingStatisticsDocumentTypeDef(TypedDict):
    RuleName: str,
    ClientID: str,
    Timestamp: TimestampTypeDef,
    RequestCount: int,
    SampledCount: int,
    BorrowCount: NotRequired[int],
```

## StartTraceRetrievalRequestRequestTypeDef

```python
# StartTraceRetrievalRequestRequestTypeDef definition

class StartTraceRetrievalRequestRequestTypeDef(TypedDict):
    TraceIds: Sequence[str],
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
```

## TelemetryRecordTypeDef

```python
# TelemetryRecordTypeDef definition

class TelemetryRecordTypeDef(TypedDict):
    Timestamp: TimestampTypeDef,
    SegmentsReceivedCount: NotRequired[int],
    SegmentsSentCount: NotRequired[int],
    SegmentsSpilloverCount: NotRequired[int],
    SegmentsRejectedCount: NotRequired[int],
    BackendConnectionErrors: NotRequired[BackendConnectionErrorsTypeDef],  # (1)
```

1. See [:material-code-braces: BackendConnectionErrorsTypeDef](./type_defs.md#backendconnectionerrorstypedef) 
## GetSamplingStatisticSummariesResultTypeDef

```python
# GetSamplingStatisticSummariesResultTypeDef definition

class GetSamplingStatisticSummariesResultTypeDef(TypedDict):
    SamplingStatisticSummaries: List[SamplingStatisticSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SamplingStatisticSummaryTypeDef](./type_defs.md#samplingstatisticsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSamplingTargetsResultTypeDef

```python
# GetSamplingTargetsResultTypeDef definition

class GetSamplingTargetsResultTypeDef(TypedDict):
    SamplingTargetDocuments: List[SamplingTargetDocumentTypeDef],  # (1)
    LastRuleModification: datetime,
    UnprocessedStatistics: List[UnprocessedStatisticsTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SamplingTargetDocumentTypeDef](./type_defs.md#samplingtargetdocumenttypedef) 
2. See [:material-code-braces: UnprocessedStatisticsTypeDef](./type_defs.md#unprocessedstatisticstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTraceSummariesRequestPaginateTypeDef

```python
# GetTraceSummariesRequestPaginateTypeDef definition

class GetTraceSummariesRequestPaginateTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    TimeRangeType: NotRequired[TimeRangeTypeType],  # (1)
    Sampling: NotRequired[bool],
    SamplingStrategy: NotRequired[SamplingStrategyTypeDef],  # (2)
    FilterExpression: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: TimeRangeTypeType](./literals.md#timerangetypetype) 
2. See [:material-code-braces: SamplingStrategyTypeDef](./type_defs.md#samplingstrategytypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTraceSummariesRequestRequestTypeDef

```python
# GetTraceSummariesRequestRequestTypeDef definition

class GetTraceSummariesRequestRequestTypeDef(TypedDict):
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    TimeRangeType: NotRequired[TimeRangeTypeType],  # (1)
    Sampling: NotRequired[bool],
    SamplingStrategy: NotRequired[SamplingStrategyTypeDef],  # (2)
    FilterExpression: NotRequired[str],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: TimeRangeTypeType](./literals.md#timerangetypetype) 
2. See [:material-code-braces: SamplingStrategyTypeDef](./type_defs.md#samplingstrategytypedef) 
## IndexingRuleValueTypeDef

```python
# IndexingRuleValueTypeDef definition

class IndexingRuleValueTypeDef(TypedDict):
    Probabilistic: NotRequired[ProbabilisticRuleValueTypeDef],  # (1)
```

1. See [:material-code-braces: ProbabilisticRuleValueTypeDef](./type_defs.md#probabilisticrulevaluetypedef) 
## IndexingRuleValueUpdateTypeDef

```python
# IndexingRuleValueUpdateTypeDef definition

class IndexingRuleValueUpdateTypeDef(TypedDict):
    Probabilistic: NotRequired[ProbabilisticRuleValueUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: ProbabilisticRuleValueUpdateTypeDef](./type_defs.md#probabilisticrulevalueupdatetypedef) 
## InsightImpactGraphServiceTypeDef

```python
# InsightImpactGraphServiceTypeDef definition

class InsightImpactGraphServiceTypeDef(TypedDict):
    ReferenceId: NotRequired[int],
    Type: NotRequired[str],
    Name: NotRequired[str],
    Names: NotRequired[List[str]],
    AccountId: NotRequired[str],
    Edges: NotRequired[List[InsightImpactGraphEdgeTypeDef]],  # (1)
```

1. See [:material-code-braces: InsightImpactGraphEdgeTypeDef](./type_defs.md#insightimpactgraphedgetypedef) 
## ListResourcePoliciesResultTypeDef

```python
# ListResourcePoliciesResultTypeDef definition

class ListResourcePoliciesResultTypeDef(TypedDict):
    ResourcePolicies: List[ResourcePolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResultTypeDef

```python
# PutResourcePolicyResultTypeDef definition

class PutResourcePolicyResultTypeDef(TypedDict):
    ResourcePolicy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutTraceSegmentsResultTypeDef

```python
# PutTraceSegmentsResultTypeDef definition

class PutTraceSegmentsResultTypeDef(TypedDict):
    UnprocessedTraceSegments: List[UnprocessedTraceSegmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UnprocessedTraceSegmentTypeDef](./type_defs.md#unprocessedtracesegmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResponseTimeRootCauseServiceTypeDef

```python
# ResponseTimeRootCauseServiceTypeDef definition

class ResponseTimeRootCauseServiceTypeDef(TypedDict):
    Name: NotRequired[str],
    Names: NotRequired[List[str]],
    Type: NotRequired[str],
    AccountId: NotRequired[str],
    EntityPath: NotRequired[List[ResponseTimeRootCauseEntityTypeDef]],  # (1)
    Inferred: NotRequired[bool],
```

1. See [:material-code-braces: ResponseTimeRootCauseEntityTypeDef](./type_defs.md#responsetimerootcauseentitytypedef) 
## RetrievedTraceTypeDef

```python
# RetrievedTraceTypeDef definition

class RetrievedTraceTypeDef(TypedDict):
    Id: NotRequired[str],
    Duration: NotRequired[float],
    Spans: NotRequired[List[SpanTypeDef]],  # (1)
```

1. See [:material-code-braces: SpanTypeDef](./type_defs.md#spantypedef) 
## SamplingRuleRecordTypeDef

```python
# SamplingRuleRecordTypeDef definition

class SamplingRuleRecordTypeDef(TypedDict):
    SamplingRule: NotRequired[SamplingRuleOutputTypeDef],  # (1)
    CreatedAt: NotRequired[datetime],
    ModifiedAt: NotRequired[datetime],
```

1. See [:material-code-braces: SamplingRuleOutputTypeDef](./type_defs.md#samplingruleoutputtypedef) 
## UpdateSamplingRuleRequestRequestTypeDef

```python
# UpdateSamplingRuleRequestRequestTypeDef definition

class UpdateSamplingRuleRequestRequestTypeDef(TypedDict):
    SamplingRuleUpdate: SamplingRuleUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: SamplingRuleUpdateTypeDef](./type_defs.md#samplingruleupdatetypedef) 
## TraceTypeDef

```python
# TraceTypeDef definition

class TraceTypeDef(TypedDict):
    Id: NotRequired[str],
    Duration: NotRequired[float],
    LimitExceeded: NotRequired[bool],
    Segments: NotRequired[List[SegmentTypeDef]],  # (1)
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
## InsightEventTypeDef

```python
# InsightEventTypeDef definition

class InsightEventTypeDef(TypedDict):
    Summary: NotRequired[str],
    EventTime: NotRequired[datetime],
    ClientRequestImpactStatistics: NotRequired[RequestImpactStatisticsTypeDef],  # (1)
    RootCauseServiceRequestImpactStatistics: NotRequired[RequestImpactStatisticsTypeDef],  # (1)
    TopAnomalousServices: NotRequired[List[AnomalousServiceTypeDef]],  # (3)
```

1. See [:material-code-braces: RequestImpactStatisticsTypeDef](./type_defs.md#requestimpactstatisticstypedef) 
2. See [:material-code-braces: RequestImpactStatisticsTypeDef](./type_defs.md#requestimpactstatisticstypedef) 
3. See [:material-code-braces: AnomalousServiceTypeDef](./type_defs.md#anomalousservicetypedef) 
## InsightSummaryTypeDef

```python
# InsightSummaryTypeDef definition

class InsightSummaryTypeDef(TypedDict):
    InsightId: NotRequired[str],
    GroupARN: NotRequired[str],
    GroupName: NotRequired[str],
    RootCauseServiceId: NotRequired[ServiceIdTypeDef],  # (1)
    Categories: NotRequired[List[InsightCategoryType]],  # (2)
    State: NotRequired[InsightStateType],  # (3)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Summary: NotRequired[str],
    ClientRequestImpactStatistics: NotRequired[RequestImpactStatisticsTypeDef],  # (4)
    RootCauseServiceRequestImpactStatistics: NotRequired[RequestImpactStatisticsTypeDef],  # (4)
    TopAnomalousServices: NotRequired[List[AnomalousServiceTypeDef]],  # (6)
    LastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-braces: ServiceIdTypeDef](./type_defs.md#serviceidtypedef) 
2. See [:material-code-brackets: InsightCategoryType](./literals.md#insightcategorytype) 
3. See [:material-code-brackets: InsightStateType](./literals.md#insightstatetype) 
4. See [:material-code-braces: RequestImpactStatisticsTypeDef](./type_defs.md#requestimpactstatisticstypedef) 
5. See [:material-code-braces: RequestImpactStatisticsTypeDef](./type_defs.md#requestimpactstatisticstypedef) 
6. See [:material-code-braces: AnomalousServiceTypeDef](./type_defs.md#anomalousservicetypedef) 
## InsightTypeDef

```python
# InsightTypeDef definition

class InsightTypeDef(TypedDict):
    InsightId: NotRequired[str],
    GroupARN: NotRequired[str],
    GroupName: NotRequired[str],
    RootCauseServiceId: NotRequired[ServiceIdTypeDef],  # (1)
    Categories: NotRequired[List[InsightCategoryType]],  # (2)
    State: NotRequired[InsightStateType],  # (3)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Summary: NotRequired[str],
    ClientRequestImpactStatistics: NotRequired[RequestImpactStatisticsTypeDef],  # (4)
    RootCauseServiceRequestImpactStatistics: NotRequired[RequestImpactStatisticsTypeDef],  # (4)
    TopAnomalousServices: NotRequired[List[AnomalousServiceTypeDef]],  # (6)
```

1. See [:material-code-braces: ServiceIdTypeDef](./type_defs.md#serviceidtypedef) 
2. See [:material-code-brackets: InsightCategoryType](./literals.md#insightcategorytype) 
3. See [:material-code-brackets: InsightStateType](./literals.md#insightstatetype) 
4. See [:material-code-braces: RequestImpactStatisticsTypeDef](./type_defs.md#requestimpactstatisticstypedef) 
5. See [:material-code-braces: RequestImpactStatisticsTypeDef](./type_defs.md#requestimpactstatisticstypedef) 
6. See [:material-code-braces: AnomalousServiceTypeDef](./type_defs.md#anomalousservicetypedef) 
## GetGroupsResultTypeDef

```python
# GetGroupsResultTypeDef definition

class GetGroupsResultTypeDef(TypedDict):
    Groups: List[GroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupResultTypeDef

```python
# CreateGroupResultTypeDef definition

class CreateGroupResultTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupResultTypeDef

```python
# GetGroupResultTypeDef definition

class GetGroupResultTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGroupResultTypeDef

```python
# UpdateGroupResultTypeDef definition

class UpdateGroupResultTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EdgeTypeDef

```python
# EdgeTypeDef definition

class EdgeTypeDef(TypedDict):
    ReferenceId: NotRequired[int],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    SummaryStatistics: NotRequired[EdgeStatisticsTypeDef],  # (1)
    ResponseTimeHistogram: NotRequired[List[HistogramEntryTypeDef]],  # (2)
    Aliases: NotRequired[List[AliasTypeDef]],  # (3)
    EdgeType: NotRequired[str],
    ReceivedEventAgeHistogram: NotRequired[List[HistogramEntryTypeDef]],  # (2)
```

1. See [:material-code-braces: EdgeStatisticsTypeDef](./type_defs.md#edgestatisticstypedef) 
2. See [:material-code-braces: HistogramEntryTypeDef](./type_defs.md#histogramentrytypedef) 
3. See [:material-code-braces: AliasTypeDef](./type_defs.md#aliastypedef) 
4. See [:material-code-braces: HistogramEntryTypeDef](./type_defs.md#histogramentrytypedef) 
## TimeSeriesServiceStatisticsTypeDef

```python
# TimeSeriesServiceStatisticsTypeDef definition

class TimeSeriesServiceStatisticsTypeDef(TypedDict):
    Timestamp: NotRequired[datetime],
    EdgeSummaryStatistics: NotRequired[EdgeStatisticsTypeDef],  # (1)
    ServiceSummaryStatistics: NotRequired[ServiceStatisticsTypeDef],  # (2)
    ServiceForecastStatistics: NotRequired[ForecastStatisticsTypeDef],  # (3)
    ResponseTimeHistogram: NotRequired[List[HistogramEntryTypeDef]],  # (4)
```

1. See [:material-code-braces: EdgeStatisticsTypeDef](./type_defs.md#edgestatisticstypedef) 
2. See [:material-code-braces: ServiceStatisticsTypeDef](./type_defs.md#servicestatisticstypedef) 
3. See [:material-code-braces: ForecastStatisticsTypeDef](./type_defs.md#forecaststatisticstypedef) 
4. See [:material-code-braces: HistogramEntryTypeDef](./type_defs.md#histogramentrytypedef) 
## ErrorRootCauseServiceTypeDef

```python
# ErrorRootCauseServiceTypeDef definition

class ErrorRootCauseServiceTypeDef(TypedDict):
    Name: NotRequired[str],
    Names: NotRequired[List[str]],
    Type: NotRequired[str],
    AccountId: NotRequired[str],
    EntityPath: NotRequired[List[ErrorRootCauseEntityTypeDef]],  # (1)
    Inferred: NotRequired[bool],
```

1. See [:material-code-braces: ErrorRootCauseEntityTypeDef](./type_defs.md#errorrootcauseentitytypedef) 
## FaultRootCauseServiceTypeDef

```python
# FaultRootCauseServiceTypeDef definition

class FaultRootCauseServiceTypeDef(TypedDict):
    Name: NotRequired[str],
    Names: NotRequired[List[str]],
    Type: NotRequired[str],
    AccountId: NotRequired[str],
    EntityPath: NotRequired[List[FaultRootCauseEntityTypeDef]],  # (1)
    Inferred: NotRequired[bool],
```

1. See [:material-code-braces: FaultRootCauseEntityTypeDef](./type_defs.md#faultrootcauseentitytypedef) 
## GetSamplingTargetsRequestRequestTypeDef

```python
# GetSamplingTargetsRequestRequestTypeDef definition

class GetSamplingTargetsRequestRequestTypeDef(TypedDict):
    SamplingStatisticsDocuments: Sequence[SamplingStatisticsDocumentTypeDef],  # (1)
```

1. See [:material-code-braces: SamplingStatisticsDocumentTypeDef](./type_defs.md#samplingstatisticsdocumenttypedef) 
## PutTelemetryRecordsRequestRequestTypeDef

```python
# PutTelemetryRecordsRequestRequestTypeDef definition

class PutTelemetryRecordsRequestRequestTypeDef(TypedDict):
    TelemetryRecords: Sequence[TelemetryRecordTypeDef],  # (1)
    EC2InstanceId: NotRequired[str],
    Hostname: NotRequired[str],
    ResourceARN: NotRequired[str],
```

1. See [:material-code-braces: TelemetryRecordTypeDef](./type_defs.md#telemetryrecordtypedef) 
## IndexingRuleTypeDef

```python
# IndexingRuleTypeDef definition

class IndexingRuleTypeDef(TypedDict):
    Name: NotRequired[str],
    ModifiedAt: NotRequired[datetime],
    Rule: NotRequired[IndexingRuleValueTypeDef],  # (1)
```

1. See [:material-code-braces: IndexingRuleValueTypeDef](./type_defs.md#indexingrulevaluetypedef) 
## UpdateIndexingRuleRequestRequestTypeDef

```python
# UpdateIndexingRuleRequestRequestTypeDef definition

class UpdateIndexingRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    Rule: IndexingRuleValueUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: IndexingRuleValueUpdateTypeDef](./type_defs.md#indexingrulevalueupdatetypedef) 
## GetInsightImpactGraphResultTypeDef

```python
# GetInsightImpactGraphResultTypeDef definition

class GetInsightImpactGraphResultTypeDef(TypedDict):
    InsightId: str,
    StartTime: datetime,
    EndTime: datetime,
    ServiceGraphStartTime: datetime,
    ServiceGraphEndTime: datetime,
    Services: List[InsightImpactGraphServiceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InsightImpactGraphServiceTypeDef](./type_defs.md#insightimpactgraphservicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResponseTimeRootCauseTypeDef

```python
# ResponseTimeRootCauseTypeDef definition

class ResponseTimeRootCauseTypeDef(TypedDict):
    Services: NotRequired[List[ResponseTimeRootCauseServiceTypeDef]],  # (1)
    ClientImpacting: NotRequired[bool],
```

1. See [:material-code-braces: ResponseTimeRootCauseServiceTypeDef](./type_defs.md#responsetimerootcauseservicetypedef) 
## ListRetrievedTracesResultTypeDef

```python
# ListRetrievedTracesResultTypeDef definition

class ListRetrievedTracesResultTypeDef(TypedDict):
    RetrievalStatus: RetrievalStatusType,  # (1)
    TraceFormat: TraceFormatTypeType,  # (2)
    Traces: List[RetrievedTraceTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RetrievalStatusType](./literals.md#retrievalstatustype) 
2. See [:material-code-brackets: TraceFormatTypeType](./literals.md#traceformattypetype) 
3. See [:material-code-braces: RetrievedTraceTypeDef](./type_defs.md#retrievedtracetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSamplingRuleResultTypeDef

```python
# CreateSamplingRuleResultTypeDef definition

class CreateSamplingRuleResultTypeDef(TypedDict):
    SamplingRuleRecord: SamplingRuleRecordTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SamplingRuleRecordTypeDef](./type_defs.md#samplingrulerecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSamplingRuleResultTypeDef

```python
# DeleteSamplingRuleResultTypeDef definition

class DeleteSamplingRuleResultTypeDef(TypedDict):
    SamplingRuleRecord: SamplingRuleRecordTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SamplingRuleRecordTypeDef](./type_defs.md#samplingrulerecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSamplingRulesResultTypeDef

```python
# GetSamplingRulesResultTypeDef definition

class GetSamplingRulesResultTypeDef(TypedDict):
    SamplingRuleRecords: List[SamplingRuleRecordTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SamplingRuleRecordTypeDef](./type_defs.md#samplingrulerecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSamplingRuleResultTypeDef

```python
# UpdateSamplingRuleResultTypeDef definition

class UpdateSamplingRuleResultTypeDef(TypedDict):
    SamplingRuleRecord: SamplingRuleRecordTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SamplingRuleRecordTypeDef](./type_defs.md#samplingrulerecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetTracesResultTypeDef

```python
# BatchGetTracesResultTypeDef definition

class BatchGetTracesResultTypeDef(TypedDict):
    Traces: List[TraceTypeDef],  # (1)
    UnprocessedTraceIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TraceTypeDef](./type_defs.md#tracetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInsightEventsResultTypeDef

```python
# GetInsightEventsResultTypeDef definition

class GetInsightEventsResultTypeDef(TypedDict):
    InsightEvents: List[InsightEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InsightEventTypeDef](./type_defs.md#insighteventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInsightSummariesResultTypeDef

```python
# GetInsightSummariesResultTypeDef definition

class GetInsightSummariesResultTypeDef(TypedDict):
    InsightSummaries: List[InsightSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InsightSummaryTypeDef](./type_defs.md#insightsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInsightResultTypeDef

```python
# GetInsightResultTypeDef definition

class GetInsightResultTypeDef(TypedDict):
    Insight: InsightTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightTypeDef](./type_defs.md#insighttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceTypeDef

```python
# ServiceTypeDef definition

class ServiceTypeDef(TypedDict):
    ReferenceId: NotRequired[int],
    Name: NotRequired[str],
    Names: NotRequired[List[str]],
    Root: NotRequired[bool],
    AccountId: NotRequired[str],
    Type: NotRequired[str],
    State: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Edges: NotRequired[List[EdgeTypeDef]],  # (1)
    SummaryStatistics: NotRequired[ServiceStatisticsTypeDef],  # (2)
    DurationHistogram: NotRequired[List[HistogramEntryTypeDef]],  # (3)
    ResponseTimeHistogram: NotRequired[List[HistogramEntryTypeDef]],  # (3)
```

1. See [:material-code-braces: EdgeTypeDef](./type_defs.md#edgetypedef) 
2. See [:material-code-braces: ServiceStatisticsTypeDef](./type_defs.md#servicestatisticstypedef) 
3. See [:material-code-braces: HistogramEntryTypeDef](./type_defs.md#histogramentrytypedef) 
4. See [:material-code-braces: HistogramEntryTypeDef](./type_defs.md#histogramentrytypedef) 
## GetTimeSeriesServiceStatisticsResultTypeDef

```python
# GetTimeSeriesServiceStatisticsResultTypeDef definition

class GetTimeSeriesServiceStatisticsResultTypeDef(TypedDict):
    TimeSeriesServiceStatistics: List[TimeSeriesServiceStatisticsTypeDef],  # (1)
    ContainsOldGroupVersions: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TimeSeriesServiceStatisticsTypeDef](./type_defs.md#timeseriesservicestatisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ErrorRootCauseTypeDef

```python
# ErrorRootCauseTypeDef definition

class ErrorRootCauseTypeDef(TypedDict):
    Services: NotRequired[List[ErrorRootCauseServiceTypeDef]],  # (1)
    ClientImpacting: NotRequired[bool],
```

1. See [:material-code-braces: ErrorRootCauseServiceTypeDef](./type_defs.md#errorrootcauseservicetypedef) 
## FaultRootCauseTypeDef

```python
# FaultRootCauseTypeDef definition

class FaultRootCauseTypeDef(TypedDict):
    Services: NotRequired[List[FaultRootCauseServiceTypeDef]],  # (1)
    ClientImpacting: NotRequired[bool],
```

1. See [:material-code-braces: FaultRootCauseServiceTypeDef](./type_defs.md#faultrootcauseservicetypedef) 
## GetIndexingRulesResultTypeDef

```python
# GetIndexingRulesResultTypeDef definition

class GetIndexingRulesResultTypeDef(TypedDict):
    IndexingRules: List[IndexingRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IndexingRuleTypeDef](./type_defs.md#indexingruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIndexingRuleResultTypeDef

```python
# UpdateIndexingRuleResultTypeDef definition

class UpdateIndexingRuleResultTypeDef(TypedDict):
    IndexingRule: IndexingRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IndexingRuleTypeDef](./type_defs.md#indexingruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceGraphResultTypeDef

```python
# GetServiceGraphResultTypeDef definition

class GetServiceGraphResultTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: datetime,
    Services: List[ServiceTypeDef],  # (1)
    ContainsOldGroupVersions: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTraceGraphResultTypeDef

```python
# GetTraceGraphResultTypeDef definition

class GetTraceGraphResultTypeDef(TypedDict):
    Services: List[ServiceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RetrievedServiceTypeDef

```python
# RetrievedServiceTypeDef definition

class RetrievedServiceTypeDef(TypedDict):
    Service: NotRequired[ServiceTypeDef],  # (1)
    Links: NotRequired[List[GraphLinkTypeDef]],  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: GraphLinkTypeDef](./type_defs.md#graphlinktypedef) 
## TraceSummaryTypeDef

```python
# TraceSummaryTypeDef definition

class TraceSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    StartTime: NotRequired[datetime],
    Duration: NotRequired[float],
    ResponseTime: NotRequired[float],
    HasFault: NotRequired[bool],
    HasError: NotRequired[bool],
    HasThrottle: NotRequired[bool],
    IsPartial: NotRequired[bool],
    Http: NotRequired[HttpTypeDef],  # (1)
    Annotations: NotRequired[Dict[str, List[ValueWithServiceIdsTypeDef]]],  # (2)
    Users: NotRequired[List[TraceUserTypeDef]],  # (3)
    ServiceIds: NotRequired[List[ServiceIdTypeDef]],  # (4)
    ResourceARNs: NotRequired[List[ResourceARNDetailTypeDef]],  # (5)
    InstanceIds: NotRequired[List[InstanceIdDetailTypeDef]],  # (6)
    AvailabilityZones: NotRequired[List[AvailabilityZoneDetailTypeDef]],  # (7)
    EntryPoint: NotRequired[ServiceIdTypeDef],  # (8)
    FaultRootCauses: NotRequired[List[FaultRootCauseTypeDef]],  # (9)
    ErrorRootCauses: NotRequired[List[ErrorRootCauseTypeDef]],  # (10)
    ResponseTimeRootCauses: NotRequired[List[ResponseTimeRootCauseTypeDef]],  # (11)
    Revision: NotRequired[int],
    MatchedEventTime: NotRequired[datetime],
```

1. See [:material-code-braces: HttpTypeDef](./type_defs.md#httptypedef) 
2. See [:material-code-braces: ValueWithServiceIdsTypeDef](./type_defs.md#valuewithserviceidstypedef) 
3. See [:material-code-braces: TraceUserTypeDef](./type_defs.md#traceusertypedef) 
4. See [:material-code-braces: ServiceIdTypeDef](./type_defs.md#serviceidtypedef) 
5. See [:material-code-braces: ResourceARNDetailTypeDef](./type_defs.md#resourcearndetailtypedef) 
6. See [:material-code-braces: InstanceIdDetailTypeDef](./type_defs.md#instanceiddetailtypedef) 
7. See [:material-code-braces: AvailabilityZoneDetailTypeDef](./type_defs.md#availabilityzonedetailtypedef) 
8. See [:material-code-braces: ServiceIdTypeDef](./type_defs.md#serviceidtypedef) 
9. See [:material-code-braces: FaultRootCauseTypeDef](./type_defs.md#faultrootcausetypedef) 
10. See [:material-code-braces: ErrorRootCauseTypeDef](./type_defs.md#errorrootcausetypedef) 
11. See [:material-code-braces: ResponseTimeRootCauseTypeDef](./type_defs.md#responsetimerootcausetypedef) 
## GetRetrievedTracesGraphResultTypeDef

```python
# GetRetrievedTracesGraphResultTypeDef definition

class GetRetrievedTracesGraphResultTypeDef(TypedDict):
    RetrievalStatus: RetrievalStatusType,  # (1)
    Services: List[RetrievedServiceTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RetrievalStatusType](./literals.md#retrievalstatustype) 
2. See [:material-code-braces: RetrievedServiceTypeDef](./type_defs.md#retrievedservicetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTraceSummariesResultTypeDef

```python
# GetTraceSummariesResultTypeDef definition

class GetTraceSummariesResultTypeDef(TypedDict):
    TraceSummaries: List[TraceSummaryTypeDef],  # (1)
    ApproximateTime: datetime,
    TracesProcessedCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TraceSummaryTypeDef](./type_defs.md#tracesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
