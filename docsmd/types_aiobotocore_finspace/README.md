# finspace module

> [Index](../README.md) > finspace


!!! note ""

    Auto-generated documentation for [finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `finspace` service.

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

## finspaceClient

Type annotations and code completion for  `#!python session.create_client("finspace")` as [finspaceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client)

```python
# finspaceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_finspace.client import finspaceClient


session = get_session()
async with session.create_client("finspace") as client:
    client: finspaceClient
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
- [EnvironmentStatusType](./literals.md#environmentstatustype)
- [ErrorDetailsType](./literals.md#errordetailstype)
- [FederationModeType](./literals.md#federationmodetype)
- [IPAddressTypeType](./literals.md#ipaddresstypetype)
- [KxAzModeType](./literals.md#kxazmodetype)
- [KxClusterStatusType](./literals.md#kxclusterstatustype)
- [KxClusterTypeType](./literals.md#kxclustertypetype)
- [KxSavedownStorageTypeType](./literals.md#kxsavedownstoragetypetype)
- [ListKxEnvironmentsPaginatorName](./literals.md#listkxenvironmentspaginatorname)
- [dnsStatusType](./literals.md#dnsstatustype)
- [tgwStatusType](./literals.md#tgwstatustype)
- [finspaceServiceName](./literals.md#finspaceservicename)
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
- [VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef)
- [CreateKxDatabaseRequestRequestTypeDef](./type_defs.md#createkxdatabaserequestrequesttypedef)
- [CreateKxEnvironmentRequestRequestTypeDef](./type_defs.md#createkxenvironmentrequestrequesttypedef)
- [CreateKxUserRequestRequestTypeDef](./type_defs.md#createkxuserrequestrequesttypedef)
- [CustomDNSServerTypeDef](./type_defs.md#customdnsservertypedef)
- [DeleteEnvironmentRequestRequestTypeDef](./type_defs.md#deleteenvironmentrequestrequesttypedef)
- [DeleteKxClusterRequestRequestTypeDef](./type_defs.md#deletekxclusterrequestrequesttypedef)
- [DeleteKxDatabaseRequestRequestTypeDef](./type_defs.md#deletekxdatabaserequestrequesttypedef)
- [DeleteKxEnvironmentRequestRequestTypeDef](./type_defs.md#deletekxenvironmentrequestrequesttypedef)
- [DeleteKxUserRequestRequestTypeDef](./type_defs.md#deletekxuserrequestrequesttypedef)
- [GetEnvironmentRequestRequestTypeDef](./type_defs.md#getenvironmentrequestrequesttypedef)
- [GetKxChangesetRequestRequestTypeDef](./type_defs.md#getkxchangesetrequestrequesttypedef)
- [GetKxClusterRequestRequestTypeDef](./type_defs.md#getkxclusterrequestrequesttypedef)
- [GetKxConnectionStringRequestRequestTypeDef](./type_defs.md#getkxconnectionstringrequestrequesttypedef)
- [GetKxDatabaseRequestRequestTypeDef](./type_defs.md#getkxdatabaserequestrequesttypedef)
- [GetKxEnvironmentRequestRequestTypeDef](./type_defs.md#getkxenvironmentrequestrequesttypedef)
- [TransitGatewayConfigurationTypeDef](./type_defs.md#transitgatewayconfigurationtypedef)
- [GetKxUserRequestRequestTypeDef](./type_defs.md#getkxuserrequestrequesttypedef)
- [KxChangesetListEntryTypeDef](./type_defs.md#kxchangesetlistentrytypedef)
- [KxClusterTypeDef](./type_defs.md#kxclustertypedef)
- [KxDatabaseCacheConfigurationTypeDef](./type_defs.md#kxdatabasecacheconfigurationtypedef)
- [KxDatabaseListEntryTypeDef](./type_defs.md#kxdatabaselistentrytypedef)
- [KxNodeTypeDef](./type_defs.md#kxnodetypedef)
- [KxUserTypeDef](./type_defs.md#kxusertypedef)
- [ListEnvironmentsRequestRequestTypeDef](./type_defs.md#listenvironmentsrequestrequesttypedef)
- [ListKxChangesetsRequestRequestTypeDef](./type_defs.md#listkxchangesetsrequestrequesttypedef)
- [ListKxClusterNodesRequestRequestTypeDef](./type_defs.md#listkxclusternodesrequestrequesttypedef)
- [ListKxClustersRequestRequestTypeDef](./type_defs.md#listkxclustersrequestrequesttypedef)
- [ListKxDatabasesRequestRequestTypeDef](./type_defs.md#listkxdatabasesrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListKxEnvironmentsRequestRequestTypeDef](./type_defs.md#listkxenvironmentsrequestrequesttypedef)
- [ListKxUsersRequestRequestTypeDef](./type_defs.md#listkxusersrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateKxDatabaseRequestRequestTypeDef](./type_defs.md#updatekxdatabaserequestrequesttypedef)
- [UpdateKxEnvironmentRequestRequestTypeDef](./type_defs.md#updatekxenvironmentrequestrequesttypedef)
- [UpdateKxUserRequestRequestTypeDef](./type_defs.md#updatekxuserrequestrequesttypedef)
- [CreateKxChangesetRequestRequestTypeDef](./type_defs.md#createkxchangesetrequestrequesttypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [UpdateEnvironmentRequestRequestTypeDef](./type_defs.md#updateenvironmentrequestrequesttypedef)
- [CreateEnvironmentRequestRequestTypeDef](./type_defs.md#createenvironmentrequestrequesttypedef)
- [CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef)
- [CreateKxDatabaseResponseTypeDef](./type_defs.md#createkxdatabaseresponsetypedef)
- [CreateKxEnvironmentResponseTypeDef](./type_defs.md#createkxenvironmentresponsetypedef)
- [CreateKxUserResponseTypeDef](./type_defs.md#createkxuserresponsetypedef)
- [GetKxConnectionStringResponseTypeDef](./type_defs.md#getkxconnectionstringresponsetypedef)
- [GetKxDatabaseResponseTypeDef](./type_defs.md#getkxdatabaseresponsetypedef)
- [GetKxUserResponseTypeDef](./type_defs.md#getkxuserresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateKxDatabaseResponseTypeDef](./type_defs.md#updatekxdatabaseresponsetypedef)
- [UpdateKxUserResponseTypeDef](./type_defs.md#updatekxuserresponsetypedef)
- [CreateKxChangesetResponseTypeDef](./type_defs.md#createkxchangesetresponsetypedef)
- [GetKxChangesetResponseTypeDef](./type_defs.md#getkxchangesetresponsetypedef)
- [GetKxEnvironmentResponseTypeDef](./type_defs.md#getkxenvironmentresponsetypedef)
- [KxEnvironmentTypeDef](./type_defs.md#kxenvironmenttypedef)
- [UpdateKxEnvironmentNetworkRequestRequestTypeDef](./type_defs.md#updatekxenvironmentnetworkrequestrequesttypedef)
- [UpdateKxEnvironmentNetworkResponseTypeDef](./type_defs.md#updatekxenvironmentnetworkresponsetypedef)
- [UpdateKxEnvironmentResponseTypeDef](./type_defs.md#updatekxenvironmentresponsetypedef)
- [ListKxChangesetsResponseTypeDef](./type_defs.md#listkxchangesetsresponsetypedef)
- [ListKxClustersResponseTypeDef](./type_defs.md#listkxclustersresponsetypedef)
- [KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef)
- [ListKxDatabasesResponseTypeDef](./type_defs.md#listkxdatabasesresponsetypedef)
- [ListKxClusterNodesResponseTypeDef](./type_defs.md#listkxclusternodesresponsetypedef)
- [ListKxUsersResponseTypeDef](./type_defs.md#listkxusersresponsetypedef)
- [ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef](./type_defs.md#listkxenvironmentsrequestlistkxenvironmentspaginatetypedef)
- [GetEnvironmentResponseTypeDef](./type_defs.md#getenvironmentresponsetypedef)
- [ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef)
- [UpdateEnvironmentResponseTypeDef](./type_defs.md#updateenvironmentresponsetypedef)
- [ListKxEnvironmentsResponseTypeDef](./type_defs.md#listkxenvironmentsresponsetypedef)
- [CreateKxClusterRequestRequestTypeDef](./type_defs.md#createkxclusterrequestrequesttypedef)
- [CreateKxClusterResponseTypeDef](./type_defs.md#createkxclusterresponsetypedef)
- [GetKxClusterResponseTypeDef](./type_defs.md#getkxclusterresponsetypedef)
- [UpdateKxClusterDatabasesRequestRequestTypeDef](./type_defs.md#updatekxclusterdatabasesrequestrequesttypedef)

