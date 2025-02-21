# Paginators

> [Index](../README.md) > [CloudWatch](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#cloudwatch)
    type annotations stubs module [types-aiobotocore-cloudwatch](https://pypi.org/project/types-aiobotocore-cloudwatch/).

## DescribeAlarmHistoryPaginator

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_paginator("describe_alarm_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/paginator/DescribeAlarmHistory.html#CloudWatch.Paginator.DescribeAlarmHistory)

```python
# DescribeAlarmHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import DescribeAlarmHistoryPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:  # (1)
    paginator: DescribeAlarmHistoryPaginator = client.get_paginator("describe_alarm_history")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAlarmHistoryOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchClient](./client.md)
2. paginator: [DescribeAlarmHistoryPaginator](./paginators.md#describealarmhistorypaginator)
3. item: [:material-code-braces: DescribeAlarmHistoryOutputTypeDef](./type_defs.md#describealarmhistoryoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAlarmHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AlarmName: str = ...,
    AlarmTypes: Sequence[AlarmTypeType] = ...,  # (1)
    HistoryItemType: HistoryItemTypeType = ...,  # (2)
    StartDate: TimestampTypeDef = ...,
    EndDate: TimestampTypeDef = ...,
    ScanBy: ScanByType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[DescribeAlarmHistoryOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: HistoryItemTypeType](./literals.md#historyitemtypetype) 
3. See [:material-code-brackets: ScanByType](./literals.md#scanbytype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: DescribeAlarmHistoryOutputTypeDef](./type_defs.md#describealarmhistoryoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAlarmHistoryInputPaginateTypeDef = {  # (1)
    "AlarmName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAlarmHistoryInputPaginateTypeDef](./type_defs.md#describealarmhistoryinputpaginatetypedef) 
## DescribeAlarmsPaginator

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_paginator("describe_alarms")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/paginator/DescribeAlarms.html#CloudWatch.Paginator.DescribeAlarms)

```python
# DescribeAlarmsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import DescribeAlarmsPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:  # (1)
    paginator: DescribeAlarmsPaginator = client.get_paginator("describe_alarms")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAlarmsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchClient](./client.md)
2. paginator: [DescribeAlarmsPaginator](./paginators.md#describealarmspaginator)
3. item: [:material-code-braces: DescribeAlarmsOutputTypeDef](./type_defs.md#describealarmsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAlarmsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AlarmNames: Sequence[str] = ...,
    AlarmNamePrefix: str = ...,
    AlarmTypes: Sequence[AlarmTypeType] = ...,  # (1)
    ChildrenOfAlarmName: str = ...,
    ParentsOfAlarmName: str = ...,
    StateValue: StateValueType = ...,  # (2)
    ActionPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[DescribeAlarmsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: AlarmTypeType](./literals.md#alarmtypetype) 
2. See [:material-code-brackets: StateValueType](./literals.md#statevaluetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeAlarmsOutputTypeDef](./type_defs.md#describealarmsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAlarmsInputPaginateTypeDef = {  # (1)
    "AlarmNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAlarmsInputPaginateTypeDef](./type_defs.md#describealarmsinputpaginatetypedef) 
## DescribeAnomalyDetectorsPaginator

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_paginator("describe_anomaly_detectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/paginator/DescribeAnomalyDetectors.html#CloudWatch.Paginator.DescribeAnomalyDetectors)

```python
# DescribeAnomalyDetectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import DescribeAnomalyDetectorsPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:  # (1)
    paginator: DescribeAnomalyDetectorsPaginator = client.get_paginator("describe_anomaly_detectors")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAnomalyDetectorsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchClient](./client.md)
2. paginator: [DescribeAnomalyDetectorsPaginator](./paginators.md#describeanomalydetectorspaginator)
3. item: [:material-code-braces: DescribeAnomalyDetectorsOutputTypeDef](./type_defs.md#describeanomalydetectorsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAnomalyDetectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Namespace: str = ...,
    MetricName: str = ...,
    Dimensions: Sequence[DimensionTypeDef] = ...,  # (1)
    AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[DescribeAnomalyDetectorsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-brackets: AnomalyDetectorTypeType](./literals.md#anomalydetectortypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeAnomalyDetectorsOutputTypeDef](./type_defs.md#describeanomalydetectorsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAnomalyDetectorsInputPaginateTypeDef = {  # (1)
    "Namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAnomalyDetectorsInputPaginateTypeDef](./type_defs.md#describeanomalydetectorsinputpaginatetypedef) 
## GetMetricDataPaginator

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_paginator("get_metric_data")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/paginator/GetMetricData.html#CloudWatch.Paginator.GetMetricData)

```python
# GetMetricDataPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import GetMetricDataPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:  # (1)
    paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")  # (2)
    async for item in paginator.paginate(...):
        item: GetMetricDataOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchClient](./client.md)
2. paginator: [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
3. item: [:material-code-braces: GetMetricDataOutputTypeDef](./type_defs.md#getmetricdataoutputtypedef) 


### paginate

Type annotations and code completion for `#!python GetMetricDataPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],  # (1)
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    ScanBy: ScanByType = ...,  # (2)
    LabelOptions: LabelOptionsTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[GetMetricDataOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: MetricDataQueryTypeDef](./type_defs.md#metricdataquerytypedef) [:material-code-braces: MetricDataQueryOutputTypeDef](./type_defs.md#metricdataqueryoutputtypedef) 
2. See [:material-code-brackets: ScanByType](./literals.md#scanbytype) 
3. See [:material-code-braces: LabelOptionsTypeDef](./type_defs.md#labeloptionstypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: GetMetricDataOutputTypeDef](./type_defs.md#getmetricdataoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetMetricDataInputPaginateTypeDef = {  # (1)
    "MetricDataQueries": ...,
    "StartTime": ...,
    "EndTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetMetricDataInputPaginateTypeDef](./type_defs.md#getmetricdatainputpaginatetypedef) 
## ListDashboardsPaginator

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_paginator("list_dashboards")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/paginator/ListDashboards.html#CloudWatch.Paginator.ListDashboards)

```python
# ListDashboardsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import ListDashboardsPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:  # (1)
    paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")  # (2)
    async for item in paginator.paginate(...):
        item: ListDashboardsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchClient](./client.md)
2. paginator: [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
3. item: [:material-code-braces: ListDashboardsOutputTypeDef](./type_defs.md#listdashboardsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDashboardsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DashboardNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDashboardsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDashboardsOutputTypeDef](./type_defs.md#listdashboardsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDashboardsInputPaginateTypeDef = {  # (1)
    "DashboardNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDashboardsInputPaginateTypeDef](./type_defs.md#listdashboardsinputpaginatetypedef) 
## ListMetricsPaginator

Type annotations and code completion for `#!python session.create_client("cloudwatch").get_paginator("list_metrics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch/paginator/ListMetrics.html#CloudWatch.Paginator.ListMetrics)

```python
# ListMetricsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudwatch.paginator import ListMetricsPaginator

session = get_session()
async with session.create_client("cloudwatch") as client:  # (1)
    paginator: ListMetricsPaginator = client.get_paginator("list_metrics")  # (2)
    async for item in paginator.paginate(...):
        item: ListMetricsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchClient](./client.md)
2. paginator: [ListMetricsPaginator](./paginators.md#listmetricspaginator)
3. item: [:material-code-braces: ListMetricsOutputTypeDef](./type_defs.md#listmetricsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListMetricsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Namespace: str = ...,
    MetricName: str = ...,
    Dimensions: Sequence[DimensionFilterTypeDef] = ...,  # (1)
    RecentlyActive: RecentlyActiveType = ...,  # (2)
    IncludeLinkedAccounts: bool = ...,
    OwningAccount: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListMetricsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: DimensionFilterTypeDef](./type_defs.md#dimensionfiltertypedef) 
2. See [:material-code-brackets: RecentlyActiveType](./literals.md#recentlyactivetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListMetricsOutputTypeDef](./type_defs.md#listmetricsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMetricsInputPaginateTypeDef = {  # (1)
    "Namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMetricsInputPaginateTypeDef](./type_defs.md#listmetricsinputpaginatetypedef) 
