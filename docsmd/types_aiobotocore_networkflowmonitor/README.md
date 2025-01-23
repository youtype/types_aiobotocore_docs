# NetworkFlowMonitor module

> [Index](../README.md) > NetworkFlowMonitor


!!! note ""

    Auto-generated documentation for [NetworkFlowMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor.html#networkflowmonitor)
    type annotations stubs module [types-aiobotocore-networkflowmonitor](https://pypi.org/project/types-aiobotocore-networkflowmonitor/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
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
- [DeleteMonitorInputRequestTypeDef](./type_defs.md#deletemonitorinputrequesttypedef)
- [DeleteScopeInputRequestTypeDef](./type_defs.md#deletescopeinputrequesttypedef)
- [GetMonitorInputRequestTypeDef](./type_defs.md#getmonitorinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetQueryResultsMonitorTopContributorsInputRequestTypeDef](./type_defs.md#getqueryresultsmonitortopcontributorsinputrequesttypedef)
- [GetQueryResultsWorkloadInsightsTopContributorsDataInputRequestTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsdatainputrequesttypedef)
- [WorkloadInsightsTopContributorsDataPointTypeDef](./type_defs.md#workloadinsightstopcontributorsdatapointtypedef)
- [GetQueryResultsWorkloadInsightsTopContributorsInputRequestTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsinputrequesttypedef)
- [WorkloadInsightsTopContributorsRowTypeDef](./type_defs.md#workloadinsightstopcontributorsrowtypedef)
- [GetQueryStatusMonitorTopContributorsInputRequestTypeDef](./type_defs.md#getquerystatusmonitortopcontributorsinputrequesttypedef)
- [GetQueryStatusWorkloadInsightsTopContributorsDataInputRequestTypeDef](./type_defs.md#getquerystatusworkloadinsightstopcontributorsdatainputrequesttypedef)
- [GetQueryStatusWorkloadInsightsTopContributorsInputRequestTypeDef](./type_defs.md#getquerystatusworkloadinsightstopcontributorsinputrequesttypedef)
- [GetScopeInputRequestTypeDef](./type_defs.md#getscopeinputrequesttypedef)
- [KubernetesMetadataTypeDef](./type_defs.md#kubernetesmetadatatypedef)
- [ListMonitorsInputRequestTypeDef](./type_defs.md#listmonitorsinputrequesttypedef)
- [MonitorSummaryTypeDef](./type_defs.md#monitorsummarytypedef)
- [ListScopesInputRequestTypeDef](./type_defs.md#listscopesinputrequesttypedef)
- [ScopeSummaryTypeDef](./type_defs.md#scopesummarytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [TraversedComponentTypeDef](./type_defs.md#traversedcomponenttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [StopQueryMonitorTopContributorsInputRequestTypeDef](./type_defs.md#stopquerymonitortopcontributorsinputrequesttypedef)
- [StopQueryWorkloadInsightsTopContributorsDataInputRequestTypeDef](./type_defs.md#stopqueryworkloadinsightstopcontributorsdatainputrequesttypedef)
- [StopQueryWorkloadInsightsTopContributorsInputRequestTypeDef](./type_defs.md#stopqueryworkloadinsightstopcontributorsinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [TargetIdTypeDef](./type_defs.md#targetidtypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [CreateMonitorInputRequestTypeDef](./type_defs.md#createmonitorinputrequesttypedef)
- [UpdateMonitorInputRequestTypeDef](./type_defs.md#updatemonitorinputrequesttypedef)
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
- [StartQueryMonitorTopContributorsInputRequestTypeDef](./type_defs.md#startquerymonitortopcontributorsinputrequesttypedef)
- [StartQueryWorkloadInsightsTopContributorsDataInputRequestTypeDef](./type_defs.md#startqueryworkloadinsightstopcontributorsdatainputrequesttypedef)
- [StartQueryWorkloadInsightsTopContributorsInputRequestTypeDef](./type_defs.md#startqueryworkloadinsightstopcontributorsinputrequesttypedef)
- [TargetIdentifierTypeDef](./type_defs.md#targetidentifiertypedef)
- [GetQueryResultsMonitorTopContributorsOutputTypeDef](./type_defs.md#getqueryresultsmonitortopcontributorsoutputtypedef)
- [TargetResourceTypeDef](./type_defs.md#targetresourcetypedef)
- [CreateScopeInputRequestTypeDef](./type_defs.md#createscopeinputrequesttypedef)
- [GetScopeOutputTypeDef](./type_defs.md#getscopeoutputtypedef)
- [UpdateScopeInputRequestTypeDef](./type_defs.md#updatescopeinputrequesttypedef)

