# Examples

> [Index](../README.md) > [FraudDetector](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FraudDetector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#frauddetector)
    type annotations stubs module [types-aiobotocore-frauddetector](https://pypi.org/project/types-aiobotocore-frauddetector/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[frauddetector]` package installed.

Write your `FraudDetector` code as usual,
type checking and code completion should work out of the box.



```python
# FraudDetectorClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("frauddetector") as client:  # (1)
    result = await client.batch_create_variable()  # (2)
```

1. client: [FraudDetectorClient](./client.md)
2. result: [:material-code-braces: BatchCreateVariableResultTypeDef](./type_defs.md#batchcreatevariableresulttypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[frauddetector]`
or a standalone `types_aiobotocore_frauddetector` package, you have to explicitly specify
`client: FraudDetectorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# FraudDetectorClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_frauddetector.client import FraudDetectorClient
from types_aiobotocore_frauddetector.type_defs import BatchCreateVariableResultTypeDef
from types_aiobotocore_frauddetector.type_defs import BatchCreateVariableRequestTypeDef


session = get_session()

async with session.create_client("frauddetector") as client:
    client: FraudDetectorClient
    kwargs: BatchCreateVariableRequestTypeDef = {...}
    result: BatchCreateVariableResultTypeDef = await client.batch_create_variable(**kwargs)
```




