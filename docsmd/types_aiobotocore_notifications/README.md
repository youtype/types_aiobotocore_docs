# UserNotifications module

> [Index](../README.md) > UserNotifications


!!! note ""

    Auto-generated documentation for [UserNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#usernotifications)
    type annotations stubs module [types-aiobotocore-notifications](https://pypi.org/project/types-aiobotocore-notifications/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `UserNotifications` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `UserNotifications` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[notifications]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[notifications]'

# standalone installation
python -m pip install types-aiobotocore-notifications
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-notifications
```

## Usage

Code samples can be found in [Examples](./usage.md).

## UserNotificationsClient

Type annotations and code completion for  `#!python session.create_client("notifications")` as [UserNotificationsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#UserNotifications.Client)

```python
# UserNotificationsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_notifications.client import UserNotificationsClient


session = get_session()
async with session.create_client("notifications") as client:
    client: UserNotificationsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("notifications").get_paginator("...")`.

```python
# ListChannelsPaginator usage example

from types_aiobotocore_notifications.paginator import ListChannelsPaginator

def get_list_channels_paginator() -> ListChannelsPaginator:
    return client.get_paginator("list_channels"))
```

- [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- [ListEventRulesPaginator](./paginators.md#listeventrulespaginator)
- [ListNotificationConfigurationsPaginator](./paginators.md#listnotificationconfigurationspaginator)
- [ListNotificationEventsPaginator](./paginators.md#listnotificationeventspaginator)
- [ListNotificationHubsPaginator](./paginators.md#listnotificationhubspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AggregationDurationType usage example

from types_aiobotocore_notifications.literals import AggregationDurationType

def get_value() -> AggregationDurationType:
    return "LONG"
```

- [AggregationDurationType](./literals.md#aggregationdurationtype)
- [AggregationEventTypeType](./literals.md#aggregationeventtypetype)
- [EventRuleStatusType](./literals.md#eventrulestatustype)
- [EventStatusType](./literals.md#eventstatustype)
- [ListChannelsPaginatorName](./literals.md#listchannelspaginatorname)
- [ListEventRulesPaginatorName](./literals.md#listeventrulespaginatorname)
- [ListNotificationConfigurationsPaginatorName](./literals.md#listnotificationconfigurationspaginatorname)
- [ListNotificationEventsPaginatorName](./literals.md#listnotificationeventspaginatorname)
- [ListNotificationHubsPaginatorName](./literals.md#listnotificationhubspaginatorname)
- [LocaleCodeType](./literals.md#localecodetype)
- [MediaElementTypeType](./literals.md#mediaelementtypetype)
- [NotificationConfigurationStatusType](./literals.md#notificationconfigurationstatustype)
- [NotificationHubStatusType](./literals.md#notificationhubstatustype)
- [NotificationTypeType](./literals.md#notificationtypetype)
- [SchemaVersionType](./literals.md#schemaversiontype)
- [TextPartTypeType](./literals.md#textparttypetype)
- [UserNotificationsServiceName](./literals.md#usernotificationsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssociateChannelRequestRequestTypeDef](./type_defs.md#associatechannelrequestrequesttypedef)
- [CreateEventRuleRequestRequestTypeDef](./type_defs.md#createeventrulerequestrequesttypedef)
- [EventRuleStatusSummaryTypeDef](./type_defs.md#eventrulestatussummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateNotificationConfigurationRequestRequestTypeDef](./type_defs.md#createnotificationconfigurationrequestrequesttypedef)
- [DeleteEventRuleRequestRequestTypeDef](./type_defs.md#deleteeventrulerequestrequesttypedef)
- [DeleteNotificationConfigurationRequestRequestTypeDef](./type_defs.md#deletenotificationconfigurationrequestrequesttypedef)
- [DeregisterNotificationHubRequestRequestTypeDef](./type_defs.md#deregisternotificationhubrequestrequesttypedef)
- [NotificationHubStatusSummaryTypeDef](./type_defs.md#notificationhubstatussummarytypedef)
- [DimensionTypeDef](./type_defs.md#dimensiontypedef)
- [DisassociateChannelRequestRequestTypeDef](./type_defs.md#disassociatechannelrequestrequesttypedef)
- [GetEventRuleRequestRequestTypeDef](./type_defs.md#geteventrulerequestrequesttypedef)
- [GetNotificationConfigurationRequestRequestTypeDef](./type_defs.md#getnotificationconfigurationrequestrequesttypedef)
- [GetNotificationEventRequestRequestTypeDef](./type_defs.md#getnotificationeventrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef)
- [ListEventRulesRequestRequestTypeDef](./type_defs.md#listeventrulesrequestrequesttypedef)
- [ListNotificationConfigurationsRequestRequestTypeDef](./type_defs.md#listnotificationconfigurationsrequestrequesttypedef)
- [NotificationConfigurationStructureTypeDef](./type_defs.md#notificationconfigurationstructuretypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListNotificationHubsRequestRequestTypeDef](./type_defs.md#listnotificationhubsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [MediaElementTypeDef](./type_defs.md#mediaelementtypedef)
- [MessageComponentsSummaryTypeDef](./type_defs.md#messagecomponentssummarytypedef)
- [SourceEventMetadataSummaryTypeDef](./type_defs.md#sourceeventmetadatasummarytypedef)
- [TextPartValueTypeDef](./type_defs.md#textpartvaluetypedef)
- [RegisterNotificationHubRequestRequestTypeDef](./type_defs.md#registernotificationhubrequestrequesttypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateEventRuleRequestRequestTypeDef](./type_defs.md#updateeventrulerequestrequesttypedef)
- [UpdateNotificationConfigurationRequestRequestTypeDef](./type_defs.md#updatenotificationconfigurationrequestrequesttypedef)
- [EventRuleStructureTypeDef](./type_defs.md#eventrulestructuretypedef)
- [CreateEventRuleResponseTypeDef](./type_defs.md#createeventruleresponsetypedef)
- [CreateNotificationConfigurationResponseTypeDef](./type_defs.md#createnotificationconfigurationresponsetypedef)
- [GetEventRuleResponseTypeDef](./type_defs.md#geteventruleresponsetypedef)
- [GetNotificationConfigurationResponseTypeDef](./type_defs.md#getnotificationconfigurationresponsetypedef)
- [ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateEventRuleResponseTypeDef](./type_defs.md#updateeventruleresponsetypedef)
- [UpdateNotificationConfigurationResponseTypeDef](./type_defs.md#updatenotificationconfigurationresponsetypedef)
- [DeregisterNotificationHubResponseTypeDef](./type_defs.md#deregisternotificationhubresponsetypedef)
- [NotificationHubOverviewTypeDef](./type_defs.md#notificationhuboverviewtypedef)
- [RegisterNotificationHubResponseTypeDef](./type_defs.md#registernotificationhubresponsetypedef)
- [MessageComponentsTypeDef](./type_defs.md#messagecomponentstypedef)
- [ListChannelsRequestListChannelsPaginateTypeDef](./type_defs.md#listchannelsrequestlistchannelspaginatetypedef)
- [ListEventRulesRequestListEventRulesPaginateTypeDef](./type_defs.md#listeventrulesrequestlisteventrulespaginatetypedef)
- [ListNotificationConfigurationsRequestListNotificationConfigurationsPaginateTypeDef](./type_defs.md#listnotificationconfigurationsrequestlistnotificationconfigurationspaginatetypedef)
- [ListNotificationHubsRequestListNotificationHubsPaginateTypeDef](./type_defs.md#listnotificationhubsrequestlistnotificationhubspaginatetypedef)
- [ListNotificationConfigurationsResponseTypeDef](./type_defs.md#listnotificationconfigurationsresponsetypedef)
- [ListNotificationEventsRequestListNotificationEventsPaginateTypeDef](./type_defs.md#listnotificationeventsrequestlistnotificationeventspaginatetypedef)
- [ListNotificationEventsRequestRequestTypeDef](./type_defs.md#listnotificationeventsrequestrequesttypedef)
- [NotificationEventSummaryTypeDef](./type_defs.md#notificationeventsummarytypedef)
- [SourceEventMetadataTypeDef](./type_defs.md#sourceeventmetadatatypedef)
- [ListEventRulesResponseTypeDef](./type_defs.md#listeventrulesresponsetypedef)
- [ListNotificationHubsResponseTypeDef](./type_defs.md#listnotificationhubsresponsetypedef)
- [NotificationEventOverviewTypeDef](./type_defs.md#notificationeventoverviewtypedef)
- [NotificationEventTypeDef](./type_defs.md#notificationeventtypedef)
- [ListNotificationEventsResponseTypeDef](./type_defs.md#listnotificationeventsresponsetypedef)
- [GetNotificationEventResponseTypeDef](./type_defs.md#getnotificationeventresponsetypedef)

