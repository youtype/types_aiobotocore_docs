# Paginators

> [Index](../README.md) > [SMS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
    type annotations stubs module [types-aiobotocore-sms](https://pypi.org/project/types-aiobotocore-sms/).

## GetConnectorsPaginator

Type annotations and code completion for `#!python session.create_client("sms").get_paginator("get_connectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetConnectorsPaginator

session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
    paginator: GetConnectorsPaginator = client.get_paginator("get_connectors")
```


### paginate

Type annotations and code completion for `#!python GetConnectorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetConnectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetConnectorsResponseTypeDef](./type_defs.md#getconnectorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetConnectorsRequestGetConnectorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetConnectorsRequestGetConnectorsPaginateTypeDef](./type_defs.md#getconnectorsrequestgetconnectorspaginatetypedef) 
## GetReplicationJobsPaginator

Type annotations and code completion for `#!python session.create_client("sms").get_paginator("get_replication_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetReplicationJobsPaginator

session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
    paginator: GetReplicationJobsPaginator = client.get_paginator("get_replication_jobs")
```


### paginate

Type annotations and code completion for `#!python GetReplicationJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    replicationJobId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetReplicationJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetReplicationJobsResponseTypeDef](./type_defs.md#getreplicationjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef = {  # (1)
    "replicationJobId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef](./type_defs.md#getreplicationjobsrequestgetreplicationjobspaginatetypedef) 
## GetReplicationRunsPaginator

Type annotations and code completion for `#!python session.create_client("sms").get_paginator("get_replication_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetReplicationRunsPaginator

session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
    paginator: GetReplicationRunsPaginator = client.get_paginator("get_replication_runs")
```


### paginate

Type annotations and code completion for `#!python GetReplicationRunsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    replicationJobId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetReplicationRunsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetReplicationRunsResponseTypeDef](./type_defs.md#getreplicationrunsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef = {  # (1)
    "replicationJobId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef](./type_defs.md#getreplicationrunsrequestgetreplicationrunspaginatetypedef) 
## GetServersPaginator

Type annotations and code completion for `#!python session.create_client("sms").get_paginator("get_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetServersPaginator

session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
    paginator: GetServersPaginator = client.get_paginator("get_servers")
```


### paginate

Type annotations and code completion for `#!python GetServersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    vmServerAddressList: Sequence[VmServerAddressTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetServersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: VmServerAddressTypeDef](./type_defs.md#vmserveraddresstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetServersResponseTypeDef](./type_defs.md#getserversresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetServersRequestGetServersPaginateTypeDef = {  # (1)
    "vmServerAddressList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetServersRequestGetServersPaginateTypeDef](./type_defs.md#getserversrequestgetserverspaginatetypedef) 
## ListAppsPaginator

Type annotations and code completion for `#!python session.create_client("sms").get_paginator("list_apps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import ListAppsPaginator

session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
    paginator: ListAppsPaginator = client.get_paginator("list_apps")
```


### paginate

Type annotations and code completion for `#!python ListAppsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAppsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppsResponseTypeDef](./type_defs.md#listappsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAppsRequestListAppsPaginateTypeDef = {  # (1)
    "appIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppsRequestListAppsPaginateTypeDef](./type_defs.md#listappsrequestlistappspaginatetypedef) 
