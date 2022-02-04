<a id="paginators-for-aiobotocore-sqs-module"></a>

# Paginators for aiobotocore SQS module

> [Index](..) > [SQS](.) > Paginators

Auto-generated documentation for
[SQS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
type annotations stubs module
[types-aiobotocore-sqs](https://pypi.org/project/types-aiobotocore-sqs/).

- [Paginators for aiobotocore SQS module](#paginators-for-aiobotocore-sqs-module)
  - [ListDeadLetterSourceQueuesPaginator](#listdeadlettersourcequeuespaginator)
  - [ListQueuesPaginator](#listqueuespaginator)

<a id="listdeadlettersourcequeuespaginator"></a>

## ListDeadLetterSourceQueuesPaginator

Type annotations for
`aiobotocore.create_client("sqs").get_paginator("list_dead_letter_source_queues")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_sqs.paginator import ListDeadLetterSourceQueuesPaginator

def get_list_dead_letter_source_queues_paginator() -> ListDeadLetterSourceQueuesPaginator:
    return Session().create_client("sqs").get_paginator("list_dead_letter_source_queues")
```

Boto3 documentation:
[SQS.Paginator.ListDeadLetterSourceQueues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)

Arguments for `ListDeadLetterSourceQueuesPaginator.paginate` method:

- `QueueUrl`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeadLetterSourceQueuesPaginator.paginate` returns
`_PageIterator`\[[ListDeadLetterSourceQueuesResultTypeDef](./type_defs.md#listdeadlettersourcequeuesresulttypedef)\].

<a id="listqueuespaginator"></a>

## ListQueuesPaginator

Type annotations for
`aiobotocore.create_client("sqs").get_paginator("list_queues")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_sqs.paginator import ListQueuesPaginator

def get_list_queues_paginator() -> ListQueuesPaginator:
    return Session().create_client("sqs").get_paginator("list_queues")
```

Boto3 documentation:
[SQS.Paginator.ListQueues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)

Arguments for `ListQueuesPaginator.paginate` method:

- `QueueNamePrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListQueuesPaginator.paginate` returns
`_PageIterator`\[[ListQueuesResultTypeDef](./type_defs.md#listqueuesresulttypedef)\].
