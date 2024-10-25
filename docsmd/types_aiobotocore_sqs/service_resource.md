# SQSServiceResource

> [Index](../README.md) > [SQS](./README.md) > SQSServiceResource

!!! note ""

    Auto-generated documentation for [SQS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
    type annotations stubs module [types-aiobotocore-sqs](https://pypi.org/project/types-aiobotocore-sqs/).

## SQSServiceResource

Type annotations and code completion for `#!python session.resource("sqs")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource)

```python
# SQSServiceResource usage example

from types_aiobotocore_sqs.service_resource import SQSServiceResource

def get_sqs_resource() -> SQSServiceResource:
    return session.resource("sqs")
```


## Attributes


- `meta`: `"SQSResourceMeta"`

- `queues`: `ServiceResourceQueuesCollection`




## Collections

### ServiceResourceQueuesCollection

Provides access to [Queue](#queue) resource.

Type annotations and code completion for `#!python session.resource("sqs").queues` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.queues)

```python
# ServiceResourceQueuesCollection usage example

from types_aiobotocore_sqs.service_resource import ServiceResourceQueuesCollection

def get_collection() -> ServiceResourceQueuesCollection:
    return session.resource("sqs").queues
```



## Methods

### SQSServiceResource.Message method

Creates a Message resource.

Type annotations and code completion for `#!python session.resource("sqs").Message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Message)

```python
# Message method definition

await def Message(
    self,
    queue_url: str,
    receipt_handle: str,
) -> "_Message":
    ...
```


### SQSServiceResource.Queue method

Creates a Queue resource.

Type annotations and code completion for `#!python session.resource("sqs").Queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Queue)

```python
# Queue method definition

await def Queue(
    self,
    url: str,
) -> "_Queue":
    ...
```


### SQSServiceResource.create\_queue method

Creates a new standard or FIFO queue.

Type annotations and code completion for `#!python session.resource("sqs").create_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.create_queue)

```python
# create_queue method definition

await def create_queue(
    self,
    *,
    QueueName: str,
    Attributes: Mapping[QueueAttributeNameType, str] = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> "_Queue":
    ...
```

1. See [:material-code-brackets: QueueAttributeNameType](./literals.md#queueattributenametype) 


```python
# create_queue method usage example with argument unpacking

kwargs: CreateQueueRequestServiceResourceCreateQueueTypeDef = {  # (1)
    "QueueName": ...,
}

parent.create_queue(**kwargs)
```

1. See [:material-code-braces: CreateQueueRequestServiceResourceCreateQueueTypeDef](./type_defs.md#createqueuerequestserviceresourcecreatequeuetypedef) 

### SQSServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python session.resource("sqs").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


### SQSServiceResource.get\_queue\_by\_name method

Returns the URL of an existing Amazon SQS queue.

Type annotations and code completion for `#!python session.resource("sqs").get_queue_by_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.get_queue_by_name)

```python
# get_queue_by_name method definition

await def get_queue_by_name(
    self,
    *,
    QueueName: str,
    QueueOwnerAWSAccountId: str = ...,
) -> "_Queue":
    ...
```



```python
# get_queue_by_name method usage example with argument unpacking

kwargs: GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef = {  # (1)
    "QueueName": ...,
}

parent.get_queue_by_name(**kwargs)
```

1. See [:material-code-braces: GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef](./type_defs.md#getqueueurlrequestserviceresourcegetqueuebynametypedef) 



## Message

Type annotations and code completion for `#!python session.resource("sqs").Message` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Message)

```python
# Message usage example

from types_aiobotocore_sqs.service_resource import Message

def get_resource() -> Message:
    return session.resource("sqs").Message(...)
```


### Message attributes


- `message_id`: `Awaitable`[`str`]
- `md5_of_body`: `Awaitable`[`str`]
- `body`: `Awaitable`[`str`]
- `attributes`: `Awaitable`[`Dict`[[MessageSystemAttributeNameType](./literals.md#messagesystemattributenametype), `str`]]
- `md5_of_message_attributes`: `Awaitable`[`str`]
- `message_attributes`: `Awaitable`[`Dict`[`str`, [MessageAttributeValueOutputTypeDef](./type_defs.md#messageattributevalueoutputtypedef)]]
- `queue_url`: `str`
- `receipt_handle`: `str`
- `meta`: `"SQSResourceMeta"`





### Message methods


#### Message.Queue method

Creates a Queue resource.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").Queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Message.Queue)

```python
# Queue method definition

await def Queue(
    self,
) -> "_Queue":
    ...
```


#### Message.change\_visibility method

Changes the visibility timeout of a specified message in a queue to a new value.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").change_visibility` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Message.change_visibility)

```python
# change_visibility method definition

await def change_visibility(
    self,
    *,
    VisibilityTimeout: int,
) -> None:
    ...
```



```python
# change_visibility method usage example with argument unpacking

kwargs: ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef = {  # (1)
    "VisibilityTimeout": ...,
}

parent.change_visibility(**kwargs)
```

1. See [:material-code-braces: ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef](./type_defs.md#changemessagevisibilityrequestmessagechangevisibilitytypedef) 

#### Message.delete method

Deletes the specified message from the specified queue.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Message.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Message.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Message.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```





## Queue

Type annotations and code completion for `#!python session.resource("sqs").Queue` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.ServiceResource.Queue)

```python
# Queue usage example

from types_aiobotocore_sqs.service_resource import Queue

def get_resource() -> Queue:
    return session.resource("sqs").Queue(...)
```


### Queue attributes


- `attributes`: `Awaitable`[`Dict`[[QueueAttributeNameType](./literals.md#queueattributenametype), `str`]]
- `url`: `str`
- `dead_letter_source_queues`: `QueueDeadLetterSourceQueuesCollection`
- `meta`: `"SQSResourceMeta"`



### Queue collections


#### Queue.dead_letter_source_queues

Provides access to [Queue](#queue) resource.

Type annotations and code completion for `#!python session.resource("sqs").Queue(...).dead_letter_source_queues` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.dead_letter_source_queues)

```python
# QueueDeadLetterSourceQueuesCollection usage example

from types_aiobotocore_sqs.service_resource import QueueDeadLetterSourceQueuesCollection

def get_collection() -> QueueDeadLetterSourceQueuesCollection:
    resource = session.resource("sqs").Queue(...)
    return resource.dead_letter_source_queues
```




### Queue methods


#### Queue.Message method

Creates a Message resource.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").Message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.Message)

```python
# Message method definition

await def Message(
    self,
    receipt_handle: str,
) -> "_Message":
    ...
```


#### Queue.add\_permission method

Adds a permission to a queue for a specific
[principal](https://docs.aws.amazon.com/general/latest/gr/glos-chap.html#P).

Type annotations and code completion for `#!python aiobotocore.resource("sqs").add_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.add_permission)

```python
# add_permission method definition

await def add_permission(
    self,
    *,
    Label: str,
    AWSAccountIds: Sequence[str],
    Actions: Sequence[str],
) -> None:
    ...
```



```python
# add_permission method usage example with argument unpacking

kwargs: AddPermissionRequestQueueAddPermissionTypeDef = {  # (1)
    "Label": ...,
    "AWSAccountIds": ...,
    "Actions": ...,
}

parent.add_permission(**kwargs)
```

1. See [:material-code-braces: AddPermissionRequestQueueAddPermissionTypeDef](./type_defs.md#addpermissionrequestqueueaddpermissiontypedef) 

#### Queue.change\_message\_visibility\_batch method

Changes the visibility timeout of multiple messages.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").change_message_visibility_batch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.change_message_visibility_batch)

```python
# change_message_visibility_batch method definition

await def change_message_visibility_batch(
    self,
    *,
    Entries: Sequence[ChangeMessageVisibilityBatchRequestEntryTypeDef],  # (1)
) -> ChangeMessageVisibilityBatchResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ChangeMessageVisibilityBatchRequestEntryTypeDef](./type_defs.md#changemessagevisibilitybatchrequestentrytypedef) 
2. See [:material-code-braces: ChangeMessageVisibilityBatchResultTypeDef](./type_defs.md#changemessagevisibilitybatchresulttypedef) 


```python
# change_message_visibility_batch method usage example with argument unpacking

kwargs: ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef = {  # (1)
    "Entries": ...,
}

parent.change_message_visibility_batch(**kwargs)
```

1. See [:material-code-braces: ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef](./type_defs.md#changemessagevisibilitybatchrequestqueuechangemessagevisibilitybatchtypedef) 

#### Queue.delete method

Deletes the queue specified by the `QueueUrl`, regardless of the queue's
contents.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.delete)

```python
# delete method definition

await def delete(
    self,
) -> None:
    ...
```


#### Queue.delete\_messages method

Deletes up to ten messages from the specified queue.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").delete_messages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.delete_messages)

```python
# delete_messages method definition

await def delete_messages(
    self,
    *,
    Entries: Sequence[DeleteMessageBatchRequestEntryTypeDef],  # (1)
) -> DeleteMessageBatchResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeleteMessageBatchRequestEntryTypeDef](./type_defs.md#deletemessagebatchrequestentrytypedef) 
2. See [:material-code-braces: DeleteMessageBatchResultTypeDef](./type_defs.md#deletemessagebatchresulttypedef) 


```python
# delete_messages method usage example with argument unpacking

kwargs: DeleteMessageBatchRequestQueueDeleteMessagesTypeDef = {  # (1)
    "Entries": ...,
}

parent.delete_messages(**kwargs)
```

1. See [:material-code-braces: DeleteMessageBatchRequestQueueDeleteMessagesTypeDef](./type_defs.md#deletemessagebatchrequestqueuedeletemessagestypedef) 

#### Queue.get\_available\_subresources method

Returns a list of all the available sub-resources for this Resource.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.get_available_subresources)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Queue.load method

Calls :py:meth:`SQS.Client.get_queue_attributes` to update the attributes of
the Queue
resource.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.load)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Queue.purge method

Deletes available messages in a queue (including in-flight messages) specified
by the `QueueURL`
parameter.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").purge` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.purge)

```python
# purge method definition

await def purge(
    self,
) -> None:
    ...
```


#### Queue.receive\_messages method

Retrieves one or more messages (up to 10), from the specified queue.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").receive_messages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.receive_messages)

```python
# receive_messages method definition

await def receive_messages(
    self,
    *,
    AttributeNames: Sequence[QueueAttributeFilterType] = ...,  # (1)
    MessageSystemAttributeNames: Sequence[MessageSystemAttributeNameType] = ...,  # (2)
    MessageAttributeNames: Sequence[str] = ...,
    MaxNumberOfMessages: int = ...,
    VisibilityTimeout: int = ...,
    WaitTimeSeconds: int = ...,
    ReceiveRequestAttemptId: str = ...,
) -> List["_Message"]:
    ...
```

1. See [:material-code-brackets: QueueAttributeFilterType](./literals.md#queueattributefiltertype) 
2. See [:material-code-brackets: MessageSystemAttributeNameType](./literals.md#messagesystemattributenametype) 


```python
# receive_messages method usage example with argument unpacking

kwargs: ReceiveMessageRequestQueueReceiveMessagesTypeDef = {  # (1)
    "AttributeNames": ...,
}

parent.receive_messages(**kwargs)
```

1. See [:material-code-braces: ReceiveMessageRequestQueueReceiveMessagesTypeDef](./type_defs.md#receivemessagerequestqueuereceivemessagestypedef) 

#### Queue.reload method

Calls :py:meth:`SQS.Client.get_queue_attributes` to update the attributes of
the Queue
resource.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.reload)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```


#### Queue.remove\_permission method

Revokes any permissions in the queue policy that matches the specified `Label`
parameter.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").remove_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.remove_permission)

```python
# remove_permission method definition

await def remove_permission(
    self,
    *,
    Label: str,
) -> None:
    ...
```



```python
# remove_permission method usage example with argument unpacking

kwargs: RemovePermissionRequestQueueRemovePermissionTypeDef = {  # (1)
    "Label": ...,
}

parent.remove_permission(**kwargs)
```

1. See [:material-code-braces: RemovePermissionRequestQueueRemovePermissionTypeDef](./type_defs.md#removepermissionrequestqueueremovepermissiontypedef) 

#### Queue.send\_message method

Delivers a message to the specified queue.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").send_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_message)

```python
# send_message method definition

await def send_message(
    self,
    *,
    MessageBody: str,
    DelaySeconds: int = ...,
    MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,  # (1)
    MessageSystemAttributes: Mapping[MessageSystemAttributeNameForSendsType, MessageSystemAttributeValueTypeDef] = ...,  # (2)
    MessageDeduplicationId: str = ...,
    MessageGroupId: str = ...,
) -> SendMessageResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
2. See [:material-code-brackets: MessageSystemAttributeNameForSendsType](./literals.md#messagesystemattributenameforsendstype) [:material-code-braces: MessageSystemAttributeValueTypeDef](./type_defs.md#messagesystemattributevaluetypedef) 
3. See [:material-code-braces: SendMessageResultTypeDef](./type_defs.md#sendmessageresulttypedef) 


```python
# send_message method usage example with argument unpacking

kwargs: SendMessageRequestQueueSendMessageTypeDef = {  # (1)
    "MessageBody": ...,
}

parent.send_message(**kwargs)
```

1. See [:material-code-braces: SendMessageRequestQueueSendMessageTypeDef](./type_defs.md#sendmessagerequestqueuesendmessagetypedef) 

#### Queue.send\_messages method

You can use `SendMessageBatch` to send up to 10 messages to the specified queue
by assigning either identical or different values to each message (or by not
assigning values at
all).

Type annotations and code completion for `#!python aiobotocore.resource("sqs").send_messages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)

```python
# send_messages method definition

await def send_messages(
    self,
    *,
    Entries: Sequence[SendMessageBatchRequestEntryTypeDef],  # (1)
) -> SendMessageBatchResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SendMessageBatchRequestEntryTypeDef](./type_defs.md#sendmessagebatchrequestentrytypedef) 
2. See [:material-code-braces: SendMessageBatchResultTypeDef](./type_defs.md#sendmessagebatchresulttypedef) 


```python
# send_messages method usage example with argument unpacking

kwargs: SendMessageBatchRequestQueueSendMessagesTypeDef = {  # (1)
    "Entries": ...,
}

parent.send_messages(**kwargs)
```

1. See [:material-code-braces: SendMessageBatchRequestQueueSendMessagesTypeDef](./type_defs.md#sendmessagebatchrequestqueuesendmessagestypedef) 

#### Queue.set\_attributes method

Sets the value of one or more queue attributes, like a policy.

Type annotations and code completion for `#!python aiobotocore.resource("sqs").set_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.set_attributes)

```python
# set_attributes method definition

await def set_attributes(
    self,
    *,
    Attributes: Mapping[QueueAttributeNameType, str],  # (1)
) -> None:
    ...
```

1. See [:material-code-brackets: QueueAttributeNameType](./literals.md#queueattributenametype) 


```python
# set_attributes method usage example with argument unpacking

kwargs: SetQueueAttributesRequestQueueSetAttributesTypeDef = {  # (1)
    "Attributes": ...,
}

parent.set_attributes(**kwargs)
```

1. See [:material-code-braces: SetQueueAttributesRequestQueueSetAttributesTypeDef](./type_defs.md#setqueueattributesrequestqueuesetattributestypedef) 



