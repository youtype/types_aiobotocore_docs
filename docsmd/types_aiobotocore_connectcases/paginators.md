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
3. item: [:material-code-braces: ListCaseRulesResponseTypeDef](./type_defs.md#listcaserulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCaseRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCaseRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCaseRulesResponseTypeDef](./type_defs.md#listcaserulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCaseRulesRequestPaginateTypeDef = {  # (1)
    "domainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCaseRulesRequestPaginateTypeDef](./type_defs.md#listcaserulesrequestpaginatetypedef) 
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
3. item: [:material-code-braces: SearchCasesResponseTypeDef](./type_defs.md#searchcasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchCasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainId: str,
    fields: Sequence[FieldIdentifierTypeDef] = ...,  # (1)
    filter: CaseFilterPaginatorTypeDef = ...,  # (2)
    searchTerm: str = ...,
    sorts: Sequence[SortTypeDef] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[SearchCasesResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
2. See [:material-code-braces: CaseFilterPaginatorTypeDef](./type_defs.md#casefilterpaginatortypedef) 
3. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: SearchCasesResponseTypeDef](./type_defs.md#searchcasesresponsetypedef) 


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
3. item: [:material-code-braces: SearchRelatedItemsResponseTypeDef](./type_defs.md#searchrelateditemsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchRelatedItemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    caseId: str,
    domainId: str,
    filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[SearchRelatedItemsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: RelatedItemTypeFilterTypeDef](./type_defs.md#relateditemtypefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchRelatedItemsResponseTypeDef](./type_defs.md#searchrelateditemsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchRelatedItemsRequestPaginateTypeDef = {  # (1)
    "caseId": ...,
    "domainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchRelatedItemsRequestPaginateTypeDef](./type_defs.md#searchrelateditemsrequestpaginatetypedef) 
