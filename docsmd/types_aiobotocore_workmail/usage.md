# Examples

> [Index](../README.md) > [WorkMail](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkMail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
    type annotations stubs module [types-aiobotocore-workmail](https://pypi.org/project/types-aiobotocore-workmail/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[workmail]` package installed.

Write your `WorkMail` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("workmail") as client:  # (1)
        result = await client.create_group()  # (2)
    ```

    1. client: [WorkMailClient](./client.md)
    2. result: [:material-code-braces: CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("workmail") as client:  # (1)
        paginator = client.get_paginator("list_aliases")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [WorkMailClient](./client.md)
    2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
    3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[workmail]`
or a standalone `types_aiobotocore_workmail` package, you have to explicitly specify
`client: WorkMailClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_workmail.client import WorkMailClient
    from types_aiobotocore_workmail.type_defs import CreateGroupResponseTypeDef
    from types_aiobotocore_workmail.type_defs import CreateGroupRequestRequestTypeDef


    session = get_session()

    async with session.create_client("workmail") as client:
        client: WorkMailClient
        kwargs: CreateGroupRequestRequestTypeDef = {...}
        result: CreateGroupResponseTypeDef = await client.create_group(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_workmail.client import WorkMailClient
    from types_aiobotocore_workmail.paginator import ListAliasesPaginator
    from types_aiobotocore_workmail.type_defs import ListAliasesResponseTypeDef


    session = get_session()

    async with session.create_client("workmail") as client:
        client: WorkMailClient
        paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
        async for item in paginator.paginate(...):
            item: ListAliasesResponseTypeDef
            print(item)
    ```


