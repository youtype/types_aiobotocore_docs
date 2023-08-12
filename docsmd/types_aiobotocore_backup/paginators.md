# Paginators

> [Index](../README.md) > [Backup](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup)
    type annotations stubs module [types-aiobotocore-backup](https://pypi.org/project/types-aiobotocore-backup/).

## ListBackupJobsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupJobs)

```python
# ListBackupJobsPaginator usage example

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

```python
# paginate method definition

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
    ByParentJobId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListBackupJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: BackupJobStateType](./literals.md#backupjobstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBackupJobsOutputTypeDef](./type_defs.md#listbackupjobsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupJobsInputListBackupJobsPaginateTypeDef = {  # (1)
    "ByResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupJobsInputListBackupJobsPaginateTypeDef](./type_defs.md#listbackupjobsinputlistbackupjobspaginatetypedef) 
## ListBackupPlanTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_plan_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanTemplates)

```python
# ListBackupPlanTemplatesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBackupPlanTemplatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBackupPlanTemplatesOutputTypeDef](./type_defs.md#listbackupplantemplatesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupPlanTemplatesInputListBackupPlanTemplatesPaginateTypeDef](./type_defs.md#listbackupplantemplatesinputlistbackupplantemplatespaginatetypedef) 
## ListBackupPlanVersionsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_plan_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlanVersions)

```python
# ListBackupPlanVersionsPaginator usage example

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

```python
# paginate method definition

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


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef = {  # (1)
    "BackupPlanId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupPlanVersionsInputListBackupPlanVersionsPaginateTypeDef](./type_defs.md#listbackupplanversionsinputlistbackupplanversionspaginatetypedef) 
## ListBackupPlansPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_plans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupPlans)

```python
# ListBackupPlansPaginator usage example

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

```python
# paginate method definition

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


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupPlansInputListBackupPlansPaginateTypeDef = {  # (1)
    "IncludeDeleted": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupPlansInputListBackupPlansPaginateTypeDef](./type_defs.md#listbackupplansinputlistbackupplanspaginatetypedef) 
## ListBackupSelectionsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_selections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupSelections)

```python
# ListBackupSelectionsPaginator usage example

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

```python
# paginate method definition

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


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef = {  # (1)
    "BackupPlanId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupSelectionsInputListBackupSelectionsPaginateTypeDef](./type_defs.md#listbackupselectionsinputlistbackupselectionspaginatetypedef) 
## ListBackupVaultsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_vaults")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListBackupVaults)

```python
# ListBackupVaultsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    ByVaultType: VaultTypeType = ...,  # (1)
    ByShared: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListBackupVaultsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBackupVaultsOutputTypeDef](./type_defs.md#listbackupvaultsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupVaultsInputListBackupVaultsPaginateTypeDef = {  # (1)
    "ByVaultType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupVaultsInputListBackupVaultsPaginateTypeDef](./type_defs.md#listbackupvaultsinputlistbackupvaultspaginatetypedef) 
## ListCopyJobsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_copy_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListCopyJobs)

```python
# ListCopyJobsPaginator usage example

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

```python
# paginate method definition

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
    ByParentJobId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListCopyJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: CopyJobStateType](./literals.md#copyjobstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCopyJobsOutputTypeDef](./type_defs.md#listcopyjobsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCopyJobsInputListCopyJobsPaginateTypeDef = {  # (1)
    "ByResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCopyJobsInputListCopyJobsPaginateTypeDef](./type_defs.md#listcopyjobsinputlistcopyjobspaginatetypedef) 
## ListLegalHoldsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_legal_holds")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListLegalHolds)

```python
# ListLegalHoldsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListLegalHoldsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListLegalHoldsPaginator = client.get_paginator("list_legal_holds")  # (2)
    async for item in paginator.paginate(...):
        item: ListLegalHoldsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListLegalHoldsPaginator](./paginators.md#listlegalholdspaginator)
3. item: [:material-code-braces: ListLegalHoldsOutputTypeDef](./type_defs.md#listlegalholdsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListLegalHoldsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLegalHoldsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLegalHoldsOutputTypeDef](./type_defs.md#listlegalholdsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLegalHoldsInputListLegalHoldsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLegalHoldsInputListLegalHoldsPaginateTypeDef](./type_defs.md#listlegalholdsinputlistlegalholdspaginatetypedef) 
## ListProtectedResourcesPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_protected_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResources)

```python
# ListProtectedResourcesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProtectedResourcesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProtectedResourcesOutputTypeDef](./type_defs.md#listprotectedresourcesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectedResourcesInputListProtectedResourcesPaginateTypeDef](./type_defs.md#listprotectedresourcesinputlistprotectedresourcespaginatetypedef) 
## ListProtectedResourcesByBackupVaultPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_protected_resources_by_backup_vault")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListProtectedResourcesByBackupVault)

```python
# ListProtectedResourcesByBackupVaultPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListProtectedResourcesByBackupVaultPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListProtectedResourcesByBackupVaultPaginator = client.get_paginator("list_protected_resources_by_backup_vault")  # (2)
    async for item in paginator.paginate(...):
        item: ListProtectedResourcesByBackupVaultOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListProtectedResourcesByBackupVaultPaginator](./paginators.md#listprotectedresourcesbybackupvaultpaginator)
3. item: [:material-code-braces: ListProtectedResourcesByBackupVaultOutputTypeDef](./type_defs.md#listprotectedresourcesbybackupvaultoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListProtectedResourcesByBackupVaultPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BackupVaultName: str,
    BackupVaultAccountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProtectedResourcesByBackupVaultOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProtectedResourcesByBackupVaultOutputTypeDef](./type_defs.md#listprotectedresourcesbybackupvaultoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProtectedResourcesByBackupVaultInputListProtectedResourcesByBackupVaultPaginateTypeDef = {  # (1)
    "BackupVaultName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectedResourcesByBackupVaultInputListProtectedResourcesByBackupVaultPaginateTypeDef](./type_defs.md#listprotectedresourcesbybackupvaultinputlistprotectedresourcesbybackupvaultpaginatetypedef) 
## ListRecoveryPointsByBackupVaultPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_recovery_points_by_backup_vault")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByBackupVault)

```python
# ListRecoveryPointsByBackupVaultPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    BackupVaultName: str,
    BackupVaultAccountId: str = ...,
    ByResourceArn: str = ...,
    ByResourceType: str = ...,
    ByBackupPlanId: str = ...,
    ByCreatedBefore: Union[datetime, str] = ...,
    ByCreatedAfter: Union[datetime, str] = ...,
    ByParentRecoveryPointArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecoveryPointsByBackupVaultOutputTypeDef](./type_defs.md#listrecoverypointsbybackupvaultoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef = {  # (1)
    "BackupVaultName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecoveryPointsByBackupVaultInputListRecoveryPointsByBackupVaultPaginateTypeDef](./type_defs.md#listrecoverypointsbybackupvaultinputlistrecoverypointsbybackupvaultpaginatetypedef) 
## ListRecoveryPointsByLegalHoldPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_recovery_points_by_legal_hold")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByLegalHold)

```python
# ListRecoveryPointsByLegalHoldPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListRecoveryPointsByLegalHoldPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListRecoveryPointsByLegalHoldPaginator = client.get_paginator("list_recovery_points_by_legal_hold")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecoveryPointsByLegalHoldOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListRecoveryPointsByLegalHoldPaginator](./paginators.md#listrecoverypointsbylegalholdpaginator)
3. item: [:material-code-braces: ListRecoveryPointsByLegalHoldOutputTypeDef](./type_defs.md#listrecoverypointsbylegalholdoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListRecoveryPointsByLegalHoldPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LegalHoldId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRecoveryPointsByLegalHoldOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRecoveryPointsByLegalHoldOutputTypeDef](./type_defs.md#listrecoverypointsbylegalholdoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef = {  # (1)
    "LegalHoldId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecoveryPointsByLegalHoldInputListRecoveryPointsByLegalHoldPaginateTypeDef](./type_defs.md#listrecoverypointsbylegalholdinputlistrecoverypointsbylegalholdpaginatetypedef) 
## ListRecoveryPointsByResourcePaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_recovery_points_by_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRecoveryPointsByResource)

```python
# ListRecoveryPointsByResourcePaginator usage example

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

```python
# paginate method definition

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


```python
# paginate method usage example with argument unpacking

kwargs: ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecoveryPointsByResourceInputListRecoveryPointsByResourcePaginateTypeDef](./type_defs.md#listrecoverypointsbyresourceinputlistrecoverypointsbyresourcepaginatetypedef) 
## ListRestoreJobsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_restore_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#Backup.Paginator.ListRestoreJobs)

```python
# ListRestoreJobsPaginator usage example

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

```python
# paginate method definition

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


```python
# paginate method usage example with argument unpacking

kwargs: ListRestoreJobsInputListRestoreJobsPaginateTypeDef = {  # (1)
    "ByAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRestoreJobsInputListRestoreJobsPaginateTypeDef](./type_defs.md#listrestorejobsinputlistrestorejobspaginatetypedef) 
