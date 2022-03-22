<a id="examples-for-aiobotocore-kafka-module"></a>

# Examples for aiobotocore Kafka module

> [Index](../README.md) > [Kafka](./README.md) > Examples

- [Examples for aiobotocore Kafka module](#examples-for-aiobotocore-kafka-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[kafka]` package installed.

Write your `Kafka` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type KafkaClient
# and provides type checking and code completion
async with session.create_client("kafka") as client:
    
    # result has type BatchAssociateScramSecretResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_associate_scram_secret()
    

    
    # paginator has type ListClusterOperationsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_cluster_operations")
    async for item in paginator.paginate(...):
        # item has type ListClusterOperationsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[kafka]` or a standalone `types_aiobotocore_kafka`
package, you have to explicitly specify `client: KafkaClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafka.client import KafkaClient
from types_aiobotocore_kafka.type_defs import BatchAssociateScramSecretResponseTypeDef
from types_aiobotocore_kafka.paginator import ListClusterOperationsPaginator

from types_aiobotocore_kafka.literals import PaginatorName



session = get_session()

async with session.create_client("kafka") as client:
    client: KafkaClient

    
    result: BatchAssociateScramSecretResponseTypeDef = client.batch_associate_scram_secret()
    

    
    paginator_name: PaginatorName = "list_cluster_operations"
    paginator: ListClusterOperationsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListClusterOperationsResponseTypeDef
        print(item)
    

    
```
