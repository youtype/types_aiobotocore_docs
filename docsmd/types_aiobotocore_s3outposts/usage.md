# Examples

> [Index](../README.md) > [S3Outposts](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
    type annotations stubs module [types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[s3outposts]` package installed.

Write your `S3Outposts` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("s3outposts") as client:  # (1)
        result = await client.create_endpoint()  # (2)
    ```

    1. client: [S3OutpostsClient](./client.md)
    2. result: [:material-code-braces: CreateEndpointResultTypeDef](./type_defs.md#createendpointresulttypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("s3outposts") as client:  # (1)
        paginator = client.get_paginator("list_endpoints")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [S3OutpostsClient](./client.md)
    2. paginator: [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
    3. item: [:material-code-braces: ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[s3outposts]`
or a standalone `types_aiobotocore_s3outposts` package, you have to explicitly specify
`client: S3OutpostsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_s3outposts.client import S3OutpostsClient
    from types_aiobotocore_s3outposts.type_defs import CreateEndpointResultTypeDef
    from types_aiobotocore_s3outposts.type_defs import CreateEndpointRequestRequestTypeDef


    session = get_session()

    async with session.create_client("s3outposts") as client:
        client: S3OutpostsClient
        kwargs: CreateEndpointRequestRequestTypeDef = {...}
        result: CreateEndpointResultTypeDef = await client.create_endpoint(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_s3outposts.client import S3OutpostsClient
    from types_aiobotocore_s3outposts.paginator import ListEndpointsPaginator
    from types_aiobotocore_s3outposts.type_defs import ListEndpointsResultTypeDef


    session = get_session()

    async with session.create_client("s3outposts") as client:
        client: S3OutpostsClient
        paginator: ListEndpointsPaginator = client.get_paginator("list_endpoints")
        async for item in paginator.paginate(...):
            item: ListEndpointsResultTypeDef
            print(item)
    ```


