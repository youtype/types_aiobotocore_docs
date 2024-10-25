# Paginators

> [Index](../README.md) > [TimestreamInfluxDB](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [TimestreamInfluxDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB)
    type annotations stubs module [types-aiobotocore-timestream-influxdb](https://pypi.org/project/types-aiobotocore-timestream-influxdb/).

## ListDbInstancesPaginator

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").get_paginator("list_db_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Paginator.ListDbInstances)

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
) -> AsyncIterator[ListDbInstancesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDbInstancesOutputTypeDef](./type_defs.md#listdbinstancesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDbInstancesInputListDbInstancesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDbInstancesInputListDbInstancesPaginateTypeDef](./type_defs.md#listdbinstancesinputlistdbinstancespaginatetypedef) 
## ListDbParameterGroupsPaginator

Type annotations and code completion for `#!python session.create_client("timestream-influxdb").get_paginator("list_db_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB.Paginator.ListDbParameterGroups)

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
) -> AsyncIterator[ListDbParameterGroupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDbParameterGroupsOutputTypeDef](./type_defs.md#listdbparametergroupsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDbParameterGroupsInputListDbParameterGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDbParameterGroupsInputListDbParameterGroupsPaginateTypeDef](./type_defs.md#listdbparametergroupsinputlistdbparametergroupspaginatetypedef) 
