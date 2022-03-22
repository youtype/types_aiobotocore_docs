<a id="paginators-for-aiobotocore-transfer-module"></a>

# Paginators for aiobotocore Transfer module

> [Index](../README.md) > [Transfer](./README.md) > Paginators

Auto-generated documentation for
[Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
type annotations stubs module
[types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

- [Paginators for aiobotocore Transfer module](#paginators-for-aiobotocore-transfer-module)
  - [ListAccessesPaginator](#listaccessespaginator)
  - [ListExecutionsPaginator](#listexecutionspaginator)
  - [ListSecurityPoliciesPaginator](#listsecuritypoliciespaginator)
  - [ListServersPaginator](#listserverspaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)
  - [ListUsersPaginator](#listuserspaginator)
  - [ListWorkflowsPaginator](#listworkflowspaginator)

<a id="listaccessespaginator"></a>

## ListAccessesPaginator

Type annotations for
`session.create_client("transfer").get_paginator("list_accesses")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListAccessesPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListAccessesPaginator = client.get_paginator("list_accesses")
```

Boto3 documentation:
[Transfer.Paginator.ListAccesses](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListAccesses)

Arguments for `ListAccessesPaginator.paginate` method:

- `ServerId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccessesPaginator.paginate` returns
`AsyncIterator`\[[ListAccessesResponseTypeDef](./type_defs.md#listaccessesresponsetypedef)\].

<a id="listexecutionspaginator"></a>

## ListExecutionsPaginator

Type annotations for
`session.create_client("transfer").get_paginator("list_executions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListExecutionsPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListExecutionsPaginator = client.get_paginator("list_executions")
```

Boto3 documentation:
[Transfer.Paginator.ListExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListExecutions)

Arguments for `ListExecutionsPaginator.paginate` method:

- `WorkflowId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListExecutionsPaginator.paginate` returns
`AsyncIterator`\[[ListExecutionsResponseTypeDef](./type_defs.md#listexecutionsresponsetypedef)\].

<a id="listsecuritypoliciespaginator"></a>

## ListSecurityPoliciesPaginator

Type annotations for
`session.create_client("transfer").get_paginator("list_security_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListSecurityPoliciesPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListSecurityPoliciesPaginator = client.get_paginator("list_security_policies")
```

Boto3 documentation:
[Transfer.Paginator.ListSecurityPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListSecurityPolicies)

Arguments for `ListSecurityPoliciesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSecurityPoliciesPaginator.paginate` returns
`AsyncIterator`\[[ListSecurityPoliciesResponseTypeDef](./type_defs.md#listsecuritypoliciesresponsetypedef)\].

<a id="listserverspaginator"></a>

## ListServersPaginator

Type annotations for
`session.create_client("transfer").get_paginator("list_servers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListServersPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListServersPaginator = client.get_paginator("list_servers")
```

Boto3 documentation:
[Transfer.Paginator.ListServers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers)

Arguments for `ListServersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListServersPaginator.paginate` returns
`AsyncIterator`\[[ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("transfer").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[Transfer.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `Arn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterator`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].

<a id="listuserspaginator"></a>

## ListUsersPaginator

Type annotations for
`session.create_client("transfer").get_paginator("list_users")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListUsersPaginator = client.get_paginator("list_users")
```

Boto3 documentation:
[Transfer.Paginator.ListUsers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListUsers)

Arguments for `ListUsersPaginator.paginate` method:

- `ServerId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUsersPaginator.paginate` returns
`AsyncIterator`\[[ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)\].

<a id="listworkflowspaginator"></a>

## ListWorkflowsPaginator

Type annotations for
`session.create_client("transfer").get_paginator("list_workflows")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListWorkflowsPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListWorkflowsPaginator = client.get_paginator("list_workflows")
```

Boto3 documentation:
[Transfer.Paginator.ListWorkflows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListWorkflows)

Arguments for `ListWorkflowsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorkflowsPaginator.paginate` returns
`AsyncIterator`\[[ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef)\].
