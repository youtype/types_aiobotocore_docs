# Paginators

> [Index](../README.md) > [Kinesis](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#kinesis)
    type annotations stubs module [types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

## DescribeStreamPaginator

Type annotations and code completion for `#!python session.create_client("kinesis").get_paginator("describe_stream")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/paginator/DescribeStream.html#Kinesis.Paginator.DescribeStream)

```python
# DescribeStreamPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesis.paginator import DescribeStreamPaginator

session = get_session()
async with session.create_client("kinesis") as client:  # (1)
    paginator: DescribeStreamPaginator = client.get_paginator("describe_stream")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStreamOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisClient](./client.md)
2. paginator: [DescribeStreamPaginator](./paginators.md#describestreampaginator)
3. item: [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeStreamPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeStreamOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeStreamInputPaginateTypeDef = {  # (1)
    "StreamName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStreamInputPaginateTypeDef](./type_defs.md#describestreaminputpaginatetypedef) 
## ListShardsPaginator

Type annotations and code completion for `#!python session.create_client("kinesis").get_paginator("list_shards")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/paginator/ListShards.html#Kinesis.Paginator.ListShards)

```python
# ListShardsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesis.paginator import ListShardsPaginator

session = get_session()
async with session.create_client("kinesis") as client:  # (1)
    paginator: ListShardsPaginator = client.get_paginator("list_shards")  # (2)
    async for item in paginator.paginate(...):
        item: ListShardsOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisClient](./client.md)
2. paginator: [ListShardsPaginator](./paginators.md#listshardspaginator)
3. item: [:material-code-braces: ListShardsOutputTypeDef](./type_defs.md#listshardsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListShardsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StreamName: str = ...,
    ExclusiveStartShardId: str = ...,
    StreamCreationTimestamp: TimestampTypeDef = ...,
    ShardFilter: ShardFilterTypeDef = ...,  # (1)
    StreamARN: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListShardsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ShardFilterTypeDef](./type_defs.md#shardfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListShardsOutputTypeDef](./type_defs.md#listshardsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListShardsInputPaginateTypeDef = {  # (1)
    "StreamName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListShardsInputPaginateTypeDef](./type_defs.md#listshardsinputpaginatetypedef) 
## ListStreamConsumersPaginator

Type annotations and code completion for `#!python session.create_client("kinesis").get_paginator("list_stream_consumers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/paginator/ListStreamConsumers.html#Kinesis.Paginator.ListStreamConsumers)

```python
# ListStreamConsumersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesis.paginator import ListStreamConsumersPaginator

session = get_session()
async with session.create_client("kinesis") as client:  # (1)
    paginator: ListStreamConsumersPaginator = client.get_paginator("list_stream_consumers")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamConsumersOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisClient](./client.md)
2. paginator: [ListStreamConsumersPaginator](./paginators.md#liststreamconsumerspaginator)
3. item: [:material-code-braces: ListStreamConsumersOutputTypeDef](./type_defs.md#liststreamconsumersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStreamConsumersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StreamARN: str,
    StreamCreationTimestamp: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListStreamConsumersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStreamConsumersOutputTypeDef](./type_defs.md#liststreamconsumersoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamConsumersInputPaginateTypeDef = {  # (1)
    "StreamARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamConsumersInputPaginateTypeDef](./type_defs.md#liststreamconsumersinputpaginatetypedef) 
## ListStreamsPaginator

Type annotations and code completion for `#!python session.create_client("kinesis").get_paginator("list_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/paginator/ListStreams.html#Kinesis.Paginator.ListStreams)

```python
# ListStreamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kinesis.paginator import ListStreamsPaginator

session = get_session()
async with session.create_client("kinesis") as client:  # (1)
    paginator: ListStreamsPaginator = client.get_paginator("list_streams")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamsOutputTypeDef
        print(item)  # (3)
```

1. client: [KinesisClient](./client.md)
2. paginator: [ListStreamsPaginator](./paginators.md#liststreamspaginator)
3. item: [:material-code-braces: ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStreamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ExclusiveStartStreamName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListStreamsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamsInputPaginateTypeDef = {  # (1)
    "ExclusiveStartStreamName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamsInputPaginateTypeDef](./type_defs.md#liststreamsinputpaginatetypedef) 
