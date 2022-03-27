# Examples

> [Index](../README.md) > [mgn](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
    type annotations stubs module [types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mgn]` package installed.

Write your `mgn` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("mgn") as client:  # (1)
        result = await client.change_server_life_cycle_state()  # (2)
    ```

    1. client: [mgnClient](./client.md)
    2. result: [:material-code-braces: SourceServerResponseMetadataTypeDef](./type_defs.md#sourceserverresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("mgn") as client:  # (1)
        paginator = client.get_paginator("describe_job_log_items")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [mgnClient](./client.md)
    2. paginator: [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
    3. item: [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[mgn]`
or a standalone `types_aiobotocore_mgn` package, you have to explicitly specify
`client: mgnClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_mgn.client import mgnClient
    from types_aiobotocore_mgn.type_defs import SourceServerResponseMetadataTypeDef
    from types_aiobotocore_mgn.type_defs import ChangeServerLifeCycleStateRequestRequestTypeDef


    session = get_session()

    async with session.create_client("mgn") as client:
        client: mgnClient
        kwargs: ChangeServerLifeCycleStateRequestRequestTypeDef = {...}
        result: SourceServerResponseMetadataTypeDef = await client.change_server_life_cycle_state(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_mgn.client import mgnClient
    from types_aiobotocore_mgn.paginator import DescribeJobLogItemsPaginator
    from types_aiobotocore_mgn.type_defs import DescribeJobLogItemsResponseTypeDef


    session = get_session()

    async with session.create_client("mgn") as client:
        client: mgnClient
        paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")
        async for item in paginator.paginate(...):
            item: DescribeJobLogItemsResponseTypeDef
            print(item)
    ```


