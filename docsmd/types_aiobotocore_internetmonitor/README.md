# CloudWatchInternetMonitor module

> [Index](../README.md) > CloudWatchInternetMonitor


!!! note ""

    Auto-generated documentation for [CloudWatchInternetMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
    type annotations stubs module [types-aiobotocore-internetmonitor](https://pypi.org/project/types-aiobotocore-internetmonitor/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `CloudWatchInternetMonitor` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[internetmonitor]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[internetmonitor]'


# standalone installation
python -m pip install types-aiobotocore-internetmonitor
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-internetmonitor
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CloudWatchInternetMonitorClient

Type annotations and code completion for  `#!python session.create_client("internetmonitor")` as [CloudWatchInternetMonitorClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
# CloudWatchInternetMonitorClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_internetmonitor.client import CloudWatchInternetMonitorClient


session = get_session()
async with session.create_client("internetmonitor") as client:
    client: CloudWatchInternetMonitorClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("internetmonitor").get_paginator("...")`.

```python
# ListHealthEventsPaginator usage example

from types_aiobotocore_internetmonitor.paginator import ListHealthEventsPaginator

def get_list_health_events_paginator() -> ListHealthEventsPaginator:
    return client.get_paginator("list_health_events"))
```

- [ListHealthEventsPaginator](./paginators.md#listhealtheventspaginator)
- [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# HealthEventImpactTypeType usage example

from types_aiobotocore_internetmonitor.literals import HealthEventImpactTypeType

def get_value() -> HealthEventImpactTypeType:
    return "AVAILABILITY"
```

- [HealthEventImpactTypeType](./literals.md#healtheventimpacttypetype)
- [HealthEventStatusType](./literals.md#healtheventstatustype)
- [ListHealthEventsPaginatorName](./literals.md#listhealtheventspaginatorname)
- [ListMonitorsPaginatorName](./literals.md#listmonitorspaginatorname)
- [LocalHealthEventsConfigStatusType](./literals.md#localhealtheventsconfigstatustype)
- [LogDeliveryStatusType](./literals.md#logdeliverystatustype)
- [MonitorConfigStateType](./literals.md#monitorconfigstatetype)
- [MonitorProcessingStatusCodeType](./literals.md#monitorprocessingstatuscodetype)
- [TriangulationEventTypeType](./literals.md#triangulationeventtypetype)
- [CloudWatchInternetMonitorServiceName](./literals.md#cloudwatchinternetmonitorservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AvailabilityMeasurementTypeDef](./type_defs.md#availabilitymeasurementtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteMonitorInputRequestTypeDef](./type_defs.md#deletemonitorinputrequesttypedef)
- [GetHealthEventInputRequestTypeDef](./type_defs.md#gethealtheventinputrequesttypedef)
- [GetMonitorInputRequestTypeDef](./type_defs.md#getmonitorinputrequesttypedef)
- [LocalHealthEventsConfigTypeDef](./type_defs.md#localhealtheventsconfigtypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListMonitorsInputRequestTypeDef](./type_defs.md#listmonitorsinputrequesttypedef)
- [MonitorTypeDef](./type_defs.md#monitortypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [NetworkTypeDef](./type_defs.md#networktypedef)
- [RoundTripTimeTypeDef](./type_defs.md#roundtriptimetypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [UpdateMonitorOutputTypeDef](./type_defs.md#updatemonitoroutputtypedef)
- [HealthEventsConfigTypeDef](./type_defs.md#healtheventsconfigtypedef)
- [InternetMeasurementsLogDeliveryTypeDef](./type_defs.md#internetmeasurementslogdeliverytypedef)
- [ListMonitorsInputListMonitorsPaginateTypeDef](./type_defs.md#listmonitorsinputlistmonitorspaginatetypedef)
- [ListHealthEventsInputListHealthEventsPaginateTypeDef](./type_defs.md#listhealtheventsinputlisthealtheventspaginatetypedef)
- [ListHealthEventsInputRequestTypeDef](./type_defs.md#listhealtheventsinputrequesttypedef)
- [ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef)
- [NetworkImpairmentTypeDef](./type_defs.md#networkimpairmenttypedef)
- [PerformanceMeasurementTypeDef](./type_defs.md#performancemeasurementtypedef)
- [CreateMonitorInputRequestTypeDef](./type_defs.md#createmonitorinputrequesttypedef)
- [GetMonitorOutputTypeDef](./type_defs.md#getmonitoroutputtypedef)
- [UpdateMonitorInputRequestTypeDef](./type_defs.md#updatemonitorinputrequesttypedef)
- [InternetHealthTypeDef](./type_defs.md#internethealthtypedef)
- [ImpactedLocationTypeDef](./type_defs.md#impactedlocationtypedef)
- [GetHealthEventOutputTypeDef](./type_defs.md#gethealtheventoutputtypedef)
- [HealthEventTypeDef](./type_defs.md#healtheventtypedef)
- [ListHealthEventsOutputTypeDef](./type_defs.md#listhealtheventsoutputtypedef)

