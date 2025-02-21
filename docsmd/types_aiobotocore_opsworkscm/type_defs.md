# Type definitions

> [Index](../README.md) > [OpsWorksCM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#opsworkscm)
    type annotations stubs module [types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).



## AccountAttributeTypeDef

```python
# AccountAttributeTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import AccountAttributeTypeDef


def get_value() -> AccountAttributeTypeDef:
    return {
        "Name": ...,
    }


# AccountAttributeTypeDef definition

class AccountAttributeTypeDef(TypedDict):
    Name: NotRequired[str],
    Maximum: NotRequired[int],
    Used: NotRequired[int],
```

## EngineAttributeTypeDef

```python
# EngineAttributeTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import EngineAttributeTypeDef


def get_value() -> EngineAttributeTypeDef:
    return {
        "Name": ...,
    }


# EngineAttributeTypeDef definition

class EngineAttributeTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## BackupTypeDef

```python
# BackupTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import BackupTypeDef


def get_value() -> BackupTypeDef:
    return {
        "BackupArn": ...,
    }


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
# TagTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteBackupRequestTypeDef

```python
# DeleteBackupRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DeleteBackupRequestTypeDef


def get_value() -> DeleteBackupRequestTypeDef:
    return {
        "BackupId": ...,
    }


# DeleteBackupRequestTypeDef definition

class DeleteBackupRequestTypeDef(TypedDict):
    BackupId: str,
```

## DeleteServerRequestTypeDef

```python
# DeleteServerRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DeleteServerRequestTypeDef


def get_value() -> DeleteServerRequestTypeDef:
    return {
        "ServerName": ...,
    }


# DeleteServerRequestTypeDef definition

class DeleteServerRequestTypeDef(TypedDict):
    ServerName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeBackupsRequestTypeDef

```python
# DescribeBackupsRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeBackupsRequestTypeDef


def get_value() -> DescribeBackupsRequestTypeDef:
    return {
        "BackupId": ...,
    }


# DescribeBackupsRequestTypeDef definition

class DescribeBackupsRequestTypeDef(TypedDict):
    BackupId: NotRequired[str],
    ServerName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeEventsRequestTypeDef

```python
# DescribeEventsRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeEventsRequestTypeDef


def get_value() -> DescribeEventsRequestTypeDef:
    return {
        "ServerName": ...,
    }


# DescribeEventsRequestTypeDef definition

class DescribeEventsRequestTypeDef(TypedDict):
    ServerName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ServerEventTypeDef

```python
# ServerEventTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import ServerEventTypeDef


def get_value() -> ServerEventTypeDef:
    return {
        "CreatedAt": ...,
    }


# ServerEventTypeDef definition

class ServerEventTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    ServerName: NotRequired[str],
    Message: NotRequired[str],
    LogUrl: NotRequired[str],
```

## DescribeNodeAssociationStatusRequestTypeDef

```python
# DescribeNodeAssociationStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeNodeAssociationStatusRequestTypeDef


def get_value() -> DescribeNodeAssociationStatusRequestTypeDef:
    return {
        "NodeAssociationStatusToken": ...,
    }


# DescribeNodeAssociationStatusRequestTypeDef definition

class DescribeNodeAssociationStatusRequestTypeDef(TypedDict):
    NodeAssociationStatusToken: str,
    ServerName: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeServersRequestTypeDef

```python
# DescribeServersRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeServersRequestTypeDef


def get_value() -> DescribeServersRequestTypeDef:
    return {
        "ServerName": ...,
    }


# DescribeServersRequestTypeDef definition

class DescribeServersRequestTypeDef(TypedDict):
    ServerName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RestoreServerRequestTypeDef

```python
# RestoreServerRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import RestoreServerRequestTypeDef


def get_value() -> RestoreServerRequestTypeDef:
    return {
        "BackupId": ...,
    }


# RestoreServerRequestTypeDef definition

class RestoreServerRequestTypeDef(TypedDict):
    BackupId: str,
    ServerName: str,
    InstanceType: NotRequired[str],
    KeyPair: NotRequired[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateServerEngineAttributesRequestTypeDef

```python
# UpdateServerEngineAttributesRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import UpdateServerEngineAttributesRequestTypeDef


def get_value() -> UpdateServerEngineAttributesRequestTypeDef:
    return {
        "ServerName": ...,
    }


# UpdateServerEngineAttributesRequestTypeDef definition

class UpdateServerEngineAttributesRequestTypeDef(TypedDict):
    ServerName: str,
    AttributeName: str,
    AttributeValue: NotRequired[str],
```

## UpdateServerRequestTypeDef

```python
# UpdateServerRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import UpdateServerRequestTypeDef


def get_value() -> UpdateServerRequestTypeDef:
    return {
        "ServerName": ...,
    }


# UpdateServerRequestTypeDef definition

class UpdateServerRequestTypeDef(TypedDict):
    ServerName: str,
    DisableAutomatedBackup: NotRequired[bool],
    BackupRetentionCount: NotRequired[int],
    PreferredMaintenanceWindow: NotRequired[str],
    PreferredBackupWindow: NotRequired[str],
```

## AssociateNodeRequestTypeDef

```python
# AssociateNodeRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import AssociateNodeRequestTypeDef


def get_value() -> AssociateNodeRequestTypeDef:
    return {
        "ServerName": ...,
    }


# AssociateNodeRequestTypeDef definition

class AssociateNodeRequestTypeDef(TypedDict):
    ServerName: str,
    NodeName: str,
    EngineAttributes: Sequence[EngineAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
## DisassociateNodeRequestTypeDef

```python
# DisassociateNodeRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DisassociateNodeRequestTypeDef


def get_value() -> DisassociateNodeRequestTypeDef:
    return {
        "ServerName": ...,
    }


# DisassociateNodeRequestTypeDef definition

class DisassociateNodeRequestTypeDef(TypedDict):
    ServerName: str,
    NodeName: str,
    EngineAttributes: NotRequired[Sequence[EngineAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
## ExportServerEngineAttributeRequestTypeDef

```python
# ExportServerEngineAttributeRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import ExportServerEngineAttributeRequestTypeDef


def get_value() -> ExportServerEngineAttributeRequestTypeDef:
    return {
        "ExportAttributeName": ...,
    }


# ExportServerEngineAttributeRequestTypeDef definition

class ExportServerEngineAttributeRequestTypeDef(TypedDict):
    ExportAttributeName: str,
    ServerName: str,
    InputAttributes: NotRequired[Sequence[EngineAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
## ServerTypeDef

```python
# ServerTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import ServerTypeDef


def get_value() -> ServerTypeDef:
    return {
        "AssociatePublicIpAddress": ...,
    }


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
## StartMaintenanceRequestTypeDef

```python
# StartMaintenanceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import StartMaintenanceRequestTypeDef


def get_value() -> StartMaintenanceRequestTypeDef:
    return {
        "ServerName": ...,
    }


# StartMaintenanceRequestTypeDef definition

class StartMaintenanceRequestTypeDef(TypedDict):
    ServerName: str,
    EngineAttributes: NotRequired[Sequence[EngineAttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
## AssociateNodeResponseTypeDef

```python
# AssociateNodeResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import AssociateNodeResponseTypeDef


def get_value() -> AssociateNodeResponseTypeDef:
    return {
        "NodeAssociationStatusToken": ...,
    }


# AssociateNodeResponseTypeDef definition

class AssociateNodeResponseTypeDef(TypedDict):
    NodeAssociationStatusToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountAttributesResponseTypeDef

```python
# DescribeAccountAttributesResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeAccountAttributesResponseTypeDef


def get_value() -> DescribeAccountAttributesResponseTypeDef:
    return {
        "Attributes": ...,
    }


# DescribeAccountAttributesResponseTypeDef definition

class DescribeAccountAttributesResponseTypeDef(TypedDict):
    Attributes: List[AccountAttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountAttributeTypeDef](./type_defs.md#accountattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNodeAssociationStatusResponseTypeDef

```python
# DescribeNodeAssociationStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeNodeAssociationStatusResponseTypeDef


def get_value() -> DescribeNodeAssociationStatusResponseTypeDef:
    return {
        "NodeAssociationStatus": ...,
    }


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
# DisassociateNodeResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DisassociateNodeResponseTypeDef


def get_value() -> DisassociateNodeResponseTypeDef:
    return {
        "NodeAssociationStatusToken": ...,
    }


# DisassociateNodeResponseTypeDef definition

class DisassociateNodeResponseTypeDef(TypedDict):
    NodeAssociationStatusToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportServerEngineAttributeResponseTypeDef

```python
# ExportServerEngineAttributeResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import ExportServerEngineAttributeResponseTypeDef


def get_value() -> ExportServerEngineAttributeResponseTypeDef:
    return {
        "EngineAttribute": ...,
    }


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
# CreateBackupResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import CreateBackupResponseTypeDef


def get_value() -> CreateBackupResponseTypeDef:
    return {
        "Backup": ...,
    }


# CreateBackupResponseTypeDef definition

class CreateBackupResponseTypeDef(TypedDict):
    Backup: BackupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupTypeDef](./type_defs.md#backuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBackupsResponseTypeDef

```python
# DescribeBackupsResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeBackupsResponseTypeDef


def get_value() -> DescribeBackupsResponseTypeDef:
    return {
        "Backups": ...,
    }


# DescribeBackupsResponseTypeDef definition

class DescribeBackupsResponseTypeDef(TypedDict):
    Backups: List[BackupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BackupTypeDef](./type_defs.md#backuptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBackupRequestTypeDef

```python
# CreateBackupRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import CreateBackupRequestTypeDef


def get_value() -> CreateBackupRequestTypeDef:
    return {
        "ServerName": ...,
    }


# CreateBackupRequestTypeDef definition

class CreateBackupRequestTypeDef(TypedDict):
    ServerName: str,
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateServerRequestTypeDef

```python
# CreateServerRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import CreateServerRequestTypeDef


def get_value() -> CreateServerRequestTypeDef:
    return {
        "Engine": ...,
    }


# CreateServerRequestTypeDef definition

class CreateServerRequestTypeDef(TypedDict):
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
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeBackupsRequestPaginateTypeDef

```python
# DescribeBackupsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeBackupsRequestPaginateTypeDef


def get_value() -> DescribeBackupsRequestPaginateTypeDef:
    return {
        "BackupId": ...,
    }


# DescribeBackupsRequestPaginateTypeDef definition

class DescribeBackupsRequestPaginateTypeDef(TypedDict):
    BackupId: NotRequired[str],
    ServerName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsRequestPaginateTypeDef

```python
# DescribeEventsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeEventsRequestPaginateTypeDef


def get_value() -> DescribeEventsRequestPaginateTypeDef:
    return {
        "ServerName": ...,
    }


# DescribeEventsRequestPaginateTypeDef definition

class DescribeEventsRequestPaginateTypeDef(TypedDict):
    ServerName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeServersRequestPaginateTypeDef

```python
# DescribeServersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeServersRequestPaginateTypeDef


def get_value() -> DescribeServersRequestPaginateTypeDef:
    return {
        "ServerName": ...,
    }


# DescribeServersRequestPaginateTypeDef definition

class DescribeServersRequestPaginateTypeDef(TypedDict):
    ServerName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestPaginateTypeDef

```python
# ListTagsForResourceRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import ListTagsForResourceRequestPaginateTypeDef


def get_value() -> ListTagsForResourceRequestPaginateTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestPaginateTypeDef definition

class ListTagsForResourceRequestPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsResponseTypeDef

```python
# DescribeEventsResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeEventsResponseTypeDef


def get_value() -> DescribeEventsResponseTypeDef:
    return {
        "ServerEvents": ...,
    }


# DescribeEventsResponseTypeDef definition

class DescribeEventsResponseTypeDef(TypedDict):
    ServerEvents: List[ServerEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServerEventTypeDef](./type_defs.md#servereventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNodeAssociationStatusRequestWaitTypeDef

```python
# DescribeNodeAssociationStatusRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeNodeAssociationStatusRequestWaitTypeDef


def get_value() -> DescribeNodeAssociationStatusRequestWaitTypeDef:
    return {
        "NodeAssociationStatusToken": ...,
    }


# DescribeNodeAssociationStatusRequestWaitTypeDef definition

class DescribeNodeAssociationStatusRequestWaitTypeDef(TypedDict):
    NodeAssociationStatusToken: str,
    ServerName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## CreateServerResponseTypeDef

```python
# CreateServerResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import CreateServerResponseTypeDef


def get_value() -> CreateServerResponseTypeDef:
    return {
        "Server": ...,
    }


# CreateServerResponseTypeDef definition

class CreateServerResponseTypeDef(TypedDict):
    Server: ServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServersResponseTypeDef

```python
# DescribeServersResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import DescribeServersResponseTypeDef


def get_value() -> DescribeServersResponseTypeDef:
    return {
        "Servers": ...,
    }


# DescribeServersResponseTypeDef definition

class DescribeServersResponseTypeDef(TypedDict):
    Servers: List[ServerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreServerResponseTypeDef

```python
# RestoreServerResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import RestoreServerResponseTypeDef


def get_value() -> RestoreServerResponseTypeDef:
    return {
        "Server": ...,
    }


# RestoreServerResponseTypeDef definition

class RestoreServerResponseTypeDef(TypedDict):
    Server: ServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMaintenanceResponseTypeDef

```python
# StartMaintenanceResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import StartMaintenanceResponseTypeDef


def get_value() -> StartMaintenanceResponseTypeDef:
    return {
        "Server": ...,
    }


# StartMaintenanceResponseTypeDef definition

class StartMaintenanceResponseTypeDef(TypedDict):
    Server: ServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServerEngineAttributesResponseTypeDef

```python
# UpdateServerEngineAttributesResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import UpdateServerEngineAttributesResponseTypeDef


def get_value() -> UpdateServerEngineAttributesResponseTypeDef:
    return {
        "Server": ...,
    }


# UpdateServerEngineAttributesResponseTypeDef definition

class UpdateServerEngineAttributesResponseTypeDef(TypedDict):
    Server: ServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServerResponseTypeDef

```python
# UpdateServerResponseTypeDef TypedDict usage example

from types_aiobotocore_opsworkscm.type_defs import UpdateServerResponseTypeDef


def get_value() -> UpdateServerResponseTypeDef:
    return {
        "Server": ...,
    }


# UpdateServerResponseTypeDef definition

class UpdateServerResponseTypeDef(TypedDict):
    Server: ServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
