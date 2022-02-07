<a id="paginators-for-aiobotocore-mgn-module"></a>

# Paginators for aiobotocore mgn module

> [Index](..) > [mgn](.) > Paginators

Auto-generated documentation for
[mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn)
type annotations stubs module
[types-aiobotocore-mgn](https://pypi.org/project/types-aiobotocore-mgn/).

- [Paginators for aiobotocore mgn module](#paginators-for-aiobotocore-mgn-module)
  - [DescribeJobLogItemsPaginator](#describejoblogitemspaginator)
  - [DescribeJobsPaginator](#describejobspaginator)
  - [DescribeReplicationConfigurationTemplatesPaginator](#describereplicationconfigurationtemplatespaginator)
  - [DescribeSourceServersPaginator](#describesourceserverspaginator)
  - [DescribeVcenterClientsPaginator](#describevcenterclientspaginator)

<a id="describejoblogitemspaginator"></a>

## DescribeJobLogItemsPaginator

Type annotations for
`session.create_client("mgn").get_paginator("describe_job_log_items")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeJobLogItemsPaginator

session = get_session()
async with session.create_client("mgn") as client:
    client: mgnClient
    paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")
```

Boto3 documentation:
[mgn.Paginator.DescribeJobLogItems](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobLogItems)

Arguments for `DescribeJobLogItemsPaginator.paginate` method:

- `jobID`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeJobLogItemsPaginator.paginate` returns
`_PageIterator`\[[DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef)\].

<a id="describejobspaginator"></a>

## DescribeJobsPaginator

Type annotations for
`session.create_client("mgn").get_paginator("describe_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeJobsPaginator

session = get_session()
async with session.create_client("mgn") as client:
    client: mgnClient
    paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")
```

Boto3 documentation:
[mgn.Paginator.DescribeJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeJobs)

Arguments for `DescribeJobsPaginator.paginate` method:

- `filters`:
  [DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeJobsPaginator.paginate` returns
`_PageIterator`\[[DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef)\].

<a id="describereplicationconfigurationtemplatespaginator"></a>

## DescribeReplicationConfigurationTemplatesPaginator

Type annotations for
`session.create_client("mgn").get_paginator("describe_replication_configuration_templates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeReplicationConfigurationTemplatesPaginator

session = get_session()
async with session.create_client("mgn") as client:
    client: mgnClient
    paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator("describe_replication_configuration_templates")
```

Boto3 documentation:
[mgn.Paginator.DescribeReplicationConfigurationTemplates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeReplicationConfigurationTemplates)

Arguments for `DescribeReplicationConfigurationTemplatesPaginator.paginate`
method:

- `replicationConfigurationTemplateIDs`: `Sequence`\[`str`\] *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeReplicationConfigurationTemplatesPaginator.paginate` returns
`_PageIterator`\[[DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef)\].

<a id="describesourceserverspaginator"></a>

## DescribeSourceServersPaginator

Type annotations for
`session.create_client("mgn").get_paginator("describe_source_servers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeSourceServersPaginator

session = get_session()
async with session.create_client("mgn") as client:
    client: mgnClient
    paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
```

Boto3 documentation:
[mgn.Paginator.DescribeSourceServers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeSourceServers)

Arguments for `DescribeSourceServersPaginator.paginate` method:

- `filters`:
  [DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeSourceServersPaginator.paginate` returns
`_PageIterator`\[[DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef)\].

<a id="describevcenterclientspaginator"></a>

## DescribeVcenterClientsPaginator

Type annotations for
`session.create_client("mgn").get_paginator("describe_vcenter_clients")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mgn.paginator import DescribeVcenterClientsPaginator

session = get_session()
async with session.create_client("mgn") as client:
    client: mgnClient
    paginator: DescribeVcenterClientsPaginator = client.get_paginator("describe_vcenter_clients")
```

Boto3 documentation:
[mgn.Paginator.DescribeVcenterClients](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn.Paginator.DescribeVcenterClients)

Arguments for `DescribeVcenterClientsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeVcenterClientsPaginator.paginate` returns
`_PageIterator`\[[DescribeVcenterClientsResponseTypeDef](./type_defs.md#describevcenterclientsresponsetypedef)\].
