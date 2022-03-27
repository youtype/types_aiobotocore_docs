# Examples

> [Index](../README.md) > [DirectoryService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DirectoryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
    type annotations stubs module [types-aiobotocore-ds](https://pypi.org/project/types-aiobotocore-ds/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ds]` package installed.

Write your `DirectoryService` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("ds") as client:  # (1)
        result = await client.accept_shared_directory()  # (2)
    ```

    1. client: [DirectoryServiceClient](./client.md)
    2. result: [:material-code-braces: AcceptSharedDirectoryResultTypeDef](./type_defs.md#acceptshareddirectoryresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("ds") as client:  # (1)
        paginator = client.get_paginator("describe_directories")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [DirectoryServiceClient](./client.md)
    2. paginator: [DescribeDirectoriesPaginator](./paginators.md#describedirectoriespaginator)
    3. item: [:material-code-braces: DescribeDirectoriesResultTypeDef](./type_defs.md#describedirectoriesresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[ds]`
or a standalone `types_aiobotocore_ds` package, you have to explicitly specify
`client: DirectoryServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_ds.client import DirectoryServiceClient
    from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryResultTypeDef
    from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryRequestRequestTypeDef


    session = get_session()

    async with session.create_client("ds") as client:
        client: DirectoryServiceClient
        kwargs: AcceptSharedDirectoryRequestRequestTypeDef = {...}
        result: AcceptSharedDirectoryResultTypeDef = await client.accept_shared_directory(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_ds.client import DirectoryServiceClient
    from types_aiobotocore_ds.paginator import DescribeDirectoriesPaginator
    from types_aiobotocore_ds.type_defs import DescribeDirectoriesResultTypeDef


    session = get_session()

    async with session.create_client("ds") as client:
        client: DirectoryServiceClient
        paginator: DescribeDirectoriesPaginator = client.get_paginator("describe_directories")
        async for item in paginator.paginate(...):
            item: DescribeDirectoriesResultTypeDef
            print(item)
    ```


