<a id="timestreamqueryclient-for-aiobotocore-timestreamquery-module"></a>

# TimestreamQueryClient for aiobotocore TimestreamQuery module

> [Index](..) > [TimestreamQuery](.) > TimestreamQueryClient

Auto-generated documentation for
[TimestreamQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
type annotations stubs module
[types-aiobotocore-timestream-query](https://pypi.org/project/types-aiobotocore-timestream-query/).

- [TimestreamQueryClient for aiobotocore TimestreamQuery module](#timestreamqueryclient-for-aiobotocore-timestreamquery-module)
  - [TimestreamQueryClient](#timestreamqueryclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [cancel_query](#cancel_query)
    - [create_scheduled_query](#create_scheduled_query)
    - [delete_scheduled_query](#delete_scheduled_query)
    - [describe_endpoints](#describe_endpoints)
    - [describe_scheduled_query](#describe_scheduled_query)
    - [execute_scheduled_query](#execute_scheduled_query)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_scheduled_queries](#list_scheduled_queries)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [prepare_query](#prepare_query)
    - [query](#query)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_scheduled_query](#update_scheduled_query)
    - [get_paginator](#get_paginator)

<a id="timestreamqueryclient"></a>

## TimestreamQueryClient

Type annotations for `aiobotocore.create_client("timestream-query")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_timestream_query.client import TimestreamQueryClient

def get_timestream-query_client() -> TimestreamQueryClient:
    return Session().client("timestream-query")
```

Boto3 documentation:
[TimestreamQuery.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_timestream_query.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.InvalidEndpointException`
- `Exceptions.QueryExecutionException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

TimestreamQueryClient exceptions.

Type annotations for `aiobotocore.create_client("timestream-query").exceptions`
method.

Boto3 documentation:
[TimestreamQuery.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`aiobotocore.create_client("timestream-query").can_paginate` method.

Boto3 documentation:
[TimestreamQuery.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="cancel_query"></a>

### cancel_query

Cancels a query that has been issued.

Type annotations for
`aiobotocore.create_client("timestream-query").cancel_query` method.

Boto3 documentation:
[TimestreamQuery.Client.cancel_query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.cancel_query)

Asynchronous method. Use `await cancel_query(...)` for a synchronous call.

Arguments mapping described in
[CancelQueryRequestRequestTypeDef](./type_defs.md#cancelqueryrequestrequesttypedef).

Keyword-only arguments:

- `QueryId`: `str` *(required)*

Returns a `Coroutine` for
[CancelQueryResponseTypeDef](./type_defs.md#cancelqueryresponsetypedef).

<a id="create_scheduled_query"></a>

### create_scheduled_query

Create a scheduled query that will be run on your behalf at the configured
schedule.

Type annotations for
`aiobotocore.create_client("timestream-query").create_scheduled_query` method.

Boto3 documentation:
[TimestreamQuery.Client.create_scheduled_query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.create_scheduled_query)

Asynchronous method. Use `await create_scheduled_query(...)` for a synchronous
call.

Arguments mapping described in
[CreateScheduledQueryRequestRequestTypeDef](./type_defs.md#createscheduledqueryrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `QueryString`: `str` *(required)*
- `ScheduleConfiguration`:
  [ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef)
  *(required)*
- `NotificationConfiguration`:
  [NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef)
  *(required)*
- `ScheduledQueryExecutionRoleArn`: `str` *(required)*
- `ErrorReportConfiguration`:
  [ErrorReportConfigurationTypeDef](./type_defs.md#errorreportconfigurationtypedef)
  *(required)*
- `TargetConfiguration`:
  [TargetConfigurationTypeDef](./type_defs.md#targetconfigurationtypedef)
- `ClientToken`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `KmsKeyId`: `str`

Returns a `Coroutine` for
[CreateScheduledQueryResponseTypeDef](./type_defs.md#createscheduledqueryresponsetypedef).

<a id="delete_scheduled_query"></a>

### delete_scheduled_query

Deletes a given scheduled query.

Type annotations for
`aiobotocore.create_client("timestream-query").delete_scheduled_query` method.

Boto3 documentation:
[TimestreamQuery.Client.delete_scheduled_query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.delete_scheduled_query)

Asynchronous method. Use `await delete_scheduled_query(...)` for a synchronous
call.

Arguments mapping described in
[DeleteScheduledQueryRequestRequestTypeDef](./type_defs.md#deletescheduledqueryrequestrequesttypedef).

Keyword-only arguments:

- `ScheduledQueryArn`: `str` *(required)*

<a id="describe_endpoints"></a>

### describe_endpoints

DescribeEndpoints returns a list of available endpoints to make Timestream API
calls against.

Type annotations for
`aiobotocore.create_client("timestream-query").describe_endpoints` method.

Boto3 documentation:
[TimestreamQuery.Client.describe_endpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.describe_endpoints)

Asynchronous method. Use `await describe_endpoints(...)` for a synchronous
call.

Returns a `Coroutine` for
[DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef).

<a id="describe_scheduled_query"></a>

### describe_scheduled_query

Provides detailed information about a scheduled query.

Type annotations for
`aiobotocore.create_client("timestream-query").describe_scheduled_query`
method.

Boto3 documentation:
[TimestreamQuery.Client.describe_scheduled_query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.describe_scheduled_query)

Asynchronous method. Use `await describe_scheduled_query(...)` for a
synchronous call.

Arguments mapping described in
[DescribeScheduledQueryRequestRequestTypeDef](./type_defs.md#describescheduledqueryrequestrequesttypedef).

Keyword-only arguments:

- `ScheduledQueryArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeScheduledQueryResponseTypeDef](./type_defs.md#describescheduledqueryresponsetypedef).

<a id="execute_scheduled_query"></a>

### execute_scheduled_query

You can use this API to run a scheduled query manually.

Type annotations for
`aiobotocore.create_client("timestream-query").execute_scheduled_query` method.

Boto3 documentation:
[TimestreamQuery.Client.execute_scheduled_query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.execute_scheduled_query)

Asynchronous method. Use `await execute_scheduled_query(...)` for a synchronous
call.

Arguments mapping described in
[ExecuteScheduledQueryRequestRequestTypeDef](./type_defs.md#executescheduledqueryrequestrequesttypedef).

Keyword-only arguments:

- `ScheduledQueryArn`: `str` *(required)*
- `InvocationTime`: `Union`\[`datetime`, `str`\] *(required)*
- `ClientToken`: `str`

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("timestream-query").generate_presigned_url` method.

Boto3 documentation:
[TimestreamQuery.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_scheduled_queries"></a>

### list_scheduled_queries

Gets a list of all scheduled queries in the caller's Amazon account and Region.

Type annotations for
`aiobotocore.create_client("timestream-query").list_scheduled_queries` method.

Boto3 documentation:
[TimestreamQuery.Client.list_scheduled_queries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.list_scheduled_queries)

Asynchronous method. Use `await list_scheduled_queries(...)` for a synchronous
call.

Arguments mapping described in
[ListScheduledQueriesRequestRequestTypeDef](./type_defs.md#listscheduledqueriesrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListScheduledQueriesResponseTypeDef](./type_defs.md#listscheduledqueriesresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

List all tags on a Timestream query resource.

Type annotations for
`aiobotocore.create_client("timestream-query").list_tags_for_resource` method.

Boto3 documentation:
[TimestreamQuery.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="prepare_query"></a>

### prepare_query

A synchronous operation that allows you to submit a query with parameters to be
stored by Timestream for later running.

Type annotations for
`aiobotocore.create_client("timestream-query").prepare_query` method.

Boto3 documentation:
[TimestreamQuery.Client.prepare_query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.prepare_query)

Asynchronous method. Use `await prepare_query(...)` for a synchronous call.

Arguments mapping described in
[PrepareQueryRequestRequestTypeDef](./type_defs.md#preparequeryrequestrequesttypedef).

Keyword-only arguments:

- `QueryString`: `str` *(required)*
- `ValidateOnly`: `bool`

Returns a `Coroutine` for
[PrepareQueryResponseTypeDef](./type_defs.md#preparequeryresponsetypedef).

<a id="query"></a>

### query

`Query` is a synchronous operation that enables you to run a query against your
Amazon Timestream data.

Type annotations for `aiobotocore.create_client("timestream-query").query`
method.

Boto3 documentation:
[TimestreamQuery.Client.query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.query)

Asynchronous method. Use `await query(...)` for a synchronous call.

Arguments mapping described in
[QueryRequestRequestTypeDef](./type_defs.md#queryrequestrequesttypedef).

Keyword-only arguments:

- `QueryString`: `str` *(required)*
- `ClientToken`: `str`
- `NextToken`: `str`
- `MaxRows`: `int`

Returns a `Coroutine` for
[QueryResponseTypeDef](./type_defs.md#queryresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Associate a set of tags with a Timestream resource.

Type annotations for
`aiobotocore.create_client("timestream-query").tag_resource` method.

Boto3 documentation:
[TimestreamQuery.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes the association of tags from a Timestream query resource.

Type annotations for
`aiobotocore.create_client("timestream-query").untag_resource` method.

Boto3 documentation:
[TimestreamQuery.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_scheduled_query"></a>

### update_scheduled_query

Update a scheduled query.

Type annotations for
`aiobotocore.create_client("timestream-query").update_scheduled_query` method.

Boto3 documentation:
[TimestreamQuery.Client.update_scheduled_query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.update_scheduled_query)

Asynchronous method. Use `await update_scheduled_query(...)` for a synchronous
call.

Arguments mapping described in
[UpdateScheduledQueryRequestRequestTypeDef](./type_defs.md#updatescheduledqueryrequestrequesttypedef).

Keyword-only arguments:

- `ScheduledQueryArn`: `str` *(required)*
- `State`: [ScheduledQueryStateType](./literals.md#scheduledquerystatetype)
  *(required)*

<a id="get_paginator"></a>

### get_paginator

Type annotations for
`aiobotocore.create_client("timestream-query").get_paginator` method with
overloads.

- `client.get_paginator("list_scheduled_queries")` ->
  [ListScheduledQueriesPaginator](./paginators.md#listscheduledqueriespaginator)
- `client.get_paginator("list_tags_for_resource")` ->
  [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("query")` ->
  [QueryPaginator](./paginators.md#querypaginator)
