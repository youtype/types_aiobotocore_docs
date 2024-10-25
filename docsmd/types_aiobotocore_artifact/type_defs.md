# Type definitions

> [Index](../README.md) > [Artifact](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
    type annotations stubs module [types-aiobotocore-artifact](https://pypi.org/project/types-aiobotocore-artifact/).



## AccountSettingsTypeDef

```python
# AccountSettingsTypeDef definition

class AccountSettingsTypeDef(TypedDict):
    notificationSubscriptionStatus: NotRequired[NotificationSubscriptionStatusType],  # (1)
```

1. See [:material-code-brackets: NotificationSubscriptionStatusType](./literals.md#notificationsubscriptionstatustype) 
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

## GetReportMetadataRequestRequestTypeDef

```python
# GetReportMetadataRequestRequestTypeDef definition

class GetReportMetadataRequestRequestTypeDef(TypedDict):
    reportId: str,
    reportVersion: NotRequired[int],
```

## ReportDetailTypeDef

```python
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
## GetReportRequestRequestTypeDef

```python
# GetReportRequestRequestTypeDef definition

class GetReportRequestRequestTypeDef(TypedDict):
    reportId: str,
    termToken: str,
    reportVersion: NotRequired[int],
```

## GetTermForReportRequestRequestTypeDef

```python
# GetTermForReportRequestRequestTypeDef definition

class GetTermForReportRequestRequestTypeDef(TypedDict):
    reportId: str,
    reportVersion: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListReportsRequestRequestTypeDef

```python
# ListReportsRequestRequestTypeDef definition

class ListReportsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ReportSummaryTypeDef

```python
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
## PutAccountSettingsRequestRequestTypeDef

```python
# PutAccountSettingsRequestRequestTypeDef definition

class PutAccountSettingsRequestRequestTypeDef(TypedDict):
    notificationSubscriptionStatus: NotRequired[NotificationSubscriptionStatusType],  # (1)
```

1. See [:material-code-brackets: NotificationSubscriptionStatusType](./literals.md#notificationsubscriptionstatustype) 
## GetAccountSettingsResponseTypeDef

```python
# GetAccountSettingsResponseTypeDef definition

class GetAccountSettingsResponseTypeDef(TypedDict):
    accountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReportResponseTypeDef

```python
# GetReportResponseTypeDef definition

class GetReportResponseTypeDef(TypedDict):
    documentPresignedUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTermForReportResponseTypeDef

```python
# GetTermForReportResponseTypeDef definition

class GetTermForReportResponseTypeDef(TypedDict):
    documentPresignedUrl: str,
    termToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAccountSettingsResponseTypeDef

```python
# PutAccountSettingsResponseTypeDef definition

class PutAccountSettingsResponseTypeDef(TypedDict):
    accountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReportMetadataResponseTypeDef

```python
# GetReportMetadataResponseTypeDef definition

class GetReportMetadataResponseTypeDef(TypedDict):
    reportDetails: ReportDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportDetailTypeDef](./type_defs.md#reportdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReportsRequestListReportsPaginateTypeDef

```python
# ListReportsRequestListReportsPaginateTypeDef definition

class ListReportsRequestListReportsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReportsResponseTypeDef

```python
# ListReportsResponseTypeDef definition

class ListReportsResponseTypeDef(TypedDict):
    reports: List[ReportSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReportSummaryTypeDef](./type_defs.md#reportsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
