# Type definitions

> [Index](../README.md) > [Health](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Health](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#health)
    type annotations stubs module [types-aiobotocore-health](https://pypi.org/project/types-aiobotocore-health/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AccountEntityAggregateTypeDef

```python
# AccountEntityAggregateTypeDef definition

class AccountEntityAggregateTypeDef(TypedDict):
    accountId: NotRequired[str],
    count: NotRequired[int],
    statuses: NotRequired[Dict[EntityStatusCodeType, int]],  # (1)
```

1. See [:material-code-brackets: EntityStatusCodeType](./literals.md#entitystatuscodetype) 
## AffectedEntityTypeDef

```python
# AffectedEntityTypeDef definition

class AffectedEntityTypeDef(TypedDict):
    entityArn: NotRequired[str],
    eventArn: NotRequired[str],
    entityValue: NotRequired[str],
    entityUrl: NotRequired[str],
    awsAccountId: NotRequired[str],
    lastUpdatedTime: NotRequired[datetime],
    statusCode: NotRequired[EntityStatusCodeType],  # (1)
    tags: NotRequired[Dict[str, str]],
    entityMetadata: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: EntityStatusCodeType](./literals.md#entitystatuscodetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAffectedAccountsForOrganizationRequestRequestTypeDef

```python
# DescribeAffectedAccountsForOrganizationRequestRequestTypeDef definition

class DescribeAffectedAccountsForOrganizationRequestRequestTypeDef(TypedDict):
    eventArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

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

## EntityAccountFilterTypeDef

```python
# EntityAccountFilterTypeDef definition

class EntityAccountFilterTypeDef(TypedDict):
    eventArn: str,
    awsAccountId: NotRequired[str],
    statusCodes: NotRequired[Sequence[EntityStatusCodeType]],  # (1)
```

1. See [:material-code-brackets: EntityStatusCodeType](./literals.md#entitystatuscodetype) 
## EventAccountFilterTypeDef

```python
# EventAccountFilterTypeDef definition

class EventAccountFilterTypeDef(TypedDict):
    eventArn: str,
    awsAccountId: NotRequired[str],
```

## OrganizationAffectedEntitiesErrorItemTypeDef

```python
# OrganizationAffectedEntitiesErrorItemTypeDef definition

class OrganizationAffectedEntitiesErrorItemTypeDef(TypedDict):
    awsAccountId: NotRequired[str],
    eventArn: NotRequired[str],
    errorName: NotRequired[str],
    errorMessage: NotRequired[str],
```

## DescribeEntityAggregatesForOrganizationRequestRequestTypeDef

```python
# DescribeEntityAggregatesForOrganizationRequestRequestTypeDef definition

class DescribeEntityAggregatesForOrganizationRequestRequestTypeDef(TypedDict):
    eventArns: Sequence[str],
    awsAccountIds: NotRequired[Sequence[str]],
```

## DescribeEntityAggregatesRequestRequestTypeDef

```python
# DescribeEntityAggregatesRequestRequestTypeDef definition

class DescribeEntityAggregatesRequestRequestTypeDef(TypedDict):
    eventArns: NotRequired[Sequence[str]],
```

## EntityAggregateTypeDef

```python
# EntityAggregateTypeDef definition

class EntityAggregateTypeDef(TypedDict):
    eventArn: NotRequired[str],
    count: NotRequired[int],
    statuses: NotRequired[Dict[EntityStatusCodeType, int]],  # (1)
```

1. See [:material-code-brackets: EntityStatusCodeType](./literals.md#entitystatuscodetype) 
## EventAggregateTypeDef

```python
# EventAggregateTypeDef definition

class EventAggregateTypeDef(TypedDict):
    aggregateValue: NotRequired[str],
    count: NotRequired[int],
```

## OrganizationEventDetailsErrorItemTypeDef

```python
# OrganizationEventDetailsErrorItemTypeDef definition

class OrganizationEventDetailsErrorItemTypeDef(TypedDict):
    awsAccountId: NotRequired[str],
    eventArn: NotRequired[str],
    errorName: NotRequired[str],
    errorMessage: NotRequired[str],
```

## DescribeEventDetailsRequestRequestTypeDef

```python
# DescribeEventDetailsRequestRequestTypeDef definition

class DescribeEventDetailsRequestRequestTypeDef(TypedDict):
    eventArns: Sequence[str],
    locale: NotRequired[str],
```

## EventDetailsErrorItemTypeDef

```python
# EventDetailsErrorItemTypeDef definition

class EventDetailsErrorItemTypeDef(TypedDict):
    eventArn: NotRequired[str],
    errorName: NotRequired[str],
    errorMessage: NotRequired[str],
```

## EventTypeFilterTypeDef

```python
# EventTypeFilterTypeDef definition

class EventTypeFilterTypeDef(TypedDict):
    eventTypeCodes: NotRequired[Sequence[str]],
    services: NotRequired[Sequence[str]],
    eventTypeCategories: NotRequired[Sequence[EventTypeCategoryType]],  # (1)
```

1. See [:material-code-brackets: EventTypeCategoryType](./literals.md#eventtypecategorytype) 
## EventTypeTypeDef

```python
# EventTypeTypeDef definition

class EventTypeTypeDef(TypedDict):
    service: NotRequired[str],
    code: NotRequired[str],
    category: NotRequired[EventTypeCategoryType],  # (1)
```

1. See [:material-code-brackets: EventTypeCategoryType](./literals.md#eventtypecategorytype) 
## OrganizationEventTypeDef

```python
# OrganizationEventTypeDef definition

class OrganizationEventTypeDef(TypedDict):
    arn: NotRequired[str],
    service: NotRequired[str],
    eventTypeCode: NotRequired[str],
    eventTypeCategory: NotRequired[EventTypeCategoryType],  # (1)
    eventScopeCode: NotRequired[EventScopeCodeType],  # (2)
    region: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
    statusCode: NotRequired[EventStatusCodeType],  # (3)
```

1. See [:material-code-brackets: EventTypeCategoryType](./literals.md#eventtypecategorytype) 
2. See [:material-code-brackets: EventScopeCodeType](./literals.md#eventscopecodetype) 
3. See [:material-code-brackets: EventStatusCodeType](./literals.md#eventstatuscodetype) 
## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    arn: NotRequired[str],
    service: NotRequired[str],
    eventTypeCode: NotRequired[str],
    eventTypeCategory: NotRequired[EventTypeCategoryType],  # (1)
    region: NotRequired[str],
    availabilityZone: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
    statusCode: NotRequired[EventStatusCodeType],  # (2)
    eventScopeCode: NotRequired[EventScopeCodeType],  # (3)
```

1. See [:material-code-brackets: EventTypeCategoryType](./literals.md#eventtypecategorytype) 
2. See [:material-code-brackets: EventStatusCodeType](./literals.md#eventstatuscodetype) 
3. See [:material-code-brackets: EventScopeCodeType](./literals.md#eventscopecodetype) 
## EventDescriptionTypeDef

```python
# EventDescriptionTypeDef definition

class EventDescriptionTypeDef(TypedDict):
    latestDescription: NotRequired[str],
```

## OrganizationEntityAggregateTypeDef

```python
# OrganizationEntityAggregateTypeDef definition

class OrganizationEntityAggregateTypeDef(TypedDict):
    eventArn: NotRequired[str],
    count: NotRequired[int],
    statuses: NotRequired[Dict[EntityStatusCodeType, int]],  # (1)
    accounts: NotRequired[List[AccountEntityAggregateTypeDef]],  # (2)
```

1. See [:material-code-brackets: EntityStatusCodeType](./literals.md#entitystatuscodetype) 
2. See [:material-code-braces: AccountEntityAggregateTypeDef](./type_defs.md#accountentityaggregatetypedef) 
## DateTimeRangeTypeDef

```python
# DateTimeRangeTypeDef definition

class DateTimeRangeTypeDef(TypedDict):
    from: NotRequired[TimestampTypeDef],
    to: NotRequired[TimestampTypeDef],
```

## DescribeAffectedAccountsForOrganizationRequestPaginateTypeDef

```python
# DescribeAffectedAccountsForOrganizationRequestPaginateTypeDef definition

class DescribeAffectedAccountsForOrganizationRequestPaginateTypeDef(TypedDict):
    eventArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAffectedAccountsForOrganizationResponseTypeDef

```python
# DescribeAffectedAccountsForOrganizationResponseTypeDef definition

class DescribeAffectedAccountsForOrganizationResponseTypeDef(TypedDict):
    affectedAccounts: List[str],
    eventScopeCode: EventScopeCodeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: EventScopeCodeType](./literals.md#eventscopecodetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAffectedEntitiesResponseTypeDef

```python
# DescribeAffectedEntitiesResponseTypeDef definition

class DescribeAffectedEntitiesResponseTypeDef(TypedDict):
    entities: List[AffectedEntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AffectedEntityTypeDef](./type_defs.md#affectedentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeHealthServiceStatusForOrganizationResponseTypeDef

```python
# DescribeHealthServiceStatusForOrganizationResponseTypeDef definition

class DescribeHealthServiceStatusForOrganizationResponseTypeDef(TypedDict):
    healthServiceAccessStatusForOrganization: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAffectedEntitiesForOrganizationRequestPaginateTypeDef

```python
# DescribeAffectedEntitiesForOrganizationRequestPaginateTypeDef definition

class DescribeAffectedEntitiesForOrganizationRequestPaginateTypeDef(TypedDict):
    organizationEntityFilters: NotRequired[Sequence[EventAccountFilterTypeDef]],  # (1)
    locale: NotRequired[str],
    organizationEntityAccountFilters: NotRequired[Sequence[EntityAccountFilterTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef) 
2. See [:material-code-braces: EntityAccountFilterTypeDef](./type_defs.md#entityaccountfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef

```python
# DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef definition

class DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef(TypedDict):
    organizationEntityFilters: NotRequired[Sequence[EventAccountFilterTypeDef]],  # (1)
    locale: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    organizationEntityAccountFilters: NotRequired[Sequence[EntityAccountFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef) 
2. See [:material-code-braces: EntityAccountFilterTypeDef](./type_defs.md#entityaccountfiltertypedef) 
## DescribeEventDetailsForOrganizationRequestRequestTypeDef

```python
# DescribeEventDetailsForOrganizationRequestRequestTypeDef definition

class DescribeEventDetailsForOrganizationRequestRequestTypeDef(TypedDict):
    organizationEventDetailFilters: Sequence[EventAccountFilterTypeDef],  # (1)
    locale: NotRequired[str],
```

1. See [:material-code-braces: EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef) 
## DescribeAffectedEntitiesForOrganizationResponseTypeDef

```python
# DescribeAffectedEntitiesForOrganizationResponseTypeDef definition

class DescribeAffectedEntitiesForOrganizationResponseTypeDef(TypedDict):
    entities: List[AffectedEntityTypeDef],  # (1)
    failedSet: List[OrganizationAffectedEntitiesErrorItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AffectedEntityTypeDef](./type_defs.md#affectedentitytypedef) 
2. See [:material-code-braces: OrganizationAffectedEntitiesErrorItemTypeDef](./type_defs.md#organizationaffectedentitieserroritemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEntityAggregatesResponseTypeDef

```python
# DescribeEntityAggregatesResponseTypeDef definition

class DescribeEntityAggregatesResponseTypeDef(TypedDict):
    entityAggregates: List[EntityAggregateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntityAggregateTypeDef](./type_defs.md#entityaggregatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventAggregatesResponseTypeDef

```python
# DescribeEventAggregatesResponseTypeDef definition

class DescribeEventAggregatesResponseTypeDef(TypedDict):
    eventAggregates: List[EventAggregateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EventAggregateTypeDef](./type_defs.md#eventaggregatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventTypesRequestPaginateTypeDef

```python
# DescribeEventTypesRequestPaginateTypeDef definition

class DescribeEventTypesRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[EventTypeFilterTypeDef],  # (1)
    locale: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EventTypeFilterTypeDef](./type_defs.md#eventtypefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventTypesRequestRequestTypeDef

```python
# DescribeEventTypesRequestRequestTypeDef definition

class DescribeEventTypesRequestRequestTypeDef(TypedDict):
    filter: NotRequired[EventTypeFilterTypeDef],  # (1)
    locale: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: EventTypeFilterTypeDef](./type_defs.md#eventtypefiltertypedef) 
## DescribeEventTypesResponseTypeDef

```python
# DescribeEventTypesResponseTypeDef definition

class DescribeEventTypesResponseTypeDef(TypedDict):
    eventTypes: List[EventTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EventTypeTypeDef](./type_defs.md#eventtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventsForOrganizationResponseTypeDef

```python
# DescribeEventsForOrganizationResponseTypeDef definition

class DescribeEventsForOrganizationResponseTypeDef(TypedDict):
    events: List[OrganizationEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationEventTypeDef](./type_defs.md#organizationeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventsResponseTypeDef

```python
# DescribeEventsResponseTypeDef definition

class DescribeEventsResponseTypeDef(TypedDict):
    events: List[EventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventDetailsTypeDef

```python
# EventDetailsTypeDef definition

class EventDetailsTypeDef(TypedDict):
    event: NotRequired[EventTypeDef],  # (1)
    eventDescription: NotRequired[EventDescriptionTypeDef],  # (2)
    eventMetadata: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: EventDescriptionTypeDef](./type_defs.md#eventdescriptiontypedef) 
## OrganizationEventDetailsTypeDef

```python
# OrganizationEventDetailsTypeDef definition

class OrganizationEventDetailsTypeDef(TypedDict):
    awsAccountId: NotRequired[str],
    event: NotRequired[EventTypeDef],  # (1)
    eventDescription: NotRequired[EventDescriptionTypeDef],  # (2)
    eventMetadata: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: EventDescriptionTypeDef](./type_defs.md#eventdescriptiontypedef) 
## DescribeEntityAggregatesForOrganizationResponseTypeDef

```python
# DescribeEntityAggregatesForOrganizationResponseTypeDef definition

class DescribeEntityAggregatesForOrganizationResponseTypeDef(TypedDict):
    organizationEntityAggregates: List[OrganizationEntityAggregateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationEntityAggregateTypeDef](./type_defs.md#organizationentityaggregatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EntityFilterTypeDef

```python
# EntityFilterTypeDef definition

class EntityFilterTypeDef(TypedDict):
    eventArns: Sequence[str],
    entityArns: NotRequired[Sequence[str]],
    entityValues: NotRequired[Sequence[str]],
    lastUpdatedTimes: NotRequired[Sequence[DateTimeRangeTypeDef]],  # (1)
    tags: NotRequired[Sequence[Mapping[str, str]]],
    statusCodes: NotRequired[Sequence[EntityStatusCodeType]],  # (2)
```

1. See [:material-code-braces: DateTimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
2. See [:material-code-brackets: EntityStatusCodeType](./literals.md#entitystatuscodetype) 
## EventFilterTypeDef

```python
# EventFilterTypeDef definition

class EventFilterTypeDef(TypedDict):
    eventArns: NotRequired[Sequence[str]],
    eventTypeCodes: NotRequired[Sequence[str]],
    services: NotRequired[Sequence[str]],
    regions: NotRequired[Sequence[str]],
    availabilityZones: NotRequired[Sequence[str]],
    startTimes: NotRequired[Sequence[DateTimeRangeTypeDef]],  # (1)
    endTimes: NotRequired[Sequence[DateTimeRangeTypeDef]],  # (1)
    lastUpdatedTimes: NotRequired[Sequence[DateTimeRangeTypeDef]],  # (1)
    entityArns: NotRequired[Sequence[str]],
    entityValues: NotRequired[Sequence[str]],
    eventTypeCategories: NotRequired[Sequence[EventTypeCategoryType]],  # (4)
    tags: NotRequired[Sequence[Mapping[str, str]]],
    eventStatusCodes: NotRequired[Sequence[EventStatusCodeType]],  # (5)
```

1. See [:material-code-braces: DateTimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
2. See [:material-code-braces: DateTimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
3. See [:material-code-braces: DateTimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
4. See [:material-code-brackets: EventTypeCategoryType](./literals.md#eventtypecategorytype) 
5. See [:material-code-brackets: EventStatusCodeType](./literals.md#eventstatuscodetype) 
## OrganizationEventFilterTypeDef

```python
# OrganizationEventFilterTypeDef definition

class OrganizationEventFilterTypeDef(TypedDict):
    eventTypeCodes: NotRequired[Sequence[str]],
    awsAccountIds: NotRequired[Sequence[str]],
    services: NotRequired[Sequence[str]],
    regions: NotRequired[Sequence[str]],
    startTime: NotRequired[DateTimeRangeTypeDef],  # (1)
    endTime: NotRequired[DateTimeRangeTypeDef],  # (1)
    lastUpdatedTime: NotRequired[DateTimeRangeTypeDef],  # (1)
    entityArns: NotRequired[Sequence[str]],
    entityValues: NotRequired[Sequence[str]],
    eventTypeCategories: NotRequired[Sequence[EventTypeCategoryType]],  # (4)
    eventStatusCodes: NotRequired[Sequence[EventStatusCodeType]],  # (5)
```

1. See [:material-code-braces: DateTimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
2. See [:material-code-braces: DateTimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
3. See [:material-code-braces: DateTimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
4. See [:material-code-brackets: EventTypeCategoryType](./literals.md#eventtypecategorytype) 
5. See [:material-code-brackets: EventStatusCodeType](./literals.md#eventstatuscodetype) 
## DescribeEventDetailsResponseTypeDef

```python
# DescribeEventDetailsResponseTypeDef definition

class DescribeEventDetailsResponseTypeDef(TypedDict):
    successfulSet: List[EventDetailsTypeDef],  # (1)
    failedSet: List[EventDetailsErrorItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EventDetailsTypeDef](./type_defs.md#eventdetailstypedef) 
2. See [:material-code-braces: EventDetailsErrorItemTypeDef](./type_defs.md#eventdetailserroritemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventDetailsForOrganizationResponseTypeDef

```python
# DescribeEventDetailsForOrganizationResponseTypeDef definition

class DescribeEventDetailsForOrganizationResponseTypeDef(TypedDict):
    successfulSet: List[OrganizationEventDetailsTypeDef],  # (1)
    failedSet: List[OrganizationEventDetailsErrorItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: OrganizationEventDetailsTypeDef](./type_defs.md#organizationeventdetailstypedef) 
2. See [:material-code-braces: OrganizationEventDetailsErrorItemTypeDef](./type_defs.md#organizationeventdetailserroritemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAffectedEntitiesRequestPaginateTypeDef

```python
# DescribeAffectedEntitiesRequestPaginateTypeDef definition

class DescribeAffectedEntitiesRequestPaginateTypeDef(TypedDict):
    filter: EntityFilterTypeDef,  # (1)
    locale: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EntityFilterTypeDef](./type_defs.md#entityfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAffectedEntitiesRequestRequestTypeDef

```python
# DescribeAffectedEntitiesRequestRequestTypeDef definition

class DescribeAffectedEntitiesRequestRequestTypeDef(TypedDict):
    filter: EntityFilterTypeDef,  # (1)
    locale: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: EntityFilterTypeDef](./type_defs.md#entityfiltertypedef) 
## DescribeEventAggregatesRequestPaginateTypeDef

```python
# DescribeEventAggregatesRequestPaginateTypeDef definition

class DescribeEventAggregatesRequestPaginateTypeDef(TypedDict):
    aggregateField: EventAggregateFieldType,  # (1)
    filter: NotRequired[EventFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EventAggregateFieldType](./literals.md#eventaggregatefieldtype) 
2. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventAggregatesRequestRequestTypeDef

```python
# DescribeEventAggregatesRequestRequestTypeDef definition

class DescribeEventAggregatesRequestRequestTypeDef(TypedDict):
    aggregateField: EventAggregateFieldType,  # (1)
    filter: NotRequired[EventFilterTypeDef],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: EventAggregateFieldType](./literals.md#eventaggregatefieldtype) 
2. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
## DescribeEventsRequestPaginateTypeDef

```python
# DescribeEventsRequestPaginateTypeDef definition

class DescribeEventsRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[EventFilterTypeDef],  # (1)
    locale: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsRequestRequestTypeDef

```python
# DescribeEventsRequestRequestTypeDef definition

class DescribeEventsRequestRequestTypeDef(TypedDict):
    filter: NotRequired[EventFilterTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    locale: NotRequired[str],
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
## DescribeEventsForOrganizationRequestPaginateTypeDef

```python
# DescribeEventsForOrganizationRequestPaginateTypeDef definition

class DescribeEventsForOrganizationRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[OrganizationEventFilterTypeDef],  # (1)
    locale: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OrganizationEventFilterTypeDef](./type_defs.md#organizationeventfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsForOrganizationRequestRequestTypeDef

```python
# DescribeEventsForOrganizationRequestRequestTypeDef definition

class DescribeEventsForOrganizationRequestRequestTypeDef(TypedDict):
    filter: NotRequired[OrganizationEventFilterTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    locale: NotRequired[str],
```

1. See [:material-code-braces: OrganizationEventFilterTypeDef](./type_defs.md#organizationeventfiltertypedef) 
