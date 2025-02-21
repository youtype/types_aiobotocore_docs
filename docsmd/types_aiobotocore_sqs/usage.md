# Examples

> [Index](../README.md) > [SQS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SQS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#sqs)
    type annotations stubs module [types-aiobotocore-sqs](https://pypi.org/project/types-aiobotocore-sqs/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sqs]` package installed.

Write your `SQS` code as usual,
type checking and code completion should work out of the box.



```python
# SQSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sqs") as client:  # (1)
    result = await client.add_permission()  # (2)
```

1. client: [SQSClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListDeadLetterSourceQueuesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sqs") as client:  # (1)
    paginator = client.get_paginator("list_dead_letter_source_queues")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SQSClient](./client.md)
2. paginator: [ListDeadLetterSourceQueuesPaginator](./paginators.md#listdeadlettersourcequeuespaginator)
3. item: [:material-code-braces: ListDeadLetterSourceQueuesResultTypeDef](./type_defs.md#listdeadlettersourcequeuesresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[sqs]`
or a standalone `types_aiobotocore_sqs` package, you have to explicitly specify
`client: SQSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SQSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sqs.client import SQSClient
from types_aiobotocore_sqs.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_sqs.type_defs import AddPermissionRequestTypeDef


session = get_session()

async with session.create_client("sqs") as client:
    client: SQSClient
    kwargs: AddPermissionRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.add_permission(**kwargs)
```



```python
# ListDeadLetterSourceQueuesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sqs.client import SQSClient
from types_aiobotocore_sqs.paginator import ListDeadLetterSourceQueuesPaginator
from types_aiobotocore_sqs.type_defs import ListDeadLetterSourceQueuesResultTypeDef


session = get_session()

async with session.create_client("sqs") as client:
    client: SQSClient
    paginator: ListDeadLetterSourceQueuesPaginator = client.get_paginator("list_dead_letter_source_queues")
    async for item in paginator.paginate(...):
        item: ListDeadLetterSourceQueuesResultTypeDef
        print(item)
```


