# Examples

> [Index](../README.md) > [Kafka](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#kafka)
    type annotations stubs module [types-aiobotocore-kafka](https://pypi.org/project/types-aiobotocore-kafka/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kafka]` package installed.

Write your `Kafka` code as usual,
type checking and code completion should work out of the box.



```python
# KafkaClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kafka") as client:  # (1)
    result = await client.batch_associate_scram_secret()  # (2)
```

1. client: [KafkaClient](./client.md)
2. result: [:material-code-braces: BatchAssociateScramSecretResponseTypeDef](./type_defs.md#batchassociatescramsecretresponsetypedef) 



```python
# ListClientVpcConnectionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kafka") as client:  # (1)
    paginator = client.get_paginator("list_client_vpc_connections")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [KafkaClient](./client.md)
2. paginator: [ListClientVpcConnectionsPaginator](./paginators.md#listclientvpcconnectionspaginator)
3. item: [:material-code-braces: ListClientVpcConnectionsResponseTypeDef](./type_defs.md#listclientvpcconnectionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[kafka]`
or a standalone `types_aiobotocore_kafka` package, you have to explicitly specify
`client: KafkaClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KafkaClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kafka.client import KafkaClient
from types_aiobotocore_kafka.type_defs import BatchAssociateScramSecretResponseTypeDef
from types_aiobotocore_kafka.type_defs import BatchAssociateScramSecretRequestTypeDef


session = get_session()

async with session.create_client("kafka") as client:
    client: KafkaClient
    kwargs: BatchAssociateScramSecretRequestTypeDef = {...}
    result: BatchAssociateScramSecretResponseTypeDef = await client.batch_associate_scram_secret(**kwargs)
```



```python
# ListClientVpcConnectionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kafka.client import KafkaClient
from types_aiobotocore_kafka.paginator import ListClientVpcConnectionsPaginator
from types_aiobotocore_kafka.type_defs import ListClientVpcConnectionsResponseTypeDef


session = get_session()

async with session.create_client("kafka") as client:
    client: KafkaClient
    paginator: ListClientVpcConnectionsPaginator = client.get_paginator("list_client_vpc_connections")
    async for item in paginator.paginate(...):
        item: ListClientVpcConnectionsResponseTypeDef
        print(item)
```


