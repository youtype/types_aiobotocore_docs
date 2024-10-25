# Type definitions

> [Index](../README.md) > [SQS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SQS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
    type annotations stubs module [types-aiobotocore-sqs](https://pypi.org/project/types-aiobotocore-sqs/).

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


## MessageAttributeValueUnionTypeDef

```python
# MessageAttributeValueUnionTypeDef definition

MessageAttributeValueUnionTypeDef = Union[
    MessageAttributeValueTypeDef,  # (1)
    MessageAttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
2. See [:material-code-braces: MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef) 



## AddPermissionRequestQueueAddPermissionTypeDef

```python
# AddPermissionRequestQueueAddPermissionTypeDef definition

class AddPermissionRequestQueueAddPermissionTypeDef(TypedDict):
    Label: str,
    AWSAccountIds: Sequence[str],
    Actions: Sequence[str],
```

## AddPermissionRequestRequestTypeDef

```python
# AddPermissionRequestRequestTypeDef definition

class AddPermissionRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    Label: str,
    AWSAccountIds: Sequence[str],
    Actions: Sequence[str],
```

## BatchResultErrorEntryTypeDef

```python
# BatchResultErrorEntryTypeDef definition

class BatchResultErrorEntryTypeDef(TypedDict):
    Id: str,
    SenderFault: bool,
    Code: str,
    Message: NotRequired[str],
```

## CancelMessageMoveTaskRequestRequestTypeDef

```python
# CancelMessageMoveTaskRequestRequestTypeDef definition

class CancelMessageMoveTaskRequestRequestTypeDef(TypedDict):
    TaskHandle: str,
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

## ChangeMessageVisibilityBatchRequestEntryTypeDef

```python
# ChangeMessageVisibilityBatchRequestEntryTypeDef definition

class ChangeMessageVisibilityBatchRequestEntryTypeDef(TypedDict):
    Id: str,
    ReceiptHandle: str,
    VisibilityTimeout: NotRequired[int],
```

## ChangeMessageVisibilityBatchResultEntryTypeDef

```python
# ChangeMessageVisibilityBatchResultEntryTypeDef definition

class ChangeMessageVisibilityBatchResultEntryTypeDef(TypedDict):
    Id: str,
```

## ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef

```python
# ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef definition

class ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef(TypedDict):
    VisibilityTimeout: int,
```

## ChangeMessageVisibilityRequestRequestTypeDef

```python
# ChangeMessageVisibilityRequestRequestTypeDef definition

class ChangeMessageVisibilityRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    ReceiptHandle: str,
    VisibilityTimeout: int,
```

## CreateQueueRequestRequestTypeDef

```python
# CreateQueueRequestRequestTypeDef definition

class CreateQueueRequestRequestTypeDef(TypedDict):
    QueueName: str,
    Attributes: NotRequired[Mapping[QueueAttributeNameType, str]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: QueueAttributeNameType](./literals.md#queueattributenametype) 
## CreateQueueRequestServiceResourceCreateQueueTypeDef

```python
# CreateQueueRequestServiceResourceCreateQueueTypeDef definition

class CreateQueueRequestServiceResourceCreateQueueTypeDef(TypedDict):
    QueueName: str,
    Attributes: NotRequired[Mapping[QueueAttributeNameType, str]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: QueueAttributeNameType](./literals.md#queueattributenametype) 
## DeleteMessageBatchRequestEntryTypeDef

```python
# DeleteMessageBatchRequestEntryTypeDef definition

class DeleteMessageBatchRequestEntryTypeDef(TypedDict):
    Id: str,
    ReceiptHandle: str,
```

## DeleteMessageBatchResultEntryTypeDef

```python
# DeleteMessageBatchResultEntryTypeDef definition

class DeleteMessageBatchResultEntryTypeDef(TypedDict):
    Id: str,
```

## DeleteMessageRequestRequestTypeDef

```python
# DeleteMessageRequestRequestTypeDef definition

class DeleteMessageRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    ReceiptHandle: str,
```

## DeleteQueueRequestRequestTypeDef

```python
# DeleteQueueRequestRequestTypeDef definition

class DeleteQueueRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
```

## GetQueueAttributesRequestRequestTypeDef

```python
# GetQueueAttributesRequestRequestTypeDef definition

class GetQueueAttributesRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    AttributeNames: NotRequired[Sequence[QueueAttributeFilterType]],  # (1)
```

1. See [:material-code-brackets: QueueAttributeFilterType](./literals.md#queueattributefiltertype) 
## GetQueueUrlRequestRequestTypeDef

```python
# GetQueueUrlRequestRequestTypeDef definition

class GetQueueUrlRequestRequestTypeDef(TypedDict):
    QueueName: str,
    QueueOwnerAWSAccountId: NotRequired[str],
```

## GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef

```python
# GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef definition

class GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef(TypedDict):
    QueueName: str,
    QueueOwnerAWSAccountId: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDeadLetterSourceQueuesRequestRequestTypeDef

```python
# ListDeadLetterSourceQueuesRequestRequestTypeDef definition

class ListDeadLetterSourceQueuesRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListMessageMoveTasksRequestRequestTypeDef

```python
# ListMessageMoveTasksRequestRequestTypeDef definition

class ListMessageMoveTasksRequestRequestTypeDef(TypedDict):
    SourceArn: str,
    MaxResults: NotRequired[int],
```

## ListMessageMoveTasksResultEntryTypeDef

```python
# ListMessageMoveTasksResultEntryTypeDef definition

class ListMessageMoveTasksResultEntryTypeDef(TypedDict):
    TaskHandle: NotRequired[str],
    Status: NotRequired[str],
    SourceArn: NotRequired[str],
    DestinationArn: NotRequired[str],
    MaxNumberOfMessagesPerSecond: NotRequired[int],
    ApproximateNumberOfMessagesMoved: NotRequired[int],
    ApproximateNumberOfMessagesToMove: NotRequired[int],
    FailureReason: NotRequired[str],
    StartedTimestamp: NotRequired[int],
```

## ListQueueTagsRequestRequestTypeDef

```python
# ListQueueTagsRequestRequestTypeDef definition

class ListQueueTagsRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
```

## ListQueuesRequestRequestTypeDef

```python
# ListQueuesRequestRequestTypeDef definition

class ListQueuesRequestRequestTypeDef(TypedDict):
    QueueNamePrefix: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MessageAttributeValueOutputTypeDef

```python
# MessageAttributeValueOutputTypeDef definition

class MessageAttributeValueOutputTypeDef(TypedDict):
    DataType: str,
    StringValue: NotRequired[str],
    BinaryValue: NotRequired[bytes],
    StringListValues: NotRequired[List[str]],
    BinaryListValues: NotRequired[List[bytes]],
```

## PurgeQueueRequestRequestTypeDef

```python
# PurgeQueueRequestRequestTypeDef definition

class PurgeQueueRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
```

## ReceiveMessageRequestQueueReceiveMessagesTypeDef

```python
# ReceiveMessageRequestQueueReceiveMessagesTypeDef definition

class ReceiveMessageRequestQueueReceiveMessagesTypeDef(TypedDict):
    AttributeNames: NotRequired[Sequence[QueueAttributeFilterType]],  # (1)
    MessageSystemAttributeNames: NotRequired[Sequence[MessageSystemAttributeNameType]],  # (2)
    MessageAttributeNames: NotRequired[Sequence[str]],
    MaxNumberOfMessages: NotRequired[int],
    VisibilityTimeout: NotRequired[int],
    WaitTimeSeconds: NotRequired[int],
    ReceiveRequestAttemptId: NotRequired[str],
```

1. See [:material-code-brackets: QueueAttributeFilterType](./literals.md#queueattributefiltertype) 
2. See [:material-code-brackets: MessageSystemAttributeNameType](./literals.md#messagesystemattributenametype) 
## ReceiveMessageRequestRequestTypeDef

```python
# ReceiveMessageRequestRequestTypeDef definition

class ReceiveMessageRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    AttributeNames: NotRequired[Sequence[QueueAttributeFilterType]],  # (1)
    MessageSystemAttributeNames: NotRequired[Sequence[MessageSystemAttributeNameType]],  # (2)
    MessageAttributeNames: NotRequired[Sequence[str]],
    MaxNumberOfMessages: NotRequired[int],
    VisibilityTimeout: NotRequired[int],
    WaitTimeSeconds: NotRequired[int],
    ReceiveRequestAttemptId: NotRequired[str],
```

1. See [:material-code-brackets: QueueAttributeFilterType](./literals.md#queueattributefiltertype) 
2. See [:material-code-brackets: MessageSystemAttributeNameType](./literals.md#messagesystemattributenametype) 
## RemovePermissionRequestQueueRemovePermissionTypeDef

```python
# RemovePermissionRequestQueueRemovePermissionTypeDef definition

class RemovePermissionRequestQueueRemovePermissionTypeDef(TypedDict):
    Label: str,
```

## RemovePermissionRequestRequestTypeDef

```python
# RemovePermissionRequestRequestTypeDef definition

class RemovePermissionRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    Label: str,
```

## SendMessageBatchResultEntryTypeDef

```python
# SendMessageBatchResultEntryTypeDef definition

class SendMessageBatchResultEntryTypeDef(TypedDict):
    Id: str,
    MessageId: str,
    MD5OfMessageBody: str,
    MD5OfMessageAttributes: NotRequired[str],
    MD5OfMessageSystemAttributes: NotRequired[str],
    SequenceNumber: NotRequired[str],
```

## SetQueueAttributesRequestQueueSetAttributesTypeDef

```python
# SetQueueAttributesRequestQueueSetAttributesTypeDef definition

class SetQueueAttributesRequestQueueSetAttributesTypeDef(TypedDict):
    Attributes: Mapping[QueueAttributeNameType, str],  # (1)
```

1. See [:material-code-brackets: QueueAttributeNameType](./literals.md#queueattributenametype) 
## SetQueueAttributesRequestRequestTypeDef

```python
# SetQueueAttributesRequestRequestTypeDef definition

class SetQueueAttributesRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    Attributes: Mapping[QueueAttributeNameType, str],  # (1)
```

1. See [:material-code-brackets: QueueAttributeNameType](./literals.md#queueattributenametype) 
## StartMessageMoveTaskRequestRequestTypeDef

```python
# StartMessageMoveTaskRequestRequestTypeDef definition

class StartMessageMoveTaskRequestRequestTypeDef(TypedDict):
    SourceArn: str,
    DestinationArn: NotRequired[str],
    MaxNumberOfMessagesPerSecond: NotRequired[int],
```

## TagQueueRequestRequestTypeDef

```python
# TagQueueRequestRequestTypeDef definition

class TagQueueRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    Tags: Mapping[str, str],
```

## UntagQueueRequestRequestTypeDef

```python
# UntagQueueRequestRequestTypeDef definition

class UntagQueueRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    TagKeys: Sequence[str],
```

## MessageAttributeValueTypeDef

```python
# MessageAttributeValueTypeDef definition

class MessageAttributeValueTypeDef(TypedDict):
    DataType: str,
    StringValue: NotRequired[str],
    BinaryValue: NotRequired[BlobTypeDef],
    StringListValues: NotRequired[Sequence[str]],
    BinaryListValues: NotRequired[Sequence[BlobTypeDef]],
```

## MessageSystemAttributeValueTypeDef

```python
# MessageSystemAttributeValueTypeDef definition

class MessageSystemAttributeValueTypeDef(TypedDict):
    DataType: str,
    StringValue: NotRequired[str],
    BinaryValue: NotRequired[BlobTypeDef],
    StringListValues: NotRequired[Sequence[str]],
    BinaryListValues: NotRequired[Sequence[BlobTypeDef]],
```

## CancelMessageMoveTaskResultTypeDef

```python
# CancelMessageMoveTaskResultTypeDef definition

class CancelMessageMoveTaskResultTypeDef(TypedDict):
    ApproximateNumberOfMessagesMoved: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQueueResultTypeDef

```python
# CreateQueueResultTypeDef definition

class CreateQueueResultTypeDef(TypedDict):
    QueueUrl: str,
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
## GetQueueAttributesResultTypeDef

```python
# GetQueueAttributesResultTypeDef definition

class GetQueueAttributesResultTypeDef(TypedDict):
    Attributes: Dict[QueueAttributeNameType, str],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: QueueAttributeNameType](./literals.md#queueattributenametype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueueUrlResultTypeDef

```python
# GetQueueUrlResultTypeDef definition

class GetQueueUrlResultTypeDef(TypedDict):
    QueueUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeadLetterSourceQueuesResultTypeDef

```python
# ListDeadLetterSourceQueuesResultTypeDef definition

class ListDeadLetterSourceQueuesResultTypeDef(TypedDict):
    queueUrls: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueueTagsResultTypeDef

```python
# ListQueueTagsResultTypeDef definition

class ListQueueTagsResultTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueuesResultTypeDef

```python
# ListQueuesResultTypeDef definition

class ListQueuesResultTypeDef(TypedDict):
    QueueUrls: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendMessageResultTypeDef

```python
# SendMessageResultTypeDef definition

class SendMessageResultTypeDef(TypedDict):
    MD5OfMessageBody: str,
    MD5OfMessageAttributes: str,
    MD5OfMessageSystemAttributes: str,
    MessageId: str,
    SequenceNumber: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMessageMoveTaskResultTypeDef

```python
# StartMessageMoveTaskResultTypeDef definition

class StartMessageMoveTaskResultTypeDef(TypedDict):
    TaskHandle: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef

```python
# ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef definition

class ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef(TypedDict):
    Entries: Sequence[ChangeMessageVisibilityBatchRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: ChangeMessageVisibilityBatchRequestEntryTypeDef](./type_defs.md#changemessagevisibilitybatchrequestentrytypedef) 
## ChangeMessageVisibilityBatchRequestRequestTypeDef

```python
# ChangeMessageVisibilityBatchRequestRequestTypeDef definition

class ChangeMessageVisibilityBatchRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    Entries: Sequence[ChangeMessageVisibilityBatchRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: ChangeMessageVisibilityBatchRequestEntryTypeDef](./type_defs.md#changemessagevisibilitybatchrequestentrytypedef) 
## ChangeMessageVisibilityBatchResultTypeDef

```python
# ChangeMessageVisibilityBatchResultTypeDef definition

class ChangeMessageVisibilityBatchResultTypeDef(TypedDict):
    Successful: List[ChangeMessageVisibilityBatchResultEntryTypeDef],  # (1)
    Failed: List[BatchResultErrorEntryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ChangeMessageVisibilityBatchResultEntryTypeDef](./type_defs.md#changemessagevisibilitybatchresultentrytypedef) 
2. See [:material-code-braces: BatchResultErrorEntryTypeDef](./type_defs.md#batchresulterrorentrytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMessageBatchRequestQueueDeleteMessagesTypeDef

```python
# DeleteMessageBatchRequestQueueDeleteMessagesTypeDef definition

class DeleteMessageBatchRequestQueueDeleteMessagesTypeDef(TypedDict):
    Entries: Sequence[DeleteMessageBatchRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: DeleteMessageBatchRequestEntryTypeDef](./type_defs.md#deletemessagebatchrequestentrytypedef) 
## DeleteMessageBatchRequestRequestTypeDef

```python
# DeleteMessageBatchRequestRequestTypeDef definition

class DeleteMessageBatchRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    Entries: Sequence[DeleteMessageBatchRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: DeleteMessageBatchRequestEntryTypeDef](./type_defs.md#deletemessagebatchrequestentrytypedef) 
## DeleteMessageBatchResultTypeDef

```python
# DeleteMessageBatchResultTypeDef definition

class DeleteMessageBatchResultTypeDef(TypedDict):
    Successful: List[DeleteMessageBatchResultEntryTypeDef],  # (1)
    Failed: List[BatchResultErrorEntryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DeleteMessageBatchResultEntryTypeDef](./type_defs.md#deletemessagebatchresultentrytypedef) 
2. See [:material-code-braces: BatchResultErrorEntryTypeDef](./type_defs.md#batchresulterrorentrytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef

```python
# ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef definition

class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(TypedDict):
    QueueUrl: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueuesRequestListQueuesPaginateTypeDef

```python
# ListQueuesRequestListQueuesPaginateTypeDef definition

class ListQueuesRequestListQueuesPaginateTypeDef(TypedDict):
    QueueNamePrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMessageMoveTasksResultTypeDef

```python
# ListMessageMoveTasksResultTypeDef definition

class ListMessageMoveTasksResultTypeDef(TypedDict):
    Results: List[ListMessageMoveTasksResultEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListMessageMoveTasksResultEntryTypeDef](./type_defs.md#listmessagemovetasksresultentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    MessageId: NotRequired[str],
    ReceiptHandle: NotRequired[str],
    MD5OfBody: NotRequired[str],
    Body: NotRequired[str],
    Attributes: NotRequired[Dict[MessageSystemAttributeNameType, str]],  # (1)
    MD5OfMessageAttributes: NotRequired[str],
    MessageAttributes: NotRequired[Dict[str, MessageAttributeValueOutputTypeDef]],  # (2)
```

1. See [:material-code-brackets: MessageSystemAttributeNameType](./literals.md#messagesystemattributenametype) 
2. See [:material-code-braces: MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef) 
## SendMessageBatchResultTypeDef

```python
# SendMessageBatchResultTypeDef definition

class SendMessageBatchResultTypeDef(TypedDict):
    Successful: List[SendMessageBatchResultEntryTypeDef],  # (1)
    Failed: List[BatchResultErrorEntryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SendMessageBatchResultEntryTypeDef](./type_defs.md#sendmessagebatchresultentrytypedef) 
2. See [:material-code-braces: BatchResultErrorEntryTypeDef](./type_defs.md#batchresulterrorentrytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendMessageBatchRequestEntryTypeDef

```python
# SendMessageBatchRequestEntryTypeDef definition

class SendMessageBatchRequestEntryTypeDef(TypedDict):
    Id: str,
    MessageBody: str,
    DelaySeconds: NotRequired[int],
    MessageAttributes: NotRequired[Mapping[str, MessageAttributeValueTypeDef]],  # (1)
    MessageSystemAttributes: NotRequired[Mapping[MessageSystemAttributeNameForSendsType, MessageSystemAttributeValueTypeDef]],  # (2)
    MessageDeduplicationId: NotRequired[str],
    MessageGroupId: NotRequired[str],
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
2. See [:material-code-brackets: MessageSystemAttributeNameForSendsType](./literals.md#messagesystemattributenameforsendstype) [:material-code-braces: MessageSystemAttributeValueTypeDef](./type_defs.md#messagesystemattributevaluetypedef) 
## SendMessageRequestQueueSendMessageTypeDef

```python
# SendMessageRequestQueueSendMessageTypeDef definition

class SendMessageRequestQueueSendMessageTypeDef(TypedDict):
    MessageBody: str,
    DelaySeconds: NotRequired[int],
    MessageAttributes: NotRequired[Mapping[str, MessageAttributeValueTypeDef]],  # (1)
    MessageSystemAttributes: NotRequired[Mapping[MessageSystemAttributeNameForSendsType, MessageSystemAttributeValueTypeDef]],  # (2)
    MessageDeduplicationId: NotRequired[str],
    MessageGroupId: NotRequired[str],
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
2. See [:material-code-brackets: MessageSystemAttributeNameForSendsType](./literals.md#messagesystemattributenameforsendstype) [:material-code-braces: MessageSystemAttributeValueTypeDef](./type_defs.md#messagesystemattributevaluetypedef) 
## ReceiveMessageResultTypeDef

```python
# ReceiveMessageResultTypeDef definition

class ReceiveMessageResultTypeDef(TypedDict):
    Messages: List[MessageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendMessageRequestRequestTypeDef

```python
# SendMessageRequestRequestTypeDef definition

class SendMessageRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    MessageBody: str,
    DelaySeconds: NotRequired[int],
    MessageAttributes: NotRequired[Mapping[str, MessageAttributeValueUnionTypeDef]],  # (1)
    MessageSystemAttributes: NotRequired[Mapping[MessageSystemAttributeNameForSendsType, MessageSystemAttributeValueTypeDef]],  # (2)
    MessageDeduplicationId: NotRequired[str],
    MessageGroupId: NotRequired[str],
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) [:material-code-braces: MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef) 
2. See [:material-code-brackets: MessageSystemAttributeNameForSendsType](./literals.md#messagesystemattributenameforsendstype) [:material-code-braces: MessageSystemAttributeValueTypeDef](./type_defs.md#messagesystemattributevaluetypedef) 
## SendMessageBatchRequestQueueSendMessagesTypeDef

```python
# SendMessageBatchRequestQueueSendMessagesTypeDef definition

class SendMessageBatchRequestQueueSendMessagesTypeDef(TypedDict):
    Entries: Sequence[SendMessageBatchRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: SendMessageBatchRequestEntryTypeDef](./type_defs.md#sendmessagebatchrequestentrytypedef) 
## SendMessageBatchRequestRequestTypeDef

```python
# SendMessageBatchRequestRequestTypeDef definition

class SendMessageBatchRequestRequestTypeDef(TypedDict):
    QueueUrl: str,
    Entries: Sequence[SendMessageBatchRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: SendMessageBatchRequestEntryTypeDef](./type_defs.md#sendmessagebatchrequestentrytypedef) 
