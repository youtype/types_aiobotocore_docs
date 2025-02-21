# Examples

> [Index](../README.md) > [MQ](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MQ](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#mq)
    type annotations stubs module [types-aiobotocore-mq](https://pypi.org/project/types-aiobotocore-mq/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mq]` package installed.

Write your `MQ` code as usual,
type checking and code completion should work out of the box.



```python
# MQClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mq") as client:  # (1)
    result = await client.create_broker()  # (2)
```

1. client: [MQClient](./client.md)
2. result: [:material-code-braces: CreateBrokerResponseTypeDef](./type_defs.md#createbrokerresponsetypedef) 



```python
# ListBrokersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mq") as client:  # (1)
    paginator = client.get_paginator("list_brokers")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MQClient](./client.md)
2. paginator: [ListBrokersPaginator](./paginators.md#listbrokerspaginator)
3. item: [:material-code-braces: ListBrokersResponseTypeDef](./type_defs.md#listbrokersresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[mq]`
or a standalone `types_aiobotocore_mq` package, you have to explicitly specify
`client: MQClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MQClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mq.client import MQClient
from types_aiobotocore_mq.type_defs import CreateBrokerResponseTypeDef
from types_aiobotocore_mq.type_defs import CreateBrokerRequestTypeDef


session = get_session()

async with session.create_client("mq") as client:
    client: MQClient
    kwargs: CreateBrokerRequestTypeDef = {...}
    result: CreateBrokerResponseTypeDef = await client.create_broker(**kwargs)
```



```python
# ListBrokersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mq.client import MQClient
from types_aiobotocore_mq.paginator import ListBrokersPaginator
from types_aiobotocore_mq.type_defs import ListBrokersResponseTypeDef


session = get_session()

async with session.create_client("mq") as client:
    client: MQClient
    paginator: ListBrokersPaginator = client.get_paginator("list_brokers")
    async for item in paginator.paginate(...):
        item: ListBrokersResponseTypeDef
        print(item)
```


