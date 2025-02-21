# Examples

> [Index](../README.md) > [Backup](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#backup)
    type annotations stubs module [types-aiobotocore-backup](https://pypi.org/project/types-aiobotocore-backup/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[backup]` package installed.

Write your `Backup` code as usual,
type checking and code completion should work out of the box.



```python
# BackupClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("backup") as client:  # (1)
    result = await client.create_backup_plan()  # (2)
```

1. client: [BackupClient](./client.md)
2. result: [:material-code-braces: CreateBackupPlanOutputTypeDef](./type_defs.md#createbackupplanoutputtypedef) 



```python
# ListBackupJobsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("backup") as client:  # (1)
    paginator = client.get_paginator("list_backup_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BackupClient](./client.md)
2. paginator: [ListBackupJobsPaginator](./paginators.md#listbackupjobspaginator)
3. item: [:material-code-braces: ListBackupJobsOutputTypeDef](./type_defs.md#listbackupjobsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[backup]`
or a standalone `types_aiobotocore_backup` package, you have to explicitly specify
`client: BackupClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# BackupClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_backup.client import BackupClient
from types_aiobotocore_backup.type_defs import CreateBackupPlanOutputTypeDef
from types_aiobotocore_backup.type_defs import CreateBackupPlanInputTypeDef


session = get_session()

async with session.create_client("backup") as client:
    client: BackupClient
    kwargs: CreateBackupPlanInputTypeDef = {...}
    result: CreateBackupPlanOutputTypeDef = await client.create_backup_plan(**kwargs)
```



```python
# ListBackupJobsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_backup.client import BackupClient
from types_aiobotocore_backup.paginator import ListBackupJobsPaginator
from types_aiobotocore_backup.type_defs import ListBackupJobsOutputTypeDef


session = get_session()

async with session.create_client("backup") as client:
    client: BackupClient
    paginator: ListBackupJobsPaginator = client.get_paginator("list_backup_jobs")
    async for item in paginator.paginate(...):
        item: ListBackupJobsOutputTypeDef
        print(item)
```


