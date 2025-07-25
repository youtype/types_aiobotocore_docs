# Paginators

> [Index](../README.md) > [LakeFormation](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LakeFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#lakeformation)
    type annotations stubs module [types-aiobotocore-lakeformation](https://pypi.org/project/types-aiobotocore-lakeformation/).

## GetWorkUnitsPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("get_work_units")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation/paginator/GetWorkUnits.html#LakeFormation.Paginator.GetWorkUnits)

```python
# GetWorkUnitsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import GetWorkUnitsPaginator

session = get_session()
async with session.create_client("lakeformation") as client:  # (1)
    paginator: GetWorkUnitsPaginator = client.get_paginator("get_work_units")  # (2)
    async for item in paginator.paginate(...):
        item: GetWorkUnitsResponseTypeDef
        print(item)  # (3)
```

1. client: [LakeFormationClient](./client.md)
2. paginator: [GetWorkUnitsPaginator](./paginators.md#getworkunitspaginator)
3. item: `AioPageIterator[GetWorkUnitsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetWorkUnitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    QueryId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetWorkUnitsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetWorkUnitsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetWorkUnitsRequestPaginateTypeDef = {  # (1)
    "QueryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetWorkUnitsRequestPaginateTypeDef](./type_defs.md#getworkunitsrequestpaginatetypedef)
## ListDataCellsFilterPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("list_data_cells_filter")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation/paginator/ListDataCellsFilter.html#LakeFormation.Paginator.ListDataCellsFilter)

```python
# ListDataCellsFilterPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import ListDataCellsFilterPaginator

session = get_session()
async with session.create_client("lakeformation") as client:  # (1)
    paginator: ListDataCellsFilterPaginator = client.get_paginator("list_data_cells_filter")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataCellsFilterResponseTypeDef
        print(item)  # (3)
```

1. client: [LakeFormationClient](./client.md)
2. paginator: [ListDataCellsFilterPaginator](./paginators.md#listdatacellsfilterpaginator)
3. item: `AioPageIterator[ListDataCellsFilterResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataCellsFilterPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Table: TableResourceUnionTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDataCellsFilterResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TableResourceUnionTypeDef](#tableresourceuniontypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDataCellsFilterResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataCellsFilterRequestPaginateTypeDef = {  # (1)
    "Table": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataCellsFilterRequestPaginateTypeDef](./type_defs.md#listdatacellsfilterrequestpaginatetypedef)
## ListLFTagExpressionsPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("list_lf_tag_expressions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation/paginator/ListLFTagExpressions.html#LakeFormation.Paginator.ListLFTagExpressions)

```python
# ListLFTagExpressionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import ListLFTagExpressionsPaginator

session = get_session()
async with session.create_client("lakeformation") as client:  # (1)
    paginator: ListLFTagExpressionsPaginator = client.get_paginator("list_lf_tag_expressions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLFTagExpressionsResponseTypeDef
        print(item)  # (3)
```

1. client: [LakeFormationClient](./client.md)
2. paginator: [ListLFTagExpressionsPaginator](./paginators.md#listlftagexpressionspaginator)
3. item: `AioPageIterator[ListLFTagExpressionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLFTagExpressionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CatalogId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListLFTagExpressionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListLFTagExpressionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLFTagExpressionsRequestPaginateTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLFTagExpressionsRequestPaginateTypeDef](./type_defs.md#listlftagexpressionsrequestpaginatetypedef)
## ListLFTagsPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("list_lf_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation/paginator/ListLFTags.html#LakeFormation.Paginator.ListLFTags)

```python
# ListLFTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import ListLFTagsPaginator

session = get_session()
async with session.create_client("lakeformation") as client:  # (1)
    paginator: ListLFTagsPaginator = client.get_paginator("list_lf_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListLFTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [LakeFormationClient](./client.md)
2. paginator: [ListLFTagsPaginator](./paginators.md#listlftagspaginator)
3. item: `AioPageIterator[ListLFTagsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListLFTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CatalogId: str = ...,
    ResourceShareType: ResourceShareTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListLFTagsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListLFTagsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListLFTagsRequestPaginateTypeDef = {  # (1)
    "CatalogId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLFTagsRequestPaginateTypeDef](./type_defs.md#listlftagsrequestpaginatetypedef)
## SearchDatabasesByLFTagsPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("search_databases_by_lf_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation/paginator/SearchDatabasesByLFTags.html#LakeFormation.Paginator.SearchDatabasesByLFTags)

```python
# SearchDatabasesByLFTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import SearchDatabasesByLFTagsPaginator

session = get_session()
async with session.create_client("lakeformation") as client:  # (1)
    paginator: SearchDatabasesByLFTagsPaginator = client.get_paginator("search_databases_by_lf_tags")  # (2)
    async for item in paginator.paginate(...):
        item: SearchDatabasesByLFTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [LakeFormationClient](./client.md)
2. paginator: [SearchDatabasesByLFTagsPaginator](./paginators.md#searchdatabasesbylftagspaginator)
3. item: `AioPageIterator[SearchDatabasesByLFTagsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchDatabasesByLFTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Expression: Sequence[LFTagUnionTypeDef],  # (1)
    CatalogId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchDatabasesByLFTagsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[LFTagUnionTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchDatabasesByLFTagsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchDatabasesByLFTagsRequestPaginateTypeDef = {  # (1)
    "Expression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchDatabasesByLFTagsRequestPaginateTypeDef](./type_defs.md#searchdatabasesbylftagsrequestpaginatetypedef)
## SearchTablesByLFTagsPaginator

Type annotations and code completion for `#!python session.create_client("lakeformation").get_paginator("search_tables_by_lf_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation/paginator/SearchTablesByLFTags.html#LakeFormation.Paginator.SearchTablesByLFTags)

```python
# SearchTablesByLFTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lakeformation.paginator import SearchTablesByLFTagsPaginator

session = get_session()
async with session.create_client("lakeformation") as client:  # (1)
    paginator: SearchTablesByLFTagsPaginator = client.get_paginator("search_tables_by_lf_tags")  # (2)
    async for item in paginator.paginate(...):
        item: SearchTablesByLFTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [LakeFormationClient](./client.md)
2. paginator: [SearchTablesByLFTagsPaginator](./paginators.md#searchtablesbylftagspaginator)
3. item: `AioPageIterator[SearchTablesByLFTagsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchTablesByLFTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Expression: Sequence[LFTagUnionTypeDef],  # (1)
    CatalogId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchTablesByLFTagsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[LFTagUnionTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchTablesByLFTagsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchTablesByLFTagsRequestPaginateTypeDef = {  # (1)
    "Expression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchTablesByLFTagsRequestPaginateTypeDef](./type_defs.md#searchtablesbylftagsrequestpaginatetypedef)
