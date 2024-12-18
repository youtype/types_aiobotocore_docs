# CloudWatchApplicationSignals module

> [Index](../README.md) > CloudWatchApplicationSignals


!!! note ""

    Auto-generated documentation for [CloudWatchApplicationSignals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-signals.html#cloudwatchapplicationsignals)
    type annotations stubs module [types-aiobotocore-application-signals](https://pypi.org/project/types-aiobotocore-application-signals/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudWatchApplicationSignals` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudWatchApplicationSignals` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[application-signals]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[application-signals]'

# standalone installation
python -m pip install types-aiobotocore-application-signals
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-application-signals
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchApplicationSignalsClient

Type annotations and code completion for  `#!python session.create_client("application-signals")` as [CloudWatchApplicationSignalsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-signals.html#CloudWatchApplicationSignals.Client)

```python
# CloudWatchApplicationSignalsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_application_signals.client import CloudWatchApplicationSignalsClient


session = get_session()
async with session.create_client("application-signals") as client:
    client: CloudWatchApplicationSignalsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("application-signals").get_paginator("...")`.

```python
# ListServiceDependenciesPaginator usage example

from types_aiobotocore_application_signals.paginator import ListServiceDependenciesPaginator

def get_list_service_dependencies_paginator() -> ListServiceDependenciesPaginator:
    return client.get_paginator("list_service_dependencies"))
```

- [ListServiceDependenciesPaginator](./paginators.md#listservicedependenciespaginator)
- [ListServiceDependentsPaginator](./paginators.md#listservicedependentspaginator)
- [ListServiceLevelObjectivesPaginator](./paginators.md#listservicelevelobjectivespaginator)
- [ListServiceOperationsPaginator](./paginators.md#listserviceoperationspaginator)
- [ListServicesPaginator](./paginators.md#listservicespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DurationUnitType usage example

from types_aiobotocore_application_signals.literals import DurationUnitType

def get_value() -> DurationUnitType:
    return "DAY"
```

- [DurationUnitType](./literals.md#durationunittype)
- [EvaluationTypeType](./literals.md#evaluationtypetype)
- [ListServiceDependenciesPaginatorName](./literals.md#listservicedependenciespaginatorname)
- [ListServiceDependentsPaginatorName](./literals.md#listservicedependentspaginatorname)
- [ListServiceLevelObjectivesPaginatorName](./literals.md#listservicelevelobjectivespaginatorname)
- [ListServiceOperationsPaginatorName](./literals.md#listserviceoperationspaginatorname)
- [ListServicesPaginatorName](./literals.md#listservicespaginatorname)
- [ServiceLevelIndicatorComparisonOperatorType](./literals.md#servicelevelindicatorcomparisonoperatortype)
- [ServiceLevelIndicatorMetricTypeType](./literals.md#servicelevelindicatormetrictypetype)
- [ServiceLevelObjectiveBudgetStatusType](./literals.md#servicelevelobjectivebudgetstatustype)
- [StandardUnitType](./literals.md#standardunittype)
- [CloudWatchApplicationSignalsServiceName](./literals.md#cloudwatchapplicationsignalsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ServiceLevelObjectiveBudgetReportErrorTypeDef](./type_defs.md#servicelevelobjectivebudgetreporterrortypedef)
- [BurnRateConfigurationTypeDef](./type_defs.md#burnrateconfigurationtypedef)
- [CalendarIntervalOutputTypeDef](./type_defs.md#calendarintervaloutputtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DeleteServiceLevelObjectiveInputRequestTypeDef](./type_defs.md#deleteservicelevelobjectiveinputrequesttypedef)
- [DimensionTypeDef](./type_defs.md#dimensiontypedef)
- [GetServiceLevelObjectiveInputRequestTypeDef](./type_defs.md#getservicelevelobjectiveinputrequesttypedef)
- [RollingIntervalTypeDef](./type_defs.md#rollingintervaltypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListServiceLevelObjectivesInputRequestTypeDef](./type_defs.md#listservicelevelobjectivesinputrequesttypedef)
- [ServiceLevelObjectiveSummaryTypeDef](./type_defs.md#servicelevelobjectivesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [BatchGetServiceLevelObjectiveBudgetReportInputRequestTypeDef](./type_defs.md#batchgetservicelevelobjectivebudgetreportinputrequesttypedef)
- [CalendarIntervalTypeDef](./type_defs.md#calendarintervaltypedef)
- [GetServiceInputRequestTypeDef](./type_defs.md#getserviceinputrequesttypedef)
- [ListServiceDependenciesInputRequestTypeDef](./type_defs.md#listservicedependenciesinputrequesttypedef)
- [ListServiceDependentsInputRequestTypeDef](./type_defs.md#listservicedependentsinputrequesttypedef)
- [ListServiceOperationsInputRequestTypeDef](./type_defs.md#listserviceoperationsinputrequesttypedef)
- [ListServicesInputRequestTypeDef](./type_defs.md#listservicesinputrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [MetricOutputTypeDef](./type_defs.md#metricoutputtypedef)
- [MetricReferenceTypeDef](./type_defs.md#metricreferencetypedef)
- [MetricTypeDef](./type_defs.md#metrictypedef)
- [IntervalOutputTypeDef](./type_defs.md#intervaloutputtypedef)
- [ListServiceDependenciesInputListServiceDependenciesPaginateTypeDef](./type_defs.md#listservicedependenciesinputlistservicedependenciespaginatetypedef)
- [ListServiceDependentsInputListServiceDependentsPaginateTypeDef](./type_defs.md#listservicedependentsinputlistservicedependentspaginatetypedef)
- [ListServiceLevelObjectivesInputListServiceLevelObjectivesPaginateTypeDef](./type_defs.md#listservicelevelobjectivesinputlistservicelevelobjectivespaginatetypedef)
- [ListServiceOperationsInputListServiceOperationsPaginateTypeDef](./type_defs.md#listserviceoperationsinputlistserviceoperationspaginatetypedef)
- [ListServicesInputListServicesPaginateTypeDef](./type_defs.md#listservicesinputlistservicespaginatetypedef)
- [ListServiceLevelObjectivesOutputTypeDef](./type_defs.md#listservicelevelobjectivesoutputtypedef)
- [CalendarIntervalUnionTypeDef](./type_defs.md#calendarintervaluniontypedef)
- [MetricStatOutputTypeDef](./type_defs.md#metricstatoutputtypedef)
- [ServiceDependencyTypeDef](./type_defs.md#servicedependencytypedef)
- [ServiceDependentTypeDef](./type_defs.md#servicedependenttypedef)
- [ServiceOperationTypeDef](./type_defs.md#serviceoperationtypedef)
- [ServiceSummaryTypeDef](./type_defs.md#servicesummarytypedef)
- [ServiceTypeDef](./type_defs.md#servicetypedef)
- [MetricUnionTypeDef](./type_defs.md#metricuniontypedef)
- [GoalOutputTypeDef](./type_defs.md#goaloutputtypedef)
- [IntervalTypeDef](./type_defs.md#intervaltypedef)
- [MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef)
- [ListServiceDependenciesOutputTypeDef](./type_defs.md#listservicedependenciesoutputtypedef)
- [ListServiceDependentsOutputTypeDef](./type_defs.md#listservicedependentsoutputtypedef)
- [ListServiceOperationsOutputTypeDef](./type_defs.md#listserviceoperationsoutputtypedef)
- [ListServicesOutputTypeDef](./type_defs.md#listservicesoutputtypedef)
- [GetServiceOutputTypeDef](./type_defs.md#getserviceoutputtypedef)
- [MetricStatTypeDef](./type_defs.md#metricstattypedef)
- [IntervalUnionTypeDef](./type_defs.md#intervaluniontypedef)
- [MonitoredRequestCountMetricDataQueriesOutputTypeDef](./type_defs.md#monitoredrequestcountmetricdataqueriesoutputtypedef)
- [ServiceLevelIndicatorMetricTypeDef](./type_defs.md#servicelevelindicatormetrictypedef)
- [MetricStatUnionTypeDef](./type_defs.md#metricstatuniontypedef)
- [GoalTypeDef](./type_defs.md#goaltypedef)
- [RequestBasedServiceLevelIndicatorMetricTypeDef](./type_defs.md#requestbasedservicelevelindicatormetrictypedef)
- [ServiceLevelIndicatorTypeDef](./type_defs.md#servicelevelindicatortypedef)
- [MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef)
- [RequestBasedServiceLevelIndicatorTypeDef](./type_defs.md#requestbasedservicelevelindicatortypedef)
- [MetricDataQueryUnionTypeDef](./type_defs.md#metricdataqueryuniontypedef)
- [MonitoredRequestCountMetricDataQueriesTypeDef](./type_defs.md#monitoredrequestcountmetricdataqueriestypedef)
- [ServiceLevelObjectiveBudgetReportTypeDef](./type_defs.md#servicelevelobjectivebudgetreporttypedef)
- [ServiceLevelObjectiveTypeDef](./type_defs.md#servicelevelobjectivetypedef)
- [ServiceLevelIndicatorMetricConfigTypeDef](./type_defs.md#servicelevelindicatormetricconfigtypedef)
- [MonitoredRequestCountMetricDataQueriesUnionTypeDef](./type_defs.md#monitoredrequestcountmetricdataqueriesuniontypedef)
- [BatchGetServiceLevelObjectiveBudgetReportOutputTypeDef](./type_defs.md#batchgetservicelevelobjectivebudgetreportoutputtypedef)
- [CreateServiceLevelObjectiveOutputTypeDef](./type_defs.md#createservicelevelobjectiveoutputtypedef)
- [GetServiceLevelObjectiveOutputTypeDef](./type_defs.md#getservicelevelobjectiveoutputtypedef)
- [UpdateServiceLevelObjectiveOutputTypeDef](./type_defs.md#updateservicelevelobjectiveoutputtypedef)
- [ServiceLevelIndicatorConfigTypeDef](./type_defs.md#servicelevelindicatorconfigtypedef)
- [RequestBasedServiceLevelIndicatorMetricConfigTypeDef](./type_defs.md#requestbasedservicelevelindicatormetricconfigtypedef)
- [RequestBasedServiceLevelIndicatorConfigTypeDef](./type_defs.md#requestbasedservicelevelindicatorconfigtypedef)
- [CreateServiceLevelObjectiveInputRequestTypeDef](./type_defs.md#createservicelevelobjectiveinputrequesttypedef)
- [UpdateServiceLevelObjectiveInputRequestTypeDef](./type_defs.md#updateservicelevelobjectiveinputrequesttypedef)

