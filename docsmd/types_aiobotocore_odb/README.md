# Odb module

> [Index](../README.md) > Odb


!!! note ""

    Auto-generated documentation for [Odb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb.html#odb)
    type annotations stubs module [types-aiobotocore-odb](https://pypi.org/project/types-aiobotocore-odb/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Odb` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Odb` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[odb]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[odb]'

# standalone installation
python -m pip install types-aiobotocore-odb
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-odb
```

## Usage

Code samples can be found in [Examples](./usage.md).

## OdbClient

Type annotations and code completion for  `#!python session.create_client("odb")` as [OdbClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb.html#Odb.Client)

```python
# OdbClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.client import OdbClient


session = get_session()
async with session.create_client("odb") as client:
    client: OdbClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("odb").get_paginator("...")`.

```python
# ListAutonomousVirtualMachinesPaginator usage example

from types_aiobotocore_odb.paginator import ListAutonomousVirtualMachinesPaginator

def get_list_autonomous_virtual_machines_paginator() -> ListAutonomousVirtualMachinesPaginator:
    return client.get_paginator("list_autonomous_virtual_machines"))
```

- [ListAutonomousVirtualMachinesPaginator](./paginators.md#listautonomousvirtualmachinespaginator)
- [ListCloudAutonomousVmClustersPaginator](./paginators.md#listcloudautonomousvmclusterspaginator)
- [ListCloudExadataInfrastructuresPaginator](./paginators.md#listcloudexadatainfrastructurespaginator)
- [ListCloudVmClustersPaginator](./paginators.md#listcloudvmclusterspaginator)
- [ListDbNodesPaginator](./paginators.md#listdbnodespaginator)
- [ListDbServersPaginator](./paginators.md#listdbserverspaginator)
- [ListDbSystemShapesPaginator](./paginators.md#listdbsystemshapespaginator)
- [ListGiVersionsPaginator](./paginators.md#listgiversionspaginator)
- [ListOdbNetworksPaginator](./paginators.md#listodbnetworkspaginator)
- [ListOdbPeeringConnectionsPaginator](./paginators.md#listodbpeeringconnectionspaginator)
- [ListSystemVersionsPaginator](./paginators.md#listsystemversionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessType usage example

from types_aiobotocore_odb.literals import AccessType

def get_value() -> AccessType:
    return "DISABLED"
```

- [AccessType](./literals.md#accesstype)
- [ComputeModelType](./literals.md#computemodeltype)
- [DayOfWeekNameType](./literals.md#dayofweeknametype)
- [DbNodeMaintenanceTypeType](./literals.md#dbnodemaintenancetypetype)
- [DbNodeResourceStatusType](./literals.md#dbnoderesourcestatustype)
- [DbServerPatchingStatusType](./literals.md#dbserverpatchingstatustype)
- [DiskRedundancyType](./literals.md#diskredundancytype)
- [IamRoleStatusType](./literals.md#iamrolestatustype)
- [IormLifecycleStateType](./literals.md#iormlifecyclestatetype)
- [LicenseModelType](./literals.md#licensemodeltype)
- [ListAutonomousVirtualMachinesPaginatorName](./literals.md#listautonomousvirtualmachinespaginatorname)
- [ListCloudAutonomousVmClustersPaginatorName](./literals.md#listcloudautonomousvmclusterspaginatorname)
- [ListCloudExadataInfrastructuresPaginatorName](./literals.md#listcloudexadatainfrastructurespaginatorname)
- [ListCloudVmClustersPaginatorName](./literals.md#listcloudvmclusterspaginatorname)
- [ListDbNodesPaginatorName](./literals.md#listdbnodespaginatorname)
- [ListDbServersPaginatorName](./literals.md#listdbserverspaginatorname)
- [ListDbSystemShapesPaginatorName](./literals.md#listdbsystemshapespaginatorname)
- [ListGiVersionsPaginatorName](./literals.md#listgiversionspaginatorname)
- [ListOdbNetworksPaginatorName](./literals.md#listodbnetworkspaginatorname)
- [ListOdbPeeringConnectionsPaginatorName](./literals.md#listodbpeeringconnectionspaginatorname)
- [ListSystemVersionsPaginatorName](./literals.md#listsystemversionspaginatorname)
- [ManagedResourceStatusType](./literals.md#managedresourcestatustype)
- [MonthNameType](./literals.md#monthnametype)
- [ObjectiveType](./literals.md#objectivetype)
- [OciOnboardingStatusType](./literals.md#ocionboardingstatustype)
- [PatchingModeTypeType](./literals.md#patchingmodetypetype)
- [PreferenceTypeType](./literals.md#preferencetypetype)
- [ResourceStatusType](./literals.md#resourcestatustype)
- [ShapeTypeType](./literals.md#shapetypetype)
- [SupportedAwsIntegrationType](./literals.md#supportedawsintegrationtype)
- [VpcEndpointTypeType](./literals.md#vpcendpointtypetype)
- [OdbServiceName](./literals.md#odbservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptMarketplaceRegistrationInputTypeDef](./type_defs.md#acceptmarketplaceregistrationinputtypedef)
- [AssociateIamRoleToResourceInputTypeDef](./type_defs.md#associateiamroletoresourceinputtypedef)
- [AutonomousVirtualMachineSummaryTypeDef](./type_defs.md#autonomousvirtualmachinesummarytypedef)
- [CloudAutonomousVmClusterResourceDetailsTypeDef](./type_defs.md#cloudautonomousvmclusterresourcedetailstypedef)
- [IamRoleTypeDef](./type_defs.md#iamroletypedef)
- [CustomerContactTypeDef](./type_defs.md#customercontacttypedef)
- [DataCollectionOptionsTypeDef](./type_defs.md#datacollectionoptionstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateOdbNetworkInputTypeDef](./type_defs.md#createodbnetworkinputtypedef)
- [CreateOdbPeeringConnectionInputTypeDef](./type_defs.md#createodbpeeringconnectioninputtypedef)
- [CrossRegionS3RestoreSourcesAccessTypeDef](./type_defs.md#crossregions3restoresourcesaccesstypedef)
- [DayOfWeekTypeDef](./type_defs.md#dayofweektypedef)
- [DbIormConfigTypeDef](./type_defs.md#dbiormconfigtypedef)
- [DbNodeSummaryTypeDef](./type_defs.md#dbnodesummarytypedef)
- [DbNodeTypeDef](./type_defs.md#dbnodetypedef)
- [DbServerPatchingDetailsTypeDef](./type_defs.md#dbserverpatchingdetailstypedef)
- [DbSystemShapeSummaryTypeDef](./type_defs.md#dbsystemshapesummarytypedef)
- [DeleteCloudAutonomousVmClusterInputTypeDef](./type_defs.md#deletecloudautonomousvmclusterinputtypedef)
- [DeleteCloudExadataInfrastructureInputTypeDef](./type_defs.md#deletecloudexadatainfrastructureinputtypedef)
- [DeleteCloudVmClusterInputTypeDef](./type_defs.md#deletecloudvmclusterinputtypedef)
- [DeleteOdbNetworkInputTypeDef](./type_defs.md#deleteodbnetworkinputtypedef)
- [DeleteOdbPeeringConnectionInputTypeDef](./type_defs.md#deleteodbpeeringconnectioninputtypedef)
- [DisassociateIamRoleFromResourceInputTypeDef](./type_defs.md#disassociateiamrolefromresourceinputtypedef)
- [GetCloudAutonomousVmClusterInputTypeDef](./type_defs.md#getcloudautonomousvmclusterinputtypedef)
- [GetCloudExadataInfrastructureInputTypeDef](./type_defs.md#getcloudexadatainfrastructureinputtypedef)
- [GetCloudExadataInfrastructureUnallocatedResourcesInputTypeDef](./type_defs.md#getcloudexadatainfrastructureunallocatedresourcesinputtypedef)
- [GetCloudVmClusterInputTypeDef](./type_defs.md#getcloudvmclusterinputtypedef)
- [GetDbNodeInputTypeDef](./type_defs.md#getdbnodeinputtypedef)
- [GetDbServerInputTypeDef](./type_defs.md#getdbserverinputtypedef)
- [OciIdentityDomainTypeDef](./type_defs.md#ociidentitydomaintypedef)
- [GetOdbNetworkInputTypeDef](./type_defs.md#getodbnetworkinputtypedef)
- [GetOdbPeeringConnectionInputTypeDef](./type_defs.md#getodbpeeringconnectioninputtypedef)
- [OdbPeeringConnectionTypeDef](./type_defs.md#odbpeeringconnectiontypedef)
- [GiVersionSummaryTypeDef](./type_defs.md#giversionsummarytypedef)
- [InitializeServiceInputTypeDef](./type_defs.md#initializeserviceinputtypedef)
- [KmsAccessTypeDef](./type_defs.md#kmsaccesstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAutonomousVirtualMachinesInputTypeDef](./type_defs.md#listautonomousvirtualmachinesinputtypedef)
- [ListCloudAutonomousVmClustersInputTypeDef](./type_defs.md#listcloudautonomousvmclustersinputtypedef)
- [ListCloudExadataInfrastructuresInputTypeDef](./type_defs.md#listcloudexadatainfrastructuresinputtypedef)
- [ListCloudVmClustersInputTypeDef](./type_defs.md#listcloudvmclustersinputtypedef)
- [ListDbNodesInputTypeDef](./type_defs.md#listdbnodesinputtypedef)
- [ListDbServersInputTypeDef](./type_defs.md#listdbserversinputtypedef)
- [ListDbSystemShapesInputTypeDef](./type_defs.md#listdbsystemshapesinputtypedef)
- [ListGiVersionsInputTypeDef](./type_defs.md#listgiversionsinputtypedef)
- [ListOdbNetworksInputTypeDef](./type_defs.md#listodbnetworksinputtypedef)
- [ListOdbPeeringConnectionsInputTypeDef](./type_defs.md#listodbpeeringconnectionsinputtypedef)
- [OdbPeeringConnectionSummaryTypeDef](./type_defs.md#odbpeeringconnectionsummarytypedef)
- [ListSystemVersionsInputTypeDef](./type_defs.md#listsystemversionsinputtypedef)
- [SystemVersionSummaryTypeDef](./type_defs.md#systemversionsummarytypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [MonthTypeDef](./type_defs.md#monthtypedef)
- [ManagedS3BackupAccessTypeDef](./type_defs.md#manageds3backupaccesstypedef)
- [S3AccessTypeDef](./type_defs.md#s3accesstypedef)
- [ServiceNetworkEndpointTypeDef](./type_defs.md#servicenetworkendpointtypedef)
- [StsAccessTypeDef](./type_defs.md#stsaccesstypedef)
- [ZeroEtlAccessTypeDef](./type_defs.md#zeroetlaccesstypedef)
- [OciDnsForwardingConfigTypeDef](./type_defs.md#ocidnsforwardingconfigtypedef)
- [RebootDbNodeInputTypeDef](./type_defs.md#rebootdbnodeinputtypedef)
- [StartDbNodeInputTypeDef](./type_defs.md#startdbnodeinputtypedef)
- [StopDbNodeInputTypeDef](./type_defs.md#stopdbnodeinputtypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateOdbNetworkInputTypeDef](./type_defs.md#updateodbnetworkinputtypedef)
- [UpdateOdbPeeringConnectionInputTypeDef](./type_defs.md#updateodbpeeringconnectioninputtypedef)
- [CloudExadataInfrastructureUnallocatedResourcesTypeDef](./type_defs.md#cloudexadatainfrastructureunallocatedresourcestypedef)
- [CreateCloudVmClusterInputTypeDef](./type_defs.md#createcloudvmclusterinputtypedef)
- [CreateCloudAutonomousVmClusterOutputTypeDef](./type_defs.md#createcloudautonomousvmclusteroutputtypedef)
- [CreateCloudExadataInfrastructureOutputTypeDef](./type_defs.md#createcloudexadatainfrastructureoutputtypedef)
- [CreateCloudVmClusterOutputTypeDef](./type_defs.md#createcloudvmclusteroutputtypedef)
- [CreateOdbNetworkOutputTypeDef](./type_defs.md#createodbnetworkoutputtypedef)
- [CreateOdbPeeringConnectionOutputTypeDef](./type_defs.md#createodbpeeringconnectionoutputtypedef)
- [ListAutonomousVirtualMachinesOutputTypeDef](./type_defs.md#listautonomousvirtualmachinesoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [RebootDbNodeOutputTypeDef](./type_defs.md#rebootdbnodeoutputtypedef)
- [StartDbNodeOutputTypeDef](./type_defs.md#startdbnodeoutputtypedef)
- [StopDbNodeOutputTypeDef](./type_defs.md#stopdbnodeoutputtypedef)
- [UpdateCloudExadataInfrastructureOutputTypeDef](./type_defs.md#updatecloudexadatainfrastructureoutputtypedef)
- [UpdateOdbNetworkOutputTypeDef](./type_defs.md#updateodbnetworkoutputtypedef)
- [UpdateOdbPeeringConnectionOutputTypeDef](./type_defs.md#updateodbpeeringconnectionoutputtypedef)
- [ExadataIormConfigTypeDef](./type_defs.md#exadataiormconfigtypedef)
- [ListDbNodesOutputTypeDef](./type_defs.md#listdbnodesoutputtypedef)
- [GetDbNodeOutputTypeDef](./type_defs.md#getdbnodeoutputtypedef)
- [DbServerSummaryTypeDef](./type_defs.md#dbserversummarytypedef)
- [DbServerTypeDef](./type_defs.md#dbservertypedef)
- [ListDbSystemShapesOutputTypeDef](./type_defs.md#listdbsystemshapesoutputtypedef)
- [GetOciOnboardingStatusOutputTypeDef](./type_defs.md#getocionboardingstatusoutputtypedef)
- [GetOdbPeeringConnectionOutputTypeDef](./type_defs.md#getodbpeeringconnectionoutputtypedef)
- [ListGiVersionsOutputTypeDef](./type_defs.md#listgiversionsoutputtypedef)
- [ListAutonomousVirtualMachinesInputPaginateTypeDef](./type_defs.md#listautonomousvirtualmachinesinputpaginatetypedef)
- [ListCloudAutonomousVmClustersInputPaginateTypeDef](./type_defs.md#listcloudautonomousvmclustersinputpaginatetypedef)
- [ListCloudExadataInfrastructuresInputPaginateTypeDef](./type_defs.md#listcloudexadatainfrastructuresinputpaginatetypedef)
- [ListCloudVmClustersInputPaginateTypeDef](./type_defs.md#listcloudvmclustersinputpaginatetypedef)
- [ListDbNodesInputPaginateTypeDef](./type_defs.md#listdbnodesinputpaginatetypedef)
- [ListDbServersInputPaginateTypeDef](./type_defs.md#listdbserversinputpaginatetypedef)
- [ListDbSystemShapesInputPaginateTypeDef](./type_defs.md#listdbsystemshapesinputpaginatetypedef)
- [ListGiVersionsInputPaginateTypeDef](./type_defs.md#listgiversionsinputpaginatetypedef)
- [ListOdbNetworksInputPaginateTypeDef](./type_defs.md#listodbnetworksinputpaginatetypedef)
- [ListOdbPeeringConnectionsInputPaginateTypeDef](./type_defs.md#listodbpeeringconnectionsinputpaginatetypedef)
- [ListSystemVersionsInputPaginateTypeDef](./type_defs.md#listsystemversionsinputpaginatetypedef)
- [ListOdbPeeringConnectionsOutputTypeDef](./type_defs.md#listodbpeeringconnectionsoutputtypedef)
- [ListSystemVersionsOutputTypeDef](./type_defs.md#listsystemversionsoutputtypedef)
- [MaintenanceWindowOutputTypeDef](./type_defs.md#maintenancewindowoutputtypedef)
- [MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef)
- [ManagedServicesTypeDef](./type_defs.md#managedservicestypedef)
- [GetCloudExadataInfrastructureUnallocatedResourcesOutputTypeDef](./type_defs.md#getcloudexadatainfrastructureunallocatedresourcesoutputtypedef)
- [CloudVmClusterSummaryTypeDef](./type_defs.md#cloudvmclustersummarytypedef)
- [CloudVmClusterTypeDef](./type_defs.md#cloudvmclustertypedef)
- [ListDbServersOutputTypeDef](./type_defs.md#listdbserversoutputtypedef)
- [GetDbServerOutputTypeDef](./type_defs.md#getdbserveroutputtypedef)
- [CloudAutonomousVmClusterSummaryTypeDef](./type_defs.md#cloudautonomousvmclustersummarytypedef)
- [CloudAutonomousVmClusterTypeDef](./type_defs.md#cloudautonomousvmclustertypedef)
- [CloudExadataInfrastructureSummaryTypeDef](./type_defs.md#cloudexadatainfrastructuresummarytypedef)
- [CloudExadataInfrastructureTypeDef](./type_defs.md#cloudexadatainfrastructuretypedef)
- [MaintenanceWindowUnionTypeDef](./type_defs.md#maintenancewindowuniontypedef)
- [OdbNetworkSummaryTypeDef](./type_defs.md#odbnetworksummarytypedef)
- [OdbNetworkTypeDef](./type_defs.md#odbnetworktypedef)
- [ListCloudVmClustersOutputTypeDef](./type_defs.md#listcloudvmclustersoutputtypedef)
- [GetCloudVmClusterOutputTypeDef](./type_defs.md#getcloudvmclusteroutputtypedef)
- [ListCloudAutonomousVmClustersOutputTypeDef](./type_defs.md#listcloudautonomousvmclustersoutputtypedef)
- [GetCloudAutonomousVmClusterOutputTypeDef](./type_defs.md#getcloudautonomousvmclusteroutputtypedef)
- [ListCloudExadataInfrastructuresOutputTypeDef](./type_defs.md#listcloudexadatainfrastructuresoutputtypedef)
- [GetCloudExadataInfrastructureOutputTypeDef](./type_defs.md#getcloudexadatainfrastructureoutputtypedef)
- [CreateCloudAutonomousVmClusterInputTypeDef](./type_defs.md#createcloudautonomousvmclusterinputtypedef)
- [CreateCloudExadataInfrastructureInputTypeDef](./type_defs.md#createcloudexadatainfrastructureinputtypedef)
- [UpdateCloudExadataInfrastructureInputTypeDef](./type_defs.md#updatecloudexadatainfrastructureinputtypedef)
- [ListOdbNetworksOutputTypeDef](./type_defs.md#listodbnetworksoutputtypedef)
- [GetOdbNetworkOutputTypeDef](./type_defs.md#getodbnetworkoutputtypedef)

