# Paginators

> [Index](../README.md) > [LakeFormation](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LakeFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation)
    type annotations stubs module [types-aiobotocore-lakeformation](https://pypi.org/project/types-aiobotocore-lakeformation/).

## GetWorkUnitsPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("get_work_units")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.GetWorkUnits)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import GetWorkUnitsPaginator

session = get_session()
async with session.create_client("lakeformation") as client:
    client: LakeFormationClient
    paginator: GetWorkUnitsPaginator = client.get_paginator("get_work_units")
```


### paginate

Type annotations and code completion for `#!python GetWorkUnitsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    QueryId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetWorkUnitsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetWorkUnitsResponseTypeDef](./type_defs.md#getworkunitsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef = {  # (1)
    "QueryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetWorkUnitsRequestGetWorkUnitsPaginateTypeDef](./type_defs.md#getworkunitsrequestgetworkunitspaginatetypedef) 
## ListDataCellsFilterPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("list_data_cells_filter")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListDataCellsFilter)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import ListDataCellsFilterPaginator

session = get_session()
async with session.create_client("lakeformation") as client:
    client: LakeFormationClient
    paginator: ListDataCellsFilterPaginator = client.get_paginator("list_data_cells_filter")
```


### paginate

Type annotations and code completion for `#!python ListDataCellsFilterPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Table: TableResourceTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDataCellsFilterResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TableResourceTypeDef](./type_defs.md#tableresourcetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDataCellsFilterResponseTypeDef](./type_defs.md#listdatacellsfilterresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef = {  # (1)
    "Table": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataCellsFilterRequestListDataCellsFilterPaginateTypeDef](./type_defs.md#listdatacellsfilterrequestlistdatacellsfilterpaginatetypedef) 
## ListLFTagsPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("list_lf_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.ListLFTags)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import ListLFTagsPaginator

session = get_session()
async with session.create_client("lakeformation") as client:
    client: LakeFormationClient
    paginator: ListLFTagsPaginator = client.get_paginator("list_lf_tags")
```


### paginate

Type annotations and code completion for `#!python ListLFTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CatalogId: str = ...,
    ResourceShareType: ResourceShareTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListLFTagsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLFTagsResponseTypeDef](./type_defs.md#listlftagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListLFTagsRequestListLFTagsPaginateTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLFTagsRequestListLFTagsPaginateTypeDef](./type_defs.md#listlftagsrequestlistlftagspaginatetypedef) 
## SearchDatabasesByLFTagsPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("search_databases_by_lf_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchDatabasesByLFTags)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import SearchDatabasesByLFTagsPaginator

session = get_session()
async with session.create_client("lakeformation") as client:
    client: LakeFormationClient
    paginator: SearchDatabasesByLFTagsPaginator = client.get_paginator("search_databases_by_lf_tags")
```


### paginate

Type annotations and code completion for `#!python SearchDatabasesByLFTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Expression: Sequence[LFTagTypeDef],  # (1)
    CatalogId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SearchDatabasesByLFTagsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchDatabasesByLFTagsResponseTypeDef](./type_defs.md#searchdatabasesbylftagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef = {  # (1)
    "Expression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchDatabasesByLFTagsRequestSearchDatabasesByLFTagsPaginateTypeDef](./type_defs.md#searchdatabasesbylftagsrequestsearchdatabasesbylftagspaginatetypedef) 
## SearchTablesByLFTagsPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("search_tables_by_lf_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#LakeFormation.Paginator.SearchTablesByLFTags)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import SearchTablesByLFTagsPaginator

session = get_session()
async with session.create_client("lakeformation") as client:
    client: LakeFormationClient
    paginator: SearchTablesByLFTagsPaginator = client.get_paginator("search_tables_by_lf_tags")
```


### paginate

Type annotations and code completion for `#!python SearchTablesByLFTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Expression: Sequence[LFTagTypeDef],  # (1)
    CatalogId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SearchTablesByLFTagsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: LFTagTypeDef](./type_defs.md#lftagtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchTablesByLFTagsResponseTypeDef](./type_defs.md#searchtablesbylftagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef = {  # (1)
    "Expression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchTablesByLFTagsRequestSearchTablesByLFTagsPaginateTypeDef](./type_defs.md#searchtablesbylftagsrequestsearchtablesbylftagspaginatetypedef) 
