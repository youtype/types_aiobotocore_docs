# Examples

> [Index](../README.md) > [IoTJobsDataPlane](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTJobsDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#iotjobsdataplane)
    type annotations stubs module [types-aiobotocore-iot-jobs-data](https://pypi.org/project/types-aiobotocore-iot-jobs-data/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iot-jobs-data]` package installed.

Write your `IoTJobsDataPlane` code as usual,
type checking and code completion should work out of the box.



```python
# IoTJobsDataPlaneClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iot-jobs-data") as client:  # (1)
    result = await client.describe_job_execution()  # (2)
```

1. client: [IoTJobsDataPlaneClient](./client.md)
2. result: [:material-code-braces: DescribeJobExecutionResponseTypeDef](./type_defs.md#describejobexecutionresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[iot-jobs-data]`
or a standalone `types_aiobotocore_iot_jobs_data` package, you have to explicitly specify
`client: IoTJobsDataPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTJobsDataPlaneClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iot_jobs_data.client import IoTJobsDataPlaneClient
from types_aiobotocore_iot_jobs_data.type_defs import DescribeJobExecutionResponseTypeDef
from types_aiobotocore_iot_jobs_data.type_defs import DescribeJobExecutionRequestTypeDef


session = get_session()

async with session.create_client("iot-jobs-data") as client:
    client: IoTJobsDataPlaneClient
    kwargs: DescribeJobExecutionRequestTypeDef = {...}
    result: DescribeJobExecutionResponseTypeDef = await client.describe_job_execution(**kwargs)
```




