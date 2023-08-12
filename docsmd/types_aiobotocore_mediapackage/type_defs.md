# Type definitions

> [Index](../README.md) > [MediaPackage](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaPackage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
    type annotations stubs module [types-aiobotocore-mediapackage](https://pypi.org/project/types-aiobotocore-mediapackage/).



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

## IngressAccessLogsTypeDef

```python
# IngressAccessLogsTypeDef definition

class IngressAccessLogsTypeDef(TypedDict):
    LogGroupName: NotRequired[str],
```

## HlsManifestCreateOrUpdateParametersTypeDef

```python
# HlsManifestCreateOrUpdateParametersTypeDef definition

class HlsManifestCreateOrUpdateParametersTypeDef(TypedDict):
    Id: str,
    AdMarkers: NotRequired[AdMarkersType],  # (1)
    AdTriggers: NotRequired[Sequence[AdTriggersElementType]],  # (2)
    AdsOnDeliveryRestrictions: NotRequired[AdsOnDeliveryRestrictionsType],  # (3)
    IncludeIframeOnlyStream: NotRequired[bool],
    ManifestName: NotRequired[str],
    PlaylistType: NotRequired[PlaylistTypeType],  # (4)
    PlaylistWindowSeconds: NotRequired[int],
    ProgramDateTimeIntervalSeconds: NotRequired[int],
```

1. See [:material-code-brackets: AdMarkersType](./literals.md#admarkerstype) 
2. See [:material-code-brackets: AdTriggersElementType](./literals.md#adtriggerselementtype) 
3. See [:material-code-brackets: AdsOnDeliveryRestrictionsType](./literals.md#adsondeliveryrestrictionstype) 
4. See [:material-code-brackets: PlaylistTypeType](./literals.md#playlisttypetype) 
## StreamSelectionTypeDef

```python
# StreamSelectionTypeDef definition

class StreamSelectionTypeDef(TypedDict):
    MaxVideoBitsPerSecond: NotRequired[int],
    MinVideoBitsPerSecond: NotRequired[int],
    StreamOrder: NotRequired[StreamOrderType],  # (1)
```

1. See [:material-code-brackets: StreamOrderType](./literals.md#streamordertype) 
## HlsManifestTypeDef

```python
# HlsManifestTypeDef definition

class HlsManifestTypeDef(TypedDict):
    Id: str,
    AdMarkers: NotRequired[AdMarkersType],  # (1)
    IncludeIframeOnlyStream: NotRequired[bool],
    ManifestName: NotRequired[str],
    PlaylistType: NotRequired[PlaylistTypeType],  # (2)
    PlaylistWindowSeconds: NotRequired[int],
    ProgramDateTimeIntervalSeconds: NotRequired[int],
    Url: NotRequired[str],
    AdTriggers: NotRequired[List[AdTriggersElementType]],  # (3)
    AdsOnDeliveryRestrictions: NotRequired[AdsOnDeliveryRestrictionsType],  # (4)
```

1. See [:material-code-brackets: AdMarkersType](./literals.md#admarkerstype) 
2. See [:material-code-brackets: PlaylistTypeType](./literals.md#playlisttypetype) 
3. See [:material-code-brackets: AdTriggersElementType](./literals.md#adtriggerselementtype) 
4. See [:material-code-brackets: AdsOnDeliveryRestrictionsType](./literals.md#adsondeliveryrestrictionstype) 
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
    Id: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## S3DestinationTypeDef

```python
# S3DestinationTypeDef definition

class S3DestinationTypeDef(TypedDict):
    BucketName: str,
    ManifestKey: str,
    RoleArn: str,
```

## DeleteChannelRequestRequestTypeDef

```python
# DeleteChannelRequestRequestTypeDef definition

class DeleteChannelRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteOriginEndpointRequestRequestTypeDef

```python
# DeleteOriginEndpointRequestRequestTypeDef definition

class DeleteOriginEndpointRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DescribeChannelRequestRequestTypeDef

```python
# DescribeChannelRequestRequestTypeDef definition

class DescribeChannelRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DescribeHarvestJobRequestRequestTypeDef

```python
# DescribeHarvestJobRequestRequestTypeDef definition

class DescribeHarvestJobRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DescribeOriginEndpointRequestRequestTypeDef

```python
# DescribeOriginEndpointRequestRequestTypeDef definition

class DescribeOriginEndpointRequestRequestTypeDef(TypedDict):
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
## IngestEndpointTypeDef

```python
# IngestEndpointTypeDef definition

class IngestEndpointTypeDef(TypedDict):
    Id: NotRequired[str],
    Password: NotRequired[str],
    Url: NotRequired[str],
    Username: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListHarvestJobsRequestRequestTypeDef

```python
# ListHarvestJobsRequestRequestTypeDef definition

class ListHarvestJobsRequestRequestTypeDef(TypedDict):
    IncludeChannelId: NotRequired[str],
    IncludeStatus: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListOriginEndpointsRequestRequestTypeDef

```python
# ListOriginEndpointsRequestRequestTypeDef definition

class ListOriginEndpointsRequestRequestTypeDef(TypedDict):
    ChannelId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## RotateChannelCredentialsRequestRequestTypeDef

```python
# RotateChannelCredentialsRequestRequestTypeDef definition

class RotateChannelCredentialsRequestRequestTypeDef(TypedDict):
    Id: str,
```

## RotateIngestEndpointCredentialsRequestRequestTypeDef

```python
# RotateIngestEndpointCredentialsRequestRequestTypeDef definition

class RotateIngestEndpointCredentialsRequestRequestTypeDef(TypedDict):
    Id: str,
    IngestEndpointId: str,
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

## UpdateChannelRequestRequestTypeDef

```python
# UpdateChannelRequestRequestTypeDef definition

class UpdateChannelRequestRequestTypeDef(TypedDict):
    Id: str,
    Description: NotRequired[str],
```

## ConfigureLogsRequestRequestTypeDef

```python
# ConfigureLogsRequestRequestTypeDef definition

class ConfigureLogsRequestRequestTypeDef(TypedDict):
    Id: str,
    EgressAccessLogs: NotRequired[EgressAccessLogsTypeDef],  # (1)
    IngressAccessLogs: NotRequired[IngressAccessLogsTypeDef],  # (2)
```

1. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
2. See [:material-code-braces: IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHarvestJobRequestRequestTypeDef

```python
# CreateHarvestJobRequestRequestTypeDef definition

class CreateHarvestJobRequestRequestTypeDef(TypedDict):
    EndTime: str,
    Id: str,
    OriginEndpointId: str,
    S3Destination: S3DestinationTypeDef,  # (1)
    StartTime: str,
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
## CreateHarvestJobResponseTypeDef

```python
# CreateHarvestJobResponseTypeDef definition

class CreateHarvestJobResponseTypeDef(TypedDict):
    Arn: str,
    ChannelId: str,
    CreatedAt: str,
    EndTime: str,
    Id: str,
    OriginEndpointId: str,
    S3Destination: S3DestinationTypeDef,  # (1)
    StartTime: str,
    Status: StatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeHarvestJobResponseTypeDef

```python
# DescribeHarvestJobResponseTypeDef definition

class DescribeHarvestJobResponseTypeDef(TypedDict):
    Arn: str,
    ChannelId: str,
    CreatedAt: str,
    EndTime: str,
    Id: str,
    OriginEndpointId: str,
    S3Destination: S3DestinationTypeDef,  # (1)
    StartTime: str,
    Status: StatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HarvestJobTypeDef

```python
# HarvestJobTypeDef definition

class HarvestJobTypeDef(TypedDict):
    Arn: NotRequired[str],
    ChannelId: NotRequired[str],
    CreatedAt: NotRequired[str],
    EndTime: NotRequired[str],
    Id: NotRequired[str],
    OriginEndpointId: NotRequired[str],
    S3Destination: NotRequired[S3DestinationTypeDef],  # (1)
    StartTime: NotRequired[str],
    Status: NotRequired[StatusType],  # (2)
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## SpekeKeyProviderTypeDef

```python
# SpekeKeyProviderTypeDef definition

class SpekeKeyProviderTypeDef(TypedDict):
    ResourceId: str,
    RoleArn: str,
    SystemIds: Sequence[str],
    Url: str,
    CertificateArn: NotRequired[str],
    EncryptionContractConfiguration: NotRequired[EncryptionContractConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionContractConfigurationTypeDef](./type_defs.md#encryptioncontractconfigurationtypedef) 
## HlsIngestTypeDef

```python
# HlsIngestTypeDef definition

class HlsIngestTypeDef(TypedDict):
    IngestEndpoints: NotRequired[List[IngestEndpointTypeDef]],  # (1)
```

1. See [:material-code-braces: IngestEndpointTypeDef](./type_defs.md#ingestendpointtypedef) 
## ListChannelsRequestListChannelsPaginateTypeDef

```python
# ListChannelsRequestListChannelsPaginateTypeDef definition

class ListChannelsRequestListChannelsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHarvestJobsRequestListHarvestJobsPaginateTypeDef

```python
# ListHarvestJobsRequestListHarvestJobsPaginateTypeDef definition

class ListHarvestJobsRequestListHarvestJobsPaginateTypeDef(TypedDict):
    IncludeChannelId: NotRequired[str],
    IncludeStatus: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef

```python
# ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef definition

class ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef(TypedDict):
    ChannelId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHarvestJobsResponseTypeDef

```python
# ListHarvestJobsResponseTypeDef definition

class ListHarvestJobsResponseTypeDef(TypedDict):
    HarvestJobs: List[HarvestJobTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HarvestJobTypeDef](./type_defs.md#harvestjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CmafEncryptionTypeDef

```python
# CmafEncryptionTypeDef definition

class CmafEncryptionTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderTypeDef,  # (2)
    ConstantInitializationVector: NotRequired[str],
    EncryptionMethod: NotRequired[CmafEncryptionMethodType],  # (1)
    KeyRotationIntervalSeconds: NotRequired[int],
```

1. See [:material-code-brackets: CmafEncryptionMethodType](./literals.md#cmafencryptionmethodtype) 
2. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
## DashEncryptionTypeDef

```python
# DashEncryptionTypeDef definition

class DashEncryptionTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderTypeDef,  # (1)
    KeyRotationIntervalSeconds: NotRequired[int],
```

1. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
## HlsEncryptionTypeDef

```python
# HlsEncryptionTypeDef definition

class HlsEncryptionTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderTypeDef,  # (2)
    ConstantInitializationVector: NotRequired[str],
    EncryptionMethod: NotRequired[EncryptionMethodType],  # (1)
    KeyRotationIntervalSeconds: NotRequired[int],
    RepeatExtXKey: NotRequired[bool],
```

1. See [:material-code-brackets: EncryptionMethodType](./literals.md#encryptionmethodtype) 
2. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
## MssEncryptionTypeDef

```python
# MssEncryptionTypeDef definition

class MssEncryptionTypeDef(TypedDict):
    SpekeKeyProvider: SpekeKeyProviderTypeDef,  # (1)
```

1. See [:material-code-braces: SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef) 
## ChannelTypeDef

```python
# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedAt: NotRequired[str],
    Description: NotRequired[str],
    EgressAccessLogs: NotRequired[EgressAccessLogsTypeDef],  # (1)
    HlsIngest: NotRequired[HlsIngestTypeDef],  # (2)
    Id: NotRequired[str],
    IngressAccessLogs: NotRequired[IngressAccessLogsTypeDef],  # (3)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
2. See [:material-code-braces: HlsIngestTypeDef](./type_defs.md#hlsingesttypedef) 
3. See [:material-code-braces: IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef) 
## ConfigureLogsResponseTypeDef

```python
# ConfigureLogsResponseTypeDef definition

class ConfigureLogsResponseTypeDef(TypedDict):
    Arn: str,
    CreatedAt: str,
    Description: str,
    EgressAccessLogs: EgressAccessLogsTypeDef,  # (1)
    HlsIngest: HlsIngestTypeDef,  # (2)
    Id: str,
    IngressAccessLogs: IngressAccessLogsTypeDef,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
2. See [:material-code-braces: HlsIngestTypeDef](./type_defs.md#hlsingesttypedef) 
3. See [:material-code-braces: IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelResponseTypeDef

```python
# CreateChannelResponseTypeDef definition

class CreateChannelResponseTypeDef(TypedDict):
    Arn: str,
    CreatedAt: str,
    Description: str,
    EgressAccessLogs: EgressAccessLogsTypeDef,  # (1)
    HlsIngest: HlsIngestTypeDef,  # (2)
    Id: str,
    IngressAccessLogs: IngressAccessLogsTypeDef,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
2. See [:material-code-braces: HlsIngestTypeDef](./type_defs.md#hlsingesttypedef) 
3. See [:material-code-braces: IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeChannelResponseTypeDef

```python
# DescribeChannelResponseTypeDef definition

class DescribeChannelResponseTypeDef(TypedDict):
    Arn: str,
    CreatedAt: str,
    Description: str,
    EgressAccessLogs: EgressAccessLogsTypeDef,  # (1)
    HlsIngest: HlsIngestTypeDef,  # (2)
    Id: str,
    IngressAccessLogs: IngressAccessLogsTypeDef,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
2. See [:material-code-braces: HlsIngestTypeDef](./type_defs.md#hlsingesttypedef) 
3. See [:material-code-braces: IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotateChannelCredentialsResponseTypeDef

```python
# RotateChannelCredentialsResponseTypeDef definition

class RotateChannelCredentialsResponseTypeDef(TypedDict):
    Arn: str,
    CreatedAt: str,
    Description: str,
    EgressAccessLogs: EgressAccessLogsTypeDef,  # (1)
    HlsIngest: HlsIngestTypeDef,  # (2)
    Id: str,
    IngressAccessLogs: IngressAccessLogsTypeDef,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
2. See [:material-code-braces: HlsIngestTypeDef](./type_defs.md#hlsingesttypedef) 
3. See [:material-code-braces: IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotateIngestEndpointCredentialsResponseTypeDef

```python
# RotateIngestEndpointCredentialsResponseTypeDef definition

class RotateIngestEndpointCredentialsResponseTypeDef(TypedDict):
    Arn: str,
    CreatedAt: str,
    Description: str,
    EgressAccessLogs: EgressAccessLogsTypeDef,  # (1)
    HlsIngest: HlsIngestTypeDef,  # (2)
    Id: str,
    IngressAccessLogs: IngressAccessLogsTypeDef,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
2. See [:material-code-braces: HlsIngestTypeDef](./type_defs.md#hlsingesttypedef) 
3. See [:material-code-braces: IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelResponseTypeDef

```python
# UpdateChannelResponseTypeDef definition

class UpdateChannelResponseTypeDef(TypedDict):
    Arn: str,
    CreatedAt: str,
    Description: str,
    EgressAccessLogs: EgressAccessLogsTypeDef,  # (1)
    HlsIngest: HlsIngestTypeDef,  # (2)
    Id: str,
    IngressAccessLogs: IngressAccessLogsTypeDef,  # (3)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef) 
2. See [:material-code-braces: HlsIngestTypeDef](./type_defs.md#hlsingesttypedef) 
3. See [:material-code-braces: IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CmafPackageCreateOrUpdateParametersTypeDef

```python
# CmafPackageCreateOrUpdateParametersTypeDef definition

class CmafPackageCreateOrUpdateParametersTypeDef(TypedDict):
    Encryption: NotRequired[CmafEncryptionTypeDef],  # (1)
    HlsManifests: NotRequired[Sequence[HlsManifestCreateOrUpdateParametersTypeDef]],  # (2)
    SegmentDurationSeconds: NotRequired[int],
    SegmentPrefix: NotRequired[str],
    StreamSelection: NotRequired[StreamSelectionTypeDef],  # (3)
```

1. See [:material-code-braces: CmafEncryptionTypeDef](./type_defs.md#cmafencryptiontypedef) 
2. See [:material-code-braces: HlsManifestCreateOrUpdateParametersTypeDef](./type_defs.md#hlsmanifestcreateorupdateparameterstypedef) 
3. See [:material-code-braces: StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef) 
## CmafPackageTypeDef

```python
# CmafPackageTypeDef definition

class CmafPackageTypeDef(TypedDict):
    Encryption: NotRequired[CmafEncryptionTypeDef],  # (1)
    HlsManifests: NotRequired[List[HlsManifestTypeDef]],  # (2)
    SegmentDurationSeconds: NotRequired[int],
    SegmentPrefix: NotRequired[str],
    StreamSelection: NotRequired[StreamSelectionTypeDef],  # (3)
```

1. See [:material-code-braces: CmafEncryptionTypeDef](./type_defs.md#cmafencryptiontypedef) 
2. See [:material-code-braces: HlsManifestTypeDef](./type_defs.md#hlsmanifesttypedef) 
3. See [:material-code-braces: StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef) 
## DashPackageTypeDef

```python
# DashPackageTypeDef definition

class DashPackageTypeDef(TypedDict):
    AdTriggers: NotRequired[Sequence[AdTriggersElementType]],  # (1)
    AdsOnDeliveryRestrictions: NotRequired[AdsOnDeliveryRestrictionsType],  # (2)
    Encryption: NotRequired[DashEncryptionTypeDef],  # (3)
    IncludeIframeOnlyStream: NotRequired[bool],
    ManifestLayout: NotRequired[ManifestLayoutType],  # (4)
    ManifestWindowSeconds: NotRequired[int],
    MinBufferTimeSeconds: NotRequired[int],
    MinUpdatePeriodSeconds: NotRequired[int],
    PeriodTriggers: NotRequired[Sequence[PeriodTriggersElementType]],  # (5)
    Profile: NotRequired[ProfileType],  # (6)
    SegmentDurationSeconds: NotRequired[int],
    SegmentTemplateFormat: NotRequired[SegmentTemplateFormatType],  # (7)
    StreamSelection: NotRequired[StreamSelectionTypeDef],  # (8)
    SuggestedPresentationDelaySeconds: NotRequired[int],
    UtcTiming: NotRequired[UtcTimingType],  # (9)
    UtcTimingUri: NotRequired[str],
```

1. See [:material-code-brackets: AdTriggersElementType](./literals.md#adtriggerselementtype) 
2. See [:material-code-brackets: AdsOnDeliveryRestrictionsType](./literals.md#adsondeliveryrestrictionstype) 
3. See [:material-code-braces: DashEncryptionTypeDef](./type_defs.md#dashencryptiontypedef) 
4. See [:material-code-brackets: ManifestLayoutType](./literals.md#manifestlayouttype) 
5. See [:material-code-brackets: PeriodTriggersElementType](./literals.md#periodtriggerselementtype) 
6. See [:material-code-brackets: ProfileType](./literals.md#profiletype) 
7. See [:material-code-brackets: SegmentTemplateFormatType](./literals.md#segmenttemplateformattype) 
8. See [:material-code-braces: StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef) 
9. See [:material-code-brackets: UtcTimingType](./literals.md#utctimingtype) 
## HlsPackageTypeDef

```python
# HlsPackageTypeDef definition

class HlsPackageTypeDef(TypedDict):
    AdMarkers: NotRequired[AdMarkersType],  # (1)
    AdTriggers: NotRequired[Sequence[AdTriggersElementType]],  # (2)
    AdsOnDeliveryRestrictions: NotRequired[AdsOnDeliveryRestrictionsType],  # (3)
    Encryption: NotRequired[HlsEncryptionTypeDef],  # (4)
    IncludeDvbSubtitles: NotRequired[bool],
    IncludeIframeOnlyStream: NotRequired[bool],
    PlaylistType: NotRequired[PlaylistTypeType],  # (5)
    PlaylistWindowSeconds: NotRequired[int],
    ProgramDateTimeIntervalSeconds: NotRequired[int],
    SegmentDurationSeconds: NotRequired[int],
    StreamSelection: NotRequired[StreamSelectionTypeDef],  # (6)
    UseAudioRenditionGroup: NotRequired[bool],
```

1. See [:material-code-brackets: AdMarkersType](./literals.md#admarkerstype) 
2. See [:material-code-brackets: AdTriggersElementType](./literals.md#adtriggerselementtype) 
3. See [:material-code-brackets: AdsOnDeliveryRestrictionsType](./literals.md#adsondeliveryrestrictionstype) 
4. See [:material-code-braces: HlsEncryptionTypeDef](./type_defs.md#hlsencryptiontypedef) 
5. See [:material-code-brackets: PlaylistTypeType](./literals.md#playlisttypetype) 
6. See [:material-code-braces: StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef) 
## MssPackageTypeDef

```python
# MssPackageTypeDef definition

class MssPackageTypeDef(TypedDict):
    Encryption: NotRequired[MssEncryptionTypeDef],  # (1)
    ManifestWindowSeconds: NotRequired[int],
    SegmentDurationSeconds: NotRequired[int],
    StreamSelection: NotRequired[StreamSelectionTypeDef],  # (2)
```

1. See [:material-code-braces: MssEncryptionTypeDef](./type_defs.md#mssencryptiontypedef) 
2. See [:material-code-braces: StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    Channels: List[ChannelTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOriginEndpointRequestRequestTypeDef

```python
# CreateOriginEndpointRequestRequestTypeDef definition

class CreateOriginEndpointRequestRequestTypeDef(TypedDict):
    ChannelId: str,
    Id: str,
    Authorization: NotRequired[AuthorizationTypeDef],  # (1)
    CmafPackage: NotRequired[CmafPackageCreateOrUpdateParametersTypeDef],  # (2)
    DashPackage: NotRequired[DashPackageTypeDef],  # (3)
    Description: NotRequired[str],
    HlsPackage: NotRequired[HlsPackageTypeDef],  # (4)
    ManifestName: NotRequired[str],
    MssPackage: NotRequired[MssPackageTypeDef],  # (5)
    Origination: NotRequired[OriginationType],  # (6)
    StartoverWindowSeconds: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
    TimeDelaySeconds: NotRequired[int],
    Whitelist: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: CmafPackageCreateOrUpdateParametersTypeDef](./type_defs.md#cmafpackagecreateorupdateparameterstypedef) 
3. See [:material-code-braces: DashPackageTypeDef](./type_defs.md#dashpackagetypedef) 
4. See [:material-code-braces: HlsPackageTypeDef](./type_defs.md#hlspackagetypedef) 
5. See [:material-code-braces: MssPackageTypeDef](./type_defs.md#msspackagetypedef) 
6. See [:material-code-brackets: OriginationType](./literals.md#originationtype) 
## CreateOriginEndpointResponseTypeDef

```python
# CreateOriginEndpointResponseTypeDef definition

class CreateOriginEndpointResponseTypeDef(TypedDict):
    Arn: str,
    Authorization: AuthorizationTypeDef,  # (1)
    ChannelId: str,
    CmafPackage: CmafPackageTypeDef,  # (2)
    CreatedAt: str,
    DashPackage: DashPackageTypeDef,  # (3)
    Description: str,
    HlsPackage: HlsPackageTypeDef,  # (4)
    Id: str,
    ManifestName: str,
    MssPackage: MssPackageTypeDef,  # (5)
    Origination: OriginationType,  # (6)
    StartoverWindowSeconds: int,
    Tags: Dict[str, str],
    TimeDelaySeconds: int,
    Url: str,
    Whitelist: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: CmafPackageTypeDef](./type_defs.md#cmafpackagetypedef) 
3. See [:material-code-braces: DashPackageTypeDef](./type_defs.md#dashpackagetypedef) 
4. See [:material-code-braces: HlsPackageTypeDef](./type_defs.md#hlspackagetypedef) 
5. See [:material-code-braces: MssPackageTypeDef](./type_defs.md#msspackagetypedef) 
6. See [:material-code-brackets: OriginationType](./literals.md#originationtype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOriginEndpointResponseTypeDef

```python
# DescribeOriginEndpointResponseTypeDef definition

class DescribeOriginEndpointResponseTypeDef(TypedDict):
    Arn: str,
    Authorization: AuthorizationTypeDef,  # (1)
    ChannelId: str,
    CmafPackage: CmafPackageTypeDef,  # (2)
    CreatedAt: str,
    DashPackage: DashPackageTypeDef,  # (3)
    Description: str,
    HlsPackage: HlsPackageTypeDef,  # (4)
    Id: str,
    ManifestName: str,
    MssPackage: MssPackageTypeDef,  # (5)
    Origination: OriginationType,  # (6)
    StartoverWindowSeconds: int,
    Tags: Dict[str, str],
    TimeDelaySeconds: int,
    Url: str,
    Whitelist: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: CmafPackageTypeDef](./type_defs.md#cmafpackagetypedef) 
3. See [:material-code-braces: DashPackageTypeDef](./type_defs.md#dashpackagetypedef) 
4. See [:material-code-braces: HlsPackageTypeDef](./type_defs.md#hlspackagetypedef) 
5. See [:material-code-braces: MssPackageTypeDef](./type_defs.md#msspackagetypedef) 
6. See [:material-code-brackets: OriginationType](./literals.md#originationtype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OriginEndpointTypeDef

```python
# OriginEndpointTypeDef definition

class OriginEndpointTypeDef(TypedDict):
    Arn: NotRequired[str],
    Authorization: NotRequired[AuthorizationTypeDef],  # (1)
    ChannelId: NotRequired[str],
    CmafPackage: NotRequired[CmafPackageTypeDef],  # (2)
    CreatedAt: NotRequired[str],
    DashPackage: NotRequired[DashPackageTypeDef],  # (3)
    Description: NotRequired[str],
    HlsPackage: NotRequired[HlsPackageTypeDef],  # (4)
    Id: NotRequired[str],
    ManifestName: NotRequired[str],
    MssPackage: NotRequired[MssPackageTypeDef],  # (5)
    Origination: NotRequired[OriginationType],  # (6)
    StartoverWindowSeconds: NotRequired[int],
    Tags: NotRequired[Dict[str, str]],
    TimeDelaySeconds: NotRequired[int],
    Url: NotRequired[str],
    Whitelist: NotRequired[List[str]],
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: CmafPackageTypeDef](./type_defs.md#cmafpackagetypedef) 
3. See [:material-code-braces: DashPackageTypeDef](./type_defs.md#dashpackagetypedef) 
4. See [:material-code-braces: HlsPackageTypeDef](./type_defs.md#hlspackagetypedef) 
5. See [:material-code-braces: MssPackageTypeDef](./type_defs.md#msspackagetypedef) 
6. See [:material-code-brackets: OriginationType](./literals.md#originationtype) 
## UpdateOriginEndpointRequestRequestTypeDef

```python
# UpdateOriginEndpointRequestRequestTypeDef definition

class UpdateOriginEndpointRequestRequestTypeDef(TypedDict):
    Id: str,
    Authorization: NotRequired[AuthorizationTypeDef],  # (1)
    CmafPackage: NotRequired[CmafPackageCreateOrUpdateParametersTypeDef],  # (2)
    DashPackage: NotRequired[DashPackageTypeDef],  # (3)
    Description: NotRequired[str],
    HlsPackage: NotRequired[HlsPackageTypeDef],  # (4)
    ManifestName: NotRequired[str],
    MssPackage: NotRequired[MssPackageTypeDef],  # (5)
    Origination: NotRequired[OriginationType],  # (6)
    StartoverWindowSeconds: NotRequired[int],
    TimeDelaySeconds: NotRequired[int],
    Whitelist: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: CmafPackageCreateOrUpdateParametersTypeDef](./type_defs.md#cmafpackagecreateorupdateparameterstypedef) 
3. See [:material-code-braces: DashPackageTypeDef](./type_defs.md#dashpackagetypedef) 
4. See [:material-code-braces: HlsPackageTypeDef](./type_defs.md#hlspackagetypedef) 
5. See [:material-code-braces: MssPackageTypeDef](./type_defs.md#msspackagetypedef) 
6. See [:material-code-brackets: OriginationType](./literals.md#originationtype) 
## UpdateOriginEndpointResponseTypeDef

```python
# UpdateOriginEndpointResponseTypeDef definition

class UpdateOriginEndpointResponseTypeDef(TypedDict):
    Arn: str,
    Authorization: AuthorizationTypeDef,  # (1)
    ChannelId: str,
    CmafPackage: CmafPackageTypeDef,  # (2)
    CreatedAt: str,
    DashPackage: DashPackageTypeDef,  # (3)
    Description: str,
    HlsPackage: HlsPackageTypeDef,  # (4)
    Id: str,
    ManifestName: str,
    MssPackage: MssPackageTypeDef,  # (5)
    Origination: OriginationType,  # (6)
    StartoverWindowSeconds: int,
    Tags: Dict[str, str],
    TimeDelaySeconds: int,
    Url: str,
    Whitelist: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: AuthorizationTypeDef](./type_defs.md#authorizationtypedef) 
2. See [:material-code-braces: CmafPackageTypeDef](./type_defs.md#cmafpackagetypedef) 
3. See [:material-code-braces: DashPackageTypeDef](./type_defs.md#dashpackagetypedef) 
4. See [:material-code-braces: HlsPackageTypeDef](./type_defs.md#hlspackagetypedef) 
5. See [:material-code-braces: MssPackageTypeDef](./type_defs.md#msspackagetypedef) 
6. See [:material-code-brackets: OriginationType](./literals.md#originationtype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOriginEndpointsResponseTypeDef

```python
# ListOriginEndpointsResponseTypeDef definition

class ListOriginEndpointsResponseTypeDef(TypedDict):
    NextToken: str,
    OriginEndpoints: List[OriginEndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OriginEndpointTypeDef](./type_defs.md#originendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
