# Type definitions

> [Index](../README.md) > [CodeStar](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeStar](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar)
    type annotations stubs module [types-aiobotocore-codestar](https://pypi.org/project/types-aiobotocore-codestar/).



## AssociateTeamMemberRequestRequestTypeDef

```python
# AssociateTeamMemberRequestRequestTypeDef definition

class AssociateTeamMemberRequestRequestTypeDef(TypedDict):
    projectId: str,
    userArn: str,
    projectRole: str,
    clientRequestToken: NotRequired[str],
    remoteAccessAllowed: NotRequired[bool],
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

## CodeCommitCodeDestinationTypeDef

```python
# CodeCommitCodeDestinationTypeDef definition

class CodeCommitCodeDestinationTypeDef(TypedDict):
    name: str,
```

## GitHubCodeDestinationTypeDef

```python
# GitHubCodeDestinationTypeDef definition

class GitHubCodeDestinationTypeDef(TypedDict):
    name: str,
    type: str,
    owner: str,
    privateRepository: bool,
    issuesEnabled: bool,
    token: str,
    description: NotRequired[str],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucketName: NotRequired[str],
    bucketKey: NotRequired[str],
```

## CreateUserProfileRequestRequestTypeDef

```python
# CreateUserProfileRequestRequestTypeDef definition

class CreateUserProfileRequestRequestTypeDef(TypedDict):
    userArn: str,
    displayName: str,
    emailAddress: str,
    sshPublicKey: NotRequired[str],
```

## DeleteProjectRequestRequestTypeDef

```python
# DeleteProjectRequestRequestTypeDef definition

class DeleteProjectRequestRequestTypeDef(TypedDict):
    id: str,
    clientRequestToken: NotRequired[str],
    deleteStack: NotRequired[bool],
```

## DeleteUserProfileRequestRequestTypeDef

```python
# DeleteUserProfileRequestRequestTypeDef definition

class DeleteUserProfileRequestRequestTypeDef(TypedDict):
    userArn: str,
```

## DescribeProjectRequestRequestTypeDef

```python
# DescribeProjectRequestRequestTypeDef definition

class DescribeProjectRequestRequestTypeDef(TypedDict):
    id: str,
```

## ProjectStatusTypeDef

```python
# ProjectStatusTypeDef definition

class ProjectStatusTypeDef(TypedDict):
    state: str,
    reason: NotRequired[str],
```

## DescribeUserProfileRequestRequestTypeDef

```python
# DescribeUserProfileRequestRequestTypeDef definition

class DescribeUserProfileRequestRequestTypeDef(TypedDict):
    userArn: str,
```

## DisassociateTeamMemberRequestRequestTypeDef

```python
# DisassociateTeamMemberRequestRequestTypeDef definition

class DisassociateTeamMemberRequestRequestTypeDef(TypedDict):
    projectId: str,
    userArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListProjectsRequestRequestTypeDef

```python
# ListProjectsRequestRequestTypeDef definition

class ListProjectsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    projectId: NotRequired[str],
    projectArn: NotRequired[str],
```

## ListResourcesRequestRequestTypeDef

```python
# ListResourcesRequestRequestTypeDef definition

class ListResourcesRequestRequestTypeDef(TypedDict):
    projectId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    id: str,
```

## ListTagsForProjectRequestRequestTypeDef

```python
# ListTagsForProjectRequestRequestTypeDef definition

class ListTagsForProjectRequestRequestTypeDef(TypedDict):
    id: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTeamMembersRequestRequestTypeDef

```python
# ListTeamMembersRequestRequestTypeDef definition

class ListTeamMembersRequestRequestTypeDef(TypedDict):
    projectId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TeamMemberTypeDef

```python
# TeamMemberTypeDef definition

class TeamMemberTypeDef(TypedDict):
    userArn: str,
    projectRole: str,
    remoteAccessAllowed: NotRequired[bool],
```

## ListUserProfilesRequestRequestTypeDef

```python
# ListUserProfilesRequestRequestTypeDef definition

class ListUserProfilesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## UserProfileSummaryTypeDef

```python
# UserProfileSummaryTypeDef definition

class UserProfileSummaryTypeDef(TypedDict):
    userArn: NotRequired[str],
    displayName: NotRequired[str],
    emailAddress: NotRequired[str],
    sshPublicKey: NotRequired[str],
```

## TagProjectRequestRequestTypeDef

```python
# TagProjectRequestRequestTypeDef definition

class TagProjectRequestRequestTypeDef(TypedDict):
    id: str,
    tags: Mapping[str, str],
```

## UntagProjectRequestRequestTypeDef

```python
# UntagProjectRequestRequestTypeDef definition

class UntagProjectRequestRequestTypeDef(TypedDict):
    id: str,
    tags: Sequence[str],
```

## UpdateProjectRequestRequestTypeDef

```python
# UpdateProjectRequestRequestTypeDef definition

class UpdateProjectRequestRequestTypeDef(TypedDict):
    id: str,
    name: NotRequired[str],
    description: NotRequired[str],
```

## UpdateTeamMemberRequestRequestTypeDef

```python
# UpdateTeamMemberRequestRequestTypeDef definition

class UpdateTeamMemberRequestRequestTypeDef(TypedDict):
    projectId: str,
    userArn: str,
    projectRole: NotRequired[str],
    remoteAccessAllowed: NotRequired[bool],
```

## UpdateUserProfileRequestRequestTypeDef

```python
# UpdateUserProfileRequestRequestTypeDef definition

class UpdateUserProfileRequestRequestTypeDef(TypedDict):
    userArn: str,
    displayName: NotRequired[str],
    emailAddress: NotRequired[str],
    sshPublicKey: NotRequired[str],
```

## AssociateTeamMemberResultTypeDef

```python
# AssociateTeamMemberResultTypeDef definition

class AssociateTeamMemberResultTypeDef(TypedDict):
    clientRequestToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectResultTypeDef

```python
# CreateProjectResultTypeDef definition

class CreateProjectResultTypeDef(TypedDict):
    id: str,
    arn: str,
    clientRequestToken: str,
    projectTemplateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserProfileResultTypeDef

```python
# CreateUserProfileResultTypeDef definition

class CreateUserProfileResultTypeDef(TypedDict):
    userArn: str,
    displayName: str,
    emailAddress: str,
    sshPublicKey: str,
    createdTimestamp: datetime,
    lastModifiedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProjectResultTypeDef

```python
# DeleteProjectResultTypeDef definition

class DeleteProjectResultTypeDef(TypedDict):
    stackId: str,
    projectArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteUserProfileResultTypeDef

```python
# DeleteUserProfileResultTypeDef definition

class DeleteUserProfileResultTypeDef(TypedDict):
    userArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserProfileResultTypeDef

```python
# DescribeUserProfileResultTypeDef definition

class DescribeUserProfileResultTypeDef(TypedDict):
    userArn: str,
    displayName: str,
    emailAddress: str,
    sshPublicKey: str,
    createdTimestamp: datetime,
    lastModifiedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForProjectResultTypeDef

```python
# ListTagsForProjectResultTypeDef definition

class ListTagsForProjectResultTypeDef(TypedDict):
    tags: Dict[str, str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagProjectResultTypeDef

```python
# TagProjectResultTypeDef definition

class TagProjectResultTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTeamMemberResultTypeDef

```python
# UpdateTeamMemberResultTypeDef definition

class UpdateTeamMemberResultTypeDef(TypedDict):
    userArn: str,
    projectRole: str,
    remoteAccessAllowed: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserProfileResultTypeDef

```python
# UpdateUserProfileResultTypeDef definition

class UpdateUserProfileResultTypeDef(TypedDict):
    userArn: str,
    displayName: str,
    emailAddress: str,
    sshPublicKey: str,
    createdTimestamp: datetime,
    lastModifiedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CodeDestinationTypeDef

```python
# CodeDestinationTypeDef definition

class CodeDestinationTypeDef(TypedDict):
    codeCommit: NotRequired[CodeCommitCodeDestinationTypeDef],  # (1)
    gitHub: NotRequired[GitHubCodeDestinationTypeDef],  # (2)
```

1. See [:material-code-braces: CodeCommitCodeDestinationTypeDef](./type_defs.md#codecommitcodedestinationtypedef) 
2. See [:material-code-braces: GitHubCodeDestinationTypeDef](./type_defs.md#githubcodedestinationtypedef) 
## CodeSourceTypeDef

```python
# CodeSourceTypeDef definition

class CodeSourceTypeDef(TypedDict):
    s3: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ToolchainSourceTypeDef

```python
# ToolchainSourceTypeDef definition

class ToolchainSourceTypeDef(TypedDict):
    s3: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## DescribeProjectResultTypeDef

```python
# DescribeProjectResultTypeDef definition

class DescribeProjectResultTypeDef(TypedDict):
    name: str,
    id: str,
    arn: str,
    description: str,
    clientRequestToken: str,
    createdTimeStamp: datetime,
    stackId: str,
    projectTemplateId: str,
    status: ProjectStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectStatusTypeDef](./type_defs.md#projectstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectsRequestListProjectsPaginateTypeDef

```python
# ListProjectsRequestListProjectsPaginateTypeDef definition

class ListProjectsRequestListProjectsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourcesRequestListResourcesPaginateTypeDef

```python
# ListResourcesRequestListResourcesPaginateTypeDef definition

class ListResourcesRequestListResourcesPaginateTypeDef(TypedDict):
    projectId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTeamMembersRequestListTeamMembersPaginateTypeDef

```python
# ListTeamMembersRequestListTeamMembersPaginateTypeDef definition

class ListTeamMembersRequestListTeamMembersPaginateTypeDef(TypedDict):
    projectId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserProfilesRequestListUserProfilesPaginateTypeDef

```python
# ListUserProfilesRequestListUserProfilesPaginateTypeDef definition

class ListUserProfilesRequestListUserProfilesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsResultTypeDef

```python
# ListProjectsResultTypeDef definition

class ListProjectsResultTypeDef(TypedDict):
    projects: List[ProjectSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesResultTypeDef

```python
# ListResourcesResultTypeDef definition

class ListResourcesResultTypeDef(TypedDict):
    resources: List[ResourceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTeamMembersResultTypeDef

```python
# ListTeamMembersResultTypeDef definition

class ListTeamMembersResultTypeDef(TypedDict):
    teamMembers: List[TeamMemberTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TeamMemberTypeDef](./type_defs.md#teammembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserProfilesResultTypeDef

```python
# ListUserProfilesResultTypeDef definition

class ListUserProfilesResultTypeDef(TypedDict):
    userProfiles: List[UserProfileSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserProfileSummaryTypeDef](./type_defs.md#userprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CodeTypeDef

```python
# CodeTypeDef definition

class CodeTypeDef(TypedDict):
    source: CodeSourceTypeDef,  # (1)
    destination: CodeDestinationTypeDef,  # (2)
```

1. See [:material-code-braces: CodeSourceTypeDef](./type_defs.md#codesourcetypedef) 
2. See [:material-code-braces: CodeDestinationTypeDef](./type_defs.md#codedestinationtypedef) 
## ToolchainTypeDef

```python
# ToolchainTypeDef definition

class ToolchainTypeDef(TypedDict):
    source: ToolchainSourceTypeDef,  # (1)
    roleArn: NotRequired[str],
    stackParameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ToolchainSourceTypeDef](./type_defs.md#toolchainsourcetypedef) 
## CreateProjectRequestRequestTypeDef

```python
# CreateProjectRequestRequestTypeDef definition

class CreateProjectRequestRequestTypeDef(TypedDict):
    name: str,
    id: str,
    description: NotRequired[str],
    clientRequestToken: NotRequired[str],
    sourceCode: NotRequired[Sequence[CodeTypeDef]],  # (1)
    toolchain: NotRequired[ToolchainTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CodeTypeDef](./type_defs.md#codetypedef) 
2. See [:material-code-braces: ToolchainTypeDef](./type_defs.md#toolchaintypedef) 
