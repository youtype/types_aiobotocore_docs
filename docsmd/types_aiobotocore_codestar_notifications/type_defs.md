# Type definitions

> [Index](../README.md) > [CodeStarNotifications](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeStarNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications)
    type annotations stubs module [types-aiobotocore-codestar-notifications](https://pypi.org/project/types-aiobotocore-codestar-notifications/).



## TargetTypeDef

```python
# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    TargetType: NotRequired[str],
    TargetAddress: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## DeleteNotificationRuleRequestRequestTypeDef

```python
# DeleteNotificationRuleRequestRequestTypeDef definition

class DeleteNotificationRuleRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## DeleteTargetRequestRequestTypeDef

```python
# DeleteTargetRequestRequestTypeDef definition

class DeleteTargetRequestRequestTypeDef(TypedDict):
    TargetAddress: str,
    ForceUnsubscribeAll: NotRequired[bool],
```

## DescribeNotificationRuleRequestRequestTypeDef

```python
# DescribeNotificationRuleRequestRequestTypeDef definition

class DescribeNotificationRuleRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## EventTypeSummaryTypeDef

```python
# EventTypeSummaryTypeDef definition

class EventTypeSummaryTypeDef(TypedDict):
    EventTypeId: NotRequired[str],
    ServiceName: NotRequired[str],
    EventTypeName: NotRequired[str],
    ResourceType: NotRequired[str],
```

## TargetSummaryTypeDef

```python
# TargetSummaryTypeDef definition

class TargetSummaryTypeDef(TypedDict):
    TargetAddress: NotRequired[str],
    TargetType: NotRequired[str],
    TargetStatus: NotRequired[TargetStatusType],  # (1)
```

1. See [:material-code-brackets: TargetStatusType](./literals.md#targetstatustype) 
## ListEventTypesFilterTypeDef

```python
# ListEventTypesFilterTypeDef definition

class ListEventTypesFilterTypeDef(TypedDict):
    Name: ListEventTypesFilterNameType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: ListEventTypesFilterNameType](./literals.md#listeventtypesfilternametype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListNotificationRulesFilterTypeDef

```python
# ListNotificationRulesFilterTypeDef definition

class ListNotificationRulesFilterTypeDef(TypedDict):
    Name: ListNotificationRulesFilterNameType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: ListNotificationRulesFilterNameType](./literals.md#listnotificationrulesfilternametype) 
## NotificationRuleSummaryTypeDef

```python
# NotificationRuleSummaryTypeDef definition

class NotificationRuleSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## ListTargetsFilterTypeDef

```python
# ListTargetsFilterTypeDef definition

class ListTargetsFilterTypeDef(TypedDict):
    Name: ListTargetsFilterNameType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: ListTargetsFilterNameType](./literals.md#listtargetsfilternametype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
    Tags: Mapping[str, str],
```

## UnsubscribeRequestRequestTypeDef

```python
# UnsubscribeRequestRequestTypeDef definition

class UnsubscribeRequestRequestTypeDef(TypedDict):
    Arn: str,
    TargetAddress: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    Arn: str,
    TagKeys: Sequence[str],
```

## CreateNotificationRuleRequestRequestTypeDef

```python
# CreateNotificationRuleRequestRequestTypeDef definition

class CreateNotificationRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    EventTypeIds: Sequence[str],
    Resource: str,
    Targets: Sequence[TargetTypeDef],  # (1)
    DetailType: DetailTypeType,  # (2)
    ClientRequestToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    Status: NotRequired[NotificationRuleStatusType],  # (3)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-brackets: DetailTypeType](./literals.md#detailtypetype) 
3. See [:material-code-brackets: NotificationRuleStatusType](./literals.md#notificationrulestatustype) 
## SubscribeRequestRequestTypeDef

```python
# SubscribeRequestRequestTypeDef definition

class SubscribeRequestRequestTypeDef(TypedDict):
    Arn: str,
    Target: TargetTypeDef,  # (1)
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## UpdateNotificationRuleRequestRequestTypeDef

```python
# UpdateNotificationRuleRequestRequestTypeDef definition

class UpdateNotificationRuleRequestRequestTypeDef(TypedDict):
    Arn: str,
    Name: NotRequired[str],
    Status: NotRequired[NotificationRuleStatusType],  # (1)
    EventTypeIds: NotRequired[Sequence[str]],
    Targets: NotRequired[Sequence[TargetTypeDef]],  # (2)
    DetailType: NotRequired[DetailTypeType],  # (3)
```

1. See [:material-code-brackets: NotificationRuleStatusType](./literals.md#notificationrulestatustype) 
2. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
3. See [:material-code-brackets: DetailTypeType](./literals.md#detailtypetype) 
## CreateNotificationRuleResultTypeDef

```python
# CreateNotificationRuleResultTypeDef definition

class CreateNotificationRuleResultTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteNotificationRuleResultTypeDef

```python
# DeleteNotificationRuleResultTypeDef definition

class DeleteNotificationRuleResultTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscribeResultTypeDef

```python
# SubscribeResultTypeDef definition

class SubscribeResultTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceResultTypeDef

```python
# TagResourceResultTypeDef definition

class TagResourceResultTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UnsubscribeResultTypeDef

```python
# UnsubscribeResultTypeDef definition

class UnsubscribeResultTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventTypesResultTypeDef

```python
# ListEventTypesResultTypeDef definition

class ListEventTypesResultTypeDef(TypedDict):
    EventTypes: List[EventTypeSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventTypeSummaryTypeDef](./type_defs.md#eventtypesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNotificationRuleResultTypeDef

```python
# DescribeNotificationRuleResultTypeDef definition

class DescribeNotificationRuleResultTypeDef(TypedDict):
    Arn: str,
    Name: str,
    EventTypes: List[EventTypeSummaryTypeDef],  # (1)
    Resource: str,
    Targets: List[TargetSummaryTypeDef],  # (2)
    DetailType: DetailTypeType,  # (3)
    CreatedBy: str,
    Status: NotificationRuleStatusType,  # (4)
    CreatedTimestamp: datetime,
    LastModifiedTimestamp: datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: EventTypeSummaryTypeDef](./type_defs.md#eventtypesummarytypedef) 
2. See [:material-code-braces: TargetSummaryTypeDef](./type_defs.md#targetsummarytypedef) 
3. See [:material-code-brackets: DetailTypeType](./literals.md#detailtypetype) 
4. See [:material-code-brackets: NotificationRuleStatusType](./literals.md#notificationrulestatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTargetsResultTypeDef

```python
# ListTargetsResultTypeDef definition

class ListTargetsResultTypeDef(TypedDict):
    Targets: List[TargetSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetSummaryTypeDef](./type_defs.md#targetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventTypesRequestRequestTypeDef

```python
# ListEventTypesRequestRequestTypeDef definition

class ListEventTypesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ListEventTypesFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ListEventTypesFilterTypeDef](./type_defs.md#listeventtypesfiltertypedef) 
## ListEventTypesRequestListEventTypesPaginateTypeDef

```python
# ListEventTypesRequestListEventTypesPaginateTypeDef definition

class ListEventTypesRequestListEventTypesPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ListEventTypesFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListEventTypesFilterTypeDef](./type_defs.md#listeventtypesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotificationRulesRequestListNotificationRulesPaginateTypeDef

```python
# ListNotificationRulesRequestListNotificationRulesPaginateTypeDef definition

class ListNotificationRulesRequestListNotificationRulesPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ListNotificationRulesFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListNotificationRulesFilterTypeDef](./type_defs.md#listnotificationrulesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotificationRulesRequestRequestTypeDef

```python
# ListNotificationRulesRequestRequestTypeDef definition

class ListNotificationRulesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ListNotificationRulesFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ListNotificationRulesFilterTypeDef](./type_defs.md#listnotificationrulesfiltertypedef) 
## ListNotificationRulesResultTypeDef

```python
# ListNotificationRulesResultTypeDef definition

class ListNotificationRulesResultTypeDef(TypedDict):
    NextToken: str,
    NotificationRules: List[NotificationRuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotificationRuleSummaryTypeDef](./type_defs.md#notificationrulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTargetsRequestListTargetsPaginateTypeDef

```python
# ListTargetsRequestListTargetsPaginateTypeDef definition

class ListTargetsRequestListTargetsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ListTargetsFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListTargetsFilterTypeDef](./type_defs.md#listtargetsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTargetsRequestRequestTypeDef

```python
# ListTargetsRequestRequestTypeDef definition

class ListTargetsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ListTargetsFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ListTargetsFilterTypeDef](./type_defs.md#listtargetsfiltertypedef) 
