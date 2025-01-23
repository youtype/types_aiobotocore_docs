# Type definitions

> [Index](../README.md) > [Ivschat](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Ivschat](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
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
    capabilities: NotRequired[Sequence[ChatTokenCapabilityType]],  # (1)
    sessionDurationInMinutes: NotRequired[int],
    attributes: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ChatTokenCapabilityType](./literals.md#chattokencapabilitytype) 
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

## MessageReviewHandlerTypeDef

```python
# MessageReviewHandlerTypeDef definition

class MessageReviewHandlerTypeDef(TypedDict):
    uri: NotRequired[str],
    fallbackResult: NotRequired[FallbackResultType],  # (1)
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
    roomIdentifier: str,
    id: str,
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
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListRoomsRequestRequestTypeDef

```python
# ListRoomsRequestRequestTypeDef definition

class ListRoomsRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    messageReviewHandlerUri: NotRequired[str],
    loggingConfigurationIdentifier: NotRequired[str],
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
    roomIdentifier: str,
    eventName: str,
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
    token: str,
    tokenExpirationTime: datetime,
    sessionExpirationTime: datetime,
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
    name: NotRequired[str],
    maximumMessageRatePerSecond: NotRequired[int],
    maximumMessageLength: NotRequired[int],
    messageReviewHandler: NotRequired[MessageReviewHandlerTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
    loggingConfigurationIdentifiers: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
## CreateRoomResponseTypeDef

```python
# CreateRoomResponseTypeDef definition

class CreateRoomResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    maximumMessageRatePerSecond: int,
    maximumMessageLength: int,
    messageReviewHandler: MessageReviewHandlerTypeDef,  # (1)
    tags: Dict[str, str],
    loggingConfigurationIdentifiers: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRoomResponseTypeDef

```python
# GetRoomResponseTypeDef definition

class GetRoomResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    maximumMessageRatePerSecond: int,
    maximumMessageLength: int,
    messageReviewHandler: MessageReviewHandlerTypeDef,  # (1)
    tags: Dict[str, str],
    loggingConfigurationIdentifiers: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RoomSummaryTypeDef

```python
# RoomSummaryTypeDef definition

class RoomSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    id: NotRequired[str],
    name: NotRequired[str],
    messageReviewHandler: NotRequired[MessageReviewHandlerTypeDef],  # (1)
    createTime: NotRequired[datetime],
    updateTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    loggingConfigurationIdentifiers: NotRequired[List[str]],
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
## UpdateRoomRequestRequestTypeDef

```python
# UpdateRoomRequestRequestTypeDef definition

class UpdateRoomRequestRequestTypeDef(TypedDict):
    identifier: str,
    name: NotRequired[str],
    maximumMessageRatePerSecond: NotRequired[int],
    maximumMessageLength: NotRequired[int],
    messageReviewHandler: NotRequired[MessageReviewHandlerTypeDef],  # (1)
    loggingConfigurationIdentifiers: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
## UpdateRoomResponseTypeDef

```python
# UpdateRoomResponseTypeDef definition

class UpdateRoomResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    maximumMessageRatePerSecond: int,
    maximumMessageLength: int,
    messageReviewHandler: MessageReviewHandlerTypeDef,  # (1)
    tags: Dict[str, str],
    loggingConfigurationIdentifiers: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageReviewHandlerTypeDef](./type_defs.md#messagereviewhandlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DestinationConfigurationTypeDef

```python
# DestinationConfigurationTypeDef definition

class DestinationConfigurationTypeDef(TypedDict):
    s3: NotRequired[S3DestinationConfigurationTypeDef],  # (1)
    cloudWatchLogs: NotRequired[CloudWatchLogsDestinationConfigurationTypeDef],  # (2)
    firehose: NotRequired[FirehoseDestinationConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
2. See [:material-code-braces: CloudWatchLogsDestinationConfigurationTypeDef](./type_defs.md#cloudwatchlogsdestinationconfigurationtypedef) 
3. See [:material-code-braces: FirehoseDestinationConfigurationTypeDef](./type_defs.md#firehosedestinationconfigurationtypedef) 
## ListRoomsResponseTypeDef

```python
# ListRoomsResponseTypeDef definition

class ListRoomsResponseTypeDef(TypedDict):
    rooms: List[RoomSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
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
    id: str,
    createTime: datetime,
    updateTime: datetime,
    name: str,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    state: CreateLoggingConfigurationStateType,  # (2)
    tags: Dict[str, str],
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
    id: str,
    createTime: datetime,
    updateTime: datetime,
    name: str,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    state: LoggingConfigurationStateType,  # (2)
    tags: Dict[str, str],
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
    id: NotRequired[str],
    createTime: NotRequired[datetime],
    updateTime: NotRequired[datetime],
    name: NotRequired[str],
    destinationConfiguration: NotRequired[DestinationConfigurationTypeDef],  # (1)
    state: NotRequired[LoggingConfigurationStateType],  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
2. See [:material-code-brackets: LoggingConfigurationStateType](./literals.md#loggingconfigurationstatetype) 
## UpdateLoggingConfigurationRequestRequestTypeDef

```python
# UpdateLoggingConfigurationRequestRequestTypeDef definition

class UpdateLoggingConfigurationRequestRequestTypeDef(TypedDict):
    identifier: str,
    name: NotRequired[str],
    destinationConfiguration: NotRequired[DestinationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) 
## UpdateLoggingConfigurationResponseTypeDef

```python
# UpdateLoggingConfigurationResponseTypeDef definition

class UpdateLoggingConfigurationResponseTypeDef(TypedDict):
    arn: str,
    id: str,
    createTime: datetime,
    updateTime: datetime,
    name: str,
    destinationConfiguration: DestinationConfigurationTypeDef,  # (1)
    state: UpdateLoggingConfigurationStateType,  # (2)
    tags: Dict[str, str],
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LoggingConfigurationSummaryTypeDef](./type_defs.md#loggingconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
