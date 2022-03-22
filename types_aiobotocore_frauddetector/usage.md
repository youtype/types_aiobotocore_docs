<a id="examples-for-aiobotocore-frauddetector-module"></a>

# Examples for aiobotocore FraudDetector module

> [Index](../README.md) > [FraudDetector](./README.md) > Examples

- [Examples for aiobotocore FraudDetector module](#examples-for-aiobotocore-frauddetector-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[frauddetector]` package installed.

Write your `FraudDetector` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type FraudDetectorClient
# and provides type checking and code completion
async with session.create_client("frauddetector") as client:
    
    # result has type BatchCreateVariableResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_create_variable()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[frauddetector]` or a standalone
`types_aiobotocore_frauddetector` package, you have to explicitly specify
`client: FraudDetectorClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_frauddetector.client import FraudDetectorClient
from types_aiobotocore_frauddetector.type_defs import BatchCreateVariableResultTypeDef






session = get_session()

async with session.create_client("frauddetector") as client:
    client: FraudDetectorClient

    
    result: BatchCreateVariableResultTypeDef = client.batch_create_variable()
    

    

    
```
