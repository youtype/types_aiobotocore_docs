# CloudTrailClient

> [Index](../README.md) > [CloudTrail](./README.md) > CloudTrailClient

!!! note ""

    Auto-generated documentation for [CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
    type annotations stubs module [types-aiobotocore-cloudtrail](https://pypi.org/project/types-aiobotocore-cloudtrail/).

## CloudTrailClient

Type annotations and code completion for `#!python session.create_client("cloudtrail")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client)

```python
CloudTrailClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cloudtrail.client import CloudTrailClient

session = get_session()
async with session.create_client("cloudtrail") as client:
    client: CloudTrailClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cloudtrail").exceptions` structure.

```python
CloudTrailClient.exceptions usage example

async with session.create_client("cloudtrail") as client:
    try:
        do_something(client)
    except (
            client.AccountHasOngoingImportException,
        client.AccountNotFoundException,
        client.AccountNotRegisteredException,
        client.AccountRegisteredException,
        client.CannotDelegateManagementAccountException,
        client.ChannelARNInvalidException,
        client.ChannelAlreadyExistsException,
        client.ChannelExistsForEDSException,
        client.ChannelMaxLimitExceededException,
        client.ChannelNotFoundException,
        client.ClientError,
        client.CloudTrailARNInvalidException,
        client.CloudTrailAccessNotEnabledException,
        client.CloudTrailInvalidClientTokenIdException,
        client.CloudWatchLogsDeliveryUnavailableException,
        client.ConflictException,
        client.DelegatedAdminAccountLimitExceededException,
        client.EventDataStoreARNInvalidException,
        client.EventDataStoreAlreadyExistsException,
        client.EventDataStoreHasOngoingImportException,
        client.EventDataStoreMaxLimitExceededException,
        client.EventDataStoreNotFoundException,
        client.EventDataStoreTerminationProtectedException,
        client.ImportNotFoundException,
        client.InactiveEventDataStoreException,
        client.InactiveQueryException,
        client.InsightNotEnabledException,
        client.InsufficientDependencyServiceAccessPermissionException,
        client.InsufficientEncryptionPolicyException,
        client.InsufficientS3BucketPolicyException,
        client.InsufficientSnsTopicPolicyException,
        client.InvalidCloudWatchLogsLogGroupArnException,
        client.InvalidCloudWatchLogsRoleArnException,
        client.InvalidDateRangeException,
        client.InvalidEventCategoryException,
        client.InvalidEventDataStoreCategoryException,
        client.InvalidEventDataStoreStatusException,
        client.InvalidEventSelectorsException,
        client.InvalidHomeRegionException,
        client.InvalidImportSourceException,
        client.InvalidInsightSelectorsException,
        client.InvalidKmsKeyIdException,
        client.InvalidLookupAttributesException,
        client.InvalidMaxResultsException,
        client.InvalidNextTokenException,
        client.InvalidParameterCombinationException,
        client.InvalidParameterException,
        client.InvalidQueryStatementException,
        client.InvalidQueryStatusException,
        client.InvalidS3BucketNameException,
        client.InvalidS3PrefixException,
        client.InvalidSnsTopicNameException,
        client.InvalidSourceException,
        client.InvalidTagParameterException,
        client.InvalidTimeRangeException,
        client.InvalidTokenException,
        client.InvalidTrailNameException,
        client.KmsException,
        client.KmsKeyDisabledException,
        client.KmsKeyNotFoundException,
        client.MaxConcurrentQueriesException,
        client.MaximumNumberOfTrailsExceededException,
        client.NoManagementAccountSLRExistsException,
        client.NotOrganizationManagementAccountException,
        client.NotOrganizationMasterAccountException,
        client.OperationNotPermittedException,
        client.OrganizationNotInAllFeaturesModeException,
        client.OrganizationsNotInUseException,
        client.QueryIdNotFoundException,
        client.ResourceARNNotValidException,
        client.ResourceNotFoundException,
        client.ResourcePolicyNotFoundException,
        client.ResourcePolicyNotValidException,
        client.ResourceTypeNotSupportedException,
        client.S3BucketDoesNotExistException,
        client.TagsLimitExceededException,
        client.TrailAlreadyExistsException,
        client.TrailNotFoundException,
        client.TrailNotProvidedException,
        client.UnsupportedOperationException,
    ) as e:
        print(e)
```

```python
CloudTrailClient usage type checking example

from types_aiobotocore_cloudtrail.client import Exceptions

def handle_error(exc: Exceptions.AccountHasOngoingImportException) -> None:
    ...
```


## Methods


### add\_tags

Adds one or more tags to a trail, event data store, or channel, up to a limit of
50.

Type annotations and code completion for `#!python session.create_client("cloudtrail").add_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.add_tags)

```python
# add_tags method definition

await def add_tags(
    self,
    *,
    ResourceId: str,
    TagsList: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# add_tags method usage example with argument unpacking

kwargs: AddTagsRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "TagsList": ...,
}

parent.add_tags(**kwargs)
```

1. See [:material-code-braces: AddTagsRequestRequestTypeDef](./type_defs.md#addtagsrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("cloudtrail").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_query

Cancels a query if the query is not in a terminated state, such as `CANCELLED`,
`FAILED`, `TIMED_OUT`, or `FINISHED`.

Type annotations and code completion for `#!python session.create_client("cloudtrail").cancel_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.cancel_query)

```python
# cancel_query method definition

await def cancel_query(
    self,
    *,
    QueryId: str,
    EventDataStore: str = ...,
) -> CancelQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef) 


```python
# cancel_query method usage example with argument unpacking

kwargs: CancelQueryRequestRequestTypeDef = {  # (1)
    "QueryId": ...,
}

parent.cancel_query(**kwargs)
```

1. See [:material-code-braces: CancelQueryRequestRequestTypeDef](./type_defs.md#cancelqueryrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("cloudtrail").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_channel

Creates a channel for CloudTrail to ingest events from a partner or external
source.

Type annotations and code completion for `#!python session.create_client("cloudtrail").create_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_channel)

```python
# create_channel method definition

await def create_channel(
    self,
    *,
    Name: str,
    Source: str,
    Destinations: Sequence[DestinationTypeDef],  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateChannelResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef) 


```python
# create_channel method usage example with argument unpacking

kwargs: CreateChannelRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Source": ...,
    "Destinations": ...,
}

parent.create_channel(**kwargs)
```

1. See [:material-code-braces: CreateChannelRequestRequestTypeDef](./type_defs.md#createchannelrequestrequesttypedef) 

### create\_event\_data\_store

Creates a new event data store.

Type annotations and code completion for `#!python session.create_client("cloudtrail").create_event_data_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_event_data_store)

```python
# create_event_data_store method definition

await def create_event_data_store(
    self,
    *,
    Name: str,
    AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,  # (1)
    MultiRegionEnabled: bool = ...,
    OrganizationEnabled: bool = ...,
    RetentionPeriod: int = ...,
    TerminationProtectionEnabled: bool = ...,
    TagsList: Sequence[TagTypeDef] = ...,  # (2)
    KmsKeyId: str = ...,
    StartIngestion: bool = ...,
) -> CreateEventDataStoreResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateEventDataStoreResponseTypeDef](./type_defs.md#createeventdatastoreresponsetypedef) 


```python
# create_event_data_store method usage example with argument unpacking

kwargs: CreateEventDataStoreRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_event_data_store(**kwargs)
```

1. See [:material-code-braces: CreateEventDataStoreRequestRequestTypeDef](./type_defs.md#createeventdatastorerequestrequesttypedef) 

### create\_trail

Creates a trail that specifies the settings for delivery of log data to an
Amazon S3 bucket.

Type annotations and code completion for `#!python session.create_client("cloudtrail").create_trail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_trail)

```python
# create_trail method definition

await def create_trail(
    self,
    *,
    Name: str,
    S3BucketName: str,
    S3KeyPrefix: str = ...,
    SnsTopicName: str = ...,
    IncludeGlobalServiceEvents: bool = ...,
    IsMultiRegionTrail: bool = ...,
    EnableLogFileValidation: bool = ...,
    CloudWatchLogsLogGroupArn: str = ...,
    CloudWatchLogsRoleArn: str = ...,
    KmsKeyId: str = ...,
    IsOrganizationTrail: bool = ...,
    TagsList: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateTrailResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateTrailResponseTypeDef](./type_defs.md#createtrailresponsetypedef) 


```python
# create_trail method usage example with argument unpacking

kwargs: CreateTrailRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "S3BucketName": ...,
}

