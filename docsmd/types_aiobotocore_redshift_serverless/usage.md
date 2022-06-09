# Examples

> [Index](../README.md) > [RedshiftServerless](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RedshiftServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
    type annotations stubs module [types-aiobotocore-redshift-serverless](https://pypi.org/project/types-aiobotocore-redshift-serverless/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[redshift-serverless]` package installed.

Write your `RedshiftServerless` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("redshift-serverless") as client:  # (1)
        result = await client.convert_recovery_point_to_snapshot()  # (2)
    ```

    1. client: [RedshiftServerlessClient](./client.md)
    2. result: [:material-code-braces: ConvertRecoveryPointToSnapshotResponseTypeDef](./type_defs.md#convertrecoverypointtosnapshotresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("redshift-serverless") as client:  # (1)
        paginator = client.get_paginator("list_endpoint_access")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [RedshiftServerlessClient](./client.md)
    2. paginator: [ListEndpointAccessPaginator](./paginators.md#listendpointaccesspaginator)
    3. item: [:material-code-braces: ListEndpointAccessResponseTypeDef](./type_defs.md#listendpointaccessresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[redshift-serverless]`
or a standalone `types_aiobotocore_redshift_serverless` package, you have to explicitly specify
`client: RedshiftServerlessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_redshift_serverless.client import RedshiftServerlessClient
    from types_aiobotocore_redshift_serverless.type_defs import ConvertRecoveryPointToSnapshotResponseTypeDef
    from types_aiobotocore_redshift_serverless.type_defs import ConvertRecoveryPointToSnapshotRequestRequestTypeDef


    session = get_session()

    async with session.create_client("redshift-serverless") as client:
        client: RedshiftServerlessClient
        kwargs: ConvertRecoveryPointToSnapshotRequestRequestTypeDef = {...}
        result: ConvertRecoveryPointToSnapshotResponseTypeDef = await client.convert_recovery_point_to_snapshot(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_redshift_serverless.client import RedshiftServerlessClient
    from types_aiobotocore_redshift_serverless.paginator import ListEndpointAccessPaginator
    from types_aiobotocore_redshift_serverless.type_defs import ListEndpointAccessResponseTypeDef


    session = get_session()

    async with session.create_client("redshift-serverless") as client:
        client: RedshiftServerlessClient
        paginator: ListEndpointAccessPaginator = client.get_paginator("list_endpoint_access")
        async for item in paginator.paginate(...):
            item: ListEndpointAccessResponseTypeDef
            print(item)
    ```


