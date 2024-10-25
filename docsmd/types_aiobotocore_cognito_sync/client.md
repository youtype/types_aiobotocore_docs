# CognitoSyncClient

> [Index](../README.md) > [CognitoSync](./README.md) > CognitoSyncClient

!!! note ""

    Auto-generated documentation for [CognitoSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync)
    type annotations stubs module [types-aiobotocore-cognito-sync](https://pypi.org/project/types-aiobotocore-cognito-sync/).

## CognitoSyncClient

Type annotations and code completion for `#!python session.create_client("cognito-sync")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client)

```python
# CognitoSyncClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cognito_sync.client import CognitoSyncClient

session = get_session()
async with session.create_client("cognito-sync") as client:
    client: CognitoSyncClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cognito-sync").exceptions` structure.

```python
# CognitoSyncClient.exceptions usage example

async with session.create_client("cognito-sync") as client:
    try:
        do_something(client)
    except (
            client.AlreadyStreamedException,
        client.ClientError,
        client.ConcurrentModificationException,
        client.DuplicateRequestException,
        client.InternalErrorException,
        client.InvalidConfigurationException,
        client.InvalidLambdaFunctionOutputException,
        client.InvalidParameterException,
        client.LambdaThrottledException,
        client.LimitExceededException,
        client.NotAuthorizedException,
        client.ResourceConflictException,
        client.ResourceNotFoundException,
        client.TooManyRequestsException,
    ) as e:
        print(e)
```

```python
# CognitoSyncClient usage type checking example

from types_aiobotocore_cognito_sync.client import Exceptions

def handle_error(exc: Exceptions.AlreadyStreamedException) -> None:
    ...
```


## Methods


### bulk\_publish

Initiates a bulk publish of all existing datasets for an Identity Pool to the
configured
stream.

Type annotations and code completion for `#!python session.create_client("cognito-sync").bulk_publish` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.bulk_publish)

```python
# bulk_publish method definition

await def bulk_publish(
    self,
    *,
    IdentityPoolId: str,
) -> BulkPublishResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BulkPublishResponseTypeDef](./type_defs.md#bulkpublishresponsetypedef) 


```python
# bulk_publish method usage example with argument unpacking

kwargs: BulkPublishRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.bulk_publish(**kwargs)
```

1. See [:material-code-braces: BulkPublishRequestRequestTypeDef](./type_defs.md#bulkpublishrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("cognito-sync").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("cognito-sync").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### delete\_dataset

Deletes the specific dataset.

Type annotations and code completion for `#!python session.create_client("cognito-sync").delete_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.delete_dataset)

```python
# delete_dataset method definition

await def delete_dataset(
    self,
    *,
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
) -> DeleteDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDatasetResponseTypeDef](./type_defs.md#deletedatasetresponsetypedef) 


```python
# delete_dataset method usage example with argument unpacking

kwargs: DeleteDatasetRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityId": ...,
    "DatasetName": ...,
}

parent.delete_dataset(**kwargs)
```

1. See [:material-code-braces: DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef) 

### describe\_dataset

Gets meta data about a dataset by identity and dataset name.

Type annotations and code completion for `#!python session.create_client("cognito-sync").describe_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.describe_dataset)

```python
# describe_dataset method definition

await def describe_dataset(
    self,
    *,
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
) -> DescribeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef) 


```python
# describe_dataset method usage example with argument unpacking

kwargs: DescribeDatasetRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityId": ...,
    "DatasetName": ...,
}

parent.describe_dataset(**kwargs)
```

1. See [:material-code-braces: DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef) 

### describe\_identity\_pool\_usage

Gets usage details (for example, data storage) about a particular identity pool.

Type annotations and code completion for `#!python session.create_client("cognito-sync").describe_identity_pool_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.describe_identity_pool_usage)

```python
# describe_identity_pool_usage method definition

await def describe_identity_pool_usage(
    self,
    *,
    IdentityPoolId: str,
) -> DescribeIdentityPoolUsageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIdentityPoolUsageResponseTypeDef](./type_defs.md#describeidentitypoolusageresponsetypedef) 


```python
# describe_identity_pool_usage method usage example with argument unpacking

kwargs: DescribeIdentityPoolUsageRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.describe_identity_pool_usage(**kwargs)
```

1. See [:material-code-braces: DescribeIdentityPoolUsageRequestRequestTypeDef](./type_defs.md#describeidentitypoolusagerequestrequesttypedef) 

### describe\_identity\_usage

Gets usage information for an identity, including number of datasets and data
usage.

Type annotations and code completion for `#!python session.create_client("cognito-sync").describe_identity_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.describe_identity_usage)

```python
# describe_identity_usage method definition

await def describe_identity_usage(
    self,
    *,
    IdentityPoolId: str,
    IdentityId: str,
) -> DescribeIdentityUsageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeIdentityUsageResponseTypeDef](./type_defs.md#describeidentityusageresponsetypedef) 


```python
# describe_identity_usage method usage example with argument unpacking

kwargs: DescribeIdentityUsageRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityId": ...,
}

