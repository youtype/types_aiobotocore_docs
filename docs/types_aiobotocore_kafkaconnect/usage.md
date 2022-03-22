<a id="examples-for-aiobotocore-kafkaconnect-module"></a>

# Examples for aiobotocore KafkaConnect module

> [Index](../README.md) > [KafkaConnect](./README.md) > Examples

- [Examples for aiobotocore KafkaConnect module](#examples-for-aiobotocore-kafkaconnect-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[kafkaconnect]` package installed.

Write your `KafkaConnect` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type KafkaConnectClient
# and provides type checking and code completion
async with session.create_client("kafkaconnect") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListConnectorsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_connectors")
    async for item in paginator.paginate(...):
        # item has type ListConnectorsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[kafkaconnect]` or a standalone
`types_aiobotocore_kafkaconnect` package, you have to explicitly specify
`client: KafkaConnectClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_kafkaconnect.client import KafkaConnectClient
from types_aiobotocore_kafkaconnect.type_defs import bool
from types_aiobotocore_kafkaconnect.paginator import ListConnectorsPaginator

from types_aiobotocore_kafkaconnect.literals import PaginatorName



session = get_session()

async with session.create_client("kafkaconnect") as client:
    client: KafkaConnectClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_connectors"
    paginator: ListConnectorsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListConnectorsResponseTypeDef
        print(item)
    

    
```
