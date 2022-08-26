# Paginators

> [Index](../README.md) > [Backup](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
    type annotations stubs module [types-aiobotocore-backup](https://pypi.org/project/types-aiobotocore-backup/).

## ListBackupJobsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListBackupJobsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListBackupJobsPaginator = client.get_paginator("list_backup_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListBackupJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListBackupJobsPaginator](./paginators.md#listbackupjobspaginator)
3. item: [:material-code-braces: ListBackupJobsOutputTypeDef](./type_defs.md#listbackupjobsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBackupJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ByResourceArn: str = ...,
    ByState: BackupJobStateType = ...,  # (1)
    ByBackupVaultName: str = ...,
    ByCreatedBefore: Union[datetime, str] = ...,
    ByCreatedAfter: Union[datetime, str] = ...,
    ByResourceType: str = ...,
    ByAccountId: str = ...,
    ByCompleteAfter: Union[datetime, str] = ...,
    ByCompleteBefore: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListBackupJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: BackupJobStateType](./literals.md#backupjobstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBackupJobsOutputTypeDef](./type_defs.md#listbackupjobsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBackupJobsInputListBackupJobsPaginateTypeDef = {  # (1)
    "ByResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupJobsInputListBackupJobsPaginateTypeDef](./type_defs.md#listbackupjobsinputlistbackupjobspaginatetypedef) 
## ListBackupPlanTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_plan_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListBackupPlanTemplatesPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListBackupPlanTemplatesPaginator = client.get_paginator("list_backup_plan_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListBackupPlanTemplatesOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListBackupPlanTemplatesPaginator](./paginators.md#listbackupplantemplatespaginator)
3. item: [:material-code-braces: ListBackupPlanTemplatesOutputTypeDef](./type_defs.md#listbackupplantemplatesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBackupPlanTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBackupPlanTemplatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBackupPlanTemplatesOutputTypeDef](./type_defs.md#listbackupplantemplatesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef](./type_defs.md#listbackupplantemplatesinputlistbackupplantemplatespaginatetypedef) 
## ListBackupPlanVersionsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_plan_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListBackupPlanVersionsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListBackupPlanVersionsPaginator = client.get_paginator("list_backup_plan_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListBackupPlanVersionsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListBackupPlanVersionsPaginator](./paginators.md#listbackupplanversionspaginator)
3. item: [:material-code-braces: ListBackupPlanVersionsOutputTypeDef](./type_defs.md#listbackupplanversionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBackupPlanVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    BackupPlanId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBackupPlanVersionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBackupPlanVersionsOutputTypeDef](./type_defs.md#listbackupplanversionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = {  # (1)
    "BackupPlanId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef](./type_defs.md#listbackupplanversionsinputlistbackupplanversionspaginatetypedef) 
## ListBackupPlansPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_plans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListBackupPlansPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListBackupPlansPaginator = client.get_paginator("list_backup_plans")  # (2)
    async for item in paginator.paginate(...):
        item: ListBackupPlansOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListBackupPlansPaginator](./paginators.md#listbackupplanspaginator)
3. item: [:material-code-braces: ListBackupPlansOutputTypeDef](./type_defs.md#listbackupplansoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBackupPlansPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    IncludeDeleted: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBackupPlansOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBackupPlansOutputTypeDef](./type_defs.md#listbackupplansoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBackupPlansInputListBackupPlansPaginateTypeDef = {  # (1)
    "IncludeDeleted": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupPlansInputListBackupPlansPaginateTypeDef](./type_defs.md#listbackupplansinputlistbackupplanspaginatetypedef) 
## ListBackupSelectionsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_selections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListBackupSelectionsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListBackupSelectionsPaginator = client.get_paginator("list_backup_selections")  # (2)
    async for item in paginator.paginate(...):
        item: ListBackupSelectionsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListBackupSelectionsPaginator](./paginators.md#listbackupselectionspaginator)
3. item: [:material-code-braces: ListBackupSelectionsOutputTypeDef](./type_defs.md#listbackupselectionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBackupSelectionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    BackupPlanId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBackupSelectionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBackupSelectionsOutputTypeDef](./type_defs.md#listbackupselectionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = {  # (1)
    "BackupPlanId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef](./type_defs.md#listbackupselectionsinputlistbackupselectionspaginatetypedef) 
## ListBackupVaultsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_vaults")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListBackupVaultsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListBackupVaultsPaginator = client.get_paginator("list_backup_vaults")  # (2)
    async for item in paginator.paginate(...):
        item: ListBackupVaultsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListBackupVaultsPaginator](./paginators.md#listbackupvaultspaginator)
3. item: [:material-code-braces: ListBackupVaultsOutputTypeDef](./type_defs.md#listbackupvaultsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBackupVaultsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBackupVaultsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBackupVaultsOutputTypeDef](./type_defs.md#listbackupvaultsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListBackupVaultsInputListBackupVaultsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupVaultsInputListBackupVaultsPaginateTypeDef](./type_defs.md#listbackupvaultsinputlistbackupvaultspaginatetypedef) 
## ListCopyJobsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_copy_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListCopyJobsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListCopyJobsPaginator = client.get_paginator("list_copy_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListCopyJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListCopyJobsPaginator](./paginators.md#listcopyjobspaginator)
3. item: [:material-code-braces: ListCopyJobsOutputTypeDef](./type_defs.md#listcopyjobsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListCopyJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ByResourceArn: str = ...,
    ByState: CopyJobStateType = ...,  # (1)
    ByCreatedBefore: Union[datetime, str] = ...,
    ByCreatedAfter: Union[datetime, str] = ...,
    ByResourceType: str = ...,
    ByDestinationVaultArn: str = ...,
    ByAccountId: str = ...,
    ByCompleteBefore: Union[datetime, str] = ...,
    ByCompleteAfter: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListCopyJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: CopyJobStateType](./literals.md#copyjobstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCopyJobsOutputTypeDef](./type_defs.md#listcopyjobsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListCopyJobsInputListCopyJobsPaginateTypeDef = {  # (1)
    "ByResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCopyJobsInputListCopyJobsPaginateTypeDef](./type_defs.md#listcopyjobsinputlistcopyjobspaginatetypedef) 
## ListProtectedResourcesPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_protected_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListProtectedResourcesPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListProtectedResourcesPaginator = client.get_paginator("list_protected_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListProtectedResourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListProtectedResourcesPaginator](./paginators.md#listprotectedresourcespaginator)
3. item: [:material-code-braces: ListProtectedResourcesOutputTypeDef](./type_defs.md#listprotectedresourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListProtectedResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProtectedResourcesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProtectedResourcesOutputTypeDef](./type_defs.md#listprotectedresourcesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef](./type_defs.md#listprotectedresourcesinputlistprotectedresourcespaginatetypedef) 
## ListRecoveryPointsByBackupVaultPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_recovery_points_by_backup_vault")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListRecoveryPointsByBackupVaultPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListRecoveryPointsByBackupVaultPaginator = client.get_paginator("list_recovery_points_by_backup_vault")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecoveryPointsByBackupVaultOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListRecoveryPointsByBackupVaultPaginator](./paginators.md#listrecoverypointsbybackupvaultpaginator)
3. item: [:material-code-braces: ListRecoveryPointsByBackupVaultOutputTypeDef](./type_defs.md#listrecoverypointsbybackupvaultoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListRecoveryPointsByBackupVaultPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    BackupVaultName: str,
    ByResourceArn: str = ...,
    ByResourceType: str = ...,
    ByBackupPlanId: str = ...,
    ByCreatedBefore: Union[datetime, str] = ...,
    ByCreatedAfter: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecoveryPointsByBackupVaultOutputTypeDef](./type_defs.md#listrecoverypointsbybackupvaultoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = {  # (1)
    "BackupVaultName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef](./type_defs.md#listrecoverypointsbybackupvaultinputlistrecoverypointsbybackupvaultpaginatetypedef) 
## ListRecoveryPointsByResourcePaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_recovery_points_by_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListRecoveryPointsByResourcePaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListRecoveryPointsByResourcePaginator = client.get_paginator("list_recovery_points_by_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecoveryPointsByResourceOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListRecoveryPointsByResourcePaginator](./paginators.md#listrecoverypointsbyresourcepaginator)
3. item: [:material-code-braces: ListRecoveryPointsByResourceOutputTypeDef](./type_defs.md#listrecoverypointsbyresourceoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListRecoveryPointsByResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecoveryPointsByResourceOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecoveryPointsByResourceOutputTypeDef](./type_defs.md#listrecoverypointsbyresourceoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef](./type_defs.md#listrecoverypointsbyresourceinputlistrecoverypointsbyresourcepaginatetypedef) 
## ListRestoreJobsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_restore_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListRestoreJobsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListRestoreJobsPaginator = client.get_paginator("list_restore_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListRestoreJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListRestoreJobsPaginator](./paginators.md#listrestorejobspaginator)
3. item: [:material-code-braces: ListRestoreJobsOutputTypeDef](./type_defs.md#listrestorejobsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListRestoreJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ByAccountId: str = ...,
    ByCreatedBefore: Union[datetime, str] = ...,
    ByCreatedAfter: Union[datetime, str] = ...,
    ByStatus: RestoreJobStatusType = ...,  # (1)
    ByCompleteBefore: Union[datetime, str] = ...,
    ByCompleteAfter: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListRestoreJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListRestoreJobsOutputTypeDef](./type_defs.md#listrestorejobsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListRestoreJobsInputListRestoreJobsPaginateTypeDef = {  # (1)
    "ByAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRestoreJobsInputListRestoreJobsPaginateTypeDef](./type_defs.md#listrestorejobsinputlistrestorejobspaginatetypedef) 
