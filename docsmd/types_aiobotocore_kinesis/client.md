# KinesisClient

> [Index](../README.md) > [Kinesis](./README.md) > KinesisClient

!!! note ""

    Auto-generated documentation for [Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#kinesis)
    type annotations stubs module [types-aiobotocore-kinesis](https://pypi.org/project/types-aiobotocore-kinesis/).

## KinesisClient

Type annotations and code completion for `#!python session.create_client("kinesis")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client)

```python
# KinesisClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_kinesis.client import KinesisClient

session = get_session()
async with session.create_client("kinesis") as client:
    client: KinesisClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("kinesis").exceptions` structure.

```python
# KinesisClient.exceptions usage example

async with session.create_client("kinesis") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ExpiredIteratorException,
        client.ExpiredNextTokenException,
        client.InternalFailureException,
        client.InvalidArgumentException,
        client.KMSAccessDeniedException,
        client.KMSDisabledException,
        client.KMSInvalidStateException,
        client.KMSNotFoundException,
        client.KMSOptInRequired,
        client.KMSThrottlingException,
        client.LimitExceededException,
        client.ProvisionedThroughputExceededException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# KinesisClient usage type checking example

from types_aiobotocore_kinesis.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("kinesis").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("kinesis").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### add\_tags\_to\_stream

Adds or updates tags for the specified Kinesis data stream.

Type annotations and code completion for `#!python session.create_client("kinesis").add_tags_to_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/add_tags_to_stream.html)

```python
# add_tags_to_stream method definition

await def add_tags_to_stream(
    self,
    *,
    Tags: Mapping[str, str],
    StreamName: str = ...,
    StreamARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# add_tags_to_stream method usage example with argument unpacking

kwargs: AddTagsToStreamInputTypeDef = {  # (1)
    "Tags": ...,
}

parent.add_tags_to_stream(**kwargs)
```

1. See [:material-code-braces: AddTagsToStreamInputTypeDef](./type_defs.md#addtagstostreaminputtypedef) 

### create\_stream

Creates a Kinesis data stream.

Type annotations and code completion for `#!python session.create_client("kinesis").create_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/create_stream.html)

```python
# create_stream method definition

await def create_stream(
    self,
    *,
    StreamName: str,
    ShardCount: int = ...,
    StreamModeDetails: StreamModeDetailsTypeDef = ...,  # (1)
    Tags: Mapping[str, str] = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamModeDetailsTypeDef](./type_defs.md#streammodedetailstypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_stream method usage example with argument unpacking

kwargs: CreateStreamInputTypeDef = {  # (1)
    "StreamName": ...,
}

parent.create_stream(**kwargs)
```

1. See [:material-code-braces: CreateStreamInputTypeDef](./type_defs.md#createstreaminputtypedef) 

### decrease\_stream\_retention\_period

Decreases the Kinesis data stream's retention period, which is the length of
time data records are accessible after they are added to the stream.

Type annotations and code completion for `#!python session.create_client("kinesis").decrease_stream_retention_period` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/decrease_stream_retention_period.html)

```python
# decrease_stream_retention_period method definition

await def decrease_stream_retention_period(
    self,
    *,
    RetentionPeriodHours: int,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# decrease_stream_retention_period method usage example with argument unpacking

kwargs: DecreaseStreamRetentionPeriodInputTypeDef = {  # (1)
    "RetentionPeriodHours": ...,
}

parent.decrease_stream_retention_period(**kwargs)
```

1. See [:material-code-braces: DecreaseStreamRetentionPeriodInputTypeDef](./type_defs.md#decreasestreamretentionperiodinputtypedef) 

### delete\_resource\_policy

Delete a policy for the specified data stream or consumer.

Type annotations and code completion for `#!python session.create_client("kinesis").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/delete_resource_policy.html)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    ResourceARN: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyInputTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyInputTypeDef](./type_defs.md#deleteresourcepolicyinputtypedef) 

### delete\_stream

Deletes a Kinesis data stream and all its shards and data.

Type annotations and code completion for `#!python session.create_client("kinesis").delete_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/delete_stream.html)

```python
# delete_stream method definition

await def delete_stream(
    self,
    *,
    StreamName: str = ...,
    EnforceConsumerDeletion: bool = ...,
    StreamARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_stream method usage example with argument unpacking

kwargs: DeleteStreamInputTypeDef = {  # (1)
    "StreamName": ...,
}

parent.delete_stream(**kwargs)
```

1. See [:material-code-braces: DeleteStreamInputTypeDef](./type_defs.md#deletestreaminputtypedef) 

### deregister\_stream\_consumer

To deregister a consumer, provide its ARN.

Type annotations and code completion for `#!python session.create_client("kinesis").deregister_stream_consumer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/deregister_stream_consumer.html)

```python
# deregister_stream_consumer method definition

await def deregister_stream_consumer(
    self,
    *,
    StreamARN: str = ...,
    ConsumerName: str = ...,
    ConsumerARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deregister_stream_consumer method usage example with argument unpacking

kwargs: DeregisterStreamConsumerInputTypeDef = {  # (1)
    "StreamARN": ...,
}

parent.deregister_stream_consumer(**kwargs)
```

1. See [:material-code-braces: DeregisterStreamConsumerInputTypeDef](./type_defs.md#deregisterstreamconsumerinputtypedef) 

### describe\_limits

Describes the shard limits and usage for the account.

Type annotations and code completion for `#!python session.create_client("kinesis").describe_limits` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/describe_limits.html)

```python
# describe_limits method definition

await def describe_limits(
    self,
) -> DescribeLimitsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLimitsOutputTypeDef](./type_defs.md#describelimitsoutputtypedef) 

### describe\_stream

Describes the specified Kinesis data stream.

Type annotations and code completion for `#!python session.create_client("kinesis").describe_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/describe_stream.html)

```python
# describe_stream method definition

await def describe_stream(
    self,
    *,
    StreamName: str = ...,
    Limit: int = ...,
    ExclusiveStartShardId: str = ...,
    StreamARN: str = ...,
) -> DescribeStreamOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStreamOutputTypeDef](./type_defs.md#describestreamoutputtypedef) 


```python
# describe_stream method usage example with argument unpacking

kwargs: DescribeStreamInputTypeDef = {  # (1)
    "StreamName": ...,
}

parent.describe_stream(**kwargs)
```

1. See [:material-code-braces: DescribeStreamInputTypeDef](./type_defs.md#describestreaminputtypedef) 

### describe\_stream\_consumer

To get the description of a registered consumer, provide the ARN of the
consumer.

Type annotations and code completion for `#!python session.create_client("kinesis").describe_stream_consumer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/describe_stream_consumer.html)

```python
# describe_stream_consumer method definition

await def describe_stream_consumer(
    self,
    *,
    StreamARN: str = ...,
    ConsumerName: str = ...,
    ConsumerARN: str = ...,
) -> DescribeStreamConsumerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStreamConsumerOutputTypeDef](./type_defs.md#describestreamconsumeroutputtypedef) 


```python
# describe_stream_consumer method usage example with argument unpacking

kwargs: DescribeStreamConsumerInputTypeDef = {  # (1)
    "StreamARN": ...,
}

parent.describe_stream_consumer(**kwargs)
```

1. See [:material-code-braces: DescribeStreamConsumerInputTypeDef](./type_defs.md#describestreamconsumerinputtypedef) 

### describe\_stream\_summary

Provides a summarized description of the specified Kinesis data stream without
the shard list.

Type annotations and code completion for `#!python session.create_client("kinesis").describe_stream_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/describe_stream_summary.html)

```python
# describe_stream_summary method definition

await def describe_stream_summary(
    self,
    *,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> DescribeStreamSummaryOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStreamSummaryOutputTypeDef](./type_defs.md#describestreamsummaryoutputtypedef) 


```python
# describe_stream_summary method usage example with argument unpacking

kwargs: DescribeStreamSummaryInputTypeDef = {  # (1)
    "StreamName": ...,
}

parent.describe_stream_summary(**kwargs)
```

1. See [:material-code-braces: DescribeStreamSummaryInputTypeDef](./type_defs.md#describestreamsummaryinputtypedef) 

### disable\_enhanced\_monitoring

Disables enhanced monitoring.

Type annotations and code completion for `#!python session.create_client("kinesis").disable_enhanced_monitoring` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/disable_enhanced_monitoring.html)

```python
# disable_enhanced_monitoring method definition

await def disable_enhanced_monitoring(
    self,
    *,
    ShardLevelMetrics: Sequence[MetricsNameType],  # (1)
    StreamName: str = ...,
    StreamARN: str = ...,
) -> EnhancedMonitoringOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MetricsNameType](./literals.md#metricsnametype) 
2. See [:material-code-braces: EnhancedMonitoringOutputTypeDef](./type_defs.md#enhancedmonitoringoutputtypedef) 


```python
# disable_enhanced_monitoring method usage example with argument unpacking

kwargs: DisableEnhancedMonitoringInputTypeDef = {  # (1)
    "ShardLevelMetrics": ...,
}

parent.disable_enhanced_monitoring(**kwargs)
```

1. See [:material-code-braces: DisableEnhancedMonitoringInputTypeDef](./type_defs.md#disableenhancedmonitoringinputtypedef) 

### enable\_enhanced\_monitoring

Enables enhanced Kinesis data stream monitoring for shard-level metrics.

Type annotations and code completion for `#!python session.create_client("kinesis").enable_enhanced_monitoring` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/enable_enhanced_monitoring.html)

```python
# enable_enhanced_monitoring method definition

await def enable_enhanced_monitoring(
    self,
    *,
    ShardLevelMetrics: Sequence[MetricsNameType],  # (1)
    StreamName: str = ...,
    StreamARN: str = ...,
) -> EnhancedMonitoringOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MetricsNameType](./literals.md#metricsnametype) 
2. See [:material-code-braces: EnhancedMonitoringOutputTypeDef](./type_defs.md#enhancedmonitoringoutputtypedef) 


```python
# enable_enhanced_monitoring method usage example with argument unpacking

kwargs: EnableEnhancedMonitoringInputTypeDef = {  # (1)
    "ShardLevelMetrics": ...,
}

parent.enable_enhanced_monitoring(**kwargs)
```

1. See [:material-code-braces: EnableEnhancedMonitoringInputTypeDef](./type_defs.md#enableenhancedmonitoringinputtypedef) 

### get\_records

Gets data records from a Kinesis data stream's shard.

Type annotations and code completion for `#!python session.create_client("kinesis").get_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/get_records.html)

```python
# get_records method definition

await def get_records(
    self,
    *,
    ShardIterator: str,
    Limit: int = ...,
    StreamARN: str = ...,
) -> GetRecordsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRecordsOutputTypeDef](./type_defs.md#getrecordsoutputtypedef) 


```python
# get_records method usage example with argument unpacking

kwargs: GetRecordsInputTypeDef = {  # (1)
    "ShardIterator": ...,
}

parent.get_records(**kwargs)
```

1. See [:material-code-braces: GetRecordsInputTypeDef](./type_defs.md#getrecordsinputtypedef) 

### get\_resource\_policy

Returns a policy attached to the specified data stream or consumer.

Type annotations and code completion for `#!python session.create_client("kinesis").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/get_resource_policy.html)

```python
# get_resource_policy method definition

await def get_resource_policy(
    self,
    *,
    ResourceARN: str,
) -> GetResourcePolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePolicyOutputTypeDef](./type_defs.md#getresourcepolicyoutputtypedef) 


```python
# get_resource_policy method usage example with argument unpacking

kwargs: GetResourcePolicyInputTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.get_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetResourcePolicyInputTypeDef](./type_defs.md#getresourcepolicyinputtypedef) 

### get\_shard\_iterator

Gets an Amazon Kinesis shard iterator.

Type annotations and code completion for `#!python session.create_client("kinesis").get_shard_iterator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/get_shard_iterator.html)

```python
# get_shard_iterator method definition

await def get_shard_iterator(
    self,
    *,
    ShardId: str,
    ShardIteratorType: ShardIteratorTypeType,  # (1)
    StreamName: str = ...,
    StartingSequenceNumber: str = ...,
    Timestamp: TimestampTypeDef = ...,
    StreamARN: str = ...,
) -> GetShardIteratorOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ShardIteratorTypeType](./literals.md#sharditeratortypetype) 
2. See [:material-code-braces: GetShardIteratorOutputTypeDef](./type_defs.md#getsharditeratoroutputtypedef) 


```python
# get_shard_iterator method usage example with argument unpacking

kwargs: GetShardIteratorInputTypeDef = {  # (1)
    "ShardId": ...,
    "ShardIteratorType": ...,
}

parent.get_shard_iterator(**kwargs)
```

1. See [:material-code-braces: GetShardIteratorInputTypeDef](./type_defs.md#getsharditeratorinputtypedef) 

### increase\_stream\_retention\_period

Increases the Kinesis data stream's retention period, which is the length of
time data records are accessible after they are added to the stream.

Type annotations and code completion for `#!python session.create_client("kinesis").increase_stream_retention_period` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/increase_stream_retention_period.html)

```python
# increase_stream_retention_period method definition

await def increase_stream_retention_period(
    self,
    *,
    RetentionPeriodHours: int,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# increase_stream_retention_period method usage example with argument unpacking

kwargs: IncreaseStreamRetentionPeriodInputTypeDef = {  # (1)
    "RetentionPeriodHours": ...,
}

parent.increase_stream_retention_period(**kwargs)
```

1. See [:material-code-braces: IncreaseStreamRetentionPeriodInputTypeDef](./type_defs.md#increasestreamretentionperiodinputtypedef) 

### list\_shards

Lists the shards in a stream and provides information about each shard.

Type annotations and code completion for `#!python session.create_client("kinesis").list_shards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/list_shards.html)

```python
# list_shards method definition

await def list_shards(
    self,
    *,
    StreamName: str = ...,
    NextToken: str = ...,
    ExclusiveStartShardId: str = ...,
    MaxResults: int = ...,
    StreamCreationTimestamp: TimestampTypeDef = ...,
    ShardFilter: ShardFilterTypeDef = ...,  # (1)
    StreamARN: str = ...,
) -> ListShardsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ShardFilterTypeDef](./type_defs.md#shardfiltertypedef) 
2. See [:material-code-braces: ListShardsOutputTypeDef](./type_defs.md#listshardsoutputtypedef) 


```python
# list_shards method usage example with argument unpacking

kwargs: ListShardsInputTypeDef = {  # (1)
    "StreamName": ...,
}

parent.list_shards(**kwargs)
```

1. See [:material-code-braces: ListShardsInputTypeDef](./type_defs.md#listshardsinputtypedef) 

### list\_stream\_consumers

Lists the consumers registered to receive data from a stream using enhanced
fan-out, and provides information about each consumer.

Type annotations and code completion for `#!python session.create_client("kinesis").list_stream_consumers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/list_stream_consumers.html)

```python
# list_stream_consumers method definition

await def list_stream_consumers(
    self,
    *,
    StreamARN: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    StreamCreationTimestamp: TimestampTypeDef = ...,
) -> ListStreamConsumersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStreamConsumersOutputTypeDef](./type_defs.md#liststreamconsumersoutputtypedef) 


```python
# list_stream_consumers method usage example with argument unpacking

kwargs: ListStreamConsumersInputTypeDef = {  # (1)
    "StreamARN": ...,
}

parent.list_stream_consumers(**kwargs)
```

1. See [:material-code-braces: ListStreamConsumersInputTypeDef](./type_defs.md#liststreamconsumersinputtypedef) 

### list\_streams

Lists your Kinesis data streams.

Type annotations and code completion for `#!python session.create_client("kinesis").list_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/list_streams.html)

```python
# list_streams method definition

await def list_streams(
    self,
    *,
    Limit: int = ...,
    ExclusiveStartStreamName: str = ...,
    NextToken: str = ...,
) -> ListStreamsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStreamsOutputTypeDef](./type_defs.md#liststreamsoutputtypedef) 


```python
# list_streams method usage example with argument unpacking

kwargs: ListStreamsInputTypeDef = {  # (1)
    "Limit": ...,
}

parent.list_streams(**kwargs)
```

1. See [:material-code-braces: ListStreamsInputTypeDef](./type_defs.md#liststreamsinputtypedef) 

### list\_tags\_for\_stream

Lists the tags for the specified Kinesis data stream.

Type annotations and code completion for `#!python session.create_client("kinesis").list_tags_for_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/list_tags_for_stream.html)

```python
# list_tags_for_stream method definition

await def list_tags_for_stream(
    self,
    *,
    StreamName: str = ...,
    ExclusiveStartTagKey: str = ...,
    Limit: int = ...,
    StreamARN: str = ...,
) -> ListTagsForStreamOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForStreamOutputTypeDef](./type_defs.md#listtagsforstreamoutputtypedef) 


```python
# list_tags_for_stream method usage example with argument unpacking

kwargs: ListTagsForStreamInputTypeDef = {  # (1)
    "StreamName": ...,
}

parent.list_tags_for_stream(**kwargs)
```

1. See [:material-code-braces: ListTagsForStreamInputTypeDef](./type_defs.md#listtagsforstreaminputtypedef) 

### merge\_shards

Merges two adjacent shards in a Kinesis data stream and combines them into a
single shard to reduce the stream's capacity to ingest and transport data.

Type annotations and code completion for `#!python session.create_client("kinesis").merge_shards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/merge_shards.html)

```python
# merge_shards method definition

await def merge_shards(
    self,
    *,
    ShardToMerge: str,
    AdjacentShardToMerge: str,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# merge_shards method usage example with argument unpacking

kwargs: MergeShardsInputTypeDef = {  # (1)
    "ShardToMerge": ...,
    "AdjacentShardToMerge": ...,
}

parent.merge_shards(**kwargs)
```

1. See [:material-code-braces: MergeShardsInputTypeDef](./type_defs.md#mergeshardsinputtypedef) 

### put\_record

Writes a single data record into an Amazon Kinesis data stream.

Type annotations and code completion for `#!python session.create_client("kinesis").put_record` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/put_record.html)

```python
# put_record method definition

await def put_record(
    self,
    *,
    Data: BlobTypeDef,
    PartitionKey: str,
    StreamName: str = ...,
    ExplicitHashKey: str = ...,
    SequenceNumberForOrdering: str = ...,
    StreamARN: str = ...,
) -> PutRecordOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutRecordOutputTypeDef](./type_defs.md#putrecordoutputtypedef) 


```python
# put_record method usage example with argument unpacking

kwargs: PutRecordInputTypeDef = {  # (1)
    "Data": ...,
    "PartitionKey": ...,
}

parent.put_record(**kwargs)
```

1. See [:material-code-braces: PutRecordInputTypeDef](./type_defs.md#putrecordinputtypedef) 

### put\_records

Writes multiple data records into a Kinesis data stream in a single call (also
referred to as a <code>PutRecords</code> request).

Type annotations and code completion for `#!python session.create_client("kinesis").put_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/put_records.html)

```python
# put_records method definition

await def put_records(
    self,
    *,
    Records: Sequence[PutRecordsRequestEntryTypeDef],  # (1)
    StreamName: str = ...,
    StreamARN: str = ...,
) -> PutRecordsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PutRecordsRequestEntryTypeDef](./type_defs.md#putrecordsrequestentrytypedef) 
2. See [:material-code-braces: PutRecordsOutputTypeDef](./type_defs.md#putrecordsoutputtypedef) 


```python
# put_records method usage example with argument unpacking

kwargs: PutRecordsInputTypeDef = {  # (1)
    "Records": ...,
}

parent.put_records(**kwargs)
```

1. See [:material-code-braces: PutRecordsInputTypeDef](./type_defs.md#putrecordsinputtypedef) 

### put\_resource\_policy

Attaches a resource-based policy to a data stream or registered consumer.

Type annotations and code completion for `#!python session.create_client("kinesis").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/put_resource_policy.html)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    ResourceARN: str,
    Policy: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyInputTypeDef = {  # (1)
    "ResourceARN": ...,
    "Policy": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyInputTypeDef](./type_defs.md#putresourcepolicyinputtypedef) 

### register\_stream\_consumer

Registers a consumer with a Kinesis data stream.

Type annotations and code completion for `#!python session.create_client("kinesis").register_stream_consumer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/register_stream_consumer.html)

```python
# register_stream_consumer method definition

await def register_stream_consumer(
    self,
    *,
    StreamARN: str,
    ConsumerName: str,
) -> RegisterStreamConsumerOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterStreamConsumerOutputTypeDef](./type_defs.md#registerstreamconsumeroutputtypedef) 


```python
# register_stream_consumer method usage example with argument unpacking

kwargs: RegisterStreamConsumerInputTypeDef = {  # (1)
    "StreamARN": ...,
    "ConsumerName": ...,
}

parent.register_stream_consumer(**kwargs)
```

1. See [:material-code-braces: RegisterStreamConsumerInputTypeDef](./type_defs.md#registerstreamconsumerinputtypedef) 

### remove\_tags\_from\_stream

Removes tags from the specified Kinesis data stream.

Type annotations and code completion for `#!python session.create_client("kinesis").remove_tags_from_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/remove_tags_from_stream.html)

```python
# remove_tags_from_stream method definition

await def remove_tags_from_stream(
    self,
    *,
    TagKeys: Sequence[str],
    StreamName: str = ...,
    StreamARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# remove_tags_from_stream method usage example with argument unpacking

kwargs: RemoveTagsFromStreamInputTypeDef = {  # (1)
    "TagKeys": ...,
}

parent.remove_tags_from_stream(**kwargs)
```

1. See [:material-code-braces: RemoveTagsFromStreamInputTypeDef](./type_defs.md#removetagsfromstreaminputtypedef) 

### split\_shard

Splits a shard into two new shards in the Kinesis data stream, to increase the
stream's capacity to ingest and transport data.

Type annotations and code completion for `#!python session.create_client("kinesis").split_shard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/split_shard.html)

```python
# split_shard method definition

await def split_shard(
    self,
    *,
    ShardToSplit: str,
    NewStartingHashKey: str,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# split_shard method usage example with argument unpacking

kwargs: SplitShardInputTypeDef = {  # (1)
    "ShardToSplit": ...,
    "NewStartingHashKey": ...,
}

parent.split_shard(**kwargs)
```

1. See [:material-code-braces: SplitShardInputTypeDef](./type_defs.md#splitshardinputtypedef) 

### start\_stream\_encryption

Enables or updates server-side encryption using an Amazon Web Services KMS key
for a specified stream.

Type annotations and code completion for `#!python session.create_client("kinesis").start_stream_encryption` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/start_stream_encryption.html)

```python
# start_stream_encryption method definition

await def start_stream_encryption(
    self,
    *,
    EncryptionType: EncryptionTypeType,  # (1)
    KeyId: str,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_stream_encryption method usage example with argument unpacking

kwargs: StartStreamEncryptionInputTypeDef = {  # (1)
    "EncryptionType": ...,
    "KeyId": ...,
}

parent.start_stream_encryption(**kwargs)
```

1. See [:material-code-braces: StartStreamEncryptionInputTypeDef](./type_defs.md#startstreamencryptioninputtypedef) 

### stop\_stream\_encryption

Disables server-side encryption for a specified stream.

Type annotations and code completion for `#!python session.create_client("kinesis").stop_stream_encryption` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/stop_stream_encryption.html)

```python
# stop_stream_encryption method definition

await def stop_stream_encryption(
    self,
    *,
    EncryptionType: EncryptionTypeType,  # (1)
    KeyId: str,
    StreamName: str = ...,
    StreamARN: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_stream_encryption method usage example with argument unpacking

kwargs: StopStreamEncryptionInputTypeDef = {  # (1)
    "EncryptionType": ...,
    "KeyId": ...,
}

parent.stop_stream_encryption(**kwargs)
```

1. See [:material-code-braces: StopStreamEncryptionInputTypeDef](./type_defs.md#stopstreamencryptioninputtypedef) 

### subscribe\_to\_shard

This operation establishes an HTTP/2 connection between the consumer you
specify in the <code>ConsumerARN</code> parameter and the shard you specify in
the <code>ShardId</code> parameter.

Type annotations and code completion for `#!python session.create_client("kinesis").subscribe_to_shard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/subscribe_to_shard.html)

```python
# subscribe_to_shard method definition

await def subscribe_to_shard(
    self,
    *,
    ConsumerARN: str,
    ShardId: str,
    StartingPosition: StartingPositionTypeDef,  # (1)
) -> SubscribeToShardOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StartingPositionTypeDef](./type_defs.md#startingpositiontypedef) 
2. See [:material-code-braces: SubscribeToShardOutputTypeDef](./type_defs.md#subscribetoshardoutputtypedef) 


```python
# subscribe_to_shard method usage example with argument unpacking

kwargs: SubscribeToShardInputTypeDef = {  # (1)
    "ConsumerARN": ...,
    "ShardId": ...,
    "StartingPosition": ...,
}

parent.subscribe_to_shard(**kwargs)
```

1. See [:material-code-braces: SubscribeToShardInputTypeDef](./type_defs.md#subscribetoshardinputtypedef) 

### update\_shard\_count

Updates the shard count of the specified stream to the specified number of
shards.

Type annotations and code completion for `#!python session.create_client("kinesis").update_shard_count` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/update_shard_count.html)

```python
# update_shard_count method definition

await def update_shard_count(
    self,
    *,
    TargetShardCount: int,
    ScalingType: ScalingTypeType,  # (1)
    StreamName: str = ...,
    StreamARN: str = ...,
) -> UpdateShardCountOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScalingTypeType](./literals.md#scalingtypetype) 
2. See [:material-code-braces: UpdateShardCountOutputTypeDef](./type_defs.md#updateshardcountoutputtypedef) 


```python
# update_shard_count method usage example with argument unpacking

kwargs: UpdateShardCountInputTypeDef = {  # (1)
    "TargetShardCount": ...,
    "ScalingType": ...,
}

parent.update_shard_count(**kwargs)
```

1. See [:material-code-braces: UpdateShardCountInputTypeDef](./type_defs.md#updateshardcountinputtypedef) 

### update\_stream\_mode

Updates the capacity mode of the data stream.

Type annotations and code completion for `#!python session.create_client("kinesis").update_stream_mode` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis/client/update_stream_mode.html)

```python
# update_stream_mode method definition

await def update_stream_mode(
    self,
    *,
    StreamARN: str,
    StreamModeDetails: StreamModeDetailsTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamModeDetailsTypeDef](./type_defs.md#streammodedetailstypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_stream_mode method usage example with argument unpacking

kwargs: UpdateStreamModeInputTypeDef = {  # (1)
    "StreamARN": ...,
    "StreamModeDetails": ...,
}

parent.update_stream_mode(**kwargs)
```

1. See [:material-code-braces: UpdateStreamModeInputTypeDef](./type_defs.md#updatestreammodeinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("kinesis").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("kinesis").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("kinesis").get_paginator` method with overloads.

- `client.get_paginator("describe_stream")` -> [DescribeStreamPaginator](./paginators.md#describestreampaginator)
- `client.get_paginator("list_shards")` -> [ListShardsPaginator](./paginators.md#listshardspaginator)
- `client.get_paginator("list_stream_consumers")` -> [ListStreamConsumersPaginator](./paginators.md#liststreamconsumerspaginator)
- `client.get_paginator("list_streams")` -> [ListStreamsPaginator](./paginators.md#liststreamspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("kinesis").get_waiter` method with overloads.

- `client.get_waiter("stream_exists")` -> [StreamExistsWaiter](./waiters.md#streamexistswaiter)
- `client.get_waiter("stream_not_exists")` -> [StreamNotExistsWaiter](./waiters.md#streamnotexistswaiter)

