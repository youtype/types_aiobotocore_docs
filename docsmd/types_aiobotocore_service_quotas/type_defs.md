# Type definitions

> [Index](../README.md) > [ServiceQuotas](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ServiceQuotas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#servicequotas)
    type annotations stubs module [types-aiobotocore-service-quotas](https://pypi.org/project/types-aiobotocore-service-quotas/).



## DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef

```python
# DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef definition

class DeleteServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    AwsRegion: str,
```

## ErrorReasonTypeDef

```python
# ErrorReasonTypeDef definition

class ErrorReasonTypeDef(TypedDict):
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## GetAWSDefaultServiceQuotaRequestRequestTypeDef

```python
# GetAWSDefaultServiceQuotaRequestRequestTypeDef definition

class GetAWSDefaultServiceQuotaRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
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

## GetRequestedServiceQuotaChangeRequestRequestTypeDef

```python
# GetRequestedServiceQuotaChangeRequestRequestTypeDef definition

class GetRequestedServiceQuotaChangeRequestRequestTypeDef(TypedDict):
    RequestId: str,
```

## GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef

```python
# GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef definition

class GetServiceQuotaIncreaseRequestFromTemplateRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    AwsRegion: str,
```

## ServiceQuotaIncreaseRequestInTemplateTypeDef

```python
# ServiceQuotaIncreaseRequestInTemplateTypeDef definition

class ServiceQuotaIncreaseRequestInTemplateTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    ServiceName: NotRequired[str],
    QuotaCode: NotRequired[str],
    QuotaName: NotRequired[str],
    DesiredValue: NotRequired[float],
    AwsRegion: NotRequired[str],
    Unit: NotRequired[str],
    GlobalQuota: NotRequired[bool],
```

## GetServiceQuotaRequestRequestTypeDef

```python
# GetServiceQuotaRequestRequestTypeDef definition

class GetServiceQuotaRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    ContextId: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAWSDefaultServiceQuotasRequestRequestTypeDef

```python
# ListAWSDefaultServiceQuotasRequestRequestTypeDef definition

class ListAWSDefaultServiceQuotasRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef

```python
# ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef definition

class ListRequestedServiceQuotaChangeHistoryByQuotaRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    Status: NotRequired[RequestStatusType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    QuotaRequestedAtLevel: NotRequired[AppliedLevelEnumType],  # (2)
```

1. See [:material-code-brackets: RequestStatusType](./literals.md#requeststatustype) 
2. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
## ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef

```python
# ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef definition

class ListRequestedServiceQuotaChangeHistoryRequestRequestTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    Status: NotRequired[RequestStatusType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    QuotaRequestedAtLevel: NotRequired[AppliedLevelEnumType],  # (2)
```

1. See [:material-code-brackets: RequestStatusType](./literals.md#requeststatustype) 
2. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
## ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef

```python
# ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef definition

class ListServiceQuotaIncreaseRequestsInTemplateRequestRequestTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    AwsRegion: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListServiceQuotasRequestRequestTypeDef

```python
# ListServiceQuotasRequestRequestTypeDef definition

class ListServiceQuotasRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    QuotaCode: NotRequired[str],
    QuotaAppliedAtLevel: NotRequired[AppliedLevelEnumType],  # (1)
```

1. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
## ListServicesRequestRequestTypeDef

```python
# ListServicesRequestRequestTypeDef definition

class ListServicesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ServiceInfoTypeDef

```python
# ServiceInfoTypeDef definition

class ServiceInfoTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    ServiceName: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## MetricInfoTypeDef

```python
# MetricInfoTypeDef definition

class MetricInfoTypeDef(TypedDict):
    MetricNamespace: NotRequired[str],
    MetricName: NotRequired[str],
    MetricDimensions: NotRequired[Dict[str, str]],
    MetricStatisticRecommendation: NotRequired[str],
```

## PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef

```python
# PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef definition

class PutServiceQuotaIncreaseRequestIntoTemplateRequestRequestTypeDef(TypedDict):
    QuotaCode: str,
    ServiceCode: str,
    AwsRegion: str,
    DesiredValue: float,
```

## QuotaContextInfoTypeDef

```python
# QuotaContextInfoTypeDef definition

class QuotaContextInfoTypeDef(TypedDict):
    ContextScope: NotRequired[QuotaContextScopeType],  # (1)
    ContextScopeType: NotRequired[str],
    ContextId: NotRequired[str],
```

1. See [:material-code-brackets: QuotaContextScopeType](./literals.md#quotacontextscopetype) 
## QuotaPeriodTypeDef

```python
# QuotaPeriodTypeDef definition

class QuotaPeriodTypeDef(TypedDict):
    PeriodValue: NotRequired[int],
    PeriodUnit: NotRequired[PeriodUnitType],  # (1)
```

1. See [:material-code-brackets: PeriodUnitType](./literals.md#periodunittype) 
## RequestServiceQuotaIncreaseRequestRequestTypeDef

```python
# RequestServiceQuotaIncreaseRequestRequestTypeDef definition

class RequestServiceQuotaIncreaseRequestRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    DesiredValue: float,
    ContextId: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## GetAssociationForServiceQuotaTemplateResponseTypeDef

```python
# GetAssociationForServiceQuotaTemplateResponseTypeDef definition

class GetAssociationForServiceQuotaTemplateResponseTypeDef(TypedDict):
    ServiceQuotaTemplateAssociationStatus: ServiceQuotaTemplateAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceQuotaTemplateAssociationStatusType](./literals.md#servicequotatemplateassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef

```python
# GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef definition

class GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef(TypedDict):
    ServiceQuotaIncreaseRequestInTemplate: ServiceQuotaIncreaseRequestInTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceQuotaIncreaseRequestInTemplateTypeDef](./type_defs.md#servicequotaincreaserequestintemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef

```python
# ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef definition

class ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef(TypedDict):
    ServiceQuotaIncreaseRequestInTemplateList: List[ServiceQuotaIncreaseRequestInTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceQuotaIncreaseRequestInTemplateTypeDef](./type_defs.md#servicequotaincreaserequestintemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef

```python
# PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef definition

class PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef(TypedDict):
    ServiceQuotaIncreaseRequestInTemplate: ServiceQuotaIncreaseRequestInTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceQuotaIncreaseRequestInTemplateTypeDef](./type_defs.md#servicequotaincreaserequestintemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAWSDefaultServiceQuotasRequestPaginateTypeDef

```python
# ListAWSDefaultServiceQuotasRequestPaginateTypeDef definition

class ListAWSDefaultServiceQuotasRequestPaginateTypeDef(TypedDict):
    ServiceCode: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRequestedServiceQuotaChangeHistoryByQuotaRequestPaginateTypeDef

```python
# ListRequestedServiceQuotaChangeHistoryByQuotaRequestPaginateTypeDef definition

class ListRequestedServiceQuotaChangeHistoryByQuotaRequestPaginateTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    Status: NotRequired[RequestStatusType],  # (1)
    QuotaRequestedAtLevel: NotRequired[AppliedLevelEnumType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RequestStatusType](./literals.md#requeststatustype) 
2. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRequestedServiceQuotaChangeHistoryRequestPaginateTypeDef

```python
# ListRequestedServiceQuotaChangeHistoryRequestPaginateTypeDef definition

class ListRequestedServiceQuotaChangeHistoryRequestPaginateTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    Status: NotRequired[RequestStatusType],  # (1)
    QuotaRequestedAtLevel: NotRequired[AppliedLevelEnumType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RequestStatusType](./literals.md#requeststatustype) 
2. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceQuotaIncreaseRequestsInTemplateRequestPaginateTypeDef

```python
# ListServiceQuotaIncreaseRequestsInTemplateRequestPaginateTypeDef definition

class ListServiceQuotaIncreaseRequestsInTemplateRequestPaginateTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    AwsRegion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceQuotasRequestPaginateTypeDef

```python
# ListServiceQuotasRequestPaginateTypeDef definition

class ListServiceQuotasRequestPaginateTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: NotRequired[str],
    QuotaAppliedAtLevel: NotRequired[AppliedLevelEnumType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesRequestPaginateTypeDef

```python
# ListServicesRequestPaginateTypeDef definition

class ListServicesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesResponseTypeDef

```python
# ListServicesResponseTypeDef definition

class ListServicesResponseTypeDef(TypedDict):
    Services: List[ServiceInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceInfoTypeDef](./type_defs.md#serviceinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## RequestedServiceQuotaChangeTypeDef

```python
# RequestedServiceQuotaChangeTypeDef definition

class RequestedServiceQuotaChangeTypeDef(TypedDict):
    Id: NotRequired[str],
    CaseId: NotRequired[str],
    ServiceCode: NotRequired[str],
    ServiceName: NotRequired[str],
    QuotaCode: NotRequired[str],
    QuotaName: NotRequired[str],
    DesiredValue: NotRequired[float],
    Status: NotRequired[RequestStatusType],  # (1)
    Created: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    Requester: NotRequired[str],
    QuotaArn: NotRequired[str],
    GlobalQuota: NotRequired[bool],
    Unit: NotRequired[str],
    QuotaRequestedAtLevel: NotRequired[AppliedLevelEnumType],  # (2)
    QuotaContext: NotRequired[QuotaContextInfoTypeDef],  # (3)
```

1. See [:material-code-brackets: RequestStatusType](./literals.md#requeststatustype) 
2. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
3. See [:material-code-braces: QuotaContextInfoTypeDef](./type_defs.md#quotacontextinfotypedef) 
## ServiceQuotaTypeDef

```python
# ServiceQuotaTypeDef definition

class ServiceQuotaTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    ServiceName: NotRequired[str],
    QuotaArn: NotRequired[str],
    QuotaCode: NotRequired[str],
    QuotaName: NotRequired[str],
    Value: NotRequired[float],
    Unit: NotRequired[str],
    Adjustable: NotRequired[bool],
    GlobalQuota: NotRequired[bool],
    UsageMetric: NotRequired[MetricInfoTypeDef],  # (1)
    Period: NotRequired[QuotaPeriodTypeDef],  # (2)
    ErrorReason: NotRequired[ErrorReasonTypeDef],  # (3)
    QuotaAppliedAtLevel: NotRequired[AppliedLevelEnumType],  # (4)
    QuotaContext: NotRequired[QuotaContextInfoTypeDef],  # (5)
```

1. See [:material-code-braces: MetricInfoTypeDef](./type_defs.md#metricinfotypedef) 
2. See [:material-code-braces: QuotaPeriodTypeDef](./type_defs.md#quotaperiodtypedef) 
3. See [:material-code-braces: ErrorReasonTypeDef](./type_defs.md#errorreasontypedef) 
4. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
5. See [:material-code-braces: QuotaContextInfoTypeDef](./type_defs.md#quotacontextinfotypedef) 
## GetRequestedServiceQuotaChangeResponseTypeDef

```python
# GetRequestedServiceQuotaChangeResponseTypeDef definition

class GetRequestedServiceQuotaChangeResponseTypeDef(TypedDict):
    RequestedQuota: RequestedServiceQuotaChangeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RequestedServiceQuotaChangeTypeDef](./type_defs.md#requestedservicequotachangetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef

```python
# ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef definition

class ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef(TypedDict):
    RequestedQuotas: List[RequestedServiceQuotaChangeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RequestedServiceQuotaChangeTypeDef](./type_defs.md#requestedservicequotachangetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRequestedServiceQuotaChangeHistoryResponseTypeDef

```python
# ListRequestedServiceQuotaChangeHistoryResponseTypeDef definition

class ListRequestedServiceQuotaChangeHistoryResponseTypeDef(TypedDict):
    RequestedQuotas: List[RequestedServiceQuotaChangeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RequestedServiceQuotaChangeTypeDef](./type_defs.md#requestedservicequotachangetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RequestServiceQuotaIncreaseResponseTypeDef

```python
# RequestServiceQuotaIncreaseResponseTypeDef definition

class RequestServiceQuotaIncreaseResponseTypeDef(TypedDict):
    RequestedQuota: RequestedServiceQuotaChangeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RequestedServiceQuotaChangeTypeDef](./type_defs.md#requestedservicequotachangetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAWSDefaultServiceQuotaResponseTypeDef

```python
# GetAWSDefaultServiceQuotaResponseTypeDef definition

class GetAWSDefaultServiceQuotaResponseTypeDef(TypedDict):
    Quota: ServiceQuotaTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceQuotaTypeDef](./type_defs.md#servicequotatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceQuotaResponseTypeDef

```python
# GetServiceQuotaResponseTypeDef definition

class GetServiceQuotaResponseTypeDef(TypedDict):
    Quota: ServiceQuotaTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceQuotaTypeDef](./type_defs.md#servicequotatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAWSDefaultServiceQuotasResponseTypeDef

```python
# ListAWSDefaultServiceQuotasResponseTypeDef definition

class ListAWSDefaultServiceQuotasResponseTypeDef(TypedDict):
    Quotas: List[ServiceQuotaTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceQuotaTypeDef](./type_defs.md#servicequotatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceQuotasResponseTypeDef

```python
# ListServiceQuotasResponseTypeDef definition

class ListServiceQuotasResponseTypeDef(TypedDict):
    Quotas: List[ServiceQuotaTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceQuotaTypeDef](./type_defs.md#servicequotatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
