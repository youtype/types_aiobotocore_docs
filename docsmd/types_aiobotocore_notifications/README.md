# UserNotifications module

> [Index](../README.md) > UserNotifications


!!! note ""

    Auto-generated documentation for [UserNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#usernotifications)
    type annotations stubs module [types-aiobotocore-notifications](https://pypi.org/project/types-aiobotocore-notifications/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
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
- [ListManagedNotificationChannelAssociationsPaginator](./paginators.md#listmanagednotificationchannelassociationspaginator)
- [ListManagedNotificationChildEventsPaginator](./paginators.md#listmanagednotificationchildeventspaginator)
- [ListManagedNotificationConfigurationsPaginator](./paginators.md#listmanagednotificationconfigurationspaginator)
- [ListManagedNotificationEventsPaginator](./paginators.md#listmanagednotificationeventspaginator)
- [ListNotificationConfigurationsPaginator](./paginators.md#listnotificationconfigurationspaginator)
- [ListNotificationEventsPaginator](./paginators.md#listnotificationeventspaginator)
- [ListNotificationHubsPaginator](./paginators.md#listnotificationhubspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessStatusType usage example

from types_aiobotocore_notifications.literals import AccessStatusType

def get_value() -> AccessStatusType:
    return "DISABLED"
```

- [AccessStatusType](./literals.md#accessstatustype)
- [AccountContactTypeType](./literals.md#accountcontacttypetype)
- [AggregationDurationType](./literals.md#aggregationdurationtype)
- [AggregationEventTypeType](./literals.md#aggregationeventtypetype)
- [ChannelAssociationOverrideOptionType](./literals.md#channelassociationoverrideoptiontype)
- [ChannelTypeType](./literals.md#channeltypetype)
- [EventRuleStatusType](./literals.md#eventrulestatustype)
- [EventStatusType](./literals.md#eventstatustype)
- [ListChannelsPaginatorName](./literals.md#listchannelspaginatorname)
- [ListEventRulesPaginatorName](./literals.md#listeventrulespaginatorname)
- [ListManagedNotificationChannelAssociationsPaginatorName](./literals.md#listmanagednotificationchannelassociationspaginatorname)
- [ListManagedNotificationChildEventsPaginatorName](./literals.md#listmanagednotificationchildeventspaginatorname)
- [ListManagedNotificationConfigurationsPaginatorName](./literals.md#listmanagednotificationconfigurationspaginatorname)
- [ListManagedNotificationEventsPaginatorName](./literals.md#listmanagednotificationeventspaginatorname)
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

- [SummarizationDimensionDetailTypeDef](./type_defs.md#summarizationdimensiondetailtypedef)
- [AggregationKeyTypeDef](./type_defs.md#aggregationkeytypedef)
- [SummarizationDimensionOverviewTypeDef](./type_defs.md#summarizationdimensionoverviewtypedef)
- [AssociateChannelRequestRequestTypeDef](./type_defs.md#associatechannelrequestrequesttypedef)
- [AssociateManagedNotificationAccountContactRequestRequestTypeDef](./type_defs.md#associatemanagednotificationaccountcontactrequestrequesttypedef)
- [AssociateManagedNotificationAdditionalChannelRequestRequestTypeDef](./type_defs.md#associatemanagednotificationadditionalchannelrequestrequesttypedef)
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
- [DisassociateManagedNotificationAccountContactRequestRequestTypeDef](./type_defs.md#disassociatemanagednotificationaccountcontactrequestrequesttypedef)
- [DisassociateManagedNotificationAdditionalChannelRequestRequestTypeDef](./type_defs.md#disassociatemanagednotificationadditionalchannelrequestrequesttypedef)
- [GetEventRuleRequestRequestTypeDef](./type_defs.md#geteventrulerequestrequesttypedef)
- [GetManagedNotificationChildEventRequestRequestTypeDef](./type_defs.md#getmanagednotificationchildeventrequestrequesttypedef)
- [GetManagedNotificationConfigurationRequestRequestTypeDef](./type_defs.md#getmanagednotificationconfigurationrequestrequesttypedef)
- [GetManagedNotificationEventRequestRequestTypeDef](./type_defs.md#getmanagednotificationeventrequestrequesttypedef)
- [GetNotificationConfigurationRequestRequestTypeDef](./type_defs.md#getnotificationconfigurationrequestrequesttypedef)
- [GetNotificationEventRequestRequestTypeDef](./type_defs.md#getnotificationeventrequestrequesttypedef)
- [NotificationsAccessForOrganizationTypeDef](./type_defs.md#notificationsaccessfororganizationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef)
- [ListEventRulesRequestRequestTypeDef](./type_defs.md#listeventrulesrequestrequesttypedef)
- [ListManagedNotificationChannelAssociationsRequestRequestTypeDef](./type_defs.md#listmanagednotificationchannelassociationsrequestrequesttypedef)
- [ManagedNotificationChannelAssociationSummaryTypeDef](./type_defs.md#managednotificationchannelassociationsummarytypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListManagedNotificationConfigurationsRequestRequestTypeDef](./type_defs.md#listmanagednotificationconfigurationsrequestrequesttypedef)
- [ManagedNotificationConfigurationStructureTypeDef](./type_defs.md#managednotificationconfigurationstructuretypedef)
- [ListNotificationConfigurationsRequestRequestTypeDef](./type_defs.md#listnotificationconfigurationsrequestrequesttypedef)
- [NotificationConfigurationStructureTypeDef](./type_defs.md#notificationconfigurationstructuretypedef)
- [ListNotificationHubsRequestRequestTypeDef](./type_defs.md#listnotificationhubsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ManagedSourceEventMetadataSummaryTypeDef](./type_defs.md#managedsourceeventmetadatasummarytypedef)
- [MessageComponentsSummaryTypeDef](./type_defs.md#messagecomponentssummarytypedef)
- [TextPartValueTypeDef](./type_defs.md#textpartvaluetypedef)
- [MediaElementTypeDef](./type_defs.md#mediaelementtypedef)
- [SourceEventMetadataSummaryTypeDef](./type_defs.md#sourceeventmetadatasummarytypedef)
- [RegisterNotificationHubRequestRequestTypeDef](./type_defs.md#registernotificationhubrequestrequesttypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateEventRuleRequestRequestTypeDef](./type_defs.md#updateeventrulerequestrequesttypedef)
- [UpdateNotificationConfigurationRequestRequestTypeDef](./type_defs.md#updatenotificationconfigurationrequestrequesttypedef)
- [AggregationDetailTypeDef](./type_defs.md#aggregationdetailtypedef)
- [AggregationSummaryTypeDef](./type_defs.md#aggregationsummarytypedef)
- [EventRuleStructureTypeDef](./type_defs.md#eventrulestructuretypedef)
- [CreateEventRuleResponseTypeDef](./type_defs.md#createeventruleresponsetypedef)
- [CreateNotificationConfigurationResponseTypeDef](./type_defs.md#createnotificationconfigurationresponsetypedef)
- [GetEventRuleResponseTypeDef](./type_defs.md#geteventruleresponsetypedef)
- [GetManagedNotificationConfigurationResponseTypeDef](./type_defs.md#getmanagednotificationconfigurationresponsetypedef)
- [GetNotificationConfigurationResponseTypeDef](./type_defs.md#getnotificationconfigurationresponsetypedef)
- [ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateEventRuleResponseTypeDef](./type_defs.md#updateeventruleresponsetypedef)
- [UpdateNotificationConfigurationResponseTypeDef](./type_defs.md#updatenotificationconfigurationresponsetypedef)
- [DeregisterNotificationHubResponseTypeDef](./type_defs.md#deregisternotificationhubresponsetypedef)
- [NotificationHubOverviewTypeDef](./type_defs.md#notificationhuboverviewtypedef)
- [RegisterNotificationHubResponseTypeDef](./type_defs.md#registernotificationhubresponsetypedef)
- [MessageComponentsTypeDef](./type_defs.md#messagecomponentstypedef)
- [GetNotificationsAccessForOrganizationResponseTypeDef](./type_defs.md#getnotificationsaccessfororganizationresponsetypedef)
- [ListChannelsRequestPaginateTypeDef](./type_defs.md#listchannelsrequestpaginatetypedef)
- [ListEventRulesRequestPaginateTypeDef](./type_defs.md#listeventrulesrequestpaginatetypedef)
- [ListManagedNotificationChannelAssociationsRequestPaginateTypeDef](./type_defs.md#listmanagednotificationchannelassociationsrequestpaginatetypedef)
- [ListManagedNotificationConfigurationsRequestPaginateTypeDef](./type_defs.md#listmanagednotificationconfigurationsrequestpaginatetypedef)
- [ListNotificationConfigurationsRequestPaginateTypeDef](./type_defs.md#listnotificationconfigurationsrequestpaginatetypedef)
- [ListNotificationHubsRequestPaginateTypeDef](./type_defs.md#listnotificationhubsrequestpaginatetypedef)
- [ListManagedNotificationChannelAssociationsResponseTypeDef](./type_defs.md#listmanagednotificationchannelassociationsresponsetypedef)
- [ListManagedNotificationChildEventsRequestPaginateTypeDef](./type_defs.md#listmanagednotificationchildeventsrequestpaginatetypedef)
- [ListManagedNotificationChildEventsRequestRequestTypeDef](./type_defs.md#listmanagednotificationchildeventsrequestrequesttypedef)
- [ListManagedNotificationEventsRequestPaginateTypeDef](./type_defs.md#listmanagednotificationeventsrequestpaginatetypedef)
- [ListManagedNotificationEventsRequestRequestTypeDef](./type_defs.md#listmanagednotificationeventsrequestrequesttypedef)
- [ListNotificationEventsRequestPaginateTypeDef](./type_defs.md#listnotificationeventsrequestpaginatetypedef)
- [ListNotificationEventsRequestRequestTypeDef](./type_defs.md#listnotificationeventsrequestrequesttypedef)
- [ListManagedNotificationConfigurationsResponseTypeDef](./type_defs.md#listmanagednotificationconfigurationsresponsetypedef)
- [ListNotificationConfigurationsResponseTypeDef](./type_defs.md#listnotificationconfigurationsresponsetypedef)
- [ManagedNotificationEventSummaryTypeDef](./type_defs.md#managednotificationeventsummarytypedef)
- [NotificationEventSummaryTypeDef](./type_defs.md#notificationeventsummarytypedef)
- [SourceEventMetadataTypeDef](./type_defs.md#sourceeventmetadatatypedef)
- [ManagedNotificationChildEventSummaryTypeDef](./type_defs.md#managednotificationchildeventsummarytypedef)
- [ListEventRulesResponseTypeDef](./type_defs.md#listeventrulesresponsetypedef)
- [ListNotificationHubsResponseTypeDef](./type_defs.md#listnotificationhubsresponsetypedef)
- [ManagedNotificationChildEventTypeDef](./type_defs.md#managednotificationchildeventtypedef)
- [ManagedNotificationEventTypeDef](./type_defs.md#managednotificationeventtypedef)
- [ManagedNotificationEventOverviewTypeDef](./type_defs.md#managednotificationeventoverviewtypedef)
- [NotificationEventOverviewTypeDef](./type_defs.md#notificationeventoverviewtypedef)
- [NotificationEventTypeDef](./type_defs.md#notificationeventtypedef)
- [ManagedNotificationChildEventOverviewTypeDef](./type_defs.md#managednotificationchildeventoverviewtypedef)
- [GetManagedNotificationChildEventResponseTypeDef](./type_defs.md#getmanagednotificationchildeventresponsetypedef)
- [GetManagedNotificationEventResponseTypeDef](./type_defs.md#getmanagednotificationeventresponsetypedef)
- [ListManagedNotificationEventsResponseTypeDef](./type_defs.md#listmanagednotificationeventsresponsetypedef)
- [ListNotificationEventsResponseTypeDef](./type_defs.md#listnotificationeventsresponsetypedef)
- [GetNotificationEventResponseTypeDef](./type_defs.md#getnotificationeventresponsetypedef)
- [ListManagedNotificationChildEventsResponseTypeDef](./type_defs.md#listmanagednotificationchildeventsresponsetypedef)

