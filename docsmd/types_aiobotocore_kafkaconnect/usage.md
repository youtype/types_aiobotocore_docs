# Examples

> [Index](../README.md) > [KafkaConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KafkaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
    type annotations stubs module [types-aiobotocore-kafkaconnect](https://pypi.org/project/types-aiobotocore-kafkaconnect/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kafkaconnect]` package installed.

Write your `KafkaConnect` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("kafkaconnect") as client:  # (1)
        result = await client.create_connector()  # (2)
    ```

    1. client: [KafkaConnectClient](./client.md)
    2. result: [:material-code-braces: CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("kafkaconnect") as client:  # (1)
        paginator = client.get_paginator("list_connectors")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [KafkaConnectClient](./client.md)
    2. paginator: [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)
    3. item: [:material-code-braces: ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[kafkaconnect]`
or a standalone `types_aiobotocore_kafkaconnect` package, you have to explicitly specify
`client: KafkaConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_kafkaconnect.client import KafkaConnectClient
    from types_aiobotocore_kafkaconnect.type_defs import CreateConnectorResponseTypeDef
    from types_aiobotocore_kafkaconnect.type_defs import CreateConnectorRequestRequestTypeDef


    session = get_session()

    async with session.create_client("kafkaconnect") as client:
        client: KafkaConnectClient
        kwargs: CreateConnectorRequestRequestTypeDef = {...}
        result: CreateConnectorResponseTypeDef = await client.create_connector(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_kafkaconnect.client import KafkaConnectClient
    from types_aiobotocore_kafkaconnect.paginator import ListConnectorsPaginator
    from types_aiobotocore_kafkaconnect.type_defs import ListConnectorsResponseTypeDef


    session = get_session()

    async with session.create_client("kafkaconnect") as client:
        client: KafkaConnectClient
        paginator: ListConnectorsPaginator = client.get_paginator("list_connectors")
        async for item in paginator.paginate(...):
            item: ListConnectorsResponseTypeDef
            print(item)
    ```


