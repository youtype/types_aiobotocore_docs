<a id="paginators-for-aiobotocore-opsworkscm-module"></a>

# Paginators for aiobotocore OpsWorksCM module

> [Index](..) > [OpsWorksCM](.) > Paginators

Auto-generated documentation for
[OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
type annotations stubs module
[types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).

- [Paginators for aiobotocore OpsWorksCM module](#paginators-for-aiobotocore-opsworkscm-module)
  - [DescribeBackupsPaginator](#describebackupspaginator)
  - [DescribeEventsPaginator](#describeeventspaginator)
  - [DescribeServersPaginator](#describeserverspaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)

<a id="describebackupspaginator"></a>

## DescribeBackupsPaginator

Type annotations for
`session.create_client("opsworkscm").get_paginator("describe_backups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.paginator import DescribeBackupsPaginator

session = get_session()
async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient
    paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")
```

Boto3 documentation:
[OpsWorksCM.Paginator.DescribeBackups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeBackups)

Arguments for `DescribeBackupsPaginator.paginate` method:

- `BackupId`: `str`
- `ServerName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeBackupsPaginator.paginate` returns
`_PageIterator`\[[DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef)\].

<a id="describeeventspaginator"></a>

## DescribeEventsPaginator

Type annotations for
`session.create_client("opsworkscm").get_paginator("describe_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
```

Boto3 documentation:
[OpsWorksCM.Paginator.DescribeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents)

Arguments for `DescribeEventsPaginator.paginate` method:

- `ServerName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEventsPaginator.paginate` returns
`_PageIterator`\[[DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef)\].

<a id="describeserverspaginator"></a>

## DescribeServersPaginator

Type annotations for
`session.create_client("opsworkscm").get_paginator("describe_servers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.paginator import DescribeServersPaginator

session = get_session()
async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient
    paginator: DescribeServersPaginator = client.get_paginator("describe_servers")
```

Boto3 documentation:
[OpsWorksCM.Paginator.DescribeServers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers)

Arguments for `DescribeServersPaginator.paginate` method:

- `ServerName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeServersPaginator.paginate` returns
`_PageIterator`\[[DescribeServersResponseTypeDef](./type_defs.md#describeserversresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("opsworkscm").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[OpsWorksCM.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `ResourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`_PageIterator`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].
