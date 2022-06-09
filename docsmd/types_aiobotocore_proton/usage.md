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
        paginator = client.get_paginator("list_component_outputs")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ProtonClient](./client.md)
    2. paginator: [ListComponentOutputsPaginator](./paginators.md#listcomponentoutputspaginator)
    3. item: [:material-code-braces: ListComponentOutputsOutputTypeDef](./type_defs.md#listcomponentoutputsoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("proton") as client:  # (1)
        waiter = client.get_waiter("component_deleted")  # (2)
        await waiter.wait()
    ```

    1. client: [ProtonClient](./client.md)
    2. waiter: [ComponentDeletedWaiter](./waiters.md#componentdeletedwaiter)


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
    from types_aiobotocore_proton.paginator import ListComponentOutputsPaginator
    from types_aiobotocore_proton.type_defs import ListComponentOutputsOutputTypeDef


    session = get_session()

    async with session.create_client("proton") as client:
        client: ProtonClient
        paginator: ListComponentOutputsPaginator = client.get_paginator("list_component_outputs")
        async for item in paginator.paginate(...):
            item: ListComponentOutputsOutputTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_proton.client import ProtonClient
    from types_aiobotocore_proton.waiter import ComponentDeletedWaiter


    session = get_session()

    async with session.create_client("proton") as client:
        client: ProtonClient
        waiter: ComponentDeletedWaiter = client.get_waiter("component_deleted")
        await waiter.wait()
    ```