parent.describe_identity_usage(**kwargs)
```

1. See [:material-code-braces: DescribeIdentityUsageRequestRequestTypeDef](./type_defs.md#describeidentityusagerequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("cognito-sync").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.generate_presigned_url)

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


### get\_bulk\_publish\_details

Get the status of the last BulkPublish operation for an identity pool.

Type annotations and code completion for `#!python session.create_client("cognito-sync").get_bulk_publish_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.get_bulk_publish_details)

```python
# get_bulk_publish_details method definition

await def get_bulk_publish_details(
    self,
    *,
    IdentityPoolId: str,
) -> GetBulkPublishDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBulkPublishDetailsResponseTypeDef](./type_defs.md#getbulkpublishdetailsresponsetypedef) 


```python
# get_bulk_publish_details method usage example with argument unpacking

kwargs: GetBulkPublishDetailsRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.get_bulk_publish_details(**kwargs)
```

1. See [:material-code-braces: GetBulkPublishDetailsRequestRequestTypeDef](./type_defs.md#getbulkpublishdetailsrequestrequesttypedef) 

### get\_cognito\_events

Gets the events and the corresponding Lambda functions associated with an
identity
pool.

Type annotations and code completion for `#!python session.create_client("cognito-sync").get_cognito_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.get_cognito_events)

```python
# get_cognito_events method definition

await def get_cognito_events(
    self,
    *,
    IdentityPoolId: str,
) -> GetCognitoEventsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCognitoEventsResponseTypeDef](./type_defs.md#getcognitoeventsresponsetypedef) 


```python
# get_cognito_events method usage example with argument unpacking

kwargs: GetCognitoEventsRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.get_cognito_events(**kwargs)
```

1. See [:material-code-braces: GetCognitoEventsRequestRequestTypeDef](./type_defs.md#getcognitoeventsrequestrequesttypedef) 

### get\_identity\_pool\_configuration

Gets the configuration settings of an identity pool.

Type annotations and code completion for `#!python session.create_client("cognito-sync").get_identity_pool_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.get_identity_pool_configuration)

```python
# get_identity_pool_configuration method definition

await def get_identity_pool_configuration(
    self,
    *,
    IdentityPoolId: str,
) -> GetIdentityPoolConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdentityPoolConfigurationResponseTypeDef](./type_defs.md#getidentitypoolconfigurationresponsetypedef) 


```python
# get_identity_pool_configuration method usage example with argument unpacking

kwargs: GetIdentityPoolConfigurationRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.get_identity_pool_configuration(**kwargs)
```

1. See [:material-code-braces: GetIdentityPoolConfigurationRequestRequestTypeDef](./type_defs.md#getidentitypoolconfigurationrequestrequesttypedef) 

### list\_datasets

Lists datasets for an identity.

Type annotations and code completion for `#!python session.create_client("cognito-sync").list_datasets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.list_datasets)

```python
# list_datasets method definition

await def list_datasets(
    self,
    *,
    IdentityPoolId: str,
    IdentityId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDatasetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# list_datasets method usage example with argument unpacking

kwargs: ListDatasetsRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityId": ...,
}

parent.list_datasets(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef) 

### list\_identity\_pool\_usage

Gets a list of identity pools registered with Cognito.

Type annotations and code completion for `#!python session.create_client("cognito-sync").list_identity_pool_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.list_identity_pool_usage)

```python
# list_identity_pool_usage method definition

await def list_identity_pool_usage(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListIdentityPoolUsageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdentityPoolUsageResponseTypeDef](./type_defs.md#listidentitypoolusageresponsetypedef) 


```python
# list_identity_pool_usage method usage example with argument unpacking

kwargs: ListIdentityPoolUsageRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_identity_pool_usage(**kwargs)
```

1. See [:material-code-braces: ListIdentityPoolUsageRequestRequestTypeDef](./type_defs.md#listidentitypoolusagerequestrequesttypedef) 

### list\_records

Gets paginated records, optionally changed after a particular sync count for a
dataset and
identity.

Type annotations and code completion for `#!python session.create_client("cognito-sync").list_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.list_records)

```python
# list_records method definition

await def list_records(
    self,
    *,
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
    LastSyncCount: int = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    SyncSessionToken: str = ...,
) -> ListRecordsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRecordsResponseTypeDef](./type_defs.md#listrecordsresponsetypedef) 


```python
# list_records method usage example with argument unpacking

kwargs: ListRecordsRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityId": ...,
    "DatasetName": ...,
}

parent.list_records(**kwargs)
```

1. See [:material-code-braces: ListRecordsRequestRequestTypeDef](./type_defs.md#listrecordsrequestrequesttypedef) 

### register\_device

Registers a device to receive push sync notifications.

Type annotations and code completion for `#!python session.create_client("cognito-sync").register_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.register_device)

```python
# register_device method definition

await def register_device(
    self,
    *,
    IdentityPoolId: str,
    IdentityId: str,
    Platform: PlatformType,  # (1)
    Token: str,
) -> RegisterDeviceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: RegisterDeviceResponseTypeDef](./type_defs.md#registerdeviceresponsetypedef) 


```python
# register_device method usage example with argument unpacking

