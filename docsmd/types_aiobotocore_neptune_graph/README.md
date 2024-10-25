# NeptuneGraph module

> [Index](../README.md) > NeptuneGraph


!!! note ""

    Auto-generated documentation for [NeptuneGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph)
    type annotations stubs module [types-aiobotocore-neptune-graph](https://pypi.org/project/types-aiobotocore-neptune-graph/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `NeptuneGraph` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[neptune-graph]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[neptune-graph]'


# standalone installation
python -m pip install types-aiobotocore-neptune-graph
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-neptune-graph
```

## Usage

Code samples can be found in [Examples](./usage.md).

## NeptuneGraphClient

Type annotations and code completion for  `#!python session.create_client("neptune-graph")` as [NeptuneGraphClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#NeptuneGraph.Client)

```python
# NeptuneGraphClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_neptune_graph.client import NeptuneGraphClient


session = get_session()
async with session.create_client("neptune-graph") as client:
    client: NeptuneGraphClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("neptune-graph").get_paginator("...")`.

```python
# ListGraphSnapshotsPaginator usage example

from types_aiobotocore_neptune_graph.paginator import ListGraphSnapshotsPaginator

def get_list_graph_snapshots_paginator() -> ListGraphSnapshotsPaginator:
    return client.get_paginator("list_graph_snapshots"))
```

- [ListGraphSnapshotsPaginator](./paginators.md#listgraphsnapshotspaginator)
- [ListGraphsPaginator](./paginators.md#listgraphspaginator)
- [ListImportTasksPaginator](./paginators.md#listimporttaskspaginator)
- [ListPrivateGraphEndpointsPaginator](./paginators.md#listprivategraphendpointspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("neptune-graph").get_waiter("...")`.

```python
# GraphAvailableWaiter usage example

from types_aiobotocore_neptune_graph.waiter import GraphAvailableWaiter

def get_graph_available_waiter() -> GraphAvailableWaiter:
    return Session().client("neptune-graph").get_waiter("graph_available")
```

- [GraphAvailableWaiter](./waiters.md#graphavailablewaiter)
- [GraphDeletedWaiter](./waiters.md#graphdeletedwaiter)
- [GraphSnapshotAvailableWaiter](./waiters.md#graphsnapshotavailablewaiter)
- [GraphSnapshotDeletedWaiter](./waiters.md#graphsnapshotdeletedwaiter)
- [ImportTaskCancelledWaiter](./waiters.md#importtaskcancelledwaiter)
- [ImportTaskSuccessfulWaiter](./waiters.md#importtasksuccessfulwaiter)
- [PrivateGraphEndpointAvailableWaiter](./waiters.md#privategraphendpointavailablewaiter)
- [PrivateGraphEndpointDeletedWaiter](./waiters.md#privategraphendpointdeletedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BlankNodeHandlingType usage example

from types_aiobotocore_neptune_graph.literals import BlankNodeHandlingType

def get_value() -> BlankNodeHandlingType:
    return "convertToIri"
```

- [BlankNodeHandlingType](./literals.md#blanknodehandlingtype)
- [ExplainModeType](./literals.md#explainmodetype)
- [FormatType](./literals.md#formattype)
- [GraphAvailableWaiterName](./literals.md#graphavailablewaitername)
- [GraphDeletedWaiterName](./literals.md#graphdeletedwaitername)
- [GraphSnapshotAvailableWaiterName](./literals.md#graphsnapshotavailablewaitername)
- [GraphSnapshotDeletedWaiterName](./literals.md#graphsnapshotdeletedwaitername)
- [GraphStatusType](./literals.md#graphstatustype)
- [GraphSummaryModeType](./literals.md#graphsummarymodetype)
- [ImportTaskCancelledWaiterName](./literals.md#importtaskcancelledwaitername)
- [ImportTaskStatusType](./literals.md#importtaskstatustype)
- [ImportTaskSuccessfulWaiterName](./literals.md#importtasksuccessfulwaitername)
- [ListGraphSnapshotsPaginatorName](./literals.md#listgraphsnapshotspaginatorname)
- [ListGraphsPaginatorName](./literals.md#listgraphspaginatorname)
- [ListImportTasksPaginatorName](./literals.md#listimporttaskspaginatorname)
- [ListPrivateGraphEndpointsPaginatorName](./literals.md#listprivategraphendpointspaginatorname)
- [PlanCacheTypeType](./literals.md#plancachetypetype)
- [PrivateGraphEndpointAvailableWaiterName](./literals.md#privategraphendpointavailablewaitername)
- [PrivateGraphEndpointDeletedWaiterName](./literals.md#privategraphendpointdeletedwaitername)
- [PrivateGraphEndpointStatusType](./literals.md#privategraphendpointstatustype)
- [QueryLanguageType](./literals.md#querylanguagetype)
- [QueryStateInputType](./literals.md#querystateinputtype)
- [QueryStateType](./literals.md#querystatetype)
- [SnapshotStatusType](./literals.md#snapshotstatustype)
- [NeptuneGraphServiceName](./literals.md#neptunegraphservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CancelImportTaskInputRequestTypeDef](./type_defs.md#cancelimporttaskinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CancelQueryInputRequestTypeDef](./type_defs.md#cancelqueryinputrequesttypedef)
- [VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef)
- [CreateGraphSnapshotInputRequestTypeDef](./type_defs.md#creategraphsnapshotinputrequesttypedef)
- [CreatePrivateGraphEndpointInputRequestTypeDef](./type_defs.md#createprivategraphendpointinputrequesttypedef)
- [DeleteGraphInputRequestTypeDef](./type_defs.md#deletegraphinputrequesttypedef)
- [DeleteGraphSnapshotInputRequestTypeDef](./type_defs.md#deletegraphsnapshotinputrequesttypedef)
- [DeletePrivateGraphEndpointInputRequestTypeDef](./type_defs.md#deleteprivategraphendpointinputrequesttypedef)
- [EdgeStructureTypeDef](./type_defs.md#edgestructuretypedef)
- [ExecuteQueryInputRequestTypeDef](./type_defs.md#executequeryinputrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetGraphInputRequestTypeDef](./type_defs.md#getgraphinputrequesttypedef)
- [GetGraphSnapshotInputRequestTypeDef](./type_defs.md#getgraphsnapshotinputrequesttypedef)
- [GetGraphSummaryInputRequestTypeDef](./type_defs.md#getgraphsummaryinputrequesttypedef)
- [GetImportTaskInputRequestTypeDef](./type_defs.md#getimporttaskinputrequesttypedef)
- [ImportTaskDetailsTypeDef](./type_defs.md#importtaskdetailstypedef)
- [GetPrivateGraphEndpointInputRequestTypeDef](./type_defs.md#getprivategraphendpointinputrequesttypedef)
- [GetQueryInputRequestTypeDef](./type_defs.md#getqueryinputrequesttypedef)
- [NodeStructureTypeDef](./type_defs.md#nodestructuretypedef)
- [GraphSnapshotSummaryTypeDef](./type_defs.md#graphsnapshotsummarytypedef)
- [GraphSummaryTypeDef](./type_defs.md#graphsummarytypedef)
- [NeptuneImportOptionsTypeDef](./type_defs.md#neptuneimportoptionstypedef)
- [ImportTaskSummaryTypeDef](./type_defs.md#importtasksummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListGraphSnapshotsInputRequestTypeDef](./type_defs.md#listgraphsnapshotsinputrequesttypedef)
- [ListGraphsInputRequestTypeDef](./type_defs.md#listgraphsinputrequesttypedef)
- [ListImportTasksInputRequestTypeDef](./type_defs.md#listimporttasksinputrequesttypedef)
- [ListPrivateGraphEndpointsInputRequestTypeDef](./type_defs.md#listprivategraphendpointsinputrequesttypedef)
- [PrivateGraphEndpointSummaryTypeDef](./type_defs.md#privategraphendpointsummarytypedef)
- [ListQueriesInputRequestTypeDef](./type_defs.md#listqueriesinputrequesttypedef)
- [QuerySummaryTypeDef](./type_defs.md#querysummarytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ResetGraphInputRequestTypeDef](./type_defs.md#resetgraphinputrequesttypedef)
- [RestoreGraphFromSnapshotInputRequestTypeDef](./type_defs.md#restoregraphfromsnapshotinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateGraphInputRequestTypeDef](./type_defs.md#updategraphinputrequesttypedef)
- [CancelImportTaskOutputTypeDef](./type_defs.md#cancelimporttaskoutputtypedef)
- [CreateGraphSnapshotOutputTypeDef](./type_defs.md#creategraphsnapshotoutputtypedef)
- [CreatePrivateGraphEndpointOutputTypeDef](./type_defs.md#createprivategraphendpointoutputtypedef)
- [DeleteGraphSnapshotOutputTypeDef](./type_defs.md#deletegraphsnapshotoutputtypedef)
- [DeletePrivateGraphEndpointOutputTypeDef](./type_defs.md#deleteprivategraphendpointoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExecuteQueryOutputTypeDef](./type_defs.md#executequeryoutputtypedef)
- [GetGraphSnapshotOutputTypeDef](./type_defs.md#getgraphsnapshotoutputtypedef)
- [GetPrivateGraphEndpointOutputTypeDef](./type_defs.md#getprivategraphendpointoutputtypedef)
- [GetQueryOutputTypeDef](./type_defs.md#getqueryoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [CreateGraphInputRequestTypeDef](./type_defs.md#creategraphinputrequesttypedef)
- [CreateGraphOutputTypeDef](./type_defs.md#creategraphoutputtypedef)
- [DeleteGraphOutputTypeDef](./type_defs.md#deletegraphoutputtypedef)
- [GetGraphOutputTypeDef](./type_defs.md#getgraphoutputtypedef)
- [ResetGraphOutputTypeDef](./type_defs.md#resetgraphoutputtypedef)
- [RestoreGraphFromSnapshotOutputTypeDef](./type_defs.md#restoregraphfromsnapshotoutputtypedef)
- [UpdateGraphOutputTypeDef](./type_defs.md#updategraphoutputtypedef)
- [GetGraphInputGraphAvailableWaitTypeDef](./type_defs.md#getgraphinputgraphavailablewaittypedef)
- [GetGraphInputGraphDeletedWaitTypeDef](./type_defs.md#getgraphinputgraphdeletedwaittypedef)
- [GetGraphSnapshotInputGraphSnapshotAvailableWaitTypeDef](./type_defs.md#getgraphsnapshotinputgraphsnapshotavailablewaittypedef)
- [GetGraphSnapshotInputGraphSnapshotDeletedWaitTypeDef](./type_defs.md#getgraphsnapshotinputgraphsnapshotdeletedwaittypedef)
- [GetImportTaskInputImportTaskCancelledWaitTypeDef](./type_defs.md#getimporttaskinputimporttaskcancelledwaittypedef)
- [GetImportTaskInputImportTaskSuccessfulWaitTypeDef](./type_defs.md#getimporttaskinputimporttasksuccessfulwaittypedef)
- [GetPrivateGraphEndpointInputPrivateGraphEndpointAvailableWaitTypeDef](./type_defs.md#getprivategraphendpointinputprivategraphendpointavailablewaittypedef)
- [GetPrivateGraphEndpointInputPrivateGraphEndpointDeletedWaitTypeDef](./type_defs.md#getprivategraphendpointinputprivategraphendpointdeletedwaittypedef)
- [GraphDataSummaryTypeDef](./type_defs.md#graphdatasummarytypedef)
- [ListGraphSnapshotsOutputTypeDef](./type_defs.md#listgraphsnapshotsoutputtypedef)
- [ListGraphsOutputTypeDef](./type_defs.md#listgraphsoutputtypedef)
- [ImportOptionsTypeDef](./type_defs.md#importoptionstypedef)
- [ListImportTasksOutputTypeDef](./type_defs.md#listimporttasksoutputtypedef)
- [ListGraphSnapshotsInputListGraphSnapshotsPaginateTypeDef](./type_defs.md#listgraphsnapshotsinputlistgraphsnapshotspaginatetypedef)
- [ListGraphsInputListGraphsPaginateTypeDef](./type_defs.md#listgraphsinputlistgraphspaginatetypedef)
- [ListImportTasksInputListImportTasksPaginateTypeDef](./type_defs.md#listimporttasksinputlistimporttaskspaginatetypedef)
- [ListPrivateGraphEndpointsInputListPrivateGraphEndpointsPaginateTypeDef](./type_defs.md#listprivategraphendpointsinputlistprivategraphendpointspaginatetypedef)
- [ListPrivateGraphEndpointsOutputTypeDef](./type_defs.md#listprivategraphendpointsoutputtypedef)
- [ListQueriesOutputTypeDef](./type_defs.md#listqueriesoutputtypedef)
- [GetGraphSummaryOutputTypeDef](./type_defs.md#getgraphsummaryoutputtypedef)
- [CreateGraphUsingImportTaskInputRequestTypeDef](./type_defs.md#creategraphusingimporttaskinputrequesttypedef)
- [CreateGraphUsingImportTaskOutputTypeDef](./type_defs.md#creategraphusingimporttaskoutputtypedef)
- [GetImportTaskOutputTypeDef](./type_defs.md#getimporttaskoutputtypedef)
- [StartImportTaskInputRequestTypeDef](./type_defs.md#startimporttaskinputrequesttypedef)
- [StartImportTaskOutputTypeDef](./type_defs.md#startimporttaskoutputtypedef)

