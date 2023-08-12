# Type definitions

> [Index](../README.md) > [mediapackagev2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [mediapackagev2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
    type annotations stubs module [types-aiobotocore-mediapackagev2](https://pypi.org/project/types-aiobotocore-mediapackagev2/).



## ChannelGroupListConfigurationTypeDef

```python
# ChannelGroupListConfigurationTypeDef definition

class ChannelGroupListConfigurationTypeDef(TypedDict):
    ChannelGroupName: str,
    Arn: str,
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: NotRequired[str],
```

## ChannelListConfigurationTypeDef

```python
# ChannelListConfigurationTypeDef definition

class ChannelListConfigurationTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ChannelGroupName: str,
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: NotRequired[str],
```

## CreateChannelGroupRequestRequestTypeDef

```python
# CreateChannelGroupRequestRequestTypeDef definition

class CreateChannelGroupRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
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

## CreateChannelRequestRequestTypeDef

```python
# CreateChannelRequestRequestTypeDef definition

class CreateChannelRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## IngestEndpointTypeDef

```python
# IngestEndpointTypeDef definition

class IngestEndpointTypeDef(TypedDict):
    Id: NotRequired[str],
    Url: NotRequired[str],
```

## ScteHlsTypeDef

```python
# ScteHlsTypeDef definition

class ScteHlsTypeDef(TypedDict):
    AdMarkerHls: NotRequired[AdMarkerHlsType],  # (1)
```

1. See [:material-code-brackets: AdMarkerHlsType](./literals.md#admarkerhlstype) 
## DeleteChannelGroupRequestRequestTypeDef

```python
# DeleteChannelGroupRequestRequestTypeDef definition

class DeleteChannelGroupRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
```

## DeleteChannelPolicyRequestRequestTypeDef

```python
# DeleteChannelPolicyRequestRequestTypeDef definition

class DeleteChannelPolicyRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
```

## DeleteChannelRequestRequestTypeDef

```python
# DeleteChannelRequestRequestTypeDef definition

class DeleteChannelRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
```

## DeleteOriginEndpointPolicyRequestRequestTypeDef

```python
# DeleteOriginEndpointPolicyRequestRequestTypeDef definition

class DeleteOriginEndpointPolicyRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
```

## DeleteOriginEndpointRequestRequestTypeDef

```python
# DeleteOriginEndpointRequestRequestTypeDef definition

class DeleteOriginEndpointRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
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
## EncryptionMethodTypeDef

```python
# EncryptionMethodTypeDef definition

class EncryptionMethodTypeDef(TypedDict):
    TsEncryptionMethod: NotRequired[TsEncryptionMethodType],  # (1)
    CmafEncryptionMethod: NotRequired[CmafEncryptionMethodType],  # (2)
```

1. See [:material-code-brackets: TsEncryptionMethodType](./literals.md#tsencryptionmethodtype) 
2. See [:material-code-brackets: CmafEncryptionMethodType](./literals.md#cmafencryptionmethodtype) 
## GetChannelGroupRequestRequestTypeDef

```python
# GetChannelGroupRequestRequestTypeDef definition

class GetChannelGroupRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
```

## GetChannelPolicyRequestRequestTypeDef

```python
# GetChannelPolicyRequestRequestTypeDef definition

class GetChannelPolicyRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
```

## GetChannelRequestRequestTypeDef

```python
# GetChannelRequestRequestTypeDef definition

class GetChannelRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
```

## GetOriginEndpointPolicyRequestRequestTypeDef

```python
# GetOriginEndpointPolicyRequestRequestTypeDef definition

class GetOriginEndpointPolicyRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
```

## GetOriginEndpointRequestRequestTypeDef

```python
# GetOriginEndpointRequestRequestTypeDef definition

class GetOriginEndpointRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListChannelGroupsRequestRequestTypeDef

```python
# ListChannelGroupsRequestRequestTypeDef definition

class ListChannelGroupsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListHlsManifestConfigurationTypeDef

```python
# ListHlsManifestConfigurationTypeDef definition

class ListHlsManifestConfigurationTypeDef(TypedDict):
    ManifestName: str,
    ChildManifestName: NotRequired[str],
    Url: NotRequired[str],
```

## ListLowLatencyHlsManifestConfigurationTypeDef

```python
# ListLowLatencyHlsManifestConfigurationTypeDef definition

class ListLowLatencyHlsManifestConfigurationTypeDef(TypedDict):
    ManifestName: str,
    ChildManifestName: NotRequired[str],
    Url: NotRequired[str],
```

## ListOriginEndpointsRequestRequestTypeDef

```python
# ListOriginEndpointsRequestRequestTypeDef definition

class ListOriginEndpointsRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PutChannelPolicyRequestRequestTypeDef

```python
# PutChannelPolicyRequestRequestTypeDef definition

class PutChannelPolicyRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    Policy: str,
```

## PutOriginEndpointPolicyRequestRequestTypeDef

```python
# PutOriginEndpointPolicyRequestRequestTypeDef definition

class PutOriginEndpointPolicyRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    Policy: str,
```

## ScteTypeDef

```python
# ScteTypeDef definition

class ScteTypeDef(TypedDict):
    ScteFilter: NotRequired[Sequence[ScteFilterType]],  # (1)
```

1. See [:material-code-brackets: ScteFilterType](./literals.md#sctefiltertype) 
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

## UpdateChannelGroupRequestRequestTypeDef

```python
# UpdateChannelGroupRequestRequestTypeDef definition

class UpdateChannelGroupRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    Description: NotRequired[str],
```

## UpdateChannelRequestRequestTypeDef

```python
# UpdateChannelRequestRequestTypeDef definition

class UpdateChannelRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    Description: NotRequired[str],
```

## CreateChannelGroupResponseTypeDef

```python
# CreateChannelGroupResponseTypeDef definition

class CreateChannelGroupResponseTypeDef(TypedDict):
    ChannelGroupName: str,
    Arn: str,
    EgressDomain: str,
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: str,
    Tags: Dict[str, str],
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
## GetChannelGroupResponseTypeDef

```python
# GetChannelGroupResponseTypeDef definition

class GetChannelGroupResponseTypeDef(TypedDict):
    ChannelGroupName: str,
    Arn: str,
    EgressDomain: str,
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChannelPolicyResponseTypeDef

```python
# GetChannelPolicyResponseTypeDef definition

class GetChannelPolicyResponseTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOriginEndpointPolicyResponseTypeDef

```python
# GetOriginEndpointPolicyResponseTypeDef definition

class GetOriginEndpointPolicyResponseTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelGroupsResponseTypeDef

```python
# ListChannelGroupsResponseTypeDef definition

class ListChannelGroupsResponseTypeDef(TypedDict):
    Items: List[ChannelGroupListConfigurationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelGroupListConfigurationTypeDef](./type_defs.md#channelgrouplistconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    Items: List[ChannelListConfigurationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelListConfigurationTypeDef](./type_defs.md#channellistconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelGroupResponseTypeDef

```python
# UpdateChannelGroupResponseTypeDef definition

class UpdateChannelGroupResponseTypeDef(TypedDict):
    ChannelGroupName: str,
    Arn: str,
    EgressDomain: str,
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelResponseTypeDef

```python
# CreateChannelResponseTypeDef definition

class CreateChannelResponseTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ChannelGroupName: str,
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: str,
    IngestEndpoints: List[IngestEndpointTypeDef],  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestEndpointTypeDef](./type_defs.md#ingestendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChannelResponseTypeDef

```python
# GetChannelResponseTypeDef definition

class GetChannelResponseTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ChannelGroupName: str,
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: str,
    IngestEndpoints: List[IngestEndpointTypeDef],  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestEndpointTypeDef](./type_defs.md#ingestendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelResponseTypeDef

```python
# UpdateChannelResponseTypeDef definition

class UpdateChannelResponseTypeDef(TypedDict):
    Arn: str,
    ChannelName: str,
    ChannelGroupName: str,
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: str,
    IngestEndpoints: List[IngestEndpointTypeDef],  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestEndpointTypeDef](./type_defs.md#ingestendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHlsManifestConfigurationTypeDef

```python
# CreateHlsManifestConfigurationTypeDef definition

class CreateHlsManifestConfigurationTypeDef(TypedDict):
    ManifestName: str,
    ChildManifestName: NotRequired[str],
    ScteHls: NotRequired[ScteHlsTypeDef],  # (1)
    ManifestWindowSeconds: NotRequired[int],
    ProgramDateTimeIntervalSeconds: NotRequired[int],
```

1. See [:material-code-braces: ScteHlsTypeDef](./type_defs.md#sctehlstypedef) 
## CreateLowLatencyHlsManifestConfigurationTypeDef

```python
# CreateLowLatencyHlsManifestConfigurationTypeDef definition

class CreateLowLatencyHlsManifestConfigurationTypeDef(TypedDict):
    ManifestName: str,
    ChildManifestName: NotRequired[str],
    ScteHls: NotRequired[ScteHlsTypeDef],  # (1)
    ManifestWindowSeconds: NotRequired[int],
    ProgramDateTimeIntervalSeconds: NotRequired[int],
```

1. See [:material-code-braces: ScteHlsTypeDef](./type_defs.md#sctehlstypedef) 
## GetHlsManifestConfigurationTypeDef

```python
# GetHlsManifestConfigurationTypeDef definition

class GetHlsManifestConfigurationTypeDef(TypedDict):
    ManifestName: str,
    Url: str,
    ChildManifestName: NotRequired[str],
    ManifestWindowSeconds: NotRequired[int],
    ProgramDateTimeIntervalSeconds: NotRequired[int],
    ScteHls: NotRequired[ScteHlsTypeDef],  # (1)
```

1. See [:material-code-braces: ScteHlsTypeDef](./type_defs.md#sctehlstypedef) 
## GetLowLatencyHlsManifestConfigurationTypeDef

```python
# GetLowLatencyHlsManifestConfigurationTypeDef definition

class GetLowLatencyHlsManifestConfigurationTypeDef(TypedDict):
    ManifestName: str,
    Url: str,
    ChildManifestName: NotRequired[str],
    ManifestWindowSeconds: NotRequired[int],
    ProgramDateTimeIntervalSeconds: NotRequired[int],
    ScteHls: NotRequired[ScteHlsTypeDef],  # (1)
```

1. See [:material-code-braces: ScteHlsTypeDef](./type_defs.md#sctehlstypedef) 
## SpekeKeyProviderTypeDef

```python
# SpekeKeyProviderTypeDef definition

class SpekeKeyProviderTypeDef(TypedDict):
    EncryptionContractConfiguration: EncryptionContractConfigurationTypeDef,  # (1)
    ResourceId: str,
    DrmSystems: Sequence[DrmSystemType],  # (2)
    RoleArn: str,
    Url: str,
```

1. See [:material-code-braces: EncryptionContractConfigurationTypeDef](./type_defs.md#encryptioncontractconfigurationtypedef) 
2. See [:material-code-brackets: DrmSystemType](./literals.md#drmsystemtype) 
## ListChannelGroupsRequestListChannelGroupsPaginateTypeDef

```python
# ListChannelGroupsRequestListChannelGroupsPaginateTypeDef definition

class ListChannelGroupsRequestListChannelGroupsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListChannelsRequestListChannelsPaginateTypeDef

```python
# ListChannelsRequestListChannelsPaginateTypeDef definition

class ListChannelsRequestListChannelsPaginateTypeDef(TypedDict):
    ChannelGroupName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef

```python
# ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef definition

class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## OriginEndpointListConfigurationTypeDef

```python
# OriginEndpointListConfigurationTypeDef definition

class OriginEndpointListConfigurationTypeDef(TypedDict):
    Arn: str,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    ContainerType: ContainerTypeType,  # (1)
    Description: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    ModifiedAt: NotRequired[datetime],
    HlsManifests: NotRequired[List[ListHlsManifestConfigurationTypeDef]],  # (2)
    LowLatencyHlsManifests: NotRequired[List[ListLowLatencyHlsManifestConfigurationTypeDef]],  # (3)
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: ListHlsManifestConfigurationTypeDef](./type_defs.md#listhlsmanifestconfigurationtypedef) 
3. See [:material-code-braces: ListLowLatencyHlsManifestConfigurationTypeDef](./type_defs.md#listlowlatencyhlsmanifestconfigurationtypedef) 
## EncryptionTypeDef

```python
# EncryptionTypeDef definition

class EncryptionTypeDef(TypedDict):
    EncryptionMethod: EncryptionMethodTypeDef,  # (1)
    SpekeKeyProvider: SpekeKeyProviderTypeDef,  # (2)
    ConstantInitializationVector: NotRequired[str],
    KeyRotationIntervalSeconds: NotRequired[int],
```

1. See [:material-code-braces: EncryptionMethodTypeDef](./type_defs.md#encryptionmethodtypedef) 
2. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
## ListOriginEndpointsResponseTypeDef

```python
# ListOriginEndpointsResponseTypeDef definition

class ListOriginEndpointsResponseTypeDef(TypedDict):
    Items: List[OriginEndpointListConfigurationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginEndpointListConfigurationTypeDef](./type_defs.md#originendpointlistconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SegmentTypeDef

```python
# SegmentTypeDef definition

class SegmentTypeDef(TypedDict):
    SegmentDurationSeconds: NotRequired[int],
    SegmentName: NotRequired[str],
    TsUseAudioRenditionGroup: NotRequired[bool],
    IncludeIframeOnlyStreams: NotRequired[bool],
    TsIncludeDvbSubtitles: NotRequired[bool],
    Scte: NotRequired[ScteTypeDef],  # (1)
    Encryption: NotRequired[EncryptionTypeDef],  # (2)
```

1. See [:material-code-braces: ScteTypeDef](./type_defs.md#sctetypedef) 
2. See [:material-code-braces: EncryptionTypeDef](./type_defs.md#encryptiontypedef) 
## CreateOriginEndpointRequestRequestTypeDef

```python
# CreateOriginEndpointRequestRequestTypeDef definition

class CreateOriginEndpointRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    ContainerType: ContainerTypeType,  # (1)
    Segment: NotRequired[SegmentTypeDef],  # (2)
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    StartoverWindowSeconds: NotRequired[int],
    HlsManifests: NotRequired[Sequence[CreateHlsManifestConfigurationTypeDef]],  # (3)
    LowLatencyHlsManifests: NotRequired[Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef]],  # (4)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
3. See [:material-code-braces: CreateHlsManifestConfigurationTypeDef](./type_defs.md#createhlsmanifestconfigurationtypedef) 
4. See [:material-code-braces: CreateLowLatencyHlsManifestConfigurationTypeDef](./type_defs.md#createlowlatencyhlsmanifestconfigurationtypedef) 
## CreateOriginEndpointResponseTypeDef

```python
# CreateOriginEndpointResponseTypeDef definition

class CreateOriginEndpointResponseTypeDef(TypedDict):
    Arn: str,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    ContainerType: ContainerTypeType,  # (1)
    Segment: SegmentTypeDef,  # (2)
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: str,
    StartoverWindowSeconds: int,
    HlsManifests: List[GetHlsManifestConfigurationTypeDef],  # (3)
    LowLatencyHlsManifests: List[GetLowLatencyHlsManifestConfigurationTypeDef],  # (4)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
3. See [:material-code-braces: GetHlsManifestConfigurationTypeDef](./type_defs.md#gethlsmanifestconfigurationtypedef) 
4. See [:material-code-braces: GetLowLatencyHlsManifestConfigurationTypeDef](./type_defs.md#getlowlatencyhlsmanifestconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOriginEndpointResponseTypeDef

```python
# GetOriginEndpointResponseTypeDef definition

class GetOriginEndpointResponseTypeDef(TypedDict):
    Arn: str,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    ContainerType: ContainerTypeType,  # (1)
    Segment: SegmentTypeDef,  # (2)
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: str,
    StartoverWindowSeconds: int,
    HlsManifests: List[GetHlsManifestConfigurationTypeDef],  # (3)
    LowLatencyHlsManifests: List[GetLowLatencyHlsManifestConfigurationTypeDef],  # (4)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
3. See [:material-code-braces: GetHlsManifestConfigurationTypeDef](./type_defs.md#gethlsmanifestconfigurationtypedef) 
4. See [:material-code-braces: GetLowLatencyHlsManifestConfigurationTypeDef](./type_defs.md#getlowlatencyhlsmanifestconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOriginEndpointRequestRequestTypeDef

```python
# UpdateOriginEndpointRequestRequestTypeDef definition

class UpdateOriginEndpointRequestRequestTypeDef(TypedDict):
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    ContainerType: ContainerTypeType,  # (1)
    Segment: NotRequired[SegmentTypeDef],  # (2)
    Description: NotRequired[str],
    StartoverWindowSeconds: NotRequired[int],
    HlsManifests: NotRequired[Sequence[CreateHlsManifestConfigurationTypeDef]],  # (3)
    LowLatencyHlsManifests: NotRequired[Sequence[CreateLowLatencyHlsManifestConfigurationTypeDef]],  # (4)
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
3. See [:material-code-braces: CreateHlsManifestConfigurationTypeDef](./type_defs.md#createhlsmanifestconfigurationtypedef) 
4. See [:material-code-braces: CreateLowLatencyHlsManifestConfigurationTypeDef](./type_defs.md#createlowlatencyhlsmanifestconfigurationtypedef) 
## UpdateOriginEndpointResponseTypeDef

```python
# UpdateOriginEndpointResponseTypeDef definition

class UpdateOriginEndpointResponseTypeDef(TypedDict):
    Arn: str,
    ChannelGroupName: str,
    ChannelName: str,
    OriginEndpointName: str,
    ContainerType: ContainerTypeType,  # (1)
    Segment: SegmentTypeDef,  # (2)
    CreatedAt: datetime,
    ModifiedAt: datetime,
    Description: str,
    StartoverWindowSeconds: int,
    HlsManifests: List[GetHlsManifestConfigurationTypeDef],  # (3)
    LowLatencyHlsManifests: List[GetLowLatencyHlsManifestConfigurationTypeDef],  # (4)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
3. See [:material-code-braces: GetHlsManifestConfigurationTypeDef](./type_defs.md#gethlsmanifestconfigurationtypedef) 
4. See [:material-code-braces: GetLowLatencyHlsManifestConfigurationTypeDef](./type_defs.md#getlowlatencyhlsmanifestconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
