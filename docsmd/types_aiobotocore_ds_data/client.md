# DirectoryServiceDataClient

> [Index](../README.md) > [DirectoryServiceData](./README.md) > DirectoryServiceDataClient

!!! note ""

    Auto-generated documentation for [DirectoryServiceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data.html#directoryservicedata)
    type annotations stubs module [types-aiobotocore-ds-data](https://pypi.org/project/types-aiobotocore-ds-data/).

## DirectoryServiceDataClient

Type annotations and code completion for `#!python session.create_client("ds-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data.html#DirectoryServiceData.Client)

```python
# DirectoryServiceDataClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_ds_data.client import DirectoryServiceDataClient

session = get_session()
async with session.create_client("ds-data") as client:
    client: DirectoryServiceDataClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("ds-data").exceptions` structure.

```python
# DirectoryServiceDataClient.exceptions usage example

async with session.create_client("ds-data") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.DirectoryUnavailableException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# DirectoryServiceDataClient usage type checking example

from types_aiobotocore_ds_data.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("ds-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("ds-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### close



Type annotations and code completion for `#!python session.create_client("ds-data").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### add\_group\_member

Adds an existing user, group, or computer as a group member.

Type annotations and code completion for `#!python session.create_client("ds-data").add_group_member` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/add_group_member.html)

```python
# add_group_member method definition

await def add_group_member(
    self,
    *,
    DirectoryId: str,
    GroupName: str,
    MemberName: str,
    ClientToken: str = ...,
    MemberRealm: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# add_group_member method usage example with argument unpacking

kwargs: AddGroupMemberRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "GroupName": ...,
    "MemberName": ...,
}

parent.add_group_member(**kwargs)
```

1. See [:material-code-braces: AddGroupMemberRequestRequestTypeDef](./type_defs.md#addgroupmemberrequestrequesttypedef) 

### create\_group

Creates a new group.

Type annotations and code completion for `#!python session.create_client("ds-data").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/create_group.html)

```python
# create_group method definition

await def create_group(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: str = ...,
    GroupScope: GroupScopeType = ...,  # (1)
    GroupType: GroupTypeType = ...,  # (2)
    OtherAttributes: Mapping[str, AttributeValueUnionTypeDef] = ...,  # (3)
) -> CreateGroupResultTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: GroupScopeType](./literals.md#groupscopetype) 
2. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
3. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
4. See [:material-code-braces: CreateGroupResultTypeDef](./type_defs.md#creategroupresulttypedef) 


```python
# create_group method usage example with argument unpacking

kwargs: CreateGroupRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef) 

### create\_user

Creates a new user.

Type annotations and code completion for `#!python session.create_client("ds-data").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/create_user.html)

```python
# create_user method definition

await def create_user(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: str = ...,
    EmailAddress: str = ...,
    GivenName: str = ...,
    OtherAttributes: Mapping[str, AttributeValueTypeDef] = ...,  # (1)
    Surname: str = ...,
) -> CreateUserResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: CreateUserResultTypeDef](./type_defs.md#createuserresulttypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef) 

### delete\_group

Deletes a group.

Type annotations and code completion for `#!python session.create_client("ds-data").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/delete_group.html)

```python
# delete_group method definition

await def delete_group(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_group method usage example with argument unpacking

kwargs: DeleteGroupRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef) 

### delete\_user

Deletes a user.

Type annotations and code completion for `#!python session.create_client("ds-data").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/delete_user.html)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### describe\_group

Returns information about a specific group.

Type annotations and code completion for `#!python session.create_client("ds-data").describe_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/describe_group.html)

```python
# describe_group method definition

await def describe_group(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    OtherAttributes: Sequence[str] = ...,
    Realm: str = ...,
) -> DescribeGroupResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGroupResultTypeDef](./type_defs.md#describegroupresulttypedef) 


```python
# describe_group method usage example with argument unpacking

kwargs: DescribeGroupRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.describe_group(**kwargs)
```

1. See [:material-code-braces: DescribeGroupRequestRequestTypeDef](./type_defs.md#describegrouprequestrequesttypedef) 

### describe\_user

Returns information about a specific user.

Type annotations and code completion for `#!python session.create_client("ds-data").describe_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/describe_user.html)

```python
# describe_user method definition

await def describe_user(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    OtherAttributes: Sequence[str] = ...,
    Realm: str = ...,
) -> DescribeUserResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserResultTypeDef](./type_defs.md#describeuserresulttypedef) 


```python
# describe_user method usage example with argument unpacking

kwargs: DescribeUserRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.describe_user(**kwargs)
```

1. See [:material-code-braces: DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef) 

### disable\_user

Deactivates an active user account.

Type annotations and code completion for `#!python session.create_client("ds-data").disable_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/disable_user.html)

```python
# disable_user method definition

await def disable_user(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disable_user method usage example with argument unpacking

kwargs: DisableUserRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.disable_user(**kwargs)
```

1. See [:material-code-braces: DisableUserRequestRequestTypeDef](./type_defs.md#disableuserrequestrequesttypedef) 

### list\_group\_members

Returns member information for the specified group.

Type annotations and code completion for `#!python session.create_client("ds-data").list_group_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/list_group_members.html)

```python
# list_group_members method definition

await def list_group_members(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    MaxResults: int = ...,
    MemberRealm: str = ...,
    NextToken: str = ...,
    Realm: str = ...,
) -> ListGroupMembersResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupMembersResultTypeDef](./type_defs.md#listgroupmembersresulttypedef) 


```python
# list_group_members method usage example with argument unpacking

kwargs: ListGroupMembersRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.list_group_members(**kwargs)
```

1. See [:material-code-braces: ListGroupMembersRequestRequestTypeDef](./type_defs.md#listgroupmembersrequestrequesttypedef) 

### list\_groups

Returns group information for the specified directory.

Type annotations and code completion for `#!python session.create_client("ds-data").list_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/list_groups.html)

```python
# list_groups method definition

await def list_groups(
    self,
    *,
    DirectoryId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Realm: str = ...,
) -> ListGroupsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupsResultTypeDef](./type_defs.md#listgroupsresulttypedef) 


```python
# list_groups method usage example with argument unpacking

kwargs: ListGroupsRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.list_groups(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef) 

### list\_groups\_for\_member

Returns group information for the specified member.

Type annotations and code completion for `#!python session.create_client("ds-data").list_groups_for_member` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/list_groups_for_member.html)

```python
# list_groups_for_member method definition

await def list_groups_for_member(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    MaxResults: int = ...,
    MemberRealm: str = ...,
    NextToken: str = ...,
    Realm: str = ...,
) -> ListGroupsForMemberResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupsForMemberResultTypeDef](./type_defs.md#listgroupsformemberresulttypedef) 


```python
# list_groups_for_member method usage example with argument unpacking

kwargs: ListGroupsForMemberRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.list_groups_for_member(**kwargs)
```

1. See [:material-code-braces: ListGroupsForMemberRequestRequestTypeDef](./type_defs.md#listgroupsformemberrequestrequesttypedef) 

### list\_users

Returns user information for the specified directory.

Type annotations and code completion for `#!python session.create_client("ds-data").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/list_users.html)

```python
# list_users method definition

await def list_users(
    self,
    *,
    DirectoryId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Realm: str = ...,
) -> ListUsersResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUsersResultTypeDef](./type_defs.md#listusersresulttypedef) 


```python
# list_users method usage example with argument unpacking

kwargs: ListUsersRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.list_users(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef) 

### remove\_group\_member

Removes a member from a group.

Type annotations and code completion for `#!python session.create_client("ds-data").remove_group_member` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/remove_group_member.html)

```python
# remove_group_member method definition

await def remove_group_member(
    self,
    *,
    DirectoryId: str,
    GroupName: str,
    MemberName: str,
    ClientToken: str = ...,
    MemberRealm: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# remove_group_member method usage example with argument unpacking

kwargs: RemoveGroupMemberRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "GroupName": ...,
    "MemberName": ...,
}

parent.remove_group_member(**kwargs)
```

1. See [:material-code-braces: RemoveGroupMemberRequestRequestTypeDef](./type_defs.md#removegroupmemberrequestrequesttypedef) 

### search\_groups

Searches the specified directory for a group.

Type annotations and code completion for `#!python session.create_client("ds-data").search_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/search_groups.html)

```python
# search_groups method definition

await def search_groups(
    self,
    *,
    DirectoryId: str,
    SearchAttributes: Sequence[str],
    SearchString: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Realm: str = ...,
) -> SearchGroupsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SearchGroupsResultTypeDef](./type_defs.md#searchgroupsresulttypedef) 


```python
# search_groups method usage example with argument unpacking

kwargs: SearchGroupsRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SearchAttributes": ...,
    "SearchString": ...,
}

parent.search_groups(**kwargs)
```

1. See [:material-code-braces: SearchGroupsRequestRequestTypeDef](./type_defs.md#searchgroupsrequestrequesttypedef) 

### search\_users

Searches the specified directory for a user.

Type annotations and code completion for `#!python session.create_client("ds-data").search_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/search_users.html)

```python
# search_users method definition

await def search_users(
    self,
    *,
    DirectoryId: str,
    SearchAttributes: Sequence[str],
    SearchString: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Realm: str = ...,
) -> SearchUsersResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SearchUsersResultTypeDef](./type_defs.md#searchusersresulttypedef) 


```python
# search_users method usage example with argument unpacking

kwargs: SearchUsersRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SearchAttributes": ...,
    "SearchString": ...,
}

parent.search_users(**kwargs)
```

1. See [:material-code-braces: SearchUsersRequestRequestTypeDef](./type_defs.md#searchusersrequestrequesttypedef) 

### update\_group

Updates group information.

Type annotations and code completion for `#!python session.create_client("ds-data").update_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/update_group.html)

```python
# update_group method definition

await def update_group(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: str = ...,
    GroupScope: GroupScopeType = ...,  # (1)
    GroupType: GroupTypeType = ...,  # (2)
    OtherAttributes: Mapping[str, AttributeValueTypeDef] = ...,  # (3)
    UpdateType: UpdateTypeType = ...,  # (4)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: GroupScopeType](./literals.md#groupscopetype) 
2. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
3. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
4. See [:material-code-brackets: UpdateTypeType](./literals.md#updatetypetype) 


```python
# update_group method usage example with argument unpacking

kwargs: UpdateGroupRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.update_group(**kwargs)
```

1. See [:material-code-braces: UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef) 

### update\_user

Updates user information.

Type annotations and code completion for `#!python session.create_client("ds-data").update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data/client/update_user.html)

```python
# update_user method definition

await def update_user(
    self,
    *,
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: str = ...,
    EmailAddress: str = ...,
    GivenName: str = ...,
    OtherAttributes: Mapping[str, AttributeValueTypeDef] = ...,  # (1)
    Surname: str = ...,
    UpdateType: UpdateTypeType = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: UpdateTypeType](./literals.md#updatetypetype) 


```python
# update_user method usage example with argument unpacking

kwargs: UpdateUserRequestRequestTypeDef = {  # (1)
    "DirectoryId": ...,
    "SAMAccountName": ...,
}

parent.update_user(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("ds-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data.html#DirectoryServiceData.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "DirectoryServiceDataClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("ds-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data.html#DirectoryServiceData.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("ds-data").get_paginator` method with overloads.

- `client.get_paginator("list_group_members")` -> [ListGroupMembersPaginator](./paginators.md#listgroupmemberspaginator)
- `client.get_paginator("list_groups_for_member")` -> [ListGroupsForMemberPaginator](./paginators.md#listgroupsformemberpaginator)
- `client.get_paginator("list_groups")` -> [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- `client.get_paginator("list_users")` -> [ListUsersPaginator](./paginators.md#listuserspaginator)
- `client.get_paginator("search_groups")` -> [SearchGroupsPaginator](./paginators.md#searchgroupspaginator)
- `client.get_paginator("search_users")` -> [SearchUsersPaginator](./paginators.md#searchuserspaginator)



