<a id="resourcegroupstaggingapiclient-for-aiobotocore-resourcegroupstaggingapi-module"></a>

# ResourceGroupsTaggingAPIClient for aiobotocore ResourceGroupsTaggingAPI module

> [Index](..) > [ResourceGroupsTaggingAPI](.) > ResourceGroupsTaggingAPIClient

Auto-generated documentation for
[ResourceGroupsTaggingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
type annotations stubs module
[types-aiobotocore-resourcegroupstaggingapi](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi/).

- [ResourceGroupsTaggingAPIClient for aiobotocore ResourceGroupsTaggingAPI module](#resourcegroupstaggingapiclient-for-aiobotocore-resourcegroupstaggingapi-module)
  - [ResourceGroupsTaggingAPIClient](#resourcegroupstaggingapiclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [describe_report_creation](#describe_report_creation)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_compliance_summary](#get_compliance_summary)
    - [get_resources](#get_resources)
    - [get_tag_keys](#get_tag_keys)
    - [get_tag_values](#get_tag_values)
    - [start_report_creation](#start_report_creation)
    - [tag_resources](#tag_resources)
    - [untag_resources](#untag_resources)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="resourcegroupstaggingapiclient"></a>

## ResourceGroupsTaggingAPIClient

Type annotations for `session.create_client("resourcegroupstaggingapi")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_resourcegroupstaggingapi.client import ResourceGroupsTaggingAPIClient

session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:
    client: ResourceGroupsTaggingAPIClient
```

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_resourcegroupstaggingapi.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConcurrentModificationException`
- `Exceptions.ConstraintViolationException`
- `Exceptions.InternalServiceException`
- `Exceptions.InvalidParameterException`
- `Exceptions.PaginationTokenExpiredException`
- `Exceptions.ThrottledException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ResourceGroupsTaggingAPIClient exceptions.

Type annotations for
`session.create_client("resourcegroupstaggingapi").exceptions` method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("resourcegroupstaggingapi").can_paginate` method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="describe_report_creation"></a>

### describe_report_creation

Describes the status of the `StartReportCreation` operation.

Type annotations for
`session.create_client("resourcegroupstaggingapi").describe_report_creation`
method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.describe_report_creation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.describe_report_creation)

Asynchronous method. Use `await describe_report_creation(...)` for a
synchronous call.

Returns a `Coroutine` for
[DescribeReportCreationOutputTypeDef](./type_defs.md#describereportcreationoutputtypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("resourcegroupstaggingapi").generate_presigned_url`
method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_compliance_summary"></a>

### get_compliance_summary

Returns a table that shows counts of resources that are noncompliant with their
tag policies.

Type annotations for
`session.create_client("resourcegroupstaggingapi").get_compliance_summary`
method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.get_compliance_summary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.get_compliance_summary)

Asynchronous method. Use `await get_compliance_summary(...)` for a synchronous
call.

Arguments mapping described in
[GetComplianceSummaryInputRequestTypeDef](./type_defs.md#getcompliancesummaryinputrequesttypedef).

Keyword-only arguments:

- `TargetIdFilters`: `Sequence`\[`str`\]
- `RegionFilters`: `Sequence`\[`str`\]
- `ResourceTypeFilters`: `Sequence`\[`str`\]
- `TagKeyFilters`: `Sequence`\[`str`\]
- `GroupBy`:
  `Sequence`\[[GroupByAttributeType](./literals.md#groupbyattributetype)\]
- `MaxResults`: `int`
- `PaginationToken`: `str`

Returns a `Coroutine` for
[GetComplianceSummaryOutputTypeDef](./type_defs.md#getcompliancesummaryoutputtypedef).

<a id="get_resources"></a>

### get_resources

Returns all the tagged or previously tagged resources that are located in the
specified Amazon Web Services Region for the account.

Type annotations for
`session.create_client("resourcegroupstaggingapi").get_resources` method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.get_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.get_resources)

Asynchronous method. Use `await get_resources(...)` for a synchronous call.

Arguments mapping described in
[GetResourcesInputRequestTypeDef](./type_defs.md#getresourcesinputrequesttypedef).

Keyword-only arguments:

- `PaginationToken`: `str`
- `TagFilters`:
  `Sequence`\[[TagFilterTypeDef](./type_defs.md#tagfiltertypedef)\]
- `ResourcesPerPage`: `int`
- `TagsPerPage`: `int`
- `ResourceTypeFilters`: `Sequence`\[`str`\]
- `IncludeComplianceDetails`: `bool`
- `ExcludeCompliantResources`: `bool`
- `ResourceARNList`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[GetResourcesOutputTypeDef](./type_defs.md#getresourcesoutputtypedef).

<a id="get_tag_keys"></a>

### get_tag_keys

Returns all tag keys currently in use in the specified Amazon Web Services
Region for the calling account.

Type annotations for
`session.create_client("resourcegroupstaggingapi").get_tag_keys` method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.get_tag_keys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.get_tag_keys)

Asynchronous method. Use `await get_tag_keys(...)` for a synchronous call.

Arguments mapping described in
[GetTagKeysInputRequestTypeDef](./type_defs.md#gettagkeysinputrequesttypedef).

Keyword-only arguments:

- `PaginationToken`: `str`

Returns a `Coroutine` for
[GetTagKeysOutputTypeDef](./type_defs.md#gettagkeysoutputtypedef).

<a id="get_tag_values"></a>

### get_tag_values

Returns all tag values for the specified key that are used in the specified
Amazon Web Services Region for the calling account.

Type annotations for
`session.create_client("resourcegroupstaggingapi").get_tag_values` method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.get_tag_values](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.get_tag_values)

Asynchronous method. Use `await get_tag_values(...)` for a synchronous call.

Arguments mapping described in
[GetTagValuesInputRequestTypeDef](./type_defs.md#gettagvaluesinputrequesttypedef).

Keyword-only arguments:

- `Key`: `str` *(required)*
- `PaginationToken`: `str`

Returns a `Coroutine` for
[GetTagValuesOutputTypeDef](./type_defs.md#gettagvaluesoutputtypedef).

<a id="start_report_creation"></a>

### start_report_creation

Generates a report that lists all tagged resources in the accounts across your
organization and tells whether each resource is compliant with the effective
tag policy.

Type annotations for
`session.create_client("resourcegroupstaggingapi").start_report_creation`
method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.start_report_creation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.start_report_creation)

Asynchronous method. Use `await start_report_creation(...)` for a synchronous
call.

Arguments mapping described in
[StartReportCreationInputRequestTypeDef](./type_defs.md#startreportcreationinputrequesttypedef).

Keyword-only arguments:

- `S3Bucket`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag_resources"></a>

### tag_resources

.

Type annotations for
`session.create_client("resourcegroupstaggingapi").tag_resources` method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.tag_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.tag_resources)

Asynchronous method. Use `await tag_resources(...)` for a synchronous call.

Arguments mapping described in
[TagResourcesInputRequestTypeDef](./type_defs.md#tagresourcesinputrequesttypedef).

Keyword-only arguments:

- `ResourceARNList`: `Sequence`\[`str`\] *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for
[TagResourcesOutputTypeDef](./type_defs.md#tagresourcesoutputtypedef).

<a id="untag_resources"></a>

### untag_resources

.

Type annotations for
`session.create_client("resourcegroupstaggingapi").untag_resources` method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.untag_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.untag_resources)

Asynchronous method. Use `await untag_resources(...)` for a synchronous call.

Arguments mapping described in
[UntagResourcesInputRequestTypeDef](./type_defs.md#untagresourcesinputrequesttypedef).

Keyword-only arguments:

- `ResourceARNList`: `Sequence`\[`str`\] *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[UntagResourcesOutputTypeDef](./type_defs.md#untagresourcesoutputtypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for
`session.create_client("resourcegroupstaggingapi").__aenter__` method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[ResourceGroupsTaggingAPIClient](#resourcegroupstaggingapiclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for
`session.create_client("resourcegroupstaggingapi").__aexit__` method.

Boto3 documentation:
[ResourceGroupsTaggingAPI.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for
`session.create_client("resourcegroupstaggingapi").get_paginator` method with
overloads.

- `client.get_paginator("get_compliance_summary")` ->
  [GetComplianceSummaryPaginator](./paginators.md#getcompliancesummarypaginator)
- `client.get_paginator("get_resources")` ->
  [GetResourcesPaginator](./paginators.md#getresourcespaginator)
- `client.get_paginator("get_tag_keys")` ->
  [GetTagKeysPaginator](./paginators.md#gettagkeyspaginator)
- `client.get_paginator("get_tag_values")` ->
  [GetTagValuesPaginator](./paginators.md#gettagvaluespaginator)
