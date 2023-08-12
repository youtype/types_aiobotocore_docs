# Type definitions

> [Index](../README.md) > [CloudHSMV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudHSMV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
    type annotations stubs module [types-aiobotocore-cloudhsmv2](https://pypi.org/project/types-aiobotocore-cloudhsmv2/).



## BackupRetentionPolicyTypeDef

```python
# BackupRetentionPolicyTypeDef definition

class BackupRetentionPolicyTypeDef(TypedDict):
    Type: NotRequired[BackupRetentionTypeType],  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: BackupRetentionTypeType](./literals.md#backupretentiontypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CertificatesTypeDef

```python
# CertificatesTypeDef definition

class CertificatesTypeDef(TypedDict):
    ClusterCsr: NotRequired[str],
    HsmCertificate: NotRequired[str],
    AwsHardwareCertificate: NotRequired[str],
    ManufacturerHardwareCertificate: NotRequired[str],
    ClusterCertificate: NotRequired[str],
```

## HsmTypeDef

```python
# HsmTypeDef definition

class HsmTypeDef(TypedDict):
    HsmId: str,
    AvailabilityZone: NotRequired[str],
    ClusterId: NotRequired[str],
    SubnetId: NotRequired[str],
    EniId: NotRequired[str],
    EniIp: NotRequired[str],
    State: NotRequired[HsmStateType],  # (1)
    StateMessage: NotRequired[str],
```

1. See [:material-code-brackets: HsmStateType](./literals.md#hsmstatetype) 
## DestinationBackupTypeDef

```python
# DestinationBackupTypeDef definition

class DestinationBackupTypeDef(TypedDict):
    CreateTimestamp: NotRequired[datetime],
    SourceRegion: NotRequired[str],
    SourceBackup: NotRequired[str],
    SourceCluster: NotRequired[str],
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

## CreateHsmRequestRequestTypeDef

```python
# CreateHsmRequestRequestTypeDef definition

class CreateHsmRequestRequestTypeDef(TypedDict):
    ClusterId: str,
    AvailabilityZone: str,
    IpAddress: NotRequired[str],
```

## DeleteBackupRequestRequestTypeDef

```python
# DeleteBackupRequestRequestTypeDef definition

class DeleteBackupRequestRequestTypeDef(TypedDict):
    BackupId: str,
```

## DeleteClusterRequestRequestTypeDef

```python
# DeleteClusterRequestRequestTypeDef definition

class DeleteClusterRequestRequestTypeDef(TypedDict):
    ClusterId: str,
```

## DeleteHsmRequestRequestTypeDef

```python
# DeleteHsmRequestRequestTypeDef definition

class DeleteHsmRequestRequestTypeDef(TypedDict):
    ClusterId: str,
    HsmId: NotRequired[str],
    EniId: NotRequired[str],
    EniIp: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeBackupsRequestRequestTypeDef

```python
# DescribeBackupsRequestRequestTypeDef definition

class DescribeBackupsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Mapping[str, Sequence[str]]],
    SortAscending: NotRequired[bool],
```

## DescribeClustersRequestRequestTypeDef

```python
# DescribeClustersRequestRequestTypeDef definition

class DescribeClustersRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Mapping[str, Sequence[str]]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## InitializeClusterRequestRequestTypeDef

```python
# InitializeClusterRequestRequestTypeDef definition

class InitializeClusterRequestRequestTypeDef(TypedDict):
    ClusterId: str,
    SignedCert: str,
    TrustAnchor: str,
```

## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ModifyBackupAttributesRequestRequestTypeDef

```python
# ModifyBackupAttributesRequestRequestTypeDef definition

class ModifyBackupAttributesRequestRequestTypeDef(TypedDict):
    BackupId: str,
    NeverExpires: bool,
```

## RestoreBackupRequestRequestTypeDef

```python
# RestoreBackupRequestRequestTypeDef definition

class RestoreBackupRequestRequestTypeDef(TypedDict):
    BackupId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    TagKeyList: Sequence[str],
```

## ModifyClusterRequestRequestTypeDef

```python
# ModifyClusterRequestRequestTypeDef definition

class ModifyClusterRequestRequestTypeDef(TypedDict):
    BackupRetentionPolicy: BackupRetentionPolicyTypeDef,  # (1)
    ClusterId: str,
```

1. See [:material-code-braces: BackupRetentionPolicyTypeDef](./type_defs.md#backupretentionpolicytypedef) 
## BackupTypeDef

```python
# BackupTypeDef definition

class BackupTypeDef(TypedDict):
    BackupId: str,
    BackupState: NotRequired[BackupStateType],  # (1)
    ClusterId: NotRequired[str],
    CreateTimestamp: NotRequired[datetime],
    CopyTimestamp: NotRequired[datetime],
    NeverExpires: NotRequired[bool],
    SourceRegion: NotRequired[str],
    SourceBackup: NotRequired[str],
    SourceCluster: NotRequired[str],
    DeleteTimestamp: NotRequired[datetime],
    TagList: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: BackupStateType](./literals.md#backupstatetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CopyBackupToRegionRequestRequestTypeDef

```python
# CopyBackupToRegionRequestRequestTypeDef definition

class CopyBackupToRegionRequestRequestTypeDef(TypedDict):
    DestinationRegion: str,
    BackupId: str,
    TagList: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateClusterRequestRequestTypeDef

```python
# CreateClusterRequestRequestTypeDef definition

class CreateClusterRequestRequestTypeDef(TypedDict):
    HsmType: str,
    SubnetIds: Sequence[str],
    BackupRetentionPolicy: NotRequired[BackupRetentionPolicyTypeDef],  # (1)
    SourceBackupId: NotRequired[str],
    TagList: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: BackupRetentionPolicyTypeDef](./type_defs.md#backupretentionpolicytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    TagList: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    BackupPolicy: NotRequired[BackupPolicyType],  # (1)
    BackupRetentionPolicy: NotRequired[BackupRetentionPolicyTypeDef],  # (2)
    ClusterId: NotRequired[str],
    CreateTimestamp: NotRequired[datetime],
    Hsms: NotRequired[List[HsmTypeDef]],  # (3)
    HsmType: NotRequired[str],
    PreCoPassword: NotRequired[str],
    SecurityGroup: NotRequired[str],
    SourceBackupId: NotRequired[str],
    State: NotRequired[ClusterStateType],  # (4)
    StateMessage: NotRequired[str],
    SubnetMapping: NotRequired[Dict[str, str]],
    VpcId: NotRequired[str],
    Certificates: NotRequired[CertificatesTypeDef],  # (5)
    TagList: NotRequired[List[TagTypeDef]],  # (6)
```

1. See [:material-code-brackets: BackupPolicyType](./literals.md#backuppolicytype) 
2. See [:material-code-braces: BackupRetentionPolicyTypeDef](./type_defs.md#backupretentionpolicytypedef) 
3. See [:material-code-braces: HsmTypeDef](./type_defs.md#hsmtypedef) 
4. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
5. See [:material-code-braces: CertificatesTypeDef](./type_defs.md#certificatestypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CopyBackupToRegionResponseTypeDef

```python
# CopyBackupToRegionResponseTypeDef definition

class CopyBackupToRegionResponseTypeDef(TypedDict):
    DestinationBackup: DestinationBackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DestinationBackupTypeDef](./type_defs.md#destinationbackuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHsmResponseTypeDef

```python
# CreateHsmResponseTypeDef definition

class CreateHsmResponseTypeDef(TypedDict):
    Hsm: HsmTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HsmTypeDef](./type_defs.md#hsmtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteHsmResponseTypeDef

```python
# DeleteHsmResponseTypeDef definition

class DeleteHsmResponseTypeDef(TypedDict):
    HsmId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InitializeClusterResponseTypeDef

```python
# InitializeClusterResponseTypeDef definition

class InitializeClusterResponseTypeDef(TypedDict):
    State: ClusterStateType,  # (1)
    StateMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsResponseTypeDef

```python
# ListTagsResponseTypeDef definition

class ListTagsResponseTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBackupsRequestDescribeBackupsPaginateTypeDef

```python
# DescribeBackupsRequestDescribeBackupsPaginateTypeDef definition

class DescribeBackupsRequestDescribeBackupsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Mapping[str, Sequence[str]]],
    SortAscending: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClustersRequestDescribeClustersPaginateTypeDef

```python
# DescribeClustersRequestDescribeClustersPaginateTypeDef definition

class DescribeClustersRequestDescribeClustersPaginateTypeDef(TypedDict):
    Filters: NotRequired[Mapping[str, Sequence[str]]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsRequestListTagsPaginateTypeDef

```python
# ListTagsRequestListTagsPaginateTypeDef definition

class ListTagsRequestListTagsPaginateTypeDef(TypedDict):
    ResourceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DeleteBackupResponseTypeDef

```python
# DeleteBackupResponseTypeDef definition

class DeleteBackupResponseTypeDef(TypedDict):
    Backup: BackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupTypeDef](./type_defs.md#backuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBackupsResponseTypeDef

```python
# DescribeBackupsResponseTypeDef definition

class DescribeBackupsResponseTypeDef(TypedDict):
    Backups: List[BackupTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupTypeDef](./type_defs.md#backuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyBackupAttributesResponseTypeDef

```python
# ModifyBackupAttributesResponseTypeDef definition

class ModifyBackupAttributesResponseTypeDef(TypedDict):
    Backup: BackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupTypeDef](./type_defs.md#backuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreBackupResponseTypeDef

```python
# RestoreBackupResponseTypeDef definition

class RestoreBackupResponseTypeDef(TypedDict):
    Backup: BackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupTypeDef](./type_defs.md#backuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef definition

class CreateClusterResponseTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterResponseTypeDef

```python
# DeleteClusterResponseTypeDef definition

class DeleteClusterResponseTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeClustersResponseTypeDef

```python
# DescribeClustersResponseTypeDef definition

class DescribeClustersResponseTypeDef(TypedDict):
    Clusters: List[ClusterTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyClusterResponseTypeDef

```python
# ModifyClusterResponseTypeDef definition

class ModifyClusterResponseTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
