# Paginators

> [Index](../README.md) > [Drs](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
    type annotations stubs module [types-aiobotocore-drs](https://pypi.org/project/types-aiobotocore-drs/).

## DescribeJobLogItemsPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_job_log_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/DescribeJobLogItems.html#Drs.Paginator.DescribeJobLogItems)

```python
# DescribeJobLogItemsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeJobLogItemsPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: DescribeJobLogItemsPaginator = client.get_paginator("describe_job_log_items")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobLogItemsResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [DescribeJobLogItemsPaginator](./paginators.md#describejoblogitemspaginator)
3. item: [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeJobLogItemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    jobID: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeJobLogItemsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeJobLogItemsResponseTypeDef](./type_defs.md#describejoblogitemsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeJobLogItemsRequestPaginateTypeDef = {  # (1)
    "jobID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobLogItemsRequestPaginateTypeDef](./type_defs.md#describejoblogitemsrequestpaginatetypedef) 
## DescribeJobsPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/DescribeJobs.html#Drs.Paginator.DescribeJobs)

```python
# DescribeJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeJobsPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: DescribeJobsPaginator = client.get_paginator("describe_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [DescribeJobsPaginator](./paginators.md#describejobspaginator)
3. item: [:material-code-braces: DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: DescribeJobsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeJobsRequestFiltersTypeDef](./type_defs.md#describejobsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeJobsResponseTypeDef](./type_defs.md#describejobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeJobsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobsRequestPaginateTypeDef](./type_defs.md#describejobsrequestpaginatetypedef) 
## DescribeLaunchConfigurationTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_launch_configuration_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/DescribeLaunchConfigurationTemplates.html#Drs.Paginator.DescribeLaunchConfigurationTemplates)

```python
# DescribeLaunchConfigurationTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeLaunchConfigurationTemplatesPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: DescribeLaunchConfigurationTemplatesPaginator = client.get_paginator("describe_launch_configuration_templates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLaunchConfigurationTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [DescribeLaunchConfigurationTemplatesPaginator](./paginators.md#describelaunchconfigurationtemplatespaginator)
3. item: [:material-code-braces: DescribeLaunchConfigurationTemplatesResponseTypeDef](./type_defs.md#describelaunchconfigurationtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLaunchConfigurationTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    launchConfigurationTemplateIDs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeLaunchConfigurationTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeLaunchConfigurationTemplatesResponseTypeDef](./type_defs.md#describelaunchconfigurationtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef = {  # (1)
    "launchConfigurationTemplateIDs": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLaunchConfigurationTemplatesRequestPaginateTypeDef](./type_defs.md#describelaunchconfigurationtemplatesrequestpaginatetypedef) 
## DescribeRecoveryInstancesPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_recovery_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/DescribeRecoveryInstances.html#Drs.Paginator.DescribeRecoveryInstances)

```python
# DescribeRecoveryInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeRecoveryInstancesPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: DescribeRecoveryInstancesPaginator = client.get_paginator("describe_recovery_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRecoveryInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [DescribeRecoveryInstancesPaginator](./paginators.md#describerecoveryinstancespaginator)
3. item: [:material-code-braces: DescribeRecoveryInstancesResponseTypeDef](./type_defs.md#describerecoveryinstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRecoveryInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: DescribeRecoveryInstancesRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeRecoveryInstancesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeRecoveryInstancesRequestFiltersTypeDef](./type_defs.md#describerecoveryinstancesrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeRecoveryInstancesResponseTypeDef](./type_defs.md#describerecoveryinstancesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRecoveryInstancesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRecoveryInstancesRequestPaginateTypeDef](./type_defs.md#describerecoveryinstancesrequestpaginatetypedef) 
## DescribeRecoverySnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_recovery_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/DescribeRecoverySnapshots.html#Drs.Paginator.DescribeRecoverySnapshots)

```python
# DescribeRecoverySnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeRecoverySnapshotsPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: DescribeRecoverySnapshotsPaginator = client.get_paginator("describe_recovery_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRecoverySnapshotsResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [DescribeRecoverySnapshotsPaginator](./paginators.md#describerecoverysnapshotspaginator)
3. item: [:material-code-braces: DescribeRecoverySnapshotsResponseTypeDef](./type_defs.md#describerecoverysnapshotsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRecoverySnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sourceServerID: str,
    filters: DescribeRecoverySnapshotsRequestFiltersTypeDef = ...,  # (1)
    order: RecoverySnapshotsOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[DescribeRecoverySnapshotsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: DescribeRecoverySnapshotsRequestFiltersTypeDef](./type_defs.md#describerecoverysnapshotsrequestfilterstypedef) 
2. See [:material-code-brackets: RecoverySnapshotsOrderType](./literals.md#recoverysnapshotsordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeRecoverySnapshotsResponseTypeDef](./type_defs.md#describerecoverysnapshotsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRecoverySnapshotsRequestPaginateTypeDef = {  # (1)
    "sourceServerID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRecoverySnapshotsRequestPaginateTypeDef](./type_defs.md#describerecoverysnapshotsrequestpaginatetypedef) 
## DescribeReplicationConfigurationTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_replication_configuration_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/DescribeReplicationConfigurationTemplates.html#Drs.Paginator.DescribeReplicationConfigurationTemplates)

```python
# DescribeReplicationConfigurationTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeReplicationConfigurationTemplatesPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: DescribeReplicationConfigurationTemplatesPaginator = client.get_paginator("describe_replication_configuration_templates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReplicationConfigurationTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [DescribeReplicationConfigurationTemplatesPaginator](./paginators.md#describereplicationconfigurationtemplatespaginator)
3. item: [:material-code-braces: DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReplicationConfigurationTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    replicationConfigurationTemplateIDs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeReplicationConfigurationTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReplicationConfigurationTemplatesResponseTypeDef](./type_defs.md#describereplicationconfigurationtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef = {  # (1)
    "replicationConfigurationTemplateIDs": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationConfigurationTemplatesRequestPaginateTypeDef](./type_defs.md#describereplicationconfigurationtemplatesrequestpaginatetypedef) 
## DescribeSourceNetworksPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_source_networks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/DescribeSourceNetworks.html#Drs.Paginator.DescribeSourceNetworks)

```python
# DescribeSourceNetworksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeSourceNetworksPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: DescribeSourceNetworksPaginator = client.get_paginator("describe_source_networks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSourceNetworksResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [DescribeSourceNetworksPaginator](./paginators.md#describesourcenetworkspaginator)
3. item: [:material-code-braces: DescribeSourceNetworksResponseTypeDef](./type_defs.md#describesourcenetworksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSourceNetworksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: DescribeSourceNetworksRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeSourceNetworksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeSourceNetworksRequestFiltersTypeDef](./type_defs.md#describesourcenetworksrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSourceNetworksResponseTypeDef](./type_defs.md#describesourcenetworksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSourceNetworksRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSourceNetworksRequestPaginateTypeDef](./type_defs.md#describesourcenetworksrequestpaginatetypedef) 
## DescribeSourceServersPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("describe_source_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/DescribeSourceServers.html#Drs.Paginator.DescribeSourceServers)

```python
# DescribeSourceServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import DescribeSourceServersPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: DescribeSourceServersPaginator = client.get_paginator("describe_source_servers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSourceServersResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [DescribeSourceServersPaginator](./paginators.md#describesourceserverspaginator)
3. item: [:material-code-braces: DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSourceServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: DescribeSourceServersRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeSourceServersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeSourceServersRequestFiltersTypeDef](./type_defs.md#describesourceserversrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSourceServersResponseTypeDef](./type_defs.md#describesourceserversresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSourceServersRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSourceServersRequestPaginateTypeDef](./type_defs.md#describesourceserversrequestpaginatetypedef) 
## ListExtensibleSourceServersPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("list_extensible_source_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/ListExtensibleSourceServers.html#Drs.Paginator.ListExtensibleSourceServers)

```python
# ListExtensibleSourceServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import ListExtensibleSourceServersPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: ListExtensibleSourceServersPaginator = client.get_paginator("list_extensible_source_servers")  # (2)
    async for item in paginator.paginate(...):
        item: ListExtensibleSourceServersResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [ListExtensibleSourceServersPaginator](./paginators.md#listextensiblesourceserverspaginator)
3. item: [:material-code-braces: ListExtensibleSourceServersResponseTypeDef](./type_defs.md#listextensiblesourceserversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExtensibleSourceServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    stagingAccountID: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListExtensibleSourceServersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListExtensibleSourceServersResponseTypeDef](./type_defs.md#listextensiblesourceserversresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExtensibleSourceServersRequestPaginateTypeDef = {  # (1)
    "stagingAccountID": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExtensibleSourceServersRequestPaginateTypeDef](./type_defs.md#listextensiblesourceserversrequestpaginatetypedef) 
## ListLaunchActionsPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("list_launch_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/ListLaunchActions.html#Drs.Paginator.ListLaunchActions)

```python
# ListLaunchActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import ListLaunchActionsPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: ListLaunchActionsPaginator = client.get_paginator("list_launch_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLaunchActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [ListLaunchActionsPaginator](./paginators.md#listlaunchactionspaginator)
3. item: [:material-code-braces: ListLaunchActionsResponseTypeDef](./type_defs.md#listlaunchactionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLaunchActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceId: str,
    filters: LaunchActionsRequestFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListLaunchActionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: LaunchActionsRequestFiltersTypeDef](./type_defs.md#launchactionsrequestfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLaunchActionsResponseTypeDef](./type_defs.md#listlaunchactionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLaunchActionsRequestPaginateTypeDef = {  # (1)
    "resourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLaunchActionsRequestPaginateTypeDef](./type_defs.md#listlaunchactionsrequestpaginatetypedef) 
## ListStagingAccountsPaginator

Type annotations and code completion for `#!python session.create_client("drs").get_paginator("list_staging_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs/paginator/ListStagingAccounts.html#Drs.Paginator.ListStagingAccounts)

```python
# ListStagingAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_drs.paginator import ListStagingAccountsPaginator

session = get_session()
async with session.create_client("drs") as client:  # (1)
    paginator: ListStagingAccountsPaginator = client.get_paginator("list_staging_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListStagingAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [DrsClient](./client.md)
2. paginator: [ListStagingAccountsPaginator](./paginators.md#liststagingaccountspaginator)
3. item: [:material-code-braces: ListStagingAccountsResponseTypeDef](./type_defs.md#liststagingaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListStagingAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListStagingAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStagingAccountsResponseTypeDef](./type_defs.md#liststagingaccountsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListStagingAccountsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStagingAccountsRequestPaginateTypeDef](./type_defs.md#liststagingaccountsrequestpaginatetypedef) 
