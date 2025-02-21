# IoTAnalyticsClient

> [Index](../README.md) > [IoTAnalytics](./README.md) > IoTAnalyticsClient

!!! note ""

    Auto-generated documentation for [IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#iotanalytics)
    type annotations stubs module [types-aiobotocore-iotanalytics](https://pypi.org/project/types-aiobotocore-iotanalytics/).

## IoTAnalyticsClient

Type annotations and code completion for `#!python session.create_client("iotanalytics")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client)

```python
# IoTAnalyticsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iotanalytics.client import IoTAnalyticsClient

session = get_session()
async with session.create_client("iotanalytics") as client:
    client: IoTAnalyticsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iotanalytics").exceptions` structure.

```python
# IoTAnalyticsClient.exceptions usage example

async with session.create_client("iotanalytics") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalFailureException,
        client.InvalidRequestException,
        client.LimitExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python
# IoTAnalyticsClient usage type checking example

from types_aiobotocore_iotanalytics.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("iotanalytics").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("iotanalytics").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/generate_presigned_url.html)

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


### batch\_put\_message

Sends messages to a channel.

Type annotations and code completion for `#!python session.create_client("iotanalytics").batch_put_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/batch_put_message.html)

```python
# batch_put_message method definition

await def batch_put_message(
    self,
    *,
    channelName: str,
    messages: Sequence[MessageTypeDef],  # (1)
) -> BatchPutMessageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: BatchPutMessageResponseTypeDef](./type_defs.md#batchputmessageresponsetypedef) 


```python
# batch_put_message method usage example with argument unpacking

kwargs: BatchPutMessageRequestTypeDef = {  # (1)
    "channelName": ...,
    "messages": ...,
}

parent.batch_put_message(**kwargs)
```

1. See [:material-code-braces: BatchPutMessageRequestTypeDef](./type_defs.md#batchputmessagerequesttypedef) 

### cancel\_pipeline\_reprocessing

Cancels the reprocessing of data through the pipeline.

Type annotations and code completion for `#!python session.create_client("iotanalytics").cancel_pipeline_reprocessing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/cancel_pipeline_reprocessing.html)

```python
# cancel_pipeline_reprocessing method definition

await def cancel_pipeline_reprocessing(
    self,
    *,
    pipelineName: str,
    reprocessingId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_pipeline_reprocessing method usage example with argument unpacking

kwargs: CancelPipelineReprocessingRequestTypeDef = {  # (1)
    "pipelineName": ...,
    "reprocessingId": ...,
}

parent.cancel_pipeline_reprocessing(**kwargs)
```

1. See [:material-code-braces: CancelPipelineReprocessingRequestTypeDef](./type_defs.md#cancelpipelinereprocessingrequesttypedef) 

### create\_channel

Used to create a channel.

Type annotations and code completion for `#!python session.create_client("iotanalytics").create_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/create_channel.html)

```python
# create_channel method definition

await def create_channel(
    self,
    *,
    channelName: str,
    channelStorage: ChannelStorageUnionTypeDef = ...,  # (1)
    retentionPeriod: RetentionPeriodTypeDef = ...,  # (2)
    tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateChannelResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ChannelStorageTypeDef](./type_defs.md#channelstoragetypedef) [:material-code-braces: ChannelStorageOutputTypeDef](./type_defs.md#channelstorageoutputtypedef) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef) 


```python
# create_channel method usage example with argument unpacking

kwargs: CreateChannelRequestTypeDef = {  # (1)
    "channelName": ...,
}

parent.create_channel(**kwargs)
```

1. See [:material-code-braces: CreateChannelRequestTypeDef](./type_defs.md#createchannelrequesttypedef) 

### create\_dataset

Used to create a dataset.

Type annotations and code completion for `#!python session.create_client("iotanalytics").create_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/create_dataset.html)

```python
# create_dataset method definition

await def create_dataset(
    self,
    *,
    datasetName: str,
    actions: Sequence[DatasetActionUnionTypeDef],  # (1)
    triggers: Sequence[DatasetTriggerTypeDef] = ...,  # (2)
    contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,  # (3)
    retentionPeriod: RetentionPeriodTypeDef = ...,  # (4)
    versioningConfiguration: VersioningConfigurationTypeDef = ...,  # (5)
    tags: Sequence[TagTypeDef] = ...,  # (6)
    lateDataRules: Sequence[LateDataRuleTypeDef] = ...,  # (7)
) -> CreateDatasetResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: DatasetActionTypeDef](./type_defs.md#datasetactiontypedef) [:material-code-braces: DatasetActionOutputTypeDef](./type_defs.md#datasetactionoutputtypedef) 
2. See [:material-code-braces: DatasetTriggerTypeDef](./type_defs.md#datasettriggertypedef) 
3. See [:material-code-braces: DatasetContentDeliveryRuleTypeDef](./type_defs.md#datasetcontentdeliveryruletypedef) 
4. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
5. See [:material-code-braces: VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: LateDataRuleTypeDef](./type_defs.md#latedataruletypedef) 
8. See [:material-code-braces: CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef) 


```python
# create_dataset method usage example with argument unpacking

kwargs: CreateDatasetRequestTypeDef = {  # (1)
    "datasetName": ...,
    "actions": ...,
}

parent.create_dataset(**kwargs)
```

1. See [:material-code-braces: CreateDatasetRequestTypeDef](./type_defs.md#createdatasetrequesttypedef) 

### create\_dataset\_content

Creates the content of a dataset by applying a <code>queryAction</code> (a SQL
query) or a <code>containerAction</code> (executing a containerized
application).

Type annotations and code completion for `#!python session.create_client("iotanalytics").create_dataset_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/create_dataset_content.html)

```python
# create_dataset_content method definition

await def create_dataset_content(
    self,
    *,
    datasetName: str,
    versionId: str = ...,
) -> CreateDatasetContentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateDatasetContentResponseTypeDef](./type_defs.md#createdatasetcontentresponsetypedef) 


```python
# create_dataset_content method usage example with argument unpacking

kwargs: CreateDatasetContentRequestTypeDef = {  # (1)
    "datasetName": ...,
}

parent.create_dataset_content(**kwargs)
```

1. See [:material-code-braces: CreateDatasetContentRequestTypeDef](./type_defs.md#createdatasetcontentrequesttypedef) 

### create\_datastore

Creates a data store, which is a repository for messages.

Type annotations and code completion for `#!python session.create_client("iotanalytics").create_datastore` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/create_datastore.html)

```python
# create_datastore method definition

await def create_datastore(
    self,
    *,
    datastoreName: str,
    datastoreStorage: DatastoreStorageUnionTypeDef = ...,  # (1)
    retentionPeriod: RetentionPeriodTypeDef = ...,  # (2)
    tags: Sequence[TagTypeDef] = ...,  # (3)
    fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...,  # (4)
    datastorePartitions: DatastorePartitionsUnionTypeDef = ...,  # (5)
) -> CreateDatastoreResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: DatastoreStorageTypeDef](./type_defs.md#datastorestoragetypedef) [:material-code-braces: DatastoreStorageOutputTypeDef](./type_defs.md#datastorestorageoutputtypedef) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: FileFormatConfigurationTypeDef](./type_defs.md#fileformatconfigurationtypedef) [:material-code-braces: FileFormatConfigurationOutputTypeDef](./type_defs.md#fileformatconfigurationoutputtypedef) 
5. See [:material-code-braces: DatastorePartitionsTypeDef](./type_defs.md#datastorepartitionstypedef) [:material-code-braces: DatastorePartitionsOutputTypeDef](./type_defs.md#datastorepartitionsoutputtypedef) 
6. See [:material-code-braces: CreateDatastoreResponseTypeDef](./type_defs.md#createdatastoreresponsetypedef) 


```python
# create_datastore method usage example with argument unpacking

kwargs: CreateDatastoreRequestTypeDef = {  # (1)
    "datastoreName": ...,
}

parent.create_datastore(**kwargs)
```

1. See [:material-code-braces: CreateDatastoreRequestTypeDef](./type_defs.md#createdatastorerequesttypedef) 

### create\_pipeline

Creates a pipeline.

Type annotations and code completion for `#!python session.create_client("iotanalytics").create_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/create_pipeline.html)

```python
# create_pipeline method definition

await def create_pipeline(
    self,
    *,
    pipelineName: str,
    pipelineActivities: Sequence[PipelineActivityUnionTypeDef],  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreatePipelineResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) [:material-code-braces: PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef) 


```python
# create_pipeline method usage example with argument unpacking

kwargs: CreatePipelineRequestTypeDef = {  # (1)
    "pipelineName": ...,
    "pipelineActivities": ...,
}

parent.create_pipeline(**kwargs)
```

1. See [:material-code-braces: CreatePipelineRequestTypeDef](./type_defs.md#createpipelinerequesttypedef) 

### delete\_channel

Deletes the specified channel.

Type annotations and code completion for `#!python session.create_client("iotanalytics").delete_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/delete_channel.html)

```python
# delete_channel method definition

await def delete_channel(
    self,
    *,
    channelName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_channel method usage example with argument unpacking

kwargs: DeleteChannelRequestTypeDef = {  # (1)
    "channelName": ...,
}

parent.delete_channel(**kwargs)
```

1. See [:material-code-braces: DeleteChannelRequestTypeDef](./type_defs.md#deletechannelrequesttypedef) 

### delete\_dataset

Deletes the specified dataset.

Type annotations and code completion for `#!python session.create_client("iotanalytics").delete_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/delete_dataset.html)

```python
# delete_dataset method definition

await def delete_dataset(
    self,
    *,
    datasetName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_dataset method usage example with argument unpacking

kwargs: DeleteDatasetRequestTypeDef = {  # (1)
    "datasetName": ...,
}

parent.delete_dataset(**kwargs)
```

1. See [:material-code-braces: DeleteDatasetRequestTypeDef](./type_defs.md#deletedatasetrequesttypedef) 

### delete\_dataset\_content

Deletes the content of the specified dataset.

Type annotations and code completion for `#!python session.create_client("iotanalytics").delete_dataset_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/delete_dataset_content.html)

```python
# delete_dataset_content method definition

await def delete_dataset_content(
    self,
    *,
    datasetName: str,
    versionId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_dataset_content method usage example with argument unpacking

kwargs: DeleteDatasetContentRequestTypeDef = {  # (1)
    "datasetName": ...,
}

parent.delete_dataset_content(**kwargs)
```

1. See [:material-code-braces: DeleteDatasetContentRequestTypeDef](./type_defs.md#deletedatasetcontentrequesttypedef) 

### delete\_datastore

Deletes the specified data store.

Type annotations and code completion for `#!python session.create_client("iotanalytics").delete_datastore` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/delete_datastore.html)

```python
# delete_datastore method definition

await def delete_datastore(
    self,
    *,
    datastoreName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_datastore method usage example with argument unpacking

kwargs: DeleteDatastoreRequestTypeDef = {  # (1)
    "datastoreName": ...,
}

parent.delete_datastore(**kwargs)
```

1. See [:material-code-braces: DeleteDatastoreRequestTypeDef](./type_defs.md#deletedatastorerequesttypedef) 

### delete\_pipeline

Deletes the specified pipeline.

Type annotations and code completion for `#!python session.create_client("iotanalytics").delete_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/delete_pipeline.html)

```python
# delete_pipeline method definition

await def delete_pipeline(
    self,
    *,
    pipelineName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_pipeline method usage example with argument unpacking

kwargs: DeletePipelineRequestTypeDef = {  # (1)
    "pipelineName": ...,
}

parent.delete_pipeline(**kwargs)
```

1. See [:material-code-braces: DeletePipelineRequestTypeDef](./type_defs.md#deletepipelinerequesttypedef) 

### describe\_channel

Retrieves information about a channel.

Type annotations and code completion for `#!python session.create_client("iotanalytics").describe_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/describe_channel.html)

```python
# describe_channel method definition

await def describe_channel(
    self,
    *,
    channelName: str,
    includeStatistics: bool = ...,
) -> DescribeChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelResponseTypeDef](./type_defs.md#describechannelresponsetypedef) 


```python
# describe_channel method usage example with argument unpacking

kwargs: DescribeChannelRequestTypeDef = {  # (1)
    "channelName": ...,
}

parent.describe_channel(**kwargs)
```

1. See [:material-code-braces: DescribeChannelRequestTypeDef](./type_defs.md#describechannelrequesttypedef) 

### describe\_dataset

Retrieves information about a dataset.

Type annotations and code completion for `#!python session.create_client("iotanalytics").describe_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/describe_dataset.html)

```python
# describe_dataset method definition

await def describe_dataset(
    self,
    *,
    datasetName: str,
) -> DescribeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef) 


```python
# describe_dataset method usage example with argument unpacking

kwargs: DescribeDatasetRequestTypeDef = {  # (1)
    "datasetName": ...,
}

parent.describe_dataset(**kwargs)
```

1. See [:material-code-braces: DescribeDatasetRequestTypeDef](./type_defs.md#describedatasetrequesttypedef) 

### describe\_datastore

Retrieves information about a data store.

Type annotations and code completion for `#!python session.create_client("iotanalytics").describe_datastore` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/describe_datastore.html)

```python
# describe_datastore method definition

await def describe_datastore(
    self,
    *,
    datastoreName: str,
    includeStatistics: bool = ...,
) -> DescribeDatastoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatastoreResponseTypeDef](./type_defs.md#describedatastoreresponsetypedef) 


```python
# describe_datastore method usage example with argument unpacking

kwargs: DescribeDatastoreRequestTypeDef = {  # (1)
    "datastoreName": ...,
}

parent.describe_datastore(**kwargs)
```

1. See [:material-code-braces: DescribeDatastoreRequestTypeDef](./type_defs.md#describedatastorerequesttypedef) 

### describe\_logging\_options

Retrieves the current settings of the IoT Analytics logging options.

Type annotations and code completion for `#!python session.create_client("iotanalytics").describe_logging_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/describe_logging_options.html)

```python
# describe_logging_options method definition

await def describe_logging_options(
    self,
) -> DescribeLoggingOptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLoggingOptionsResponseTypeDef](./type_defs.md#describeloggingoptionsresponsetypedef) 

### describe\_pipeline

Retrieves information about a pipeline.

Type annotations and code completion for `#!python session.create_client("iotanalytics").describe_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/describe_pipeline.html)

```python
# describe_pipeline method definition

await def describe_pipeline(
    self,
    *,
    pipelineName: str,
) -> DescribePipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePipelineResponseTypeDef](./type_defs.md#describepipelineresponsetypedef) 


```python
# describe_pipeline method usage example with argument unpacking

kwargs: DescribePipelineRequestTypeDef = {  # (1)
    "pipelineName": ...,
}

parent.describe_pipeline(**kwargs)
```

1. See [:material-code-braces: DescribePipelineRequestTypeDef](./type_defs.md#describepipelinerequesttypedef) 

### get\_dataset\_content

Retrieves the contents of a dataset as presigned URIs.

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_dataset_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/get_dataset_content.html)

```python
# get_dataset_content method definition

await def get_dataset_content(
    self,
    *,
    datasetName: str,
    versionId: str = ...,
) -> GetDatasetContentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDatasetContentResponseTypeDef](./type_defs.md#getdatasetcontentresponsetypedef) 


```python
# get_dataset_content method usage example with argument unpacking

kwargs: GetDatasetContentRequestTypeDef = {  # (1)
    "datasetName": ...,
}

parent.get_dataset_content(**kwargs)
```

1. See [:material-code-braces: GetDatasetContentRequestTypeDef](./type_defs.md#getdatasetcontentrequesttypedef) 

### list\_channels

Retrieves a list of channels.

Type annotations and code completion for `#!python session.create_client("iotanalytics").list_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/list_channels.html)

```python
# list_channels method definition

await def list_channels(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# list_channels method usage example with argument unpacking

kwargs: ListChannelsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_channels(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestTypeDef](./type_defs.md#listchannelsrequesttypedef) 

### list\_dataset\_contents

Lists information about dataset contents that have been created.

Type annotations and code completion for `#!python session.create_client("iotanalytics").list_dataset_contents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/list_dataset_contents.html)

```python
# list_dataset_contents method definition

await def list_dataset_contents(
    self,
    *,
    datasetName: str,
    nextToken: str = ...,
    maxResults: int = ...,
    scheduledOnOrAfter: TimestampTypeDef = ...,
    scheduledBefore: TimestampTypeDef = ...,
) -> ListDatasetContentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatasetContentsResponseTypeDef](./type_defs.md#listdatasetcontentsresponsetypedef) 


```python
# list_dataset_contents method usage example with argument unpacking

kwargs: ListDatasetContentsRequestTypeDef = {  # (1)
    "datasetName": ...,
}

parent.list_dataset_contents(**kwargs)
```

1. See [:material-code-braces: ListDatasetContentsRequestTypeDef](./type_defs.md#listdatasetcontentsrequesttypedef) 

### list\_datasets

Retrieves information about datasets.

Type annotations and code completion for `#!python session.create_client("iotanalytics").list_datasets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/list_datasets.html)

```python
# list_datasets method definition

await def list_datasets(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDatasetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# list_datasets method usage example with argument unpacking

kwargs: ListDatasetsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_datasets(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestTypeDef](./type_defs.md#listdatasetsrequesttypedef) 

### list\_datastores

Retrieves a list of data stores.

Type annotations and code completion for `#!python session.create_client("iotanalytics").list_datastores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/list_datastores.html)

```python
# list_datastores method definition

await def list_datastores(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDatastoresResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatastoresResponseTypeDef](./type_defs.md#listdatastoresresponsetypedef) 


```python
# list_datastores method usage example with argument unpacking

kwargs: ListDatastoresRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_datastores(**kwargs)
```

1. See [:material-code-braces: ListDatastoresRequestTypeDef](./type_defs.md#listdatastoresrequesttypedef) 

### list\_pipelines

Retrieves a list of pipelines.

Type annotations and code completion for `#!python session.create_client("iotanalytics").list_pipelines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/list_pipelines.html)

```python
# list_pipelines method definition

await def list_pipelines(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPipelinesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef) 


```python
# list_pipelines method usage example with argument unpacking

kwargs: ListPipelinesRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_pipelines(**kwargs)
```

1. See [:material-code-braces: ListPipelinesRequestTypeDef](./type_defs.md#listpipelinesrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags (metadata) that you have assigned to the resource.

Type annotations and code completion for `#!python session.create_client("iotanalytics").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### put\_logging\_options

Sets or updates the IoT Analytics logging options.

Type annotations and code completion for `#!python session.create_client("iotanalytics").put_logging_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/put_logging_options.html)

```python
# put_logging_options method definition

await def put_logging_options(
    self,
    *,
    loggingOptions: LoggingOptionsTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_logging_options method usage example with argument unpacking

kwargs: PutLoggingOptionsRequestTypeDef = {  # (1)
    "loggingOptions": ...,
}

parent.put_logging_options(**kwargs)
```

1. See [:material-code-braces: PutLoggingOptionsRequestTypeDef](./type_defs.md#putloggingoptionsrequesttypedef) 

### run\_pipeline\_activity

Simulates the results of running a pipeline activity on a message payload.

Type annotations and code completion for `#!python session.create_client("iotanalytics").run_pipeline_activity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/run_pipeline_activity.html)

```python
# run_pipeline_activity method definition

await def run_pipeline_activity(
    self,
    *,
    pipelineActivity: PipelineActivityUnionTypeDef,  # (1)
    payloads: Sequence[BlobTypeDef],
) -> RunPipelineActivityResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) [:material-code-braces: PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef) 
2. See [:material-code-braces: RunPipelineActivityResponseTypeDef](./type_defs.md#runpipelineactivityresponsetypedef) 


```python
# run_pipeline_activity method usage example with argument unpacking

kwargs: RunPipelineActivityRequestTypeDef = {  # (1)
    "pipelineActivity": ...,
    "payloads": ...,
}

parent.run_pipeline_activity(**kwargs)
```

1. See [:material-code-braces: RunPipelineActivityRequestTypeDef](./type_defs.md#runpipelineactivityrequesttypedef) 

### sample\_channel\_data

Retrieves a sample of messages from the specified channel ingested during the
specified timeframe.

Type annotations and code completion for `#!python session.create_client("iotanalytics").sample_channel_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/sample_channel_data.html)

```python
# sample_channel_data method definition

await def sample_channel_data(
    self,
    *,
    channelName: str,
    maxMessages: int = ...,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
) -> SampleChannelDataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SampleChannelDataResponseTypeDef](./type_defs.md#samplechanneldataresponsetypedef) 


```python
# sample_channel_data method usage example with argument unpacking

kwargs: SampleChannelDataRequestTypeDef = {  # (1)
    "channelName": ...,
}

parent.sample_channel_data(**kwargs)
```

1. See [:material-code-braces: SampleChannelDataRequestTypeDef](./type_defs.md#samplechanneldatarequesttypedef) 

### start\_pipeline\_reprocessing

Starts the reprocessing of raw message data through the pipeline.

Type annotations and code completion for `#!python session.create_client("iotanalytics").start_pipeline_reprocessing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/start_pipeline_reprocessing.html)

```python
# start_pipeline_reprocessing method definition

await def start_pipeline_reprocessing(
    self,
    *,
    pipelineName: str,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    channelMessages: ChannelMessagesTypeDef = ...,  # (1)
) -> StartPipelineReprocessingResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ChannelMessagesTypeDef](./type_defs.md#channelmessagestypedef) 
2. See [:material-code-braces: StartPipelineReprocessingResponseTypeDef](./type_defs.md#startpipelinereprocessingresponsetypedef) 


```python
# start_pipeline_reprocessing method usage example with argument unpacking

kwargs: StartPipelineReprocessingRequestTypeDef = {  # (1)
    "pipelineName": ...,
}

parent.start_pipeline_reprocessing(**kwargs)
```

1. See [:material-code-braces: StartPipelineReprocessingRequestTypeDef](./type_defs.md#startpipelinereprocessingrequesttypedef) 

### tag\_resource

Adds to or modifies the tags of the given resource.

Type annotations and code completion for `#!python session.create_client("iotanalytics").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes the given tags (metadata) from the resource.

Type annotations and code completion for `#!python session.create_client("iotanalytics").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_channel

Used to update the settings of a channel.

Type annotations and code completion for `#!python session.create_client("iotanalytics").update_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/update_channel.html)

```python
# update_channel method definition

await def update_channel(
    self,
    *,
    channelName: str,
    channelStorage: ChannelStorageUnionTypeDef = ...,  # (1)
    retentionPeriod: RetentionPeriodTypeDef = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ChannelStorageTypeDef](./type_defs.md#channelstoragetypedef) [:material-code-braces: ChannelStorageOutputTypeDef](./type_defs.md#channelstorageoutputtypedef) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_channel method usage example with argument unpacking

kwargs: UpdateChannelRequestTypeDef = {  # (1)
    "channelName": ...,
}

parent.update_channel(**kwargs)
```

1. See [:material-code-braces: UpdateChannelRequestTypeDef](./type_defs.md#updatechannelrequesttypedef) 

### update\_dataset

Updates the settings of a dataset.

Type annotations and code completion for `#!python session.create_client("iotanalytics").update_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/update_dataset.html)

```python
# update_dataset method definition

await def update_dataset(
    self,
    *,
    datasetName: str,
    actions: Sequence[DatasetActionUnionTypeDef],  # (1)
    triggers: Sequence[DatasetTriggerTypeDef] = ...,  # (2)
    contentDeliveryRules: Sequence[DatasetContentDeliveryRuleTypeDef] = ...,  # (3)
    retentionPeriod: RetentionPeriodTypeDef = ...,  # (4)
    versioningConfiguration: VersioningConfigurationTypeDef = ...,  # (5)
    lateDataRules: Sequence[LateDataRuleTypeDef] = ...,  # (6)
) -> EmptyResponseMetadataTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: DatasetActionTypeDef](./type_defs.md#datasetactiontypedef) [:material-code-braces: DatasetActionOutputTypeDef](./type_defs.md#datasetactionoutputtypedef) 
2. See [:material-code-braces: DatasetTriggerTypeDef](./type_defs.md#datasettriggertypedef) 
3. See [:material-code-braces: DatasetContentDeliveryRuleTypeDef](./type_defs.md#datasetcontentdeliveryruletypedef) 
4. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
5. See [:material-code-braces: VersioningConfigurationTypeDef](./type_defs.md#versioningconfigurationtypedef) 
6. See [:material-code-braces: LateDataRuleTypeDef](./type_defs.md#latedataruletypedef) 
7. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_dataset method usage example with argument unpacking

kwargs: UpdateDatasetRequestTypeDef = {  # (1)
    "datasetName": ...,
    "actions": ...,
}

parent.update_dataset(**kwargs)
```

1. See [:material-code-braces: UpdateDatasetRequestTypeDef](./type_defs.md#updatedatasetrequesttypedef) 

### update\_datastore

Used to update the settings of a data store.

Type annotations and code completion for `#!python session.create_client("iotanalytics").update_datastore` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/update_datastore.html)

```python
# update_datastore method definition

await def update_datastore(
    self,
    *,
    datastoreName: str,
    retentionPeriod: RetentionPeriodTypeDef = ...,  # (1)
    datastoreStorage: DatastoreStorageUnionTypeDef = ...,  # (2)
    fileFormatConfiguration: FileFormatConfigurationUnionTypeDef = ...,  # (3)
) -> EmptyResponseMetadataTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-braces: DatastoreStorageTypeDef](./type_defs.md#datastorestoragetypedef) [:material-code-braces: DatastoreStorageOutputTypeDef](./type_defs.md#datastorestorageoutputtypedef) 
3. See [:material-code-braces: FileFormatConfigurationTypeDef](./type_defs.md#fileformatconfigurationtypedef) [:material-code-braces: FileFormatConfigurationOutputTypeDef](./type_defs.md#fileformatconfigurationoutputtypedef) 
4. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_datastore method usage example with argument unpacking

kwargs: UpdateDatastoreRequestTypeDef = {  # (1)
    "datastoreName": ...,
}

parent.update_datastore(**kwargs)
```

1. See [:material-code-braces: UpdateDatastoreRequestTypeDef](./type_defs.md#updatedatastorerequesttypedef) 

### update\_pipeline

Updates the settings of a pipeline.

Type annotations and code completion for `#!python session.create_client("iotanalytics").update_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/client/update_pipeline.html)

```python
# update_pipeline method definition

await def update_pipeline(
    self,
    *,
    pipelineName: str,
    pipelineActivities: Sequence[PipelineActivityUnionTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PipelineActivityTypeDef](./type_defs.md#pipelineactivitytypedef) [:material-code-braces: PipelineActivityOutputTypeDef](./type_defs.md#pipelineactivityoutputtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_pipeline method usage example with argument unpacking

kwargs: UpdatePipelineRequestTypeDef = {  # (1)
    "pipelineName": ...,
    "pipelineActivities": ...,
}

parent.update_pipeline(**kwargs)
```

1. See [:material-code-braces: UpdatePipelineRequestTypeDef](./type_defs.md#updatepipelinerequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iotanalytics").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iotanalytics").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Client)

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

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator` method with overloads.

- `client.get_paginator("list_channels")` -> [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- `client.get_paginator("list_dataset_contents")` -> [ListDatasetContentsPaginator](./paginators.md#listdatasetcontentspaginator)
- `client.get_paginator("list_datasets")` -> [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- `client.get_paginator("list_datastores")` -> [ListDatastoresPaginator](./paginators.md#listdatastorespaginator)
- `client.get_paginator("list_pipelines")` -> [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)



