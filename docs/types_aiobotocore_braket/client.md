<a id="braketclient-for-aiobotocore-braket-module"></a>

# BraketClient for aiobotocore Braket module

> [Index](../README.md) > [Braket](./README.md) > BraketClient

Auto-generated documentation for
[Braket](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
type annotations stubs module
[types-aiobotocore-braket](https://pypi.org/project/types-aiobotocore-braket/).

- [BraketClient for aiobotocore Braket module](#braketclient-for-aiobotocore-braket-module)
  - [BraketClient](#braketclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [cancel_job](#cancel_job)
    - [cancel_quantum_task](#cancel_quantum_task)
    - [create_job](#create_job)
    - [create_quantum_task](#create_quantum_task)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_device](#get_device)
    - [get_job](#get_job)
    - [get_quantum_task](#get_quantum_task)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [search_devices](#search_devices)
    - [search_jobs](#search_jobs)
    - [search_quantum_tasks](#search_quantum_tasks)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="braketclient"></a>

## BraketClient

Type annotations for `session.create_client("braket")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_braket.client import BraketClient

session = get_session()
async with session.create_client("braket") as client:
    client: BraketClient
```

Boto3 documentation:
[Braket.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_braket.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.DeviceOfflineException`
- `Exceptions.DeviceRetiredException`
- `Exceptions.InternalServiceException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

BraketClient exceptions.

Type annotations for `session.create_client("braket").exceptions` method.

Boto3 documentation:
[Braket.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("braket").can_paginate` method.

Boto3 documentation:
[Braket.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_job"></a>

### cancel_job

Cancels an Amazon Braket job.

Type annotations for `session.create_client("braket").cancel_job` method.

Boto3 documentation:
[Braket.Client.cancel_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.cancel_job)

Asynchronous method. Use `await cancel_job(...)` for a synchronous call.

Arguments mapping described in
[CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef).

Keyword-only arguments:

- `jobArn`: `str` *(required)*

Returns a `Coroutine` for
[CancelJobResponseTypeDef](./type_defs.md#canceljobresponsetypedef).

<a id="cancel\_quantum\_task"></a>

### cancel_quantum_task

Cancels the specified task.

Type annotations for `session.create_client("braket").cancel_quantum_task`
method.

Boto3 documentation:
[Braket.Client.cancel_quantum_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.cancel_quantum_task)

Asynchronous method. Use `await cancel_quantum_task(...)` for a synchronous
call.

Arguments mapping described in
[CancelQuantumTaskRequestRequestTypeDef](./type_defs.md#cancelquantumtaskrequestrequesttypedef).

Keyword-only arguments:

- `clientToken`: `str` *(required)*
- `quantumTaskArn`: `str` *(required)*

Returns a `Coroutine` for
[CancelQuantumTaskResponseTypeDef](./type_defs.md#cancelquantumtaskresponsetypedef).

<a id="create\_job"></a>

### create_job

Creates an Amazon Braket job.

Type annotations for `session.create_client("braket").create_job` method.

Boto3 documentation:
[Braket.Client.create_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.create_job)

Asynchronous method. Use `await create_job(...)` for a synchronous call.

Arguments mapping described in
[CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef).

Keyword-only arguments:

- `algorithmSpecification`:
  [AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef)
  *(required)*
- `clientToken`: `str` *(required)*
- `deviceConfig`: [DeviceConfigTypeDef](./type_defs.md#deviceconfigtypedef)
  *(required)*
- `instanceConfig`:
  [InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef) *(required)*
- `jobName`: `str` *(required)*
- `outputDataConfig`:
  [JobOutputDataConfigTypeDef](./type_defs.md#joboutputdataconfigtypedef)
  *(required)*
- `roleArn`: `str` *(required)*
- `checkpointConfig`:
  [JobCheckpointConfigTypeDef](./type_defs.md#jobcheckpointconfigtypedef)
- `hyperParameters`: `Mapping`\[`str`, `str`\]
- `inputDataConfig`:
  `Sequence`\[[InputFileConfigTypeDef](./type_defs.md#inputfileconfigtypedef)\]
- `stoppingCondition`:
  [JobStoppingConditionTypeDef](./type_defs.md#jobstoppingconditiontypedef)
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateJobResponseTypeDef](./type_defs.md#createjobresponsetypedef).

<a id="create\_quantum\_task"></a>

### create_quantum_task

Creates a quantum task.

Type annotations for `session.create_client("braket").create_quantum_task`
method.

Boto3 documentation:
[Braket.Client.create_quantum_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.create_quantum_task)

Asynchronous method. Use `await create_quantum_task(...)` for a synchronous
call.

Arguments mapping described in
[CreateQuantumTaskRequestRequestTypeDef](./type_defs.md#createquantumtaskrequestrequesttypedef).

Keyword-only arguments:

- `action`: `str` *(required)*
- `clientToken`: `str` *(required)*
- `deviceArn`: `str` *(required)*
- `outputS3Bucket`: `str` *(required)*
- `outputS3KeyPrefix`: `str` *(required)*
- `shots`: `int` *(required)*
- `deviceParameters`: `str`
- `jobToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateQuantumTaskResponseTypeDef](./type_defs.md#createquantumtaskresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("braket").generate_presigned_url`
method.

Boto3 documentation:
[Braket.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_device"></a>

### get_device

Retrieves the devices available in Amazon Braket.

Type annotations for `session.create_client("braket").get_device` method.

Boto3 documentation:
[Braket.Client.get_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.get_device)

Asynchronous method. Use `await get_device(...)` for a synchronous call.

Arguments mapping described in
[GetDeviceRequestRequestTypeDef](./type_defs.md#getdevicerequestrequesttypedef).

Keyword-only arguments:

- `deviceArn`: `str` *(required)*

Returns a `Coroutine` for
[GetDeviceResponseTypeDef](./type_defs.md#getdeviceresponsetypedef).

<a id="get\_job"></a>

### get_job

Retrieves the specified Amazon Braket job.

Type annotations for `session.create_client("braket").get_job` method.

Boto3 documentation:
[Braket.Client.get_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.get_job)

Asynchronous method. Use `await get_job(...)` for a synchronous call.

Arguments mapping described in
[GetJobRequestRequestTypeDef](./type_defs.md#getjobrequestrequesttypedef).

Keyword-only arguments:

- `jobArn`: `str` *(required)*

Returns a `Coroutine` for
[GetJobResponseTypeDef](./type_defs.md#getjobresponsetypedef).

<a id="get\_quantum\_task"></a>

### get_quantum_task

Retrieves the specified quantum task.

Type annotations for `session.create_client("braket").get_quantum_task` method.

Boto3 documentation:
[Braket.Client.get_quantum_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.get_quantum_task)

Asynchronous method. Use `await get_quantum_task(...)` for a synchronous call.

Arguments mapping described in
[GetQuantumTaskRequestRequestTypeDef](./type_defs.md#getquantumtaskrequestrequesttypedef).

Keyword-only arguments:

- `quantumTaskArn`: `str` *(required)*

Returns a `Coroutine` for
[GetQuantumTaskResponseTypeDef](./type_defs.md#getquantumtaskresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Shows the tags associated with this resource.

Type annotations for `session.create_client("braket").list_tags_for_resource`
method.

Boto3 documentation:
[Braket.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="search\_devices"></a>

### search_devices

Searches for devices using the specified filters.

Type annotations for `session.create_client("braket").search_devices` method.

Boto3 documentation:
[Braket.Client.search_devices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_devices)

Asynchronous method. Use `await search_devices(...)` for a synchronous call.

Arguments mapping described in
[SearchDevicesRequestRequestTypeDef](./type_defs.md#searchdevicesrequestrequesttypedef).

Keyword-only arguments:

- `filters`:
  `Sequence`\[[SearchDevicesFilterTypeDef](./type_defs.md#searchdevicesfiltertypedef)\]
  *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef).

<a id="search\_jobs"></a>

### search_jobs

Searches for Amazon Braket jobs that match the specified filter values.

Type annotations for `session.create_client("braket").search_jobs` method.

Boto3 documentation:
[Braket.Client.search_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_jobs)

Asynchronous method. Use `await search_jobs(...)` for a synchronous call.

Arguments mapping described in
[SearchJobsRequestRequestTypeDef](./type_defs.md#searchjobsrequestrequesttypedef).

Keyword-only arguments:

- `filters`:
  `Sequence`\[[SearchJobsFilterTypeDef](./type_defs.md#searchjobsfiltertypedef)\]
  *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[SearchJobsResponseTypeDef](./type_defs.md#searchjobsresponsetypedef).

<a id="search\_quantum\_tasks"></a>

### search_quantum_tasks

Searches for tasks that match the specified filter values.

Type annotations for `session.create_client("braket").search_quantum_tasks`
method.

Boto3 documentation:
[Braket.Client.search_quantum_tasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_quantum_tasks)

Asynchronous method. Use `await search_quantum_tasks(...)` for a synchronous
call.

Arguments mapping described in
[SearchQuantumTasksRequestRequestTypeDef](./type_defs.md#searchquantumtasksrequestrequesttypedef).

Keyword-only arguments:

- `filters`:
  `Sequence`\[[SearchQuantumTasksFilterTypeDef](./type_defs.md#searchquantumtasksfiltertypedef)\]
  *(required)*
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[SearchQuantumTasksResponseTypeDef](./type_defs.md#searchquantumtasksresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Add a tag to the specified resource.

Type annotations for `session.create_client("braket").tag_resource` method.

Boto3 documentation:
[Braket.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Remove tags from a resource.

Type annotations for `session.create_client("braket").untag_resource` method.

Boto3 documentation:
[Braket.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("braket").__aenter__` method.

Boto3 documentation:
[Braket.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [BraketClient](#braketclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("braket").__aexit__` method.

Boto3 documentation:
[Braket.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("braket").get_paginator` method
with overloads.

- `client.get_paginator("search_devices")` ->
  [SearchDevicesPaginator](./paginators.md#searchdevicespaginator)
- `client.get_paginator("search_jobs")` ->
  [SearchJobsPaginator](./paginators.md#searchjobspaginator)
- `client.get_paginator("search_quantum_tasks")` ->
  [SearchQuantumTasksPaginator](./paginators.md#searchquantumtaskspaginator)
