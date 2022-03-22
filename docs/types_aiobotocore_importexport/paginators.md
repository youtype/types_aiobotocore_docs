<a id="paginators-for-aiobotocore-importexport-module"></a>

# Paginators for aiobotocore ImportExport module

> [Index](../README.md) > [ImportExport](./README.md) > Paginators

Auto-generated documentation for
[ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
type annotations stubs module
[types-aiobotocore-importexport](https://pypi.org/project/types-aiobotocore-importexport/).

- [Paginators for aiobotocore ImportExport module](#paginators-for-aiobotocore-importexport-module)
  - [ListJobsPaginator](#listjobspaginator)

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for
`session.create_client("importexport").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_importexport.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("importexport") as client:
    client: ImportExportClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```

Boto3 documentation:
[ImportExport.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `APIVersion`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`AsyncIterator`\[[ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef)\].
