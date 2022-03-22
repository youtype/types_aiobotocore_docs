<a id="paginators-for-aiobotocore-sms-module"></a>

# Paginators for aiobotocore SMS module

> [Index](../README.md) > [SMS](./README.md) > Paginators

Auto-generated documentation for
[SMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
type annotations stubs module
[types-aiobotocore-sms](https://pypi.org/project/types-aiobotocore-sms/).

- [Paginators for aiobotocore SMS module](#paginators-for-aiobotocore-sms-module)
  - [GetConnectorsPaginator](#getconnectorspaginator)
  - [GetReplicationJobsPaginator](#getreplicationjobspaginator)
  - [GetReplicationRunsPaginator](#getreplicationrunspaginator)
  - [GetServersPaginator](#getserverspaginator)
  - [ListAppsPaginator](#listappspaginator)

<a id="getconnectorspaginator"></a>

## GetConnectorsPaginator

Type annotations for
`session.create_client("sms").get_paginator("get_connectors")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetConnectorsPaginator

session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
    paginator: GetConnectorsPaginator = client.get_paginator("get_connectors")
```

Boto3 documentation:
[SMS.Paginator.GetConnectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetConnectors)

Arguments for `GetConnectorsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetConnectorsPaginator.paginate` returns
`AsyncIterator`\[[GetConnectorsResponseTypeDef](./type_defs.md#getconnectorsresponsetypedef)\].

<a id="getreplicationjobspaginator"></a>

## GetReplicationJobsPaginator

Type annotations for
`session.create_client("sms").get_paginator("get_replication_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetReplicationJobsPaginator

session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
    paginator: GetReplicationJobsPaginator = client.get_paginator("get_replication_jobs")
```

Boto3 documentation:
[SMS.Paginator.GetReplicationJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationJobs)

Arguments for `GetReplicationJobsPaginator.paginate` method:

- `replicationJobId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetReplicationJobsPaginator.paginate` returns
`AsyncIterator`\[[GetReplicationJobsResponseTypeDef](./type_defs.md#getreplicationjobsresponsetypedef)\].

<a id="getreplicationrunspaginator"></a>

## GetReplicationRunsPaginator

Type annotations for
`session.create_client("sms").get_paginator("get_replication_runs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetReplicationRunsPaginator

session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
    paginator: GetReplicationRunsPaginator = client.get_paginator("get_replication_runs")
```

Boto3 documentation:
[SMS.Paginator.GetReplicationRuns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetReplicationRuns)

Arguments for `GetReplicationRunsPaginator.paginate` method:

- `replicationJobId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetReplicationRunsPaginator.paginate` returns
`AsyncIterator`\[[GetReplicationRunsResponseTypeDef](./type_defs.md#getreplicationrunsresponsetypedef)\].

<a id="getserverspaginator"></a>

## GetServersPaginator

Type annotations for
`session.create_client("sms").get_paginator("get_servers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import GetServersPaginator

session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
    paginator: GetServersPaginator = client.get_paginator("get_servers")
```

Boto3 documentation:
[SMS.Paginator.GetServers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.GetServers)

Arguments for `GetServersPaginator.paginate` method:

- `vmServerAddressList`:
  `Sequence`\[[VmServerAddressTypeDef](./type_defs.md#vmserveraddresstypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetServersPaginator.paginate` returns
`AsyncIterator`\[[GetServersResponseTypeDef](./type_defs.md#getserversresponsetypedef)\].

<a id="listappspaginator"></a>

## ListAppsPaginator

Type annotations for `session.create_client("sms").get_paginator("list_apps")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sms.paginator import ListAppsPaginator

session = get_session()
async with session.create_client("sms") as client:
    client: SMSClient
    paginator: ListAppsPaginator = client.get_paginator("list_apps")
```

Boto3 documentation:
[SMS.Paginator.ListApps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS.Paginator.ListApps)

Arguments for `ListAppsPaginator.paginate` method:

- `appIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAppsPaginator.paginate` returns
`AsyncIterator`\[[ListAppsResponseTypeDef](./type_defs.md#listappsresponsetypedef)\].
