# FirehoseClient

> [Index](../README.md) > [Firehose](./README.md) > FirehoseClient

!!! note ""

    Auto-generated documentation for [Firehose](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#firehose)
    type annotations stubs module [types-aiobotocore-firehose](https://pypi.org/project/types-aiobotocore-firehose/).

## FirehoseClient

Type annotations and code completion for `#!python session.create_client("firehose")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client)

```python
# FirehoseClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_firehose.client import FirehoseClient

session = get_session()
async with session.create_client("firehose") as client:
    client: FirehoseClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("firehose").exceptions` structure.

```python
# FirehoseClient.exceptions usage example

async with session.create_client("firehose") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConcurrentModificationException,
        client.InvalidArgumentException,
        client.InvalidKMSResourceException,
        client.InvalidSourceException,
        client.LimitExceededException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
    ) as e:
        print(e)
```

```python
# FirehoseClient usage type checking example

from types_aiobotocore_firehose.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("firehose").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("firehose").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/generate_presigned_url.html)

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


### create\_delivery\_stream

Creates a Firehose stream.

Type annotations and code completion for `#!python session.create_client("firehose").create_delivery_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/create_delivery_stream.html)

```python
# create_delivery_stream method definition

await def create_delivery_stream(
    self,
    *,
    DeliveryStreamName: str,
    DeliveryStreamType: DeliveryStreamTypeType = ...,  # (1)
    KinesisStreamSourceConfiguration: KinesisStreamSourceConfigurationTypeDef = ...,  # (2)
    DeliveryStreamEncryptionConfigurationInput: DeliveryStreamEncryptionConfigurationInputTypeDef = ...,  # (3)
    S3DestinationConfiguration: S3DestinationConfigurationTypeDef = ...,  # (4)
    ExtendedS3DestinationConfiguration: ExtendedS3DestinationConfigurationTypeDef = ...,  # (5)
    RedshiftDestinationConfiguration: RedshiftDestinationConfigurationTypeDef = ...,  # (6)
    ElasticsearchDestinationConfiguration: ElasticsearchDestinationConfigurationTypeDef = ...,  # (7)
    AmazonopensearchserviceDestinationConfiguration: AmazonopensearchserviceDestinationConfigurationTypeDef = ...,  # (8)
    SplunkDestinationConfiguration: SplunkDestinationConfigurationTypeDef = ...,  # (9)
    HttpEndpointDestinationConfiguration: HttpEndpointDestinationConfigurationTypeDef = ...,  # (10)
    Tags: Sequence[TagTypeDef] = ...,  # (11)
    AmazonOpenSearchServerlessDestinationConfiguration: AmazonOpenSearchServerlessDestinationConfigurationTypeDef = ...,  # (12)
    MSKSourceConfiguration: MSKSourceConfigurationTypeDef = ...,  # (13)
    SnowflakeDestinationConfiguration: SnowflakeDestinationConfigurationTypeDef = ...,  # (14)
    IcebergDestinationConfiguration: IcebergDestinationConfigurationTypeDef = ...,  # (15)
    DatabaseSourceConfiguration: DatabaseSourceConfigurationTypeDef = ...,  # (16)
) -> CreateDeliveryStreamOutputTypeDef:  # (17)
    ...
```

1. See [:material-code-brackets: DeliveryStreamTypeType](./literals.md#deliverystreamtypetype) 
2. See [:material-code-braces: KinesisStreamSourceConfigurationTypeDef](./type_defs.md#kinesisstreamsourceconfigurationtypedef) 
3. See [:material-code-braces: DeliveryStreamEncryptionConfigurationInputTypeDef](./type_defs.md#deliverystreamencryptionconfigurationinputtypedef) 
4. See [:material-code-braces: S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef) 
5. See [:material-code-braces: ExtendedS3DestinationConfigurationTypeDef](./type_defs.md#extendeds3destinationconfigurationtypedef) 
6. See [:material-code-braces: RedshiftDestinationConfigurationTypeDef](./type_defs.md#redshiftdestinationconfigurationtypedef) 
7. See [:material-code-braces: ElasticsearchDestinationConfigurationTypeDef](./type_defs.md#elasticsearchdestinationconfigurationtypedef) 
8. See [:material-code-braces: AmazonopensearchserviceDestinationConfigurationTypeDef](./type_defs.md#amazonopensearchservicedestinationconfigurationtypedef) 
9. See [:material-code-braces: SplunkDestinationConfigurationTypeDef](./type_defs.md#splunkdestinationconfigurationtypedef) 
10. See [:material-code-braces: HttpEndpointDestinationConfigurationTypeDef](./type_defs.md#httpendpointdestinationconfigurationtypedef) 
11. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
12. See [:material-code-braces: AmazonOpenSearchServerlessDestinationConfigurationTypeDef](./type_defs.md#amazonopensearchserverlessdestinationconfigurationtypedef) 
13. See [:material-code-braces: MSKSourceConfigurationTypeDef](./type_defs.md#msksourceconfigurationtypedef) 
14. See [:material-code-braces: SnowflakeDestinationConfigurationTypeDef](./type_defs.md#snowflakedestinationconfigurationtypedef) 
15. See [:material-code-braces: IcebergDestinationConfigurationTypeDef](./type_defs.md#icebergdestinationconfigurationtypedef) 
16. See [:material-code-braces: DatabaseSourceConfigurationTypeDef](./type_defs.md#databasesourceconfigurationtypedef) 
17. See [:material-code-braces: CreateDeliveryStreamOutputTypeDef](./type_defs.md#createdeliverystreamoutputtypedef) 


```python
# create_delivery_stream method usage example with argument unpacking

