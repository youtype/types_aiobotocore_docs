# Type definitions

> [Index](../README.md) > [OpsWorksCM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
    type annotations stubs module [types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).



## AccountAttributeTypeDef

```python
# AccountAttributeTypeDef definition

class AccountAttributeTypeDef(TypedDict):
    Name: NotRequired[str],
    Maximum: NotRequired[int],
    Used: NotRequired[int],
```

## EngineAttributeTypeDef

```python
# EngineAttributeTypeDef definition

class EngineAttributeTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
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

## BackupTypeDef

```python
# BackupTypeDef definition

class BackupTypeDef(TypedDict):
    BackupArn: NotRequired[str],
    BackupId: NotRequired[str],
    BackupType: NotRequired[BackupTypeType],  # (1)
    CreatedAt: NotRequired[datetime],
    Description: NotRequired[str],
    Engine: NotRequired[str],
    EngineModel: NotRequired[str],
    EngineVersion: NotRequired[str],
    InstanceProfileArn: NotRequired[str],
    InstanceType: NotRequired[str],
    KeyPair: NotRequired[str],
    PreferredBackupWindow: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    S3DataSize: NotRequired[int],
    S3DataUrl: NotRequired[str],
    S3LogUrl: NotRequired[str],
    SecurityGroupIds: NotRequired[List[str]],
    ServerName: NotRequired[str],
    ServiceRoleArn: NotRequired[str],
    Status: NotRequired[BackupStatusType],  # (2)
    StatusDescription: NotRequired[str],
    SubnetIds: NotRequired[List[str]],
    ToolsVersion: NotRequired[str],
    UserArn: NotRequired[str],
```

1. See [:material-code-brackets: BackupTypeType](./literals.md#backuptypetype) 
2. See [:material-code-brackets: BackupStatusType](./literals.md#backupstatustype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteBackupRequestRequestTypeDef

```python
# DeleteBackupRequestRequestTypeDef definition

class DeleteBackupRequestRequestTypeDef(TypedDict):
    BackupId: str,
```

## DeleteServerRequestRequestTypeDef

```python
# DeleteServerRequestRequestTypeDef definition

class DeleteServerRequestRequestTypeDef(TypedDict):
    ServerName: str,
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
    BackupId: NotRequired[str],
    ServerName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeEventsRequestRequestTypeDef

```python
# DescribeEventsRequestRequestTypeDef definition

class DescribeEventsRequestRequestTypeDef(TypedDict):
    ServerName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ServerEventTypeDef

```python
# ServerEventTypeDef definition

class ServerEventTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    ServerName: NotRequired[str],
    Message: NotRequired[str],
    LogUrl: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeNodeAssociationStatusRequestRequestTypeDef

```python
# DescribeNodeAssociationStatusRequestRequestTypeDef definition

class DescribeNodeAssociationStatusRequestRequestTypeDef(TypedDict):
    NodeAssociationStatusToken: str,
    ServerName: str,
```

## DescribeServersRequestRequestTypeDef

```python
# DescribeServersRequestRequestTypeDef definition

class DescribeServersRequestRequestTypeDef(TypedDict):
    ServerName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RestoreServerRequestRequestTypeDef

```python
# RestoreServerRequestRequestTypeDef definition

class RestoreServerRequestRequestTypeDef(TypedDict):
    BackupId: str,
    ServerName: str,
    InstanceType: NotRequired[str],
    KeyPair: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateServerEngineAttributesRequestRequestTypeDef

```python
# UpdateServerEngineAttributesRequestRequestTypeDef definition

class UpdateServerEngineAttributesRequestRequestTypeDef(TypedDict):
    ServerName: str,
    AttributeName: str,
    AttributeValue: NotRequired[str],
```

## UpdateServerRequestRequestTypeDef

```python
# UpdateServerRequestRequestTypeDef definition

class UpdateServerRequestRequestTypeDef(TypedDict):
    ServerName: str,
    DisableAutomatedBackup: NotRequired[bool],
    BackupRetentionCount: NotRequired[int],
    PreferredMaintenanceWindow: NotRequired[str],
    PreferredBackupWindow: NotRequired[str],
```

## AssociateNodeRequestRequestTypeDef

```python
# AssociateNodeRequestRequestTypeDef definition

class AssociateNodeRequestRequestTypeDef(TypedDict):
    ServerName: str,
    NodeName: str,
    EngineAttributes: Sequence[EngineAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
## DisassociateNodeRequestRequestTypeDef

```python
# DisassociateNodeRequestRequestTypeDef definition

class DisassociateNodeRequestRequestTypeDef(TypedDict):
    ServerName: str,
    NodeName: str,
    EngineAttributes: NotRequired[Sequence[EngineAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
## ExportServerEngineAttributeRequestRequestTypeDef

```python
# ExportServerEngineAttributeRequestRequestTypeDef definition

class ExportServerEngineAttributeRequestRequestTypeDef(TypedDict):
    ExportAttributeName: str,
    ServerName: str,
    InputAttributes: NotRequired[Sequence[EngineAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
## ServerTypeDef

```python
# ServerTypeDef definition

class ServerTypeDef(TypedDict):
    AssociatePublicIpAddress: NotRequired[bool],
    BackupRetentionCount: NotRequired[int],
    ServerName: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    CloudFormationStackArn: NotRequired[str],
    CustomDomain: NotRequired[str],
    DisableAutomatedBackup: NotRequired[bool],
    Endpoint: NotRequired[str],
    Engine: NotRequired[str],
    EngineModel: NotRequired[str],
    EngineAttributes: NotRequired[List[EngineAttributeTypeDef]],  # (1)
    EngineVersion: NotRequired[str],
    InstanceProfileArn: NotRequired[str],
    InstanceType: NotRequired[str],
    KeyPair: NotRequired[str],
    MaintenanceStatus: NotRequired[MaintenanceStatusType],  # (2)
    PreferredMaintenanceWindow: NotRequired[str],
    PreferredBackupWindow: NotRequired[str],
    SecurityGroupIds: NotRequired[List[str]],
    ServiceRoleArn: NotRequired[str],
    Status: NotRequired[ServerStatusType],  # (3)
    StatusReason: NotRequired[str],
    SubnetIds: NotRequired[List[str]],
    ServerArn: NotRequired[str],
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
2. See [:material-code-brackets: MaintenanceStatusType](./literals.md#maintenancestatustype) 
3. See [:material-code-brackets: ServerStatusType](./literals.md#serverstatustype) 
## StartMaintenanceRequestRequestTypeDef

```python
# StartMaintenanceRequestRequestTypeDef definition

class StartMaintenanceRequestRequestTypeDef(TypedDict):
    ServerName: str,
    EngineAttributes: NotRequired[Sequence[EngineAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
## AssociateNodeResponseTypeDef

```python
# AssociateNodeResponseTypeDef definition

class AssociateNodeResponseTypeDef(TypedDict):
    NodeAssociationStatusToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountAttributesResponseTypeDef

```python
# DescribeAccountAttributesResponseTypeDef definition

class DescribeAccountAttributesResponseTypeDef(TypedDict):
    Attributes: List[AccountAttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAttributeTypeDef](./type_defs.md#accountattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNodeAssociationStatusResponseTypeDef

```python
# DescribeNodeAssociationStatusResponseTypeDef definition

class DescribeNodeAssociationStatusResponseTypeDef(TypedDict):
    NodeAssociationStatus: NodeAssociationStatusType,  # (1)
    EngineAttributes: List[EngineAttributeTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: NodeAssociationStatusType](./literals.md#nodeassociationstatustype) 
2. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateNodeResponseTypeDef

```python
# DisassociateNodeResponseTypeDef definition

class DisassociateNodeResponseTypeDef(TypedDict):
    NodeAssociationStatusToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportServerEngineAttributeResponseTypeDef

```python
# ExportServerEngineAttributeResponseTypeDef definition

class ExportServerEngineAttributeResponseTypeDef(TypedDict):
    EngineAttribute: EngineAttributeTypeDef,  # (1)
    ServerName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackupResponseTypeDef

```python
# CreateBackupResponseTypeDef definition

class CreateBackupResponseTypeDef(TypedDict):
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
## CreateBackupRequestRequestTypeDef

```python
# CreateBackupRequestRequestTypeDef definition

class CreateBackupRequestRequestTypeDef(TypedDict):
    ServerName: str,
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateServerRequestRequestTypeDef

```python
# CreateServerRequestRequestTypeDef definition

class CreateServerRequestRequestTypeDef(TypedDict):
    Engine: str,
    ServerName: str,
    InstanceProfileArn: str,
    InstanceType: str,
    ServiceRoleArn: str,
    AssociatePublicIpAddress: NotRequired[bool],
    CustomDomain: NotRequired[str],
    CustomCertificate: NotRequired[str],
    CustomPrivateKey: NotRequired[str],
    DisableAutomatedBackup: NotRequired[bool],
    EngineModel: NotRequired[str],
    EngineVersion: NotRequired[str],
    EngineAttributes: NotRequired[Sequence[EngineAttributeTypeDef]],  # (1)
    BackupRetentionCount: NotRequired[int],
    KeyPair: NotRequired[str],
    PreferredMaintenanceWindow: NotRequired[str],
    PreferredBackupWindow: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    SubnetIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    BackupId: NotRequired[str],
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeBackupsRequestDescribeBackupsPaginateTypeDef

```python
# DescribeBackupsRequestDescribeBackupsPaginateTypeDef definition

class DescribeBackupsRequestDescribeBackupsPaginateTypeDef(TypedDict):
    BackupId: NotRequired[str],
    ServerName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsRequestDescribeEventsPaginateTypeDef

```python
# DescribeEventsRequestDescribeEventsPaginateTypeDef definition

class DescribeEventsRequestDescribeEventsPaginateTypeDef(TypedDict):
    ServerName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeServersRequestDescribeServersPaginateTypeDef

```python
# DescribeServersRequestDescribeServersPaginateTypeDef definition

class DescribeServersRequestDescribeServersPaginateTypeDef(TypedDict):
    ServerName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceRequestListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsResponseTypeDef

```python
# DescribeEventsResponseTypeDef definition

class DescribeEventsResponseTypeDef(TypedDict):
    ServerEvents: List[ServerEventTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerEventTypeDef](./type_defs.md#servereventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef

```python
# DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef definition

class DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef(TypedDict):
    NodeAssociationStatusToken: str,
    ServerName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## CreateServerResponseTypeDef

```python
# CreateServerResponseTypeDef definition

class CreateServerResponseTypeDef(TypedDict):
    Server: ServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServersResponseTypeDef

```python
# DescribeServersResponseTypeDef definition

class DescribeServersResponseTypeDef(TypedDict):
    Servers: List[ServerTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreServerResponseTypeDef

```python
# RestoreServerResponseTypeDef definition

class RestoreServerResponseTypeDef(TypedDict):
    Server: ServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMaintenanceResponseTypeDef

```python
# StartMaintenanceResponseTypeDef definition

class StartMaintenanceResponseTypeDef(TypedDict):
    Server: ServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServerEngineAttributesResponseTypeDef

```python
# UpdateServerEngineAttributesResponseTypeDef definition

class UpdateServerEngineAttributesResponseTypeDef(TypedDict):
    Server: ServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServerResponseTypeDef

```python
# UpdateServerResponseTypeDef definition

class UpdateServerResponseTypeDef(TypedDict):
    Server: ServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
