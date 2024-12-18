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




## AssociateChannelRequestRequestTypeDef

```python
# AssociateChannelRequestRequestTypeDef definition

class AssociateChannelRequestRequestTypeDef(TypedDict):
    arn: str,
    notificationConfigurationArn: str,
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

## GetEventRuleRequestRequestTypeDef

```python
# GetEventRuleRequestRequestTypeDef definition

class GetEventRuleRequestRequestTypeDef(TypedDict):
    arn: str,
```

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
## MessageComponentsSummaryTypeDef

```python
# MessageComponentsSummaryTypeDef definition

class MessageComponentsSummaryTypeDef(TypedDict):
    headline: str,
```

## SourceEventMetadataSummaryTypeDef

```python
# SourceEventMetadataSummaryTypeDef definition

class SourceEventMetadataSummaryTypeDef(TypedDict):
    source: str,
    eventType: str,
    eventOriginRegion: NotRequired[str],
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
## ListChannelsRequestListChannelsPaginateTypeDef

```python
# ListChannelsRequestListChannelsPaginateTypeDef definition

class ListChannelsRequestListChannelsPaginateTypeDef(TypedDict):
    notificationConfigurationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEventRulesRequestListEventRulesPaginateTypeDef

```python
# ListEventRulesRequestListEventRulesPaginateTypeDef definition

class ListEventRulesRequestListEventRulesPaginateTypeDef(TypedDict):
    notificationConfigurationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotificationConfigurationsRequestListNotificationConfigurationsPaginateTypeDef

```python
# ListNotificationConfigurationsRequestListNotificationConfigurationsPaginateTypeDef definition

class ListNotificationConfigurationsRequestListNotificationConfigurationsPaginateTypeDef(TypedDict):
    eventRuleSource: NotRequired[str],
    channelArn: NotRequired[str],
    status: NotRequired[NotificationConfigurationStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NotificationConfigurationStatusType](./literals.md#notificationconfigurationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotificationHubsRequestListNotificationHubsPaginateTypeDef

```python
# ListNotificationHubsRequestListNotificationHubsPaginateTypeDef definition

class ListNotificationHubsRequestListNotificationHubsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
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
## ListNotificationEventsRequestListNotificationEventsPaginateTypeDef

```python
# ListNotificationEventsRequestListNotificationEventsPaginateTypeDef definition

class ListNotificationEventsRequestListNotificationEventsPaginateTypeDef(TypedDict):
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
```

1. See [:material-code-braces: NotificationEventSummaryTypeDef](./type_defs.md#notificationeventsummarytypedef) 
2. See [:material-code-brackets: AggregationEventTypeType](./literals.md#aggregationeventtypetype) 
## NotificationEventTypeDef

```python
# NotificationEventTypeDef definition

class NotificationEventTypeDef(TypedDict):
    schemaVersion: SchemaVersionType,  # (1)
    id: str,
    sourceEventMetadata: SourceEventMetadataTypeDef,  # (2)
    messageComponents: MessageComponentsTypeDef,  # (3)
    notificationType: NotificationTypeType,  # (4)
    textParts: Dict[str, TextPartValueTypeDef],  # (7)
    media: List[MediaElementTypeDef],  # (8)
    sourceEventDetailUrl: NotRequired[str],
    sourceEventDetailUrlDisplayText: NotRequired[str],
    eventStatus: NotRequired[EventStatusType],  # (5)
    aggregationEventType: NotRequired[AggregationEventTypeType],  # (6)
    aggregateNotificationEventArn: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
```

1. See [:material-code-brackets: SchemaVersionType](./literals.md#schemaversiontype) 
2. See [:material-code-braces: SourceEventMetadataTypeDef](./type_defs.md#sourceeventmetadatatypedef) 
3. See [:material-code-braces: MessageComponentsTypeDef](./type_defs.md#messagecomponentstypedef) 
4. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
5. See [:material-code-brackets: EventStatusType](./literals.md#eventstatustype) 
6. See [:material-code-brackets: AggregationEventTypeType](./literals.md#aggregationeventtypetype) 
7. See [:material-code-braces: TextPartValueTypeDef](./type_defs.md#textpartvaluetypedef) 
8. See [:material-code-braces: MediaElementTypeDef](./type_defs.md#mediaelementtypedef) 
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
