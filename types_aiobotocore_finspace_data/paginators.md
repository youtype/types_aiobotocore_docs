<a id="paginators-for-aiobotocore-finspacedata-module"></a>

# Paginators for aiobotocore FinSpaceData module

> [Index](..) > [FinSpaceData](.) > Paginators

Auto-generated documentation for
[FinSpaceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
type annotations stubs module
[types-aiobotocore-finspace-data](https://pypi.org/project/types-aiobotocore-finspace-data/).

- [Paginators for aiobotocore FinSpaceData module](#paginators-for-aiobotocore-finspacedata-module)
  - [ListChangesetsPaginator](#listchangesetspaginator)
  - [ListDataViewsPaginator](#listdataviewspaginator)
  - [ListDatasetsPaginator](#listdatasetspaginator)

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
`AsyncIterable`\[[ListChangesetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef)\].

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
`AsyncIterable`\[[ListDataViewsResponseTypeDef](./type_defs.md#listdataviewsresponsetypedef)\].

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
`AsyncIterable`\[[ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)\].
