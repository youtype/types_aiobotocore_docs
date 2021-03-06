# Paginators

> [Index](../README.md) > [drs](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
    type annotations stubs module [types-aiobotocore-drs](https://pypi.org/project/types-aiobotocore-drs/).

## DescribeJobLogItemsPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_job_log_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobLogItems)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeJobLogItemsPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")
```


### paginate

Type annotations and code completion for `#!python DescribeJobLogItemsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    jobID: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeJobLogItemsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef = {  # (1)
    "jobID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobLogItemsRequestDescribeJobLogItemsPaginateTypeDef](./type_defs.md#describejoblogitemsrequestdescribejoblogitemspaginatetypedef) 
## DescribeJobsPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeJobsPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")
```


### paginate

Type annotations and code completion for `#!python DescribeJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: DescribeJobsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeJobsRequestDescribeJobsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobsRequestDescribeJobsPaginateTypeDef](./type_defs.md#describejobsrequestdescribejobspaginatetypedef) 
## DescribeRecoveryInstancesPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_recovery_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoveryInstances)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeRecoveryInstancesPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeRecoveryInstancesPaginator = client.get_paginator("describe_recovery_instances")
```


### paginate

Type annotations and code completion for `#!python DescribeRecoveryInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeRecoveryInstancesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeRecoveryInstancesRequestFiltersTypeDef](./type_defs.md#describerecoveryinstancesrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeRecoveryInstancesResponseTypeDef](./type_defs.md#describerecoveryinstancesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRecoveryInstancesRequestDescribeRecoveryInstancesPaginateTypeDef](./type_defs.md#describerecoveryinstancesrequestdescriberecoveryinstancespaginatetypedef) 
## DescribeRecoverySnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_recovery_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeRecoverySnapshots)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeRecoverySnapshotsPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeRecoverySnapshotsPaginator = client.get_paginator("describe_recovery_snapshots")
```


### paginate

Type annotations and code completion for `#!python DescribeRecoverySnapshotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    sourceServerID: str,
    filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,  # (1)
    order: RecoverySnapshotsOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeRecoverySnapshotsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: DescribeRecoverySnapshotsRequestFiltersTypeDef](./type_defs.md#describerecoverysnapshotsrequestfilterstypedef) 
2. See [:material-code-brackets: RecoverySnapshotsOrderType](./literals.md#recoverysnapshotsordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeRecoverySnapshotsResponseTypeDef](./type_defs.md#describerecoverysnapshotsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRecoverySnapshotsRequestDescribeRecoverySnapshotsPaginateTypeDef](./type_defs.md#describerecoverysnapshotsrequestdescriberecoverysnapshotspaginatetypedef) 
## DescribeReplicationConfigurationTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_replication_configuration_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeReplicationConfigurationTemplates)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeReplicationConfigurationTemplatesPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator("describe_replication_configuration_templates")
```


### paginate

Type annotations and code completion for `#!python DescribeReplicationConfigurationTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    replicationConfigurationTemplateIDs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef = {  # (1)
    "replicationConfigurationTemplateIDs": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationConfigurationTemplatesRequestDescribeReplicationConfigurationTemplatesPaginateTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestdescribereplicationconfigurationtemplatespaginatetypedef) 
## DescribeSourceServersPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_source_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.DescribeSourceServers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeSourceServersPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")
```


### paginate

Type annotations and code completion for `#!python DescribeSourceServersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: DescribeSourceServersRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSourceServersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSourceServersRequestDescribeSourceServersPaginateTypeDef](./type_defs.md#describesourceserversrequestdescribesourceserverspaginatetypedef) 
## ListExtensibleSourceServersPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("list_extensible_source_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListExtensibleSourceServers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import ListExtensibleSourceServersPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: ListExtensibleSourceServersPaginator = client.get_paginator("list_extensible_source_servers")
```


### paginate

Type annotations and code completion for `#!python ListExtensibleSourceServersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    stagingAccountID: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListExtensibleSourceServersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListExtensibleSourceServersResponseTypeDef](./type_defs.md#listextensiblesourceserversresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef = {  # (1)
    "stagingAccountID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExtensibleSourceServersRequestListExtensibleSourceServersPaginateTypeDef](./type_defs.md#listextensiblesourceserversrequestlistextensiblesourceserverspaginatetypedef) 
## ListStagingAccountsPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("list_staging_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs.Paginator.ListStagingAccounts)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import ListStagingAccountsPaginator

session = get_session()
async with session.create_client("drs") as client:
    client: drsClient
    paginator: ListStagingAccountsPaginator = client.get_paginator("list_staging_accounts")
```


### paginate

Type annotations and code completion for `#!python ListStagingAccountsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStagingAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStagingAccountsResponseTypeDef](./type_defs.md#liststagingaccountsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStagingAccountsRequestListStagingAccountsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStagingAccountsRequestListStagingAccountsPaginateTypeDef](./type_defs.md#liststagingaccountsrequestliststagingaccountspaginatetypedef) 
