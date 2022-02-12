<a id="paginators-for-aiobotocore-efs-module"></a>

# Paginators for aiobotocore EFS module

> [Index](..) > [EFS](.) > Paginators

Auto-generated documentation for
[EFS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
type annotations stubs module
[types-aiobotocore-efs](https://pypi.org/project/types-aiobotocore-efs/).

- [Paginators for aiobotocore EFS module](#paginators-for-aiobotocore-efs-module)
  - [DescribeFileSystemsPaginator](#describefilesystemspaginator)
  - [DescribeMountTargetsPaginator](#describemounttargetspaginator)
  - [DescribeTagsPaginator](#describetagspaginator)

<a id="describefilesystemspaginator"></a>

## DescribeFileSystemsPaginator

Type annotations for
`session.create_client("efs").get_paginator("describe_file_systems")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_efs.paginator import DescribeFileSystemsPaginator

session = get_session()
async with session.create_client("efs") as client:
    client: EFSClient
    paginator: DescribeFileSystemsPaginator = client.get_paginator("describe_file_systems")
```

Boto3 documentation:
[EFS.Paginator.DescribeFileSystems](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems)

Arguments for `DescribeFileSystemsPaginator.paginate` method:

- `CreationToken`: `str`
- `FileSystemId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeFileSystemsPaginator.paginate` returns
`AsyncIterable`\[[DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef)\].

<a id="describemounttargetspaginator"></a>

## DescribeMountTargetsPaginator

Type annotations for
`session.create_client("efs").get_paginator("describe_mount_targets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_efs.paginator import DescribeMountTargetsPaginator

session = get_session()
async with session.create_client("efs") as client:
    client: EFSClient
    paginator: DescribeMountTargetsPaginator = client.get_paginator("describe_mount_targets")
```

Boto3 documentation:
[EFS.Paginator.DescribeMountTargets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets)

Arguments for `DescribeMountTargetsPaginator.paginate` method:

- `FileSystemId`: `str`
- `MountTargetId`: `str`
- `AccessPointId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeMountTargetsPaginator.paginate` returns
`AsyncIterable`\[[DescribeMountTargetsResponseTypeDef](./type_defs.md#describemounttargetsresponsetypedef)\].

<a id="describetagspaginator"></a>

## DescribeTagsPaginator

Type annotations for
`session.create_client("efs").get_paginator("describe_tags")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_efs.paginator import DescribeTagsPaginator

session = get_session()
async with session.create_client("efs") as client:
    client: EFSClient
    paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
```

Boto3 documentation:
[EFS.Paginator.DescribeTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags)

Arguments for `DescribeTagsPaginator.paginate` method:

- `FileSystemId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeTagsPaginator.paginate` returns
`AsyncIterable`\[[DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef)\].
