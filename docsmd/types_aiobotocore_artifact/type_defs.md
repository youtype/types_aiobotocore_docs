# Type definitions

> [Index](../README.md) > [Artifact](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#artifact)
    type annotations stubs module [types-aiobotocore-artifact](https://pypi.org/project/types-aiobotocore-artifact/).



## AccountSettingsTypeDef

```python
# AccountSettingsTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import AccountSettingsTypeDef


def get_value() -> AccountSettingsTypeDef:
    return {
        "notificationSubscriptionStatus": ...,
    }


# AccountSettingsTypeDef definition

class AccountSettingsTypeDef(TypedDict):
    notificationSubscriptionStatus: NotRequired[NotificationSubscriptionStatusType],  # (1)
```

1. See [:material-code-brackets: NotificationSubscriptionStatusType](./literals.md#notificationsubscriptionstatustype) 
## CustomerAgreementSummaryTypeDef

```python
# CustomerAgreementSummaryTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import CustomerAgreementSummaryTypeDef


def get_value() -> CustomerAgreementSummaryTypeDef:
    return {
        "name": ...,
    }


# CustomerAgreementSummaryTypeDef definition

class CustomerAgreementSummaryTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    id: NotRequired[str],
    agreementArn: NotRequired[str],
    awsAccountId: NotRequired[str],
    organizationArn: NotRequired[str],
    effectiveStart: NotRequired[datetime],
    effectiveEnd: NotRequired[datetime],
    state: NotRequired[CustomerAgreementStateType],  # (1)
    description: NotRequired[str],
    acceptanceTerms: NotRequired[List[str]],
    terminateTerms: NotRequired[List[str]],
    type: NotRequired[AgreementTypeType],  # (2)
```

1. See [:material-code-brackets: CustomerAgreementStateType](./literals.md#customeragreementstatetype) 
2. See [:material-code-brackets: AgreementTypeType](./literals.md#agreementtypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import ResponseMetadataTypeDef


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

## GetReportMetadataRequestTypeDef

```python
# GetReportMetadataRequestTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import GetReportMetadataRequestTypeDef


def get_value() -> GetReportMetadataRequestTypeDef:
    return {
        "reportId": ...,
    }


# GetReportMetadataRequestTypeDef definition

class GetReportMetadataRequestTypeDef(TypedDict):
    reportId: str,
    reportVersion: NotRequired[int],
```

## ReportDetailTypeDef

```python
# ReportDetailTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import ReportDetailTypeDef


def get_value() -> ReportDetailTypeDef:
    return {
        "id": ...,
    }


# ReportDetailTypeDef definition

class ReportDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    periodStart: NotRequired[datetime],
    periodEnd: NotRequired[datetime],
    createdAt: NotRequired[datetime],
    lastModifiedAt: NotRequired[datetime],
    deletedAt: NotRequired[datetime],
    state: NotRequired[PublishedStateType],  # (1)
    arn: NotRequired[str],
    series: NotRequired[str],
    category: NotRequired[str],
    companyName: NotRequired[str],
    productName: NotRequired[str],
    termArn: NotRequired[str],
    version: NotRequired[int],
    acceptanceType: NotRequired[AcceptanceTypeType],  # (2)
    sequenceNumber: NotRequired[int],
    uploadState: NotRequired[UploadStateType],  # (3)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: PublishedStateType](./literals.md#publishedstatetype) 
2. See [:material-code-brackets: AcceptanceTypeType](./literals.md#acceptancetypetype) 
3. See [:material-code-brackets: UploadStateType](./literals.md#uploadstatetype) 
## GetReportRequestTypeDef

```python
# GetReportRequestTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import GetReportRequestTypeDef


def get_value() -> GetReportRequestTypeDef:
    return {
        "reportId": ...,
    }


# GetReportRequestTypeDef definition

class GetReportRequestTypeDef(TypedDict):
    reportId: str,
    termToken: str,
    reportVersion: NotRequired[int],
```

## GetTermForReportRequestTypeDef

```python
# GetTermForReportRequestTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import GetTermForReportRequestTypeDef


def get_value() -> GetTermForReportRequestTypeDef:
    return {
        "reportId": ...,
    }


# GetTermForReportRequestTypeDef definition

class GetTermForReportRequestTypeDef(TypedDict):
    reportId: str,
    reportVersion: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import PaginatorConfigTypeDef


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

## ListCustomerAgreementsRequestTypeDef

```python
# ListCustomerAgreementsRequestTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import ListCustomerAgreementsRequestTypeDef


def get_value() -> ListCustomerAgreementsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListCustomerAgreementsRequestTypeDef definition

class ListCustomerAgreementsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListReportsRequestTypeDef

```python
# ListReportsRequestTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import ListReportsRequestTypeDef


def get_value() -> ListReportsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListReportsRequestTypeDef definition

class ListReportsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ReportSummaryTypeDef

```python
# ReportSummaryTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import ReportSummaryTypeDef


def get_value() -> ReportSummaryTypeDef:
    return {
        "id": ...,
    }


# ReportSummaryTypeDef definition

class ReportSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    state: NotRequired[PublishedStateType],  # (1)
    arn: NotRequired[str],
    version: NotRequired[int],
    uploadState: NotRequired[UploadStateType],  # (2)
    description: NotRequired[str],
    periodStart: NotRequired[datetime],
    periodEnd: NotRequired[datetime],
    series: NotRequired[str],
    category: NotRequired[str],
    companyName: NotRequired[str],
    productName: NotRequired[str],
    statusMessage: NotRequired[str],
    acceptanceType: NotRequired[AcceptanceTypeType],  # (3)
```

1. See [:material-code-brackets: PublishedStateType](./literals.md#publishedstatetype) 
2. See [:material-code-brackets: UploadStateType](./literals.md#uploadstatetype) 
3. See [:material-code-brackets: AcceptanceTypeType](./literals.md#acceptancetypetype) 
## PutAccountSettingsRequestTypeDef

```python
# PutAccountSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import PutAccountSettingsRequestTypeDef


def get_value() -> PutAccountSettingsRequestTypeDef:
    return {
        "notificationSubscriptionStatus": ...,
    }


# PutAccountSettingsRequestTypeDef definition

class PutAccountSettingsRequestTypeDef(TypedDict):
    notificationSubscriptionStatus: NotRequired[NotificationSubscriptionStatusType],  # (1)
```

1. See [:material-code-brackets: NotificationSubscriptionStatusType](./literals.md#notificationsubscriptionstatustype) 
## GetAccountSettingsResponseTypeDef

```python
# GetAccountSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import GetAccountSettingsResponseTypeDef


def get_value() -> GetAccountSettingsResponseTypeDef:
    return {
        "accountSettings": ...,
    }


# GetAccountSettingsResponseTypeDef definition

class GetAccountSettingsResponseTypeDef(TypedDict):
    accountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReportResponseTypeDef

```python
# GetReportResponseTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import GetReportResponseTypeDef


def get_value() -> GetReportResponseTypeDef:
    return {
        "documentPresignedUrl": ...,
    }


# GetReportResponseTypeDef definition

class GetReportResponseTypeDef(TypedDict):
    documentPresignedUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTermForReportResponseTypeDef

```python
# GetTermForReportResponseTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import GetTermForReportResponseTypeDef


def get_value() -> GetTermForReportResponseTypeDef:
    return {
        "documentPresignedUrl": ...,
    }


# GetTermForReportResponseTypeDef definition

class GetTermForReportResponseTypeDef(TypedDict):
    documentPresignedUrl: str,
    termToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomerAgreementsResponseTypeDef

```python
# ListCustomerAgreementsResponseTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import ListCustomerAgreementsResponseTypeDef


def get_value() -> ListCustomerAgreementsResponseTypeDef:
    return {
        "customerAgreements": ...,
    }


# ListCustomerAgreementsResponseTypeDef definition

class ListCustomerAgreementsResponseTypeDef(TypedDict):
    customerAgreements: List[CustomerAgreementSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomerAgreementSummaryTypeDef](./type_defs.md#customeragreementsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAccountSettingsResponseTypeDef

```python
# PutAccountSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import PutAccountSettingsResponseTypeDef


def get_value() -> PutAccountSettingsResponseTypeDef:
    return {
        "accountSettings": ...,
    }


# PutAccountSettingsResponseTypeDef definition

class PutAccountSettingsResponseTypeDef(TypedDict):
    accountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReportMetadataResponseTypeDef

```python
# GetReportMetadataResponseTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import GetReportMetadataResponseTypeDef


def get_value() -> GetReportMetadataResponseTypeDef:
    return {
        "reportDetails": ...,
    }


# GetReportMetadataResponseTypeDef definition

class GetReportMetadataResponseTypeDef(TypedDict):
    reportDetails: ReportDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportDetailTypeDef](./type_defs.md#reportdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomerAgreementsRequestPaginateTypeDef

```python
# ListCustomerAgreementsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import ListCustomerAgreementsRequestPaginateTypeDef


def get_value() -> ListCustomerAgreementsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListCustomerAgreementsRequestPaginateTypeDef definition

class ListCustomerAgreementsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReportsRequestPaginateTypeDef

```python
# ListReportsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import ListReportsRequestPaginateTypeDef


def get_value() -> ListReportsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListReportsRequestPaginateTypeDef definition

class ListReportsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReportsResponseTypeDef

```python
# ListReportsResponseTypeDef TypedDict usage example

from types_aiobotocore_artifact.type_defs import ListReportsResponseTypeDef


def get_value() -> ListReportsResponseTypeDef:
    return {
        "reports": ...,
    }


# ListReportsResponseTypeDef definition

class ListReportsResponseTypeDef(TypedDict):
    reports: List[ReportSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReportSummaryTypeDef](./type_defs.md#reportsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
