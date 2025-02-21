# Examples

> [Index](../README.md) > [BackupSearch](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BackupSearch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupsearch.html#backupsearch)
    type annotations stubs module [types-aiobotocore-backupsearch](https://pypi.org/project/types-aiobotocore-backupsearch/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[backupsearch]` package installed.

Write your `BackupSearch` code as usual,
type checking and code completion should work out of the box.



```python
# BackupSearchClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("backupsearch") as client:  # (1)
    result = await client.get_search_job()  # (2)
```

1. client: [BackupSearchClient](./client.md)
2. result: [:material-code-braces: GetSearchJobOutputTypeDef](./type_defs.md#getsearchjoboutputtypedef) 



```python
# ListSearchJobBackupsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("backupsearch") as client:  # (1)
    paginator = client.get_paginator("list_search_job_backups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BackupSearchClient](./client.md)
2. paginator: [ListSearchJobBackupsPaginator](./paginators.md#listsearchjobbackupspaginator)
3. item: [:material-code-braces: ListSearchJobBackupsOutputTypeDef](./type_defs.md#listsearchjobbackupsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[backupsearch]`
or a standalone `types_aiobotocore_backupsearch` package, you have to explicitly specify
`client: BackupSearchClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# BackupSearchClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_backupsearch.client import BackupSearchClient
from types_aiobotocore_backupsearch.type_defs import GetSearchJobOutputTypeDef
from types_aiobotocore_backupsearch.type_defs import GetSearchJobInputTypeDef


session = get_session()

async with session.create_client("backupsearch") as client:
    client: BackupSearchClient
    kwargs: GetSearchJobInputTypeDef = {...}
    result: GetSearchJobOutputTypeDef = await client.get_search_job(**kwargs)
```



```python
# ListSearchJobBackupsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_backupsearch.client import BackupSearchClient
from types_aiobotocore_backupsearch.paginator import ListSearchJobBackupsPaginator
from types_aiobotocore_backupsearch.type_defs import ListSearchJobBackupsOutputTypeDef


session = get_session()

async with session.create_client("backupsearch") as client:
    client: BackupSearchClient
    paginator: ListSearchJobBackupsPaginator = client.get_paginator("list_search_job_backups")
    async for item in paginator.paginate(...):
        item: ListSearchJobBackupsOutputTypeDef
        print(item)
```


