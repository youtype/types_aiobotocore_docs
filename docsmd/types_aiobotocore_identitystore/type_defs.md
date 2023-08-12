# Type definitions

> [Index](../README.md) > [IdentityStore](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IdentityStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
    type annotations stubs module [types-aiobotocore-identitystore](https://pypi.org/project/types-aiobotocore-identitystore/).



## AddressTypeDef

```python
# AddressTypeDef definition

class AddressTypeDef(TypedDict):
    StreetAddress: NotRequired[str],
    Locality: NotRequired[str],
    Region: NotRequired[str],
    PostalCode: NotRequired[str],
    Country: NotRequired[str],
    Formatted: NotRequired[str],
    Type: NotRequired[str],
    Primary: NotRequired[bool],
```

## ExternalIdTypeDef

```python
# ExternalIdTypeDef definition

class ExternalIdTypeDef(TypedDict):
    Issuer: str,
    Id: str,
```

## UniqueAttributeTypeDef

```python
# UniqueAttributeTypeDef definition

class UniqueAttributeTypeDef(TypedDict):
    AttributePath: str,
    AttributeValue: Mapping[str, Any],
```

## AttributeOperationTypeDef

```python
# AttributeOperationTypeDef definition

class AttributeOperationTypeDef(TypedDict):
    AttributePath: str,
    AttributeValue: NotRequired[Mapping[str, Any]],
```

## MemberIdTypeDef

```python
# MemberIdTypeDef definition

class MemberIdTypeDef(TypedDict):
    UserId: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## CreateGroupRequestRequestTypeDef

```python
# CreateGroupRequestRequestTypeDef definition

class CreateGroupRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
```

## EmailTypeDef

```python
# EmailTypeDef definition

class EmailTypeDef(TypedDict):
    Value: NotRequired[str],
    Type: NotRequired[str],
    Primary: NotRequired[bool],
```

## NameTypeDef

```python
# NameTypeDef definition

class NameTypeDef(TypedDict):
    Formatted: NotRequired[str],
    FamilyName: NotRequired[str],
    GivenName: NotRequired[str],
    MiddleName: NotRequired[str],
    HonorificPrefix: NotRequired[str],
    HonorificSuffix: NotRequired[str],
```

## PhoneNumberTypeDef

```python
# PhoneNumberTypeDef definition

class PhoneNumberTypeDef(TypedDict):
    Value: NotRequired[str],
    Type: NotRequired[str],
    Primary: NotRequired[bool],
```

## DeleteGroupMembershipRequestRequestTypeDef

```python
# DeleteGroupMembershipRequestRequestTypeDef definition

class DeleteGroupMembershipRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    MembershipId: str,
```

## DeleteGroupRequestRequestTypeDef

```python
# DeleteGroupRequestRequestTypeDef definition

class DeleteGroupRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    GroupId: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    UserId: str,
```

## DescribeGroupMembershipRequestRequestTypeDef

```python
# DescribeGroupMembershipRequestRequestTypeDef definition

class DescribeGroupMembershipRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    MembershipId: str,
```

## DescribeGroupRequestRequestTypeDef

```python
# DescribeGroupRequestRequestTypeDef definition

class DescribeGroupRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    GroupId: str,
```

## DescribeUserRequestRequestTypeDef

```python
# DescribeUserRequestRequestTypeDef definition

class DescribeUserRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    UserId: str,
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    AttributePath: str,
    AttributeValue: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListGroupMembershipsRequestRequestTypeDef

```python
# ListGroupMembershipsRequestRequestTypeDef definition

class ListGroupMembershipsRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    GroupId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GroupTypeDef

```python
# GroupTypeDef definition

class GroupTypeDef(TypedDict):
    GroupId: str,
    IdentityStoreId: str,
    DisplayName: NotRequired[str],
    ExternalIds: NotRequired[List[ExternalIdTypeDef]],  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ExternalIdTypeDef](./type_defs.md#externalidtypedef) 
## AlternateIdentifierTypeDef

```python
# AlternateIdentifierTypeDef definition

class AlternateIdentifierTypeDef(TypedDict):
    ExternalId: NotRequired[ExternalIdTypeDef],  # (1)
    UniqueAttribute: NotRequired[UniqueAttributeTypeDef],  # (2)
```

1. See [:material-code-braces: ExternalIdTypeDef](./type_defs.md#externalidtypedef) 
2. See [:material-code-braces: UniqueAttributeTypeDef](./type_defs.md#uniqueattributetypedef) 
## UpdateGroupRequestRequestTypeDef

```python
# UpdateGroupRequestRequestTypeDef definition

class UpdateGroupRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    GroupId: str,
    Operations: Sequence[AttributeOperationTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeOperationTypeDef](./type_defs.md#attributeoperationtypedef) 
## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    UserId: str,
    Operations: Sequence[AttributeOperationTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeOperationTypeDef](./type_defs.md#attributeoperationtypedef) 
## CreateGroupMembershipRequestRequestTypeDef

```python
# CreateGroupMembershipRequestRequestTypeDef definition

class CreateGroupMembershipRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    GroupId: str,
    MemberId: MemberIdTypeDef,  # (1)
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
## GetGroupMembershipIdRequestRequestTypeDef

```python
# GetGroupMembershipIdRequestRequestTypeDef definition

class GetGroupMembershipIdRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    GroupId: str,
    MemberId: MemberIdTypeDef,  # (1)
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
## GroupMembershipExistenceResultTypeDef

```python
# GroupMembershipExistenceResultTypeDef definition

class GroupMembershipExistenceResultTypeDef(TypedDict):
    GroupId: NotRequired[str],
    MemberId: NotRequired[MemberIdTypeDef],  # (1)
    MembershipExists: NotRequired[bool],
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
## GroupMembershipTypeDef

```python
# GroupMembershipTypeDef definition

class GroupMembershipTypeDef(TypedDict):
    IdentityStoreId: str,
    MembershipId: NotRequired[str],
    GroupId: NotRequired[str],
    MemberId: NotRequired[MemberIdTypeDef],  # (1)
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
## IsMemberInGroupsRequestRequestTypeDef

```python
# IsMemberInGroupsRequestRequestTypeDef definition

class IsMemberInGroupsRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    MemberId: MemberIdTypeDef,  # (1)
    GroupIds: Sequence[str],
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
## ListGroupMembershipsForMemberRequestRequestTypeDef

```python
# ListGroupMembershipsForMemberRequestRequestTypeDef definition

class ListGroupMembershipsForMemberRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    MemberId: MemberIdTypeDef,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
## CreateGroupMembershipResponseTypeDef

```python
# CreateGroupMembershipResponseTypeDef definition

class CreateGroupMembershipResponseTypeDef(TypedDict):
    MembershipId: str,
    IdentityStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupResponseTypeDef

```python
# CreateGroupResponseTypeDef definition

class CreateGroupResponseTypeDef(TypedDict):
    GroupId: str,
    IdentityStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    UserId: str,
    IdentityStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGroupMembershipResponseTypeDef

```python
# DescribeGroupMembershipResponseTypeDef definition

class DescribeGroupMembershipResponseTypeDef(TypedDict):
    IdentityStoreId: str,
    MembershipId: str,
    GroupId: str,
    MemberId: MemberIdTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGroupResponseTypeDef

```python
# DescribeGroupResponseTypeDef definition

class DescribeGroupResponseTypeDef(TypedDict):
    GroupId: str,
    DisplayName: str,
    ExternalIds: List[ExternalIdTypeDef],  # (1)
    Description: str,
    IdentityStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExternalIdTypeDef](./type_defs.md#externalidtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupIdResponseTypeDef

```python
# GetGroupIdResponseTypeDef definition

class GetGroupIdResponseTypeDef(TypedDict):
    GroupId: str,
    IdentityStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupMembershipIdResponseTypeDef

```python
# GetGroupMembershipIdResponseTypeDef definition

class GetGroupMembershipIdResponseTypeDef(TypedDict):
    MembershipId: str,
    IdentityStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserIdResponseTypeDef

```python
# GetUserIdResponseTypeDef definition

class GetUserIdResponseTypeDef(TypedDict):
    UserId: str,
    IdentityStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    UserName: NotRequired[str],
    Name: NotRequired[NameTypeDef],  # (1)
    DisplayName: NotRequired[str],
    NickName: NotRequired[str],
    ProfileUrl: NotRequired[str],
    Emails: NotRequired[Sequence[EmailTypeDef]],  # (2)
    Addresses: NotRequired[Sequence[AddressTypeDef]],  # (3)
    PhoneNumbers: NotRequired[Sequence[PhoneNumberTypeDef]],  # (4)
    UserType: NotRequired[str],
    Title: NotRequired[str],
    PreferredLanguage: NotRequired[str],
    Locale: NotRequired[str],
    Timezone: NotRequired[str],
```

1. See [:material-code-braces: NameTypeDef](./type_defs.md#nametypedef) 
2. See [:material-code-braces: EmailTypeDef](./type_defs.md#emailtypedef) 
3. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
4. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
## DescribeUserResponseTypeDef

```python
# DescribeUserResponseTypeDef definition

class DescribeUserResponseTypeDef(TypedDict):
    UserName: str,
    UserId: str,
    ExternalIds: List[ExternalIdTypeDef],  # (1)
    Name: NameTypeDef,  # (2)
    DisplayName: str,
    NickName: str,
    ProfileUrl: str,
    Emails: List[EmailTypeDef],  # (3)
    Addresses: List[AddressTypeDef],  # (4)
    PhoneNumbers: List[PhoneNumberTypeDef],  # (5)
    UserType: str,
    Title: str,
    PreferredLanguage: str,
    Locale: str,
    Timezone: str,
    IdentityStoreId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ExternalIdTypeDef](./type_defs.md#externalidtypedef) 
2. See [:material-code-braces: NameTypeDef](./type_defs.md#nametypedef) 
3. See [:material-code-braces: EmailTypeDef](./type_defs.md#emailtypedef) 
4. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
5. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    UserId: str,
    IdentityStoreId: str,
    UserName: NotRequired[str],
    ExternalIds: NotRequired[List[ExternalIdTypeDef]],  # (1)
    Name: NotRequired[NameTypeDef],  # (2)
    DisplayName: NotRequired[str],
    NickName: NotRequired[str],
    ProfileUrl: NotRequired[str],
    Emails: NotRequired[List[EmailTypeDef]],  # (3)
    Addresses: NotRequired[List[AddressTypeDef]],  # (4)
    PhoneNumbers: NotRequired[List[PhoneNumberTypeDef]],  # (5)
    UserType: NotRequired[str],
    Title: NotRequired[str],
    PreferredLanguage: NotRequired[str],
    Locale: NotRequired[str],
    Timezone: NotRequired[str],
```

1. See [:material-code-braces: ExternalIdTypeDef](./type_defs.md#externalidtypedef) 
2. See [:material-code-braces: NameTypeDef](./type_defs.md#nametypedef) 
3. See [:material-code-braces: EmailTypeDef](./type_defs.md#emailtypedef) 
4. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
5. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
## ListGroupsRequestRequestTypeDef

```python
# ListGroupsRequestRequestTypeDef definition

class ListGroupsRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef

```python
# ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef definition

class ListGroupMembershipsForMemberRequestListGroupMembershipsForMemberPaginateTypeDef(TypedDict):
    IdentityStoreId: str,
    MemberId: MemberIdTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MemberIdTypeDef](./type_defs.md#memberidtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef

```python
# ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef definition

class ListGroupMembershipsRequestListGroupMembershipsPaginateTypeDef(TypedDict):
    IdentityStoreId: str,
    GroupId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsRequestListGroupsPaginateTypeDef

```python
# ListGroupsRequestListGroupsPaginateTypeDef definition

class ListGroupsRequestListGroupsPaginateTypeDef(TypedDict):
    IdentityStoreId: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestListUsersPaginateTypeDef

```python
# ListUsersRequestListUsersPaginateTypeDef definition

class ListUsersRequestListUsersPaginateTypeDef(TypedDict):
    IdentityStoreId: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsResponseTypeDef

```python
# ListGroupsResponseTypeDef definition

class ListGroupsResponseTypeDef(TypedDict):
    Groups: List[GroupTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupIdRequestRequestTypeDef

```python
# GetGroupIdRequestRequestTypeDef definition

class GetGroupIdRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    AlternateIdentifier: AlternateIdentifierTypeDef,  # (1)
```

1. See [:material-code-braces: AlternateIdentifierTypeDef](./type_defs.md#alternateidentifiertypedef) 
## GetUserIdRequestRequestTypeDef

```python
# GetUserIdRequestRequestTypeDef definition

class GetUserIdRequestRequestTypeDef(TypedDict):
    IdentityStoreId: str,
    AlternateIdentifier: AlternateIdentifierTypeDef,  # (1)
```

1. See [:material-code-braces: AlternateIdentifierTypeDef](./type_defs.md#alternateidentifiertypedef) 
## IsMemberInGroupsResponseTypeDef

```python
# IsMemberInGroupsResponseTypeDef definition

class IsMemberInGroupsResponseTypeDef(TypedDict):
    Results: List[GroupMembershipExistenceResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupMembershipExistenceResultTypeDef](./type_defs.md#groupmembershipexistenceresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupMembershipsForMemberResponseTypeDef

```python
# ListGroupMembershipsForMemberResponseTypeDef definition

class ListGroupMembershipsForMemberResponseTypeDef(TypedDict):
    GroupMemberships: List[GroupMembershipTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupMembershipTypeDef](./type_defs.md#groupmembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupMembershipsResponseTypeDef

```python
# ListGroupMembershipsResponseTypeDef definition

class ListGroupMembershipsResponseTypeDef(TypedDict):
    GroupMemberships: List[GroupMembershipTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupMembershipTypeDef](./type_defs.md#groupmembershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python
# ListUsersResponseTypeDef definition

class ListUsersResponseTypeDef(TypedDict):
    Users: List[UserTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
