# Type definitions

> [Index](../README.md) > [IoTDataPlane](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#iotdataplane)
    type annotations stubs module [types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## DeleteThingShadowRequestRequestTypeDef

```python
# DeleteThingShadowRequestRequestTypeDef definition

class DeleteThingShadowRequestRequestTypeDef(TypedDict):
    thingName: str,
    shadowName: NotRequired[str],
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

## GetRetainedMessageRequestRequestTypeDef

```python
# GetRetainedMessageRequestRequestTypeDef definition

class GetRetainedMessageRequestRequestTypeDef(TypedDict):
    topic: str,
```

## GetThingShadowRequestRequestTypeDef

```python
# GetThingShadowRequestRequestTypeDef definition

class GetThingShadowRequestRequestTypeDef(TypedDict):
    thingName: str,
    shadowName: NotRequired[str],
```

## ListNamedShadowsForThingRequestRequestTypeDef

```python
# ListNamedShadowsForThingRequestRequestTypeDef definition

class ListNamedShadowsForThingRequestRequestTypeDef(TypedDict):
    thingName: str,
    nextToken: NotRequired[str],
    pageSize: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListRetainedMessagesRequestRequestTypeDef

```python
# ListRetainedMessagesRequestRequestTypeDef definition

class ListRetainedMessagesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## RetainedMessageSummaryTypeDef

```python
# RetainedMessageSummaryTypeDef definition

class RetainedMessageSummaryTypeDef(TypedDict):
    topic: NotRequired[str],
    payloadSize: NotRequired[int],
    qos: NotRequired[int],
    lastModifiedTime: NotRequired[int],
```

## PublishRequestRequestTypeDef

```python
# PublishRequestRequestTypeDef definition

class PublishRequestRequestTypeDef(TypedDict):
    topic: str,
    qos: NotRequired[int],
    retain: NotRequired[bool],
    payload: NotRequired[BlobTypeDef],
    userProperties: NotRequired[str],
    payloadFormatIndicator: NotRequired[PayloadFormatIndicatorType],  # (1)
    contentType: NotRequired[str],
    responseTopic: NotRequired[str],
    correlationData: NotRequired[str],
    messageExpiry: NotRequired[int],
```

1. See [:material-code-brackets: PayloadFormatIndicatorType](./literals.md#payloadformatindicatortype) 
## UpdateThingShadowRequestRequestTypeDef

```python
# UpdateThingShadowRequestRequestTypeDef definition

class UpdateThingShadowRequestRequestTypeDef(TypedDict):
    thingName: str,
    payload: BlobTypeDef,
    shadowName: NotRequired[str],
```

## DeleteThingShadowResponseTypeDef

```python
# DeleteThingShadowResponseTypeDef definition

class DeleteThingShadowResponseTypeDef(TypedDict):
    payload: StreamingBody,
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
## GetRetainedMessageResponseTypeDef

```python
# GetRetainedMessageResponseTypeDef definition

class GetRetainedMessageResponseTypeDef(TypedDict):
    topic: str,
    payload: bytes,
    qos: int,
    lastModifiedTime: int,
    userProperties: bytes,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetThingShadowResponseTypeDef

```python
# GetThingShadowResponseTypeDef definition

class GetThingShadowResponseTypeDef(TypedDict):
    payload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNamedShadowsForThingResponseTypeDef

```python
# ListNamedShadowsForThingResponseTypeDef definition

class ListNamedShadowsForThingResponseTypeDef(TypedDict):
    results: List[str],
    timestamp: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateThingShadowResponseTypeDef

```python
# UpdateThingShadowResponseTypeDef definition

class UpdateThingShadowResponseTypeDef(TypedDict):
    payload: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRetainedMessagesRequestPaginateTypeDef

```python
# ListRetainedMessagesRequestPaginateTypeDef definition

class ListRetainedMessagesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRetainedMessagesResponseTypeDef

```python
# ListRetainedMessagesResponseTypeDef definition

class ListRetainedMessagesResponseTypeDef(TypedDict):
    retainedTopics: List[RetainedMessageSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RetainedMessageSummaryTypeDef](./type_defs.md#retainedmessagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
