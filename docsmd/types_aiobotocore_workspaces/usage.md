# Examples

> [Index](../README.md) > [WorkSpaces](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
    type annotations stubs module [types-aiobotocore-workspaces](https://pypi.org/project/types-aiobotocore-workspaces/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[workspaces]` package installed.

Write your `WorkSpaces` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("workspaces") as client:  # (1)
        result = await client.associate_connection_alias()  # (2)
    ```

    1. client: [WorkSpacesClient](./client.md)
    2. result: [:material-code-braces: AssociateConnectionAliasResultTypeDef](./type_defs.md#associateconnectionaliasresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("workspaces") as client:  # (1)
        paginator = client.get_paginator("describe_account_modifications")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [WorkSpacesClient](./client.md)
    2. paginator: [DescribeAccountModificationsPaginator](./paginators.md#describeaccountmodificationspaginator)
    3. item: [:material-code-braces: DescribeAccountModificationsResultTypeDef](./type_defs.md#describeaccountmodificationsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[workspaces]`
or a standalone `types_aiobotocore_workspaces` package, you have to explicitly specify
`client: WorkSpacesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_workspaces.client import WorkSpacesClient
    from types_aiobotocore_workspaces.type_defs import AssociateConnectionAliasResultTypeDef
    from types_aiobotocore_workspaces.type_defs import AssociateConnectionAliasRequestRequestTypeDef


    session = get_session()

    async with session.create_client("workspaces") as client:
        client: WorkSpacesClient
        kwargs: AssociateConnectionAliasRequestRequestTypeDef = {...}
        result: AssociateConnectionAliasResultTypeDef = await client.associate_connection_alias(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_workspaces.client import WorkSpacesClient
    from types_aiobotocore_workspaces.paginator import DescribeAccountModificationsPaginator
    from types_aiobotocore_workspaces.type_defs import DescribeAccountModificationsResultTypeDef


    session = get_session()

    async with session.create_client("workspaces") as client:
        client: WorkSpacesClient
        paginator: DescribeAccountModificationsPaginator = client.get_paginator("describe_account_modifications")
        async for item in paginator.paginate(...):
            item: DescribeAccountModificationsResultTypeDef
            print(item)
    ```


