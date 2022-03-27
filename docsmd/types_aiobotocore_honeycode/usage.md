# Examples

> [Index](../README.md) > [Honeycode](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Honeycode](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
    type annotations stubs module [types-aiobotocore-honeycode](https://pypi.org/project/types-aiobotocore-honeycode/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[honeycode]` package installed.

Write your `Honeycode` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("honeycode") as client:  # (1)
        result = await client.batch_create_table_rows()  # (2)
    ```

    1. client: [HoneycodeClient](./client.md)
    2. result: [:material-code-braces: BatchCreateTableRowsResultTypeDef](./type_defs.md#batchcreatetablerowsresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("honeycode") as client:  # (1)
        paginator = client.get_paginator("list_table_columns")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [HoneycodeClient](./client.md)
    2. paginator: [ListTableColumnsPaginator](./paginators.md#listtablecolumnspaginator)
    3. item: [:material-code-braces: ListTableColumnsResultTypeDef](./type_defs.md#listtablecolumnsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[honeycode]`
or a standalone `types_aiobotocore_honeycode` package, you have to explicitly specify
`client: HoneycodeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_honeycode.client import HoneycodeClient
    from types_aiobotocore_honeycode.type_defs import BatchCreateTableRowsResultTypeDef
    from types_aiobotocore_honeycode.type_defs import BatchCreateTableRowsRequestRequestTypeDef


    session = get_session()

    async with session.create_client("honeycode") as client:
        client: HoneycodeClient
        kwargs: BatchCreateTableRowsRequestRequestTypeDef = {...}
        result: BatchCreateTableRowsResultTypeDef = await client.batch_create_table_rows(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_honeycode.client import HoneycodeClient
    from types_aiobotocore_honeycode.paginator import ListTableColumnsPaginator
    from types_aiobotocore_honeycode.type_defs import ListTableColumnsResultTypeDef


    session = get_session()

    async with session.create_client("honeycode") as client:
        client: HoneycodeClient
        paginator: ListTableColumnsPaginator = client.get_paginator("list_table_columns")
        async for item in paginator.paginate(...):
            item: ListTableColumnsResultTypeDef
            print(item)
    ```


