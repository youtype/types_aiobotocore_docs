# NetworkFlowMonitor module

> [Index](../README.md) > NetworkFlowMonitor


!!! note ""

    Auto-generated documentation for [NetworkFlowMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor.html#networkflowmonitor)
    type annotations stubs module [types-aiobotocore-networkflowmonitor](https://pypi.org/project/types-aiobotocore-networkflowmonitor/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `NetworkFlowMonitor` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `NetworkFlowMonitor` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[networkflowmonitor]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[networkflowmonitor]'

# standalone installation
python -m pip install types-aiobotocore-networkflowmonitor
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-networkflowmonitor
```

## Usage

Code samples can be found in [Examples](./usage.md).

## NetworkFlowMonitorClient

Type annotations and code completion for  `#!python session.create_client("networkflowmonitor")` as [NetworkFlowMonitorClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor.html#NetworkFlowMonitor.Client)

```python
# NetworkFlowMonitorClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_networkflowmonitor.client import NetworkFlowMonitorClient


session = get_session()
async with session.create_client("networkflowmonitor") as client:
    client: NetworkFlowMonitorClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("networkflowmonitor").get_paginator("...")`.

```python
# GetQueryResultsMonitorTopContributorsPaginator usage example

from types_aiobotocore_networkflowmonitor.paginator import GetQueryResultsMonitorTopContributorsPaginator

def get_get_query_results_monitor_top_contributors_paginator() -> GetQueryResultsMonitorTopContributorsPaginator:
    return client.get_paginator("get_query_results_monitor_top_contributors"))
```

- [GetQueryResultsMonitorTopContributorsPaginator](./paginators.md#getqueryresultsmonitortopcontributorspaginator)
- [GetQueryResultsWorkloadInsightsTopContributorsDataPaginator](./paginators.md#getqueryresultsworkloadinsightstopcontributorsdatapaginator)
- [GetQueryResultsWorkloadInsightsTopContributorsPaginator](./paginators.md#getqueryresultsworkloadinsightstopcontributorspaginator)
- [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)
- [ListScopesPaginator](./paginators.md#listscopespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DestinationCategoryType usage example

from types_aiobotocore_networkflowmonitor.literals import DestinationCategoryType

def get_value() -> DestinationCategoryType:
    return "AMAZON_DYNAMODB"
```

- [DestinationCategoryType](./literals.md#destinationcategorytype)
- [GetQueryResultsMonitorTopContributorsPaginatorName](./literals.md#getqueryresultsmonitortopcontributorspaginatorname)
- [GetQueryResultsWorkloadInsightsTopContributorsDataPaginatorName](./literals.md#getqueryresultsworkloadinsightstopcontributorsdatapaginatorname)
- [GetQueryResultsWorkloadInsightsTopContributorsPaginatorName](./literals.md#getqueryresultsworkloadinsightstopcontributorspaginatorname)
- [ListMonitorsPaginatorName](./literals.md#listmonitorspaginatorname)
- [ListScopesPaginatorName](./literals.md#listscopespaginatorname)
- [MetricUnitType](./literals.md#metricunittype)
- [MonitorLocalResourceTypeType](./literals.md#monitorlocalresourcetypetype)
- [MonitorMetricType](./literals.md#monitormetrictype)
- [MonitorRemoteResourceTypeType](./literals.md#monitorremoteresourcetypetype)
- [MonitorStatusType](./literals.md#monitorstatustype)
- [QueryStatusType](./literals.md#querystatustype)
- [ScopeStatusType](./literals.md#scopestatustype)
- [TargetTypeType](./literals.md#targettypetype)
- [WorkloadInsightsMetricType](./literals.md#workloadinsightsmetrictype)
- [NetworkFlowMonitorServiceName](./literals.md#networkflowmonitorservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [MonitorLocalResourceTypeDef](./type_defs.md#monitorlocalresourcetypedef)
- [MonitorRemoteResourceTypeDef](./type_defs.md#monitorremoteresourcetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteMonitorInputTypeDef](./type_defs.md#deletemonitorinputtypedef)
- [DeleteScopeInputTypeDef](./type_defs.md#deletescopeinputtypedef)
- [GetMonitorInputTypeDef](./type_defs.md#getmonitorinputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetQueryResultsMonitorTopContributorsInputTypeDef](./type_defs.md#getqueryresultsmonitortopcontributorsinputtypedef)
- [GetQueryResultsWorkloadInsightsTopContributorsDataInputTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsdatainputtypedef)
- [WorkloadInsightsTopContributorsDataPointTypeDef](./type_defs.md#workloadinsightstopcontributorsdatapointtypedef)
- [GetQueryResultsWorkloadInsightsTopContributorsInputTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsinputtypedef)
- [WorkloadInsightsTopContributorsRowTypeDef](./type_defs.md#workloadinsightstopcontributorsrowtypedef)
- [GetQueryStatusMonitorTopContributorsInputTypeDef](./type_defs.md#getquerystatusmonitortopcontributorsinputtypedef)
- [GetQueryStatusWorkloadInsightsTopContributorsDataInputTypeDef](./type_defs.md#getquerystatusworkloadinsightstopcontributorsdatainputtypedef)
- [GetQueryStatusWorkloadInsightsTopContributorsInputTypeDef](./type_defs.md#getquerystatusworkloadinsightstopcontributorsinputtypedef)
- [GetScopeInputTypeDef](./type_defs.md#getscopeinputtypedef)
- [KubernetesMetadataTypeDef](./type_defs.md#kubernetesmetadatatypedef)
- [ListMonitorsInputTypeDef](./type_defs.md#listmonitorsinputtypedef)
- [MonitorSummaryTypeDef](./type_defs.md#monitorsummarytypedef)
- [ListScopesInputTypeDef](./type_defs.md#listscopesinputtypedef)
- [ScopeSummaryTypeDef](./type_defs.md#scopesummarytypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [TraversedComponentTypeDef](./type_defs.md#traversedcomponenttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [StopQueryMonitorTopContributorsInputTypeDef](./type_defs.md#stopquerymonitortopcontributorsinputtypedef)
- [StopQueryWorkloadInsightsTopContributorsDataInputTypeDef](./type_defs.md#stopqueryworkloadinsightstopcontributorsdatainputtypedef)
- [StopQueryWorkloadInsightsTopContributorsInputTypeDef](./type_defs.md#stopqueryworkloadinsightstopcontributorsinputtypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [TargetIdTypeDef](./type_defs.md#targetidtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [CreateMonitorInputTypeDef](./type_defs.md#createmonitorinputtypedef)
- [UpdateMonitorInputTypeDef](./type_defs.md#updatemonitorinputtypedef)
- [CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef)
- [CreateScopeOutputTypeDef](./type_defs.md#createscopeoutputtypedef)
- [GetMonitorOutputTypeDef](./type_defs.md#getmonitoroutputtypedef)
- [GetQueryStatusMonitorTopContributorsOutputTypeDef](./type_defs.md#getquerystatusmonitortopcontributorsoutputtypedef)
- [GetQueryStatusWorkloadInsightsTopContributorsDataOutputTypeDef](./type_defs.md#getquerystatusworkloadinsightstopcontributorsdataoutputtypedef)
- [GetQueryStatusWorkloadInsightsTopContributorsOutputTypeDef](./type_defs.md#getquerystatusworkloadinsightstopcontributorsoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [StartQueryMonitorTopContributorsOutputTypeDef](./type_defs.md#startquerymonitortopcontributorsoutputtypedef)
- [StartQueryWorkloadInsightsTopContributorsDataOutputTypeDef](./type_defs.md#startqueryworkloadinsightstopcontributorsdataoutputtypedef)
- [StartQueryWorkloadInsightsTopContributorsOutputTypeDef](./type_defs.md#startqueryworkloadinsightstopcontributorsoutputtypedef)
- [UpdateMonitorOutputTypeDef](./type_defs.md#updatemonitoroutputtypedef)
- [UpdateScopeOutputTypeDef](./type_defs.md#updatescopeoutputtypedef)
- [GetQueryResultsMonitorTopContributorsInputPaginateTypeDef](./type_defs.md#getqueryresultsmonitortopcontributorsinputpaginatetypedef)
- [GetQueryResultsWorkloadInsightsTopContributorsDataInputPaginateTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsdatainputpaginatetypedef)
- [GetQueryResultsWorkloadInsightsTopContributorsInputPaginateTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsinputpaginatetypedef)
- [ListMonitorsInputPaginateTypeDef](./type_defs.md#listmonitorsinputpaginatetypedef)
- [ListScopesInputPaginateTypeDef](./type_defs.md#listscopesinputpaginatetypedef)
- [GetQueryResultsWorkloadInsightsTopContributorsDataOutputTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsdataoutputtypedef)
- [GetQueryResultsWorkloadInsightsTopContributorsOutputTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsoutputtypedef)
- [ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef)
- [ListScopesOutputTypeDef](./type_defs.md#listscopesoutputtypedef)
- [MonitorTopContributorsRowTypeDef](./type_defs.md#monitortopcontributorsrowtypedef)
- [StartQueryMonitorTopContributorsInputTypeDef](./type_defs.md#startquerymonitortopcontributorsinputtypedef)
- [StartQueryWorkloadInsightsTopContributorsDataInputTypeDef](./type_defs.md#startqueryworkloadinsightstopcontributorsdatainputtypedef)
- [StartQueryWorkloadInsightsTopContributorsInputTypeDef](./type_defs.md#startqueryworkloadinsightstopcontributorsinputtypedef)
- [TargetIdentifierTypeDef](./type_defs.md#targetidentifiertypedef)
- [GetQueryResultsMonitorTopContributorsOutputTypeDef](./type_defs.md#getqueryresultsmonitortopcontributorsoutputtypedef)
- [TargetResourceTypeDef](./type_defs.md#targetresourcetypedef)
- [CreateScopeInputTypeDef](./type_defs.md#createscopeinputtypedef)
- [GetScopeOutputTypeDef](./type_defs.md#getscopeoutputtypedef)
- [UpdateScopeInputTypeDef](./type_defs.md#updatescopeinputtypedef)

