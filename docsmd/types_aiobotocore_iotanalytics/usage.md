# Examples

> [Index](../README.md) > [IoTAnalytics](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#iotanalytics)
    type annotations stubs module [types-aiobotocore-iotanalytics](https://pypi.org/project/types-aiobotocore-iotanalytics/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iotanalytics]` package installed.

Write your `IoTAnalytics` code as usual,
type checking and code completion should work out of the box.



```python
# IoTAnalyticsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotanalytics") as client:  # (1)
    result = await client.batch_put_message()  # (2)
```

1. client: [IoTAnalyticsClient](./client.md)
2. result: [:material-code-braces: BatchPutMessageResponseTypeDef](./type_defs.md#batchputmessageresponsetypedef) 



```python
# ListChannelsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotanalytics") as client:  # (1)
    paginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTAnalyticsClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[iotanalytics]`
or a standalone `types_aiobotocore_iotanalytics` package, you have to explicitly specify
`client: IoTAnalyticsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTAnalyticsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.client import IoTAnalyticsClient
from types_aiobotocore_iotanalytics.type_defs import BatchPutMessageResponseTypeDef
from types_aiobotocore_iotanalytics.type_defs import BatchPutMessageRequestTypeDef


session = get_session()

async with session.create_client("iotanalytics") as client:
    client: IoTAnalyticsClient
    kwargs: BatchPutMessageRequestTypeDef = {...}
    result: BatchPutMessageResponseTypeDef = await client.batch_put_message(**kwargs)
```



```python
# ListChannelsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.client import IoTAnalyticsClient
from types_aiobotocore_iotanalytics.paginator import ListChannelsPaginator
from types_aiobotocore_iotanalytics.type_defs import ListChannelsResponseTypeDef


session = get_session()

async with session.create_client("iotanalytics") as client:
    client: IoTAnalyticsClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)
```


