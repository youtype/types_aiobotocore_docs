<a id="paginators-for-aiobotocore-kinesisanalyticsv2-module"></a>

# Paginators for aiobotocore KinesisAnalyticsV2 module

> [Index](..) > [KinesisAnalyticsV2](.) > Paginators

Auto-generated documentation for
[KinesisAnalyticsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
type annotations stubs module
[types-aiobotocore-kinesisanalyticsv2](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2/).

- [Paginators for aiobotocore KinesisAnalyticsV2 module](#paginators-for-aiobotocore-kinesisanalyticsv2-module)
  - [ListApplicationSnapshotsPaginator](#listapplicationsnapshotspaginator)
  - [ListApplicationsPaginator](#listapplicationspaginator)

<a id="listapplicationsnapshotspaginator"></a>

## ListApplicationSnapshotsPaginator

Type annotations for
`aiobotocore.create_client("kinesisanalyticsv2").get_paginator("list_application_snapshots")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_kinesisanalyticsv2.paginator import ListApplicationSnapshotsPaginator

def get_list_application_snapshots_paginator() -> ListApplicationSnapshotsPaginator:
    return Session().create_client("kinesisanalyticsv2").get_paginator("list_application_snapshots")
```

Boto3 documentation:
[KinesisAnalyticsV2.Paginator.ListApplicationSnapshots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplicationSnapshots)

Arguments for `ListApplicationSnapshotsPaginator.paginate` method:

- `ApplicationName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationSnapshotsPaginator.paginate` returns
`_PageIterator`\[[ListApplicationSnapshotsResponseTypeDef](./type_defs.md#listapplicationsnapshotsresponsetypedef)\].

<a id="listapplicationspaginator"></a>

## ListApplicationsPaginator

Type annotations for
`aiobotocore.create_client("kinesisanalyticsv2").get_paginator("list_applications")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_kinesisanalyticsv2.paginator import ListApplicationsPaginator

def get_list_applications_paginator() -> ListApplicationsPaginator:
    return Session().create_client("kinesisanalyticsv2").get_paginator("list_applications")
```

Boto3 documentation:
[KinesisAnalyticsV2.Paginator.ListApplications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Paginator.ListApplications)

Arguments for `ListApplicationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationsPaginator.paginate` returns
`_PageIterator`\[[ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)\].
