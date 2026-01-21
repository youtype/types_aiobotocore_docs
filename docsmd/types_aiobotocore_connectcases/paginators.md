# Paginators

> [Index](../README.md) > [ConnectCases](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#connectcases)
    type annotations stubs module [types-aiobotocore-connectcases](https://pypi.org/project/types-aiobotocore-connectcases/).

## ListCaseRulesPaginator

Type annotations and code completion for `#!python session.create_client("connectcases").get_paginator("list_case_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases/paginator/ListCaseRules.html#ConnectCases.Paginator.ListCaseRules)

```python
# ListCaseRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connectcases.paginator import ListCaseRulesPaginator

session = get_session()
async with session.create_client("connectcases") as client:  # (1)
    paginator: ListCaseRulesPaginator = client.get_paginator("list_case_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListCaseRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. paginator: [ListCaseRulesPaginator](./paginators.md#listcaserulespaginator)
3. item: `AioPageIterator[ListCaseRulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCaseRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCaseRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCaseRulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCaseRulesRequestPaginateTypeDef = {  # (1)
    "domainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCaseRulesRequestPaginateTypeDef](./type_defs.md#listcaserulesrequestpaginatetypedef)
## SearchAllRelatedItemsPaginator

Type annotations and code completion for `#!python session.create_client("connectcases").get_paginator("search_all_related_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases/paginator/SearchAllRelatedItems.html#ConnectCases.Paginator.SearchAllRelatedItems)

```python
# SearchAllRelatedItemsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connectcases.paginator import SearchAllRelatedItemsPaginator

session = get_session()
async with session.create_client("connectcases") as client:  # (1)
    paginator: SearchAllRelatedItemsPaginator = client.get_paginator("search_all_related_items")  # (2)
    async for item in paginator.paginate(...):
        item: SearchAllRelatedItemsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. paginator: [SearchAllRelatedItemsPaginator](./paginators.md#searchallrelateditemspaginator)
3. item: `AioPageIterator[SearchAllRelatedItemsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchAllRelatedItemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainId: str,
    filters: Sequence[RelatedItemTypeFilterPaginatorTypeDef] = ...,  # (1)
    sorts: Sequence[SearchAllRelatedItemsSortTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchAllRelatedItemsResponseTypeDef]:  # (4)
    ...
```

1. See `Sequence[RelatedItemTypeFilterPaginatorTypeDef]`
2. See `Sequence[SearchAllRelatedItemsSortTypeDef]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchAllRelatedItemsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchAllRelatedItemsRequestPaginateTypeDef = {  # (1)
    "domainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchAllRelatedItemsRequestPaginateTypeDef](./type_defs.md#searchallrelateditemsrequestpaginatetypedef)
## SearchCasesPaginator

Type annotations and code completion for `#!python session.create_client("connectcases").get_paginator("search_cases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases/paginator/SearchCases.html#ConnectCases.Paginator.SearchCases)

```python
# SearchCasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connectcases.paginator import SearchCasesPaginator

session = get_session()
async with session.create_client("connectcases") as client:  # (1)
    paginator: SearchCasesPaginator = client.get_paginator("search_cases")  # (2)
    async for item in paginator.paginate(...):
        item: SearchCasesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. paginator: [SearchCasesPaginator](./paginators.md#searchcasespaginator)
3. item: `AioPageIterator[SearchCasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchCasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainId: str,
    searchTerm: str = ...,
    filter: CaseFilterPaginatorTypeDef = ...,  # (1)
    sorts: Sequence[SortTypeDef] = ...,  # (2)
    fields: Sequence[FieldIdentifierTypeDef] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[SearchCasesResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: CaseFilterPaginatorTypeDef](./type_defs.md#casefilterpaginatortypedef)
2. See `Sequence[SortTypeDef]`
3. See `Sequence[FieldIdentifierTypeDef]`
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[SearchCasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchCasesRequestPaginateTypeDef = {  # (1)
    "domainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchCasesRequestPaginateTypeDef](./type_defs.md#searchcasesrequestpaginatetypedef)
## SearchRelatedItemsPaginator

Type annotations and code completion for `#!python session.create_client("connectcases").get_paginator("search_related_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases/paginator/SearchRelatedItems.html#ConnectCases.Paginator.SearchRelatedItems)

```python
# SearchRelatedItemsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connectcases.paginator import SearchRelatedItemsPaginator

session = get_session()
async with session.create_client("connectcases") as client:  # (1)
    paginator: SearchRelatedItemsPaginator = client.get_paginator("search_related_items")  # (2)
    async for item in paginator.paginate(...):
        item: SearchRelatedItemsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectCasesClient](./client.md)
2. paginator: [SearchRelatedItemsPaginator](./paginators.md#searchrelateditemspaginator)
3. item: `AioPageIterator[SearchRelatedItemsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchRelatedItemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainId: str,
    caseId: str,
    filters: Sequence[RelatedItemTypeFilterPaginatorTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchRelatedItemsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[RelatedItemTypeFilterPaginatorTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchRelatedItemsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchRelatedItemsRequestPaginateTypeDef = {  # (1)
    "domainId": ...,
    "caseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchRelatedItemsRequestPaginateTypeDef](./type_defs.md#searchrelateditemsrequestpaginatetypedef)
