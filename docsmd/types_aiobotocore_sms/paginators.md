# Paginators

> [Index](../README.md) > [SMS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#sms)
    type annotations stubs module [types-aiobotocore-sms](https://pypi.org/project/types-aiobotocore-sms/).

## GetConnectorsPaginator

Type annotations and code completion for `#!python session.create_client("sms").get_paginator("get_connectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms/paginator/GetConnectors.html#SMS.Paginator.GetConnectors)

```python
# GetConnectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetConnectorsPaginator

session = get_session()
async with session.create_client("sms") as client:  # (1)
    paginator: GetConnectorsPaginator = client.get_paginator("get_connectors")  # (2)
    async for item in paginator.paginate(...):
        item: GetConnectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [SMSClient](./client.md)
2. paginator: [GetConnectorsPaginator](./paginators.md#getconnectorspaginator)
3. item: [:material-code-braces: GetConnectorsResponseTypeDef](./type_defs.md#getconnectorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetConnectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetConnectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetConnectorsResponseTypeDef](./type_defs.md#getconnectorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetConnectorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetConnectorsRequestPaginateTypeDef](./type_defs.md#getconnectorsrequestpaginatetypedef) 
## GetReplicationJobsPaginator

Type annotations and code completion for `#!python session.create_client("sms").get_paginator("get_replication_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms/paginator/GetReplicationJobs.html#SMS.Paginator.GetReplicationJobs)

```python
# GetReplicationJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetReplicationJobsPaginator

session = get_session()
async with session.create_client("sms") as client:  # (1)
    paginator: GetReplicationJobsPaginator = client.get_paginator("get_replication_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: GetReplicationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [SMSClient](./client.md)
2. paginator: [GetReplicationJobsPaginator](./paginators.md#getreplicationjobspaginator)
3. item: [:material-code-braces: GetReplicationJobsResponseTypeDef](./type_defs.md#getreplicationjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetReplicationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    replicationJobId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetReplicationJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetReplicationJobsResponseTypeDef](./type_defs.md#getreplicationjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetReplicationJobsRequestPaginateTypeDef = {  # (1)
    "replicationJobId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetReplicationJobsRequestPaginateTypeDef](./type_defs.md#getreplicationjobsrequestpaginatetypedef) 
## GetReplicationRunsPaginator

Type annotations and code completion for `#!python session.create_client("sms").get_paginator("get_replication_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms/paginator/GetReplicationRuns.html#SMS.Paginator.GetReplicationRuns)

```python
# GetReplicationRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetReplicationRunsPaginator

session = get_session()
async with session.create_client("sms") as client:  # (1)
    paginator: GetReplicationRunsPaginator = client.get_paginator("get_replication_runs")  # (2)
    async for item in paginator.paginate(...):
        item: GetReplicationRunsResponseTypeDef
        print(item)  # (3)
```

1. client: [SMSClient](./client.md)
2. paginator: [GetReplicationRunsPaginator](./paginators.md#getreplicationrunspaginator)
3. item: [:material-code-braces: GetReplicationRunsResponseTypeDef](./type_defs.md#getreplicationrunsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetReplicationRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    replicationJobId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetReplicationRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetReplicationRunsResponseTypeDef](./type_defs.md#getreplicationrunsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetReplicationRunsRequestPaginateTypeDef = {  # (1)
    "replicationJobId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetReplicationRunsRequestPaginateTypeDef](./type_defs.md#getreplicationrunsrequestpaginatetypedef) 
## GetServersPaginator

Type annotations and code completion for `#!python session.create_client("sms").get_paginator("get_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms/paginator/GetServers.html#SMS.Paginator.GetServers)

```python
# GetServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetServersPaginator

session = get_session()
async with session.create_client("sms") as client:  # (1)
    paginator: GetServersPaginator = client.get_paginator("get_servers")  # (2)
    async for item in paginator.paginate(...):
        item: GetServersResponseTypeDef
        print(item)  # (3)
```

1. client: [SMSClient](./client.md)
2. paginator: [GetServersPaginator](./paginators.md#getserverspaginator)
3. item: [:material-code-braces: GetServersResponseTypeDef](./type_defs.md#getserversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetServersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: VmServerAddressTypeDef](./type_defs.md#vmserveraddresstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetServersResponseTypeDef](./type_defs.md#getserversresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetServersRequestPaginateTypeDef = {  # (1)
    "vmServerAddressList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetServersRequestPaginateTypeDef](./type_defs.md#getserversrequestpaginatetypedef) 
## ListAppsPaginator

Type annotations and code completion for `#!python session.create_client("sms").get_paginator("list_apps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms/paginator/ListApps.html#SMS.Paginator.ListApps)

```python
# ListAppsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import ListAppsPaginator

session = get_session()
async with session.create_client("sms") as client:  # (1)
    paginator: ListAppsPaginator = client.get_paginator("list_apps")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppsResponseTypeDef
        print(item)  # (3)
```

1. client: [SMSClient](./client.md)
2. paginator: [ListAppsPaginator](./paginators.md#listappspaginator)
3. item: [:material-code-braces: ListAppsResponseTypeDef](./type_defs.md#listappsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAppsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAppsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppsResponseTypeDef](./type_defs.md#listappsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAppsRequestPaginateTypeDef = {  # (1)
    "appIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppsRequestPaginateTypeDef](./type_defs.md#listappsrequestpaginatetypedef) 
