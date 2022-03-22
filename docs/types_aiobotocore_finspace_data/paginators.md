<a id="paginators-for-aiobotocore-finspacedata-module"></a>

# Paginators for aiobotocore FinSpaceData module

> [Index](../README.md) > [FinSpaceData](./README.md) > Paginators

Auto-generated documentation for
[FinSpaceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
type annotations stubs module
[types-aiobotocore-finspace-data](https://pypi.org/project/types-aiobotocore-finspace-data/).

- [Paginators for aiobotocore FinSpaceData module](#paginators-for-aiobotocore-finspacedata-module)
  - [ListChangesetsPaginator](#listchangesetspaginator)
  - [ListDataViewsPaginator](#listdataviewspaginator)
  - [ListDatasetsPaginator](#listdatasetspaginator)
  - [ListPermissionGroupsPaginator](#listpermissiongroupspaginator)
  - [ListUsersPaginator](#listuserspaginator)

<a id="listchangesetspaginator"></a>

## ListChangesetsPaginator

Type annotations for
`session.create_client("finspace-data").get_paginator("list_changesets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.paginator import ListChangesetsPaginator

session = get_session()
async with session.create_client("finspace-data") as client:
    client: FinSpaceDataClient
    paginator: ListChangesetsPaginator = client.get_paginator("list_changesets")
```

Boto3 documentation:
[FinSpaceData.Paginator.ListChangesets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListChangesets)

Arguments for `ListChangesetsPaginator.paginate` method:

- `datasetId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListChangesetsPaginator.paginate` returns
`AsyncIterator`\[[ListChangesetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef)\].

<a id="listdataviewspaginator"></a>

## ListDataViewsPaginator

Type annotations for
`session.create_client("finspace-data").get_paginator("list_data_views")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.paginator import ListDataViewsPaginator

session = get_session()
async with session.create_client("finspace-data") as client:
    client: FinSpaceDataClient
    paginator: ListDataViewsPaginator = client.get_paginator("list_data_views")
```

Boto3 documentation:
[FinSpaceData.Paginator.ListDataViews](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDataViews)

Arguments for `ListDataViewsPaginator.paginate` method:

- `datasetId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDataViewsPaginator.paginate` returns
`AsyncIterator`\[[ListDataViewsResponseTypeDef](./type_defs.md#listdataviewsresponsetypedef)\].

<a id="listdatasetspaginator"></a>

## ListDatasetsPaginator

Type annotations for
`session.create_client("finspace-data").get_paginator("list_datasets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("finspace-data") as client:
    client: FinSpaceDataClient
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
```

Boto3 documentation:
[FinSpaceData.Paginator.ListDatasets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDatasets)

Arguments for `ListDatasetsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetsPaginator.paginate` returns
`AsyncIterator`\[[ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)\].

<a id="listpermissiongroupspaginator"></a>

## ListPermissionGroupsPaginator

Type annotations for
`session.create_client("finspace-data").get_paginator("list_permission_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.paginator import ListPermissionGroupsPaginator

session = get_session()
async with session.create_client("finspace-data") as client:
    client: FinSpaceDataClient
    paginator: ListPermissionGroupsPaginator = client.get_paginator("list_permission_groups")
```

Boto3 documentation:
[FinSpaceData.Paginator.ListPermissionGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListPermissionGroups)

Arguments for `ListPermissionGroupsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPermissionGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListPermissionGroupsResponseTypeDef](./type_defs.md#listpermissiongroupsresponsetypedef)\].

<a id="listuserspaginator"></a>

## ListUsersPaginator

Type annotations for
`session.create_client("finspace-data").get_paginator("list_users")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_finspace_data.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("finspace-data") as client:
    client: FinSpaceDataClient
    paginator: ListUsersPaginator = client.get_paginator("list_users")
```

Boto3 documentation:
[FinSpaceData.Paginator.ListUsers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListUsers)

Arguments for `ListUsersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUsersPaginator.paginate` returns
`AsyncIterator`\[[ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)\].
