# IoTJobsDataPlaneClient

> [Index](../README.md) > [IoTJobsDataPlane](./README.md) > IoTJobsDataPlaneClient

!!! note ""

    Auto-generated documentation for [IoTJobsDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
    type annotations stubs module [types-aiobotocore-iot-jobs-data](https://pypi.org/project/types-aiobotocore-iot-jobs-data/).

## IoTJobsDataPlaneClient

Type annotations and code completion for `#!python session.create_client("iot-jobs-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_iot_jobs_data.client import IoTJobsDataPlaneClient

session = get_session()
async with session.create_client("iot-jobs-data") as client:
    client: IoTJobsDataPlaneClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iot-jobs-data").exceptions` structure.

```python title="Usage example"
async with session.create_client("iot-jobs-data") as client:
    try:
        do_something(client)
    except (
            client.CertificateValidationException,
        client.ClientError,
        client.InvalidRequestException,
        client.InvalidStateTransitionException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.TerminalStateException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_iot_jobs_data.client import Exceptions

def handle_error(exc: Exceptions.CertificateValidationException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("iot-jobs-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### describe\_job\_execution

Gets details of a job execution.

Type annotations and code completion for `#!python session.create_client("iot-jobs-data").describe_job_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.describe_job_execution)

```python title="Method definition"
await def describe_job_execution(
    self,
    *,
    jobId: str,
    thingName: str,
    includeJobDocument: bool = ...,
    executionNumber: int = ...,
) -> DescribeJobExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeJobExecutionResponseTypeDef](./type_defs.md#describejobexecutionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeJobExecutionRequestRequestTypeDef = {  # (1)
    "jobId": ...,
    "thingName": ...,
}

parent.describe_job_execution(**kwargs)
```

1. See [:material-code-braces: DescribeJobExecutionRequestRequestTypeDef](./type_defs.md#describejobexecutionrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("iot-jobs-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_pending\_job\_executions

Gets the list of all jobs for a thing that are not in a terminal status.

Type annotations and code completion for `#!python session.create_client("iot-jobs-data").get_pending_job_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.get_pending_job_executions)

```python title="Method definition"
await def get_pending_job_executions(
    self,
    *,
    thingName: str,
) -> GetPendingJobExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPendingJobExecutionsResponseTypeDef](./type_defs.md#getpendingjobexecutionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetPendingJobExecutionsRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.get_pending_job_executions(**kwargs)
```

1. See [:material-code-braces: GetPendingJobExecutionsRequestRequestTypeDef](./type_defs.md#getpendingjobexecutionsrequestrequesttypedef) 

### start\_next\_pending\_job\_execution

Gets and starts the next pending (status IN_PROGRESS or QUEUED) job execution
for a thing.

Type annotations and code completion for `#!python session.create_client("iot-jobs-data").start_next_pending_job_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.start_next_pending_job_execution)

```python title="Method definition"
await def start_next_pending_job_execution(
    self,
    *,
    thingName: str,
    statusDetails: Mapping[str, str] = ...,
    stepTimeoutInMinutes: int = ...,
) -> StartNextPendingJobExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartNextPendingJobExecutionResponseTypeDef](./type_defs.md#startnextpendingjobexecutionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: StartNextPendingJobExecutionRequestRequestTypeDef = {  # (1)
    "thingName": ...,
}

parent.start_next_pending_job_execution(**kwargs)
```

1. See [:material-code-braces: StartNextPendingJobExecutionRequestRequestTypeDef](./type_defs.md#startnextpendingjobexecutionrequestrequesttypedef) 

### update\_job\_execution

Updates the status of a job execution.

Type annotations and code completion for `#!python session.create_client("iot-jobs-data").update_job_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.update_job_execution)

```python title="Method definition"
await def update_job_execution(
    self,
    *,
    jobId: str,
    thingName: str,
    status: JobExecutionStatusType,  # (1)
    statusDetails: Mapping[str, str] = ...,
    stepTimeoutInMinutes: int = ...,
    expectedVersion: int = ...,
    includeJobExecutionState: bool = ...,
    includeJobDocument: bool = ...,
    executionNumber: int = ...,
) -> UpdateJobExecutionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
2. See [:material-code-braces: UpdateJobExecutionResponseTypeDef](./type_defs.md#updatejobexecutionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: UpdateJobExecutionRequestRequestTypeDef = {  # (1)
    "jobId": ...,
    "thingName": ...,
    "status": ...,
}

parent.update_job_execution(**kwargs)
```

1. See [:material-code-braces: UpdateJobExecutionRequestRequestTypeDef](./type_defs.md#updatejobexecutionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iot-jobs-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> IoTJobsDataPlaneClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iot-jobs-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





