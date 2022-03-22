<a id="examples-for-aiobotocore-sqs-module"></a>

# Examples for aiobotocore SQS module

> [Index](../README.md) > [SQS](./README.md) > Examples

- [Examples for aiobotocore SQS module](#examples-for-aiobotocore-sqs-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sqs]` package installed.

Write your `SQS` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SQSClient
# and provides type checking and code completion
async with session.create_client("sqs") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_permission()
    

    
    # paginator has type ListDeadLetterSourceQueuesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_dead_letter_source_queues")
    async for item in paginator.paginate(...):
        # item has type ListDeadLetterSourceQueuesResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sqs]` or a standalone `types_aiobotocore_sqs`
package, you have to explicitly specify `client: SQSClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sqs.client import SQSClient
from types_aiobotocore_sqs.type_defs import None
from types_aiobotocore_sqs.paginator import ListDeadLetterSourceQueuesPaginator

from types_aiobotocore_sqs.literals import PaginatorName



session = get_session()

async with session.create_client("sqs") as client:
    client: SQSClient

    
    result: None = client.add_permission()
    

    
    paginator_name: PaginatorName = "list_dead_letter_source_queues"
    paginator: ListDeadLetterSourceQueuesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListDeadLetterSourceQueuesResultTypeDef
        print(item)
    

    
```
