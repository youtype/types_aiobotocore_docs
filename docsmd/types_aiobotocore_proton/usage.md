# Examples

> [Index](../README.md) > [Proton](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Proton](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
    type annotations stubs module [types-aiobotocore-proton](https://pypi.org/project/types-aiobotocore-proton/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[proton]` package installed.

Write your `Proton` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("proton") as client:  # (1)
        result = await client.accept_environment_account_connection()  # (2)
    ```

    1. client: [ProtonClient](./client.md)
    2. result: [:material-code-braces: AcceptEnvironmentAccountConnectionOutputTypeDef](./type_defs.md#acceptenvironmentaccountconnectionoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("proton") as client:  # (1)
        paginator = client.get_paginator("list_environment_account_connections")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ProtonClient](./client.md)
    2. paginator: [ListEnvironmentAccountConnectionsPaginator](./paginators.md#listenvironmentaccountconnectionspaginator)
    3. item: [:material-code-braces: ListEnvironmentAccountConnectionsOutputTypeDef](./type_defs.md#listenvironmentaccountconnectionsoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("proton") as client:  # (1)
        waiter = client.get_waiter("environment_deployed")  # (2)
        await waiter.wait()
    ```

    1. client: [ProtonClient](./client.md)
    2. waiter: [EnvironmentDeployedWaiter](./waiters.md#environmentdeployedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[proton]`
or a standalone `types_aiobotocore_proton` package, you have to explicitly specify
`client: ProtonClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_proton.client import ProtonClient
    from types_aiobotocore_proton.type_defs import AcceptEnvironmentAccountConnectionOutputTypeDef
    from types_aiobotocore_proton.type_defs import AcceptEnvironmentAccountConnectionInputRequestTypeDef


    session = get_session()

    async with session.create_client("proton") as client:
        client: ProtonClient
        kwargs: AcceptEnvironmentAccountConnectionInputRequestTypeDef = {...}
        result: AcceptEnvironmentAccountConnectionOutputTypeDef = await client.accept_environment_account_connection(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_proton.client import ProtonClient
    from types_aiobotocore_proton.paginator import ListEnvironmentAccountConnectionsPaginator
    from types_aiobotocore_proton.type_defs import ListEnvironmentAccountConnectionsOutputTypeDef


    session = get_session()

    async with session.create_client("proton") as client:
        client: ProtonClient
        paginator: ListEnvironmentAccountConnectionsPaginator = client.get_paginator("list_environment_account_connections")
        async for item in paginator.paginate(...):
            item: ListEnvironmentAccountConnectionsOutputTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_proton.client import ProtonClient
    from types_aiobotocore_proton.waiter import EnvironmentDeployedWaiter


    session = get_session()

    async with session.create_client("proton") as client:
        client: ProtonClient
        waiter: EnvironmentDeployedWaiter = client.get_waiter("environment_deployed")
        await waiter.wait()
    ```
