# Examples

> [Index](../README.md) > [KinesisAnalytics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#kinesisanalytics)
    type annotations stubs module [types-aiobotocore-kinesisanalytics](https://pypi.org/project/types-aiobotocore-kinesisanalytics/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kinesisanalytics]` package installed.

Write your `KinesisAnalytics` code as usual,
type checking and code completion should work out of the box.



```python
# KinesisAnalyticsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesisanalytics") as client:  # (1)
    result = await client.create_application()  # (2)
```

1. client: [KinesisAnalyticsClient](./client.md)
2. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[kinesisanalytics]`
or a standalone `types_aiobotocore_kinesisanalytics` package, you have to explicitly specify
`client: KinesisAnalyticsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KinesisAnalyticsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesisanalytics.client import KinesisAnalyticsClient
from types_aiobotocore_kinesisanalytics.type_defs import CreateApplicationResponseTypeDef
from types_aiobotocore_kinesisanalytics.type_defs import CreateApplicationRequestTypeDef


session = get_session()

async with session.create_client("kinesisanalytics") as client:
    client: KinesisAnalyticsClient
    kwargs: CreateApplicationRequestTypeDef = {...}
    result: CreateApplicationResponseTypeDef = await client.create_application(**kwargs)
```




