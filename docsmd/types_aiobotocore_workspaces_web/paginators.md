# Paginators

> [Index](../README.md) > [WorkSpacesWeb](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#workspacesweb)
    type annotations stubs module [types-aiobotocore-workspaces-web](https://pypi.org/project/types-aiobotocore-workspaces-web/).

## ListDataProtectionSettingsPaginator

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_paginator("list_data_protection_settings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web/paginator/ListDataProtectionSettings.html#WorkSpacesWeb.Paginator.ListDataProtectionSettings)

```python
# ListDataProtectionSettingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_web.paginator import ListDataProtectionSettingsPaginator

session = get_session()
async with session.create_client("workspaces-web") as client:  # (1)
    paginator: ListDataProtectionSettingsPaginator = client.get_paginator("list_data_protection_settings")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataProtectionSettingsResponseTypeDef
        print(item)  # (3)
```

1. client: [WorkSpacesWebClient](./client.md)
2. paginator: [ListDataProtectionSettingsPaginator](./paginators.md#listdataprotectionsettingspaginator)
3. item: [:material-code-braces: ListDataProtectionSettingsResponseTypeDef](./type_defs.md#listdataprotectionsettingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDataProtectionSettingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDataProtectionSettingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataProtectionSettingsResponseTypeDef](./type_defs.md#listdataprotectionsettingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDataProtectionSettingsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataProtectionSettingsRequestPaginateTypeDef](./type_defs.md#listdataprotectionsettingsrequestpaginatetypedef) 
## ListSessionsPaginator

Type annotations and code completion for `#!python session.create_client("workspaces-web").get_paginator("list_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web/paginator/ListSessions.html#WorkSpacesWeb.Paginator.ListSessions)

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
) -> AioPageIterator[ListSessionsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SessionSortByType](./literals.md#sessionsortbytype) 
2. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListSessionsResponseTypeDef](./type_defs.md#listsessionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSessionsRequestPaginateTypeDef = {  # (1)
    "portalId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSessionsRequestPaginateTypeDef](./type_defs.md#listsessionsrequestpaginatetypedef) 
