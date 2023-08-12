# Type definitions

> [Index](../README.md) > [ConnectParticipant](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ConnectParticipant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
    type annotations stubs module [types-aiobotocore-connectparticipant](https://pypi.org/project/types-aiobotocore-connectparticipant/).



## AttachmentItemTypeDef

```python
# AttachmentItemTypeDef definition

class AttachmentItemTypeDef(TypedDict):
    ContentType: NotRequired[str],
    AttachmentId: NotRequired[str],
    AttachmentName: NotRequired[str],
    Status: NotRequired[ArtifactStatusType],  # (1)
```

1. See [:material-code-brackets: ArtifactStatusType](./literals.md#artifactstatustype) 
## CompleteAttachmentUploadRequestRequestTypeDef

```python
# CompleteAttachmentUploadRequestRequestTypeDef definition

class CompleteAttachmentUploadRequestRequestTypeDef(TypedDict):
    AttachmentIds: Sequence[str],
    ClientToken: str,
    ConnectionToken: str,
```

## ConnectionCredentialsTypeDef

```python
# ConnectionCredentialsTypeDef definition

class ConnectionCredentialsTypeDef(TypedDict):
    ConnectionToken: NotRequired[str],
    Expiry: NotRequired[str],
```

## CreateParticipantConnectionRequestRequestTypeDef

```python
# CreateParticipantConnectionRequestRequestTypeDef definition

class CreateParticipantConnectionRequestRequestTypeDef(TypedDict):
    ParticipantToken: str,
    Type: NotRequired[Sequence[ConnectionTypeType]],  # (1)
    ConnectParticipant: NotRequired[bool],
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
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

## WebsocketTypeDef

```python
# WebsocketTypeDef definition

class WebsocketTypeDef(TypedDict):
    Url: NotRequired[str],
    ConnectionExpiry: NotRequired[str],
```

## DisconnectParticipantRequestRequestTypeDef

```python
# DisconnectParticipantRequestRequestTypeDef definition

class DisconnectParticipantRequestRequestTypeDef(TypedDict):
    ConnectionToken: str,
    ClientToken: NotRequired[str],
```

## GetAttachmentRequestRequestTypeDef

```python
# GetAttachmentRequestRequestTypeDef definition

class GetAttachmentRequestRequestTypeDef(TypedDict):
    AttachmentId: str,
    ConnectionToken: str,
```

## StartPositionTypeDef

```python
# StartPositionTypeDef definition

class StartPositionTypeDef(TypedDict):
    Id: NotRequired[str],
    AbsoluteTime: NotRequired[str],
    MostRecent: NotRequired[int],
```

## ReceiptTypeDef

```python
# ReceiptTypeDef definition

class ReceiptTypeDef(TypedDict):
    DeliveredTimestamp: NotRequired[str],
    ReadTimestamp: NotRequired[str],
    RecipientParticipantId: NotRequired[str],
```

## SendEventRequestRequestTypeDef

```python
# SendEventRequestRequestTypeDef definition

class SendEventRequestRequestTypeDef(TypedDict):
    ContentType: str,
    ConnectionToken: str,
    Content: NotRequired[str],
    ClientToken: NotRequired[str],
```

## SendMessageRequestRequestTypeDef

```python
# SendMessageRequestRequestTypeDef definition

class SendMessageRequestRequestTypeDef(TypedDict):
    ContentType: str,
    Content: str,
    ConnectionToken: str,
    ClientToken: NotRequired[str],
```

## StartAttachmentUploadRequestRequestTypeDef

```python
# StartAttachmentUploadRequestRequestTypeDef definition

class StartAttachmentUploadRequestRequestTypeDef(TypedDict):
    ContentType: str,
    AttachmentSizeInBytes: int,
    AttachmentName: str,
    ClientToken: str,
    ConnectionToken: str,
```

## UploadMetadataTypeDef

```python
# UploadMetadataTypeDef definition

class UploadMetadataTypeDef(TypedDict):
    Url: NotRequired[str],
    UrlExpiry: NotRequired[str],
    HeadersToInclude: NotRequired[Dict[str, str]],
```

## GetAttachmentResponseTypeDef

```python
# GetAttachmentResponseTypeDef definition

class GetAttachmentResponseTypeDef(TypedDict):
    Url: str,
    UrlExpiry: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendEventResponseTypeDef

```python
# SendEventResponseTypeDef definition

class SendEventResponseTypeDef(TypedDict):
    Id: str,
    AbsoluteTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendMessageResponseTypeDef

```python
# SendMessageResponseTypeDef definition

class SendMessageResponseTypeDef(TypedDict):
    Id: str,
    AbsoluteTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateParticipantConnectionResponseTypeDef

```python
# CreateParticipantConnectionResponseTypeDef definition

class CreateParticipantConnectionResponseTypeDef(TypedDict):
    Websocket: WebsocketTypeDef,  # (1)
    ConnectionCredentials: ConnectionCredentialsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: WebsocketTypeDef](./type_defs.md#websockettypedef) 
2. See [:material-code-braces: ConnectionCredentialsTypeDef](./type_defs.md#connectioncredentialstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTranscriptRequestRequestTypeDef

```python
# GetTranscriptRequestRequestTypeDef definition

class GetTranscriptRequestRequestTypeDef(TypedDict):
    ConnectionToken: str,
    ContactId: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ScanDirection: NotRequired[ScanDirectionType],  # (1)
    SortOrder: NotRequired[SortKeyType],  # (2)
    StartPosition: NotRequired[StartPositionTypeDef],  # (3)
```

1. See [:material-code-brackets: ScanDirectionType](./literals.md#scandirectiontype) 
2. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
3. See [:material-code-braces: StartPositionTypeDef](./type_defs.md#startpositiontypedef) 
## MessageMetadataTypeDef

```python
# MessageMetadataTypeDef definition

class MessageMetadataTypeDef(TypedDict):
    MessageId: NotRequired[str],
    Receipts: NotRequired[List[ReceiptTypeDef]],  # (1)
```

1. See [:material-code-braces: ReceiptTypeDef](./type_defs.md#receipttypedef) 
## StartAttachmentUploadResponseTypeDef

```python
# StartAttachmentUploadResponseTypeDef definition

class StartAttachmentUploadResponseTypeDef(TypedDict):
    AttachmentId: str,
    UploadMetadata: UploadMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UploadMetadataTypeDef](./type_defs.md#uploadmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ItemTypeDef

```python
# ItemTypeDef definition

class ItemTypeDef(TypedDict):
    AbsoluteTime: NotRequired[str],
    Content: NotRequired[str],
    ContentType: NotRequired[str],
    Id: NotRequired[str],
    Type: NotRequired[ChatItemTypeType],  # (1)
    ParticipantId: NotRequired[str],
    DisplayName: NotRequired[str],
    ParticipantRole: NotRequired[ParticipantRoleType],  # (2)
    Attachments: NotRequired[List[AttachmentItemTypeDef]],  # (3)
    MessageMetadata: NotRequired[MessageMetadataTypeDef],  # (4)
    RelatedContactId: NotRequired[str],
    ContactId: NotRequired[str],
```

1. See [:material-code-brackets: ChatItemTypeType](./literals.md#chatitemtypetype) 
2. See [:material-code-brackets: ParticipantRoleType](./literals.md#participantroletype) 
3. See [:material-code-braces: AttachmentItemTypeDef](./type_defs.md#attachmentitemtypedef) 
4. See [:material-code-braces: MessageMetadataTypeDef](./type_defs.md#messagemetadatatypedef) 
## GetTranscriptResponseTypeDef

```python
# GetTranscriptResponseTypeDef definition

class GetTranscriptResponseTypeDef(TypedDict):
    InitialContactId: str,
    Transcript: List[ItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ItemTypeDef](./type_defs.md#itemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