kwargs: CreateDeliveryStreamInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
}

parent.create_delivery_stream(**kwargs)
```

1. See [:material-code-braces: CreateDeliveryStreamInputRequestTypeDef](./type_defs.md#createdeliverystreaminputrequesttypedef) 

### delete\_delivery\_stream

Deletes a Firehose stream and its data.

Type annotations and code completion for `#!python session.create_client("firehose").delete_delivery_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/delete_delivery_stream.html)

```python
# delete_delivery_stream method definition

await def delete_delivery_stream(
    self,
    *,
    DeliveryStreamName: str,
    AllowForceDelete: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_delivery_stream method usage example with argument unpacking

kwargs: DeleteDeliveryStreamInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
}

parent.delete_delivery_stream(**kwargs)
```

1. See [:material-code-braces: DeleteDeliveryStreamInputRequestTypeDef](./type_defs.md#deletedeliverystreaminputrequesttypedef) 

### describe\_delivery\_stream

Describes the specified Firehose stream and its status.

Type annotations and code completion for `#!python session.create_client("firehose").describe_delivery_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/describe_delivery_stream.html)

```python
# describe_delivery_stream method definition

await def describe_delivery_stream(
    self,
    *,
    DeliveryStreamName: str,
    Limit: int = ...,
    ExclusiveStartDestinationId: str = ...,
) -> DescribeDeliveryStreamOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeliveryStreamOutputTypeDef](./type_defs.md#describedeliverystreamoutputtypedef) 


```python
# describe_delivery_stream method usage example with argument unpacking

kwargs: DescribeDeliveryStreamInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
}

parent.describe_delivery_stream(**kwargs)
```

1. See [:material-code-braces: DescribeDeliveryStreamInputRequestTypeDef](./type_defs.md#describedeliverystreaminputrequesttypedef) 

### list\_delivery\_streams

Lists your Firehose streams in alphabetical order of their names.

Type annotations and code completion for `#!python session.create_client("firehose").list_delivery_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/list_delivery_streams.html)

```python
# list_delivery_streams method definition

await def list_delivery_streams(
    self,
    *,
    Limit: int = ...,
    DeliveryStreamType: DeliveryStreamTypeType = ...,  # (1)
    ExclusiveStartDeliveryStreamName: str = ...,
) -> ListDeliveryStreamsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeliveryStreamTypeType](./literals.md#deliverystreamtypetype) 
2. See [:material-code-braces: ListDeliveryStreamsOutputTypeDef](./type_defs.md#listdeliverystreamsoutputtypedef) 


```python
# list_delivery_streams method usage example with argument unpacking

kwargs: ListDeliveryStreamsInputRequestTypeDef = {  # (1)
    "Limit": ...,
}

parent.list_delivery_streams(**kwargs)
```

1. See [:material-code-braces: ListDeliveryStreamsInputRequestTypeDef](./type_defs.md#listdeliverystreamsinputrequesttypedef) 

### list\_tags\_for\_delivery\_stream

Lists the tags for the specified Firehose stream.

Type annotations and code completion for `#!python session.create_client("firehose").list_tags_for_delivery_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/list_tags_for_delivery_stream.html)

```python
# list_tags_for_delivery_stream method definition

await def list_tags_for_delivery_stream(
    self,
    *,
    DeliveryStreamName: str,
    ExclusiveStartTagKey: str = ...,
    Limit: int = ...,
) -> ListTagsForDeliveryStreamOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForDeliveryStreamOutputTypeDef](./type_defs.md#listtagsfordeliverystreamoutputtypedef) 


```python
# list_tags_for_delivery_stream method usage example with argument unpacking

kwargs: ListTagsForDeliveryStreamInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
}

parent.list_tags_for_delivery_stream(**kwargs)
```

1. See [:material-code-braces: ListTagsForDeliveryStreamInputRequestTypeDef](./type_defs.md#listtagsfordeliverystreaminputrequesttypedef) 

### put\_record

Writes a single data record into an Firehose stream.

Type annotations and code completion for `#!python session.create_client("firehose").put_record` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/put_record.html)

```python
# put_record method definition

await def put_record(
    self,
    *,
    DeliveryStreamName: str,
    Record: RecordTypeDef,  # (1)
) -> PutRecordOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
2. See [:material-code-braces: PutRecordOutputTypeDef](./type_defs.md#putrecordoutputtypedef) 


```python
# put_record method usage example with argument unpacking

kwargs: PutRecordInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
    "Record": ...,
}

parent.put_record(**kwargs)
```

1. See [:material-code-braces: PutRecordInputRequestTypeDef](./type_defs.md#putrecordinputrequesttypedef) 

### put\_record\_batch

Writes multiple data records into a Firehose stream in a single call, which can
achieve higher throughput per producer than when writing single records.

Type annotations and code completion for `#!python session.create_client("firehose").put_record_batch` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/put_record_batch.html)

```python
# put_record_batch method definition

await def put_record_batch(
    self,
    *,
    DeliveryStreamName: str,
    Records: Sequence[RecordTypeDef],  # (1)
) -> PutRecordBatchOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
2. See [:material-code-braces: PutRecordBatchOutputTypeDef](./type_defs.md#putrecordbatchoutputtypedef) 


```python
# put_record_batch method usage example with argument unpacking

kwargs: PutRecordBatchInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
    "Records": ...,
}

parent.put_record_batch(**kwargs)
```

1. See [:material-code-braces: PutRecordBatchInputRequestTypeDef](./type_defs.md#putrecordbatchinputrequesttypedef) 

### start\_delivery\_stream\_encryption

Enables server-side encryption (SSE) for the Firehose stream.

Type annotations and code completion for `#!python session.create_client("firehose").start_delivery_stream_encryption` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/start_delivery_stream_encryption.html)

```python
# start_delivery_stream_encryption method definition

await def start_delivery_stream_encryption(
    self,
    *,
    DeliveryStreamName: str,
    DeliveryStreamEncryptionConfigurationInput: DeliveryStreamEncryptionConfigurationInputTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: DeliveryStreamEncryptionConfigurationInputTypeDef](./type_defs.md#deliverystreamencryptionconfigurationinputtypedef) 


```python
# start_delivery_stream_encryption method usage example with argument unpacking

kwargs: StartDeliveryStreamEncryptionInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
}

parent.start_delivery_stream_encryption(**kwargs)
```

1. See [:material-code-braces: StartDeliveryStreamEncryptionInputRequestTypeDef](./type_defs.md#startdeliverystreamencryptioninputrequesttypedef) 

### stop\_delivery\_stream\_encryption

Disables server-side encryption (SSE) for the Firehose stream.

Type annotations and code completion for `#!python session.create_client("firehose").stop_delivery_stream_encryption` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/stop_delivery_stream_encryption.html)

```python
# stop_delivery_stream_encryption method definition

await def stop_delivery_stream_encryption(
    self,
    *,
    DeliveryStreamName: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_delivery_stream_encryption method usage example with argument unpacking

kwargs: StopDeliveryStreamEncryptionInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
}

parent.stop_delivery_stream_encryption(**kwargs)
```

1. See [:material-code-braces: StopDeliveryStreamEncryptionInputRequestTypeDef](./type_defs.md#stopdeliverystreamencryptioninputrequesttypedef) 

### tag\_delivery\_stream

Adds or updates tags for the specified Firehose stream.

Type annotations and code completion for `#!python session.create_client("firehose").tag_delivery_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/tag_delivery_stream.html)

```python
# tag_delivery_stream method definition

await def tag_delivery_stream(
    self,
    *,
    DeliveryStreamName: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_delivery_stream method usage example with argument unpacking

kwargs: TagDeliveryStreamInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
    "Tags": ...,
}

parent.tag_delivery_stream(**kwargs)
```

1. See [:material-code-braces: TagDeliveryStreamInputRequestTypeDef](./type_defs.md#tagdeliverystreaminputrequesttypedef) 

### untag\_delivery\_stream

Removes tags from the specified Firehose stream.

Type annotations and code completion for `#!python session.create_client("firehose").untag_delivery_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/untag_delivery_stream.html)

```python
# untag_delivery_stream method definition

await def untag_delivery_stream(
    self,
    *,
    DeliveryStreamName: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_delivery_stream method usage example with argument unpacking

kwargs: UntagDeliveryStreamInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
    "TagKeys": ...,
}

parent.untag_delivery_stream(**kwargs)
```

1. See [:material-code-braces: UntagDeliveryStreamInputRequestTypeDef](./type_defs.md#untagdeliverystreaminputrequesttypedef) 

### update\_destination

Updates the specified destination of the specified Firehose stream.

Type annotations and code completion for `#!python session.create_client("firehose").update_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose/client/update_destination.html)

```python
# update_destination method definition

await def update_destination(
    self,
    *,
    DeliveryStreamName: str,
    CurrentDeliveryStreamVersionId: str,
    DestinationId: str,
    S3DestinationUpdate: S3DestinationUpdateTypeDef = ...,  # (1)
    ExtendedS3DestinationUpdate: ExtendedS3DestinationUpdateTypeDef = ...,  # (2)
    RedshiftDestinationUpdate: RedshiftDestinationUpdateTypeDef = ...,  # (3)
    ElasticsearchDestinationUpdate: ElasticsearchDestinationUpdateTypeDef = ...,  # (4)
    AmazonopensearchserviceDestinationUpdate: AmazonopensearchserviceDestinationUpdateTypeDef = ...,  # (5)
    SplunkDestinationUpdate: SplunkDestinationUpdateTypeDef = ...,  # (6)
    HttpEndpointDestinationUpdate: HttpEndpointDestinationUpdateTypeDef = ...,  # (7)
    AmazonOpenSearchServerlessDestinationUpdate: AmazonOpenSearchServerlessDestinationUpdateTypeDef = ...,  # (8)
    SnowflakeDestinationUpdate: SnowflakeDestinationUpdateTypeDef = ...,  # (9)
    IcebergDestinationUpdate: IcebergDestinationUpdateTypeDef = ...,  # (10)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: S3DestinationUpdateTypeDef](./type_defs.md#s3destinationupdatetypedef) 
2. See [:material-code-braces: ExtendedS3DestinationUpdateTypeDef](./type_defs.md#extendeds3destinationupdatetypedef) 
3. See [:material-code-braces: RedshiftDestinationUpdateTypeDef](./type_defs.md#redshiftdestinationupdatetypedef) 
4. See [:material-code-braces: ElasticsearchDestinationUpdateTypeDef](./type_defs.md#elasticsearchdestinationupdatetypedef) 
5. See [:material-code-braces: AmazonopensearchserviceDestinationUpdateTypeDef](./type_defs.md#amazonopensearchservicedestinationupdatetypedef) 
6. See [:material-code-braces: SplunkDestinationUpdateTypeDef](./type_defs.md#splunkdestinationupdatetypedef) 
7. See [:material-code-braces: HttpEndpointDestinationUpdateTypeDef](./type_defs.md#httpendpointdestinationupdatetypedef) 
8. See [:material-code-braces: AmazonOpenSearchServerlessDestinationUpdateTypeDef](./type_defs.md#amazonopensearchserverlessdestinationupdatetypedef) 
9. See [:material-code-braces: SnowflakeDestinationUpdateTypeDef](./type_defs.md#snowflakedestinationupdatetypedef) 
10. See [:material-code-braces: IcebergDestinationUpdateTypeDef](./type_defs.md#icebergdestinationupdatetypedef) 


```python
# update_destination method usage example with argument unpacking

kwargs: UpdateDestinationInputRequestTypeDef = {  # (1)
    "DeliveryStreamName": ...,
    "CurrentDeliveryStreamVersionId": ...,
    "DestinationId": ...,
}

parent.update_destination(**kwargs)
```

1. See [:material-code-braces: UpdateDestinationInputRequestTypeDef](./type_defs.md#updatedestinationinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("firehose").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("firehose").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#Firehose.Client)

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





