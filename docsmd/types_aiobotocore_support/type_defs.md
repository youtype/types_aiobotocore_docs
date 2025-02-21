# Type definitions

> [Index](../README.md) > [Support](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Support](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#support)
    type annotations stubs module [types-aiobotocore-support](https://pypi.org/project/types-aiobotocore-support/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_support.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## AttachmentUnionTypeDef

```python
# AttachmentUnionTypeDef Union usage example

from types_aiobotocore_support.type_defs import AttachmentUnionTypeDef


def get_value() -> AttachmentUnionTypeDef:
    return ...


# AttachmentUnionTypeDef definition

AttachmentUnionTypeDef = Union[
    AttachmentTypeDef,  # (1)
    AttachmentOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
2. See [:material-code-braces: AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef) 



## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import ResponseMetadataTypeDef


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

## AddCommunicationToCaseRequestTypeDef

```python
# AddCommunicationToCaseRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import AddCommunicationToCaseRequestTypeDef


def get_value() -> AddCommunicationToCaseRequestTypeDef:
    return {
        "communicationBody": ...,
    }


# AddCommunicationToCaseRequestTypeDef definition

class AddCommunicationToCaseRequestTypeDef(TypedDict):
    communicationBody: str,
    caseId: NotRequired[str],
    ccEmailAddresses: NotRequired[Sequence[str]],
    attachmentSetId: NotRequired[str],
```

## AttachmentDetailsTypeDef

```python
# AttachmentDetailsTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import AttachmentDetailsTypeDef


def get_value() -> AttachmentDetailsTypeDef:
    return {
        "attachmentId": ...,
    }


# AttachmentDetailsTypeDef definition

class AttachmentDetailsTypeDef(TypedDict):
    attachmentId: NotRequired[str],
    fileName: NotRequired[str],
```

## AttachmentOutputTypeDef

```python
# AttachmentOutputTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import AttachmentOutputTypeDef


def get_value() -> AttachmentOutputTypeDef:
    return {
        "fileName": ...,
    }


# AttachmentOutputTypeDef definition

class AttachmentOutputTypeDef(TypedDict):
    fileName: NotRequired[str],
    data: NotRequired[bytes],
```

## CategoryTypeDef

```python
# CategoryTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import CategoryTypeDef


def get_value() -> CategoryTypeDef:
    return {
        "code": ...,
    }


# CategoryTypeDef definition

class CategoryTypeDef(TypedDict):
    code: NotRequired[str],
    name: NotRequired[str],
```

## DateIntervalTypeDef

```python
# DateIntervalTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DateIntervalTypeDef


def get_value() -> DateIntervalTypeDef:
    return {
        "startDateTime": ...,
    }


# DateIntervalTypeDef definition

class DateIntervalTypeDef(TypedDict):
    startDateTime: NotRequired[str],
    endDateTime: NotRequired[str],
```

## SupportedHourTypeDef

```python
# SupportedHourTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import SupportedHourTypeDef


def get_value() -> SupportedHourTypeDef:
    return {
        "startTime": ...,
    }


# SupportedHourTypeDef definition

class SupportedHourTypeDef(TypedDict):
    startTime: NotRequired[str],
    endTime: NotRequired[str],
```

## CreateCaseRequestTypeDef

```python
# CreateCaseRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import CreateCaseRequestTypeDef


def get_value() -> CreateCaseRequestTypeDef:
    return {
        "subject": ...,
    }


# CreateCaseRequestTypeDef definition

class CreateCaseRequestTypeDef(TypedDict):
    subject: str,
    communicationBody: str,
    serviceCode: NotRequired[str],
    severityCode: NotRequired[str],
    categoryCode: NotRequired[str],
    ccEmailAddresses: NotRequired[Sequence[str]],
    language: NotRequired[str],
    issueType: NotRequired[str],
    attachmentSetId: NotRequired[str],
```

## DescribeAttachmentRequestTypeDef

```python
# DescribeAttachmentRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeAttachmentRequestTypeDef


def get_value() -> DescribeAttachmentRequestTypeDef:
    return {
        "attachmentId": ...,
    }


# DescribeAttachmentRequestTypeDef definition

class DescribeAttachmentRequestTypeDef(TypedDict):
    attachmentId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import PaginatorConfigTypeDef


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

## DescribeCasesRequestTypeDef

```python
# DescribeCasesRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeCasesRequestTypeDef


def get_value() -> DescribeCasesRequestTypeDef:
    return {
        "caseIdList": ...,
    }


# DescribeCasesRequestTypeDef definition

class DescribeCasesRequestTypeDef(TypedDict):
    caseIdList: NotRequired[Sequence[str]],
    displayId: NotRequired[str],
    afterTime: NotRequired[str],
    beforeTime: NotRequired[str],
    includeResolvedCases: NotRequired[bool],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    language: NotRequired[str],
    includeCommunications: NotRequired[bool],
```

## DescribeCommunicationsRequestTypeDef

```python
# DescribeCommunicationsRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeCommunicationsRequestTypeDef


def get_value() -> DescribeCommunicationsRequestTypeDef:
    return {
        "caseId": ...,
    }


# DescribeCommunicationsRequestTypeDef definition

class DescribeCommunicationsRequestTypeDef(TypedDict):
    caseId: str,
    beforeTime: NotRequired[str],
    afterTime: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## DescribeCreateCaseOptionsRequestTypeDef

```python
# DescribeCreateCaseOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeCreateCaseOptionsRequestTypeDef


def get_value() -> DescribeCreateCaseOptionsRequestTypeDef:
    return {
        "issueType": ...,
    }


# DescribeCreateCaseOptionsRequestTypeDef definition

class DescribeCreateCaseOptionsRequestTypeDef(TypedDict):
    issueType: str,
    serviceCode: str,
    language: str,
    categoryCode: str,
```

## DescribeServicesRequestTypeDef

```python
# DescribeServicesRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeServicesRequestTypeDef


def get_value() -> DescribeServicesRequestTypeDef:
    return {
        "serviceCodeList": ...,
    }


# DescribeServicesRequestTypeDef definition

class DescribeServicesRequestTypeDef(TypedDict):
    serviceCodeList: NotRequired[Sequence[str]],
    language: NotRequired[str],
```

## DescribeSeverityLevelsRequestTypeDef

```python
# DescribeSeverityLevelsRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeSeverityLevelsRequestTypeDef


def get_value() -> DescribeSeverityLevelsRequestTypeDef:
    return {
        "language": ...,
    }


# DescribeSeverityLevelsRequestTypeDef definition

class DescribeSeverityLevelsRequestTypeDef(TypedDict):
    language: NotRequired[str],
```

## SeverityLevelTypeDef

```python
# SeverityLevelTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import SeverityLevelTypeDef


def get_value() -> SeverityLevelTypeDef:
    return {
        "code": ...,
    }


# SeverityLevelTypeDef definition

class SeverityLevelTypeDef(TypedDict):
    code: NotRequired[str],
    name: NotRequired[str],
```

## DescribeSupportedLanguagesRequestTypeDef

```python
# DescribeSupportedLanguagesRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeSupportedLanguagesRequestTypeDef


def get_value() -> DescribeSupportedLanguagesRequestTypeDef:
    return {
        "issueType": ...,
    }


# DescribeSupportedLanguagesRequestTypeDef definition

class DescribeSupportedLanguagesRequestTypeDef(TypedDict):
    issueType: str,
    serviceCode: str,
    categoryCode: str,
```

## SupportedLanguageTypeDef

```python
# SupportedLanguageTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import SupportedLanguageTypeDef


def get_value() -> SupportedLanguageTypeDef:
    return {
        "code": ...,
    }


# SupportedLanguageTypeDef definition

class SupportedLanguageTypeDef(TypedDict):
    code: NotRequired[str],
    language: NotRequired[str],
    display: NotRequired[str],
```

## DescribeTrustedAdvisorCheckRefreshStatusesRequestTypeDef

```python
# DescribeTrustedAdvisorCheckRefreshStatusesRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeTrustedAdvisorCheckRefreshStatusesRequestTypeDef


def get_value() -> DescribeTrustedAdvisorCheckRefreshStatusesRequestTypeDef:
    return {
        "checkIds": ...,
    }


# DescribeTrustedAdvisorCheckRefreshStatusesRequestTypeDef definition

class DescribeTrustedAdvisorCheckRefreshStatusesRequestTypeDef(TypedDict):
    checkIds: Sequence[str],
```

## TrustedAdvisorCheckRefreshStatusTypeDef

```python
# TrustedAdvisorCheckRefreshStatusTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import TrustedAdvisorCheckRefreshStatusTypeDef


def get_value() -> TrustedAdvisorCheckRefreshStatusTypeDef:
    return {
        "checkId": ...,
    }


# TrustedAdvisorCheckRefreshStatusTypeDef definition

class TrustedAdvisorCheckRefreshStatusTypeDef(TypedDict):
    checkId: str,
    status: str,
    millisUntilNextRefreshable: int,
```

## DescribeTrustedAdvisorCheckResultRequestTypeDef

```python
# DescribeTrustedAdvisorCheckResultRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeTrustedAdvisorCheckResultRequestTypeDef


def get_value() -> DescribeTrustedAdvisorCheckResultRequestTypeDef:
    return {
        "checkId": ...,
    }


# DescribeTrustedAdvisorCheckResultRequestTypeDef definition

class DescribeTrustedAdvisorCheckResultRequestTypeDef(TypedDict):
    checkId: str,
    language: NotRequired[str],
```

## DescribeTrustedAdvisorCheckSummariesRequestTypeDef

```python
# DescribeTrustedAdvisorCheckSummariesRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeTrustedAdvisorCheckSummariesRequestTypeDef


def get_value() -> DescribeTrustedAdvisorCheckSummariesRequestTypeDef:
    return {
        "checkIds": ...,
    }


# DescribeTrustedAdvisorCheckSummariesRequestTypeDef definition

class DescribeTrustedAdvisorCheckSummariesRequestTypeDef(TypedDict):
    checkIds: Sequence[str],
```

## DescribeTrustedAdvisorChecksRequestTypeDef

```python
# DescribeTrustedAdvisorChecksRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeTrustedAdvisorChecksRequestTypeDef


def get_value() -> DescribeTrustedAdvisorChecksRequestTypeDef:
    return {
        "language": ...,
    }


# DescribeTrustedAdvisorChecksRequestTypeDef definition

class DescribeTrustedAdvisorChecksRequestTypeDef(TypedDict):
    language: str,
```

## TrustedAdvisorCheckDescriptionTypeDef

```python
# TrustedAdvisorCheckDescriptionTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import TrustedAdvisorCheckDescriptionTypeDef


def get_value() -> TrustedAdvisorCheckDescriptionTypeDef:
    return {
        "id": ...,
    }


# TrustedAdvisorCheckDescriptionTypeDef definition

class TrustedAdvisorCheckDescriptionTypeDef(TypedDict):
    id: str,
    name: str,
    description: str,
    category: str,
    metadata: List[str],
```

## RefreshTrustedAdvisorCheckRequestTypeDef

```python
# RefreshTrustedAdvisorCheckRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import RefreshTrustedAdvisorCheckRequestTypeDef


def get_value() -> RefreshTrustedAdvisorCheckRequestTypeDef:
    return {
        "checkId": ...,
    }


# RefreshTrustedAdvisorCheckRequestTypeDef definition

class RefreshTrustedAdvisorCheckRequestTypeDef(TypedDict):
    checkId: str,
```

## ResolveCaseRequestTypeDef

```python
# ResolveCaseRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import ResolveCaseRequestTypeDef


def get_value() -> ResolveCaseRequestTypeDef:
    return {
        "caseId": ...,
    }


# ResolveCaseRequestTypeDef definition

class ResolveCaseRequestTypeDef(TypedDict):
    caseId: NotRequired[str],
```

## TrustedAdvisorCostOptimizingSummaryTypeDef

```python
# TrustedAdvisorCostOptimizingSummaryTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import TrustedAdvisorCostOptimizingSummaryTypeDef


def get_value() -> TrustedAdvisorCostOptimizingSummaryTypeDef:
    return {
        "estimatedMonthlySavings": ...,
    }


# TrustedAdvisorCostOptimizingSummaryTypeDef definition

class TrustedAdvisorCostOptimizingSummaryTypeDef(TypedDict):
    estimatedMonthlySavings: float,
    estimatedPercentMonthlySavings: float,
```

## TrustedAdvisorResourceDetailTypeDef

```python
# TrustedAdvisorResourceDetailTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import TrustedAdvisorResourceDetailTypeDef


def get_value() -> TrustedAdvisorResourceDetailTypeDef:
    return {
        "status": ...,
    }


# TrustedAdvisorResourceDetailTypeDef definition

class TrustedAdvisorResourceDetailTypeDef(TypedDict):
    status: str,
    resourceId: str,
    metadata: List[str],
    region: NotRequired[str],
    isSuppressed: NotRequired[bool],
```

## TrustedAdvisorResourcesSummaryTypeDef

```python
# TrustedAdvisorResourcesSummaryTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import TrustedAdvisorResourcesSummaryTypeDef


def get_value() -> TrustedAdvisorResourcesSummaryTypeDef:
    return {
        "resourcesProcessed": ...,
    }


# TrustedAdvisorResourcesSummaryTypeDef definition

class TrustedAdvisorResourcesSummaryTypeDef(TypedDict):
    resourcesProcessed: int,
    resourcesFlagged: int,
    resourcesIgnored: int,
    resourcesSuppressed: int,
```

## AddAttachmentsToSetResponseTypeDef

```python
# AddAttachmentsToSetResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import AddAttachmentsToSetResponseTypeDef


def get_value() -> AddAttachmentsToSetResponseTypeDef:
    return {
        "attachmentSetId": ...,
    }


# AddAttachmentsToSetResponseTypeDef definition

class AddAttachmentsToSetResponseTypeDef(TypedDict):
    attachmentSetId: str,
    expiryTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddCommunicationToCaseResponseTypeDef

```python
# AddCommunicationToCaseResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import AddCommunicationToCaseResponseTypeDef


def get_value() -> AddCommunicationToCaseResponseTypeDef:
    return {
        "result": ...,
    }


# AddCommunicationToCaseResponseTypeDef definition

class AddCommunicationToCaseResponseTypeDef(TypedDict):
    result: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCaseResponseTypeDef

```python
# CreateCaseResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import CreateCaseResponseTypeDef


def get_value() -> CreateCaseResponseTypeDef:
    return {
        "caseId": ...,
    }


# CreateCaseResponseTypeDef definition

class CreateCaseResponseTypeDef(TypedDict):
    caseId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResolveCaseResponseTypeDef

```python
# ResolveCaseResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import ResolveCaseResponseTypeDef


def get_value() -> ResolveCaseResponseTypeDef:
    return {
        "initialCaseStatus": ...,
    }


# ResolveCaseResponseTypeDef definition

class ResolveCaseResponseTypeDef(TypedDict):
    initialCaseStatus: str,
    finalCaseStatus: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CommunicationTypeDef

```python
# CommunicationTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import CommunicationTypeDef


def get_value() -> CommunicationTypeDef:
    return {
        "caseId": ...,
    }


# CommunicationTypeDef definition

class CommunicationTypeDef(TypedDict):
    caseId: NotRequired[str],
    body: NotRequired[str],
    submittedBy: NotRequired[str],
    timeCreated: NotRequired[str],
    attachmentSet: NotRequired[List[AttachmentDetailsTypeDef]],  # (1)
```

1. See [:material-code-braces: AttachmentDetailsTypeDef](./type_defs.md#attachmentdetailstypedef) 
## DescribeAttachmentResponseTypeDef

```python
# DescribeAttachmentResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeAttachmentResponseTypeDef


def get_value() -> DescribeAttachmentResponseTypeDef:
    return {
        "attachment": ...,
    }


# DescribeAttachmentResponseTypeDef definition

class DescribeAttachmentResponseTypeDef(TypedDict):
    attachment: AttachmentOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttachmentTypeDef

```python
# AttachmentTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import AttachmentTypeDef


def get_value() -> AttachmentTypeDef:
    return {
        "fileName": ...,
    }


# AttachmentTypeDef definition

class AttachmentTypeDef(TypedDict):
    fileName: NotRequired[str],
    data: NotRequired[BlobTypeDef],
```

## ServiceTypeDef

```python
# ServiceTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import ServiceTypeDef


def get_value() -> ServiceTypeDef:
    return {
        "code": ...,
    }


# ServiceTypeDef definition

class ServiceTypeDef(TypedDict):
    code: NotRequired[str],
    name: NotRequired[str],
    categories: NotRequired[List[CategoryTypeDef]],  # (1)
```

1. See [:material-code-braces: CategoryTypeDef](./type_defs.md#categorytypedef) 
## CommunicationTypeOptionsTypeDef

```python
# CommunicationTypeOptionsTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import CommunicationTypeOptionsTypeDef


def get_value() -> CommunicationTypeOptionsTypeDef:
    return {
        "type": ...,
    }


# CommunicationTypeOptionsTypeDef definition

class CommunicationTypeOptionsTypeDef(TypedDict):
    type: NotRequired[str],
    supportedHours: NotRequired[List[SupportedHourTypeDef]],  # (1)
    datesWithoutSupport: NotRequired[List[DateIntervalTypeDef]],  # (2)
```

1. See [:material-code-braces: SupportedHourTypeDef](./type_defs.md#supportedhourtypedef) 
2. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef) 
## DescribeCasesRequestPaginateTypeDef

```python
# DescribeCasesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeCasesRequestPaginateTypeDef


def get_value() -> DescribeCasesRequestPaginateTypeDef:
    return {
        "caseIdList": ...,
    }


# DescribeCasesRequestPaginateTypeDef definition

class DescribeCasesRequestPaginateTypeDef(TypedDict):
    caseIdList: NotRequired[Sequence[str]],
    displayId: NotRequired[str],
    afterTime: NotRequired[str],
    beforeTime: NotRequired[str],
    includeResolvedCases: NotRequired[bool],
    language: NotRequired[str],
    includeCommunications: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeCommunicationsRequestPaginateTypeDef

```python
# DescribeCommunicationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeCommunicationsRequestPaginateTypeDef


def get_value() -> DescribeCommunicationsRequestPaginateTypeDef:
    return {
        "caseId": ...,
    }


# DescribeCommunicationsRequestPaginateTypeDef definition

class DescribeCommunicationsRequestPaginateTypeDef(TypedDict):
    caseId: str,
    beforeTime: NotRequired[str],
    afterTime: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSeverityLevelsResponseTypeDef

```python
# DescribeSeverityLevelsResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeSeverityLevelsResponseTypeDef


def get_value() -> DescribeSeverityLevelsResponseTypeDef:
    return {
        "severityLevels": ...,
    }


# DescribeSeverityLevelsResponseTypeDef definition

class DescribeSeverityLevelsResponseTypeDef(TypedDict):
    severityLevels: List[SeverityLevelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SeverityLevelTypeDef](./type_defs.md#severityleveltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSupportedLanguagesResponseTypeDef

```python
# DescribeSupportedLanguagesResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeSupportedLanguagesResponseTypeDef


def get_value() -> DescribeSupportedLanguagesResponseTypeDef:
    return {
        "supportedLanguages": ...,
    }


# DescribeSupportedLanguagesResponseTypeDef definition

class DescribeSupportedLanguagesResponseTypeDef(TypedDict):
    supportedLanguages: List[SupportedLanguageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SupportedLanguageTypeDef](./type_defs.md#supportedlanguagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef

```python
# DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef


def get_value() -> DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef:
    return {
        "statuses": ...,
    }


# DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef definition

class DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef(TypedDict):
    statuses: List[TrustedAdvisorCheckRefreshStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustedAdvisorCheckRefreshStatusTypeDef](./type_defs.md#trustedadvisorcheckrefreshstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RefreshTrustedAdvisorCheckResponseTypeDef

```python
# RefreshTrustedAdvisorCheckResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import RefreshTrustedAdvisorCheckResponseTypeDef


def get_value() -> RefreshTrustedAdvisorCheckResponseTypeDef:
    return {
        "status": ...,
    }


# RefreshTrustedAdvisorCheckResponseTypeDef definition

class RefreshTrustedAdvisorCheckResponseTypeDef(TypedDict):
    status: TrustedAdvisorCheckRefreshStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustedAdvisorCheckRefreshStatusTypeDef](./type_defs.md#trustedadvisorcheckrefreshstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrustedAdvisorChecksResponseTypeDef

```python
# DescribeTrustedAdvisorChecksResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeTrustedAdvisorChecksResponseTypeDef


def get_value() -> DescribeTrustedAdvisorChecksResponseTypeDef:
    return {
        "checks": ...,
    }


# DescribeTrustedAdvisorChecksResponseTypeDef definition

class DescribeTrustedAdvisorChecksResponseTypeDef(TypedDict):
    checks: List[TrustedAdvisorCheckDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustedAdvisorCheckDescriptionTypeDef](./type_defs.md#trustedadvisorcheckdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrustedAdvisorCategorySpecificSummaryTypeDef

```python
# TrustedAdvisorCategorySpecificSummaryTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import TrustedAdvisorCategorySpecificSummaryTypeDef


def get_value() -> TrustedAdvisorCategorySpecificSummaryTypeDef:
    return {
        "costOptimizing": ...,
    }


# TrustedAdvisorCategorySpecificSummaryTypeDef definition

class TrustedAdvisorCategorySpecificSummaryTypeDef(TypedDict):
    costOptimizing: NotRequired[TrustedAdvisorCostOptimizingSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: TrustedAdvisorCostOptimizingSummaryTypeDef](./type_defs.md#trustedadvisorcostoptimizingsummarytypedef) 
## DescribeCommunicationsResponseTypeDef

```python
# DescribeCommunicationsResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeCommunicationsResponseTypeDef


def get_value() -> DescribeCommunicationsResponseTypeDef:
    return {
        "communications": ...,
    }


# DescribeCommunicationsResponseTypeDef definition

class DescribeCommunicationsResponseTypeDef(TypedDict):
    communications: List[CommunicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CommunicationTypeDef](./type_defs.md#communicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecentCaseCommunicationsTypeDef

```python
# RecentCaseCommunicationsTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import RecentCaseCommunicationsTypeDef


def get_value() -> RecentCaseCommunicationsTypeDef:
    return {
        "communications": ...,
    }


# RecentCaseCommunicationsTypeDef definition

class RecentCaseCommunicationsTypeDef(TypedDict):
    communications: NotRequired[List[CommunicationTypeDef]],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CommunicationTypeDef](./type_defs.md#communicationtypedef) 
## DescribeServicesResponseTypeDef

```python
# DescribeServicesResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeServicesResponseTypeDef


def get_value() -> DescribeServicesResponseTypeDef:
    return {
        "services": ...,
    }


# DescribeServicesResponseTypeDef definition

class DescribeServicesResponseTypeDef(TypedDict):
    services: List[ServiceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCreateCaseOptionsResponseTypeDef

```python
# DescribeCreateCaseOptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeCreateCaseOptionsResponseTypeDef


def get_value() -> DescribeCreateCaseOptionsResponseTypeDef:
    return {
        "languageAvailability": ...,
    }


# DescribeCreateCaseOptionsResponseTypeDef definition

class DescribeCreateCaseOptionsResponseTypeDef(TypedDict):
    languageAvailability: str,
    communicationTypes: List[CommunicationTypeOptionsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommunicationTypeOptionsTypeDef](./type_defs.md#communicationtypeoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrustedAdvisorCheckResultTypeDef

```python
# TrustedAdvisorCheckResultTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import TrustedAdvisorCheckResultTypeDef


def get_value() -> TrustedAdvisorCheckResultTypeDef:
    return {
        "checkId": ...,
    }


# TrustedAdvisorCheckResultTypeDef definition

class TrustedAdvisorCheckResultTypeDef(TypedDict):
    checkId: str,
    timestamp: str,
    status: str,
    resourcesSummary: TrustedAdvisorResourcesSummaryTypeDef,  # (1)
    categorySpecificSummary: TrustedAdvisorCategorySpecificSummaryTypeDef,  # (2)
    flaggedResources: List[TrustedAdvisorResourceDetailTypeDef],  # (3)
```

1. See [:material-code-braces: TrustedAdvisorResourcesSummaryTypeDef](./type_defs.md#trustedadvisorresourcessummarytypedef) 
2. See [:material-code-braces: TrustedAdvisorCategorySpecificSummaryTypeDef](./type_defs.md#trustedadvisorcategoryspecificsummarytypedef) 
3. See [:material-code-braces: TrustedAdvisorResourceDetailTypeDef](./type_defs.md#trustedadvisorresourcedetailtypedef) 
## TrustedAdvisorCheckSummaryTypeDef

```python
# TrustedAdvisorCheckSummaryTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import TrustedAdvisorCheckSummaryTypeDef


def get_value() -> TrustedAdvisorCheckSummaryTypeDef:
    return {
        "checkId": ...,
    }


# TrustedAdvisorCheckSummaryTypeDef definition

class TrustedAdvisorCheckSummaryTypeDef(TypedDict):
    checkId: str,
    timestamp: str,
    status: str,
    resourcesSummary: TrustedAdvisorResourcesSummaryTypeDef,  # (1)
    categorySpecificSummary: TrustedAdvisorCategorySpecificSummaryTypeDef,  # (2)
    hasFlaggedResources: NotRequired[bool],
```

1. See [:material-code-braces: TrustedAdvisorResourcesSummaryTypeDef](./type_defs.md#trustedadvisorresourcessummarytypedef) 
2. See [:material-code-braces: TrustedAdvisorCategorySpecificSummaryTypeDef](./type_defs.md#trustedadvisorcategoryspecificsummarytypedef) 
## CaseDetailsTypeDef

```python
# CaseDetailsTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import CaseDetailsTypeDef


def get_value() -> CaseDetailsTypeDef:
    return {
        "caseId": ...,
    }


# CaseDetailsTypeDef definition

class CaseDetailsTypeDef(TypedDict):
    caseId: NotRequired[str],
    displayId: NotRequired[str],
    subject: NotRequired[str],
    status: NotRequired[str],
    serviceCode: NotRequired[str],
    categoryCode: NotRequired[str],
    severityCode: NotRequired[str],
    submittedBy: NotRequired[str],
    timeCreated: NotRequired[str],
    recentCommunications: NotRequired[RecentCaseCommunicationsTypeDef],  # (1)
    ccEmailAddresses: NotRequired[List[str]],
    language: NotRequired[str],
```

1. See [:material-code-braces: RecentCaseCommunicationsTypeDef](./type_defs.md#recentcasecommunicationstypedef) 
## AddAttachmentsToSetRequestTypeDef

```python
# AddAttachmentsToSetRequestTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import AddAttachmentsToSetRequestTypeDef


def get_value() -> AddAttachmentsToSetRequestTypeDef:
    return {
        "attachments": ...,
    }


# AddAttachmentsToSetRequestTypeDef definition

class AddAttachmentsToSetRequestTypeDef(TypedDict):
    attachments: Sequence[AttachmentUnionTypeDef],  # (1)
    attachmentSetId: NotRequired[str],
```

1. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) [:material-code-braces: AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef) 
## DescribeTrustedAdvisorCheckResultResponseTypeDef

```python
# DescribeTrustedAdvisorCheckResultResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeTrustedAdvisorCheckResultResponseTypeDef


def get_value() -> DescribeTrustedAdvisorCheckResultResponseTypeDef:
    return {
        "result": ...,
    }


# DescribeTrustedAdvisorCheckResultResponseTypeDef definition

class DescribeTrustedAdvisorCheckResultResponseTypeDef(TypedDict):
    result: TrustedAdvisorCheckResultTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustedAdvisorCheckResultTypeDef](./type_defs.md#trustedadvisorcheckresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrustedAdvisorCheckSummariesResponseTypeDef

```python
# DescribeTrustedAdvisorCheckSummariesResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeTrustedAdvisorCheckSummariesResponseTypeDef


def get_value() -> DescribeTrustedAdvisorCheckSummariesResponseTypeDef:
    return {
        "summaries": ...,
    }


# DescribeTrustedAdvisorCheckSummariesResponseTypeDef definition

class DescribeTrustedAdvisorCheckSummariesResponseTypeDef(TypedDict):
    summaries: List[TrustedAdvisorCheckSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrustedAdvisorCheckSummaryTypeDef](./type_defs.md#trustedadvisorchecksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCasesResponseTypeDef

```python
# DescribeCasesResponseTypeDef TypedDict usage example

from types_aiobotocore_support.type_defs import DescribeCasesResponseTypeDef


def get_value() -> DescribeCasesResponseTypeDef:
    return {
        "cases": ...,
    }


# DescribeCasesResponseTypeDef definition

class DescribeCasesResponseTypeDef(TypedDict):
    cases: List[CaseDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CaseDetailsTypeDef](./type_defs.md#casedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