kwargs: RegisterDeviceRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityId": ...,
    "Platform": ...,
    "Token": ...,
}

parent.register_device(**kwargs)
```

1. See [:material-code-braces: RegisterDeviceRequestRequestTypeDef](./type_defs.md#registerdevicerequestrequesttypedef) 

### set\_cognito\_events

Sets the AWS Lambda function for a given event type for an identity pool.

Type annotations and code completion for `#!python session.create_client("cognito-sync").set_cognito_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.set_cognito_events)

```python
# set_cognito_events method definition

await def set_cognito_events(
    self,
    *,
    IdentityPoolId: str,
    Events: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# set_cognito_events method usage example with argument unpacking

kwargs: SetCognitoEventsRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "Events": ...,
}

parent.set_cognito_events(**kwargs)
```

1. See [:material-code-braces: SetCognitoEventsRequestRequestTypeDef](./type_defs.md#setcognitoeventsrequestrequesttypedef) 

### set\_identity\_pool\_configuration

Sets the necessary configuration for push sync.

Type annotations and code completion for `#!python session.create_client("cognito-sync").set_identity_pool_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.set_identity_pool_configuration)

```python
# set_identity_pool_configuration method definition

await def set_identity_pool_configuration(
    self,
    *,
    IdentityPoolId: str,
    PushSync: PushSyncTypeDef = ...,  # (1)
    CognitoStreams: CognitoStreamsTypeDef = ...,  # (2)
) -> SetIdentityPoolConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PushSyncTypeDef](./type_defs.md#pushsynctypedef) 
2. See [:material-code-braces: CognitoStreamsTypeDef](./type_defs.md#cognitostreamstypedef) 
3. See [:material-code-braces: SetIdentityPoolConfigurationResponseTypeDef](./type_defs.md#setidentitypoolconfigurationresponsetypedef) 


```python
# set_identity_pool_configuration method usage example with argument unpacking

kwargs: SetIdentityPoolConfigurationRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
}

parent.set_identity_pool_configuration(**kwargs)
```

1. See [:material-code-braces: SetIdentityPoolConfigurationRequestRequestTypeDef](./type_defs.md#setidentitypoolconfigurationrequestrequesttypedef) 

### subscribe\_to\_dataset

Subscribes to receive notifications when a dataset is modified by another
device.

Type annotations and code completion for `#!python session.create_client("cognito-sync").subscribe_to_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.subscribe_to_dataset)

```python
# subscribe_to_dataset method definition

await def subscribe_to_dataset(
    self,
    *,
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
    DeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# subscribe_to_dataset method usage example with argument unpacking

kwargs: SubscribeToDatasetRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityId": ...,
    "DatasetName": ...,
    "DeviceId": ...,
}

parent.subscribe_to_dataset(**kwargs)
```

1. See [:material-code-braces: SubscribeToDatasetRequestRequestTypeDef](./type_defs.md#subscribetodatasetrequestrequesttypedef) 

### unsubscribe\_from\_dataset

Unsubscribes from receiving notifications when a dataset is modified by another
device.

Type annotations and code completion for `#!python session.create_client("cognito-sync").unsubscribe_from_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.unsubscribe_from_dataset)

```python
# unsubscribe_from_dataset method definition

await def unsubscribe_from_dataset(
    self,
    *,
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
    DeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# unsubscribe_from_dataset method usage example with argument unpacking

kwargs: UnsubscribeFromDatasetRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityId": ...,
    "DatasetName": ...,
    "DeviceId": ...,
}

parent.unsubscribe_from_dataset(**kwargs)
```

1. See [:material-code-braces: UnsubscribeFromDatasetRequestRequestTypeDef](./type_defs.md#unsubscribefromdatasetrequestrequesttypedef) 

### update\_records

Posts updates to records and adds and deletes records for a dataset and user.

Type annotations and code completion for `#!python session.create_client("cognito-sync").update_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.update_records)

```python
# update_records method definition

await def update_records(
    self,
    *,
    IdentityPoolId: str,
    IdentityId: str,
    DatasetName: str,
    SyncSessionToken: str,
    DeviceId: str = ...,
    RecordPatches: Sequence[RecordPatchTypeDef] = ...,  # (1)
    ClientContext: str = ...,
) -> UpdateRecordsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RecordPatchTypeDef](./type_defs.md#recordpatchtypedef) 
2. See [:material-code-braces: UpdateRecordsResponseTypeDef](./type_defs.md#updaterecordsresponsetypedef) 


```python
# update_records method usage example with argument unpacking

kwargs: UpdateRecordsRequestRequestTypeDef = {  # (1)
    "IdentityPoolId": ...,
    "IdentityId": ...,
    "DatasetName": ...,
    "SyncSessionToken": ...,
}

parent.update_records(**kwargs)
```

1. See [:material-code-braces: UpdateRecordsRequestRequestTypeDef](./type_defs.md#updaterecordsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cognito-sync").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CognitoSyncClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cognito-sync").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#CognitoSync.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





