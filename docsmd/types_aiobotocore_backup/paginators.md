# Paginators

> [Index](../README.md) > [Backup](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#backup)
    type annotations stubs module [types-aiobotocore-backup](https://pypi.org/project/types-aiobotocore-backup/).

## ListBackupJobsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListBackupJobs.html#Backup.Paginator.ListBackupJobs)

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
3. item: `AioPageIterator[ListBackupJobsOutputTypeDef]`


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
    ByCreatedBefore: TimestampTypeDef = ...,
    ByCreatedAfter: TimestampTypeDef = ...,
    ByResourceType: str = ...,
    ByAccountId: str = ...,
    ByCompleteAfter: TimestampTypeDef = ...,
    ByCompleteBefore: TimestampTypeDef = ...,
    ByParentJobId: str = ...,
    ByMessageCategory: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBackupJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: BackupJobStateType](./literals.md#backupjobstatetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBackupJobsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupJobsInputPaginateTypeDef = {  # (1)
    "ByResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupJobsInputPaginateTypeDef](./type_defs.md#listbackupjobsinputpaginatetypedef)
## ListBackupPlanTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_plan_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListBackupPlanTemplates.html#Backup.Paginator.ListBackupPlanTemplates)

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
3. item: `AioPageIterator[ListBackupPlanTemplatesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBackupPlanTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBackupPlanTemplatesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBackupPlanTemplatesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupPlanTemplatesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupPlanTemplatesInputPaginateTypeDef](./type_defs.md#listbackupplantemplatesinputpaginatetypedef)
## ListBackupPlanVersionsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_plan_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListBackupPlanVersions.html#Backup.Paginator.ListBackupPlanVersions)

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
3. item: `AioPageIterator[ListBackupPlanVersionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBackupPlanVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BackupPlanId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBackupPlanVersionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBackupPlanVersionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupPlanVersionsInputPaginateTypeDef = {  # (1)
    "BackupPlanId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupPlanVersionsInputPaginateTypeDef](./type_defs.md#listbackupplanversionsinputpaginatetypedef)
## ListBackupPlansPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_plans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListBackupPlans.html#Backup.Paginator.ListBackupPlans)

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
3. item: `AioPageIterator[ListBackupPlansOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBackupPlansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IncludeDeleted: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBackupPlansOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBackupPlansOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupPlansInputPaginateTypeDef = {  # (1)
    "IncludeDeleted": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupPlansInputPaginateTypeDef](./type_defs.md#listbackupplansinputpaginatetypedef)
## ListBackupSelectionsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_selections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListBackupSelections.html#Backup.Paginator.ListBackupSelections)

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
3. item: `AioPageIterator[ListBackupSelectionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBackupSelectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BackupPlanId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBackupSelectionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBackupSelectionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupSelectionsInputPaginateTypeDef = {  # (1)
    "BackupPlanId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupSelectionsInputPaginateTypeDef](./type_defs.md#listbackupselectionsinputpaginatetypedef)
## ListBackupVaultsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_backup_vaults")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListBackupVaults.html#Backup.Paginator.ListBackupVaults)

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
3. item: `AioPageIterator[ListBackupVaultsOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListBackupVaultsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: VaultTypeType](./literals.md#vaulttypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBackupVaultsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBackupVaultsInputPaginateTypeDef = {  # (1)
    "ByVaultType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupVaultsInputPaginateTypeDef](./type_defs.md#listbackupvaultsinputpaginatetypedef)
## ListCopyJobsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_copy_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListCopyJobs.html#Backup.Paginator.ListCopyJobs)

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
3. item: `AioPageIterator[ListCopyJobsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCopyJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ByResourceArn: str = ...,
    ByState: CopyJobStateType = ...,  # (1)
    ByCreatedBefore: TimestampTypeDef = ...,
    ByCreatedAfter: TimestampTypeDef = ...,
    ByResourceType: str = ...,
    ByDestinationVaultArn: str = ...,
    ByAccountId: str = ...,
    ByCompleteBefore: TimestampTypeDef = ...,
    ByCompleteAfter: TimestampTypeDef = ...,
    ByParentJobId: str = ...,
    ByMessageCategory: str = ...,
    BySourceRecoveryPointArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListCopyJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: CopyJobStateType](./literals.md#copyjobstatetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListCopyJobsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCopyJobsInputPaginateTypeDef = {  # (1)
    "ByResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCopyJobsInputPaginateTypeDef](./type_defs.md#listcopyjobsinputpaginatetypedef)
## ListIndexedRecoveryPointsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_indexed_recovery_points")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListIndexedRecoveryPoints.html#Backup.Paginator.ListIndexedRecoveryPoints)

```python
# ListIndexedRecoveryPointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListIndexedRecoveryPointsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListIndexedRecoveryPointsPaginator = client.get_paginator("list_indexed_recovery_points")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndexedRecoveryPointsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListIndexedRecoveryPointsPaginator](./paginators.md#listindexedrecoverypointspaginator)
3. item: `AioPageIterator[ListIndexedRecoveryPointsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIndexedRecoveryPointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SourceResourceArn: str = ...,
    CreatedBefore: TimestampTypeDef = ...,
    CreatedAfter: TimestampTypeDef = ...,
    ResourceType: str = ...,
    IndexStatus: IndexStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListIndexedRecoveryPointsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListIndexedRecoveryPointsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIndexedRecoveryPointsInputPaginateTypeDef = {  # (1)
    "SourceResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndexedRecoveryPointsInputPaginateTypeDef](./type_defs.md#listindexedrecoverypointsinputpaginatetypedef)
## ListLegalHoldsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_legal_holds")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListLegalHolds.html#Backup.Paginator.ListLegalHolds)

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
3. item: `AioPageIterator[ListLegalHoldsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLegalHoldsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListLegalHoldsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListLegalHoldsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLegalHoldsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLegalHoldsInputPaginateTypeDef](./type_defs.md#listlegalholdsinputpaginatetypedef)
## ListProtectedResourcesByBackupVaultPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_protected_resources_by_backup_vault")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListProtectedResourcesByBackupVault.html#Backup.Paginator.ListProtectedResourcesByBackupVault)

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
3. item: `AioPageIterator[ListProtectedResourcesByBackupVaultOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListProtectedResourcesByBackupVaultOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProtectedResourcesByBackupVaultOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProtectedResourcesByBackupVaultInputPaginateTypeDef = {  # (1)
    "BackupVaultName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectedResourcesByBackupVaultInputPaginateTypeDef](./type_defs.md#listprotectedresourcesbybackupvaultinputpaginatetypedef)
## ListProtectedResourcesPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_protected_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListProtectedResources.html#Backup.Paginator.ListProtectedResources)

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
3. item: `AioPageIterator[ListProtectedResourcesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProtectedResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProtectedResourcesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProtectedResourcesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProtectedResourcesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectedResourcesInputPaginateTypeDef](./type_defs.md#listprotectedresourcesinputpaginatetypedef)
## ListRecoveryPointsByBackupVaultPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_recovery_points_by_backup_vault")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListRecoveryPointsByBackupVault.html#Backup.Paginator.ListRecoveryPointsByBackupVault)

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
3. item: `AioPageIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]`


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
    ByCreatedBefore: TimestampTypeDef = ...,
    ByCreatedAfter: TimestampTypeDef = ...,
    ByParentRecoveryPointArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRecoveryPointsByBackupVaultOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecoveryPointsByBackupVaultInputPaginateTypeDef = {  # (1)
    "BackupVaultName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecoveryPointsByBackupVaultInputPaginateTypeDef](./type_defs.md#listrecoverypointsbybackupvaultinputpaginatetypedef)
## ListRecoveryPointsByLegalHoldPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_recovery_points_by_legal_hold")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListRecoveryPointsByLegalHold.html#Backup.Paginator.ListRecoveryPointsByLegalHold)

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
3. item: `AioPageIterator[ListRecoveryPointsByLegalHoldOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecoveryPointsByLegalHoldPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LegalHoldId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRecoveryPointsByLegalHoldOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRecoveryPointsByLegalHoldOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecoveryPointsByLegalHoldInputPaginateTypeDef = {  # (1)
    "LegalHoldId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecoveryPointsByLegalHoldInputPaginateTypeDef](./type_defs.md#listrecoverypointsbylegalholdinputpaginatetypedef)
## ListRecoveryPointsByResourcePaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_recovery_points_by_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListRecoveryPointsByResource.html#Backup.Paginator.ListRecoveryPointsByResource)

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
3. item: `AioPageIterator[ListRecoveryPointsByResourceOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecoveryPointsByResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    ManagedByAWSBackupOnly: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRecoveryPointsByResourceOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRecoveryPointsByResourceOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecoveryPointsByResourceInputPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecoveryPointsByResourceInputPaginateTypeDef](./type_defs.md#listrecoverypointsbyresourceinputpaginatetypedef)
## ListRestoreAccessBackupVaultsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_restore_access_backup_vaults")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListRestoreAccessBackupVaults.html#Backup.Paginator.ListRestoreAccessBackupVaults)

```python
# ListRestoreAccessBackupVaultsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListRestoreAccessBackupVaultsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListRestoreAccessBackupVaultsPaginator = client.get_paginator("list_restore_access_backup_vaults")  # (2)
    async for item in paginator.paginate(...):
        item: ListRestoreAccessBackupVaultsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListRestoreAccessBackupVaultsPaginator](./paginators.md#listrestoreaccessbackupvaultspaginator)
3. item: `AioPageIterator[ListRestoreAccessBackupVaultsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRestoreAccessBackupVaultsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BackupVaultName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRestoreAccessBackupVaultsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRestoreAccessBackupVaultsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRestoreAccessBackupVaultsInputPaginateTypeDef = {  # (1)
    "BackupVaultName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRestoreAccessBackupVaultsInputPaginateTypeDef](./type_defs.md#listrestoreaccessbackupvaultsinputpaginatetypedef)
## ListRestoreJobsByProtectedResourcePaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_restore_jobs_by_protected_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListRestoreJobsByProtectedResource.html#Backup.Paginator.ListRestoreJobsByProtectedResource)

```python
# ListRestoreJobsByProtectedResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListRestoreJobsByProtectedResourcePaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListRestoreJobsByProtectedResourcePaginator = client.get_paginator("list_restore_jobs_by_protected_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListRestoreJobsByProtectedResourceOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListRestoreJobsByProtectedResourcePaginator](./paginators.md#listrestorejobsbyprotectedresourcepaginator)
3. item: `AioPageIterator[ListRestoreJobsByProtectedResourceOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRestoreJobsByProtectedResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    ByStatus: RestoreJobStatusType = ...,  # (1)
    ByRecoveryPointCreationDateAfter: TimestampTypeDef = ...,
    ByRecoveryPointCreationDateBefore: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRestoreJobsByProtectedResourceOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRestoreJobsByProtectedResourceOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRestoreJobsByProtectedResourceInputPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRestoreJobsByProtectedResourceInputPaginateTypeDef](./type_defs.md#listrestorejobsbyprotectedresourceinputpaginatetypedef)
## ListRestoreJobsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_restore_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListRestoreJobs.html#Backup.Paginator.ListRestoreJobs)

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
3. item: `AioPageIterator[ListRestoreJobsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRestoreJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ByAccountId: str = ...,
    ByResourceType: str = ...,
    ByCreatedBefore: TimestampTypeDef = ...,
    ByCreatedAfter: TimestampTypeDef = ...,
    ByStatus: RestoreJobStatusType = ...,  # (1)
    ByCompleteBefore: TimestampTypeDef = ...,
    ByCompleteAfter: TimestampTypeDef = ...,
    ByRestoreTestingPlanArn: str = ...,
    ByParentJobId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRestoreJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RestoreJobStatusType](./literals.md#restorejobstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRestoreJobsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRestoreJobsInputPaginateTypeDef = {  # (1)
    "ByAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRestoreJobsInputPaginateTypeDef](./type_defs.md#listrestorejobsinputpaginatetypedef)
## ListRestoreTestingPlansPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_restore_testing_plans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListRestoreTestingPlans.html#Backup.Paginator.ListRestoreTestingPlans)

```python
# ListRestoreTestingPlansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListRestoreTestingPlansPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListRestoreTestingPlansPaginator = client.get_paginator("list_restore_testing_plans")  # (2)
    async for item in paginator.paginate(...):
        item: ListRestoreTestingPlansOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListRestoreTestingPlansPaginator](./paginators.md#listrestoretestingplanspaginator)
3. item: `AioPageIterator[ListRestoreTestingPlansOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRestoreTestingPlansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRestoreTestingPlansOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRestoreTestingPlansOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRestoreTestingPlansInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRestoreTestingPlansInputPaginateTypeDef](./type_defs.md#listrestoretestingplansinputpaginatetypedef)
## ListRestoreTestingSelectionsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_restore_testing_selections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListRestoreTestingSelections.html#Backup.Paginator.ListRestoreTestingSelections)

```python
# ListRestoreTestingSelectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListRestoreTestingSelectionsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListRestoreTestingSelectionsPaginator = client.get_paginator("list_restore_testing_selections")  # (2)
    async for item in paginator.paginate(...):
        item: ListRestoreTestingSelectionsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListRestoreTestingSelectionsPaginator](./paginators.md#listrestoretestingselectionspaginator)
3. item: `AioPageIterator[ListRestoreTestingSelectionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRestoreTestingSelectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RestoreTestingPlanName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRestoreTestingSelectionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRestoreTestingSelectionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRestoreTestingSelectionsInputPaginateTypeDef = {  # (1)
    "RestoreTestingPlanName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRestoreTestingSelectionsInputPaginateTypeDef](./type_defs.md#listrestoretestingselectionsinputpaginatetypedef)
## ListScanJobSummariesPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_scan_job_summaries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListScanJobSummaries.html#Backup.Paginator.ListScanJobSummaries)

```python
# ListScanJobSummariesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListScanJobSummariesPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListScanJobSummariesPaginator = client.get_paginator("list_scan_job_summaries")  # (2)
    async for item in paginator.paginate(...):
        item: ListScanJobSummariesOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListScanJobSummariesPaginator](./paginators.md#listscanjobsummariespaginator)
3. item: `AioPageIterator[ListScanJobSummariesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListScanJobSummariesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str = ...,
    ResourceType: str = ...,
    MalwareScanner: MalwareScannerType = ...,  # (1)
    ScanResultStatus: ScanResultStatusType = ...,  # (2)
    State: ScanJobStatusType = ...,  # (3)
    AggregationPeriod: AggregationPeriodType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> aiobotocore.paginate.AioPageIterator[ListScanJobSummariesOutputTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: MalwareScannerType](./literals.md#malwarescannertype)
2. See [:material-code-brackets: ScanResultStatusType](./literals.md#scanresultstatustype)
3. See [:material-code-brackets: ScanJobStatusType](./literals.md#scanjobstatustype)
4. See [:material-code-brackets: AggregationPeriodType](./literals.md#aggregationperiodtype)
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
6. See `AioPageIterator[ListScanJobSummariesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListScanJobSummariesInputPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScanJobSummariesInputPaginateTypeDef](./type_defs.md#listscanjobsummariesinputpaginatetypedef)
## ListScanJobsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_scan_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListScanJobs.html#Backup.Paginator.ListScanJobs)

```python
# ListScanJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListScanJobsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListScanJobsPaginator = client.get_paginator("list_scan_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListScanJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListScanJobsPaginator](./paginators.md#listscanjobspaginator)
3. item: `AioPageIterator[ListScanJobsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListScanJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ByAccountId: str = ...,
    ByBackupVaultName: str = ...,
    ByCompleteAfter: TimestampTypeDef = ...,
    ByCompleteBefore: TimestampTypeDef = ...,
    ByMalwareScanner: MalwareScannerType = ...,  # (1)
    ByRecoveryPointArn: str = ...,
    ByResourceArn: str = ...,
    ByResourceType: ScanResourceTypeType = ...,  # (2)
    ByScanResultStatus: ScanResultStatusType = ...,  # (3)
    ByState: ScanStateType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> aiobotocore.paginate.AioPageIterator[ListScanJobsOutputTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: MalwareScannerType](./literals.md#malwarescannertype)
2. See [:material-code-brackets: ScanResourceTypeType](./literals.md#scanresourcetypetype)
3. See [:material-code-brackets: ScanResultStatusType](./literals.md#scanresultstatustype)
4. See [:material-code-brackets: ScanStateType](./literals.md#scanstatetype)
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
6. See `AioPageIterator[ListScanJobsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListScanJobsInputPaginateTypeDef = {  # (1)
    "ByAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScanJobsInputPaginateTypeDef](./type_defs.md#listscanjobsinputpaginatetypedef)
## ListTieringConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("backup").get_paginator("list_tiering_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup/paginator/ListTieringConfigurations.html#Backup.Paginator.ListTieringConfigurations)

```python
# ListTieringConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backup.paginator import ListTieringConfigurationsPaginator

session = get_session()
async with session.create_client("backup") as client:  # (1)
    paginator: ListTieringConfigurationsPaginator = client.get_paginator("list_tiering_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListTieringConfigurationsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListTieringConfigurationsPaginator](./paginators.md#listtieringconfigurationspaginator)
3. item: `AioPageIterator[ListTieringConfigurationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTieringConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTieringConfigurationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTieringConfigurationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTieringConfigurationsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTieringConfigurationsInputPaginateTypeDef](./type_defs.md#listtieringconfigurationsinputpaginatetypedef)