parent.create_trail(**kwargs)
```

1. See [:material-code-braces: CreateTrailRequestRequestTypeDef](./type_defs.md#createtrailrequestrequesttypedef) 

### delete\_channel

Deletes a channel.

Type annotations and code completion for `#!python session.create_client("cloudtrail").delete_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_channel)

```python
# delete_channel method definition

await def delete_channel(
    self,
    *,
    Channel: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_channel method usage example with argument unpacking

kwargs: DeleteChannelRequestRequestTypeDef = {  # (1)
    "Channel": ...,
}

parent.delete_channel(**kwargs)
```

1. See [:material-code-braces: DeleteChannelRequestRequestTypeDef](./type_defs.md#deletechannelrequestrequesttypedef) 

### delete\_event\_data\_store

Disables the event data store specified by `EventDataStore`, which accepts an
event data store ARN.

Type annotations and code completion for `#!python session.create_client("cloudtrail").delete_event_data_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_event_data_store)

```python
# delete_event_data_store method definition

await def delete_event_data_store(
    self,
    *,
    EventDataStore: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_event_data_store method usage example with argument unpacking

kwargs: DeleteEventDataStoreRequestRequestTypeDef = {  # (1)
    "EventDataStore": ...,
}

parent.delete_event_data_store(**kwargs)
```

1. See [:material-code-braces: DeleteEventDataStoreRequestRequestTypeDef](./type_defs.md#deleteeventdatastorerequestrequesttypedef) 

### delete\_resource\_policy

Deletes the resource-based policy attached to the CloudTrail channel.

Type annotations and code completion for `#!python session.create_client("cloudtrail").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_resource_policy)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    ResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef) 

### delete\_trail

Deletes a trail.

Type annotations and code completion for `#!python session.create_client("cloudtrail").delete_trail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_trail)

```python
# delete_trail method definition

await def delete_trail(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_trail method usage example with argument unpacking

kwargs: DeleteTrailRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_trail(**kwargs)
```

1. See [:material-code-braces: DeleteTrailRequestRequestTypeDef](./type_defs.md#deletetrailrequestrequesttypedef) 

### deregister\_organization\_delegated\_admin

Removes CloudTrail delegated administrator permissions from a member account in
an organization.

Type annotations and code completion for `#!python session.create_client("cloudtrail").deregister_organization_delegated_admin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.deregister_organization_delegated_admin)

```python
# deregister_organization_delegated_admin method definition

await def deregister_organization_delegated_admin(
    self,
    *,
    DelegatedAdminAccountId: str,
) -> Dict[str, Any]:
    ...
```



```python
# deregister_organization_delegated_admin method usage example with argument unpacking

kwargs: DeregisterOrganizationDelegatedAdminRequestRequestTypeDef = {  # (1)
    "DelegatedAdminAccountId": ...,
}

parent.deregister_organization_delegated_admin(**kwargs)
```

1. See [:material-code-braces: DeregisterOrganizationDelegatedAdminRequestRequestTypeDef](./type_defs.md#deregisterorganizationdelegatedadminrequestrequesttypedef) 

### describe\_query

Returns metadata about a query, including query run time in milliseconds, number
of events scanned and matched, and query status.

Type annotations and code completion for `#!python session.create_client("cloudtrail").describe_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_query)

```python
# describe_query method definition

await def describe_query(
    self,
    *,
    EventDataStore: str = ...,
    QueryId: str = ...,
    QueryAlias: str = ...,
) -> DescribeQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeQueryResponseTypeDef](./type_defs.md#describequeryresponsetypedef) 


```python
# describe_query method usage example with argument unpacking

kwargs: DescribeQueryRequestRequestTypeDef = {  # (1)
    "EventDataStore": ...,
}

parent.describe_query(**kwargs)
```

1. See [:material-code-braces: DescribeQueryRequestRequestTypeDef](./type_defs.md#describequeryrequestrequesttypedef) 

### describe\_trails

Retrieves settings for one or more trails associated with the current Region for
your account.

Type annotations and code completion for `#!python session.create_client("cloudtrail").describe_trails` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_trails)

```python
# describe_trails method definition

await def describe_trails(
    self,
    *,
    trailNameList: Sequence[str] = ...,
    includeShadowTrails: bool = ...,
) -> DescribeTrailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrailsResponseTypeDef](./type_defs.md#describetrailsresponsetypedef) 


```python
# describe_trails method usage example with argument unpacking

kwargs: DescribeTrailsRequestRequestTypeDef = {  # (1)
    "trailNameList": ...,
}

parent.describe_trails(**kwargs)
```

1. See [:material-code-braces: DescribeTrailsRequestRequestTypeDef](./type_defs.md#describetrailsrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("cloudtrail").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.generate_presigned_url)

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


### get\_channel

Returns information about a specific channel.

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_channel)

```python
# get_channel method definition

await def get_channel(
    self,
    *,
    Channel: str,
) -> GetChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelResponseTypeDef](./type_defs.md#getchannelresponsetypedef) 


```python
# get_channel method usage example with argument unpacking

kwargs: GetChannelRequestRequestTypeDef = {  # (1)
    "Channel": ...,
}

parent.get_channel(**kwargs)
```

1. See [:material-code-braces: GetChannelRequestRequestTypeDef](./type_defs.md#getchannelrequestrequesttypedef) 

### get\_event\_data\_store

Returns information about an event data store specified as either an ARN or the
ID portion of the ARN.

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_event_data_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_event_data_store)

```python
# get_event_data_store method definition

await def get_event_data_store(
    self,
    *,
    EventDataStore: str,
) -> GetEventDataStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventDataStoreResponseTypeDef](./type_defs.md#geteventdatastoreresponsetypedef) 


```python
# get_event_data_store method usage example with argument unpacking

kwargs: GetEventDataStoreRequestRequestTypeDef = {  # (1)
    "EventDataStore": ...,
}

parent.get_event_data_store(**kwargs)
```

1. See [:material-code-braces: GetEventDataStoreRequestRequestTypeDef](./type_defs.md#geteventdatastorerequestrequesttypedef) 

### get\_event\_selectors

Describes the settings for the event selectors that you configured for your
trail.

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_event_selectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_event_selectors)

```python
# get_event_selectors method definition

await def get_event_selectors(
    self,
    *,
    TrailName: str,
) -> GetEventSelectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventSelectorsResponseTypeDef](./type_defs.md#geteventselectorsresponsetypedef) 


```python
# get_event_selectors method usage example with argument unpacking

kwargs: GetEventSelectorsRequestRequestTypeDef = {  # (1)
    "TrailName": ...,
}

parent.get_event_selectors(**kwargs)
```

1. See [:material-code-braces: GetEventSelectorsRequestRequestTypeDef](./type_defs.md#geteventselectorsrequestrequesttypedef) 

### get\_import

Returns information about a specific import.

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_import)

```python
# get_import method definition

await def get_import(
    self,
    *,
    ImportId: str,
) -> GetImportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImportResponseTypeDef](./type_defs.md#getimportresponsetypedef) 


```python
# get_import method usage example with argument unpacking

kwargs: GetImportRequestRequestTypeDef = {  # (1)
    "ImportId": ...,
}

parent.get_import(**kwargs)
```

1. See [:material-code-braces: GetImportRequestRequestTypeDef](./type_defs.md#getimportrequestrequesttypedef) 

### get\_insight\_selectors

Describes the settings for the Insights event selectors that you configured for
your trail.

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_insight_selectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_insight_selectors)

```python
# get_insight_selectors method definition

await def get_insight_selectors(
    self,
    *,
    TrailName: str,
) -> GetInsightSelectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInsightSelectorsResponseTypeDef](./type_defs.md#getinsightselectorsresponsetypedef) 


```python
# get_insight_selectors method usage example with argument unpacking

kwargs: GetInsightSelectorsRequestRequestTypeDef = {  # (1)
    "TrailName": ...,
}

parent.get_insight_selectors(**kwargs)
```

1. See [:material-code-braces: GetInsightSelectorsRequestRequestTypeDef](./type_defs.md#getinsightselectorsrequestrequesttypedef) 

### get\_query\_results

Gets event data results of a query.

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_query_results` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_query_results)

```python
# get_query_results method definition

await def get_query_results(
    self,
    *,
    QueryId: str,
    EventDataStore: str = ...,
    NextToken: str = ...,
    MaxQueryResults: int = ...,
) -> GetQueryResultsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryResultsResponseTypeDef](./type_defs.md#getqueryresultsresponsetypedef) 


```python
# get_query_results method usage example with argument unpacking

kwargs: GetQueryResultsRequestRequestTypeDef = {  # (1)
    "QueryId": ...,
}

parent.get_query_results(**kwargs)
```

1. See [:material-code-braces: GetQueryResultsRequestRequestTypeDef](./type_defs.md#getqueryresultsrequestrequesttypedef) 

### get\_resource\_policy

Retrieves the JSON text of the resource-based policy document attached to the
CloudTrail channel.

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_resource_policy)

```python
# get_resource_policy method definition

await def get_resource_policy(
    self,
    *,
    ResourceArn: str,
) -> GetResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef) 


```python
# get_resource_policy method usage example with argument unpacking

kwargs: GetResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.get_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef) 

### get\_trail

Returns settings information for a specified trail.

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_trail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_trail)

```python
# get_trail method definition

await def get_trail(
    self,
    *,
    Name: str,
) -> GetTrailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrailResponseTypeDef](./type_defs.md#gettrailresponsetypedef) 


```python
# get_trail method usage example with argument unpacking

kwargs: GetTrailRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_trail(**kwargs)
```

1. See [:material-code-braces: GetTrailRequestRequestTypeDef](./type_defs.md#gettrailrequestrequesttypedef) 

### get\_trail\_status

Returns a JSON-formatted list of information about the specified trail.

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_trail_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_trail_status)

```python
# get_trail_status method definition

await def get_trail_status(
    self,
    *,
    Name: str,
) -> GetTrailStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrailStatusResponseTypeDef](./type_defs.md#gettrailstatusresponsetypedef) 


```python
# get_trail_status method usage example with argument unpacking

kwargs: GetTrailStatusRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_trail_status(**kwargs)
```

1. See [:material-code-braces: GetTrailStatusRequestRequestTypeDef](./type_defs.md#gettrailstatusrequestrequesttypedef) 

### list\_channels

Lists the channels in the current account, and their source names.

Type annotations and code completion for `#!python session.create_client("cloudtrail").list_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_channels)

```python
# list_channels method definition

await def list_channels(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# list_channels method usage example with argument unpacking

kwargs: ListChannelsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_channels(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef) 

### list\_event\_data\_stores

Returns information about all event data stores in the account, in the current
Region.

Type annotations and code completion for `#!python session.create_client("cloudtrail").list_event_data_stores` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_event_data_stores)

```python
# list_event_data_stores method definition

await def list_event_data_stores(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEventDataStoresResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventDataStoresResponseTypeDef](./type_defs.md#listeventdatastoresresponsetypedef) 


```python
# list_event_data_stores method usage example with argument unpacking

kwargs: ListEventDataStoresRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_event_data_stores(**kwargs)
```

1. See [:material-code-braces: ListEventDataStoresRequestRequestTypeDef](./type_defs.md#listeventdatastoresrequestrequesttypedef) 

### list\_import\_failures

Returns a list of failures for the specified import.

Type annotations and code completion for `#!python session.create_client("cloudtrail").list_import_failures` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_import_failures)

```python
# list_import_failures method definition

await def list_import_failures(
    self,
    *,
    ImportId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListImportFailuresResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListImportFailuresResponseTypeDef](./type_defs.md#listimportfailuresresponsetypedef) 


```python
# list_import_failures method usage example with argument unpacking

kwargs: ListImportFailuresRequestRequestTypeDef = {  # (1)
    "ImportId": ...,
}

parent.list_import_failures(**kwargs)
```

1. See [:material-code-braces: ListImportFailuresRequestRequestTypeDef](./type_defs.md#listimportfailuresrequestrequesttypedef) 

### list\_imports

Returns information on all imports, or a select set of imports by `ImportStatus`
or `Destination`.

Type annotations and code completion for `#!python session.create_client("cloudtrail").list_imports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_imports)

```python
# list_imports method definition

await def list_imports(
    self,
    *,
    MaxResults: int = ...,
    Destination: str = ...,
    ImportStatus: ImportStatusType = ...,  # (1)
    NextToken: str = ...,
) -> ListImportsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
2. See [:material-code-braces: ListImportsResponseTypeDef](./type_defs.md#listimportsresponsetypedef) 


```python
# list_imports method usage example with argument unpacking

kwargs: ListImportsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_imports(**kwargs)
```

1. See [:material-code-braces: ListImportsRequestRequestTypeDef](./type_defs.md#listimportsrequestrequesttypedef) 

### list\_public\_keys

Returns all public keys whose private keys were used to sign the digest files
within the specified time range.

Type annotations and code completion for `#!python session.create_client("cloudtrail").list_public_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_public_keys)

```python
# list_public_keys method definition

await def list_public_keys(
    self,
    *,
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    NextToken: str = ...,
) -> ListPublicKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef) 


```python
# list_public_keys method usage example with argument unpacking

kwargs: ListPublicKeysRequestRequestTypeDef = {  # (1)
    "StartTime": ...,
}

parent.list_public_keys(**kwargs)
```

1. See [:material-code-braces: ListPublicKeysRequestRequestTypeDef](./type_defs.md#listpublickeysrequestrequesttypedef) 

### list\_queries

Returns a list of queries and query statuses for the past seven days.

Type annotations and code completion for `#!python session.create_client("cloudtrail").list_queries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_queries)

```python
# list_queries method definition

await def list_queries(
    self,
    *,
    EventDataStore: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    QueryStatus: QueryStatusType = ...,  # (1)
) -> ListQueriesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
2. See [:material-code-braces: ListQueriesResponseTypeDef](./type_defs.md#listqueriesresponsetypedef) 


```python
# list_queries method usage example with argument unpacking

kwargs: ListQueriesRequestRequestTypeDef = {  # (1)
    "EventDataStore": ...,
}

parent.list_queries(**kwargs)
```

1. See [:material-code-braces: ListQueriesRequestRequestTypeDef](./type_defs.md#listqueriesrequestrequesttypedef) 

### list\_tags

Lists the tags for the specified trails, event data stores, or channels in the
current Region.

Type annotations and code completion for `#!python session.create_client("cloudtrail").list_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_tags)

```python
# list_tags method definition

await def list_tags(
    self,
    *,
    ResourceIdList: Sequence[str],
    NextToken: str = ...,
) -> ListTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


```python
# list_tags method usage example with argument unpacking

kwargs: ListTagsRequestRequestTypeDef = {  # (1)
    "ResourceIdList": ...,
}

parent.list_tags(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef) 

### list\_trails

Lists trails that are in the current account.

Type annotations and code completion for `#!python session.create_client("cloudtrail").list_trails` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_trails)

```python
# list_trails method definition

await def list_trails(
    self,
    *,
    NextToken: str = ...,
) -> ListTrailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrailsResponseTypeDef](./type_defs.md#listtrailsresponsetypedef) 


```python
# list_trails method usage example with argument unpacking

kwargs: ListTrailsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_trails(**kwargs)
```

1. See [:material-code-braces: ListTrailsRequestRequestTypeDef](./type_defs.md#listtrailsrequestrequesttypedef) 

### lookup\_events

Looks up [management
events](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-
concepts.html#cloudtrail-concepts-management-events)_ or `CloudTrail Insights
events <https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-
concepts.html#cloudtrail-concepts-insigh...`.

Type annotations and code completion for `#!python session.create_client("cloudtrail").lookup_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.lookup_events)

```python
# lookup_events method definition

await def lookup_events(
    self,
    *,
    LookupAttributes: Sequence[LookupAttributeTypeDef] = ...,  # (1)
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    EventCategory: EventCategoryType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> LookupEventsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LookupAttributeTypeDef](./type_defs.md#lookupattributetypedef) 
2. See [:material-code-brackets: EventCategoryType](./literals.md#eventcategorytype) 
3. See [:material-code-braces: LookupEventsResponseTypeDef](./type_defs.md#lookupeventsresponsetypedef) 


```python
# lookup_events method usage example with argument unpacking

kwargs: LookupEventsRequestRequestTypeDef = {  # (1)
    "LookupAttributes": ...,
}

parent.lookup_events(**kwargs)
```

1. See [:material-code-braces: LookupEventsRequestRequestTypeDef](./type_defs.md#lookupeventsrequestrequesttypedef) 

### put\_event\_selectors

Configures an event selector or advanced event selectors for your trail.

Type annotations and code completion for `#!python session.create_client("cloudtrail").put_event_selectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_event_selectors)

```python
# put_event_selectors method definition

await def put_event_selectors(
    self,
    *,
    TrailName: str,
    EventSelectors: Sequence[EventSelectorTypeDef] = ...,  # (1)
    AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,  # (2)
) -> PutEventSelectorsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EventSelectorTypeDef](./type_defs.md#eventselectortypedef) 
2. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
3. See [:material-code-braces: PutEventSelectorsResponseTypeDef](./type_defs.md#puteventselectorsresponsetypedef) 


```python
# put_event_selectors method usage example with argument unpacking

kwargs: PutEventSelectorsRequestRequestTypeDef = {  # (1)
    "TrailName": ...,
}

parent.put_event_selectors(**kwargs)
```

1. See [:material-code-braces: PutEventSelectorsRequestRequestTypeDef](./type_defs.md#puteventselectorsrequestrequesttypedef) 

### put\_insight\_selectors

Lets you enable Insights event logging by specifying the Insights selectors that
you want to enable on an existing trail.

Type annotations and code completion for `#!python session.create_client("cloudtrail").put_insight_selectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_insight_selectors)

```python
# put_insight_selectors method definition

await def put_insight_selectors(
    self,
    *,
    TrailName: str,
    InsightSelectors: Sequence[InsightSelectorTypeDef],  # (1)
) -> PutInsightSelectorsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InsightSelectorTypeDef](./type_defs.md#insightselectortypedef) 
2. See [:material-code-braces: PutInsightSelectorsResponseTypeDef](./type_defs.md#putinsightselectorsresponsetypedef) 


```python
# put_insight_selectors method usage example with argument unpacking

kwargs: PutInsightSelectorsRequestRequestTypeDef = {  # (1)
    "TrailName": ...,
    "InsightSelectors": ...,
}

parent.put_insight_selectors(**kwargs)
```

1. See [:material-code-braces: PutInsightSelectorsRequestRequestTypeDef](./type_defs.md#putinsightselectorsrequestrequesttypedef) 

### put\_resource\_policy

Attaches a resource-based permission policy to a CloudTrail channel that is used
for an integration with an event source outside of Amazon Web Services.

Type annotations and code completion for `#!python session.create_client("cloudtrail").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_resource_policy)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    ResourceArn: str,
    ResourcePolicy: str,
) -> PutResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef) 


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "ResourcePolicy": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef) 

### register\_organization\_delegated\_admin

Registers an organization’s member account as the CloudTrail delegated
administrator.

Type annotations and code completion for `#!python session.create_client("cloudtrail").register_organization_delegated_admin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.register_organization_delegated_admin)

```python
# register_organization_delegated_admin method definition

await def register_organization_delegated_admin(
    self,
    *,
    MemberAccountId: str,
) -> Dict[str, Any]:
    ...
```



```python
# register_organization_delegated_admin method usage example with argument unpacking

kwargs: RegisterOrganizationDelegatedAdminRequestRequestTypeDef = {  # (1)
    "MemberAccountId": ...,
}

parent.register_organization_delegated_admin(**kwargs)
```

1. See [:material-code-braces: RegisterOrganizationDelegatedAdminRequestRequestTypeDef](./type_defs.md#registerorganizationdelegatedadminrequestrequesttypedef) 

### remove\_tags

Removes the specified tags from a trail, event data store, or channel.

Type annotations and code completion for `#!python session.create_client("cloudtrail").remove_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.remove_tags)

```python
# remove_tags method definition

await def remove_tags(
    self,
    *,
    ResourceId: str,
    TagsList: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# remove_tags method usage example with argument unpacking

kwargs: RemoveTagsRequestRequestTypeDef = {  # (1)
    "ResourceId": ...,
    "TagsList": ...,
}

parent.remove_tags(**kwargs)
```

1. See [:material-code-braces: RemoveTagsRequestRequestTypeDef](./type_defs.md#removetagsrequestrequesttypedef) 

### restore\_event\_data\_store

Restores a deleted event data store specified by `EventDataStore`, which accepts
an event data store ARN.

Type annotations and code completion for `#!python session.create_client("cloudtrail").restore_event_data_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.restore_event_data_store)

```python
# restore_event_data_store method definition

await def restore_event_data_store(
    self,
    *,
    EventDataStore: str,
) -> RestoreEventDataStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestoreEventDataStoreResponseTypeDef](./type_defs.md#restoreeventdatastoreresponsetypedef) 


```python
# restore_event_data_store method usage example with argument unpacking

kwargs: RestoreEventDataStoreRequestRequestTypeDef = {  # (1)
    "EventDataStore": ...,
}

parent.restore_event_data_store(**kwargs)
```

1. See [:material-code-braces: RestoreEventDataStoreRequestRequestTypeDef](./type_defs.md#restoreeventdatastorerequestrequesttypedef) 

### start\_event\_data\_store\_ingestion

Starts the ingestion of live events on an event data store specified as either
an ARN or the ID portion of the ARN.

Type annotations and code completion for `#!python session.create_client("cloudtrail").start_event_data_store_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_event_data_store_ingestion)

```python
# start_event_data_store_ingestion method definition

await def start_event_data_store_ingestion(
    self,
    *,
    EventDataStore: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_event_data_store_ingestion method usage example with argument unpacking

kwargs: StartEventDataStoreIngestionRequestRequestTypeDef = {  # (1)
    "EventDataStore": ...,
}

parent.start_event_data_store_ingestion(**kwargs)
```

1. See [:material-code-braces: StartEventDataStoreIngestionRequestRequestTypeDef](./type_defs.md#starteventdatastoreingestionrequestrequesttypedef) 

### start\_import

Starts an import of logged trail events from a source S3 bucket to a destination
event data store.

Type annotations and code completion for `#!python session.create_client("cloudtrail").start_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_import)

```python
# start_import method definition

await def start_import(
    self,
    *,
    Destinations: Sequence[str] = ...,
    ImportSource: ImportSourceTypeDef = ...,  # (1)
    StartEventTime: Union[datetime, str] = ...,
    EndEventTime: Union[datetime, str] = ...,
    ImportId: str = ...,
) -> StartImportResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ImportSourceTypeDef](./type_defs.md#importsourcetypedef) 
2. See [:material-code-braces: StartImportResponseTypeDef](./type_defs.md#startimportresponsetypedef) 


```python
# start_import method usage example with argument unpacking

kwargs: StartImportRequestRequestTypeDef = {  # (1)
    "Destinations": ...,
}

parent.start_import(**kwargs)
```

1. See [:material-code-braces: StartImportRequestRequestTypeDef](./type_defs.md#startimportrequestrequesttypedef) 

### start\_logging

Starts the recording of Amazon Web Services API calls and log file delivery for
a trail.

Type annotations and code completion for `#!python session.create_client("cloudtrail").start_logging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_logging)

```python
# start_logging method definition

await def start_logging(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_logging method usage example with argument unpacking

kwargs: StartLoggingRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.start_logging(**kwargs)
```

1. See [:material-code-braces: StartLoggingRequestRequestTypeDef](./type_defs.md#startloggingrequestrequesttypedef) 

### start\_query

Starts a CloudTrail Lake query.

Type annotations and code completion for `#!python session.create_client("cloudtrail").start_query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_query)

```python
# start_query method definition

await def start_query(
    self,
    *,
    QueryStatement: str = ...,
    DeliveryS3Uri: str = ...,
    QueryAlias: str = ...,
    QueryParameters: Sequence[str] = ...,
) -> StartQueryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartQueryResponseTypeDef](./type_defs.md#startqueryresponsetypedef) 


```python
# start_query method usage example with argument unpacking

kwargs: StartQueryRequestRequestTypeDef = {  # (1)
    "QueryStatement": ...,
}

parent.start_query(**kwargs)
```

1. See [:material-code-braces: StartQueryRequestRequestTypeDef](./type_defs.md#startqueryrequestrequesttypedef) 

### stop\_event\_data\_store\_ingestion

Stops the ingestion of live events on an event data store specified as either an
ARN or the ID portion of the ARN.

Type annotations and code completion for `#!python session.create_client("cloudtrail").stop_event_data_store_ingestion` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_event_data_store_ingestion)

```python
# stop_event_data_store_ingestion method definition

await def stop_event_data_store_ingestion(
    self,
    *,
    EventDataStore: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_event_data_store_ingestion method usage example with argument unpacking

kwargs: StopEventDataStoreIngestionRequestRequestTypeDef = {  # (1)
    "EventDataStore": ...,
}

parent.stop_event_data_store_ingestion(**kwargs)
```

1. See [:material-code-braces: StopEventDataStoreIngestionRequestRequestTypeDef](./type_defs.md#stopeventdatastoreingestionrequestrequesttypedef) 

### stop\_import

Stops a specified import.

Type annotations and code completion for `#!python session.create_client("cloudtrail").stop_import` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_import)

```python
# stop_import method definition

await def stop_import(
    self,
    *,
    ImportId: str,
) -> StopImportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopImportResponseTypeDef](./type_defs.md#stopimportresponsetypedef) 


```python
# stop_import method usage example with argument unpacking

kwargs: StopImportRequestRequestTypeDef = {  # (1)
    "ImportId": ...,
}

parent.stop_import(**kwargs)
```

1. See [:material-code-braces: StopImportRequestRequestTypeDef](./type_defs.md#stopimportrequestrequesttypedef) 

### stop\_logging

Suspends the recording of Amazon Web Services API calls and log file delivery
for the specified trail.

Type annotations and code completion for `#!python session.create_client("cloudtrail").stop_logging` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_logging)

```python
# stop_logging method definition

await def stop_logging(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_logging method usage example with argument unpacking

kwargs: StopLoggingRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.stop_logging(**kwargs)
```

1. See [:material-code-braces: StopLoggingRequestRequestTypeDef](./type_defs.md#stoploggingrequestrequesttypedef) 

### update\_channel

Updates a channel specified by a required channel ARN or UUID.

Type annotations and code completion for `#!python session.create_client("cloudtrail").update_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_channel)

```python
# update_channel method definition

await def update_channel(
    self,
    *,
    Channel: str,
    Destinations: Sequence[DestinationTypeDef] = ...,  # (1)
    Name: str = ...,
) -> UpdateChannelResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef) 


```python
# update_channel method usage example with argument unpacking

kwargs: UpdateChannelRequestRequestTypeDef = {  # (1)
    "Channel": ...,
}

parent.update_channel(**kwargs)
```

1. See [:material-code-braces: UpdateChannelRequestRequestTypeDef](./type_defs.md#updatechannelrequestrequesttypedef) 

### update\_event\_data\_store

Updates an event data store.

Type annotations and code completion for `#!python session.create_client("cloudtrail").update_event_data_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_event_data_store)

```python
# update_event_data_store method definition

await def update_event_data_store(
    self,
    *,
    EventDataStore: str,
    Name: str = ...,
    AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,  # (1)
    MultiRegionEnabled: bool = ...,
    OrganizationEnabled: bool = ...,
    RetentionPeriod: int = ...,
    TerminationProtectionEnabled: bool = ...,
    KmsKeyId: str = ...,
) -> UpdateEventDataStoreResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
2. See [:material-code-braces: UpdateEventDataStoreResponseTypeDef](./type_defs.md#updateeventdatastoreresponsetypedef) 


```python
# update_event_data_store method usage example with argument unpacking

kwargs: UpdateEventDataStoreRequestRequestTypeDef = {  # (1)
    "EventDataStore": ...,
}

parent.update_event_data_store(**kwargs)
```

1. See [:material-code-braces: UpdateEventDataStoreRequestRequestTypeDef](./type_defs.md#updateeventdatastorerequestrequesttypedef) 

### update\_trail

Updates trail settings that control what events you are logging, and how to
handle log files.

Type annotations and code completion for `#!python session.create_client("cloudtrail").update_trail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_trail)

```python
# update_trail method definition

await def update_trail(
    self,
    *,
    Name: str,
    S3BucketName: str = ...,
    S3KeyPrefix: str = ...,
    SnsTopicName: str = ...,
    IncludeGlobalServiceEvents: bool = ...,
    IsMultiRegionTrail: bool = ...,
    EnableLogFileValidation: bool = ...,
    CloudWatchLogsLogGroupArn: str = ...,
    CloudWatchLogsRoleArn: str = ...,
    KmsKeyId: str = ...,
    IsOrganizationTrail: bool = ...,
) -> UpdateTrailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateTrailResponseTypeDef](./type_defs.md#updatetrailresponsetypedef) 


```python
# update_trail method usage example with argument unpacking

kwargs: UpdateTrailRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_trail(**kwargs)
```

1. See [:material-code-braces: UpdateTrailRequestRequestTypeDef](./type_defs.md#updatetrailrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cloudtrail").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> CloudTrailClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cloudtrail").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.__aexit__)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("cloudtrail").get_paginator` method with overloads.

- `client.get_paginator("list_import_failures")` -> [ListImportFailuresPaginator](./paginators.md#listimportfailurespaginator)
- `client.get_paginator("list_imports")` -> [ListImportsPaginator](./paginators.md#listimportspaginator)
- `client.get_paginator("list_public_keys")` -> [ListPublicKeysPaginator](./paginators.md#listpublickeyspaginator)
- `client.get_paginator("list_tags")` -> [ListTagsPaginator](./paginators.md#listtagspaginator)
- `client.get_paginator("list_trails")` -> [ListTrailsPaginator](./paginators.md#listtrailspaginator)
- `client.get_paginator("lookup_events")` -> [LookupEventsPaginator](./paginators.md#lookupeventspaginator)



