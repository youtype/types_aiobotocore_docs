# CloudWatchRUM module

> [Index](../README.md) > CloudWatchRUM


!!! note ""

    Auto-generated documentation for [CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
    type annotations stubs module [types-aiobotocore-rum](https://pypi.org/project/types-aiobotocore-rum/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `CloudWatchRUM` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[rum]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[rum]'


# standalone installation
python -m pip install types-aiobotocore-rum
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-rum
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchRUMClient

Type annotations and code completion for  `#!python session.create_client("rum")` as [CloudWatchRUMClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client)

```python
# CloudWatchRUMClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_rum.client import CloudWatchRUMClient


session = get_session()
async with session.create_client("rum") as client:
    client: CloudWatchRUMClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("rum").get_paginator("...")`.

```python
# BatchGetRumMetricDefinitionsPaginator usage example

from types_aiobotocore_rum.paginator import BatchGetRumMetricDefinitionsPaginator

def get_batch_get_rum_metric_definitions_paginator() -> BatchGetRumMetricDefinitionsPaginator:
    return client.get_paginator("batch_get_rum_metric_definitions"))
```

- [BatchGetRumMetricDefinitionsPaginator](./paginators.md#batchgetrummetricdefinitionspaginator)
- [GetAppMonitorDataPaginator](./paginators.md#getappmonitordatapaginator)
- [ListAppMonitorsPaginator](./paginators.md#listappmonitorspaginator)
- [ListRumMetricsDestinationsPaginator](./paginators.md#listrummetricsdestinationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BatchGetRumMetricDefinitionsPaginatorName usage example

from types_aiobotocore_rum.literals import BatchGetRumMetricDefinitionsPaginatorName

def get_value() -> BatchGetRumMetricDefinitionsPaginatorName:
    return "batch_get_rum_metric_definitions"
```

- [BatchGetRumMetricDefinitionsPaginatorName](./literals.md#batchgetrummetricdefinitionspaginatorname)
- [CustomEventsStatusType](./literals.md#customeventsstatustype)
- [GetAppMonitorDataPaginatorName](./literals.md#getappmonitordatapaginatorname)
- [ListAppMonitorsPaginatorName](./literals.md#listappmonitorspaginatorname)
- [ListRumMetricsDestinationsPaginatorName](./literals.md#listrummetricsdestinationspaginatorname)
- [MetricDestinationType](./literals.md#metricdestinationtype)
- [StateEnumType](./literals.md#stateenumtype)
- [TelemetryType](./literals.md#telemetrytype)
- [CloudWatchRUMServiceName](./literals.md#cloudwatchrumservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AppMonitorConfigurationOutputTypeDef](./type_defs.md#appmonitorconfigurationoutputtypedef)
- [AppMonitorConfigurationTypeDef](./type_defs.md#appmonitorconfigurationtypedef)
- [AppMonitorDetailsTypeDef](./type_defs.md#appmonitordetailstypedef)
- [AppMonitorSummaryTypeDef](./type_defs.md#appmonitorsummarytypedef)
- [CustomEventsTypeDef](./type_defs.md#customeventstypedef)
- [MetricDefinitionRequestOutputTypeDef](./type_defs.md#metricdefinitionrequestoutputtypedef)
- [MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchDeleteRumMetricDefinitionsErrorTypeDef](./type_defs.md#batchdeleterummetricdefinitionserrortypedef)
- [BatchDeleteRumMetricDefinitionsRequestRequestTypeDef](./type_defs.md#batchdeleterummetricdefinitionsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [BatchGetRumMetricDefinitionsRequestRequestTypeDef](./type_defs.md#batchgetrummetricdefinitionsrequestrequesttypedef)
- [CwLogTypeDef](./type_defs.md#cwlogtypedef)
- [DeleteAppMonitorRequestRequestTypeDef](./type_defs.md#deleteappmonitorrequestrequesttypedef)
- [DeleteRumMetricsDestinationRequestRequestTypeDef](./type_defs.md#deleterummetricsdestinationrequestrequesttypedef)
- [QueryFilterTypeDef](./type_defs.md#queryfiltertypedef)
- [TimeRangeTypeDef](./type_defs.md#timerangetypedef)
- [GetAppMonitorRequestRequestTypeDef](./type_defs.md#getappmonitorrequestrequesttypedef)
- [ListAppMonitorsRequestRequestTypeDef](./type_defs.md#listappmonitorsrequestrequesttypedef)
- [ListRumMetricsDestinationsRequestRequestTypeDef](./type_defs.md#listrummetricsdestinationsrequestrequesttypedef)
- [MetricDestinationSummaryTypeDef](./type_defs.md#metricdestinationsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [MetricDefinitionRequestTypeDef](./type_defs.md#metricdefinitionrequesttypedef)
- [UserDetailsTypeDef](./type_defs.md#userdetailstypedef)
- [PutRumMetricsDestinationRequestRequestTypeDef](./type_defs.md#putrummetricsdestinationrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [CreateAppMonitorRequestRequestTypeDef](./type_defs.md#createappmonitorrequestrequesttypedef)
- [UpdateAppMonitorRequestRequestTypeDef](./type_defs.md#updateappmonitorrequestrequesttypedef)
- [BatchCreateRumMetricDefinitionsErrorTypeDef](./type_defs.md#batchcreaterummetricdefinitionserrortypedef)
- [BatchGetRumMetricDefinitionsResponseTypeDef](./type_defs.md#batchgetrummetricdefinitionsresponsetypedef)
- [CreateAppMonitorResponseTypeDef](./type_defs.md#createappmonitorresponsetypedef)
- [GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef)
- [ListAppMonitorsResponseTypeDef](./type_defs.md#listappmonitorsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [BatchDeleteRumMetricDefinitionsResponseTypeDef](./type_defs.md#batchdeleterummetricdefinitionsresponsetypedef)
- [BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef](./type_defs.md#batchgetrummetricdefinitionsrequestbatchgetrummetricdefinitionspaginatetypedef)
- [ListAppMonitorsRequestListAppMonitorsPaginateTypeDef](./type_defs.md#listappmonitorsrequestlistappmonitorspaginatetypedef)
- [ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef](./type_defs.md#listrummetricsdestinationsrequestlistrummetricsdestinationspaginatetypedef)
- [DataStorageTypeDef](./type_defs.md#datastoragetypedef)
- [GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef](./type_defs.md#getappmonitordatarequestgetappmonitordatapaginatetypedef)
- [GetAppMonitorDataRequestRequestTypeDef](./type_defs.md#getappmonitordatarequestrequesttypedef)
- [ListRumMetricsDestinationsResponseTypeDef](./type_defs.md#listrummetricsdestinationsresponsetypedef)
- [MetricDefinitionRequestUnionTypeDef](./type_defs.md#metricdefinitionrequestuniontypedef)
- [UpdateRumMetricDefinitionRequestRequestTypeDef](./type_defs.md#updaterummetricdefinitionrequestrequesttypedef)
- [RumEventTypeDef](./type_defs.md#rumeventtypedef)
- [BatchCreateRumMetricDefinitionsResponseTypeDef](./type_defs.md#batchcreaterummetricdefinitionsresponsetypedef)
- [AppMonitorTypeDef](./type_defs.md#appmonitortypedef)
- [BatchCreateRumMetricDefinitionsRequestRequestTypeDef](./type_defs.md#batchcreaterummetricdefinitionsrequestrequesttypedef)
- [PutRumEventsRequestRequestTypeDef](./type_defs.md#putrumeventsrequestrequesttypedef)
- [GetAppMonitorResponseTypeDef](./type_defs.md#getappmonitorresponsetypedef)

