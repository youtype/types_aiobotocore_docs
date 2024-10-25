# Type definitions

> [Index](../README.md) > [AppFabric](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AppFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
    type annotations stubs module [types-aiobotocore-appfabric](https://pypi.org/project/types-aiobotocore-appfabric/).



## ApiKeyCredentialTypeDef

```python
# ApiKeyCredentialTypeDef definition

class ApiKeyCredentialTypeDef(TypedDict):
    apiKey: str,
```

## TenantTypeDef

```python
# TenantTypeDef definition

class TenantTypeDef(TypedDict):
    tenantIdentifier: str,
    tenantDisplayName: str,
```

## AppBundleSummaryTypeDef

```python
# AppBundleSummaryTypeDef definition

class AppBundleSummaryTypeDef(TypedDict):
    arn: str,
```

## AppBundleTypeDef

```python
# AppBundleTypeDef definition

class AppBundleTypeDef(TypedDict):
    arn: str,
    customerManagedKeyArn: NotRequired[str],
```

## AuditLogProcessingConfigurationTypeDef

```python
# AuditLogProcessingConfigurationTypeDef definition

class AuditLogProcessingConfigurationTypeDef(TypedDict):
    schema: SchemaType,  # (1)
    format: FormatType,  # (2)
```

1. See [:material-code-brackets: SchemaType](./literals.md#schematype) 
2. See [:material-code-brackets: FormatType](./literals.md#formattype) 
## AuthRequestTypeDef

```python
# AuthRequestTypeDef definition

class AuthRequestTypeDef(TypedDict):
    redirectUri: str,
    code: str,
```

## BatchGetUserAccessTasksRequestRequestTypeDef

```python
# BatchGetUserAccessTasksRequestRequestTypeDef definition

class BatchGetUserAccessTasksRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    taskIdList: Sequence[str],
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

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## IngestionTypeDef

```python
# IngestionTypeDef definition

class IngestionTypeDef(TypedDict):
    arn: str,
    appBundleArn: str,
    app: str,
    tenantId: str,
    createdAt: datetime,
    updatedAt: datetime,
    state: IngestionStateType,  # (1)
    ingestionType: IngestionTypeType,  # (2)
```

1. See [:material-code-brackets: IngestionStateType](./literals.md#ingestionstatetype) 
2. See [:material-code-brackets: IngestionTypeType](./literals.md#ingestiontypetype) 
## Oauth2CredentialTypeDef

```python
# Oauth2CredentialTypeDef definition

class Oauth2CredentialTypeDef(TypedDict):
    clientId: str,
    clientSecret: str,
```

## DeleteAppAuthorizationRequestRequestTypeDef

```python
# DeleteAppAuthorizationRequestRequestTypeDef definition

class DeleteAppAuthorizationRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    appAuthorizationIdentifier: str,
```

## DeleteAppBundleRequestRequestTypeDef

```python
# DeleteAppBundleRequestRequestTypeDef definition

class DeleteAppBundleRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
```

## DeleteIngestionDestinationRequestRequestTypeDef

```python
# DeleteIngestionDestinationRequestRequestTypeDef definition

class DeleteIngestionDestinationRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    ingestionDestinationIdentifier: str,
```

## DeleteIngestionRequestRequestTypeDef

```python
# DeleteIngestionRequestRequestTypeDef definition

class DeleteIngestionRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    ingestionIdentifier: str,
```

## FirehoseStreamTypeDef

```python
# FirehoseStreamTypeDef definition

class FirehoseStreamTypeDef(TypedDict):
    streamName: str,
```

## S3BucketTypeDef

```python
# S3BucketTypeDef definition

class S3BucketTypeDef(TypedDict):
    bucketName: str,
    prefix: NotRequired[str],
```

## GetAppAuthorizationRequestRequestTypeDef

```python
# GetAppAuthorizationRequestRequestTypeDef definition

class GetAppAuthorizationRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    appAuthorizationIdentifier: str,
```

## GetAppBundleRequestRequestTypeDef

```python
# GetAppBundleRequestRequestTypeDef definition

class GetAppBundleRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
```

## GetIngestionDestinationRequestRequestTypeDef

```python
# GetIngestionDestinationRequestRequestTypeDef definition

class GetIngestionDestinationRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    ingestionDestinationIdentifier: str,
```

## GetIngestionRequestRequestTypeDef

```python
# GetIngestionRequestRequestTypeDef definition

class GetIngestionRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    ingestionIdentifier: str,
```

## IngestionDestinationSummaryTypeDef

```python
# IngestionDestinationSummaryTypeDef definition

class IngestionDestinationSummaryTypeDef(TypedDict):
    arn: str,
```

## IngestionSummaryTypeDef

```python
# IngestionSummaryTypeDef definition

class IngestionSummaryTypeDef(TypedDict):
    arn: str,
    app: str,
    tenantId: str,
    state: IngestionStateType,  # (1)
```

1. See [:material-code-brackets: IngestionStateType](./literals.md#ingestionstatetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAppAuthorizationsRequestRequestTypeDef

```python
# ListAppAuthorizationsRequestRequestTypeDef definition

class ListAppAuthorizationsRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAppBundlesRequestRequestTypeDef

```python
# ListAppBundlesRequestRequestTypeDef definition

class ListAppBundlesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIngestionDestinationsRequestRequestTypeDef

```python
# ListIngestionDestinationsRequestRequestTypeDef definition

class ListIngestionDestinationsRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIngestionsRequestRequestTypeDef

```python
# ListIngestionsRequestRequestTypeDef definition

class ListIngestionsRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## StartIngestionRequestRequestTypeDef

```python
# StartIngestionRequestRequestTypeDef definition

class StartIngestionRequestRequestTypeDef(TypedDict):
    ingestionIdentifier: str,
    appBundleIdentifier: str,
```

## StartUserAccessTasksRequestRequestTypeDef

```python
# StartUserAccessTasksRequestRequestTypeDef definition

class StartUserAccessTasksRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    email: str,
```

## StopIngestionRequestRequestTypeDef

```python
# StopIngestionRequestRequestTypeDef definition

class StopIngestionRequestRequestTypeDef(TypedDict):
    ingestionIdentifier: str,
    appBundleIdentifier: str,
```

## TaskErrorTypeDef

```python
# TaskErrorTypeDef definition

class TaskErrorTypeDef(TypedDict):
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AppAuthorizationSummaryTypeDef

```python
# AppAuthorizationSummaryTypeDef definition

class AppAuthorizationSummaryTypeDef(TypedDict):
    appAuthorizationArn: str,
    appBundleArn: str,
    app: str,
    tenant: TenantTypeDef,  # (1)
    status: AppAuthorizationStatusType,  # (2)
    updatedAt: datetime,
```

1. See [:material-code-braces: TenantTypeDef](./type_defs.md#tenanttypedef) 
2. See [:material-code-brackets: AppAuthorizationStatusType](./literals.md#appauthorizationstatustype) 
## AppAuthorizationTypeDef

```python
# AppAuthorizationTypeDef definition

class AppAuthorizationTypeDef(TypedDict):
    appAuthorizationArn: str,
    appBundleArn: str,
    app: str,
    tenant: TenantTypeDef,  # (1)
    authType: AuthTypeType,  # (2)
    status: AppAuthorizationStatusType,  # (3)
    createdAt: datetime,
    updatedAt: datetime,
    persona: NotRequired[PersonaType],  # (4)
    authUrl: NotRequired[str],
```

1. See [:material-code-braces: TenantTypeDef](./type_defs.md#tenanttypedef) 
2. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
3. See [:material-code-brackets: AppAuthorizationStatusType](./literals.md#appauthorizationstatustype) 
4. See [:material-code-brackets: PersonaType](./literals.md#personatype) 
## ProcessingConfigurationTypeDef

```python
# ProcessingConfigurationTypeDef definition

class ProcessingConfigurationTypeDef(TypedDict):
    auditLog: NotRequired[AuditLogProcessingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AuditLogProcessingConfigurationTypeDef](./type_defs.md#auditlogprocessingconfigurationtypedef) 
## ConnectAppAuthorizationRequestRequestTypeDef

```python
# ConnectAppAuthorizationRequestRequestTypeDef definition

class ConnectAppAuthorizationRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    appAuthorizationIdentifier: str,
    authRequest: NotRequired[AuthRequestTypeDef],  # (1)
```

1. See [:material-code-braces: AuthRequestTypeDef](./type_defs.md#authrequesttypedef) 
## CreateAppBundleResponseTypeDef

```python
# CreateAppBundleResponseTypeDef definition

class CreateAppBundleResponseTypeDef(TypedDict):
    appBundle: AppBundleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppBundleTypeDef](./type_defs.md#appbundletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppBundleResponseTypeDef

```python
# GetAppBundleResponseTypeDef definition

class GetAppBundleResponseTypeDef(TypedDict):
    appBundle: AppBundleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppBundleTypeDef](./type_defs.md#appbundletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppBundlesResponseTypeDef

```python
# ListAppBundlesResponseTypeDef definition

class ListAppBundlesResponseTypeDef(TypedDict):
    appBundleSummaryList: List[AppBundleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AppBundleSummaryTypeDef](./type_defs.md#appbundlesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppBundleRequestRequestTypeDef

```python
# CreateAppBundleRequestRequestTypeDef definition

class CreateAppBundleRequestRequestTypeDef(TypedDict):
    clientToken: NotRequired[str],
    customerManagedKeyIdentifier: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIngestionRequestRequestTypeDef

```python
# CreateIngestionRequestRequestTypeDef definition

class CreateIngestionRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    app: str,
    tenantId: str,
    ingestionType: IngestionTypeType,  # (1)
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: IngestionTypeType](./literals.md#ingestiontypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIngestionResponseTypeDef

```python
# CreateIngestionResponseTypeDef definition

class CreateIngestionResponseTypeDef(TypedDict):
    ingestion: IngestionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionTypeDef](./type_defs.md#ingestiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIngestionResponseTypeDef

```python
# GetIngestionResponseTypeDef definition

class GetIngestionResponseTypeDef(TypedDict):
    ingestion: IngestionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionTypeDef](./type_defs.md#ingestiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CredentialTypeDef

```python
# CredentialTypeDef definition

class CredentialTypeDef(TypedDict):
    oauth2Credential: NotRequired[Oauth2CredentialTypeDef],  # (1)
    apiKeyCredential: NotRequired[ApiKeyCredentialTypeDef],  # (2)
```

1. See [:material-code-braces: Oauth2CredentialTypeDef](./type_defs.md#oauth2credentialtypedef) 
2. See [:material-code-braces: ApiKeyCredentialTypeDef](./type_defs.md#apikeycredentialtypedef) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    s3Bucket: NotRequired[S3BucketTypeDef],  # (1)
    firehoseStream: NotRequired[FirehoseStreamTypeDef],  # (2)
```

1. See [:material-code-braces: S3BucketTypeDef](./type_defs.md#s3buckettypedef) 
2. See [:material-code-braces: FirehoseStreamTypeDef](./type_defs.md#firehosestreamtypedef) 
## ListIngestionDestinationsResponseTypeDef

```python
# ListIngestionDestinationsResponseTypeDef definition

class ListIngestionDestinationsResponseTypeDef(TypedDict):
    ingestionDestinations: List[IngestionDestinationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IngestionDestinationSummaryTypeDef](./type_defs.md#ingestiondestinationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIngestionsResponseTypeDef

```python
# ListIngestionsResponseTypeDef definition

class ListIngestionsResponseTypeDef(TypedDict):
    ingestions: List[IngestionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IngestionSummaryTypeDef](./type_defs.md#ingestionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef

```python
# ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef definition

class ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef(TypedDict):
    appBundleIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAppBundlesRequestListAppBundlesPaginateTypeDef

```python
# ListAppBundlesRequestListAppBundlesPaginateTypeDef definition

class ListAppBundlesRequestListAppBundlesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef

```python
# ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef definition

class ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef(TypedDict):
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIngestionsRequestListIngestionsPaginateTypeDef

```python
# ListIngestionsRequestListIngestionsPaginateTypeDef definition

class ListIngestionsRequestListIngestionsPaginateTypeDef(TypedDict):
    appBundleIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## UserAccessResultItemTypeDef

```python
# UserAccessResultItemTypeDef definition

class UserAccessResultItemTypeDef(TypedDict):
    app: NotRequired[str],
    tenantId: NotRequired[str],
    tenantDisplayName: NotRequired[str],
    taskId: NotRequired[str],
    resultStatus: NotRequired[ResultStatusType],  # (1)
    email: NotRequired[str],
    userId: NotRequired[str],
    userFullName: NotRequired[str],
    userFirstName: NotRequired[str],
    userLastName: NotRequired[str],
    userStatus: NotRequired[str],
    taskError: NotRequired[TaskErrorTypeDef],  # (2)
```

1. See [:material-code-brackets: ResultStatusType](./literals.md#resultstatustype) 
2. See [:material-code-braces: TaskErrorTypeDef](./type_defs.md#taskerrortypedef) 
## UserAccessTaskItemTypeDef

```python
# UserAccessTaskItemTypeDef definition

class UserAccessTaskItemTypeDef(TypedDict):
    app: str,
    tenantId: str,
    taskId: NotRequired[str],
    error: NotRequired[TaskErrorTypeDef],  # (1)
```

1. See [:material-code-braces: TaskErrorTypeDef](./type_defs.md#taskerrortypedef) 
## ConnectAppAuthorizationResponseTypeDef

```python
# ConnectAppAuthorizationResponseTypeDef definition

class ConnectAppAuthorizationResponseTypeDef(TypedDict):
    appAuthorizationSummary: AppAuthorizationSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppAuthorizationSummaryTypeDef](./type_defs.md#appauthorizationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppAuthorizationsResponseTypeDef

```python
# ListAppAuthorizationsResponseTypeDef definition

class ListAppAuthorizationsResponseTypeDef(TypedDict):
    appAuthorizationSummaryList: List[AppAuthorizationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AppAuthorizationSummaryTypeDef](./type_defs.md#appauthorizationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppAuthorizationResponseTypeDef

```python
# CreateAppAuthorizationResponseTypeDef definition

class CreateAppAuthorizationResponseTypeDef(TypedDict):
    appAuthorization: AppAuthorizationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppAuthorizationTypeDef](./type_defs.md#appauthorizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppAuthorizationResponseTypeDef

```python
# GetAppAuthorizationResponseTypeDef definition

class GetAppAuthorizationResponseTypeDef(TypedDict):
    appAuthorization: AppAuthorizationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppAuthorizationTypeDef](./type_defs.md#appauthorizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppAuthorizationResponseTypeDef

```python
# UpdateAppAuthorizationResponseTypeDef definition

class UpdateAppAuthorizationResponseTypeDef(TypedDict):
    appAuthorization: AppAuthorizationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppAuthorizationTypeDef](./type_defs.md#appauthorizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppAuthorizationRequestRequestTypeDef

```python
# CreateAppAuthorizationRequestRequestTypeDef definition

class CreateAppAuthorizationRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    app: str,
    credential: CredentialTypeDef,  # (1)
    tenant: TenantTypeDef,  # (2)
    authType: AuthTypeType,  # (3)
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: CredentialTypeDef](./type_defs.md#credentialtypedef) 
2. See [:material-code-braces: TenantTypeDef](./type_defs.md#tenanttypedef) 
3. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateAppAuthorizationRequestRequestTypeDef

```python
# UpdateAppAuthorizationRequestRequestTypeDef definition

class UpdateAppAuthorizationRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    appAuthorizationIdentifier: str,
    credential: NotRequired[CredentialTypeDef],  # (1)
    tenant: NotRequired[TenantTypeDef],  # (2)
```

1. See [:material-code-braces: CredentialTypeDef](./type_defs.md#credentialtypedef) 
2. See [:material-code-braces: TenantTypeDef](./type_defs.md#tenanttypedef) 
## AuditLogDestinationConfigurationTypeDef

```python
# AuditLogDestinationConfigurationTypeDef definition

class AuditLogDestinationConfigurationTypeDef(TypedDict):
    destination: DestinationTypeDef,  # (1)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
## BatchGetUserAccessTasksResponseTypeDef

```python
# BatchGetUserAccessTasksResponseTypeDef definition

class BatchGetUserAccessTasksResponseTypeDef(TypedDict):
    userAccessResultsList: List[UserAccessResultItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserAccessResultItemTypeDef](./type_defs.md#useraccessresultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartUserAccessTasksResponseTypeDef

```python
# StartUserAccessTasksResponseTypeDef definition

class StartUserAccessTasksResponseTypeDef(TypedDict):
    userAccessTasksList: List[UserAccessTaskItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserAccessTaskItemTypeDef](./type_defs.md#useraccesstaskitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationConfigurationTypeDef

```python
# DestinationConfigurationTypeDef definition

class DestinationConfigurationTypeDef(TypedDict):
    auditLog: NotRequired[AuditLogDestinationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AuditLogDestinationConfigurationTypeDef](./type_defs.md#auditlogdestinationconfigurationtypedef) 
## CreateIngestionDestinationRequestRequestTypeDef

```python
# CreateIngestionDestinationRequestRequestTypeDef definition

class CreateIngestionDestinationRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    processingConfiguration: ProcessingConfigurationTypeDef,  # (1)
    destinationConfiguration: DestinationConfigurationTypeDef,  # (2)
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) 
2. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## IngestionDestinationTypeDef

```python
# IngestionDestinationTypeDef definition

class IngestionDestinationTypeDef(TypedDict):
    arn: str,
    ingestionArn: str,
    processingConfiguration: ProcessingConfigurationTypeDef,  # (1)
    destinationConfiguration: DestinationConfigurationTypeDef,  # (2)
    status: NotRequired[IngestionDestinationStatusType],  # (3)
    statusReason: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: ProcessingConfigurationTypeDef](./type_defs.md#processingconfigurationtypedef) 
2. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
3. See [:material-code-brackets: IngestionDestinationStatusType](./literals.md#ingestiondestinationstatustype) 
## UpdateIngestionDestinationRequestRequestTypeDef

```python
# UpdateIngestionDestinationRequestRequestTypeDef definition

class UpdateIngestionDestinationRequestRequestTypeDef(TypedDict):
    appBundleIdentifier: str,
    ingestionIdentifier: str,
    ingestionDestinationIdentifier: str,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
## CreateIngestionDestinationResponseTypeDef

```python
# CreateIngestionDestinationResponseTypeDef definition

class CreateIngestionDestinationResponseTypeDef(TypedDict):
    ingestionDestination: IngestionDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionDestinationTypeDef](./type_defs.md#ingestiondestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIngestionDestinationResponseTypeDef

```python
# GetIngestionDestinationResponseTypeDef definition

class GetIngestionDestinationResponseTypeDef(TypedDict):
    ingestionDestination: IngestionDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionDestinationTypeDef](./type_defs.md#ingestiondestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIngestionDestinationResponseTypeDef

```python
# UpdateIngestionDestinationResponseTypeDef definition

class UpdateIngestionDestinationResponseTypeDef(TypedDict):
    ingestionDestination: IngestionDestinationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionDestinationTypeDef](./type_defs.md#ingestiondestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
