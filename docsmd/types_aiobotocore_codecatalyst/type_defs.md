# Type definitions

> [Index](../README.md) > [CodeCatalyst](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeCatalyst](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#codecatalyst)
    type annotations stubs module [types-aiobotocore-codecatalyst](https://pypi.org/project/types-aiobotocore-codecatalyst/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AccessTokenSummaryTypeDef

```python
# AccessTokenSummaryTypeDef definition

class AccessTokenSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    expiresTime: NotRequired[datetime],
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

## IdeConfigurationTypeDef

```python
# IdeConfigurationTypeDef definition

class IdeConfigurationTypeDef(TypedDict):
    runtime: NotRequired[str],
    name: NotRequired[str],
```

## PersistentStorageConfigurationTypeDef

```python
# PersistentStorageConfigurationTypeDef definition

class PersistentStorageConfigurationTypeDef(TypedDict):
    sizeInGiB: int,
```

## RepositoryInputTypeDef

```python
# RepositoryInputTypeDef definition

class RepositoryInputTypeDef(TypedDict):
    repositoryName: str,
    branchName: NotRequired[str],
```

## CreateProjectRequestRequestTypeDef

```python
# CreateProjectRequestRequestTypeDef definition

class CreateProjectRequestRequestTypeDef(TypedDict):
    spaceName: str,
    displayName: str,
    description: NotRequired[str],
```

## CreateSourceRepositoryBranchRequestRequestTypeDef

```python
# CreateSourceRepositoryBranchRequestRequestTypeDef definition

class CreateSourceRepositoryBranchRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    sourceRepositoryName: str,
    name: str,
    headCommitId: NotRequired[str],
```

## CreateSourceRepositoryRequestRequestTypeDef

```python
# CreateSourceRepositoryRequestRequestTypeDef definition

class CreateSourceRepositoryRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    name: str,
    description: NotRequired[str],
```

## DeleteAccessTokenRequestRequestTypeDef

```python
# DeleteAccessTokenRequestRequestTypeDef definition

class DeleteAccessTokenRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteDevEnvironmentRequestRequestTypeDef

```python
# DeleteDevEnvironmentRequestRequestTypeDef definition

class DeleteDevEnvironmentRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
```

## DeleteProjectRequestRequestTypeDef

```python
# DeleteProjectRequestRequestTypeDef definition

class DeleteProjectRequestRequestTypeDef(TypedDict):
    spaceName: str,
    name: str,
```

## DeleteSourceRepositoryRequestRequestTypeDef

```python
# DeleteSourceRepositoryRequestRequestTypeDef definition

class DeleteSourceRepositoryRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    name: str,
```

## DeleteSpaceRequestRequestTypeDef

```python
# DeleteSpaceRequestRequestTypeDef definition

class DeleteSpaceRequestRequestTypeDef(TypedDict):
    name: str,
```

## DevEnvironmentAccessDetailsTypeDef

```python
# DevEnvironmentAccessDetailsTypeDef definition

class DevEnvironmentAccessDetailsTypeDef(TypedDict):
    streamUrl: str,
    tokenValue: str,
```

## DevEnvironmentRepositorySummaryTypeDef

```python
# DevEnvironmentRepositorySummaryTypeDef definition

class DevEnvironmentRepositorySummaryTypeDef(TypedDict):
    repositoryName: str,
    branchName: NotRequired[str],
```

## ExecuteCommandSessionConfigurationTypeDef

```python
# ExecuteCommandSessionConfigurationTypeDef definition

class ExecuteCommandSessionConfigurationTypeDef(TypedDict):
    command: str,
    arguments: NotRequired[Sequence[str]],
```

## DevEnvironmentSessionSummaryTypeDef

```python
# DevEnvironmentSessionSummaryTypeDef definition

class DevEnvironmentSessionSummaryTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    devEnvironmentId: str,
    startedTime: datetime,
    id: str,
```

## IdeTypeDef

```python
# IdeTypeDef definition

class IdeTypeDef(TypedDict):
    runtime: NotRequired[str],
    name: NotRequired[str],
```

## PersistentStorageTypeDef

```python
# PersistentStorageTypeDef definition

class PersistentStorageTypeDef(TypedDict):
    sizeInGiB: int,
```

## EmailAddressTypeDef

```python
# EmailAddressTypeDef definition

class EmailAddressTypeDef(TypedDict):
    email: NotRequired[str],
    verified: NotRequired[bool],
```

## EventPayloadTypeDef

```python
# EventPayloadTypeDef definition

class EventPayloadTypeDef(TypedDict):
    contentType: NotRequired[str],
    data: NotRequired[str],
```

## ProjectInformationTypeDef

```python
# ProjectInformationTypeDef definition

class ProjectInformationTypeDef(TypedDict):
    name: NotRequired[str],
    projectId: NotRequired[str],
```

## UserIdentityTypeDef

```python
# UserIdentityTypeDef definition

class UserIdentityTypeDef(TypedDict):
    userType: UserTypeType,  # (1)
    principalId: str,
    userName: NotRequired[str],
    awsAccountId: NotRequired[str],
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    key: str,
    values: Sequence[str],
    comparisonOperator: NotRequired[str],
```

## GetDevEnvironmentRequestRequestTypeDef

```python
# GetDevEnvironmentRequestRequestTypeDef definition

class GetDevEnvironmentRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
```

## GetProjectRequestRequestTypeDef

```python
# GetProjectRequestRequestTypeDef definition

class GetProjectRequestRequestTypeDef(TypedDict):
    spaceName: str,
    name: str,
```

## GetSourceRepositoryCloneUrlsRequestRequestTypeDef

```python
# GetSourceRepositoryCloneUrlsRequestRequestTypeDef definition

class GetSourceRepositoryCloneUrlsRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    sourceRepositoryName: str,
```

## GetSourceRepositoryRequestRequestTypeDef

```python
# GetSourceRepositoryRequestRequestTypeDef definition

class GetSourceRepositoryRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    name: str,
```

## GetSpaceRequestRequestTypeDef

```python
# GetSpaceRequestRequestTypeDef definition

class GetSpaceRequestRequestTypeDef(TypedDict):
    name: str,
```

## GetSubscriptionRequestRequestTypeDef

```python
# GetSubscriptionRequestRequestTypeDef definition

class GetSubscriptionRequestRequestTypeDef(TypedDict):
    spaceName: str,
```

## GetUserDetailsRequestRequestTypeDef

```python
# GetUserDetailsRequestRequestTypeDef definition

class GetUserDetailsRequestRequestTypeDef(TypedDict):
    id: NotRequired[str],
    userName: NotRequired[str],
```

## GetWorkflowRequestRequestTypeDef

```python
# GetWorkflowRequestRequestTypeDef definition

class GetWorkflowRequestRequestTypeDef(TypedDict):
    spaceName: str,
    id: str,
    projectName: str,
```

## WorkflowDefinitionTypeDef

```python
# WorkflowDefinitionTypeDef definition

class WorkflowDefinitionTypeDef(TypedDict):
    path: str,
```

## GetWorkflowRunRequestRequestTypeDef

```python
# GetWorkflowRunRequestRequestTypeDef definition

class GetWorkflowRunRequestRequestTypeDef(TypedDict):
    spaceName: str,
    id: str,
    projectName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAccessTokensRequestRequestTypeDef

```python
# ListAccessTokensRequestRequestTypeDef definition

class ListAccessTokensRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDevEnvironmentSessionsRequestRequestTypeDef

```python
# ListDevEnvironmentSessionsRequestRequestTypeDef definition

class ListDevEnvironmentSessionsRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    devEnvironmentId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ProjectListFilterTypeDef

```python
# ProjectListFilterTypeDef definition

class ProjectListFilterTypeDef(TypedDict):
    key: FilterKeyType,  # (1)
    values: Sequence[str],
    comparisonOperator: NotRequired[ComparisonOperatorType],  # (2)
```

1. See [:material-code-brackets: FilterKeyType](./literals.md#filterkeytype) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    name: str,
    displayName: NotRequired[str],
    description: NotRequired[str],
```

## ListSourceRepositoriesItemTypeDef

```python
# ListSourceRepositoriesItemTypeDef definition

class ListSourceRepositoriesItemTypeDef(TypedDict):
    id: str,
    name: str,
    lastUpdatedTime: datetime,
    createdTime: datetime,
    description: NotRequired[str],
```

## ListSourceRepositoriesRequestRequestTypeDef

```python
# ListSourceRepositoriesRequestRequestTypeDef definition

class ListSourceRepositoriesRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListSourceRepositoryBranchesItemTypeDef

```python
# ListSourceRepositoryBranchesItemTypeDef definition

class ListSourceRepositoryBranchesItemTypeDef(TypedDict):
    ref: NotRequired[str],
    name: NotRequired[str],
    lastUpdatedTime: NotRequired[datetime],
    headCommitId: NotRequired[str],
```

## ListSourceRepositoryBranchesRequestRequestTypeDef

```python
# ListSourceRepositoryBranchesRequestRequestTypeDef definition

class ListSourceRepositoryBranchesRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    sourceRepositoryName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListSpacesRequestRequestTypeDef

```python
# ListSpacesRequestRequestTypeDef definition

class ListSpacesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## SpaceSummaryTypeDef

```python
# SpaceSummaryTypeDef definition

class SpaceSummaryTypeDef(TypedDict):
    name: str,
    regionName: str,
    displayName: NotRequired[str],
    description: NotRequired[str],
```

## ListWorkflowRunsRequestRequestTypeDef

```python
# ListWorkflowRunsRequestRequestTypeDef definition

class ListWorkflowRunsRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    workflowId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    sortBy: NotRequired[Sequence[Mapping[str, Any]]],
```

## WorkflowRunSummaryTypeDef

```python
# WorkflowRunSummaryTypeDef definition

class WorkflowRunSummaryTypeDef(TypedDict):
    id: str,
    workflowId: str,
    workflowName: str,
    status: WorkflowRunStatusType,  # (1)
    startTime: datetime,
    lastUpdatedTime: datetime,
    statusReasons: NotRequired[List[Dict[str, Any]]],
    endTime: NotRequired[datetime],
```

1. See [:material-code-brackets: WorkflowRunStatusType](./literals.md#workflowrunstatustype) 
## ListWorkflowsRequestRequestTypeDef

```python
# ListWorkflowsRequestRequestTypeDef definition

class ListWorkflowsRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    sortBy: NotRequired[Sequence[Mapping[str, Any]]],
```

## StartWorkflowRunRequestRequestTypeDef

```python
# StartWorkflowRunRequestRequestTypeDef definition

class StartWorkflowRunRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    workflowId: str,
    clientToken: NotRequired[str],
```

## StopDevEnvironmentRequestRequestTypeDef

```python
# StopDevEnvironmentRequestRequestTypeDef definition

class StopDevEnvironmentRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
```

## StopDevEnvironmentSessionRequestRequestTypeDef

```python
# StopDevEnvironmentSessionRequestRequestTypeDef definition

class StopDevEnvironmentSessionRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    sessionId: str,
```

## UpdateProjectRequestRequestTypeDef

```python
# UpdateProjectRequestRequestTypeDef definition

class UpdateProjectRequestRequestTypeDef(TypedDict):
    spaceName: str,
    name: str,
    description: NotRequired[str],
```

## UpdateSpaceRequestRequestTypeDef

```python
# UpdateSpaceRequestRequestTypeDef definition

class UpdateSpaceRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
```

## WorkflowDefinitionSummaryTypeDef

```python
# WorkflowDefinitionSummaryTypeDef definition

class WorkflowDefinitionSummaryTypeDef(TypedDict):
    path: str,
```

## CreateAccessTokenRequestRequestTypeDef

```python
# CreateAccessTokenRequestRequestTypeDef definition

class CreateAccessTokenRequestRequestTypeDef(TypedDict):
    name: str,
    expiresTime: NotRequired[TimestampTypeDef],
```

## ListEventLogsRequestRequestTypeDef

```python
# ListEventLogsRequestRequestTypeDef definition

class ListEventLogsRequestRequestTypeDef(TypedDict):
    spaceName: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    eventName: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## CreateAccessTokenResponseTypeDef

```python
# CreateAccessTokenResponseTypeDef definition

class CreateAccessTokenResponseTypeDef(TypedDict):
    secret: str,
    name: str,
    expiresTime: datetime,
    accessTokenId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDevEnvironmentResponseTypeDef

```python
# CreateDevEnvironmentResponseTypeDef definition

class CreateDevEnvironmentResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    vpcConnectionName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectResponseTypeDef

```python
# CreateProjectResponseTypeDef definition

class CreateProjectResponseTypeDef(TypedDict):
    spaceName: str,
    name: str,
    displayName: str,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSourceRepositoryBranchResponseTypeDef

```python
# CreateSourceRepositoryBranchResponseTypeDef definition

class CreateSourceRepositoryBranchResponseTypeDef(TypedDict):
    ref: str,
    name: str,
    lastUpdatedTime: datetime,
    headCommitId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSourceRepositoryResponseTypeDef

```python
# CreateSourceRepositoryResponseTypeDef definition

class CreateSourceRepositoryResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    name: str,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDevEnvironmentResponseTypeDef

```python
# DeleteDevEnvironmentResponseTypeDef definition

class DeleteDevEnvironmentResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProjectResponseTypeDef

```python
# DeleteProjectResponseTypeDef definition

class DeleteProjectResponseTypeDef(TypedDict):
    spaceName: str,
    name: str,
    displayName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSourceRepositoryResponseTypeDef

```python
# DeleteSourceRepositoryResponseTypeDef definition

class DeleteSourceRepositoryResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSpaceResponseTypeDef

```python
# DeleteSpaceResponseTypeDef definition

class DeleteSpaceResponseTypeDef(TypedDict):
    name: str,
    displayName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProjectResponseTypeDef

```python
# GetProjectResponseTypeDef definition

class GetProjectResponseTypeDef(TypedDict):
    spaceName: str,
    name: str,
    displayName: str,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSourceRepositoryCloneUrlsResponseTypeDef

```python
# GetSourceRepositoryCloneUrlsResponseTypeDef definition

class GetSourceRepositoryCloneUrlsResponseTypeDef(TypedDict):
    https: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSourceRepositoryResponseTypeDef

```python
# GetSourceRepositoryResponseTypeDef definition

class GetSourceRepositoryResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    name: str,
    description: str,
    lastUpdatedTime: datetime,
    createdTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSpaceResponseTypeDef

```python
# GetSpaceResponseTypeDef definition

class GetSpaceResponseTypeDef(TypedDict):
    name: str,
    regionName: str,
    displayName: str,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSubscriptionResponseTypeDef

```python
# GetSubscriptionResponseTypeDef definition

class GetSubscriptionResponseTypeDef(TypedDict):
    subscriptionType: str,
    awsAccountName: str,
    pendingSubscriptionType: str,
    pendingSubscriptionStartTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowRunResponseTypeDef

```python
# GetWorkflowRunResponseTypeDef definition

class GetWorkflowRunResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    workflowId: str,
    status: WorkflowRunStatusType,  # (1)
    statusReasons: List[Dict[str, Any]],
    startTime: datetime,
    endTime: datetime,
    lastUpdatedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: WorkflowRunStatusType](./literals.md#workflowrunstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessTokensResponseTypeDef

```python
# ListAccessTokensResponseTypeDef definition

class ListAccessTokensResponseTypeDef(TypedDict):
    items: List[AccessTokenSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccessTokenSummaryTypeDef](./type_defs.md#accesstokensummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDevEnvironmentResponseTypeDef

```python
# StartDevEnvironmentResponseTypeDef definition

class StartDevEnvironmentResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    status: DevEnvironmentStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DevEnvironmentStatusType](./literals.md#devenvironmentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartWorkflowRunResponseTypeDef

```python
# StartWorkflowRunResponseTypeDef definition

class StartWorkflowRunResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    workflowId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopDevEnvironmentResponseTypeDef

```python
# StopDevEnvironmentResponseTypeDef definition

class StopDevEnvironmentResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    status: DevEnvironmentStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DevEnvironmentStatusType](./literals.md#devenvironmentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopDevEnvironmentSessionResponseTypeDef

```python
# StopDevEnvironmentSessionResponseTypeDef definition

class StopDevEnvironmentSessionResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    sessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectResponseTypeDef

```python
# UpdateProjectResponseTypeDef definition

class UpdateProjectResponseTypeDef(TypedDict):
    spaceName: str,
    name: str,
    displayName: str,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSpaceResponseTypeDef

```python
# UpdateSpaceResponseTypeDef definition

class UpdateSpaceResponseTypeDef(TypedDict):
    name: str,
    displayName: str,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifySessionResponseTypeDef

```python
# VerifySessionResponseTypeDef definition

class VerifySessionResponseTypeDef(TypedDict):
    identity: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDevEnvironmentRequestRequestTypeDef

```python
# StartDevEnvironmentRequestRequestTypeDef definition

class StartDevEnvironmentRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    ides: NotRequired[Sequence[IdeConfigurationTypeDef]],  # (1)
    instanceType: NotRequired[InstanceTypeType],  # (2)
    inactivityTimeoutMinutes: NotRequired[int],
```

1. See [:material-code-braces: IdeConfigurationTypeDef](./type_defs.md#ideconfigurationtypedef) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## UpdateDevEnvironmentRequestRequestTypeDef

```python
# UpdateDevEnvironmentRequestRequestTypeDef definition

class UpdateDevEnvironmentRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    alias: NotRequired[str],
    ides: NotRequired[Sequence[IdeConfigurationTypeDef]],  # (1)
    instanceType: NotRequired[InstanceTypeType],  # (2)
    inactivityTimeoutMinutes: NotRequired[int],
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: IdeConfigurationTypeDef](./type_defs.md#ideconfigurationtypedef) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## UpdateDevEnvironmentResponseTypeDef

```python
# UpdateDevEnvironmentResponseTypeDef definition

class UpdateDevEnvironmentResponseTypeDef(TypedDict):
    id: str,
    spaceName: str,
    projectName: str,
    alias: str,
    ides: List[IdeConfigurationTypeDef],  # (1)
    instanceType: InstanceTypeType,  # (2)
    inactivityTimeoutMinutes: int,
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: IdeConfigurationTypeDef](./type_defs.md#ideconfigurationtypedef) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDevEnvironmentRequestRequestTypeDef

```python
# CreateDevEnvironmentRequestRequestTypeDef definition

class CreateDevEnvironmentRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    instanceType: InstanceTypeType,  # (1)
    persistentStorage: PersistentStorageConfigurationTypeDef,  # (2)
    repositories: NotRequired[Sequence[RepositoryInputTypeDef]],  # (3)
    clientToken: NotRequired[str],
    alias: NotRequired[str],
    ides: NotRequired[Sequence[IdeConfigurationTypeDef]],  # (4)
    inactivityTimeoutMinutes: NotRequired[int],
    vpcConnectionName: NotRequired[str],
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
2. See [:material-code-braces: PersistentStorageConfigurationTypeDef](./type_defs.md#persistentstorageconfigurationtypedef) 
3. See [:material-code-braces: RepositoryInputTypeDef](./type_defs.md#repositoryinputtypedef) 
4. See [:material-code-braces: IdeConfigurationTypeDef](./type_defs.md#ideconfigurationtypedef) 
## StartDevEnvironmentSessionResponseTypeDef

```python
# StartDevEnvironmentSessionResponseTypeDef definition

class StartDevEnvironmentSessionResponseTypeDef(TypedDict):
    accessDetails: DevEnvironmentAccessDetailsTypeDef,  # (1)
    sessionId: str,
    spaceName: str,
    projectName: str,
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DevEnvironmentAccessDetailsTypeDef](./type_defs.md#devenvironmentaccessdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DevEnvironmentSessionConfigurationTypeDef

```python
# DevEnvironmentSessionConfigurationTypeDef definition

class DevEnvironmentSessionConfigurationTypeDef(TypedDict):
    sessionType: DevEnvironmentSessionTypeType,  # (1)
    executeCommandSessionConfiguration: NotRequired[ExecuteCommandSessionConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: DevEnvironmentSessionTypeType](./literals.md#devenvironmentsessiontypetype) 
2. See [:material-code-braces: ExecuteCommandSessionConfigurationTypeDef](./type_defs.md#executecommandsessionconfigurationtypedef) 
## ListDevEnvironmentSessionsResponseTypeDef

```python
# ListDevEnvironmentSessionsResponseTypeDef definition

class ListDevEnvironmentSessionsResponseTypeDef(TypedDict):
    items: List[DevEnvironmentSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DevEnvironmentSessionSummaryTypeDef](./type_defs.md#devenvironmentsessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DevEnvironmentSummaryTypeDef

```python
# DevEnvironmentSummaryTypeDef definition

class DevEnvironmentSummaryTypeDef(TypedDict):
    id: str,
    lastUpdatedTime: datetime,
    creatorId: str,
    status: DevEnvironmentStatusType,  # (1)
    repositories: List[DevEnvironmentRepositorySummaryTypeDef],  # (2)
    instanceType: InstanceTypeType,  # (4)
    inactivityTimeoutMinutes: int,
    persistentStorage: PersistentStorageTypeDef,  # (5)
    spaceName: NotRequired[str],
    projectName: NotRequired[str],
    statusReason: NotRequired[str],
    alias: NotRequired[str],
    ides: NotRequired[List[IdeTypeDef]],  # (3)
    vpcConnectionName: NotRequired[str],
```

1. See [:material-code-brackets: DevEnvironmentStatusType](./literals.md#devenvironmentstatustype) 
2. See [:material-code-braces: DevEnvironmentRepositorySummaryTypeDef](./type_defs.md#devenvironmentrepositorysummarytypedef) 
3. See [:material-code-braces: IdeTypeDef](./type_defs.md#idetypedef) 
4. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
5. See [:material-code-braces: PersistentStorageTypeDef](./type_defs.md#persistentstoragetypedef) 
## GetDevEnvironmentResponseTypeDef

```python
# GetDevEnvironmentResponseTypeDef definition

class GetDevEnvironmentResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    lastUpdatedTime: datetime,
    creatorId: str,
    status: DevEnvironmentStatusType,  # (1)
    statusReason: str,
    repositories: List[DevEnvironmentRepositorySummaryTypeDef],  # (2)
    alias: str,
    ides: List[IdeTypeDef],  # (3)
    instanceType: InstanceTypeType,  # (4)
    inactivityTimeoutMinutes: int,
    persistentStorage: PersistentStorageTypeDef,  # (5)
    vpcConnectionName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: DevEnvironmentStatusType](./literals.md#devenvironmentstatustype) 
2. See [:material-code-braces: DevEnvironmentRepositorySummaryTypeDef](./type_defs.md#devenvironmentrepositorysummarytypedef) 
3. See [:material-code-braces: IdeTypeDef](./type_defs.md#idetypedef) 
4. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
5. See [:material-code-braces: PersistentStorageTypeDef](./type_defs.md#persistentstoragetypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserDetailsResponseTypeDef

```python
# GetUserDetailsResponseTypeDef definition

class GetUserDetailsResponseTypeDef(TypedDict):
    userId: str,
    userName: str,
    displayName: str,
    primaryEmail: EmailAddressTypeDef,  # (1)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmailAddressTypeDef](./type_defs.md#emailaddresstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventLogEntryTypeDef

```python
# EventLogEntryTypeDef definition

class EventLogEntryTypeDef(TypedDict):
    id: str,
    eventName: str,
    eventType: str,
    eventCategory: str,
    eventSource: str,
    eventTime: datetime,
    operationType: OperationTypeType,  # (1)
    userIdentity: UserIdentityTypeDef,  # (2)
    projectInformation: NotRequired[ProjectInformationTypeDef],  # (3)
    requestId: NotRequired[str],
    requestPayload: NotRequired[EventPayloadTypeDef],  # (4)
    responsePayload: NotRequired[EventPayloadTypeDef],  # (4)
    errorCode: NotRequired[str],
    sourceIpAddress: NotRequired[str],
    userAgent: NotRequired[str],
```

1. See [:material-code-brackets: OperationTypeType](./literals.md#operationtypetype) 
2. See [:material-code-braces: UserIdentityTypeDef](./type_defs.md#useridentitytypedef) 
3. See [:material-code-braces: ProjectInformationTypeDef](./type_defs.md#projectinformationtypedef) 
4. See [:material-code-braces: EventPayloadTypeDef](./type_defs.md#eventpayloadtypedef) 
5. See [:material-code-braces: EventPayloadTypeDef](./type_defs.md#eventpayloadtypedef) 
## ListDevEnvironmentsRequestRequestTypeDef

```python
# ListDevEnvironmentsRequestRequestTypeDef definition

class ListDevEnvironmentsRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: NotRequired[str],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetWorkflowResponseTypeDef

```python
# GetWorkflowResponseTypeDef definition

class GetWorkflowResponseTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    name: str,
    sourceRepositoryName: str,
    sourceBranchName: str,
    definition: WorkflowDefinitionTypeDef,  # (1)
    createdTime: datetime,
    lastUpdatedTime: datetime,
    runMode: WorkflowRunModeType,  # (2)
    status: WorkflowStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: WorkflowDefinitionTypeDef](./type_defs.md#workflowdefinitiontypedef) 
2. See [:material-code-brackets: WorkflowRunModeType](./literals.md#workflowrunmodetype) 
3. See [:material-code-brackets: WorkflowStatusType](./literals.md#workflowstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessTokensRequestPaginateTypeDef

```python
# ListAccessTokensRequestPaginateTypeDef definition

class ListAccessTokensRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDevEnvironmentSessionsRequestPaginateTypeDef

```python
# ListDevEnvironmentSessionsRequestPaginateTypeDef definition

class ListDevEnvironmentSessionsRequestPaginateTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    devEnvironmentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDevEnvironmentsRequestPaginateTypeDef

```python
# ListDevEnvironmentsRequestPaginateTypeDef definition

class ListDevEnvironmentsRequestPaginateTypeDef(TypedDict):
    spaceName: str,
    projectName: NotRequired[str],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEventLogsRequestPaginateTypeDef

```python
# ListEventLogsRequestPaginateTypeDef definition

class ListEventLogsRequestPaginateTypeDef(TypedDict):
    spaceName: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    eventName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSourceRepositoriesRequestPaginateTypeDef

```python
# ListSourceRepositoriesRequestPaginateTypeDef definition

class ListSourceRepositoriesRequestPaginateTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSourceRepositoryBranchesRequestPaginateTypeDef

```python
# ListSourceRepositoryBranchesRequestPaginateTypeDef definition

class ListSourceRepositoryBranchesRequestPaginateTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    sourceRepositoryName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSpacesRequestPaginateTypeDef

```python
# ListSpacesRequestPaginateTypeDef definition

class ListSpacesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkflowRunsRequestPaginateTypeDef

```python
# ListWorkflowRunsRequestPaginateTypeDef definition

class ListWorkflowRunsRequestPaginateTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    workflowId: NotRequired[str],
    sortBy: NotRequired[Sequence[Mapping[str, Any]]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkflowsRequestPaginateTypeDef

```python
# ListWorkflowsRequestPaginateTypeDef definition

class ListWorkflowsRequestPaginateTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    sortBy: NotRequired[Sequence[Mapping[str, Any]]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestPaginateTypeDef

```python
# ListProjectsRequestPaginateTypeDef definition

class ListProjectsRequestPaginateTypeDef(TypedDict):
    spaceName: str,
    filters: NotRequired[Sequence[ProjectListFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ProjectListFilterTypeDef](./type_defs.md#projectlistfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestRequestTypeDef

```python
# ListProjectsRequestRequestTypeDef definition

class ListProjectsRequestRequestTypeDef(TypedDict):
    spaceName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[ProjectListFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: ProjectListFilterTypeDef](./type_defs.md#projectlistfiltertypedef) 
## ListProjectsResponseTypeDef

```python
# ListProjectsResponseTypeDef definition

class ListProjectsResponseTypeDef(TypedDict):
    items: List[ProjectSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSourceRepositoriesResponseTypeDef

```python
# ListSourceRepositoriesResponseTypeDef definition

class ListSourceRepositoriesResponseTypeDef(TypedDict):
    items: List[ListSourceRepositoriesItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListSourceRepositoriesItemTypeDef](./type_defs.md#listsourcerepositoriesitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSourceRepositoryBranchesResponseTypeDef

```python
# ListSourceRepositoryBranchesResponseTypeDef definition

class ListSourceRepositoryBranchesResponseTypeDef(TypedDict):
    items: List[ListSourceRepositoryBranchesItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListSourceRepositoryBranchesItemTypeDef](./type_defs.md#listsourcerepositorybranchesitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSpacesResponseTypeDef

```python
# ListSpacesResponseTypeDef definition

class ListSpacesResponseTypeDef(TypedDict):
    items: List[SpaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SpaceSummaryTypeDef](./type_defs.md#spacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkflowRunsResponseTypeDef

```python
# ListWorkflowRunsResponseTypeDef definition

class ListWorkflowRunsResponseTypeDef(TypedDict):
    items: List[WorkflowRunSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkflowRunSummaryTypeDef](./type_defs.md#workflowrunsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkflowSummaryTypeDef

```python
# WorkflowSummaryTypeDef definition

class WorkflowSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    sourceRepositoryName: str,
    sourceBranchName: str,
    definition: WorkflowDefinitionSummaryTypeDef,  # (1)
    createdTime: datetime,
    lastUpdatedTime: datetime,
    runMode: WorkflowRunModeType,  # (2)
    status: WorkflowStatusType,  # (3)
```

1. See [:material-code-braces: WorkflowDefinitionSummaryTypeDef](./type_defs.md#workflowdefinitionsummarytypedef) 
2. See [:material-code-brackets: WorkflowRunModeType](./literals.md#workflowrunmodetype) 
3. See [:material-code-brackets: WorkflowStatusType](./literals.md#workflowstatustype) 
## StartDevEnvironmentSessionRequestRequestTypeDef

```python
# StartDevEnvironmentSessionRequestRequestTypeDef definition

class StartDevEnvironmentSessionRequestRequestTypeDef(TypedDict):
    spaceName: str,
    projectName: str,
    id: str,
    sessionConfiguration: DevEnvironmentSessionConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: DevEnvironmentSessionConfigurationTypeDef](./type_defs.md#devenvironmentsessionconfigurationtypedef) 
## ListDevEnvironmentsResponseTypeDef

```python
# ListDevEnvironmentsResponseTypeDef definition

class ListDevEnvironmentsResponseTypeDef(TypedDict):
    items: List[DevEnvironmentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DevEnvironmentSummaryTypeDef](./type_defs.md#devenvironmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventLogsResponseTypeDef

```python
# ListEventLogsResponseTypeDef definition

class ListEventLogsResponseTypeDef(TypedDict):
    items: List[EventLogEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EventLogEntryTypeDef](./type_defs.md#eventlogentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkflowsResponseTypeDef

```python
# ListWorkflowsResponseTypeDef definition

class ListWorkflowsResponseTypeDef(TypedDict):
    items: List[WorkflowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkflowSummaryTypeDef](./type_defs.md#workflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
