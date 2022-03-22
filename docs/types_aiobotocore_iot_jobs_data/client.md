<a id="iotjobsdataplaneclient-for-aiobotocore-iotjobsdataplane-module"></a>

# IoTJobsDataPlaneClient for aiobotocore IoTJobsDataPlane module

> [Index](../README.md) > [IoTJobsDataPlane](./README.md) >
> IoTJobsDataPlaneClient

Auto-generated documentation for
[IoTJobsDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
type annotations stubs module
[types-aiobotocore-iot-jobs-data](https://pypi.org/project/types-aiobotocore-iot-jobs-data/).

- [IoTJobsDataPlaneClient for aiobotocore IoTJobsDataPlane module](#iotjobsdataplaneclient-for-aiobotocore-iotjobsdataplane-module)
  - [IoTJobsDataPlaneClient](#iotjobsdataplaneclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [describe_job_execution](#describe_job_execution)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_pending_job_executions](#get_pending_job_executions)
    - [start_next_pending_job_execution](#start_next_pending_job_execution)
    - [update_job_execution](#update_job_execution)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="iotjobsdataplaneclient"></a>

## IoTJobsDataPlaneClient

Type annotations for `session.create_client("iot-jobs-data")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_iot_jobs_data.client import IoTJobsDataPlaneClient

session = get_session()
async with session.create_client("iot-jobs-data") as client:
    client: IoTJobsDataPlaneClient
```

Boto3 documentation:
[IoTJobsDataPlane.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_iot_jobs_data.client import Exceptions

def handle_error(exc: Exceptions.CertificateValidationException) -> None:
    ...
```

Exceptions:

- `Exceptions.CertificateValidationException`
- `Exceptions.ClientError`
- `Exceptions.InvalidRequestException`
- `Exceptions.InvalidStateTransitionException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.TerminalStateException`
- `Exceptions.ThrottlingException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

IoTJobsDataPlaneClient exceptions.

Type annotations for `session.create_client("iot-jobs-data").exceptions`
method.

Boto3 documentation:
[IoTJobsDataPlane.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("iot-jobs-data").can_paginate`
method.

Boto3 documentation:
[IoTJobsDataPlane.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="describe\_job\_execution"></a>

### describe_job_execution

Gets details of a job execution.

Type annotations for
`session.create_client("iot-jobs-data").describe_job_execution` method.

Boto3 documentation:
[IoTJobsDataPlane.Client.describe_job_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.describe_job_execution)

Asynchronous method. Use `await describe_job_execution(...)` for a synchronous
call.

Arguments mapping described in
[DescribeJobExecutionRequestRequestTypeDef](./type_defs.md#describejobexecutionrequestrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `thingName`: `str` *(required)*
- `includeJobDocument`: `bool`
- `executionNumber`: `int`

Returns a `Coroutine` for
[DescribeJobExecutionResponseTypeDef](./type_defs.md#describejobexecutionresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("iot-jobs-data").generate_presigned_url` method.

Boto3 documentation:
[IoTJobsDataPlane.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_pending\_job\_executions"></a>

### get_pending_job_executions

Gets the list of all jobs for a thing that are not in a terminal status.

Type annotations for
`session.create_client("iot-jobs-data").get_pending_job_executions` method.

Boto3 documentation:
[IoTJobsDataPlane.Client.get_pending_job_executions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.get_pending_job_executions)

Asynchronous method. Use `await get_pending_job_executions(...)` for a
synchronous call.

Arguments mapping described in
[GetPendingJobExecutionsRequestRequestTypeDef](./type_defs.md#getpendingjobexecutionsrequestrequesttypedef).

Keyword-only arguments:

- `thingName`: `str` *(required)*

Returns a `Coroutine` for
[GetPendingJobExecutionsResponseTypeDef](./type_defs.md#getpendingjobexecutionsresponsetypedef).

<a id="start\_next\_pending\_job\_execution"></a>

### start_next_pending_job_execution

Gets and starts the next pending (status IN_PROGRESS or QUEUED) job execution
for a thing.

Type annotations for
`session.create_client("iot-jobs-data").start_next_pending_job_execution`
method.

Boto3 documentation:
[IoTJobsDataPlane.Client.start_next_pending_job_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.start_next_pending_job_execution)

Asynchronous method. Use `await start_next_pending_job_execution(...)` for a
synchronous call.

Arguments mapping described in
[StartNextPendingJobExecutionRequestRequestTypeDef](./type_defs.md#startnextpendingjobexecutionrequestrequesttypedef).

Keyword-only arguments:

- `thingName`: `str` *(required)*
- `statusDetails`: `Mapping`\[`str`, `str`\]
- `stepTimeoutInMinutes`: `int`

Returns a `Coroutine` for
[StartNextPendingJobExecutionResponseTypeDef](./type_defs.md#startnextpendingjobexecutionresponsetypedef).

<a id="update\_job\_execution"></a>

### update_job_execution

Updates the status of a job execution.

Type annotations for
`session.create_client("iot-jobs-data").update_job_execution` method.

Boto3 documentation:
[IoTJobsDataPlane.Client.update_job_execution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.update_job_execution)

Asynchronous method. Use `await update_job_execution(...)` for a synchronous
call.

Arguments mapping described in
[UpdateJobExecutionRequestRequestTypeDef](./type_defs.md#updatejobexecutionrequestrequesttypedef).

Keyword-only arguments:

- `jobId`: `str` *(required)*
- `thingName`: `str` *(required)*
- `status`: [JobExecutionStatusType](./literals.md#jobexecutionstatustype)
  *(required)*
- `statusDetails`: `Mapping`\[`str`, `str`\]
- `stepTimeoutInMinutes`: `int`
- `expectedVersion`: `int`
- `includeJobExecutionState`: `bool`
- `includeJobDocument`: `bool`
- `executionNumber`: `int`

Returns a `Coroutine` for
[UpdateJobExecutionResponseTypeDef](./type_defs.md#updatejobexecutionresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("iot-jobs-data").__aenter__`
method.

Boto3 documentation:
[IoTJobsDataPlane.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [IoTJobsDataPlaneClient](#iotjobsdataplaneclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("iot-jobs-data").__aexit__` method.

Boto3 documentation:
[IoTJobsDataPlane.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
