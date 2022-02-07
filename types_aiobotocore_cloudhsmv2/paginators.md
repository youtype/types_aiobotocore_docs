<a id="paginators-for-aiobotocore-cloudhsmv2-module"></a>

# Paginators for aiobotocore CloudHSMV2 module

> [Index](..) > [CloudHSMV2](.) > Paginators

Auto-generated documentation for
[CloudHSMV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
type annotations stubs module
[types-aiobotocore-cloudhsmv2](https://pypi.org/project/types-aiobotocore-cloudhsmv2/).

- [Paginators for aiobotocore CloudHSMV2 module](#paginators-for-aiobotocore-cloudhsmv2-module)
  - [DescribeBackupsPaginator](#describebackupspaginator)
  - [DescribeClustersPaginator](#describeclusterspaginator)
  - [ListTagsPaginator](#listtagspaginator)

<a id="describebackupspaginator"></a>

## DescribeBackupsPaginator

Type annotations for
`session.create_client("cloudhsmv2").get_paginator("describe_backups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudhsmv2.paginator import DescribeBackupsPaginator

session = get_session()
async with session.create_client("cloudhsmv2") as client:
    client: CloudHSMV2Client
    paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")
```

Boto3 documentation:
[CloudHSMV2.Paginator.DescribeBackups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeBackups)

Arguments for `DescribeBackupsPaginator.paginate` method:

- `Filters`: `Mapping`\[`str`, `Sequence`\[`str`\]\]
- `SortAscending`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeBackupsPaginator.paginate` returns
`_PageIterator`\[[DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef)\].

<a id="describeclusterspaginator"></a>

## DescribeClustersPaginator

Type annotations for
`session.create_client("cloudhsmv2").get_paginator("describe_clusters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudhsmv2.paginator import DescribeClustersPaginator

session = get_session()
async with session.create_client("cloudhsmv2") as client:
    client: CloudHSMV2Client
    paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
```

Boto3 documentation:
[CloudHSMV2.Paginator.DescribeClusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeClusters)

Arguments for `DescribeClustersPaginator.paginate` method:

- `Filters`: `Mapping`\[`str`, `Sequence`\[`str`\]\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeClustersPaginator.paginate` returns
`_PageIterator`\[[DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef)\].

<a id="listtagspaginator"></a>

## ListTagsPaginator

Type annotations for
`session.create_client("cloudhsmv2").get_paginator("list_tags")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudhsmv2.paginator import ListTagsPaginator

session = get_session()
async with session.create_client("cloudhsmv2") as client:
    client: CloudHSMV2Client
    paginator: ListTagsPaginator = client.get_paginator("list_tags")
```

Boto3 documentation:
[CloudHSMV2.Paginator.ListTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.ListTags)

Arguments for `ListTagsPaginator.paginate` method:

- `ResourceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsPaginator.paginate` returns
`_PageIterator`\[[ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)\].
