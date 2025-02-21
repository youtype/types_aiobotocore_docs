# Examples

> [Index](../README.md) > [SESV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#sesv2)
    type annotations stubs module [types-aiobotocore-sesv2](https://pypi.org/project/types-aiobotocore-sesv2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sesv2]` package installed.

Write your `SESV2` code as usual,
type checking and code completion should work out of the box.



```python
# SESV2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sesv2") as client:  # (1)
    result = await client.batch_get_metric_data()  # (2)
```

1. client: [SESV2Client](./client.md)
2. result: [:material-code-braces: BatchGetMetricDataResponseTypeDef](./type_defs.md#batchgetmetricdataresponsetypedef) 



```python
# ListMultiRegionEndpointsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sesv2") as client:  # (1)
    paginator = client.get_paginator("list_multi_region_endpoints")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SESV2Client](./client.md)
2. paginator: [ListMultiRegionEndpointsPaginator](./paginators.md#listmultiregionendpointspaginator)
3. item: [:material-code-braces: ListMultiRegionEndpointsResponseTypeDef](./type_defs.md#listmultiregionendpointsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[sesv2]`
or a standalone `types_aiobotocore_sesv2` package, you have to explicitly specify
`client: SESV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SESV2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sesv2.client import SESV2Client
from types_aiobotocore_sesv2.type_defs import BatchGetMetricDataResponseTypeDef
from types_aiobotocore_sesv2.type_defs import BatchGetMetricDataRequestTypeDef


session = get_session()

async with session.create_client("sesv2") as client:
    client: SESV2Client
    kwargs: BatchGetMetricDataRequestTypeDef = {...}
    result: BatchGetMetricDataResponseTypeDef = await client.batch_get_metric_data(**kwargs)
```



```python
# ListMultiRegionEndpointsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sesv2.client import SESV2Client
from types_aiobotocore_sesv2.paginator import ListMultiRegionEndpointsPaginator
from types_aiobotocore_sesv2.type_defs import ListMultiRegionEndpointsResponseTypeDef


session = get_session()

async with session.create_client("sesv2") as client:
    client: SESV2Client
    paginator: ListMultiRegionEndpointsPaginator = client.get_paginator("list_multi_region_endpoints")
    async for item in paginator.paginate(...):
        item: ListMultiRegionEndpointsResponseTypeDef
        print(item)
```


