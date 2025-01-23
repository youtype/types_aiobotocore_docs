# DocDBElastic module

> [Index](../README.md) > DocDBElastic


!!! note ""

    Auto-generated documentation for [DocDBElastic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#docdbelastic)
    type annotations stubs module [types-aiobotocore-docdb-elastic](https://pypi.org/project/types-aiobotocore-docdb-elastic/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `DocDBElastic` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `DocDBElastic` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[docdb-elastic]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[docdb-elastic]'

# standalone installation
python -m pip install types-aiobotocore-docdb-elastic
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-docdb-elastic
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DocDBElasticClient

Type annotations and code completion for  `#!python session.create_client("docdb-elastic")` as [DocDBElasticClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Client)

```python
# DocDBElasticClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_docdb_elastic.client import DocDBElasticClient


session = get_session()
async with session.create_client("docdb-elastic") as client:
    client: DocDBElasticClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("docdb-elastic").get_paginator("...")`.

```python
# ListClusterSnapshotsPaginator usage example

from types_aiobotocore_docdb_elastic.paginator import ListClusterSnapshotsPaginator

def get_list_cluster_snapshots_paginator() -> ListClusterSnapshotsPaginator:
    return client.get_paginator("list_cluster_snapshots"))
```

- [ListClusterSnapshotsPaginator](./paginators.md#listclustersnapshotspaginator)
- [ListClustersPaginator](./paginators.md#listclusterspaginator)
- [ListPendingMaintenanceActionsPaginator](./paginators.md#listpendingmaintenanceactionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AuthType usage example

from types_aiobotocore_docdb_elastic.literals import AuthType

def get_value() -> AuthType:
    return "PLAIN_TEXT"
```

- [AuthType](./literals.md#authtype)
- [ListClusterSnapshotsPaginatorName](./literals.md#listclustersnapshotspaginatorname)
- [ListClustersPaginatorName](./literals.md#listclusterspaginatorname)
- [ListPendingMaintenanceActionsPaginatorName](./literals.md#listpendingmaintenanceactionspaginatorname)
- [OptInTypeType](./literals.md#optintypetype)
- [SnapshotTypeType](./literals.md#snapshottypetype)
- [StatusType](./literals.md#statustype)
- [DocDBElasticServiceName](./literals.md#docdbelasticservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ApplyPendingMaintenanceActionInputRequestTypeDef](./type_defs.md#applypendingmaintenanceactioninputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ClusterInListTypeDef](./type_defs.md#clusterinlisttypedef)
- [ClusterSnapshotInListTypeDef](./type_defs.md#clustersnapshotinlisttypedef)
- [ClusterSnapshotTypeDef](./type_defs.md#clustersnapshottypedef)
- [ShardTypeDef](./type_defs.md#shardtypedef)
- [CopyClusterSnapshotInputRequestTypeDef](./type_defs.md#copyclustersnapshotinputrequesttypedef)
- [CreateClusterInputRequestTypeDef](./type_defs.md#createclusterinputrequesttypedef)
- [CreateClusterSnapshotInputRequestTypeDef](./type_defs.md#createclustersnapshotinputrequesttypedef)
- [DeleteClusterInputRequestTypeDef](./type_defs.md#deleteclusterinputrequesttypedef)
- [DeleteClusterSnapshotInputRequestTypeDef](./type_defs.md#deleteclustersnapshotinputrequesttypedef)
- [GetClusterInputRequestTypeDef](./type_defs.md#getclusterinputrequesttypedef)
- [GetClusterSnapshotInputRequestTypeDef](./type_defs.md#getclustersnapshotinputrequesttypedef)
- [GetPendingMaintenanceActionInputRequestTypeDef](./type_defs.md#getpendingmaintenanceactioninputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListClusterSnapshotsInputRequestTypeDef](./type_defs.md#listclustersnapshotsinputrequesttypedef)
- [ListClustersInputRequestTypeDef](./type_defs.md#listclustersinputrequesttypedef)
- [ListPendingMaintenanceActionsInputRequestTypeDef](./type_defs.md#listpendingmaintenanceactionsinputrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PendingMaintenanceActionDetailsTypeDef](./type_defs.md#pendingmaintenanceactiondetailstypedef)
- [RestoreClusterFromSnapshotInputRequestTypeDef](./type_defs.md#restoreclusterfromsnapshotinputrequesttypedef)
- [StartClusterInputRequestTypeDef](./type_defs.md#startclusterinputrequesttypedef)
- [StopClusterInputRequestTypeDef](./type_defs.md#stopclusterinputrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateClusterInputRequestTypeDef](./type_defs.md#updateclusterinputrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef)
- [ListClusterSnapshotsOutputTypeDef](./type_defs.md#listclustersnapshotsoutputtypedef)
- [CopyClusterSnapshotOutputTypeDef](./type_defs.md#copyclustersnapshotoutputtypedef)
- [CreateClusterSnapshotOutputTypeDef](./type_defs.md#createclustersnapshotoutputtypedef)
- [DeleteClusterSnapshotOutputTypeDef](./type_defs.md#deleteclustersnapshotoutputtypedef)
- [GetClusterSnapshotOutputTypeDef](./type_defs.md#getclustersnapshotoutputtypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [ListClusterSnapshotsInputPaginateTypeDef](./type_defs.md#listclustersnapshotsinputpaginatetypedef)
- [ListClustersInputPaginateTypeDef](./type_defs.md#listclustersinputpaginatetypedef)
- [ListPendingMaintenanceActionsInputPaginateTypeDef](./type_defs.md#listpendingmaintenanceactionsinputpaginatetypedef)
- [ResourcePendingMaintenanceActionTypeDef](./type_defs.md#resourcependingmaintenanceactiontypedef)
- [CreateClusterOutputTypeDef](./type_defs.md#createclusteroutputtypedef)
- [DeleteClusterOutputTypeDef](./type_defs.md#deleteclusteroutputtypedef)
- [GetClusterOutputTypeDef](./type_defs.md#getclusteroutputtypedef)
- [RestoreClusterFromSnapshotOutputTypeDef](./type_defs.md#restoreclusterfromsnapshotoutputtypedef)
- [StartClusterOutputTypeDef](./type_defs.md#startclusteroutputtypedef)
- [StopClusterOutputTypeDef](./type_defs.md#stopclusteroutputtypedef)
- [UpdateClusterOutputTypeDef](./type_defs.md#updateclusteroutputtypedef)
- [ApplyPendingMaintenanceActionOutputTypeDef](./type_defs.md#applypendingmaintenanceactionoutputtypedef)
- [GetPendingMaintenanceActionOutputTypeDef](./type_defs.md#getpendingmaintenanceactionoutputtypedef)
- [ListPendingMaintenanceActionsOutputTypeDef](./type_defs.md#listpendingmaintenanceactionsoutputtypedef)

