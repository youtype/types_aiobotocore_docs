<a id="syntheticsclient-for-aiobotocore-synthetics-module"></a>

# SyntheticsClient for aiobotocore Synthetics module

> [Index](..) > [Synthetics](.) > SyntheticsClient

Auto-generated documentation for
[Synthetics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
type annotations stubs module
[types-aiobotocore-synthetics](https://pypi.org/project/types-aiobotocore-synthetics/).

- [SyntheticsClient for aiobotocore Synthetics module](#syntheticsclient-for-aiobotocore-synthetics-module)
  - [SyntheticsClient](#syntheticsclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_canary](#create_canary)
    - [delete_canary](#delete_canary)
    - [describe_canaries](#describe_canaries)
    - [describe_canaries_last_run](#describe_canaries_last_run)
    - [describe_runtime_versions](#describe_runtime_versions)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_canary](#get_canary)
    - [get_canary_runs](#get_canary_runs)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [start_canary](#start_canary)
    - [stop_canary](#stop_canary)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_canary](#update_canary)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="syntheticsclient"></a>

## SyntheticsClient

Type annotations for `session.create_client("synthetics")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_synthetics.client import SyntheticsClient

session = get_session()
async with session.create_client("synthetics") as client:
    client: SyntheticsClient
```

Boto3 documentation:
[Synthetics.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_synthetics.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

SyntheticsClient exceptions.

Type annotations for `session.create_client("synthetics").exceptions` method.

Boto3 documentation:
[Synthetics.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("synthetics").can_paginate` method.

Boto3 documentation:
[Synthetics.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_canary"></a>

### create_canary

Creates a canary.

Type annotations for `session.create_client("synthetics").create_canary`
method.

Boto3 documentation:
[Synthetics.Client.create_canary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.create_canary)

Asynchronous method. Use `await create_canary(...)` for a synchronous call.

Arguments mapping described in
[CreateCanaryRequestRequestTypeDef](./type_defs.md#createcanaryrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Code`: [CanaryCodeInputTypeDef](./type_defs.md#canarycodeinputtypedef)
  *(required)*
- `ArtifactS3Location`: `str` *(required)*
- `ExecutionRoleArn`: `str` *(required)*
- `Schedule`:
  [CanaryScheduleInputTypeDef](./type_defs.md#canaryscheduleinputtypedef)
  *(required)*
- `RuntimeVersion`: `str` *(required)*
- `RunConfig`:
  [CanaryRunConfigInputTypeDef](./type_defs.md#canaryrunconfiginputtypedef)
- `SuccessRetentionPeriodInDays`: `int`
- `FailureRetentionPeriodInDays`: `int`
- `VpcConfig`: [VpcConfigInputTypeDef](./type_defs.md#vpcconfiginputtypedef)
- `Tags`: `Mapping`\[`str`, `str`\]
- `ArtifactConfig`:
  [ArtifactConfigInputTypeDef](./type_defs.md#artifactconfiginputtypedef)

Returns a `Coroutine` for
[CreateCanaryResponseTypeDef](./type_defs.md#createcanaryresponsetypedef).

<a id="delete_canary"></a>

### delete_canary

Permanently deletes the specified canary.

Type annotations for `session.create_client("synthetics").delete_canary`
method.

Boto3 documentation:
[Synthetics.Client.delete_canary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.delete_canary)

Asynchronous method. Use `await delete_canary(...)` for a synchronous call.

Arguments mapping described in
[DeleteCanaryRequestRequestTypeDef](./type_defs.md#deletecanaryrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_canaries"></a>

### describe_canaries

This operation returns a list of the canaries in your account, along with full
details about each canary.

Type annotations for `session.create_client("synthetics").describe_canaries`
method.

Boto3 documentation:
[Synthetics.Client.describe_canaries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.describe_canaries)

Asynchronous method. Use `await describe_canaries(...)` for a synchronous call.

Arguments mapping described in
[DescribeCanariesRequestRequestTypeDef](./type_defs.md#describecanariesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[DescribeCanariesResponseTypeDef](./type_defs.md#describecanariesresponsetypedef).

<a id="describe_canaries_last_run"></a>

### describe_canaries_last_run

Use this operation to see information from the most recent run of each canary
that you have created.

Type annotations for
`session.create_client("synthetics").describe_canaries_last_run` method.

Boto3 documentation:
[Synthetics.Client.describe_canaries_last_run](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.describe_canaries_last_run)

Asynchronous method. Use `await describe_canaries_last_run(...)` for a
synchronous call.

Arguments mapping described in
[DescribeCanariesLastRunRequestRequestTypeDef](./type_defs.md#describecanarieslastrunrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[DescribeCanariesLastRunResponseTypeDef](./type_defs.md#describecanarieslastrunresponsetypedef).

<a id="describe_runtime_versions"></a>

### describe_runtime_versions

Returns a list of Synthetics canary runtime versions.

Type annotations for
`session.create_client("synthetics").describe_runtime_versions` method.

Boto3 documentation:
[Synthetics.Client.describe_runtime_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.describe_runtime_versions)

Asynchronous method. Use `await describe_runtime_versions(...)` for a
synchronous call.

Arguments mapping described in
[DescribeRuntimeVersionsRequestRequestTypeDef](./type_defs.md#describeruntimeversionsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[DescribeRuntimeVersionsResponseTypeDef](./type_defs.md#describeruntimeversionsresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("synthetics").generate_presigned_url` method.

Boto3 documentation:
[Synthetics.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_canary"></a>

### get_canary

Retrieves complete information about one canary.

Type annotations for `session.create_client("synthetics").get_canary` method.

Boto3 documentation:
[Synthetics.Client.get_canary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.get_canary)

Asynchronous method. Use `await get_canary(...)` for a synchronous call.

Arguments mapping described in
[GetCanaryRequestRequestTypeDef](./type_defs.md#getcanaryrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[GetCanaryResponseTypeDef](./type_defs.md#getcanaryresponsetypedef).

<a id="get_canary_runs"></a>

### get_canary_runs

Retrieves a list of runs for a specified canary.

Type annotations for `session.create_client("synthetics").get_canary_runs`
method.

Boto3 documentation:
[Synthetics.Client.get_canary_runs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.get_canary_runs)

Asynchronous method. Use `await get_canary_runs(...)` for a synchronous call.

Arguments mapping described in
[GetCanaryRunsRequestRequestTypeDef](./type_defs.md#getcanaryrunsrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[GetCanaryRunsResponseTypeDef](./type_defs.md#getcanaryrunsresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Displays the tags associated with a canary.

Type annotations for
`session.create_client("synthetics").list_tags_for_resource` method.

Boto3 documentation:
[Synthetics.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="start_canary"></a>

### start_canary

Use this operation to run a canary that has already been created.

Type annotations for `session.create_client("synthetics").start_canary` method.

Boto3 documentation:
[Synthetics.Client.start_canary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.start_canary)

Asynchronous method. Use `await start_canary(...)` for a synchronous call.

Arguments mapping described in
[StartCanaryRequestRequestTypeDef](./type_defs.md#startcanaryrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="stop_canary"></a>

### stop_canary

Stops the canary to prevent all future runs.

Type annotations for `session.create_client("synthetics").stop_canary` method.

Boto3 documentation:
[Synthetics.Client.stop_canary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.stop_canary)

Asynchronous method. Use `await stop_canary(...)` for a synchronous call.

Arguments mapping described in
[StopCanaryRequestRequestTypeDef](./type_defs.md#stopcanaryrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag_resource"></a>

### tag_resource

Assigns one or more tags (key-value pairs) to the specified canary.

Type annotations for `session.create_client("synthetics").tag_resource` method.

Boto3 documentation:
[Synthetics.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes one or more tags from the specified canary.

Type annotations for `session.create_client("synthetics").untag_resource`
method.

Boto3 documentation:
[Synthetics.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_canary"></a>

### update_canary

Use this operation to change the settings of a canary that has already been
created.

Type annotations for `session.create_client("synthetics").update_canary`
method.

Boto3 documentation:
[Synthetics.Client.update_canary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.update_canary)

Asynchronous method. Use `await update_canary(...)` for a synchronous call.

Arguments mapping described in
[UpdateCanaryRequestRequestTypeDef](./type_defs.md#updatecanaryrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Code`: [CanaryCodeInputTypeDef](./type_defs.md#canarycodeinputtypedef)
- `ExecutionRoleArn`: `str`
- `RuntimeVersion`: `str`
- `Schedule`:
  [CanaryScheduleInputTypeDef](./type_defs.md#canaryscheduleinputtypedef)
- `RunConfig`:
  [CanaryRunConfigInputTypeDef](./type_defs.md#canaryrunconfiginputtypedef)
- `SuccessRetentionPeriodInDays`: `int`
- `FailureRetentionPeriodInDays`: `int`
- `VpcConfig`: [VpcConfigInputTypeDef](./type_defs.md#vpcconfiginputtypedef)
- `VisualReference`:
  [VisualReferenceInputTypeDef](./type_defs.md#visualreferenceinputtypedef)
- `ArtifactS3Location`: `str`
- `ArtifactConfig`:
  [ArtifactConfigInputTypeDef](./type_defs.md#artifactconfiginputtypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("synthetics").__aenter__` method.

Boto3 documentation:
[Synthetics.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [SyntheticsClient](#syntheticsclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("synthetics").__aexit__` method.

Boto3 documentation:
[Synthetics.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
