# Examples

> [Index](../README.md) > [LookoutMetrics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LookoutMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#lookoutmetrics)
    type annotations stubs module [types-aiobotocore-lookoutmetrics](https://pypi.org/project/types-aiobotocore-lookoutmetrics/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[lookoutmetrics]` package installed.

Write your `LookoutMetrics` code as usual,
type checking and code completion should work out of the box.



```python
# LookoutMetricsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lookoutmetrics") as client:  # (1)
    result = await client.create_alert()  # (2)
```

1. client: [LookoutMetricsClient](./client.md)
2. result: [:material-code-braces: CreateAlertResponseTypeDef](./type_defs.md#createalertresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[lookoutmetrics]`
or a standalone `types_aiobotocore_lookoutmetrics` package, you have to explicitly specify
`client: LookoutMetricsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LookoutMetricsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lookoutmetrics.client import LookoutMetricsClient
from types_aiobotocore_lookoutmetrics.type_defs import CreateAlertResponseTypeDef
from types_aiobotocore_lookoutmetrics.type_defs import CreateAlertRequestTypeDef


session = get_session()

async with session.create_client("lookoutmetrics") as client:
    client: LookoutMetricsClient
    kwargs: CreateAlertRequestTypeDef = {...}
    result: CreateAlertResponseTypeDef = await client.create_alert(**kwargs)
```




