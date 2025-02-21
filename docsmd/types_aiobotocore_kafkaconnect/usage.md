# Examples

> [Index](../README.md) > [KafkaConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KafkaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#kafkaconnect)
    type annotations stubs module [types-aiobotocore-kafkaconnect](https://pypi.org/project/types-aiobotocore-kafkaconnect/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kafkaconnect]` package installed.

Write your `KafkaConnect` code as usual,
type checking and code completion should work out of the box.



```python
# KafkaConnectClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kafkaconnect") as client:  # (1)
    result = await client.create_connector()  # (2)
```

1. client: [KafkaConnectClient](./client.md)
2. result: [:material-code-braces: CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef) 



```python
# ListConnectorOperationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kafkaconnect") as client:  # (1)
    paginator = client.get_paginator("list_connector_operations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [KafkaConnectClient](./client.md)
2. paginator: [ListConnectorOperationsPaginator](./paginators.md#listconnectoroperationspaginator)
3. item: [:material-code-braces: ListConnectorOperationsResponseTypeDef](./type_defs.md#listconnectoroperationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[kafkaconnect]`
or a standalone `types_aiobotocore_kafkaconnect` package, you have to explicitly specify
`client: KafkaConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KafkaConnectClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kafkaconnect.client import KafkaConnectClient
from types_aiobotocore_kafkaconnect.type_defs import CreateConnectorResponseTypeDef
from types_aiobotocore_kafkaconnect.type_defs import CreateConnectorRequestTypeDef


session = get_session()

async with session.create_client("kafkaconnect") as client:
    client: KafkaConnectClient
    kwargs: CreateConnectorRequestTypeDef = {...}
    result: CreateConnectorResponseTypeDef = await client.create_connector(**kwargs)
```



```python
# ListConnectorOperationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kafkaconnect.client import KafkaConnectClient
from types_aiobotocore_kafkaconnect.paginator import ListConnectorOperationsPaginator
from types_aiobotocore_kafkaconnect.type_defs import ListConnectorOperationsResponseTypeDef


session = get_session()

async with session.create_client("kafkaconnect") as client:
    client: KafkaConnectClient
    paginator: ListConnectorOperationsPaginator = client.get_paginator("list_connector_operations")
    async for item in paginator.paginate(...):
        item: ListConnectorOperationsResponseTypeDef
        print(item)
```


