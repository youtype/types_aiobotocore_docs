# IdentityStoreClient

> [Index](../README.md) > [IdentityStore](./README.md) > IdentityStoreClient

!!! note ""

    Auto-generated documentation for [IdentityStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#identitystore)
    type annotations stubs module [types-aiobotocore-identitystore](https://pypi.org/project/types-aiobotocore-identitystore/).

## IdentityStoreClient

Type annotations and code completion for `#!python session.create_client("identitystore")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Client)

```python
# IdentityStoreClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_identitystore.client import IdentityStoreClient

session = get_session()
async with session.create_client("identitystore") as client:
    client: IdentityStoreClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("identitystore").exceptions` structure.

```python
# IdentityStoreClient.exceptions usage example

async with session.create_client("identitystore") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# IdentityStoreClient usage type checking example

from types_aiobotocore_identitystore.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("identitystore").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("identitystore").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/generate_presigned_url.html)

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


### create\_group

Creates a group within the specified identity store.

Type annotations and code completion for `#!python session.create_client("identitystore").create_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/create_group.html)

```python
# create_group method definition

await def create_group(
    self,
    *,
    IdentityStoreId: str,
    DisplayName: str = ...,
    Description: str = ...,
) -> CreateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGroupResponseTypeDef](./type_defs.md#creategroupresponsetypedef) 


```python
# create_group method usage example with argument unpacking

kwargs: CreateGroupRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
}

parent.create_group(**kwargs)
```

1. See [:material-code-braces: CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef) 

### create\_group\_membership

Creates a relationship between a member and a group.

Type annotations and code completion for `#!python session.create_client("identitystore").create_group_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/create_group_membership.html)

```python
# create_group_membership method definition

await def create_group_membership(
    self,
    *,
    IdentityStoreId: str,
    GroupId: str,
    MemberId: MemberIdTypeDef,  # (1)
) -> CreateGroupMembershipResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
2. See [:material-code-braces: CreateGroupMembershipResponseTypeDef](./type_defs.md#creategroupmembershipresponsetypedef) 


```python
# create_group_membership method usage example with argument unpacking

kwargs: CreateGroupMembershipRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "GroupId": ...,
    "MemberId": ...,
}

parent.create_group_membership(**kwargs)
```

1. See [:material-code-braces: CreateGroupMembershipRequestRequestTypeDef](./type_defs.md#creategroupmembershiprequestrequesttypedef) 

### create\_user

Creates a user within the specified identity store.

Type annotations and code completion for `#!python session.create_client("identitystore").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/create_user.html)

```python
# create_user method definition

await def create_user(
    self,
    *,
    IdentityStoreId: str,
    UserName: str = ...,
    Name: NameTypeDef = ...,  # (1)
    DisplayName: str = ...,
    NickName: str = ...,
    ProfileUrl: str = ...,
    Emails: Sequence[EmailTypeDef] = ...,  # (2)
    Addresses: Sequence[AddressTypeDef] = ...,  # (3)
    PhoneNumbers: Sequence[PhoneNumberTypeDef] = ...,  # (4)
    UserType: str = ...,
    Title: str = ...,
    PreferredLanguage: str = ...,
    Locale: str = ...,
    Timezone: str = ...,
) -> CreateUserResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: NameTypeDef](./type_defs.md#nametypedef) 
2. See [:material-code-braces: EmailTypeDef](./type_defs.md#emailtypedef) 
3. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
4. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
5. See [:material-code-braces: CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef) 

### delete\_group

Delete a group within an identity store given <code>GroupId</code>.

Type annotations and code completion for `#!python session.create_client("identitystore").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/delete_group.html)

```python
# delete_group method definition

await def delete_group(
    self,
    *,
    IdentityStoreId: str,
    GroupId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_group method usage example with argument unpacking

kwargs: DeleteGroupRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "GroupId": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef) 

### delete\_group\_membership

Delete a membership within a group given <code>MembershipId</code>.

Type annotations and code completion for `#!python session.create_client("identitystore").delete_group_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/delete_group_membership.html)

```python
# delete_group_membership method definition

await def delete_group_membership(
    self,
    *,
    IdentityStoreId: str,
    MembershipId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_group_membership method usage example with argument unpacking

kwargs: DeleteGroupMembershipRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "MembershipId": ...,
}

parent.delete_group_membership(**kwargs)
```

1. See [:material-code-braces: DeleteGroupMembershipRequestRequestTypeDef](./type_defs.md#deletegroupmembershiprequestrequesttypedef) 

### delete\_user

Deletes a user within an identity store given <code>UserId</code>.

Type annotations and code completion for `#!python session.create_client("identitystore").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/delete_user.html)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    IdentityStoreId: str,
    UserId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "UserId": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### describe\_group

Retrieves the group metadata and attributes from <code>GroupId</code> in an
identity store.

Type annotations and code completion for `#!python session.create_client("identitystore").describe_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/describe_group.html)

```python
# describe_group method definition

await def describe_group(
    self,
    *,
    IdentityStoreId: str,
    GroupId: str,
) -> DescribeGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGroupResponseTypeDef](./type_defs.md#describegroupresponsetypedef) 


```python
# describe_group method usage example with argument unpacking

kwargs: DescribeGroupRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "GroupId": ...,
}

parent.describe_group(**kwargs)
```

1. See [:material-code-braces: DescribeGroupRequestRequestTypeDef](./type_defs.md#describegrouprequestrequesttypedef) 

### describe\_group\_membership

Retrieves membership metadata and attributes from <code>MembershipId</code> in
an identity store.

Type annotations and code completion for `#!python session.create_client("identitystore").describe_group_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/describe_group_membership.html)

```python
# describe_group_membership method definition

await def describe_group_membership(
    self,
    *,
    IdentityStoreId: str,
    MembershipId: str,
) -> DescribeGroupMembershipResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeGroupMembershipResponseTypeDef](./type_defs.md#describegroupmembershipresponsetypedef) 


```python
# describe_group_membership method usage example with argument unpacking

kwargs: DescribeGroupMembershipRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "MembershipId": ...,
}

parent.describe_group_membership(**kwargs)
```

1. See [:material-code-braces: DescribeGroupMembershipRequestRequestTypeDef](./type_defs.md#describegroupmembershiprequestrequesttypedef) 

### describe\_user

Retrieves the user metadata and attributes from the <code>UserId</code> in an
identity store.

Type annotations and code completion for `#!python session.create_client("identitystore").describe_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/describe_user.html)

```python
# describe_user method definition

await def describe_user(
    self,
    *,
    IdentityStoreId: str,
    UserId: str,
) -> DescribeUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef) 


```python
# describe_user method usage example with argument unpacking

kwargs: DescribeUserRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "UserId": ...,
}

parent.describe_user(**kwargs)
```

1. See [:material-code-braces: DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef) 

### get\_group\_id

Retrieves <code>GroupId</code> in an identity store.

Type annotations and code completion for `#!python session.create_client("identitystore").get_group_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/get_group_id.html)

```python
# get_group_id method definition

await def get_group_id(
    self,
    *,
    IdentityStoreId: str,
    AlternateIdentifier: AlternateIdentifierTypeDef,  # (1)
) -> GetGroupIdResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AlternateIdentifierTypeDef](./type_defs.md#alternateidentifiertypedef) 
2. See [:material-code-braces: GetGroupIdResponseTypeDef](./type_defs.md#getgroupidresponsetypedef) 


```python
# get_group_id method usage example with argument unpacking

kwargs: GetGroupIdRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "AlternateIdentifier": ...,
}

parent.get_group_id(**kwargs)
```

1. See [:material-code-braces: GetGroupIdRequestRequestTypeDef](./type_defs.md#getgroupidrequestrequesttypedef) 

### get\_group\_membership\_id

Retrieves the <code>MembershipId</code> in an identity store.

Type annotations and code completion for `#!python session.create_client("identitystore").get_group_membership_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/get_group_membership_id.html)

```python
# get_group_membership_id method definition

await def get_group_membership_id(
    self,
    *,
    IdentityStoreId: str,
    GroupId: str,
    MemberId: MemberIdTypeDef,  # (1)
) -> GetGroupMembershipIdResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
2. See [:material-code-braces: GetGroupMembershipIdResponseTypeDef](./type_defs.md#getgroupmembershipidresponsetypedef) 


```python
# get_group_membership_id method usage example with argument unpacking

kwargs: GetGroupMembershipIdRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "GroupId": ...,
    "MemberId": ...,
}

parent.get_group_membership_id(**kwargs)
```

1. See [:material-code-braces: GetGroupMembershipIdRequestRequestTypeDef](./type_defs.md#getgroupmembershipidrequestrequesttypedef) 

### get\_user\_id

Retrieves the <code>UserId</code> in an identity store.

Type annotations and code completion for `#!python session.create_client("identitystore").get_user_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/get_user_id.html)

```python
# get_user_id method definition

await def get_user_id(
    self,
    *,
    IdentityStoreId: str,
    AlternateIdentifier: AlternateIdentifierTypeDef,  # (1)
) -> GetUserIdResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AlternateIdentifierTypeDef](./type_defs.md#alternateidentifiertypedef) 
2. See [:material-code-braces: GetUserIdResponseTypeDef](./type_defs.md#getuseridresponsetypedef) 


```python
# get_user_id method usage example with argument unpacking

kwargs: GetUserIdRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "AlternateIdentifier": ...,
}

parent.get_user_id(**kwargs)
```

1. See [:material-code-braces: GetUserIdRequestRequestTypeDef](./type_defs.md#getuseridrequestrequesttypedef) 

### is\_member\_in\_groups

Checks the user's membership in all requested groups and returns if the member
exists in all queried groups.

Type annotations and code completion for `#!python session.create_client("identitystore").is_member_in_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/is_member_in_groups.html)

```python
# is_member_in_groups method definition

await def is_member_in_groups(
    self,
    *,
    IdentityStoreId: str,
    MemberId: MemberIdTypeDef,  # (1)
    GroupIds: Sequence[str],
) -> IsMemberInGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
2. See [:material-code-braces: IsMemberInGroupsResponseTypeDef](./type_defs.md#ismemberingroupsresponsetypedef) 


```python
# is_member_in_groups method usage example with argument unpacking

kwargs: IsMemberInGroupsRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "MemberId": ...,
    "GroupIds": ...,
}

parent.is_member_in_groups(**kwargs)
```

1. See [:material-code-braces: IsMemberInGroupsRequestRequestTypeDef](./type_defs.md#ismemberingroupsrequestrequesttypedef) 

### list\_group\_memberships

For the specified group in the specified identity store, returns the list of
all <code>GroupMembership</code> objects and returns results in paginated form.

Type annotations and code completion for `#!python session.create_client("identitystore").list_group_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/list_group_memberships.html)

```python
# list_group_memberships method definition

await def list_group_memberships(
    self,
    *,
    IdentityStoreId: str,
    GroupId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListGroupMembershipsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupMembershipsResponseTypeDef](./type_defs.md#listgroupmembershipsresponsetypedef) 


```python
# list_group_memberships method usage example with argument unpacking

kwargs: ListGroupMembershipsRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "GroupId": ...,
}

parent.list_group_memberships(**kwargs)
```

1. See [:material-code-braces: ListGroupMembershipsRequestRequestTypeDef](./type_defs.md#listgroupmembershipsrequestrequesttypedef) 

### list\_group\_memberships\_for\_member

For the specified member in the specified identity store, returns the list of
all <code>GroupMembership</code> objects and returns results in paginated form.

Type annotations and code completion for `#!python session.create_client("identitystore").list_group_memberships_for_member` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/list_group_memberships_for_member.html)

```python
# list_group_memberships_for_member method definition

await def list_group_memberships_for_member(
    self,
    *,
    IdentityStoreId: str,
    MemberId: MemberIdTypeDef,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListGroupMembershipsForMemberResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
2. See [:material-code-braces: ListGroupMembershipsForMemberResponseTypeDef](./type_defs.md#listgroupmembershipsformemberresponsetypedef) 


```python
# list_group_memberships_for_member method usage example with argument unpacking

kwargs: ListGroupMembershipsForMemberRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "MemberId": ...,
}

parent.list_group_memberships_for_member(**kwargs)
```

1. See [:material-code-braces: ListGroupMembershipsForMemberRequestRequestTypeDef](./type_defs.md#listgroupmembershipsformemberrequestrequesttypedef) 

### list\_groups

Lists all groups in the identity store.

Type annotations and code completion for `#!python session.create_client("identitystore").list_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/list_groups.html)

```python
# list_groups method definition

await def list_groups(
    self,
    *,
    IdentityStoreId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# list_groups method usage example with argument unpacking

kwargs: ListGroupsRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
}

parent.list_groups(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef) 

### list\_users

Lists all users in the identity store.

Type annotations and code completion for `#!python session.create_client("identitystore").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/list_users.html)

```python
# list_users method definition

await def list_users(
    self,
    *,
    IdentityStoreId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
) -> ListUsersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# list_users method usage example with argument unpacking

kwargs: ListUsersRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
}

parent.list_users(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef) 

### update\_group

For the specified group in the specified identity store, updates the group
metadata and attributes.

Type annotations and code completion for `#!python session.create_client("identitystore").update_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/update_group.html)

```python
# update_group method definition

await def update_group(
    self,
    *,
    IdentityStoreId: str,
    GroupId: str,
    Operations: Sequence[AttributeOperationTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AttributeOperationTypeDef](./type_defs.md#attributeoperationtypedef) 


```python
# update_group method usage example with argument unpacking

kwargs: UpdateGroupRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "GroupId": ...,
    "Operations": ...,
}

parent.update_group(**kwargs)
```

1. See [:material-code-braces: UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef) 

### update\_user

For the specified user in the specified identity store, updates the user
metadata and attributes.

Type annotations and code completion for `#!python session.create_client("identitystore").update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore/client/update_user.html)

```python
# update_user method definition

await def update_user(
    self,
    *,
    IdentityStoreId: str,
    UserId: str,
    Operations: Sequence[AttributeOperationTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AttributeOperationTypeDef](./type_defs.md#attributeoperationtypedef) 


```python
# update_user method usage example with argument unpacking

kwargs: UpdateUserRequestRequestTypeDef = {  # (1)
    "IdentityStoreId": ...,
    "UserId": ...,
    "Operations": ...,
}

parent.update_user(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("identitystore").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("identitystore").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("identitystore").get_paginator` method with overloads.

- `client.get_paginator("list_group_memberships_for_member")` -> [ListGroupMembershipsForMemberPaginator](./paginators.md#listgroupmembershipsformemberpaginator)
- `client.get_paginator("list_group_memberships")` -> [ListGroupMembershipsPaginator](./paginators.md#listgroupmembershipspaginator)
- `client.get_paginator("list_groups")` -> [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- `client.get_paginator("list_users")` -> [ListUsersPaginator](./paginators.md#listuserspaginator)



