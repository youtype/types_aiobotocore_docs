# Examples

> [Index](../README.md) > [Transfer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
    type annotations stubs module [types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[transfer]` package installed.

Write your `Transfer` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("transfer") as client:  # (1)
        result = await client.create_access()  # (2)
    ```

    1. client: [TransferClient](./client.md)
    2. result: [:material-code-braces: CreateAccessResponseTypeDef](./type_defs.md#createaccessresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("transfer") as client:  # (1)
        paginator = client.get_paginator("list_accesses")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [TransferClient](./client.md)
    2. paginator: [ListAccessesPaginator](./paginators.md#listaccessespaginator)
    3. item: [:material-code-braces: ListAccessesResponseTypeDef](./type_defs.md#listaccessesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("transfer") as client:  # (1)
        waiter = client.get_waiter("server_offline")  # (2)
        await waiter.wait()
    ```

    1. client: [TransferClient](./client.md)
    2. waiter: [ServerOfflineWaiter](./waiters.md#serverofflinewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[transfer]`
or a standalone `types_aiobotocore_transfer` package, you have to explicitly specify
`client: TransferClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_transfer.client import TransferClient
    from types_aiobotocore_transfer.type_defs import CreateAccessResponseTypeDef
    from types_aiobotocore_transfer.type_defs import CreateAccessRequestRequestTypeDef


    session = get_session()

    async with session.create_client("transfer") as client:
        client: TransferClient
        kwargs: CreateAccessRequestRequestTypeDef = {...}
        result: CreateAccessResponseTypeDef = await client.create_access(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_transfer.client import TransferClient
    from types_aiobotocore_transfer.paginator import ListAccessesPaginator
    from types_aiobotocore_transfer.type_defs import ListAccessesResponseTypeDef


    session = get_session()

    async with session.create_client("transfer") as client:
        client: TransferClient
        paginator: ListAccessesPaginator = client.get_paginator("list_accesses")
        async for item in paginator.paginate(...):
            item: ListAccessesResponseTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_transfer.client import TransferClient
    from types_aiobotocore_transfer.waiter import ServerOfflineWaiter


    session = get_session()

    async with session.create_client("transfer") as client:
        client: TransferClient
        waiter: ServerOfflineWaiter = client.get_waiter("server_offline")
        await waiter.wait()
    ```
