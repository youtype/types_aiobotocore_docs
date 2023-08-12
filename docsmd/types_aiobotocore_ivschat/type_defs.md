# Type definitions

> [Index](../README.md) > [ivschat](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ivschat](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
    type annotations stubs module [types-aiobotocore-ivschat](https://pypi.org/project/types-aiobotocore-ivschat/).



## CloudWatchLogsDestinationConfigurationTypeDef

```python
# CloudWatchLogsDestinationConfigurationTypeDef definition

class CloudWatchLogsDestinationConfigurationTypeDef(TypedDict):
    logGroupName: str,
```

## CreateChatTokenRequestRequestTypeDef

```python
# CreateChatTokenRequestRequestTypeDef definition

class CreateChatTokenRequestRequestTypeDef(TypedDict):
    roomIdentifier: str,
    userId: str,
    attributes: NotRequired[Mapping[str, str]],
    capabilities: NotRequired[Sequence[ChatTokenCapabilityType]],  # (1)
    sessionDurationInMinutes: NotRequired[int],
```

1. See [:material-code-brackets: ChatTokenCapabilityType](./literals.md#chattokencapabilitytype) 
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

## MessageReviewHandlerTypeDef

```python
# MessageReviewHandlerTypeDef definition

class MessageReviewHandlerTypeDef(TypedDict):
    fallbackResult: NotRequired[FallbackResultType],  # (1)
    uri: NotRequired[str],
```

1. See [:material-code-brackets: FallbackResultType](./literals.md#fallbackresulttype) 
## DeleteLoggingConfigurationRequestRequestTypeDef

```python
# DeleteLoggingConfigurationRequestRequestTypeDef definition

class DeleteLoggingConfigurationRequestRequestTypeDef(TypedDict):
    identifier: str,
```

## DeleteMessageRequestRequestTypeDef

```python
# DeleteMessageRequestRequestTypeDef definition

class DeleteMessageRequestRequestTypeDef(TypedDict):
    id: str,
    roomIdentifier: str,
    reason: NotRequired[str],
```

## DeleteRoomRequestRequestTypeDef

```python
# DeleteRoomRequestRequestTypeDef definition

class DeleteRoomRequestRequestTypeDef(TypedDict):
    identifier: str,
```

## FirehoseDestinationConfigurationTypeDef

```python
# FirehoseDestinationConfigurationTypeDef definition

class FirehoseDestinationConfigurationTypeDef(TypedDict):
    deliveryStreamName: str,
```

## S3DestinationConfigurationTypeDef

```python
# S3DestinationConfigurationTypeDef definition

class S3DestinationConfigurationTypeDef(TypedDict):
    bucketName: str,
```

## DisconnectUserRequestRequestTypeDef

```python
# DisconnectUserRequestRequestTypeDef definition

class DisconnectUserRequestRequestTypeDef(TypedDict):
    roomIdentifier: str,
    userId: str,
    reason: NotRequired[str],
```

## GetLoggingConfigurationRequestRequestTypeDef

```python
# GetLoggingConfigurationRequestRequestTypeDef definition

class GetLoggingConfigurationRequestRequestTypeDef(TypedDict):
    identifier: str,
```

## GetRoomRequestRequestTypeDef

```python
# GetRoomRequestRequestTypeDef definition

class GetRoomRequestRequestTypeDef(TypedDict):
    identifier: str,
```

## ListLoggingConfigurationsRequestRequestTypeDef

```python
# ListLoggingConfigurationsRequestRequestTypeDef definition

class ListLoggingConfigurationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListRoomsRequestRequestTypeDef

```python
# ListRoomsRequestRequestTypeDef definition

class ListRoomsRequestRequestTypeDef(TypedDict):
    loggingConfigurationIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    messageReviewHandlerUri: NotRequired[str],
    name: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## SendEventRequestRequestTypeDef

```python
# SendEventRequestRequestTypeDef definition

class SendEventRequestRequestTypeDef(TypedDict):
    eventName: str,
    roomIdentifier: str,
    attributes: NotRequired[Mapping[str, str]],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## CreateChatTokenResponseTypeDef

```python
# CreateChatTokenResponseTypeDef definition

class CreateChatTokenResponseTypeDef(TypedDict):
    sessionExpirationTime: datetime,
    token: str,
    tokenExpirationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMessageResponseTypeDef

```python
# DeleteMessageResponseTypeDef definition

class DeleteMessageResponseTypeDef(TypedDict):
    id: str,
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
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendEventResponseTypeDef

```python
# SendEventResponseTypeDef definition

class SendEventResponseTypeDef(TypedDict):
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRoomRequestRequestTypeDef

```python
# CreateRoomRequestRequestTypeDef definition

class CreateRoomRequestRequestTypeDef(TypedDict):
    loggingConfigurationIdentifiers: NotRequired[Sequence[str]],
    maximumMessageLength: NotRequired[int],
    maximumMessageRatePerSecond: NotRequired[int],
    messageReviewHandler: NotRequired[MessageReviewHandlerTypeDef],  # (1)
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
## CreateRoomResponseTypeDef

```python
# CreateRoomResponseTypeDef definition

class CreateRoomResponseTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    loggingConfigurationIdentifiers: List[str],
    maximumMessageLength: int,
    maximumMessageRatePerSecond: int,
    messageReviewHandler: MessageReviewHandlerTypeDef,  # (1)
    name: str,
    tags: Dict[str, str],
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRoomResponseTypeDef

```python
# GetRoomResponseTypeDef definition

class GetRoomResponseTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    loggingConfigurationIdentifiers: List[str],
    maximumMessageLength: int,
    maximumMessageRatePerSecond: int,
    messageReviewHandler: MessageReviewHandlerTypeDef,  # (1)
    name: str,
    tags: Dict[str, str],
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RoomSummaryTypeDef

```python
# RoomSummaryTypeDef definition

class RoomSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createTime: NotRequired[datetime],
    id: NotRequired[str],
    loggingConfigurationIdentifiers: NotRequired[List[str]],
    messageReviewHandler: NotRequired[MessageReviewHandlerTypeDef],  # (1)
    name: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    updateTime: NotRequired[datetime],
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
## UpdateRoomRequestRequestTypeDef

```python
# UpdateRoomRequestRequestTypeDef definition

class UpdateRoomRequestRequestTypeDef(TypedDict):
    identifier: str,
    loggingConfigurationIdentifiers: NotRequired[Sequence[str]],
    maximumMessageLength: NotRequired[int],
    maximumMessageRatePerSecond: NotRequired[int],
    messageReviewHandler: NotRequired[MessageReviewHandlerTypeDef],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
## UpdateRoomResponseTypeDef

```python
# UpdateRoomResponseTypeDef definition

class UpdateRoomResponseTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    loggingConfigurationIdentifiers: List[str],
    maximumMessageLength: int,
    maximumMessageRatePerSecond: int,
    messageReviewHandler: MessageReviewHandlerTypeDef,  # (1)
    name: str,
    tags: Dict[str, str],
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationConfigurationTypeDef

```python
# DestinationConfigurationTypeDef definition

class DestinationConfigurationTypeDef(TypedDict):
    cloudWatchLogs: NotRequired[CloudWatchLogsDestinationConfigurationTypeDef],  # (1)
    firehose: NotRequired[FirehoseDestinationConfigurationTypeDef],  # (2)
    s3: NotRequired[S3DestinationConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: CloudWatchLogsDestinationConfigurationTypeDef](./type_defs.md#cloudwatchlogsdestinationconfigurationtypedef) 
2. See [:material-code-braces: FirehoseDestinationConfigurationTypeDef](./type_defs.md#firehosedestinationconfigurationtypedef) 
3. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
## ListRoomsResponseTypeDef

```python
# ListRoomsResponseTypeDef definition

class ListRoomsResponseTypeDef(TypedDict):
    nextToken: str,
    rooms: List[RoomSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RoomSummaryTypeDef](./type_defs.md#roomsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLoggingConfigurationRequestRequestTypeDef

```python
# CreateLoggingConfigurationRequestRequestTypeDef definition

class CreateLoggingConfigurationRequestRequestTypeDef(TypedDict):
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    name: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
## CreateLoggingConfigurationResponseTypeDef

```python
# CreateLoggingConfigurationResponseTypeDef definition

class CreateLoggingConfigurationResponseTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    id: str,
    name: str,
    state: CreateLoggingConfigurationStateType,  # (2)
    tags: Dict[str, str],
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-brackets: CreateLoggingConfigurationStateType](./literals.md#createloggingconfigurationstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLoggingConfigurationResponseTypeDef

```python
# GetLoggingConfigurationResponseTypeDef definition

class GetLoggingConfigurationResponseTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    id: str,
    name: str,
    state: LoggingConfigurationStateType,  # (2)
    tags: Dict[str, str],
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-brackets: LoggingConfigurationStateType](./literals.md#loggingconfigurationstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingConfigurationSummaryTypeDef

```python
# LoggingConfigurationSummaryTypeDef definition

class LoggingConfigurationSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createTime: NotRequired[datetime],
    destinationConfiguration: NotRequired[DestinationConfigurationTypeDef],  # (1)
    id: NotRequired[str],
    name: NotRequired[str],
    state: NotRequired[LoggingConfigurationStateType],  # (2)
    tags: NotRequired[Dict[str, str]],
    updateTime: NotRequired[datetime],
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-brackets: LoggingConfigurationStateType](./literals.md#loggingconfigurationstatetype) 
## UpdateLoggingConfigurationRequestRequestTypeDef

```python
# UpdateLoggingConfigurationRequestRequestTypeDef definition

class UpdateLoggingConfigurationRequestRequestTypeDef(TypedDict):
    identifier: str,
    destinationConfiguration: NotRequired[DestinationConfigurationTypeDef],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
## UpdateLoggingConfigurationResponseTypeDef

```python
# UpdateLoggingConfigurationResponseTypeDef definition

class UpdateLoggingConfigurationResponseTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    id: str,
    name: str,
    state: UpdateLoggingConfigurationStateType,  # (2)
    tags: Dict[str, str],
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-brackets: UpdateLoggingConfigurationStateType](./literals.md#updateloggingconfigurationstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLoggingConfigurationsResponseTypeDef

```python
# ListLoggingConfigurationsResponseTypeDef definition

class ListLoggingConfigurationsResponseTypeDef(TypedDict):
    loggingConfigurations: List[LoggingConfigurationSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationSummaryTypeDef](./type_defs.md#loggingconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
