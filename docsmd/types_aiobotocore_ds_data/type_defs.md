# Type definitions

> [Index](../README.md) > [DirectoryServiceData](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DirectoryServiceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data.html#directoryservicedata)
    type annotations stubs module [types-aiobotocore-ds-data](https://pypi.org/project/types-aiobotocore-ds-data/).

## AttributeValueUnionTypeDef

```python
# AttributeValueUnionTypeDef definition

AttributeValueUnionTypeDef = Union[
    AttributeValueTypeDef,  # (1)
    AttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 



## AddGroupMemberRequestRequestTypeDef

```python
# AddGroupMemberRequestRequestTypeDef definition

class AddGroupMemberRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    GroupName: str,
    MemberName: str,
    ClientToken: NotRequired[str],
    MemberRealm: NotRequired[str],
```

## AttributeValueOutputTypeDef

```python
# AttributeValueOutputTypeDef definition

class AttributeValueOutputTypeDef(TypedDict):
    BOOL: NotRequired[bool],
    N: NotRequired[int],
    S: NotRequired[str],
    SS: NotRequired[List[str]],
```

## AttributeValueTypeDef

```python
# AttributeValueTypeDef definition

class AttributeValueTypeDef(TypedDict):
    BOOL: NotRequired[bool],
    N: NotRequired[int],
    S: NotRequired[str],
    SS: NotRequired[Sequence[str]],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DeleteGroupRequestRequestTypeDef

```python
# DeleteGroupRequestRequestTypeDef definition

class DeleteGroupRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: NotRequired[str],
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: NotRequired[str],
```

## DescribeGroupRequestRequestTypeDef

```python
# DescribeGroupRequestRequestTypeDef definition

class DescribeGroupRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    OtherAttributes: NotRequired[Sequence[str]],
    Realm: NotRequired[str],
```

## DescribeUserRequestRequestTypeDef

```python
# DescribeUserRequestRequestTypeDef definition

class DescribeUserRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    OtherAttributes: NotRequired[Sequence[str]],
    Realm: NotRequired[str],
```

## DisableUserRequestRequestTypeDef

```python
# DisableUserRequestRequestTypeDef definition

class DisableUserRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: NotRequired[str],
```

## GroupSummaryTypeDef

```python
# GroupSummaryTypeDef definition

class GroupSummaryTypeDef(TypedDict):
    GroupScope: GroupScopeType,  # (1)
    GroupType: GroupTypeType,  # (2)
    SAMAccountName: str,
    SID: str,
```

1. See [:material-code-brackets: GroupScopeType](./literals.md#groupscopetype) 
2. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListGroupMembersRequestRequestTypeDef

```python
# ListGroupMembersRequestRequestTypeDef definition

class ListGroupMembersRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    MaxResults: NotRequired[int],
    MemberRealm: NotRequired[str],
    NextToken: NotRequired[str],
    Realm: NotRequired[str],
```

## MemberTypeDef

```python
# MemberTypeDef definition

class MemberTypeDef(TypedDict):
    MemberType: MemberTypeType,  # (1)
    SAMAccountName: str,
    SID: str,
```

1. See [:material-code-brackets: MemberTypeType](./literals.md#membertypetype) 
## ListGroupsForMemberRequestRequestTypeDef

```python
# ListGroupsForMemberRequestRequestTypeDef definition

class ListGroupsForMemberRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    MaxResults: NotRequired[int],
    MemberRealm: NotRequired[str],
    NextToken: NotRequired[str],
    Realm: NotRequired[str],
```

## ListGroupsRequestRequestTypeDef

```python
# ListGroupsRequestRequestTypeDef definition

class ListGroupsRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Realm: NotRequired[str],
```

## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Realm: NotRequired[str],
```

## UserSummaryTypeDef

```python
# UserSummaryTypeDef definition

class UserSummaryTypeDef(TypedDict):
    Enabled: bool,
    SAMAccountName: str,
    SID: str,
    GivenName: NotRequired[str],
    Surname: NotRequired[str],
```

## RemoveGroupMemberRequestRequestTypeDef

```python
# RemoveGroupMemberRequestRequestTypeDef definition

class RemoveGroupMemberRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    GroupName: str,
    MemberName: str,
    ClientToken: NotRequired[str],
    MemberRealm: NotRequired[str],
```

## SearchGroupsRequestRequestTypeDef

```python
# SearchGroupsRequestRequestTypeDef definition

class SearchGroupsRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SearchAttributes: Sequence[str],
    SearchString: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Realm: NotRequired[str],
```

## SearchUsersRequestRequestTypeDef

```python
# SearchUsersRequestRequestTypeDef definition

class SearchUsersRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SearchAttributes: Sequence[str],
    SearchString: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Realm: NotRequired[str],
```

## GroupTypeDef

```python
# GroupTypeDef definition

class GroupTypeDef(TypedDict):
    SAMAccountName: str,
    DistinguishedName: NotRequired[str],
    GroupScope: NotRequired[GroupScopeType],  # (1)
    GroupType: NotRequired[GroupTypeType],  # (2)
    OtherAttributes: NotRequired[Dict[str, AttributeValueOutputTypeDef]],  # (3)
    SID: NotRequired[str],
```

1. See [:material-code-brackets: GroupScopeType](./literals.md#groupscopetype) 
2. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
3. See [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    SAMAccountName: str,
    DistinguishedName: NotRequired[str],
    EmailAddress: NotRequired[str],
    Enabled: NotRequired[bool],
    GivenName: NotRequired[str],
    OtherAttributes: NotRequired[Dict[str, AttributeValueOutputTypeDef]],  # (1)
    SID: NotRequired[str],
    Surname: NotRequired[str],
    UserPrincipalName: NotRequired[str],
```

1. See [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: NotRequired[str],
    EmailAddress: NotRequired[str],
    GivenName: NotRequired[str],
    OtherAttributes: NotRequired[Mapping[str, AttributeValueTypeDef]],  # (1)
    Surname: NotRequired[str],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## UpdateGroupRequestRequestTypeDef

```python
# UpdateGroupRequestRequestTypeDef definition

class UpdateGroupRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: NotRequired[str],
    GroupScope: NotRequired[GroupScopeType],  # (1)
    GroupType: NotRequired[GroupTypeType],  # (2)
    OtherAttributes: NotRequired[Mapping[str, AttributeValueTypeDef]],  # (3)
    UpdateType: NotRequired[UpdateTypeType],  # (4)
```

1. See [:material-code-brackets: GroupScopeType](./literals.md#groupscopetype) 
2. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
3. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
4. See [:material-code-brackets: UpdateTypeType](./literals.md#updatetypetype) 
## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: NotRequired[str],
    EmailAddress: NotRequired[str],
    GivenName: NotRequired[str],
    OtherAttributes: NotRequired[Mapping[str, AttributeValueTypeDef]],  # (1)
    Surname: NotRequired[str],
    UpdateType: NotRequired[UpdateTypeType],  # (2)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: UpdateTypeType](./literals.md#updatetypetype) 
## CreateGroupResultTypeDef

```python
# CreateGroupResultTypeDef definition

class CreateGroupResultTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    SID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserResultTypeDef

```python
# CreateUserResultTypeDef definition

class CreateUserResultTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    SID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGroupResultTypeDef

```python
# DescribeGroupResultTypeDef definition

class DescribeGroupResultTypeDef(TypedDict):
    DirectoryId: str,
    DistinguishedName: str,
    GroupScope: GroupScopeType,  # (1)
    GroupType: GroupTypeType,  # (2)
    OtherAttributes: Dict[str, AttributeValueOutputTypeDef],  # (3)
    Realm: str,
    SAMAccountName: str,
    SID: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: GroupScopeType](./literals.md#groupscopetype) 
2. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
3. See [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserResultTypeDef

```python
# DescribeUserResultTypeDef definition

class DescribeUserResultTypeDef(TypedDict):
    DirectoryId: str,
    DistinguishedName: str,
    EmailAddress: str,
    Enabled: bool,
    GivenName: str,
    OtherAttributes: Dict[str, AttributeValueOutputTypeDef],  # (1)
    Realm: str,
    SAMAccountName: str,
    SID: str,
    Surname: str,
    UserPrincipalName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupsForMemberResultTypeDef

```python
# ListGroupsForMemberResultTypeDef definition

class ListGroupsForMemberResultTypeDef(TypedDict):
    DirectoryId: str,
    Groups: List[GroupSummaryTypeDef],  # (1)
    MemberRealm: str,
    Realm: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupsResultTypeDef

```python
# ListGroupsResultTypeDef definition

class ListGroupsResultTypeDef(TypedDict):
    DirectoryId: str,
    Groups: List[GroupSummaryTypeDef],  # (1)
    Realm: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupMembersRequestPaginateTypeDef

```python
# ListGroupMembersRequestPaginateTypeDef definition

class ListGroupMembersRequestPaginateTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    MemberRealm: NotRequired[str],
    Realm: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsForMemberRequestPaginateTypeDef

```python
# ListGroupsForMemberRequestPaginateTypeDef definition

class ListGroupsForMemberRequestPaginateTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    MemberRealm: NotRequired[str],
    Realm: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsRequestPaginateTypeDef

```python
# ListGroupsRequestPaginateTypeDef definition

class ListGroupsRequestPaginateTypeDef(TypedDict):
    DirectoryId: str,
    Realm: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestPaginateTypeDef

```python
# ListUsersRequestPaginateTypeDef definition

class ListUsersRequestPaginateTypeDef(TypedDict):
    DirectoryId: str,
    Realm: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchGroupsRequestPaginateTypeDef

```python
# SearchGroupsRequestPaginateTypeDef definition

class SearchGroupsRequestPaginateTypeDef(TypedDict):
    DirectoryId: str,
    SearchAttributes: Sequence[str],
    SearchString: str,
    Realm: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchUsersRequestPaginateTypeDef

```python
# SearchUsersRequestPaginateTypeDef definition

class SearchUsersRequestPaginateTypeDef(TypedDict):
    DirectoryId: str,
    SearchAttributes: Sequence[str],
    SearchString: str,
    Realm: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupMembersResultTypeDef

```python
# ListGroupMembersResultTypeDef definition

class ListGroupMembersResultTypeDef(TypedDict):
    DirectoryId: str,
    MemberRealm: str,
    Members: List[MemberTypeDef],  # (1)
    Realm: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResultTypeDef

```python
# ListUsersResultTypeDef definition

class ListUsersResultTypeDef(TypedDict):
    DirectoryId: str,
    Realm: str,
    Users: List[UserSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserSummaryTypeDef](./type_defs.md#usersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchGroupsResultTypeDef

```python
# SearchGroupsResultTypeDef definition

class SearchGroupsResultTypeDef(TypedDict):
    DirectoryId: str,
    Groups: List[GroupTypeDef],  # (1)
    Realm: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchUsersResultTypeDef

```python
# SearchUsersResultTypeDef definition

class SearchUsersResultTypeDef(TypedDict):
    DirectoryId: str,
    Realm: str,
    Users: List[UserTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupRequestRequestTypeDef

```python
# CreateGroupRequestRequestTypeDef definition

class CreateGroupRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    SAMAccountName: str,
    ClientToken: NotRequired[str],
    GroupScope: NotRequired[GroupScopeType],  # (1)
    GroupType: NotRequired[GroupTypeType],  # (2)
    OtherAttributes: NotRequired[Mapping[str, AttributeValueUnionTypeDef]],  # (3)
```

1. See [:material-code-brackets: GroupScopeType](./literals.md#groupscopetype) 
2. See [:material-code-brackets: GroupTypeType](./literals.md#grouptypetype) 
3. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) [:material-code-braces: AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef) 
