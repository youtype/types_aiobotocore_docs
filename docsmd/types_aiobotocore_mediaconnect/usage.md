# Examples

> [Index](../README.md) > [MediaConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mediaconnect]` package installed.

Write your `MediaConnect` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("mediaconnect") as client:  # (1)
        result = await client.add_flow_media_streams()  # (2)
    ```

    1. client: [MediaConnectClient](./client.md)
    2. result: [:material-code-braces: AddFlowMediaStreamsResponseTypeDef](./type_defs.md#addflowmediastreamsresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("mediaconnect") as client:  # (1)
        paginator = client.get_paginator("list_entitlements")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [MediaConnectClient](./client.md)
    2. paginator: [ListEntitlementsPaginator](./paginators.md#listentitlementspaginator)
    3. item: [:material-code-braces: ListEntitlementsResponseTypeDef](./type_defs.md#listentitlementsresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("mediaconnect") as client:  # (1)
        waiter = client.get_waiter("flow_active")  # (2)
        await waiter.wait()
    ```

    1. client: [MediaConnectClient](./client.md)
    2. waiter: [FlowActiveWaiter](./waiters.md#flowactivewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[mediaconnect]`
or a standalone `types_aiobotocore_mediaconnect` package, you have to explicitly specify
`client: MediaConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_mediaconnect.client import MediaConnectClient
    from types_aiobotocore_mediaconnect.type_defs import AddFlowMediaStreamsResponseTypeDef
    from types_aiobotocore_mediaconnect.type_defs import AddFlowMediaStreamsRequestRequestTypeDef


    session = get_session()

    async with session.create_client("mediaconnect") as client:
        client: MediaConnectClient
        kwargs: AddFlowMediaStreamsRequestRequestTypeDef = {...}
        result: AddFlowMediaStreamsResponseTypeDef = await client.add_flow_media_streams(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_mediaconnect.client import MediaConnectClient
    from types_aiobotocore_mediaconnect.paginator import ListEntitlementsPaginator
    from types_aiobotocore_mediaconnect.type_defs import ListEntitlementsResponseTypeDef


    session = get_session()

    async with session.create_client("mediaconnect") as client:
        client: MediaConnectClient
        paginator: ListEntitlementsPaginator = client.get_paginator("list_entitlements")
        async for item in paginator.paginate(...):
            item: ListEntitlementsResponseTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_mediaconnect.client import MediaConnectClient
    from types_aiobotocore_mediaconnect.waiter import FlowActiveWaiter


    session = get_session()

    async with session.create_client("mediaconnect") as client:
        client: MediaConnectClient
        waiter: FlowActiveWaiter = client.get_waiter("flow_active")
        await waiter.wait()
    ```
