<a id="datapipelineclient-for-aiobotocore-datapipeline-module"></a>

# DataPipelineClient for aiobotocore DataPipeline module

> [Index](..) > [DataPipeline](.) > DataPipelineClient

Auto-generated documentation for
[DataPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
type annotations stubs module
[types-aiobotocore-datapipeline](https://pypi.org/project/types-aiobotocore-datapipeline/).

- [DataPipelineClient for aiobotocore DataPipeline module](#datapipelineclient-for-aiobotocore-datapipeline-module)
  - [DataPipelineClient](#datapipelineclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [activate_pipeline](#activate_pipeline)
    - [add_tags](#add_tags)
    - [can_paginate](#can_paginate)
    - [create_pipeline](#create_pipeline)
    - [deactivate_pipeline](#deactivate_pipeline)
    - [delete_pipeline](#delete_pipeline)
    - [describe_objects](#describe_objects)
    - [describe_pipelines](#describe_pipelines)
    - [evaluate_expression](#evaluate_expression)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_pipeline_definition](#get_pipeline_definition)
    - [list_pipelines](#list_pipelines)
    - [poll_for_task](#poll_for_task)
    - [put_pipeline_definition](#put_pipeline_definition)
    - [query_objects](#query_objects)
    - [remove_tags](#remove_tags)
    - [report_task_progress](#report_task_progress)
    - [report_task_runner_heartbeat](#report_task_runner_heartbeat)
    - [set_status](#set_status)
    - [set_task_status](#set_task_status)
    - [validate_pipeline_definition](#validate_pipeline_definition)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="datapipelineclient"></a>

## DataPipelineClient

Type annotations for `session.create_client("datapipeline")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_datapipeline.client import DataPipelineClient

session = get_session()
async with session.create_client("datapipeline") as client:
    client: DataPipelineClient
```

Boto3 documentation:
[DataPipeline.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_datapipeline.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InternalServiceError`
- `Exceptions.InvalidRequestException`
- `Exceptions.PipelineDeletedException`
- `Exceptions.PipelineNotFoundException`
- `Exceptions.TaskNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

DataPipelineClient exceptions.

Type annotations for `session.create_client("datapipeline").exceptions` method.

Boto3 documentation:
[DataPipeline.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="activate_pipeline"></a>

### activate_pipeline

Validates the specified pipeline and starts processing pipeline tasks.

Type annotations for `session.create_client("datapipeline").activate_pipeline`
method.

Boto3 documentation:
[DataPipeline.Client.activate_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.activate_pipeline)

Asynchronous method. Use `await activate_pipeline(...)` for a synchronous call.

Arguments mapping described in
[ActivatePipelineInputRequestTypeDef](./type_defs.md#activatepipelineinputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `parameterValues`:
  `Sequence`\[[ParameterValueTypeDef](./type_defs.md#parametervaluetypedef)\]
- `startTimestamp`: `Union`\[`datetime`, `str`\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="add_tags"></a>

### add_tags

Adds or modifies tags for the specified pipeline.

Type annotations for `session.create_client("datapipeline").add_tags` method.

Boto3 documentation:
[DataPipeline.Client.add_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.add_tags)

Asynchronous method. Use `await add_tags(...)` for a synchronous call.

Arguments mapping described in
[AddTagsInputRequestTypeDef](./type_defs.md#addtagsinputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("datapipeline").can_paginate`
method.

Boto3 documentation:
[DataPipeline.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_pipeline"></a>

### create_pipeline

Creates a new, empty pipeline.

Type annotations for `session.create_client("datapipeline").create_pipeline`
method.

Boto3 documentation:
[DataPipeline.Client.create_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.create_pipeline)

Asynchronous method. Use `await create_pipeline(...)` for a synchronous call.

Arguments mapping described in
[CreatePipelineInputRequestTypeDef](./type_defs.md#createpipelineinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `uniqueId`: `str` *(required)*
- `description`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreatePipelineOutputTypeDef](./type_defs.md#createpipelineoutputtypedef).

<a id="deactivate_pipeline"></a>

### deactivate_pipeline

Deactivates the specified running pipeline.

Type annotations for
`session.create_client("datapipeline").deactivate_pipeline` method.

Boto3 documentation:
[DataPipeline.Client.deactivate_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.deactivate_pipeline)

Asynchronous method. Use `await deactivate_pipeline(...)` for a synchronous
call.

Arguments mapping described in
[DeactivatePipelineInputRequestTypeDef](./type_defs.md#deactivatepipelineinputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `cancelActive`: `bool`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_pipeline"></a>

### delete_pipeline

Deletes a pipeline, its pipeline definition, and its run history.

Type annotations for `session.create_client("datapipeline").delete_pipeline`
method.

Boto3 documentation:
[DataPipeline.Client.delete_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.delete_pipeline)

Asynchronous method. Use `await delete_pipeline(...)` for a synchronous call.

Arguments mapping described in
[DeletePipelineInputRequestTypeDef](./type_defs.md#deletepipelineinputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*

<a id="describe_objects"></a>

### describe_objects

Gets the object definitions for a set of objects associated with the pipeline.

Type annotations for `session.create_client("datapipeline").describe_objects`
method.

Boto3 documentation:
[DataPipeline.Client.describe_objects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.describe_objects)

Asynchronous method. Use `await describe_objects(...)` for a synchronous call.

Arguments mapping described in
[DescribeObjectsInputRequestTypeDef](./type_defs.md#describeobjectsinputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `objectIds`: `Sequence`\[`str`\] *(required)*
- `evaluateExpressions`: `bool`
- `marker`: `str`

Returns a `Coroutine` for
[DescribeObjectsOutputTypeDef](./type_defs.md#describeobjectsoutputtypedef).

<a id="describe_pipelines"></a>

### describe_pipelines

Retrieves metadata about one or more pipelines.

Type annotations for `session.create_client("datapipeline").describe_pipelines`
method.

Boto3 documentation:
[DataPipeline.Client.describe_pipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.describe_pipelines)

Asynchronous method. Use `await describe_pipelines(...)` for a synchronous
call.

Arguments mapping described in
[DescribePipelinesInputRequestTypeDef](./type_defs.md#describepipelinesinputrequesttypedef).

Keyword-only arguments:

- `pipelineIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DescribePipelinesOutputTypeDef](./type_defs.md#describepipelinesoutputtypedef).

<a id="evaluate_expression"></a>

### evaluate_expression

Task runners call `EvaluateExpression` to evaluate a string in the context of
the specified object.

Type annotations for
`session.create_client("datapipeline").evaluate_expression` method.

Boto3 documentation:
[DataPipeline.Client.evaluate_expression](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.evaluate_expression)

Asynchronous method. Use `await evaluate_expression(...)` for a synchronous
call.

Arguments mapping described in
[EvaluateExpressionInputRequestTypeDef](./type_defs.md#evaluateexpressioninputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `objectId`: `str` *(required)*
- `expression`: `str` *(required)*

Returns a `Coroutine` for
[EvaluateExpressionOutputTypeDef](./type_defs.md#evaluateexpressionoutputtypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("datapipeline").generate_presigned_url` method.

Boto3 documentation:
[DataPipeline.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_pipeline_definition"></a>

### get_pipeline_definition

Gets the definition of the specified pipeline.

Type annotations for
`session.create_client("datapipeline").get_pipeline_definition` method.

Boto3 documentation:
[DataPipeline.Client.get_pipeline_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.get_pipeline_definition)

Asynchronous method. Use `await get_pipeline_definition(...)` for a synchronous
call.

Arguments mapping described in
[GetPipelineDefinitionInputRequestTypeDef](./type_defs.md#getpipelinedefinitioninputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `version`: `str`

Returns a `Coroutine` for
[GetPipelineDefinitionOutputTypeDef](./type_defs.md#getpipelinedefinitionoutputtypedef).

<a id="list_pipelines"></a>

### list_pipelines

Lists the pipeline identifiers for all active pipelines that you have
permission to access.

Type annotations for `session.create_client("datapipeline").list_pipelines`
method.

Boto3 documentation:
[DataPipeline.Client.list_pipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.list_pipelines)

Asynchronous method. Use `await list_pipelines(...)` for a synchronous call.

Arguments mapping described in
[ListPipelinesInputRequestTypeDef](./type_defs.md#listpipelinesinputrequesttypedef).

Keyword-only arguments:

- `marker`: `str`

Returns a `Coroutine` for
[ListPipelinesOutputTypeDef](./type_defs.md#listpipelinesoutputtypedef).

<a id="poll_for_task"></a>

### poll_for_task

Task runners call `PollForTask` to receive a task to perform from AWS Data
Pipeline.

Type annotations for `session.create_client("datapipeline").poll_for_task`
method.

Boto3 documentation:
[DataPipeline.Client.poll_for_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.poll_for_task)

Asynchronous method. Use `await poll_for_task(...)` for a synchronous call.

Arguments mapping described in
[PollForTaskInputRequestTypeDef](./type_defs.md#pollfortaskinputrequesttypedef).

Keyword-only arguments:

- `workerGroup`: `str` *(required)*
- `hostname`: `str`
- `instanceIdentity`:
  [InstanceIdentityTypeDef](./type_defs.md#instanceidentitytypedef)

Returns a `Coroutine` for
[PollForTaskOutputTypeDef](./type_defs.md#pollfortaskoutputtypedef).

<a id="put_pipeline_definition"></a>

### put_pipeline_definition

Adds tasks, schedules, and preconditions to the specified pipeline.

Type annotations for
`session.create_client("datapipeline").put_pipeline_definition` method.

Boto3 documentation:
[DataPipeline.Client.put_pipeline_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.put_pipeline_definition)

Asynchronous method. Use `await put_pipeline_definition(...)` for a synchronous
call.

Arguments mapping described in
[PutPipelineDefinitionInputRequestTypeDef](./type_defs.md#putpipelinedefinitioninputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `pipelineObjects`:
  `Sequence`\[[PipelineObjectTypeDef](./type_defs.md#pipelineobjecttypedef)\]
  *(required)*
- `parameterObjects`:
  `Sequence`\[[ParameterObjectTypeDef](./type_defs.md#parameterobjecttypedef)\]
- `parameterValues`:
  `Sequence`\[[ParameterValueTypeDef](./type_defs.md#parametervaluetypedef)\]

Returns a `Coroutine` for
[PutPipelineDefinitionOutputTypeDef](./type_defs.md#putpipelinedefinitionoutputtypedef).

<a id="query_objects"></a>

### query_objects

Queries the specified pipeline for the names of objects that match the
specified set of conditions.

Type annotations for `session.create_client("datapipeline").query_objects`
method.

Boto3 documentation:
[DataPipeline.Client.query_objects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.query_objects)

Asynchronous method. Use `await query_objects(...)` for a synchronous call.

Arguments mapping described in
[QueryObjectsInputRequestTypeDef](./type_defs.md#queryobjectsinputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `sphere`: `str` *(required)*
- `query`: [QueryTypeDef](./type_defs.md#querytypedef)
- `marker`: `str`
- `limit`: `int`

Returns a `Coroutine` for
[QueryObjectsOutputTypeDef](./type_defs.md#queryobjectsoutputtypedef).

<a id="remove_tags"></a>

### remove_tags

Removes existing tags from the specified pipeline.

Type annotations for `session.create_client("datapipeline").remove_tags`
method.

Boto3 documentation:
[DataPipeline.Client.remove_tags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.remove_tags)

Asynchronous method. Use `await remove_tags(...)` for a synchronous call.

Arguments mapping described in
[RemoveTagsInputRequestTypeDef](./type_defs.md#removetagsinputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="report_task_progress"></a>

### report_task_progress

Task runners call `ReportTaskProgress` when assigned a task to acknowledge that
it has the task.

Type annotations for
`session.create_client("datapipeline").report_task_progress` method.

Boto3 documentation:
[DataPipeline.Client.report_task_progress](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.report_task_progress)

Asynchronous method. Use `await report_task_progress(...)` for a synchronous
call.

Arguments mapping described in
[ReportTaskProgressInputRequestTypeDef](./type_defs.md#reporttaskprogressinputrequesttypedef).

Keyword-only arguments:

- `taskId`: `str` *(required)*
- `fields`: `Sequence`\[[FieldTypeDef](./type_defs.md#fieldtypedef)\]

Returns a `Coroutine` for
[ReportTaskProgressOutputTypeDef](./type_defs.md#reporttaskprogressoutputtypedef).

<a id="report_task_runner_heartbeat"></a>

### report_task_runner_heartbeat

Task runners call `ReportTaskRunnerHeartbeat` every 15 minutes to indicate that
they are operational.

Type annotations for
`session.create_client("datapipeline").report_task_runner_heartbeat` method.

Boto3 documentation:
[DataPipeline.Client.report_task_runner_heartbeat](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.report_task_runner_heartbeat)

Asynchronous method. Use `await report_task_runner_heartbeat(...)` for a
synchronous call.

Arguments mapping described in
[ReportTaskRunnerHeartbeatInputRequestTypeDef](./type_defs.md#reporttaskrunnerheartbeatinputrequesttypedef).

Keyword-only arguments:

- `taskrunnerId`: `str` *(required)*
- `workerGroup`: `str`
- `hostname`: `str`

Returns a `Coroutine` for
[ReportTaskRunnerHeartbeatOutputTypeDef](./type_defs.md#reporttaskrunnerheartbeatoutputtypedef).

<a id="set_status"></a>

### set_status

Requests that the status of the specified physical or logical pipeline objects
be updated in the specified pipeline.

Type annotations for `session.create_client("datapipeline").set_status` method.

Boto3 documentation:
[DataPipeline.Client.set_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.set_status)

Asynchronous method. Use `await set_status(...)` for a synchronous call.

Arguments mapping described in
[SetStatusInputRequestTypeDef](./type_defs.md#setstatusinputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `objectIds`: `Sequence`\[`str`\] *(required)*
- `status`: `str` *(required)*

<a id="set_task_status"></a>

### set_task_status

Task runners call `SetTaskStatus` to notify AWS Data Pipeline that a task is
completed and provide information about the final status.

Type annotations for `session.create_client("datapipeline").set_task_status`
method.

Boto3 documentation:
[DataPipeline.Client.set_task_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.set_task_status)

Asynchronous method. Use `await set_task_status(...)` for a synchronous call.

Arguments mapping described in
[SetTaskStatusInputRequestTypeDef](./type_defs.md#settaskstatusinputrequesttypedef).

Keyword-only arguments:

- `taskId`: `str` *(required)*
- `taskStatus`: [TaskStatusType](./literals.md#taskstatustype) *(required)*
- `errorId`: `str`
- `errorMessage`: `str`
- `errorStackTrace`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="validate_pipeline_definition"></a>

### validate_pipeline_definition

Validates the specified pipeline definition to ensure that it is well formed
and can be run without error.

Type annotations for
`session.create_client("datapipeline").validate_pipeline_definition` method.

Boto3 documentation:
[DataPipeline.Client.validate_pipeline_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.validate_pipeline_definition)

Asynchronous method. Use `await validate_pipeline_definition(...)` for a
synchronous call.

Arguments mapping described in
[ValidatePipelineDefinitionInputRequestTypeDef](./type_defs.md#validatepipelinedefinitioninputrequesttypedef).

Keyword-only arguments:

- `pipelineId`: `str` *(required)*
- `pipelineObjects`:
  `Sequence`\[[PipelineObjectTypeDef](./type_defs.md#pipelineobjecttypedef)\]
  *(required)*
- `parameterObjects`:
  `Sequence`\[[ParameterObjectTypeDef](./type_defs.md#parameterobjecttypedef)\]
- `parameterValues`:
  `Sequence`\[[ParameterValueTypeDef](./type_defs.md#parametervaluetypedef)\]

Returns a `Coroutine` for
[ValidatePipelineDefinitionOutputTypeDef](./type_defs.md#validatepipelinedefinitionoutputtypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("datapipeline").__aenter__` method.

Boto3 documentation:
[DataPipeline.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [DataPipelineClient](#datapipelineclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("datapipeline").__aexit__` method.

Boto3 documentation:
[DataPipeline.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("datapipeline").get_paginator`
method with overloads.

- `client.get_paginator("describe_objects")` ->
  [DescribeObjectsPaginator](./paginators.md#describeobjectspaginator)
- `client.get_paginator("list_pipelines")` ->
  [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
- `client.get_paginator("query_objects")` ->
  [QueryObjectsPaginator](./paginators.md#queryobjectspaginator)
