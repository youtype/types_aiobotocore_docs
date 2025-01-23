# Paginators

> [Index](../README.md) > [ImportExport](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#importexport)
    type annotations stubs module [types-aiobotocore-importexport](https://pypi.org/project/types-aiobotocore-importexport/).

## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("importexport").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport/paginator/ListJobs.html#ImportExport.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_importexport.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("importexport") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [ImportExportClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    APIVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListJobsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsInputPaginateTypeDef = {  # (1)
    "APIVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsInputPaginateTypeDef](./type_defs.md#listjobsinputpaginatetypedef) 
