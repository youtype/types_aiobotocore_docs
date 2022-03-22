<a id="paginators-for-aiobotocore-glacier-module"></a>

# Paginators for aiobotocore Glacier module

> [Index](../README.md) > [Glacier](./README.md) > Paginators

Auto-generated documentation for
[Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
type annotations stubs module
[types-aiobotocore-glacier](https://pypi.org/project/types-aiobotocore-glacier/).

- [Paginators for aiobotocore Glacier module](#paginators-for-aiobotocore-glacier-module)
  - [ListJobsPaginator](#listjobspaginator)
  - [ListMultipartUploadsPaginator](#listmultipartuploadspaginator)
  - [ListPartsPaginator](#listpartspaginator)
  - [ListVaultsPaginator](#listvaultspaginator)

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for
`session.create_client("glacier").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glacier.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("glacier") as client:
    client: GlacierClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```

Boto3 documentation:
[Glacier.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `accountId`: `str` *(required)*
- `vaultName`: `str` *(required)*
- `statuscode`: `str`
- `completed`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`AsyncIterator`\[[ListJobsOutputTypeDef](./type_defs.md#listjobsoutputtypedef)\].

<a id="listmultipartuploadspaginator"></a>

## ListMultipartUploadsPaginator

Type annotations for
`session.create_client("glacier").get_paginator("list_multipart_uploads")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glacier.paginator import ListMultipartUploadsPaginator

session = get_session()
async with session.create_client("glacier") as client:
    client: GlacierClient
    paginator: ListMultipartUploadsPaginator = client.get_paginator("list_multipart_uploads")
```

Boto3 documentation:
[Glacier.Paginator.ListMultipartUploads](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListMultipartUploads)

Arguments for `ListMultipartUploadsPaginator.paginate` method:

- `accountId`: `str` *(required)*
- `vaultName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMultipartUploadsPaginator.paginate` returns
`AsyncIterator`\[[ListMultipartUploadsOutputTypeDef](./type_defs.md#listmultipartuploadsoutputtypedef)\].

<a id="listpartspaginator"></a>

## ListPartsPaginator

Type annotations for
`session.create_client("glacier").get_paginator("list_parts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glacier.paginator import ListPartsPaginator

session = get_session()
async with session.create_client("glacier") as client:
    client: GlacierClient
    paginator: ListPartsPaginator = client.get_paginator("list_parts")
```

Boto3 documentation:
[Glacier.Paginator.ListParts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListParts)

Arguments for `ListPartsPaginator.paginate` method:

- `accountId`: `str` *(required)*
- `vaultName`: `str` *(required)*
- `uploadId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPartsPaginator.paginate` returns
`AsyncIterator`\[[ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef)\].

<a id="listvaultspaginator"></a>

## ListVaultsPaginator

Type annotations for
`session.create_client("glacier").get_paginator("list_vaults")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_glacier.paginator import ListVaultsPaginator

session = get_session()
async with session.create_client("glacier") as client:
    client: GlacierClient
    paginator: ListVaultsPaginator = client.get_paginator("list_vaults")
```

Boto3 documentation:
[Glacier.Paginator.ListVaults](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListVaults)

Arguments for `ListVaultsPaginator.paginate` method:

- `accountId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListVaultsPaginator.paginate` returns
`AsyncIterator`\[[ListVaultsOutputTypeDef](./type_defs.md#listvaultsoutputtypedef)\].
