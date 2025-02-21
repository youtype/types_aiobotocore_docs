# Examples

> [Index](../README.md) > [DataSync](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#datasync)
    type annotations stubs module [types-aiobotocore-datasync](https://pypi.org/project/types-aiobotocore-datasync/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[datasync]` package installed.

Write your `DataSync` code as usual,
type checking and code completion should work out of the box.



```python
# DataSyncClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("datasync") as client:  # (1)
    result = await client.add_storage_system()  # (2)
```

1. client: [DataSyncClient](./client.md)
2. result: [:material-code-braces: AddStorageSystemResponseTypeDef](./type_defs.md#addstoragesystemresponsetypedef) 



```python
# DescribeStorageSystemResourceMetricsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("datasync") as client:  # (1)
    paginator = client.get_paginator("describe_storage_system_resource_metrics")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DataSyncClient](./client.md)
2. paginator: [DescribeStorageSystemResourceMetricsPaginator](./paginators.md#describestoragesystemresourcemetricspaginator)
3. item: [:material-code-braces: DescribeStorageSystemResourceMetricsResponseTypeDef](./type_defs.md#describestoragesystemresourcemetricsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[datasync]`
or a standalone `types_aiobotocore_datasync` package, you have to explicitly specify
`client: DataSyncClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DataSyncClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_datasync.client import DataSyncClient
from types_aiobotocore_datasync.type_defs import AddStorageSystemResponseTypeDef
from types_aiobotocore_datasync.type_defs import AddStorageSystemRequestTypeDef


session = get_session()

async with session.create_client("datasync") as client:
    client: DataSyncClient
    kwargs: AddStorageSystemRequestTypeDef = {...}
    result: AddStorageSystemResponseTypeDef = await client.add_storage_system(**kwargs)
```



```python
# DescribeStorageSystemResourceMetricsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_datasync.client import DataSyncClient
from types_aiobotocore_datasync.paginator import DescribeStorageSystemResourceMetricsPaginator
from types_aiobotocore_datasync.type_defs import DescribeStorageSystemResourceMetricsResponseTypeDef


session = get_session()

async with session.create_client("datasync") as client:
    client: DataSyncClient
    paginator: DescribeStorageSystemResourceMetricsPaginator = client.get_paginator("describe_storage_system_resource_metrics")
    async for item in paginator.paginate(...):
        item: DescribeStorageSystemResourceMetricsResponseTypeDef
        print(item)
```


