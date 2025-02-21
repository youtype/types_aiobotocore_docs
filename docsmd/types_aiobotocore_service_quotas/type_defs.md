# Type definitions

> [Index](../README.md) > [ServiceQuotas](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ServiceQuotas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#servicequotas)
    type annotations stubs module [types-aiobotocore-service-quotas](https://pypi.org/project/types-aiobotocore-service-quotas/).



## DeleteServiceQuotaIncreaseRequestFromTemplateRequestTypeDef

```python
# DeleteServiceQuotaIncreaseRequestFromTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import DeleteServiceQuotaIncreaseRequestFromTemplateRequestTypeDef


def get_value() -> DeleteServiceQuotaIncreaseRequestFromTemplateRequestTypeDef:
    return {
        "ServiceCode": ...,
    }


# DeleteServiceQuotaIncreaseRequestFromTemplateRequestTypeDef definition

class DeleteServiceQuotaIncreaseRequestFromTemplateRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    AwsRegion: str,
```

## ErrorReasonTypeDef

```python
# ErrorReasonTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ErrorReasonTypeDef


def get_value() -> ErrorReasonTypeDef:
    return {
        "ErrorCode": ...,
    }


# ErrorReasonTypeDef definition

class ErrorReasonTypeDef(TypedDict):
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## GetAWSDefaultServiceQuotaRequestTypeDef

```python
# GetAWSDefaultServiceQuotaRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import GetAWSDefaultServiceQuotaRequestTypeDef


def get_value() -> GetAWSDefaultServiceQuotaRequestTypeDef:
    return {
        "ServiceCode": ...,
    }


# GetAWSDefaultServiceQuotaRequestTypeDef definition

class GetAWSDefaultServiceQuotaRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ResponseMetadataTypeDef


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

## GetRequestedServiceQuotaChangeRequestTypeDef

```python
# GetRequestedServiceQuotaChangeRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import GetRequestedServiceQuotaChangeRequestTypeDef


def get_value() -> GetRequestedServiceQuotaChangeRequestTypeDef:
    return {
        "RequestId": ...,
    }


# GetRequestedServiceQuotaChangeRequestTypeDef definition

class GetRequestedServiceQuotaChangeRequestTypeDef(TypedDict):
    RequestId: str,
```

## GetServiceQuotaIncreaseRequestFromTemplateRequestTypeDef

```python
# GetServiceQuotaIncreaseRequestFromTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import GetServiceQuotaIncreaseRequestFromTemplateRequestTypeDef


def get_value() -> GetServiceQuotaIncreaseRequestFromTemplateRequestTypeDef:
    return {
        "ServiceCode": ...,
    }


# GetServiceQuotaIncreaseRequestFromTemplateRequestTypeDef definition

class GetServiceQuotaIncreaseRequestFromTemplateRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    AwsRegion: str,
```

## ServiceQuotaIncreaseRequestInTemplateTypeDef

```python
# ServiceQuotaIncreaseRequestInTemplateTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ServiceQuotaIncreaseRequestInTemplateTypeDef


def get_value() -> ServiceQuotaIncreaseRequestInTemplateTypeDef:
    return {
        "ServiceCode": ...,
    }


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

## GetServiceQuotaRequestTypeDef

```python
# GetServiceQuotaRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import GetServiceQuotaRequestTypeDef


def get_value() -> GetServiceQuotaRequestTypeDef:
    return {
        "ServiceCode": ...,
    }


# GetServiceQuotaRequestTypeDef definition

class GetServiceQuotaRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    ContextId: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import PaginatorConfigTypeDef


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

## ListAWSDefaultServiceQuotasRequestTypeDef

```python
# ListAWSDefaultServiceQuotasRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListAWSDefaultServiceQuotasRequestTypeDef


def get_value() -> ListAWSDefaultServiceQuotasRequestTypeDef:
    return {
        "ServiceCode": ...,
    }


# ListAWSDefaultServiceQuotasRequestTypeDef definition

class ListAWSDefaultServiceQuotasRequestTypeDef(TypedDict):
    ServiceCode: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListRequestedServiceQuotaChangeHistoryByQuotaRequestTypeDef

```python
# ListRequestedServiceQuotaChangeHistoryByQuotaRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListRequestedServiceQuotaChangeHistoryByQuotaRequestTypeDef


def get_value() -> ListRequestedServiceQuotaChangeHistoryByQuotaRequestTypeDef:
    return {
        "ServiceCode": ...,
    }


# ListRequestedServiceQuotaChangeHistoryByQuotaRequestTypeDef definition

class ListRequestedServiceQuotaChangeHistoryByQuotaRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    Status: NotRequired[RequestStatusType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    QuotaRequestedAtLevel: NotRequired[AppliedLevelEnumType],  # (2)
```

1. See [:material-code-brackets: RequestStatusType](./literals.md#requeststatustype) 
2. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
## ListRequestedServiceQuotaChangeHistoryRequestTypeDef

```python
# ListRequestedServiceQuotaChangeHistoryRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListRequestedServiceQuotaChangeHistoryRequestTypeDef


def get_value() -> ListRequestedServiceQuotaChangeHistoryRequestTypeDef:
    return {
        "ServiceCode": ...,
    }


# ListRequestedServiceQuotaChangeHistoryRequestTypeDef definition

class ListRequestedServiceQuotaChangeHistoryRequestTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    Status: NotRequired[RequestStatusType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    QuotaRequestedAtLevel: NotRequired[AppliedLevelEnumType],  # (2)
```

1. See [:material-code-brackets: RequestStatusType](./literals.md#requeststatustype) 
2. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
## ListServiceQuotaIncreaseRequestsInTemplateRequestTypeDef

```python
# ListServiceQuotaIncreaseRequestsInTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListServiceQuotaIncreaseRequestsInTemplateRequestTypeDef


def get_value() -> ListServiceQuotaIncreaseRequestsInTemplateRequestTypeDef:
    return {
        "ServiceCode": ...,
    }


# ListServiceQuotaIncreaseRequestsInTemplateRequestTypeDef definition

class ListServiceQuotaIncreaseRequestsInTemplateRequestTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    AwsRegion: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListServiceQuotasRequestTypeDef

```python
# ListServiceQuotasRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListServiceQuotasRequestTypeDef


def get_value() -> ListServiceQuotasRequestTypeDef:
    return {
        "ServiceCode": ...,
    }


# ListServiceQuotasRequestTypeDef definition

class ListServiceQuotasRequestTypeDef(TypedDict):
    ServiceCode: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    QuotaCode: NotRequired[str],
    QuotaAppliedAtLevel: NotRequired[AppliedLevelEnumType],  # (1)
```

1. See [:material-code-brackets: AppliedLevelEnumType](./literals.md#appliedlevelenumtype) 
## ListServicesRequestTypeDef

```python
# ListServicesRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListServicesRequestTypeDef


def get_value() -> ListServicesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListServicesRequestTypeDef definition

class ListServicesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ServiceInfoTypeDef

```python
# ServiceInfoTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ServiceInfoTypeDef


def get_value() -> ServiceInfoTypeDef:
    return {
        "ServiceCode": ...,
    }


# ServiceInfoTypeDef definition

class ServiceInfoTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    ServiceName: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceARN": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## MetricInfoTypeDef

```python
# MetricInfoTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import MetricInfoTypeDef


def get_value() -> MetricInfoTypeDef:
    return {
        "MetricNamespace": ...,
    }


# MetricInfoTypeDef definition

class MetricInfoTypeDef(TypedDict):
    MetricNamespace: NotRequired[str],
    MetricName: NotRequired[str],
    MetricDimensions: NotRequired[Dict[str, str]],
    MetricStatisticRecommendation: NotRequired[str],
```

## PutServiceQuotaIncreaseRequestIntoTemplateRequestTypeDef

```python
# PutServiceQuotaIncreaseRequestIntoTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import PutServiceQuotaIncreaseRequestIntoTemplateRequestTypeDef


def get_value() -> PutServiceQuotaIncreaseRequestIntoTemplateRequestTypeDef:
    return {
        "QuotaCode": ...,
    }


# PutServiceQuotaIncreaseRequestIntoTemplateRequestTypeDef definition

class PutServiceQuotaIncreaseRequestIntoTemplateRequestTypeDef(TypedDict):
    QuotaCode: str,
    ServiceCode: str,
    AwsRegion: str,
    DesiredValue: float,
```

## QuotaContextInfoTypeDef

```python
# QuotaContextInfoTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import QuotaContextInfoTypeDef


def get_value() -> QuotaContextInfoTypeDef:
    return {
        "ContextScope": ...,
    }


# QuotaContextInfoTypeDef definition

class QuotaContextInfoTypeDef(TypedDict):
    ContextScope: NotRequired[QuotaContextScopeType],  # (1)
    ContextScopeType: NotRequired[str],
    ContextId: NotRequired[str],
```

1. See [:material-code-brackets: QuotaContextScopeType](./literals.md#quotacontextscopetype) 
## QuotaPeriodTypeDef

```python
# QuotaPeriodTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import QuotaPeriodTypeDef


def get_value() -> QuotaPeriodTypeDef:
    return {
        "PeriodValue": ...,
    }


# QuotaPeriodTypeDef definition

class QuotaPeriodTypeDef(TypedDict):
    PeriodValue: NotRequired[int],
    PeriodUnit: NotRequired[PeriodUnitType],  # (1)
```

1. See [:material-code-brackets: PeriodUnitType](./literals.md#periodunittype) 
## RequestServiceQuotaIncreaseRequestTypeDef

```python
# RequestServiceQuotaIncreaseRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import RequestServiceQuotaIncreaseRequestTypeDef


def get_value() -> RequestServiceQuotaIncreaseRequestTypeDef:
    return {
        "ServiceCode": ...,
    }


# RequestServiceQuotaIncreaseRequestTypeDef definition

class RequestServiceQuotaIncreaseRequestTypeDef(TypedDict):
    ServiceCode: str,
    QuotaCode: str,
    DesiredValue: float,
    ContextId: NotRequired[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceARN": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## GetAssociationForServiceQuotaTemplateResponseTypeDef

```python
# GetAssociationForServiceQuotaTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import GetAssociationForServiceQuotaTemplateResponseTypeDef


def get_value() -> GetAssociationForServiceQuotaTemplateResponseTypeDef:
    return {
        "ServiceQuotaTemplateAssociationStatus": ...,
    }


# GetAssociationForServiceQuotaTemplateResponseTypeDef definition

class GetAssociationForServiceQuotaTemplateResponseTypeDef(TypedDict):
    ServiceQuotaTemplateAssociationStatus: ServiceQuotaTemplateAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceQuotaTemplateAssociationStatusType](./literals.md#servicequotatemplateassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef

```python
# GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef


def get_value() -> GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef:
    return {
        "ServiceQuotaIncreaseRequestInTemplate": ...,
    }


# GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef definition

class GetServiceQuotaIncreaseRequestFromTemplateResponseTypeDef(TypedDict):
    ServiceQuotaIncreaseRequestInTemplate: ServiceQuotaIncreaseRequestInTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceQuotaIncreaseRequestInTemplateTypeDef](./type_defs.md#servicequotaincreaserequestintemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef

```python
# ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef


def get_value() -> ListServiceQuotaIncreaseRequestsInTemplateResponseTypeDef:
    return {
        "ServiceQuotaIncreaseRequestInTemplateList": ...,
    }


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
# PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef


def get_value() -> PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef:
    return {
        "ServiceQuotaIncreaseRequestInTemplate": ...,
    }


# PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef definition

class PutServiceQuotaIncreaseRequestIntoTemplateResponseTypeDef(TypedDict):
    ServiceQuotaIncreaseRequestInTemplate: ServiceQuotaIncreaseRequestInTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceQuotaIncreaseRequestInTemplateTypeDef](./type_defs.md#servicequotaincreaserequestintemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAWSDefaultServiceQuotasRequestPaginateTypeDef

```python
# ListAWSDefaultServiceQuotasRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListAWSDefaultServiceQuotasRequestPaginateTypeDef


def get_value() -> ListAWSDefaultServiceQuotasRequestPaginateTypeDef:
    return {
        "ServiceCode": ...,
    }


# ListAWSDefaultServiceQuotasRequestPaginateTypeDef definition

class ListAWSDefaultServiceQuotasRequestPaginateTypeDef(TypedDict):
    ServiceCode: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRequestedServiceQuotaChangeHistoryByQuotaRequestPaginateTypeDef

```python
# ListRequestedServiceQuotaChangeHistoryByQuotaRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListRequestedServiceQuotaChangeHistoryByQuotaRequestPaginateTypeDef


def get_value() -> ListRequestedServiceQuotaChangeHistoryByQuotaRequestPaginateTypeDef:
    return {
        "ServiceCode": ...,
    }


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
# ListRequestedServiceQuotaChangeHistoryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListRequestedServiceQuotaChangeHistoryRequestPaginateTypeDef


def get_value() -> ListRequestedServiceQuotaChangeHistoryRequestPaginateTypeDef:
    return {
        "ServiceCode": ...,
    }


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
# ListServiceQuotaIncreaseRequestsInTemplateRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListServiceQuotaIncreaseRequestsInTemplateRequestPaginateTypeDef


def get_value() -> ListServiceQuotaIncreaseRequestsInTemplateRequestPaginateTypeDef:
    return {
        "ServiceCode": ...,
    }


# ListServiceQuotaIncreaseRequestsInTemplateRequestPaginateTypeDef definition

class ListServiceQuotaIncreaseRequestsInTemplateRequestPaginateTypeDef(TypedDict):
    ServiceCode: NotRequired[str],
    AwsRegion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceQuotasRequestPaginateTypeDef

```python
# ListServiceQuotasRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListServiceQuotasRequestPaginateTypeDef


def get_value() -> ListServiceQuotasRequestPaginateTypeDef:
    return {
        "ServiceCode": ...,
    }


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
# ListServicesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListServicesRequestPaginateTypeDef


def get_value() -> ListServicesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListServicesRequestPaginateTypeDef definition

class ListServicesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesResponseTypeDef

```python
# ListServicesResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListServicesResponseTypeDef


def get_value() -> ListServicesResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceARN": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RequestedServiceQuotaChangeTypeDef

```python
# RequestedServiceQuotaChangeTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import RequestedServiceQuotaChangeTypeDef


def get_value() -> RequestedServiceQuotaChangeTypeDef:
    return {
        "Id": ...,
    }


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
# ServiceQuotaTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ServiceQuotaTypeDef


def get_value() -> ServiceQuotaTypeDef:
    return {
        "ServiceCode": ...,
    }


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
# GetRequestedServiceQuotaChangeResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import GetRequestedServiceQuotaChangeResponseTypeDef


def get_value() -> GetRequestedServiceQuotaChangeResponseTypeDef:
    return {
        "RequestedQuota": ...,
    }


# GetRequestedServiceQuotaChangeResponseTypeDef definition

class GetRequestedServiceQuotaChangeResponseTypeDef(TypedDict):
    RequestedQuota: RequestedServiceQuotaChangeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RequestedServiceQuotaChangeTypeDef](./type_defs.md#requestedservicequotachangetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef

```python
# ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef


def get_value() -> ListRequestedServiceQuotaChangeHistoryByQuotaResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListRequestedServiceQuotaChangeHistoryResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListRequestedServiceQuotaChangeHistoryResponseTypeDef


def get_value() -> ListRequestedServiceQuotaChangeHistoryResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# RequestServiceQuotaIncreaseResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import RequestServiceQuotaIncreaseResponseTypeDef


def get_value() -> RequestServiceQuotaIncreaseResponseTypeDef:
    return {
        "RequestedQuota": ...,
    }


# RequestServiceQuotaIncreaseResponseTypeDef definition

class RequestServiceQuotaIncreaseResponseTypeDef(TypedDict):
    RequestedQuota: RequestedServiceQuotaChangeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RequestedServiceQuotaChangeTypeDef](./type_defs.md#requestedservicequotachangetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAWSDefaultServiceQuotaResponseTypeDef

```python
# GetAWSDefaultServiceQuotaResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import GetAWSDefaultServiceQuotaResponseTypeDef


def get_value() -> GetAWSDefaultServiceQuotaResponseTypeDef:
    return {
        "Quota": ...,
    }


# GetAWSDefaultServiceQuotaResponseTypeDef definition

class GetAWSDefaultServiceQuotaResponseTypeDef(TypedDict):
    Quota: ServiceQuotaTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceQuotaTypeDef](./type_defs.md#servicequotatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceQuotaResponseTypeDef

```python
# GetServiceQuotaResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import GetServiceQuotaResponseTypeDef


def get_value() -> GetServiceQuotaResponseTypeDef:
    return {
        "Quota": ...,
    }


# GetServiceQuotaResponseTypeDef definition

class GetServiceQuotaResponseTypeDef(TypedDict):
    Quota: ServiceQuotaTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceQuotaTypeDef](./type_defs.md#servicequotatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAWSDefaultServiceQuotasResponseTypeDef

```python
# ListAWSDefaultServiceQuotasResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListAWSDefaultServiceQuotasResponseTypeDef


def get_value() -> ListAWSDefaultServiceQuotasResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListServiceQuotasResponseTypeDef TypedDict usage example

from types_aiobotocore_service_quotas.type_defs import ListServiceQuotasResponseTypeDef


def get_value() -> ListServiceQuotasResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListServiceQuotasResponseTypeDef definition

class ListServiceQuotasResponseTypeDef(TypedDict):
    Quotas: List[ServiceQuotaTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceQuotaTypeDef](./type_defs.md#servicequotatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
