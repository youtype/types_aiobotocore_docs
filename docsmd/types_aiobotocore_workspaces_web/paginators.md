# Paginators

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb)
    type annotations stubs module [types-aiobotocore-workspaces-web](https://pypi.org/project/types-aiobotocore-workspaces-web/).

## ListSessionsPaginator

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_paginator("list_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#WorkSpacesWeb.Paginator.ListSessions)

```python
# ListSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_web.paginator import ListSessionsPaginator

session = get_session()
async with session.create_client("workspaces-web") as client:  # (1)
    paginator: ListSessionsPaginator = client.get_paginator("list_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSessionsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesWebClient](./client.md)
2. paginator: [ListSessionsPaginator](./paginators.md#listsessionspaginator)
3. item: [:material-code-braces: ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    portalId: str,
    sessionId: str = ...,
    sortBy: SessionSortByType = ...,  # (1)
    status: SessionStatusType = ...,  # (2)
    username: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListSessionsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SessionSortByType](./literals.md#sessionsortbytype) 
2. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSessionsRequestListSessionsPaginateTypeDef = {  # (1)
    "portalId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSessionsRequestListSessionsPaginateTypeDef](./type_defs.md#listsessionsrequestlistsessionspaginatetypedef) 
