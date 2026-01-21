# Type definitions

> [Index](../README.md) > [Odb](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Odb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb.html#odb)
    type annotations stubs module [types-aiobotocore-odb](https://pypi.org/project/types-aiobotocore-odb/).

## MaintenanceWindowUnionTypeDef

```python
# MaintenanceWindowUnionTypeDef Union usage example

from types_aiobotocore_odb.type_defs import MaintenanceWindowUnionTypeDef


def get_value() -> MaintenanceWindowUnionTypeDef:
    return ...


# MaintenanceWindowUnionTypeDef definition

MaintenanceWindowUnionTypeDef = Union[
    MaintenanceWindowTypeDef,  # (1)
    MaintenanceWindowOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef)
2. See [:material-code-braces: MaintenanceWindowOutputTypeDef](./type_defs.md#maintenancewindowoutputtypedef)



## AcceptMarketplaceRegistrationInputTypeDef

```python
# AcceptMarketplaceRegistrationInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import AcceptMarketplaceRegistrationInputTypeDef


def get_value() -> AcceptMarketplaceRegistrationInputTypeDef:
    return {
        "marketplaceRegistrationToken": ...,
    }


# AcceptMarketplaceRegistrationInputTypeDef definition

class AcceptMarketplaceRegistrationInputTypeDef(TypedDict):
    marketplaceRegistrationToken: str,
```


## AssociateIamRoleToResourceInputTypeDef

```python
# AssociateIamRoleToResourceInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import AssociateIamRoleToResourceInputTypeDef


def get_value() -> AssociateIamRoleToResourceInputTypeDef:
    return {
        "iamRoleArn": ...,
    }


# AssociateIamRoleToResourceInputTypeDef definition

class AssociateIamRoleToResourceInputTypeDef(TypedDict):
    iamRoleArn: str,
    awsIntegration: SupportedAwsIntegrationType,  # (1)
    resourceArn: str,
```

1. See [:material-code-brackets: SupportedAwsIntegrationType](./literals.md#supportedawsintegrationtype)

## AutonomousVirtualMachineSummaryTypeDef

```python
# AutonomousVirtualMachineSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import AutonomousVirtualMachineSummaryTypeDef


def get_value() -> AutonomousVirtualMachineSummaryTypeDef:
    return {
        "autonomousVirtualMachineId": ...,
    }


# AutonomousVirtualMachineSummaryTypeDef definition

class AutonomousVirtualMachineSummaryTypeDef(TypedDict):
    autonomousVirtualMachineId: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    vmName: NotRequired[str],
    dbServerId: NotRequired[str],
    dbServerDisplayName: NotRequired[str],
    cpuCoreCount: NotRequired[int],
    memorySizeInGBs: NotRequired[int],
    dbNodeStorageSizeInGBs: NotRequired[int],
    clientIpAddress: NotRequired[str],
    cloudAutonomousVmClusterId: NotRequired[str],
    ocid: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)

## CloudAutonomousVmClusterResourceDetailsTypeDef

```python
# CloudAutonomousVmClusterResourceDetailsTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CloudAutonomousVmClusterResourceDetailsTypeDef


def get_value() -> CloudAutonomousVmClusterResourceDetailsTypeDef:
    return {
        "cloudAutonomousVmClusterId": ...,
    }


# CloudAutonomousVmClusterResourceDetailsTypeDef definition

class CloudAutonomousVmClusterResourceDetailsTypeDef(TypedDict):
    cloudAutonomousVmClusterId: NotRequired[str],
    unallocatedAdbStorageInTBs: NotRequired[float],
```


## IamRoleTypeDef

```python
# IamRoleTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import IamRoleTypeDef


def get_value() -> IamRoleTypeDef:
    return {
        "iamRoleArn": ...,
    }


# IamRoleTypeDef definition

class IamRoleTypeDef(TypedDict):
    iamRoleArn: NotRequired[str],
    status: NotRequired[IamRoleStatusType],  # (1)
    statusReason: NotRequired[str],
    awsIntegration: NotRequired[SupportedAwsIntegrationType],  # (2)
```

1. See [:material-code-brackets: IamRoleStatusType](./literals.md#iamrolestatustype)
2. See [:material-code-brackets: SupportedAwsIntegrationType](./literals.md#supportedawsintegrationtype)

## CustomerContactTypeDef

```python
# CustomerContactTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CustomerContactTypeDef


def get_value() -> CustomerContactTypeDef:
    return {
        "email": ...,
    }


# CustomerContactTypeDef definition

class CustomerContactTypeDef(TypedDict):
    email: NotRequired[str],
```


## DataCollectionOptionsTypeDef

```python
# DataCollectionOptionsTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DataCollectionOptionsTypeDef


def get_value() -> DataCollectionOptionsTypeDef:
    return {
        "isDiagnosticsEventsEnabled": ...,
    }


# DataCollectionOptionsTypeDef definition

class DataCollectionOptionsTypeDef(TypedDict):
    isDiagnosticsEventsEnabled: NotRequired[bool],
    isHealthMonitoringEnabled: NotRequired[bool],
    isIncidentLogsEnabled: NotRequired[bool],
```


## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```


## CreateOdbNetworkInputTypeDef

```python
# CreateOdbNetworkInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CreateOdbNetworkInputTypeDef


def get_value() -> CreateOdbNetworkInputTypeDef:
    return {
        "displayName": ...,
    }


# CreateOdbNetworkInputTypeDef definition

class CreateOdbNetworkInputTypeDef(TypedDict):
    displayName: str,
    clientSubnetCidr: str,
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    backupSubnetCidr: NotRequired[str],
    customDomainName: NotRequired[str],
    defaultDnsPrefix: NotRequired[str],
    clientToken: NotRequired[str],
    s3Access: NotRequired[AccessType],  # (1)
    zeroEtlAccess: NotRequired[AccessType],  # (1)
    stsAccess: NotRequired[AccessType],  # (1)
    kmsAccess: NotRequired[AccessType],  # (1)
    s3PolicyDocument: NotRequired[str],
    stsPolicyDocument: NotRequired[str],
    kmsPolicyDocument: NotRequired[str],
    crossRegionS3RestoreSourcesToEnable: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AccessType](./literals.md#accesstype)
2. See [:material-code-brackets: AccessType](./literals.md#accesstype)
3. See [:material-code-brackets: AccessType](./literals.md#accesstype)
4. See [:material-code-brackets: AccessType](./literals.md#accesstype)

## CreateOdbPeeringConnectionInputTypeDef

```python
# CreateOdbPeeringConnectionInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CreateOdbPeeringConnectionInputTypeDef


def get_value() -> CreateOdbPeeringConnectionInputTypeDef:
    return {
        "odbNetworkId": ...,
    }


# CreateOdbPeeringConnectionInputTypeDef definition

class CreateOdbPeeringConnectionInputTypeDef(TypedDict):
    odbNetworkId: str,
    peerNetworkId: str,
    displayName: NotRequired[str],
    peerNetworkCidrsToBeAdded: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```


## CrossRegionS3RestoreSourcesAccessTypeDef

```python
# CrossRegionS3RestoreSourcesAccessTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CrossRegionS3RestoreSourcesAccessTypeDef


def get_value() -> CrossRegionS3RestoreSourcesAccessTypeDef:
    return {
        "region": ...,
    }


# CrossRegionS3RestoreSourcesAccessTypeDef definition

class CrossRegionS3RestoreSourcesAccessTypeDef(TypedDict):
    region: NotRequired[str],
    ipv4Addresses: NotRequired[list[str]],
    status: NotRequired[ManagedResourceStatusType],  # (1)
```

1. See [:material-code-brackets: ManagedResourceStatusType](./literals.md#managedresourcestatustype)

## DayOfWeekTypeDef

```python
# DayOfWeekTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DayOfWeekTypeDef


def get_value() -> DayOfWeekTypeDef:
    return {
        "name": ...,
    }


# DayOfWeekTypeDef definition

class DayOfWeekTypeDef(TypedDict):
    name: NotRequired[DayOfWeekNameType],  # (1)
```

1. See [:material-code-brackets: DayOfWeekNameType](./literals.md#dayofweeknametype)

## DbIormConfigTypeDef

```python
# DbIormConfigTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DbIormConfigTypeDef


def get_value() -> DbIormConfigTypeDef:
    return {
        "dbName": ...,
    }


# DbIormConfigTypeDef definition

class DbIormConfigTypeDef(TypedDict):
    dbName: NotRequired[str],
    flashCacheLimit: NotRequired[str],
    share: NotRequired[int],
```


## DbNodeSummaryTypeDef

```python
# DbNodeSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DbNodeSummaryTypeDef


def get_value() -> DbNodeSummaryTypeDef:
    return {
        "dbNodeId": ...,
    }


# DbNodeSummaryTypeDef definition

class DbNodeSummaryTypeDef(TypedDict):
    dbNodeId: NotRequired[str],
    dbNodeArn: NotRequired[str],
    status: NotRequired[DbNodeResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    additionalDetails: NotRequired[str],
    backupIpId: NotRequired[str],
    backupVnic2Id: NotRequired[str],
    backupVnicId: NotRequired[str],
    cpuCoreCount: NotRequired[int],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServerId: NotRequired[str],
    dbSystemId: NotRequired[str],
    faultDomain: NotRequired[str],
    hostIpId: NotRequired[str],
    hostname: NotRequired[str],
    ocid: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    maintenanceType: NotRequired[DbNodeMaintenanceTypeType],  # (2)
    memorySizeInGBs: NotRequired[int],
    softwareStorageSizeInGB: NotRequired[int],
    createdAt: NotRequired[datetime.datetime],
    timeMaintenanceWindowEnd: NotRequired[str],
    timeMaintenanceWindowStart: NotRequired[str],
    totalCpuCoreCount: NotRequired[int],
    vnic2Id: NotRequired[str],
    vnicId: NotRequired[str],
```

1. See [:material-code-brackets: DbNodeResourceStatusType](./literals.md#dbnoderesourcestatustype)
2. See [:material-code-brackets: DbNodeMaintenanceTypeType](./literals.md#dbnodemaintenancetypetype)

## DbNodeTypeDef

```python
# DbNodeTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DbNodeTypeDef


def get_value() -> DbNodeTypeDef:
    return {
        "dbNodeId": ...,
    }


# DbNodeTypeDef definition

class DbNodeTypeDef(TypedDict):
    dbNodeId: NotRequired[str],
    dbNodeArn: NotRequired[str],
    status: NotRequired[DbNodeResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    additionalDetails: NotRequired[str],
    backupIpId: NotRequired[str],
    backupVnic2Id: NotRequired[str],
    backupVnicId: NotRequired[str],
    cpuCoreCount: NotRequired[int],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServerId: NotRequired[str],
    dbSystemId: NotRequired[str],
    faultDomain: NotRequired[str],
    hostIpId: NotRequired[str],
    hostname: NotRequired[str],
    ocid: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    maintenanceType: NotRequired[DbNodeMaintenanceTypeType],  # (2)
    memorySizeInGBs: NotRequired[int],
    softwareStorageSizeInGB: NotRequired[int],
    createdAt: NotRequired[datetime.datetime],
    timeMaintenanceWindowEnd: NotRequired[str],
    timeMaintenanceWindowStart: NotRequired[str],
    totalCpuCoreCount: NotRequired[int],
    vnic2Id: NotRequired[str],
    vnicId: NotRequired[str],
    privateIpAddress: NotRequired[str],
    floatingIpAddress: NotRequired[str],
```

1. See [:material-code-brackets: DbNodeResourceStatusType](./literals.md#dbnoderesourcestatustype)
2. See [:material-code-brackets: DbNodeMaintenanceTypeType](./literals.md#dbnodemaintenancetypetype)

## DbServerPatchingDetailsTypeDef

```python
# DbServerPatchingDetailsTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DbServerPatchingDetailsTypeDef


def get_value() -> DbServerPatchingDetailsTypeDef:
    return {
        "estimatedPatchDuration": ...,
    }


# DbServerPatchingDetailsTypeDef definition

class DbServerPatchingDetailsTypeDef(TypedDict):
    estimatedPatchDuration: NotRequired[int],
    patchingStatus: NotRequired[DbServerPatchingStatusType],  # (1)
    timePatchingEnded: NotRequired[str],
    timePatchingStarted: NotRequired[str],
```

1. See [:material-code-brackets: DbServerPatchingStatusType](./literals.md#dbserverpatchingstatustype)

## DbSystemShapeSummaryTypeDef

```python
# DbSystemShapeSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DbSystemShapeSummaryTypeDef


def get_value() -> DbSystemShapeSummaryTypeDef:
    return {
        "availableCoreCount": ...,
    }


# DbSystemShapeSummaryTypeDef definition

class DbSystemShapeSummaryTypeDef(TypedDict):
    availableCoreCount: NotRequired[int],
    availableCoreCountPerNode: NotRequired[int],
    availableDataStorageInTBs: NotRequired[int],
    availableDataStoragePerServerInTBs: NotRequired[int],
    availableDbNodePerNodeInGBs: NotRequired[int],
    availableDbNodeStorageInGBs: NotRequired[int],
    availableMemoryInGBs: NotRequired[int],
    availableMemoryPerNodeInGBs: NotRequired[int],
    coreCountIncrement: NotRequired[int],
    maxStorageCount: NotRequired[int],
    maximumNodeCount: NotRequired[int],
    minCoreCountPerNode: NotRequired[int],
    minDataStorageInTBs: NotRequired[int],
    minDbNodeStoragePerNodeInGBs: NotRequired[int],
    minMemoryPerNodeInGBs: NotRequired[int],
    minStorageCount: NotRequired[int],
    minimumCoreCount: NotRequired[int],
    minimumNodeCount: NotRequired[int],
    runtimeMinimumCoreCount: NotRequired[int],
    shapeFamily: NotRequired[str],
    shapeType: NotRequired[ShapeTypeType],  # (1)
    name: NotRequired[str],
    computeModel: NotRequired[ComputeModelType],  # (2)
    areServerTypesSupported: NotRequired[bool],
```

1. See [:material-code-brackets: ShapeTypeType](./literals.md#shapetypetype)
2. See [:material-code-brackets: ComputeModelType](./literals.md#computemodeltype)

## DeleteCloudAutonomousVmClusterInputTypeDef

```python
# DeleteCloudAutonomousVmClusterInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DeleteCloudAutonomousVmClusterInputTypeDef


def get_value() -> DeleteCloudAutonomousVmClusterInputTypeDef:
    return {
        "cloudAutonomousVmClusterId": ...,
    }


# DeleteCloudAutonomousVmClusterInputTypeDef definition

class DeleteCloudAutonomousVmClusterInputTypeDef(TypedDict):
    cloudAutonomousVmClusterId: str,
```


## DeleteCloudExadataInfrastructureInputTypeDef

```python
# DeleteCloudExadataInfrastructureInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DeleteCloudExadataInfrastructureInputTypeDef


def get_value() -> DeleteCloudExadataInfrastructureInputTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# DeleteCloudExadataInfrastructureInputTypeDef definition

class DeleteCloudExadataInfrastructureInputTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
```


## DeleteCloudVmClusterInputTypeDef

```python
# DeleteCloudVmClusterInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DeleteCloudVmClusterInputTypeDef


def get_value() -> DeleteCloudVmClusterInputTypeDef:
    return {
        "cloudVmClusterId": ...,
    }


# DeleteCloudVmClusterInputTypeDef definition

class DeleteCloudVmClusterInputTypeDef(TypedDict):
    cloudVmClusterId: str,
```


## DeleteOdbNetworkInputTypeDef

```python
# DeleteOdbNetworkInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DeleteOdbNetworkInputTypeDef


def get_value() -> DeleteOdbNetworkInputTypeDef:
    return {
        "odbNetworkId": ...,
    }


# DeleteOdbNetworkInputTypeDef definition

class DeleteOdbNetworkInputTypeDef(TypedDict):
    odbNetworkId: str,
    deleteAssociatedResources: bool,
```


## DeleteOdbPeeringConnectionInputTypeDef

```python
# DeleteOdbPeeringConnectionInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DeleteOdbPeeringConnectionInputTypeDef


def get_value() -> DeleteOdbPeeringConnectionInputTypeDef:
    return {
        "odbPeeringConnectionId": ...,
    }


# DeleteOdbPeeringConnectionInputTypeDef definition

class DeleteOdbPeeringConnectionInputTypeDef(TypedDict):
    odbPeeringConnectionId: str,
```


## DisassociateIamRoleFromResourceInputTypeDef

```python
# DisassociateIamRoleFromResourceInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DisassociateIamRoleFromResourceInputTypeDef


def get_value() -> DisassociateIamRoleFromResourceInputTypeDef:
    return {
        "iamRoleArn": ...,
    }


# DisassociateIamRoleFromResourceInputTypeDef definition

class DisassociateIamRoleFromResourceInputTypeDef(TypedDict):
    iamRoleArn: str,
    awsIntegration: SupportedAwsIntegrationType,  # (1)
    resourceArn: str,
```

1. See [:material-code-brackets: SupportedAwsIntegrationType](./literals.md#supportedawsintegrationtype)

## GetCloudAutonomousVmClusterInputTypeDef

```python
# GetCloudAutonomousVmClusterInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetCloudAutonomousVmClusterInputTypeDef


def get_value() -> GetCloudAutonomousVmClusterInputTypeDef:
    return {
        "cloudAutonomousVmClusterId": ...,
    }


# GetCloudAutonomousVmClusterInputTypeDef definition

class GetCloudAutonomousVmClusterInputTypeDef(TypedDict):
    cloudAutonomousVmClusterId: str,
```


## GetCloudExadataInfrastructureInputTypeDef

```python
# GetCloudExadataInfrastructureInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetCloudExadataInfrastructureInputTypeDef


def get_value() -> GetCloudExadataInfrastructureInputTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# GetCloudExadataInfrastructureInputTypeDef definition

class GetCloudExadataInfrastructureInputTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
```


## GetCloudExadataInfrastructureUnallocatedResourcesInputTypeDef

```python
# GetCloudExadataInfrastructureUnallocatedResourcesInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetCloudExadataInfrastructureUnallocatedResourcesInputTypeDef


def get_value() -> GetCloudExadataInfrastructureUnallocatedResourcesInputTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# GetCloudExadataInfrastructureUnallocatedResourcesInputTypeDef definition

class GetCloudExadataInfrastructureUnallocatedResourcesInputTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
    dbServers: NotRequired[Sequence[str]],
```


## GetCloudVmClusterInputTypeDef

```python
# GetCloudVmClusterInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetCloudVmClusterInputTypeDef


def get_value() -> GetCloudVmClusterInputTypeDef:
    return {
        "cloudVmClusterId": ...,
    }


# GetCloudVmClusterInputTypeDef definition

class GetCloudVmClusterInputTypeDef(TypedDict):
    cloudVmClusterId: str,
```


## GetDbNodeInputTypeDef

```python
# GetDbNodeInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetDbNodeInputTypeDef


def get_value() -> GetDbNodeInputTypeDef:
    return {
        "cloudVmClusterId": ...,
    }


# GetDbNodeInputTypeDef definition

class GetDbNodeInputTypeDef(TypedDict):
    cloudVmClusterId: str,
    dbNodeId: str,
```


## GetDbServerInputTypeDef

```python
# GetDbServerInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetDbServerInputTypeDef


def get_value() -> GetDbServerInputTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# GetDbServerInputTypeDef definition

class GetDbServerInputTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
    dbServerId: str,
```


## OciIdentityDomainTypeDef

```python
# OciIdentityDomainTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import OciIdentityDomainTypeDef


def get_value() -> OciIdentityDomainTypeDef:
    return {
        "ociIdentityDomainId": ...,
    }


# OciIdentityDomainTypeDef definition

class OciIdentityDomainTypeDef(TypedDict):
    ociIdentityDomainId: NotRequired[str],
    ociIdentityDomainResourceUrl: NotRequired[str],
    ociIdentityDomainUrl: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    accountSetupCloudFormationUrl: NotRequired[str],
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)

## GetOdbNetworkInputTypeDef

```python
# GetOdbNetworkInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetOdbNetworkInputTypeDef


def get_value() -> GetOdbNetworkInputTypeDef:
    return {
        "odbNetworkId": ...,
    }


# GetOdbNetworkInputTypeDef definition

class GetOdbNetworkInputTypeDef(TypedDict):
    odbNetworkId: str,
```


## GetOdbPeeringConnectionInputTypeDef

```python
# GetOdbPeeringConnectionInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetOdbPeeringConnectionInputTypeDef


def get_value() -> GetOdbPeeringConnectionInputTypeDef:
    return {
        "odbPeeringConnectionId": ...,
    }


# GetOdbPeeringConnectionInputTypeDef definition

class GetOdbPeeringConnectionInputTypeDef(TypedDict):
    odbPeeringConnectionId: str,
```


## OdbPeeringConnectionTypeDef

```python
# OdbPeeringConnectionTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import OdbPeeringConnectionTypeDef


def get_value() -> OdbPeeringConnectionTypeDef:
    return {
        "odbPeeringConnectionId": ...,
    }


# OdbPeeringConnectionTypeDef definition

class OdbPeeringConnectionTypeDef(TypedDict):
    odbPeeringConnectionId: str,
    displayName: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    odbPeeringConnectionArn: NotRequired[str],
    odbNetworkArn: NotRequired[str],
    peerNetworkArn: NotRequired[str],
    odbPeeringConnectionType: NotRequired[str],
    peerNetworkCidrs: NotRequired[list[str]],
    createdAt: NotRequired[datetime.datetime],
    percentProgress: NotRequired[float],
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)

## GiVersionSummaryTypeDef

```python
# GiVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GiVersionSummaryTypeDef


def get_value() -> GiVersionSummaryTypeDef:
    return {
        "version": ...,
    }


# GiVersionSummaryTypeDef definition

class GiVersionSummaryTypeDef(TypedDict):
    version: NotRequired[str],
```


## InitializeServiceInputTypeDef

```python
# InitializeServiceInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import InitializeServiceInputTypeDef


def get_value() -> InitializeServiceInputTypeDef:
    return {
        "ociIdentityDomain": ...,
    }


# InitializeServiceInputTypeDef definition

class InitializeServiceInputTypeDef(TypedDict):
    ociIdentityDomain: NotRequired[bool],
```


## KmsAccessTypeDef

```python
# KmsAccessTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import KmsAccessTypeDef


def get_value() -> KmsAccessTypeDef:
    return {
        "status": ...,
    }


# KmsAccessTypeDef definition

class KmsAccessTypeDef(TypedDict):
    status: NotRequired[ManagedResourceStatusType],  # (1)
    ipv4Addresses: NotRequired[list[str]],
    domainName: NotRequired[str],
    kmsPolicyDocument: NotRequired[str],
```

1. See [:material-code-brackets: ManagedResourceStatusType](./literals.md#managedresourcestatustype)

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import PaginatorConfigTypeDef


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


## ListAutonomousVirtualMachinesInputTypeDef

```python
# ListAutonomousVirtualMachinesInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListAutonomousVirtualMachinesInputTypeDef


def get_value() -> ListAutonomousVirtualMachinesInputTypeDef:
    return {
        "cloudAutonomousVmClusterId": ...,
    }


# ListAutonomousVirtualMachinesInputTypeDef definition

class ListAutonomousVirtualMachinesInputTypeDef(TypedDict):
    cloudAutonomousVmClusterId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListCloudAutonomousVmClustersInputTypeDef

```python
# ListCloudAutonomousVmClustersInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListCloudAutonomousVmClustersInputTypeDef


def get_value() -> ListCloudAutonomousVmClustersInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListCloudAutonomousVmClustersInputTypeDef definition

class ListCloudAutonomousVmClustersInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    cloudExadataInfrastructureId: NotRequired[str],
```


## ListCloudExadataInfrastructuresInputTypeDef

```python
# ListCloudExadataInfrastructuresInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListCloudExadataInfrastructuresInputTypeDef


def get_value() -> ListCloudExadataInfrastructuresInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListCloudExadataInfrastructuresInputTypeDef definition

class ListCloudExadataInfrastructuresInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListCloudVmClustersInputTypeDef

```python
# ListCloudVmClustersInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListCloudVmClustersInputTypeDef


def get_value() -> ListCloudVmClustersInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListCloudVmClustersInputTypeDef definition

class ListCloudVmClustersInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    cloudExadataInfrastructureId: NotRequired[str],
```


## ListDbNodesInputTypeDef

```python
# ListDbNodesInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListDbNodesInputTypeDef


def get_value() -> ListDbNodesInputTypeDef:
    return {
        "cloudVmClusterId": ...,
    }


# ListDbNodesInputTypeDef definition

class ListDbNodesInputTypeDef(TypedDict):
    cloudVmClusterId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListDbServersInputTypeDef

```python
# ListDbServersInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListDbServersInputTypeDef


def get_value() -> ListDbServersInputTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# ListDbServersInputTypeDef definition

class ListDbServersInputTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListDbSystemShapesInputTypeDef

```python
# ListDbSystemShapesInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListDbSystemShapesInputTypeDef


def get_value() -> ListDbSystemShapesInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListDbSystemShapesInputTypeDef definition

class ListDbSystemShapesInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
```


## ListGiVersionsInputTypeDef

```python
# ListGiVersionsInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListGiVersionsInputTypeDef


def get_value() -> ListGiVersionsInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListGiVersionsInputTypeDef definition

class ListGiVersionsInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    shape: NotRequired[str],
```


## ListOdbNetworksInputTypeDef

```python
# ListOdbNetworksInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListOdbNetworksInputTypeDef


def get_value() -> ListOdbNetworksInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListOdbNetworksInputTypeDef definition

class ListOdbNetworksInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListOdbPeeringConnectionsInputTypeDef

```python
# ListOdbPeeringConnectionsInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListOdbPeeringConnectionsInputTypeDef


def get_value() -> ListOdbPeeringConnectionsInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListOdbPeeringConnectionsInputTypeDef definition

class ListOdbPeeringConnectionsInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    odbNetworkId: NotRequired[str],
```


## OdbPeeringConnectionSummaryTypeDef

```python
# OdbPeeringConnectionSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import OdbPeeringConnectionSummaryTypeDef


def get_value() -> OdbPeeringConnectionSummaryTypeDef:
    return {
        "odbPeeringConnectionId": ...,
    }


# OdbPeeringConnectionSummaryTypeDef definition

class OdbPeeringConnectionSummaryTypeDef(TypedDict):
    odbPeeringConnectionId: str,
    displayName: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    odbPeeringConnectionArn: NotRequired[str],
    odbNetworkArn: NotRequired[str],
    peerNetworkArn: NotRequired[str],
    odbPeeringConnectionType: NotRequired[str],
    peerNetworkCidrs: NotRequired[list[str]],
    createdAt: NotRequired[datetime.datetime],
    percentProgress: NotRequired[float],
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)

## ListSystemVersionsInputTypeDef

```python
# ListSystemVersionsInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListSystemVersionsInputTypeDef


def get_value() -> ListSystemVersionsInputTypeDef:
    return {
        "giVersion": ...,
    }


# ListSystemVersionsInputTypeDef definition

class ListSystemVersionsInputTypeDef(TypedDict):
    giVersion: str,
    shape: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## SystemVersionSummaryTypeDef

```python
# SystemVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import SystemVersionSummaryTypeDef


def get_value() -> SystemVersionSummaryTypeDef:
    return {
        "giVersion": ...,
    }


# SystemVersionSummaryTypeDef definition

class SystemVersionSummaryTypeDef(TypedDict):
    giVersion: NotRequired[str],
    shape: NotRequired[str],
    systemVersions: NotRequired[list[str]],
```


## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```


## MonthTypeDef

```python
# MonthTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import MonthTypeDef


def get_value() -> MonthTypeDef:
    return {
        "name": ...,
    }


# MonthTypeDef definition

class MonthTypeDef(TypedDict):
    name: NotRequired[MonthNameType],  # (1)
```

1. See [:material-code-brackets: MonthNameType](./literals.md#monthnametype)

## ManagedS3BackupAccessTypeDef

```python
# ManagedS3BackupAccessTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ManagedS3BackupAccessTypeDef


def get_value() -> ManagedS3BackupAccessTypeDef:
    return {
        "status": ...,
    }


# ManagedS3BackupAccessTypeDef definition

class ManagedS3BackupAccessTypeDef(TypedDict):
    status: NotRequired[ManagedResourceStatusType],  # (1)
    ipv4Addresses: NotRequired[list[str]],
```

1. See [:material-code-brackets: ManagedResourceStatusType](./literals.md#managedresourcestatustype)

## S3AccessTypeDef

```python
# S3AccessTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import S3AccessTypeDef


def get_value() -> S3AccessTypeDef:
    return {
        "status": ...,
    }


# S3AccessTypeDef definition

class S3AccessTypeDef(TypedDict):
    status: NotRequired[ManagedResourceStatusType],  # (1)
    ipv4Addresses: NotRequired[list[str]],
    domainName: NotRequired[str],
    s3PolicyDocument: NotRequired[str],
```

1. See [:material-code-brackets: ManagedResourceStatusType](./literals.md#managedresourcestatustype)

## ServiceNetworkEndpointTypeDef

```python
# ServiceNetworkEndpointTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ServiceNetworkEndpointTypeDef


def get_value() -> ServiceNetworkEndpointTypeDef:
    return {
        "vpcEndpointId": ...,
    }


# ServiceNetworkEndpointTypeDef definition

class ServiceNetworkEndpointTypeDef(TypedDict):
    vpcEndpointId: NotRequired[str],
    vpcEndpointType: NotRequired[VpcEndpointTypeType],  # (1)
```

1. See [:material-code-brackets: VpcEndpointTypeType](./literals.md#vpcendpointtypetype)

## StsAccessTypeDef

```python
# StsAccessTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import StsAccessTypeDef


def get_value() -> StsAccessTypeDef:
    return {
        "status": ...,
    }


# StsAccessTypeDef definition

class StsAccessTypeDef(TypedDict):
    status: NotRequired[ManagedResourceStatusType],  # (1)
    ipv4Addresses: NotRequired[list[str]],
    domainName: NotRequired[str],
    stsPolicyDocument: NotRequired[str],
```

1. See [:material-code-brackets: ManagedResourceStatusType](./literals.md#managedresourcestatustype)

## ZeroEtlAccessTypeDef

```python
# ZeroEtlAccessTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ZeroEtlAccessTypeDef


def get_value() -> ZeroEtlAccessTypeDef:
    return {
        "status": ...,
    }


# ZeroEtlAccessTypeDef definition

class ZeroEtlAccessTypeDef(TypedDict):
    status: NotRequired[ManagedResourceStatusType],  # (1)
    cidr: NotRequired[str],
```

1. See [:material-code-brackets: ManagedResourceStatusType](./literals.md#managedresourcestatustype)

## OciDnsForwardingConfigTypeDef

```python
# OciDnsForwardingConfigTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import OciDnsForwardingConfigTypeDef


def get_value() -> OciDnsForwardingConfigTypeDef:
    return {
        "domainName": ...,
    }


# OciDnsForwardingConfigTypeDef definition

class OciDnsForwardingConfigTypeDef(TypedDict):
    domainName: NotRequired[str],
    ociDnsListenerIp: NotRequired[str],
```


## RebootDbNodeInputTypeDef

```python
# RebootDbNodeInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import RebootDbNodeInputTypeDef


def get_value() -> RebootDbNodeInputTypeDef:
    return {
        "cloudVmClusterId": ...,
    }


# RebootDbNodeInputTypeDef definition

class RebootDbNodeInputTypeDef(TypedDict):
    cloudVmClusterId: str,
    dbNodeId: str,
```


## StartDbNodeInputTypeDef

```python
# StartDbNodeInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import StartDbNodeInputTypeDef


def get_value() -> StartDbNodeInputTypeDef:
    return {
        "cloudVmClusterId": ...,
    }


# StartDbNodeInputTypeDef definition

class StartDbNodeInputTypeDef(TypedDict):
    cloudVmClusterId: str,
    dbNodeId: str,
```


## StopDbNodeInputTypeDef

```python
# StopDbNodeInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import StopDbNodeInputTypeDef


def get_value() -> StopDbNodeInputTypeDef:
    return {
        "cloudVmClusterId": ...,
    }


# StopDbNodeInputTypeDef definition

class StopDbNodeInputTypeDef(TypedDict):
    cloudVmClusterId: str,
    dbNodeId: str,
```


## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```


## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```


## UpdateOdbNetworkInputTypeDef

```python
# UpdateOdbNetworkInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import UpdateOdbNetworkInputTypeDef


def get_value() -> UpdateOdbNetworkInputTypeDef:
    return {
        "odbNetworkId": ...,
    }


# UpdateOdbNetworkInputTypeDef definition

class UpdateOdbNetworkInputTypeDef(TypedDict):
    odbNetworkId: str,
    displayName: NotRequired[str],
    peeredCidrsToBeAdded: NotRequired[Sequence[str]],
    peeredCidrsToBeRemoved: NotRequired[Sequence[str]],
    s3Access: NotRequired[AccessType],  # (1)
    zeroEtlAccess: NotRequired[AccessType],  # (1)
    stsAccess: NotRequired[AccessType],  # (1)
    kmsAccess: NotRequired[AccessType],  # (1)
    s3PolicyDocument: NotRequired[str],
    stsPolicyDocument: NotRequired[str],
    kmsPolicyDocument: NotRequired[str],
    crossRegionS3RestoreSourcesToEnable: NotRequired[Sequence[str]],
    crossRegionS3RestoreSourcesToDisable: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AccessType](./literals.md#accesstype)
2. See [:material-code-brackets: AccessType](./literals.md#accesstype)
3. See [:material-code-brackets: AccessType](./literals.md#accesstype)
4. See [:material-code-brackets: AccessType](./literals.md#accesstype)

## UpdateOdbPeeringConnectionInputTypeDef

```python
# UpdateOdbPeeringConnectionInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import UpdateOdbPeeringConnectionInputTypeDef


def get_value() -> UpdateOdbPeeringConnectionInputTypeDef:
    return {
        "odbPeeringConnectionId": ...,
    }


# UpdateOdbPeeringConnectionInputTypeDef definition

class UpdateOdbPeeringConnectionInputTypeDef(TypedDict):
    odbPeeringConnectionId: str,
    displayName: NotRequired[str],
    peerNetworkCidrsToBeAdded: NotRequired[Sequence[str]],
    peerNetworkCidrsToBeRemoved: NotRequired[Sequence[str]],
```


## CloudExadataInfrastructureUnallocatedResourcesTypeDef

```python
# CloudExadataInfrastructureUnallocatedResourcesTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CloudExadataInfrastructureUnallocatedResourcesTypeDef


def get_value() -> CloudExadataInfrastructureUnallocatedResourcesTypeDef:
    return {
        "cloudAutonomousVmClusters": ...,
    }


# CloudExadataInfrastructureUnallocatedResourcesTypeDef definition

class CloudExadataInfrastructureUnallocatedResourcesTypeDef(TypedDict):
    cloudAutonomousVmClusters: NotRequired[list[CloudAutonomousVmClusterResourceDetailsTypeDef]],  # (1)
    cloudExadataInfrastructureDisplayName: NotRequired[str],
    exadataStorageInTBs: NotRequired[float],
    cloudExadataInfrastructureId: NotRequired[str],
    localStorageInGBs: NotRequired[int],
    memoryInGBs: NotRequired[int],
    ocpus: NotRequired[int],
```

1. See `list[CloudAutonomousVmClusterResourceDetailsTypeDef]`

## CreateCloudVmClusterInputTypeDef

```python
# CreateCloudVmClusterInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CreateCloudVmClusterInputTypeDef


def get_value() -> CreateCloudVmClusterInputTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# CreateCloudVmClusterInputTypeDef definition

class CreateCloudVmClusterInputTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
    cpuCoreCount: int,
    displayName: str,
    giVersion: str,
    hostname: str,
    sshPublicKeys: Sequence[str],
    odbNetworkId: str,
    clusterName: NotRequired[str],
    dataCollectionOptions: NotRequired[DataCollectionOptionsTypeDef],  # (1)
    dataStorageSizeInTBs: NotRequired[float],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServers: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
    isLocalBackupEnabled: NotRequired[bool],
    isSparseDiskgroupEnabled: NotRequired[bool],
    licenseModel: NotRequired[LicenseModelType],  # (2)
    memorySizeInGBs: NotRequired[int],
    systemVersion: NotRequired[str],
    timeZone: NotRequired[str],
    clientToken: NotRequired[str],
    scanListenerPortTcp: NotRequired[int],
```

1. See [:material-code-braces: DataCollectionOptionsTypeDef](./type_defs.md#datacollectionoptionstypedef)
2. See [:material-code-brackets: LicenseModelType](./literals.md#licensemodeltype)

## CreateCloudAutonomousVmClusterOutputTypeDef

```python
# CreateCloudAutonomousVmClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CreateCloudAutonomousVmClusterOutputTypeDef


def get_value() -> CreateCloudAutonomousVmClusterOutputTypeDef:
    return {
        "displayName": ...,
    }


# CreateCloudAutonomousVmClusterOutputTypeDef definition

class CreateCloudAutonomousVmClusterOutputTypeDef(TypedDict):
    displayName: str,
    status: ResourceStatusType,  # (1)
    statusReason: str,
    cloudAutonomousVmClusterId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateCloudExadataInfrastructureOutputTypeDef

```python
# CreateCloudExadataInfrastructureOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CreateCloudExadataInfrastructureOutputTypeDef


def get_value() -> CreateCloudExadataInfrastructureOutputTypeDef:
    return {
        "displayName": ...,
    }


# CreateCloudExadataInfrastructureOutputTypeDef definition

class CreateCloudExadataInfrastructureOutputTypeDef(TypedDict):
    displayName: str,
    status: ResourceStatusType,  # (1)
    statusReason: str,
    cloudExadataInfrastructureId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateCloudVmClusterOutputTypeDef

```python
# CreateCloudVmClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CreateCloudVmClusterOutputTypeDef


def get_value() -> CreateCloudVmClusterOutputTypeDef:
    return {
        "displayName": ...,
    }


# CreateCloudVmClusterOutputTypeDef definition

class CreateCloudVmClusterOutputTypeDef(TypedDict):
    displayName: str,
    status: ResourceStatusType,  # (1)
    statusReason: str,
    cloudVmClusterId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateOdbNetworkOutputTypeDef

```python
# CreateOdbNetworkOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CreateOdbNetworkOutputTypeDef


def get_value() -> CreateOdbNetworkOutputTypeDef:
    return {
        "displayName": ...,
    }


# CreateOdbNetworkOutputTypeDef definition

class CreateOdbNetworkOutputTypeDef(TypedDict):
    displayName: str,
    status: ResourceStatusType,  # (1)
    statusReason: str,
    odbNetworkId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateOdbPeeringConnectionOutputTypeDef

```python
# CreateOdbPeeringConnectionOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CreateOdbPeeringConnectionOutputTypeDef


def get_value() -> CreateOdbPeeringConnectionOutputTypeDef:
    return {
        "displayName": ...,
    }


# CreateOdbPeeringConnectionOutputTypeDef definition

class CreateOdbPeeringConnectionOutputTypeDef(TypedDict):
    displayName: str,
    status: ResourceStatusType,  # (1)
    statusReason: str,
    odbPeeringConnectionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListAutonomousVirtualMachinesOutputTypeDef

```python
# ListAutonomousVirtualMachinesOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListAutonomousVirtualMachinesOutputTypeDef


def get_value() -> ListAutonomousVirtualMachinesOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListAutonomousVirtualMachinesOutputTypeDef definition

class ListAutonomousVirtualMachinesOutputTypeDef(TypedDict):
    autonomousVirtualMachines: list[AutonomousVirtualMachineSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[AutonomousVirtualMachineSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## RebootDbNodeOutputTypeDef

```python
# RebootDbNodeOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import RebootDbNodeOutputTypeDef


def get_value() -> RebootDbNodeOutputTypeDef:
    return {
        "dbNodeId": ...,
    }


# RebootDbNodeOutputTypeDef definition

class RebootDbNodeOutputTypeDef(TypedDict):
    dbNodeId: str,
    status: DbNodeResourceStatusType,  # (1)
    statusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DbNodeResourceStatusType](./literals.md#dbnoderesourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StartDbNodeOutputTypeDef

```python
# StartDbNodeOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import StartDbNodeOutputTypeDef


def get_value() -> StartDbNodeOutputTypeDef:
    return {
        "dbNodeId": ...,
    }


# StartDbNodeOutputTypeDef definition

class StartDbNodeOutputTypeDef(TypedDict):
    dbNodeId: str,
    status: DbNodeResourceStatusType,  # (1)
    statusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DbNodeResourceStatusType](./literals.md#dbnoderesourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StopDbNodeOutputTypeDef

```python
# StopDbNodeOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import StopDbNodeOutputTypeDef


def get_value() -> StopDbNodeOutputTypeDef:
    return {
        "dbNodeId": ...,
    }


# StopDbNodeOutputTypeDef definition

class StopDbNodeOutputTypeDef(TypedDict):
    dbNodeId: str,
    status: DbNodeResourceStatusType,  # (1)
    statusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DbNodeResourceStatusType](./literals.md#dbnoderesourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateCloudExadataInfrastructureOutputTypeDef

```python
# UpdateCloudExadataInfrastructureOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import UpdateCloudExadataInfrastructureOutputTypeDef


def get_value() -> UpdateCloudExadataInfrastructureOutputTypeDef:
    return {
        "displayName": ...,
    }


# UpdateCloudExadataInfrastructureOutputTypeDef definition

class UpdateCloudExadataInfrastructureOutputTypeDef(TypedDict):
    displayName: str,
    status: ResourceStatusType,  # (1)
    statusReason: str,
    cloudExadataInfrastructureId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateOdbNetworkOutputTypeDef

```python
# UpdateOdbNetworkOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import UpdateOdbNetworkOutputTypeDef


def get_value() -> UpdateOdbNetworkOutputTypeDef:
    return {
        "displayName": ...,
    }


# UpdateOdbNetworkOutputTypeDef definition

class UpdateOdbNetworkOutputTypeDef(TypedDict):
    displayName: str,
    status: ResourceStatusType,  # (1)
    statusReason: str,
    odbNetworkId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateOdbPeeringConnectionOutputTypeDef

```python
# UpdateOdbPeeringConnectionOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import UpdateOdbPeeringConnectionOutputTypeDef


def get_value() -> UpdateOdbPeeringConnectionOutputTypeDef:
    return {
        "displayName": ...,
    }


# UpdateOdbPeeringConnectionOutputTypeDef definition

class UpdateOdbPeeringConnectionOutputTypeDef(TypedDict):
    displayName: str,
    status: ResourceStatusType,  # (1)
    statusReason: str,
    odbPeeringConnectionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ExadataIormConfigTypeDef

```python
# ExadataIormConfigTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ExadataIormConfigTypeDef


def get_value() -> ExadataIormConfigTypeDef:
    return {
        "dbPlans": ...,
    }


# ExadataIormConfigTypeDef definition

class ExadataIormConfigTypeDef(TypedDict):
    dbPlans: NotRequired[list[DbIormConfigTypeDef]],  # (1)
    lifecycleDetails: NotRequired[str],
    lifecycleState: NotRequired[IormLifecycleStateType],  # (2)
    objective: NotRequired[ObjectiveType],  # (3)
```

1. See `list[DbIormConfigTypeDef]`
2. See [:material-code-brackets: IormLifecycleStateType](./literals.md#iormlifecyclestatetype)
3. See [:material-code-brackets: ObjectiveType](./literals.md#objectivetype)

## ListDbNodesOutputTypeDef

```python
# ListDbNodesOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListDbNodesOutputTypeDef


def get_value() -> ListDbNodesOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListDbNodesOutputTypeDef definition

class ListDbNodesOutputTypeDef(TypedDict):
    dbNodes: list[DbNodeSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[DbNodeSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetDbNodeOutputTypeDef

```python
# GetDbNodeOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetDbNodeOutputTypeDef


def get_value() -> GetDbNodeOutputTypeDef:
    return {
        "dbNode": ...,
    }


# GetDbNodeOutputTypeDef definition

class GetDbNodeOutputTypeDef(TypedDict):
    dbNode: DbNodeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DbNodeTypeDef](./type_defs.md#dbnodetypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DbServerSummaryTypeDef

```python
# DbServerSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DbServerSummaryTypeDef


def get_value() -> DbServerSummaryTypeDef:
    return {
        "dbServerId": ...,
    }


# DbServerSummaryTypeDef definition

class DbServerSummaryTypeDef(TypedDict):
    dbServerId: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    cpuCoreCount: NotRequired[int],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServerPatchingDetails: NotRequired[DbServerPatchingDetailsTypeDef],  # (2)
    displayName: NotRequired[str],
    exadataInfrastructureId: NotRequired[str],
    ocid: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    maxCpuCount: NotRequired[int],
    maxDbNodeStorageInGBs: NotRequired[int],
    maxMemoryInGBs: NotRequired[int],
    memorySizeInGBs: NotRequired[int],
    shape: NotRequired[str],
    createdAt: NotRequired[datetime.datetime],
    vmClusterIds: NotRequired[list[str]],
    computeModel: NotRequired[ComputeModelType],  # (3)
    autonomousVmClusterIds: NotRequired[list[str]],
    autonomousVirtualMachineIds: NotRequired[list[str]],
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: DbServerPatchingDetailsTypeDef](./type_defs.md#dbserverpatchingdetailstypedef)
3. See [:material-code-brackets: ComputeModelType](./literals.md#computemodeltype)

## DbServerTypeDef

```python
# DbServerTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import DbServerTypeDef


def get_value() -> DbServerTypeDef:
    return {
        "dbServerId": ...,
    }


# DbServerTypeDef definition

class DbServerTypeDef(TypedDict):
    dbServerId: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    cpuCoreCount: NotRequired[int],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServerPatchingDetails: NotRequired[DbServerPatchingDetailsTypeDef],  # (2)
    displayName: NotRequired[str],
    exadataInfrastructureId: NotRequired[str],
    ocid: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    maxCpuCount: NotRequired[int],
    maxDbNodeStorageInGBs: NotRequired[int],
    maxMemoryInGBs: NotRequired[int],
    memorySizeInGBs: NotRequired[int],
    shape: NotRequired[str],
    createdAt: NotRequired[datetime.datetime],
    vmClusterIds: NotRequired[list[str]],
    computeModel: NotRequired[ComputeModelType],  # (3)
    autonomousVmClusterIds: NotRequired[list[str]],
    autonomousVirtualMachineIds: NotRequired[list[str]],
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: DbServerPatchingDetailsTypeDef](./type_defs.md#dbserverpatchingdetailstypedef)
3. See [:material-code-brackets: ComputeModelType](./literals.md#computemodeltype)

## ListDbSystemShapesOutputTypeDef

```python
# ListDbSystemShapesOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListDbSystemShapesOutputTypeDef


def get_value() -> ListDbSystemShapesOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListDbSystemShapesOutputTypeDef definition

class ListDbSystemShapesOutputTypeDef(TypedDict):
    dbSystemShapes: list[DbSystemShapeSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[DbSystemShapeSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetOciOnboardingStatusOutputTypeDef

```python
# GetOciOnboardingStatusOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetOciOnboardingStatusOutputTypeDef


def get_value() -> GetOciOnboardingStatusOutputTypeDef:
    return {
        "status": ...,
    }


# GetOciOnboardingStatusOutputTypeDef definition

class GetOciOnboardingStatusOutputTypeDef(TypedDict):
    status: OciOnboardingStatusType,  # (1)
    existingTenancyActivationLink: str,
    newTenancyActivationLink: str,
    ociIdentityDomain: OciIdentityDomainTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: OciOnboardingStatusType](./literals.md#ocionboardingstatustype)
2. See [:material-code-braces: OciIdentityDomainTypeDef](./type_defs.md#ociidentitydomaintypedef)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetOdbPeeringConnectionOutputTypeDef

```python
# GetOdbPeeringConnectionOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetOdbPeeringConnectionOutputTypeDef


def get_value() -> GetOdbPeeringConnectionOutputTypeDef:
    return {
        "odbPeeringConnection": ...,
    }


# GetOdbPeeringConnectionOutputTypeDef definition

class GetOdbPeeringConnectionOutputTypeDef(TypedDict):
    odbPeeringConnection: OdbPeeringConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OdbPeeringConnectionTypeDef](./type_defs.md#odbpeeringconnectiontypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListGiVersionsOutputTypeDef

```python
# ListGiVersionsOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListGiVersionsOutputTypeDef


def get_value() -> ListGiVersionsOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListGiVersionsOutputTypeDef definition

class ListGiVersionsOutputTypeDef(TypedDict):
    giVersions: list[GiVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[GiVersionSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListAutonomousVirtualMachinesInputPaginateTypeDef

```python
# ListAutonomousVirtualMachinesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListAutonomousVirtualMachinesInputPaginateTypeDef


def get_value() -> ListAutonomousVirtualMachinesInputPaginateTypeDef:
    return {
        "cloudAutonomousVmClusterId": ...,
    }


# ListAutonomousVirtualMachinesInputPaginateTypeDef definition

class ListAutonomousVirtualMachinesInputPaginateTypeDef(TypedDict):
    cloudAutonomousVmClusterId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListCloudAutonomousVmClustersInputPaginateTypeDef

```python
# ListCloudAutonomousVmClustersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListCloudAutonomousVmClustersInputPaginateTypeDef


def get_value() -> ListCloudAutonomousVmClustersInputPaginateTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# ListCloudAutonomousVmClustersInputPaginateTypeDef definition

class ListCloudAutonomousVmClustersInputPaginateTypeDef(TypedDict):
    cloudExadataInfrastructureId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListCloudExadataInfrastructuresInputPaginateTypeDef

```python
# ListCloudExadataInfrastructuresInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListCloudExadataInfrastructuresInputPaginateTypeDef


def get_value() -> ListCloudExadataInfrastructuresInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListCloudExadataInfrastructuresInputPaginateTypeDef definition

class ListCloudExadataInfrastructuresInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListCloudVmClustersInputPaginateTypeDef

```python
# ListCloudVmClustersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListCloudVmClustersInputPaginateTypeDef


def get_value() -> ListCloudVmClustersInputPaginateTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# ListCloudVmClustersInputPaginateTypeDef definition

class ListCloudVmClustersInputPaginateTypeDef(TypedDict):
    cloudExadataInfrastructureId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListDbNodesInputPaginateTypeDef

```python
# ListDbNodesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListDbNodesInputPaginateTypeDef


def get_value() -> ListDbNodesInputPaginateTypeDef:
    return {
        "cloudVmClusterId": ...,
    }


# ListDbNodesInputPaginateTypeDef definition

class ListDbNodesInputPaginateTypeDef(TypedDict):
    cloudVmClusterId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListDbServersInputPaginateTypeDef

```python
# ListDbServersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListDbServersInputPaginateTypeDef


def get_value() -> ListDbServersInputPaginateTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# ListDbServersInputPaginateTypeDef definition

class ListDbServersInputPaginateTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListDbSystemShapesInputPaginateTypeDef

```python
# ListDbSystemShapesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListDbSystemShapesInputPaginateTypeDef


def get_value() -> ListDbSystemShapesInputPaginateTypeDef:
    return {
        "availabilityZone": ...,
    }


# ListDbSystemShapesInputPaginateTypeDef definition

class ListDbSystemShapesInputPaginateTypeDef(TypedDict):
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListGiVersionsInputPaginateTypeDef

```python
# ListGiVersionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListGiVersionsInputPaginateTypeDef


def get_value() -> ListGiVersionsInputPaginateTypeDef:
    return {
        "shape": ...,
    }


# ListGiVersionsInputPaginateTypeDef definition

class ListGiVersionsInputPaginateTypeDef(TypedDict):
    shape: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListOdbNetworksInputPaginateTypeDef

```python
# ListOdbNetworksInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListOdbNetworksInputPaginateTypeDef


def get_value() -> ListOdbNetworksInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListOdbNetworksInputPaginateTypeDef definition

class ListOdbNetworksInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListOdbPeeringConnectionsInputPaginateTypeDef

```python
# ListOdbPeeringConnectionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListOdbPeeringConnectionsInputPaginateTypeDef


def get_value() -> ListOdbPeeringConnectionsInputPaginateTypeDef:
    return {
        "odbNetworkId": ...,
    }


# ListOdbPeeringConnectionsInputPaginateTypeDef definition

class ListOdbPeeringConnectionsInputPaginateTypeDef(TypedDict):
    odbNetworkId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListSystemVersionsInputPaginateTypeDef

```python
# ListSystemVersionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListSystemVersionsInputPaginateTypeDef


def get_value() -> ListSystemVersionsInputPaginateTypeDef:
    return {
        "giVersion": ...,
    }


# ListSystemVersionsInputPaginateTypeDef definition

class ListSystemVersionsInputPaginateTypeDef(TypedDict):
    giVersion: str,
    shape: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListOdbPeeringConnectionsOutputTypeDef

```python
# ListOdbPeeringConnectionsOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListOdbPeeringConnectionsOutputTypeDef


def get_value() -> ListOdbPeeringConnectionsOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListOdbPeeringConnectionsOutputTypeDef definition

class ListOdbPeeringConnectionsOutputTypeDef(TypedDict):
    odbPeeringConnections: list[OdbPeeringConnectionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[OdbPeeringConnectionSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListSystemVersionsOutputTypeDef

```python
# ListSystemVersionsOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListSystemVersionsOutputTypeDef


def get_value() -> ListSystemVersionsOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListSystemVersionsOutputTypeDef definition

class ListSystemVersionsOutputTypeDef(TypedDict):
    systemVersions: list[SystemVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[SystemVersionSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## MaintenanceWindowOutputTypeDef

```python
# MaintenanceWindowOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import MaintenanceWindowOutputTypeDef


def get_value() -> MaintenanceWindowOutputTypeDef:
    return {
        "customActionTimeoutInMins": ...,
    }


# MaintenanceWindowOutputTypeDef definition

class MaintenanceWindowOutputTypeDef(TypedDict):
    customActionTimeoutInMins: NotRequired[int],
    daysOfWeek: NotRequired[list[DayOfWeekTypeDef]],  # (1)
    hoursOfDay: NotRequired[list[int]],
    isCustomActionTimeoutEnabled: NotRequired[bool],
    leadTimeInWeeks: NotRequired[int],
    months: NotRequired[list[MonthTypeDef]],  # (2)
    patchingMode: NotRequired[PatchingModeTypeType],  # (3)
    preference: NotRequired[PreferenceTypeType],  # (4)
    skipRu: NotRequired[bool],
    weeksOfMonth: NotRequired[list[int]],
```

1. See `list[DayOfWeekTypeDef]`
2. See `list[MonthTypeDef]`
3. See [:material-code-brackets: PatchingModeTypeType](./literals.md#patchingmodetypetype)
4. See [:material-code-brackets: PreferenceTypeType](./literals.md#preferencetypetype)

## MaintenanceWindowTypeDef

```python
# MaintenanceWindowTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import MaintenanceWindowTypeDef


def get_value() -> MaintenanceWindowTypeDef:
    return {
        "customActionTimeoutInMins": ...,
    }


# MaintenanceWindowTypeDef definition

class MaintenanceWindowTypeDef(TypedDict):
    customActionTimeoutInMins: NotRequired[int],
    daysOfWeek: NotRequired[Sequence[DayOfWeekTypeDef]],  # (1)
    hoursOfDay: NotRequired[Sequence[int]],
    isCustomActionTimeoutEnabled: NotRequired[bool],
    leadTimeInWeeks: NotRequired[int],
    months: NotRequired[Sequence[MonthTypeDef]],  # (2)
    patchingMode: NotRequired[PatchingModeTypeType],  # (3)
    preference: NotRequired[PreferenceTypeType],  # (4)
    skipRu: NotRequired[bool],
    weeksOfMonth: NotRequired[Sequence[int]],
```

1. See `Sequence[DayOfWeekTypeDef]`
2. See `Sequence[MonthTypeDef]`
3. See [:material-code-brackets: PatchingModeTypeType](./literals.md#patchingmodetypetype)
4. See [:material-code-brackets: PreferenceTypeType](./literals.md#preferencetypetype)

## ManagedServicesTypeDef

```python
# ManagedServicesTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ManagedServicesTypeDef


def get_value() -> ManagedServicesTypeDef:
    return {
        "serviceNetworkArn": ...,
    }


# ManagedServicesTypeDef definition

class ManagedServicesTypeDef(TypedDict):
    serviceNetworkArn: NotRequired[str],
    resourceGatewayArn: NotRequired[str],
    managedServicesIpv4Cidrs: NotRequired[list[str]],
    serviceNetworkEndpoint: NotRequired[ServiceNetworkEndpointTypeDef],  # (1)
    managedS3BackupAccess: NotRequired[ManagedS3BackupAccessTypeDef],  # (2)
    zeroEtlAccess: NotRequired[ZeroEtlAccessTypeDef],  # (3)
    s3Access: NotRequired[S3AccessTypeDef],  # (4)
    stsAccess: NotRequired[StsAccessTypeDef],  # (5)
    kmsAccess: NotRequired[KmsAccessTypeDef],  # (6)
    crossRegionS3RestoreSourcesAccess: NotRequired[list[CrossRegionS3RestoreSourcesAccessTypeDef]],  # (7)
```

1. See [:material-code-braces: ServiceNetworkEndpointTypeDef](./type_defs.md#servicenetworkendpointtypedef)
2. See [:material-code-braces: ManagedS3BackupAccessTypeDef](./type_defs.md#manageds3backupaccesstypedef)
3. See [:material-code-braces: ZeroEtlAccessTypeDef](./type_defs.md#zeroetlaccesstypedef)
4. See [:material-code-braces: S3AccessTypeDef](./type_defs.md#s3accesstypedef)
5. See [:material-code-braces: StsAccessTypeDef](./type_defs.md#stsaccesstypedef)
6. See [:material-code-braces: KmsAccessTypeDef](./type_defs.md#kmsaccesstypedef)
7. See `list[CrossRegionS3RestoreSourcesAccessTypeDef]`

## GetCloudExadataInfrastructureUnallocatedResourcesOutputTypeDef

```python
# GetCloudExadataInfrastructureUnallocatedResourcesOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetCloudExadataInfrastructureUnallocatedResourcesOutputTypeDef


def get_value() -> GetCloudExadataInfrastructureUnallocatedResourcesOutputTypeDef:
    return {
        "cloudExadataInfrastructureUnallocatedResources": ...,
    }


# GetCloudExadataInfrastructureUnallocatedResourcesOutputTypeDef definition

class GetCloudExadataInfrastructureUnallocatedResourcesOutputTypeDef(TypedDict):
    cloudExadataInfrastructureUnallocatedResources: CloudExadataInfrastructureUnallocatedResourcesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudExadataInfrastructureUnallocatedResourcesTypeDef](./type_defs.md#cloudexadatainfrastructureunallocatedresourcestypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CloudVmClusterSummaryTypeDef

```python
# CloudVmClusterSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CloudVmClusterSummaryTypeDef


def get_value() -> CloudVmClusterSummaryTypeDef:
    return {
        "cloudVmClusterId": ...,
    }


# CloudVmClusterSummaryTypeDef definition

class CloudVmClusterSummaryTypeDef(TypedDict):
    cloudVmClusterId: str,
    displayName: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    cloudVmClusterArn: NotRequired[str],
    cloudExadataInfrastructureId: NotRequired[str],
    cloudExadataInfrastructureArn: NotRequired[str],
    clusterName: NotRequired[str],
    cpuCoreCount: NotRequired[int],
    dataCollectionOptions: NotRequired[DataCollectionOptionsTypeDef],  # (2)
    dataStorageSizeInTBs: NotRequired[float],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServers: NotRequired[list[str]],
    diskRedundancy: NotRequired[DiskRedundancyType],  # (3)
    giVersion: NotRequired[str],
    hostname: NotRequired[str],
    iormConfigCache: NotRequired[ExadataIormConfigTypeDef],  # (4)
    isLocalBackupEnabled: NotRequired[bool],
    isSparseDiskgroupEnabled: NotRequired[bool],
    lastUpdateHistoryEntryId: NotRequired[str],
    licenseModel: NotRequired[LicenseModelType],  # (5)
    listenerPort: NotRequired[int],
    memorySizeInGBs: NotRequired[int],
    nodeCount: NotRequired[int],
    ocid: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    ociUrl: NotRequired[str],
    domain: NotRequired[str],
    scanDnsName: NotRequired[str],
    scanDnsRecordId: NotRequired[str],
    scanIpIds: NotRequired[list[str]],
    shape: NotRequired[str],
    sshPublicKeys: NotRequired[list[str]],
    storageSizeInGBs: NotRequired[int],
    systemVersion: NotRequired[str],
    createdAt: NotRequired[datetime.datetime],
    timeZone: NotRequired[str],
    vipIds: NotRequired[list[str]],
    odbNetworkId: NotRequired[str],
    odbNetworkArn: NotRequired[str],
    percentProgress: NotRequired[float],
    computeModel: NotRequired[ComputeModelType],  # (6)
    iamRoles: NotRequired[list[IamRoleTypeDef]],  # (7)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: DataCollectionOptionsTypeDef](./type_defs.md#datacollectionoptionstypedef)
3. See [:material-code-brackets: DiskRedundancyType](./literals.md#diskredundancytype)
4. See [:material-code-braces: ExadataIormConfigTypeDef](./type_defs.md#exadataiormconfigtypedef)
5. See [:material-code-brackets: LicenseModelType](./literals.md#licensemodeltype)
6. See [:material-code-brackets: ComputeModelType](./literals.md#computemodeltype)
7. See `list[IamRoleTypeDef]`

## CloudVmClusterTypeDef

```python
# CloudVmClusterTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CloudVmClusterTypeDef


def get_value() -> CloudVmClusterTypeDef:
    return {
        "cloudVmClusterId": ...,
    }


# CloudVmClusterTypeDef definition

class CloudVmClusterTypeDef(TypedDict):
    cloudVmClusterId: str,
    displayName: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    cloudVmClusterArn: NotRequired[str],
    cloudExadataInfrastructureId: NotRequired[str],
    cloudExadataInfrastructureArn: NotRequired[str],
    clusterName: NotRequired[str],
    cpuCoreCount: NotRequired[int],
    dataCollectionOptions: NotRequired[DataCollectionOptionsTypeDef],  # (2)
    dataStorageSizeInTBs: NotRequired[float],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServers: NotRequired[list[str]],
    diskRedundancy: NotRequired[DiskRedundancyType],  # (3)
    giVersion: NotRequired[str],
    hostname: NotRequired[str],
    iormConfigCache: NotRequired[ExadataIormConfigTypeDef],  # (4)
    isLocalBackupEnabled: NotRequired[bool],
    isSparseDiskgroupEnabled: NotRequired[bool],
    lastUpdateHistoryEntryId: NotRequired[str],
    licenseModel: NotRequired[LicenseModelType],  # (5)
    listenerPort: NotRequired[int],
    memorySizeInGBs: NotRequired[int],
    nodeCount: NotRequired[int],
    ocid: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    ociUrl: NotRequired[str],
    domain: NotRequired[str],
    scanDnsName: NotRequired[str],
    scanDnsRecordId: NotRequired[str],
    scanIpIds: NotRequired[list[str]],
    shape: NotRequired[str],
    sshPublicKeys: NotRequired[list[str]],
    storageSizeInGBs: NotRequired[int],
    systemVersion: NotRequired[str],
    createdAt: NotRequired[datetime.datetime],
    timeZone: NotRequired[str],
    vipIds: NotRequired[list[str]],
    odbNetworkId: NotRequired[str],
    odbNetworkArn: NotRequired[str],
    percentProgress: NotRequired[float],
    computeModel: NotRequired[ComputeModelType],  # (6)
    iamRoles: NotRequired[list[IamRoleTypeDef]],  # (7)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-braces: DataCollectionOptionsTypeDef](./type_defs.md#datacollectionoptionstypedef)
3. See [:material-code-brackets: DiskRedundancyType](./literals.md#diskredundancytype)
4. See [:material-code-braces: ExadataIormConfigTypeDef](./type_defs.md#exadataiormconfigtypedef)
5. See [:material-code-brackets: LicenseModelType](./literals.md#licensemodeltype)
6. See [:material-code-brackets: ComputeModelType](./literals.md#computemodeltype)
7. See `list[IamRoleTypeDef]`

## ListDbServersOutputTypeDef

```python
# ListDbServersOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListDbServersOutputTypeDef


def get_value() -> ListDbServersOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListDbServersOutputTypeDef definition

class ListDbServersOutputTypeDef(TypedDict):
    dbServers: list[DbServerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[DbServerSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetDbServerOutputTypeDef

```python
# GetDbServerOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetDbServerOutputTypeDef


def get_value() -> GetDbServerOutputTypeDef:
    return {
        "dbServer": ...,
    }


# GetDbServerOutputTypeDef definition

class GetDbServerOutputTypeDef(TypedDict):
    dbServer: DbServerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DbServerTypeDef](./type_defs.md#dbservertypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CloudAutonomousVmClusterSummaryTypeDef

```python
# CloudAutonomousVmClusterSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CloudAutonomousVmClusterSummaryTypeDef


def get_value() -> CloudAutonomousVmClusterSummaryTypeDef:
    return {
        "cloudAutonomousVmClusterId": ...,
    }


# CloudAutonomousVmClusterSummaryTypeDef definition

class CloudAutonomousVmClusterSummaryTypeDef(TypedDict):
    cloudAutonomousVmClusterId: str,
    cloudAutonomousVmClusterArn: NotRequired[str],
    odbNetworkId: NotRequired[str],
    odbNetworkArn: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    percentProgress: NotRequired[float],
    displayName: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    cloudExadataInfrastructureId: NotRequired[str],
    cloudExadataInfrastructureArn: NotRequired[str],
    autonomousDataStoragePercentage: NotRequired[float],
    autonomousDataStorageSizeInTBs: NotRequired[float],
    availableAutonomousDataStorageSizeInTBs: NotRequired[float],
    availableContainerDatabases: NotRequired[int],
    availableCpus: NotRequired[float],
    computeModel: NotRequired[ComputeModelType],  # (2)
    cpuCoreCount: NotRequired[int],
    cpuCoreCountPerNode: NotRequired[int],
    cpuPercentage: NotRequired[float],
    dataStorageSizeInGBs: NotRequired[float],
    dataStorageSizeInTBs: NotRequired[float],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServers: NotRequired[list[str]],
    description: NotRequired[str],
    domain: NotRequired[str],
    exadataStorageInTBsLowestScaledValue: NotRequired[float],
    hostname: NotRequired[str],
    ocid: NotRequired[str],
    ociUrl: NotRequired[str],
    isMtlsEnabledVmCluster: NotRequired[bool],
    licenseModel: NotRequired[LicenseModelType],  # (3)
    maintenanceWindow: NotRequired[MaintenanceWindowOutputTypeDef],  # (4)
    maxAcdsLowestScaledValue: NotRequired[int],
    memoryPerOracleComputeUnitInGBs: NotRequired[int],
    memorySizeInGBs: NotRequired[int],
    nodeCount: NotRequired[int],
    nonProvisionableAutonomousContainerDatabases: NotRequired[int],
    provisionableAutonomousContainerDatabases: NotRequired[int],
    provisionedAutonomousContainerDatabases: NotRequired[int],
    provisionedCpus: NotRequired[float],
    reclaimableCpus: NotRequired[float],
    reservedCpus: NotRequired[float],
    scanListenerPortNonTls: NotRequired[int],
    scanListenerPortTls: NotRequired[int],
    shape: NotRequired[str],
    createdAt: NotRequired[datetime.datetime],
    timeDatabaseSslCertificateExpires: NotRequired[datetime.datetime],
    timeOrdsCertificateExpires: NotRequired[datetime.datetime],
    timeZone: NotRequired[str],
    totalContainerDatabases: NotRequired[int],
    iamRoles: NotRequired[list[IamRoleTypeDef]],  # (5)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-brackets: ComputeModelType](./literals.md#computemodeltype)
3. See [:material-code-brackets: LicenseModelType](./literals.md#licensemodeltype)
4. See [:material-code-braces: MaintenanceWindowOutputTypeDef](./type_defs.md#maintenancewindowoutputtypedef)
5. See `list[IamRoleTypeDef]`

## CloudAutonomousVmClusterTypeDef

```python
# CloudAutonomousVmClusterTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CloudAutonomousVmClusterTypeDef


def get_value() -> CloudAutonomousVmClusterTypeDef:
    return {
        "cloudAutonomousVmClusterId": ...,
    }


# CloudAutonomousVmClusterTypeDef definition

class CloudAutonomousVmClusterTypeDef(TypedDict):
    cloudAutonomousVmClusterId: str,
    cloudAutonomousVmClusterArn: NotRequired[str],
    odbNetworkId: NotRequired[str],
    odbNetworkArn: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    percentProgress: NotRequired[float],
    displayName: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    cloudExadataInfrastructureId: NotRequired[str],
    cloudExadataInfrastructureArn: NotRequired[str],
    autonomousDataStoragePercentage: NotRequired[float],
    autonomousDataStorageSizeInTBs: NotRequired[float],
    availableAutonomousDataStorageSizeInTBs: NotRequired[float],
    availableContainerDatabases: NotRequired[int],
    availableCpus: NotRequired[float],
    computeModel: NotRequired[ComputeModelType],  # (2)
    cpuCoreCount: NotRequired[int],
    cpuCoreCountPerNode: NotRequired[int],
    cpuPercentage: NotRequired[float],
    dataStorageSizeInGBs: NotRequired[float],
    dataStorageSizeInTBs: NotRequired[float],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServers: NotRequired[list[str]],
    description: NotRequired[str],
    domain: NotRequired[str],
    exadataStorageInTBsLowestScaledValue: NotRequired[float],
    hostname: NotRequired[str],
    ocid: NotRequired[str],
    ociUrl: NotRequired[str],
    isMtlsEnabledVmCluster: NotRequired[bool],
    licenseModel: NotRequired[LicenseModelType],  # (3)
    maintenanceWindow: NotRequired[MaintenanceWindowOutputTypeDef],  # (4)
    maxAcdsLowestScaledValue: NotRequired[int],
    memoryPerOracleComputeUnitInGBs: NotRequired[int],
    memorySizeInGBs: NotRequired[int],
    nodeCount: NotRequired[int],
    nonProvisionableAutonomousContainerDatabases: NotRequired[int],
    provisionableAutonomousContainerDatabases: NotRequired[int],
    provisionedAutonomousContainerDatabases: NotRequired[int],
    provisionedCpus: NotRequired[float],
    reclaimableCpus: NotRequired[float],
    reservedCpus: NotRequired[float],
    scanListenerPortNonTls: NotRequired[int],
    scanListenerPortTls: NotRequired[int],
    shape: NotRequired[str],
    createdAt: NotRequired[datetime.datetime],
    timeDatabaseSslCertificateExpires: NotRequired[datetime.datetime],
    timeOrdsCertificateExpires: NotRequired[datetime.datetime],
    timeZone: NotRequired[str],
    totalContainerDatabases: NotRequired[int],
    iamRoles: NotRequired[list[IamRoleTypeDef]],  # (5)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See [:material-code-brackets: ComputeModelType](./literals.md#computemodeltype)
3. See [:material-code-brackets: LicenseModelType](./literals.md#licensemodeltype)
4. See [:material-code-braces: MaintenanceWindowOutputTypeDef](./type_defs.md#maintenancewindowoutputtypedef)
5. See `list[IamRoleTypeDef]`

## CloudExadataInfrastructureSummaryTypeDef

```python
# CloudExadataInfrastructureSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CloudExadataInfrastructureSummaryTypeDef


def get_value() -> CloudExadataInfrastructureSummaryTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# CloudExadataInfrastructureSummaryTypeDef definition

class CloudExadataInfrastructureSummaryTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
    displayName: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    cloudExadataInfrastructureArn: NotRequired[str],
    activatedStorageCount: NotRequired[int],
    additionalStorageCount: NotRequired[int],
    availableStorageSizeInGBs: NotRequired[int],
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    computeCount: NotRequired[int],
    cpuCount: NotRequired[int],
    customerContactsToSendToOCI: NotRequired[list[CustomerContactTypeDef]],  # (2)
    dataStorageSizeInTBs: NotRequired[float],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServerVersion: NotRequired[str],
    lastMaintenanceRunId: NotRequired[str],
    maintenanceWindow: NotRequired[MaintenanceWindowOutputTypeDef],  # (3)
    maxCpuCount: NotRequired[int],
    maxDataStorageInTBs: NotRequired[float],
    maxDbNodeStorageSizeInGBs: NotRequired[int],
    maxMemoryInGBs: NotRequired[int],
    memorySizeInGBs: NotRequired[int],
    monthlyDbServerVersion: NotRequired[str],
    monthlyStorageServerVersion: NotRequired[str],
    nextMaintenanceRunId: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    ociUrl: NotRequired[str],
    ocid: NotRequired[str],
    shape: NotRequired[str],
    storageCount: NotRequired[int],
    storageServerVersion: NotRequired[str],
    createdAt: NotRequired[datetime.datetime],
    totalStorageSizeInGBs: NotRequired[int],
    percentProgress: NotRequired[float],
    databaseServerType: NotRequired[str],
    storageServerType: NotRequired[str],
    computeModel: NotRequired[ComputeModelType],  # (4)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See `list[CustomerContactTypeDef]`
3. See [:material-code-braces: MaintenanceWindowOutputTypeDef](./type_defs.md#maintenancewindowoutputtypedef)
4. See [:material-code-brackets: ComputeModelType](./literals.md#computemodeltype)

## CloudExadataInfrastructureTypeDef

```python
# CloudExadataInfrastructureTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CloudExadataInfrastructureTypeDef


def get_value() -> CloudExadataInfrastructureTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# CloudExadataInfrastructureTypeDef definition

class CloudExadataInfrastructureTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
    displayName: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    cloudExadataInfrastructureArn: NotRequired[str],
    activatedStorageCount: NotRequired[int],
    additionalStorageCount: NotRequired[int],
    availableStorageSizeInGBs: NotRequired[int],
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    computeCount: NotRequired[int],
    cpuCount: NotRequired[int],
    customerContactsToSendToOCI: NotRequired[list[CustomerContactTypeDef]],  # (2)
    dataStorageSizeInTBs: NotRequired[float],
    dbNodeStorageSizeInGBs: NotRequired[int],
    dbServerVersion: NotRequired[str],
    lastMaintenanceRunId: NotRequired[str],
    maintenanceWindow: NotRequired[MaintenanceWindowOutputTypeDef],  # (3)
    maxCpuCount: NotRequired[int],
    maxDataStorageInTBs: NotRequired[float],
    maxDbNodeStorageSizeInGBs: NotRequired[int],
    maxMemoryInGBs: NotRequired[int],
    memorySizeInGBs: NotRequired[int],
    monthlyDbServerVersion: NotRequired[str],
    monthlyStorageServerVersion: NotRequired[str],
    nextMaintenanceRunId: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    ociUrl: NotRequired[str],
    ocid: NotRequired[str],
    shape: NotRequired[str],
    storageCount: NotRequired[int],
    storageServerVersion: NotRequired[str],
    createdAt: NotRequired[datetime.datetime],
    totalStorageSizeInGBs: NotRequired[int],
    percentProgress: NotRequired[float],
    databaseServerType: NotRequired[str],
    storageServerType: NotRequired[str],
    computeModel: NotRequired[ComputeModelType],  # (4)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See `list[CustomerContactTypeDef]`
3. See [:material-code-braces: MaintenanceWindowOutputTypeDef](./type_defs.md#maintenancewindowoutputtypedef)
4. See [:material-code-brackets: ComputeModelType](./literals.md#computemodeltype)

## OdbNetworkSummaryTypeDef

```python
# OdbNetworkSummaryTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import OdbNetworkSummaryTypeDef


def get_value() -> OdbNetworkSummaryTypeDef:
    return {
        "odbNetworkId": ...,
    }


# OdbNetworkSummaryTypeDef definition

class OdbNetworkSummaryTypeDef(TypedDict):
    odbNetworkId: str,
    displayName: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    odbNetworkArn: NotRequired[str],
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    clientSubnetCidr: NotRequired[str],
    backupSubnetCidr: NotRequired[str],
    customDomainName: NotRequired[str],
    defaultDnsPrefix: NotRequired[str],
    peeredCidrs: NotRequired[list[str]],
    ociNetworkAnchorId: NotRequired[str],
    ociNetworkAnchorUrl: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    ociVcnId: NotRequired[str],
    ociVcnUrl: NotRequired[str],
    ociDnsForwardingConfigs: NotRequired[list[OciDnsForwardingConfigTypeDef]],  # (2)
    createdAt: NotRequired[datetime.datetime],
    percentProgress: NotRequired[float],
    managedServices: NotRequired[ManagedServicesTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See `list[OciDnsForwardingConfigTypeDef]`
3. See [:material-code-braces: ManagedServicesTypeDef](./type_defs.md#managedservicestypedef)

## OdbNetworkTypeDef

```python
# OdbNetworkTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import OdbNetworkTypeDef


def get_value() -> OdbNetworkTypeDef:
    return {
        "odbNetworkId": ...,
    }


# OdbNetworkTypeDef definition

class OdbNetworkTypeDef(TypedDict):
    odbNetworkId: str,
    displayName: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusReason: NotRequired[str],
    odbNetworkArn: NotRequired[str],
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    clientSubnetCidr: NotRequired[str],
    backupSubnetCidr: NotRequired[str],
    customDomainName: NotRequired[str],
    defaultDnsPrefix: NotRequired[str],
    peeredCidrs: NotRequired[list[str]],
    ociNetworkAnchorId: NotRequired[str],
    ociNetworkAnchorUrl: NotRequired[str],
    ociResourceAnchorName: NotRequired[str],
    ociVcnId: NotRequired[str],
    ociVcnUrl: NotRequired[str],
    ociDnsForwardingConfigs: NotRequired[list[OciDnsForwardingConfigTypeDef]],  # (2)
    createdAt: NotRequired[datetime.datetime],
    percentProgress: NotRequired[float],
    managedServices: NotRequired[ManagedServicesTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype)
2. See `list[OciDnsForwardingConfigTypeDef]`
3. See [:material-code-braces: ManagedServicesTypeDef](./type_defs.md#managedservicestypedef)

## ListCloudVmClustersOutputTypeDef

```python
# ListCloudVmClustersOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListCloudVmClustersOutputTypeDef


def get_value() -> ListCloudVmClustersOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListCloudVmClustersOutputTypeDef definition

class ListCloudVmClustersOutputTypeDef(TypedDict):
    cloudVmClusters: list[CloudVmClusterSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[CloudVmClusterSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetCloudVmClusterOutputTypeDef

```python
# GetCloudVmClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetCloudVmClusterOutputTypeDef


def get_value() -> GetCloudVmClusterOutputTypeDef:
    return {
        "cloudVmCluster": ...,
    }


# GetCloudVmClusterOutputTypeDef definition

class GetCloudVmClusterOutputTypeDef(TypedDict):
    cloudVmCluster: CloudVmClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudVmClusterTypeDef](./type_defs.md#cloudvmclustertypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListCloudAutonomousVmClustersOutputTypeDef

```python
# ListCloudAutonomousVmClustersOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListCloudAutonomousVmClustersOutputTypeDef


def get_value() -> ListCloudAutonomousVmClustersOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListCloudAutonomousVmClustersOutputTypeDef definition

class ListCloudAutonomousVmClustersOutputTypeDef(TypedDict):
    cloudAutonomousVmClusters: list[CloudAutonomousVmClusterSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[CloudAutonomousVmClusterSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetCloudAutonomousVmClusterOutputTypeDef

```python
# GetCloudAutonomousVmClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetCloudAutonomousVmClusterOutputTypeDef


def get_value() -> GetCloudAutonomousVmClusterOutputTypeDef:
    return {
        "cloudAutonomousVmCluster": ...,
    }


# GetCloudAutonomousVmClusterOutputTypeDef definition

class GetCloudAutonomousVmClusterOutputTypeDef(TypedDict):
    cloudAutonomousVmCluster: CloudAutonomousVmClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudAutonomousVmClusterTypeDef](./type_defs.md#cloudautonomousvmclustertypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListCloudExadataInfrastructuresOutputTypeDef

```python
# ListCloudExadataInfrastructuresOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListCloudExadataInfrastructuresOutputTypeDef


def get_value() -> ListCloudExadataInfrastructuresOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListCloudExadataInfrastructuresOutputTypeDef definition

class ListCloudExadataInfrastructuresOutputTypeDef(TypedDict):
    cloudExadataInfrastructures: list[CloudExadataInfrastructureSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[CloudExadataInfrastructureSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetCloudExadataInfrastructureOutputTypeDef

```python
# GetCloudExadataInfrastructureOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetCloudExadataInfrastructureOutputTypeDef


def get_value() -> GetCloudExadataInfrastructureOutputTypeDef:
    return {
        "cloudExadataInfrastructure": ...,
    }


# GetCloudExadataInfrastructureOutputTypeDef definition

class GetCloudExadataInfrastructureOutputTypeDef(TypedDict):
    cloudExadataInfrastructure: CloudExadataInfrastructureTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudExadataInfrastructureTypeDef](./type_defs.md#cloudexadatainfrastructuretypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateCloudAutonomousVmClusterInputTypeDef

```python
# CreateCloudAutonomousVmClusterInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CreateCloudAutonomousVmClusterInputTypeDef


def get_value() -> CreateCloudAutonomousVmClusterInputTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# CreateCloudAutonomousVmClusterInputTypeDef definition

class CreateCloudAutonomousVmClusterInputTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
    odbNetworkId: str,
    displayName: str,
    autonomousDataStorageSizeInTBs: float,
    cpuCoreCountPerNode: int,
    memoryPerOracleComputeUnitInGBs: int,
    totalContainerDatabases: int,
    clientToken: NotRequired[str],
    dbServers: NotRequired[Sequence[str]],
    description: NotRequired[str],
    isMtlsEnabledVmCluster: NotRequired[bool],
    licenseModel: NotRequired[LicenseModelType],  # (1)
    maintenanceWindow: NotRequired[MaintenanceWindowUnionTypeDef],  # (2)
    scanListenerPortNonTls: NotRequired[int],
    scanListenerPortTls: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
    timeZone: NotRequired[str],
```

1. See [:material-code-brackets: LicenseModelType](./literals.md#licensemodeltype)
2. See [:material-code-braces: MaintenanceWindowUnionTypeDef](#maintenancewindowuniontypedef)

## CreateCloudExadataInfrastructureInputTypeDef

```python
# CreateCloudExadataInfrastructureInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import CreateCloudExadataInfrastructureInputTypeDef


def get_value() -> CreateCloudExadataInfrastructureInputTypeDef:
    return {
        "displayName": ...,
    }


# CreateCloudExadataInfrastructureInputTypeDef definition

class CreateCloudExadataInfrastructureInputTypeDef(TypedDict):
    displayName: str,
    shape: str,
    computeCount: int,
    storageCount: int,
    availabilityZone: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    customerContactsToSendToOCI: NotRequired[Sequence[CustomerContactTypeDef]],  # (1)
    maintenanceWindow: NotRequired[MaintenanceWindowUnionTypeDef],  # (2)
    clientToken: NotRequired[str],
    databaseServerType: NotRequired[str],
    storageServerType: NotRequired[str],
```

1. See `Sequence[CustomerContactTypeDef]`
2. See [:material-code-braces: MaintenanceWindowUnionTypeDef](#maintenancewindowuniontypedef)

## UpdateCloudExadataInfrastructureInputTypeDef

```python
# UpdateCloudExadataInfrastructureInputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import UpdateCloudExadataInfrastructureInputTypeDef


def get_value() -> UpdateCloudExadataInfrastructureInputTypeDef:
    return {
        "cloudExadataInfrastructureId": ...,
    }


# UpdateCloudExadataInfrastructureInputTypeDef definition

class UpdateCloudExadataInfrastructureInputTypeDef(TypedDict):
    cloudExadataInfrastructureId: str,
    maintenanceWindow: NotRequired[MaintenanceWindowUnionTypeDef],  # (1)
```

1. See [:material-code-braces: MaintenanceWindowUnionTypeDef](#maintenancewindowuniontypedef)

## ListOdbNetworksOutputTypeDef

```python
# ListOdbNetworksOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import ListOdbNetworksOutputTypeDef


def get_value() -> ListOdbNetworksOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListOdbNetworksOutputTypeDef definition

class ListOdbNetworksOutputTypeDef(TypedDict):
    odbNetworks: list[OdbNetworkSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[OdbNetworkSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetOdbNetworkOutputTypeDef

```python
# GetOdbNetworkOutputTypeDef TypedDict usage example

from types_aiobotocore_odb.type_defs import GetOdbNetworkOutputTypeDef


def get_value() -> GetOdbNetworkOutputTypeDef:
    return {
        "odbNetwork": ...,
    }


# GetOdbNetworkOutputTypeDef definition

class GetOdbNetworkOutputTypeDef(TypedDict):
    odbNetwork: OdbNetworkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OdbNetworkTypeDef](./type_defs.md#odbnetworktypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

