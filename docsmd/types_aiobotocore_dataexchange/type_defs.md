# Type definitions

> [Index](../README.md) > [DataExchange](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#DataExchange)
    type annotations stubs module [types-aiobotocore-dataexchange](https://pypi.org/project/types-aiobotocore-dataexchange/).



## ApiGatewayApiAssetTypeDef

```python
# ApiGatewayApiAssetTypeDef definition

class ApiGatewayApiAssetTypeDef(TypedDict):
    ApiDescription: NotRequired[str],
    ApiEndpoint: NotRequired[str],
    ApiId: NotRequired[str],
    ApiKey: NotRequired[str],
    ApiName: NotRequired[str],
    ApiSpecificationDownloadUrl: NotRequired[str],
    ApiSpecificationDownloadUrlExpiresAt: NotRequired[datetime],
    ProtocolType: NotRequired[ProtocolTypeType],  # (1)
    Stage: NotRequired[str],
```

1. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
## AssetDestinationEntryTypeDef

```python
# AssetDestinationEntryTypeDef definition

class AssetDestinationEntryTypeDef(TypedDict):
    AssetId: str,
    Bucket: str,
    Key: NotRequired[str],
```

## RedshiftDataShareAssetTypeDef

```python
# RedshiftDataShareAssetTypeDef definition

class RedshiftDataShareAssetTypeDef(TypedDict):
    Arn: str,
```

## S3SnapshotAssetTypeDef

```python
# S3SnapshotAssetTypeDef definition

class S3SnapshotAssetTypeDef(TypedDict):
    Size: float,
```

## AssetSourceEntryTypeDef

```python
# AssetSourceEntryTypeDef definition

class AssetSourceEntryTypeDef(TypedDict):
    Bucket: str,
    Key: str,
```

## AutoExportRevisionDestinationEntryTypeDef

```python
# AutoExportRevisionDestinationEntryTypeDef definition

class AutoExportRevisionDestinationEntryTypeDef(TypedDict):
    Bucket: str,
    KeyPattern: NotRequired[str],
```

## ExportServerSideEncryptionTypeDef

```python
# ExportServerSideEncryptionTypeDef definition

class ExportServerSideEncryptionTypeDef(TypedDict):
    Type: ServerSideEncryptionTypesType,  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: ServerSideEncryptionTypesType](./literals.md#serversideencryptiontypestype) 
## CancelJobRequestRequestTypeDef

```python
# CancelJobRequestRequestTypeDef definition

class CancelJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## CreateDataSetRequestRequestTypeDef

```python
# CreateDataSetRequestRequestTypeDef definition

class CreateDataSetRequestRequestTypeDef(TypedDict):
    AssetType: AssetTypeType,  # (1)
    Description: str,
    Name: str,
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
## OriginDetailsTypeDef

```python
# OriginDetailsTypeDef definition

class OriginDetailsTypeDef(TypedDict):
    ProductId: str,
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

## CreateRevisionRequestRequestTypeDef

```python
# CreateRevisionRequestRequestTypeDef definition

class CreateRevisionRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    Comment: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## LFTagTypeDef

```python
# LFTagTypeDef definition

class LFTagTypeDef(TypedDict):
    TagKey: str,
    TagValues: Sequence[str],
```

## DeleteAssetRequestRequestTypeDef

```python
# DeleteAssetRequestRequestTypeDef definition

class DeleteAssetRequestRequestTypeDef(TypedDict):
    AssetId: str,
    DataSetId: str,
    RevisionId: str,
```

## DeleteDataSetRequestRequestTypeDef

```python
# DeleteDataSetRequestRequestTypeDef definition

class DeleteDataSetRequestRequestTypeDef(TypedDict):
    DataSetId: str,
```

## DeleteEventActionRequestRequestTypeDef

```python
# DeleteEventActionRequestRequestTypeDef definition

class DeleteEventActionRequestRequestTypeDef(TypedDict):
    EventActionId: str,
```

## DeleteRevisionRequestRequestTypeDef

```python
# DeleteRevisionRequestRequestTypeDef definition

class DeleteRevisionRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    RevisionId: str,
```

## ImportAssetFromSignedUrlJobErrorDetailsTypeDef

```python
# ImportAssetFromSignedUrlJobErrorDetailsTypeDef definition

class ImportAssetFromSignedUrlJobErrorDetailsTypeDef(TypedDict):
    AssetName: str,
```

## RevisionPublishedTypeDef

```python
# RevisionPublishedTypeDef definition

class RevisionPublishedTypeDef(TypedDict):
    DataSetId: str,
```

## ExportAssetToSignedUrlRequestDetailsTypeDef

```python
# ExportAssetToSignedUrlRequestDetailsTypeDef definition

class ExportAssetToSignedUrlRequestDetailsTypeDef(TypedDict):
    AssetId: str,
    DataSetId: str,
    RevisionId: str,
```

## ExportAssetToSignedUrlResponseDetailsTypeDef

```python
# ExportAssetToSignedUrlResponseDetailsTypeDef definition

class ExportAssetToSignedUrlResponseDetailsTypeDef(TypedDict):
    AssetId: str,
    DataSetId: str,
    RevisionId: str,
    SignedUrl: NotRequired[str],
    SignedUrlExpiresAt: NotRequired[datetime],
```

## RevisionDestinationEntryTypeDef

```python
# RevisionDestinationEntryTypeDef definition

class RevisionDestinationEntryTypeDef(TypedDict):
    Bucket: str,
    RevisionId: str,
    KeyPattern: NotRequired[str],
```

## GetAssetRequestRequestTypeDef

```python
# GetAssetRequestRequestTypeDef definition

class GetAssetRequestRequestTypeDef(TypedDict):
    AssetId: str,
    DataSetId: str,
    RevisionId: str,
```

## GetDataSetRequestRequestTypeDef

```python
# GetDataSetRequestRequestTypeDef definition

class GetDataSetRequestRequestTypeDef(TypedDict):
    DataSetId: str,
```

## GetEventActionRequestRequestTypeDef

```python
# GetEventActionRequestRequestTypeDef definition

class GetEventActionRequestRequestTypeDef(TypedDict):
    EventActionId: str,
```

## GetJobRequestRequestTypeDef

```python
# GetJobRequestRequestTypeDef definition

class GetJobRequestRequestTypeDef(TypedDict):
    JobId: str,
```

## GetRevisionRequestRequestTypeDef

```python
# GetRevisionRequestRequestTypeDef definition

class GetRevisionRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    RevisionId: str,
```

## ImportAssetFromApiGatewayApiRequestDetailsTypeDef

```python
# ImportAssetFromApiGatewayApiRequestDetailsTypeDef definition

class ImportAssetFromApiGatewayApiRequestDetailsTypeDef(TypedDict):
    ApiId: str,
    ApiName: str,
    ApiSpecificationMd5Hash: str,
    DataSetId: str,
    ProtocolType: ProtocolTypeType,  # (1)
    RevisionId: str,
    Stage: str,
    ApiDescription: NotRequired[str],
    ApiKey: NotRequired[str],
```

1. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
## ImportAssetFromApiGatewayApiResponseDetailsTypeDef

```python
# ImportAssetFromApiGatewayApiResponseDetailsTypeDef definition

class ImportAssetFromApiGatewayApiResponseDetailsTypeDef(TypedDict):
    ApiId: str,
    ApiName: str,
    ApiSpecificationMd5Hash: str,
    ApiSpecificationUploadUrl: str,
    ApiSpecificationUploadUrlExpiresAt: datetime,
    DataSetId: str,
    ProtocolType: ProtocolTypeType,  # (1)
    RevisionId: str,
    Stage: str,
    ApiDescription: NotRequired[str],
    ApiKey: NotRequired[str],
```

1. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
## ImportAssetFromSignedUrlRequestDetailsTypeDef

```python
# ImportAssetFromSignedUrlRequestDetailsTypeDef definition

class ImportAssetFromSignedUrlRequestDetailsTypeDef(TypedDict):
    AssetName: str,
    DataSetId: str,
    Md5Hash: str,
    RevisionId: str,
```

## ImportAssetFromSignedUrlResponseDetailsTypeDef

```python
# ImportAssetFromSignedUrlResponseDetailsTypeDef definition

class ImportAssetFromSignedUrlResponseDetailsTypeDef(TypedDict):
    AssetName: str,
    DataSetId: str,
    RevisionId: str,
    Md5Hash: NotRequired[str],
    SignedUrl: NotRequired[str],
    SignedUrlExpiresAt: NotRequired[datetime],
```

## RedshiftDataShareAssetSourceEntryTypeDef

```python
# RedshiftDataShareAssetSourceEntryTypeDef definition

class RedshiftDataShareAssetSourceEntryTypeDef(TypedDict):
    DataShareArn: str,
```

## KmsKeyToGrantTypeDef

```python
# KmsKeyToGrantTypeDef definition

class KmsKeyToGrantTypeDef(TypedDict):
    KmsKeyArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDataSetRevisionsRequestRequestTypeDef

```python
# ListDataSetRevisionsRequestRequestTypeDef definition

class ListDataSetRevisionsRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## RevisionEntryTypeDef

```python
# RevisionEntryTypeDef definition

class RevisionEntryTypeDef(TypedDict):
    Arn: str,
    CreatedAt: datetime,
    DataSetId: str,
    Id: str,
    UpdatedAt: datetime,
    Comment: NotRequired[str],
    Finalized: NotRequired[bool],
    SourceId: NotRequired[str],
    RevocationComment: NotRequired[str],
    Revoked: NotRequired[bool],
    RevokedAt: NotRequired[datetime],
```

## ListDataSetsRequestRequestTypeDef

```python
# ListDataSetsRequestRequestTypeDef definition

class ListDataSetsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Origin: NotRequired[str],
```

## ListEventActionsRequestRequestTypeDef

```python
# ListEventActionsRequestRequestTypeDef definition

class ListEventActionsRequestRequestTypeDef(TypedDict):
    EventSourceId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    DataSetId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    RevisionId: NotRequired[str],
```

## ListRevisionAssetsRequestRequestTypeDef

```python
# ListRevisionAssetsRequestRequestTypeDef definition

class ListRevisionAssetsRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    RevisionId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## RevokeRevisionRequestRequestTypeDef

```python
# RevokeRevisionRequestRequestTypeDef definition

class RevokeRevisionRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    RevisionId: str,
    RevocationComment: str,
```

## SendApiAssetRequestRequestTypeDef

```python
# SendApiAssetRequestRequestTypeDef definition

class SendApiAssetRequestRequestTypeDef(TypedDict):
    AssetId: str,
    DataSetId: str,
    RevisionId: str,
    Body: NotRequired[str],
    QueryStringParameters: NotRequired[Mapping[str, str]],
    RequestHeaders: NotRequired[Mapping[str, str]],
    Method: NotRequired[str],
    Path: NotRequired[str],
```

## StartJobRequestRequestTypeDef

```python
# StartJobRequestRequestTypeDef definition

class StartJobRequestRequestTypeDef(TypedDict):
    JobId: str,
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

## UpdateAssetRequestRequestTypeDef

```python
# UpdateAssetRequestRequestTypeDef definition

class UpdateAssetRequestRequestTypeDef(TypedDict):
    AssetId: str,
    DataSetId: str,
    Name: str,
    RevisionId: str,
```

## UpdateDataSetRequestRequestTypeDef

```python
# UpdateDataSetRequestRequestTypeDef definition

class UpdateDataSetRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    Description: NotRequired[str],
    Name: NotRequired[str],
```

## UpdateRevisionRequestRequestTypeDef

```python
# UpdateRevisionRequestRequestTypeDef definition

class UpdateRevisionRequestRequestTypeDef(TypedDict):
    DataSetId: str,
    RevisionId: str,
    Comment: NotRequired[str],
    Finalized: NotRequired[bool],
```

## ImportAssetsFromS3RequestDetailsTypeDef

```python
# ImportAssetsFromS3RequestDetailsTypeDef definition

class ImportAssetsFromS3RequestDetailsTypeDef(TypedDict):
    AssetSources: Sequence[AssetSourceEntryTypeDef],  # (1)
    DataSetId: str,
    RevisionId: str,
```

1. See [:material-code-braces: AssetSourceEntryTypeDef](./type_defs.md#assetsourceentrytypedef) 
## ImportAssetsFromS3ResponseDetailsTypeDef

```python
# ImportAssetsFromS3ResponseDetailsTypeDef definition

class ImportAssetsFromS3ResponseDetailsTypeDef(TypedDict):
    AssetSources: List[AssetSourceEntryTypeDef],  # (1)
    DataSetId: str,
    RevisionId: str,
```

1. See [:material-code-braces: AssetSourceEntryTypeDef](./type_defs.md#assetsourceentrytypedef) 
## AutoExportRevisionToS3RequestDetailsTypeDef

```python
# AutoExportRevisionToS3RequestDetailsTypeDef definition

class AutoExportRevisionToS3RequestDetailsTypeDef(TypedDict):
    RevisionDestination: AutoExportRevisionDestinationEntryTypeDef,  # (2)
    Encryption: NotRequired[ExportServerSideEncryptionTypeDef],  # (1)
```

1. See [:material-code-braces: ExportServerSideEncryptionTypeDef](./type_defs.md#exportserversideencryptiontypedef) 
2. See [:material-code-braces: AutoExportRevisionDestinationEntryTypeDef](./type_defs.md#autoexportrevisiondestinationentrytypedef) 
## ExportAssetsToS3RequestDetailsTypeDef

```python
# ExportAssetsToS3RequestDetailsTypeDef definition

class ExportAssetsToS3RequestDetailsTypeDef(TypedDict):
    AssetDestinations: Sequence[AssetDestinationEntryTypeDef],  # (1)
    DataSetId: str,
    RevisionId: str,
    Encryption: NotRequired[ExportServerSideEncryptionTypeDef],  # (2)
```

1. See [:material-code-braces: AssetDestinationEntryTypeDef](./type_defs.md#assetdestinationentrytypedef) 
2. See [:material-code-braces: ExportServerSideEncryptionTypeDef](./type_defs.md#exportserversideencryptiontypedef) 
## ExportAssetsToS3ResponseDetailsTypeDef

```python
# ExportAssetsToS3ResponseDetailsTypeDef definition

class ExportAssetsToS3ResponseDetailsTypeDef(TypedDict):
    AssetDestinations: List[AssetDestinationEntryTypeDef],  # (1)
    DataSetId: str,
    RevisionId: str,
    Encryption: NotRequired[ExportServerSideEncryptionTypeDef],  # (2)
```

1. See [:material-code-braces: AssetDestinationEntryTypeDef](./type_defs.md#assetdestinationentrytypedef) 
2. See [:material-code-braces: ExportServerSideEncryptionTypeDef](./type_defs.md#exportserversideencryptiontypedef) 
## DataSetEntryTypeDef

```python
# DataSetEntryTypeDef definition

class DataSetEntryTypeDef(TypedDict):
    Arn: str,
    AssetType: AssetTypeType,  # (1)
    CreatedAt: datetime,
    Description: str,
    Id: str,
    Name: str,
    Origin: OriginType,  # (2)
    UpdatedAt: datetime,
    OriginDetails: NotRequired[OriginDetailsTypeDef],  # (3)
    SourceId: NotRequired[str],
```

1. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
2. See [:material-code-brackets: OriginType](./literals.md#origintype) 
3. See [:material-code-braces: OriginDetailsTypeDef](./type_defs.md#origindetailstypedef) 
## CreateDataSetResponseTypeDef

```python
# CreateDataSetResponseTypeDef definition

class CreateDataSetResponseTypeDef(TypedDict):
    Arn: str,
    AssetType: AssetTypeType,  # (1)
    CreatedAt: datetime,
    Description: str,
    Id: str,
    Name: str,
    Origin: OriginType,  # (2)
    OriginDetails: OriginDetailsTypeDef,  # (3)
    SourceId: str,
    Tags: Dict[str, str],
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
2. See [:material-code-brackets: OriginType](./literals.md#origintype) 
3. See [:material-code-braces: OriginDetailsTypeDef](./type_defs.md#origindetailstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRevisionResponseTypeDef

```python
# CreateRevisionResponseTypeDef definition

class CreateRevisionResponseTypeDef(TypedDict):
    Arn: str,
    Comment: str,
    CreatedAt: datetime,
    DataSetId: str,
    Finalized: bool,
    Id: str,
    SourceId: str,
    Tags: Dict[str, str],
    UpdatedAt: datetime,
    RevocationComment: str,
    Revoked: bool,
    RevokedAt: datetime,
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
## GetDataSetResponseTypeDef

```python
# GetDataSetResponseTypeDef definition

class GetDataSetResponseTypeDef(TypedDict):
    Arn: str,
    AssetType: AssetTypeType,  # (1)
    CreatedAt: datetime,
    Description: str,
    Id: str,
    Name: str,
    Origin: OriginType,  # (2)
    OriginDetails: OriginDetailsTypeDef,  # (3)
    SourceId: str,
    Tags: Dict[str, str],
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
2. See [:material-code-brackets: OriginType](./literals.md#origintype) 
3. See [:material-code-braces: OriginDetailsTypeDef](./type_defs.md#origindetailstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRevisionResponseTypeDef

```python
# GetRevisionResponseTypeDef definition

class GetRevisionResponseTypeDef(TypedDict):
    Arn: str,
    Comment: str,
    CreatedAt: datetime,
    DataSetId: str,
    Finalized: bool,
    Id: str,
    SourceId: str,
    Tags: Dict[str, str],
    UpdatedAt: datetime,
    RevocationComment: str,
    Revoked: bool,
    RevokedAt: datetime,
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
## RevokeRevisionResponseTypeDef

```python
# RevokeRevisionResponseTypeDef definition

class RevokeRevisionResponseTypeDef(TypedDict):
    Arn: str,
    Comment: str,
    CreatedAt: datetime,
    DataSetId: str,
    Finalized: bool,
    Id: str,
    SourceId: str,
    UpdatedAt: datetime,
    RevocationComment: str,
    Revoked: bool,
    RevokedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendApiAssetResponseTypeDef

```python
# SendApiAssetResponseTypeDef definition

class SendApiAssetResponseTypeDef(TypedDict):
    Body: str,
    ResponseHeaders: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataSetResponseTypeDef

```python
# UpdateDataSetResponseTypeDef definition

class UpdateDataSetResponseTypeDef(TypedDict):
    Arn: str,
    AssetType: AssetTypeType,  # (1)
    CreatedAt: datetime,
    Description: str,
    Id: str,
    Name: str,
    Origin: OriginType,  # (2)
    OriginDetails: OriginDetailsTypeDef,  # (3)
    SourceId: str,
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
2. See [:material-code-brackets: OriginType](./literals.md#origintype) 
3. See [:material-code-braces: OriginDetailsTypeDef](./type_defs.md#origindetailstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRevisionResponseTypeDef

```python
# UpdateRevisionResponseTypeDef definition

class UpdateRevisionResponseTypeDef(TypedDict):
    Arn: str,
    Comment: str,
    CreatedAt: datetime,
    DataSetId: str,
    Finalized: bool,
    Id: str,
    SourceId: str,
    UpdatedAt: datetime,
    RevocationComment: str,
    Revoked: bool,
    RevokedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatabaseLFTagPolicyAndPermissionsTypeDef

```python
# DatabaseLFTagPolicyAndPermissionsTypeDef definition

class DatabaseLFTagPolicyAndPermissionsTypeDef(TypedDict):
    Expression: Sequence[LFTagTypeDef],  # (1)
    Permissions: Sequence[DatabaseLFTagPolicyPermissionType],  # (2)
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
2. See [:material-code-brackets: DatabaseLFTagPolicyPermissionType](./literals.md#databaselftagpolicypermissiontype) 
## DatabaseLFTagPolicyTypeDef

```python
# DatabaseLFTagPolicyTypeDef definition

class DatabaseLFTagPolicyTypeDef(TypedDict):
    Expression: List[LFTagTypeDef],  # (1)
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
## TableLFTagPolicyAndPermissionsTypeDef

```python
# TableLFTagPolicyAndPermissionsTypeDef definition

class TableLFTagPolicyAndPermissionsTypeDef(TypedDict):
    Expression: Sequence[LFTagTypeDef],  # (1)
    Permissions: Sequence[TableTagPolicyLFPermissionType],  # (2)
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
2. See [:material-code-brackets: TableTagPolicyLFPermissionType](./literals.md#tabletagpolicylfpermissiontype) 
## TableLFTagPolicyTypeDef

```python
# TableLFTagPolicyTypeDef definition

class TableLFTagPolicyTypeDef(TypedDict):
    Expression: List[LFTagTypeDef],  # (1)
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
## DetailsTypeDef

```python
# DetailsTypeDef definition

class DetailsTypeDef(TypedDict):
    ImportAssetFromSignedUrlJobErrorDetails: NotRequired[ImportAssetFromSignedUrlJobErrorDetailsTypeDef],  # (1)
    ImportAssetsFromS3JobErrorDetails: NotRequired[List[AssetSourceEntryTypeDef]],  # (2)
```

1. See [:material-code-braces: ImportAssetFromSignedUrlJobErrorDetailsTypeDef](./type_defs.md#importassetfromsignedurljoberrordetailstypedef) 
2. See [:material-code-braces: AssetSourceEntryTypeDef](./type_defs.md#assetsourceentrytypedef) 
## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    RevisionPublished: NotRequired[RevisionPublishedTypeDef],  # (1)
```

1. See [:material-code-braces: RevisionPublishedTypeDef](./type_defs.md#revisionpublishedtypedef) 
## ExportRevisionsToS3RequestDetailsTypeDef

```python
# ExportRevisionsToS3RequestDetailsTypeDef definition

class ExportRevisionsToS3RequestDetailsTypeDef(TypedDict):
    DataSetId: str,
    RevisionDestinations: Sequence[RevisionDestinationEntryTypeDef],  # (2)
    Encryption: NotRequired[ExportServerSideEncryptionTypeDef],  # (1)
```

1. See [:material-code-braces: ExportServerSideEncryptionTypeDef](./type_defs.md#exportserversideencryptiontypedef) 
2. See [:material-code-braces: RevisionDestinationEntryTypeDef](./type_defs.md#revisiondestinationentrytypedef) 
## ExportRevisionsToS3ResponseDetailsTypeDef

```python
# ExportRevisionsToS3ResponseDetailsTypeDef definition

class ExportRevisionsToS3ResponseDetailsTypeDef(TypedDict):
    DataSetId: str,
    RevisionDestinations: List[RevisionDestinationEntryTypeDef],  # (2)
    Encryption: NotRequired[ExportServerSideEncryptionTypeDef],  # (1)
    EventActionArn: NotRequired[str],
```

1. See [:material-code-braces: ExportServerSideEncryptionTypeDef](./type_defs.md#exportserversideencryptiontypedef) 
2. See [:material-code-braces: RevisionDestinationEntryTypeDef](./type_defs.md#revisiondestinationentrytypedef) 
## ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef

```python
# ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef definition

class ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef(TypedDict):
    AssetSources: Sequence[RedshiftDataShareAssetSourceEntryTypeDef],  # (1)
    DataSetId: str,
    RevisionId: str,
```

1. See [:material-code-braces: RedshiftDataShareAssetSourceEntryTypeDef](./type_defs.md#redshiftdatashareassetsourceentrytypedef) 
## ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef

```python
# ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef definition

class ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef(TypedDict):
    AssetSources: List[RedshiftDataShareAssetSourceEntryTypeDef],  # (1)
    DataSetId: str,
    RevisionId: str,
```

1. See [:material-code-braces: RedshiftDataShareAssetSourceEntryTypeDef](./type_defs.md#redshiftdatashareassetsourceentrytypedef) 
## S3DataAccessAssetSourceEntryTypeDef

```python
# S3DataAccessAssetSourceEntryTypeDef definition

class S3DataAccessAssetSourceEntryTypeDef(TypedDict):
    Bucket: str,
    KeyPrefixes: NotRequired[Sequence[str]],
    Keys: NotRequired[Sequence[str]],
    KmsKeysToGrant: NotRequired[Sequence[KmsKeyToGrantTypeDef]],  # (1)
```

1. See [:material-code-braces: KmsKeyToGrantTypeDef](./type_defs.md#kmskeytogranttypedef) 
## S3DataAccessAssetTypeDef

```python
# S3DataAccessAssetTypeDef definition

class S3DataAccessAssetTypeDef(TypedDict):
    Bucket: str,
    KeyPrefixes: NotRequired[List[str]],
    Keys: NotRequired[List[str]],
    S3AccessPointAlias: NotRequired[str],
    S3AccessPointArn: NotRequired[str],
    KmsKeysToGrant: NotRequired[List[KmsKeyToGrantTypeDef]],  # (1)
```

1. See [:material-code-braces: KmsKeyToGrantTypeDef](./type_defs.md#kmskeytogranttypedef) 
## ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef

```python
# ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef definition

class ListDataSetRevisionsRequestListDataSetRevisionsPaginateTypeDef(TypedDict):
    DataSetId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSetsRequestListDataSetsPaginateTypeDef

```python
# ListDataSetsRequestListDataSetsPaginateTypeDef definition

class ListDataSetsRequestListDataSetsPaginateTypeDef(TypedDict):
    Origin: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEventActionsRequestListEventActionsPaginateTypeDef

```python
# ListEventActionsRequestListEventActionsPaginateTypeDef definition

class ListEventActionsRequestListEventActionsPaginateTypeDef(TypedDict):
    EventSourceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestListJobsPaginateTypeDef

```python
# ListJobsRequestListJobsPaginateTypeDef definition

class ListJobsRequestListJobsPaginateTypeDef(TypedDict):
    DataSetId: NotRequired[str],
    RevisionId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef

```python
# ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef definition

class ListRevisionAssetsRequestListRevisionAssetsPaginateTypeDef(TypedDict):
    DataSetId: str,
    RevisionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSetRevisionsResponseTypeDef

```python
# ListDataSetRevisionsResponseTypeDef definition

class ListDataSetRevisionsResponseTypeDef(TypedDict):
    NextToken: str,
    Revisions: List[RevisionEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RevisionEntryTypeDef](./type_defs.md#revisionentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    ExportRevisionToS3: NotRequired[AutoExportRevisionToS3RequestDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: AutoExportRevisionToS3RequestDetailsTypeDef](./type_defs.md#autoexportrevisiontos3requestdetailstypedef) 
## ListDataSetsResponseTypeDef

```python
# ListDataSetsResponseTypeDef definition

class ListDataSetsResponseTypeDef(TypedDict):
    DataSets: List[DataSetEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSetEntryTypeDef](./type_defs.md#datasetentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef

```python
# ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef definition

class ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef(TypedDict):
    CatalogId: str,
    RoleArn: str,
    DataSetId: str,
    RevisionId: str,
    Database: NotRequired[DatabaseLFTagPolicyAndPermissionsTypeDef],  # (1)
    Table: NotRequired[TableLFTagPolicyAndPermissionsTypeDef],  # (2)
```

1. See [:material-code-braces: DatabaseLFTagPolicyAndPermissionsTypeDef](./type_defs.md#databaselftagpolicyandpermissionstypedef) 
2. See [:material-code-braces: TableLFTagPolicyAndPermissionsTypeDef](./type_defs.md#tablelftagpolicyandpermissionstypedef) 
## ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef

```python
# ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef definition

class ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef(TypedDict):
    CatalogId: str,
    RoleArn: str,
    DataSetId: str,
    RevisionId: str,
    Database: NotRequired[DatabaseLFTagPolicyAndPermissionsTypeDef],  # (1)
    Table: NotRequired[TableLFTagPolicyAndPermissionsTypeDef],  # (2)
```

1. See [:material-code-braces: DatabaseLFTagPolicyAndPermissionsTypeDef](./type_defs.md#databaselftagpolicyandpermissionstypedef) 
2. See [:material-code-braces: TableLFTagPolicyAndPermissionsTypeDef](./type_defs.md#tablelftagpolicyandpermissionstypedef) 
## LFResourceDetailsTypeDef

```python
# LFResourceDetailsTypeDef definition

class LFResourceDetailsTypeDef(TypedDict):
    Database: NotRequired[DatabaseLFTagPolicyTypeDef],  # (1)
    Table: NotRequired[TableLFTagPolicyTypeDef],  # (2)
```

1. See [:material-code-braces: DatabaseLFTagPolicyTypeDef](./type_defs.md#databaselftagpolicytypedef) 
2. See [:material-code-braces: TableLFTagPolicyTypeDef](./type_defs.md#tablelftagpolicytypedef) 
## JobErrorTypeDef

```python
# JobErrorTypeDef definition

class JobErrorTypeDef(TypedDict):
    Code: CodeType,  # (1)
    Message: str,
    Details: NotRequired[DetailsTypeDef],  # (2)
    LimitName: NotRequired[JobErrorLimitNameType],  # (3)
    LimitValue: NotRequired[float],
    ResourceId: NotRequired[str],
    ResourceType: NotRequired[JobErrorResourceTypesType],  # (4)
```

1. See [:material-code-brackets: CodeType](./literals.md#codetype) 
2. See [:material-code-braces: DetailsTypeDef](./type_defs.md#detailstypedef) 
3. See [:material-code-brackets: JobErrorLimitNameType](./literals.md#joberrorlimitnametype) 
4. See [:material-code-brackets: JobErrorResourceTypesType](./literals.md#joberrorresourcetypestype) 
## CreateS3DataAccessFromS3BucketRequestDetailsTypeDef

```python
# CreateS3DataAccessFromS3BucketRequestDetailsTypeDef definition

class CreateS3DataAccessFromS3BucketRequestDetailsTypeDef(TypedDict):
    AssetSource: S3DataAccessAssetSourceEntryTypeDef,  # (1)
    DataSetId: str,
    RevisionId: str,
```

1. See [:material-code-braces: S3DataAccessAssetSourceEntryTypeDef](./type_defs.md#s3dataaccessassetsourceentrytypedef) 
## CreateS3DataAccessFromS3BucketResponseDetailsTypeDef

```python
# CreateS3DataAccessFromS3BucketResponseDetailsTypeDef definition

class CreateS3DataAccessFromS3BucketResponseDetailsTypeDef(TypedDict):
    AssetSource: S3DataAccessAssetSourceEntryTypeDef,  # (1)
    DataSetId: str,
    RevisionId: str,
```

1. See [:material-code-braces: S3DataAccessAssetSourceEntryTypeDef](./type_defs.md#s3dataaccessassetsourceentrytypedef) 
## CreateEventActionRequestRequestTypeDef

```python
# CreateEventActionRequestRequestTypeDef definition

class CreateEventActionRequestRequestTypeDef(TypedDict):
    Action: ActionTypeDef,  # (1)
    Event: EventTypeDef,  # (2)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
## CreateEventActionResponseTypeDef

```python
# CreateEventActionResponseTypeDef definition

class CreateEventActionResponseTypeDef(TypedDict):
    Action: ActionTypeDef,  # (1)
    Arn: str,
    CreatedAt: datetime,
    Event: EventTypeDef,  # (2)
    Id: str,
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventActionEntryTypeDef

```python
# EventActionEntryTypeDef definition

class EventActionEntryTypeDef(TypedDict):
    Action: ActionTypeDef,  # (1)
    Arn: str,
    CreatedAt: datetime,
    Event: EventTypeDef,  # (2)
    Id: str,
    UpdatedAt: datetime,
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
## GetEventActionResponseTypeDef

```python
# GetEventActionResponseTypeDef definition

class GetEventActionResponseTypeDef(TypedDict):
    Action: ActionTypeDef,  # (1)
    Arn: str,
    CreatedAt: datetime,
    Event: EventTypeDef,  # (2)
    Id: str,
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEventActionRequestRequestTypeDef

```python
# UpdateEventActionRequestRequestTypeDef definition

class UpdateEventActionRequestRequestTypeDef(TypedDict):
    EventActionId: str,
    Action: NotRequired[ActionTypeDef],  # (1)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## UpdateEventActionResponseTypeDef

```python
# UpdateEventActionResponseTypeDef definition

class UpdateEventActionResponseTypeDef(TypedDict):
    Action: ActionTypeDef,  # (1)
    Arn: str,
    CreatedAt: datetime,
    Event: EventTypeDef,  # (2)
    Id: str,
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LFTagPolicyDetailsTypeDef

```python
# LFTagPolicyDetailsTypeDef definition

class LFTagPolicyDetailsTypeDef(TypedDict):
    CatalogId: str,
    ResourceType: LFResourceTypeType,  # (1)
    ResourceDetails: LFResourceDetailsTypeDef,  # (2)
```

1. See [:material-code-brackets: LFResourceTypeType](./literals.md#lfresourcetypetype) 
2. See [:material-code-braces: LFResourceDetailsTypeDef](./type_defs.md#lfresourcedetailstypedef) 
## RequestDetailsTypeDef

```python
# RequestDetailsTypeDef definition

class RequestDetailsTypeDef(TypedDict):
    ExportAssetToSignedUrl: NotRequired[ExportAssetToSignedUrlRequestDetailsTypeDef],  # (1)
    ExportAssetsToS3: NotRequired[ExportAssetsToS3RequestDetailsTypeDef],  # (2)
    ExportRevisionsToS3: NotRequired[ExportRevisionsToS3RequestDetailsTypeDef],  # (3)
    ImportAssetFromSignedUrl: NotRequired[ImportAssetFromSignedUrlRequestDetailsTypeDef],  # (4)
    ImportAssetsFromS3: NotRequired[ImportAssetsFromS3RequestDetailsTypeDef],  # (5)
    ImportAssetsFromRedshiftDataShares: NotRequired[ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef],  # (6)
    ImportAssetFromApiGatewayApi: NotRequired[ImportAssetFromApiGatewayApiRequestDetailsTypeDef],  # (7)
    CreateS3DataAccessFromS3Bucket: NotRequired[CreateS3DataAccessFromS3BucketRequestDetailsTypeDef],  # (8)
    ImportAssetsFromLakeFormationTagPolicy: NotRequired[ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef],  # (9)
```

1. See [:material-code-braces: ExportAssetToSignedUrlRequestDetailsTypeDef](./type_defs.md#exportassettosignedurlrequestdetailstypedef) 
2. See [:material-code-braces: ExportAssetsToS3RequestDetailsTypeDef](./type_defs.md#exportassetstos3requestdetailstypedef) 
3. See [:material-code-braces: ExportRevisionsToS3RequestDetailsTypeDef](./type_defs.md#exportrevisionstos3requestdetailstypedef) 
4. See [:material-code-braces: ImportAssetFromSignedUrlRequestDetailsTypeDef](./type_defs.md#importassetfromsignedurlrequestdetailstypedef) 
5. See [:material-code-braces: ImportAssetsFromS3RequestDetailsTypeDef](./type_defs.md#importassetsfroms3requestdetailstypedef) 
6. See [:material-code-braces: ImportAssetsFromRedshiftDataSharesRequestDetailsTypeDef](./type_defs.md#importassetsfromredshiftdatasharesrequestdetailstypedef) 
7. See [:material-code-braces: ImportAssetFromApiGatewayApiRequestDetailsTypeDef](./type_defs.md#importassetfromapigatewayapirequestdetailstypedef) 
8. See [:material-code-braces: CreateS3DataAccessFromS3BucketRequestDetailsTypeDef](./type_defs.md#creates3dataaccessfroms3bucketrequestdetailstypedef) 
9. See [:material-code-braces: ImportAssetsFromLakeFormationTagPolicyRequestDetailsTypeDef](./type_defs.md#importassetsfromlakeformationtagpolicyrequestdetailstypedef) 
## ResponseDetailsTypeDef

```python
# ResponseDetailsTypeDef definition

class ResponseDetailsTypeDef(TypedDict):
    ExportAssetToSignedUrl: NotRequired[ExportAssetToSignedUrlResponseDetailsTypeDef],  # (1)
    ExportAssetsToS3: NotRequired[ExportAssetsToS3ResponseDetailsTypeDef],  # (2)
    ExportRevisionsToS3: NotRequired[ExportRevisionsToS3ResponseDetailsTypeDef],  # (3)
    ImportAssetFromSignedUrl: NotRequired[ImportAssetFromSignedUrlResponseDetailsTypeDef],  # (4)
    ImportAssetsFromS3: NotRequired[ImportAssetsFromS3ResponseDetailsTypeDef],  # (5)
    ImportAssetsFromRedshiftDataShares: NotRequired[ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef],  # (6)
    ImportAssetFromApiGatewayApi: NotRequired[ImportAssetFromApiGatewayApiResponseDetailsTypeDef],  # (7)
    CreateS3DataAccessFromS3Bucket: NotRequired[CreateS3DataAccessFromS3BucketResponseDetailsTypeDef],  # (8)
    ImportAssetsFromLakeFormationTagPolicy: NotRequired[ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef],  # (9)
```

1. See [:material-code-braces: ExportAssetToSignedUrlResponseDetailsTypeDef](./type_defs.md#exportassettosignedurlresponsedetailstypedef) 
2. See [:material-code-braces: ExportAssetsToS3ResponseDetailsTypeDef](./type_defs.md#exportassetstos3responsedetailstypedef) 
3. See [:material-code-braces: ExportRevisionsToS3ResponseDetailsTypeDef](./type_defs.md#exportrevisionstos3responsedetailstypedef) 
4. See [:material-code-braces: ImportAssetFromSignedUrlResponseDetailsTypeDef](./type_defs.md#importassetfromsignedurlresponsedetailstypedef) 
5. See [:material-code-braces: ImportAssetsFromS3ResponseDetailsTypeDef](./type_defs.md#importassetsfroms3responsedetailstypedef) 
6. See [:material-code-braces: ImportAssetsFromRedshiftDataSharesResponseDetailsTypeDef](./type_defs.md#importassetsfromredshiftdatasharesresponsedetailstypedef) 
7. See [:material-code-braces: ImportAssetFromApiGatewayApiResponseDetailsTypeDef](./type_defs.md#importassetfromapigatewayapiresponsedetailstypedef) 
8. See [:material-code-braces: CreateS3DataAccessFromS3BucketResponseDetailsTypeDef](./type_defs.md#creates3dataaccessfroms3bucketresponsedetailstypedef) 
9. See [:material-code-braces: ImportAssetsFromLakeFormationTagPolicyResponseDetailsTypeDef](./type_defs.md#importassetsfromlakeformationtagpolicyresponsedetailstypedef) 
## ListEventActionsResponseTypeDef

```python
# ListEventActionsResponseTypeDef definition

class ListEventActionsResponseTypeDef(TypedDict):
    EventActions: List[EventActionEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventActionEntryTypeDef](./type_defs.md#eventactionentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LakeFormationDataPermissionDetailsTypeDef

```python
# LakeFormationDataPermissionDetailsTypeDef definition

class LakeFormationDataPermissionDetailsTypeDef(TypedDict):
    LFTagPolicy: NotRequired[LFTagPolicyDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: LFTagPolicyDetailsTypeDef](./type_defs.md#lftagpolicydetailstypedef) 
## CreateJobRequestRequestTypeDef

```python
# CreateJobRequestRequestTypeDef definition

class CreateJobRequestRequestTypeDef(TypedDict):
    Details: RequestDetailsTypeDef,  # (1)
    Type: TypeType,  # (2)
```

1. See [:material-code-braces: RequestDetailsTypeDef](./type_defs.md#requestdetailstypedef) 
2. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## CreateJobResponseTypeDef

```python
# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    Arn: str,
    CreatedAt: datetime,
    Details: ResponseDetailsTypeDef,  # (1)
    Errors: List[JobErrorTypeDef],  # (2)
    Id: str,
    State: StateType,  # (3)
    Type: TypeType,  # (4)
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ResponseDetailsTypeDef](./type_defs.md#responsedetailstypedef) 
2. See [:material-code-braces: JobErrorTypeDef](./type_defs.md#joberrortypedef) 
3. See [:material-code-brackets: StateType](./literals.md#statetype) 
4. See [:material-code-brackets: TypeType](./literals.md#typetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobResponseTypeDef

```python
# GetJobResponseTypeDef definition

class GetJobResponseTypeDef(TypedDict):
    Arn: str,
    CreatedAt: datetime,
    Details: ResponseDetailsTypeDef,  # (1)
    Errors: List[JobErrorTypeDef],  # (2)
    Id: str,
    State: StateType,  # (3)
    Type: TypeType,  # (4)
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ResponseDetailsTypeDef](./type_defs.md#responsedetailstypedef) 
2. See [:material-code-braces: JobErrorTypeDef](./type_defs.md#joberrortypedef) 
3. See [:material-code-brackets: StateType](./literals.md#statetype) 
4. See [:material-code-brackets: TypeType](./literals.md#typetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobEntryTypeDef

```python
# JobEntryTypeDef definition

class JobEntryTypeDef(TypedDict):
    Arn: str,
    CreatedAt: datetime,
    Details: ResponseDetailsTypeDef,  # (1)
    Id: str,
    State: StateType,  # (3)
    Type: TypeType,  # (4)
    UpdatedAt: datetime,
    Errors: NotRequired[List[JobErrorTypeDef]],  # (2)
```

1. See [:material-code-braces: ResponseDetailsTypeDef](./type_defs.md#responsedetailstypedef) 
2. See [:material-code-braces: JobErrorTypeDef](./type_defs.md#joberrortypedef) 
3. See [:material-code-brackets: StateType](./literals.md#statetype) 
4. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## LakeFormationDataPermissionAssetTypeDef

```python
# LakeFormationDataPermissionAssetTypeDef definition

class LakeFormationDataPermissionAssetTypeDef(TypedDict):
    LakeFormationDataPermissionDetails: LakeFormationDataPermissionDetailsTypeDef,  # (1)
    LakeFormationDataPermissionType: LakeFormationDataPermissionTypeType,  # (2)
    Permissions: List[LFPermissionType],  # (3)
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: LakeFormationDataPermissionDetailsTypeDef](./type_defs.md#lakeformationdatapermissiondetailstypedef) 
2. See [:material-code-brackets: LakeFormationDataPermissionTypeType](./literals.md#lakeformationdatapermissiontypetype) 
3. See [:material-code-brackets: LFPermissionType](./literals.md#lfpermissiontype) 
## ListJobsResponseTypeDef

```python
# ListJobsResponseTypeDef definition

class ListJobsResponseTypeDef(TypedDict):
    Jobs: List[JobEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobEntryTypeDef](./type_defs.md#jobentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetDetailsTypeDef

```python
# AssetDetailsTypeDef definition

class AssetDetailsTypeDef(TypedDict):
    S3SnapshotAsset: NotRequired[S3SnapshotAssetTypeDef],  # (1)
    RedshiftDataShareAsset: NotRequired[RedshiftDataShareAssetTypeDef],  # (2)
    ApiGatewayApiAsset: NotRequired[ApiGatewayApiAssetTypeDef],  # (3)
    S3DataAccessAsset: NotRequired[S3DataAccessAssetTypeDef],  # (4)
    LakeFormationDataPermissionAsset: NotRequired[LakeFormationDataPermissionAssetTypeDef],  # (5)
```

1. See [:material-code-braces: S3SnapshotAssetTypeDef](./type_defs.md#s3snapshotassettypedef) 
2. See [:material-code-braces: RedshiftDataShareAssetTypeDef](./type_defs.md#redshiftdatashareassettypedef) 
3. See [:material-code-braces: ApiGatewayApiAssetTypeDef](./type_defs.md#apigatewayapiassettypedef) 
4. See [:material-code-braces: S3DataAccessAssetTypeDef](./type_defs.md#s3dataaccessassettypedef) 
5. See [:material-code-braces: LakeFormationDataPermissionAssetTypeDef](./type_defs.md#lakeformationdatapermissionassettypedef) 
## AssetEntryTypeDef

```python
# AssetEntryTypeDef definition

class AssetEntryTypeDef(TypedDict):
    Arn: str,
    AssetDetails: AssetDetailsTypeDef,  # (1)
    AssetType: AssetTypeType,  # (2)
    CreatedAt: datetime,
    DataSetId: str,
    Id: str,
    Name: str,
    RevisionId: str,
    UpdatedAt: datetime,
    SourceId: NotRequired[str],
```

1. See [:material-code-braces: AssetDetailsTypeDef](./type_defs.md#assetdetailstypedef) 
2. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
## GetAssetResponseTypeDef

```python
# GetAssetResponseTypeDef definition

class GetAssetResponseTypeDef(TypedDict):
    Arn: str,
    AssetDetails: AssetDetailsTypeDef,  # (1)
    AssetType: AssetTypeType,  # (2)
    CreatedAt: datetime,
    DataSetId: str,
    Id: str,
    Name: str,
    RevisionId: str,
    SourceId: str,
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssetDetailsTypeDef](./type_defs.md#assetdetailstypedef) 
2. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssetResponseTypeDef

```python
# UpdateAssetResponseTypeDef definition

class UpdateAssetResponseTypeDef(TypedDict):
    Arn: str,
    AssetDetails: AssetDetailsTypeDef,  # (1)
    AssetType: AssetTypeType,  # (2)
    CreatedAt: datetime,
    DataSetId: str,
    Id: str,
    Name: str,
    RevisionId: str,
    SourceId: str,
    UpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssetDetailsTypeDef](./type_defs.md#assetdetailstypedef) 
2. See [:material-code-brackets: AssetTypeType](./literals.md#assettypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRevisionAssetsResponseTypeDef

```python
# ListRevisionAssetsResponseTypeDef definition

class ListRevisionAssetsResponseTypeDef(TypedDict):
    Assets: List[AssetEntryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetEntryTypeDef](./type_defs.md#assetentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
