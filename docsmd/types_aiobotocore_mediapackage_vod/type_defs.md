# Type definitions

> [Index](../README.md) > [MediaPackageVod](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaPackageVod](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
    type annotations stubs module [types-aiobotocore-mediapackage-vod](https://pypi.org/project/types-aiobotocore-mediapackage-vod/).

## SpekeKeyProviderUnionTypeDef

```python
# SpekeKeyProviderUnionTypeDef definition

SpekeKeyProviderUnionTypeDef = Union[
    SpekeKeyProviderTypeDef,  # (1)
    SpekeKeyProviderOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
2. See [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 

## CmafEncryptionUnionTypeDef

```python
# CmafEncryptionUnionTypeDef definition

CmafEncryptionUnionTypeDef = Union[
    CmafEncryptionTypeDef,  # (1)
    CmafEncryptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CmafEncryptionTypeDef](./type_defs.md#cmafencryptiontypedef) 
2. See [:material-code-braces: CmafEncryptionOutputTypeDef](./type_defs.md#cmafencryptionoutputtypedef) 

## DashEncryptionUnionTypeDef

```python
# DashEncryptionUnionTypeDef definition

DashEncryptionUnionTypeDef = Union[
    DashEncryptionTypeDef,  # (1)
    DashEncryptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DashEncryptionTypeDef](./type_defs.md#dashencryptiontypedef) 
2. See [:material-code-braces: DashEncryptionOutputTypeDef](./type_defs.md#dashencryptionoutputtypedef) 

## HlsEncryptionUnionTypeDef

```python
# HlsEncryptionUnionTypeDef definition

HlsEncryptionUnionTypeDef = Union[
    HlsEncryptionTypeDef,  # (1)
    HlsEncryptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HlsEncryptionTypeDef](./type_defs.md#hlsencryptiontypedef) 
2. See [:material-code-braces: HlsEncryptionOutputTypeDef](./type_defs.md#hlsencryptionoutputtypedef) 

## MssEncryptionUnionTypeDef

```python
# MssEncryptionUnionTypeDef definition

MssEncryptionUnionTypeDef = Union[
    MssEncryptionTypeDef,  # (1)
    MssEncryptionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MssEncryptionTypeDef](./type_defs.md#mssencryptiontypedef) 
2. See [:material-code-braces: MssEncryptionOutputTypeDef](./type_defs.md#mssencryptionoutputtypedef) 



## AssetShallowTypeDef

```python
# AssetShallowTypeDef definition

class AssetShallowTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedAt: NotRequired[str],
    Id: NotRequired[str],
    PackagingGroupId: NotRequired[str],
    ResourceId: NotRequired[str],
    SourceArn: NotRequired[str],
    SourceRoleArn: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

## AuthorizationTypeDef

```python
# AuthorizationTypeDef definition

class AuthorizationTypeDef(TypedDict):
    CdnIdentifierSecret: str,
    SecretsRoleArn: str,
```

## EgressAccessLogsTypeDef

```python
# EgressAccessLogsTypeDef definition

class EgressAccessLogsTypeDef(TypedDict):
    LogGroupName: NotRequired[str],
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

## CreateAssetRequestRequestTypeDef

```python
# CreateAssetRequestRequestTypeDef definition

class CreateAssetRequestRequestTypeDef(TypedDict):
    Id: str,
    PackagingGroupId: str,
    SourceArn: str,
    SourceRoleArn: str,
    ResourceId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## EgressEndpointTypeDef

```python
# EgressEndpointTypeDef definition

class EgressEndpointTypeDef(TypedDict):
    PackagingConfigurationId: NotRequired[str],
    Status: NotRequired[str],
    Url: NotRequired[str],
```

## StreamSelectionTypeDef

```python
# StreamSelectionTypeDef definition

class StreamSelectionTypeDef(TypedDict):
    MaxVideoBitsPerSecond: NotRequired[int],
    MinVideoBitsPerSecond: NotRequired[int],
    StreamOrder: NotRequired[StreamOrderType],  # (1)
```

1. See [:material-code-brackets: StreamOrderType](./literals.md#streamordertype) 
## DeleteAssetRequestRequestTypeDef

```python
# DeleteAssetRequestRequestTypeDef definition

class DeleteAssetRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeletePackagingConfigurationRequestRequestTypeDef

```python
# DeletePackagingConfigurationRequestRequestTypeDef definition

class DeletePackagingConfigurationRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeletePackagingGroupRequestRequestTypeDef

```python
# DeletePackagingGroupRequestRequestTypeDef definition

class DeletePackagingGroupRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DescribeAssetRequestRequestTypeDef

```python
# DescribeAssetRequestRequestTypeDef definition

class DescribeAssetRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DescribePackagingConfigurationRequestRequestTypeDef

```python
# DescribePackagingConfigurationRequestRequestTypeDef definition

class DescribePackagingConfigurationRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DescribePackagingGroupRequestRequestTypeDef

```python
# DescribePackagingGroupRequestRequestTypeDef definition

class DescribePackagingGroupRequestRequestTypeDef(TypedDict):
    Id: str,
```

## EncryptionContractConfigurationTypeDef

```python
# EncryptionContractConfigurationTypeDef definition

class EncryptionContractConfigurationTypeDef(TypedDict):
    PresetSpeke20Audio: PresetSpeke20AudioType,  # (1)
    PresetSpeke20Video: PresetSpeke20VideoType,  # (2)
```

1. See [:material-code-brackets: PresetSpeke20AudioType](./literals.md#presetspeke20audiotype) 
2. See [:material-code-brackets: PresetSpeke20VideoType](./literals.md#presetspeke20videotype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAssetsRequestRequestTypeDef

```python
# ListAssetsRequestRequestTypeDef definition

class ListAssetsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    PackagingGroupId: NotRequired[str],
```

## ListPackagingConfigurationsRequestRequestTypeDef

```python
# ListPackagingConfigurationsRequestRequestTypeDef definition

class ListPackagingConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    PackagingGroupId: NotRequired[str],
```

## ListPackagingGroupsRequestRequestTypeDef

```python
# ListPackagingGroupsRequestRequestTypeDef definition

class ListPackagingGroupsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdatePackagingGroupRequestRequestTypeDef

```python
# UpdatePackagingGroupRequestRequestTypeDef definition

class UpdatePackagingGroupRequestRequestTypeDef(TypedDict):
    Id: str,
    Authorization: NotRequired[AuthorizationTypeDef],  # (1)
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
## ConfigureLogsRequestRequestTypeDef

```python
# ConfigureLogsRequestRequestTypeDef definition

class ConfigureLogsRequestRequestTypeDef(TypedDict):
    Id: str,
    EgressAccessLogs: NotRequired[EgressAccessLogsTypeDef],  # (1)
```

1. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
## CreatePackagingGroupRequestRequestTypeDef

```python
# CreatePackagingGroupRequestRequestTypeDef definition

class CreatePackagingGroupRequestRequestTypeDef(TypedDict):
    Id: str,
    Authorization: NotRequired[AuthorizationTypeDef],  # (1)
    EgressAccessLogs: NotRequired[EgressAccessLogsTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
## PackagingGroupTypeDef

```python
# PackagingGroupTypeDef definition

class PackagingGroupTypeDef(TypedDict):
    ApproximateAssetCount: NotRequired[int],
    Arn: NotRequired[str],
    Authorization: NotRequired[AuthorizationTypeDef],  # (1)
    CreatedAt: NotRequired[str],
    DomainName: NotRequired[str],
    EgressAccessLogs: NotRequired[EgressAccessLogsTypeDef],  # (2)
    Id: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
## ConfigureLogsResponseTypeDef

```python
# ConfigureLogsResponseTypeDef definition

class ConfigureLogsResponseTypeDef(TypedDict):
    Arn: str,
    Authorization: AuthorizationTypeDef,  # (1)
    CreatedAt: str,
    DomainName: str,
    EgressAccessLogs: EgressAccessLogsTypeDef,  # (2)
    Id: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePackagingGroupResponseTypeDef

```python
# CreatePackagingGroupResponseTypeDef definition

class CreatePackagingGroupResponseTypeDef(TypedDict):
    Arn: str,
    Authorization: AuthorizationTypeDef,  # (1)
    CreatedAt: str,
    DomainName: str,
    EgressAccessLogs: EgressAccessLogsTypeDef,  # (2)
    Id: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePackagingGroupResponseTypeDef

```python
# DescribePackagingGroupResponseTypeDef definition

class DescribePackagingGroupResponseTypeDef(TypedDict):
    ApproximateAssetCount: int,
    Arn: str,
    Authorization: AuthorizationTypeDef,  # (1)
    CreatedAt: str,
    DomainName: str,
    EgressAccessLogs: EgressAccessLogsTypeDef,  # (2)
    Id: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetsResponseTypeDef

```python
# ListAssetsResponseTypeDef definition

class ListAssetsResponseTypeDef(TypedDict):
    Assets: List[AssetShallowTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetShallowTypeDef](./type_defs.md#assetshallowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePackagingGroupResponseTypeDef

```python
# UpdatePackagingGroupResponseTypeDef definition

class UpdatePackagingGroupResponseTypeDef(TypedDict):
    ApproximateAssetCount: int,
    Arn: str,
    Authorization: AuthorizationTypeDef,  # (1)
    CreatedAt: str,
    DomainName: str,
    EgressAccessLogs: EgressAccessLogsTypeDef,  # (2)
    Id: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAssetResponseTypeDef

```python
# CreateAssetResponseTypeDef definition

class CreateAssetResponseTypeDef(TypedDict):
    Arn: str,
    CreatedAt: str,
    EgressEndpoints: List[EgressEndpointTypeDef],  # (1)
    Id: str,
    PackagingGroupId: str,
    ResourceId: str,
    SourceArn: str,
    SourceRoleArn: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EgressEndpointTypeDef](./type_defs.md#egressendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAssetResponseTypeDef

```python
# DescribeAssetResponseTypeDef definition

class DescribeAssetResponseTypeDef(TypedDict):
    Arn: str,
    CreatedAt: str,
    EgressEndpoints: List[EgressEndpointTypeDef],  # (1)
    Id: str,
    PackagingGroupId: str,
    ResourceId: str,
    SourceArn: str,
    SourceRoleArn: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EgressEndpointTypeDef](./type_defs.md#egressendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DashManifestTypeDef

```python
# DashManifestTypeDef definition

class DashManifestTypeDef(TypedDict):
    ManifestLayout: NotRequired[ManifestLayoutType],  # (1)
    ManifestName: NotRequired[str],
    MinBufferTimeSeconds: NotRequired[int],
    Profile: NotRequired[ProfileType],  # (2)
    ScteMarkersSource: NotRequired[ScteMarkersSourceType],  # (3)
    StreamSelection: NotRequired[StreamSelectionTypeDef],  # (4)
```

1. See [:material-code-brackets: ManifestLayoutType](./literals.md#manifestlayouttype) 
2. See [:material-code-brackets: ProfileType](./literals.md#profiletype) 
3. See [:material-code-brackets: ScteMarkersSourceType](./literals.md#sctemarkerssourcetype) 
4. See [:material-code-braces: StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef) 
## HlsManifestTypeDef

```python
# HlsManifestTypeDef definition

class HlsManifestTypeDef(TypedDict):
    AdMarkers: NotRequired[AdMarkersType],  # (1)
    IncludeIframeOnlyStream: NotRequired[bool],
    ManifestName: NotRequired[str],
    ProgramDateTimeIntervalSeconds: NotRequired[int],
    RepeatExtXKey: NotRequired[bool],
    StreamSelection: NotRequired[StreamSelectionTypeDef],  # (2)
```

1. See [:material-code-brackets: AdMarkersType](./literals.md#admarkerstype) 
2. See [:material-code-braces: StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef) 
## MssManifestTypeDef

```python
# MssManifestTypeDef definition

class MssManifestTypeDef(TypedDict):
    ManifestName: NotRequired[str],
    StreamSelection: NotRequired[StreamSelectionTypeDef],  # (1)
```

1. See [:material-code-braces: StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef) 
## SpekeKeyProviderOutputTypeDef

```python
# SpekeKeyProviderOutputTypeDef definition

class SpekeKeyProviderOutputTypeDef(TypedDict):
    RoleArn: str,
    SystemIds: List[str],
    Url: str,
    EncryptionContractConfiguration: NotRequired[EncryptionContractConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionContractConfigurationTypeDef](./type_defs.md#encryptioncontractconfigurationtypedef) 
## SpekeKeyProviderTypeDef

```python
# SpekeKeyProviderTypeDef definition

class SpekeKeyProviderTypeDef(TypedDict):
    RoleArn: str,
    SystemIds: Sequence[str],
    Url: str,
    EncryptionContractConfiguration: NotRequired[EncryptionContractConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionContractConfigurationTypeDef](./type_defs.md#encryptioncontractconfigurationtypedef) 
## ListAssetsRequestListAssetsPaginateTypeDef

```python
# ListAssetsRequestListAssetsPaginateTypeDef definition

class ListAssetsRequestListAssetsPaginateTypeDef(TypedDict):
    PackagingGroupId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef

```python
# ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef definition

class ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef(TypedDict):
    PackagingGroupId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef

```python
# ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef definition

class ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPackagingGroupsResponseTypeDef

```python
# ListPackagingGroupsResponseTypeDef definition

class ListPackagingGroupsResponseTypeDef(TypedDict):
    PackagingGroups: List[PackagingGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PackagingGroupTypeDef](./type_defs.md#packaginggrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CmafEncryptionOutputTypeDef

```python
# CmafEncryptionOutputTypeDef definition

class CmafEncryptionOutputTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderOutputTypeDef,  # (1)
    ConstantInitializationVector: NotRequired[str],
```

1. See [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
## DashEncryptionOutputTypeDef

```python
# DashEncryptionOutputTypeDef definition

class DashEncryptionOutputTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderOutputTypeDef,  # (1)
```

1. See [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
## HlsEncryptionOutputTypeDef

```python
# HlsEncryptionOutputTypeDef definition

class HlsEncryptionOutputTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderOutputTypeDef,  # (2)
    ConstantInitializationVector: NotRequired[str],
    EncryptionMethod: NotRequired[EncryptionMethodType],  # (1)
```

1. See [:material-code-brackets: EncryptionMethodType](./literals.md#encryptionmethodtype) 
2. See [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
## MssEncryptionOutputTypeDef

```python
# MssEncryptionOutputTypeDef definition

class MssEncryptionOutputTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderOutputTypeDef,  # (1)
```

1. See [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
## CmafPackageOutputTypeDef

```python
# CmafPackageOutputTypeDef definition

class CmafPackageOutputTypeDef(TypedDict):
    HlsManifests: List[HlsManifestTypeDef],  # (2)
    Encryption: NotRequired[CmafEncryptionOutputTypeDef],  # (1)
    IncludeEncoderConfigurationInSegments: NotRequired[bool],
    SegmentDurationSeconds: NotRequired[int],
```

1. See [:material-code-braces: CmafEncryptionOutputTypeDef](./type_defs.md#cmafencryptionoutputtypedef) 
2. See [:material-code-braces: HlsManifestTypeDef](./type_defs.md#hlsmanifesttypedef) 
## DashPackageOutputTypeDef

```python
# DashPackageOutputTypeDef definition

class DashPackageOutputTypeDef(TypedDict):
    DashManifests: List[DashManifestTypeDef],  # (1)
    Encryption: NotRequired[DashEncryptionOutputTypeDef],  # (2)
    IncludeEncoderConfigurationInSegments: NotRequired[bool],
    IncludeIframeOnlyStream: NotRequired[bool],
    PeriodTriggers: NotRequired[List[PeriodTriggersElementType]],  # (3)
    SegmentDurationSeconds: NotRequired[int],
    SegmentTemplateFormat: NotRequired[SegmentTemplateFormatType],  # (4)
```

1. See [:material-code-braces: DashManifestTypeDef](./type_defs.md#dashmanifesttypedef) 
2. See [:material-code-braces: DashEncryptionOutputTypeDef](./type_defs.md#dashencryptionoutputtypedef) 
3. See [:material-code-brackets: PeriodTriggersElementType](./literals.md#periodtriggerselementtype) 
4. See [:material-code-brackets: SegmentTemplateFormatType](./literals.md#segmenttemplateformattype) 
## HlsPackageOutputTypeDef

```python
# HlsPackageOutputTypeDef definition

class HlsPackageOutputTypeDef(TypedDict):
    HlsManifests: List[HlsManifestTypeDef],  # (2)
    Encryption: NotRequired[HlsEncryptionOutputTypeDef],  # (1)
    IncludeDvbSubtitles: NotRequired[bool],
    SegmentDurationSeconds: NotRequired[int],
    UseAudioRenditionGroup: NotRequired[bool],
```

1. See [:material-code-braces: HlsEncryptionOutputTypeDef](./type_defs.md#hlsencryptionoutputtypedef) 
2. See [:material-code-braces: HlsManifestTypeDef](./type_defs.md#hlsmanifesttypedef) 
## MssPackageOutputTypeDef

```python
# MssPackageOutputTypeDef definition

class MssPackageOutputTypeDef(TypedDict):
    MssManifests: List[MssManifestTypeDef],  # (2)
    Encryption: NotRequired[MssEncryptionOutputTypeDef],  # (1)
    SegmentDurationSeconds: NotRequired[int],
```

1. See [:material-code-braces: MssEncryptionOutputTypeDef](./type_defs.md#mssencryptionoutputtypedef) 
2. See [:material-code-braces: MssManifestTypeDef](./type_defs.md#mssmanifesttypedef) 
## CmafEncryptionTypeDef

```python
# CmafEncryptionTypeDef definition

class CmafEncryptionTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderUnionTypeDef,  # (1)
    ConstantInitializationVector: NotRequired[str],
```

1. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
## DashEncryptionTypeDef

```python
# DashEncryptionTypeDef definition

class DashEncryptionTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderUnionTypeDef,  # (1)
```

1. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
## HlsEncryptionTypeDef

```python
# HlsEncryptionTypeDef definition

class HlsEncryptionTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderUnionTypeDef,  # (2)
    ConstantInitializationVector: NotRequired[str],
    EncryptionMethod: NotRequired[EncryptionMethodType],  # (1)
```

1. See [:material-code-brackets: EncryptionMethodType](./literals.md#encryptionmethodtype) 
2. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
## MssEncryptionTypeDef

```python
# MssEncryptionTypeDef definition

class MssEncryptionTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderUnionTypeDef,  # (1)
```

1. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) [:material-code-braces: SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef) 
## CreatePackagingConfigurationResponseTypeDef

```python
# CreatePackagingConfigurationResponseTypeDef definition

class CreatePackagingConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    CmafPackage: CmafPackageOutputTypeDef,  # (1)
    CreatedAt: str,
    DashPackage: DashPackageOutputTypeDef,  # (2)
    HlsPackage: HlsPackageOutputTypeDef,  # (3)
    Id: str,
    MssPackage: MssPackageOutputTypeDef,  # (4)
    PackagingGroupId: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: CmafPackageOutputTypeDef](./type_defs.md#cmafpackageoutputtypedef) 
2. See [:material-code-braces: DashPackageOutputTypeDef](./type_defs.md#dashpackageoutputtypedef) 
3. See [:material-code-braces: HlsPackageOutputTypeDef](./type_defs.md#hlspackageoutputtypedef) 
4. See [:material-code-braces: MssPackageOutputTypeDef](./type_defs.md#msspackageoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePackagingConfigurationResponseTypeDef

```python
# DescribePackagingConfigurationResponseTypeDef definition

class DescribePackagingConfigurationResponseTypeDef(TypedDict):
    Arn: str,
    CmafPackage: CmafPackageOutputTypeDef,  # (1)
    CreatedAt: str,
    DashPackage: DashPackageOutputTypeDef,  # (2)
    HlsPackage: HlsPackageOutputTypeDef,  # (3)
    Id: str,
    MssPackage: MssPackageOutputTypeDef,  # (4)
    PackagingGroupId: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: CmafPackageOutputTypeDef](./type_defs.md#cmafpackageoutputtypedef) 
2. See [:material-code-braces: DashPackageOutputTypeDef](./type_defs.md#dashpackageoutputtypedef) 
3. See [:material-code-braces: HlsPackageOutputTypeDef](./type_defs.md#hlspackageoutputtypedef) 
4. See [:material-code-braces: MssPackageOutputTypeDef](./type_defs.md#msspackageoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PackagingConfigurationTypeDef

```python
# PackagingConfigurationTypeDef definition

class PackagingConfigurationTypeDef(TypedDict):
    Arn: NotRequired[str],
    CmafPackage: NotRequired[CmafPackageOutputTypeDef],  # (1)
    CreatedAt: NotRequired[str],
    DashPackage: NotRequired[DashPackageOutputTypeDef],  # (2)
    HlsPackage: NotRequired[HlsPackageOutputTypeDef],  # (3)
    Id: NotRequired[str],
    MssPackage: NotRequired[MssPackageOutputTypeDef],  # (4)
    PackagingGroupId: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: CmafPackageOutputTypeDef](./type_defs.md#cmafpackageoutputtypedef) 
2. See [:material-code-braces: DashPackageOutputTypeDef](./type_defs.md#dashpackageoutputtypedef) 
3. See [:material-code-braces: HlsPackageOutputTypeDef](./type_defs.md#hlspackageoutputtypedef) 
4. See [:material-code-braces: MssPackageOutputTypeDef](./type_defs.md#msspackageoutputtypedef) 
## ListPackagingConfigurationsResponseTypeDef

```python
# ListPackagingConfigurationsResponseTypeDef definition

class ListPackagingConfigurationsResponseTypeDef(TypedDict):
    PackagingConfigurations: List[PackagingConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PackagingConfigurationTypeDef](./type_defs.md#packagingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CmafPackageTypeDef

```python
# CmafPackageTypeDef definition

class CmafPackageTypeDef(TypedDict):
    HlsManifests: Sequence[HlsManifestTypeDef],  # (2)
    Encryption: NotRequired[CmafEncryptionUnionTypeDef],  # (1)
    IncludeEncoderConfigurationInSegments: NotRequired[bool],
    SegmentDurationSeconds: NotRequired[int],
```

1. See [:material-code-braces: CmafEncryptionTypeDef](./type_defs.md#cmafencryptiontypedef) [:material-code-braces: CmafEncryptionOutputTypeDef](./type_defs.md#cmafencryptionoutputtypedef) 
2. See [:material-code-braces: HlsManifestTypeDef](./type_defs.md#hlsmanifesttypedef) 
## DashPackageTypeDef

```python
# DashPackageTypeDef definition

class DashPackageTypeDef(TypedDict):
    DashManifests: Sequence[DashManifestTypeDef],  # (1)
    Encryption: NotRequired[DashEncryptionUnionTypeDef],  # (2)
    IncludeEncoderConfigurationInSegments: NotRequired[bool],
    IncludeIframeOnlyStream: NotRequired[bool],
    PeriodTriggers: NotRequired[Sequence[PeriodTriggersElementType]],  # (3)
    SegmentDurationSeconds: NotRequired[int],
    SegmentTemplateFormat: NotRequired[SegmentTemplateFormatType],  # (4)
```

1. See [:material-code-braces: DashManifestTypeDef](./type_defs.md#dashmanifesttypedef) 
2. See [:material-code-braces: DashEncryptionTypeDef](./type_defs.md#dashencryptiontypedef) [:material-code-braces: DashEncryptionOutputTypeDef](./type_defs.md#dashencryptionoutputtypedef) 
3. See [:material-code-brackets: PeriodTriggersElementType](./literals.md#periodtriggerselementtype) 
4. See [:material-code-brackets: SegmentTemplateFormatType](./literals.md#segmenttemplateformattype) 
## HlsPackageTypeDef

```python
# HlsPackageTypeDef definition

class HlsPackageTypeDef(TypedDict):
    HlsManifests: Sequence[HlsManifestTypeDef],  # (2)
    Encryption: NotRequired[HlsEncryptionUnionTypeDef],  # (1)
    IncludeDvbSubtitles: NotRequired[bool],
    SegmentDurationSeconds: NotRequired[int],
    UseAudioRenditionGroup: NotRequired[bool],
```

1. See [:material-code-braces: HlsEncryptionTypeDef](./type_defs.md#hlsencryptiontypedef) [:material-code-braces: HlsEncryptionOutputTypeDef](./type_defs.md#hlsencryptionoutputtypedef) 
2. See [:material-code-braces: HlsManifestTypeDef](./type_defs.md#hlsmanifesttypedef) 
## MssPackageTypeDef

```python
# MssPackageTypeDef definition

class MssPackageTypeDef(TypedDict):
    MssManifests: Sequence[MssManifestTypeDef],  # (2)
    Encryption: NotRequired[MssEncryptionUnionTypeDef],  # (1)
    SegmentDurationSeconds: NotRequired[int],
```

1. See [:material-code-braces: MssEncryptionTypeDef](./type_defs.md#mssencryptiontypedef) [:material-code-braces: MssEncryptionOutputTypeDef](./type_defs.md#mssencryptionoutputtypedef) 
2. See [:material-code-braces: MssManifestTypeDef](./type_defs.md#mssmanifesttypedef) 
## CreatePackagingConfigurationRequestRequestTypeDef

```python
# CreatePackagingConfigurationRequestRequestTypeDef definition

class CreatePackagingConfigurationRequestRequestTypeDef(TypedDict):
    Id: str,
    PackagingGroupId: str,
    CmafPackage: NotRequired[CmafPackageTypeDef],  # (1)
    DashPackage: NotRequired[DashPackageTypeDef],  # (2)
    HlsPackage: NotRequired[HlsPackageTypeDef],  # (3)
    MssPackage: NotRequired[MssPackageTypeDef],  # (4)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CmafPackageTypeDef](./type_defs.md#cmafpackagetypedef) 
2. See [:material-code-braces: DashPackageTypeDef](./type_defs.md#dashpackagetypedef) 
3. See [:material-code-braces: HlsPackageTypeDef](./type_defs.md#hlspackagetypedef) 
4. See [:material-code-braces: MssPackageTypeDef](./type_defs.md#msspackagetypedef) 
