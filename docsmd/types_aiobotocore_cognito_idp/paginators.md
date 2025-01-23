# Paginators

> [Index](../README.md) > [CognitoIdentityProvider](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CognitoIdentityProvider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#cognitoidentityprovider)
    type annotations stubs module [types-aiobotocore-cognito-idp](https://pypi.org/project/types-aiobotocore-cognito-idp/).

## AdminListGroupsForUserPaginator

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_paginator("admin_list_groups_for_user")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/paginator/AdminListGroupsForUser.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)

```python
# AdminListGroupsForUserPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import AdminListGroupsForUserPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:  # (1)
    paginator: AdminListGroupsForUserPaginator = client.get_paginator("admin_list_groups_for_user")  # (2)
    async for item in paginator.paginate(...):
        item: AdminListGroupsForUserResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [AdminListGroupsForUserPaginator](./paginators.md#adminlistgroupsforuserpaginator)
3. item: [:material-code-braces: AdminListGroupsForUserResponseTypeDef](./type_defs.md#adminlistgroupsforuserresponsetypedef) 


### paginate

Type annotations and code completion for `#!python AdminListGroupsForUserPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Username: str,
    UserPoolId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[AdminListGroupsForUserResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: AdminListGroupsForUserResponseTypeDef](./type_defs.md#adminlistgroupsforuserresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: AdminListGroupsForUserRequestPaginateTypeDef = {  # (1)
    "Username": ...,
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: AdminListGroupsForUserRequestPaginateTypeDef](./type_defs.md#adminlistgroupsforuserrequestpaginatetypedef) 
## AdminListUserAuthEventsPaginator

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_paginator("admin_list_user_auth_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/paginator/AdminListUserAuthEvents.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)

```python
# AdminListUserAuthEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import AdminListUserAuthEventsPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:  # (1)
    paginator: AdminListUserAuthEventsPaginator = client.get_paginator("admin_list_user_auth_events")  # (2)
    async for item in paginator.paginate(...):
        item: AdminListUserAuthEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [AdminListUserAuthEventsPaginator](./paginators.md#adminlistuserautheventspaginator)
3. item: [:material-code-braces: AdminListUserAuthEventsResponseTypeDef](./type_defs.md#adminlistuserautheventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python AdminListUserAuthEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserPoolId: str,
    Username: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[AdminListUserAuthEventsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: AdminListUserAuthEventsResponseTypeDef](./type_defs.md#adminlistuserautheventsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: AdminListUserAuthEventsRequestPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
    "Username": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: AdminListUserAuthEventsRequestPaginateTypeDef](./type_defs.md#adminlistuserautheventsrequestpaginatetypedef) 
## ListGroupsPaginator

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_paginator("list_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/paginator/ListGroups.html#CognitoIdentityProvider.Paginator.ListGroups)

```python
# ListGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListGroupsPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:  # (1)
    paginator: ListGroupsPaginator = client.get_paginator("list_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListGroupsPaginator](./paginators.md#listgroupspaginator)
3. item: [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserPoolId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGroupsRequestPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestPaginateTypeDef](./type_defs.md#listgroupsrequestpaginatetypedef) 
## ListIdentityProvidersPaginator

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_paginator("list_identity_providers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/paginator/ListIdentityProviders.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)

```python
# ListIdentityProvidersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListIdentityProvidersPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:  # (1)
    paginator: ListIdentityProvidersPaginator = client.get_paginator("list_identity_providers")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdentityProvidersResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListIdentityProvidersPaginator](./paginators.md#listidentityproviderspaginator)
3. item: [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIdentityProvidersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserPoolId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListIdentityProvidersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdentityProvidersResponseTypeDef](./type_defs.md#listidentityprovidersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdentityProvidersRequestPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdentityProvidersRequestPaginateTypeDef](./type_defs.md#listidentityprovidersrequestpaginatetypedef) 
## ListResourceServersPaginator

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_paginator("list_resource_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/paginator/ListResourceServers.html#CognitoIdentityProvider.Paginator.ListResourceServers)

```python
# ListResourceServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListResourceServersPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:  # (1)
    paginator: ListResourceServersPaginator = client.get_paginator("list_resource_servers")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceServersResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListResourceServersPaginator](./paginators.md#listresourceserverspaginator)
3. item: [:material-code-braces: ListResourceServersResponseTypeDef](./type_defs.md#listresourceserversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserPoolId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResourceServersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceServersResponseTypeDef](./type_defs.md#listresourceserversresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceServersRequestPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceServersRequestPaginateTypeDef](./type_defs.md#listresourceserversrequestpaginatetypedef) 
## ListUserPoolClientsPaginator

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_paginator("list_user_pool_clients")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/paginator/ListUserPoolClients.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)

```python
# ListUserPoolClientsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListUserPoolClientsPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:  # (1)
    paginator: ListUserPoolClientsPaginator = client.get_paginator("list_user_pool_clients")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserPoolClientsResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListUserPoolClientsPaginator](./paginators.md#listuserpoolclientspaginator)
3. item: [:material-code-braces: ListUserPoolClientsResponseTypeDef](./type_defs.md#listuserpoolclientsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUserPoolClientsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserPoolId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListUserPoolClientsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUserPoolClientsResponseTypeDef](./type_defs.md#listuserpoolclientsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUserPoolClientsRequestPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserPoolClientsRequestPaginateTypeDef](./type_defs.md#listuserpoolclientsrequestpaginatetypedef) 
## ListUserPoolsPaginator

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_paginator("list_user_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/paginator/ListUserPools.html#CognitoIdentityProvider.Paginator.ListUserPools)

```python
# ListUserPoolsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListUserPoolsPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:  # (1)
    paginator: ListUserPoolsPaginator = client.get_paginator("list_user_pools")  # (2)
    async for item in paginator.paginate(...):
        item: ListUserPoolsResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListUserPoolsPaginator](./paginators.md#listuserpoolspaginator)
3. item: [:material-code-braces: ListUserPoolsResponseTypeDef](./type_defs.md#listuserpoolsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUserPoolsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListUserPoolsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUserPoolsResponseTypeDef](./type_defs.md#listuserpoolsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUserPoolsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUserPoolsRequestPaginateTypeDef](./type_defs.md#listuserpoolsrequestpaginatetypedef) 
## ListUsersInGroupPaginator

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_paginator("list_users_in_group")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/paginator/ListUsersInGroup.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)

```python
# ListUsersInGroupPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListUsersInGroupPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:  # (1)
    paginator: ListUsersInGroupPaginator = client.get_paginator("list_users_in_group")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersInGroupResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListUsersInGroupPaginator](./paginators.md#listusersingrouppaginator)
3. item: [:material-code-braces: ListUsersInGroupResponseTypeDef](./type_defs.md#listusersingroupresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersInGroupPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserPoolId: str,
    GroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListUsersInGroupResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersInGroupResponseTypeDef](./type_defs.md#listusersingroupresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersInGroupRequestPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
    "GroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersInGroupRequestPaginateTypeDef](./type_defs.md#listusersingrouprequestpaginatetypedef) 
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("cognito-idp").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/paginator/ListUsers.html#CognitoIdentityProvider.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("cognito-idp") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    UserPoolId: str,
    AttributesToGet: Sequence[str] = ...,
    Filter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "UserPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef) 
