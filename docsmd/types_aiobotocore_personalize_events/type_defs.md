# Type definitions

> [Index](../README.md) > [PersonalizeEvents](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PersonalizeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
    type annotations stubs module [types-aiobotocore-personalize-events](https://pypi.org/project/types-aiobotocore-personalize-events/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
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

## MetricAttributionTypeDef

```python
# MetricAttributionTypeDef definition

class MetricAttributionTypeDef(TypedDict):
    eventAttributionSource: str,
```

## ItemTypeDef

```python
# ItemTypeDef definition

class ItemTypeDef(TypedDict):
    itemId: str,
    properties: NotRequired[str],
```

## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    userId: str,
    properties: NotRequired[str],
```

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    eventType: str,
    sentAt: Union[datetime, str],
    eventId: NotRequired[str],
    eventValue: NotRequired[float],
    itemId: NotRequired[str],
    properties: NotRequired[str],
    recommendationId: NotRequired[str],
    impression: NotRequired[Sequence[str]],
    metricAttribution: NotRequired[MetricAttributionTypeDef],  # (1)
```

1. See [:material-code-braces: MetricAttributionTypeDef](./type_defs.md#metricattributiontypedef) 
## PutItemsRequestRequestTypeDef

```python
# PutItemsRequestRequestTypeDef definition

class PutItemsRequestRequestTypeDef(TypedDict):
    datasetArn: str,
    items: Sequence[ItemTypeDef],  # (1)
```

1. See [:material-code-braces: ItemTypeDef](./type_defs.md#itemtypedef) 
## PutUsersRequestRequestTypeDef

```python
# PutUsersRequestRequestTypeDef definition

class PutUsersRequestRequestTypeDef(TypedDict):
    datasetArn: str,
    users: Sequence[UserTypeDef],  # (1)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
## PutEventsRequestRequestTypeDef

```python
# PutEventsRequestRequestTypeDef definition

class PutEventsRequestRequestTypeDef(TypedDict):
    trackingId: str,
    sessionId: str,
    eventList: Sequence[EventTypeDef],  # (1)
    userId: NotRequired[str],
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
