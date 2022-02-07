<a id="paginators-for-aiobotocore-iot1clickprojects-module"></a>

# Paginators for aiobotocore IoT1ClickProjects module

> [Index](..) > [IoT1ClickProjects](.) > Paginators

Auto-generated documentation for
[IoT1ClickProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects)
type annotations stubs module
[types-aiobotocore-iot1click-projects](https://pypi.org/project/types-aiobotocore-iot1click-projects/).

- [Paginators for aiobotocore IoT1ClickProjects module](#paginators-for-aiobotocore-iot1clickprojects-module)
  - [ListPlacementsPaginator](#listplacementspaginator)
  - [ListProjectsPaginator](#listprojectspaginator)

<a id="listplacementspaginator"></a>

## ListPlacementsPaginator

Type annotations for
`session.create_client("iot1click-projects").get_paginator("list_placements")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot1click_projects.paginator import ListPlacementsPaginator

session = get_session()
async with session.create_client("iot1click-projects") as client:
    client: IoT1ClickProjectsClient
    paginator: ListPlacementsPaginator = client.get_paginator("list_placements")
```

Boto3 documentation:
[IoT1ClickProjects.Paginator.ListPlacements](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListPlacements)

Arguments for `ListPlacementsPaginator.paginate` method:

- `projectName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPlacementsPaginator.paginate` returns
`_PageIterator`\[[ListPlacementsResponseTypeDef](./type_defs.md#listplacementsresponsetypedef)\].

<a id="listprojectspaginator"></a>

## ListProjectsPaginator

Type annotations for
`session.create_client("iot1click-projects").get_paginator("list_projects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot1click_projects.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("iot1click-projects") as client:
    client: IoT1ClickProjectsClient
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")
```

Boto3 documentation:
[IoT1ClickProjects.Paginator.ListProjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Paginator.ListProjects)

Arguments for `ListProjectsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProjectsPaginator.paginate` returns
`_PageIterator`\[[ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef)\].
