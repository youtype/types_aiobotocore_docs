# Paginators

> [Index](../README.md) > [SQS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SQS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#sqs)
    type annotations stubs module [types-aiobotocore-sqs](https://pypi.org/project/types-aiobotocore-sqs/).

## ListDeadLetterSourceQueuesPaginator

Type annotations and code completion for `#!python session.create_client("sqs").get_paginator("list_dead_letter_source_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs/paginator/ListDeadLetterSourceQueues.html#SQS.Paginator.ListDeadLetterSourceQueues)

```python
# ListDeadLetterSourceQueuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sqs.paginator import ListDeadLetterSourceQueuesPaginator

session = get_session()
async with session.create_client("sqs") as client:  # (1)
    paginator: ListDeadLetterSourceQueuesPaginator = client.get_paginator("list_dead_letter_source_queues")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeadLetterSourceQueuesResultTypeDef
        print(item)  # (3)
```

1. client: [SQSClient](./client.md)
2. paginator: [ListDeadLetterSourceQueuesPaginator](./paginators.md#listdeadlettersourcequeuespaginator)
3. item: [:material-code-braces: ListDeadLetterSourceQueuesResultTypeDef](./type_defs.md#listdeadlettersourcequeuesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListDeadLetterSourceQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    QueueUrl: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDeadLetterSourceQueuesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeadLetterSourceQueuesResultTypeDef](./type_defs.md#listdeadlettersourcequeuesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeadLetterSourceQueuesRequestPaginateTypeDef = {  # (1)
    "QueueUrl": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeadLetterSourceQueuesRequestPaginateTypeDef](./type_defs.md#listdeadlettersourcequeuesrequestpaginatetypedef) 
## ListQueuesPaginator

Type annotations and code completion for `#!python session.create_client("sqs").get_paginator("list_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs/paginator/ListQueues.html#SQS.Paginator.ListQueues)

```python
# ListQueuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sqs.paginator import ListQueuesPaginator

session = get_session()
async with session.create_client("sqs") as client:  # (1)
    paginator: ListQueuesPaginator = client.get_paginator("list_queues")  # (2)
    async for item in paginator.paginate(...):
        item: ListQueuesResultTypeDef
        print(item)  # (3)
```

1. client: [SQSClient](./client.md)
2. paginator: [ListQueuesPaginator](./paginators.md#listqueuespaginator)
3. item: [:material-code-braces: ListQueuesResultTypeDef](./type_defs.md#listqueuesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    QueueNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListQueuesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQueuesResultTypeDef](./type_defs.md#listqueuesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListQueuesRequestPaginateTypeDef = {  # (1)
    "QueueNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQueuesRequestPaginateTypeDef](./type_defs.md#listqueuesrequestpaginatetypedef) 
