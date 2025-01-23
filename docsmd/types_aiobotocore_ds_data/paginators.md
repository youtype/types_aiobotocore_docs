# Paginators

> [Index](../README.md) > [DirectoryServiceData](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DirectoryServiceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data.html#directoryservicedata)
    type annotations stubs module [types-aiobotocore-ds-data](https://pypi.org/project/types-aiobotocore-ds-data/).

## ListGroupMembersPaginator

Type annotations and code completion for `#!python session.create_client("ds-data").get_paginator("list_group_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/paginator/ListGroupMembers.html#DirectoryServiceData.Paginator.ListGroupMembers)

```python
# ListGroupMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds_data.paginator import ListGroupMembersPaginator

session = get_session()
async with session.create_client("ds-data") as client:  # (1)
    paginator: ListGroupMembersPaginator = client.get_paginator("list_group_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupMembersResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceDataClient](./client.md)
2. paginator: [ListGroupMembersPaginator](./paginators.md#listgroupmemberspaginator)
3. item: [:material-code-braces: ListGroupMembersResultTypeDef](./type_defs.md#listgroupmembersresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    MemberRealm: str = ...,
    Realm: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGroupMembersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupMembersResultTypeDef](./type_defs.md#listgroupmembersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupMembersRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupMembersRequestPaginateTypeDef](./type_defs.md#listgroupmembersrequestpaginatetypedef) 
## ListGroupsForMemberPaginator

Type annotations and code completion for `#!python session.create_client("ds-data").get_paginator("list_groups_for_member")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/paginator/ListGroupsForMember.html#DirectoryServiceData.Paginator.ListGroupsForMember)

```python
# ListGroupsForMemberPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds_data.paginator import ListGroupsForMemberPaginator

session = get_session()
async with session.create_client("ds-data") as client:  # (1)
    paginator: ListGroupsForMemberPaginator = client.get_paginator("list_groups_for_member")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsForMemberResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceDataClient](./client.md)
2. paginator: [ListGroupsForMemberPaginator](./paginators.md#listgroupsformemberpaginator)
3. item: [:material-code-braces: ListGroupsForMemberResultTypeDef](./type_defs.md#listgroupsformemberresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsForMemberPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    MemberRealm: str = ...,
    Realm: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGroupsForMemberResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsForMemberResultTypeDef](./type_defs.md#listgroupsformemberresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsForMemberRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsForMemberRequestPaginateTypeDef](./type_defs.md#listgroupsformemberrequestpaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ds-data").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/paginator/ListGroups.html#DirectoryServiceData.Paginator.ListGroups)

```python
# ListGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds_data.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("ds-data") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceDataClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsResultTypeDef](./type_defs.md#listgroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    Realm: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGroupsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsResultTypeDef](./type_defs.md#listgroupsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestPaginateTypeDef](./type_defs.md#listgroupsrequestpaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("ds-data").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/paginator/ListUsers.html#DirectoryServiceData.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds_data.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("ds-data") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceDataClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResultTypeDef](./type_defs.md#listusersresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    Realm: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListUsersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResultTypeDef](./type_defs.md#listusersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef) 
## SearchGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ds-data").get_paginator("search_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/paginator/SearchGroups.html#DirectoryServiceData.Paginator.SearchGroups)

```python
# SearchGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds_data.paginator import SearchGroupsPaginator

session = get_session()
async with session.create_client("ds-data") as client:  # (1)
    paginator: SearchGroupsPaginator = client.get_paginator("search_groups")  # (2)
    async for item in paginator.paginate(...):
        item: SearchGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceDataClient](./client.md)
2. paginator: [SearchGroupsPaginator](./paginators.md#searchgroupspaginator)
3. item: [:material-code-braces: SearchGroupsResultTypeDef](./type_defs.md#searchgroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python SearchGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    SearchAttributes: Sequence[str],
    SearchString: str,
    Realm: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[SearchGroupsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SearchGroupsResultTypeDef](./type_defs.md#searchgroupsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchGroupsRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
    "SearchAttributes": ...,
    "SearchString": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchGroupsRequestPaginateTypeDef](./type_defs.md#searchgroupsrequestpaginatetypedef) 
## SearchUsersPaginator

Type annotations and code completion for `#!python session.create_client("ds-data").get_paginator("search_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/paginator/SearchUsers.html#DirectoryServiceData.Paginator.SearchUsers)

```python
# SearchUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds_data.paginator import SearchUsersPaginator

session = get_session()
async with session.create_client("ds-data") as client:  # (1)
    paginator: SearchUsersPaginator = client.get_paginator("search_users")  # (2)
    async for item in paginator.paginate(...):
        item: SearchUsersResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceDataClient](./client.md)
2. paginator: [SearchUsersPaginator](./paginators.md#searchuserspaginator)
3. item: [:material-code-braces: SearchUsersResultTypeDef](./type_defs.md#searchusersresulttypedef) 


### paginate

Type annotations and code completion for `#!python SearchUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryId: str,
    SearchAttributes: Sequence[str],
    SearchString: str,
    Realm: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[SearchUsersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SearchUsersResultTypeDef](./type_defs.md#searchusersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchUsersRequestPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
    "SearchAttributes": ...,
    "SearchString": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchUsersRequestPaginateTypeDef](./type_defs.md#searchusersrequestpaginatetypedef) 
