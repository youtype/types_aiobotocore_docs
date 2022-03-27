# Examples

> [Index](../README.md) > [Macie2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Macie2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
    type annotations stubs module [types-aiobotocore-macie2](https://pypi.org/project/types-aiobotocore-macie2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[macie2]` package installed.

Write your `Macie2` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("macie2") as client:  # (1)
        result = await client.batch_get_custom_data_identifiers()  # (2)
    ```

    1. client: [Macie2Client](./client.md)
    2. result: [:material-code-braces: BatchGetCustomDataIdentifiersResponseTypeDef](./type_defs.md#batchgetcustomdataidentifiersresponsetypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("macie2") as client:  # (1)
        paginator = client.get_paginator("describe_buckets")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [Macie2Client](./client.md)
    2. paginator: [DescribeBucketsPaginator](./paginators.md#describebucketspaginator)
    3. item: [:material-code-braces: DescribeBucketsResponseTypeDef](./type_defs.md#describebucketsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[macie2]`
or a standalone `types_aiobotocore_macie2` package, you have to explicitly specify
`client: Macie2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_macie2.client import Macie2Client
    from types_aiobotocore_macie2.type_defs import BatchGetCustomDataIdentifiersResponseTypeDef
    from types_aiobotocore_macie2.type_defs import BatchGetCustomDataIdentifiersRequestRequestTypeDef


    session = get_session()

    async with session.create_client("macie2") as client:
        client: Macie2Client
        kwargs: BatchGetCustomDataIdentifiersRequestRequestTypeDef = {...}
        result: BatchGetCustomDataIdentifiersResponseTypeDef = await client.batch_get_custom_data_identifiers(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_macie2.client import Macie2Client
    from types_aiobotocore_macie2.paginator import DescribeBucketsPaginator
    from types_aiobotocore_macie2.type_defs import DescribeBucketsResponseTypeDef


    session = get_session()

    async with session.create_client("macie2") as client:
        client: Macie2Client
        paginator: DescribeBucketsPaginator = client.get_paginator("describe_buckets")
        async for item in paginator.paginate(...):
            item: DescribeBucketsResponseTypeDef
            print(item)
    ```


