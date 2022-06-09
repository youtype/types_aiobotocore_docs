# Examples

> [Index](../README.md) > [Connect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
    type annotations stubs module [types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[connect]` package installed.

Write your `Connect` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("connect") as client:  # (1)
        result = await client.associate_approved_origin()  # (2)
    ```

    1. client: [ConnectClient](./client.md)
    2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("connect") as client:  # (1)
        paginator = client.get_paginator("get_metric_data")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [ConnectClient](./client.md)
    2. paginator: [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
    3. item: [:material-code-braces: GetMetricDataResponseTypeDef](./type_defs.md#getmetricdataresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[connect]`
or a standalone `types_aiobotocore_connect` package, you have to explicitly specify
`client: ConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_connect.client import ConnectClient
    from types_aiobotocore_connect.type_defs import EmptyResponseMetadataTypeDef
    from types_aiobotocore_connect.type_defs import AssociateApprovedOriginRequestRequestTypeDef


    session = get_session()

    async with session.create_client("connect") as client:
        client: ConnectClient
        kwargs: AssociateApprovedOriginRequestRequestTypeDef = {...}
        result: EmptyResponseMetadataTypeDef = await client.associate_approved_origin(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_connect.client import ConnectClient
    from types_aiobotocore_connect.paginator import GetMetricDataPaginator
    from types_aiobotocore_connect.type_defs import GetMetricDataResponseTypeDef


    session = get_session()

    async with session.create_client("connect") as client:
        client: ConnectClient
        paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")
        async for item in paginator.paginate(...):
            item: GetMetricDataResponseTypeDef
            print(item)
    ```


