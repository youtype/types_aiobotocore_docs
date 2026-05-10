# Paginators

> [Index](../README.md) > [WickrAdminAPI](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [WickrAdminAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr.html#wickradminapi)
    type annotations stubs module [types-aiobotocore-wickr](https://pypi.org/project/types-aiobotocore-wickr/).

## ListBlockedGuestUsersPaginator

Type annotations and code completion for `#!python session.create_client("wickr").get_paginator("list_blocked_guest_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr/paginator/ListBlockedGuestUsers.html#WickrAdminAPI.Paginator.ListBlockedGuestUsers)

```python
# ListBlockedGuestUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_wickr.paginator import ListBlockedGuestUsersPaginator

session = get_session()
async with session.create_client("wickr") as client:  # (1)
    paginator: ListBlockedGuestUsersPaginator = client.get_paginator("list_blocked_guest_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListBlockedGuestUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [WickrAdminAPIClient](./client.md)
2. paginator: [ListBlockedGuestUsersPaginator](./paginators.md#listblockedguestuserspaginator)
3. item: `AioPageIterator[ListBlockedGuestUsersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBlockedGuestUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkId: str,
    sortDirection: SortDirectionType = ...,  # (1)
    sortFields: str = ...,
    username: str = ...,
    admin: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBlockedGuestUsersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBlockedGuestUsersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBlockedGuestUsersRequestPaginateTypeDef = {  # (1)
    "networkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBlockedGuestUsersRequestPaginateTypeDef](./type_defs.md#listblockedguestusersrequestpaginatetypedef)
## ListBotsPaginator

Type annotations and code completion for `#!python session.create_client("wickr").get_paginator("list_bots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr/paginator/ListBots.html#WickrAdminAPI.Paginator.ListBots)

```python
# ListBotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_wickr.paginator import ListBotsPaginator

session = get_session()
async with session.create_client("wickr") as client:  # (1)
    paginator: ListBotsPaginator = client.get_paginator("list_bots")  # (2)
    async for item in paginator.paginate(...):
        item: ListBotsResponseTypeDef
        print(item)  # (3)
```

1. client: [WickrAdminAPIClient](./client.md)
2. paginator: [ListBotsPaginator](./paginators.md#listbotspaginator)
3. item: `AioPageIterator[ListBotsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkId: str,
    sortFields: str = ...,
    sortDirection: SortDirectionType = ...,  # (1)
    displayName: str = ...,
    username: str = ...,
    status: int = ...,
    groupId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBotsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBotsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBotsRequestPaginateTypeDef = {  # (1)
    "networkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBotsRequestPaginateTypeDef](./type_defs.md#listbotsrequestpaginatetypedef)
## ListDevicesForUserPaginator

Type annotations and code completion for `#!python session.create_client("wickr").get_paginator("list_devices_for_user")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr/paginator/ListDevicesForUser.html#WickrAdminAPI.Paginator.ListDevicesForUser)

```python
# ListDevicesForUserPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_wickr.paginator import ListDevicesForUserPaginator

session = get_session()
async with session.create_client("wickr") as client:  # (1)
    paginator: ListDevicesForUserPaginator = client.get_paginator("list_devices_for_user")  # (2)
    async for item in paginator.paginate(...):
        item: ListDevicesForUserResponseTypeDef
        print(item)  # (3)
```

1. client: [WickrAdminAPIClient](./client.md)
2. paginator: [ListDevicesForUserPaginator](./paginators.md#listdevicesforuserpaginator)
3. item: `AioPageIterator[ListDevicesForUserResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDevicesForUserPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkId: str,
    userId: str,
    sortFields: str = ...,
    sortDirection: SortDirectionType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDevicesForUserResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDevicesForUserResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDevicesForUserRequestPaginateTypeDef = {  # (1)
    "networkId": ...,
    "userId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicesForUserRequestPaginateTypeDef](./type_defs.md#listdevicesforuserrequestpaginatetypedef)
## ListGuestUsersPaginator

Type annotations and code completion for `#!python session.create_client("wickr").get_paginator("list_guest_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr/paginator/ListGuestUsers.html#WickrAdminAPI.Paginator.ListGuestUsers)

```python
# ListGuestUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_wickr.paginator import ListGuestUsersPaginator

session = get_session()
async with session.create_client("wickr") as client:  # (1)
    paginator: ListGuestUsersPaginator = client.get_paginator("list_guest_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListGuestUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [WickrAdminAPIClient](./client.md)
2. paginator: [ListGuestUsersPaginator](./paginators.md#listguestuserspaginator)
3. item: `AioPageIterator[ListGuestUsersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGuestUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkId: str,
    sortDirection: SortDirectionType = ...,  # (1)
    sortFields: str = ...,
    username: str = ...,
    billingPeriod: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListGuestUsersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListGuestUsersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGuestUsersRequestPaginateTypeDef = {  # (1)
    "networkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGuestUsersRequestPaginateTypeDef](./type_defs.md#listguestusersrequestpaginatetypedef)
## ListNetworksPaginator

Type annotations and code completion for `#!python session.create_client("wickr").get_paginator("list_networks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr/paginator/ListNetworks.html#WickrAdminAPI.Paginator.ListNetworks)

```python
# ListNetworksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_wickr.paginator import ListNetworksPaginator

session = get_session()
async with session.create_client("wickr") as client:  # (1)
    paginator: ListNetworksPaginator = client.get_paginator("list_networks")  # (2)
    async for item in paginator.paginate(...):
        item: ListNetworksResponseTypeDef
        print(item)  # (3)
```

1. client: [WickrAdminAPIClient](./client.md)
2. paginator: [ListNetworksPaginator](./paginators.md#listnetworkspaginator)
3. item: `AioPageIterator[ListNetworksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListNetworksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sortFields: str = ...,
    sortDirection: SortDirectionType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListNetworksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListNetworksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNetworksRequestPaginateTypeDef = {  # (1)
    "sortFields": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNetworksRequestPaginateTypeDef](./type_defs.md#listnetworksrequestpaginatetypedef)
## ListSecurityGroupUsersPaginator

Type annotations and code completion for `#!python session.create_client("wickr").get_paginator("list_security_group_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr/paginator/ListSecurityGroupUsers.html#WickrAdminAPI.Paginator.ListSecurityGroupUsers)

```python
# ListSecurityGroupUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_wickr.paginator import ListSecurityGroupUsersPaginator

session = get_session()
async with session.create_client("wickr") as client:  # (1)
    paginator: ListSecurityGroupUsersPaginator = client.get_paginator("list_security_group_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityGroupUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [WickrAdminAPIClient](./client.md)
2. paginator: [ListSecurityGroupUsersPaginator](./paginators.md#listsecuritygroupuserspaginator)
3. item: `AioPageIterator[ListSecurityGroupUsersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSecurityGroupUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkId: str,
    groupId: str,
    sortFields: str = ...,
    sortDirection: SortDirectionType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListSecurityGroupUsersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSecurityGroupUsersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityGroupUsersRequestPaginateTypeDef = {  # (1)
    "networkId": ...,
    "groupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityGroupUsersRequestPaginateTypeDef](./type_defs.md#listsecuritygroupusersrequestpaginatetypedef)
## ListSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("wickr").get_paginator("list_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr/paginator/ListSecurityGroups.html#WickrAdminAPI.Paginator.ListSecurityGroups)

```python
# ListSecurityGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_wickr.paginator import ListSecurityGroupsPaginator

session = get_session()
async with session.create_client("wickr") as client:  # (1)
    paginator: ListSecurityGroupsPaginator = client.get_paginator("list_security_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecurityGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [WickrAdminAPIClient](./client.md)
2. paginator: [ListSecurityGroupsPaginator](./paginators.md#listsecuritygroupspaginator)
3. item: `AioPageIterator[ListSecurityGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSecurityGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkId: str,
    sortFields: str = ...,
    sortDirection: SortDirectionType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListSecurityGroupsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSecurityGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSecurityGroupsRequestPaginateTypeDef = {  # (1)
    "networkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecurityGroupsRequestPaginateTypeDef](./type_defs.md#listsecuritygroupsrequestpaginatetypedef)
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("wickr").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr/paginator/ListUsers.html#WickrAdminAPI.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_wickr.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("wickr") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [WickrAdminAPIClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: `AioPageIterator[ListUsersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    networkId: str,
    sortFields: str = ...,
    sortDirection: SortDirectionType = ...,  # (1)
    firstName: str = ...,
    lastName: str = ...,
    username: str = ...,
    status: int = ...,
    groupId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListUsersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortDirectionType](./literals.md#sortdirectiontype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListUsersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "networkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef)
