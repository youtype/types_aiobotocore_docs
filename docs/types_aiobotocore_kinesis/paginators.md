<a id="paginators-for-aiobotocore-kinesis-module"></a>

# Paginators for aiobotocore Kinesis module

> [Index](../README.md) > [Kinesis](./README.md) > Paginators

Auto-generated documentation for
[Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
type annotations stubs module
[types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

- [Paginators for aiobotocore Kinesis module](#paginators-for-aiobotocore-kinesis-module)
  - [DescribeStreamPaginator](#describestreampaginator)
  - [ListShardsPaginator](#listshardspaginator)
  - [ListStreamConsumersPaginator](#liststreamconsumerspaginator)
  - [ListStreamsPaginator](#liststreamspaginator)

<a id="describestreampaginator"></a>

## DescribeStreamPaginator

Type annotations for
`session.create_client("kinesis").get_paginator("describe_stream")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesis.paginator import DescribeStreamPaginator

session = get_session()
async with session.create_client("kinesis") as client:
    client: KinesisClient
    paginator: DescribeStreamPaginator = client.get_paginator("describe_stream")
```

Boto3 documentation:
[Kinesis.Paginator.DescribeStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.DescribeStream)

Arguments for `DescribeStreamPaginator.paginate` method:

- `StreamName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeStreamPaginator.paginate` returns
`AsyncIterator`\[[DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef)\].

<a id="listshardspaginator"></a>

## ListShardsPaginator

Type annotations for
`session.create_client("kinesis").get_paginator("list_shards")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesis.paginator import ListShardsPaginator

session = get_session()
async with session.create_client("kinesis") as client:
    client: KinesisClient
    paginator: ListShardsPaginator = client.get_paginator("list_shards")
```

Boto3 documentation:
[Kinesis.Paginator.ListShards](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListShards)

Arguments for `ListShardsPaginator.paginate` method:

- `StreamName`: `str`
- `ExclusiveStartShardId`: `str`
- `StreamCreationTimestamp`: `Union`\[`datetime`, `str`\]
- `ShardFilter`: [ShardFilterTypeDef](./type_defs.md#shardfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListShardsPaginator.paginate` returns
`AsyncIterator`\[[ListShardsOutputTypeDef](./type_defs.md#listshardsoutputtypedef)\].

<a id="liststreamconsumerspaginator"></a>

## ListStreamConsumersPaginator

Type annotations for
`session.create_client("kinesis").get_paginator("list_stream_consumers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesis.paginator import ListStreamConsumersPaginator

session = get_session()
async with session.create_client("kinesis") as client:
    client: KinesisClient
    paginator: ListStreamConsumersPaginator = client.get_paginator("list_stream_consumers")
```

Boto3 documentation:
[Kinesis.Paginator.ListStreamConsumers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreamConsumers)

Arguments for `ListStreamConsumersPaginator.paginate` method:

- `StreamARN`: `str` *(required)*
- `StreamCreationTimestamp`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStreamConsumersPaginator.paginate` returns
`AsyncIterator`\[[ListStreamConsumersOutputTypeDef](./type_defs.md#liststreamconsumersoutputtypedef)\].

<a id="liststreamspaginator"></a>

## ListStreamsPaginator

Type annotations for
`session.create_client("kinesis").get_paginator("list_streams")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesis.paginator import ListStreamsPaginator

session = get_session()
async with session.create_client("kinesis") as client:
    client: KinesisClient
    paginator: ListStreamsPaginator = client.get_paginator("list_streams")
```

Boto3 documentation:
[Kinesis.Paginator.ListStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreams)

Arguments for `ListStreamsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStreamsPaginator.paginate` returns
`AsyncIterator`\[[ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef)\].
