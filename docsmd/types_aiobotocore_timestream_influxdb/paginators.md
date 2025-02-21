# Paginators

> [Index](../README.md) > [TimestreamInfluxDB](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [TimestreamInfluxDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#timestreaminfluxdb)
    type annotations stubs module [types-aiobotocore-timestream-influxdb](https://pypi.org/project/types-aiobotocore-timestream-influxdb/).

## ListDbClustersPaginator

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").get_paginator("list_db_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb/paginator/ListDbClusters.html#TimestreamInfluxDB.Paginator.ListDbClusters)

```python
# ListDbClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_timestream_influxdb.paginator import ListDbClustersPaginator

session = get_session()
async with session.create_client("timestream-influxdb") as client:  # (1)
    paginator: ListDbClustersPaginator = client.get_paginator("list_db_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListDbClustersOutputTypeDef
        print(item)  # (3)
```

1. client: [TimestreamInfluxDBClient](./client.md)
2. paginator: [ListDbClustersPaginator](./paginators.md#listdbclusterspaginator)
3. item: [:material-code-braces: ListDbClustersOutputTypeDef](./type_defs.md#listdbclustersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDbClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDbClustersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDbClustersOutputTypeDef](./type_defs.md#listdbclustersoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDbClustersInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDbClustersInputPaginateTypeDef](./type_defs.md#listdbclustersinputpaginatetypedef) 
## ListDbInstancesForClusterPaginator

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").get_paginator("list_db_instances_for_cluster")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb/paginator/ListDbInstancesForCluster.html#TimestreamInfluxDB.Paginator.ListDbInstancesForCluster)

```python
# ListDbInstancesForClusterPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_timestream_influxdb.paginator import ListDbInstancesForClusterPaginator

session = get_session()
async with session.create_client("timestream-influxdb") as client:  # (1)
    paginator: ListDbInstancesForClusterPaginator = client.get_paginator("list_db_instances_for_cluster")  # (2)
    async for item in paginator.paginate(...):
        item: ListDbInstancesForClusterOutputTypeDef
        print(item)  # (3)
```

1. client: [TimestreamInfluxDBClient](./client.md)
2. paginator: [ListDbInstancesForClusterPaginator](./paginators.md#listdbinstancesforclusterpaginator)
3. item: [:material-code-braces: ListDbInstancesForClusterOutputTypeDef](./type_defs.md#listdbinstancesforclusteroutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDbInstancesForClusterPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    dbClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDbInstancesForClusterOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDbInstancesForClusterOutputTypeDef](./type_defs.md#listdbinstancesforclusteroutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDbInstancesForClusterInputPaginateTypeDef = {  # (1)
    "dbClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDbInstancesForClusterInputPaginateTypeDef](./type_defs.md#listdbinstancesforclusterinputpaginatetypedef) 
## ListDbInstancesPaginator

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").get_paginator("list_db_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb/paginator/ListDbInstances.html#TimestreamInfluxDB.Paginator.ListDbInstances)

```python
# ListDbInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_timestream_influxdb.paginator import ListDbInstancesPaginator

session = get_session()
async with session.create_client("timestream-influxdb") as client:  # (1)
    paginator: ListDbInstancesPaginator = client.get_paginator("list_db_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListDbInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [TimestreamInfluxDBClient](./client.md)
2. paginator: [ListDbInstancesPaginator](./paginators.md#listdbinstancespaginator)
3. item: [:material-code-braces: ListDbInstancesOutputTypeDef](./type_defs.md#listdbinstancesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDbInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDbInstancesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDbInstancesOutputTypeDef](./type_defs.md#listdbinstancesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDbInstancesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDbInstancesInputPaginateTypeDef](./type_defs.md#listdbinstancesinputpaginatetypedef) 
## ListDbParameterGroupsPaginator

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").get_paginator("list_db_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb/paginator/ListDbParameterGroups.html#TimestreamInfluxDB.Paginator.ListDbParameterGroups)

```python
# ListDbParameterGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_timestream_influxdb.paginator import ListDbParameterGroupsPaginator

session = get_session()
async with session.create_client("timestream-influxdb") as client:  # (1)
    paginator: ListDbParameterGroupsPaginator = client.get_paginator("list_db_parameter_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListDbParameterGroupsOutputTypeDef
        print(item)  # (3)
```

1. client: [TimestreamInfluxDBClient](./client.md)
2. paginator: [ListDbParameterGroupsPaginator](./paginators.md#listdbparametergroupspaginator)
3. item: [:material-code-braces: ListDbParameterGroupsOutputTypeDef](./type_defs.md#listdbparametergroupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDbParameterGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDbParameterGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDbParameterGroupsOutputTypeDef](./type_defs.md#listdbparametergroupsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDbParameterGroupsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDbParameterGroupsInputPaginateTypeDef](./type_defs.md#listdbparametergroupsinputpaginatetypedef) 
