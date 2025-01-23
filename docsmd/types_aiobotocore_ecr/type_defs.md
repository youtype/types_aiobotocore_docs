# Type definitions

> [Index](../README.md) > [ECR](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ecr)
    type annotations stubs module [types-aiobotocore-ecr](https://pypi.org/project/types-aiobotocore-ecr/).

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


## RegistryScanningRuleUnionTypeDef

```python
# RegistryScanningRuleUnionTypeDef definition

RegistryScanningRuleUnionTypeDef = Union[
    RegistryScanningRuleTypeDef,  # (1)
    RegistryScanningRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RegistryScanningRuleTypeDef](./type_defs.md#registryscanningruletypedef) 
2. See [:material-code-braces: RegistryScanningRuleOutputTypeDef](./type_defs.md#registryscanningruleoutputtypedef) 

## ReplicationRuleUnionTypeDef

```python
# ReplicationRuleUnionTypeDef definition

ReplicationRuleUnionTypeDef = Union[
    ReplicationRuleTypeDef,  # (1)
    ReplicationRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ReplicationRuleTypeDef](./type_defs.md#replicationruletypedef) 
2. See [:material-code-braces: ReplicationRuleOutputTypeDef](./type_defs.md#replicationruleoutputtypedef) 



## AttributeTypeDef

```python
# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    key: str,
    value: NotRequired[str],
```

## AuthorizationDataTypeDef

```python
# AuthorizationDataTypeDef definition

class AuthorizationDataTypeDef(TypedDict):
    authorizationToken: NotRequired[str],
    expiresAt: NotRequired[datetime],
    proxyEndpoint: NotRequired[str],
```

## AwsEcrContainerImageDetailsTypeDef

```python
# AwsEcrContainerImageDetailsTypeDef definition

class AwsEcrContainerImageDetailsTypeDef(TypedDict):
    architecture: NotRequired[str],
    author: NotRequired[str],
    imageHash: NotRequired[str],
    imageTags: NotRequired[List[str]],
    platform: NotRequired[str],
    pushedAt: NotRequired[datetime],
    registry: NotRequired[str],
    repositoryName: NotRequired[str],
```

## BatchCheckLayerAvailabilityRequestRequestTypeDef

```python
# BatchCheckLayerAvailabilityRequestRequestTypeDef definition

class BatchCheckLayerAvailabilityRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    layerDigests: Sequence[str],
    registryId: NotRequired[str],
```

## LayerFailureTypeDef

```python
# LayerFailureTypeDef definition

class LayerFailureTypeDef(TypedDict):
    layerDigest: NotRequired[str],
    failureCode: NotRequired[LayerFailureCodeType],  # (1)
    failureReason: NotRequired[str],
```

1. See [:material-code-brackets: LayerFailureCodeType](./literals.md#layerfailurecodetype) 
## LayerTypeDef

```python
# LayerTypeDef definition

class LayerTypeDef(TypedDict):
    layerDigest: NotRequired[str],
    layerAvailability: NotRequired[LayerAvailabilityType],  # (1)
    layerSize: NotRequired[int],
    mediaType: NotRequired[str],
```

1. See [:material-code-brackets: LayerAvailabilityType](./literals.md#layeravailabilitytype) 
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

## ImageIdentifierTypeDef

```python
# ImageIdentifierTypeDef definition

class ImageIdentifierTypeDef(TypedDict):
    imageDigest: NotRequired[str],
    imageTag: NotRequired[str],
```

## BatchGetRepositoryScanningConfigurationRequestRequestTypeDef

```python
# BatchGetRepositoryScanningConfigurationRequestRequestTypeDef definition

class BatchGetRepositoryScanningConfigurationRequestRequestTypeDef(TypedDict):
    repositoryNames: Sequence[str],
```

## RepositoryScanningConfigurationFailureTypeDef

```python
# RepositoryScanningConfigurationFailureTypeDef definition

class RepositoryScanningConfigurationFailureTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    failureCode: NotRequired[ScanningConfigurationFailureCodeType],  # (1)
    failureReason: NotRequired[str],
```

1. See [:material-code-brackets: ScanningConfigurationFailureCodeType](./literals.md#scanningconfigurationfailurecodetype) 
## CompleteLayerUploadRequestRequestTypeDef

```python
# CompleteLayerUploadRequestRequestTypeDef definition

class CompleteLayerUploadRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    uploadId: str,
    layerDigests: Sequence[str],
    registryId: NotRequired[str],
```

## CreatePullThroughCacheRuleRequestRequestTypeDef

```python
# CreatePullThroughCacheRuleRequestRequestTypeDef definition

class CreatePullThroughCacheRuleRequestRequestTypeDef(TypedDict):
    ecrRepositoryPrefix: str,
    upstreamRegistryUrl: str,
    registryId: NotRequired[str],
    upstreamRegistry: NotRequired[UpstreamRegistryType],  # (1)
    credentialArn: NotRequired[str],
```

1. See [:material-code-brackets: UpstreamRegistryType](./literals.md#upstreamregistrytype) 
## EncryptionConfigurationForRepositoryCreationTemplateTypeDef

```python
# EncryptionConfigurationForRepositoryCreationTemplateTypeDef definition

class EncryptionConfigurationForRepositoryCreationTemplateTypeDef(TypedDict):
    encryptionType: EncryptionTypeType,  # (1)
    kmsKey: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    encryptionType: EncryptionTypeType,  # (1)
    kmsKey: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## ImageScanningConfigurationTypeDef

```python
# ImageScanningConfigurationTypeDef definition

class ImageScanningConfigurationTypeDef(TypedDict):
    scanOnPush: NotRequired[bool],
```

## CvssScoreAdjustmentTypeDef

```python
# CvssScoreAdjustmentTypeDef definition

class CvssScoreAdjustmentTypeDef(TypedDict):
    metric: NotRequired[str],
    reason: NotRequired[str],
```

## CvssScoreTypeDef

```python
# CvssScoreTypeDef definition

class CvssScoreTypeDef(TypedDict):
    baseScore: NotRequired[float],
    scoringVector: NotRequired[str],
    source: NotRequired[str],
    version: NotRequired[str],
```

## DeleteLifecyclePolicyRequestRequestTypeDef

```python
# DeleteLifecyclePolicyRequestRequestTypeDef definition

class DeleteLifecyclePolicyRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
```

## DeletePullThroughCacheRuleRequestRequestTypeDef

```python
# DeletePullThroughCacheRuleRequestRequestTypeDef definition

class DeletePullThroughCacheRuleRequestRequestTypeDef(TypedDict):
    ecrRepositoryPrefix: str,
    registryId: NotRequired[str],
```

## DeleteRepositoryCreationTemplateRequestRequestTypeDef

```python
# DeleteRepositoryCreationTemplateRequestRequestTypeDef definition

class DeleteRepositoryCreationTemplateRequestRequestTypeDef(TypedDict):
    prefix: str,
```

## DeleteRepositoryPolicyRequestRequestTypeDef

```python
# DeleteRepositoryPolicyRequestRequestTypeDef definition

class DeleteRepositoryPolicyRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
```

## DeleteRepositoryRequestRequestTypeDef

```python
# DeleteRepositoryRequestRequestTypeDef definition

class DeleteRepositoryRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    force: NotRequired[bool],
```

## ImageReplicationStatusTypeDef

```python
# ImageReplicationStatusTypeDef definition

class ImageReplicationStatusTypeDef(TypedDict):
    region: NotRequired[str],
    registryId: NotRequired[str],
    status: NotRequired[ReplicationStatusType],  # (1)
    failureCode: NotRequired[str],
```

1. See [:material-code-brackets: ReplicationStatusType](./literals.md#replicationstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## ImageScanStatusTypeDef

```python
# ImageScanStatusTypeDef definition

class ImageScanStatusTypeDef(TypedDict):
    status: NotRequired[ScanStatusType],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: ScanStatusType](./literals.md#scanstatustype) 
## DescribeImagesFilterTypeDef

```python
# DescribeImagesFilterTypeDef definition

class DescribeImagesFilterTypeDef(TypedDict):
    tagStatus: NotRequired[TagStatusType],  # (1)
```

1. See [:material-code-brackets: TagStatusType](./literals.md#tagstatustype) 
## DescribePullThroughCacheRulesRequestRequestTypeDef

```python
# DescribePullThroughCacheRulesRequestRequestTypeDef definition

class DescribePullThroughCacheRulesRequestRequestTypeDef(TypedDict):
    registryId: NotRequired[str],
    ecrRepositoryPrefixes: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PullThroughCacheRuleTypeDef

```python
# PullThroughCacheRuleTypeDef definition

class PullThroughCacheRuleTypeDef(TypedDict):
    ecrRepositoryPrefix: NotRequired[str],
    upstreamRegistryUrl: NotRequired[str],
    createdAt: NotRequired[datetime],
    registryId: NotRequired[str],
    credentialArn: NotRequired[str],
    upstreamRegistry: NotRequired[UpstreamRegistryType],  # (1)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: UpstreamRegistryType](./literals.md#upstreamregistrytype) 
## DescribeRepositoriesRequestRequestTypeDef

```python
# DescribeRepositoriesRequestRequestTypeDef definition

class DescribeRepositoriesRequestRequestTypeDef(TypedDict):
    registryId: NotRequired[str],
    repositoryNames: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## DescribeRepositoryCreationTemplatesRequestRequestTypeDef

```python
# DescribeRepositoryCreationTemplatesRequestRequestTypeDef definition

class DescribeRepositoryCreationTemplatesRequestRequestTypeDef(TypedDict):
    prefixes: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetAccountSettingRequestRequestTypeDef

```python
# GetAccountSettingRequestRequestTypeDef definition

class GetAccountSettingRequestRequestTypeDef(TypedDict):
    name: str,
```

## GetAuthorizationTokenRequestRequestTypeDef

```python
# GetAuthorizationTokenRequestRequestTypeDef definition

class GetAuthorizationTokenRequestRequestTypeDef(TypedDict):
    registryIds: NotRequired[Sequence[str]],
```

## GetDownloadUrlForLayerRequestRequestTypeDef

```python
# GetDownloadUrlForLayerRequestRequestTypeDef definition

class GetDownloadUrlForLayerRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    layerDigest: str,
    registryId: NotRequired[str],
```

## LifecyclePolicyPreviewFilterTypeDef

```python
# LifecyclePolicyPreviewFilterTypeDef definition

class LifecyclePolicyPreviewFilterTypeDef(TypedDict):
    tagStatus: NotRequired[TagStatusType],  # (1)
```

1. See [:material-code-brackets: TagStatusType](./literals.md#tagstatustype) 
## LifecyclePolicyPreviewSummaryTypeDef

```python
# LifecyclePolicyPreviewSummaryTypeDef definition

class LifecyclePolicyPreviewSummaryTypeDef(TypedDict):
    expiringImageTotalCount: NotRequired[int],
```

## GetLifecyclePolicyRequestRequestTypeDef

```python
# GetLifecyclePolicyRequestRequestTypeDef definition

class GetLifecyclePolicyRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
```

## GetRepositoryPolicyRequestRequestTypeDef

```python
# GetRepositoryPolicyRequestRequestTypeDef definition

class GetRepositoryPolicyRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
```

## ImageScanFindingsSummaryTypeDef

```python
# ImageScanFindingsSummaryTypeDef definition

class ImageScanFindingsSummaryTypeDef(TypedDict):
    imageScanCompletedAt: NotRequired[datetime],
    vulnerabilitySourceUpdatedAt: NotRequired[datetime],
    findingSeverityCounts: NotRequired[Dict[FindingSeverityType, int]],  # (1)
```

1. See [:material-code-brackets: FindingSeverityType](./literals.md#findingseveritytype) 
## InitiateLayerUploadRequestRequestTypeDef

```python
# InitiateLayerUploadRequestRequestTypeDef definition

class InitiateLayerUploadRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
```

## LifecyclePolicyRuleActionTypeDef

```python
# LifecyclePolicyRuleActionTypeDef definition

class LifecyclePolicyRuleActionTypeDef(TypedDict):
    type: NotRequired[ImageActionTypeType],  # (1)
```

1. See [:material-code-brackets: ImageActionTypeType](./literals.md#imageactiontypetype) 
## ListImagesFilterTypeDef

```python
# ListImagesFilterTypeDef definition

class ListImagesFilterTypeDef(TypedDict):
    tagStatus: NotRequired[TagStatusType],  # (1)
```

1. See [:material-code-brackets: TagStatusType](./literals.md#tagstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## VulnerablePackageTypeDef

```python
# VulnerablePackageTypeDef definition

class VulnerablePackageTypeDef(TypedDict):
    arch: NotRequired[str],
    epoch: NotRequired[int],
    filePath: NotRequired[str],
    name: NotRequired[str],
    packageManager: NotRequired[str],
    release: NotRequired[str],
    sourceLayerHash: NotRequired[str],
    version: NotRequired[str],
    fixedInVersion: NotRequired[str],
```

## PutAccountSettingRequestRequestTypeDef

```python
# PutAccountSettingRequestRequestTypeDef definition

class PutAccountSettingRequestRequestTypeDef(TypedDict):
    name: str,
    value: str,
```

## PutImageRequestRequestTypeDef

```python
# PutImageRequestRequestTypeDef definition

class PutImageRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    imageManifest: str,
    registryId: NotRequired[str],
    imageManifestMediaType: NotRequired[str],
    imageTag: NotRequired[str],
    imageDigest: NotRequired[str],
```

## PutImageTagMutabilityRequestRequestTypeDef

```python
# PutImageTagMutabilityRequestRequestTypeDef definition

class PutImageTagMutabilityRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    imageTagMutability: ImageTagMutabilityType,  # (1)
    registryId: NotRequired[str],
```

1. See [:material-code-brackets: ImageTagMutabilityType](./literals.md#imagetagmutabilitytype) 
## PutLifecyclePolicyRequestRequestTypeDef

```python
# PutLifecyclePolicyRequestRequestTypeDef definition

class PutLifecyclePolicyRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    lifecyclePolicyText: str,
    registryId: NotRequired[str],
```

## PutRegistryPolicyRequestRequestTypeDef

```python
# PutRegistryPolicyRequestRequestTypeDef definition

class PutRegistryPolicyRequestRequestTypeDef(TypedDict):
    policyText: str,
```

## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    url: NotRequired[str],
    text: NotRequired[str],
```

## ScanningRepositoryFilterTypeDef

```python
# ScanningRepositoryFilterTypeDef definition

class ScanningRepositoryFilterTypeDef(TypedDict):
    filter: str,
    filterType: ScanningRepositoryFilterTypeType,  # (1)
```

1. See [:material-code-brackets: ScanningRepositoryFilterTypeType](./literals.md#scanningrepositoryfiltertypetype) 
## ReplicationDestinationTypeDef

```python
# ReplicationDestinationTypeDef definition

class ReplicationDestinationTypeDef(TypedDict):
    region: str,
    registryId: str,
```

## RepositoryFilterTypeDef

```python
# RepositoryFilterTypeDef definition

class RepositoryFilterTypeDef(TypedDict):
    filter: str,
    filterType: RepositoryFilterTypeType,  # (1)
```

1. See [:material-code-brackets: RepositoryFilterTypeType](./literals.md#repositoryfiltertypetype) 
## SetRepositoryPolicyRequestRequestTypeDef

```python
# SetRepositoryPolicyRequestRequestTypeDef definition

class SetRepositoryPolicyRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    policyText: str,
    registryId: NotRequired[str],
    force: NotRequired[bool],
```

## StartLifecyclePolicyPreviewRequestRequestTypeDef

```python
# StartLifecyclePolicyPreviewRequestRequestTypeDef definition

class StartLifecyclePolicyPreviewRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    lifecyclePolicyText: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdatePullThroughCacheRuleRequestRequestTypeDef

```python
# UpdatePullThroughCacheRuleRequestRequestTypeDef definition

class UpdatePullThroughCacheRuleRequestRequestTypeDef(TypedDict):
    ecrRepositoryPrefix: str,
    credentialArn: str,
    registryId: NotRequired[str],
```

## ValidatePullThroughCacheRuleRequestRequestTypeDef

```python
# ValidatePullThroughCacheRuleRequestRequestTypeDef definition

class ValidatePullThroughCacheRuleRequestRequestTypeDef(TypedDict):
    ecrRepositoryPrefix: str,
    registryId: NotRequired[str],
```

## ImageScanFindingTypeDef

```python
# ImageScanFindingTypeDef definition

class ImageScanFindingTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    uri: NotRequired[str],
    severity: NotRequired[FindingSeverityType],  # (1)
    attributes: NotRequired[List[AttributeTypeDef]],  # (2)
```

1. See [:material-code-brackets: FindingSeverityType](./literals.md#findingseveritytype) 
2. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    awsEcrContainerImage: NotRequired[AwsEcrContainerImageDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AwsEcrContainerImageDetailsTypeDef](./type_defs.md#awsecrcontainerimagedetailstypedef) 
## BatchCheckLayerAvailabilityResponseTypeDef

```python
# BatchCheckLayerAvailabilityResponseTypeDef definition

class BatchCheckLayerAvailabilityResponseTypeDef(TypedDict):
    layers: List[LayerTypeDef],  # (1)
    failures: List[LayerFailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LayerTypeDef](./type_defs.md#layertypedef) 
2. See [:material-code-braces: LayerFailureTypeDef](./type_defs.md#layerfailuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CompleteLayerUploadResponseTypeDef

```python
# CompleteLayerUploadResponseTypeDef definition

class CompleteLayerUploadResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    uploadId: str,
    layerDigest: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePullThroughCacheRuleResponseTypeDef

```python
# CreatePullThroughCacheRuleResponseTypeDef definition

class CreatePullThroughCacheRuleResponseTypeDef(TypedDict):
    ecrRepositoryPrefix: str,
    upstreamRegistryUrl: str,
    createdAt: datetime,
    registryId: str,
    upstreamRegistry: UpstreamRegistryType,  # (1)
    credentialArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: UpstreamRegistryType](./literals.md#upstreamregistrytype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteLifecyclePolicyResponseTypeDef

```python
# DeleteLifecyclePolicyResponseTypeDef definition

class DeleteLifecyclePolicyResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    lifecyclePolicyText: str,
    lastEvaluatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePullThroughCacheRuleResponseTypeDef

```python
# DeletePullThroughCacheRuleResponseTypeDef definition

class DeletePullThroughCacheRuleResponseTypeDef(TypedDict):
    ecrRepositoryPrefix: str,
    upstreamRegistryUrl: str,
    createdAt: datetime,
    registryId: str,
    credentialArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRegistryPolicyResponseTypeDef

```python
# DeleteRegistryPolicyResponseTypeDef definition

class DeleteRegistryPolicyResponseTypeDef(TypedDict):
    registryId: str,
    policyText: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRepositoryPolicyResponseTypeDef

```python
# DeleteRepositoryPolicyResponseTypeDef definition

class DeleteRepositoryPolicyResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    policyText: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountSettingResponseTypeDef

```python
# GetAccountSettingResponseTypeDef definition

class GetAccountSettingResponseTypeDef(TypedDict):
    name: str,
    value: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAuthorizationTokenResponseTypeDef

```python
# GetAuthorizationTokenResponseTypeDef definition

class GetAuthorizationTokenResponseTypeDef(TypedDict):
    authorizationData: List[AuthorizationDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthorizationDataTypeDef](./type_defs.md#authorizationdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDownloadUrlForLayerResponseTypeDef

```python
# GetDownloadUrlForLayerResponseTypeDef definition

class GetDownloadUrlForLayerResponseTypeDef(TypedDict):
    downloadUrl: str,
    layerDigest: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLifecyclePolicyResponseTypeDef

```python
# GetLifecyclePolicyResponseTypeDef definition

class GetLifecyclePolicyResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    lifecyclePolicyText: str,
    lastEvaluatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRegistryPolicyResponseTypeDef

```python
# GetRegistryPolicyResponseTypeDef definition

class GetRegistryPolicyResponseTypeDef(TypedDict):
    registryId: str,
    policyText: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRepositoryPolicyResponseTypeDef

```python
# GetRepositoryPolicyResponseTypeDef definition

class GetRepositoryPolicyResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    policyText: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InitiateLayerUploadResponseTypeDef

```python
# InitiateLayerUploadResponseTypeDef definition

class InitiateLayerUploadResponseTypeDef(TypedDict):
    uploadId: str,
    partSize: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAccountSettingResponseTypeDef

```python
# PutAccountSettingResponseTypeDef definition

class PutAccountSettingResponseTypeDef(TypedDict):
    name: str,
    value: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutImageTagMutabilityResponseTypeDef

```python
# PutImageTagMutabilityResponseTypeDef definition

class PutImageTagMutabilityResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    imageTagMutability: ImageTagMutabilityType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ImageTagMutabilityType](./literals.md#imagetagmutabilitytype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLifecyclePolicyResponseTypeDef

```python
# PutLifecyclePolicyResponseTypeDef definition

class PutLifecyclePolicyResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    lifecyclePolicyText: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRegistryPolicyResponseTypeDef

```python
# PutRegistryPolicyResponseTypeDef definition

class PutRegistryPolicyResponseTypeDef(TypedDict):
    registryId: str,
    policyText: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetRepositoryPolicyResponseTypeDef

```python
# SetRepositoryPolicyResponseTypeDef definition

class SetRepositoryPolicyResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    policyText: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartLifecyclePolicyPreviewResponseTypeDef

```python
# StartLifecyclePolicyPreviewResponseTypeDef definition

class StartLifecyclePolicyPreviewResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    lifecyclePolicyText: str,
    status: LifecyclePolicyPreviewStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LifecyclePolicyPreviewStatusType](./literals.md#lifecyclepolicypreviewstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePullThroughCacheRuleResponseTypeDef

```python
# UpdatePullThroughCacheRuleResponseTypeDef definition

class UpdatePullThroughCacheRuleResponseTypeDef(TypedDict):
    ecrRepositoryPrefix: str,
    registryId: str,
    updatedAt: datetime,
    credentialArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UploadLayerPartResponseTypeDef

```python
# UploadLayerPartResponseTypeDef definition

class UploadLayerPartResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    uploadId: str,
    lastByteReceived: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ValidatePullThroughCacheRuleResponseTypeDef

```python
# ValidatePullThroughCacheRuleResponseTypeDef definition

class ValidatePullThroughCacheRuleResponseTypeDef(TypedDict):
    ecrRepositoryPrefix: str,
    registryId: str,
    upstreamRegistryUrl: str,
    credentialArn: str,
    isValid: bool,
    failure: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteImageRequestRequestTypeDef

```python
# BatchDeleteImageRequestRequestTypeDef definition

class BatchDeleteImageRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    imageIds: Sequence[ImageIdentifierTypeDef],  # (1)
    registryId: NotRequired[str],
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
## BatchGetImageRequestRequestTypeDef

```python
# BatchGetImageRequestRequestTypeDef definition

class BatchGetImageRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    imageIds: Sequence[ImageIdentifierTypeDef],  # (1)
    registryId: NotRequired[str],
    acceptedMediaTypes: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
## DescribeImageReplicationStatusRequestRequestTypeDef

```python
# DescribeImageReplicationStatusRequestRequestTypeDef definition

class DescribeImageReplicationStatusRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    registryId: NotRequired[str],
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
## DescribeImageScanFindingsRequestRequestTypeDef

```python
# DescribeImageScanFindingsRequestRequestTypeDef definition

class DescribeImageScanFindingsRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    registryId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
## ImageFailureTypeDef

```python
# ImageFailureTypeDef definition

class ImageFailureTypeDef(TypedDict):
    imageId: NotRequired[ImageIdentifierTypeDef],  # (1)
    failureCode: NotRequired[ImageFailureCodeType],  # (2)
    failureReason: NotRequired[str],
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-brackets: ImageFailureCodeType](./literals.md#imagefailurecodetype) 
## ImageTypeDef

```python
# ImageTypeDef definition

class ImageTypeDef(TypedDict):
    registryId: NotRequired[str],
    repositoryName: NotRequired[str],
    imageId: NotRequired[ImageIdentifierTypeDef],  # (1)
    imageManifest: NotRequired[str],
    imageManifestMediaType: NotRequired[str],
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
## ListImagesResponseTypeDef

```python
# ListImagesResponseTypeDef definition

class ListImagesResponseTypeDef(TypedDict):
    imageIds: List[ImageIdentifierTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImageScanRequestRequestTypeDef

```python
# StartImageScanRequestRequestTypeDef definition

class StartImageScanRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    registryId: NotRequired[str],
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
## UploadLayerPartRequestRequestTypeDef

```python
# UploadLayerPartRequestRequestTypeDef definition

class UploadLayerPartRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    uploadId: str,
    partFirstByte: int,
    partLastByte: int,
    layerPartBlob: BlobTypeDef,
    registryId: NotRequired[str],
```

## CreateRepositoryCreationTemplateRequestRequestTypeDef

```python
# CreateRepositoryCreationTemplateRequestRequestTypeDef definition

class CreateRepositoryCreationTemplateRequestRequestTypeDef(TypedDict):
    prefix: str,
    appliedFor: Sequence[RCTAppliedForType],  # (1)
    description: NotRequired[str],
    encryptionConfiguration: NotRequired[EncryptionConfigurationForRepositoryCreationTemplateTypeDef],  # (2)
    resourceTags: NotRequired[Sequence[TagTypeDef]],  # (3)
    imageTagMutability: NotRequired[ImageTagMutabilityType],  # (4)
    repositoryPolicy: NotRequired[str],
    lifecyclePolicy: NotRequired[str],
    customRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: RCTAppliedForType](./literals.md#rctappliedfortype) 
2. See [:material-code-braces: EncryptionConfigurationForRepositoryCreationTemplateTypeDef](./type_defs.md#encryptionconfigurationforrepositorycreationtemplatetypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: ImageTagMutabilityType](./literals.md#imagetagmutabilitytype) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RepositoryCreationTemplateTypeDef

```python
# RepositoryCreationTemplateTypeDef definition

class RepositoryCreationTemplateTypeDef(TypedDict):
    prefix: NotRequired[str],
    description: NotRequired[str],
    encryptionConfiguration: NotRequired[EncryptionConfigurationForRepositoryCreationTemplateTypeDef],  # (1)
    resourceTags: NotRequired[List[TagTypeDef]],  # (2)
    imageTagMutability: NotRequired[ImageTagMutabilityType],  # (3)
    repositoryPolicy: NotRequired[str],
    lifecyclePolicy: NotRequired[str],
    appliedFor: NotRequired[List[RCTAppliedForType]],  # (4)
    customRoleArn: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: EncryptionConfigurationForRepositoryCreationTemplateTypeDef](./type_defs.md#encryptionconfigurationforrepositorycreationtemplatetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: ImageTagMutabilityType](./literals.md#imagetagmutabilitytype) 
4. See [:material-code-brackets: RCTAppliedForType](./literals.md#rctappliedfortype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateRepositoryCreationTemplateRequestRequestTypeDef

```python
# UpdateRepositoryCreationTemplateRequestRequestTypeDef definition

class UpdateRepositoryCreationTemplateRequestRequestTypeDef(TypedDict):
    prefix: str,
    description: NotRequired[str],
    encryptionConfiguration: NotRequired[EncryptionConfigurationForRepositoryCreationTemplateTypeDef],  # (1)
    resourceTags: NotRequired[Sequence[TagTypeDef]],  # (2)
    imageTagMutability: NotRequired[ImageTagMutabilityType],  # (3)
    repositoryPolicy: NotRequired[str],
    lifecyclePolicy: NotRequired[str],
    appliedFor: NotRequired[Sequence[RCTAppliedForType]],  # (4)
    customRoleArn: NotRequired[str],
```

1. See [:material-code-braces: EncryptionConfigurationForRepositoryCreationTemplateTypeDef](./type_defs.md#encryptionconfigurationforrepositorycreationtemplatetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: ImageTagMutabilityType](./literals.md#imagetagmutabilitytype) 
4. See [:material-code-brackets: RCTAppliedForType](./literals.md#rctappliedfortype) 
## CreateRepositoryRequestRequestTypeDef

```python
# CreateRepositoryRequestRequestTypeDef definition

class CreateRepositoryRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    imageTagMutability: NotRequired[ImageTagMutabilityType],  # (2)
    imageScanningConfiguration: NotRequired[ImageScanningConfigurationTypeDef],  # (3)
    encryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: ImageTagMutabilityType](./literals.md#imagetagmutabilitytype) 
3. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
4. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## PutImageScanningConfigurationRequestRequestTypeDef

```python
# PutImageScanningConfigurationRequestRequestTypeDef definition

class PutImageScanningConfigurationRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    imageScanningConfiguration: ImageScanningConfigurationTypeDef,  # (1)
    registryId: NotRequired[str],
```

1. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
## PutImageScanningConfigurationResponseTypeDef

```python
# PutImageScanningConfigurationResponseTypeDef definition

class PutImageScanningConfigurationResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    imageScanningConfiguration: ImageScanningConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RepositoryTypeDef

```python
# RepositoryTypeDef definition

class RepositoryTypeDef(TypedDict):
    repositoryArn: NotRequired[str],
    registryId: NotRequired[str],
    repositoryName: NotRequired[str],
    repositoryUri: NotRequired[str],
    createdAt: NotRequired[datetime],
    imageTagMutability: NotRequired[ImageTagMutabilityType],  # (1)
    imageScanningConfiguration: NotRequired[ImageScanningConfigurationTypeDef],  # (2)
    encryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: ImageTagMutabilityType](./literals.md#imagetagmutabilitytype) 
2. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## CvssScoreDetailsTypeDef

```python
# CvssScoreDetailsTypeDef definition

class CvssScoreDetailsTypeDef(TypedDict):
    adjustments: NotRequired[List[CvssScoreAdjustmentTypeDef]],  # (1)
    score: NotRequired[float],
    scoreSource: NotRequired[str],
    scoringVector: NotRequired[str],
    version: NotRequired[str],
```

1. See [:material-code-braces: CvssScoreAdjustmentTypeDef](./type_defs.md#cvssscoreadjustmenttypedef) 
## DescribeImageReplicationStatusResponseTypeDef

```python
# DescribeImageReplicationStatusResponseTypeDef definition

class DescribeImageReplicationStatusResponseTypeDef(TypedDict):
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    replicationStatuses: List[ImageReplicationStatusTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: ImageReplicationStatusTypeDef](./type_defs.md#imagereplicationstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImageScanFindingsRequestPaginateTypeDef

```python
# DescribeImageScanFindingsRequestPaginateTypeDef definition

class DescribeImageScanFindingsRequestPaginateTypeDef(TypedDict):
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    registryId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePullThroughCacheRulesRequestPaginateTypeDef

```python
# DescribePullThroughCacheRulesRequestPaginateTypeDef definition

class DescribePullThroughCacheRulesRequestPaginateTypeDef(TypedDict):
    registryId: NotRequired[str],
    ecrRepositoryPrefixes: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRepositoriesRequestPaginateTypeDef

```python
# DescribeRepositoriesRequestPaginateTypeDef definition

class DescribeRepositoriesRequestPaginateTypeDef(TypedDict):
    registryId: NotRequired[str],
    repositoryNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRepositoryCreationTemplatesRequestPaginateTypeDef

```python
# DescribeRepositoryCreationTemplatesRequestPaginateTypeDef definition

class DescribeRepositoryCreationTemplatesRequestPaginateTypeDef(TypedDict):
    prefixes: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeImageScanFindingsRequestWaitTypeDef

```python
# DescribeImageScanFindingsRequestWaitTypeDef definition

class DescribeImageScanFindingsRequestWaitTypeDef(TypedDict):
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    registryId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## StartImageScanResponseTypeDef

```python
# StartImageScanResponseTypeDef definition

class StartImageScanResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    imageScanStatus: ImageScanStatusTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: ImageScanStatusTypeDef](./type_defs.md#imagescanstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImagesRequestPaginateTypeDef

```python
# DescribeImagesRequestPaginateTypeDef definition

class DescribeImagesRequestPaginateTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    imageIds: NotRequired[Sequence[ImageIdentifierTypeDef]],  # (1)
    filter: NotRequired[DescribeImagesFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: DescribeImagesFilterTypeDef](./type_defs.md#describeimagesfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeImagesRequestRequestTypeDef

```python
# DescribeImagesRequestRequestTypeDef definition

class DescribeImagesRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    imageIds: NotRequired[Sequence[ImageIdentifierTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[DescribeImagesFilterTypeDef],  # (2)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: DescribeImagesFilterTypeDef](./type_defs.md#describeimagesfiltertypedef) 
## DescribePullThroughCacheRulesResponseTypeDef

```python
# DescribePullThroughCacheRulesResponseTypeDef definition

class DescribePullThroughCacheRulesResponseTypeDef(TypedDict):
    pullThroughCacheRules: List[PullThroughCacheRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PullThroughCacheRuleTypeDef](./type_defs.md#pullthroughcacheruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLifecyclePolicyPreviewRequestPaginateTypeDef

```python
# GetLifecyclePolicyPreviewRequestPaginateTypeDef definition

class GetLifecyclePolicyPreviewRequestPaginateTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    imageIds: NotRequired[Sequence[ImageIdentifierTypeDef]],  # (1)
    filter: NotRequired[LifecyclePolicyPreviewFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: LifecyclePolicyPreviewFilterTypeDef](./type_defs.md#lifecyclepolicypreviewfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetLifecyclePolicyPreviewRequestRequestTypeDef

```python
# GetLifecyclePolicyPreviewRequestRequestTypeDef definition

class GetLifecyclePolicyPreviewRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    imageIds: NotRequired[Sequence[ImageIdentifierTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[LifecyclePolicyPreviewFilterTypeDef],  # (2)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: LifecyclePolicyPreviewFilterTypeDef](./type_defs.md#lifecyclepolicypreviewfiltertypedef) 
## GetLifecyclePolicyPreviewRequestWaitTypeDef

```python
# GetLifecyclePolicyPreviewRequestWaitTypeDef definition

class GetLifecyclePolicyPreviewRequestWaitTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    imageIds: NotRequired[Sequence[ImageIdentifierTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[LifecyclePolicyPreviewFilterTypeDef],  # (2)
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: LifecyclePolicyPreviewFilterTypeDef](./type_defs.md#lifecyclepolicypreviewfiltertypedef) 
3. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## ImageDetailTypeDef

```python
# ImageDetailTypeDef definition

class ImageDetailTypeDef(TypedDict):
    registryId: NotRequired[str],
    repositoryName: NotRequired[str],
    imageDigest: NotRequired[str],
    imageTags: NotRequired[List[str]],
    imageSizeInBytes: NotRequired[int],
    imagePushedAt: NotRequired[datetime],
    imageScanStatus: NotRequired[ImageScanStatusTypeDef],  # (1)
    imageScanFindingsSummary: NotRequired[ImageScanFindingsSummaryTypeDef],  # (2)
    imageManifestMediaType: NotRequired[str],
    artifactMediaType: NotRequired[str],
    lastRecordedPullTime: NotRequired[datetime],
```

1. See [:material-code-braces: ImageScanStatusTypeDef](./type_defs.md#imagescanstatustypedef) 
2. See [:material-code-braces: ImageScanFindingsSummaryTypeDef](./type_defs.md#imagescanfindingssummarytypedef) 
## LifecyclePolicyPreviewResultTypeDef

```python
# LifecyclePolicyPreviewResultTypeDef definition

class LifecyclePolicyPreviewResultTypeDef(TypedDict):
    imageTags: NotRequired[List[str]],
    imageDigest: NotRequired[str],
    imagePushedAt: NotRequired[datetime],
    action: NotRequired[LifecyclePolicyRuleActionTypeDef],  # (1)
    appliedRulePriority: NotRequired[int],
```

1. See [:material-code-braces: LifecyclePolicyRuleActionTypeDef](./type_defs.md#lifecyclepolicyruleactiontypedef) 
## ListImagesRequestPaginateTypeDef

```python
# ListImagesRequestPaginateTypeDef definition

class ListImagesRequestPaginateTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    filter: NotRequired[ListImagesFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListImagesFilterTypeDef](./type_defs.md#listimagesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImagesRequestRequestTypeDef

```python
# ListImagesRequestRequestTypeDef definition

class ListImagesRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[ListImagesFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ListImagesFilterTypeDef](./type_defs.md#listimagesfiltertypedef) 
## PackageVulnerabilityDetailsTypeDef

```python
# PackageVulnerabilityDetailsTypeDef definition

class PackageVulnerabilityDetailsTypeDef(TypedDict):
    cvss: NotRequired[List[CvssScoreTypeDef]],  # (1)
    referenceUrls: NotRequired[List[str]],
    relatedVulnerabilities: NotRequired[List[str]],
    source: NotRequired[str],
    sourceUrl: NotRequired[str],
    vendorCreatedAt: NotRequired[datetime],
    vendorSeverity: NotRequired[str],
    vendorUpdatedAt: NotRequired[datetime],
    vulnerabilityId: NotRequired[str],
    vulnerablePackages: NotRequired[List[VulnerablePackageTypeDef]],  # (2)
```

1. See [:material-code-braces: CvssScoreTypeDef](./type_defs.md#cvssscoretypedef) 
2. See [:material-code-braces: VulnerablePackageTypeDef](./type_defs.md#vulnerablepackagetypedef) 
## RemediationTypeDef

```python
# RemediationTypeDef definition

class RemediationTypeDef(TypedDict):
    recommendation: NotRequired[RecommendationTypeDef],  # (1)
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
## RegistryScanningRuleOutputTypeDef

```python
# RegistryScanningRuleOutputTypeDef definition

class RegistryScanningRuleOutputTypeDef(TypedDict):
    scanFrequency: ScanFrequencyType,  # (1)
    repositoryFilters: List[ScanningRepositoryFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: ScanFrequencyType](./literals.md#scanfrequencytype) 
2. See [:material-code-braces: ScanningRepositoryFilterTypeDef](./type_defs.md#scanningrepositoryfiltertypedef) 
## RegistryScanningRuleTypeDef

```python
# RegistryScanningRuleTypeDef definition

class RegistryScanningRuleTypeDef(TypedDict):
    scanFrequency: ScanFrequencyType,  # (1)
    repositoryFilters: Sequence[ScanningRepositoryFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: ScanFrequencyType](./literals.md#scanfrequencytype) 
2. See [:material-code-braces: ScanningRepositoryFilterTypeDef](./type_defs.md#scanningrepositoryfiltertypedef) 
## RepositoryScanningConfigurationTypeDef

```python
# RepositoryScanningConfigurationTypeDef definition

class RepositoryScanningConfigurationTypeDef(TypedDict):
    repositoryArn: NotRequired[str],
    repositoryName: NotRequired[str],
    scanOnPush: NotRequired[bool],
    scanFrequency: NotRequired[ScanFrequencyType],  # (1)
    appliedScanFilters: NotRequired[List[ScanningRepositoryFilterTypeDef]],  # (2)
```

1. See [:material-code-brackets: ScanFrequencyType](./literals.md#scanfrequencytype) 
2. See [:material-code-braces: ScanningRepositoryFilterTypeDef](./type_defs.md#scanningrepositoryfiltertypedef) 
## ReplicationRuleOutputTypeDef

```python
# ReplicationRuleOutputTypeDef definition

class ReplicationRuleOutputTypeDef(TypedDict):
    destinations: List[ReplicationDestinationTypeDef],  # (1)
    repositoryFilters: NotRequired[List[RepositoryFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: ReplicationDestinationTypeDef](./type_defs.md#replicationdestinationtypedef) 
2. See [:material-code-braces: RepositoryFilterTypeDef](./type_defs.md#repositoryfiltertypedef) 
## ReplicationRuleTypeDef

```python
# ReplicationRuleTypeDef definition

class ReplicationRuleTypeDef(TypedDict):
    destinations: Sequence[ReplicationDestinationTypeDef],  # (1)
    repositoryFilters: NotRequired[Sequence[RepositoryFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: ReplicationDestinationTypeDef](./type_defs.md#replicationdestinationtypedef) 
2. See [:material-code-braces: RepositoryFilterTypeDef](./type_defs.md#repositoryfiltertypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    details: NotRequired[ResourceDetailsTypeDef],  # (1)
    id: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    type: NotRequired[str],
```

1. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
## BatchDeleteImageResponseTypeDef

```python
# BatchDeleteImageResponseTypeDef definition

class BatchDeleteImageResponseTypeDef(TypedDict):
    imageIds: List[ImageIdentifierTypeDef],  # (1)
    failures: List[ImageFailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: ImageFailureTypeDef](./type_defs.md#imagefailuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetImageResponseTypeDef

```python
# BatchGetImageResponseTypeDef definition

class BatchGetImageResponseTypeDef(TypedDict):
    images: List[ImageTypeDef],  # (1)
    failures: List[ImageFailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ImageFailureTypeDef](./type_defs.md#imagefailuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutImageResponseTypeDef

```python
# PutImageResponseTypeDef definition

class PutImageResponseTypeDef(TypedDict):
    image: ImageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRepositoryCreationTemplateResponseTypeDef

```python
# CreateRepositoryCreationTemplateResponseTypeDef definition

class CreateRepositoryCreationTemplateResponseTypeDef(TypedDict):
    registryId: str,
    repositoryCreationTemplate: RepositoryCreationTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryCreationTemplateTypeDef](./type_defs.md#repositorycreationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRepositoryCreationTemplateResponseTypeDef

```python
# DeleteRepositoryCreationTemplateResponseTypeDef definition

class DeleteRepositoryCreationTemplateResponseTypeDef(TypedDict):
    registryId: str,
    repositoryCreationTemplate: RepositoryCreationTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryCreationTemplateTypeDef](./type_defs.md#repositorycreationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRepositoryCreationTemplatesResponseTypeDef

```python
# DescribeRepositoryCreationTemplatesResponseTypeDef definition

class DescribeRepositoryCreationTemplatesResponseTypeDef(TypedDict):
    registryId: str,
    repositoryCreationTemplates: List[RepositoryCreationTemplateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RepositoryCreationTemplateTypeDef](./type_defs.md#repositorycreationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRepositoryCreationTemplateResponseTypeDef

```python
# UpdateRepositoryCreationTemplateResponseTypeDef definition

class UpdateRepositoryCreationTemplateResponseTypeDef(TypedDict):
    registryId: str,
    repositoryCreationTemplate: RepositoryCreationTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryCreationTemplateTypeDef](./type_defs.md#repositorycreationtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRepositoryResponseTypeDef

```python
# CreateRepositoryResponseTypeDef definition

class CreateRepositoryResponseTypeDef(TypedDict):
    repository: RepositoryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryTypeDef](./type_defs.md#repositorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRepositoryResponseTypeDef

```python
# DeleteRepositoryResponseTypeDef definition

class DeleteRepositoryResponseTypeDef(TypedDict):
    repository: RepositoryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryTypeDef](./type_defs.md#repositorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRepositoriesResponseTypeDef

```python
# DescribeRepositoriesResponseTypeDef definition

class DescribeRepositoriesResponseTypeDef(TypedDict):
    repositories: List[RepositoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RepositoryTypeDef](./type_defs.md#repositorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScoreDetailsTypeDef

```python
# ScoreDetailsTypeDef definition

class ScoreDetailsTypeDef(TypedDict):
    cvss: NotRequired[CvssScoreDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: CvssScoreDetailsTypeDef](./type_defs.md#cvssscoredetailstypedef) 
## DescribeImagesResponseTypeDef

```python
# DescribeImagesResponseTypeDef definition

class DescribeImagesResponseTypeDef(TypedDict):
    imageDetails: List[ImageDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImageDetailTypeDef](./type_defs.md#imagedetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLifecyclePolicyPreviewResponseTypeDef

```python
# GetLifecyclePolicyPreviewResponseTypeDef definition

class GetLifecyclePolicyPreviewResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    lifecyclePolicyText: str,
    status: LifecyclePolicyPreviewStatusType,  # (1)
    previewResults: List[LifecyclePolicyPreviewResultTypeDef],  # (2)
    summary: LifecyclePolicyPreviewSummaryTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: LifecyclePolicyPreviewStatusType](./literals.md#lifecyclepolicypreviewstatustype) 
2. See [:material-code-braces: LifecyclePolicyPreviewResultTypeDef](./type_defs.md#lifecyclepolicypreviewresulttypedef) 
3. See [:material-code-braces: LifecyclePolicyPreviewSummaryTypeDef](./type_defs.md#lifecyclepolicypreviewsummarytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegistryScanningConfigurationTypeDef

```python
# RegistryScanningConfigurationTypeDef definition

class RegistryScanningConfigurationTypeDef(TypedDict):
    scanType: NotRequired[ScanTypeType],  # (1)
    rules: NotRequired[List[RegistryScanningRuleOutputTypeDef]],  # (2)
```

1. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
2. See [:material-code-braces: RegistryScanningRuleOutputTypeDef](./type_defs.md#registryscanningruleoutputtypedef) 
## BatchGetRepositoryScanningConfigurationResponseTypeDef

```python
# BatchGetRepositoryScanningConfigurationResponseTypeDef definition

class BatchGetRepositoryScanningConfigurationResponseTypeDef(TypedDict):
    scanningConfigurations: List[RepositoryScanningConfigurationTypeDef],  # (1)
    failures: List[RepositoryScanningConfigurationFailureTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RepositoryScanningConfigurationTypeDef](./type_defs.md#repositoryscanningconfigurationtypedef) 
2. See [:material-code-braces: RepositoryScanningConfigurationFailureTypeDef](./type_defs.md#repositoryscanningconfigurationfailuretypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicationConfigurationOutputTypeDef

```python
# ReplicationConfigurationOutputTypeDef definition

class ReplicationConfigurationOutputTypeDef(TypedDict):
    rules: List[ReplicationRuleOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ReplicationRuleOutputTypeDef](./type_defs.md#replicationruleoutputtypedef) 
## EnhancedImageScanFindingTypeDef

```python
# EnhancedImageScanFindingTypeDef definition

class EnhancedImageScanFindingTypeDef(TypedDict):
    awsAccountId: NotRequired[str],
    description: NotRequired[str],
    findingArn: NotRequired[str],
    firstObservedAt: NotRequired[datetime],
    lastObservedAt: NotRequired[datetime],
    packageVulnerabilityDetails: NotRequired[PackageVulnerabilityDetailsTypeDef],  # (1)
    remediation: NotRequired[RemediationTypeDef],  # (2)
    resources: NotRequired[List[ResourceTypeDef]],  # (3)
    score: NotRequired[float],
    scoreDetails: NotRequired[ScoreDetailsTypeDef],  # (4)
    severity: NotRequired[str],
    status: NotRequired[str],
    title: NotRequired[str],
    type: NotRequired[str],
    updatedAt: NotRequired[datetime],
    fixAvailable: NotRequired[str],
    exploitAvailable: NotRequired[str],
```

1. See [:material-code-braces: PackageVulnerabilityDetailsTypeDef](./type_defs.md#packagevulnerabilitydetailstypedef) 
2. See [:material-code-braces: RemediationTypeDef](./type_defs.md#remediationtypedef) 
3. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
4. See [:material-code-braces: ScoreDetailsTypeDef](./type_defs.md#scoredetailstypedef) 
## GetRegistryScanningConfigurationResponseTypeDef

```python
# GetRegistryScanningConfigurationResponseTypeDef definition

class GetRegistryScanningConfigurationResponseTypeDef(TypedDict):
    registryId: str,
    scanningConfiguration: RegistryScanningConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegistryScanningConfigurationTypeDef](./type_defs.md#registryscanningconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRegistryScanningConfigurationResponseTypeDef

```python
# PutRegistryScanningConfigurationResponseTypeDef definition

class PutRegistryScanningConfigurationResponseTypeDef(TypedDict):
    registryScanningConfiguration: RegistryScanningConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegistryScanningConfigurationTypeDef](./type_defs.md#registryscanningconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRegistryScanningConfigurationRequestRequestTypeDef

```python
# PutRegistryScanningConfigurationRequestRequestTypeDef definition

class PutRegistryScanningConfigurationRequestRequestTypeDef(TypedDict):
    scanType: NotRequired[ScanTypeType],  # (1)
    rules: NotRequired[Sequence[RegistryScanningRuleUnionTypeDef]],  # (2)
```

1. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
2. See [:material-code-braces: RegistryScanningRuleTypeDef](./type_defs.md#registryscanningruletypedef) [:material-code-braces: RegistryScanningRuleOutputTypeDef](./type_defs.md#registryscanningruleoutputtypedef) 
## DescribeRegistryResponseTypeDef

```python
# DescribeRegistryResponseTypeDef definition

class DescribeRegistryResponseTypeDef(TypedDict):
    registryId: str,
    replicationConfiguration: ReplicationConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationConfigurationOutputTypeDef](./type_defs.md#replicationconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutReplicationConfigurationResponseTypeDef

```python
# PutReplicationConfigurationResponseTypeDef definition

class PutReplicationConfigurationResponseTypeDef(TypedDict):
    replicationConfiguration: ReplicationConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationConfigurationOutputTypeDef](./type_defs.md#replicationconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicationConfigurationTypeDef

```python
# ReplicationConfigurationTypeDef definition

class ReplicationConfigurationTypeDef(TypedDict):
    rules: Sequence[ReplicationRuleUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ReplicationRuleTypeDef](./type_defs.md#replicationruletypedef) [:material-code-braces: ReplicationRuleOutputTypeDef](./type_defs.md#replicationruleoutputtypedef) 
## ImageScanFindingsTypeDef

```python
# ImageScanFindingsTypeDef definition

class ImageScanFindingsTypeDef(TypedDict):
    imageScanCompletedAt: NotRequired[datetime],
    vulnerabilitySourceUpdatedAt: NotRequired[datetime],
    findingSeverityCounts: NotRequired[Dict[FindingSeverityType, int]],  # (1)
    findings: NotRequired[List[ImageScanFindingTypeDef]],  # (2)
    enhancedFindings: NotRequired[List[EnhancedImageScanFindingTypeDef]],  # (3)
```

1. See [:material-code-brackets: FindingSeverityType](./literals.md#findingseveritytype) 
2. See [:material-code-braces: ImageScanFindingTypeDef](./type_defs.md#imagescanfindingtypedef) 
3. See [:material-code-braces: EnhancedImageScanFindingTypeDef](./type_defs.md#enhancedimagescanfindingtypedef) 
## PutReplicationConfigurationRequestRequestTypeDef

```python
# PutReplicationConfigurationRequestRequestTypeDef definition

class PutReplicationConfigurationRequestRequestTypeDef(TypedDict):
    replicationConfiguration: ReplicationConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef) 
## DescribeImageScanFindingsResponseTypeDef

```python
# DescribeImageScanFindingsResponseTypeDef definition

class DescribeImageScanFindingsResponseTypeDef(TypedDict):
    registryId: str,
    repositoryName: str,
    imageId: ImageIdentifierTypeDef,  # (1)
    imageScanStatus: ImageScanStatusTypeDef,  # (2)
    imageScanFindings: ImageScanFindingsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: ImageScanStatusTypeDef](./type_defs.md#imagescanstatustypedef) 
3. See [:material-code-braces: ImageScanFindingsTypeDef](./type_defs.md#imagescanfindingstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
