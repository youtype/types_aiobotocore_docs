# Paginators

> [Index](../README.md) > [PrometheusService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#prometheusservice)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## ListRuleGroupsNamespacesPaginator

Type annotations and code completion for `#!python session.create_client("amp").get_paginator("list_rule_groups_namespaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/paginator/ListRuleGroupsNamespaces.html#PrometheusService.Paginator.ListRuleGroupsNamespaces)

```python
# ListRuleGroupsNamespacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amp.paginator import ListRuleGroupsNamespacesPaginator

session = get_session()
async with session.create_client("amp") as client:  # (1)
    paginator: ListRuleGroupsNamespacesPaginator = client.get_paginator("list_rule_groups_namespaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleGroupsNamespacesResponseTypeDef
        print(item)  # (3)
```

1. client: [PrometheusServiceClient](./client.md)
2. paginator: [ListRuleGroupsNamespacesPaginator](./paginators.md#listrulegroupsnamespacespaginator)
3. item: [:material-code-braces: ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRuleGroupsNamespacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workspaceId: str,
    name: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRuleGroupsNamespacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRuleGroupsNamespacesRequestPaginateTypeDef = {  # (1)
    "workspaceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsNamespacesRequestPaginateTypeDef](./type_defs.md#listrulegroupsnamespacesrequestpaginatetypedef) 
## ListScrapersPaginator

Type annotations and code completion for `#!python session.create_client("amp").get_paginator("list_scrapers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/paginator/ListScrapers.html#PrometheusService.Paginator.ListScrapers)

```python
# ListScrapersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amp.paginator import ListScrapersPaginator

session = get_session()
async with session.create_client("amp") as client:  # (1)
    paginator: ListScrapersPaginator = client.get_paginator("list_scrapers")  # (2)
    async for item in paginator.paginate(...):
        item: ListScrapersResponseTypeDef
        print(item)  # (3)
```

1. client: [PrometheusServiceClient](./client.md)
2. paginator: [ListScrapersPaginator](./paginators.md#listscraperspaginator)
3. item: [:material-code-braces: ListScrapersResponseTypeDef](./type_defs.md#listscrapersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListScrapersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Mapping[str, Sequence[str]] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListScrapersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListScrapersResponseTypeDef](./type_defs.md#listscrapersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListScrapersRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListScrapersRequestPaginateTypeDef](./type_defs.md#listscrapersrequestpaginatetypedef) 
## ListWorkspacesPaginator

Type annotations and code completion for `#!python session.create_client("amp").get_paginator("list_workspaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp/paginator/ListWorkspaces.html#PrometheusService.Paginator.ListWorkspaces)

```python
# ListWorkspacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amp.paginator import ListWorkspacesPaginator

session = get_session()
async with session.create_client("amp") as client:  # (1)
    paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkspacesResponseTypeDef
        print(item)  # (3)
```

1. client: [PrometheusServiceClient](./client.md)
2. paginator: [ListWorkspacesPaginator](./paginators.md#listworkspacespaginator)
3. item: [:material-code-braces: ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkspacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    alias: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWorkspacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkspacesRequestPaginateTypeDef = {  # (1)
    "alias": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkspacesRequestPaginateTypeDef](./type_defs.md#listworkspacesrequestpaginatetypedef) 
