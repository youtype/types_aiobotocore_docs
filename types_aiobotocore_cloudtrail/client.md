<a id="cloudtrailclient-for-aiobotocore-cloudtrail-module"></a>

# CloudTrailClient for aiobotocore CloudTrail module

> [Index](..) > [CloudTrail](.) > CloudTrailClient

Auto-generated documentation for
[CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
type annotations stubs module
[types-aiobotocore-cloudtrail](https://pypi.org/project/types-aiobotocore-cloudtrail/).

- [CloudTrailClient for aiobotocore CloudTrail module](#cloudtrailclient-for-aiobotocore-cloudtrail-module)
  - [CloudTrailClient](#cloudtrailclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [add_tags](#add_tags)
    - [can_paginate](#can_paginate)
    - [create_trail](#create_trail)
    - [delete_trail](#delete_trail)
    - [describe_trails](#describe_trails)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_event_selectors](#get_event_selectors)
    - [get_insight_selectors](#get_insight_selectors)
    - [get_trail](#get_trail)
    - [get_trail_status](#get_trail_status)
    - [list_public_keys](#list_public_keys)
    - [list_tags](#list_tags)
    - [list_trails](#list_trails)
    - [lookup_events](#lookup_events)
    - [put_event_selectors](#put_event_selectors)
    - [put_insight_selectors](#put_insight_selectors)
    - [remove_tags](#remove_tags)
    - [start_logging](#start_logging)
    - [stop_logging](#stop_logging)
    - [update_trail](#update_trail)
    - [get_paginator](#get_paginator)

<a id="cloudtrailclient"></a>

## CloudTrailClient

Type annotations for `aiobotocore.create_client("cloudtrail")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_cloudtrail.client import CloudTrailClient

def get_cloudtrail_client() -> CloudTrailClient:
    return Session().client("cloudtrail")
```

Boto3 documentation:
[CloudTrail.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_cloudtrail.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.CloudTrailARNInvalidException`
- `Exceptions.CloudTrailAccessNotEnabledException`
- `Exceptions.CloudTrailInvalidClientTokenIdException`
- `Exceptions.CloudWatchLogsDeliveryUnavailableException`
- `Exceptions.ConflictException`
- `Exceptions.InsightNotEnabledException`
- `Exceptions.InsufficientDependencyServiceAccessPermissionException`
- `Exceptions.InsufficientEncryptionPolicyException`
- `Exceptions.InsufficientS3BucketPolicyException`
- `Exceptions.InsufficientSnsTopicPolicyException`
- `Exceptions.InvalidCloudWatchLogsLogGroupArnException`
- `Exceptions.InvalidCloudWatchLogsRoleArnException`
- `Exceptions.InvalidEventCategoryException`
- `Exceptions.InvalidEventSelectorsException`
- `Exceptions.InvalidHomeRegionException`
- `Exceptions.InvalidInsightSelectorsException`
- `Exceptions.InvalidKmsKeyIdException`
- `Exceptions.InvalidLookupAttributesException`
- `Exceptions.InvalidMaxResultsException`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.InvalidParameterCombinationException`
- `Exceptions.InvalidS3BucketNameException`
- `Exceptions.InvalidS3PrefixException`
- `Exceptions.InvalidSnsTopicNameException`
- `Exceptions.InvalidTagParameterException`
- `Exceptions.InvalidTimeRangeException`
- `Exceptions.InvalidTokenException`
- `Exceptions.InvalidTrailNameException`
- `Exceptions.KmsException`
- `Exceptions.KmsKeyDisabledException`
- `Exceptions.KmsKeyNotFoundException`
- `Exceptions.MaximumNumberOfTrailsExceededException`
- `Exceptions.NotOrganizationMasterAccountException`
- `Exceptions.OperationNotPermittedException`
- `Exceptions.OrganizationNotInAllFeaturesModeException`
- `Exceptions.OrganizationsNotInUseException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ResourceTypeNotSupportedException`
- `Exceptions.S3BucketDoesNotExistException`
- `Exceptions.TagsLimitExceededException`
- `Exceptions.TrailAlreadyExistsException`
- `Exceptions.TrailNotFoundException`
- `Exceptions.TrailNotProvidedException`
- `Exceptions.UnsupportedOperationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CloudTrailClient exceptions.

Type annotations for `aiobotocore.create_client("cloudtrail").exceptions`
method.

Boto3 documentation:
[CloudTrail.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="add_tags"></a>

### add_tags

Adds one or more tags to a trail, up to a limit of 50.

Type annotations for `aiobotocore.create_client("cloudtrail").add_tags` method.

Boto3 documentation:
[CloudTrail.Client.add_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.add_tags)

Asynchronous method. Use `await add_tags(...)` for a synchronous call.

Arguments mapping described in
[AddTagsRequestRequestTypeDef](./type_defs.md#addtagsrequestrequesttypedef).

Keyword-only arguments:

- `ResourceId`: `str` *(required)*
- `TagsList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("cloudtrail").can_paginate`
method.

Boto3 documentation:
[CloudTrail.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_trail"></a>

### create_trail

Creates a trail that specifies the settings for delivery of log data to an
Amazon S3 bucket.

Type annotations for `aiobotocore.create_client("cloudtrail").create_trail`
method.

Boto3 documentation:
[CloudTrail.Client.create_trail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_trail)

Asynchronous method. Use `await create_trail(...)` for a synchronous call.

Arguments mapping described in
[CreateTrailRequestRequestTypeDef](./type_defs.md#createtrailrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `S3BucketName`: `str` *(required)*
- `S3KeyPrefix`: `str`
- `SnsTopicName`: `str`
- `IncludeGlobalServiceEvents`: `bool`
- `IsMultiRegionTrail`: `bool`
- `EnableLogFileValidation`: `bool`
- `CloudWatchLogsLogGroupArn`: `str`
- `CloudWatchLogsRoleArn`: `str`
- `KmsKeyId`: `str`
- `IsOrganizationTrail`: `bool`
- `TagsList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateTrailResponseTypeDef](./type_defs.md#createtrailresponsetypedef).

<a id="delete_trail"></a>

### delete_trail

Deletes a trail.

Type annotations for `aiobotocore.create_client("cloudtrail").delete_trail`
method.

Boto3 documentation:
[CloudTrail.Client.delete_trail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.delete_trail)

Asynchronous method. Use `await delete_trail(...)` for a synchronous call.

Arguments mapping described in
[DeleteTrailRequestRequestTypeDef](./type_defs.md#deletetrailrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_trails"></a>

### describe_trails

Retrieves settings for one or more trails associated with the current region
for your account.

Type annotations for `aiobotocore.create_client("cloudtrail").describe_trails`
method.

Boto3 documentation:
[CloudTrail.Client.describe_trails](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.describe_trails)

Asynchronous method. Use `await describe_trails(...)` for a synchronous call.

Arguments mapping described in
[DescribeTrailsRequestRequestTypeDef](./type_defs.md#describetrailsrequestrequesttypedef).

Keyword-only arguments:

- `trailNameList`: `Sequence`\[`str`\]
- `includeShadowTrails`: `bool`

Returns a `Coroutine` for
[DescribeTrailsResponseTypeDef](./type_defs.md#describetrailsresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("cloudtrail").generate_presigned_url` method.

Boto3 documentation:
[CloudTrail.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_event_selectors"></a>

### get_event_selectors

Describes the settings for the event selectors that you configured for your
trail.

Type annotations for
`aiobotocore.create_client("cloudtrail").get_event_selectors` method.

Boto3 documentation:
[CloudTrail.Client.get_event_selectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_event_selectors)

Asynchronous method. Use `await get_event_selectors(...)` for a synchronous
call.

Arguments mapping described in
[GetEventSelectorsRequestRequestTypeDef](./type_defs.md#geteventselectorsrequestrequesttypedef).

Keyword-only arguments:

- `TrailName`: `str` *(required)*

Returns a `Coroutine` for
[GetEventSelectorsResponseTypeDef](./type_defs.md#geteventselectorsresponsetypedef).

<a id="get_insight_selectors"></a>

### get_insight_selectors

Describes the settings for the Insights event selectors that you configured for
your trail.

Type annotations for
`aiobotocore.create_client("cloudtrail").get_insight_selectors` method.

Boto3 documentation:
[CloudTrail.Client.get_insight_selectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_insight_selectors)

Asynchronous method. Use `await get_insight_selectors(...)` for a synchronous
call.

Arguments mapping described in
[GetInsightSelectorsRequestRequestTypeDef](./type_defs.md#getinsightselectorsrequestrequesttypedef).

Keyword-only arguments:

- `TrailName`: `str` *(required)*

Returns a `Coroutine` for
[GetInsightSelectorsResponseTypeDef](./type_defs.md#getinsightselectorsresponsetypedef).

<a id="get_trail"></a>

### get_trail

Returns settings information for a specified trail.

Type annotations for `aiobotocore.create_client("cloudtrail").get_trail`
method.

Boto3 documentation:
[CloudTrail.Client.get_trail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_trail)

Asynchronous method. Use `await get_trail(...)` for a synchronous call.

Arguments mapping described in
[GetTrailRequestRequestTypeDef](./type_defs.md#gettrailrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[GetTrailResponseTypeDef](./type_defs.md#gettrailresponsetypedef).

<a id="get_trail_status"></a>

### get_trail_status

Returns a JSON-formatted list of information about the specified trail.

Type annotations for `aiobotocore.create_client("cloudtrail").get_trail_status`
method.

Boto3 documentation:
[CloudTrail.Client.get_trail_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.get_trail_status)

Asynchronous method. Use `await get_trail_status(...)` for a synchronous call.

Arguments mapping described in
[GetTrailStatusRequestRequestTypeDef](./type_defs.md#gettrailstatusrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[GetTrailStatusResponseTypeDef](./type_defs.md#gettrailstatusresponsetypedef).

<a id="list_public_keys"></a>

### list_public_keys

Returns all public keys whose private keys were used to sign the digest files
within the specified time range.

Type annotations for `aiobotocore.create_client("cloudtrail").list_public_keys`
method.

Boto3 documentation:
[CloudTrail.Client.list_public_keys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_public_keys)

Asynchronous method. Use `await list_public_keys(...)` for a synchronous call.

Arguments mapping described in
[ListPublicKeysRequestRequestTypeDef](./type_defs.md#listpublickeysrequestrequesttypedef).

Keyword-only arguments:

- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `NextToken`: `str`

Returns a `Coroutine` for
[ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef).

<a id="list_tags"></a>

### list_tags

Lists the tags for the trail in the current region.

Type annotations for `aiobotocore.create_client("cloudtrail").list_tags`
method.

Boto3 documentation:
[CloudTrail.Client.list_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_tags)

Asynchronous method. Use `await list_tags(...)` for a synchronous call.

Arguments mapping described in
[ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef).

Keyword-only arguments:

- `ResourceIdList`: `Sequence`\[`str`\] *(required)*
- `NextToken`: `str`

Returns a `Coroutine` for
[ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef).

<a id="list_trails"></a>

### list_trails

Lists trails that are in the current account.

Type annotations for `aiobotocore.create_client("cloudtrail").list_trails`
method.

Boto3 documentation:
[CloudTrail.Client.list_trails](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.list_trails)

Asynchronous method. Use `await list_trails(...)` for a synchronous call.

Arguments mapping described in
[ListTrailsRequestRequestTypeDef](./type_defs.md#listtrailsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`

Returns a `Coroutine` for
[ListTrailsResponseTypeDef](./type_defs.md#listtrailsresponsetypedef).

<a id="lookup_events"></a>

### lookup_events

Looks up \[management
events\](https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail-
concepts.html#cloudtrail-concepts-management-events)\_ or
`CloudTrail Insights events <https://docs.aws.amazon.com/awscloudtrail/latest/userguide/cloudtrail- concepts.html#cloudtrail-concepts-insigh...`.

Type annotations for `aiobotocore.create_client("cloudtrail").lookup_events`
method.

Boto3 documentation:
[CloudTrail.Client.lookup_events](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.lookup_events)

Asynchronous method. Use `await lookup_events(...)` for a synchronous call.

Arguments mapping described in
[LookupEventsRequestRequestTypeDef](./type_defs.md#lookupeventsrequestrequesttypedef).

Keyword-only arguments:

- `LookupAttributes`:
  `Sequence`\[[LookupAttributeTypeDef](./type_defs.md#lookupattributetypedef)\]
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `EventCategory`: `Literal['insight']` (see
  [EventCategoryType](./literals.md#eventcategorytype))
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[LookupEventsResponseTypeDef](./type_defs.md#lookupeventsresponsetypedef).

<a id="put_event_selectors"></a>

### put_event_selectors

Configures an event selector or advanced event selectors for your trail.

Type annotations for
`aiobotocore.create_client("cloudtrail").put_event_selectors` method.

Boto3 documentation:
[CloudTrail.Client.put_event_selectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_event_selectors)

Asynchronous method. Use `await put_event_selectors(...)` for a synchronous
call.

Arguments mapping described in
[PutEventSelectorsRequestRequestTypeDef](./type_defs.md#puteventselectorsrequestrequesttypedef).

Keyword-only arguments:

- `TrailName`: `str` *(required)*
- `EventSelectors`:
  `Sequence`\[[EventSelectorTypeDef](./type_defs.md#eventselectortypedef)\]
- `AdvancedEventSelectors`:
  `Sequence`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]

Returns a `Coroutine` for
[PutEventSelectorsResponseTypeDef](./type_defs.md#puteventselectorsresponsetypedef).

<a id="put_insight_selectors"></a>

### put_insight_selectors

Lets you enable Insights event logging by specifying the Insights selectors
that you want to enable on an existing trail.

Type annotations for
`aiobotocore.create_client("cloudtrail").put_insight_selectors` method.

Boto3 documentation:
[CloudTrail.Client.put_insight_selectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_insight_selectors)

Asynchronous method. Use `await put_insight_selectors(...)` for a synchronous
call.

Arguments mapping described in
[PutInsightSelectorsRequestRequestTypeDef](./type_defs.md#putinsightselectorsrequestrequesttypedef).

Keyword-only arguments:

- `TrailName`: `str` *(required)*
- `InsightSelectors`:
  `Sequence`\[[InsightSelectorTypeDef](./type_defs.md#insightselectortypedef)\]
  *(required)*

Returns a `Coroutine` for
[PutInsightSelectorsResponseTypeDef](./type_defs.md#putinsightselectorsresponsetypedef).

<a id="remove_tags"></a>

### remove_tags

Removes the specified tags from a trail.

Type annotations for `aiobotocore.create_client("cloudtrail").remove_tags`
method.

Boto3 documentation:
[CloudTrail.Client.remove_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.remove_tags)

Asynchronous method. Use `await remove_tags(...)` for a synchronous call.

Arguments mapping described in
[RemoveTagsRequestRequestTypeDef](./type_defs.md#removetagsrequestrequesttypedef).

Keyword-only arguments:

- `ResourceId`: `str` *(required)*
- `TagsList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="start_logging"></a>

### start_logging

Starts the recording of Amazon Web Services API calls and log file delivery for
a trail.

Type annotations for `aiobotocore.create_client("cloudtrail").start_logging`
method.

Boto3 documentation:
[CloudTrail.Client.start_logging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.start_logging)

Asynchronous method. Use `await start_logging(...)` for a synchronous call.

Arguments mapping described in
[StartLoggingRequestRequestTypeDef](./type_defs.md#startloggingrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="stop_logging"></a>

### stop_logging

Suspends the recording of Amazon Web Services API calls and log file delivery
for the specified trail.

Type annotations for `aiobotocore.create_client("cloudtrail").stop_logging`
method.

Boto3 documentation:
[CloudTrail.Client.stop_logging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.stop_logging)

Asynchronous method. Use `await stop_logging(...)` for a synchronous call.

Arguments mapping described in
[StopLoggingRequestRequestTypeDef](./type_defs.md#stoploggingrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_trail"></a>

### update_trail

Updates trail settings that control what events you are logging, and how to
handle log files.

Type annotations for `aiobotocore.create_client("cloudtrail").update_trail`
method.

Boto3 documentation:
[CloudTrail.Client.update_trail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.update_trail)

Asynchronous method. Use `await update_trail(...)` for a synchronous call.

Arguments mapping described in
[UpdateTrailRequestRequestTypeDef](./type_defs.md#updatetrailrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `S3BucketName`: `str`
- `S3KeyPrefix`: `str`
- `SnsTopicName`: `str`
- `IncludeGlobalServiceEvents`: `bool`
- `IsMultiRegionTrail`: `bool`
- `EnableLogFileValidation`: `bool`
- `CloudWatchLogsLogGroupArn`: `str`
- `CloudWatchLogsRoleArn`: `str`
- `KmsKeyId`: `str`
- `IsOrganizationTrail`: `bool`

Returns a `Coroutine` for
[UpdateTrailResponseTypeDef](./type_defs.md#updatetrailresponsetypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("cloudtrail").get_paginator`
method with overloads.

- `client.get_paginator("list_public_keys")` ->
  [ListPublicKeysPaginator](./paginators.md#listpublickeyspaginator)
- `client.get_paginator("list_tags")` ->
  [ListTagsPaginator](./paginators.md#listtagspaginator)
- `client.get_paginator("list_trails")` ->
  [ListTrailsPaginator](./paginators.md#listtrailspaginator)
- `client.get_paginator("lookup_events")` ->
  [LookupEventsPaginator](./paginators.md#lookupeventspaginator)
