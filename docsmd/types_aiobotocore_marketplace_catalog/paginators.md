# Paginators

> [Index](../README.md) > [MarketplaceCatalog](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#marketplacecatalog)
    type annotations stubs module [types-aiobotocore-marketplace-catalog](https://pypi.org/project/types-aiobotocore-marketplace-catalog/).

## ListChangeSetsPaginator

Type annotations and code completion for `#!python session.create_client("marketplace-catalog").get_paginator("list_change_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog/paginator/ListChangeSets.html#MarketplaceCatalog.Paginator.ListChangeSets)

```python
# ListChangeSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_catalog.paginator import ListChangeSetsPaginator

session = get_session()
async with session.create_client("marketplace-catalog") as client:  # (1)
    paginator: ListChangeSetsPaginator = client.get_paginator("list_change_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListChangeSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [MarketplaceCatalogClient](./client.md)
2. paginator: [ListChangeSetsPaginator](./paginators.md#listchangesetspaginator)
3. item: [:material-code-braces: ListChangeSetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChangeSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    FilterList: Sequence[FilterTypeDef] = ...,  # (1)
    Sort: SortTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListChangeSetsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListChangeSetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChangeSetsRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChangeSetsRequestPaginateTypeDef](./type_defs.md#listchangesetsrequestpaginatetypedef) 
## ListEntitiesPaginator

Type annotations and code completion for `#!python session.create_client("marketplace-catalog").get_paginator("list_entities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog/paginator/ListEntities.html#MarketplaceCatalog.Paginator.ListEntities)

```python
# ListEntitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_catalog.paginator import ListEntitiesPaginator

session = get_session()
async with session.create_client("marketplace-catalog") as client:  # (1)
    paginator: ListEntitiesPaginator = client.get_paginator("list_entities")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [MarketplaceCatalogClient](./client.md)
2. paginator: [ListEntitiesPaginator](./paginators.md#listentitiespaginator)
3. item: [:material-code-braces: ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEntitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    EntityType: str,
    FilterList: Sequence[FilterTypeDef] = ...,  # (1)
    Sort: SortTypeDef = ...,  # (2)
    OwnershipType: OwnershipTypeType = ...,  # (3)
    EntityTypeFilters: EntityTypeFiltersTypeDef = ...,  # (4)
    EntityTypeSort: EntityTypeSortTypeDef = ...,  # (5)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (6)
) -> AioPageIterator[ListEntitiesResponseTypeDef]:  # (7)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-brackets: OwnershipTypeType](./literals.md#ownershiptypetype) 
4. See [:material-code-braces: EntityTypeFiltersTypeDef](./type_defs.md#entitytypefilterstypedef) 
5. See [:material-code-braces: EntityTypeSortTypeDef](./type_defs.md#entitytypesorttypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
7. See [:material-code-braces: ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEntitiesRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
    "EntityType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitiesRequestPaginateTypeDef](./type_defs.md#listentitiesrequestpaginatetypedef) 
