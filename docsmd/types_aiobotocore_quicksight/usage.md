# Examples

> [Index](../README.md) > [QuickSight](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QuickSight](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
    type annotations stubs module [types-aiobotocore-quicksight](https://pypi.org/project/types-aiobotocore-quicksight/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[quicksight]` package installed.

Write your `QuickSight` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("quicksight") as client:  # (1)
        result = await client.cancel_ingestion()  # (2)
    ```

    1. client: [QuickSightClient](./client.md)
    2. result: [:material-code-braces: CancelIngestionResponseTypeDef](./type_defs.md#cancelingestionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("quicksight") as client:  # (1)
        paginator = client.get_paginator("list_analyses")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [QuickSightClient](./client.md)
    2. paginator: [ListAnalysesPaginator](./paginators.md#listanalysespaginator)
    3. item: [:material-code-braces: ListAnalysesResponseTypeDef](./type_defs.md#listanalysesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[quicksight]`
or a standalone `types_aiobotocore_quicksight` package, you have to explicitly specify
`client: QuickSightClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_quicksight.client import QuickSightClient
    from types_aiobotocore_quicksight.type_defs import CancelIngestionResponseTypeDef
    from types_aiobotocore_quicksight.type_defs import CancelIngestionRequestRequestTypeDef


    session = get_session()

    async with session.create_client("quicksight") as client:
        client: QuickSightClient
        kwargs: CancelIngestionRequestRequestTypeDef = {...}
        result: CancelIngestionResponseTypeDef = await client.cancel_ingestion(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_quicksight.client import QuickSightClient
    from types_aiobotocore_quicksight.paginator import ListAnalysesPaginator
    from types_aiobotocore_quicksight.type_defs import ListAnalysesResponseTypeDef


    session = get_session()

    async with session.create_client("quicksight") as client:
        client: QuickSightClient
        paginator: ListAnalysesPaginator = client.get_paginator("list_analyses")
        async for item in paginator.paginate(...):
            item: ListAnalysesResponseTypeDef
            print(item)
    ```


