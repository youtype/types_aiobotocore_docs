<a id="paginators-for-aiobotocore-lakeformation-module"></a>

# Paginators for aiobotocore LakeFormation module

> [Index](..) > [LakeFormation](.) > Paginators

Auto-generated documentation for
[LakeFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
type annotations stubs module
[types-aiobotocore-lakeformation](https://pypi.org/project/types-aiobotocore-lakeformation/).

- [Paginators for aiobotocore LakeFormation module](#paginators-for-aiobotocore-lakeformation-module)
  - [GetWorkUnitsPaginator](#getworkunitspaginator)
  - [ListDataCellsFilterPaginator](#listdatacellsfilterpaginator)
  - [ListLFTagsPaginator](#listlftagspaginator)
  - [SearchDatabasesByLFTagsPaginator](#searchdatabasesbylftagspaginator)
  - [SearchTablesByLFTagsPaginator](#searchtablesbylftagspaginator)

<a id="getworkunitspaginator"></a>

## GetWorkUnitsPaginator

Type annotations for
`aiobotocore.create_client("lakeformation").get_paginator("get_work_units")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_lakeformation.paginator import GetWorkUnitsPaginator

def get_get_work_units_paginator() -> GetWorkUnitsPaginator:
    return Session().create_client("lakeformation").get_paginator("get_work_units")
```

Boto3 documentation:
[LakeFormation.Paginator.GetWorkUnits](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)

Arguments for `GetWorkUnitsPaginator.paginate` method:

- `QueryId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetWorkUnitsPaginator.paginate` returns
`_PageIterator`\[[GetWorkUnitsResponseTypeDef](./type_defs.md#getworkunitsresponsetypedef)\].

<a id="listdatacellsfilterpaginator"></a>

## ListDataCellsFilterPaginator

Type annotations for
`aiobotocore.create_client("lakeformation").get_paginator("list_data_cells_filter")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_lakeformation.paginator import ListDataCellsFilterPaginator

def get_list_data_cells_filter_paginator() -> ListDataCellsFilterPaginator:
    return Session().create_client("lakeformation").get_paginator("list_data_cells_filter")
```

Boto3 documentation:
[LakeFormation.Paginator.ListDataCellsFilter](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)

Arguments for `ListDataCellsFilterPaginator.paginate` method:

- `Table`: [TableResourceTypeDef](./type_defs.md#tableresourcetypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDataCellsFilterPaginator.paginate` returns
`_PageIterator`\[[ListDataCellsFilterResponseTypeDef](./type_defs.md#listdatacellsfilterresponsetypedef)\].

<a id="listlftagspaginator"></a>

## ListLFTagsPaginator

Type annotations for
`aiobotocore.create_client("lakeformation").get_paginator("list_lf_tags")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_lakeformation.paginator import ListLFTagsPaginator

def get_list_lf_tags_paginator() -> ListLFTagsPaginator:
    return Session().create_client("lakeformation").get_paginator("list_lf_tags")
```

Boto3 documentation:
[LakeFormation.Paginator.ListLFTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags)

Arguments for `ListLFTagsPaginator.paginate` method:

- `CatalogId`: `str`
- `ResourceShareType`:
  [ResourceShareTypeType](./literals.md#resourcesharetypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLFTagsPaginator.paginate` returns
`_PageIterator`\[[ListLFTagsResponseTypeDef](./type_defs.md#listlftagsresponsetypedef)\].

<a id="searchdatabasesbylftagspaginator"></a>

## SearchDatabasesByLFTagsPaginator

Type annotations for
`aiobotocore.create_client("lakeformation").get_paginator("search_databases_by_lf_tags")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_lakeformation.paginator import SearchDatabasesByLFTagsPaginator

def get_search_databases_by_lf_tags_paginator() -> SearchDatabasesByLFTagsPaginator:
    return Session().create_client("lakeformation").get_paginator("search_databases_by_lf_tags")
```

Boto3 documentation:
[LakeFormation.Paginator.SearchDatabasesByLFTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)

Arguments for `SearchDatabasesByLFTagsPaginator.paginate` method:

- `Expression`: `Sequence`\[[LFTagTypeDef](./type_defs.md#lftagtypedef)\]
  *(required)*
- `CatalogId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchDatabasesByLFTagsPaginator.paginate` returns
`_PageIterator`\[[SearchDatabasesByLFTagsResponseTypeDef](./type_defs.md#searchdatabasesbylftagsresponsetypedef)\].

<a id="searchtablesbylftagspaginator"></a>

## SearchTablesByLFTagsPaginator

Type annotations for
`aiobotocore.create_client("lakeformation").get_paginator("search_tables_by_lf_tags")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_lakeformation.paginator import SearchTablesByLFTagsPaginator

def get_search_tables_by_lf_tags_paginator() -> SearchTablesByLFTagsPaginator:
    return Session().create_client("lakeformation").get_paginator("search_tables_by_lf_tags")
```

Boto3 documentation:
[LakeFormation.Paginator.SearchTablesByLFTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)

Arguments for `SearchTablesByLFTagsPaginator.paginate` method:

- `Expression`: `Sequence`\[[LFTagTypeDef](./type_defs.md#lftagtypedef)\]
  *(required)*
- `CatalogId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchTablesByLFTagsPaginator.paginate` returns
`_PageIterator`\[[SearchTablesByLFTagsResponseTypeDef](./type_defs.md#searchtablesbylftagsresponsetypedef)\].
