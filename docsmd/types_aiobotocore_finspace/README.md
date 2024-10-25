# Finspace module

> [Index](../README.md) > Finspace


!!! note ""

    Auto-generated documentation for [Finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#Finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Finspace` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[finspace]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[finspace]'


# standalone installation
python -m pip install types-aiobotocore-finspace
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-finspace
```

## Usage

Code samples can be found in [Examples](./usage.md).

## FinspaceClient

Type annotations and code completion for  `#!python session.create_client("finspace")` as [FinspaceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#Finspace.Client)

```python
# FinspaceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_finspace.client import FinspaceClient


session = get_session()
async with session.create_client("finspace") as client:
    client: FinspaceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("finspace").get_paginator("...")`.

```python
# ListKxEnvironmentsPaginator usage example

from types_aiobotocore_finspace.paginator import ListKxEnvironmentsPaginator

def get_list_kx_environments_paginator() -> ListKxEnvironmentsPaginator:
    return client.get_paginator("list_kx_environments"))
```

- [ListKxEnvironmentsPaginator](./paginators.md#listkxenvironmentspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AutoScalingMetricType usage example

from types_aiobotocore_finspace.literals import AutoScalingMetricType

def get_value() -> AutoScalingMetricType:
    return "CPU_UTILIZATION_PERCENTAGE"
```

- [AutoScalingMetricType](./literals.md#autoscalingmetrictype)
- [ChangeTypeType](./literals.md#changetypetype)
- [ChangesetStatusType](./literals.md#changesetstatustype)
- [DnsStatusType](./literals.md#dnsstatustype)
- [EnvironmentStatusType](./literals.md#environmentstatustype)
- [ErrorDetailsType](./literals.md#errordetailstype)
- [FederationModeType](./literals.md#federationmodetype)
- [IPAddressTypeType](./literals.md#ipaddresstypetype)
- [KxAzModeType](./literals.md#kxazmodetype)
- [KxClusterCodeDeploymentStrategyType](./literals.md#kxclustercodedeploymentstrategytype)
- [KxClusterStatusType](./literals.md#kxclusterstatustype)
- [KxClusterTypeType](./literals.md#kxclustertypetype)
- [KxDataviewStatusType](./literals.md#kxdataviewstatustype)
- [KxDeploymentStrategyType](./literals.md#kxdeploymentstrategytype)
- [KxNAS1TypeType](./literals.md#kxnas1typetype)
- [KxNodeStatusType](./literals.md#kxnodestatustype)
- [KxSavedownStorageTypeType](./literals.md#kxsavedownstoragetypetype)
- [KxScalingGroupStatusType](./literals.md#kxscalinggroupstatustype)
- [KxVolumeStatusType](./literals.md#kxvolumestatustype)
- [KxVolumeTypeType](./literals.md#kxvolumetypetype)
- [ListKxEnvironmentsPaginatorName](./literals.md#listkxenvironmentspaginatorname)
- [RuleActionType](./literals.md#ruleactiontype)
- [TgwStatusType](./literals.md#tgwstatustype)
- [VolumeTypeType](./literals.md#volumetypetype)
- [FinspaceServiceName](./literals.md#finspaceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AutoScalingConfigurationTypeDef](./type_defs.md#autoscalingconfigurationtypedef)
- [CapacityConfigurationTypeDef](./type_defs.md#capacityconfigurationtypedef)
- [ChangeRequestTypeDef](./type_defs.md#changerequesttypedef)
- [CodeConfigurationTypeDef](./type_defs.md#codeconfigurationtypedef)
- [FederationParametersTypeDef](./type_defs.md#federationparameterstypedef)
- [SuperuserParametersTypeDef](./type_defs.md#superuserparameterstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ErrorInfoTypeDef](./type_defs.md#errorinfotypedef)
- [KxCacheStorageConfigurationTypeDef](./type_defs.md#kxcachestorageconfigurationtypedef)
- [KxCommandLineArgumentTypeDef](./type_defs.md#kxcommandlineargumenttypedef)
- [KxSavedownStorageConfigurationTypeDef](./type_defs.md#kxsavedownstorageconfigurationtypedef)
- [KxScalingGroupConfigurationTypeDef](./type_defs.md#kxscalinggroupconfigurationtypedef)
- [TickerplantLogConfigurationTypeDef](./type_defs.md#tickerplantlogconfigurationtypedef)
- [VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef)
- [TickerplantLogConfigurationOutputTypeDef](./type_defs.md#tickerplantlogconfigurationoutputtypedef)
- [VolumeTypeDef](./type_defs.md#volumetypedef)
- [VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef)
- [CreateKxDatabaseRequestRequestTypeDef](./type_defs.md#createkxdatabaserequestrequesttypedef)
- [KxDataviewSegmentConfigurationOutputTypeDef](./type_defs.md#kxdataviewsegmentconfigurationoutputtypedef)
- [CreateKxEnvironmentRequestRequestTypeDef](./type_defs.md#createkxenvironmentrequestrequesttypedef)
- [CreateKxScalingGroupRequestRequestTypeDef](./type_defs.md#createkxscalinggrouprequestrequesttypedef)
- [CreateKxUserRequestRequestTypeDef](./type_defs.md#createkxuserrequestrequesttypedef)
- [KxNAS1ConfigurationTypeDef](./type_defs.md#kxnas1configurationtypedef)
- [CustomDNSServerTypeDef](./type_defs.md#customdnsservertypedef)
- [DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef)
- [DeleteKxClusterNodeRequestRequestTypeDef](./type_defs.md#deletekxclusternoderequestrequesttypedef)
- [DeleteKxClusterRequestRequestTypeDef](./type_defs.md#deletekxclusterrequestrequesttypedef)
- [DeleteKxDatabaseRequestRequestTypeDef](./type_defs.md#deletekxdatabaserequestrequesttypedef)
- [DeleteKxDataviewRequestRequestTypeDef](./type_defs.md#deletekxdataviewrequestrequesttypedef)
- [DeleteKxEnvironmentRequestRequestTypeDef](./type_defs.md#deletekxenvironmentrequestrequesttypedef)
- [DeleteKxScalingGroupRequestRequestTypeDef](./type_defs.md#deletekxscalinggrouprequestrequesttypedef)
- [DeleteKxUserRequestRequestTypeDef](./type_defs.md#deletekxuserrequestrequesttypedef)
- [DeleteKxVolumeRequestRequestTypeDef](./type_defs.md#deletekxvolumerequestrequesttypedef)
- [FederationParametersOutputTypeDef](./type_defs.md#federationparametersoutputtypedef)
- [GetEnvironmentRequestRequestTypeDef](./type_defs.md#getenvironmentrequestrequesttypedef)
- [GetKxChangesetRequestRequestTypeDef](./type_defs.md#getkxchangesetrequestrequesttypedef)
- [GetKxClusterRequestRequestTypeDef](./type_defs.md#getkxclusterrequestrequesttypedef)
- [GetKxConnectionStringRequestRequestTypeDef](./type_defs.md#getkxconnectionstringrequestrequesttypedef)
- [GetKxDatabaseRequestRequestTypeDef](./type_defs.md#getkxdatabaserequestrequesttypedef)
- [GetKxDataviewRequestRequestTypeDef](./type_defs.md#getkxdataviewrequestrequesttypedef)
- [GetKxEnvironmentRequestRequestTypeDef](./type_defs.md#getkxenvironmentrequestrequesttypedef)
- [GetKxScalingGroupRequestRequestTypeDef](./type_defs.md#getkxscalinggrouprequestrequesttypedef)
- [GetKxUserRequestRequestTypeDef](./type_defs.md#getkxuserrequestrequesttypedef)
- [GetKxVolumeRequestRequestTypeDef](./type_defs.md#getkxvolumerequestrequesttypedef)
- [KxAttachedClusterTypeDef](./type_defs.md#kxattachedclustertypedef)
- [IcmpTypeCodeTypeDef](./type_defs.md#icmptypecodetypedef)
- [KxChangesetListEntryTypeDef](./type_defs.md#kxchangesetlistentrytypedef)
- [KxClusterCodeDeploymentConfigurationTypeDef](./type_defs.md#kxclustercodedeploymentconfigurationtypedef)
- [KxDatabaseCacheConfigurationOutputTypeDef](./type_defs.md#kxdatabasecacheconfigurationoutputtypedef)
- [KxDatabaseCacheConfigurationTypeDef](./type_defs.md#kxdatabasecacheconfigurationtypedef)
- [KxDatabaseListEntryTypeDef](./type_defs.md#kxdatabaselistentrytypedef)
- [KxDataviewSegmentConfigurationTypeDef](./type_defs.md#kxdataviewsegmentconfigurationtypedef)
- [KxDeploymentConfigurationTypeDef](./type_defs.md#kxdeploymentconfigurationtypedef)
- [KxNodeTypeDef](./type_defs.md#kxnodetypedef)
- [KxScalingGroupTypeDef](./type_defs.md#kxscalinggrouptypedef)
- [KxUserTypeDef](./type_defs.md#kxusertypedef)
- [KxVolumeTypeDef](./type_defs.md#kxvolumetypedef)
- [ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef)
- [ListKxChangesetsRequestRequestTypeDef](./type_defs.md#listkxchangesetsrequestrequesttypedef)
- [ListKxClusterNodesRequestRequestTypeDef](./type_defs.md#listkxclusternodesrequestrequesttypedef)
- [ListKxClustersRequestRequestTypeDef](./type_defs.md#listkxclustersrequestrequesttypedef)
- [ListKxDatabasesRequestRequestTypeDef](./type_defs.md#listkxdatabasesrequestrequesttypedef)
- [ListKxDataviewsRequestRequestTypeDef](./type_defs.md#listkxdataviewsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListKxEnvironmentsRequestRequestTypeDef](./type_defs.md#listkxenvironmentsrequestrequesttypedef)
- [ListKxScalingGroupsRequestRequestTypeDef](./type_defs.md#listkxscalinggroupsrequestrequesttypedef)
- [ListKxUsersRequestRequestTypeDef](./type_defs.md#listkxusersrequestrequesttypedef)
- [ListKxVolumesRequestRequestTypeDef](./type_defs.md#listkxvolumesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PortRangeTypeDef](./type_defs.md#portrangetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateKxDatabaseRequestRequestTypeDef](./type_defs.md#updatekxdatabaserequestrequesttypedef)
- [UpdateKxEnvironmentRequestRequestTypeDef](./type_defs.md#updatekxenvironmentrequestrequesttypedef)
- [UpdateKxUserRequestRequestTypeDef](./type_defs.md#updatekxuserrequestrequesttypedef)
- [CreateKxChangesetRequestRequestTypeDef](./type_defs.md#createkxchangesetrequestrequesttypedef)
- [UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef)
- [CreateEnvironmentRequestRequestTypeDef](./type_defs.md#createenvironmentrequestrequesttypedef)
- [CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef)
- [CreateKxDatabaseResponseTypeDef](./type_defs.md#createkxdatabaseresponsetypedef)
- [CreateKxEnvironmentResponseTypeDef](./type_defs.md#createkxenvironmentresponsetypedef)
- [CreateKxScalingGroupResponseTypeDef](./type_defs.md#createkxscalinggroupresponsetypedef)
- [CreateKxUserResponseTypeDef](./type_defs.md#createkxuserresponsetypedef)
- [GetKxConnectionStringResponseTypeDef](./type_defs.md#getkxconnectionstringresponsetypedef)
- [GetKxDatabaseResponseTypeDef](./type_defs.md#getkxdatabaseresponsetypedef)
- [GetKxScalingGroupResponseTypeDef](./type_defs.md#getkxscalinggroupresponsetypedef)
- [GetKxUserResponseTypeDef](./type_defs.md#getkxuserresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateKxDatabaseResponseTypeDef](./type_defs.md#updatekxdatabaseresponsetypedef)
- [UpdateKxUserResponseTypeDef](./type_defs.md#updatekxuserresponsetypedef)
- [CreateKxChangesetResponseTypeDef](./type_defs.md#createkxchangesetresponsetypedef)
- [GetKxChangesetResponseTypeDef](./type_defs.md#getkxchangesetresponsetypedef)
- [KxClusterTypeDef](./type_defs.md#kxclustertypedef)
- [CreateKxDataviewResponseTypeDef](./type_defs.md#createkxdataviewresponsetypedef)
- [KxDataviewActiveVersionTypeDef](./type_defs.md#kxdataviewactiveversiontypedef)
- [KxDataviewConfigurationOutputTypeDef](./type_defs.md#kxdataviewconfigurationoutputtypedef)
- [CreateKxVolumeRequestRequestTypeDef](./type_defs.md#createkxvolumerequestrequesttypedef)
- [CreateKxVolumeResponseTypeDef](./type_defs.md#createkxvolumeresponsetypedef)
- [UpdateKxVolumeRequestRequestTypeDef](./type_defs.md#updatekxvolumerequestrequesttypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [GetKxVolumeResponseTypeDef](./type_defs.md#getkxvolumeresponsetypedef)
- [UpdateKxVolumeResponseTypeDef](./type_defs.md#updatekxvolumeresponsetypedef)
- [ListKxChangesetsResponseTypeDef](./type_defs.md#listkxchangesetsresponsetypedef)
- [UpdateKxClusterCodeConfigurationRequestRequestTypeDef](./type_defs.md#updatekxclustercodeconfigurationrequestrequesttypedef)
- [KxDatabaseCacheConfigurationUnionTypeDef](./type_defs.md#kxdatabasecacheconfigurationuniontypedef)
- [ListKxDatabasesResponseTypeDef](./type_defs.md#listkxdatabasesresponsetypedef)
- [KxDataviewSegmentConfigurationUnionTypeDef](./type_defs.md#kxdataviewsegmentconfigurationuniontypedef)
- [UpdateKxDataviewRequestRequestTypeDef](./type_defs.md#updatekxdataviewrequestrequesttypedef)
- [ListKxClusterNodesResponseTypeDef](./type_defs.md#listkxclusternodesresponsetypedef)
- [ListKxScalingGroupsResponseTypeDef](./type_defs.md#listkxscalinggroupsresponsetypedef)
- [ListKxUsersResponseTypeDef](./type_defs.md#listkxusersresponsetypedef)
- [ListKxVolumesResponseTypeDef](./type_defs.md#listkxvolumesresponsetypedef)
- [ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef](./type_defs.md#listkxenvironmentsrequestlistkxenvironmentspaginatetypedef)
- [NetworkACLEntryTypeDef](./type_defs.md#networkaclentrytypedef)
- [ListKxClustersResponseTypeDef](./type_defs.md#listkxclustersresponsetypedef)
- [GetKxDataviewResponseTypeDef](./type_defs.md#getkxdataviewresponsetypedef)
- [KxDataviewListEntryTypeDef](./type_defs.md#kxdataviewlistentrytypedef)
- [UpdateKxDataviewResponseTypeDef](./type_defs.md#updatekxdataviewresponsetypedef)
- [KxDatabaseConfigurationOutputTypeDef](./type_defs.md#kxdatabaseconfigurationoutputtypedef)
- [GetEnvironmentResponseTypeDef](./type_defs.md#getenvironmentresponsetypedef)
- [ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef)
- [UpdateEnvironmentResponseTypeDef](./type_defs.md#updateenvironmentresponsetypedef)
- [CreateKxDataviewRequestRequestTypeDef](./type_defs.md#createkxdataviewrequestrequesttypedef)
- [KxDataviewConfigurationTypeDef](./type_defs.md#kxdataviewconfigurationtypedef)
- [TransitGatewayConfigurationOutputTypeDef](./type_defs.md#transitgatewayconfigurationoutputtypedef)
- [TransitGatewayConfigurationTypeDef](./type_defs.md#transitgatewayconfigurationtypedef)
- [ListKxDataviewsResponseTypeDef](./type_defs.md#listkxdataviewsresponsetypedef)
- [CreateKxClusterResponseTypeDef](./type_defs.md#createkxclusterresponsetypedef)
- [GetKxClusterResponseTypeDef](./type_defs.md#getkxclusterresponsetypedef)
- [KxDataviewConfigurationUnionTypeDef](./type_defs.md#kxdataviewconfigurationuniontypedef)
- [GetKxEnvironmentResponseTypeDef](./type_defs.md#getkxenvironmentresponsetypedef)
- [KxEnvironmentTypeDef](./type_defs.md#kxenvironmenttypedef)
- [UpdateKxEnvironmentNetworkResponseTypeDef](./type_defs.md#updatekxenvironmentnetworkresponsetypedef)
- [UpdateKxEnvironmentResponseTypeDef](./type_defs.md#updatekxenvironmentresponsetypedef)
- [UpdateKxEnvironmentNetworkRequestRequestTypeDef](./type_defs.md#updatekxenvironmentnetworkrequestrequesttypedef)
- [KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef)
- [ListKxEnvironmentsResponseTypeDef](./type_defs.md#listkxenvironmentsresponsetypedef)
- [KxDatabaseConfigurationUnionTypeDef](./type_defs.md#kxdatabaseconfigurationuniontypedef)
- [UpdateKxClusterDatabasesRequestRequestTypeDef](./type_defs.md#updatekxclusterdatabasesrequestrequesttypedef)
- [CreateKxClusterRequestRequestTypeDef](./type_defs.md#createkxclusterrequestrequesttypedef)

