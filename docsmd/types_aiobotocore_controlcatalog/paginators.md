# Paginators

> [Index](../README.md) > [ControlCatalog](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ControlCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#controlcatalog)
    type annotations stubs module [types-aiobotocore-controlcatalog](https://pypi.org/project/types-aiobotocore-controlcatalog/).

## ListCommonControlsPaginator

Type annotations and code completion for `#!python session.create_client("controlcatalog").get_paginator("list_common_controls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/paginator/ListCommonControls.html#ControlCatalog.Paginator.ListCommonControls)

```python
# ListCommonControlsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_controlcatalog.paginator import ListCommonControlsPaginator

session = get_session()
async with session.create_client("controlcatalog") as client:  # (1)
    paginator: ListCommonControlsPaginator = client.get_paginator("list_common_controls")  # (2)
    async for item in paginator.paginate(...):
        item: ListCommonControlsResponseTypeDef
        print(item)  # (3)
```

1. client: [ControlCatalogClient](./client.md)
2. paginator: [ListCommonControlsPaginator](./paginators.md#listcommoncontrolspaginator)
3. item: [:material-code-braces: ListCommonControlsResponseTypeDef](./type_defs.md#listcommoncontrolsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCommonControlsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CommonControlFilter: CommonControlFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListCommonControlsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: CommonControlFilterTypeDef](./type_defs.md#commoncontrolfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCommonControlsResponseTypeDef](./type_defs.md#listcommoncontrolsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCommonControlsRequestPaginateTypeDef = {  # (1)
    "CommonControlFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCommonControlsRequestPaginateTypeDef](./type_defs.md#listcommoncontrolsrequestpaginatetypedef) 
## ListControlsPaginator

Type annotations and code completion for `#!python session.create_client("controlcatalog").get_paginator("list_controls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/paginator/ListControls.html#ControlCatalog.Paginator.ListControls)

```python
# ListControlsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_controlcatalog.paginator import ListControlsPaginator

session = get_session()
async with session.create_client("controlcatalog") as client:  # (1)
    paginator: ListControlsPaginator = client.get_paginator("list_controls")  # (2)
    async for item in paginator.paginate(...):
        item: ListControlsResponseTypeDef
        print(item)  # (3)
```

1. client: [ControlCatalogClient](./client.md)
2. paginator: [ListControlsPaginator](./paginators.md#listcontrolspaginator)
3. item: [:material-code-braces: ListControlsResponseTypeDef](./type_defs.md#listcontrolsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListControlsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListControlsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListControlsResponseTypeDef](./type_defs.md#listcontrolsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListControlsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListControlsRequestPaginateTypeDef](./type_defs.md#listcontrolsrequestpaginatetypedef) 
## ListDomainsPaginator

Type annotations and code completion for `#!python session.create_client("controlcatalog").get_paginator("list_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/paginator/ListDomains.html#ControlCatalog.Paginator.ListDomains)

```python
# ListDomainsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_controlcatalog.paginator import ListDomainsPaginator

session = get_session()
async with session.create_client("controlcatalog") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsResponseTypeDef
        print(item)  # (3)
```

1. client: [ControlCatalogClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDomainsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainsRequestPaginateTypeDef](./type_defs.md#listdomainsrequestpaginatetypedef) 
## ListObjectivesPaginator

Type annotations and code completion for `#!python session.create_client("controlcatalog").get_paginator("list_objectives")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/paginator/ListObjectives.html#ControlCatalog.Paginator.ListObjectives)

```python
# ListObjectivesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_controlcatalog.paginator import ListObjectivesPaginator

session = get_session()
async with session.create_client("controlcatalog") as client:  # (1)
    paginator: ListObjectivesPaginator = client.get_paginator("list_objectives")  # (2)
    async for item in paginator.paginate(...):
        item: ListObjectivesResponseTypeDef
        print(item)  # (3)
```

1. client: [ControlCatalogClient](./client.md)
2. paginator: [ListObjectivesPaginator](./paginators.md#listobjectivespaginator)
3. item: [:material-code-braces: ListObjectivesResponseTypeDef](./type_defs.md#listobjectivesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListObjectivesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ObjectiveFilter: ObjectiveFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListObjectivesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ObjectiveFilterTypeDef](./type_defs.md#objectivefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListObjectivesResponseTypeDef](./type_defs.md#listobjectivesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListObjectivesRequestPaginateTypeDef = {  # (1)
    "ObjectiveFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectivesRequestPaginateTypeDef](./type_defs.md#listobjectivesrequestpaginatetypedef) 
