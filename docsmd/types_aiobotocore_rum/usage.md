# Examples

> [Index](../README.md) > [CloudWatchRUM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
    type annotations stubs module [types-aiobotocore-rum](https://pypi.org/project/types-aiobotocore-rum/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[rum]` package installed.

Write your `CloudWatchRUM` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("rum") as client:  # (1)
        result = await client.create_app_monitor()  # (2)
    ```

    1. client: [CloudWatchRUMClient](./client.md)
    2. result: [:material-code-braces: CreateAppMonitorResponseTypeDef](./type_defs.md#createappmonitorresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("rum") as client:  # (1)
        paginator = client.get_paginator("get_app_monitor_data")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [CloudWatchRUMClient](./client.md)
    2. paginator: [GetAppMonitorDataPaginator](./paginators.md#getappmonitordatapaginator)
    3. item: [:material-code-braces: GetAppMonitorDataResponseTypeDef](./type_defs.md#getappmonitordataresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[rum]`
or a standalone `types_aiobotocore_rum` package, you have to explicitly specify
`client: CloudWatchRUMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_rum.client import CloudWatchRUMClient
    from types_aiobotocore_rum.type_defs import CreateAppMonitorResponseTypeDef
    from types_aiobotocore_rum.type_defs import CreateAppMonitorRequestRequestTypeDef


    session = get_session()

    async with session.create_client("rum") as client:
        client: CloudWatchRUMClient
        kwargs: CreateAppMonitorRequestRequestTypeDef = {...}
        result: CreateAppMonitorResponseTypeDef = await client.create_app_monitor(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_rum.client import CloudWatchRUMClient
    from types_aiobotocore_rum.paginator import GetAppMonitorDataPaginator
    from types_aiobotocore_rum.type_defs import GetAppMonitorDataResponseTypeDef


    session = get_session()

    async with session.create_client("rum") as client:
        client: CloudWatchRUMClient
        paginator: GetAppMonitorDataPaginator = client.get_paginator("get_app_monitor_data")
        async for item in paginator.paginate(...):
            item: GetAppMonitorDataResponseTypeDef
            print(item)
    ```


