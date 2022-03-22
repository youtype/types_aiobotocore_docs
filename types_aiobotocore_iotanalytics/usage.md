<a id="examples-for-aiobotocore-iotanalytics-module"></a>

# Examples for aiobotocore IoTAnalytics module

> [Index](../README.md) > [IoTAnalytics](./README.md) > Examples

- [Examples for aiobotocore IoTAnalytics module](#examples-for-aiobotocore-iotanalytics-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iotanalytics]` package installed.

Write your `IoTAnalytics` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTAnalyticsClient
# and provides type checking and code completion
async with session.create_client("iotanalytics") as client:
    
    # result has type BatchPutMessageResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_put_message()
    

    
    # paginator has type ListChannelsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_channels")
    async for item in paginator.paginate(...):
        # item has type ListChannelsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iotanalytics]` or a standalone
`types_aiobotocore_iotanalytics` package, you have to explicitly specify
`client: IoTAnalyticsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.client import IoTAnalyticsClient
from types_aiobotocore_iotanalytics.type_defs import BatchPutMessageResponseTypeDef
from types_aiobotocore_iotanalytics.paginator import ListChannelsPaginator

from types_aiobotocore_iotanalytics.literals import PaginatorName



session = get_session()

async with session.create_client("iotanalytics") as client:
    client: IoTAnalyticsClient

    
    result: BatchPutMessageResponseTypeDef = client.batch_put_message()
    

    
    paginator_name: PaginatorName = "list_channels"
    paginator: ListChannelsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)
    

    
```
