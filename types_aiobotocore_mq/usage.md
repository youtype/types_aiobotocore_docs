<a id="examples-for-aiobotocore-mq-module"></a>

# Examples for aiobotocore MQ module

> [Index](../README.md) > [MQ](./README.md) > Examples

- [Examples for aiobotocore MQ module](#examples-for-aiobotocore-mq-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mq]` package installed.

Write your `MQ` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MQClient
# and provides type checking and code completion
async with session.create_client("mq") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListBrokersPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_brokers")
    async for item in paginator.paginate(...):
        # item has type ListBrokersResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mq]` or a standalone `types_aiobotocore_mq`
package, you have to explicitly specify `client: MQClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mq.client import MQClient
from types_aiobotocore_mq.type_defs import bool
from types_aiobotocore_mq.paginator import ListBrokersPaginator

from types_aiobotocore_mq.literals import PaginatorName



session = get_session()

async with session.create_client("mq") as client:
    client: MQClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_brokers"
    paginator: ListBrokersPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListBrokersResponseTypeDef
        print(item)
    

    
```
