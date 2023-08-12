# Type definitions

> [Index](../README.md) > [ECRPublic](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ECRPublic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic)
    type annotations stubs module [types-aiobotocore-ecr-public](https://pypi.org/project/types-aiobotocore-ecr-public/).

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




## AuthorizationDataTypeDef

```python
# AuthorizationDataTypeDef definition

class AuthorizationDataTypeDef(TypedDict):
    authorizationToken: NotRequired[str],
    expiresAt: NotRequired[datetime],
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
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## ImageIdentifierTypeDef

```python
# ImageIdentifierTypeDef definition

class ImageIdentifierTypeDef(TypedDict):
    imageDigest: NotRequired[str],
    imageTag: NotRequired[str],
```

## CompleteLayerUploadRequestRequestTypeDef

```python
# CompleteLayerUploadRequestRequestTypeDef definition

class CompleteLayerUploadRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    uploadId: str,
    layerDigests: Sequence[str],
    registryId: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## RepositoryCatalogDataTypeDef

```python
# RepositoryCatalogDataTypeDef definition

class RepositoryCatalogDataTypeDef(TypedDict):
    description: NotRequired[str],
    architectures: NotRequired[List[str]],
    operatingSystems: NotRequired[List[str]],
    logoUrl: NotRequired[str],
    aboutText: NotRequired[str],
    usageText: NotRequired[str],
    marketplaceCertified: NotRequired[bool],
```

## RepositoryTypeDef

```python
# RepositoryTypeDef definition

class RepositoryTypeDef(TypedDict):
    repositoryArn: NotRequired[str],
    registryId: NotRequired[str],
    repositoryName: NotRequired[str],
    repositoryUri: NotRequired[str],
    createdAt: NotRequired[datetime],
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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeImageTagsRequestRequestTypeDef

```python
# DescribeImageTagsRequestRequestTypeDef definition

class DescribeImageTagsRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

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
    imageManifestMediaType: NotRequired[str],
    artifactMediaType: NotRequired[str],
```

## DescribeRegistriesRequestRequestTypeDef

```python
# DescribeRegistriesRequestRequestTypeDef definition

class DescribeRegistriesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## DescribeRepositoriesRequestRequestTypeDef

```python
# DescribeRepositoriesRequestRequestTypeDef definition

class DescribeRepositoriesRequestRequestTypeDef(TypedDict):
    registryId: NotRequired[str],
    repositoryNames: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RegistryCatalogDataTypeDef

```python
# RegistryCatalogDataTypeDef definition

class RegistryCatalogDataTypeDef(TypedDict):
    displayName: NotRequired[str],
```

## GetRepositoryCatalogDataRequestRequestTypeDef

```python
# GetRepositoryCatalogDataRequestRequestTypeDef definition

class GetRepositoryCatalogDataRequestRequestTypeDef(TypedDict):
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

## ReferencedImageDetailTypeDef

```python
# ReferencedImageDetailTypeDef definition

class ReferencedImageDetailTypeDef(TypedDict):
    imageDigest: NotRequired[str],
    imageSizeInBytes: NotRequired[int],
    imagePushedAt: NotRequired[datetime],
    imageManifestMediaType: NotRequired[str],
    artifactMediaType: NotRequired[str],
```

## InitiateLayerUploadRequestRequestTypeDef

```python
# InitiateLayerUploadRequestRequestTypeDef definition

class InitiateLayerUploadRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
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

## PutRegistryCatalogDataRequestRequestTypeDef

```python
# PutRegistryCatalogDataRequestRequestTypeDef definition

class PutRegistryCatalogDataRequestRequestTypeDef(TypedDict):
    displayName: NotRequired[str],
```

## RegistryAliasTypeDef

```python
# RegistryAliasTypeDef definition

class RegistryAliasTypeDef(TypedDict):
    name: str,
    status: RegistryAliasStatusType,  # (1)
    primaryRegistryAlias: bool,
    defaultRegistryAlias: bool,
```

1. See [:material-code-brackets: RegistryAliasStatusType](./literals.md#registryaliasstatustype) 
## SetRepositoryPolicyRequestRequestTypeDef

```python
# SetRepositoryPolicyRequestRequestTypeDef definition

class SetRepositoryPolicyRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    policyText: str,
    registryId: NotRequired[str],
    force: NotRequired[bool],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

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
## GetAuthorizationTokenResponseTypeDef

```python
# GetAuthorizationTokenResponseTypeDef definition

class GetAuthorizationTokenResponseTypeDef(TypedDict):
    authorizationData: AuthorizationDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthorizationDataTypeDef](./type_defs.md#authorizationdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## BatchDeleteImageRequestRequestTypeDef

```python
# BatchDeleteImageRequestRequestTypeDef definition

class BatchDeleteImageRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    imageIds: Sequence[ImageIdentifierTypeDef],  # (1)
    registryId: NotRequired[str],
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
## DescribeImagesRequestRequestTypeDef

```python
# DescribeImagesRequestRequestTypeDef definition

class DescribeImagesRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    imageIds: NotRequired[Sequence[ImageIdentifierTypeDef]],  # (1)
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
## RepositoryCatalogDataInputTypeDef

```python
# RepositoryCatalogDataInputTypeDef definition

class RepositoryCatalogDataInputTypeDef(TypedDict):
    description: NotRequired[str],
    architectures: NotRequired[Sequence[str]],
    operatingSystems: NotRequired[Sequence[str]],
    logoImageBlob: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    aboutText: NotRequired[str],
    usageText: NotRequired[str],
```

## UploadLayerPartRequestRequestTypeDef

```python
# UploadLayerPartRequestRequestTypeDef definition

class UploadLayerPartRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    uploadId: str,
    partFirstByte: int,
    partLastByte: int,
    layerPartBlob: Union[str, bytes, IO[Any], StreamingBody],
    registryId: NotRequired[str],
```

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
## GetRepositoryCatalogDataResponseTypeDef

```python
# GetRepositoryCatalogDataResponseTypeDef definition

class GetRepositoryCatalogDataResponseTypeDef(TypedDict):
    catalogData: RepositoryCatalogDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryCatalogDataTypeDef](./type_defs.md#repositorycatalogdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRepositoryCatalogDataResponseTypeDef

```python
# PutRepositoryCatalogDataResponseTypeDef definition

class PutRepositoryCatalogDataResponseTypeDef(TypedDict):
    catalogData: RepositoryCatalogDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryCatalogDataTypeDef](./type_defs.md#repositorycatalogdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRepositoryResponseTypeDef

```python
# CreateRepositoryResponseTypeDef definition

class CreateRepositoryResponseTypeDef(TypedDict):
    repository: RepositoryTypeDef,  # (1)
    catalogData: RepositoryCatalogDataTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RepositoryTypeDef](./type_defs.md#repositorytypedef) 
2. See [:material-code-braces: RepositoryCatalogDataTypeDef](./type_defs.md#repositorycatalogdatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryTypeDef](./type_defs.md#repositorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef

```python
# DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef definition

class DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeImagesRequestDescribeImagesPaginateTypeDef

```python
# DescribeImagesRequestDescribeImagesPaginateTypeDef definition

class DescribeImagesRequestDescribeImagesPaginateTypeDef(TypedDict):
    repositoryName: str,
    registryId: NotRequired[str],
    imageIds: NotRequired[Sequence[ImageIdentifierTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef

```python
# DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef definition

class DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef

```python
# DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef definition

class DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef(TypedDict):
    registryId: NotRequired[str],
    repositoryNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeImagesResponseTypeDef

```python
# DescribeImagesResponseTypeDef definition

class DescribeImagesResponseTypeDef(TypedDict):
    imageDetails: List[ImageDetailTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageDetailTypeDef](./type_defs.md#imagedetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRegistryCatalogDataResponseTypeDef

```python
# GetRegistryCatalogDataResponseTypeDef definition

class GetRegistryCatalogDataResponseTypeDef(TypedDict):
    registryCatalogData: RegistryCatalogDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegistryCatalogDataTypeDef](./type_defs.md#registrycatalogdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRegistryCatalogDataResponseTypeDef

```python
# PutRegistryCatalogDataResponseTypeDef definition

class PutRegistryCatalogDataResponseTypeDef(TypedDict):
    registryCatalogData: RegistryCatalogDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegistryCatalogDataTypeDef](./type_defs.md#registrycatalogdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImageTagDetailTypeDef

```python
# ImageTagDetailTypeDef definition

class ImageTagDetailTypeDef(TypedDict):
    imageTag: NotRequired[str],
    createdAt: NotRequired[datetime],
    imageDetail: NotRequired[ReferencedImageDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ReferencedImageDetailTypeDef](./type_defs.md#referencedimagedetailtypedef) 
## RegistryTypeDef

```python
# RegistryTypeDef definition

class RegistryTypeDef(TypedDict):
    registryId: str,
    registryArn: str,
    registryUri: str,
    verified: bool,
    aliases: List[RegistryAliasTypeDef],  # (1)
```

1. See [:material-code-braces: RegistryAliasTypeDef](./type_defs.md#registryaliastypedef) 
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
## PutImageResponseTypeDef

```python
# PutImageResponseTypeDef definition

class PutImageResponseTypeDef(TypedDict):
    image: ImageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRepositoryRequestRequestTypeDef

```python
# CreateRepositoryRequestRequestTypeDef definition

class CreateRepositoryRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    catalogData: NotRequired[RepositoryCatalogDataInputTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: RepositoryCatalogDataInputTypeDef](./type_defs.md#repositorycatalogdatainputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutRepositoryCatalogDataRequestRequestTypeDef

```python
# PutRepositoryCatalogDataRequestRequestTypeDef definition

class PutRepositoryCatalogDataRequestRequestTypeDef(TypedDict):
    repositoryName: str,
    catalogData: RepositoryCatalogDataInputTypeDef,  # (1)
    registryId: NotRequired[str],
```

1. See [:material-code-braces: RepositoryCatalogDataInputTypeDef](./type_defs.md#repositorycatalogdatainputtypedef) 
## DescribeImageTagsResponseTypeDef

```python
# DescribeImageTagsResponseTypeDef definition

class DescribeImageTagsResponseTypeDef(TypedDict):
    imageTagDetails: List[ImageTagDetailTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageTagDetailTypeDef](./type_defs.md#imagetagdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRegistriesResponseTypeDef

```python
# DescribeRegistriesResponseTypeDef definition

class DescribeRegistriesResponseTypeDef(TypedDict):
    registries: List[RegistryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RegistryTypeDef](./type_defs.md#registrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
