<a id="elastictranscoderclient-for-aiobotocore-elastictranscoder-module"></a>

# ElasticTranscoderClient for aiobotocore ElasticTranscoder module

> [Index](..) > [ElasticTranscoder](.) > ElasticTranscoderClient

Auto-generated documentation for
[ElasticTranscoder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
type annotations stubs module
[types-aiobotocore-elastictranscoder](https://pypi.org/project/types-aiobotocore-elastictranscoder/).

- [ElasticTranscoderClient for aiobotocore ElasticTranscoder module](#elastictranscoderclient-for-aiobotocore-elastictranscoder-module)
  - [ElasticTranscoderClient](#elastictranscoderclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [cancel_job](#cancel_job)
    - [create_job](#create_job)
    - [create_pipeline](#create_pipeline)
    - [create_preset](#create_preset)
    - [delete_pipeline](#delete_pipeline)
    - [delete_preset](#delete_preset)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_jobs_by_pipeline](#list_jobs_by_pipeline)
    - [list_jobs_by_status](#list_jobs_by_status)
    - [list_pipelines](#list_pipelines)
    - [list_presets](#list_presets)
    - [read_job](#read_job)
    - [read_pipeline](#read_pipeline)
    - [read_preset](#read_preset)
    - [test_role](#test_role)
    - [update_pipeline](#update_pipeline)
    - [update_pipeline_notifications](#update_pipeline_notifications)
    - [update_pipeline_status](#update_pipeline_status)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)
    - [get_waiter](#get_waiter)

<a id="elastictranscoderclient"></a>

## ElasticTranscoderClient

Type annotations for `session.create_client("elastictranscoder")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_elastictranscoder.client import ElasticTranscoderClient

session = get_session()
async with session.create_client("elastictranscoder") as client:
    client: ElasticTranscoderClient
```

Boto3 documentation:
[ElasticTranscoder.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_elastictranscoder.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.IncompatibleVersionException`
- `Exceptions.InternalServiceException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceInUseException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ElasticTranscoderClient exceptions.

Type annotations for `session.create_client("elastictranscoder").exceptions`
method.

Boto3 documentation:
[ElasticTranscoder.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("elastictranscoder").can_paginate`
method.

Boto3 documentation:
[ElasticTranscoder.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel_job"></a>

### cancel_job

The CancelJob operation cancels an unfinished job.

Type annotations for `session.create_client("elastictranscoder").cancel_job`
method.

Boto3 documentation:
[ElasticTranscoder.Client.cancel_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.cancel_job)

Asynchronous method. Use `await cancel_job(...)` for a synchronous call.

Arguments mapping described in
[CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create_job"></a>

### create_job

When you create a job, Elastic Transcoder returns JSON data that includes the
values that you specified plus information about the job that is created.

Type annotations for `session.create_client("elastictranscoder").create_job`
method.

Boto3 documentation:
[ElasticTranscoder.Client.create_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_job)

Asynchronous method. Use `await create_job(...)` for a synchronous call.

Arguments mapping described in
[CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef).

Keyword-only arguments:

- `PipelineId`: `str` *(required)*
- `Input`: [JobInputTypeDef](./type_defs.md#jobinputtypedef)
- `Inputs`: `Sequence`\[[JobInputTypeDef](./type_defs.md#jobinputtypedef)\]
- `Output`: [CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef)
- `Outputs`:
  `Sequence`\[[CreateJobOutputTypeDef](./type_defs.md#createjoboutputtypedef)\]
- `OutputKeyPrefix`: `str`
- `Playlists`:
  `Sequence`\[[CreateJobPlaylistTypeDef](./type_defs.md#createjobplaylisttypedef)\]
- `UserMetadata`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef).

<a id="create_pipeline"></a>

### create_pipeline

The CreatePipeline operation creates a pipeline with settings that you specify.

Type annotations for
`session.create_client("elastictranscoder").create_pipeline` method.

Boto3 documentation:
[ElasticTranscoder.Client.create_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_pipeline)

Asynchronous method. Use `await create_pipeline(...)` for a synchronous call.

Arguments mapping described in
[CreatePipelineRequestRequestTypeDef](./type_defs.md#createpipelinerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `InputBucket`: `str` *(required)*
- `Role`: `str` *(required)*
- `OutputBucket`: `str`
- `AwsKmsKeyArn`: `str`
- `Notifications`: [NotificationsTypeDef](./type_defs.md#notificationstypedef)
- `ContentConfig`:
  [PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef)
- `ThumbnailConfig`:
  [PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef)

Returns a `Coroutine` for
[CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef).

<a id="create_preset"></a>

### create_preset

The CreatePreset operation creates a preset with settings that you specify.

Type annotations for `session.create_client("elastictranscoder").create_preset`
method.

Boto3 documentation:
[ElasticTranscoder.Client.create_preset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_preset)

Asynchronous method. Use `await create_preset(...)` for a synchronous call.

Arguments mapping described in
[CreatePresetRequestRequestTypeDef](./type_defs.md#createpresetrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Container`: `str` *(required)*
- `Description`: `str`
- `Video`: [VideoParametersTypeDef](./type_defs.md#videoparameterstypedef)
- `Audio`: [AudioParametersTypeDef](./type_defs.md#audioparameterstypedef)
- `Thumbnails`: [ThumbnailsTypeDef](./type_defs.md#thumbnailstypedef)

Returns a `Coroutine` for
[CreatePresetResponseTypeDef](./type_defs.md#createpresetresponsetypedef).

<a id="delete_pipeline"></a>

### delete_pipeline

The DeletePipeline operation removes a pipeline.

Type annotations for
`session.create_client("elastictranscoder").delete_pipeline` method.

Boto3 documentation:
[ElasticTranscoder.Client.delete_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.delete_pipeline)

Asynchronous method. Use `await delete_pipeline(...)` for a synchronous call.

Arguments mapping described in
[DeletePipelineRequestRequestTypeDef](./type_defs.md#deletepipelinerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_preset"></a>

### delete_preset

The DeletePreset operation removes a preset that you've added in an AWS region.

Type annotations for `session.create_client("elastictranscoder").delete_preset`
method.

Boto3 documentation:
[ElasticTranscoder.Client.delete_preset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.delete_preset)

Asynchronous method. Use `await delete_preset(...)` for a synchronous call.

Arguments mapping described in
[DeletePresetRequestRequestTypeDef](./type_defs.md#deletepresetrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("elastictranscoder").generate_presigned_url` method.

Boto3 documentation:
[ElasticTranscoder.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_jobs_by_pipeline"></a>

### list_jobs_by_pipeline

The ListJobsByPipeline operation gets a list of the jobs currently in a
pipeline.

Type annotations for
`session.create_client("elastictranscoder").list_jobs_by_pipeline` method.

Boto3 documentation:
[ElasticTranscoder.Client.list_jobs_by_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_jobs_by_pipeline)

Asynchronous method. Use `await list_jobs_by_pipeline(...)` for a synchronous
call.

Arguments mapping described in
[ListJobsByPipelineRequestRequestTypeDef](./type_defs.md#listjobsbypipelinerequestrequesttypedef).

Keyword-only arguments:

- `PipelineId`: `str` *(required)*
- `Ascending`: `str`
- `PageToken`: `str`

Returns a `Coroutine` for
[ListJobsByPipelineResponseTypeDef](./type_defs.md#listjobsbypipelineresponsetypedef).

<a id="list_jobs_by_status"></a>

### list_jobs_by_status

The ListJobsByStatus operation gets a list of jobs that have a specified
status.

Type annotations for
`session.create_client("elastictranscoder").list_jobs_by_status` method.

Boto3 documentation:
[ElasticTranscoder.Client.list_jobs_by_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_jobs_by_status)

Asynchronous method. Use `await list_jobs_by_status(...)` for a synchronous
call.

Arguments mapping described in
[ListJobsByStatusRequestRequestTypeDef](./type_defs.md#listjobsbystatusrequestrequesttypedef).

Keyword-only arguments:

- `Status`: `str` *(required)*
- `Ascending`: `str`
- `PageToken`: `str`

Returns a `Coroutine` for
[ListJobsByStatusResponseTypeDef](./type_defs.md#listjobsbystatusresponsetypedef).

<a id="list_pipelines"></a>

### list_pipelines

The ListPipelines operation gets a list of the pipelines associated with the
current AWS account.

Type annotations for
`session.create_client("elastictranscoder").list_pipelines` method.

Boto3 documentation:
[ElasticTranscoder.Client.list_pipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_pipelines)

Asynchronous method. Use `await list_pipelines(...)` for a synchronous call.

Arguments mapping described in
[ListPipelinesRequestRequestTypeDef](./type_defs.md#listpipelinesrequestrequesttypedef).

Keyword-only arguments:

- `Ascending`: `str`
- `PageToken`: `str`

Returns a `Coroutine` for
[ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef).

<a id="list_presets"></a>

### list_presets

The ListPresets operation gets a list of the default presets included with
Elastic Transcoder and the presets that you've added in an AWS region.

Type annotations for `session.create_client("elastictranscoder").list_presets`
method.

Boto3 documentation:
[ElasticTranscoder.Client.list_presets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.list_presets)

Asynchronous method. Use `await list_presets(...)` for a synchronous call.

Arguments mapping described in
[ListPresetsRequestRequestTypeDef](./type_defs.md#listpresetsrequestrequesttypedef).

Keyword-only arguments:

- `Ascending`: `str`
- `PageToken`: `str`

Returns a `Coroutine` for
[ListPresetsResponseTypeDef](./type_defs.md#listpresetsresponsetypedef).

<a id="read_job"></a>

### read_job

The ReadJob operation returns detailed information about a job.

Type annotations for `session.create_client("elastictranscoder").read_job`
method.

Boto3 documentation:
[ElasticTranscoder.Client.read_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.read_job)

Asynchronous method. Use `await read_job(...)` for a synchronous call.

Arguments mapping described in
[ReadJobRequestRequestTypeDef](./type_defs.md#readjobrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[ReadJobResponseTypeDef](./type_defs.md#readjobresponsetypedef).

<a id="read_pipeline"></a>

### read_pipeline

The ReadPipeline operation gets detailed information about a pipeline.

Type annotations for `session.create_client("elastictranscoder").read_pipeline`
method.

Boto3 documentation:
[ElasticTranscoder.Client.read_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.read_pipeline)

Asynchronous method. Use `await read_pipeline(...)` for a synchronous call.

Arguments mapping described in
[ReadPipelineRequestRequestTypeDef](./type_defs.md#readpipelinerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[ReadPipelineResponseTypeDef](./type_defs.md#readpipelineresponsetypedef).

<a id="read_preset"></a>

### read_preset

The ReadPreset operation gets detailed information about a preset.

Type annotations for `session.create_client("elastictranscoder").read_preset`
method.

Boto3 documentation:
[ElasticTranscoder.Client.read_preset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.read_preset)

Asynchronous method. Use `await read_preset(...)` for a synchronous call.

Arguments mapping described in
[ReadPresetRequestRequestTypeDef](./type_defs.md#readpresetrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[ReadPresetResponseTypeDef](./type_defs.md#readpresetresponsetypedef).

<a id="test_role"></a>

### test_role

The TestRole operation tests the IAM role used to create the pipeline.

Type annotations for `session.create_client("elastictranscoder").test_role`
method.

Boto3 documentation:
[ElasticTranscoder.Client.test_role](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.test_role)

Asynchronous method. Use `await test_role(...)` for a synchronous call.

Arguments mapping described in
[TestRoleRequestRequestTypeDef](./type_defs.md#testrolerequestrequesttypedef).

Keyword-only arguments:

- `Role`: `str` *(required)*
- `InputBucket`: `str` *(required)*
- `OutputBucket`: `str` *(required)*
- `Topics`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[TestRoleResponseTypeDef](./type_defs.md#testroleresponsetypedef).

<a id="update_pipeline"></a>

### update_pipeline

Use the `UpdatePipeline` operation to update settings for a pipeline.

Type annotations for
`session.create_client("elastictranscoder").update_pipeline` method.

Boto3 documentation:
[ElasticTranscoder.Client.update_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline)

Asynchronous method. Use `await update_pipeline(...)` for a synchronous call.

Arguments mapping described in
[UpdatePipelineRequestRequestTypeDef](./type_defs.md#updatepipelinerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Name`: `str`
- `InputBucket`: `str`
- `Role`: `str`
- `AwsKmsKeyArn`: `str`
- `Notifications`: [NotificationsTypeDef](./type_defs.md#notificationstypedef)
- `ContentConfig`:
  [PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef)
- `ThumbnailConfig`:
  [PipelineOutputConfigTypeDef](./type_defs.md#pipelineoutputconfigtypedef)

Returns a `Coroutine` for
[UpdatePipelineResponseTypeDef](./type_defs.md#updatepipelineresponsetypedef).

<a id="update_pipeline_notifications"></a>

### update_pipeline_notifications

With the UpdatePipelineNotifications operation, you can update Amazon Simple
Notification Service (Amazon SNS) notifications for a pipeline.

Type annotations for
`session.create_client("elastictranscoder").update_pipeline_notifications`
method.

Boto3 documentation:
[ElasticTranscoder.Client.update_pipeline_notifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline_notifications)

Asynchronous method. Use `await update_pipeline_notifications(...)` for a
synchronous call.

Arguments mapping described in
[UpdatePipelineNotificationsRequestRequestTypeDef](./type_defs.md#updatepipelinenotificationsrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Notifications`: [NotificationsTypeDef](./type_defs.md#notificationstypedef)
  *(required)*

Returns a `Coroutine` for
[UpdatePipelineNotificationsResponseTypeDef](./type_defs.md#updatepipelinenotificationsresponsetypedef).

<a id="update_pipeline_status"></a>

### update_pipeline_status

The UpdatePipelineStatus operation pauses or reactivates a pipeline, so that
the pipeline stops or restarts the processing of jobs.

Type annotations for
`session.create_client("elastictranscoder").update_pipeline_status` method.

Boto3 documentation:
[ElasticTranscoder.Client.update_pipeline_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline_status)

Asynchronous method. Use `await update_pipeline_status(...)` for a synchronous
call.

Arguments mapping described in
[UpdatePipelineStatusRequestRequestTypeDef](./type_defs.md#updatepipelinestatusrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Status`: `str` *(required)*

Returns a `Coroutine` for
[UpdatePipelineStatusResponseTypeDef](./type_defs.md#updatepipelinestatusresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("elastictranscoder").__aenter__`
method.

Boto3 documentation:
[ElasticTranscoder.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [ElasticTranscoderClient](#elastictranscoderclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("elastictranscoder").__aexit__`
method.

Boto3 documentation:
[ElasticTranscoder.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("elastictranscoder").get_paginator`
method with overloads.

- `client.get_paginator("list_jobs_by_pipeline")` ->
  [ListJobsByPipelinePaginator](./paginators.md#listjobsbypipelinepaginator)
- `client.get_paginator("list_jobs_by_status")` ->
  [ListJobsByStatusPaginator](./paginators.md#listjobsbystatuspaginator)
- `client.get_paginator("list_pipelines")` ->
  [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
- `client.get_paginator("list_presets")` ->
  [ListPresetsPaginator](./paginators.md#listpresetspaginator)

<a id="get_waiter"></a>

### get_waiter

Type annotations for `session.create_client("elastictranscoder").get_waiter`
method with overloads.

- `client.get_waiter("job_complete")` ->
  [JobCompleteWaiter](./waiters.md#jobcompletewaiter)
