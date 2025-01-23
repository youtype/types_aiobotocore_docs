# Type definitions

> [Index](../README.md) > [UserNotifications](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [UserNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#usernotifications)
    type annotations stubs module [types-aiobotocore-notifications](https://pypi.org/project/types-aiobotocore-notifications/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## SummarizationDimensionDetailTypeDef

```python
# SummarizationDimensionDetailTypeDef definition

class SummarizationDimensionDetailTypeDef(TypedDict):
    name: str,
    value: str,
```

## AggregationKeyTypeDef

```python
# AggregationKeyTypeDef definition

class AggregationKeyTypeDef(TypedDict):
    name: str,
    value: str,
```

## SummarizationDimensionOverviewTypeDef

```python
# SummarizationDimensionOverviewTypeDef definition

class SummarizationDimensionOverviewTypeDef(TypedDict):
    name: str,
    count: int,
    sampleValues: NotRequired[List[str]],
```

## AssociateChannelRequestRequestTypeDef

```python
# AssociateChannelRequestRequestTypeDef definition

class AssociateChannelRequestRequestTypeDef(TypedDict):
    arn: str,
    notificationConfigurationArn: str,
```

## AssociateManagedNotificationAccountContactRequestRequestTypeDef

```python
# AssociateManagedNotificationAccountContactRequestRequestTypeDef definition

class AssociateManagedNotificationAccountContactRequestRequestTypeDef(TypedDict):
    contactIdentifier: AccountContactTypeType,  # (1)
    managedNotificationConfigurationArn: str,
```

1. See [:material-code-brackets: AccountContactTypeType](./literals.md#accountcontacttypetype) 
## AssociateManagedNotificationAdditionalChannelRequestRequestTypeDef

```python
# AssociateManagedNotificationAdditionalChannelRequestRequestTypeDef definition

class AssociateManagedNotificationAdditionalChannelRequestRequestTypeDef(TypedDict):
    channelArn: str,
    managedNotificationConfigurationArn: str,
```

## CreateEventRuleRequestRequestTypeDef

```python
# CreateEventRuleRequestRequestTypeDef definition

class CreateEventRuleRequestRequestTypeDef(TypedDict):
    notificationConfigurationArn: str,
    source: str,
    eventType: str,
    regions: Sequence[str],
    eventPattern: NotRequired[str],
```

## EventRuleStatusSummaryTypeDef

```python
# EventRuleStatusSummaryTypeDef definition

class EventRuleStatusSummaryTypeDef(TypedDict):
    status: EventRuleStatusType,  # (1)
    reason: str,
```

1. See [:material-code-brackets: EventRuleStatusType](./literals.md#eventrulestatustype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## CreateNotificationConfigurationRequestRequestTypeDef

```python
# CreateNotificationConfigurationRequestRequestTypeDef definition

class CreateNotificationConfigurationRequestRequestTypeDef(TypedDict):
    name: str,
    description: str,
    aggregationDuration: NotRequired[AggregationDurationType],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AggregationDurationType](./literals.md#aggregationdurationtype) 
## DeleteEventRuleRequestRequestTypeDef

```python
# DeleteEventRuleRequestRequestTypeDef definition

class DeleteEventRuleRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteNotificationConfigurationRequestRequestTypeDef

```python
# DeleteNotificationConfigurationRequestRequestTypeDef definition

class DeleteNotificationConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DeregisterNotificationHubRequestRequestTypeDef

```python
# DeregisterNotificationHubRequestRequestTypeDef definition

class DeregisterNotificationHubRequestRequestTypeDef(TypedDict):
    notificationHubRegion: str,
```

## NotificationHubStatusSummaryTypeDef

```python
# NotificationHubStatusSummaryTypeDef definition

class NotificationHubStatusSummaryTypeDef(TypedDict):
    status: NotificationHubStatusType,  # (1)
    reason: str,
```

1. See [:material-code-brackets: NotificationHubStatusType](./literals.md#notificationhubstatustype) 
## DimensionTypeDef

```python
# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    name: str,
    value: str,
```

## DisassociateChannelRequestRequestTypeDef

```python
# DisassociateChannelRequestRequestTypeDef definition

class DisassociateChannelRequestRequestTypeDef(TypedDict):
    arn: str,
    notificationConfigurationArn: str,
```

## DisassociateManagedNotificationAccountContactRequestRequestTypeDef

```python
# DisassociateManagedNotificationAccountContactRequestRequestTypeDef definition

class DisassociateManagedNotificationAccountContactRequestRequestTypeDef(TypedDict):
    contactIdentifier: AccountContactTypeType,  # (1)
    managedNotificationConfigurationArn: str,
```

1. See [:material-code-brackets: AccountContactTypeType](./literals.md#accountcontacttypetype) 
## DisassociateManagedNotificationAdditionalChannelRequestRequestTypeDef

```python
# DisassociateManagedNotificationAdditionalChannelRequestRequestTypeDef definition

class DisassociateManagedNotificationAdditionalChannelRequestRequestTypeDef(TypedDict):
    channelArn: str,
    managedNotificationConfigurationArn: str,
```

## GetEventRuleRequestRequestTypeDef

```python
# GetEventRuleRequestRequestTypeDef definition

class GetEventRuleRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetManagedNotificationChildEventRequestRequestTypeDef

```python
# GetManagedNotificationChildEventRequestRequestTypeDef definition

class GetManagedNotificationChildEventRequestRequestTypeDef(TypedDict):
    arn: str,
    locale: NotRequired[LocaleCodeType],  # (1)
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
## GetManagedNotificationConfigurationRequestRequestTypeDef

```python
# GetManagedNotificationConfigurationRequestRequestTypeDef definition

class GetManagedNotificationConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetManagedNotificationEventRequestRequestTypeDef

```python
# GetManagedNotificationEventRequestRequestTypeDef definition

class GetManagedNotificationEventRequestRequestTypeDef(TypedDict):
    arn: str,
    locale: NotRequired[LocaleCodeType],  # (1)
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
## GetNotificationConfigurationRequestRequestTypeDef

```python
# GetNotificationConfigurationRequestRequestTypeDef definition

class GetNotificationConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
```

## GetNotificationEventRequestRequestTypeDef

```python
# GetNotificationEventRequestRequestTypeDef definition

class GetNotificationEventRequestRequestTypeDef(TypedDict):
    arn: str,
    locale: NotRequired[LocaleCodeType],  # (1)
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
## NotificationsAccessForOrganizationTypeDef

```python
# NotificationsAccessForOrganizationTypeDef definition

class NotificationsAccessForOrganizationTypeDef(TypedDict):
    accessStatus: AccessStatusType,  # (1)
```

1. See [:material-code-brackets: AccessStatusType](./literals.md#accessstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    notificationConfigurationArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListEventRulesRequestRequestTypeDef

```python
# ListEventRulesRequestRequestTypeDef definition

class ListEventRulesRequestRequestTypeDef(TypedDict):
    notificationConfigurationArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListManagedNotificationChannelAssociationsRequestRequestTypeDef

```python
# ListManagedNotificationChannelAssociationsRequestRequestTypeDef definition

class ListManagedNotificationChannelAssociationsRequestRequestTypeDef(TypedDict):
    managedNotificationConfigurationArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ManagedNotificationChannelAssociationSummaryTypeDef

```python
# ManagedNotificationChannelAssociationSummaryTypeDef definition

class ManagedNotificationChannelAssociationSummaryTypeDef(TypedDict):
    channelIdentifier: str,
    channelType: ChannelTypeType,  # (1)
    overrideOption: NotRequired[ChannelAssociationOverrideOptionType],  # (2)
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-brackets: ChannelAssociationOverrideOptionType](./literals.md#channelassociationoverrideoptiontype) 
## ListManagedNotificationConfigurationsRequestRequestTypeDef

```python
# ListManagedNotificationConfigurationsRequestRequestTypeDef definition

class ListManagedNotificationConfigurationsRequestRequestTypeDef(TypedDict):
    channelIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ManagedNotificationConfigurationStructureTypeDef

```python
# ManagedNotificationConfigurationStructureTypeDef definition

class ManagedNotificationConfigurationStructureTypeDef(TypedDict):
    arn: str,
    name: str,
    description: str,
```

## ListNotificationConfigurationsRequestRequestTypeDef

```python
# ListNotificationConfigurationsRequestRequestTypeDef definition

class ListNotificationConfigurationsRequestRequestTypeDef(TypedDict):
    eventRuleSource: NotRequired[str],
    channelArn: NotRequired[str],
    status: NotRequired[NotificationConfigurationStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: NotificationConfigurationStatusType](./literals.md#notificationconfigurationstatustype) 
## NotificationConfigurationStructureTypeDef

```python
# NotificationConfigurationStructureTypeDef definition

class NotificationConfigurationStructureTypeDef(TypedDict):
    arn: str,
    name: str,
    description: str,
    status: NotificationConfigurationStatusType,  # (1)
    creationTime: datetime,
    aggregationDuration: NotRequired[AggregationDurationType],  # (2)
```

1. See [:material-code-brackets: NotificationConfigurationStatusType](./literals.md#notificationconfigurationstatustype) 
2. See [:material-code-brackets: AggregationDurationType](./literals.md#aggregationdurationtype) 
## ListNotificationHubsRequestRequestTypeDef

```python
# ListNotificationHubsRequestRequestTypeDef definition

class ListNotificationHubsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    arn: str,
```

## ManagedSourceEventMetadataSummaryTypeDef

```python
# ManagedSourceEventMetadataSummaryTypeDef definition

class ManagedSourceEventMetadataSummaryTypeDef(TypedDict):
    source: str,
    eventType: str,
    eventOriginRegion: NotRequired[str],
```

## MessageComponentsSummaryTypeDef

```python
# MessageComponentsSummaryTypeDef definition

class MessageComponentsSummaryTypeDef(TypedDict):
    headline: str,
```

## TextPartValueTypeDef

```python
# TextPartValueTypeDef definition

class TextPartValueTypeDef(TypedDict):
    type: TextPartTypeType,  # (1)
    displayText: NotRequired[str],
    textByLocale: NotRequired[Dict[LocaleCodeType, str]],  # (2)
    url: NotRequired[str],
```

1. See [:material-code-brackets: TextPartTypeType](./literals.md#textparttypetype) 
2. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
## MediaElementTypeDef

```python
# MediaElementTypeDef definition

class MediaElementTypeDef(TypedDict):
    mediaId: str,
    type: MediaElementTypeType,  # (1)
    url: str,
    caption: str,
```

1. See [:material-code-brackets: MediaElementTypeType](./literals.md#mediaelementtypetype) 
## SourceEventMetadataSummaryTypeDef

```python
# SourceEventMetadataSummaryTypeDef definition

class SourceEventMetadataSummaryTypeDef(TypedDict):
    source: str,
    eventType: str,
    eventOriginRegion: NotRequired[str],
```

## RegisterNotificationHubRequestRequestTypeDef

```python
# RegisterNotificationHubRequestRequestTypeDef definition

class RegisterNotificationHubRequestRequestTypeDef(TypedDict):
    notificationHubRegion: str,
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    detailUrl: NotRequired[str],
    tags: NotRequired[List[str]],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    arn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    arn: str,
    tagKeys: Sequence[str],
```

## UpdateEventRuleRequestRequestTypeDef

```python
# UpdateEventRuleRequestRequestTypeDef definition

class UpdateEventRuleRequestRequestTypeDef(TypedDict):
    arn: str,
    eventPattern: NotRequired[str],
    regions: NotRequired[Sequence[str]],
```

## UpdateNotificationConfigurationRequestRequestTypeDef

```python
# UpdateNotificationConfigurationRequestRequestTypeDef definition

class UpdateNotificationConfigurationRequestRequestTypeDef(TypedDict):
    arn: str,
    name: NotRequired[str],
    description: NotRequired[str],
    aggregationDuration: NotRequired[AggregationDurationType],  # (1)
```

1. See [:material-code-brackets: AggregationDurationType](./literals.md#aggregationdurationtype) 
## AggregationDetailTypeDef

```python
# AggregationDetailTypeDef definition

class AggregationDetailTypeDef(TypedDict):
    summarizationDimensions: NotRequired[List[SummarizationDimensionDetailTypeDef]],  # (1)
```

1. See [:material-code-braces: SummarizationDimensionDetailTypeDef](./type_defs.md#summarizationdimensiondetailtypedef) 
## AggregationSummaryTypeDef

```python
# AggregationSummaryTypeDef definition

class AggregationSummaryTypeDef(TypedDict):
    eventCount: int,
    aggregatedBy: List[AggregationKeyTypeDef],  # (1)
    aggregatedAccounts: SummarizationDimensionOverviewTypeDef,  # (2)
    aggregatedRegions: SummarizationDimensionOverviewTypeDef,  # (2)
    aggregatedOrganizationalUnits: NotRequired[SummarizationDimensionOverviewTypeDef],  # (2)
    additionalSummarizationDimensions: NotRequired[List[SummarizationDimensionOverviewTypeDef]],  # (5)
```

1. See [:material-code-braces: AggregationKeyTypeDef](./type_defs.md#aggregationkeytypedef) 
2. See [:material-code-braces: SummarizationDimensionOverviewTypeDef](./type_defs.md#summarizationdimensionoverviewtypedef) 
3. See [:material-code-braces: SummarizationDimensionOverviewTypeDef](./type_defs.md#summarizationdimensionoverviewtypedef) 
4. See [:material-code-braces: SummarizationDimensionOverviewTypeDef](./type_defs.md#summarizationdimensionoverviewtypedef) 
5. See [:material-code-braces: SummarizationDimensionOverviewTypeDef](./type_defs.md#summarizationdimensionoverviewtypedef) 
## EventRuleStructureTypeDef

```python
# EventRuleStructureTypeDef definition

class EventRuleStructureTypeDef(TypedDict):
    arn: str,
    notificationConfigurationArn: str,
    creationTime: datetime,
    source: str,
    eventType: str,
    eventPattern: str,
    regions: List[str],
    managedRules: List[str],
    statusSummaryByRegion: Dict[str, EventRuleStatusSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: EventRuleStatusSummaryTypeDef](./type_defs.md#eventrulestatussummarytypedef) 
## CreateEventRuleResponseTypeDef

```python
# CreateEventRuleResponseTypeDef definition

class CreateEventRuleResponseTypeDef(TypedDict):
    arn: str,
    notificationConfigurationArn: str,
    statusSummaryByRegion: Dict[str, EventRuleStatusSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventRuleStatusSummaryTypeDef](./type_defs.md#eventrulestatussummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNotificationConfigurationResponseTypeDef

```python
# CreateNotificationConfigurationResponseTypeDef definition

class CreateNotificationConfigurationResponseTypeDef(TypedDict):
    arn: str,
    status: NotificationConfigurationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: NotificationConfigurationStatusType](./literals.md#notificationconfigurationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEventRuleResponseTypeDef

```python
# GetEventRuleResponseTypeDef definition

class GetEventRuleResponseTypeDef(TypedDict):
    arn: str,
    notificationConfigurationArn: str,
    creationTime: datetime,
    source: str,
    eventType: str,
    eventPattern: str,
    regions: List[str],
    managedRules: List[str],
    statusSummaryByRegion: Dict[str, EventRuleStatusSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventRuleStatusSummaryTypeDef](./type_defs.md#eventrulestatussummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetManagedNotificationConfigurationResponseTypeDef

```python
# GetManagedNotificationConfigurationResponseTypeDef definition

class GetManagedNotificationConfigurationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    description: str,
    category: str,
    subCategory: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNotificationConfigurationResponseTypeDef

```python
# GetNotificationConfigurationResponseTypeDef definition

class GetNotificationConfigurationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    description: str,
    status: NotificationConfigurationStatusType,  # (1)
    creationTime: datetime,
    aggregationDuration: AggregationDurationType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: NotificationConfigurationStatusType](./literals.md#notificationconfigurationstatustype) 
2. See [:material-code-brackets: AggregationDurationType](./literals.md#aggregationdurationtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    channels: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEventRuleResponseTypeDef

```python
# UpdateEventRuleResponseTypeDef definition

class UpdateEventRuleResponseTypeDef(TypedDict):
    arn: str,
    notificationConfigurationArn: str,
    statusSummaryByRegion: Dict[str, EventRuleStatusSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventRuleStatusSummaryTypeDef](./type_defs.md#eventrulestatussummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNotificationConfigurationResponseTypeDef

```python
# UpdateNotificationConfigurationResponseTypeDef definition

class UpdateNotificationConfigurationResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterNotificationHubResponseTypeDef

```python
# DeregisterNotificationHubResponseTypeDef definition

class DeregisterNotificationHubResponseTypeDef(TypedDict):
    notificationHubRegion: str,
    statusSummary: NotificationHubStatusSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationHubStatusSummaryTypeDef](./type_defs.md#notificationhubstatussummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotificationHubOverviewTypeDef

```python
# NotificationHubOverviewTypeDef definition

class NotificationHubOverviewTypeDef(TypedDict):
    notificationHubRegion: str,
    statusSummary: NotificationHubStatusSummaryTypeDef,  # (1)
    creationTime: datetime,
    lastActivationTime: NotRequired[datetime],
```

1. See [:material-code-braces: NotificationHubStatusSummaryTypeDef](./type_defs.md#notificationhubstatussummarytypedef) 
## RegisterNotificationHubResponseTypeDef

```python
# RegisterNotificationHubResponseTypeDef definition

class RegisterNotificationHubResponseTypeDef(TypedDict):
    notificationHubRegion: str,
    statusSummary: NotificationHubStatusSummaryTypeDef,  # (1)
    creationTime: datetime,
    lastActivationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationHubStatusSummaryTypeDef](./type_defs.md#notificationhubstatussummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageComponentsTypeDef

```python
# MessageComponentsTypeDef definition

class MessageComponentsTypeDef(TypedDict):
    headline: NotRequired[str],
    paragraphSummary: NotRequired[str],
    completeDescription: NotRequired[str],
    dimensions: NotRequired[List[DimensionTypeDef]],  # (1)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## GetNotificationsAccessForOrganizationResponseTypeDef

```python
# GetNotificationsAccessForOrganizationResponseTypeDef definition

class GetNotificationsAccessForOrganizationResponseTypeDef(TypedDict):
    notificationsAccessForOrganization: NotificationsAccessForOrganizationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationsAccessForOrganizationTypeDef](./type_defs.md#notificationsaccessfororganizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelsRequestPaginateTypeDef

```python
# ListChannelsRequestPaginateTypeDef definition

class ListChannelsRequestPaginateTypeDef(TypedDict):
    notificationConfigurationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEventRulesRequestPaginateTypeDef

```python
# ListEventRulesRequestPaginateTypeDef definition

class ListEventRulesRequestPaginateTypeDef(TypedDict):
    notificationConfigurationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedNotificationChannelAssociationsRequestPaginateTypeDef

```python
# ListManagedNotificationChannelAssociationsRequestPaginateTypeDef definition

class ListManagedNotificationChannelAssociationsRequestPaginateTypeDef(TypedDict):
    managedNotificationConfigurationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedNotificationConfigurationsRequestPaginateTypeDef

```python
# ListManagedNotificationConfigurationsRequestPaginateTypeDef definition

class ListManagedNotificationConfigurationsRequestPaginateTypeDef(TypedDict):
    channelIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotificationConfigurationsRequestPaginateTypeDef

```python
# ListNotificationConfigurationsRequestPaginateTypeDef definition

class ListNotificationConfigurationsRequestPaginateTypeDef(TypedDict):
    eventRuleSource: NotRequired[str],
    channelArn: NotRequired[str],
    status: NotRequired[NotificationConfigurationStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NotificationConfigurationStatusType](./literals.md#notificationconfigurationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotificationHubsRequestPaginateTypeDef

```python
# ListNotificationHubsRequestPaginateTypeDef definition

class ListNotificationHubsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedNotificationChannelAssociationsResponseTypeDef

```python
# ListManagedNotificationChannelAssociationsResponseTypeDef definition

class ListManagedNotificationChannelAssociationsResponseTypeDef(TypedDict):
    channelAssociations: List[ManagedNotificationChannelAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ManagedNotificationChannelAssociationSummaryTypeDef](./type_defs.md#managednotificationchannelassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedNotificationChildEventsRequestPaginateTypeDef

```python
# ListManagedNotificationChildEventsRequestPaginateTypeDef definition

class ListManagedNotificationChildEventsRequestPaginateTypeDef(TypedDict):
    aggregateManagedNotificationEventArn: str,
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    locale: NotRequired[LocaleCodeType],  # (1)
    relatedAccount: NotRequired[str],
    organizationalUnitId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedNotificationChildEventsRequestRequestTypeDef

```python
# ListManagedNotificationChildEventsRequestRequestTypeDef definition

class ListManagedNotificationChildEventsRequestRequestTypeDef(TypedDict):
    aggregateManagedNotificationEventArn: str,
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    locale: NotRequired[LocaleCodeType],  # (1)
    maxResults: NotRequired[int],
    relatedAccount: NotRequired[str],
    organizationalUnitId: NotRequired[str],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
## ListManagedNotificationEventsRequestPaginateTypeDef

```python
# ListManagedNotificationEventsRequestPaginateTypeDef definition

class ListManagedNotificationEventsRequestPaginateTypeDef(TypedDict):
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    locale: NotRequired[LocaleCodeType],  # (1)
    source: NotRequired[str],
    organizationalUnitId: NotRequired[str],
    relatedAccount: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedNotificationEventsRequestRequestTypeDef

```python
# ListManagedNotificationEventsRequestRequestTypeDef definition

class ListManagedNotificationEventsRequestRequestTypeDef(TypedDict):
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    locale: NotRequired[LocaleCodeType],  # (1)
    source: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    organizationalUnitId: NotRequired[str],
    relatedAccount: NotRequired[str],
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
## ListNotificationEventsRequestPaginateTypeDef

```python
# ListNotificationEventsRequestPaginateTypeDef definition

class ListNotificationEventsRequestPaginateTypeDef(TypedDict):
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    locale: NotRequired[LocaleCodeType],  # (1)
    source: NotRequired[str],
    includeChildEvents: NotRequired[bool],
    aggregateNotificationEventArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotificationEventsRequestRequestTypeDef

```python
# ListNotificationEventsRequestRequestTypeDef definition

class ListNotificationEventsRequestRequestTypeDef(TypedDict):
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
    locale: NotRequired[LocaleCodeType],  # (1)
    source: NotRequired[str],
    includeChildEvents: NotRequired[bool],
    aggregateNotificationEventArn: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
## ListManagedNotificationConfigurationsResponseTypeDef

```python
# ListManagedNotificationConfigurationsResponseTypeDef definition

class ListManagedNotificationConfigurationsResponseTypeDef(TypedDict):
    managedNotificationConfigurations: List[ManagedNotificationConfigurationStructureTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ManagedNotificationConfigurationStructureTypeDef](./type_defs.md#managednotificationconfigurationstructuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNotificationConfigurationsResponseTypeDef

```python
# ListNotificationConfigurationsResponseTypeDef definition

class ListNotificationConfigurationsResponseTypeDef(TypedDict):
    notificationConfigurations: List[NotificationConfigurationStructureTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NotificationConfigurationStructureTypeDef](./type_defs.md#notificationconfigurationstructuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ManagedNotificationEventSummaryTypeDef

```python
# ManagedNotificationEventSummaryTypeDef definition

class ManagedNotificationEventSummaryTypeDef(TypedDict):
    schemaVersion: SchemaVersionType,  # (1)
    sourceEventMetadata: ManagedSourceEventMetadataSummaryTypeDef,  # (2)
    messageComponents: MessageComponentsSummaryTypeDef,  # (3)
    eventStatus: EventStatusType,  # (4)
    notificationType: NotificationTypeType,  # (5)
```

1. See [:material-code-brackets: SchemaVersionType](./literals.md#schemaversiontype) 
2. See [:material-code-braces: ManagedSourceEventMetadataSummaryTypeDef](./type_defs.md#managedsourceeventmetadatasummarytypedef) 
3. See [:material-code-braces: MessageComponentsSummaryTypeDef](./type_defs.md#messagecomponentssummarytypedef) 
4. See [:material-code-brackets: EventStatusType](./literals.md#eventstatustype) 
5. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
## NotificationEventSummaryTypeDef

```python
# NotificationEventSummaryTypeDef definition

class NotificationEventSummaryTypeDef(TypedDict):
    schemaVersion: SchemaVersionType,  # (1)
    sourceEventMetadata: SourceEventMetadataSummaryTypeDef,  # (2)
    messageComponents: MessageComponentsSummaryTypeDef,  # (3)
    eventStatus: EventStatusType,  # (4)
    notificationType: NotificationTypeType,  # (5)
```

1. See [:material-code-brackets: SchemaVersionType](./literals.md#schemaversiontype) 
2. See [:material-code-braces: SourceEventMetadataSummaryTypeDef](./type_defs.md#sourceeventmetadatasummarytypedef) 
3. See [:material-code-braces: MessageComponentsSummaryTypeDef](./type_defs.md#messagecomponentssummarytypedef) 
4. See [:material-code-brackets: EventStatusType](./literals.md#eventstatustype) 
5. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
## SourceEventMetadataTypeDef

```python
# SourceEventMetadataTypeDef definition

class SourceEventMetadataTypeDef(TypedDict):
    eventTypeVersion: str,
    sourceEventId: str,
    relatedAccount: str,
    source: str,
    eventOccurrenceTime: datetime,
    eventType: str,
    relatedResources: List[ResourceTypeDef],  # (1)
    eventOriginRegion: NotRequired[str],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## ManagedNotificationChildEventSummaryTypeDef

```python
# ManagedNotificationChildEventSummaryTypeDef definition

class ManagedNotificationChildEventSummaryTypeDef(TypedDict):
    schemaVersion: SchemaVersionType,  # (1)
    sourceEventMetadata: ManagedSourceEventMetadataSummaryTypeDef,  # (2)
    messageComponents: MessageComponentsSummaryTypeDef,  # (3)
    aggregationDetail: AggregationDetailTypeDef,  # (4)
    eventStatus: EventStatusType,  # (5)
    notificationType: NotificationTypeType,  # (6)
```

1. See [:material-code-brackets: SchemaVersionType](./literals.md#schemaversiontype) 
2. See [:material-code-braces: ManagedSourceEventMetadataSummaryTypeDef](./type_defs.md#managedsourceeventmetadatasummarytypedef) 
3. See [:material-code-braces: MessageComponentsSummaryTypeDef](./type_defs.md#messagecomponentssummarytypedef) 
4. See [:material-code-braces: AggregationDetailTypeDef](./type_defs.md#aggregationdetailtypedef) 
5. See [:material-code-brackets: EventStatusType](./literals.md#eventstatustype) 
6. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
## ListEventRulesResponseTypeDef

```python
# ListEventRulesResponseTypeDef definition

class ListEventRulesResponseTypeDef(TypedDict):
    eventRules: List[EventRuleStructureTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EventRuleStructureTypeDef](./type_defs.md#eventrulestructuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNotificationHubsResponseTypeDef

```python
# ListNotificationHubsResponseTypeDef definition

class ListNotificationHubsResponseTypeDef(TypedDict):
    notificationHubs: List[NotificationHubOverviewTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NotificationHubOverviewTypeDef](./type_defs.md#notificationhuboverviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ManagedNotificationChildEventTypeDef

```python
# ManagedNotificationChildEventTypeDef definition

class ManagedNotificationChildEventTypeDef(TypedDict):
    schemaVersion: SchemaVersionType,  # (1)
    id: str,
    messageComponents: MessageComponentsTypeDef,  # (2)
    notificationType: NotificationTypeType,  # (3)
    aggregateManagedNotificationEventArn: str,
    textParts: Dict[str, TextPartValueTypeDef],  # (5)
    sourceEventDetailUrl: NotRequired[str],
    sourceEventDetailUrlDisplayText: NotRequired[str],
    eventStatus: NotRequired[EventStatusType],  # (4)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    organizationalUnitId: NotRequired[str],
    aggregationDetail: NotRequired[AggregationDetailTypeDef],  # (6)
```

1. See [:material-code-brackets: SchemaVersionType](./literals.md#schemaversiontype) 
2. See [:material-code-braces: MessageComponentsTypeDef](./type_defs.md#messagecomponentstypedef) 
3. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
4. See [:material-code-brackets: EventStatusType](./literals.md#eventstatustype) 
5. See [:material-code-braces: TextPartValueTypeDef](./type_defs.md#textpartvaluetypedef) 
6. See [:material-code-braces: AggregationDetailTypeDef](./type_defs.md#aggregationdetailtypedef) 
## ManagedNotificationEventTypeDef

```python
# ManagedNotificationEventTypeDef definition

class ManagedNotificationEventTypeDef(TypedDict):
    schemaVersion: SchemaVersionType,  # (1)
    id: str,
    messageComponents: MessageComponentsTypeDef,  # (2)
    notificationType: NotificationTypeType,  # (3)
    textParts: Dict[str, TextPartValueTypeDef],  # (7)
    sourceEventDetailUrl: NotRequired[str],
    sourceEventDetailUrlDisplayText: NotRequired[str],
    eventStatus: NotRequired[EventStatusType],  # (4)
    aggregationEventType: NotRequired[AggregationEventTypeType],  # (5)
    aggregationSummary: NotRequired[AggregationSummaryTypeDef],  # (6)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    organizationalUnitId: NotRequired[str],
```

1. See [:material-code-brackets: SchemaVersionType](./literals.md#schemaversiontype) 
2. See [:material-code-braces: MessageComponentsTypeDef](./type_defs.md#messagecomponentstypedef) 
3. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
4. See [:material-code-brackets: EventStatusType](./literals.md#eventstatustype) 
5. See [:material-code-brackets: AggregationEventTypeType](./literals.md#aggregationeventtypetype) 
6. See [:material-code-braces: AggregationSummaryTypeDef](./type_defs.md#aggregationsummarytypedef) 
7. See [:material-code-braces: TextPartValueTypeDef](./type_defs.md#textpartvaluetypedef) 
## ManagedNotificationEventOverviewTypeDef

```python
# ManagedNotificationEventOverviewTypeDef definition

class ManagedNotificationEventOverviewTypeDef(TypedDict):
    arn: str,
    managedNotificationConfigurationArn: str,
    relatedAccount: str,
    creationTime: datetime,
    notificationEvent: ManagedNotificationEventSummaryTypeDef,  # (1)
    aggregationEventType: NotRequired[AggregationEventTypeType],  # (2)
    organizationalUnitId: NotRequired[str],
    aggregationSummary: NotRequired[AggregationSummaryTypeDef],  # (3)
    aggregatedNotificationRegions: NotRequired[List[str]],
```

1. See [:material-code-braces: ManagedNotificationEventSummaryTypeDef](./type_defs.md#managednotificationeventsummarytypedef) 
2. See [:material-code-brackets: AggregationEventTypeType](./literals.md#aggregationeventtypetype) 
3. See [:material-code-braces: AggregationSummaryTypeDef](./type_defs.md#aggregationsummarytypedef) 
## NotificationEventOverviewTypeDef

```python
# NotificationEventOverviewTypeDef definition

class NotificationEventOverviewTypeDef(TypedDict):
    arn: str,
    notificationConfigurationArn: str,
    relatedAccount: str,
    creationTime: datetime,
    notificationEvent: NotificationEventSummaryTypeDef,  # (1)
    aggregationEventType: NotRequired[AggregationEventTypeType],  # (2)
    aggregateNotificationEventArn: NotRequired[str],
    aggregationSummary: NotRequired[AggregationSummaryTypeDef],  # (3)
```

1. See [:material-code-braces: NotificationEventSummaryTypeDef](./type_defs.md#notificationeventsummarytypedef) 
2. See [:material-code-brackets: AggregationEventTypeType](./literals.md#aggregationeventtypetype) 
3. See [:material-code-braces: AggregationSummaryTypeDef](./type_defs.md#aggregationsummarytypedef) 
## NotificationEventTypeDef

```python
# NotificationEventTypeDef definition

class NotificationEventTypeDef(TypedDict):
    schemaVersion: SchemaVersionType,  # (1)
    id: str,
    sourceEventMetadata: SourceEventMetadataTypeDef,  # (2)
    messageComponents: MessageComponentsTypeDef,  # (3)
    notificationType: NotificationTypeType,  # (4)
    textParts: Dict[str, TextPartValueTypeDef],  # (8)
    media: List[MediaElementTypeDef],  # (9)
    sourceEventDetailUrl: NotRequired[str],
    sourceEventDetailUrlDisplayText: NotRequired[str],
    eventStatus: NotRequired[EventStatusType],  # (5)
    aggregationEventType: NotRequired[AggregationEventTypeType],  # (6)
    aggregateNotificationEventArn: NotRequired[str],
    aggregationSummary: NotRequired[AggregationSummaryTypeDef],  # (7)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

1. See [:material-code-brackets: SchemaVersionType](./literals.md#schemaversiontype) 
2. See [:material-code-braces: SourceEventMetadataTypeDef](./type_defs.md#sourceeventmetadatatypedef) 
3. See [:material-code-braces: MessageComponentsTypeDef](./type_defs.md#messagecomponentstypedef) 
4. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
5. See [:material-code-brackets: EventStatusType](./literals.md#eventstatustype) 
6. See [:material-code-brackets: AggregationEventTypeType](./literals.md#aggregationeventtypetype) 
7. See [:material-code-braces: AggregationSummaryTypeDef](./type_defs.md#aggregationsummarytypedef) 
8. See [:material-code-braces: TextPartValueTypeDef](./type_defs.md#textpartvaluetypedef) 
9. See [:material-code-braces: MediaElementTypeDef](./type_defs.md#mediaelementtypedef) 
## ManagedNotificationChildEventOverviewTypeDef

```python
# ManagedNotificationChildEventOverviewTypeDef definition

class ManagedNotificationChildEventOverviewTypeDef(TypedDict):
    arn: str,
    managedNotificationConfigurationArn: str,
    relatedAccount: str,
    creationTime: datetime,
    childEvent: ManagedNotificationChildEventSummaryTypeDef,  # (1)
    aggregateManagedNotificationEventArn: str,
    organizationalUnitId: NotRequired[str],
```

1. See [:material-code-braces: ManagedNotificationChildEventSummaryTypeDef](./type_defs.md#managednotificationchildeventsummarytypedef) 
## GetManagedNotificationChildEventResponseTypeDef

```python
# GetManagedNotificationChildEventResponseTypeDef definition

class GetManagedNotificationChildEventResponseTypeDef(TypedDict):
    arn: str,
    managedNotificationConfigurationArn: str,
    creationTime: datetime,
    content: ManagedNotificationChildEventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedNotificationChildEventTypeDef](./type_defs.md#managednotificationchildeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetManagedNotificationEventResponseTypeDef

```python
# GetManagedNotificationEventResponseTypeDef definition

class GetManagedNotificationEventResponseTypeDef(TypedDict):
    arn: str,
    managedNotificationConfigurationArn: str,
    creationTime: datetime,
    content: ManagedNotificationEventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedNotificationEventTypeDef](./type_defs.md#managednotificationeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedNotificationEventsResponseTypeDef

```python
# ListManagedNotificationEventsResponseTypeDef definition

class ListManagedNotificationEventsResponseTypeDef(TypedDict):
    managedNotificationEvents: List[ManagedNotificationEventOverviewTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ManagedNotificationEventOverviewTypeDef](./type_defs.md#managednotificationeventoverviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNotificationEventsResponseTypeDef

```python
# ListNotificationEventsResponseTypeDef definition

class ListNotificationEventsResponseTypeDef(TypedDict):
    notificationEvents: List[NotificationEventOverviewTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NotificationEventOverviewTypeDef](./type_defs.md#notificationeventoverviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNotificationEventResponseTypeDef

```python
# GetNotificationEventResponseTypeDef definition

class GetNotificationEventResponseTypeDef(TypedDict):
    arn: str,
    notificationConfigurationArn: str,
    creationTime: datetime,
    content: NotificationEventTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationEventTypeDef](./type_defs.md#notificationeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedNotificationChildEventsResponseTypeDef

```python
# ListManagedNotificationChildEventsResponseTypeDef definition

class ListManagedNotificationChildEventsResponseTypeDef(TypedDict):
    managedNotificationChildEvents: List[ManagedNotificationChildEventOverviewTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ManagedNotificationChildEventOverviewTypeDef](./type_defs.md#managednotificationchildeventoverviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
