# Examples

> [Index](../README.md) > [LocationService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService)
    type annotations stubs module [types-aiobotocore-location](https://pypi.org/project/types-aiobotocore-location/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[location]` package installed.

Write your `LocationService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("location") as client:  # (1)
        result = await client.batch_delete_device_position_history()  # (2)
    ```

    1. client: [LocationServiceClient](./client.md)
    2. result: [:material-code-braces: BatchDeleteDevicePositionHistoryResponseTypeDef](./type_defs.md#batchdeletedevicepositionhistoryresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("location") as client:  # (1)
        paginator = client.get_paginator("get_device_position_history")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [LocationServiceClient](./client.md)
    2. paginator: [GetDevicePositionHistoryPaginator](./paginators.md#getdevicepositionhistorypaginator)
    3. item: [:material-code-braces: GetDevicePositionHistoryResponseTypeDef](./type_defs.md#getdevicepositionhistoryresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[location]`
or a standalone `types_aiobotocore_location` package, you have to explicitly specify
`client: LocationServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_location.client import LocationServiceClient
    from types_aiobotocore_location.type_defs import BatchDeleteDevicePositionHistoryResponseTypeDef
    from types_aiobotocore_location.type_defs import BatchDeleteDevicePositionHistoryRequestRequestTypeDef


    session = get_session()

    async with session.create_client("location") as client:
        client: LocationServiceClient
        kwargs: BatchDeleteDevicePositionHistoryRequestRequestTypeDef = {...}
        result: BatchDeleteDevicePositionHistoryResponseTypeDef = await client.batch_delete_device_position_history(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_location.client import LocationServiceClient
    from types_aiobotocore_location.paginator import GetDevicePositionHistoryPaginator
    from types_aiobotocore_location.type_defs import GetDevicePositionHistoryResponseTypeDef


    session = get_session()

    async with session.create_client("location") as client:
        client: LocationServiceClient
        paginator: GetDevicePositionHistoryPaginator = client.get_paginator("get_device_position_history")
        async for item in paginator.paginate(...):
            item: GetDevicePositionHistoryResponseTypeDef
            print(item)
    ```


