<a id="paginators-for-aiobotocore-keyspaces-module"></a>

# Paginators for aiobotocore Keyspaces module

> [Index](../README.md) > [Keyspaces](./README.md) > Paginators

Auto-generated documentation for
[Keyspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
type annotations stubs module
[types-aiobotocore-keyspaces](https://pypi.org/project/types-aiobotocore-keyspaces/).

- [Paginators for aiobotocore Keyspaces module](#paginators-for-aiobotocore-keyspaces-module)
  - [ListKeyspacesPaginator](#listkeyspacespaginator)
  - [ListTablesPaginator](#listtablespaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)

<a id="listkeyspacespaginator"></a>

## ListKeyspacesPaginator

Type annotations for
`session.create_client("keyspaces").get_paginator("list_keyspaces")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_keyspaces.paginator import ListKeyspacesPaginator

session = get_session()
async with session.create_client("keyspaces") as client:
    client: KeyspacesClient
    paginator: ListKeyspacesPaginator = client.get_paginator("list_keyspaces")
```

Boto3 documentation:
[Keyspaces.Paginator.ListKeyspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListKeyspaces)

Arguments for `ListKeyspacesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListKeyspacesPaginator.paginate` returns
`AsyncIterator`\[[ListKeyspacesResponseTypeDef](./type_defs.md#listkeyspacesresponsetypedef)\].

<a id="listtablespaginator"></a>

## ListTablesPaginator

Type annotations for
`session.create_client("keyspaces").get_paginator("list_tables")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_keyspaces.paginator import ListTablesPaginator

session = get_session()
async with session.create_client("keyspaces") as client:
    client: KeyspacesClient
    paginator: ListTablesPaginator = client.get_paginator("list_tables")
```

Boto3 documentation:
[Keyspaces.Paginator.ListTables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTables)

Arguments for `ListTablesPaginator.paginate` method:

- `keyspaceName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTablesPaginator.paginate` returns
`AsyncIterator`\[[ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("keyspaces").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_keyspaces.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("keyspaces") as client:
    client: KeyspacesClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[Keyspaces.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `resourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterator`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].
