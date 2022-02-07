<a id="codepipelineclient-for-aiobotocore-codepipeline-module"></a>

# CodePipelineClient for aiobotocore CodePipeline module

> [Index](..) > [CodePipeline](.) > CodePipelineClient

Auto-generated documentation for
[CodePipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline)
type annotations stubs module
[types-aiobotocore-codepipeline](https://pypi.org/project/types-aiobotocore-codepipeline/).

- [CodePipelineClient for aiobotocore CodePipeline module](#codepipelineclient-for-aiobotocore-codepipeline-module)
  - [CodePipelineClient](#codepipelineclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [acknowledge_job](#acknowledge_job)
    - [acknowledge_third_party_job](#acknowledge_third_party_job)
    - [can_paginate](#can_paginate)
    - [create_custom_action_type](#create_custom_action_type)
    - [create_pipeline](#create_pipeline)
    - [delete_custom_action_type](#delete_custom_action_type)
    - [delete_pipeline](#delete_pipeline)
    - [delete_webhook](#delete_webhook)
    - [deregister_webhook_with_third_party](#deregister_webhook_with_third_party)
    - [disable_stage_transition](#disable_stage_transition)
    - [enable_stage_transition](#enable_stage_transition)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_action_type](#get_action_type)
    - [get_job_details](#get_job_details)
    - [get_pipeline](#get_pipeline)
    - [get_pipeline_execution](#get_pipeline_execution)
    - [get_pipeline_state](#get_pipeline_state)
    - [get_third_party_job_details](#get_third_party_job_details)
    - [list_action_executions](#list_action_executions)
    - [list_action_types](#list_action_types)
    - [list_pipeline_executions](#list_pipeline_executions)
    - [list_pipelines](#list_pipelines)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_webhooks](#list_webhooks)
    - [poll_for_jobs](#poll_for_jobs)
    - [poll_for_third_party_jobs](#poll_for_third_party_jobs)
    - [put_action_revision](#put_action_revision)
    - [put_approval_result](#put_approval_result)
    - [put_job_failure_result](#put_job_failure_result)
    - [put_job_success_result](#put_job_success_result)
    - [put_third_party_job_failure_result](#put_third_party_job_failure_result)
    - [put_third_party_job_success_result](#put_third_party_job_success_result)
    - [put_webhook](#put_webhook)
    - [register_webhook_with_third_party](#register_webhook_with_third_party)
    - [retry_stage_execution](#retry_stage_execution)
    - [start_pipeline_execution](#start_pipeline_execution)
    - [stop_pipeline_execution](#stop_pipeline_execution)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_action_type](#update_action_type)
    - [update_pipeline](#update_pipeline)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="codepipelineclient"></a>

## CodePipelineClient

Type annotations for `session.create_client("codepipeline")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_codepipeline.client import CodePipelineClient

session = get_session()
async with session.create_client("codepipeline") as client:
    client: CodePipelineClient
```

Boto3 documentation:
[CodePipeline.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_codepipeline.client import Exceptions

def handle_error(exc: Exceptions.ActionNotFoundException) -> None:
    ...
```

Exceptions:

- `Exceptions.ActionNotFoundException`
- `Exceptions.ActionTypeAlreadyExistsException`
- `Exceptions.ActionTypeNotFoundException`
- `Exceptions.ApprovalAlreadyCompletedException`
- `Exceptions.ClientError`
- `Exceptions.ConcurrentModificationException`
- `Exceptions.ConflictException`
- `Exceptions.DuplicatedStopRequestException`
- `Exceptions.InvalidActionDeclarationException`
- `Exceptions.InvalidApprovalTokenException`
- `Exceptions.InvalidArnException`
- `Exceptions.InvalidBlockerDeclarationException`
- `Exceptions.InvalidClientTokenException`
- `Exceptions.InvalidJobException`
- `Exceptions.InvalidJobStateException`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.InvalidNonceException`
- `Exceptions.InvalidStageDeclarationException`
- `Exceptions.InvalidStructureException`
- `Exceptions.InvalidTagsException`
- `Exceptions.InvalidWebhookAuthenticationParametersException`
- `Exceptions.InvalidWebhookFilterPatternException`
- `Exceptions.JobNotFoundException`
- `Exceptions.LimitExceededException`
- `Exceptions.NotLatestPipelineExecutionException`
- `Exceptions.OutputVariablesSizeExceededException`
- `Exceptions.PipelineExecutionNotFoundException`
- `Exceptions.PipelineExecutionNotStoppableException`
- `Exceptions.PipelineNameInUseException`
- `Exceptions.PipelineNotFoundException`
- `Exceptions.PipelineVersionNotFoundException`
- `Exceptions.RequestFailedException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.StageNotFoundException`
- `Exceptions.StageNotRetryableException`
- `Exceptions.TooManyTagsException`
- `Exceptions.ValidationException`
- `Exceptions.WebhookNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CodePipelineClient exceptions.

Type annotations for `session.create_client("codepipeline").exceptions` method.

Boto3 documentation:
[CodePipeline.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="acknowledge_job"></a>

### acknowledge_job

Returns information about a specified job and whether that job has been
received by the job worker.

Type annotations for `session.create_client("codepipeline").acknowledge_job`
method.

Boto3 documentation:
[CodePipeline.Client.acknowledge_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.acknowledge_job)

Asynchronous method. Use `await acknowledge_job(...)` for a synchronous call.

Arguments mapping described in
[AcknowledgeJobInputRequestTypeDef](./type_defs.md#acknowledgejobinputrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `nonce`: `str` *(required)*

Returns a `Coroutine` for
[AcknowledgeJobOutputTypeDef](./type_defs.md#acknowledgejoboutputtypedef).

<a id="acknowledge_third_party_job"></a>

### acknowledge_third_party_job

Confirms a job worker has received the specified job.

Type annotations for
`session.create_client("codepipeline").acknowledge_third_party_job` method.

Boto3 documentation:
[CodePipeline.Client.acknowledge_third_party_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.acknowledge_third_party_job)

Asynchronous method. Use `await acknowledge_third_party_job(...)` for a
synchronous call.

Arguments mapping described in
[AcknowledgeThirdPartyJobInputRequestTypeDef](./type_defs.md#acknowledgethirdpartyjobinputrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `nonce`: `str` *(required)*
- `clientToken`: `str` *(required)*

Returns a `Coroutine` for
[AcknowledgeThirdPartyJobOutputTypeDef](./type_defs.md#acknowledgethirdpartyjoboutputtypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("codepipeline").can_paginate`
method.

Boto3 documentation:
[CodePipeline.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_custom_action_type"></a>

### create_custom_action_type

Creates a new custom action that can be used in all pipelines associated with
the AWS account.

Type annotations for
`session.create_client("codepipeline").create_custom_action_type` method.

Boto3 documentation:
[CodePipeline.Client.create_custom_action_type](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_custom_action_type)

Asynchronous method. Use `await create_custom_action_type(...)` for a
synchronous call.

Arguments mapping described in
[CreateCustomActionTypeInputRequestTypeDef](./type_defs.md#createcustomactiontypeinputrequesttypedef).

Keyword-only arguments:

- `category`: [ActionCategoryType](./literals.md#actioncategorytype)
  *(required)*
- `provider`: `str` *(required)*
- `version`: `str` *(required)*
- `inputArtifactDetails`:
  [ArtifactDetailsTypeDef](./type_defs.md#artifactdetailstypedef) *(required)*
- `outputArtifactDetails`:
  [ArtifactDetailsTypeDef](./type_defs.md#artifactdetailstypedef) *(required)*
- `settings`:
  [ActionTypeSettingsTypeDef](./type_defs.md#actiontypesettingstypedef)
- `configurationProperties`:
  `Sequence`\[[ActionConfigurationPropertyTypeDef](./type_defs.md#actionconfigurationpropertytypedef)\]
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateCustomActionTypeOutputTypeDef](./type_defs.md#createcustomactiontypeoutputtypedef).

<a id="create_pipeline"></a>

### create_pipeline

Creates a pipeline.

Type annotations for `session.create_client("codepipeline").create_pipeline`
method.

Boto3 documentation:
[CodePipeline.Client.create_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.create_pipeline)

Asynchronous method. Use `await create_pipeline(...)` for a synchronous call.

Arguments mapping described in
[CreatePipelineInputRequestTypeDef](./type_defs.md#createpipelineinputrequesttypedef).

Keyword-only arguments:

- `pipeline`:
  [PipelineDeclarationTypeDef](./type_defs.md#pipelinedeclarationtypedef)
  *(required)*
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreatePipelineOutputTypeDef](./type_defs.md#createpipelineoutputtypedef).

<a id="delete_custom_action_type"></a>

### delete_custom_action_type

Marks a custom action as deleted.

Type annotations for
`session.create_client("codepipeline").delete_custom_action_type` method.

Boto3 documentation:
[CodePipeline.Client.delete_custom_action_type](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.delete_custom_action_type)

Asynchronous method. Use `await delete_custom_action_type(...)` for a
synchronous call.

Arguments mapping described in
[DeleteCustomActionTypeInputRequestTypeDef](./type_defs.md#deletecustomactiontypeinputrequesttypedef).

Keyword-only arguments:

- `category`: [ActionCategoryType](./literals.md#actioncategorytype)
  *(required)*
- `provider`: `str` *(required)*
- `version`: `str` *(required)*

<a id="delete_pipeline"></a>

### delete_pipeline

Deletes the specified pipeline.

Type annotations for `session.create_client("codepipeline").delete_pipeline`
method.

Boto3 documentation:
[CodePipeline.Client.delete_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.delete_pipeline)

Asynchronous method. Use `await delete_pipeline(...)` for a synchronous call.

Arguments mapping described in
[DeletePipelineInputRequestTypeDef](./type_defs.md#deletepipelineinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

<a id="delete_webhook"></a>

### delete_webhook

Deletes a previously created webhook by name.

Type annotations for `session.create_client("codepipeline").delete_webhook`
method.

Boto3 documentation:
[CodePipeline.Client.delete_webhook](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.delete_webhook)

Asynchronous method. Use `await delete_webhook(...)` for a synchronous call.

Arguments mapping described in
[DeleteWebhookInputRequestTypeDef](./type_defs.md#deletewebhookinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="deregister_webhook_with_third_party"></a>

### deregister_webhook_with_third_party

Removes the connection between the webhook that was created by CodePipeline and
the external tool with events to be detected.

Type annotations for
`session.create_client("codepipeline").deregister_webhook_with_third_party`
method.

Boto3 documentation:
[CodePipeline.Client.deregister_webhook_with_third_party](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.deregister_webhook_with_third_party)

Asynchronous method. Use `await deregister_webhook_with_third_party(...)` for a
synchronous call.

Arguments mapping described in
[DeregisterWebhookWithThirdPartyInputRequestTypeDef](./type_defs.md#deregisterwebhookwiththirdpartyinputrequesttypedef).

Keyword-only arguments:

- `webhookName`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disable_stage_transition"></a>

### disable_stage_transition

Prevents artifacts in a pipeline from transitioning to the next stage in the
pipeline.

Type annotations for
`session.create_client("codepipeline").disable_stage_transition` method.

Boto3 documentation:
[CodePipeline.Client.disable_stage_transition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.disable_stage_transition)

Asynchronous method. Use `await disable_stage_transition(...)` for a
synchronous call.

Arguments mapping described in
[DisableStageTransitionInputRequestTypeDef](./type_defs.md#disablestagetransitioninputrequesttypedef).

Keyword-only arguments:

- `pipelineName`: `str` *(required)*
- `stageName`: `str` *(required)*
- `transitionType`:
  [StageTransitionTypeType](./literals.md#stagetransitiontypetype) *(required)*
- `reason`: `str` *(required)*

<a id="enable_stage_transition"></a>

### enable_stage_transition

Enables artifacts in a pipeline to transition to a stage in a pipeline.

Type annotations for
`session.create_client("codepipeline").enable_stage_transition` method.

Boto3 documentation:
[CodePipeline.Client.enable_stage_transition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.enable_stage_transition)

Asynchronous method. Use `await enable_stage_transition(...)` for a synchronous
call.

Arguments mapping described in
[EnableStageTransitionInputRequestTypeDef](./type_defs.md#enablestagetransitioninputrequesttypedef).

Keyword-only arguments:

- `pipelineName`: `str` *(required)*
- `stageName`: `str` *(required)*
- `transitionType`:
  [StageTransitionTypeType](./literals.md#stagetransitiontypetype) *(required)*

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("codepipeline").generate_presigned_url` method.

Boto3 documentation:
[CodePipeline.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_action_type"></a>

### get_action_type

Returns information about an action type created for an external provider,
where the action is to be used by customers of the external provider.

Type annotations for `session.create_client("codepipeline").get_action_type`
method.

Boto3 documentation:
[CodePipeline.Client.get_action_type](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.get_action_type)

Asynchronous method. Use `await get_action_type(...)` for a synchronous call.

Arguments mapping described in
[GetActionTypeInputRequestTypeDef](./type_defs.md#getactiontypeinputrequesttypedef).

Keyword-only arguments:

- `category`: [ActionCategoryType](./literals.md#actioncategorytype)
  *(required)*
- `owner`: `str` *(required)*
- `provider`: `str` *(required)*
- `version`: `str` *(required)*

Returns a `Coroutine` for
[GetActionTypeOutputTypeDef](./type_defs.md#getactiontypeoutputtypedef).

<a id="get_job_details"></a>

### get_job_details

Returns information about a job.

Type annotations for `session.create_client("codepipeline").get_job_details`
method.

Boto3 documentation:
[CodePipeline.Client.get_job_details](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.get_job_details)

Asynchronous method. Use `await get_job_details(...)` for a synchronous call.

Arguments mapping described in
[GetJobDetailsInputRequestTypeDef](./type_defs.md#getjobdetailsinputrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*

Returns a `Coroutine` for
[GetJobDetailsOutputTypeDef](./type_defs.md#getjobdetailsoutputtypedef).

<a id="get_pipeline"></a>

### get_pipeline

Returns the metadata, structure, stages, and actions of a pipeline.

Type annotations for `session.create_client("codepipeline").get_pipeline`
method.

Boto3 documentation:
[CodePipeline.Client.get_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.get_pipeline)

Asynchronous method. Use `await get_pipeline(...)` for a synchronous call.

Arguments mapping described in
[GetPipelineInputRequestTypeDef](./type_defs.md#getpipelineinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `version`: `int`

Returns a `Coroutine` for
[GetPipelineOutputTypeDef](./type_defs.md#getpipelineoutputtypedef).

<a id="get_pipeline_execution"></a>

### get_pipeline_execution

Returns information about an execution of a pipeline, including details about
artifacts, the pipeline execution ID, and the name, version, and status of the
pipeline.

Type annotations for
`session.create_client("codepipeline").get_pipeline_execution` method.

Boto3 documentation:
[CodePipeline.Client.get_pipeline_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.get_pipeline_execution)

Asynchronous method. Use `await get_pipeline_execution(...)` for a synchronous
call.

Arguments mapping described in
[GetPipelineExecutionInputRequestTypeDef](./type_defs.md#getpipelineexecutioninputrequesttypedef).

Keyword-only arguments:

- `pipelineName`: `str` *(required)*
- `pipelineExecutionId`: `str` *(required)*

Returns a `Coroutine` for
[GetPipelineExecutionOutputTypeDef](./type_defs.md#getpipelineexecutionoutputtypedef).

<a id="get_pipeline_state"></a>

### get_pipeline_state

Returns information about the state of a pipeline, including the stages and
actions.

Type annotations for `session.create_client("codepipeline").get_pipeline_state`
method.

Boto3 documentation:
[CodePipeline.Client.get_pipeline_state](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.get_pipeline_state)

Asynchronous method. Use `await get_pipeline_state(...)` for a synchronous
call.

Arguments mapping described in
[GetPipelineStateInputRequestTypeDef](./type_defs.md#getpipelinestateinputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*

Returns a `Coroutine` for
[GetPipelineStateOutputTypeDef](./type_defs.md#getpipelinestateoutputtypedef).

<a id="get_third_party_job_details"></a>

### get_third_party_job_details

Requests the details of a job for a third party action.

Type annotations for
`session.create_client("codepipeline").get_third_party_job_details` method.

Boto3 documentation:
[CodePipeline.Client.get_third_party_job_details](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.get_third_party_job_details)

Asynchronous method. Use `await get_third_party_job_details(...)` for a
synchronous call.

Arguments mapping described in
[GetThirdPartyJobDetailsInputRequestTypeDef](./type_defs.md#getthirdpartyjobdetailsinputrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `clientToken`: `str` *(required)*

Returns a `Coroutine` for
[GetThirdPartyJobDetailsOutputTypeDef](./type_defs.md#getthirdpartyjobdetailsoutputtypedef).

<a id="list_action_executions"></a>

### list_action_executions

Lists the action executions that have occurred in a pipeline.

Type annotations for
`session.create_client("codepipeline").list_action_executions` method.

Boto3 documentation:
[CodePipeline.Client.list_action_executions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_action_executions)

Asynchronous method. Use `await list_action_executions(...)` for a synchronous
call.

Arguments mapping described in
[ListActionExecutionsInputRequestTypeDef](./type_defs.md#listactionexecutionsinputrequesttypedef).

Keyword-only arguments:

- `pipelineName`: `str` *(required)*
- `filter`:
  [ActionExecutionFilterTypeDef](./type_defs.md#actionexecutionfiltertypedef)
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListActionExecutionsOutputTypeDef](./type_defs.md#listactionexecutionsoutputtypedef).

<a id="list_action_types"></a>

### list_action_types

Gets a summary of all AWS CodePipeline action types associated with your
account.

Type annotations for `session.create_client("codepipeline").list_action_types`
method.

Boto3 documentation:
[CodePipeline.Client.list_action_types](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_action_types)

Asynchronous method. Use `await list_action_types(...)` for a synchronous call.

Arguments mapping described in
[ListActionTypesInputRequestTypeDef](./type_defs.md#listactiontypesinputrequesttypedef).

Keyword-only arguments:

- `actionOwnerFilter`: [ActionOwnerType](./literals.md#actionownertype)
- `nextToken`: `str`
- `regionFilter`: `str`

Returns a `Coroutine` for
[ListActionTypesOutputTypeDef](./type_defs.md#listactiontypesoutputtypedef).

<a id="list_pipeline_executions"></a>

### list_pipeline_executions

Gets a summary of the most recent executions for a pipeline.

Type annotations for
`session.create_client("codepipeline").list_pipeline_executions` method.

Boto3 documentation:
[CodePipeline.Client.list_pipeline_executions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_pipeline_executions)

Asynchronous method. Use `await list_pipeline_executions(...)` for a
synchronous call.

Arguments mapping described in
[ListPipelineExecutionsInputRequestTypeDef](./type_defs.md#listpipelineexecutionsinputrequesttypedef).

Keyword-only arguments:

- `pipelineName`: `str` *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListPipelineExecutionsOutputTypeDef](./type_defs.md#listpipelineexecutionsoutputtypedef).

<a id="list_pipelines"></a>

### list_pipelines

Gets a summary of all of the pipelines associated with your account.

Type annotations for `session.create_client("codepipeline").list_pipelines`
method.

Boto3 documentation:
[CodePipeline.Client.list_pipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_pipelines)

Asynchronous method. Use `await list_pipelines(...)` for a synchronous call.

Arguments mapping described in
[ListPipelinesInputRequestTypeDef](./type_defs.md#listpipelinesinputrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListPipelinesOutputTypeDef](./type_defs.md#listpipelinesoutputtypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Gets the set of key-value pairs (metadata) that are used to manage the
resource.

Type annotations for
`session.create_client("codepipeline").list_tags_for_resource` method.

Boto3 documentation:
[CodePipeline.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef).

<a id="list_webhooks"></a>

### list_webhooks

Gets a listing of all the webhooks in this AWS Region for this account.

Type annotations for `session.create_client("codepipeline").list_webhooks`
method.

Boto3 documentation:
[CodePipeline.Client.list_webhooks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.list_webhooks)

Asynchronous method. Use `await list_webhooks(...)` for a synchronous call.

Arguments mapping described in
[ListWebhooksInputRequestTypeDef](./type_defs.md#listwebhooksinputrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListWebhooksOutputTypeDef](./type_defs.md#listwebhooksoutputtypedef).

<a id="poll_for_jobs"></a>

### poll_for_jobs

Returns information about any jobs for AWS CodePipeline to act on.

Type annotations for `session.create_client("codepipeline").poll_for_jobs`
method.

Boto3 documentation:
[CodePipeline.Client.poll_for_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.poll_for_jobs)

Asynchronous method. Use `await poll_for_jobs(...)` for a synchronous call.

Arguments mapping described in
[PollForJobsInputRequestTypeDef](./type_defs.md#pollforjobsinputrequesttypedef).

Keyword-only arguments:

- `actionTypeId`: [ActionTypeIdTypeDef](./type_defs.md#actiontypeidtypedef)
  *(required)*
- `maxBatchSize`: `int`
- `queryParam`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[PollForJobsOutputTypeDef](./type_defs.md#pollforjobsoutputtypedef).

<a id="poll_for_third_party_jobs"></a>

### poll_for_third_party_jobs

Determines whether there are any third party jobs for a job worker to act on.

Type annotations for
`session.create_client("codepipeline").poll_for_third_party_jobs` method.

Boto3 documentation:
[CodePipeline.Client.poll_for_third_party_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.poll_for_third_party_jobs)

Asynchronous method. Use `await poll_for_third_party_jobs(...)` for a
synchronous call.

Arguments mapping described in
[PollForThirdPartyJobsInputRequestTypeDef](./type_defs.md#pollforthirdpartyjobsinputrequesttypedef).

Keyword-only arguments:

- `actionTypeId`: [ActionTypeIdTypeDef](./type_defs.md#actiontypeidtypedef)
  *(required)*
- `maxBatchSize`: `int`

Returns a `Coroutine` for
[PollForThirdPartyJobsOutputTypeDef](./type_defs.md#pollforthirdpartyjobsoutputtypedef).

<a id="put_action_revision"></a>

### put_action_revision

Provides information to AWS CodePipeline about new revisions to a source.

Type annotations for
`session.create_client("codepipeline").put_action_revision` method.

Boto3 documentation:
[CodePipeline.Client.put_action_revision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_action_revision)

Asynchronous method. Use `await put_action_revision(...)` for a synchronous
call.

Arguments mapping described in
[PutActionRevisionInputRequestTypeDef](./type_defs.md#putactionrevisioninputrequesttypedef).

Keyword-only arguments:

- `pipelineName`: `str` *(required)*
- `stageName`: `str` *(required)*
- `actionName`: `str` *(required)*
- `actionRevision`:
  [ActionRevisionTypeDef](./type_defs.md#actionrevisiontypedef) *(required)*

Returns a `Coroutine` for
[PutActionRevisionOutputTypeDef](./type_defs.md#putactionrevisionoutputtypedef).

<a id="put_approval_result"></a>

### put_approval_result

Provides the response to a manual approval request to AWS CodePipeline.

Type annotations for
`session.create_client("codepipeline").put_approval_result` method.

Boto3 documentation:
[CodePipeline.Client.put_approval_result](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_approval_result)

Asynchronous method. Use `await put_approval_result(...)` for a synchronous
call.

Arguments mapping described in
[PutApprovalResultInputRequestTypeDef](./type_defs.md#putapprovalresultinputrequesttypedef).

Keyword-only arguments:

- `pipelineName`: `str` *(required)*
- `stageName`: `str` *(required)*
- `actionName`: `str` *(required)*
- `result`: [ApprovalResultTypeDef](./type_defs.md#approvalresulttypedef)
  *(required)*
- `token`: `str` *(required)*

Returns a `Coroutine` for
[PutApprovalResultOutputTypeDef](./type_defs.md#putapprovalresultoutputtypedef).

<a id="put_job_failure_result"></a>

### put_job_failure_result

Represents the failure of a job as returned to the pipeline by a job worker.

Type annotations for
`session.create_client("codepipeline").put_job_failure_result` method.

Boto3 documentation:
[CodePipeline.Client.put_job_failure_result](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_job_failure_result)

Asynchronous method. Use `await put_job_failure_result(...)` for a synchronous
call.

Arguments mapping described in
[PutJobFailureResultInputRequestTypeDef](./type_defs.md#putjobfailureresultinputrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `failureDetails`:
  [FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) *(required)*

<a id="put_job_success_result"></a>

### put_job_success_result

Represents the success of a job as returned to the pipeline by a job worker.

Type annotations for
`session.create_client("codepipeline").put_job_success_result` method.

Boto3 documentation:
[CodePipeline.Client.put_job_success_result](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_job_success_result)

Asynchronous method. Use `await put_job_success_result(...)` for a synchronous
call.

Arguments mapping described in
[PutJobSuccessResultInputRequestTypeDef](./type_defs.md#putjobsuccessresultinputrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `currentRevision`:
  [CurrentRevisionTypeDef](./type_defs.md#currentrevisiontypedef)
- `continuationToken`: `str`
- `executionDetails`:
  [ExecutionDetailsTypeDef](./type_defs.md#executiondetailstypedef)
- `outputVariables`: `Mapping`\[`str`, `str`\]

<a id="put_third_party_job_failure_result"></a>

### put_third_party_job_failure_result

Represents the failure of a third party job as returned to the pipeline by a
job worker.

Type annotations for
`session.create_client("codepipeline").put_third_party_job_failure_result`
method.

Boto3 documentation:
[CodePipeline.Client.put_third_party_job_failure_result](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_failure_result)

Asynchronous method. Use `await put_third_party_job_failure_result(...)` for a
synchronous call.

Arguments mapping described in
[PutThirdPartyJobFailureResultInputRequestTypeDef](./type_defs.md#putthirdpartyjobfailureresultinputrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `clientToken`: `str` *(required)*
- `failureDetails`:
  [FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) *(required)*

<a id="put_third_party_job_success_result"></a>

### put_third_party_job_success_result

Represents the success of a third party job as returned to the pipeline by a
job worker.

Type annotations for
`session.create_client("codepipeline").put_third_party_job_success_result`
method.

Boto3 documentation:
[CodePipeline.Client.put_third_party_job_success_result](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_third_party_job_success_result)

Asynchronous method. Use `await put_third_party_job_success_result(...)` for a
synchronous call.

Arguments mapping described in
[PutThirdPartyJobSuccessResultInputRequestTypeDef](./type_defs.md#putthirdpartyjobsuccessresultinputrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `clientToken`: `str` *(required)*
- `currentRevision`:
  [CurrentRevisionTypeDef](./type_defs.md#currentrevisiontypedef)
- `continuationToken`: `str`
- `executionDetails`:
  [ExecutionDetailsTypeDef](./type_defs.md#executiondetailstypedef)

<a id="put_webhook"></a>

### put_webhook

Defines a webhook and returns a unique webhook URL generated by CodePipeline.

Type annotations for `session.create_client("codepipeline").put_webhook`
method.

Boto3 documentation:
[CodePipeline.Client.put_webhook](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.put_webhook)

Asynchronous method. Use `await put_webhook(...)` for a synchronous call.

Arguments mapping described in
[PutWebhookInputRequestTypeDef](./type_defs.md#putwebhookinputrequesttypedef).

Keyword-only arguments:

- `webhook`:
  [WebhookDefinitionTypeDef](./type_defs.md#webhookdefinitiontypedef)
  *(required)*
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[PutWebhookOutputTypeDef](./type_defs.md#putwebhookoutputtypedef).

<a id="register_webhook_with_third_party"></a>

### register_webhook_with_third_party

Configures a connection between the webhook that was created and the external
tool with events to be detected.

Type annotations for
`session.create_client("codepipeline").register_webhook_with_third_party`
method.

Boto3 documentation:
[CodePipeline.Client.register_webhook_with_third_party](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.register_webhook_with_third_party)

Asynchronous method. Use `await register_webhook_with_third_party(...)` for a
synchronous call.

Arguments mapping described in
[RegisterWebhookWithThirdPartyInputRequestTypeDef](./type_defs.md#registerwebhookwiththirdpartyinputrequesttypedef).

Keyword-only arguments:

- `webhookName`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="retry_stage_execution"></a>

### retry_stage_execution

Resumes the pipeline execution by retrying the last failed actions in a stage.

Type annotations for
`session.create_client("codepipeline").retry_stage_execution` method.

Boto3 documentation:
[CodePipeline.Client.retry_stage_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.retry_stage_execution)

Asynchronous method. Use `await retry_stage_execution(...)` for a synchronous
call.

Arguments mapping described in
[RetryStageExecutionInputRequestTypeDef](./type_defs.md#retrystageexecutioninputrequesttypedef).

Keyword-only arguments:

- `pipelineName`: `str` *(required)*
- `stageName`: `str` *(required)*
- `pipelineExecutionId`: `str` *(required)*
- `retryMode`: `Literal['FAILED_ACTIONS']` (see
  [StageRetryModeType](./literals.md#stageretrymodetype)) *(required)*

Returns a `Coroutine` for
[RetryStageExecutionOutputTypeDef](./type_defs.md#retrystageexecutionoutputtypedef).

<a id="start_pipeline_execution"></a>

### start_pipeline_execution

Starts the specified pipeline.

Type annotations for
`session.create_client("codepipeline").start_pipeline_execution` method.

Boto3 documentation:
[CodePipeline.Client.start_pipeline_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.start_pipeline_execution)

Asynchronous method. Use `await start_pipeline_execution(...)` for a
synchronous call.

Arguments mapping described in
[StartPipelineExecutionInputRequestTypeDef](./type_defs.md#startpipelineexecutioninputrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `clientRequestToken`: `str`

Returns a `Coroutine` for
[StartPipelineExecutionOutputTypeDef](./type_defs.md#startpipelineexecutionoutputtypedef).

<a id="stop_pipeline_execution"></a>

### stop_pipeline_execution

Stops the specified pipeline execution.

Type annotations for
`session.create_client("codepipeline").stop_pipeline_execution` method.

Boto3 documentation:
[CodePipeline.Client.stop_pipeline_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.stop_pipeline_execution)

Asynchronous method. Use `await stop_pipeline_execution(...)` for a synchronous
call.

Arguments mapping described in
[StopPipelineExecutionInputRequestTypeDef](./type_defs.md#stoppipelineexecutioninputrequesttypedef).

Keyword-only arguments:

- `pipelineName`: `str` *(required)*
- `pipelineExecutionId`: `str` *(required)*
- `abandon`: `bool`
- `reason`: `str`

Returns a `Coroutine` for
[StopPipelineExecutionOutputTypeDef](./type_defs.md#stoppipelineexecutionoutputtypedef).

<a id="tag_resource"></a>

### tag_resource

Adds to or modifies the tags of the given resource.

Type annotations for `session.create_client("codepipeline").tag_resource`
method.

Boto3 documentation:
[CodePipeline.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes tags from an AWS resource.

Type annotations for `session.create_client("codepipeline").untag_resource`
method.

Boto3 documentation:
[CodePipeline.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_action_type"></a>

### update_action_type

Updates an action type that was created with any supported integration model,
where the action type is to be used by customers of the action type provider.

Type annotations for `session.create_client("codepipeline").update_action_type`
method.

Boto3 documentation:
[CodePipeline.Client.update_action_type](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_action_type)

Asynchronous method. Use `await update_action_type(...)` for a synchronous
call.

Arguments mapping described in
[UpdateActionTypeInputRequestTypeDef](./type_defs.md#updateactiontypeinputrequesttypedef).

Keyword-only arguments:

- `actionType`:
  [ActionTypeDeclarationTypeDef](./type_defs.md#actiontypedeclarationtypedef)
  *(required)*

<a id="update_pipeline"></a>

### update_pipeline

Updates a specified pipeline with edits or changes to its structure.

Type annotations for `session.create_client("codepipeline").update_pipeline`
method.

Boto3 documentation:
[CodePipeline.Client.update_pipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.update_pipeline)

Asynchronous method. Use `await update_pipeline(...)` for a synchronous call.

Arguments mapping described in
[UpdatePipelineInputRequestTypeDef](./type_defs.md#updatepipelineinputrequesttypedef).

Keyword-only arguments:

- `pipeline`:
  [PipelineDeclarationTypeDef](./type_defs.md#pipelinedeclarationtypedef)
  *(required)*

Returns a `Coroutine` for
[UpdatePipelineOutputTypeDef](./type_defs.md#updatepipelineoutputtypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("codepipeline").__aenter__` method.

Boto3 documentation:
[CodePipeline.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [CodePipelineClient](#codepipelineclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("codepipeline").__aexit__` method.

Boto3 documentation:
[CodePipeline.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#CodePipeline.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("codepipeline").get_paginator`
method with overloads.

- `client.get_paginator("list_action_executions")` ->
  [ListActionExecutionsPaginator](./paginators.md#listactionexecutionspaginator)
- `client.get_paginator("list_action_types")` ->
  [ListActionTypesPaginator](./paginators.md#listactiontypespaginator)
- `client.get_paginator("list_pipeline_executions")` ->
  [ListPipelineExecutionsPaginator](./paginators.md#listpipelineexecutionspaginator)
- `client.get_paginator("list_pipelines")` ->
  [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
- `client.get_paginator("list_tags_for_resource")` ->
  [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("list_webhooks")` ->
  [ListWebhooksPaginator](./paginators.md#listwebhookspaginator)
