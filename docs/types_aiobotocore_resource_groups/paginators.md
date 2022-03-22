<a id="paginators-for-aiobotocore-resourcegroups-module"></a>

# Paginators for aiobotocore ResourceGroups module

> [Index](../README.md) > [ResourceGroups](./README.md) > Paginators

Auto-generated documentation for
[ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
type annotations stubs module
[types-aiobotocore-resource-groups](https://pypi.org/project/types-aiobotocore-resource-groups/).

- [Paginators for aiobotocore ResourceGroups module](#paginators-for-aiobotocore-resourcegroups-module)
  - [ListGroupResourcesPaginator](#listgroupresourcespaginator)
  - [ListGroupsPaginator](#listgroupspaginator)
  - [SearchResourcesPaginator](#searchresourcespaginator)

<a id="listgroupresourcespaginator"></a>

## ListGroupResourcesPaginator

Type annotations for
`session.create_client("resource-groups").get_paginator("list_group_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.paginator import ListGroupResourcesPaginator

session = get_session()
async with session.create_client("resource-groups") as client:
    client: ResourceGroupsClient
    paginator: ListGroupResourcesPaginator = client.get_paginator("list_group_resources")
```

Boto3 documentation:
[ResourceGroups.Paginator.ListGroupResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroupResources)

Arguments for `ListGroupResourcesPaginator.paginate` method:

- `GroupName`: `str`
- `Group`: `str`
- `Filters`:
  `Sequence`\[[ResourceFilterTypeDef](./type_defs.md#resourcefiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGroupResourcesPaginator.paginate` returns
`AsyncIterator`\[[ListGroupResourcesOutputTypeDef](./type_defs.md#listgroupresourcesoutputtypedef)\].

<a id="listgroupspaginator"></a>

## ListGroupsPaginator

Type annotations for
`session.create_client("resource-groups").get_paginator("list_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("resource-groups") as client:
    client: ResourceGroupsClient
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")
```

Boto3 documentation:
[ResourceGroups.Paginator.ListGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.ListGroups)

Arguments for `ListGroupsPaginator.paginate` method:

- `Filters`:
  `Sequence`\[[GroupFilterTypeDef](./type_defs.md#groupfiltertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListGroupsOutputTypeDef](./type_defs.md#listgroupsoutputtypedef)\].

<a id="searchresourcespaginator"></a>

## SearchResourcesPaginator

Type annotations for
`session.create_client("resource-groups").get_paginator("search_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_resource_groups.paginator import SearchResourcesPaginator

session = get_session()
async with session.create_client("resource-groups") as client:
    client: ResourceGroupsClient
    paginator: SearchResourcesPaginator = client.get_paginator("search_resources")
```

Boto3 documentation:
[ResourceGroups.Paginator.SearchResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups.Paginator.SearchResources)

Arguments for `SearchResourcesPaginator.paginate` method:

- `ResourceQuery`: [ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchResourcesPaginator.paginate` returns
`AsyncIterator`\[[SearchResourcesOutputTypeDef](./type_defs.md#searchresourcesoutputtypedef)\].
