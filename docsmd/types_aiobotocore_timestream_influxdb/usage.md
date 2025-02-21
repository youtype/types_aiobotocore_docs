# Examples

> [Index](../README.md) > [TimestreamInfluxDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TimestreamInfluxDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#timestreaminfluxdb)
    type annotations stubs module [types-aiobotocore-timestream-influxdb](https://pypi.org/project/types-aiobotocore-timestream-influxdb/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[timestream-influxdb]` package installed.

Write your `TimestreamInfluxDB` code as usual,
type checking and code completion should work out of the box.



```python
# TimestreamInfluxDBClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("timestream-influxdb") as client:  # (1)
    result = await client.create_db_cluster()  # (2)
```

1. client: [TimestreamInfluxDBClient](./client.md)
2. result: [:material-code-braces: CreateDbClusterOutputTypeDef](./type_defs.md#createdbclusteroutputtypedef) 



```python
# ListDbClustersPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("timestream-influxdb") as client:  # (1)
    paginator = client.get_paginator("list_db_clusters")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TimestreamInfluxDBClient](./client.md)
2. paginator: [ListDbClustersPaginator](./paginators.md#listdbclusterspaginator)
3. item: [:material-code-braces: ListDbClustersOutputTypeDef](./type_defs.md#listdbclustersoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[timestream-influxdb]`
or a standalone `types_aiobotocore_timestream_influxdb` package, you have to explicitly specify
`client: TimestreamInfluxDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# TimestreamInfluxDBClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_timestream_influxdb.client import TimestreamInfluxDBClient
from types_aiobotocore_timestream_influxdb.type_defs import CreateDbClusterOutputTypeDef
from types_aiobotocore_timestream_influxdb.type_defs import CreateDbClusterInputTypeDef


session = get_session()

async with session.create_client("timestream-influxdb") as client:
    client: TimestreamInfluxDBClient
    kwargs: CreateDbClusterInputTypeDef = {...}
    result: CreateDbClusterOutputTypeDef = await client.create_db_cluster(**kwargs)
```



```python
# ListDbClustersPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_timestream_influxdb.client import TimestreamInfluxDBClient
from types_aiobotocore_timestream_influxdb.paginator import ListDbClustersPaginator
from types_aiobotocore_timestream_influxdb.type_defs import ListDbClustersOutputTypeDef


session = get_session()

async with session.create_client("timestream-influxdb") as client:
    client: TimestreamInfluxDBClient
    paginator: ListDbClustersPaginator = client.get_paginator("list_db_clusters")
    async for item in paginator.paginate(...):
        item: ListDbClustersOutputTypeDef
        print(item)
```


