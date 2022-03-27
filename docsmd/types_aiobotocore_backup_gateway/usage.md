# Examples

> [Index](../README.md) > [BackupGateway](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BackupGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
    type annotations stubs module [types-aiobotocore-backup-gateway](https://pypi.org/project/types-aiobotocore-backup-gateway/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[backup-gateway]` package installed.

Write your `BackupGateway` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("backup-gateway") as client:  # (1)
        result = await client.associate_gateway_to_server()  # (2)
    ```

    1. client: [BackupGatewayClient](./client.md)
    2. result: [:material-code-braces: AssociateGatewayToServerOutputTypeDef](./type_defs.md#associategatewaytoserveroutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("backup-gateway") as client:  # (1)
        paginator = client.get_paginator("list_gateways")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [BackupGatewayClient](./client.md)
    2. paginator: [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
    3. item: [:material-code-braces: ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[backup-gateway]`
or a standalone `types_aiobotocore_backup_gateway` package, you have to explicitly specify
`client: BackupGatewayClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_backup_gateway.client import BackupGatewayClient
    from types_aiobotocore_backup_gateway.type_defs import AssociateGatewayToServerOutputTypeDef
    from types_aiobotocore_backup_gateway.type_defs import AssociateGatewayToServerInputRequestTypeDef


    session = get_session()

    async with session.create_client("backup-gateway") as client:
        client: BackupGatewayClient
        kwargs: AssociateGatewayToServerInputRequestTypeDef = {...}
        result: AssociateGatewayToServerOutputTypeDef = await client.associate_gateway_to_server(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_backup_gateway.client import BackupGatewayClient
    from types_aiobotocore_backup_gateway.paginator import ListGatewaysPaginator
    from types_aiobotocore_backup_gateway.type_defs import ListGatewaysOutputTypeDef


    session = get_session()

    async with session.create_client("backup-gateway") as client:
        client: BackupGatewayClient
        paginator: ListGatewaysPaginator = client.get_paginator("list_gateways")
        async for item in paginator.paginate(...):
            item: ListGatewaysOutputTypeDef
            print(item)
    ```


