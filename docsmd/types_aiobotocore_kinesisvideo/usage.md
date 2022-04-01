# Examples

> [Index](../README.md) > [KinesisVideo](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
    type annotations stubs module [types-aiobotocore-kinesisvideo](https://pypi.org/project/types-aiobotocore-kinesisvideo/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kinesisvideo]` package installed.

Write your `KinesisVideo` code as usual,
type checking and code completion should work out of the box.



=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("kinesisvideo") as client:  # (1)
        result = await client.create_signaling_channel()  # (2)
    ```

    1. client: [KinesisVideoClient](./client.md)
    2. result: [:material-code-braces: CreateSignalingChannelOutputTypeDef](./type_defs.md#createsignalingchanneloutputtypedef) 



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session


    session = get_session()

    async with session.create_client("kinesisvideo") as client:  # (1)
        paginator = client.get_paginator("list_signaling_channels")  # (2)
        async for item in paginator.paginate(...):
            print(item)  # (3)
    ```

    1. client: [KinesisVideoClient](./client.md)
    2. paginator: [ListSignalingChannelsPaginator](./paginators.md#listsignalingchannelspaginator)
    3. item: [:material-code-braces: ListSignalingChannelsOutputTypeDef](./type_defs.md#listsignalingchannelsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[kinesisvideo]`
or a standalone `types_aiobotocore_kinesisvideo` package, you have to explicitly specify
`client: KinesisVideoClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


=== "Client"

    ```python title="Client usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_kinesisvideo.client import KinesisVideoClient
    from types_aiobotocore_kinesisvideo.type_defs import CreateSignalingChannelOutputTypeDef
    from types_aiobotocore_kinesisvideo.type_defs import CreateSignalingChannelInputRequestTypeDef


    session = get_session()

    async with session.create_client("kinesisvideo") as client:
        client: KinesisVideoClient
        kwargs: CreateSignalingChannelInputRequestTypeDef = {...}
        result: CreateSignalingChannelOutputTypeDef = await client.create_signaling_channel(**kwargs)
    ```



=== "Paginators"

    ```python title="Paginator usage example"
    from aiobotocore.session import get_session

    from types_aiobotocore_kinesisvideo.client import KinesisVideoClient
    from types_aiobotocore_kinesisvideo.paginator import ListSignalingChannelsPaginator
    from types_aiobotocore_kinesisvideo.type_defs import ListSignalingChannelsOutputTypeDef


    session = get_session()

    async with session.create_client("kinesisvideo") as client:
        client: KinesisVideoClient
        paginator: ListSignalingChannelsPaginator = client.get_paginator("list_signaling_channels")
        async for item in paginator.paginate(...):
            item: ListSignalingChannelsOutputTypeDef
            print(item)
    ```


