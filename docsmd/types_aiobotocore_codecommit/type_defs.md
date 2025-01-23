# Type definitions

> [Index](../README.md) > [CodeCommit](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeCommit](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#codecommit)
    type annotations stubs module [types-aiobotocore-codecommit](https://pypi.org/project/types-aiobotocore-codecommit/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## RepositoryTriggerUnionTypeDef

```python
# RepositoryTriggerUnionTypeDef definition

RepositoryTriggerUnionTypeDef = Union[
    RepositoryTriggerTypeDef,  # (1)
    RepositoryTriggerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RepositoryTriggerTypeDef](./type_defs.md#repositorytriggertypedef) 
2. See [:material-code-braces: RepositoryTriggerOutputTypeDef](./type_defs.md#repositorytriggeroutputtypedef) 



## ApprovalRuleEventMetadataTypeDef

```python
# ApprovalRuleEventMetadataTypeDef definition

class ApprovalRuleEventMetadataTypeDef(TypedDict):
    approvalRuleName: NotRequired[str],
    approvalRuleId: NotRequired[str],
    approvalRuleContent: NotRequired[str],
```

## ApprovalRuleOverriddenEventMetadataTypeDef

```python
# ApprovalRuleOverriddenEventMetadataTypeDef definition

class ApprovalRuleOverriddenEventMetadataTypeDef(TypedDict):
    revisionId: NotRequired[str],
    overrideStatus: NotRequired[OverrideStatusType],  # (1)
```

1. See [:material-code-brackets: OverrideStatusType](./literals.md#overridestatustype) 
## ApprovalRuleTemplateTypeDef

```python
# ApprovalRuleTemplateTypeDef definition

class ApprovalRuleTemplateTypeDef(TypedDict):
    approvalRuleTemplateId: NotRequired[str],
    approvalRuleTemplateName: NotRequired[str],
    approvalRuleTemplateDescription: NotRequired[str],
    approvalRuleTemplateContent: NotRequired[str],
    ruleContentSha256: NotRequired[str],
    lastModifiedDate: NotRequired[datetime],
    creationDate: NotRequired[datetime],
    lastModifiedUser: NotRequired[str],
```

## OriginApprovalRuleTemplateTypeDef

```python
# OriginApprovalRuleTemplateTypeDef definition

class OriginApprovalRuleTemplateTypeDef(TypedDict):
    approvalRuleTemplateId: NotRequired[str],
    approvalRuleTemplateName: NotRequired[str],
```

## ApprovalStateChangedEventMetadataTypeDef

```python
# ApprovalStateChangedEventMetadataTypeDef definition

class ApprovalStateChangedEventMetadataTypeDef(TypedDict):
    revisionId: NotRequired[str],
    approvalStatus: NotRequired[ApprovalStateType],  # (1)
```

1. See [:material-code-brackets: ApprovalStateType](./literals.md#approvalstatetype) 
## ApprovalTypeDef

```python
# ApprovalTypeDef definition

class ApprovalTypeDef(TypedDict):
    userArn: NotRequired[str],
    approvalState: NotRequired[ApprovalStateType],  # (1)
```

1. See [:material-code-brackets: ApprovalStateType](./literals.md#approvalstatetype) 
## AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef

```python
# AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef definition

class AssociateApprovalRuleTemplateWithRepositoryInputRequestTypeDef(TypedDict):
    approvalRuleTemplateName: str,
    repositoryName: str,
```

## BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef

```python
# BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef definition

class BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

## BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef

```python
# BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef definition

class BatchAssociateApprovalRuleTemplateWithRepositoriesInputRequestTypeDef(TypedDict):
    approvalRuleTemplateName: str,
    repositoryNames: Sequence[str],
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

## BatchDescribeMergeConflictsErrorTypeDef

```python
# BatchDescribeMergeConflictsErrorTypeDef definition

class BatchDescribeMergeConflictsErrorTypeDef(TypedDict):
    filePath: str,
    exceptionName: str,
    message: str,
```

## BatchDescribeMergeConflictsInputRequestTypeDef

```python
# BatchDescribeMergeConflictsInputRequestTypeDef definition

class BatchDescribeMergeConflictsInputRequestTypeDef(TypedDict):
    repositoryName: str,
    destinationCommitSpecifier: str,
    sourceCommitSpecifier: str,
    mergeOption: MergeOptionTypeEnumType,  # (1)
    maxMergeHunks: NotRequired[int],
    maxConflictFiles: NotRequired[int],
    filePaths: NotRequired[Sequence[str]],
    conflictDetailLevel: NotRequired[ConflictDetailLevelTypeEnumType],  # (2)
    conflictResolutionStrategy: NotRequired[ConflictResolutionStrategyTypeEnumType],  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: MergeOptionTypeEnumType](./literals.md#mergeoptiontypeenumtype) 
2. See [:material-code-brackets: ConflictDetailLevelTypeEnumType](./literals.md#conflictdetailleveltypeenumtype) 
3. See [:material-code-brackets: ConflictResolutionStrategyTypeEnumType](./literals.md#conflictresolutionstrategytypeenumtype) 
## BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef

```python
# BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef definition

class BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

## BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef

```python
# BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef definition

class BatchDisassociateApprovalRuleTemplateFromRepositoriesInputRequestTypeDef(TypedDict):
    approvalRuleTemplateName: str,
    repositoryNames: Sequence[str],
```

## BatchGetCommitsErrorTypeDef

```python
# BatchGetCommitsErrorTypeDef definition

class BatchGetCommitsErrorTypeDef(TypedDict):
    commitId: NotRequired[str],
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

## BatchGetCommitsInputRequestTypeDef

```python
# BatchGetCommitsInputRequestTypeDef definition

class BatchGetCommitsInputRequestTypeDef(TypedDict):
    commitIds: Sequence[str],
    repositoryName: str,
```

## BatchGetRepositoriesErrorTypeDef

```python
# BatchGetRepositoriesErrorTypeDef definition

class BatchGetRepositoriesErrorTypeDef(TypedDict):
    repositoryId: NotRequired[str],
    repositoryName: NotRequired[str],
    errorCode: NotRequired[BatchGetRepositoriesErrorCodeEnumType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: BatchGetRepositoriesErrorCodeEnumType](./literals.md#batchgetrepositorieserrorcodeenumtype) 
## BatchGetRepositoriesInputRequestTypeDef

```python
# BatchGetRepositoriesInputRequestTypeDef definition

class BatchGetRepositoriesInputRequestTypeDef(TypedDict):
    repositoryNames: Sequence[str],
```

## RepositoryMetadataTypeDef

```python
# RepositoryMetadataTypeDef definition

class RepositoryMetadataTypeDef(TypedDict):
    accountId: NotRequired[str],
    repositoryId: NotRequired[str],
    repositoryName: NotRequired[str],
    repositoryDescription: NotRequired[str],
    defaultBranch: NotRequired[str],
    lastModifiedDate: NotRequired[datetime],
    creationDate: NotRequired[datetime],
    cloneUrlHttp: NotRequired[str],
    cloneUrlSsh: NotRequired[str],
    Arn: NotRequired[str],
    kmsKeyId: NotRequired[str],
```

## BlobMetadataTypeDef

```python
# BlobMetadataTypeDef definition

class BlobMetadataTypeDef(TypedDict):
    blobId: NotRequired[str],
    path: NotRequired[str],
    mode: NotRequired[str],
```

## BranchInfoTypeDef

```python
# BranchInfoTypeDef definition

class BranchInfoTypeDef(TypedDict):
    branchName: NotRequired[str],
    commitId: NotRequired[str],
```

## CommentTypeDef

```python
# CommentTypeDef definition

class CommentTypeDef(TypedDict):
    commentId: NotRequired[str],
    content: NotRequired[str],
    inReplyTo: NotRequired[str],
    creationDate: NotRequired[datetime],
    lastModifiedDate: NotRequired[datetime],
    authorArn: NotRequired[str],
    deleted: NotRequired[bool],
    clientRequestToken: NotRequired[str],
    callerReactions: NotRequired[List[str]],
    reactionCounts: NotRequired[Dict[str, int]],
```

## LocationTypeDef

```python
# LocationTypeDef definition

class LocationTypeDef(TypedDict):
    filePath: NotRequired[str],
    filePosition: NotRequired[int],
    relativeFileVersion: NotRequired[RelativeFileVersionEnumType],  # (1)
```

1. See [:material-code-brackets: RelativeFileVersionEnumType](./literals.md#relativefileversionenumtype) 
## UserInfoTypeDef

```python
# UserInfoTypeDef definition

class UserInfoTypeDef(TypedDict):
    name: NotRequired[str],
    email: NotRequired[str],
    date: NotRequired[str],
```

## FileModesTypeDef

```python
# FileModesTypeDef definition

class FileModesTypeDef(TypedDict):
    source: NotRequired[FileModeTypeEnumType],  # (1)
    destination: NotRequired[FileModeTypeEnumType],  # (1)
    base: NotRequired[FileModeTypeEnumType],  # (1)
```

1. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
2. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
3. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
## FileSizesTypeDef

```python
# FileSizesTypeDef definition

class FileSizesTypeDef(TypedDict):
    source: NotRequired[int],
    destination: NotRequired[int],
    base: NotRequired[int],
```

## IsBinaryFileTypeDef

```python
# IsBinaryFileTypeDef definition

class IsBinaryFileTypeDef(TypedDict):
    source: NotRequired[bool],
    destination: NotRequired[bool],
    base: NotRequired[bool],
```

## MergeOperationsTypeDef

```python
# MergeOperationsTypeDef definition

class MergeOperationsTypeDef(TypedDict):
    source: NotRequired[ChangeTypeEnumType],  # (1)
    destination: NotRequired[ChangeTypeEnumType],  # (1)
```

1. See [:material-code-brackets: ChangeTypeEnumType](./literals.md#changetypeenumtype) 
2. See [:material-code-brackets: ChangeTypeEnumType](./literals.md#changetypeenumtype) 
## ObjectTypesTypeDef

```python
# ObjectTypesTypeDef definition

class ObjectTypesTypeDef(TypedDict):
    source: NotRequired[ObjectTypeEnumType],  # (1)
    destination: NotRequired[ObjectTypeEnumType],  # (1)
    base: NotRequired[ObjectTypeEnumType],  # (1)
```

1. See [:material-code-brackets: ObjectTypeEnumType](./literals.md#objecttypeenumtype) 
2. See [:material-code-brackets: ObjectTypeEnumType](./literals.md#objecttypeenumtype) 
3. See [:material-code-brackets: ObjectTypeEnumType](./literals.md#objecttypeenumtype) 
## DeleteFileEntryTypeDef

```python
# DeleteFileEntryTypeDef definition

class DeleteFileEntryTypeDef(TypedDict):
    filePath: str,
```

## SetFileModeEntryTypeDef

```python
# SetFileModeEntryTypeDef definition

class SetFileModeEntryTypeDef(TypedDict):
    filePath: str,
    fileMode: FileModeTypeEnumType,  # (1)
```

1. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
## CreateApprovalRuleTemplateInputRequestTypeDef

```python
# CreateApprovalRuleTemplateInputRequestTypeDef definition

class CreateApprovalRuleTemplateInputRequestTypeDef(TypedDict):
    approvalRuleTemplateName: str,
    approvalRuleTemplateContent: str,
    approvalRuleTemplateDescription: NotRequired[str],
```

## CreateBranchInputRequestTypeDef

```python
# CreateBranchInputRequestTypeDef definition

class CreateBranchInputRequestTypeDef(TypedDict):
    repositoryName: str,
    branchName: str,
    commitId: str,
```

## FileMetadataTypeDef

```python
# FileMetadataTypeDef definition

class FileMetadataTypeDef(TypedDict):
    absolutePath: NotRequired[str],
    blobId: NotRequired[str],
    fileMode: NotRequired[FileModeTypeEnumType],  # (1)
```

1. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
## CreatePullRequestApprovalRuleInputRequestTypeDef

```python
# CreatePullRequestApprovalRuleInputRequestTypeDef definition

class CreatePullRequestApprovalRuleInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    approvalRuleName: str,
    approvalRuleContent: str,
```

## TargetTypeDef

```python
# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    repositoryName: str,
    sourceReference: str,
    destinationReference: NotRequired[str],
```

## CreateRepositoryInputRequestTypeDef

```python
# CreateRepositoryInputRequestTypeDef definition

class CreateRepositoryInputRequestTypeDef(TypedDict):
    repositoryName: str,
    repositoryDescription: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    kmsKeyId: NotRequired[str],
```

## DeleteApprovalRuleTemplateInputRequestTypeDef

```python
# DeleteApprovalRuleTemplateInputRequestTypeDef definition

class DeleteApprovalRuleTemplateInputRequestTypeDef(TypedDict):
    approvalRuleTemplateName: str,
```

## DeleteBranchInputRequestTypeDef

```python
# DeleteBranchInputRequestTypeDef definition

class DeleteBranchInputRequestTypeDef(TypedDict):
    repositoryName: str,
    branchName: str,
```

## DeleteCommentContentInputRequestTypeDef

```python
# DeleteCommentContentInputRequestTypeDef definition

class DeleteCommentContentInputRequestTypeDef(TypedDict):
    commentId: str,
```

## DeleteFileInputRequestTypeDef

```python
# DeleteFileInputRequestTypeDef definition

class DeleteFileInputRequestTypeDef(TypedDict):
    repositoryName: str,
    branchName: str,
    filePath: str,
    parentCommitId: str,
    keepEmptyFolders: NotRequired[bool],
    commitMessage: NotRequired[str],
    name: NotRequired[str],
    email: NotRequired[str],
```

## DeletePullRequestApprovalRuleInputRequestTypeDef

```python
# DeletePullRequestApprovalRuleInputRequestTypeDef definition

class DeletePullRequestApprovalRuleInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    approvalRuleName: str,
```

## DeleteRepositoryInputRequestTypeDef

```python
# DeleteRepositoryInputRequestTypeDef definition

class DeleteRepositoryInputRequestTypeDef(TypedDict):
    repositoryName: str,
```

## DescribeMergeConflictsInputRequestTypeDef

```python
# DescribeMergeConflictsInputRequestTypeDef definition

class DescribeMergeConflictsInputRequestTypeDef(TypedDict):
    repositoryName: str,
    destinationCommitSpecifier: str,
    sourceCommitSpecifier: str,
    mergeOption: MergeOptionTypeEnumType,  # (1)
    filePath: str,
    maxMergeHunks: NotRequired[int],
    conflictDetailLevel: NotRequired[ConflictDetailLevelTypeEnumType],  # (2)
    conflictResolutionStrategy: NotRequired[ConflictResolutionStrategyTypeEnumType],  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: MergeOptionTypeEnumType](./literals.md#mergeoptiontypeenumtype) 
2. See [:material-code-brackets: ConflictDetailLevelTypeEnumType](./literals.md#conflictdetailleveltypeenumtype) 
3. See [:material-code-brackets: ConflictResolutionStrategyTypeEnumType](./literals.md#conflictresolutionstrategytypeenumtype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribePullRequestEventsInputRequestTypeDef

```python
# DescribePullRequestEventsInputRequestTypeDef definition

class DescribePullRequestEventsInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    pullRequestEventType: NotRequired[PullRequestEventTypeType],  # (1)
    actorArn: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: PullRequestEventTypeType](./literals.md#pullrequesteventtypetype) 
## DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef

```python
# DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef definition

class DisassociateApprovalRuleTemplateFromRepositoryInputRequestTypeDef(TypedDict):
    approvalRuleTemplateName: str,
    repositoryName: str,
```

## EvaluatePullRequestApprovalRulesInputRequestTypeDef

```python
# EvaluatePullRequestApprovalRulesInputRequestTypeDef definition

class EvaluatePullRequestApprovalRulesInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    revisionId: str,
```

## EvaluationTypeDef

```python
# EvaluationTypeDef definition

class EvaluationTypeDef(TypedDict):
    approved: NotRequired[bool],
    overridden: NotRequired[bool],
    approvalRulesSatisfied: NotRequired[List[str]],
    approvalRulesNotSatisfied: NotRequired[List[str]],
```

## FileTypeDef

```python
# FileTypeDef definition

class FileTypeDef(TypedDict):
    blobId: NotRequired[str],
    absolutePath: NotRequired[str],
    relativePath: NotRequired[str],
    fileMode: NotRequired[FileModeTypeEnumType],  # (1)
```

1. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
## FolderTypeDef

```python
# FolderTypeDef definition

class FolderTypeDef(TypedDict):
    treeId: NotRequired[str],
    absolutePath: NotRequired[str],
    relativePath: NotRequired[str],
```

## GetApprovalRuleTemplateInputRequestTypeDef

```python
# GetApprovalRuleTemplateInputRequestTypeDef definition

class GetApprovalRuleTemplateInputRequestTypeDef(TypedDict):
    approvalRuleTemplateName: str,
```

## GetBlobInputRequestTypeDef

```python
# GetBlobInputRequestTypeDef definition

class GetBlobInputRequestTypeDef(TypedDict):
    repositoryName: str,
    blobId: str,
```

## GetBranchInputRequestTypeDef

```python
# GetBranchInputRequestTypeDef definition

class GetBranchInputRequestTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    branchName: NotRequired[str],
```

## GetCommentInputRequestTypeDef

```python
# GetCommentInputRequestTypeDef definition

class GetCommentInputRequestTypeDef(TypedDict):
    commentId: str,
```

## GetCommentReactionsInputRequestTypeDef

```python
# GetCommentReactionsInputRequestTypeDef definition

class GetCommentReactionsInputRequestTypeDef(TypedDict):
    commentId: str,
    reactionUserArn: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetCommentsForComparedCommitInputRequestTypeDef

```python
# GetCommentsForComparedCommitInputRequestTypeDef definition

class GetCommentsForComparedCommitInputRequestTypeDef(TypedDict):
    repositoryName: str,
    afterCommitId: str,
    beforeCommitId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetCommentsForPullRequestInputRequestTypeDef

```python
# GetCommentsForPullRequestInputRequestTypeDef definition

class GetCommentsForPullRequestInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    repositoryName: NotRequired[str],
    beforeCommitId: NotRequired[str],
    afterCommitId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetCommitInputRequestTypeDef

```python
# GetCommitInputRequestTypeDef definition

class GetCommitInputRequestTypeDef(TypedDict):
    repositoryName: str,
    commitId: str,
```

## GetDifferencesInputRequestTypeDef

```python
# GetDifferencesInputRequestTypeDef definition

class GetDifferencesInputRequestTypeDef(TypedDict):
    repositoryName: str,
    afterCommitSpecifier: str,
    beforeCommitSpecifier: NotRequired[str],
    beforePath: NotRequired[str],
    afterPath: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetFileInputRequestTypeDef

```python
# GetFileInputRequestTypeDef definition

class GetFileInputRequestTypeDef(TypedDict):
    repositoryName: str,
    filePath: str,
    commitSpecifier: NotRequired[str],
```

## GetFolderInputRequestTypeDef

```python
# GetFolderInputRequestTypeDef definition

class GetFolderInputRequestTypeDef(TypedDict):
    repositoryName: str,
    folderPath: str,
    commitSpecifier: NotRequired[str],
```

## SubModuleTypeDef

```python
# SubModuleTypeDef definition

class SubModuleTypeDef(TypedDict):
    commitId: NotRequired[str],
    absolutePath: NotRequired[str],
    relativePath: NotRequired[str],
```

## SymbolicLinkTypeDef

```python
# SymbolicLinkTypeDef definition

class SymbolicLinkTypeDef(TypedDict):
    blobId: NotRequired[str],
    absolutePath: NotRequired[str],
    relativePath: NotRequired[str],
    fileMode: NotRequired[FileModeTypeEnumType],  # (1)
```

1. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
## GetMergeCommitInputRequestTypeDef

```python
# GetMergeCommitInputRequestTypeDef definition

class GetMergeCommitInputRequestTypeDef(TypedDict):
    repositoryName: str,
    sourceCommitSpecifier: str,
    destinationCommitSpecifier: str,
    conflictDetailLevel: NotRequired[ConflictDetailLevelTypeEnumType],  # (1)
    conflictResolutionStrategy: NotRequired[ConflictResolutionStrategyTypeEnumType],  # (2)
```

1. See [:material-code-brackets: ConflictDetailLevelTypeEnumType](./literals.md#conflictdetailleveltypeenumtype) 
2. See [:material-code-brackets: ConflictResolutionStrategyTypeEnumType](./literals.md#conflictresolutionstrategytypeenumtype) 
## GetMergeConflictsInputRequestTypeDef

```python
# GetMergeConflictsInputRequestTypeDef definition

class GetMergeConflictsInputRequestTypeDef(TypedDict):
    repositoryName: str,
    destinationCommitSpecifier: str,
    sourceCommitSpecifier: str,
    mergeOption: MergeOptionTypeEnumType,  # (1)
    conflictDetailLevel: NotRequired[ConflictDetailLevelTypeEnumType],  # (2)
    maxConflictFiles: NotRequired[int],
    conflictResolutionStrategy: NotRequired[ConflictResolutionStrategyTypeEnumType],  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: MergeOptionTypeEnumType](./literals.md#mergeoptiontypeenumtype) 
2. See [:material-code-brackets: ConflictDetailLevelTypeEnumType](./literals.md#conflictdetailleveltypeenumtype) 
3. See [:material-code-brackets: ConflictResolutionStrategyTypeEnumType](./literals.md#conflictresolutionstrategytypeenumtype) 
## GetMergeOptionsInputRequestTypeDef

```python
# GetMergeOptionsInputRequestTypeDef definition

class GetMergeOptionsInputRequestTypeDef(TypedDict):
    repositoryName: str,
    sourceCommitSpecifier: str,
    destinationCommitSpecifier: str,
    conflictDetailLevel: NotRequired[ConflictDetailLevelTypeEnumType],  # (1)
    conflictResolutionStrategy: NotRequired[ConflictResolutionStrategyTypeEnumType],  # (2)
```

1. See [:material-code-brackets: ConflictDetailLevelTypeEnumType](./literals.md#conflictdetailleveltypeenumtype) 
2. See [:material-code-brackets: ConflictResolutionStrategyTypeEnumType](./literals.md#conflictresolutionstrategytypeenumtype) 
## GetPullRequestApprovalStatesInputRequestTypeDef

```python
# GetPullRequestApprovalStatesInputRequestTypeDef definition

class GetPullRequestApprovalStatesInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    revisionId: str,
```

## GetPullRequestInputRequestTypeDef

```python
# GetPullRequestInputRequestTypeDef definition

class GetPullRequestInputRequestTypeDef(TypedDict):
    pullRequestId: str,
```

## GetPullRequestOverrideStateInputRequestTypeDef

```python
# GetPullRequestOverrideStateInputRequestTypeDef definition

class GetPullRequestOverrideStateInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    revisionId: str,
```

## GetRepositoryInputRequestTypeDef

```python
# GetRepositoryInputRequestTypeDef definition

class GetRepositoryInputRequestTypeDef(TypedDict):
    repositoryName: str,
```

## GetRepositoryTriggersInputRequestTypeDef

```python
# GetRepositoryTriggersInputRequestTypeDef definition

class GetRepositoryTriggersInputRequestTypeDef(TypedDict):
    repositoryName: str,
```

## RepositoryTriggerOutputTypeDef

```python
# RepositoryTriggerOutputTypeDef definition

class RepositoryTriggerOutputTypeDef(TypedDict):
    name: str,
    destinationArn: str,
    events: List[RepositoryTriggerEventEnumType],  # (1)
    customData: NotRequired[str],
    branches: NotRequired[List[str]],
```

1. See [:material-code-brackets: RepositoryTriggerEventEnumType](./literals.md#repositorytriggereventenumtype) 
## ListApprovalRuleTemplatesInputRequestTypeDef

```python
# ListApprovalRuleTemplatesInputRequestTypeDef definition

class ListApprovalRuleTemplatesInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef

```python
# ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef definition

class ListAssociatedApprovalRuleTemplatesForRepositoryInputRequestTypeDef(TypedDict):
    repositoryName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListBranchesInputRequestTypeDef

```python
# ListBranchesInputRequestTypeDef definition

class ListBranchesInputRequestTypeDef(TypedDict):
    repositoryName: str,
    nextToken: NotRequired[str],
```

## ListFileCommitHistoryRequestRequestTypeDef

```python
# ListFileCommitHistoryRequestRequestTypeDef definition

class ListFileCommitHistoryRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    filePath: str,
    commitSpecifier: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListPullRequestsInputRequestTypeDef

```python
# ListPullRequestsInputRequestTypeDef definition

class ListPullRequestsInputRequestTypeDef(TypedDict):
    repositoryName: str,
    authorArn: NotRequired[str],
    pullRequestStatus: NotRequired[PullRequestStatusEnumType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: PullRequestStatusEnumType](./literals.md#pullrequeststatusenumtype) 
## ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef

```python
# ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef definition

class ListRepositoriesForApprovalRuleTemplateInputRequestTypeDef(TypedDict):
    approvalRuleTemplateName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListRepositoriesInputRequestTypeDef

```python
# ListRepositoriesInputRequestTypeDef definition

class ListRepositoriesInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortByEnumType],  # (1)
    order: NotRequired[OrderEnumType],  # (2)
```

1. See [:material-code-brackets: SortByEnumType](./literals.md#sortbyenumtype) 
2. See [:material-code-brackets: OrderEnumType](./literals.md#orderenumtype) 
## RepositoryNameIdPairTypeDef

```python
# RepositoryNameIdPairTypeDef definition

class RepositoryNameIdPairTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    repositoryId: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    nextToken: NotRequired[str],
```

## MergeBranchesByFastForwardInputRequestTypeDef

```python
# MergeBranchesByFastForwardInputRequestTypeDef definition

class MergeBranchesByFastForwardInputRequestTypeDef(TypedDict):
    repositoryName: str,
    sourceCommitSpecifier: str,
    destinationCommitSpecifier: str,
    targetBranch: NotRequired[str],
```

## MergeHunkDetailTypeDef

```python
# MergeHunkDetailTypeDef definition

class MergeHunkDetailTypeDef(TypedDict):
    startLine: NotRequired[int],
    endLine: NotRequired[int],
    hunkContent: NotRequired[str],
```

## MergeMetadataTypeDef

```python
# MergeMetadataTypeDef definition

class MergeMetadataTypeDef(TypedDict):
    isMerged: NotRequired[bool],
    mergedBy: NotRequired[str],
    mergeCommitId: NotRequired[str],
    mergeOption: NotRequired[MergeOptionTypeEnumType],  # (1)
```

1. See [:material-code-brackets: MergeOptionTypeEnumType](./literals.md#mergeoptiontypeenumtype) 
## MergePullRequestByFastForwardInputRequestTypeDef

```python
# MergePullRequestByFastForwardInputRequestTypeDef definition

class MergePullRequestByFastForwardInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    repositoryName: str,
    sourceCommitId: NotRequired[str],
```

## OverridePullRequestApprovalRulesInputRequestTypeDef

```python
# OverridePullRequestApprovalRulesInputRequestTypeDef definition

class OverridePullRequestApprovalRulesInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    revisionId: str,
    overrideStatus: OverrideStatusType,  # (1)
```

1. See [:material-code-brackets: OverrideStatusType](./literals.md#overridestatustype) 
## PostCommentReplyInputRequestTypeDef

```python
# PostCommentReplyInputRequestTypeDef definition

class PostCommentReplyInputRequestTypeDef(TypedDict):
    inReplyTo: str,
    content: str,
    clientRequestToken: NotRequired[str],
```

## PullRequestCreatedEventMetadataTypeDef

```python
# PullRequestCreatedEventMetadataTypeDef definition

class PullRequestCreatedEventMetadataTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    sourceCommitId: NotRequired[str],
    destinationCommitId: NotRequired[str],
    mergeBase: NotRequired[str],
```

## PullRequestSourceReferenceUpdatedEventMetadataTypeDef

```python
# PullRequestSourceReferenceUpdatedEventMetadataTypeDef definition

class PullRequestSourceReferenceUpdatedEventMetadataTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    beforeCommitId: NotRequired[str],
    afterCommitId: NotRequired[str],
    mergeBase: NotRequired[str],
```

## PullRequestStatusChangedEventMetadataTypeDef

```python
# PullRequestStatusChangedEventMetadataTypeDef definition

class PullRequestStatusChangedEventMetadataTypeDef(TypedDict):
    pullRequestStatus: NotRequired[PullRequestStatusEnumType],  # (1)
```

1. See [:material-code-brackets: PullRequestStatusEnumType](./literals.md#pullrequeststatusenumtype) 
## PutCommentReactionInputRequestTypeDef

```python
# PutCommentReactionInputRequestTypeDef definition

class PutCommentReactionInputRequestTypeDef(TypedDict):
    commentId: str,
    reactionValue: str,
```

## SourceFileSpecifierTypeDef

```python
# SourceFileSpecifierTypeDef definition

class SourceFileSpecifierTypeDef(TypedDict):
    filePath: str,
    isMove: NotRequired[bool],
```

## ReactionValueFormatsTypeDef

```python
# ReactionValueFormatsTypeDef definition

class ReactionValueFormatsTypeDef(TypedDict):
    emoji: NotRequired[str],
    shortCode: NotRequired[str],
    unicode: NotRequired[str],
```

## RepositoryTriggerExecutionFailureTypeDef

```python
# RepositoryTriggerExecutionFailureTypeDef definition

class RepositoryTriggerExecutionFailureTypeDef(TypedDict):
    trigger: NotRequired[str],
    failureMessage: NotRequired[str],
```

## RepositoryTriggerTypeDef

```python
# RepositoryTriggerTypeDef definition

class RepositoryTriggerTypeDef(TypedDict):
    name: str,
    destinationArn: str,
    events: Sequence[RepositoryTriggerEventEnumType],  # (1)
    customData: NotRequired[str],
    branches: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: RepositoryTriggerEventEnumType](./literals.md#repositorytriggereventenumtype) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateApprovalRuleTemplateContentInputRequestTypeDef

```python
# UpdateApprovalRuleTemplateContentInputRequestTypeDef definition

class UpdateApprovalRuleTemplateContentInputRequestTypeDef(TypedDict):
    approvalRuleTemplateName: str,
    newRuleContent: str,
    existingRuleContentSha256: NotRequired[str],
```

## UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef

```python
# UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef definition

class UpdateApprovalRuleTemplateDescriptionInputRequestTypeDef(TypedDict):
    approvalRuleTemplateName: str,
    approvalRuleTemplateDescription: str,
```

## UpdateApprovalRuleTemplateNameInputRequestTypeDef

```python
# UpdateApprovalRuleTemplateNameInputRequestTypeDef definition

class UpdateApprovalRuleTemplateNameInputRequestTypeDef(TypedDict):
    oldApprovalRuleTemplateName: str,
    newApprovalRuleTemplateName: str,
```

## UpdateCommentInputRequestTypeDef

```python
# UpdateCommentInputRequestTypeDef definition

class UpdateCommentInputRequestTypeDef(TypedDict):
    commentId: str,
    content: str,
```

## UpdateDefaultBranchInputRequestTypeDef

```python
# UpdateDefaultBranchInputRequestTypeDef definition

class UpdateDefaultBranchInputRequestTypeDef(TypedDict):
    repositoryName: str,
    defaultBranchName: str,
```

## UpdatePullRequestApprovalRuleContentInputRequestTypeDef

```python
# UpdatePullRequestApprovalRuleContentInputRequestTypeDef definition

class UpdatePullRequestApprovalRuleContentInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    approvalRuleName: str,
    newRuleContent: str,
    existingRuleContentSha256: NotRequired[str],
```

## UpdatePullRequestApprovalStateInputRequestTypeDef

```python
# UpdatePullRequestApprovalStateInputRequestTypeDef definition

class UpdatePullRequestApprovalStateInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    revisionId: str,
    approvalState: ApprovalStateType,  # (1)
```

1. See [:material-code-brackets: ApprovalStateType](./literals.md#approvalstatetype) 
## UpdatePullRequestDescriptionInputRequestTypeDef

```python
# UpdatePullRequestDescriptionInputRequestTypeDef definition

class UpdatePullRequestDescriptionInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    description: str,
```

## UpdatePullRequestStatusInputRequestTypeDef

```python
# UpdatePullRequestStatusInputRequestTypeDef definition

class UpdatePullRequestStatusInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    pullRequestStatus: PullRequestStatusEnumType,  # (1)
```

1. See [:material-code-brackets: PullRequestStatusEnumType](./literals.md#pullrequeststatusenumtype) 
## UpdatePullRequestTitleInputRequestTypeDef

```python
# UpdatePullRequestTitleInputRequestTypeDef definition

class UpdatePullRequestTitleInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    title: str,
```

## UpdateRepositoryDescriptionInputRequestTypeDef

```python
# UpdateRepositoryDescriptionInputRequestTypeDef definition

class UpdateRepositoryDescriptionInputRequestTypeDef(TypedDict):
    repositoryName: str,
    repositoryDescription: NotRequired[str],
```

## UpdateRepositoryEncryptionKeyInputRequestTypeDef

```python
# UpdateRepositoryEncryptionKeyInputRequestTypeDef definition

class UpdateRepositoryEncryptionKeyInputRequestTypeDef(TypedDict):
    repositoryName: str,
    kmsKeyId: str,
```

## UpdateRepositoryNameInputRequestTypeDef

```python
# UpdateRepositoryNameInputRequestTypeDef definition

class UpdateRepositoryNameInputRequestTypeDef(TypedDict):
    oldName: str,
    newName: str,
```

## ApprovalRuleTypeDef

```python
# ApprovalRuleTypeDef definition

class ApprovalRuleTypeDef(TypedDict):
    approvalRuleId: NotRequired[str],
    approvalRuleName: NotRequired[str],
    approvalRuleContent: NotRequired[str],
    ruleContentSha256: NotRequired[str],
    lastModifiedDate: NotRequired[datetime],
    creationDate: NotRequired[datetime],
    lastModifiedUser: NotRequired[str],
    originApprovalRuleTemplate: NotRequired[OriginApprovalRuleTemplateTypeDef],  # (1)
```

1. See [:material-code-braces: OriginApprovalRuleTemplateTypeDef](./type_defs.md#originapprovalruletemplatetypedef) 
## BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef

```python
# BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef definition

class BatchAssociateApprovalRuleTemplateWithRepositoriesOutputTypeDef(TypedDict):
    associatedRepositoryNames: List[str],
    errors: List[BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchAssociateApprovalRuleTemplateWithRepositoriesErrorTypeDef](./type_defs.md#batchassociateapprovalruletemplatewithrepositorieserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApprovalRuleTemplateOutputTypeDef

```python
# CreateApprovalRuleTemplateOutputTypeDef definition

class CreateApprovalRuleTemplateOutputTypeDef(TypedDict):
    approvalRuleTemplate: ApprovalRuleTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApprovalRuleTemplateTypeDef](./type_defs.md#approvalruletemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUnreferencedMergeCommitOutputTypeDef

```python
# CreateUnreferencedMergeCommitOutputTypeDef definition

class CreateUnreferencedMergeCommitOutputTypeDef(TypedDict):
    commitId: str,
    treeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApprovalRuleTemplateOutputTypeDef

```python
# DeleteApprovalRuleTemplateOutputTypeDef definition

class DeleteApprovalRuleTemplateOutputTypeDef(TypedDict):
    approvalRuleTemplateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFileOutputTypeDef

```python
# DeleteFileOutputTypeDef definition

class DeleteFileOutputTypeDef(TypedDict):
    commitId: str,
    blobId: str,
    treeId: str,
    filePath: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePullRequestApprovalRuleOutputTypeDef

```python
# DeletePullRequestApprovalRuleOutputTypeDef definition

class DeletePullRequestApprovalRuleOutputTypeDef(TypedDict):
    approvalRuleId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRepositoryOutputTypeDef

```python
# DeleteRepositoryOutputTypeDef definition

class DeleteRepositoryOutputTypeDef(TypedDict):
    repositoryId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApprovalRuleTemplateOutputTypeDef

```python
# GetApprovalRuleTemplateOutputTypeDef definition

class GetApprovalRuleTemplateOutputTypeDef(TypedDict):
    approvalRuleTemplate: ApprovalRuleTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApprovalRuleTemplateTypeDef](./type_defs.md#approvalruletemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlobOutputTypeDef

```python
# GetBlobOutputTypeDef definition

class GetBlobOutputTypeDef(TypedDict):
    content: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFileOutputTypeDef

```python
# GetFileOutputTypeDef definition

class GetFileOutputTypeDef(TypedDict):
    commitId: str,
    blobId: str,
    filePath: str,
    fileMode: FileModeTypeEnumType,  # (1)
    fileSize: int,
    fileContent: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMergeCommitOutputTypeDef

```python
# GetMergeCommitOutputTypeDef definition

class GetMergeCommitOutputTypeDef(TypedDict):
    sourceCommitId: str,
    destinationCommitId: str,
    baseCommitId: str,
    mergedCommitId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMergeOptionsOutputTypeDef

```python
# GetMergeOptionsOutputTypeDef definition

class GetMergeOptionsOutputTypeDef(TypedDict):
    mergeOptions: List[MergeOptionTypeEnumType],  # (1)
    sourceCommitId: str,
    destinationCommitId: str,
    baseCommitId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MergeOptionTypeEnumType](./literals.md#mergeoptiontypeenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPullRequestApprovalStatesOutputTypeDef

```python
# GetPullRequestApprovalStatesOutputTypeDef definition

class GetPullRequestApprovalStatesOutputTypeDef(TypedDict):
    approvals: List[ApprovalTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApprovalTypeDef](./type_defs.md#approvaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPullRequestOverrideStateOutputTypeDef

```python
# GetPullRequestOverrideStateOutputTypeDef definition

class GetPullRequestOverrideStateOutputTypeDef(TypedDict):
    overridden: bool,
    overrider: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApprovalRuleTemplatesOutputTypeDef

```python
# ListApprovalRuleTemplatesOutputTypeDef definition

class ListApprovalRuleTemplatesOutputTypeDef(TypedDict):
    approvalRuleTemplateNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef

```python
# ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef definition

class ListAssociatedApprovalRuleTemplatesForRepositoryOutputTypeDef(TypedDict):
    approvalRuleTemplateNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBranchesOutputTypeDef

```python
# ListBranchesOutputTypeDef definition

class ListBranchesOutputTypeDef(TypedDict):
    branches: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPullRequestsOutputTypeDef

```python
# ListPullRequestsOutputTypeDef definition

class ListPullRequestsOutputTypeDef(TypedDict):
    pullRequestIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRepositoriesForApprovalRuleTemplateOutputTypeDef

```python
# ListRepositoriesForApprovalRuleTemplateOutputTypeDef definition

class ListRepositoriesForApprovalRuleTemplateOutputTypeDef(TypedDict):
    repositoryNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MergeBranchesByFastForwardOutputTypeDef

```python
# MergeBranchesByFastForwardOutputTypeDef definition

class MergeBranchesByFastForwardOutputTypeDef(TypedDict):
    commitId: str,
    treeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MergeBranchesBySquashOutputTypeDef

```python
# MergeBranchesBySquashOutputTypeDef definition

class MergeBranchesBySquashOutputTypeDef(TypedDict):
    commitId: str,
    treeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MergeBranchesByThreeWayOutputTypeDef

```python
# MergeBranchesByThreeWayOutputTypeDef definition

class MergeBranchesByThreeWayOutputTypeDef(TypedDict):
    commitId: str,
    treeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutFileOutputTypeDef

```python
# PutFileOutputTypeDef definition

class PutFileOutputTypeDef(TypedDict):
    commitId: str,
    blobId: str,
    treeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRepositoryTriggersOutputTypeDef

```python
# PutRepositoryTriggersOutputTypeDef definition

class PutRepositoryTriggersOutputTypeDef(TypedDict):
    configurationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApprovalRuleTemplateContentOutputTypeDef

```python
# UpdateApprovalRuleTemplateContentOutputTypeDef definition

class UpdateApprovalRuleTemplateContentOutputTypeDef(TypedDict):
    approvalRuleTemplate: ApprovalRuleTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApprovalRuleTemplateTypeDef](./type_defs.md#approvalruletemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApprovalRuleTemplateDescriptionOutputTypeDef

```python
# UpdateApprovalRuleTemplateDescriptionOutputTypeDef definition

class UpdateApprovalRuleTemplateDescriptionOutputTypeDef(TypedDict):
    approvalRuleTemplate: ApprovalRuleTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApprovalRuleTemplateTypeDef](./type_defs.md#approvalruletemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApprovalRuleTemplateNameOutputTypeDef

```python
# UpdateApprovalRuleTemplateNameOutputTypeDef definition

class UpdateApprovalRuleTemplateNameOutputTypeDef(TypedDict):
    approvalRuleTemplate: ApprovalRuleTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApprovalRuleTemplateTypeDef](./type_defs.md#approvalruletemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRepositoryEncryptionKeyOutputTypeDef

```python
# UpdateRepositoryEncryptionKeyOutputTypeDef definition

class UpdateRepositoryEncryptionKeyOutputTypeDef(TypedDict):
    repositoryId: str,
    kmsKeyId: str,
    originalKmsKeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef

```python
# BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef definition

class BatchDisassociateApprovalRuleTemplateFromRepositoriesOutputTypeDef(TypedDict):
    disassociatedRepositoryNames: List[str],
    errors: List[BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDisassociateApprovalRuleTemplateFromRepositoriesErrorTypeDef](./type_defs.md#batchdisassociateapprovalruletemplatefromrepositorieserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetRepositoriesOutputTypeDef

```python
# BatchGetRepositoriesOutputTypeDef definition

class BatchGetRepositoriesOutputTypeDef(TypedDict):
    repositories: List[RepositoryMetadataTypeDef],  # (1)
    repositoriesNotFound: List[str],
    errors: List[BatchGetRepositoriesErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RepositoryMetadataTypeDef](./type_defs.md#repositorymetadatatypedef) 
2. See [:material-code-braces: BatchGetRepositoriesErrorTypeDef](./type_defs.md#batchgetrepositorieserrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRepositoryOutputTypeDef

```python
# CreateRepositoryOutputTypeDef definition

class CreateRepositoryOutputTypeDef(TypedDict):
    repositoryMetadata: RepositoryMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryMetadataTypeDef](./type_defs.md#repositorymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRepositoryOutputTypeDef

```python
# GetRepositoryOutputTypeDef definition

class GetRepositoryOutputTypeDef(TypedDict):
    repositoryMetadata: RepositoryMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryMetadataTypeDef](./type_defs.md#repositorymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DifferenceTypeDef

```python
# DifferenceTypeDef definition

class DifferenceTypeDef(TypedDict):
    beforeBlob: NotRequired[BlobMetadataTypeDef],  # (1)
    afterBlob: NotRequired[BlobMetadataTypeDef],  # (1)
    changeType: NotRequired[ChangeTypeEnumType],  # (3)
```

1. See [:material-code-braces: BlobMetadataTypeDef](./type_defs.md#blobmetadatatypedef) 
2. See [:material-code-braces: BlobMetadataTypeDef](./type_defs.md#blobmetadatatypedef) 
3. See [:material-code-brackets: ChangeTypeEnumType](./literals.md#changetypeenumtype) 
## PutFileInputRequestTypeDef

```python
# PutFileInputRequestTypeDef definition

class PutFileInputRequestTypeDef(TypedDict):
    repositoryName: str,
    branchName: str,
    fileContent: BlobTypeDef,
    filePath: str,
    fileMode: NotRequired[FileModeTypeEnumType],  # (1)
    parentCommitId: NotRequired[str],
    commitMessage: NotRequired[str],
    name: NotRequired[str],
    email: NotRequired[str],
```

1. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
## ReplaceContentEntryTypeDef

```python
# ReplaceContentEntryTypeDef definition

class ReplaceContentEntryTypeDef(TypedDict):
    filePath: str,
    replacementType: ReplacementTypeEnumType,  # (1)
    content: NotRequired[BlobTypeDef],
    fileMode: NotRequired[FileModeTypeEnumType],  # (2)
```

1. See [:material-code-brackets: ReplacementTypeEnumType](./literals.md#replacementtypeenumtype) 
2. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
## DeleteBranchOutputTypeDef

```python
# DeleteBranchOutputTypeDef definition

class DeleteBranchOutputTypeDef(TypedDict):
    deletedBranch: BranchInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BranchInfoTypeDef](./type_defs.md#branchinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBranchOutputTypeDef

```python
# GetBranchOutputTypeDef definition

class GetBranchOutputTypeDef(TypedDict):
    branch: BranchInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BranchInfoTypeDef](./type_defs.md#branchinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCommentContentOutputTypeDef

```python
# DeleteCommentContentOutputTypeDef definition

class DeleteCommentContentOutputTypeDef(TypedDict):
    comment: CommentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCommentOutputTypeDef

```python
# GetCommentOutputTypeDef definition

class GetCommentOutputTypeDef(TypedDict):
    comment: CommentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PostCommentReplyOutputTypeDef

```python
# PostCommentReplyOutputTypeDef definition

class PostCommentReplyOutputTypeDef(TypedDict):
    comment: CommentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCommentOutputTypeDef

```python
# UpdateCommentOutputTypeDef definition

class UpdateCommentOutputTypeDef(TypedDict):
    comment: CommentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CommentsForComparedCommitTypeDef

```python
# CommentsForComparedCommitTypeDef definition

class CommentsForComparedCommitTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    beforeCommitId: NotRequired[str],
    afterCommitId: NotRequired[str],
    beforeBlobId: NotRequired[str],
    afterBlobId: NotRequired[str],
    location: NotRequired[LocationTypeDef],  # (1)
    comments: NotRequired[List[CommentTypeDef]],  # (2)
```

1. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
2. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
## CommentsForPullRequestTypeDef

```python
# CommentsForPullRequestTypeDef definition

class CommentsForPullRequestTypeDef(TypedDict):
    pullRequestId: NotRequired[str],
    repositoryName: NotRequired[str],
    beforeCommitId: NotRequired[str],
    afterCommitId: NotRequired[str],
    beforeBlobId: NotRequired[str],
    afterBlobId: NotRequired[str],
    location: NotRequired[LocationTypeDef],  # (1)
    comments: NotRequired[List[CommentTypeDef]],  # (2)
```

1. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
2. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
## PostCommentForComparedCommitInputRequestTypeDef

```python
# PostCommentForComparedCommitInputRequestTypeDef definition

class PostCommentForComparedCommitInputRequestTypeDef(TypedDict):
    repositoryName: str,
    afterCommitId: str,
    content: str,
    beforeCommitId: NotRequired[str],
    location: NotRequired[LocationTypeDef],  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
## PostCommentForComparedCommitOutputTypeDef

```python
# PostCommentForComparedCommitOutputTypeDef definition

class PostCommentForComparedCommitOutputTypeDef(TypedDict):
    repositoryName: str,
    beforeCommitId: str,
    afterCommitId: str,
    beforeBlobId: str,
    afterBlobId: str,
    location: LocationTypeDef,  # (1)
    comment: CommentTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
2. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PostCommentForPullRequestInputRequestTypeDef

```python
# PostCommentForPullRequestInputRequestTypeDef definition

class PostCommentForPullRequestInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    repositoryName: str,
    beforeCommitId: str,
    afterCommitId: str,
    content: str,
    location: NotRequired[LocationTypeDef],  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
## PostCommentForPullRequestOutputTypeDef

```python
# PostCommentForPullRequestOutputTypeDef definition

class PostCommentForPullRequestOutputTypeDef(TypedDict):
    repositoryName: str,
    pullRequestId: str,
    beforeCommitId: str,
    afterCommitId: str,
    beforeBlobId: str,
    afterBlobId: str,
    location: LocationTypeDef,  # (1)
    comment: CommentTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
2. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CommitTypeDef

```python
# CommitTypeDef definition

class CommitTypeDef(TypedDict):
    commitId: NotRequired[str],
    treeId: NotRequired[str],
    parents: NotRequired[List[str]],
    message: NotRequired[str],
    author: NotRequired[UserInfoTypeDef],  # (1)
    committer: NotRequired[UserInfoTypeDef],  # (1)
    additionalData: NotRequired[str],
```

1. See [:material-code-braces: UserInfoTypeDef](./type_defs.md#userinfotypedef) 
2. See [:material-code-braces: UserInfoTypeDef](./type_defs.md#userinfotypedef) 
## ConflictMetadataTypeDef

```python
# ConflictMetadataTypeDef definition

class ConflictMetadataTypeDef(TypedDict):
    filePath: NotRequired[str],
    fileSizes: NotRequired[FileSizesTypeDef],  # (1)
    fileModes: NotRequired[FileModesTypeDef],  # (2)
    objectTypes: NotRequired[ObjectTypesTypeDef],  # (3)
    numberOfConflicts: NotRequired[int],
    isBinaryFile: NotRequired[IsBinaryFileTypeDef],  # (4)
    contentConflict: NotRequired[bool],
    fileModeConflict: NotRequired[bool],
    objectTypeConflict: NotRequired[bool],
    mergeOperations: NotRequired[MergeOperationsTypeDef],  # (5)
```

1. See [:material-code-braces: FileSizesTypeDef](./type_defs.md#filesizestypedef) 
2. See [:material-code-braces: FileModesTypeDef](./type_defs.md#filemodestypedef) 
3. See [:material-code-braces: ObjectTypesTypeDef](./type_defs.md#objecttypestypedef) 
4. See [:material-code-braces: IsBinaryFileTypeDef](./type_defs.md#isbinaryfiletypedef) 
5. See [:material-code-braces: MergeOperationsTypeDef](./type_defs.md#mergeoperationstypedef) 
## CreateCommitOutputTypeDef

```python
# CreateCommitOutputTypeDef definition

class CreateCommitOutputTypeDef(TypedDict):
    commitId: str,
    treeId: str,
    filesAdded: List[FileMetadataTypeDef],  # (1)
    filesUpdated: List[FileMetadataTypeDef],  # (1)
    filesDeleted: List[FileMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: FileMetadataTypeDef](./type_defs.md#filemetadatatypedef) 
2. See [:material-code-braces: FileMetadataTypeDef](./type_defs.md#filemetadatatypedef) 
3. See [:material-code-braces: FileMetadataTypeDef](./type_defs.md#filemetadatatypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePullRequestInputRequestTypeDef

```python
# CreatePullRequestInputRequestTypeDef definition

class CreatePullRequestInputRequestTypeDef(TypedDict):
    title: str,
    targets: Sequence[TargetTypeDef],  # (1)
    description: NotRequired[str],
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## DescribePullRequestEventsInputPaginateTypeDef

```python
# DescribePullRequestEventsInputPaginateTypeDef definition

class DescribePullRequestEventsInputPaginateTypeDef(TypedDict):
    pullRequestId: str,
    pullRequestEventType: NotRequired[PullRequestEventTypeType],  # (1)
    actorArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PullRequestEventTypeType](./literals.md#pullrequesteventtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCommentsForComparedCommitInputPaginateTypeDef

```python
# GetCommentsForComparedCommitInputPaginateTypeDef definition

class GetCommentsForComparedCommitInputPaginateTypeDef(TypedDict):
    repositoryName: str,
    afterCommitId: str,
    beforeCommitId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCommentsForPullRequestInputPaginateTypeDef

```python
# GetCommentsForPullRequestInputPaginateTypeDef definition

class GetCommentsForPullRequestInputPaginateTypeDef(TypedDict):
    pullRequestId: str,
    repositoryName: NotRequired[str],
    beforeCommitId: NotRequired[str],
    afterCommitId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDifferencesInputPaginateTypeDef

```python
# GetDifferencesInputPaginateTypeDef definition

class GetDifferencesInputPaginateTypeDef(TypedDict):
    repositoryName: str,
    afterCommitSpecifier: str,
    beforeCommitSpecifier: NotRequired[str],
    beforePath: NotRequired[str],
    afterPath: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBranchesInputPaginateTypeDef

```python
# ListBranchesInputPaginateTypeDef definition

class ListBranchesInputPaginateTypeDef(TypedDict):
    repositoryName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPullRequestsInputPaginateTypeDef

```python
# ListPullRequestsInputPaginateTypeDef definition

class ListPullRequestsInputPaginateTypeDef(TypedDict):
    repositoryName: str,
    authorArn: NotRequired[str],
    pullRequestStatus: NotRequired[PullRequestStatusEnumType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PullRequestStatusEnumType](./literals.md#pullrequeststatusenumtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRepositoriesInputPaginateTypeDef

```python
# ListRepositoriesInputPaginateTypeDef definition

class ListRepositoriesInputPaginateTypeDef(TypedDict):
    sortBy: NotRequired[SortByEnumType],  # (1)
    order: NotRequired[OrderEnumType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortByEnumType](./literals.md#sortbyenumtype) 
2. See [:material-code-brackets: OrderEnumType](./literals.md#orderenumtype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## EvaluatePullRequestApprovalRulesOutputTypeDef

```python
# EvaluatePullRequestApprovalRulesOutputTypeDef definition

class EvaluatePullRequestApprovalRulesOutputTypeDef(TypedDict):
    evaluation: EvaluationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationTypeDef](./type_defs.md#evaluationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFolderOutputTypeDef

```python
# GetFolderOutputTypeDef definition

class GetFolderOutputTypeDef(TypedDict):
    commitId: str,
    folderPath: str,
    treeId: str,
    subFolders: List[FolderTypeDef],  # (1)
    files: List[FileTypeDef],  # (2)
    symbolicLinks: List[SymbolicLinkTypeDef],  # (3)
    subModules: List[SubModuleTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: FolderTypeDef](./type_defs.md#foldertypedef) 
2. See [:material-code-braces: FileTypeDef](./type_defs.md#filetypedef) 
3. See [:material-code-braces: SymbolicLinkTypeDef](./type_defs.md#symboliclinktypedef) 
4. See [:material-code-braces: SubModuleTypeDef](./type_defs.md#submoduletypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRepositoryTriggersOutputTypeDef

```python
# GetRepositoryTriggersOutputTypeDef definition

class GetRepositoryTriggersOutputTypeDef(TypedDict):
    configurationId: str,
    triggers: List[RepositoryTriggerOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryTriggerOutputTypeDef](./type_defs.md#repositorytriggeroutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRepositoriesOutputTypeDef

```python
# ListRepositoriesOutputTypeDef definition

class ListRepositoriesOutputTypeDef(TypedDict):
    repositories: List[RepositoryNameIdPairTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RepositoryNameIdPairTypeDef](./type_defs.md#repositorynameidpairtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MergeHunkTypeDef

```python
# MergeHunkTypeDef definition

class MergeHunkTypeDef(TypedDict):
    isConflict: NotRequired[bool],
    source: NotRequired[MergeHunkDetailTypeDef],  # (1)
    destination: NotRequired[MergeHunkDetailTypeDef],  # (1)
    base: NotRequired[MergeHunkDetailTypeDef],  # (1)
```

1. See [:material-code-braces: MergeHunkDetailTypeDef](./type_defs.md#mergehunkdetailtypedef) 
2. See [:material-code-braces: MergeHunkDetailTypeDef](./type_defs.md#mergehunkdetailtypedef) 
3. See [:material-code-braces: MergeHunkDetailTypeDef](./type_defs.md#mergehunkdetailtypedef) 
## PullRequestMergedStateChangedEventMetadataTypeDef

```python
# PullRequestMergedStateChangedEventMetadataTypeDef definition

class PullRequestMergedStateChangedEventMetadataTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    destinationReference: NotRequired[str],
    mergeMetadata: NotRequired[MergeMetadataTypeDef],  # (1)
```

1. See [:material-code-braces: MergeMetadataTypeDef](./type_defs.md#mergemetadatatypedef) 
## PullRequestTargetTypeDef

```python
# PullRequestTargetTypeDef definition

class PullRequestTargetTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    sourceReference: NotRequired[str],
    destinationReference: NotRequired[str],
    destinationCommit: NotRequired[str],
    sourceCommit: NotRequired[str],
    mergeBase: NotRequired[str],
    mergeMetadata: NotRequired[MergeMetadataTypeDef],  # (1)
```

1. See [:material-code-braces: MergeMetadataTypeDef](./type_defs.md#mergemetadatatypedef) 
## PutFileEntryTypeDef

```python
# PutFileEntryTypeDef definition

class PutFileEntryTypeDef(TypedDict):
    filePath: str,
    fileMode: NotRequired[FileModeTypeEnumType],  # (1)
    fileContent: NotRequired[BlobTypeDef],
    sourceFile: NotRequired[SourceFileSpecifierTypeDef],  # (2)
```

1. See [:material-code-brackets: FileModeTypeEnumType](./literals.md#filemodetypeenumtype) 
2. See [:material-code-braces: SourceFileSpecifierTypeDef](./type_defs.md#sourcefilespecifiertypedef) 
## ReactionForCommentTypeDef

```python
# ReactionForCommentTypeDef definition

class ReactionForCommentTypeDef(TypedDict):
    reaction: NotRequired[ReactionValueFormatsTypeDef],  # (1)
    reactionUsers: NotRequired[List[str]],
    reactionsFromDeletedUsersCount: NotRequired[int],
```

1. See [:material-code-braces: ReactionValueFormatsTypeDef](./type_defs.md#reactionvalueformatstypedef) 
## TestRepositoryTriggersOutputTypeDef

```python
# TestRepositoryTriggersOutputTypeDef definition

class TestRepositoryTriggersOutputTypeDef(TypedDict):
    successfulExecutions: List[str],
    failedExecutions: List[RepositoryTriggerExecutionFailureTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryTriggerExecutionFailureTypeDef](./type_defs.md#repositorytriggerexecutionfailuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestRepositoryTriggersInputRequestTypeDef

```python
# TestRepositoryTriggersInputRequestTypeDef definition

class TestRepositoryTriggersInputRequestTypeDef(TypedDict):
    repositoryName: str,
    triggers: Sequence[RepositoryTriggerTypeDef],  # (1)
```

1. See [:material-code-braces: RepositoryTriggerTypeDef](./type_defs.md#repositorytriggertypedef) 
## CreatePullRequestApprovalRuleOutputTypeDef

```python
# CreatePullRequestApprovalRuleOutputTypeDef definition

class CreatePullRequestApprovalRuleOutputTypeDef(TypedDict):
    approvalRule: ApprovalRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApprovalRuleTypeDef](./type_defs.md#approvalruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePullRequestApprovalRuleContentOutputTypeDef

```python
# UpdatePullRequestApprovalRuleContentOutputTypeDef definition

class UpdatePullRequestApprovalRuleContentOutputTypeDef(TypedDict):
    approvalRule: ApprovalRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApprovalRuleTypeDef](./type_defs.md#approvalruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDifferencesOutputTypeDef

```python
# GetDifferencesOutputTypeDef definition

class GetDifferencesOutputTypeDef(TypedDict):
    differences: List[DifferenceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DifferenceTypeDef](./type_defs.md#differencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConflictResolutionTypeDef

```python
# ConflictResolutionTypeDef definition

class ConflictResolutionTypeDef(TypedDict):
    replaceContents: NotRequired[Sequence[ReplaceContentEntryTypeDef]],  # (1)
    deleteFiles: NotRequired[Sequence[DeleteFileEntryTypeDef]],  # (2)
    setFileModes: NotRequired[Sequence[SetFileModeEntryTypeDef]],  # (3)
```

1. See [:material-code-braces: ReplaceContentEntryTypeDef](./type_defs.md#replacecontententrytypedef) 
2. See [:material-code-braces: DeleteFileEntryTypeDef](./type_defs.md#deletefileentrytypedef) 
3. See [:material-code-braces: SetFileModeEntryTypeDef](./type_defs.md#setfilemodeentrytypedef) 
## GetCommentsForComparedCommitOutputTypeDef

```python
# GetCommentsForComparedCommitOutputTypeDef definition

class GetCommentsForComparedCommitOutputTypeDef(TypedDict):
    commentsForComparedCommitData: List[CommentsForComparedCommitTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CommentsForComparedCommitTypeDef](./type_defs.md#commentsforcomparedcommittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCommentsForPullRequestOutputTypeDef

```python
# GetCommentsForPullRequestOutputTypeDef definition

class GetCommentsForPullRequestOutputTypeDef(TypedDict):
    commentsForPullRequestData: List[CommentsForPullRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CommentsForPullRequestTypeDef](./type_defs.md#commentsforpullrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetCommitsOutputTypeDef

```python
# BatchGetCommitsOutputTypeDef definition

class BatchGetCommitsOutputTypeDef(TypedDict):
    commits: List[CommitTypeDef],  # (1)
    errors: List[BatchGetCommitsErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CommitTypeDef](./type_defs.md#committypedef) 
2. See [:material-code-braces: BatchGetCommitsErrorTypeDef](./type_defs.md#batchgetcommitserrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FileVersionTypeDef

```python
# FileVersionTypeDef definition

class FileVersionTypeDef(TypedDict):
    commit: NotRequired[CommitTypeDef],  # (1)
    blobId: NotRequired[str],
    path: NotRequired[str],
    revisionChildren: NotRequired[List[str]],
```

1. See [:material-code-braces: CommitTypeDef](./type_defs.md#committypedef) 
## GetCommitOutputTypeDef

```python
# GetCommitOutputTypeDef definition

class GetCommitOutputTypeDef(TypedDict):
    commit: CommitTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommitTypeDef](./type_defs.md#committypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMergeConflictsOutputTypeDef

```python
# GetMergeConflictsOutputTypeDef definition

class GetMergeConflictsOutputTypeDef(TypedDict):
    mergeable: bool,
    destinationCommitId: str,
    sourceCommitId: str,
    baseCommitId: str,
    conflictMetadataList: List[ConflictMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConflictMetadataTypeDef](./type_defs.md#conflictmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConflictTypeDef

```python
# ConflictTypeDef definition

class ConflictTypeDef(TypedDict):
    conflictMetadata: NotRequired[ConflictMetadataTypeDef],  # (1)
    mergeHunks: NotRequired[List[MergeHunkTypeDef]],  # (2)
```

1. See [:material-code-braces: ConflictMetadataTypeDef](./type_defs.md#conflictmetadatatypedef) 
2. See [:material-code-braces: MergeHunkTypeDef](./type_defs.md#mergehunktypedef) 
## DescribeMergeConflictsOutputTypeDef

```python
# DescribeMergeConflictsOutputTypeDef definition

class DescribeMergeConflictsOutputTypeDef(TypedDict):
    conflictMetadata: ConflictMetadataTypeDef,  # (1)
    mergeHunks: List[MergeHunkTypeDef],  # (2)
    destinationCommitId: str,
    sourceCommitId: str,
    baseCommitId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConflictMetadataTypeDef](./type_defs.md#conflictmetadatatypedef) 
2. See [:material-code-braces: MergeHunkTypeDef](./type_defs.md#mergehunktypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PullRequestEventTypeDef

```python
# PullRequestEventTypeDef definition

class PullRequestEventTypeDef(TypedDict):
    pullRequestId: NotRequired[str],
    eventDate: NotRequired[datetime],
    pullRequestEventType: NotRequired[PullRequestEventTypeType],  # (1)
    actorArn: NotRequired[str],
    pullRequestCreatedEventMetadata: NotRequired[PullRequestCreatedEventMetadataTypeDef],  # (2)
    pullRequestStatusChangedEventMetadata: NotRequired[PullRequestStatusChangedEventMetadataTypeDef],  # (3)
    pullRequestSourceReferenceUpdatedEventMetadata: NotRequired[PullRequestSourceReferenceUpdatedEventMetadataTypeDef],  # (4)
    pullRequestMergedStateChangedEventMetadata: NotRequired[PullRequestMergedStateChangedEventMetadataTypeDef],  # (5)
    approvalRuleEventMetadata: NotRequired[ApprovalRuleEventMetadataTypeDef],  # (6)
    approvalStateChangedEventMetadata: NotRequired[ApprovalStateChangedEventMetadataTypeDef],  # (7)
    approvalRuleOverriddenEventMetadata: NotRequired[ApprovalRuleOverriddenEventMetadataTypeDef],  # (8)
```

1. See [:material-code-brackets: PullRequestEventTypeType](./literals.md#pullrequesteventtypetype) 
2. See [:material-code-braces: PullRequestCreatedEventMetadataTypeDef](./type_defs.md#pullrequestcreatedeventmetadatatypedef) 
3. See [:material-code-braces: PullRequestStatusChangedEventMetadataTypeDef](./type_defs.md#pullrequeststatuschangedeventmetadatatypedef) 
4. See [:material-code-braces: PullRequestSourceReferenceUpdatedEventMetadataTypeDef](./type_defs.md#pullrequestsourcereferenceupdatedeventmetadatatypedef) 
5. See [:material-code-braces: PullRequestMergedStateChangedEventMetadataTypeDef](./type_defs.md#pullrequestmergedstatechangedeventmetadatatypedef) 
6. See [:material-code-braces: ApprovalRuleEventMetadataTypeDef](./type_defs.md#approvalruleeventmetadatatypedef) 
7. See [:material-code-braces: ApprovalStateChangedEventMetadataTypeDef](./type_defs.md#approvalstatechangedeventmetadatatypedef) 
8. See [:material-code-braces: ApprovalRuleOverriddenEventMetadataTypeDef](./type_defs.md#approvalruleoverriddeneventmetadatatypedef) 
## PullRequestTypeDef

```python
# PullRequestTypeDef definition

class PullRequestTypeDef(TypedDict):
    pullRequestId: NotRequired[str],
    title: NotRequired[str],
    description: NotRequired[str],
    lastActivityDate: NotRequired[datetime],
    creationDate: NotRequired[datetime],
    pullRequestStatus: NotRequired[PullRequestStatusEnumType],  # (1)
    authorArn: NotRequired[str],
    pullRequestTargets: NotRequired[List[PullRequestTargetTypeDef]],  # (2)
    clientRequestToken: NotRequired[str],
    revisionId: NotRequired[str],
    approvalRules: NotRequired[List[ApprovalRuleTypeDef]],  # (3)
```

1. See [:material-code-brackets: PullRequestStatusEnumType](./literals.md#pullrequeststatusenumtype) 
2. See [:material-code-braces: PullRequestTargetTypeDef](./type_defs.md#pullrequesttargettypedef) 
3. See [:material-code-braces: ApprovalRuleTypeDef](./type_defs.md#approvalruletypedef) 
## CreateCommitInputRequestTypeDef

```python
# CreateCommitInputRequestTypeDef definition

class CreateCommitInputRequestTypeDef(TypedDict):
    repositoryName: str,
    branchName: str,
    parentCommitId: NotRequired[str],
    authorName: NotRequired[str],
    email: NotRequired[str],
    commitMessage: NotRequired[str],
    keepEmptyFolders: NotRequired[bool],
    putFiles: NotRequired[Sequence[PutFileEntryTypeDef]],  # (1)
    deleteFiles: NotRequired[Sequence[DeleteFileEntryTypeDef]],  # (2)
    setFileModes: NotRequired[Sequence[SetFileModeEntryTypeDef]],  # (3)
```

1. See [:material-code-braces: PutFileEntryTypeDef](./type_defs.md#putfileentrytypedef) 
2. See [:material-code-braces: DeleteFileEntryTypeDef](./type_defs.md#deletefileentrytypedef) 
3. See [:material-code-braces: SetFileModeEntryTypeDef](./type_defs.md#setfilemodeentrytypedef) 
## GetCommentReactionsOutputTypeDef

```python
# GetCommentReactionsOutputTypeDef definition

class GetCommentReactionsOutputTypeDef(TypedDict):
    reactionsForComment: List[ReactionForCommentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReactionForCommentTypeDef](./type_defs.md#reactionforcommenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRepositoryTriggersInputRequestTypeDef

```python
# PutRepositoryTriggersInputRequestTypeDef definition

class PutRepositoryTriggersInputRequestTypeDef(TypedDict):
    repositoryName: str,
    triggers: Sequence[RepositoryTriggerUnionTypeDef],  # (1)
```

1. See [:material-code-braces: RepositoryTriggerTypeDef](./type_defs.md#repositorytriggertypedef) [:material-code-braces: RepositoryTriggerOutputTypeDef](./type_defs.md#repositorytriggeroutputtypedef) 
## CreateUnreferencedMergeCommitInputRequestTypeDef

```python
# CreateUnreferencedMergeCommitInputRequestTypeDef definition

class CreateUnreferencedMergeCommitInputRequestTypeDef(TypedDict):
    repositoryName: str,
    sourceCommitSpecifier: str,
    destinationCommitSpecifier: str,
    mergeOption: MergeOptionTypeEnumType,  # (1)
    conflictDetailLevel: NotRequired[ConflictDetailLevelTypeEnumType],  # (2)
    conflictResolutionStrategy: NotRequired[ConflictResolutionStrategyTypeEnumType],  # (3)
    authorName: NotRequired[str],
    email: NotRequired[str],
    commitMessage: NotRequired[str],
    keepEmptyFolders: NotRequired[bool],
    conflictResolution: NotRequired[ConflictResolutionTypeDef],  # (4)
```

1. See [:material-code-brackets: MergeOptionTypeEnumType](./literals.md#mergeoptiontypeenumtype) 
2. See [:material-code-brackets: ConflictDetailLevelTypeEnumType](./literals.md#conflictdetailleveltypeenumtype) 
3. See [:material-code-brackets: ConflictResolutionStrategyTypeEnumType](./literals.md#conflictresolutionstrategytypeenumtype) 
4. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
## MergeBranchesBySquashInputRequestTypeDef

```python
# MergeBranchesBySquashInputRequestTypeDef definition

class MergeBranchesBySquashInputRequestTypeDef(TypedDict):
    repositoryName: str,
    sourceCommitSpecifier: str,
    destinationCommitSpecifier: str,
    targetBranch: NotRequired[str],
    conflictDetailLevel: NotRequired[ConflictDetailLevelTypeEnumType],  # (1)
    conflictResolutionStrategy: NotRequired[ConflictResolutionStrategyTypeEnumType],  # (2)
    authorName: NotRequired[str],
    email: NotRequired[str],
    commitMessage: NotRequired[str],
    keepEmptyFolders: NotRequired[bool],
    conflictResolution: NotRequired[ConflictResolutionTypeDef],  # (3)
```

1. See [:material-code-brackets: ConflictDetailLevelTypeEnumType](./literals.md#conflictdetailleveltypeenumtype) 
2. See [:material-code-brackets: ConflictResolutionStrategyTypeEnumType](./literals.md#conflictresolutionstrategytypeenumtype) 
3. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
## MergeBranchesByThreeWayInputRequestTypeDef

```python
# MergeBranchesByThreeWayInputRequestTypeDef definition

class MergeBranchesByThreeWayInputRequestTypeDef(TypedDict):
    repositoryName: str,
    sourceCommitSpecifier: str,
    destinationCommitSpecifier: str,
    targetBranch: NotRequired[str],
    conflictDetailLevel: NotRequired[ConflictDetailLevelTypeEnumType],  # (1)
    conflictResolutionStrategy: NotRequired[ConflictResolutionStrategyTypeEnumType],  # (2)
    authorName: NotRequired[str],
    email: NotRequired[str],
    commitMessage: NotRequired[str],
    keepEmptyFolders: NotRequired[bool],
    conflictResolution: NotRequired[ConflictResolutionTypeDef],  # (3)
```

1. See [:material-code-brackets: ConflictDetailLevelTypeEnumType](./literals.md#conflictdetailleveltypeenumtype) 
2. See [:material-code-brackets: ConflictResolutionStrategyTypeEnumType](./literals.md#conflictresolutionstrategytypeenumtype) 
3. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
## MergePullRequestBySquashInputRequestTypeDef

```python
# MergePullRequestBySquashInputRequestTypeDef definition

class MergePullRequestBySquashInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    repositoryName: str,
    sourceCommitId: NotRequired[str],
    conflictDetailLevel: NotRequired[ConflictDetailLevelTypeEnumType],  # (1)
    conflictResolutionStrategy: NotRequired[ConflictResolutionStrategyTypeEnumType],  # (2)
    commitMessage: NotRequired[str],
    authorName: NotRequired[str],
    email: NotRequired[str],
    keepEmptyFolders: NotRequired[bool],
    conflictResolution: NotRequired[ConflictResolutionTypeDef],  # (3)
```

1. See [:material-code-brackets: ConflictDetailLevelTypeEnumType](./literals.md#conflictdetailleveltypeenumtype) 
2. See [:material-code-brackets: ConflictResolutionStrategyTypeEnumType](./literals.md#conflictresolutionstrategytypeenumtype) 
3. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
## MergePullRequestByThreeWayInputRequestTypeDef

```python
# MergePullRequestByThreeWayInputRequestTypeDef definition

class MergePullRequestByThreeWayInputRequestTypeDef(TypedDict):
    pullRequestId: str,
    repositoryName: str,
    sourceCommitId: NotRequired[str],
    conflictDetailLevel: NotRequired[ConflictDetailLevelTypeEnumType],  # (1)
    conflictResolutionStrategy: NotRequired[ConflictResolutionStrategyTypeEnumType],  # (2)
    commitMessage: NotRequired[str],
    authorName: NotRequired[str],
    email: NotRequired[str],
    keepEmptyFolders: NotRequired[bool],
    conflictResolution: NotRequired[ConflictResolutionTypeDef],  # (3)
```

1. See [:material-code-brackets: ConflictDetailLevelTypeEnumType](./literals.md#conflictdetailleveltypeenumtype) 
2. See [:material-code-brackets: ConflictResolutionStrategyTypeEnumType](./literals.md#conflictresolutionstrategytypeenumtype) 
3. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
## ListFileCommitHistoryResponseTypeDef

```python
# ListFileCommitHistoryResponseTypeDef definition

class ListFileCommitHistoryResponseTypeDef(TypedDict):
    revisionDag: List[FileVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FileVersionTypeDef](./type_defs.md#fileversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDescribeMergeConflictsOutputTypeDef

```python
# BatchDescribeMergeConflictsOutputTypeDef definition

class BatchDescribeMergeConflictsOutputTypeDef(TypedDict):
    conflicts: List[ConflictTypeDef],  # (1)
    errors: List[BatchDescribeMergeConflictsErrorTypeDef],  # (2)
    destinationCommitId: str,
    sourceCommitId: str,
    baseCommitId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConflictTypeDef](./type_defs.md#conflicttypedef) 
2. See [:material-code-braces: BatchDescribeMergeConflictsErrorTypeDef](./type_defs.md#batchdescribemergeconflictserrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePullRequestEventsOutputTypeDef

```python
# DescribePullRequestEventsOutputTypeDef definition

class DescribePullRequestEventsOutputTypeDef(TypedDict):
    pullRequestEvents: List[PullRequestEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PullRequestEventTypeDef](./type_defs.md#pullrequesteventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePullRequestOutputTypeDef

```python
# CreatePullRequestOutputTypeDef definition

class CreatePullRequestOutputTypeDef(TypedDict):
    pullRequest: PullRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PullRequestTypeDef](./type_defs.md#pullrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPullRequestOutputTypeDef

```python
# GetPullRequestOutputTypeDef definition

class GetPullRequestOutputTypeDef(TypedDict):
    pullRequest: PullRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PullRequestTypeDef](./type_defs.md#pullrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MergePullRequestByFastForwardOutputTypeDef

```python
# MergePullRequestByFastForwardOutputTypeDef definition

class MergePullRequestByFastForwardOutputTypeDef(TypedDict):
    pullRequest: PullRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PullRequestTypeDef](./type_defs.md#pullrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MergePullRequestBySquashOutputTypeDef

```python
# MergePullRequestBySquashOutputTypeDef definition

class MergePullRequestBySquashOutputTypeDef(TypedDict):
    pullRequest: PullRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PullRequestTypeDef](./type_defs.md#pullrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MergePullRequestByThreeWayOutputTypeDef

```python
# MergePullRequestByThreeWayOutputTypeDef definition

class MergePullRequestByThreeWayOutputTypeDef(TypedDict):
    pullRequest: PullRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PullRequestTypeDef](./type_defs.md#pullrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePullRequestDescriptionOutputTypeDef

```python
# UpdatePullRequestDescriptionOutputTypeDef definition

class UpdatePullRequestDescriptionOutputTypeDef(TypedDict):
    pullRequest: PullRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PullRequestTypeDef](./type_defs.md#pullrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePullRequestStatusOutputTypeDef

```python
# UpdatePullRequestStatusOutputTypeDef definition

class UpdatePullRequestStatusOutputTypeDef(TypedDict):
    pullRequest: PullRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PullRequestTypeDef](./type_defs.md#pullrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePullRequestTitleOutputTypeDef

```python
# UpdatePullRequestTitleOutputTypeDef definition

class UpdatePullRequestTitleOutputTypeDef(TypedDict):
    pullRequest: PullRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PullRequestTypeDef](./type_defs.md#pullrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
