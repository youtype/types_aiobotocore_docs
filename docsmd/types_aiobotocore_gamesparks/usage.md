# Examples

> [Index](../README.md) > [GameSparks](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [GameSparks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
    type annotations stubs module [types-aiobotocore-gamesparks](https://pypi.org/project/types-aiobotocore-gamesparks/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[gamesparks]` package installed.

Write your `GameSparks` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("gamesparks") as client:  # (1)
        result = await client.create_game()  # (2)
    ```

    1. client: [GameSparksClient](./client.md)
    2. result: [:material-code-braces: CreateGameResultTypeDef](./type_defs.md#creategameresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("gamesparks") as client:  # (1)
        paginator = client.get_paginator("list_extension_versions")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [GameSparksClient](./client.md)
    2. paginator: [ListExtensionVersionsPaginator](./paginators.md#listextensionversionspaginator)
    3. item: [:material-code-braces: ListExtensionVersionsResultTypeDef](./type_defs.md#listextensionversionsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[gamesparks]`
or a standalone `types_aiobotocore_gamesparks` package, you have to explicitly specify
`client: GameSparksClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_gamesparks.client import GameSparksClient
    from types_aiobotocore_gamesparks.type_defs import CreateGameResultTypeDef
    from types_aiobotocore_gamesparks.type_defs import CreateGameRequestRequestTypeDef


    session = get_session()

    async with session.create_client("gamesparks") as client:
        client: GameSparksClient
        kwargs: CreateGameRequestRequestTypeDef = {...}
        result: CreateGameResultTypeDef = await client.create_game(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_gamesparks.client import GameSparksClient
    from types_aiobotocore_gamesparks.paginator import ListExtensionVersionsPaginator
    from types_aiobotocore_gamesparks.type_defs import ListExtensionVersionsResultTypeDef


    session = get_session()

    async with session.create_client("gamesparks") as client:
        client: GameSparksClient
        paginator: ListExtensionVersionsPaginator = client.get_paginator("list_extension_versions")
        async for item in paginator.paginate(...):
            item: ListExtensionVersionsResultTypeDef
            print(item)
    ```


