<a id="paginators-for-aiobotocore-prometheusservice-module"></a>

# Paginators for aiobotocore PrometheusService module

> [Index](../README.md) > [PrometheusService](./README.md) > Paginators

Auto-generated documentation for
[PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService)
type annotations stubs module
[types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

- [Paginators for aiobotocore PrometheusService module](#paginators-for-aiobotocore-prometheusservice-module)
  - [ListRuleGroupsNamespacesPaginator](#listrulegroupsnamespacespaginator)
  - [ListWorkspacesPaginator](#listworkspacespaginator)

<a id="listrulegroupsnamespacespaginator"></a>

## ListRuleGroupsNamespacesPaginator

Type annotations for
`session.create_client("amp").get_paginator("list_rule_groups_namespaces")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amp.paginator import ListRuleGroupsNamespacesPaginator

session = get_session()
async with session.create_client("amp") as client:
    client: PrometheusServiceClient
    paginator: ListRuleGroupsNamespacesPaginator = client.get_paginator("list_rule_groups_namespaces")
```

Boto3 documentation:
[PrometheusService.Paginator.ListRuleGroupsNamespaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Paginator.ListRuleGroupsNamespaces)

Arguments for `ListRuleGroupsNamespacesPaginator.paginate` method:

- `workspaceId`: `str` *(required)*
- `name`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRuleGroupsNamespacesPaginator.paginate` returns
`AsyncIterator`\[[ListRuleGroupsNamespacesResponseTypeDef](./type_defs.md#listrulegroupsnamespacesresponsetypedef)\].

<a id="listworkspacespaginator"></a>

## ListWorkspacesPaginator

Type annotations for
`session.create_client("amp").get_paginator("list_workspaces")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amp.paginator import ListWorkspacesPaginator

session = get_session()
async with session.create_client("amp") as client:
    client: PrometheusServiceClient
    paginator: ListWorkspacesPaginator = client.get_paginator("list_workspaces")
```

Boto3 documentation:
[PrometheusService.Paginator.ListWorkspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#PrometheusService.Paginator.ListWorkspaces)

Arguments for `ListWorkspacesPaginator.paginate` method:

- `alias`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorkspacesPaginator.paginate` returns
`AsyncIterator`\[[ListWorkspacesResponseTypeDef](./type_defs.md#listworkspacesresponsetypedef)\].
