<a id="paginators-for-aiobotocore-drs-module"></a>

# Paginators for aiobotocore drs module

> [Index](../README.md) > [drs](./README.md) > Paginators

Auto-generated documentation for
[drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
type annotations stubs module
[types-aiobotocore-drs](https://pypi.org/project/types-aiobotocore-drs/).

- [Paginators for aiobotocore drs module](#paginators-for-aiobotocore-drs-module)
  - [DescribeJobLogItemsPaginator](#describejoblogitemspaginator)
  - [DescribeJobsPaginator](#describejobspaginator)
  - [DescribeRecoveryInstancesPaginator](#describerecoveryinstancespaginator)
  - [DescribeRecoverySnapshotsPaginator](#describerecoverysnapshotspaginator)
  - [DescribeReplicationConfigurationTemplatesPaginator](#describereplicationconfigurationtemplatespaginator)
  - [DescribeSourceServersPaginator](#describesourceserverspaginator)

<a id="describejoblogitemspaginator"></a>

## DescribeJobLogItemsPaginator

Type annotations for
`session.create_client("drs").get_paginator("describe_job_log_items")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeJobLogItemsPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")
```

Boto3 documentation:
[drs.Paginator.DescribeJobLogItems](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems)

Arguments for `DescribeJobLogItemsPaginator.paginate` method:

- `jobID`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeJobLogItemsPaginator.paginate` returns
`AsyncIterator`\[[DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef)\].

<a id="describejobspaginator"></a>

## DescribeJobsPaginator

Type annotations for
`session.create_client("drs").get_paginator("describe_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeJobsPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")
```

Boto3 documentation:
[drs.Paginator.DescribeJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs)

Arguments for `DescribeJobsPaginator.paginate` method:

- `filters`:
  [DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeJobsPaginator.paginate` returns
`AsyncIterator`\[[DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef)\].

<a id="describerecoveryinstancespaginator"></a>

## DescribeRecoveryInstancesPaginator

Type annotations for
`session.create_client("drs").get_paginator("describe_recovery_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeRecoveryInstancesPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeRecoveryInstancesPaginator = client.get_paginator("describe_recovery_instances")
```

Boto3 documentation:
[drs.Paginator.DescribeRecoveryInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances)

Arguments for `DescribeRecoveryInstancesPaginator.paginate` method:

- `filters`:
  [DescribeRecoveryInstancesRequestFiltersTypeDef](./type_defs.md#describerecoveryinstancesrequestfilterstypedef)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeRecoveryInstancesPaginator.paginate` returns
`AsyncIterator`\[[DescribeRecoveryInstancesResponseTypeDef](./type_defs.md#describerecoveryinstancesresponsetypedef)\].

<a id="describerecoverysnapshotspaginator"></a>

## DescribeRecoverySnapshotsPaginator

Type annotations for
`session.create_client("drs").get_paginator("describe_recovery_snapshots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeRecoverySnapshotsPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeRecoverySnapshotsPaginator = client.get_paginator("describe_recovery_snapshots")
```

Boto3 documentation:
[drs.Paginator.DescribeRecoverySnapshots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots)

Arguments for `DescribeRecoverySnapshotsPaginator.paginate` method:

- `sourceServerID`: `str` *(required)*
- `filters`:
  [DescribeRecoverySnapshotsRequestFiltersTypeDef](./type_defs.md#describerecoverysnapshotsrequestfilterstypedef)
- `order`:
  [RecoverySnapshotsOrderType](./literals.md#recoverysnapshotsordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeRecoverySnapshotsPaginator.paginate` returns
`AsyncIterator`\[[DescribeRecoverySnapshotsResponseTypeDef](./type_defs.md#describerecoverysnapshotsresponsetypedef)\].

<a id="describereplicationconfigurationtemplatespaginator"></a>

## DescribeReplicationConfigurationTemplatesPaginator

Type annotations for
`session.create_client("drs").get_paginator("describe_replication_configuration_templates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeReplicationConfigurationTemplatesPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator("describe_replication_configuration_templates")
```

Boto3 documentation:
[drs.Paginator.DescribeReplicationConfigurationTemplates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates)

Arguments for `DescribeReplicationConfigurationTemplatesPaginator.paginate`
method:

- `replicationConfigurationTemplateIDs`: `Sequence`\[`str`\] *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeReplicationConfigurationTemplatesPaginator.paginate` returns
`AsyncIterator`\[[DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef)\].

<a id="describesourceserverspaginator"></a>

## DescribeSourceServersPaginator

Type annotations for
`session.create_client("drs").get_paginator("describe_source_servers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeSourceServersPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
```

Boto3 documentation:
[drs.Paginator.DescribeSourceServers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers)

Arguments for `DescribeSourceServersPaginator.paginate` method:

- `filters`:
  [DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeSourceServersPaginator.paginate` returns
`AsyncIterator`\[[DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef)\].
