# Examples

> [Index](../README.md) > [Kinesis](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
    type annotations stubs module [types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kinesis]` package installed.

Write your `Kinesis` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("kinesis") as client:  # (1)
        result = await client.describe_stream()  # (2)
    ```

    1. client: [KinesisClient](./client.md)
    2. result: [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("kinesis") as client:  # (1)
        paginator = client.get_paginator("describe_stream")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [KinesisClient](./client.md)
    2. paginator: [DescribeStreamPaginator](./paginators.md#describestreampaginator)
    3. item: [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef) 



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("kinesis") as client:  # (1)
        waiter = client.get_waiter("stream_exists")  # (2)
        await waiter.wait()
    ```

    1. client: [KinesisClient](./client.md)
    2. waiter: [StreamExistsWaiter](./waiters.md#streamexistswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[kinesis]`
or a standalone `types_aiobotocore_kinesis` package, you have to explicitly specify
`client: KinesisClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_kinesis.client import KinesisClient
    from types_aiobotocore_kinesis.type_defs import DescribeStreamOutputTypeDef
    from types_aiobotocore_kinesis.type_defs import DescribeStreamInputRequestTypeDef


    session = get_session()

    async with session.create_client("kinesis") as client:
        client: KinesisClient
        kwargs: DescribeStreamInputRequestTypeDef = {...}
        result: DescribeStreamOutputTypeDef = await client.describe_stream(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_kinesis.client import KinesisClient
    from types_aiobotocore_kinesis.paginator import DescribeStreamPaginator
    from types_aiobotocore_kinesis.type_defs import DescribeStreamOutputTypeDef


    session = get_session()

    async with session.create_client("kinesis") as client:
        client: KinesisClient
        paginator: DescribeStreamPaginator = client.get_paginator("describe_stream")
        async for item in paginator.paginate(...):
            item: DescribeStreamOutputTypeDef
            print(item)
    ```



=== "Waiters"

    ```python title="Waiter usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_kinesis.client import KinesisClient
    from types_aiobotocore_kinesis.waiter import StreamExistsWaiter


    session = get_session()

    async with session.create_client("kinesis") as client:
        client: KinesisClient
        waiter: StreamExistsWaiter = client.get_waiter("stream_exists")
        await waiter.wait()
    ```
