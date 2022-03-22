<a id="batchclient-for-aiobotocore-batch-module"></a>

# BatchClient for aiobotocore Batch module

> [Index](../README.md) > [Batch](./README.md) > BatchClient

Auto-generated documentation for
[Batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
type annotations stubs module
[types-aiobotocore-batch](https://pypi.org/project/types-aiobotocore-batch/).

- [BatchClient for aiobotocore Batch module](#batchclient-for-aiobotocore-batch-module)
  - [BatchClient](#batchclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [cancel_job](#cancel_job)
    - [create_compute_environment](#create_compute_environment)
    - [create_job_queue](#create_job_queue)
    - [create_scheduling_policy](#create_scheduling_policy)
    - [delete_compute_environment](#delete_compute_environment)
    - [delete_job_queue](#delete_job_queue)
    - [delete_scheduling_policy](#delete_scheduling_policy)
    - [deregister_job_definition](#deregister_job_definition)
    - [describe_compute_environments](#describe_compute_environments)
    - [describe_job_definitions](#describe_job_definitions)
    - [describe_job_queues](#describe_job_queues)
    - [describe_jobs](#describe_jobs)
    - [describe_scheduling_policies](#describe_scheduling_policies)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_jobs](#list_jobs)
    - [list_scheduling_policies](#list_scheduling_policies)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [register_job_definition](#register_job_definition)
    - [submit_job](#submit_job)
    - [tag_resource](#tag_resource)
    - [terminate_job](#terminate_job)
    - [untag_resource](#untag_resource)
    - [update_compute_environment](#update_compute_environment)
    - [update_job_queue](#update_job_queue)
    - [update_scheduling_policy](#update_scheduling_policy)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="batchclient"></a>

## BatchClient

Type annotations for `session.create_client("batch")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_batch.client import BatchClient

session = get_session()
async with session.create_client("batch") as client:
    client: BatchClient
```

Boto3 documentation:
[Batch.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_batch.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ClientException`
- `Exceptions.ServerException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

BatchClient exceptions.

Type annotations for `session.create_client("batch").exceptions` method.

Boto3 documentation:
[Batch.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("batch").can_paginate` method.

Boto3 documentation:
[Batch.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_job"></a>

### cancel_job

Cancels a job in an Batch job queue.

Type annotations for `session.create_client("batch").cancel_job` method.

Boto3 documentation:
[Batch.Client.cancel_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.cancel_job)

Asynchronous method. Use `await cancel_job(...)` for a synchronous call.

Arguments mapping described in
[CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `reason`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create\_compute\_environment"></a>

### create_compute_environment

Creates an Batch compute environment.

Type annotations for
`session.create_client("batch").create_compute_environment` method.

Boto3 documentation:
[Batch.Client.create_compute_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_compute_environment)

Asynchronous method. Use `await create_compute_environment(...)` for a
synchronous call.

Arguments mapping described in
[CreateComputeEnvironmentRequestRequestTypeDef](./type_defs.md#createcomputeenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `computeEnvironmentName`: `str` *(required)*
- `type`: [CETypeType](./literals.md#cetypetype) *(required)*
- `state`: [CEStateType](./literals.md#cestatetype)
- `unmanagedvCpus`: `int`
- `computeResources`:
  [ComputeResourceTypeDef](./type_defs.md#computeresourcetypedef)
- `serviceRole`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateComputeEnvironmentResponseTypeDef](./type_defs.md#createcomputeenvironmentresponsetypedef).

<a id="create\_job\_queue"></a>

### create_job_queue

Creates an Batch job queue.

Type annotations for `session.create_client("batch").create_job_queue` method.

Boto3 documentation:
[Batch.Client.create_job_queue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_job_queue)

Asynchronous method. Use `await create_job_queue(...)` for a synchronous call.

Arguments mapping described in
[CreateJobQueueRequestRequestTypeDef](./type_defs.md#createjobqueuerequestrequesttypedef).

Keyword-only arguments:

- `jobQueueName`: `str` *(required)*
- `priority`: `int` *(required)*
- `computeEnvironmentOrder`:
  `Sequence`\[[ComputeEnvironmentOrderTypeDef](./type_defs.md#computeenvironmentordertypedef)\]
  *(required)*
- `state`: [JQStateType](./literals.md#jqstatetype)
- `schedulingPolicyArn`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateJobQueueResponseTypeDef](./type_defs.md#createjobqueueresponsetypedef).

<a id="create\_scheduling\_policy"></a>

### create_scheduling_policy

Creates an Batch scheduling policy.

Type annotations for `session.create_client("batch").create_scheduling_policy`
method.

Boto3 documentation:
[Batch.Client.create_scheduling_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.create_scheduling_policy)

Asynchronous method. Use `await create_scheduling_policy(...)` for a
synchronous call.

Arguments mapping described in
[CreateSchedulingPolicyRequestRequestTypeDef](./type_defs.md#createschedulingpolicyrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `fairsharePolicy`:
  [FairsharePolicyTypeDef](./type_defs.md#fairsharepolicytypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateSchedulingPolicyResponseTypeDef](./type_defs.md#createschedulingpolicyresponsetypedef).

<a id="delete\_compute\_environment"></a>

### delete_compute_environment

Deletes an Batch compute environment.

Type annotations for
`session.create_client("batch").delete_compute_environment` method.

Boto3 documentation:
[Batch.Client.delete_compute_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.delete_compute_environment)

Asynchronous method. Use `await delete_compute_environment(...)` for a
synchronous call.

Arguments mapping described in
[DeleteComputeEnvironmentRequestRequestTypeDef](./type_defs.md#deletecomputeenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `computeEnvironment`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_job\_queue"></a>

### delete_job_queue

Deletes the specified job queue.

Type annotations for `session.create_client("batch").delete_job_queue` method.

Boto3 documentation:
[Batch.Client.delete_job_queue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.delete_job_queue)

Asynchronous method. Use `await delete_job_queue(...)` for a synchronous call.

Arguments mapping described in
[DeleteJobQueueRequestRequestTypeDef](./type_defs.md#deletejobqueuerequestrequesttypedef).

Keyword-only arguments:

- `jobQueue`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_scheduling\_policy"></a>

### delete_scheduling_policy

Deletes the specified scheduling policy.

Type annotations for `session.create_client("batch").delete_scheduling_policy`
method.

Boto3 documentation:
[Batch.Client.delete_scheduling_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.delete_scheduling_policy)

Asynchronous method. Use `await delete_scheduling_policy(...)` for a
synchronous call.

Arguments mapping described in
[DeleteSchedulingPolicyRequestRequestTypeDef](./type_defs.md#deleteschedulingpolicyrequestrequesttypedef).

Keyword-only arguments:

- `arn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="deregister\_job\_definition"></a>

### deregister_job_definition

Deregisters an Batch job definition.

Type annotations for `session.create_client("batch").deregister_job_definition`
method.

Boto3 documentation:
[Batch.Client.deregister_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.deregister_job_definition)

Asynchronous method. Use `await deregister_job_definition(...)` for a
synchronous call.

Arguments mapping described in
[DeregisterJobDefinitionRequestRequestTypeDef](./type_defs.md#deregisterjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `jobDefinition`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe\_compute\_environments"></a>

### describe_compute_environments

Describes one or more of your compute environments.

Type annotations for
`session.create_client("batch").describe_compute_environments` method.

Boto3 documentation:
[Batch.Client.describe_compute_environments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_compute_environments)

Asynchronous method. Use `await describe_compute_environments(...)` for a
synchronous call.

Arguments mapping described in
[DescribeComputeEnvironmentsRequestRequestTypeDef](./type_defs.md#describecomputeenvironmentsrequestrequesttypedef).

Keyword-only arguments:

- `computeEnvironments`: `Sequence`\[`str`\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[DescribeComputeEnvironmentsResponseTypeDef](./type_defs.md#describecomputeenvironmentsresponsetypedef).

<a id="describe\_job\_definitions"></a>

### describe_job_definitions

Describes a list of job definitions.

Type annotations for `session.create_client("batch").describe_job_definitions`
method.

Boto3 documentation:
[Batch.Client.describe_job_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_job_definitions)

Asynchronous method. Use `await describe_job_definitions(...)` for a
synchronous call.

Arguments mapping described in
[DescribeJobDefinitionsRequestRequestTypeDef](./type_defs.md#describejobdefinitionsrequestrequesttypedef).

Keyword-only arguments:

- `jobDefinitions`: `Sequence`\[`str`\]
- `maxResults`: `int`
- `jobDefinitionName`: `str`
- `status`: `str`
- `nextToken`: `str`

Returns a `Coroutine` for
[DescribeJobDefinitionsResponseTypeDef](./type_defs.md#describejobdefinitionsresponsetypedef).

<a id="describe\_job\_queues"></a>

### describe_job_queues

Describes one or more of your job queues.

Type annotations for `session.create_client("batch").describe_job_queues`
method.

Boto3 documentation:
[Batch.Client.describe_job_queues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_job_queues)

Asynchronous method. Use `await describe_job_queues(...)` for a synchronous
call.

Arguments mapping described in
[DescribeJobQueuesRequestRequestTypeDef](./type_defs.md#describejobqueuesrequestrequesttypedef).

Keyword-only arguments:

- `jobQueues`: `Sequence`\[`str`\]
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[DescribeJobQueuesResponseTypeDef](./type_defs.md#describejobqueuesresponsetypedef).

<a id="describe\_jobs"></a>

### describe_jobs

.

Type annotations for `session.create_client("batch").describe_jobs` method.

Boto3 documentation:
[Batch.Client.describe_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_jobs)

Asynchronous method. Use `await describe_jobs(...)` for a synchronous call.

Arguments mapping described in
[DescribeJobsRequestRequestTypeDef](./type_defs.md#describejobsrequestrequesttypedef).

Keyword-only arguments:

- `jobs`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef).

<a id="describe\_scheduling\_policies"></a>

### describe_scheduling_policies

Describes one or more of your scheduling policies.

Type annotations for
`session.create_client("batch").describe_scheduling_policies` method.

Boto3 documentation:
[Batch.Client.describe_scheduling_policies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.describe_scheduling_policies)

Asynchronous method. Use `await describe_scheduling_policies(...)` for a
synchronous call.

Arguments mapping described in
[DescribeSchedulingPoliciesRequestRequestTypeDef](./type_defs.md#describeschedulingpoliciesrequestrequesttypedef).

Keyword-only arguments:

- `arns`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DescribeSchedulingPoliciesResponseTypeDef](./type_defs.md#describeschedulingpoliciesresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("batch").generate_presigned_url`
method.

Boto3 documentation:
[Batch.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_jobs"></a>

### list_jobs

Returns a list of Batch jobs.

Type annotations for `session.create_client("batch").list_jobs` method.

Boto3 documentation:
[Batch.Client.list_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_jobs)

Asynchronous method. Use `await list_jobs(...)` for a synchronous call.

Arguments mapping described in
[ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef).

Keyword-only arguments:

- `jobQueue`: `str`
- `arrayJobId`: `str`
- `multiNodeJobId`: `str`
- `jobStatus`: [JobStatusType](./literals.md#jobstatustype)
- `maxResults`: `int`
- `nextToken`: `str`
- `filters`:
  `Sequence`\[[KeyValuesPairTypeDef](./type_defs.md#keyvaluespairtypedef)\]

Returns a `Coroutine` for
[ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef).

<a id="list\_scheduling\_policies"></a>

### list_scheduling_policies

Returns a list of Batch scheduling policies.

Type annotations for `session.create_client("batch").list_scheduling_policies`
method.

Boto3 documentation:
[Batch.Client.list_scheduling_policies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_scheduling_policies)

Asynchronous method. Use `await list_scheduling_policies(...)` for a
synchronous call.

Arguments mapping described in
[ListSchedulingPoliciesRequestRequestTypeDef](./type_defs.md#listschedulingpoliciesrequestrequesttypedef).

Keyword-only arguments:

- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListSchedulingPoliciesResponseTypeDef](./type_defs.md#listschedulingpoliciesresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists the tags for an Batch resource.

Type annotations for `session.create_client("batch").list_tags_for_resource`
method.

Boto3 documentation:
[Batch.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="register\_job\_definition"></a>

### register_job_definition

Registers an Batch job definition.

Type annotations for `session.create_client("batch").register_job_definition`
method.

Boto3 documentation:
[Batch.Client.register_job_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.register_job_definition)

Asynchronous method. Use `await register_job_definition(...)` for a synchronous
call.

Arguments mapping described in
[RegisterJobDefinitionRequestRequestTypeDef](./type_defs.md#registerjobdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `jobDefinitionName`: `str` *(required)*
- `type`: [JobDefinitionTypeType](./literals.md#jobdefinitiontypetype)
  *(required)*
- `parameters`: `Mapping`\[`str`, `str`\]
- `schedulingPriority`: `int`
- `containerProperties`:
  [ContainerPropertiesTypeDef](./type_defs.md#containerpropertiestypedef)
- `nodeProperties`:
  [NodePropertiesTypeDef](./type_defs.md#nodepropertiestypedef)
- `retryStrategy`: [RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef)
- `propagateTags`: `bool`
- `timeout`: [JobTimeoutTypeDef](./type_defs.md#jobtimeouttypedef)
- `tags`: `Mapping`\[`str`, `str`\]
- `platformCapabilities`:
  `Sequence`\[[PlatformCapabilityType](./literals.md#platformcapabilitytype)\]

Returns a `Coroutine` for
[RegisterJobDefinitionResponseTypeDef](./type_defs.md#registerjobdefinitionresponsetypedef).

<a id="submit\_job"></a>

### submit_job

Submits an Batch job from a job definition.

Type annotations for `session.create_client("batch").submit_job` method.

Boto3 documentation:
[Batch.Client.submit_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.submit_job)

Asynchronous method. Use `await submit_job(...)` for a synchronous call.

Arguments mapping described in
[SubmitJobRequestRequestTypeDef](./type_defs.md#submitjobrequestrequesttypedef).

Keyword-only arguments:

- `jobName`: `str` *(required)*
- `jobQueue`: `str` *(required)*
- `jobDefinition`: `str` *(required)*
- `shareIdentifier`: `str`
- `schedulingPriorityOverride`: `int`
- `arrayProperties`:
  [ArrayPropertiesTypeDef](./type_defs.md#arraypropertiestypedef)
- `dependsOn`:
  `Sequence`\[[JobDependencyTypeDef](./type_defs.md#jobdependencytypedef)\]
- `parameters`: `Mapping`\[`str`, `str`\]
- `containerOverrides`:
  [ContainerOverridesTypeDef](./type_defs.md#containeroverridestypedef)
- `nodeOverrides`: [NodeOverridesTypeDef](./type_defs.md#nodeoverridestypedef)
- `retryStrategy`: [RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef)
- `propagateTags`: `bool`
- `timeout`: [JobTimeoutTypeDef](./type_defs.md#jobtimeouttypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[SubmitJobResponseTypeDef](./type_defs.md#submitjobresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Associates the specified tags to a resource with the specified `resourceArn`.

Type annotations for `session.create_client("batch").tag_resource` method.

Boto3 documentation:
[Batch.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="terminate\_job"></a>

### terminate_job

Terminates a job in a job queue.

Type annotations for `session.create_client("batch").terminate_job` method.

Boto3 documentation:
[Batch.Client.terminate_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.terminate_job)

Asynchronous method. Use `await terminate_job(...)` for a synchronous call.

Arguments mapping described in
[TerminateJobRequestRequestTypeDef](./type_defs.md#terminatejobrequestrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `reason`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Deletes specified tags from an Batch resource.

Type annotations for `session.create_client("batch").untag_resource` method.

Boto3 documentation:
[Batch.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_compute\_environment"></a>

### update_compute_environment

Updates an Batch compute environment.

Type annotations for
`session.create_client("batch").update_compute_environment` method.

Boto3 documentation:
[Batch.Client.update_compute_environment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_compute_environment)

Asynchronous method. Use `await update_compute_environment(...)` for a
synchronous call.

Arguments mapping described in
[UpdateComputeEnvironmentRequestRequestTypeDef](./type_defs.md#updatecomputeenvironmentrequestrequesttypedef).

Keyword-only arguments:

- `computeEnvironment`: `str` *(required)*
- `state`: [CEStateType](./literals.md#cestatetype)
- `unmanagedvCpus`: `int`
- `computeResources`:
  [ComputeResourceUpdateTypeDef](./type_defs.md#computeresourceupdatetypedef)
- `serviceRole`: `str`

Returns a `Coroutine` for
[UpdateComputeEnvironmentResponseTypeDef](./type_defs.md#updatecomputeenvironmentresponsetypedef).

<a id="update\_job\_queue"></a>

### update_job_queue

Updates a job queue.

Type annotations for `session.create_client("batch").update_job_queue` method.

Boto3 documentation:
[Batch.Client.update_job_queue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_job_queue)

Asynchronous method. Use `await update_job_queue(...)` for a synchronous call.

Arguments mapping described in
[UpdateJobQueueRequestRequestTypeDef](./type_defs.md#updatejobqueuerequestrequesttypedef).

Keyword-only arguments:

- `jobQueue`: `str` *(required)*
- `state`: [JQStateType](./literals.md#jqstatetype)
- `schedulingPolicyArn`: `str`
- `priority`: `int`
- `computeEnvironmentOrder`:
  `Sequence`\[[ComputeEnvironmentOrderTypeDef](./type_defs.md#computeenvironmentordertypedef)\]

Returns a `Coroutine` for
[UpdateJobQueueResponseTypeDef](./type_defs.md#updatejobqueueresponsetypedef).

<a id="update\_scheduling\_policy"></a>

### update_scheduling_policy

Updates a scheduling policy.

Type annotations for `session.create_client("batch").update_scheduling_policy`
method.

Boto3 documentation:
[Batch.Client.update_scheduling_policy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.update_scheduling_policy)

Asynchronous method. Use `await update_scheduling_policy(...)` for a
synchronous call.

Arguments mapping described in
[UpdateSchedulingPolicyRequestRequestTypeDef](./type_defs.md#updateschedulingpolicyrequestrequesttypedef).

Keyword-only arguments:

- `arn`: `str` *(required)*
- `fairsharePolicy`:
  [FairsharePolicyTypeDef](./type_defs.md#fairsharepolicytypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("batch").__aenter__` method.

Boto3 documentation:
[Batch.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [BatchClient](#batchclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("batch").__aexit__` method.

Boto3 documentation:
[Batch.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("batch").get_paginator` method with
overloads.

- `client.get_paginator("describe_compute_environments")` ->
  [DescribeComputeEnvironmentsPaginator](./paginators.md#describecomputeenvironmentspaginator)
- `client.get_paginator("describe_job_definitions")` ->
  [DescribeJobDefinitionsPaginator](./paginators.md#describejobdefinitionspaginator)
- `client.get_paginator("describe_job_queues")` ->
  [DescribeJobQueuesPaginator](./paginators.md#describejobqueuespaginator)
- `client.get_paginator("list_jobs")` ->
  [ListJobsPaginator](./paginators.md#listjobspaginator)
- `client.get_paginator("list_scheduling_policies")` ->
  [ListSchedulingPoliciesPaginator](./paginators.md#listschedulingpoliciespaginator)
