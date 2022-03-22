<a id="examples-for-aiobotocore-iotjobsdataplane-module"></a>

# Examples for aiobotocore IoTJobsDataPlane module

> [Index](../README.md) > [IoTJobsDataPlane](./README.md) > Examples

- [Examples for aiobotocore IoTJobsDataPlane module](#examples-for-aiobotocore-iotjobsdataplane-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iot-jobs-data]` package installed.

Write your `IoTJobsDataPlane` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTJobsDataPlaneClient
# and provides type checking and code completion
async with session.create_client("iot-jobs-data") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iot-jobs-data]` or a standalone
`types_aiobotocore_iot_jobs_data` package, you have to explicitly specify
`client: IoTJobsDataPlaneClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot_jobs_data.client import IoTJobsDataPlaneClient
from types_aiobotocore_iot_jobs_data.type_defs import bool






session = get_session()

async with session.create_client("iot-jobs-data") as client:
    client: IoTJobsDataPlaneClient

    
    result: bool = client.can_paginate()
    

    

    
```
