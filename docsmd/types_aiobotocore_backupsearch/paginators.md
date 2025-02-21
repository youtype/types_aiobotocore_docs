# Paginators

> [Index](../README.md) > [BackupSearch](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [BackupSearch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupsearch.html#backupsearch)
    type annotations stubs module [types-aiobotocore-backupsearch](https://pypi.org/project/types-aiobotocore-backupsearch/).

## ListSearchJobBackupsPaginator

Type annotations and code completion for `#!python session.create_client("backupsearch").get_paginator("list_search_job_backups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupsearch/paginator/ListSearchJobBackups.html#BackupSearch.Paginator.ListSearchJobBackups)

```python
# ListSearchJobBackupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backupsearch.paginator import ListSearchJobBackupsPaginator

session = get_session()
async with session.create_client("backupsearch") as client:  # (1)
    paginator: ListSearchJobBackupsPaginator = client.get_paginator("list_search_job_backups")  # (2)
    async for item in paginator.paginate(...):
        item: ListSearchJobBackupsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupSearchClient](./client.md)
2. paginator: [ListSearchJobBackupsPaginator](./paginators.md#listsearchjobbackupspaginator)
3. item: [:material-code-braces: ListSearchJobBackupsOutputTypeDef](./type_defs.md#listsearchjobbackupsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSearchJobBackupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SearchJobIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSearchJobBackupsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSearchJobBackupsOutputTypeDef](./type_defs.md#listsearchjobbackupsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSearchJobBackupsInputPaginateTypeDef = {  # (1)
    "SearchJobIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSearchJobBackupsInputPaginateTypeDef](./type_defs.md#listsearchjobbackupsinputpaginatetypedef) 
## ListSearchJobResultsPaginator

Type annotations and code completion for `#!python session.create_client("backupsearch").get_paginator("list_search_job_results")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupsearch/paginator/ListSearchJobResults.html#BackupSearch.Paginator.ListSearchJobResults)

```python
# ListSearchJobResultsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backupsearch.paginator import ListSearchJobResultsPaginator

session = get_session()
async with session.create_client("backupsearch") as client:  # (1)
    paginator: ListSearchJobResultsPaginator = client.get_paginator("list_search_job_results")  # (2)
    async for item in paginator.paginate(...):
        item: ListSearchJobResultsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupSearchClient](./client.md)
2. paginator: [ListSearchJobResultsPaginator](./paginators.md#listsearchjobresultspaginator)
3. item: [:material-code-braces: ListSearchJobResultsOutputTypeDef](./type_defs.md#listsearchjobresultsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSearchJobResultsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SearchJobIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSearchJobResultsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSearchJobResultsOutputTypeDef](./type_defs.md#listsearchjobresultsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSearchJobResultsInputPaginateTypeDef = {  # (1)
    "SearchJobIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSearchJobResultsInputPaginateTypeDef](./type_defs.md#listsearchjobresultsinputpaginatetypedef) 
## ListSearchJobsPaginator

Type annotations and code completion for `#!python session.create_client("backupsearch").get_paginator("list_search_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupsearch/paginator/ListSearchJobs.html#BackupSearch.Paginator.ListSearchJobs)

```python
# ListSearchJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backupsearch.paginator import ListSearchJobsPaginator

session = get_session()
async with session.create_client("backupsearch") as client:  # (1)
    paginator: ListSearchJobsPaginator = client.get_paginator("list_search_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListSearchJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupSearchClient](./client.md)
2. paginator: [ListSearchJobsPaginator](./paginators.md#listsearchjobspaginator)
3. item: [:material-code-braces: ListSearchJobsOutputTypeDef](./type_defs.md#listsearchjobsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSearchJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ByStatus: SearchJobStateType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSearchJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SearchJobStateType](./literals.md#searchjobstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSearchJobsOutputTypeDef](./type_defs.md#listsearchjobsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSearchJobsInputPaginateTypeDef = {  # (1)
    "ByStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSearchJobsInputPaginateTypeDef](./type_defs.md#listsearchjobsinputpaginatetypedef) 
## ListSearchResultExportJobsPaginator

Type annotations and code completion for `#!python session.create_client("backupsearch").get_paginator("list_search_result_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupsearch/paginator/ListSearchResultExportJobs.html#BackupSearch.Paginator.ListSearchResultExportJobs)

```python
# ListSearchResultExportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_backupsearch.paginator import ListSearchResultExportJobsPaginator

session = get_session()
async with session.create_client("backupsearch") as client:  # (1)
    paginator: ListSearchResultExportJobsPaginator = client.get_paginator("list_search_result_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListSearchResultExportJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupSearchClient](./client.md)
2. paginator: [ListSearchResultExportJobsPaginator](./paginators.md#listsearchresultexportjobspaginator)
3. item: [:material-code-braces: ListSearchResultExportJobsOutputTypeDef](./type_defs.md#listsearchresultexportjobsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSearchResultExportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Status: ExportJobStatusType = ...,  # (1)
    SearchJobIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSearchResultExportJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ExportJobStatusType](./literals.md#exportjobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSearchResultExportJobsOutputTypeDef](./type_defs.md#listsearchresultexportjobsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSearchResultExportJobsInputPaginateTypeDef = {  # (1)
    "Status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSearchResultExportJobsInputPaginateTypeDef](./type_defs.md#listsearchresultexportjobsinputpaginatetypedef) 
