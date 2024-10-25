# Type definitions

> [Index](../README.md) > [CodeGuruReviewer](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer)
    type annotations stubs module [types-aiobotocore-codeguru-reviewer](https://pypi.org/project/types-aiobotocore-codeguru-reviewer/).



## KMSKeyDetailsTypeDef

```python
# KMSKeyDetailsTypeDef definition

class KMSKeyDetailsTypeDef(TypedDict):
    KMSKeyId: NotRequired[str],
    EncryptionOption: NotRequired[EncryptionOptionType],  # (1)
```

1. See [:material-code-brackets: EncryptionOptionType](./literals.md#encryptionoptiontype) 
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

## BranchDiffSourceCodeTypeTypeDef

```python
# BranchDiffSourceCodeTypeTypeDef definition

class BranchDiffSourceCodeTypeTypeDef(TypedDict):
    SourceBranchName: str,
    DestinationBranchName: str,
```

## CodeArtifactsTypeDef

```python
# CodeArtifactsTypeDef definition

class CodeArtifactsTypeDef(TypedDict):
    SourceCodeArtifactsObjectKey: str,
    BuildArtifactsObjectKey: NotRequired[str],
```

## CodeCommitRepositoryTypeDef

```python
# CodeCommitRepositoryTypeDef definition

class CodeCommitRepositoryTypeDef(TypedDict):
    Name: str,
```

## MetricsSummaryTypeDef

```python
# MetricsSummaryTypeDef definition

class MetricsSummaryTypeDef(TypedDict):
    MeteredLinesOfCodeCount: NotRequired[int],
    SuppressedLinesOfCodeCount: NotRequired[int],
    FindingsCount: NotRequired[int],
```

## MetricsTypeDef

```python
# MetricsTypeDef definition

class MetricsTypeDef(TypedDict):
    MeteredLinesOfCodeCount: NotRequired[int],
    SuppressedLinesOfCodeCount: NotRequired[int],
    FindingsCount: NotRequired[int],
```

## CommitDiffSourceCodeTypeTypeDef

```python
# CommitDiffSourceCodeTypeTypeDef definition

class CommitDiffSourceCodeTypeTypeDef(TypedDict):
    SourceCommit: NotRequired[str],
    DestinationCommit: NotRequired[str],
    MergeBaseCommit: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeCodeReviewRequestRequestTypeDef

```python
# DescribeCodeReviewRequestRequestTypeDef definition

class DescribeCodeReviewRequestRequestTypeDef(TypedDict):
    CodeReviewArn: str,
```

## DescribeRecommendationFeedbackRequestRequestTypeDef

```python
# DescribeRecommendationFeedbackRequestRequestTypeDef definition

class DescribeRecommendationFeedbackRequestRequestTypeDef(TypedDict):
    CodeReviewArn: str,
    RecommendationId: str,
    UserId: NotRequired[str],
```

## RecommendationFeedbackTypeDef

```python
# RecommendationFeedbackTypeDef definition

class RecommendationFeedbackTypeDef(TypedDict):
    CodeReviewArn: NotRequired[str],
    RecommendationId: NotRequired[str],
    Reactions: NotRequired[List[ReactionType]],  # (1)
    UserId: NotRequired[str],
    CreatedTimeStamp: NotRequired[datetime],
    LastUpdatedTimeStamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ReactionType](./literals.md#reactiontype) 
## DescribeRepositoryAssociationRequestRequestTypeDef

```python
# DescribeRepositoryAssociationRequestRequestTypeDef definition

class DescribeRepositoryAssociationRequestRequestTypeDef(TypedDict):
    AssociationArn: str,
```

## DisassociateRepositoryRequestRequestTypeDef

```python
# DisassociateRepositoryRequestRequestTypeDef definition

class DisassociateRepositoryRequestRequestTypeDef(TypedDict):
    AssociationArn: str,
```

## EventInfoTypeDef

```python
# EventInfoTypeDef definition

class EventInfoTypeDef(TypedDict):
    Name: NotRequired[str],
    State: NotRequired[str],
```

## ListCodeReviewsRequestRequestTypeDef

```python
# ListCodeReviewsRequestRequestTypeDef definition

class ListCodeReviewsRequestRequestTypeDef(TypedDict):
    Type: TypeType,  # (1)
    ProviderTypes: NotRequired[Sequence[ProviderTypeType]],  # (2)
    States: NotRequired[Sequence[JobStateType]],  # (3)
    RepositoryNames: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
3. See [:material-code-brackets: JobStateType](./literals.md#jobstatetype) 
## ListRecommendationFeedbackRequestRequestTypeDef

```python
# ListRecommendationFeedbackRequestRequestTypeDef definition

class ListRecommendationFeedbackRequestRequestTypeDef(TypedDict):
    CodeReviewArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    UserIds: NotRequired[Sequence[str]],
    RecommendationIds: NotRequired[Sequence[str]],
```

## RecommendationFeedbackSummaryTypeDef

```python
# RecommendationFeedbackSummaryTypeDef definition

class RecommendationFeedbackSummaryTypeDef(TypedDict):
    RecommendationId: NotRequired[str],
    Reactions: NotRequired[List[ReactionType]],  # (1)
    UserId: NotRequired[str],
```

1. See [:material-code-brackets: ReactionType](./literals.md#reactiontype) 
## ListRecommendationsRequestRequestTypeDef

```python
# ListRecommendationsRequestRequestTypeDef definition

class ListRecommendationsRequestRequestTypeDef(TypedDict):
    CodeReviewArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListRepositoryAssociationsRequestRequestTypeDef

```python
# ListRepositoryAssociationsRequestRequestTypeDef definition

class ListRepositoryAssociationsRequestRequestTypeDef(TypedDict):
    ProviderTypes: NotRequired[Sequence[ProviderTypeType]],  # (1)
    States: NotRequired[Sequence[RepositoryAssociationStateType]],  # (2)
    Names: NotRequired[Sequence[str]],
    Owners: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-brackets: RepositoryAssociationStateType](./literals.md#repositoryassociationstatetype) 
## RepositoryAssociationSummaryTypeDef

```python
# RepositoryAssociationSummaryTypeDef definition

class RepositoryAssociationSummaryTypeDef(TypedDict):
    AssociationArn: NotRequired[str],
    ConnectionArn: NotRequired[str],
    LastUpdatedTimeStamp: NotRequired[datetime],
    AssociationId: NotRequired[str],
    Name: NotRequired[str],
    Owner: NotRequired[str],
    ProviderType: NotRequired[ProviderTypeType],  # (1)
    State: NotRequired[RepositoryAssociationStateType],  # (2)
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-brackets: RepositoryAssociationStateType](./literals.md#repositoryassociationstatetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PutRecommendationFeedbackRequestRequestTypeDef

```python
# PutRecommendationFeedbackRequestRequestTypeDef definition

class PutRecommendationFeedbackRequestRequestTypeDef(TypedDict):
    CodeReviewArn: str,
    RecommendationId: str,
    Reactions: Sequence[ReactionType],  # (1)
```

1. See [:material-code-brackets: ReactionType](./literals.md#reactiontype) 
## RuleMetadataTypeDef

```python
# RuleMetadataTypeDef definition

class RuleMetadataTypeDef(TypedDict):
    RuleId: NotRequired[str],
    RuleName: NotRequired[str],
    ShortDescription: NotRequired[str],
    LongDescription: NotRequired[str],
    RuleTags: NotRequired[List[str]],
```

## RepositoryHeadSourceCodeTypeTypeDef

```python
# RepositoryHeadSourceCodeTypeTypeDef definition

class RepositoryHeadSourceCodeTypeTypeDef(TypedDict):
    BranchName: str,
```

## S3RepositoryTypeDef

```python
# S3RepositoryTypeDef definition

class S3RepositoryTypeDef(TypedDict):
    Name: str,
    BucketName: str,
```

## ThirdPartySourceRepositoryTypeDef

```python
# ThirdPartySourceRepositoryTypeDef definition

class ThirdPartySourceRepositoryTypeDef(TypedDict):
    Name: str,
    ConnectionArn: str,
    Owner: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    TagKeys: Sequence[str],
```

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3RepositoryDetailsTypeDef

```python
# S3RepositoryDetailsTypeDef definition

class S3RepositoryDetailsTypeDef(TypedDict):
    BucketName: NotRequired[str],
    CodeArtifacts: NotRequired[CodeArtifactsTypeDef],  # (1)
```

1. See [:material-code-braces: CodeArtifactsTypeDef](./type_defs.md#codeartifactstypedef) 
## DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef

```python
# DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef definition

class DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef(TypedDict):
    CodeReviewArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef

```python
# DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef definition

class DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef(TypedDict):
    AssociationArn: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeRecommendationFeedbackResponseTypeDef

```python
# DescribeRecommendationFeedbackResponseTypeDef definition

class DescribeRecommendationFeedbackResponseTypeDef(TypedDict):
    RecommendationFeedback: RecommendationFeedbackTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendationFeedbackTypeDef](./type_defs.md#recommendationfeedbacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RequestMetadataTypeDef

```python
# RequestMetadataTypeDef definition

class RequestMetadataTypeDef(TypedDict):
    RequestId: NotRequired[str],
    Requester: NotRequired[str],
    EventInfo: NotRequired[EventInfoTypeDef],  # (1)
    VendorName: NotRequired[VendorNameType],  # (2)
```

1. See [:material-code-braces: EventInfoTypeDef](./type_defs.md#eventinfotypedef) 
2. See [:material-code-brackets: VendorNameType](./literals.md#vendornametype) 
## ListRecommendationFeedbackResponseTypeDef

```python
# ListRecommendationFeedbackResponseTypeDef definition

class ListRecommendationFeedbackResponseTypeDef(TypedDict):
    RecommendationFeedbackSummaries: List[RecommendationFeedbackSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationFeedbackSummaryTypeDef](./type_defs.md#recommendationfeedbacksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef

```python
# ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef definition

class ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef(TypedDict):
    ProviderTypes: NotRequired[Sequence[ProviderTypeType]],  # (1)
    States: NotRequired[Sequence[RepositoryAssociationStateType]],  # (2)
    Names: NotRequired[Sequence[str]],
    Owners: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-brackets: RepositoryAssociationStateType](./literals.md#repositoryassociationstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRepositoryAssociationsResponseTypeDef

```python
# ListRepositoryAssociationsResponseTypeDef definition

class ListRepositoryAssociationsResponseTypeDef(TypedDict):
    RepositoryAssociationSummaries: List[RepositoryAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RepositoryAssociationSummaryTypeDef](./type_defs.md#repositoryassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecommendationSummaryTypeDef

```python
# RecommendationSummaryTypeDef definition

class RecommendationSummaryTypeDef(TypedDict):
    FilePath: NotRequired[str],
    RecommendationId: NotRequired[str],
    StartLine: NotRequired[int],
    EndLine: NotRequired[int],
    Description: NotRequired[str],
    RecommendationCategory: NotRequired[RecommendationCategoryType],  # (1)
    RuleMetadata: NotRequired[RuleMetadataTypeDef],  # (2)
    Severity: NotRequired[SeverityType],  # (3)
```

1. See [:material-code-brackets: RecommendationCategoryType](./literals.md#recommendationcategorytype) 
2. See [:material-code-braces: RuleMetadataTypeDef](./type_defs.md#rulemetadatatypedef) 
3. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
## RepositoryTypeDef

```python
# RepositoryTypeDef definition

class RepositoryTypeDef(TypedDict):
    CodeCommit: NotRequired[CodeCommitRepositoryTypeDef],  # (1)
    Bitbucket: NotRequired[ThirdPartySourceRepositoryTypeDef],  # (2)
    GitHubEnterpriseServer: NotRequired[ThirdPartySourceRepositoryTypeDef],  # (2)
    S3Bucket: NotRequired[S3RepositoryTypeDef],  # (4)
```

1. See [:material-code-braces: CodeCommitRepositoryTypeDef](./type_defs.md#codecommitrepositorytypedef) 
2. See [:material-code-braces: ThirdPartySourceRepositoryTypeDef](./type_defs.md#thirdpartysourcerepositorytypedef) 
3. See [:material-code-braces: ThirdPartySourceRepositoryTypeDef](./type_defs.md#thirdpartysourcerepositorytypedef) 
4. See [:material-code-braces: S3RepositoryTypeDef](./type_defs.md#s3repositorytypedef) 
## RepositoryAssociationTypeDef

```python
# RepositoryAssociationTypeDef definition

class RepositoryAssociationTypeDef(TypedDict):
    AssociationId: NotRequired[str],
    AssociationArn: NotRequired[str],
    ConnectionArn: NotRequired[str],
    Name: NotRequired[str],
    Owner: NotRequired[str],
    ProviderType: NotRequired[ProviderTypeType],  # (1)
    State: NotRequired[RepositoryAssociationStateType],  # (2)
    StateReason: NotRequired[str],
    LastUpdatedTimeStamp: NotRequired[datetime],
    CreatedTimeStamp: NotRequired[datetime],
    KMSKeyDetails: NotRequired[KMSKeyDetailsTypeDef],  # (3)
    S3RepositoryDetails: NotRequired[S3RepositoryDetailsTypeDef],  # (4)
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-brackets: RepositoryAssociationStateType](./literals.md#repositoryassociationstatetype) 
3. See [:material-code-braces: KMSKeyDetailsTypeDef](./type_defs.md#kmskeydetailstypedef) 
4. See [:material-code-braces: S3RepositoryDetailsTypeDef](./type_defs.md#s3repositorydetailstypedef) 
## S3BucketRepositoryTypeDef

```python
# S3BucketRepositoryTypeDef definition

class S3BucketRepositoryTypeDef(TypedDict):
    Name: str,
    Details: NotRequired[S3RepositoryDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: S3RepositoryDetailsTypeDef](./type_defs.md#s3repositorydetailstypedef) 
## ListRecommendationsResponseTypeDef

```python
# ListRecommendationsResponseTypeDef definition

class ListRecommendationsResponseTypeDef(TypedDict):
    RecommendationSummaries: List[RecommendationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationSummaryTypeDef](./type_defs.md#recommendationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateRepositoryRequestRequestTypeDef

```python
# AssociateRepositoryRequestRequestTypeDef definition

class AssociateRepositoryRequestRequestTypeDef(TypedDict):
    Repository: RepositoryTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    KMSKeyDetails: NotRequired[KMSKeyDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: RepositoryTypeDef](./type_defs.md#repositorytypedef) 
2. See [:material-code-braces: KMSKeyDetailsTypeDef](./type_defs.md#kmskeydetailstypedef) 
## AssociateRepositoryResponseTypeDef

```python
# AssociateRepositoryResponseTypeDef definition

class AssociateRepositoryResponseTypeDef(TypedDict):
    RepositoryAssociation: RepositoryAssociationTypeDef,  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryAssociationTypeDef](./type_defs.md#repositoryassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRepositoryAssociationResponseTypeDef

```python
# DescribeRepositoryAssociationResponseTypeDef definition

class DescribeRepositoryAssociationResponseTypeDef(TypedDict):
    RepositoryAssociation: RepositoryAssociationTypeDef,  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryAssociationTypeDef](./type_defs.md#repositoryassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateRepositoryResponseTypeDef

```python
# DisassociateRepositoryResponseTypeDef definition

class DisassociateRepositoryResponseTypeDef(TypedDict):
    RepositoryAssociation: RepositoryAssociationTypeDef,  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryAssociationTypeDef](./type_defs.md#repositoryassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceCodeTypeTypeDef

```python
# SourceCodeTypeTypeDef definition

class SourceCodeTypeTypeDef(TypedDict):
    CommitDiff: NotRequired[CommitDiffSourceCodeTypeTypeDef],  # (1)
    RepositoryHead: NotRequired[RepositoryHeadSourceCodeTypeTypeDef],  # (2)
    BranchDiff: NotRequired[BranchDiffSourceCodeTypeTypeDef],  # (3)
    S3BucketRepository: NotRequired[S3BucketRepositoryTypeDef],  # (4)
    RequestMetadata: NotRequired[RequestMetadataTypeDef],  # (5)
```

1. See [:material-code-braces: CommitDiffSourceCodeTypeTypeDef](./type_defs.md#commitdiffsourcecodetypetypedef) 
2. See [:material-code-braces: RepositoryHeadSourceCodeTypeTypeDef](./type_defs.md#repositoryheadsourcecodetypetypedef) 
3. See [:material-code-braces: BranchDiffSourceCodeTypeTypeDef](./type_defs.md#branchdiffsourcecodetypetypedef) 
4. See [:material-code-braces: S3BucketRepositoryTypeDef](./type_defs.md#s3bucketrepositorytypedef) 
5. See [:material-code-braces: RequestMetadataTypeDef](./type_defs.md#requestmetadatatypedef) 
## CodeReviewSummaryTypeDef

```python
# CodeReviewSummaryTypeDef definition

class CodeReviewSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    CodeReviewArn: NotRequired[str],
    RepositoryName: NotRequired[str],
    Owner: NotRequired[str],
    ProviderType: NotRequired[ProviderTypeType],  # (1)
    State: NotRequired[JobStateType],  # (2)
    CreatedTimeStamp: NotRequired[datetime],
    LastUpdatedTimeStamp: NotRequired[datetime],
    Type: NotRequired[TypeType],  # (3)
    PullRequestId: NotRequired[str],
    MetricsSummary: NotRequired[MetricsSummaryTypeDef],  # (4)
    SourceCodeType: NotRequired[SourceCodeTypeTypeDef],  # (5)
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-brackets: JobStateType](./literals.md#jobstatetype) 
3. See [:material-code-brackets: TypeType](./literals.md#typetype) 
4. See [:material-code-braces: MetricsSummaryTypeDef](./type_defs.md#metricssummarytypedef) 
5. See [:material-code-braces: SourceCodeTypeTypeDef](./type_defs.md#sourcecodetypetypedef) 
## CodeReviewTypeDef

```python
# CodeReviewTypeDef definition

class CodeReviewTypeDef(TypedDict):
    Name: NotRequired[str],
    CodeReviewArn: NotRequired[str],
    RepositoryName: NotRequired[str],
    Owner: NotRequired[str],
    ProviderType: NotRequired[ProviderTypeType],  # (1)
    State: NotRequired[JobStateType],  # (2)
    StateReason: NotRequired[str],
    CreatedTimeStamp: NotRequired[datetime],
    LastUpdatedTimeStamp: NotRequired[datetime],
    Type: NotRequired[TypeType],  # (3)
    PullRequestId: NotRequired[str],
    SourceCodeType: NotRequired[SourceCodeTypeTypeDef],  # (4)
    AssociationArn: NotRequired[str],
    Metrics: NotRequired[MetricsTypeDef],  # (5)
    AnalysisTypes: NotRequired[List[AnalysisTypeType]],  # (6)
    ConfigFileState: NotRequired[ConfigFileStateType],  # (7)
```

1. See [:material-code-brackets: ProviderTypeType](./literals.md#providertypetype) 
2. See [:material-code-brackets: JobStateType](./literals.md#jobstatetype) 
3. See [:material-code-brackets: TypeType](./literals.md#typetype) 
4. See [:material-code-braces: SourceCodeTypeTypeDef](./type_defs.md#sourcecodetypetypedef) 
5. See [:material-code-braces: MetricsTypeDef](./type_defs.md#metricstypedef) 
6. See [:material-code-brackets: AnalysisTypeType](./literals.md#analysistypetype) 
7. See [:material-code-brackets: ConfigFileStateType](./literals.md#configfilestatetype) 
## RepositoryAnalysisTypeDef

```python
# RepositoryAnalysisTypeDef definition

class RepositoryAnalysisTypeDef(TypedDict):
    RepositoryHead: NotRequired[RepositoryHeadSourceCodeTypeTypeDef],  # (1)
    SourceCodeType: NotRequired[SourceCodeTypeTypeDef],  # (2)
```

1. See [:material-code-braces: RepositoryHeadSourceCodeTypeTypeDef](./type_defs.md#repositoryheadsourcecodetypetypedef) 
2. See [:material-code-braces: SourceCodeTypeTypeDef](./type_defs.md#sourcecodetypetypedef) 
## ListCodeReviewsResponseTypeDef

```python
# ListCodeReviewsResponseTypeDef definition

class ListCodeReviewsResponseTypeDef(TypedDict):
    CodeReviewSummaries: List[CodeReviewSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CodeReviewSummaryTypeDef](./type_defs.md#codereviewsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCodeReviewResponseTypeDef

```python
# CreateCodeReviewResponseTypeDef definition

class CreateCodeReviewResponseTypeDef(TypedDict):
    CodeReview: CodeReviewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeReviewTypeDef](./type_defs.md#codereviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCodeReviewResponseTypeDef

```python
# DescribeCodeReviewResponseTypeDef definition

class DescribeCodeReviewResponseTypeDef(TypedDict):
    CodeReview: CodeReviewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeReviewTypeDef](./type_defs.md#codereviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CodeReviewTypeTypeDef

```python
# CodeReviewTypeTypeDef definition

class CodeReviewTypeTypeDef(TypedDict):
    RepositoryAnalysis: RepositoryAnalysisTypeDef,  # (1)
    AnalysisTypes: NotRequired[Sequence[AnalysisTypeType]],  # (2)
```

1. See [:material-code-braces: RepositoryAnalysisTypeDef](./type_defs.md#repositoryanalysistypedef) 
2. See [:material-code-brackets: AnalysisTypeType](./literals.md#analysistypetype) 
## CreateCodeReviewRequestRequestTypeDef

```python
# CreateCodeReviewRequestRequestTypeDef definition

class CreateCodeReviewRequestRequestTypeDef(TypedDict):
    Name: str,
    RepositoryAssociationArn: str,
    Type: CodeReviewTypeTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: CodeReviewTypeTypeDef](./type_defs.md#codereviewtypetypedef) 
