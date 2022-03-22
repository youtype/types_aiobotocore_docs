<a id="paginators-for-aiobotocore-fsx-module"></a>

# Paginators for aiobotocore FSx module

> [Index](../README.md) > [FSx](./README.md) > Paginators

Auto-generated documentation for
[FSx](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
type annotations stubs module
[types-aiobotocore-fsx](https://pypi.org/project/types-aiobotocore-fsx/).

- [Paginators for aiobotocore FSx module](#paginators-for-aiobotocore-fsx-module)
  - [DescribeBackupsPaginator](#describebackupspaginator)
  - [DescribeFileSystemsPaginator](#describefilesystemspaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)

<a id="describebackupspaginator"></a>

## DescribeBackupsPaginator

Type annotations for
`session.create_client("fsx").get_paginator("describe_backups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_fsx.paginator import DescribeBackupsPaginator

session = get_session()
async with session.create_client("fsx") as client:
    client: FSxClient
    paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")
```

Boto3 documentation:
[FSx.Paginator.DescribeBackups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups)

Arguments for `DescribeBackupsPaginator.paginate` method:

- `BackupIds`: `Sequence`\[`str`\]
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeBackupsPaginator.paginate` returns
`AsyncIterator`\[[DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef)\].

<a id="describefilesystemspaginator"></a>

## DescribeFileSystemsPaginator

Type annotations for
`session.create_client("fsx").get_paginator("describe_file_systems")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_fsx.paginator import DescribeFileSystemsPaginator

session = get_session()
async with session.create_client("fsx") as client:
    client: FSxClient
    paginator: DescribeFileSystemsPaginator = client.get_paginator("describe_file_systems")
```

Boto3 documentation:
[FSx.Paginator.DescribeFileSystems](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems)

Arguments for `DescribeFileSystemsPaginator.paginate` method:

- `FileSystemIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeFileSystemsPaginator.paginate` returns
`AsyncIterator`\[[DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("fsx").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_fsx.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("fsx") as client:
    client: FSxClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[FSx.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `ResourceARN`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterator`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].
