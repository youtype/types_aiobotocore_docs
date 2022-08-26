# Paginators

> [Index](../README.md) > [IoT1ClickProjects](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoT1ClickProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
    type annotations stubs module [types-aiobotocore-iot1click-projects](https://pypi.org/project/types-aiobotocore-iot1click-projects/).

## ListPlacementsPaginator

Type annotations and code completion for `#!python session.create_client("iot1click-projects").get_paginator("list_placements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_iot1click_projects.paginator import ListPlacementsPaginator

session = get_session()
async with session.create_client("iot1click-projects") as client:  # (1)
    paginator: ListPlacementsPaginator = client.get_paginator("list_placements")  # (2)
    async for item in paginator.paginate(...):
        item: ListPlacementsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoT1ClickProjectsClient](./client.md)
2. paginator: [ListPlacementsPaginator](./paginators.md#listplacementspaginator)
3. item: [:material-code-braces: ListPlacementsResponseTypeDef](./type_defs.md#listplacementsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPlacementsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    projectName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPlacementsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPlacementsResponseTypeDef](./type_defs.md#listplacementsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPlacementsRequestListPlacementsPaginateTypeDef = {  # (1)
    "projectName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlacementsRequestListPlacementsPaginateTypeDef](./type_defs.md#listplacementsrequestlistplacementspaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.create_client("iot1click-projects").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_iot1click_projects.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("iot1click-projects") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoT1ClickProjectsClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListProjectsRequestListProjectsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestListProjectsPaginateTypeDef](./type_defs.md#listprojectsrequestlistprojectspaginatetypedef) 
