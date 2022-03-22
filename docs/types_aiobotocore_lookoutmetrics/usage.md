<a id="examples-for-aiobotocore-lookoutmetrics-module"></a>

# Examples for aiobotocore LookoutMetrics module

> [Index](../README.md) > [LookoutMetrics](./README.md) > Examples

- [Examples for aiobotocore LookoutMetrics module](#examples-for-aiobotocore-lookoutmetrics-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[lookoutmetrics]` package installed.

Write your `LookoutMetrics` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type LookoutMetricsClient
# and provides type checking and code completion
async with session.create_client("lookoutmetrics") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.activate_anomaly_detector()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[lookoutmetrics]` or a standalone
`types_aiobotocore_lookoutmetrics` package, you have to explicitly specify
`client: LookoutMetricsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_lookoutmetrics.client import LookoutMetricsClient
from types_aiobotocore_lookoutmetrics.type_defs import Dict[str, Any]






session = get_session()

async with session.create_client("lookoutmetrics") as client:
    client: LookoutMetricsClient

    
    result: Dict[str, Any] = client.activate_anomaly_detector()
    

    

    
```
