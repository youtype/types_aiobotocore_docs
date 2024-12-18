# ParallelComputingService module

> [Index](../README.md) > ParallelComputingService


!!! note ""

    Auto-generated documentation for [ParallelComputingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#parallelcomputingservice)
    type annotations stubs module [types-aiobotocore-pcs](https://pypi.org/project/types-aiobotocore-pcs/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ParallelComputingService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ParallelComputingService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[pcs]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[pcs]'

# standalone installation
python -m pip install types-aiobotocore-pcs
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-pcs
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ParallelComputingServiceClient

Type annotations and code completion for  `#!python session.create_client("pcs")` as [ParallelComputingServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#ParallelComputingService.Client)

```python
# ParallelComputingServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_pcs.client import ParallelComputingServiceClient


session = get_session()
async with session.create_client("pcs") as client:
    client: ParallelComputingServiceClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("pcs").get_paginator("...")`.

```python
# ListClustersPaginator usage example

from types_aiobotocore_pcs.paginator import ListClustersPaginator

def get_list_clusters_paginator() -> ListClustersPaginator:
    return client.get_paginator("list_clusters"))
```

- [ListClustersPaginator](./paginators.md#listclusterspaginator)
- [ListComputeNodeGroupsPaginator](./paginators.md#listcomputenodegroupspaginator)
- [ListQueuesPaginator](./paginators.md#listqueuespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ClusterStatusType usage example

from types_aiobotocore_pcs.literals import ClusterStatusType

def get_value() -> ClusterStatusType:
    return "ACTIVE"
```

- [ClusterStatusType](./literals.md#clusterstatustype)
- [ComputeNodeGroupStatusType](./literals.md#computenodegroupstatustype)
- [EndpointTypeType](./literals.md#endpointtypetype)
- [ListClustersPaginatorName](./literals.md#listclusterspaginatorname)
- [ListComputeNodeGroupsPaginatorName](./literals.md#listcomputenodegroupspaginatorname)
- [ListQueuesPaginatorName](./literals.md#listqueuespaginatorname)
- [PurchaseOptionType](./literals.md#purchaseoptiontype)
- [QueueStatusType](./literals.md#queuestatustype)
- [SchedulerTypeType](./literals.md#schedulertypetype)
- [SizeType](./literals.md#sizetype)
- [SpotAllocationStrategyType](./literals.md#spotallocationstrategytype)
- [ParallelComputingServiceServiceName](./literals.md#parallelcomputingserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [SlurmCustomSettingTypeDef](./type_defs.md#slurmcustomsettingtypedef)
- [SlurmAuthKeyTypeDef](./type_defs.md#slurmauthkeytypedef)
- [ClusterSummaryTypeDef](./type_defs.md#clustersummarytypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [ErrorInfoTypeDef](./type_defs.md#errorinfotypedef)
- [NetworkingTypeDef](./type_defs.md#networkingtypedef)
- [SchedulerTypeDef](./type_defs.md#schedulertypedef)
- [ComputeNodeGroupConfigurationTypeDef](./type_defs.md#computenodegroupconfigurationtypedef)
- [ComputeNodeGroupSummaryTypeDef](./type_defs.md#computenodegroupsummarytypedef)
- [CustomLaunchTemplateTypeDef](./type_defs.md#customlaunchtemplatetypedef)
- [InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef)
- [ScalingConfigurationTypeDef](./type_defs.md#scalingconfigurationtypedef)
- [SpotOptionsTypeDef](./type_defs.md#spotoptionstypedef)
- [NetworkingRequestTypeDef](./type_defs.md#networkingrequesttypedef)
- [SchedulerRequestTypeDef](./type_defs.md#schedulerrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ScalingConfigurationRequestTypeDef](./type_defs.md#scalingconfigurationrequesttypedef)
- [DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef)
- [DeleteComputeNodeGroupRequestRequestTypeDef](./type_defs.md#deletecomputenodegrouprequestrequesttypedef)
- [DeleteQueueRequestRequestTypeDef](./type_defs.md#deletequeuerequestrequesttypedef)
- [GetClusterRequestRequestTypeDef](./type_defs.md#getclusterrequestrequesttypedef)
- [GetComputeNodeGroupRequestRequestTypeDef](./type_defs.md#getcomputenodegrouprequestrequesttypedef)
- [GetQueueRequestRequestTypeDef](./type_defs.md#getqueuerequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef)
- [ListComputeNodeGroupsRequestRequestTypeDef](./type_defs.md#listcomputenodegroupsrequestrequesttypedef)
- [ListQueuesRequestRequestTypeDef](./type_defs.md#listqueuesrequestrequesttypedef)
- [QueueSummaryTypeDef](./type_defs.md#queuesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RegisterComputeNodeGroupInstanceRequestRequestTypeDef](./type_defs.md#registercomputenodegroupinstancerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [ClusterSlurmConfigurationRequestTypeDef](./type_defs.md#clusterslurmconfigurationrequesttypedef)
- [ComputeNodeGroupSlurmConfigurationRequestTypeDef](./type_defs.md#computenodegroupslurmconfigurationrequesttypedef)
- [ComputeNodeGroupSlurmConfigurationTypeDef](./type_defs.md#computenodegroupslurmconfigurationtypedef)
- [UpdateComputeNodeGroupSlurmConfigurationRequestTypeDef](./type_defs.md#updatecomputenodegroupslurmconfigurationrequesttypedef)
- [ClusterSlurmConfigurationTypeDef](./type_defs.md#clusterslurmconfigurationtypedef)
- [CreateQueueRequestRequestTypeDef](./type_defs.md#createqueuerequestrequesttypedef)
- [QueueTypeDef](./type_defs.md#queuetypedef)
- [UpdateQueueRequestRequestTypeDef](./type_defs.md#updatequeuerequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)
- [ListComputeNodeGroupsResponseTypeDef](./type_defs.md#listcomputenodegroupsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [RegisterComputeNodeGroupInstanceResponseTypeDef](./type_defs.md#registercomputenodegroupinstanceresponsetypedef)
- [ListClustersRequestListClustersPaginateTypeDef](./type_defs.md#listclustersrequestlistclusterspaginatetypedef)
- [ListComputeNodeGroupsRequestListComputeNodeGroupsPaginateTypeDef](./type_defs.md#listcomputenodegroupsrequestlistcomputenodegroupspaginatetypedef)
- [ListQueuesRequestListQueuesPaginateTypeDef](./type_defs.md#listqueuesrequestlistqueuespaginatetypedef)
- [ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef)
- [CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef)
- [CreateComputeNodeGroupRequestRequestTypeDef](./type_defs.md#createcomputenodegrouprequestrequesttypedef)
- [ComputeNodeGroupTypeDef](./type_defs.md#computenodegrouptypedef)
- [UpdateComputeNodeGroupRequestRequestTypeDef](./type_defs.md#updatecomputenodegrouprequestrequesttypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [CreateQueueResponseTypeDef](./type_defs.md#createqueueresponsetypedef)
- [GetQueueResponseTypeDef](./type_defs.md#getqueueresponsetypedef)
- [UpdateQueueResponseTypeDef](./type_defs.md#updatequeueresponsetypedef)
- [CreateComputeNodeGroupResponseTypeDef](./type_defs.md#createcomputenodegroupresponsetypedef)
- [GetComputeNodeGroupResponseTypeDef](./type_defs.md#getcomputenodegroupresponsetypedef)
- [UpdateComputeNodeGroupResponseTypeDef](./type_defs.md#updatecomputenodegroupresponsetypedef)
- [CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)
- [GetClusterResponseTypeDef](./type_defs.md#getclusterresponsetypedef)

