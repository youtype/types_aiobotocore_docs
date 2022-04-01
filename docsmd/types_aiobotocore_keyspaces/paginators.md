# Paginators

> [Index](../README.md) > [Keyspaces](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Keyspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
    type annotations stubs module [types-aiobotocore-keyspaces](https://pypi.org/project/types-aiobotocore-keyspaces/).

## ListKeyspacesPaginator

Type annotations and code completion for `#!python session.create_client("keyspaces").get_paginator("list_keyspaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListKeyspaces)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_keyspaces.paginator import ListKeyspacesPaginator

session = get_session()
async with session.create_client("keyspaces") as client:
    client: KeyspacesClient
    paginator: ListKeyspacesPaginator = client.get_paginator("list_keyspaces")
```


### paginate

Type annotations and code completion for `#!python ListKeyspacesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListKeyspacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKeyspacesResponseTypeDef](./type_defs.md#listkeyspacesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListKeyspacesRequestListKeyspacesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeyspacesRequestListKeyspacesPaginateTypeDef](./type_defs.md#listkeyspacesrequestlistkeyspacespaginatetypedef) 
## ListTablesPaginator

Type annotations and code completion for `#!python session.create_client("keyspaces").get_paginator("list_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTables)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_keyspaces.paginator import ListTablesPaginator

session = get_session()
async with session.create_client("keyspaces") as client:
    client: KeyspacesClient
    paginator: ListTablesPaginator = client.get_paginator("list_tables")
```


### paginate

Type annotations and code completion for `#!python ListTablesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    keyspaceName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTablesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTablesRequestListTablesPaginateTypeDef = {  # (1)
    "keyspaceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTablesRequestListTablesPaginateTypeDef](./type_defs.md#listtablesrequestlisttablespaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("keyspaces").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTagsForResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_keyspaces.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("keyspaces") as client:
    client: KeyspacesClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef) 
