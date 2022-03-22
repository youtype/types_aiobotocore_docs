<a id="sfnclient-for-aiobotocore-sfn-module"></a>

# SFNClient for aiobotocore SFN module

> [Index](../README.md) > [SFN](./README.md) > SFNClient

Auto-generated documentation for
[SFN](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
type annotations stubs module
[types-aiobotocore-stepfunctions](https://pypi.org/project/types-aiobotocore-stepfunctions/).

- [SFNClient for aiobotocore SFN module](#sfnclient-for-aiobotocore-sfn-module)
  - [SFNClient](#sfnclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_activity](#create_activity)
    - [create_state_machine](#create_state_machine)
    - [delete_activity](#delete_activity)
    - [delete_state_machine](#delete_state_machine)
    - [describe_activity](#describe_activity)
    - [describe_execution](#describe_execution)
    - [describe_state_machine](#describe_state_machine)
    - [describe_state_machine_for_execution](#describe_state_machine_for_execution)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_activity_task](#get_activity_task)
    - [get_execution_history](#get_execution_history)
    - [list_activities](#list_activities)
    - [list_executions](#list_executions)
    - [list_state_machines](#list_state_machines)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [send_task_failure](#send_task_failure)
    - [send_task_heartbeat](#send_task_heartbeat)
    - [send_task_success](#send_task_success)
    - [start_execution](#start_execution)
    - [start_sync_execution](#start_sync_execution)
    - [stop_execution](#stop_execution)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_state_machine](#update_state_machine)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="sfnclient"></a>

## SFNClient

Type annotations for `session.create_client("stepfunctions")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_stepfunctions.client import SFNClient

session = get_session()
async with session.create_client("stepfunctions") as client:
    client: SFNClient
```

Boto3 documentation:
[SFN.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_stepfunctions.client import Exceptions

def handle_error(exc: Exceptions.ActivityDoesNotExist) -> None:
    ...
```

Exceptions:

- `Exceptions.ActivityDoesNotExist`
- `Exceptions.ActivityLimitExceeded`
- `Exceptions.ActivityWorkerLimitExceeded`
- `Exceptions.ClientError`
- `Exceptions.ExecutionAlreadyExists`
- `Exceptions.ExecutionDoesNotExist`
- `Exceptions.ExecutionLimitExceeded`
- `Exceptions.InvalidArn`
- `Exceptions.InvalidDefinition`
- `Exceptions.InvalidExecutionInput`
- `Exceptions.InvalidLoggingConfiguration`
- `Exceptions.InvalidName`
- `Exceptions.InvalidOutput`
- `Exceptions.InvalidToken`
- `Exceptions.InvalidTracingConfiguration`
- `Exceptions.MissingRequiredParameter`
- `Exceptions.ResourceNotFound`
- `Exceptions.StateMachineAlreadyExists`
- `Exceptions.StateMachineDeleting`
- `Exceptions.StateMachineDoesNotExist`
- `Exceptions.StateMachineLimitExceeded`
- `Exceptions.StateMachineTypeNotSupported`
- `Exceptions.TaskDoesNotExist`
- `Exceptions.TaskTimedOut`
- `Exceptions.TooManyTags`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

SFNClient exceptions.

Type annotations for `session.create_client("stepfunctions").exceptions`
method.

Boto3 documentation:
[SFN.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("stepfunctions").can_paginate`
method.

Boto3 documentation:
[SFN.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_activity"></a>

### create_activity

Creates an activity.

Type annotations for `session.create_client("stepfunctions").create_activity`
method.

Boto3 documentation:
[SFN.Client.create_activity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_activity)

Asynchronous method. Use `await create_activity(...)` for a synchronous call.

Arguments mapping described in
[CreateActivityInputRequestTypeDef](./type_defs.md#createactivityinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateActivityOutputTypeDef](./type_defs.md#createactivityoutputtypedef).

<a id="create\_state\_machine"></a>

### create_state_machine

Creates a state machine.

Type annotations for
`session.create_client("stepfunctions").create_state_machine` method.

Boto3 documentation:
[SFN.Client.create_state_machine](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine)

Asynchronous method. Use `await create_state_machine(...)` for a synchronous
call.

Arguments mapping described in
[CreateStateMachineInputRequestTypeDef](./type_defs.md#createstatemachineinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `definition`: `str` *(required)*
- `roleArn`: `str` *(required)*
- `type`: [StateMachineTypeType](./literals.md#statemachinetypetype)
- `loggingConfiguration`:
  [LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef)
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `tracingConfiguration`:
  [TracingConfigurationTypeDef](./type_defs.md#tracingconfigurationtypedef)

Returns a `Coroutine` for
[CreateStateMachineOutputTypeDef](./type_defs.md#createstatemachineoutputtypedef).

<a id="delete\_activity"></a>

### delete_activity

Deletes an activity.

Type annotations for `session.create_client("stepfunctions").delete_activity`
method.

Boto3 documentation:
[SFN.Client.delete_activity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_activity)

Asynchronous method. Use `await delete_activity(...)` for a synchronous call.

Arguments mapping described in
[DeleteActivityInputRequestTypeDef](./type_defs.md#deleteactivityinputrequesttypedef).

Keyword-only arguments:

- `activityArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_state\_machine"></a>

### delete_state_machine

Deletes a state machine.

Type annotations for
`session.create_client("stepfunctions").delete_state_machine` method.

Boto3 documentation:
[SFN.Client.delete_state_machine](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine)

Asynchronous method. Use `await delete_state_machine(...)` for a synchronous
call.

Arguments mapping described in
[DeleteStateMachineInputRequestTypeDef](./type_defs.md#deletestatemachineinputrequesttypedef).

Keyword-only arguments:

- `stateMachineArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe\_activity"></a>

### describe_activity

Describes an activity.

Type annotations for `session.create_client("stepfunctions").describe_activity`
method.

Boto3 documentation:
[SFN.Client.describe_activity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_activity)

Asynchronous method. Use `await describe_activity(...)` for a synchronous call.

Arguments mapping described in
[DescribeActivityInputRequestTypeDef](./type_defs.md#describeactivityinputrequesttypedef).

Keyword-only arguments:

- `activityArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeActivityOutputTypeDef](./type_defs.md#describeactivityoutputtypedef).

<a id="describe\_execution"></a>

### describe_execution

Describes an execution.

Type annotations for
`session.create_client("stepfunctions").describe_execution` method.

Boto3 documentation:
[SFN.Client.describe_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_execution)

Asynchronous method. Use `await describe_execution(...)` for a synchronous
call.

Arguments mapping described in
[DescribeExecutionInputRequestTypeDef](./type_defs.md#describeexecutioninputrequesttypedef).

Keyword-only arguments:

- `executionArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeExecutionOutputTypeDef](./type_defs.md#describeexecutionoutputtypedef).

<a id="describe\_state\_machine"></a>

### describe_state_machine

Describes a state machine.

Type annotations for
`session.create_client("stepfunctions").describe_state_machine` method.

Boto3 documentation:
[SFN.Client.describe_state_machine](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine)

Asynchronous method. Use `await describe_state_machine(...)` for a synchronous
call.

Arguments mapping described in
[DescribeStateMachineInputRequestTypeDef](./type_defs.md#describestatemachineinputrequesttypedef).

Keyword-only arguments:

- `stateMachineArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeStateMachineOutputTypeDef](./type_defs.md#describestatemachineoutputtypedef).

<a id="describe\_state\_machine\_for\_execution"></a>

### describe_state_machine_for_execution

Describes the state machine associated with a specific execution.

Type annotations for
`session.create_client("stepfunctions").describe_state_machine_for_execution`
method.

Boto3 documentation:
[SFN.Client.describe_state_machine_for_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine_for_execution)

Asynchronous method. Use `await describe_state_machine_for_execution(...)` for
a synchronous call.

Arguments mapping described in
[DescribeStateMachineForExecutionInputRequestTypeDef](./type_defs.md#describestatemachineforexecutioninputrequesttypedef).

Keyword-only arguments:

- `executionArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeStateMachineForExecutionOutputTypeDef](./type_defs.md#describestatemachineforexecutionoutputtypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("stepfunctions").generate_presigned_url` method.

Boto3 documentation:
[SFN.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_activity\_task"></a>

### get_activity_task

Used by workers to retrieve a task (with the specified activity ARN) which has
been scheduled for execution by a running state machine.

Type annotations for `session.create_client("stepfunctions").get_activity_task`
method.

Boto3 documentation:
[SFN.Client.get_activity_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_activity_task)

Asynchronous method. Use `await get_activity_task(...)` for a synchronous call.

Arguments mapping described in
[GetActivityTaskInputRequestTypeDef](./type_defs.md#getactivitytaskinputrequesttypedef).

Keyword-only arguments:

- `activityArn`: `str` *(required)*
- `workerName`: `str`

Returns a `Coroutine` for
[GetActivityTaskOutputTypeDef](./type_defs.md#getactivitytaskoutputtypedef).

<a id="get\_execution\_history"></a>

### get_execution_history

Returns the history of the specified execution as a list of events.

Type annotations for
`session.create_client("stepfunctions").get_execution_history` method.

Boto3 documentation:
[SFN.Client.get_execution_history](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_execution_history)

Asynchronous method. Use `await get_execution_history(...)` for a synchronous
call.

Arguments mapping described in
[GetExecutionHistoryInputRequestTypeDef](./type_defs.md#getexecutionhistoryinputrequesttypedef).

Keyword-only arguments:

- `executionArn`: `str` *(required)*
- `maxResults`: `int`
- `reverseOrder`: `bool`
- `nextToken`: `str`
- `includeExecutionData`: `bool`

Returns a `Coroutine` for
[GetExecutionHistoryOutputTypeDef](./type_defs.md#getexecutionhistoryoutputtypedef).

<a id="list\_activities"></a>

### list_activities

Lists the existing activities.

Type annotations for `session.create_client("stepfunctions").list_activities`
method.

Boto3 documentation:
[SFN.Client.list_activities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_activities)

Asynchronous method. Use `await list_activities(...)` for a synchronous call.

Arguments mapping described in
[ListActivitiesInputRequestTypeDef](./type_defs.md#listactivitiesinputrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListActivitiesOutputTypeDef](./type_defs.md#listactivitiesoutputtypedef).

<a id="list\_executions"></a>

### list_executions

Lists the executions of a state machine that meet the filtering criteria.

Type annotations for `session.create_client("stepfunctions").list_executions`
method.

Boto3 documentation:
[SFN.Client.list_executions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_executions)

Asynchronous method. Use `await list_executions(...)` for a synchronous call.

Arguments mapping described in
[ListExecutionsInputRequestTypeDef](./type_defs.md#listexecutionsinputrequesttypedef).

Keyword-only arguments:

- `stateMachineArn`: `str` *(required)*
- `statusFilter`: [ExecutionStatusType](./literals.md#executionstatustype)
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListExecutionsOutputTypeDef](./type_defs.md#listexecutionsoutputtypedef).

<a id="list\_state\_machines"></a>

### list_state_machines

Lists the existing state machines.

Type annotations for
`session.create_client("stepfunctions").list_state_machines` method.

Boto3 documentation:
[SFN.Client.list_state_machines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machines)

Asynchronous method. Use `await list_state_machines(...)` for a synchronous
call.

Arguments mapping described in
[ListStateMachinesInputRequestTypeDef](./type_defs.md#liststatemachinesinputrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListStateMachinesOutputTypeDef](./type_defs.md#liststatemachinesoutputtypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

List tags for a given resource.

Type annotations for
`session.create_client("stepfunctions").list_tags_for_resource` method.

Boto3 documentation:
[SFN.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef).

<a id="send\_task\_failure"></a>

### send_task_failure

Used by activity workers and task states using the
\[callback\](https://docs.aws.amazon.com/step-functions/latest/dg/connect-to-
resource.html#connect-wait-token)\_ pattern to report that the task identified
by the `taskToken` failed.

Type annotations for `session.create_client("stepfunctions").send_task_failure`
method.

Boto3 documentation:
[SFN.Client.send_task_failure](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.send_task_failure)

Asynchronous method. Use `await send_task_failure(...)` for a synchronous call.

Arguments mapping described in
[SendTaskFailureInputRequestTypeDef](./type_defs.md#sendtaskfailureinputrequesttypedef).

Keyword-only arguments:

- `taskToken`: `str` *(required)*
- `error`: `str`
- `cause`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="send\_task\_heartbeat"></a>

### send_task_heartbeat

Used by activity workers and task states using the
\[callback\](https://docs.aws.amazon.com/step-functions/latest/dg/connect-to-
resource.html#connect-wait-token)\_ pattern to report to Step Functions that
the task represented by the specified `taskToken` is still making progress.

Type annotations for
`session.create_client("stepfunctions").send_task_heartbeat` method.

Boto3 documentation:
[SFN.Client.send_task_heartbeat](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.send_task_heartbeat)

Asynchronous method. Use `await send_task_heartbeat(...)` for a synchronous
call.

Arguments mapping described in
[SendTaskHeartbeatInputRequestTypeDef](./type_defs.md#sendtaskheartbeatinputrequesttypedef).

Keyword-only arguments:

- `taskToken`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="send\_task\_success"></a>

### send_task_success

Used by activity workers and task states using the
\[callback\](https://docs.aws.amazon.com/step-functions/latest/dg/connect-to-
resource.html#connect-wait-token)\_ pattern to report that the task identified
by the `taskToken` completed successfully.

Type annotations for `session.create_client("stepfunctions").send_task_success`
method.

Boto3 documentation:
[SFN.Client.send_task_success](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.send_task_success)

Asynchronous method. Use `await send_task_success(...)` for a synchronous call.

Arguments mapping described in
[SendTaskSuccessInputRequestTypeDef](./type_defs.md#sendtasksuccessinputrequesttypedef).

Keyword-only arguments:

- `taskToken`: `str` *(required)*
- `output`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="start\_execution"></a>

### start_execution

Starts a state machine execution.

Type annotations for `session.create_client("stepfunctions").start_execution`
method.

Boto3 documentation:
[SFN.Client.start_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.start_execution)

Asynchronous method. Use `await start_execution(...)` for a synchronous call.

Arguments mapping described in
[StartExecutionInputRequestTypeDef](./type_defs.md#startexecutioninputrequesttypedef).

Keyword-only arguments:

- `stateMachineArn`: `str` *(required)*
- `name`: `str`
- `input`: `str`
- `traceHeader`: `str`

Returns a `Coroutine` for
[StartExecutionOutputTypeDef](./type_defs.md#startexecutionoutputtypedef).

<a id="start\_sync\_execution"></a>

### start_sync_execution

Starts a Synchronous Express state machine execution.

Type annotations for
`session.create_client("stepfunctions").start_sync_execution` method.

Boto3 documentation:
[SFN.Client.start_sync_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.start_sync_execution)

Asynchronous method. Use `await start_sync_execution(...)` for a synchronous
call.

Arguments mapping described in
[StartSyncExecutionInputRequestTypeDef](./type_defs.md#startsyncexecutioninputrequesttypedef).

Keyword-only arguments:

- `stateMachineArn`: `str` *(required)*
- `name`: `str`
- `input`: `str`
- `traceHeader`: `str`

Returns a `Coroutine` for
[StartSyncExecutionOutputTypeDef](./type_defs.md#startsyncexecutionoutputtypedef).

<a id="stop\_execution"></a>

### stop_execution

Stops an execution.

Type annotations for `session.create_client("stepfunctions").stop_execution`
method.

Boto3 documentation:
[SFN.Client.stop_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.stop_execution)

Asynchronous method. Use `await stop_execution(...)` for a synchronous call.

Arguments mapping described in
[StopExecutionInputRequestTypeDef](./type_defs.md#stopexecutioninputrequesttypedef).

Keyword-only arguments:

- `executionArn`: `str` *(required)*
- `error`: `str`
- `cause`: `str`

Returns a `Coroutine` for
[StopExecutionOutputTypeDef](./type_defs.md#stopexecutionoutputtypedef).

<a id="tag\_resource"></a>

### tag_resource

Add a tag to a Step Functions resource.

Type annotations for `session.create_client("stepfunctions").tag_resource`
method.

Boto3 documentation:
[SFN.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Remove a tag from a Step Functions resource See also:
[AWS API Documentation](https://docs.aws.amazon.com/goto/WebAPI/states-2016-11-23/UntagResource).

Type annotations for `session.create_client("stepfunctions").untag_resource`
method.

Boto3 documentation:
[SFN.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_state\_machine"></a>

### update_state_machine

Updates an existing state machine by modifying its `definition` , `roleArn` ,
or `loggingConfiguration`.

Type annotations for
`session.create_client("stepfunctions").update_state_machine` method.

Boto3 documentation:
[SFN.Client.update_state_machine](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine)

Asynchronous method. Use `await update_state_machine(...)` for a synchronous
call.

Arguments mapping described in
[UpdateStateMachineInputRequestTypeDef](./type_defs.md#updatestatemachineinputrequesttypedef).

Keyword-only arguments:

- `stateMachineArn`: `str` *(required)*
- `definition`: `str`
- `roleArn`: `str`
- `loggingConfiguration`:
  [LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef)
- `tracingConfiguration`:
  [TracingConfigurationTypeDef](./type_defs.md#tracingconfigurationtypedef)

Returns a `Coroutine` for
[UpdateStateMachineOutputTypeDef](./type_defs.md#updatestatemachineoutputtypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("stepfunctions").__aenter__`
method.

Boto3 documentation:
[SFN.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [SFNClient](#sfnclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("stepfunctions").__aexit__` method.

Boto3 documentation:
[SFN.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("stepfunctions").get_paginator`
method with overloads.

- `client.get_paginator("get_execution_history")` ->
  [GetExecutionHistoryPaginator](./paginators.md#getexecutionhistorypaginator)
- `client.get_paginator("list_activities")` ->
  [ListActivitiesPaginator](./paginators.md#listactivitiespaginator)
- `client.get_paginator("list_executions")` ->
  [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
- `client.get_paginator("list_state_machines")` ->
  [ListStateMachinesPaginator](./paginators.md#liststatemachinespaginator)
