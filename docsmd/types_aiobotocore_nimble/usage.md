# Examples

> [Index](../README.md) > [NimbleStudio](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NimbleStudio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
    type annotations stubs module [types-aiobotocore-nimble](https://pypi.org/project/types-aiobotocore-nimble/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[nimble]` package installed.

Write your `NimbleStudio` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("nimble") as client:  # (1)
        result = await client.accept_eulas()  # (2)
    ```

    1. client: [NimbleStudioClient](./client.md)
    2. result: [:material-code-braces: AcceptEulasResponseTypeDef](./type_defs.md#accepteulasresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("nimble") as client:  # (1)
        paginator = client.get_paginator("list_eula_acceptances")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [NimbleStudioClient](./client.md)
    2. paginator: [ListEulaAcceptancesPaginator](./paginators.md#listeulaacceptancespaginator)
    3. item: [:material-code-braces: ListEulaAcceptancesResponseTypeDef](./type_defs.md#listeulaacceptancesresponsetypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("nimble") as client:  # (1)
        waiter = client.get_waiter("launch_profile_deleted")  # (2)
        await waiter.wait()
    ```

    1. client: [NimbleStudioClient](./client.md)
    2. waiter: [LaunchProfileDeletedWaiter](./waiters.md#launchprofiledeletedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[nimble]`
or a standalone `types_aiobotocore_nimble` package, you have to explicitly specify
`client: NimbleStudioClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_nimble.client import NimbleStudioClient
    from types_aiobotocore_nimble.type_defs import AcceptEulasResponseTypeDef
    from types_aiobotocore_nimble.type_defs import AcceptEulasRequestRequestTypeDef


    session = get_session()

    async with session.create_client("nimble") as client:
        client: NimbleStudioClient
        kwargs: AcceptEulasRequestRequestTypeDef = {...}
        result: AcceptEulasResponseTypeDef = await client.accept_eulas(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_nimble.client import NimbleStudioClient
    from types_aiobotocore_nimble.paginator import ListEulaAcceptancesPaginator
    from types_aiobotocore_nimble.type_defs import ListEulaAcceptancesResponseTypeDef


    session = get_session()

    async with session.create_client("nimble") as client:
        client: NimbleStudioClient
        paginator: ListEulaAcceptancesPaginator = client.get_paginator("list_eula_acceptances")
        async for item in paginator.paginate(...):
            item: ListEulaAcceptancesResponseTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_nimble.client import NimbleStudioClient
    from types_aiobotocore_nimble.waiter import LaunchProfileDeletedWaiter


    session = get_session()

    async with session.create_client("nimble") as client:
        client: NimbleStudioClient
        waiter: LaunchProfileDeletedWaiter = client.get_waiter("launch_profile_deleted")
        await waiter.wait()
    ```
