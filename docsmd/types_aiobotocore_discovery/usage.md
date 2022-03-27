# Examples

> [Index](../README.md) > [ApplicationDiscoveryService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ApplicationDiscoveryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
    type annotations stubs module [types-aiobotocore-discovery](https://pypi.org/project/types-aiobotocore-discovery/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[discovery]` package installed.

Write your `ApplicationDiscoveryService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("discovery") as client:  # (1)
        result = await client.batch_delete_import_data()  # (2)
    ```

    1. client: [ApplicationDiscoveryServiceClient](./client.md)
    2. result: [:material-code-braces: BatchDeleteImportDataResponseTypeDef](./type_defs.md#batchdeleteimportdataresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("discovery") as client:  # (1)
        paginator = client.get_paginator("describe_agents")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ApplicationDiscoveryServiceClient](./client.md)
    2. paginator: [DescribeAgentsPaginator](./paginators.md#describeagentspaginator)
    3. item: [:material-code-braces: DescribeAgentsResponseTypeDef](./type_defs.md#describeagentsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[discovery]`
or a standalone `types_aiobotocore_discovery` package, you have to explicitly specify
`client: ApplicationDiscoveryServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_discovery.client import ApplicationDiscoveryServiceClient
    from types_aiobotocore_discovery.type_defs import BatchDeleteImportDataResponseTypeDef
    from types_aiobotocore_discovery.type_defs import BatchDeleteImportDataRequestRequestTypeDef


    session = get_session()

    async with session.create_client("discovery") as client:
        client: ApplicationDiscoveryServiceClient
        kwargs: BatchDeleteImportDataRequestRequestTypeDef = {...}
        result: BatchDeleteImportDataResponseTypeDef = await client.batch_delete_import_data(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_discovery.client import ApplicationDiscoveryServiceClient
    from types_aiobotocore_discovery.paginator import DescribeAgentsPaginator
    from types_aiobotocore_discovery.type_defs import DescribeAgentsResponseTypeDef


    session = get_session()

    async with session.create_client("discovery") as client:
        client: ApplicationDiscoveryServiceClient
        paginator: DescribeAgentsPaginator = client.get_paginator("describe_agents")
        async for item in paginator.paginate(...):
            item: DescribeAgentsResponseTypeDef
            print(item)
    ```


