# Paginators

> [Index](../README.md) > [OpsWorksCM](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#opsworkscm)
    type annotations stubs module [types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).

## DescribeBackupsPaginator

Type annotations and code completion for `#!python session.create_client("opsworkscm").get_paginator("describe_backups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/paginator/DescribeBackups.html#OpsWorksCM.Paginator.DescribeBackups)

```python
# DescribeBackupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.paginator import DescribeBackupsPaginator

session = get_session()
async with session.create_client("opsworkscm") as client:  # (1)
    paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBackupsResponseTypeDef
        print(item)  # (3)
```

1. client: [OpsWorksCMClient](./client.md)
2. paginator: [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
3. item: [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeBackupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BackupId: str = ...,
    ServerName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeBackupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBackupsRequestPaginateTypeDef = {  # (1)
    "BackupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBackupsRequestPaginateTypeDef](./type_defs.md#describebackupsrequestpaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("opsworkscm").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/paginator/DescribeEvents.html#OpsWorksCM.Paginator.DescribeEvents)

```python
# DescribeEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("opsworkscm") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [OpsWorksCMClient](./client.md)
2. paginator: [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
3. item: [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServerName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeEventsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventsRequestPaginateTypeDef = {  # (1)
    "ServerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsRequestPaginateTypeDef](./type_defs.md#describeeventsrequestpaginatetypedef) 
## DescribeServersPaginator

Type annotations and code completion for `#!python session.create_client("opsworkscm").get_paginator("describe_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/paginator/DescribeServers.html#OpsWorksCM.Paginator.DescribeServers)

```python
# DescribeServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.paginator import DescribeServersPaginator

session = get_session()
async with session.create_client("opsworkscm") as client:  # (1)
    paginator: DescribeServersPaginator = client.get_paginator("describe_servers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeServersResponseTypeDef
        print(item)  # (3)
```

1. client: [OpsWorksCMClient](./client.md)
2. paginator: [DescribeServersPaginator](./paginators.md#describeserverspaginator)
3. item: [:material-code-braces: DescribeServersResponseTypeDef](./type_defs.md#describeserversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServerName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeServersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeServersResponseTypeDef](./type_defs.md#describeserversresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeServersRequestPaginateTypeDef = {  # (1)
    "ServerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeServersRequestPaginateTypeDef](./type_defs.md#describeserversrequestpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("opsworkscm").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/paginator/ListTagsForResource.html#OpsWorksCM.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("opsworkscm") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [OpsWorksCMClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef) 
