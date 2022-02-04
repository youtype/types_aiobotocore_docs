<a id="dynamodbstreamsclient-for-aiobotocore-dynamodbstreams-module"></a>

# DynamoDBStreamsClient for aiobotocore DynamoDBStreams module

> [Index](..) > [DynamoDBStreams](.) > DynamoDBStreamsClient

Auto-generated documentation for
[DynamoDBStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
type annotations stubs module
[types-aiobotocore-dynamodbstreams](https://pypi.org/project/types-aiobotocore-dynamodbstreams/).

- [DynamoDBStreamsClient for aiobotocore DynamoDBStreams module](#dynamodbstreamsclient-for-aiobotocore-dynamodbstreams-module)
  - [DynamoDBStreamsClient](#dynamodbstreamsclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [describe_stream](#describe_stream)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_records](#get_records)
    - [get_shard_iterator](#get_shard_iterator)
    - [list_streams](#list_streams)

<a id="dynamodbstreamsclient"></a>

## DynamoDBStreamsClient

Type annotations for `aiobotocore.create_client("dynamodbstreams")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_dynamodbstreams.client import DynamoDBStreamsClient

def get_dynamodbstreams_client() -> DynamoDBStreamsClient:
    return Session().client("dynamodbstreams")
```

Boto3 documentation:
[DynamoDBStreams.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_dynamodbstreams.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ExpiredIteratorException`
- `Exceptions.InternalServerError`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.TrimmedDataAccessException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

DynamoDBStreamsClient exceptions.

Type annotations for `aiobotocore.create_client("dynamodbstreams").exceptions`
method.

Boto3 documentation:
[DynamoDBStreams.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`aiobotocore.create_client("dynamodbstreams").can_paginate` method.

Boto3 documentation:
[DynamoDBStreams.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="describe_stream"></a>

### describe_stream

Returns information about a stream, including the current status of the stream,
its Amazon Resource Name (ARN), the composition of its shards, and its
corresponding DynamoDB table.

Type annotations for
`aiobotocore.create_client("dynamodbstreams").describe_stream` method.

Boto3 documentation:
[DynamoDBStreams.Client.describe_stream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client.describe_stream)

Asynchronous method. Use `await describe_stream(...)` for a synchronous call.

Arguments mapping described in
[DescribeStreamInputRequestTypeDef](./type_defs.md#describestreaminputrequesttypedef).

Keyword-only arguments:

- `StreamArn`: `str` *(required)*
- `Limit`: `int`
- `ExclusiveStartShardId`: `str`

Returns a `Coroutine` for
[DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("dynamodbstreams").generate_presigned_url` method.

Boto3 documentation:
[DynamoDBStreams.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_records"></a>

### get_records

Retrieves the stream records from a given shard.

Type annotations for `aiobotocore.create_client("dynamodbstreams").get_records`
method.

Boto3 documentation:
[DynamoDBStreams.Client.get_records](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client.get_records)

Asynchronous method. Use `await get_records(...)` for a synchronous call.

Arguments mapping described in
[GetRecordsInputRequestTypeDef](./type_defs.md#getrecordsinputrequesttypedef).

Keyword-only arguments:

- `ShardIterator`: `str` *(required)*
- `Limit`: `int`

Returns a `Coroutine` for
[GetRecordsOutputTypeDef](./type_defs.md#getrecordsoutputtypedef).

<a id="get_shard_iterator"></a>

### get_shard_iterator

Returns a shard iterator.

Type annotations for
`aiobotocore.create_client("dynamodbstreams").get_shard_iterator` method.

Boto3 documentation:
[DynamoDBStreams.Client.get_shard_iterator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client.get_shard_iterator)

Asynchronous method. Use `await get_shard_iterator(...)` for a synchronous
call.

Arguments mapping described in
[GetShardIteratorInputRequestTypeDef](./type_defs.md#getsharditeratorinputrequesttypedef).

Keyword-only arguments:

- `StreamArn`: `str` *(required)*
- `ShardId`: `str` *(required)*
- `ShardIteratorType`:
  [ShardIteratorTypeType](./literals.md#sharditeratortypetype) *(required)*
- `SequenceNumber`: `str`

Returns a `Coroutine` for
[GetShardIteratorOutputTypeDef](./type_defs.md#getsharditeratoroutputtypedef).

<a id="list_streams"></a>

### list_streams

Returns an array of stream ARNs associated with the current account and
endpoint.

Type annotations for
`aiobotocore.create_client("dynamodbstreams").list_streams` method.

Boto3 documentation:
[DynamoDBStreams.Client.list_streams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client.list_streams)

Asynchronous method. Use `await list_streams(...)` for a synchronous call.

Arguments mapping described in
[ListStreamsInputRequestTypeDef](./type_defs.md#liststreamsinputrequesttypedef).

Keyword-only arguments:

- `TableName`: `str`
- `Limit`: `int`
- `ExclusiveStartStreamArn`: `str`

Returns a `Coroutine` for
[ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef).
