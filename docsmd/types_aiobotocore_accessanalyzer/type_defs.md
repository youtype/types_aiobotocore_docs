# Type definitions

> [Index](../README.md) > [AccessAnalyzer](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AccessAnalyzer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
    type annotations stubs module [types-aiobotocore-accessanalyzer](https://pypi.org/project/types-aiobotocore-accessanalyzer/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AccessPreviewStatusReasonTypeDef

```python
# AccessPreviewStatusReasonTypeDef definition

class AccessPreviewStatusReasonTypeDef(TypedDict):
    code: AccessPreviewStatusReasonCodeType,  # (1)
```

1. See [:material-code-brackets: AccessPreviewStatusReasonCodeType](./literals.md#accesspreviewstatusreasoncodetype) 
## AclGranteeTypeDef

```python
# AclGranteeTypeDef definition

class AclGranteeTypeDef(TypedDict):
    id: NotRequired[str],
    uri: NotRequired[str],
```

## AnalyzedResourceSummaryTypeDef

```python
# AnalyzedResourceSummaryTypeDef definition

class AnalyzedResourceSummaryTypeDef(TypedDict):
    resourceArn: str,
    resourceOwnerAccount: str,
    resourceType: ResourceTypeType,  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## AnalyzedResourceTypeDef

```python
# AnalyzedResourceTypeDef definition

class AnalyzedResourceTypeDef(TypedDict):
    resourceArn: str,
    resourceType: ResourceTypeType,  # (1)
    createdAt: datetime,
    analyzedAt: datetime,
    updatedAt: datetime,
    isPublic: bool,
    resourceOwnerAccount: str,
    actions: NotRequired[List[str]],
    sharedVia: NotRequired[List[str]],
    status: NotRequired[FindingStatusType],  # (2)
    error: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype) 
## StatusReasonTypeDef

```python
# StatusReasonTypeDef definition

class StatusReasonTypeDef(TypedDict):
    code: ReasonCodeType,  # (1)
```

1. See [:material-code-brackets: ReasonCodeType](./literals.md#reasoncodetype) 
## ApplyArchiveRuleRequestRequestTypeDef

```python
# ApplyArchiveRuleRequestRequestTypeDef definition

class ApplyArchiveRuleRequestRequestTypeDef(TypedDict):
    analyzerArn: str,
    ruleName: str,
    clientToken: NotRequired[str],
```

## CriterionTypeDef

```python
# CriterionTypeDef definition

class CriterionTypeDef(TypedDict):
    eq: NotRequired[Sequence[str]],
    neq: NotRequired[Sequence[str]],
    contains: NotRequired[Sequence[str]],
    exists: NotRequired[bool],
```

## CancelPolicyGenerationRequestRequestTypeDef

```python
# CancelPolicyGenerationRequestRequestTypeDef definition

class CancelPolicyGenerationRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## TrailTypeDef

```python
# TrailTypeDef definition

class TrailTypeDef(TypedDict):
    cloudTrailArn: str,
    regions: NotRequired[Sequence[str]],
    allRegions: NotRequired[bool],
```

## TrailPropertiesTypeDef

```python
# TrailPropertiesTypeDef definition

class TrailPropertiesTypeDef(TypedDict):
    cloudTrailArn: str,
    regions: NotRequired[List[str]],
    allRegions: NotRequired[bool],
```

## EbsSnapshotConfigurationTypeDef

```python
# EbsSnapshotConfigurationTypeDef definition

class EbsSnapshotConfigurationTypeDef(TypedDict):
    userIds: NotRequired[Sequence[str]],
    groups: NotRequired[Sequence[str]],
    kmsKeyId: NotRequired[str],
```

## EcrRepositoryConfigurationTypeDef

```python
# EcrRepositoryConfigurationTypeDef definition

class EcrRepositoryConfigurationTypeDef(TypedDict):
    repositoryPolicy: NotRequired[str],
```

## EfsFileSystemConfigurationTypeDef

```python
# EfsFileSystemConfigurationTypeDef definition

class EfsFileSystemConfigurationTypeDef(TypedDict):
    fileSystemPolicy: NotRequired[str],
```

## IamRoleConfigurationTypeDef

```python
# IamRoleConfigurationTypeDef definition

class IamRoleConfigurationTypeDef(TypedDict):
    trustPolicy: NotRequired[str],
```

## SecretsManagerSecretConfigurationTypeDef

```python
# SecretsManagerSecretConfigurationTypeDef definition

class SecretsManagerSecretConfigurationTypeDef(TypedDict):
    kmsKeyId: NotRequired[str],
    secretPolicy: NotRequired[str],
```

## SnsTopicConfigurationTypeDef

```python
# SnsTopicConfigurationTypeDef definition

class SnsTopicConfigurationTypeDef(TypedDict):
    topicPolicy: NotRequired[str],
```

## SqsQueueConfigurationTypeDef

```python
# SqsQueueConfigurationTypeDef definition

class SqsQueueConfigurationTypeDef(TypedDict):
    queuePolicy: NotRequired[str],
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

## DeleteAnalyzerRequestRequestTypeDef

```python
# DeleteAnalyzerRequestRequestTypeDef definition

class DeleteAnalyzerRequestRequestTypeDef(TypedDict):
    analyzerName: str,
    clientToken: NotRequired[str],
```

## DeleteArchiveRuleRequestRequestTypeDef

```python
# DeleteArchiveRuleRequestRequestTypeDef definition

class DeleteArchiveRuleRequestRequestTypeDef(TypedDict):
    analyzerName: str,
    ruleName: str,
    clientToken: NotRequired[str],
```

## FindingSourceDetailTypeDef

```python
# FindingSourceDetailTypeDef definition

class FindingSourceDetailTypeDef(TypedDict):
    accessPointArn: NotRequired[str],
    accessPointAccount: NotRequired[str],
```

## GeneratedPolicyTypeDef

```python
# GeneratedPolicyTypeDef definition

class GeneratedPolicyTypeDef(TypedDict):
    policy: str,
```

## GetAccessPreviewRequestRequestTypeDef

```python
# GetAccessPreviewRequestRequestTypeDef definition

class GetAccessPreviewRequestRequestTypeDef(TypedDict):
    accessPreviewId: str,
    analyzerArn: str,
```

## GetAnalyzedResourceRequestRequestTypeDef

```python
# GetAnalyzedResourceRequestRequestTypeDef definition

class GetAnalyzedResourceRequestRequestTypeDef(TypedDict):
    analyzerArn: str,
    resourceArn: str,
```

## GetAnalyzerRequestRequestTypeDef

```python
# GetAnalyzerRequestRequestTypeDef definition

class GetAnalyzerRequestRequestTypeDef(TypedDict):
    analyzerName: str,
```

## GetArchiveRuleRequestRequestTypeDef

```python
# GetArchiveRuleRequestRequestTypeDef definition

class GetArchiveRuleRequestRequestTypeDef(TypedDict):
    analyzerName: str,
    ruleName: str,
```

## GetFindingRequestRequestTypeDef

```python
# GetFindingRequestRequestTypeDef definition

class GetFindingRequestRequestTypeDef(TypedDict):
    analyzerArn: str,
    id: str,
```

## GetGeneratedPolicyRequestRequestTypeDef

```python
# GetGeneratedPolicyRequestRequestTypeDef definition

class GetGeneratedPolicyRequestRequestTypeDef(TypedDict):
    jobId: str,
    includeResourcePlaceholders: NotRequired[bool],
    includeServiceLevelTemplate: NotRequired[bool],
```

## JobErrorTypeDef

```python
# JobErrorTypeDef definition

class JobErrorTypeDef(TypedDict):
    code: JobErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: JobErrorCodeType](./literals.md#joberrorcodetype) 
## KmsGrantConstraintsTypeDef

```python
# KmsGrantConstraintsTypeDef definition

class KmsGrantConstraintsTypeDef(TypedDict):
    encryptionContextEquals: NotRequired[Mapping[str, str]],
    encryptionContextSubset: NotRequired[Mapping[str, str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAccessPreviewsRequestRequestTypeDef

```python
# ListAccessPreviewsRequestRequestTypeDef definition

class ListAccessPreviewsRequestRequestTypeDef(TypedDict):
    analyzerArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListAnalyzedResourcesRequestRequestTypeDef

```python
# ListAnalyzedResourcesRequestRequestTypeDef definition

class ListAnalyzedResourcesRequestRequestTypeDef(TypedDict):
    analyzerArn: str,
    resourceType: NotRequired[ResourceTypeType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ListAnalyzersRequestRequestTypeDef

```python
# ListAnalyzersRequestRequestTypeDef definition

class ListAnalyzersRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    type: NotRequired[TypeType],  # (1)
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## ListArchiveRulesRequestRequestTypeDef

```python
# ListArchiveRulesRequestRequestTypeDef definition

class ListArchiveRulesRequestRequestTypeDef(TypedDict):
    analyzerName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## SortCriteriaTypeDef

```python
# SortCriteriaTypeDef definition

class SortCriteriaTypeDef(TypedDict):
    attributeName: NotRequired[str],
    orderBy: NotRequired[OrderByType],  # (1)
```

1. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
## ListPolicyGenerationsRequestRequestTypeDef

```python
# ListPolicyGenerationsRequestRequestTypeDef definition

class ListPolicyGenerationsRequestRequestTypeDef(TypedDict):
    principalArn: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PolicyGenerationTypeDef

```python
# PolicyGenerationTypeDef definition

class PolicyGenerationTypeDef(TypedDict):
    jobId: str,
    principalArn: str,
    status: JobStatusType,  # (1)
    startedOn: datetime,
    completedOn: NotRequired[datetime],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## VpcConfigurationTypeDef

```python
# VpcConfigurationTypeDef definition

class VpcConfigurationTypeDef(TypedDict):
    vpcId: str,
```

## SubstringTypeDef

```python
# SubstringTypeDef definition

class SubstringTypeDef(TypedDict):
    start: int,
    length: int,
```

## PolicyGenerationDetailsTypeDef

```python
# PolicyGenerationDetailsTypeDef definition

class PolicyGenerationDetailsTypeDef(TypedDict):
    principalArn: str,
```

## PositionTypeDef

```python
# PositionTypeDef definition

class PositionTypeDef(TypedDict):
    line: int,
    column: int,
    offset: int,
```

## RdsDbClusterSnapshotAttributeValueTypeDef

```python
# RdsDbClusterSnapshotAttributeValueTypeDef definition

class RdsDbClusterSnapshotAttributeValueTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
```

## RdsDbSnapshotAttributeValueTypeDef

```python
# RdsDbSnapshotAttributeValueTypeDef definition

class RdsDbSnapshotAttributeValueTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
```

## S3PublicAccessBlockConfigurationTypeDef

```python
# S3PublicAccessBlockConfigurationTypeDef definition

class S3PublicAccessBlockConfigurationTypeDef(TypedDict):
    ignorePublicAcls: bool,
    restrictPublicBuckets: bool,
```

## StartResourceScanRequestRequestTypeDef

```python
# StartResourceScanRequestRequestTypeDef definition

class StartResourceScanRequestRequestTypeDef(TypedDict):
    analyzerArn: str,
    resourceArn: str,
    resourceOwnerAccount: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateFindingsRequestRequestTypeDef

```python
# UpdateFindingsRequestRequestTypeDef definition

class UpdateFindingsRequestRequestTypeDef(TypedDict):
    analyzerArn: str,
    status: FindingStatusUpdateType,  # (1)
    ids: NotRequired[Sequence[str]],
    resourceArn: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: FindingStatusUpdateType](./literals.md#findingstatusupdatetype) 
## ValidatePolicyRequestRequestTypeDef

```python
# ValidatePolicyRequestRequestTypeDef definition

class ValidatePolicyRequestRequestTypeDef(TypedDict):
    policyDocument: str,
    policyType: PolicyTypeType,  # (1)
    locale: NotRequired[LocaleType],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    validatePolicyResourceType: NotRequired[ValidatePolicyResourceTypeType],  # (3)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
3. See [:material-code-brackets: ValidatePolicyResourceTypeType](./literals.md#validatepolicyresourcetypetype) 
## AccessPreviewSummaryTypeDef

```python
# AccessPreviewSummaryTypeDef definition

class AccessPreviewSummaryTypeDef(TypedDict):
    id: str,
    analyzerArn: str,
    createdAt: datetime,
    status: AccessPreviewStatusType,  # (1)
    statusReason: NotRequired[AccessPreviewStatusReasonTypeDef],  # (2)
```

1. See [:material-code-brackets: AccessPreviewStatusType](./literals.md#accesspreviewstatustype) 
2. See [:material-code-braces: AccessPreviewStatusReasonTypeDef](./type_defs.md#accesspreviewstatusreasontypedef) 
## S3BucketAclGrantConfigurationTypeDef

```python
# S3BucketAclGrantConfigurationTypeDef definition

class S3BucketAclGrantConfigurationTypeDef(TypedDict):
    permission: AclPermissionType,  # (1)
    grantee: AclGranteeTypeDef,  # (2)
```

1. See [:material-code-brackets: AclPermissionType](./literals.md#aclpermissiontype) 
2. See [:material-code-braces: AclGranteeTypeDef](./type_defs.md#aclgranteetypedef) 
## AnalyzerSummaryTypeDef

```python
# AnalyzerSummaryTypeDef definition

class AnalyzerSummaryTypeDef(TypedDict):
    arn: str,
    name: str,
    type: TypeType,  # (1)
    createdAt: datetime,
    status: AnalyzerStatusType,  # (2)
    lastResourceAnalyzed: NotRequired[str],
    lastResourceAnalyzedAt: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    statusReason: NotRequired[StatusReasonTypeDef],  # (3)
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-brackets: AnalyzerStatusType](./literals.md#analyzerstatustype) 
3. See [:material-code-braces: StatusReasonTypeDef](./type_defs.md#statusreasontypedef) 
## ArchiveRuleSummaryTypeDef

```python
# ArchiveRuleSummaryTypeDef definition

class ArchiveRuleSummaryTypeDef(TypedDict):
    ruleName: str,
    filter: Dict[str, CriterionTypeDef],  # (1)
    createdAt: datetime,
    updatedAt: datetime,
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
## CreateArchiveRuleRequestRequestTypeDef

```python
# CreateArchiveRuleRequestRequestTypeDef definition

class CreateArchiveRuleRequestRequestTypeDef(TypedDict):
    analyzerName: str,
    ruleName: str,
    filter: Mapping[str, CriterionTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
## InlineArchiveRuleTypeDef

```python
# InlineArchiveRuleTypeDef definition

class InlineArchiveRuleTypeDef(TypedDict):
    ruleName: str,
    filter: Mapping[str, CriterionTypeDef],  # (1)
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
## ListAccessPreviewFindingsRequestRequestTypeDef

```python
# ListAccessPreviewFindingsRequestRequestTypeDef definition

class ListAccessPreviewFindingsRequestRequestTypeDef(TypedDict):
    accessPreviewId: str,
    analyzerArn: str,
    filter: NotRequired[Mapping[str, CriterionTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
## UpdateArchiveRuleRequestRequestTypeDef

```python
# UpdateArchiveRuleRequestRequestTypeDef definition

class UpdateArchiveRuleRequestRequestTypeDef(TypedDict):
    analyzerName: str,
    ruleName: str,
    filter: Mapping[str, CriterionTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
## CloudTrailDetailsTypeDef

```python
# CloudTrailDetailsTypeDef definition

class CloudTrailDetailsTypeDef(TypedDict):
    trails: Sequence[TrailTypeDef],  # (1)
    accessRole: str,
    startTime: Union[datetime, str],
    endTime: NotRequired[Union[datetime, str]],
```

1. See [:material-code-braces: TrailTypeDef](./type_defs.md#trailtypedef) 
## CloudTrailPropertiesTypeDef

```python
# CloudTrailPropertiesTypeDef definition

class CloudTrailPropertiesTypeDef(TypedDict):
    trailProperties: List[TrailPropertiesTypeDef],  # (1)
    startTime: datetime,
    endTime: datetime,
```

1. See [:material-code-braces: TrailPropertiesTypeDef](./type_defs.md#trailpropertiestypedef) 
## CreateAccessPreviewResponseTypeDef

```python
# CreateAccessPreviewResponseTypeDef definition

class CreateAccessPreviewResponseTypeDef(TypedDict):
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAnalyzerResponseTypeDef

```python
# CreateAnalyzerResponseTypeDef definition

class CreateAnalyzerResponseTypeDef(TypedDict):
    arn: str,
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
## GetAnalyzedResourceResponseTypeDef

```python
# GetAnalyzedResourceResponseTypeDef definition

class GetAnalyzedResourceResponseTypeDef(TypedDict):
    resource: AnalyzedResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyzedResourceTypeDef](./type_defs.md#analyzedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnalyzedResourcesResponseTypeDef

```python
# ListAnalyzedResourcesResponseTypeDef definition

class ListAnalyzedResourcesResponseTypeDef(TypedDict):
    analyzedResources: List[AnalyzedResourceSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyzedResourceSummaryTypeDef](./type_defs.md#analyzedresourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPolicyGenerationResponseTypeDef

```python
# StartPolicyGenerationResponseTypeDef definition

class StartPolicyGenerationResponseTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FindingSourceTypeDef

```python
# FindingSourceTypeDef definition

class FindingSourceTypeDef(TypedDict):
    type: FindingSourceTypeType,  # (1)
    detail: NotRequired[FindingSourceDetailTypeDef],  # (2)
```

1. See [:material-code-brackets: FindingSourceTypeType](./literals.md#findingsourcetypetype) 
2. See [:material-code-braces: FindingSourceDetailTypeDef](./type_defs.md#findingsourcedetailtypedef) 
## JobDetailsTypeDef

```python
# JobDetailsTypeDef definition

class JobDetailsTypeDef(TypedDict):
    jobId: str,
    status: JobStatusType,  # (1)
    startedOn: datetime,
    completedOn: NotRequired[datetime],
    jobError: NotRequired[JobErrorTypeDef],  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: JobErrorTypeDef](./type_defs.md#joberrortypedef) 
## KmsGrantConfigurationTypeDef

```python
# KmsGrantConfigurationTypeDef definition

class KmsGrantConfigurationTypeDef(TypedDict):
    operations: Sequence[KmsGrantOperationType],  # (1)
    granteePrincipal: str,
    issuingAccount: str,
    retiringPrincipal: NotRequired[str],
    constraints: NotRequired[KmsGrantConstraintsTypeDef],  # (2)
```

1. See [:material-code-brackets: KmsGrantOperationType](./literals.md#kmsgrantoperationtype) 
2. See [:material-code-braces: KmsGrantConstraintsTypeDef](./type_defs.md#kmsgrantconstraintstypedef) 
## ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef

```python
# ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef definition

class ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef(TypedDict):
    accessPreviewId: str,
    analyzerArn: str,
    filter: NotRequired[Mapping[str, CriterionTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef

```python
# ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef definition

class ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef(TypedDict):
    analyzerArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef

```python
# ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef definition

class ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef(TypedDict):
    analyzerArn: str,
    resourceType: NotRequired[ResourceTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAnalyzersRequestListAnalyzersPaginateTypeDef

```python
# ListAnalyzersRequestListAnalyzersPaginateTypeDef definition

class ListAnalyzersRequestListAnalyzersPaginateTypeDef(TypedDict):
    type: NotRequired[TypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListArchiveRulesRequestListArchiveRulesPaginateTypeDef

```python
# ListArchiveRulesRequestListArchiveRulesPaginateTypeDef definition

class ListArchiveRulesRequestListArchiveRulesPaginateTypeDef(TypedDict):
    analyzerName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef

```python
# ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef definition

class ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef(TypedDict):
    principalArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ValidatePolicyRequestValidatePolicyPaginateTypeDef

```python
# ValidatePolicyRequestValidatePolicyPaginateTypeDef definition

class ValidatePolicyRequestValidatePolicyPaginateTypeDef(TypedDict):
    policyDocument: str,
    policyType: PolicyTypeType,  # (1)
    locale: NotRequired[LocaleType],  # (2)
    validatePolicyResourceType: NotRequired[ValidatePolicyResourceTypeType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
3. See [:material-code-brackets: ValidatePolicyResourceTypeType](./literals.md#validatepolicyresourcetypetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFindingsRequestListFindingsPaginateTypeDef

```python
# ListFindingsRequestListFindingsPaginateTypeDef definition

class ListFindingsRequestListFindingsPaginateTypeDef(TypedDict):
    analyzerArn: str,
    filter: NotRequired[Mapping[str, CriterionTypeDef]],  # (1)
    sort: NotRequired[SortCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFindingsRequestRequestTypeDef

```python
# ListFindingsRequestRequestTypeDef definition

class ListFindingsRequestRequestTypeDef(TypedDict):
    analyzerArn: str,
    filter: NotRequired[Mapping[str, CriterionTypeDef]],  # (1)
    sort: NotRequired[SortCriteriaTypeDef],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: CriterionTypeDef](./type_defs.md#criteriontypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
## ListPolicyGenerationsResponseTypeDef

```python
# ListPolicyGenerationsResponseTypeDef definition

class ListPolicyGenerationsResponseTypeDef(TypedDict):
    policyGenerations: List[PolicyGenerationTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyGenerationTypeDef](./type_defs.md#policygenerationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkOriginConfigurationTypeDef

```python
# NetworkOriginConfigurationTypeDef definition

class NetworkOriginConfigurationTypeDef(TypedDict):
    vpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (1)
    internetConfiguration: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
## PathElementTypeDef

```python
# PathElementTypeDef definition

class PathElementTypeDef(TypedDict):
    index: NotRequired[int],
    key: NotRequired[str],
    substring: NotRequired[SubstringTypeDef],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-braces: SubstringTypeDef](./type_defs.md#substringtypedef) 
## SpanTypeDef

```python
# SpanTypeDef definition

class SpanTypeDef(TypedDict):
    start: PositionTypeDef,  # (1)
    end: PositionTypeDef,  # (1)
```

1. See [:material-code-braces: PositionTypeDef](./type_defs.md#positiontypedef) 
2. See [:material-code-braces: PositionTypeDef](./type_defs.md#positiontypedef) 
## RdsDbClusterSnapshotConfigurationTypeDef

```python
# RdsDbClusterSnapshotConfigurationTypeDef definition

class RdsDbClusterSnapshotConfigurationTypeDef(TypedDict):
    attributes: NotRequired[Mapping[str, RdsDbClusterSnapshotAttributeValueTypeDef]],  # (1)
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: RdsDbClusterSnapshotAttributeValueTypeDef](./type_defs.md#rdsdbclustersnapshotattributevaluetypedef) 
## RdsDbSnapshotConfigurationTypeDef

```python
# RdsDbSnapshotConfigurationTypeDef definition

class RdsDbSnapshotConfigurationTypeDef(TypedDict):
    attributes: NotRequired[Mapping[str, RdsDbSnapshotAttributeValueTypeDef]],  # (1)
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: RdsDbSnapshotAttributeValueTypeDef](./type_defs.md#rdsdbsnapshotattributevaluetypedef) 
## ListAccessPreviewsResponseTypeDef

```python
# ListAccessPreviewsResponseTypeDef definition

class ListAccessPreviewsResponseTypeDef(TypedDict):
    accessPreviews: List[AccessPreviewSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessPreviewSummaryTypeDef](./type_defs.md#accesspreviewsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnalyzerResponseTypeDef

```python
# GetAnalyzerResponseTypeDef definition

class GetAnalyzerResponseTypeDef(TypedDict):
    analyzer: AnalyzerSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyzerSummaryTypeDef](./type_defs.md#analyzersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnalyzersResponseTypeDef

```python
# ListAnalyzersResponseTypeDef definition

class ListAnalyzersResponseTypeDef(TypedDict):
    analyzers: List[AnalyzerSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalyzerSummaryTypeDef](./type_defs.md#analyzersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetArchiveRuleResponseTypeDef

```python
# GetArchiveRuleResponseTypeDef definition

class GetArchiveRuleResponseTypeDef(TypedDict):
    archiveRule: ArchiveRuleSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ArchiveRuleSummaryTypeDef](./type_defs.md#archiverulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListArchiveRulesResponseTypeDef

```python
# ListArchiveRulesResponseTypeDef definition

class ListArchiveRulesResponseTypeDef(TypedDict):
    archiveRules: List[ArchiveRuleSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ArchiveRuleSummaryTypeDef](./type_defs.md#archiverulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAnalyzerRequestRequestTypeDef

```python
# CreateAnalyzerRequestRequestTypeDef definition

class CreateAnalyzerRequestRequestTypeDef(TypedDict):
    analyzerName: str,
    type: TypeType,  # (1)
    archiveRules: NotRequired[Sequence[InlineArchiveRuleTypeDef]],  # (2)
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
2. See [:material-code-braces: InlineArchiveRuleTypeDef](./type_defs.md#inlinearchiveruletypedef) 
## StartPolicyGenerationRequestRequestTypeDef

```python
# StartPolicyGenerationRequestRequestTypeDef definition

class StartPolicyGenerationRequestRequestTypeDef(TypedDict):
    policyGenerationDetails: PolicyGenerationDetailsTypeDef,  # (1)
    cloudTrailDetails: NotRequired[CloudTrailDetailsTypeDef],  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyGenerationDetailsTypeDef](./type_defs.md#policygenerationdetailstypedef) 
2. See [:material-code-braces: CloudTrailDetailsTypeDef](./type_defs.md#cloudtraildetailstypedef) 
## GeneratedPolicyPropertiesTypeDef

```python
# GeneratedPolicyPropertiesTypeDef definition

class GeneratedPolicyPropertiesTypeDef(TypedDict):
    principalArn: str,
    isComplete: NotRequired[bool],
    cloudTrailProperties: NotRequired[CloudTrailPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: CloudTrailPropertiesTypeDef](./type_defs.md#cloudtrailpropertiestypedef) 
## AccessPreviewFindingTypeDef

```python
# AccessPreviewFindingTypeDef definition

class AccessPreviewFindingTypeDef(TypedDict):
    id: str,
    resourceType: ResourceTypeType,  # (2)
    createdAt: datetime,
    changeType: FindingChangeTypeType,  # (3)
    status: FindingStatusType,  # (1)
    resourceOwnerAccount: str,
    existingFindingId: NotRequired[str],
    existingFindingStatus: NotRequired[FindingStatusType],  # (1)
    principal: NotRequired[Dict[str, str]],
    action: NotRequired[List[str]],
    condition: NotRequired[Dict[str, str]],
    resource: NotRequired[str],
    isPublic: NotRequired[bool],
    error: NotRequired[str],
    sources: NotRequired[List[FindingSourceTypeDef]],  # (5)
```

1. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-brackets: FindingChangeTypeType](./literals.md#findingchangetypetype) 
4. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype) 
5. See [:material-code-braces: FindingSourceTypeDef](./type_defs.md#findingsourcetypedef) 
## FindingSummaryTypeDef

```python
# FindingSummaryTypeDef definition

class FindingSummaryTypeDef(TypedDict):
    id: str,
    resourceType: ResourceTypeType,  # (1)
    condition: Dict[str, str],
    createdAt: datetime,
    analyzedAt: datetime,
    updatedAt: datetime,
    status: FindingStatusType,  # (2)
    resourceOwnerAccount: str,
    principal: NotRequired[Dict[str, str]],
    action: NotRequired[List[str]],
    resource: NotRequired[str],
    isPublic: NotRequired[bool],
    error: NotRequired[str],
    sources: NotRequired[List[FindingSourceTypeDef]],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype) 
3. See [:material-code-braces: FindingSourceTypeDef](./type_defs.md#findingsourcetypedef) 
## FindingTypeDef

```python
# FindingTypeDef definition

class FindingTypeDef(TypedDict):
    id: str,
    resourceType: ResourceTypeType,  # (1)
    condition: Dict[str, str],
    createdAt: datetime,
    analyzedAt: datetime,
    updatedAt: datetime,
    status: FindingStatusType,  # (2)
    resourceOwnerAccount: str,
    principal: NotRequired[Dict[str, str]],
    action: NotRequired[List[str]],
    resource: NotRequired[str],
    isPublic: NotRequired[bool],
    error: NotRequired[str],
    sources: NotRequired[List[FindingSourceTypeDef]],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype) 
3. See [:material-code-braces: FindingSourceTypeDef](./type_defs.md#findingsourcetypedef) 
## KmsKeyConfigurationTypeDef

```python
# KmsKeyConfigurationTypeDef definition

class KmsKeyConfigurationTypeDef(TypedDict):
    keyPolicies: NotRequired[Mapping[str, str]],
    grants: NotRequired[Sequence[KmsGrantConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: KmsGrantConfigurationTypeDef](./type_defs.md#kmsgrantconfigurationtypedef) 
## S3AccessPointConfigurationTypeDef

```python
# S3AccessPointConfigurationTypeDef definition

class S3AccessPointConfigurationTypeDef(TypedDict):
    accessPointPolicy: NotRequired[str],
    publicAccessBlock: NotRequired[S3PublicAccessBlockConfigurationTypeDef],  # (1)
    networkOrigin: NotRequired[NetworkOriginConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: S3PublicAccessBlockConfigurationTypeDef](./type_defs.md#s3publicaccessblockconfigurationtypedef) 
2. See [:material-code-braces: NetworkOriginConfigurationTypeDef](./type_defs.md#networkoriginconfigurationtypedef) 
## LocationTypeDef

```python
# LocationTypeDef definition

class LocationTypeDef(TypedDict):
    path: List[PathElementTypeDef],  # (1)
    span: SpanTypeDef,  # (2)
```

1. See [:material-code-braces: PathElementTypeDef](./type_defs.md#pathelementtypedef) 
2. See [:material-code-braces: SpanTypeDef](./type_defs.md#spantypedef) 
## GeneratedPolicyResultTypeDef

```python
# GeneratedPolicyResultTypeDef definition

class GeneratedPolicyResultTypeDef(TypedDict):
    properties: GeneratedPolicyPropertiesTypeDef,  # (1)
    generatedPolicies: NotRequired[List[GeneratedPolicyTypeDef]],  # (2)
```

1. See [:material-code-braces: GeneratedPolicyPropertiesTypeDef](./type_defs.md#generatedpolicypropertiestypedef) 
2. See [:material-code-braces: GeneratedPolicyTypeDef](./type_defs.md#generatedpolicytypedef) 
## ListAccessPreviewFindingsResponseTypeDef

```python
# ListAccessPreviewFindingsResponseTypeDef definition

class ListAccessPreviewFindingsResponseTypeDef(TypedDict):
    findings: List[AccessPreviewFindingTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessPreviewFindingTypeDef](./type_defs.md#accesspreviewfindingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFindingsResponseTypeDef

```python
# ListFindingsResponseTypeDef definition

class ListFindingsResponseTypeDef(TypedDict):
    findings: List[FindingSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FindingSummaryTypeDef](./type_defs.md#findingsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFindingResponseTypeDef

```python
# GetFindingResponseTypeDef definition

class GetFindingResponseTypeDef(TypedDict):
    finding: FindingTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FindingTypeDef](./type_defs.md#findingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## S3BucketConfigurationTypeDef

```python
# S3BucketConfigurationTypeDef definition

class S3BucketConfigurationTypeDef(TypedDict):
    bucketPolicy: NotRequired[str],
    bucketAclGrants: NotRequired[Sequence[S3BucketAclGrantConfigurationTypeDef]],  # (1)
    bucketPublicAccessBlock: NotRequired[S3PublicAccessBlockConfigurationTypeDef],  # (2)
    accessPoints: NotRequired[Mapping[str, S3AccessPointConfigurationTypeDef]],  # (3)
```

1. See [:material-code-braces: S3BucketAclGrantConfigurationTypeDef](./type_defs.md#s3bucketaclgrantconfigurationtypedef) 
2. See [:material-code-braces: S3PublicAccessBlockConfigurationTypeDef](./type_defs.md#s3publicaccessblockconfigurationtypedef) 
3. See [:material-code-braces: S3AccessPointConfigurationTypeDef](./type_defs.md#s3accesspointconfigurationtypedef) 
## ValidatePolicyFindingTypeDef

```python
# ValidatePolicyFindingTypeDef definition

class ValidatePolicyFindingTypeDef(TypedDict):
    findingDetails: str,
    findingType: ValidatePolicyFindingTypeType,  # (1)
    issueCode: str,
    learnMoreLink: str,
    locations: List[LocationTypeDef],  # (2)
```

1. See [:material-code-brackets: ValidatePolicyFindingTypeType](./literals.md#validatepolicyfindingtypetype) 
2. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
## GetGeneratedPolicyResponseTypeDef

```python
# GetGeneratedPolicyResponseTypeDef definition

class GetGeneratedPolicyResponseTypeDef(TypedDict):
    jobDetails: JobDetailsTypeDef,  # (1)
    generatedPolicyResult: GeneratedPolicyResultTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: JobDetailsTypeDef](./type_defs.md#jobdetailstypedef) 
2. See [:material-code-braces: GeneratedPolicyResultTypeDef](./type_defs.md#generatedpolicyresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigurationTypeDef

```python
# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    ebsSnapshot: NotRequired[EbsSnapshotConfigurationTypeDef],  # (1)
    ecrRepository: NotRequired[EcrRepositoryConfigurationTypeDef],  # (2)
    iamRole: NotRequired[IamRoleConfigurationTypeDef],  # (3)
    efsFileSystem: NotRequired[EfsFileSystemConfigurationTypeDef],  # (4)
    kmsKey: NotRequired[KmsKeyConfigurationTypeDef],  # (5)
    rdsDbClusterSnapshot: NotRequired[RdsDbClusterSnapshotConfigurationTypeDef],  # (6)
    rdsDbSnapshot: NotRequired[RdsDbSnapshotConfigurationTypeDef],  # (7)
    secretsManagerSecret: NotRequired[SecretsManagerSecretConfigurationTypeDef],  # (8)
    s3Bucket: NotRequired[S3BucketConfigurationTypeDef],  # (9)
    snsTopic: NotRequired[SnsTopicConfigurationTypeDef],  # (10)
    sqsQueue: NotRequired[SqsQueueConfigurationTypeDef],  # (11)
```

1. See [:material-code-braces: EbsSnapshotConfigurationTypeDef](./type_defs.md#ebssnapshotconfigurationtypedef) 
2. See [:material-code-braces: EcrRepositoryConfigurationTypeDef](./type_defs.md#ecrrepositoryconfigurationtypedef) 
3. See [:material-code-braces: IamRoleConfigurationTypeDef](./type_defs.md#iamroleconfigurationtypedef) 
4. See [:material-code-braces: EfsFileSystemConfigurationTypeDef](./type_defs.md#efsfilesystemconfigurationtypedef) 
5. See [:material-code-braces: KmsKeyConfigurationTypeDef](./type_defs.md#kmskeyconfigurationtypedef) 
6. See [:material-code-braces: RdsDbClusterSnapshotConfigurationTypeDef](./type_defs.md#rdsdbclustersnapshotconfigurationtypedef) 
7. See [:material-code-braces: RdsDbSnapshotConfigurationTypeDef](./type_defs.md#rdsdbsnapshotconfigurationtypedef) 
8. See [:material-code-braces: SecretsManagerSecretConfigurationTypeDef](./type_defs.md#secretsmanagersecretconfigurationtypedef) 
9. See [:material-code-braces: S3BucketConfigurationTypeDef](./type_defs.md#s3bucketconfigurationtypedef) 
10. See [:material-code-braces: SnsTopicConfigurationTypeDef](./type_defs.md#snstopicconfigurationtypedef) 
11. See [:material-code-braces: SqsQueueConfigurationTypeDef](./type_defs.md#sqsqueueconfigurationtypedef) 
## ValidatePolicyResponseTypeDef

```python
# ValidatePolicyResponseTypeDef definition

class ValidatePolicyResponseTypeDef(TypedDict):
    findings: List[ValidatePolicyFindingTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidatePolicyFindingTypeDef](./type_defs.md#validatepolicyfindingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AccessPreviewTypeDef

```python
# AccessPreviewTypeDef definition

class AccessPreviewTypeDef(TypedDict):
    id: str,
    analyzerArn: str,
    configurations: Dict[str, ConfigurationTypeDef],  # (1)
    createdAt: datetime,
    status: AccessPreviewStatusType,  # (2)
    statusReason: NotRequired[AccessPreviewStatusReasonTypeDef],  # (3)
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-brackets: AccessPreviewStatusType](./literals.md#accesspreviewstatustype) 
3. See [:material-code-braces: AccessPreviewStatusReasonTypeDef](./type_defs.md#accesspreviewstatusreasontypedef) 
## CreateAccessPreviewRequestRequestTypeDef

```python
# CreateAccessPreviewRequestRequestTypeDef definition

class CreateAccessPreviewRequestRequestTypeDef(TypedDict):
    analyzerArn: str,
    configurations: Mapping[str, ConfigurationTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
## GetAccessPreviewResponseTypeDef

```python
# GetAccessPreviewResponseTypeDef definition

class GetAccessPreviewResponseTypeDef(TypedDict):
    accessPreview: AccessPreviewTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessPreviewTypeDef](./type_defs.md#accesspreviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
