# Examples

> [Index](../README.md) > [Glue](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Glue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
    type annotations stubs module [types-aiobotocore-glue](https://pypi.org/project/types-aiobotocore-glue/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[glue]` package installed.

Write your `Glue` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("glue") as client:  # (1)
        result = await client.batch_create_partition()  # (2)
    ```

    1. client: [GlueClient](./client.md)
    2. result: [:material-code-braces: BatchCreatePartitionResponseTypeDef](./type_defs.md#batchcreatepartitionresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("glue") as client:  # (1)
        paginator = client.get_paginator("get_classifiers")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [GlueClient](./client.md)
    2. paginator: [GetClassifiersPaginator](./paginators.md#getclassifierspaginator)
    3. item: [:material-code-braces: GetClassifiersResponseTypeDef](./type_defs.md#getclassifiersresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[glue]`
or a standalone `types_aiobotocore_glue` package, you have to explicitly specify
`client: GlueClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_glue.client import GlueClient
    from types_aiobotocore_glue.type_defs import BatchCreatePartitionResponseTypeDef
    from types_aiobotocore_glue.type_defs import BatchCreatePartitionRequestRequestTypeDef


    session = get_session()

    async with session.create_client("glue") as client:
        client: GlueClient
        kwargs: BatchCreatePartitionRequestRequestTypeDef = {...}
        result: BatchCreatePartitionResponseTypeDef = await client.batch_create_partition(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_glue.client import GlueClient
    from types_aiobotocore_glue.paginator import GetClassifiersPaginator
    from types_aiobotocore_glue.type_defs import GetClassifiersResponseTypeDef


    session = get_session()

    async with session.create_client("glue") as client:
        client: GlueClient
        paginator: GetClassifiersPaginator = client.get_paginator("get_classifiers")
        async for item in paginator.paginate(...):
            item: GetClassifiersResponseTypeDef
            print(item)
    ```


