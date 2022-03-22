<a id="examples-for-aiobotocore-kinesisanalytics-module"></a>

# Examples for aiobotocore KinesisAnalytics module

> [Index](../README.md) > [KinesisAnalytics](./README.md) > Examples

- [Examples for aiobotocore KinesisAnalytics module](#examples-for-aiobotocore-kinesisanalytics-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[kinesisanalytics]` package installed.

Write your `KinesisAnalytics` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type KinesisAnalyticsClient
# and provides type checking and code completion
async with session.create_client("kinesisanalytics") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_application_cloud_watch_logging_option()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[kinesisanalytics]` or a standalone
`types_aiobotocore_kinesisanalytics` package, you have to explicitly specify
`client: KinesisAnalyticsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesisanalytics.client import KinesisAnalyticsClient
from types_aiobotocore_kinesisanalytics.type_defs import Dict[str, Any]






session = get_session()

async with session.create_client("kinesisanalytics") as client:
    client: KinesisAnalyticsClient

    
    result: Dict[str, Any] = client.add_application_cloud_watch_logging_option()
    

    

    
```
