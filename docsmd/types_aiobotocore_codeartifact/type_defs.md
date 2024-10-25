# Type definitions

> [Index](../README.md) > [CodeArtifact](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeArtifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
    type annotations stubs module [types-aiobotocore-codeartifact](https://pypi.org/project/types-aiobotocore-codeartifact/).

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




## AssetSummaryTypeDef

```python
# AssetSummaryTypeDef definition

class AssetSummaryTypeDef(TypedDict):
    name: str,
    size: NotRequired[int],
    hashes: NotRequired[Dict[HashAlgorithmType, str]],  # (1)
```

1. See [:material-code-brackets: HashAlgorithmType](./literals.md#hashalgorithmtype) 
## AssociateExternalConnectionRequestRequestTypeDef

```python
# AssociateExternalConnectionRequestRequestTypeDef definition

class AssociateExternalConnectionRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    externalConnection: str,
    domainOwner: NotRequired[str],
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

## AssociatedPackageTypeDef

```python
# AssociatedPackageTypeDef definition

class AssociatedPackageTypeDef(TypedDict):
    format: NotRequired[PackageFormatType],  # (1)
    namespace: NotRequired[str],
    package: NotRequired[str],
    associationType: NotRequired[PackageGroupAssociationTypeType],  # (2)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: PackageGroupAssociationTypeType](./literals.md#packagegroupassociationtypetype) 
## CopyPackageVersionsRequestRequestTypeDef

```python
# CopyPackageVersionsRequestRequestTypeDef definition

class CopyPackageVersionsRequestRequestTypeDef(TypedDict):
    domain: str,
    sourceRepository: str,
    destinationRepository: str,
    format: PackageFormatType,  # (1)
    package: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    versions: NotRequired[Sequence[str]],
    versionRevisions: NotRequired[Mapping[str, str]],
    allowOverwrite: NotRequired[bool],
    includeFromUpstream: NotRequired[bool],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
## PackageVersionErrorTypeDef

```python
# PackageVersionErrorTypeDef definition

class PackageVersionErrorTypeDef(TypedDict):
    errorCode: NotRequired[PackageVersionErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: PackageVersionErrorCodeType](./literals.md#packageversionerrorcodetype) 
## SuccessfulPackageVersionInfoTypeDef

```python
# SuccessfulPackageVersionInfoTypeDef definition

class SuccessfulPackageVersionInfoTypeDef(TypedDict):
    revision: NotRequired[str],
    status: NotRequired[PackageVersionStatusType],  # (1)
```

1. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## DomainDescriptionTypeDef

```python
# DomainDescriptionTypeDef definition

class DomainDescriptionTypeDef(TypedDict):
    name: NotRequired[str],
    owner: NotRequired[str],
    arn: NotRequired[str],
    status: NotRequired[DomainStatusType],  # (1)
    createdTime: NotRequired[datetime],
    encryptionKey: NotRequired[str],
    repositoryCount: NotRequired[int],
    assetSizeBytes: NotRequired[int],
    s3BucketArn: NotRequired[str],
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
## UpstreamRepositoryTypeDef

```python
# UpstreamRepositoryTypeDef definition

class UpstreamRepositoryTypeDef(TypedDict):
    repositoryName: str,
```

## DeleteDomainPermissionsPolicyRequestRequestTypeDef

```python
# DeleteDomainPermissionsPolicyRequestRequestTypeDef definition

class DeleteDomainPermissionsPolicyRequestRequestTypeDef(TypedDict):
    domain: str,
    domainOwner: NotRequired[str],
    policyRevision: NotRequired[str],
```

## ResourcePolicyTypeDef

```python
# ResourcePolicyTypeDef definition

class ResourcePolicyTypeDef(TypedDict):
    resourceArn: NotRequired[str],
    revision: NotRequired[str],
    document: NotRequired[str],
```

## DeleteDomainRequestRequestTypeDef

```python
# DeleteDomainRequestRequestTypeDef definition

class DeleteDomainRequestRequestTypeDef(TypedDict):
    domain: str,
    domainOwner: NotRequired[str],
```

## DeletePackageGroupRequestRequestTypeDef

```python
# DeletePackageGroupRequestRequestTypeDef definition

class DeletePackageGroupRequestRequestTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    domainOwner: NotRequired[str],
```

## DeletePackageRequestRequestTypeDef

```python
# DeletePackageRequestRequestTypeDef definition

class DeletePackageRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
## DeletePackageVersionsRequestRequestTypeDef

```python
# DeletePackageVersionsRequestRequestTypeDef definition

class DeletePackageVersionsRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    versions: Sequence[str],
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    expectedStatus: NotRequired[PackageVersionStatusType],  # (2)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
## DeleteRepositoryPermissionsPolicyRequestRequestTypeDef

```python
# DeleteRepositoryPermissionsPolicyRequestRequestTypeDef definition

class DeleteRepositoryPermissionsPolicyRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    domainOwner: NotRequired[str],
    policyRevision: NotRequired[str],
```

## DeleteRepositoryRequestRequestTypeDef

```python
# DeleteRepositoryRequestRequestTypeDef definition

class DeleteRepositoryRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    domainOwner: NotRequired[str],
```

## DescribeDomainRequestRequestTypeDef

```python
# DescribeDomainRequestRequestTypeDef definition

class DescribeDomainRequestRequestTypeDef(TypedDict):
    domain: str,
    domainOwner: NotRequired[str],
```

## DescribePackageGroupRequestRequestTypeDef

```python
# DescribePackageGroupRequestRequestTypeDef definition

class DescribePackageGroupRequestRequestTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    domainOwner: NotRequired[str],
```

## DescribePackageRequestRequestTypeDef

```python
# DescribePackageRequestRequestTypeDef definition

class DescribePackageRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
## DescribePackageVersionRequestRequestTypeDef

```python
# DescribePackageVersionRequestRequestTypeDef definition

class DescribePackageVersionRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    packageVersion: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
## DescribeRepositoryRequestRequestTypeDef

```python
# DescribeRepositoryRequestRequestTypeDef definition

class DescribeRepositoryRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    domainOwner: NotRequired[str],
```

## DisassociateExternalConnectionRequestRequestTypeDef

```python
# DisassociateExternalConnectionRequestRequestTypeDef definition

class DisassociateExternalConnectionRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    externalConnection: str,
    domainOwner: NotRequired[str],
```

## DisposePackageVersionsRequestRequestTypeDef

```python
# DisposePackageVersionsRequestRequestTypeDef definition

class DisposePackageVersionsRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    versions: Sequence[str],
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    versionRevisions: NotRequired[Mapping[str, str]],
    expectedStatus: NotRequired[PackageVersionStatusType],  # (2)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
## DomainEntryPointTypeDef

```python
# DomainEntryPointTypeDef definition

class DomainEntryPointTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    externalConnectionName: NotRequired[str],
```

## DomainSummaryTypeDef

```python
# DomainSummaryTypeDef definition

class DomainSummaryTypeDef(TypedDict):
    name: NotRequired[str],
    owner: NotRequired[str],
    arn: NotRequired[str],
    status: NotRequired[DomainStatusType],  # (1)
    createdTime: NotRequired[datetime],
    encryptionKey: NotRequired[str],
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
## GetAssociatedPackageGroupRequestRequestTypeDef

```python
# GetAssociatedPackageGroupRequestRequestTypeDef definition

class GetAssociatedPackageGroupRequestRequestTypeDef(TypedDict):
    domain: str,
    format: PackageFormatType,  # (1)
    package: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
## GetAuthorizationTokenRequestRequestTypeDef

```python
# GetAuthorizationTokenRequestRequestTypeDef definition

class GetAuthorizationTokenRequestRequestTypeDef(TypedDict):
    domain: str,
    domainOwner: NotRequired[str],
    durationSeconds: NotRequired[int],
```

## GetDomainPermissionsPolicyRequestRequestTypeDef

```python
# GetDomainPermissionsPolicyRequestRequestTypeDef definition

class GetDomainPermissionsPolicyRequestRequestTypeDef(TypedDict):
    domain: str,
    domainOwner: NotRequired[str],
```

## GetPackageVersionAssetRequestRequestTypeDef

```python
# GetPackageVersionAssetRequestRequestTypeDef definition

class GetPackageVersionAssetRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    packageVersion: str,
    asset: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    packageVersionRevision: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
## GetPackageVersionReadmeRequestRequestTypeDef

```python
# GetPackageVersionReadmeRequestRequestTypeDef definition

class GetPackageVersionReadmeRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    packageVersion: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
## GetRepositoryEndpointRequestRequestTypeDef

```python
# GetRepositoryEndpointRequestRequestTypeDef definition

class GetRepositoryEndpointRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    domainOwner: NotRequired[str],
    endpointType: NotRequired[EndpointTypeType],  # (2)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
## GetRepositoryPermissionsPolicyRequestRequestTypeDef

```python
# GetRepositoryPermissionsPolicyRequestRequestTypeDef definition

class GetRepositoryPermissionsPolicyRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    domainOwner: NotRequired[str],
```

## LicenseInfoTypeDef

```python
# LicenseInfoTypeDef definition

class LicenseInfoTypeDef(TypedDict):
    name: NotRequired[str],
    url: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAllowedRepositoriesForGroupRequestRequestTypeDef

```python
# ListAllowedRepositoriesForGroupRequestRequestTypeDef definition

class ListAllowedRepositoriesForGroupRequestRequestTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    originRestrictionType: PackageGroupOriginRestrictionTypeType,  # (1)
    domainOwner: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: PackageGroupOriginRestrictionTypeType](./literals.md#packagegrouporiginrestrictiontypetype) 
## ListAssociatedPackagesRequestRequestTypeDef

```python
# ListAssociatedPackagesRequestRequestTypeDef definition

class ListAssociatedPackagesRequestRequestTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    domainOwner: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    preview: NotRequired[bool],
```

## ListDomainsRequestRequestTypeDef

```python
# ListDomainsRequestRequestTypeDef definition

class ListDomainsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListPackageGroupsRequestRequestTypeDef

```python
# ListPackageGroupsRequestRequestTypeDef definition

class ListPackageGroupsRequestRequestTypeDef(TypedDict):
    domain: str,
    domainOwner: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    prefix: NotRequired[str],
```

## ListPackageVersionAssetsRequestRequestTypeDef

```python
# ListPackageVersionAssetsRequestRequestTypeDef definition

class ListPackageVersionAssetsRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    packageVersion: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
## ListPackageVersionDependenciesRequestRequestTypeDef

```python
# ListPackageVersionDependenciesRequestRequestTypeDef definition

class ListPackageVersionDependenciesRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    packageVersion: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
## PackageDependencyTypeDef

```python
# PackageDependencyTypeDef definition

class PackageDependencyTypeDef(TypedDict):
    namespace: NotRequired[str],
    package: NotRequired[str],
    dependencyType: NotRequired[str],
    versionRequirement: NotRequired[str],
```

## ListPackageVersionsRequestRequestTypeDef

```python
# ListPackageVersionsRequestRequestTypeDef definition

class ListPackageVersionsRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    status: NotRequired[PackageVersionStatusType],  # (2)
    sortBy: NotRequired[PackageVersionSortTypeType],  # (3)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    originType: NotRequired[PackageVersionOriginTypeType],  # (4)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
3. See [:material-code-brackets: PackageVersionSortTypeType](./literals.md#packageversionsorttypetype) 
4. See [:material-code-brackets: PackageVersionOriginTypeType](./literals.md#packageversionorigintypetype) 
## ListPackagesRequestRequestTypeDef

```python
# ListPackagesRequestRequestTypeDef definition

class ListPackagesRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    domainOwner: NotRequired[str],
    format: NotRequired[PackageFormatType],  # (1)
    namespace: NotRequired[str],
    packagePrefix: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    publish: NotRequired[AllowPublishType],  # (2)
    upstream: NotRequired[AllowUpstreamType],  # (3)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: AllowPublishType](./literals.md#allowpublishtype) 
3. See [:material-code-brackets: AllowUpstreamType](./literals.md#allowupstreamtype) 
## ListRepositoriesInDomainRequestRequestTypeDef

```python
# ListRepositoriesInDomainRequestRequestTypeDef definition

class ListRepositoriesInDomainRequestRequestTypeDef(TypedDict):
    domain: str,
    domainOwner: NotRequired[str],
    administratorAccount: NotRequired[str],
    repositoryPrefix: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## RepositorySummaryTypeDef

```python
# RepositorySummaryTypeDef definition

class RepositorySummaryTypeDef(TypedDict):
    name: NotRequired[str],
    administratorAccount: NotRequired[str],
    domainName: NotRequired[str],
    domainOwner: NotRequired[str],
    arn: NotRequired[str],
    description: NotRequired[str],
    createdTime: NotRequired[datetime],
```

## ListRepositoriesRequestRequestTypeDef

```python
# ListRepositoriesRequestRequestTypeDef definition

class ListRepositoriesRequestRequestTypeDef(TypedDict):
    repositoryPrefix: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListSubPackageGroupsRequestRequestTypeDef

```python
# ListSubPackageGroupsRequestRequestTypeDef definition

class ListSubPackageGroupsRequestRequestTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    domainOwner: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PackageGroupAllowedRepositoryTypeDef

```python
# PackageGroupAllowedRepositoryTypeDef definition

class PackageGroupAllowedRepositoryTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    originRestrictionType: NotRequired[PackageGroupOriginRestrictionTypeType],  # (1)
```

1. See [:material-code-brackets: PackageGroupOriginRestrictionTypeType](./literals.md#packagegrouporiginrestrictiontypetype) 
## PackageGroupReferenceTypeDef

```python
# PackageGroupReferenceTypeDef definition

class PackageGroupReferenceTypeDef(TypedDict):
    arn: NotRequired[str],
    pattern: NotRequired[str],
```

## PackageOriginRestrictionsTypeDef

```python
# PackageOriginRestrictionsTypeDef definition

class PackageOriginRestrictionsTypeDef(TypedDict):
    publish: AllowPublishType,  # (1)
    upstream: AllowUpstreamType,  # (2)
```

1. See [:material-code-brackets: AllowPublishType](./literals.md#allowpublishtype) 
2. See [:material-code-brackets: AllowUpstreamType](./literals.md#allowupstreamtype) 
## PutDomainPermissionsPolicyRequestRequestTypeDef

```python
# PutDomainPermissionsPolicyRequestRequestTypeDef definition

class PutDomainPermissionsPolicyRequestRequestTypeDef(TypedDict):
    domain: str,
    policyDocument: str,
    domainOwner: NotRequired[str],
    policyRevision: NotRequired[str],
```

## PutRepositoryPermissionsPolicyRequestRequestTypeDef

```python
# PutRepositoryPermissionsPolicyRequestRequestTypeDef definition

class PutRepositoryPermissionsPolicyRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    policyDocument: str,
    domainOwner: NotRequired[str],
    policyRevision: NotRequired[str],
```

## RepositoryExternalConnectionInfoTypeDef

```python
# RepositoryExternalConnectionInfoTypeDef definition

class RepositoryExternalConnectionInfoTypeDef(TypedDict):
    externalConnectionName: NotRequired[str],
    packageFormat: NotRequired[PackageFormatType],  # (1)
    status: NotRequired[ExternalConnectionStatusType],  # (2)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: ExternalConnectionStatusType](./literals.md#externalconnectionstatustype) 
## UpstreamRepositoryInfoTypeDef

```python
# UpstreamRepositoryInfoTypeDef definition

class UpstreamRepositoryInfoTypeDef(TypedDict):
    repositoryName: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdatePackageGroupRequestRequestTypeDef

```python
# UpdatePackageGroupRequestRequestTypeDef definition

class UpdatePackageGroupRequestRequestTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    domainOwner: NotRequired[str],
    contactInfo: NotRequired[str],
    description: NotRequired[str],
```

## UpdatePackageVersionsStatusRequestRequestTypeDef

```python
# UpdatePackageVersionsStatusRequestRequestTypeDef definition

class UpdatePackageVersionsStatusRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    versions: Sequence[str],
    targetStatus: PackageVersionStatusType,  # (2)
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    versionRevisions: NotRequired[Mapping[str, str]],
    expectedStatus: NotRequired[PackageVersionStatusType],  # (2)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
3. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
## GetAuthorizationTokenResultTypeDef

```python
# GetAuthorizationTokenResultTypeDef definition

class GetAuthorizationTokenResultTypeDef(TypedDict):
    authorizationToken: str,
    expiration: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPackageVersionAssetResultTypeDef

```python
# GetPackageVersionAssetResultTypeDef definition

class GetPackageVersionAssetResultTypeDef(TypedDict):
    asset: StreamingBody,
    assetName: str,
    packageVersion: str,
    packageVersionRevision: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPackageVersionReadmeResultTypeDef

```python
# GetPackageVersionReadmeResultTypeDef definition

class GetPackageVersionReadmeResultTypeDef(TypedDict):
    format: PackageFormatType,  # (1)
    namespace: str,
    package: str,
    version: str,
    versionRevision: str,
    readme: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRepositoryEndpointResultTypeDef

```python
# GetRepositoryEndpointResultTypeDef definition

class GetRepositoryEndpointResultTypeDef(TypedDict):
    repositoryEndpoint: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAllowedRepositoriesForGroupResultTypeDef

```python
# ListAllowedRepositoriesForGroupResultTypeDef definition

class ListAllowedRepositoriesForGroupResultTypeDef(TypedDict):
    allowedRepositories: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPackageVersionAssetsResultTypeDef

```python
# ListPackageVersionAssetsResultTypeDef definition

class ListPackageVersionAssetsResultTypeDef(TypedDict):
    format: PackageFormatType,  # (1)
    namespace: str,
    package: str,
    version: str,
    versionRevision: str,
    assets: List[AssetSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-braces: AssetSummaryTypeDef](./type_defs.md#assetsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishPackageVersionResultTypeDef

```python
# PublishPackageVersionResultTypeDef definition

class PublishPackageVersionResultTypeDef(TypedDict):
    format: PackageFormatType,  # (1)
    namespace: str,
    package: str,
    version: str,
    versionRevision: str,
    status: PackageVersionStatusType,  # (2)
    asset: AssetSummaryTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
3. See [:material-code-braces: AssetSummaryTypeDef](./type_defs.md#assetsummarytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssociatedPackagesResultTypeDef

```python
# ListAssociatedPackagesResultTypeDef definition

class ListAssociatedPackagesResultTypeDef(TypedDict):
    packages: List[AssociatedPackageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociatedPackageTypeDef](./type_defs.md#associatedpackagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishPackageVersionRequestRequestTypeDef

```python
# PublishPackageVersionRequestRequestTypeDef definition

class PublishPackageVersionRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    packageVersion: str,
    assetContent: BlobTypeDef,
    assetName: str,
    assetSHA256: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    unfinished: NotRequired[bool],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
## CopyPackageVersionsResultTypeDef

```python
# CopyPackageVersionsResultTypeDef definition

class CopyPackageVersionsResultTypeDef(TypedDict):
    successfulVersions: Dict[str, SuccessfulPackageVersionInfoTypeDef],  # (1)
    failedVersions: Dict[str, PackageVersionErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulPackageVersionInfoTypeDef](./type_defs.md#successfulpackageversioninfotypedef) 
2. See [:material-code-braces: PackageVersionErrorTypeDef](./type_defs.md#packageversionerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePackageVersionsResultTypeDef

```python
# DeletePackageVersionsResultTypeDef definition

class DeletePackageVersionsResultTypeDef(TypedDict):
    successfulVersions: Dict[str, SuccessfulPackageVersionInfoTypeDef],  # (1)
    failedVersions: Dict[str, PackageVersionErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulPackageVersionInfoTypeDef](./type_defs.md#successfulpackageversioninfotypedef) 
2. See [:material-code-braces: PackageVersionErrorTypeDef](./type_defs.md#packageversionerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisposePackageVersionsResultTypeDef

```python
# DisposePackageVersionsResultTypeDef definition

class DisposePackageVersionsResultTypeDef(TypedDict):
    successfulVersions: Dict[str, SuccessfulPackageVersionInfoTypeDef],  # (1)
    failedVersions: Dict[str, PackageVersionErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulPackageVersionInfoTypeDef](./type_defs.md#successfulpackageversioninfotypedef) 
2. See [:material-code-braces: PackageVersionErrorTypeDef](./type_defs.md#packageversionerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePackageVersionsStatusResultTypeDef

```python
# UpdatePackageVersionsStatusResultTypeDef definition

class UpdatePackageVersionsStatusResultTypeDef(TypedDict):
    successfulVersions: Dict[str, SuccessfulPackageVersionInfoTypeDef],  # (1)
    failedVersions: Dict[str, PackageVersionErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulPackageVersionInfoTypeDef](./type_defs.md#successfulpackageversioninfotypedef) 
2. See [:material-code-braces: PackageVersionErrorTypeDef](./type_defs.md#packageversionerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDomainRequestRequestTypeDef

```python
# CreateDomainRequestRequestTypeDef definition

class CreateDomainRequestRequestTypeDef(TypedDict):
    domain: str,
    encryptionKey: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePackageGroupRequestRequestTypeDef

```python
# CreatePackageGroupRequestRequestTypeDef definition

class CreatePackageGroupRequestRequestTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    domainOwner: NotRequired[str],
    contactInfo: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
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
## CreateDomainResultTypeDef

```python
# CreateDomainResultTypeDef definition

class CreateDomainResultTypeDef(TypedDict):
    domain: DomainDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainDescriptionTypeDef](./type_defs.md#domaindescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDomainResultTypeDef

```python
# DeleteDomainResultTypeDef definition

class DeleteDomainResultTypeDef(TypedDict):
    domain: DomainDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainDescriptionTypeDef](./type_defs.md#domaindescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDomainResultTypeDef

```python
# DescribeDomainResultTypeDef definition

class DescribeDomainResultTypeDef(TypedDict):
    domain: DomainDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainDescriptionTypeDef](./type_defs.md#domaindescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRepositoryRequestRequestTypeDef

```python
# CreateRepositoryRequestRequestTypeDef definition

class CreateRepositoryRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    domainOwner: NotRequired[str],
    description: NotRequired[str],
    upstreams: NotRequired[Sequence[UpstreamRepositoryTypeDef]],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: UpstreamRepositoryTypeDef](./type_defs.md#upstreamrepositorytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateRepositoryRequestRequestTypeDef

```python
# UpdateRepositoryRequestRequestTypeDef definition

class UpdateRepositoryRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    domainOwner: NotRequired[str],
    description: NotRequired[str],
    upstreams: NotRequired[Sequence[UpstreamRepositoryTypeDef]],  # (1)
```

1. See [:material-code-braces: UpstreamRepositoryTypeDef](./type_defs.md#upstreamrepositorytypedef) 
## DeleteDomainPermissionsPolicyResultTypeDef

```python
# DeleteDomainPermissionsPolicyResultTypeDef definition

class DeleteDomainPermissionsPolicyResultTypeDef(TypedDict):
    policy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRepositoryPermissionsPolicyResultTypeDef

```python
# DeleteRepositoryPermissionsPolicyResultTypeDef definition

class DeleteRepositoryPermissionsPolicyResultTypeDef(TypedDict):
    policy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDomainPermissionsPolicyResultTypeDef

```python
# GetDomainPermissionsPolicyResultTypeDef definition

class GetDomainPermissionsPolicyResultTypeDef(TypedDict):
    policy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRepositoryPermissionsPolicyResultTypeDef

```python
# GetRepositoryPermissionsPolicyResultTypeDef definition

class GetRepositoryPermissionsPolicyResultTypeDef(TypedDict):
    policy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDomainPermissionsPolicyResultTypeDef

```python
# PutDomainPermissionsPolicyResultTypeDef definition

class PutDomainPermissionsPolicyResultTypeDef(TypedDict):
    policy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRepositoryPermissionsPolicyResultTypeDef

```python
# PutRepositoryPermissionsPolicyResultTypeDef definition

class PutRepositoryPermissionsPolicyResultTypeDef(TypedDict):
    policy: ResourcePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PackageVersionOriginTypeDef

```python
# PackageVersionOriginTypeDef definition

class PackageVersionOriginTypeDef(TypedDict):
    domainEntryPoint: NotRequired[DomainEntryPointTypeDef],  # (1)
    originType: NotRequired[PackageVersionOriginTypeType],  # (2)
```

1. See [:material-code-braces: DomainEntryPointTypeDef](./type_defs.md#domainentrypointtypedef) 
2. See [:material-code-brackets: PackageVersionOriginTypeType](./literals.md#packageversionorigintypetype) 
## ListDomainsResultTypeDef

```python
# ListDomainsResultTypeDef definition

class ListDomainsResultTypeDef(TypedDict):
    domains: List[DomainSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAllowedRepositoriesForGroupRequestListAllowedRepositoriesForGroupPaginateTypeDef

```python
# ListAllowedRepositoriesForGroupRequestListAllowedRepositoriesForGroupPaginateTypeDef definition

class ListAllowedRepositoriesForGroupRequestListAllowedRepositoriesForGroupPaginateTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    originRestrictionType: PackageGroupOriginRestrictionTypeType,  # (1)
    domainOwner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PackageGroupOriginRestrictionTypeType](./literals.md#packagegrouporiginrestrictiontypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociatedPackagesRequestListAssociatedPackagesPaginateTypeDef

```python
# ListAssociatedPackagesRequestListAssociatedPackagesPaginateTypeDef definition

class ListAssociatedPackagesRequestListAssociatedPackagesPaginateTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    domainOwner: NotRequired[str],
    preview: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainsRequestListDomainsPaginateTypeDef

```python
# ListDomainsRequestListDomainsPaginateTypeDef definition

class ListDomainsRequestListDomainsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPackageGroupsRequestListPackageGroupsPaginateTypeDef

```python
# ListPackageGroupsRequestListPackageGroupsPaginateTypeDef definition

class ListPackageGroupsRequestListPackageGroupsPaginateTypeDef(TypedDict):
    domain: str,
    domainOwner: NotRequired[str],
    prefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef

```python
# ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef definition

class ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    packageVersion: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPackageVersionsRequestListPackageVersionsPaginateTypeDef

```python
# ListPackageVersionsRequestListPackageVersionsPaginateTypeDef definition

class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
    status: NotRequired[PackageVersionStatusType],  # (2)
    sortBy: NotRequired[PackageVersionSortTypeType],  # (3)
    originType: NotRequired[PackageVersionOriginTypeType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
3. See [:material-code-brackets: PackageVersionSortTypeType](./literals.md#packageversionsorttypetype) 
4. See [:material-code-brackets: PackageVersionOriginTypeType](./literals.md#packageversionorigintypetype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPackagesRequestListPackagesPaginateTypeDef

```python
# ListPackagesRequestListPackagesPaginateTypeDef definition

class ListPackagesRequestListPackagesPaginateTypeDef(TypedDict):
    domain: str,
    repository: str,
    domainOwner: NotRequired[str],
    format: NotRequired[PackageFormatType],  # (1)
    namespace: NotRequired[str],
    packagePrefix: NotRequired[str],
    publish: NotRequired[AllowPublishType],  # (2)
    upstream: NotRequired[AllowUpstreamType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: AllowPublishType](./literals.md#allowpublishtype) 
3. See [:material-code-brackets: AllowUpstreamType](./literals.md#allowupstreamtype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef

```python
# ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef definition

class ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef(TypedDict):
    domain: str,
    domainOwner: NotRequired[str],
    administratorAccount: NotRequired[str],
    repositoryPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRepositoriesRequestListRepositoriesPaginateTypeDef

```python
# ListRepositoriesRequestListRepositoriesPaginateTypeDef definition

class ListRepositoriesRequestListRepositoriesPaginateTypeDef(TypedDict):
    repositoryPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubPackageGroupsRequestListSubPackageGroupsPaginateTypeDef

```python
# ListSubPackageGroupsRequestListSubPackageGroupsPaginateTypeDef definition

class ListSubPackageGroupsRequestListSubPackageGroupsPaginateTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    domainOwner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPackageVersionDependenciesResultTypeDef

```python
# ListPackageVersionDependenciesResultTypeDef definition

class ListPackageVersionDependenciesResultTypeDef(TypedDict):
    format: PackageFormatType,  # (1)
    namespace: str,
    package: str,
    version: str,
    versionRevision: str,
    dependencies: List[PackageDependencyTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-braces: PackageDependencyTypeDef](./type_defs.md#packagedependencytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRepositoriesInDomainResultTypeDef

```python
# ListRepositoriesInDomainResultTypeDef definition

class ListRepositoriesInDomainResultTypeDef(TypedDict):
    repositories: List[RepositorySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RepositorySummaryTypeDef](./type_defs.md#repositorysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRepositoriesResultTypeDef

```python
# ListRepositoriesResultTypeDef definition

class ListRepositoriesResultTypeDef(TypedDict):
    repositories: List[RepositorySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RepositorySummaryTypeDef](./type_defs.md#repositorysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePackageGroupOriginConfigurationRequestRequestTypeDef

```python
# UpdatePackageGroupOriginConfigurationRequestRequestTypeDef definition

class UpdatePackageGroupOriginConfigurationRequestRequestTypeDef(TypedDict):
    domain: str,
    packageGroup: str,
    domainOwner: NotRequired[str],
    restrictions: NotRequired[Mapping[PackageGroupOriginRestrictionTypeType, PackageGroupOriginRestrictionModeType]],  # (1)
    addAllowedRepositories: NotRequired[Sequence[PackageGroupAllowedRepositoryTypeDef]],  # (2)
    removeAllowedRepositories: NotRequired[Sequence[PackageGroupAllowedRepositoryTypeDef]],  # (2)
```

1. See [:material-code-brackets: PackageGroupOriginRestrictionTypeType](./literals.md#packagegrouporiginrestrictiontypetype) [:material-code-brackets: PackageGroupOriginRestrictionModeType](./literals.md#packagegrouporiginrestrictionmodetype) 
2. See [:material-code-braces: PackageGroupAllowedRepositoryTypeDef](./type_defs.md#packagegroupallowedrepositorytypedef) 
3. See [:material-code-braces: PackageGroupAllowedRepositoryTypeDef](./type_defs.md#packagegroupallowedrepositorytypedef) 
## PackageGroupOriginRestrictionTypeDef

```python
# PackageGroupOriginRestrictionTypeDef definition

class PackageGroupOriginRestrictionTypeDef(TypedDict):
    mode: NotRequired[PackageGroupOriginRestrictionModeType],  # (1)
    effectiveMode: NotRequired[PackageGroupOriginRestrictionModeType],  # (1)
    inheritedFrom: NotRequired[PackageGroupReferenceTypeDef],  # (3)
    repositoriesCount: NotRequired[int],
```

1. See [:material-code-brackets: PackageGroupOriginRestrictionModeType](./literals.md#packagegrouporiginrestrictionmodetype) 
2. See [:material-code-brackets: PackageGroupOriginRestrictionModeType](./literals.md#packagegrouporiginrestrictionmodetype) 
3. See [:material-code-braces: PackageGroupReferenceTypeDef](./type_defs.md#packagegroupreferencetypedef) 
## PackageOriginConfigurationTypeDef

```python
# PackageOriginConfigurationTypeDef definition

class PackageOriginConfigurationTypeDef(TypedDict):
    restrictions: NotRequired[PackageOriginRestrictionsTypeDef],  # (1)
```

1. See [:material-code-braces: PackageOriginRestrictionsTypeDef](./type_defs.md#packageoriginrestrictionstypedef) 
## PutPackageOriginConfigurationRequestRequestTypeDef

```python
# PutPackageOriginConfigurationRequestRequestTypeDef definition

class PutPackageOriginConfigurationRequestRequestTypeDef(TypedDict):
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    restrictions: PackageOriginRestrictionsTypeDef,  # (2)
    domainOwner: NotRequired[str],
    namespace: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-braces: PackageOriginRestrictionsTypeDef](./type_defs.md#packageoriginrestrictionstypedef) 
## RepositoryDescriptionTypeDef

```python
# RepositoryDescriptionTypeDef definition

class RepositoryDescriptionTypeDef(TypedDict):
    name: NotRequired[str],
    administratorAccount: NotRequired[str],
    domainName: NotRequired[str],
    domainOwner: NotRequired[str],
    arn: NotRequired[str],
    description: NotRequired[str],
    upstreams: NotRequired[List[UpstreamRepositoryInfoTypeDef]],  # (1)
    externalConnections: NotRequired[List[RepositoryExternalConnectionInfoTypeDef]],  # (2)
    createdTime: NotRequired[datetime],
```

1. See [:material-code-braces: UpstreamRepositoryInfoTypeDef](./type_defs.md#upstreamrepositoryinfotypedef) 
2. See [:material-code-braces: RepositoryExternalConnectionInfoTypeDef](./type_defs.md#repositoryexternalconnectioninfotypedef) 
## PackageVersionDescriptionTypeDef

```python
# PackageVersionDescriptionTypeDef definition

class PackageVersionDescriptionTypeDef(TypedDict):
    format: NotRequired[PackageFormatType],  # (1)
    namespace: NotRequired[str],
    packageName: NotRequired[str],
    displayName: NotRequired[str],
    version: NotRequired[str],
    summary: NotRequired[str],
    homePage: NotRequired[str],
    sourceCodeRepository: NotRequired[str],
    publishedTime: NotRequired[datetime],
    licenses: NotRequired[List[LicenseInfoTypeDef]],  # (2)
    revision: NotRequired[str],
    status: NotRequired[PackageVersionStatusType],  # (3)
    origin: NotRequired[PackageVersionOriginTypeDef],  # (4)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-braces: LicenseInfoTypeDef](./type_defs.md#licenseinfotypedef) 
3. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
4. See [:material-code-braces: PackageVersionOriginTypeDef](./type_defs.md#packageversionorigintypedef) 
## PackageVersionSummaryTypeDef

```python
# PackageVersionSummaryTypeDef definition

class PackageVersionSummaryTypeDef(TypedDict):
    version: str,
    status: PackageVersionStatusType,  # (1)
    revision: NotRequired[str],
    origin: NotRequired[PackageVersionOriginTypeDef],  # (2)
```

1. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
2. See [:material-code-braces: PackageVersionOriginTypeDef](./type_defs.md#packageversionorigintypedef) 
## PackageGroupOriginConfigurationTypeDef

```python
# PackageGroupOriginConfigurationTypeDef definition

class PackageGroupOriginConfigurationTypeDef(TypedDict):
    restrictions: NotRequired[Dict[PackageGroupOriginRestrictionTypeType, PackageGroupOriginRestrictionTypeDef]],  # (1)
```

1. See [:material-code-brackets: PackageGroupOriginRestrictionTypeType](./literals.md#packagegrouporiginrestrictiontypetype) [:material-code-braces: PackageGroupOriginRestrictionTypeDef](./type_defs.md#packagegrouporiginrestrictiontypedef) 
## PackageDescriptionTypeDef

```python
# PackageDescriptionTypeDef definition

class PackageDescriptionTypeDef(TypedDict):
    format: NotRequired[PackageFormatType],  # (1)
    namespace: NotRequired[str],
    name: NotRequired[str],
    originConfiguration: NotRequired[PackageOriginConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-braces: PackageOriginConfigurationTypeDef](./type_defs.md#packageoriginconfigurationtypedef) 
## PackageSummaryTypeDef

```python
# PackageSummaryTypeDef definition

class PackageSummaryTypeDef(TypedDict):
    format: NotRequired[PackageFormatType],  # (1)
    namespace: NotRequired[str],
    package: NotRequired[str],
    originConfiguration: NotRequired[PackageOriginConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-braces: PackageOriginConfigurationTypeDef](./type_defs.md#packageoriginconfigurationtypedef) 
## PutPackageOriginConfigurationResultTypeDef

```python
# PutPackageOriginConfigurationResultTypeDef definition

class PutPackageOriginConfigurationResultTypeDef(TypedDict):
    originConfiguration: PackageOriginConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageOriginConfigurationTypeDef](./type_defs.md#packageoriginconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateExternalConnectionResultTypeDef

```python
# AssociateExternalConnectionResultTypeDef definition

class AssociateExternalConnectionResultTypeDef(TypedDict):
    repository: RepositoryDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryDescriptionTypeDef](./type_defs.md#repositorydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRepositoryResultTypeDef

```python
# CreateRepositoryResultTypeDef definition

class CreateRepositoryResultTypeDef(TypedDict):
    repository: RepositoryDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryDescriptionTypeDef](./type_defs.md#repositorydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRepositoryResultTypeDef

```python
# DeleteRepositoryResultTypeDef definition

class DeleteRepositoryResultTypeDef(TypedDict):
    repository: RepositoryDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryDescriptionTypeDef](./type_defs.md#repositorydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRepositoryResultTypeDef

```python
# DescribeRepositoryResultTypeDef definition

class DescribeRepositoryResultTypeDef(TypedDict):
    repository: RepositoryDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryDescriptionTypeDef](./type_defs.md#repositorydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateExternalConnectionResultTypeDef

```python
# DisassociateExternalConnectionResultTypeDef definition

class DisassociateExternalConnectionResultTypeDef(TypedDict):
    repository: RepositoryDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryDescriptionTypeDef](./type_defs.md#repositorydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRepositoryResultTypeDef

```python
# UpdateRepositoryResultTypeDef definition

class UpdateRepositoryResultTypeDef(TypedDict):
    repository: RepositoryDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryDescriptionTypeDef](./type_defs.md#repositorydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePackageVersionResultTypeDef

```python
# DescribePackageVersionResultTypeDef definition

class DescribePackageVersionResultTypeDef(TypedDict):
    packageVersion: PackageVersionDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageVersionDescriptionTypeDef](./type_defs.md#packageversiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPackageVersionsResultTypeDef

```python
# ListPackageVersionsResultTypeDef definition

class ListPackageVersionsResultTypeDef(TypedDict):
    defaultDisplayVersion: str,
    format: PackageFormatType,  # (1)
    namespace: str,
    package: str,
    versions: List[PackageVersionSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-braces: PackageVersionSummaryTypeDef](./type_defs.md#packageversionsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PackageGroupDescriptionTypeDef

```python
# PackageGroupDescriptionTypeDef definition

class PackageGroupDescriptionTypeDef(TypedDict):
    arn: NotRequired[str],
    pattern: NotRequired[str],
    domainName: NotRequired[str],
    domainOwner: NotRequired[str],
    createdTime: NotRequired[datetime],
    contactInfo: NotRequired[str],
    description: NotRequired[str],
    originConfiguration: NotRequired[PackageGroupOriginConfigurationTypeDef],  # (1)
    parent: NotRequired[PackageGroupReferenceTypeDef],  # (2)
```

1. See [:material-code-braces: PackageGroupOriginConfigurationTypeDef](./type_defs.md#packagegrouporiginconfigurationtypedef) 
2. See [:material-code-braces: PackageGroupReferenceTypeDef](./type_defs.md#packagegroupreferencetypedef) 
## PackageGroupSummaryTypeDef

```python
# PackageGroupSummaryTypeDef definition

class PackageGroupSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    pattern: NotRequired[str],
    domainName: NotRequired[str],
    domainOwner: NotRequired[str],
    createdTime: NotRequired[datetime],
    contactInfo: NotRequired[str],
    description: NotRequired[str],
    originConfiguration: NotRequired[PackageGroupOriginConfigurationTypeDef],  # (1)
    parent: NotRequired[PackageGroupReferenceTypeDef],  # (2)
```

1. See [:material-code-braces: PackageGroupOriginConfigurationTypeDef](./type_defs.md#packagegrouporiginconfigurationtypedef) 
2. See [:material-code-braces: PackageGroupReferenceTypeDef](./type_defs.md#packagegroupreferencetypedef) 
## DescribePackageResultTypeDef

```python
# DescribePackageResultTypeDef definition

class DescribePackageResultTypeDef(TypedDict):
    package: PackageDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageDescriptionTypeDef](./type_defs.md#packagedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePackageResultTypeDef

```python
# DeletePackageResultTypeDef definition

class DeletePackageResultTypeDef(TypedDict):
    deletedPackage: PackageSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageSummaryTypeDef](./type_defs.md#packagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPackagesResultTypeDef

```python
# ListPackagesResultTypeDef definition

class ListPackagesResultTypeDef(TypedDict):
    packages: List[PackageSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PackageSummaryTypeDef](./type_defs.md#packagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePackageGroupResultTypeDef

```python
# CreatePackageGroupResultTypeDef definition

class CreatePackageGroupResultTypeDef(TypedDict):
    packageGroup: PackageGroupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageGroupDescriptionTypeDef](./type_defs.md#packagegroupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePackageGroupResultTypeDef

```python
# DeletePackageGroupResultTypeDef definition

class DeletePackageGroupResultTypeDef(TypedDict):
    packageGroup: PackageGroupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageGroupDescriptionTypeDef](./type_defs.md#packagegroupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePackageGroupResultTypeDef

```python
# DescribePackageGroupResultTypeDef definition

class DescribePackageGroupResultTypeDef(TypedDict):
    packageGroup: PackageGroupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageGroupDescriptionTypeDef](./type_defs.md#packagegroupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssociatedPackageGroupResultTypeDef

```python
# GetAssociatedPackageGroupResultTypeDef definition

class GetAssociatedPackageGroupResultTypeDef(TypedDict):
    packageGroup: PackageGroupDescriptionTypeDef,  # (1)
    associationType: PackageGroupAssociationTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PackageGroupDescriptionTypeDef](./type_defs.md#packagegroupdescriptiontypedef) 
2. See [:material-code-brackets: PackageGroupAssociationTypeType](./literals.md#packagegroupassociationtypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePackageGroupOriginConfigurationResultTypeDef

```python
# UpdatePackageGroupOriginConfigurationResultTypeDef definition

class UpdatePackageGroupOriginConfigurationResultTypeDef(TypedDict):
    packageGroup: PackageGroupDescriptionTypeDef,  # (1)
    allowedRepositoryUpdates: Dict[PackageGroupOriginRestrictionTypeType, Dict[PackageGroupAllowedRepositoryUpdateTypeType, List[str]]],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PackageGroupDescriptionTypeDef](./type_defs.md#packagegroupdescriptiontypedef) 
2. See [:material-code-brackets: PackageGroupOriginRestrictionTypeType](./literals.md#packagegrouporiginrestrictiontypetype) [:material-code-brackets: PackageGroupAllowedRepositoryUpdateTypeType](./literals.md#packagegroupallowedrepositoryupdatetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePackageGroupResultTypeDef

```python
# UpdatePackageGroupResultTypeDef definition

class UpdatePackageGroupResultTypeDef(TypedDict):
    packageGroup: PackageGroupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PackageGroupDescriptionTypeDef](./type_defs.md#packagegroupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPackageGroupsResultTypeDef

```python
# ListPackageGroupsResultTypeDef definition

class ListPackageGroupsResultTypeDef(TypedDict):
    packageGroups: List[PackageGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PackageGroupSummaryTypeDef](./type_defs.md#packagegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubPackageGroupsResultTypeDef

```python
# ListSubPackageGroupsResultTypeDef definition

class ListSubPackageGroupsResultTypeDef(TypedDict):
    packageGroups: List[PackageGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PackageGroupSummaryTypeDef](./type_defs.md#packagegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
