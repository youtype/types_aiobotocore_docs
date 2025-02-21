# Type definitions

> [Index](../README.md) > [Health](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Health](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#health)
    type annotations stubs module [types-aiobotocore-health](https://pypi.org/project/types-aiobotocore-health/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_health.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AccountEntityAggregateTypeDef

```python
# AccountEntityAggregateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import AccountEntityAggregateTypeDef


def get_value() -> AccountEntityAggregateTypeDef:
    return {
        "accountId": ...,
    }


# AccountEntityAggregateTypeDef definition

class AccountEntityAggregateTypeDef(TypedDict):
    accountId: NotRequired[str],
    count: NotRequired[int],
    statuses: NotRequired[Dict[EntityStatusCodeType, int]],  # (1)
```

1. See [:material-code-brackets: EntityStatusCodeType](./literals.md#entitystatuscodetype) 
## AffectedEntityTypeDef

```python
# AffectedEntityTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import AffectedEntityTypeDef


def get_value() -> AffectedEntityTypeDef:
    return {
        "entityArn": ...,
    }


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
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAffectedAccountsForOrganizationRequestTypeDef

```python
# DescribeAffectedAccountsForOrganizationRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeAffectedAccountsForOrganizationRequestTypeDef


def get_value() -> DescribeAffectedAccountsForOrganizationRequestTypeDef:
    return {
        "eventArn": ...,
    }


# DescribeAffectedAccountsForOrganizationRequestTypeDef definition

class DescribeAffectedAccountsForOrganizationRequestTypeDef(TypedDict):
    eventArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


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
# EntityAccountFilterTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EntityAccountFilterTypeDef


def get_value() -> EntityAccountFilterTypeDef:
    return {
        "eventArn": ...,
    }


# EntityAccountFilterTypeDef definition

class EntityAccountFilterTypeDef(TypedDict):
    eventArn: str,
    awsAccountId: NotRequired[str],
    statusCodes: NotRequired[Sequence[EntityStatusCodeType]],  # (1)
```

1. See [:material-code-brackets: EntityStatusCodeType](./literals.md#entitystatuscodetype) 
## EventAccountFilterTypeDef

```python
# EventAccountFilterTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EventAccountFilterTypeDef


def get_value() -> EventAccountFilterTypeDef:
    return {
        "eventArn": ...,
    }


# EventAccountFilterTypeDef definition

class EventAccountFilterTypeDef(TypedDict):
    eventArn: str,
    awsAccountId: NotRequired[str],
```

## OrganizationAffectedEntitiesErrorItemTypeDef

```python
# OrganizationAffectedEntitiesErrorItemTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import OrganizationAffectedEntitiesErrorItemTypeDef


def get_value() -> OrganizationAffectedEntitiesErrorItemTypeDef:
    return {
        "awsAccountId": ...,
    }


# OrganizationAffectedEntitiesErrorItemTypeDef definition

class OrganizationAffectedEntitiesErrorItemTypeDef(TypedDict):
    awsAccountId: NotRequired[str],
    eventArn: NotRequired[str],
    errorName: NotRequired[str],
    errorMessage: NotRequired[str],
```

## DescribeEntityAggregatesForOrganizationRequestTypeDef

```python
# DescribeEntityAggregatesForOrganizationRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEntityAggregatesForOrganizationRequestTypeDef


def get_value() -> DescribeEntityAggregatesForOrganizationRequestTypeDef:
    return {
        "eventArns": ...,
    }


# DescribeEntityAggregatesForOrganizationRequestTypeDef definition

class DescribeEntityAggregatesForOrganizationRequestTypeDef(TypedDict):
    eventArns: Sequence[str],
    awsAccountIds: NotRequired[Sequence[str]],
```

## DescribeEntityAggregatesRequestTypeDef

```python
# DescribeEntityAggregatesRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEntityAggregatesRequestTypeDef


def get_value() -> DescribeEntityAggregatesRequestTypeDef:
    return {
        "eventArns": ...,
    }


# DescribeEntityAggregatesRequestTypeDef definition

class DescribeEntityAggregatesRequestTypeDef(TypedDict):
    eventArns: NotRequired[Sequence[str]],
```

## EntityAggregateTypeDef

```python
# EntityAggregateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EntityAggregateTypeDef


def get_value() -> EntityAggregateTypeDef:
    return {
        "eventArn": ...,
    }


# EntityAggregateTypeDef definition

class EntityAggregateTypeDef(TypedDict):
    eventArn: NotRequired[str],
    count: NotRequired[int],
    statuses: NotRequired[Dict[EntityStatusCodeType, int]],  # (1)
```

1. See [:material-code-brackets: EntityStatusCodeType](./literals.md#entitystatuscodetype) 
## EventAggregateTypeDef

```python
# EventAggregateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EventAggregateTypeDef


def get_value() -> EventAggregateTypeDef:
    return {
        "aggregateValue": ...,
    }


# EventAggregateTypeDef definition

class EventAggregateTypeDef(TypedDict):
    aggregateValue: NotRequired[str],
    count: NotRequired[int],
```

## OrganizationEventDetailsErrorItemTypeDef

```python
# OrganizationEventDetailsErrorItemTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import OrganizationEventDetailsErrorItemTypeDef


def get_value() -> OrganizationEventDetailsErrorItemTypeDef:
    return {
        "awsAccountId": ...,
    }


# OrganizationEventDetailsErrorItemTypeDef definition

class OrganizationEventDetailsErrorItemTypeDef(TypedDict):
    awsAccountId: NotRequired[str],
    eventArn: NotRequired[str],
    errorName: NotRequired[str],
    errorMessage: NotRequired[str],
```

## DescribeEventDetailsRequestTypeDef

```python
# DescribeEventDetailsRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventDetailsRequestTypeDef


def get_value() -> DescribeEventDetailsRequestTypeDef:
    return {
        "eventArns": ...,
    }


# DescribeEventDetailsRequestTypeDef definition

class DescribeEventDetailsRequestTypeDef(TypedDict):
    eventArns: Sequence[str],
    locale: NotRequired[str],
```

## EventDetailsErrorItemTypeDef

```python
# EventDetailsErrorItemTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EventDetailsErrorItemTypeDef


def get_value() -> EventDetailsErrorItemTypeDef:
    return {
        "eventArn": ...,
    }


# EventDetailsErrorItemTypeDef definition

class EventDetailsErrorItemTypeDef(TypedDict):
    eventArn: NotRequired[str],
    errorName: NotRequired[str],
    errorMessage: NotRequired[str],
```

## EventTypeFilterTypeDef

```python
# EventTypeFilterTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EventTypeFilterTypeDef


def get_value() -> EventTypeFilterTypeDef:
    return {
        "eventTypeCodes": ...,
    }


# EventTypeFilterTypeDef definition

class EventTypeFilterTypeDef(TypedDict):
    eventTypeCodes: NotRequired[Sequence[str]],
    services: NotRequired[Sequence[str]],
    eventTypeCategories: NotRequired[Sequence[EventTypeCategoryType]],  # (1)
```

1. See [:material-code-brackets: EventTypeCategoryType](./literals.md#eventtypecategorytype) 
## EventTypeTypeDef

```python
# EventTypeTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EventTypeTypeDef


def get_value() -> EventTypeTypeDef:
    return {
        "service": ...,
    }


# EventTypeTypeDef definition

class EventTypeTypeDef(TypedDict):
    service: NotRequired[str],
    code: NotRequired[str],
    category: NotRequired[EventTypeCategoryType],  # (1)
```

1. See [:material-code-brackets: EventTypeCategoryType](./literals.md#eventtypecategorytype) 
## OrganizationEventTypeDef

```python
# OrganizationEventTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import OrganizationEventTypeDef


def get_value() -> OrganizationEventTypeDef:
    return {
        "arn": ...,
    }


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
# EventTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EventTypeDef


def get_value() -> EventTypeDef:
    return {
        "arn": ...,
    }


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
# EventDescriptionTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EventDescriptionTypeDef


def get_value() -> EventDescriptionTypeDef:
    return {
        "latestDescription": ...,
    }


# EventDescriptionTypeDef definition

class EventDescriptionTypeDef(TypedDict):
    latestDescription: NotRequired[str],
```

## OrganizationEntityAggregateTypeDef

```python
# OrganizationEntityAggregateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import OrganizationEntityAggregateTypeDef


def get_value() -> OrganizationEntityAggregateTypeDef:
    return {
        "eventArn": ...,
    }


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
# DateTimeRangeTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DateTimeRangeTypeDef


def get_value() -> DateTimeRangeTypeDef:
    return {
        "from": ...,
    }


# DateTimeRangeTypeDef definition

class DateTimeRangeTypeDef(TypedDict):
    from: NotRequired[TimestampTypeDef],
    to: NotRequired[TimestampTypeDef],
```

## DescribeAffectedAccountsForOrganizationRequestPaginateTypeDef

```python
# DescribeAffectedAccountsForOrganizationRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeAffectedAccountsForOrganizationRequestPaginateTypeDef


def get_value() -> DescribeAffectedAccountsForOrganizationRequestPaginateTypeDef:
    return {
        "eventArn": ...,
    }


# DescribeAffectedAccountsForOrganizationRequestPaginateTypeDef definition

class DescribeAffectedAccountsForOrganizationRequestPaginateTypeDef(TypedDict):
    eventArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAffectedAccountsForOrganizationResponseTypeDef

```python
# DescribeAffectedAccountsForOrganizationResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeAffectedAccountsForOrganizationResponseTypeDef


def get_value() -> DescribeAffectedAccountsForOrganizationResponseTypeDef:
    return {
        "affectedAccounts": ...,
    }


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
# DescribeAffectedEntitiesResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeAffectedEntitiesResponseTypeDef


def get_value() -> DescribeAffectedEntitiesResponseTypeDef:
    return {
        "entities": ...,
    }


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
# DescribeHealthServiceStatusForOrganizationResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeHealthServiceStatusForOrganizationResponseTypeDef


def get_value() -> DescribeHealthServiceStatusForOrganizationResponseTypeDef:
    return {
        "healthServiceAccessStatusForOrganization": ...,
    }


# DescribeHealthServiceStatusForOrganizationResponseTypeDef definition

class DescribeHealthServiceStatusForOrganizationResponseTypeDef(TypedDict):
    healthServiceAccessStatusForOrganization: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAffectedEntitiesForOrganizationRequestPaginateTypeDef

```python
# DescribeAffectedEntitiesForOrganizationRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeAffectedEntitiesForOrganizationRequestPaginateTypeDef


def get_value() -> DescribeAffectedEntitiesForOrganizationRequestPaginateTypeDef:
    return {
        "organizationEntityFilters": ...,
    }


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
## DescribeAffectedEntitiesForOrganizationRequestTypeDef

```python
# DescribeAffectedEntitiesForOrganizationRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeAffectedEntitiesForOrganizationRequestTypeDef


def get_value() -> DescribeAffectedEntitiesForOrganizationRequestTypeDef:
    return {
        "organizationEntityFilters": ...,
    }


# DescribeAffectedEntitiesForOrganizationRequestTypeDef definition

class DescribeAffectedEntitiesForOrganizationRequestTypeDef(TypedDict):
    organizationEntityFilters: NotRequired[Sequence[EventAccountFilterTypeDef]],  # (1)
    locale: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    organizationEntityAccountFilters: NotRequired[Sequence[EntityAccountFilterTypeDef]],  # (2)
```

1. See [:material-code-braces: EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef) 
2. See [:material-code-braces: EntityAccountFilterTypeDef](./type_defs.md#entityaccountfiltertypedef) 
## DescribeEventDetailsForOrganizationRequestTypeDef

```python
# DescribeEventDetailsForOrganizationRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventDetailsForOrganizationRequestTypeDef


def get_value() -> DescribeEventDetailsForOrganizationRequestTypeDef:
    return {
        "organizationEventDetailFilters": ...,
    }


# DescribeEventDetailsForOrganizationRequestTypeDef definition

class DescribeEventDetailsForOrganizationRequestTypeDef(TypedDict):
    organizationEventDetailFilters: Sequence[EventAccountFilterTypeDef],  # (1)
    locale: NotRequired[str],
```

1. See [:material-code-braces: EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef) 
## DescribeAffectedEntitiesForOrganizationResponseTypeDef

```python
# DescribeAffectedEntitiesForOrganizationResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeAffectedEntitiesForOrganizationResponseTypeDef


def get_value() -> DescribeAffectedEntitiesForOrganizationResponseTypeDef:
    return {
        "entities": ...,
    }


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
# DescribeEntityAggregatesResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEntityAggregatesResponseTypeDef


def get_value() -> DescribeEntityAggregatesResponseTypeDef:
    return {
        "entityAggregates": ...,
    }


# DescribeEntityAggregatesResponseTypeDef definition

class DescribeEntityAggregatesResponseTypeDef(TypedDict):
    entityAggregates: List[EntityAggregateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntityAggregateTypeDef](./type_defs.md#entityaggregatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventAggregatesResponseTypeDef

```python
# DescribeEventAggregatesResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventAggregatesResponseTypeDef


def get_value() -> DescribeEventAggregatesResponseTypeDef:
    return {
        "eventAggregates": ...,
    }


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
# DescribeEventTypesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventTypesRequestPaginateTypeDef


def get_value() -> DescribeEventTypesRequestPaginateTypeDef:
    return {
        "filter": ...,
    }


# DescribeEventTypesRequestPaginateTypeDef definition

class DescribeEventTypesRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[EventTypeFilterTypeDef],  # (1)
    locale: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EventTypeFilterTypeDef](./type_defs.md#eventtypefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventTypesRequestTypeDef

```python
# DescribeEventTypesRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventTypesRequestTypeDef


def get_value() -> DescribeEventTypesRequestTypeDef:
    return {
        "filter": ...,
    }


# DescribeEventTypesRequestTypeDef definition

class DescribeEventTypesRequestTypeDef(TypedDict):
    filter: NotRequired[EventTypeFilterTypeDef],  # (1)
    locale: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: EventTypeFilterTypeDef](./type_defs.md#eventtypefiltertypedef) 
## DescribeEventTypesResponseTypeDef

```python
# DescribeEventTypesResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventTypesResponseTypeDef


def get_value() -> DescribeEventTypesResponseTypeDef:
    return {
        "eventTypes": ...,
    }


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
# DescribeEventsForOrganizationResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventsForOrganizationResponseTypeDef


def get_value() -> DescribeEventsForOrganizationResponseTypeDef:
    return {
        "events": ...,
    }


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
# DescribeEventsResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventsResponseTypeDef


def get_value() -> DescribeEventsResponseTypeDef:
    return {
        "events": ...,
    }


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
# EventDetailsTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EventDetailsTypeDef


def get_value() -> EventDetailsTypeDef:
    return {
        "event": ...,
    }


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
# OrganizationEventDetailsTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import OrganizationEventDetailsTypeDef


def get_value() -> OrganizationEventDetailsTypeDef:
    return {
        "awsAccountId": ...,
    }


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
# DescribeEntityAggregatesForOrganizationResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEntityAggregatesForOrganizationResponseTypeDef


def get_value() -> DescribeEntityAggregatesForOrganizationResponseTypeDef:
    return {
        "organizationEntityAggregates": ...,
    }


# DescribeEntityAggregatesForOrganizationResponseTypeDef definition

class DescribeEntityAggregatesForOrganizationResponseTypeDef(TypedDict):
    organizationEntityAggregates: List[OrganizationEntityAggregateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationEntityAggregateTypeDef](./type_defs.md#organizationentityaggregatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EntityFilterTypeDef

```python
# EntityFilterTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EntityFilterTypeDef


def get_value() -> EntityFilterTypeDef:
    return {
        "eventArns": ...,
    }


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
# EventFilterTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import EventFilterTypeDef


def get_value() -> EventFilterTypeDef:
    return {
        "eventArns": ...,
    }


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
# OrganizationEventFilterTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import OrganizationEventFilterTypeDef


def get_value() -> OrganizationEventFilterTypeDef:
    return {
        "eventTypeCodes": ...,
    }


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
# DescribeEventDetailsResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventDetailsResponseTypeDef


def get_value() -> DescribeEventDetailsResponseTypeDef:
    return {
        "successfulSet": ...,
    }


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
# DescribeEventDetailsForOrganizationResponseTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventDetailsForOrganizationResponseTypeDef


def get_value() -> DescribeEventDetailsForOrganizationResponseTypeDef:
    return {
        "successfulSet": ...,
    }


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
# DescribeAffectedEntitiesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeAffectedEntitiesRequestPaginateTypeDef


def get_value() -> DescribeAffectedEntitiesRequestPaginateTypeDef:
    return {
        "filter": ...,
    }


# DescribeAffectedEntitiesRequestPaginateTypeDef definition

class DescribeAffectedEntitiesRequestPaginateTypeDef(TypedDict):
    filter: EntityFilterTypeDef,  # (1)
    locale: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EntityFilterTypeDef](./type_defs.md#entityfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAffectedEntitiesRequestTypeDef

```python
# DescribeAffectedEntitiesRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeAffectedEntitiesRequestTypeDef


def get_value() -> DescribeAffectedEntitiesRequestTypeDef:
    return {
        "filter": ...,
    }


# DescribeAffectedEntitiesRequestTypeDef definition

class DescribeAffectedEntitiesRequestTypeDef(TypedDict):
    filter: EntityFilterTypeDef,  # (1)
    locale: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: EntityFilterTypeDef](./type_defs.md#entityfiltertypedef) 
## DescribeEventAggregatesRequestPaginateTypeDef

```python
# DescribeEventAggregatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventAggregatesRequestPaginateTypeDef


def get_value() -> DescribeEventAggregatesRequestPaginateTypeDef:
    return {
        "aggregateField": ...,
    }


# DescribeEventAggregatesRequestPaginateTypeDef definition

class DescribeEventAggregatesRequestPaginateTypeDef(TypedDict):
    aggregateField: EventAggregateFieldType,  # (1)
    filter: NotRequired[EventFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EventAggregateFieldType](./literals.md#eventaggregatefieldtype) 
2. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventAggregatesRequestTypeDef

```python
# DescribeEventAggregatesRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventAggregatesRequestTypeDef


def get_value() -> DescribeEventAggregatesRequestTypeDef:
    return {
        "aggregateField": ...,
    }


# DescribeEventAggregatesRequestTypeDef definition

class DescribeEventAggregatesRequestTypeDef(TypedDict):
    aggregateField: EventAggregateFieldType,  # (1)
    filter: NotRequired[EventFilterTypeDef],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: EventAggregateFieldType](./literals.md#eventaggregatefieldtype) 
2. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
## DescribeEventsRequestPaginateTypeDef

```python
# DescribeEventsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventsRequestPaginateTypeDef


def get_value() -> DescribeEventsRequestPaginateTypeDef:
    return {
        "filter": ...,
    }


# DescribeEventsRequestPaginateTypeDef definition

class DescribeEventsRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[EventFilterTypeDef],  # (1)
    locale: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsRequestTypeDef

```python
# DescribeEventsRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventsRequestTypeDef


def get_value() -> DescribeEventsRequestTypeDef:
    return {
        "filter": ...,
    }


# DescribeEventsRequestTypeDef definition

class DescribeEventsRequestTypeDef(TypedDict):
    filter: NotRequired[EventFilterTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    locale: NotRequired[str],
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
## DescribeEventsForOrganizationRequestPaginateTypeDef

```python
# DescribeEventsForOrganizationRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventsForOrganizationRequestPaginateTypeDef


def get_value() -> DescribeEventsForOrganizationRequestPaginateTypeDef:
    return {
        "filter": ...,
    }


# DescribeEventsForOrganizationRequestPaginateTypeDef definition

class DescribeEventsForOrganizationRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[OrganizationEventFilterTypeDef],  # (1)
    locale: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OrganizationEventFilterTypeDef](./type_defs.md#organizationeventfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsForOrganizationRequestTypeDef

```python
# DescribeEventsForOrganizationRequestTypeDef TypedDict usage example

from types_aiobotocore_health.type_defs import DescribeEventsForOrganizationRequestTypeDef


def get_value() -> DescribeEventsForOrganizationRequestTypeDef:
    return {
        "filter": ...,
    }


# DescribeEventsForOrganizationRequestTypeDef definition

class DescribeEventsForOrganizationRequestTypeDef(TypedDict):
    filter: NotRequired[OrganizationEventFilterTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    locale: NotRequired[str],
```

1. See [:material-code-braces: OrganizationEventFilterTypeDef](./type_defs.md#organizationeventfiltertypedef) 
