# Paginators

> [Index](../README.md) > [IdentityStore](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IdentityStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#identitystore)
    type annotations stubs module [types-aiobotocore-identitystore](https://pypi.org/project/types-aiobotocore-identitystore/).

## ListGroupMembershipsForMemberPaginator

Type annotations and code completion for `#!python session.create_client("identitystore").get_paginator("list_group_memberships_for_member")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/paginator/ListGroupMembershipsForMember.html#IdentityStore.Paginator.ListGroupMembershipsForMember)

```python
# ListGroupMembershipsForMemberPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_identitystore.paginator import ListGroupMembershipsForMemberPaginator

session = get_session()
async with session.create_client("identitystore") as client:  # (1)
    paginator: ListGroupMembershipsForMemberPaginator = client.get_paginator("list_group_memberships_for_member")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupMembershipsForMemberResponseTypeDef
        print(item)  # (3)
```

1. client: [IdentityStoreClient](./client.md)
2. paginator: [ListGroupMembershipsForMemberPaginator](./paginators.md#listgroupmembershipsformemberpaginator)
3. item: `AioPageIterator[ListGroupMembershipsForMemberResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGroupMembershipsForMemberPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IdentityStoreId: str,
    MemberId: MemberIdTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListGroupMembershipsForMemberResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListGroupMembershipsForMemberResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupMembershipsForMemberRequestPaginateTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "MemberId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupMembershipsForMemberRequestPaginateTypeDef](./type_defs.md#listgroupmembershipsformemberrequestpaginatetypedef)
## ListGroupMembershipsPaginator

Type annotations and code completion for `#!python session.create_client("identitystore").get_paginator("list_group_memberships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/paginator/ListGroupMemberships.html#IdentityStore.Paginator.ListGroupMemberships)

```python
# ListGroupMembershipsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_identitystore.paginator import ListGroupMembershipsPaginator

session = get_session()
async with session.create_client("identitystore") as client:  # (1)
    paginator: ListGroupMembershipsPaginator = client.get_paginator("list_group_memberships")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupMembershipsResponseTypeDef
        print(item)  # (3)
```

1. client: [IdentityStoreClient](./client.md)
2. paginator: [ListGroupMembershipsPaginator](./paginators.md#listgroupmembershipspaginator)
3. item: `AioPageIterator[ListGroupMembershipsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGroupMembershipsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IdentityStoreId: str,
    GroupId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListGroupMembershipsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListGroupMembershipsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupMembershipsRequestPaginateTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "GroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupMembershipsRequestPaginateTypeDef](./type_defs.md#listgroupmembershipsrequestpaginatetypedef)
## ListGroupsPaginator

Type annotations and code completion for `#!python session.create_client("identitystore").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/paginator/ListGroups.html#IdentityStore.Paginator.ListGroups)

```python
# ListGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_identitystore.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("identitystore") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [IdentityStoreClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: `AioPageIterator[ListGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IdentityStoreId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListGroupsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsRequestPaginateTypeDef = {  # (1)
    "IdentityStoreId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestPaginateTypeDef](./type_defs.md#listgroupsrequestpaginatetypedef)
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("identitystore").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/paginator/ListUsers.html#IdentityStore.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_identitystore.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("identitystore") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [IdentityStoreClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: `AioPageIterator[ListUsersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IdentityStoreId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListUsersResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListUsersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "IdentityStoreId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef)
