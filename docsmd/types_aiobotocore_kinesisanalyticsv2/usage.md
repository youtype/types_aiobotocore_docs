# Examples

> [Index](../README.md) > [KinesisAnalyticsV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KinesisAnalyticsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#kinesisanalyticsv2)
    type annotations stubs module [types-aiobotocore-kinesisanalyticsv2](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kinesisanalyticsv2]` package installed.

Write your `KinesisAnalyticsV2` code as usual,
type checking and code completion should work out of the box.



```python
# KinesisAnalyticsV2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesisanalyticsv2") as client:  # (1)
    result = await client.add_application_cloud_watch_logging_option()  # (2)
```

1. client: [KinesisAnalyticsV2Client](./client.md)
2. result: [:material-code-braces: AddApplicationCloudWatchLoggingOptionResponseTypeDef](./type_defs.md#addapplicationcloudwatchloggingoptionresponsetypedef) 



```python
# ListApplicationOperationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kinesisanalyticsv2") as client:  # (1)
    paginator = client.get_paginator("list_application_operations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [KinesisAnalyticsV2Client](./client.md)
2. paginator: [ListApplicationOperationsPaginator](./paginators.md#listapplicationoperationspaginator)
3. item: [:material-code-braces: ListApplicationOperationsResponseTypeDef](./type_defs.md#listapplicationoperationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[kinesisanalyticsv2]`
or a standalone `types_aiobotocore_kinesisanalyticsv2` package, you have to explicitly specify
`client: KinesisAnalyticsV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KinesisAnalyticsV2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesisanalyticsv2.client import KinesisAnalyticsV2Client
from types_aiobotocore_kinesisanalyticsv2.type_defs import AddApplicationCloudWatchLoggingOptionResponseTypeDef
from types_aiobotocore_kinesisanalyticsv2.type_defs import AddApplicationCloudWatchLoggingOptionRequestTypeDef


session = get_session()

async with session.create_client("kinesisanalyticsv2") as client:
    client: KinesisAnalyticsV2Client
    kwargs: AddApplicationCloudWatchLoggingOptionRequestTypeDef = {...}
    result: AddApplicationCloudWatchLoggingOptionResponseTypeDef = await client.add_application_cloud_watch_logging_option(**kwargs)
```



```python
# ListApplicationOperationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kinesisanalyticsv2.client import KinesisAnalyticsV2Client
from types_aiobotocore_kinesisanalyticsv2.paginator import ListApplicationOperationsPaginator
from types_aiobotocore_kinesisanalyticsv2.type_defs import ListApplicationOperationsResponseTypeDef


session = get_session()

async with session.create_client("kinesisanalyticsv2") as client:
    client: KinesisAnalyticsV2Client
    paginator: ListApplicationOperationsPaginator = client.get_paginator("list_application_operations")
    async for item in paginator.paginate(...):
        item: ListApplicationOperationsResponseTypeDef
        print(item)
```


