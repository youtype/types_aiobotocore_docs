# CloudWatch module

> [Index](../README.md) > CloudWatch


!!! note ""

    Auto-generated documentation for [CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#cloudwatch)
    type annotations stubs module [types-aiobotocore-cloudwatch](https://pypi.org/project/types-aiobotocore-cloudwatch/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `CloudWatch` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `CloudWatch` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[cloudwatch]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloudwatch]'

# standalone installation
python -m pip install types-aiobotocore-cloudwatch
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-cloudwatch
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchClient

Type annotations and code completion for  `#!python session.create_client("cloudwatch")` as [CloudWatchClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client)

```python
# CloudWatchClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.client import CloudWatchClient


session = get_session()
async with session.create_client("cloudwatch") as client:
    client: CloudWatchClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("cloudwatch").get_paginator("...")`.

```python
# DescribeAlarmHistoryPaginator usage example

from types_aiobotocore_cloudwatch.paginator import DescribeAlarmHistoryPaginator

def get_describe_alarm_history_paginator() -> DescribeAlarmHistoryPaginator:
    return client.get_paginator("describe_alarm_history"))
```

- [DescribeAlarmHistoryPaginator](./paginators.md#describealarmhistorypaginator)
- [DescribeAlarmsPaginator](./paginators.md#describealarmspaginator)
- [DescribeAnomalyDetectorsPaginator](./paginators.md#describeanomalydetectorspaginator)
- [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
- [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
- [ListMetricsPaginator](./paginators.md#listmetricspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("cloudwatch").get_waiter("...")`.

```python
# AlarmExistsWaiter usage example

from types_aiobotocore_cloudwatch.waiter import AlarmExistsWaiter

def get_alarm_exists_waiter() -> AlarmExistsWaiter:
    return Session().client("cloudwatch").get_waiter("alarm_exists")
```

- [AlarmExistsWaiter](./waiters.md#alarmexistswaiter)
- [CompositeAlarmExistsWaiter](./waiters.md#compositealarmexistswaiter)




## CloudWatchServiceResource

Type annotations and code completion for `#!python session.resource("cloudwatch")` as
[CloudWatchServiceResource](./service_resource.md#cloudwatchserviceresource)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/service-resource/index.html)

```python
# CloudWatchServiceResource usage example

from types_aiobotocore_cloudwatch.service_resource import CloudWatchServiceResource
```


### Collections

Type annotations and code completion for collections
from `#!python session.resource("cloudwatch").*`.

```python
# ServiceResourceAlarmsCollection usage example

from types_aiobotocore_cloudwatch.service_resource import ServiceResourceAlarmsCollection

def get_collection() -> ServiceResourceAlarmsCollection:
    return resource.alarms
```

- [ServiceResourceAlarmsCollection](./service_resource.md#serviceresourcealarmscollection)
- [ServiceResourceMetricsCollection](./service_resource.md#serviceresourcemetricscollection)





### Resources

Type annotations and code completion for additional resources
from `#!python session.resource("cloudwatch").*`.

```python
# Alarm usage example

from types_aiobotocore_cloudwatch.service_resource import Alarm

def get_resource() -> Alarm:
    return resource.Alarm(...)
```

- [Alarm](./service_resource.md#alarm)
- [Metric](./service_resource.md#metric)





## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionsSuppressedByType usage example

from types_aiobotocore_cloudwatch.literals import ActionsSuppressedByType

def get_value() -> ActionsSuppressedByType:
    return "Alarm"
```

- [ActionsSuppressedByType](./literals.md#actionssuppressedbytype)
- [AlarmExistsWaiterName](./literals.md#alarmexistswaitername)
- [AlarmTypeType](./literals.md#alarmtypetype)
- [AnomalyDetectorStateValueType](./literals.md#anomalydetectorstatevaluetype)
- [AnomalyDetectorTypeType](./literals.md#anomalydetectortypetype)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [CompositeAlarmExistsWaiterName](./literals.md#compositealarmexistswaitername)
- [DescribeAlarmHistoryPaginatorName](./literals.md#describealarmhistorypaginatorname)
- [DescribeAlarmsPaginatorName](./literals.md#describealarmspaginatorname)
- [DescribeAnomalyDetectorsPaginatorName](./literals.md#describeanomalydetectorspaginatorname)
- [EvaluationStateType](./literals.md#evaluationstatetype)
- [GetMetricDataPaginatorName](./literals.md#getmetricdatapaginatorname)
- [HistoryItemTypeType](./literals.md#historyitemtypetype)
- [ListDashboardsPaginatorName](./literals.md#listdashboardspaginatorname)
- [ListMetricsPaginatorName](./literals.md#listmetricspaginatorname)
- [MetricStreamOutputFormatType](./literals.md#metricstreamoutputformattype)
- [RecentlyActiveType](./literals.md#recentlyactivetype)
- [ScanByType](./literals.md#scanbytype)
- [StandardUnitType](./literals.md#standardunittype)
- [StateValueType](./literals.md#statevaluetype)
- [StatisticType](./literals.md#statistictype)
- [StatusCodeType](./literals.md#statuscodetype)
- [CloudWatchServiceName](./literals.md#cloudwatchservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AlarmHistoryItemTypeDef](./type_defs.md#alarmhistoryitemtypedef)
- [RangeOutputTypeDef](./type_defs.md#rangeoutputtypedef)
- [DimensionTypeDef](./type_defs.md#dimensiontypedef)
- [MetricCharacteristicsTypeDef](./type_defs.md#metriccharacteristicstypedef)
- [CloudwatchEventStateTypeDef](./type_defs.md#cloudwatcheventstatetypedef)
- [CloudwatchEventMetricStatsMetricTypeDef](./type_defs.md#cloudwatcheventmetricstatsmetrictypedef)
- [CompositeAlarmTypeDef](./type_defs.md#compositealarmtypedef)
- [DashboardEntryTypeDef](./type_defs.md#dashboardentrytypedef)
- [DashboardValidationMessageTypeDef](./type_defs.md#dashboardvalidationmessagetypedef)
- [DatapointTypeDef](./type_defs.md#datapointtypedef)
- [DeleteAlarmsInputRequestTypeDef](./type_defs.md#deletealarmsinputrequesttypedef)
- [DeleteDashboardsInputRequestTypeDef](./type_defs.md#deletedashboardsinputrequesttypedef)
- [DeleteInsightRulesInputRequestTypeDef](./type_defs.md#deleteinsightrulesinputrequesttypedef)
- [PartialFailureTypeDef](./type_defs.md#partialfailuretypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteMetricStreamInputRequestTypeDef](./type_defs.md#deletemetricstreaminputrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeAlarmsInputRequestTypeDef](./type_defs.md#describealarmsinputrequesttypedef)
- [DescribeInsightRulesInputRequestTypeDef](./type_defs.md#describeinsightrulesinputrequesttypedef)
- [InsightRuleTypeDef](./type_defs.md#insightruletypedef)
- [DimensionFilterTypeDef](./type_defs.md#dimensionfiltertypedef)
- [DisableAlarmActionsInputRequestTypeDef](./type_defs.md#disablealarmactionsinputrequesttypedef)
- [DisableInsightRulesInputRequestTypeDef](./type_defs.md#disableinsightrulesinputrequesttypedef)
- [EnableAlarmActionsInputRequestTypeDef](./type_defs.md#enablealarmactionsinputrequesttypedef)
- [EnableInsightRulesInputRequestTypeDef](./type_defs.md#enableinsightrulesinputrequesttypedef)
- [EntityTypeDef](./type_defs.md#entitytypedef)
- [GetDashboardInputRequestTypeDef](./type_defs.md#getdashboardinputrequesttypedef)
- [InsightRuleMetricDatapointTypeDef](./type_defs.md#insightrulemetricdatapointtypedef)
- [LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef)
- [MessageDataTypeDef](./type_defs.md#messagedatatypedef)
- [GetMetricStreamInputRequestTypeDef](./type_defs.md#getmetricstreaminputrequesttypedef)
- [MetricStreamFilterOutputTypeDef](./type_defs.md#metricstreamfilteroutputtypedef)
- [GetMetricWidgetImageInputRequestTypeDef](./type_defs.md#getmetricwidgetimageinputrequesttypedef)
- [InsightRuleContributorDatapointTypeDef](./type_defs.md#insightrulecontributordatapointtypedef)
- [ListDashboardsInputRequestTypeDef](./type_defs.md#listdashboardsinputrequesttypedef)
- [ListManagedInsightRulesInputRequestTypeDef](./type_defs.md#listmanagedinsightrulesinputrequesttypedef)
- [ListMetricStreamsInputRequestTypeDef](./type_defs.md#listmetricstreamsinputrequesttypedef)
- [MetricStreamEntryTypeDef](./type_defs.md#metricstreamentrytypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ManagedRuleStateTypeDef](./type_defs.md#managedrulestatetypedef)
- [StatisticSetTypeDef](./type_defs.md#statisticsettypedef)
- [MetricStreamFilterTypeDef](./type_defs.md#metricstreamfiltertypedef)
- [MetricStreamStatisticsMetricTypeDef](./type_defs.md#metricstreamstatisticsmetrictypedef)
- [PutDashboardInputRequestTypeDef](./type_defs.md#putdashboardinputrequesttypedef)
- [SetAlarmStateInputAlarmSetStateTypeDef](./type_defs.md#setalarmstateinputalarmsetstatetypedef)
- [SetAlarmStateInputRequestTypeDef](./type_defs.md#setalarmstateinputrequesttypedef)
- [StartMetricStreamsInputRequestTypeDef](./type_defs.md#startmetricstreamsinputrequesttypedef)
- [StopMetricStreamsInputRequestTypeDef](./type_defs.md#stopmetricstreamsinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [AnomalyDetectorConfigurationOutputTypeDef](./type_defs.md#anomalydetectorconfigurationoutputtypedef)
- [DescribeAlarmsForMetricInputRequestTypeDef](./type_defs.md#describealarmsformetricinputrequesttypedef)
- [DescribeAnomalyDetectorsInputRequestTypeDef](./type_defs.md#describeanomalydetectorsinputrequesttypedef)
- [MetricOutputTypeDef](./type_defs.md#metricoutputtypedef)
- [MetricTypeDef](./type_defs.md#metrictypedef)
- [SingleMetricAnomalyDetectorOutputTypeDef](./type_defs.md#singlemetricanomalydetectoroutputtypedef)
- [SingleMetricAnomalyDetectorTypeDef](./type_defs.md#singlemetricanomalydetectortypedef)
- [CloudwatchEventMetricStatsTypeDef](./type_defs.md#cloudwatcheventmetricstatstypedef)
- [DeleteInsightRulesOutputTypeDef](./type_defs.md#deleteinsightrulesoutputtypedef)
- [DescribeAlarmHistoryOutputTypeDef](./type_defs.md#describealarmhistoryoutputtypedef)
- [DisableInsightRulesOutputTypeDef](./type_defs.md#disableinsightrulesoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [EnableInsightRulesOutputTypeDef](./type_defs.md#enableinsightrulesoutputtypedef)
- [GetDashboardOutputTypeDef](./type_defs.md#getdashboardoutputtypedef)
- [GetMetricStatisticsOutputTypeDef](./type_defs.md#getmetricstatisticsoutputtypedef)
- [GetMetricWidgetImageOutputTypeDef](./type_defs.md#getmetricwidgetimageoutputtypedef)
- [ListDashboardsOutputTypeDef](./type_defs.md#listdashboardsoutputtypedef)
- [PutDashboardOutputTypeDef](./type_defs.md#putdashboardoutputtypedef)
- [PutManagedInsightRulesOutputTypeDef](./type_defs.md#putmanagedinsightrulesoutputtypedef)
- [PutMetricStreamOutputTypeDef](./type_defs.md#putmetricstreamoutputtypedef)
- [DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef](./type_defs.md#describealarmhistoryinputalarmdescribehistorytypedef)
- [DescribeAlarmHistoryInputRequestTypeDef](./type_defs.md#describealarmhistoryinputrequesttypedef)
- [GetInsightRuleReportInputRequestTypeDef](./type_defs.md#getinsightrulereportinputrequesttypedef)
- [GetMetricStatisticsInputMetricGetStatisticsTypeDef](./type_defs.md#getmetricstatisticsinputmetricgetstatisticstypedef)
- [GetMetricStatisticsInputRequestTypeDef](./type_defs.md#getmetricstatisticsinputrequesttypedef)
- [RangeTypeDef](./type_defs.md#rangetypedef)
- [DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef](./type_defs.md#describealarmhistoryinputdescribealarmhistorypaginatetypedef)
- [DescribeAlarmsInputDescribeAlarmsPaginateTypeDef](./type_defs.md#describealarmsinputdescribealarmspaginatetypedef)
- [DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef](./type_defs.md#describeanomalydetectorsinputdescribeanomalydetectorspaginatetypedef)
- [ListDashboardsInputListDashboardsPaginateTypeDef](./type_defs.md#listdashboardsinputlistdashboardspaginatetypedef)
- [DescribeAlarmsInputAlarmExistsWaitTypeDef](./type_defs.md#describealarmsinputalarmexistswaittypedef)
- [DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef](./type_defs.md#describealarmsinputcompositealarmexistswaittypedef)
- [DescribeInsightRulesOutputTypeDef](./type_defs.md#describeinsightrulesoutputtypedef)
- [ListMetricsInputListMetricsPaginateTypeDef](./type_defs.md#listmetricsinputlistmetricspaginatetypedef)
- [ListMetricsInputRequestTypeDef](./type_defs.md#listmetricsinputrequesttypedef)
- [MetricDataResultTypeDef](./type_defs.md#metricdataresulttypedef)
- [InsightRuleContributorTypeDef](./type_defs.md#insightrulecontributortypedef)
- [ListMetricStreamsOutputTypeDef](./type_defs.md#listmetricstreamsoutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [ManagedRuleTypeDef](./type_defs.md#managedruletypedef)
- [PutCompositeAlarmInputRequestTypeDef](./type_defs.md#putcompositealarminputrequesttypedef)
- [PutInsightRuleInputRequestTypeDef](./type_defs.md#putinsightruleinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [ManagedRuleDescriptionTypeDef](./type_defs.md#managedruledescriptiontypedef)
- [MetricDatumTypeDef](./type_defs.md#metricdatumtypedef)
- [MetricStreamFilterUnionTypeDef](./type_defs.md#metricstreamfilteruniontypedef)
- [MetricStreamStatisticsConfigurationOutputTypeDef](./type_defs.md#metricstreamstatisticsconfigurationoutputtypedef)
- [MetricStreamStatisticsConfigurationTypeDef](./type_defs.md#metricstreamstatisticsconfigurationtypedef)
- [ListMetricsOutputTypeDef](./type_defs.md#listmetricsoutputtypedef)
- [MetricStatOutputTypeDef](./type_defs.md#metricstatoutputtypedef)
- [MetricStatTypeDef](./type_defs.md#metricstattypedef)
- [CloudwatchEventMetricTypeDef](./type_defs.md#cloudwatcheventmetrictypedef)
- [RangeUnionTypeDef](./type_defs.md#rangeuniontypedef)
- [GetMetricDataOutputTypeDef](./type_defs.md#getmetricdataoutputtypedef)
- [GetInsightRuleReportOutputTypeDef](./type_defs.md#getinsightrulereportoutputtypedef)
- [PutManagedInsightRulesInputRequestTypeDef](./type_defs.md#putmanagedinsightrulesinputrequesttypedef)
- [ListManagedInsightRulesOutputTypeDef](./type_defs.md#listmanagedinsightrulesoutputtypedef)
- [EntityMetricDataTypeDef](./type_defs.md#entitymetricdatatypedef)
- [GetMetricStreamOutputTypeDef](./type_defs.md#getmetricstreamoutputtypedef)
- [MetricStreamStatisticsConfigurationUnionTypeDef](./type_defs.md#metricstreamstatisticsconfigurationuniontypedef)
- [MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef)
- [MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef)
- [CloudwatchEventDetailConfigurationTypeDef](./type_defs.md#cloudwatcheventdetailconfigurationtypedef)
- [AnomalyDetectorConfigurationTypeDef](./type_defs.md#anomalydetectorconfigurationtypedef)
- [PutMetricDataInputMetricPutDataTypeDef](./type_defs.md#putmetricdatainputmetricputdatatypedef)
- [PutMetricDataInputRequestTypeDef](./type_defs.md#putmetricdatainputrequesttypedef)
- [PutMetricStreamInputRequestTypeDef](./type_defs.md#putmetricstreaminputrequesttypedef)
- [MetricAlarmTypeDef](./type_defs.md#metricalarmtypedef)
- [MetricMathAnomalyDetectorOutputTypeDef](./type_defs.md#metricmathanomalydetectoroutputtypedef)
- [GetMetricDataInputGetMetricDataPaginateTypeDef](./type_defs.md#getmetricdatainputgetmetricdatapaginatetypedef)
- [MetricDataQueryUnionTypeDef](./type_defs.md#metricdataqueryuniontypedef)
- [PutMetricAlarmInputMetricPutAlarmTypeDef](./type_defs.md#putmetricalarminputmetricputalarmtypedef)
- [PutMetricAlarmInputRequestTypeDef](./type_defs.md#putmetricalarminputrequesttypedef)
- [CloudwatchEventDetailTypeDef](./type_defs.md#cloudwatcheventdetailtypedef)
- [DescribeAlarmsForMetricOutputTypeDef](./type_defs.md#describealarmsformetricoutputtypedef)
- [DescribeAlarmsOutputTypeDef](./type_defs.md#describealarmsoutputtypedef)
- [MetricStatAlarmTypeDef](./type_defs.md#metricstatalarmtypedef)
- [AnomalyDetectorTypeDef](./type_defs.md#anomalydetectortypedef)
- [GetMetricDataInputRequestTypeDef](./type_defs.md#getmetricdatainputrequesttypedef)
- [MetricMathAnomalyDetectorTypeDef](./type_defs.md#metricmathanomalydetectortypedef)
- [CloudwatchEventTypeDef](./type_defs.md#cloudwatcheventtypedef)
- [MetricDataQueryAlarmTypeDef](./type_defs.md#metricdataqueryalarmtypedef)
- [DescribeAnomalyDetectorsOutputTypeDef](./type_defs.md#describeanomalydetectorsoutputtypedef)
- [DeleteAnomalyDetectorInputRequestTypeDef](./type_defs.md#deleteanomalydetectorinputrequesttypedef)
- [PutAnomalyDetectorInputRequestTypeDef](./type_defs.md#putanomalydetectorinputrequesttypedef)

