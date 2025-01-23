# NeptuneGraph module

> [Index](../README.md) > NeptuneGraph


!!! note ""

    Auto-generated documentation for [NeptuneGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#neptunegraph)
    type annotations stubs module [types-aiobotocore-neptune-graph](https://pypi.org/project/types-aiobotocore-neptune-graph/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `NeptuneGraph` service.
1. Use provided commands to install generated packages.



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
# ListExportTasksPaginator usage example

from types_aiobotocore_neptune_graph.paginator import ListExportTasksPaginator

def get_list_export_tasks_paginator() -> ListExportTasksPaginator:
    return client.get_paginator("list_export_tasks"))
```

- [ListExportTasksPaginator](./paginators.md#listexporttaskspaginator)
- [ListGraphSnapshotsPaginator](./paginators.md#listgraphsnapshotspaginator)
- [ListGraphsPaginator](./paginators.md#listgraphspaginator)
- [ListImportTasksPaginator](./paginators.md#listimporttaskspaginator)
- [ListPrivateGraphEndpointsPaginator](./paginators.md#listprivategraphendpointspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("neptune-graph").get_waiter("...")`.

```python
# ExportTaskCancelledWaiter usage example

from types_aiobotocore_neptune_graph.waiter import ExportTaskCancelledWaiter

def get_export_task_cancelled_waiter() -> ExportTaskCancelledWaiter:
    return Session().client("neptune-graph").get_waiter("export_task_cancelled")
```

- [ExportTaskCancelledWaiter](./waiters.md#exporttaskcancelledwaiter)
- [ExportTaskSuccessfulWaiter](./waiters.md#exporttasksuccessfulwaiter)
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
- [ExportFormatType](./literals.md#exportformattype)
- [ExportTaskCancelledWaiterName](./literals.md#exporttaskcancelledwaitername)
- [ExportTaskStatusType](./literals.md#exporttaskstatustype)
- [ExportTaskSuccessfulWaiterName](./literals.md#exporttasksuccessfulwaitername)
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
- [ListExportTasksPaginatorName](./literals.md#listexporttaskspaginatorname)
- [ListGraphSnapshotsPaginatorName](./literals.md#listgraphsnapshotspaginatorname)
- [ListGraphsPaginatorName](./literals.md#listgraphspaginatorname)
- [ListImportTasksPaginatorName](./literals.md#listimporttaskspaginatorname)
- [ListPrivateGraphEndpointsPaginatorName](./literals.md#listprivategraphendpointspaginatorname)
- [MultiValueHandlingTypeType](./literals.md#multivaluehandlingtypetype)
- [ParquetTypeType](./literals.md#parquettypetype)
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

- [CancelExportTaskInputRequestTypeDef](./type_defs.md#cancelexporttaskinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CancelImportTaskInputRequestTypeDef](./type_defs.md#cancelimporttaskinputrequesttypedef)
- [CancelQueryInputRequestTypeDef](./type_defs.md#cancelqueryinputrequesttypedef)
- [VectorSearchConfigurationTypeDef](./type_defs.md#vectorsearchconfigurationtypedef)
- [CreateGraphSnapshotInputRequestTypeDef](./type_defs.md#creategraphsnapshotinputrequesttypedef)
- [CreatePrivateGraphEndpointInputRequestTypeDef](./type_defs.md#createprivategraphendpointinputrequesttypedef)
- [DeleteGraphInputRequestTypeDef](./type_defs.md#deletegraphinputrequesttypedef)
- [DeleteGraphSnapshotInputRequestTypeDef](./type_defs.md#deletegraphsnapshotinputrequesttypedef)
- [DeletePrivateGraphEndpointInputRequestTypeDef](./type_defs.md#deleteprivategraphendpointinputrequesttypedef)
- [EdgeStructureTypeDef](./type_defs.md#edgestructuretypedef)
- [ExecuteQueryInputRequestTypeDef](./type_defs.md#executequeryinputrequesttypedef)
- [ExportFilterPropertyAttributesTypeDef](./type_defs.md#exportfilterpropertyattributestypedef)
- [ExportTaskDetailsTypeDef](./type_defs.md#exporttaskdetailstypedef)
- [ExportTaskSummaryTypeDef](./type_defs.md#exporttasksummarytypedef)
- [GetExportTaskInputRequestTypeDef](./type_defs.md#getexporttaskinputrequesttypedef)
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
- [ListExportTasksInputRequestTypeDef](./type_defs.md#listexporttasksinputrequesttypedef)
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
- [CancelExportTaskOutputTypeDef](./type_defs.md#cancelexporttaskoutputtypedef)
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
- [ExportFilterElementOutputTypeDef](./type_defs.md#exportfilterelementoutputtypedef)
- [ExportFilterElementTypeDef](./type_defs.md#exportfilterelementtypedef)
- [ListExportTasksOutputTypeDef](./type_defs.md#listexporttasksoutputtypedef)
- [GetExportTaskInputWaitTypeDef](./type_defs.md#getexporttaskinputwaittypedef)
- [GetGraphInputWaitTypeDef](./type_defs.md#getgraphinputwaittypedef)
- [GetGraphSnapshotInputWaitTypeDef](./type_defs.md#getgraphsnapshotinputwaittypedef)
- [GetImportTaskInputWaitTypeDef](./type_defs.md#getimporttaskinputwaittypedef)
- [GetPrivateGraphEndpointInputWaitTypeDef](./type_defs.md#getprivategraphendpointinputwaittypedef)
- [GraphDataSummaryTypeDef](./type_defs.md#graphdatasummarytypedef)
- [ListGraphSnapshotsOutputTypeDef](./type_defs.md#listgraphsnapshotsoutputtypedef)
- [ListGraphsOutputTypeDef](./type_defs.md#listgraphsoutputtypedef)
- [ImportOptionsTypeDef](./type_defs.md#importoptionstypedef)
- [ListImportTasksOutputTypeDef](./type_defs.md#listimporttasksoutputtypedef)
- [ListExportTasksInputPaginateTypeDef](./type_defs.md#listexporttasksinputpaginatetypedef)
- [ListGraphSnapshotsInputPaginateTypeDef](./type_defs.md#listgraphsnapshotsinputpaginatetypedef)
- [ListGraphsInputPaginateTypeDef](./type_defs.md#listgraphsinputpaginatetypedef)
- [ListImportTasksInputPaginateTypeDef](./type_defs.md#listimporttasksinputpaginatetypedef)
- [ListPrivateGraphEndpointsInputPaginateTypeDef](./type_defs.md#listprivategraphendpointsinputpaginatetypedef)
- [ListPrivateGraphEndpointsOutputTypeDef](./type_defs.md#listprivategraphendpointsoutputtypedef)
- [ListQueriesOutputTypeDef](./type_defs.md#listqueriesoutputtypedef)
- [ExportFilterOutputTypeDef](./type_defs.md#exportfilteroutputtypedef)
- [ExportFilterElementUnionTypeDef](./type_defs.md#exportfilterelementuniontypedef)
- [GetGraphSummaryOutputTypeDef](./type_defs.md#getgraphsummaryoutputtypedef)
- [CreateGraphUsingImportTaskInputRequestTypeDef](./type_defs.md#creategraphusingimporttaskinputrequesttypedef)
- [CreateGraphUsingImportTaskOutputTypeDef](./type_defs.md#creategraphusingimporttaskoutputtypedef)
- [GetImportTaskOutputTypeDef](./type_defs.md#getimporttaskoutputtypedef)
- [StartImportTaskInputRequestTypeDef](./type_defs.md#startimporttaskinputrequesttypedef)
- [StartImportTaskOutputTypeDef](./type_defs.md#startimporttaskoutputtypedef)
- [GetExportTaskOutputTypeDef](./type_defs.md#getexporttaskoutputtypedef)
- [StartExportTaskOutputTypeDef](./type_defs.md#startexporttaskoutputtypedef)
- [ExportFilterTypeDef](./type_defs.md#exportfiltertypedef)
- [StartExportTaskInputRequestTypeDef](./type_defs.md#startexporttaskinputrequesttypedef)

