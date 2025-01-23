# Type definitions

> [Index](../README.md) > [WorkDocs](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WorkDocs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#workdocs)
    type annotations stubs module [types-aiobotocore-workdocs](https://pypi.org/project/types-aiobotocore-workdocs/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AbortDocumentVersionUploadRequestRequestTypeDef

```python
# AbortDocumentVersionUploadRequestRequestTypeDef definition

class AbortDocumentVersionUploadRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    VersionId: str,
    AuthenticationToken: NotRequired[str],
```

## ActivateUserRequestRequestTypeDef

```python
# ActivateUserRequestRequestTypeDef definition

class ActivateUserRequestRequestTypeDef(TypedDict):
    UserId: str,
    AuthenticationToken: NotRequired[str],
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

## UserMetadataTypeDef

```python
# UserMetadataTypeDef definition

class UserMetadataTypeDef(TypedDict):
    Id: NotRequired[str],
    Username: NotRequired[str],
    GivenName: NotRequired[str],
    Surname: NotRequired[str],
    EmailAddress: NotRequired[str],
```

## NotificationOptionsTypeDef

```python
# NotificationOptionsTypeDef definition

class NotificationOptionsTypeDef(TypedDict):
    SendEmail: NotRequired[bool],
    EmailMessage: NotRequired[str],
```

## SharePrincipalTypeDef

```python
# SharePrincipalTypeDef definition

class SharePrincipalTypeDef(TypedDict):
    Id: str,
    Type: PrincipalTypeType,  # (1)
    Role: RoleTypeType,  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: RoleTypeType](./literals.md#roletypetype) 
## ShareResultTypeDef

```python
# ShareResultTypeDef definition

class ShareResultTypeDef(TypedDict):
    PrincipalId: NotRequired[str],
    InviteePrincipalId: NotRequired[str],
    Role: NotRequired[RoleTypeType],  # (1)
    Status: NotRequired[ShareStatusTypeType],  # (2)
    ShareId: NotRequired[str],
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: RoleTypeType](./literals.md#roletypetype) 
2. See [:material-code-brackets: ShareStatusTypeType](./literals.md#sharestatustypetype) 
## CreateCommentRequestRequestTypeDef

```python
# CreateCommentRequestRequestTypeDef definition

class CreateCommentRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    VersionId: str,
    Text: str,
    AuthenticationToken: NotRequired[str],
    ParentId: NotRequired[str],
    ThreadId: NotRequired[str],
    Visibility: NotRequired[CommentVisibilityTypeType],  # (1)
    NotifyCollaborators: NotRequired[bool],
```

1. See [:material-code-brackets: CommentVisibilityTypeType](./literals.md#commentvisibilitytypetype) 
## CreateCustomMetadataRequestRequestTypeDef

```python
# CreateCustomMetadataRequestRequestTypeDef definition

class CreateCustomMetadataRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    CustomMetadata: Mapping[str, str],
    AuthenticationToken: NotRequired[str],
    VersionId: NotRequired[str],
```

## CreateFolderRequestRequestTypeDef

```python
# CreateFolderRequestRequestTypeDef definition

class CreateFolderRequestRequestTypeDef(TypedDict):
    ParentFolderId: str,
    AuthenticationToken: NotRequired[str],
    Name: NotRequired[str],
```

## FolderMetadataTypeDef

```python
# FolderMetadataTypeDef definition

class FolderMetadataTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    CreatorId: NotRequired[str],
    ParentFolderId: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    ModifiedTimestamp: NotRequired[datetime],
    ResourceState: NotRequired[ResourceStateTypeType],  # (1)
    Signature: NotRequired[str],
    Labels: NotRequired[List[str]],
    Size: NotRequired[int],
    LatestVersionSize: NotRequired[int],
```

1. See [:material-code-brackets: ResourceStateTypeType](./literals.md#resourcestatetypetype) 
## CreateLabelsRequestRequestTypeDef

```python
# CreateLabelsRequestRequestTypeDef definition

class CreateLabelsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    Labels: Sequence[str],
    AuthenticationToken: NotRequired[str],
```

## CreateNotificationSubscriptionRequestRequestTypeDef

```python
# CreateNotificationSubscriptionRequestRequestTypeDef definition

class CreateNotificationSubscriptionRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Endpoint: str,
    Protocol: SubscriptionProtocolTypeType,  # (1)
    SubscriptionType: SubscriptionTypeType,  # (2)
```

1. See [:material-code-brackets: SubscriptionProtocolTypeType](./literals.md#subscriptionprotocoltypetype) 
2. See [:material-code-brackets: SubscriptionTypeType](./literals.md#subscriptiontypetype) 
## SubscriptionTypeDef

```python
# SubscriptionTypeDef definition

class SubscriptionTypeDef(TypedDict):
    SubscriptionId: NotRequired[str],
    EndPoint: NotRequired[str],
    Protocol: NotRequired[SubscriptionProtocolTypeType],  # (1)
```

1. See [:material-code-brackets: SubscriptionProtocolTypeType](./literals.md#subscriptionprotocoltypetype) 
## StorageRuleTypeTypeDef

```python
# StorageRuleTypeTypeDef definition

class StorageRuleTypeTypeDef(TypedDict):
    StorageAllocatedInBytes: NotRequired[int],
    StorageType: NotRequired[StorageTypeType],  # (1)
```

1. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
## DeactivateUserRequestRequestTypeDef

```python
# DeactivateUserRequestRequestTypeDef definition

class DeactivateUserRequestRequestTypeDef(TypedDict):
    UserId: str,
    AuthenticationToken: NotRequired[str],
```

## DeleteCommentRequestRequestTypeDef

```python
# DeleteCommentRequestRequestTypeDef definition

class DeleteCommentRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    VersionId: str,
    CommentId: str,
    AuthenticationToken: NotRequired[str],
```

## DeleteCustomMetadataRequestRequestTypeDef

```python
# DeleteCustomMetadataRequestRequestTypeDef definition

class DeleteCustomMetadataRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    AuthenticationToken: NotRequired[str],
    VersionId: NotRequired[str],
    Keys: NotRequired[Sequence[str]],
    DeleteAll: NotRequired[bool],
```

## DeleteDocumentRequestRequestTypeDef

```python
# DeleteDocumentRequestRequestTypeDef definition

class DeleteDocumentRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    AuthenticationToken: NotRequired[str],
```

## DeleteDocumentVersionRequestRequestTypeDef

```python
# DeleteDocumentVersionRequestRequestTypeDef definition

class DeleteDocumentVersionRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    VersionId: str,
    DeletePriorVersions: bool,
    AuthenticationToken: NotRequired[str],
```

## DeleteFolderContentsRequestRequestTypeDef

```python
# DeleteFolderContentsRequestRequestTypeDef definition

class DeleteFolderContentsRequestRequestTypeDef(TypedDict):
    FolderId: str,
    AuthenticationToken: NotRequired[str],
```

## DeleteFolderRequestRequestTypeDef

```python
# DeleteFolderRequestRequestTypeDef definition

class DeleteFolderRequestRequestTypeDef(TypedDict):
    FolderId: str,
    AuthenticationToken: NotRequired[str],
```

## DeleteLabelsRequestRequestTypeDef

```python
# DeleteLabelsRequestRequestTypeDef definition

class DeleteLabelsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    AuthenticationToken: NotRequired[str],
    Labels: NotRequired[Sequence[str]],
    DeleteAll: NotRequired[bool],
```

## DeleteNotificationSubscriptionRequestRequestTypeDef

```python
# DeleteNotificationSubscriptionRequestRequestTypeDef definition

class DeleteNotificationSubscriptionRequestRequestTypeDef(TypedDict):
    SubscriptionId: str,
    OrganizationId: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    UserId: str,
    AuthenticationToken: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeCommentsRequestRequestTypeDef

```python
# DescribeCommentsRequestRequestTypeDef definition

class DescribeCommentsRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    VersionId: str,
    AuthenticationToken: NotRequired[str],
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeDocumentVersionsRequestRequestTypeDef

```python
# DescribeDocumentVersionsRequestRequestTypeDef definition

class DescribeDocumentVersionsRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    AuthenticationToken: NotRequired[str],
    Marker: NotRequired[str],
    Limit: NotRequired[int],
    Include: NotRequired[str],
    Fields: NotRequired[str],
```

## DocumentVersionMetadataTypeDef

```python
# DocumentVersionMetadataTypeDef definition

class DocumentVersionMetadataTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    ContentType: NotRequired[str],
    Size: NotRequired[int],
    Signature: NotRequired[str],
    Status: NotRequired[DocumentStatusTypeType],  # (1)
    CreatedTimestamp: NotRequired[datetime],
    ModifiedTimestamp: NotRequired[datetime],
    ContentCreatedTimestamp: NotRequired[datetime],
    ContentModifiedTimestamp: NotRequired[datetime],
    CreatorId: NotRequired[str],
    Thumbnail: NotRequired[Dict[DocumentThumbnailTypeType, str]],  # (2)
    Source: NotRequired[Dict[DocumentSourceTypeType, str]],  # (3)
```

1. See [:material-code-brackets: DocumentStatusTypeType](./literals.md#documentstatustypetype) 
2. See [:material-code-brackets: DocumentThumbnailTypeType](./literals.md#documentthumbnailtypetype) 
3. See [:material-code-brackets: DocumentSourceTypeType](./literals.md#documentsourcetypetype) 
## DescribeFolderContentsRequestRequestTypeDef

```python
# DescribeFolderContentsRequestRequestTypeDef definition

class DescribeFolderContentsRequestRequestTypeDef(TypedDict):
    FolderId: str,
    AuthenticationToken: NotRequired[str],
    Sort: NotRequired[ResourceSortTypeType],  # (1)
    Order: NotRequired[OrderTypeType],  # (2)
    Limit: NotRequired[int],
    Marker: NotRequired[str],
    Type: NotRequired[FolderContentTypeType],  # (3)
    Include: NotRequired[str],
```

1. See [:material-code-brackets: ResourceSortTypeType](./literals.md#resourcesorttypetype) 
2. See [:material-code-brackets: OrderTypeType](./literals.md#ordertypetype) 
3. See [:material-code-brackets: FolderContentTypeType](./literals.md#foldercontenttypetype) 
## DescribeGroupsRequestRequestTypeDef

```python
# DescribeGroupsRequestRequestTypeDef definition

class DescribeGroupsRequestRequestTypeDef(TypedDict):
    SearchQuery: str,
    AuthenticationToken: NotRequired[str],
    OrganizationId: NotRequired[str],
    Marker: NotRequired[str],
    Limit: NotRequired[int],
```

## GroupMetadataTypeDef

```python
# GroupMetadataTypeDef definition

class GroupMetadataTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
```

## DescribeNotificationSubscriptionsRequestRequestTypeDef

```python
# DescribeNotificationSubscriptionsRequestRequestTypeDef definition

class DescribeNotificationSubscriptionsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Marker: NotRequired[str],
    Limit: NotRequired[int],
```

## DescribeResourcePermissionsRequestRequestTypeDef

```python
# DescribeResourcePermissionsRequestRequestTypeDef definition

class DescribeResourcePermissionsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    AuthenticationToken: NotRequired[str],
    PrincipalId: NotRequired[str],
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeRootFoldersRequestRequestTypeDef

```python
# DescribeRootFoldersRequestRequestTypeDef definition

class DescribeRootFoldersRequestRequestTypeDef(TypedDict):
    AuthenticationToken: str,
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## DescribeUsersRequestRequestTypeDef

```python
# DescribeUsersRequestRequestTypeDef definition

class DescribeUsersRequestRequestTypeDef(TypedDict):
    AuthenticationToken: NotRequired[str],
    OrganizationId: NotRequired[str],
    UserIds: NotRequired[str],
    Query: NotRequired[str],
    Include: NotRequired[UserFilterTypeType],  # (1)
    Order: NotRequired[OrderTypeType],  # (2)
    Sort: NotRequired[UserSortTypeType],  # (3)
    Marker: NotRequired[str],
    Limit: NotRequired[int],
    Fields: NotRequired[str],
```

1. See [:material-code-brackets: UserFilterTypeType](./literals.md#userfiltertypetype) 
2. See [:material-code-brackets: OrderTypeType](./literals.md#ordertypetype) 
3. See [:material-code-brackets: UserSortTypeType](./literals.md#usersorttypetype) 
## LongRangeTypeTypeDef

```python
# LongRangeTypeTypeDef definition

class LongRangeTypeTypeDef(TypedDict):
    StartValue: NotRequired[int],
    EndValue: NotRequired[int],
```

## SearchPrincipalTypeTypeDef

```python
# SearchPrincipalTypeTypeDef definition

class SearchPrincipalTypeTypeDef(TypedDict):
    Id: str,
    Roles: NotRequired[Sequence[PrincipalRoleTypeType]],  # (1)
```

1. See [:material-code-brackets: PrincipalRoleTypeType](./literals.md#principalroletypetype) 
## GetCurrentUserRequestRequestTypeDef

```python
# GetCurrentUserRequestRequestTypeDef definition

class GetCurrentUserRequestRequestTypeDef(TypedDict):
    AuthenticationToken: str,
```

## GetDocumentPathRequestRequestTypeDef

```python
# GetDocumentPathRequestRequestTypeDef definition

class GetDocumentPathRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    AuthenticationToken: NotRequired[str],
    Limit: NotRequired[int],
    Fields: NotRequired[str],
    Marker: NotRequired[str],
```

## GetDocumentRequestRequestTypeDef

```python
# GetDocumentRequestRequestTypeDef definition

class GetDocumentRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    AuthenticationToken: NotRequired[str],
    IncludeCustomMetadata: NotRequired[bool],
```

## GetDocumentVersionRequestRequestTypeDef

```python
# GetDocumentVersionRequestRequestTypeDef definition

class GetDocumentVersionRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    VersionId: str,
    AuthenticationToken: NotRequired[str],
    Fields: NotRequired[str],
    IncludeCustomMetadata: NotRequired[bool],
```

## GetFolderPathRequestRequestTypeDef

```python
# GetFolderPathRequestRequestTypeDef definition

class GetFolderPathRequestRequestTypeDef(TypedDict):
    FolderId: str,
    AuthenticationToken: NotRequired[str],
    Limit: NotRequired[int],
    Fields: NotRequired[str],
    Marker: NotRequired[str],
```

## GetFolderRequestRequestTypeDef

```python
# GetFolderRequestRequestTypeDef definition

class GetFolderRequestRequestTypeDef(TypedDict):
    FolderId: str,
    AuthenticationToken: NotRequired[str],
    IncludeCustomMetadata: NotRequired[bool],
```

## GetResourcesRequestRequestTypeDef

```python
# GetResourcesRequestRequestTypeDef definition

class GetResourcesRequestRequestTypeDef(TypedDict):
    AuthenticationToken: NotRequired[str],
    UserId: NotRequired[str],
    CollectionType: NotRequired[ResourceCollectionTypeType],  # (1)
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: ResourceCollectionTypeType](./literals.md#resourcecollectiontypetype) 
## UploadMetadataTypeDef

```python
# UploadMetadataTypeDef definition

class UploadMetadataTypeDef(TypedDict):
    UploadUrl: NotRequired[str],
    SignedHeaders: NotRequired[Dict[str, str]],
```

## PermissionInfoTypeDef

```python
# PermissionInfoTypeDef definition

class PermissionInfoTypeDef(TypedDict):
    Role: NotRequired[RoleTypeType],  # (1)
    Type: NotRequired[RolePermissionTypeType],  # (2)
```

1. See [:material-code-brackets: RoleTypeType](./literals.md#roletypetype) 
2. See [:material-code-brackets: RolePermissionTypeType](./literals.md#rolepermissiontypetype) 
## RemoveAllResourcePermissionsRequestRequestTypeDef

```python
# RemoveAllResourcePermissionsRequestRequestTypeDef definition

class RemoveAllResourcePermissionsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    AuthenticationToken: NotRequired[str],
```

## RemoveResourcePermissionRequestRequestTypeDef

```python
# RemoveResourcePermissionRequestRequestTypeDef definition

class RemoveResourcePermissionRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    PrincipalId: str,
    AuthenticationToken: NotRequired[str],
    PrincipalType: NotRequired[PrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## ResourcePathComponentTypeDef

```python
# ResourcePathComponentTypeDef definition

class ResourcePathComponentTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
```

## RestoreDocumentVersionsRequestRequestTypeDef

```python
# RestoreDocumentVersionsRequestRequestTypeDef definition

class RestoreDocumentVersionsRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    AuthenticationToken: NotRequired[str],
```

## SearchSortResultTypeDef

```python
# SearchSortResultTypeDef definition

class SearchSortResultTypeDef(TypedDict):
    Field: NotRequired[OrderByFieldTypeType],  # (1)
    Order: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: OrderByFieldTypeType](./literals.md#orderbyfieldtypetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## UpdateDocumentRequestRequestTypeDef

```python
# UpdateDocumentRequestRequestTypeDef definition

class UpdateDocumentRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    AuthenticationToken: NotRequired[str],
    Name: NotRequired[str],
    ParentFolderId: NotRequired[str],
    ResourceState: NotRequired[ResourceStateTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceStateTypeType](./literals.md#resourcestatetypetype) 
## UpdateDocumentVersionRequestRequestTypeDef

```python
# UpdateDocumentVersionRequestRequestTypeDef definition

class UpdateDocumentVersionRequestRequestTypeDef(TypedDict):
    DocumentId: str,
    VersionId: str,
    AuthenticationToken: NotRequired[str],
    VersionStatus: NotRequired[DocumentVersionStatusType],  # (1)
```

1. See [:material-code-brackets: DocumentVersionStatusType](./literals.md#documentversionstatustype) 
## UpdateFolderRequestRequestTypeDef

```python
# UpdateFolderRequestRequestTypeDef definition

class UpdateFolderRequestRequestTypeDef(TypedDict):
    FolderId: str,
    AuthenticationToken: NotRequired[str],
    Name: NotRequired[str],
    ParentFolderId: NotRequired[str],
    ResourceState: NotRequired[ResourceStateTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceStateTypeType](./literals.md#resourcestatetypetype) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceMetadataTypeDef

```python
# ResourceMetadataTypeDef definition

class ResourceMetadataTypeDef(TypedDict):
    Type: NotRequired[ResourceTypeType],  # (1)
    Name: NotRequired[str],
    OriginalName: NotRequired[str],
    Id: NotRequired[str],
    VersionId: NotRequired[str],
    Owner: NotRequired[UserMetadataTypeDef],  # (2)
    ParentId: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: UserMetadataTypeDef](./type_defs.md#usermetadatatypedef) 
## AddResourcePermissionsRequestRequestTypeDef

```python
# AddResourcePermissionsRequestRequestTypeDef definition

class AddResourcePermissionsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    Principals: Sequence[SharePrincipalTypeDef],  # (1)
    AuthenticationToken: NotRequired[str],
    NotificationOptions: NotRequired[NotificationOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: SharePrincipalTypeDef](./type_defs.md#shareprincipaltypedef) 
2. See [:material-code-braces: NotificationOptionsTypeDef](./type_defs.md#notificationoptionstypedef) 
## AddResourcePermissionsResponseTypeDef

```python
# AddResourcePermissionsResponseTypeDef definition

class AddResourcePermissionsResponseTypeDef(TypedDict):
    ShareResults: List[ShareResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ShareResultTypeDef](./type_defs.md#shareresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFolderResponseTypeDef

```python
# CreateFolderResponseTypeDef definition

class CreateFolderResponseTypeDef(TypedDict):
    Metadata: FolderMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FolderMetadataTypeDef](./type_defs.md#foldermetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRootFoldersResponseTypeDef

```python
# DescribeRootFoldersResponseTypeDef definition

class DescribeRootFoldersResponseTypeDef(TypedDict):
    Folders: List[FolderMetadataTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FolderMetadataTypeDef](./type_defs.md#foldermetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFolderResponseTypeDef

```python
# GetFolderResponseTypeDef definition

class GetFolderResponseTypeDef(TypedDict):
    Metadata: FolderMetadataTypeDef,  # (1)
    CustomMetadata: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FolderMetadataTypeDef](./type_defs.md#foldermetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNotificationSubscriptionResponseTypeDef

```python
# CreateNotificationSubscriptionResponseTypeDef definition

class CreateNotificationSubscriptionResponseTypeDef(TypedDict):
    Subscription: SubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNotificationSubscriptionsResponseTypeDef

```python
# DescribeNotificationSubscriptionsResponseTypeDef definition

class DescribeNotificationSubscriptionsResponseTypeDef(TypedDict):
    Subscriptions: List[SubscriptionTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    Username: str,
    GivenName: str,
    Surname: str,
    Password: str,
    OrganizationId: NotRequired[str],
    EmailAddress: NotRequired[str],
    TimeZoneId: NotRequired[str],
    StorageRule: NotRequired[StorageRuleTypeTypeDef],  # (1)
    AuthenticationToken: NotRequired[str],
```

1. See [:material-code-braces: StorageRuleTypeTypeDef](./type_defs.md#storageruletypetypedef) 
## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
    UserId: str,
    AuthenticationToken: NotRequired[str],
    GivenName: NotRequired[str],
    Surname: NotRequired[str],
    Type: NotRequired[UserTypeType],  # (1)
    StorageRule: NotRequired[StorageRuleTypeTypeDef],  # (2)
    TimeZoneId: NotRequired[str],
    Locale: NotRequired[LocaleTypeType],  # (3)
    GrantPoweruserPrivileges: NotRequired[BooleanEnumTypeType],  # (4)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: StorageRuleTypeTypeDef](./type_defs.md#storageruletypetypedef) 
3. See [:material-code-brackets: LocaleTypeType](./literals.md#localetypetype) 
4. See [:material-code-brackets: BooleanEnumTypeType](./literals.md#booleanenumtypetype) 
## UserStorageMetadataTypeDef

```python
# UserStorageMetadataTypeDef definition

class UserStorageMetadataTypeDef(TypedDict):
    StorageUtilizedInBytes: NotRequired[int],
    StorageRule: NotRequired[StorageRuleTypeTypeDef],  # (1)
```

1. See [:material-code-braces: StorageRuleTypeTypeDef](./type_defs.md#storageruletypetypedef) 
## DateRangeTypeTypeDef

```python
# DateRangeTypeTypeDef definition

class DateRangeTypeTypeDef(TypedDict):
    StartValue: NotRequired[TimestampTypeDef],
    EndValue: NotRequired[TimestampTypeDef],
```

## DescribeActivitiesRequestRequestTypeDef

```python
# DescribeActivitiesRequestRequestTypeDef definition

class DescribeActivitiesRequestRequestTypeDef(TypedDict):
    AuthenticationToken: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    OrganizationId: NotRequired[str],
    ActivityTypes: NotRequired[str],
    ResourceId: NotRequired[str],
    UserId: NotRequired[str],
    IncludeIndirectActivities: NotRequired[bool],
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

## InitiateDocumentVersionUploadRequestRequestTypeDef

```python
# InitiateDocumentVersionUploadRequestRequestTypeDef definition

class InitiateDocumentVersionUploadRequestRequestTypeDef(TypedDict):
    AuthenticationToken: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    ContentCreatedTimestamp: NotRequired[TimestampTypeDef],
    ContentModifiedTimestamp: NotRequired[TimestampTypeDef],
    ContentType: NotRequired[str],
    DocumentSizeInBytes: NotRequired[int],
    ParentFolderId: NotRequired[str],
```

## DescribeActivitiesRequestPaginateTypeDef

```python
# DescribeActivitiesRequestPaginateTypeDef definition

class DescribeActivitiesRequestPaginateTypeDef(TypedDict):
    AuthenticationToken: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
    OrganizationId: NotRequired[str],
    ActivityTypes: NotRequired[str],
    ResourceId: NotRequired[str],
    UserId: NotRequired[str],
    IncludeIndirectActivities: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeCommentsRequestPaginateTypeDef

```python
# DescribeCommentsRequestPaginateTypeDef definition

class DescribeCommentsRequestPaginateTypeDef(TypedDict):
    DocumentId: str,
    VersionId: str,
    AuthenticationToken: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDocumentVersionsRequestPaginateTypeDef

```python
# DescribeDocumentVersionsRequestPaginateTypeDef definition

class DescribeDocumentVersionsRequestPaginateTypeDef(TypedDict):
    DocumentId: str,
    AuthenticationToken: NotRequired[str],
    Include: NotRequired[str],
    Fields: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeFolderContentsRequestPaginateTypeDef

```python
# DescribeFolderContentsRequestPaginateTypeDef definition

class DescribeFolderContentsRequestPaginateTypeDef(TypedDict):
    FolderId: str,
    AuthenticationToken: NotRequired[str],
    Sort: NotRequired[ResourceSortTypeType],  # (1)
    Order: NotRequired[OrderTypeType],  # (2)
    Type: NotRequired[FolderContentTypeType],  # (3)
    Include: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ResourceSortTypeType](./literals.md#resourcesorttypetype) 
2. See [:material-code-brackets: OrderTypeType](./literals.md#ordertypetype) 
3. See [:material-code-brackets: FolderContentTypeType](./literals.md#foldercontenttypetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeGroupsRequestPaginateTypeDef

```python
# DescribeGroupsRequestPaginateTypeDef definition

class DescribeGroupsRequestPaginateTypeDef(TypedDict):
    SearchQuery: str,
    AuthenticationToken: NotRequired[str],
    OrganizationId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeNotificationSubscriptionsRequestPaginateTypeDef

```python
# DescribeNotificationSubscriptionsRequestPaginateTypeDef definition

class DescribeNotificationSubscriptionsRequestPaginateTypeDef(TypedDict):
    OrganizationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeResourcePermissionsRequestPaginateTypeDef

```python
# DescribeResourcePermissionsRequestPaginateTypeDef definition

class DescribeResourcePermissionsRequestPaginateTypeDef(TypedDict):
    ResourceId: str,
    AuthenticationToken: NotRequired[str],
    PrincipalId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRootFoldersRequestPaginateTypeDef

```python
# DescribeRootFoldersRequestPaginateTypeDef definition

class DescribeRootFoldersRequestPaginateTypeDef(TypedDict):
    AuthenticationToken: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeUsersRequestPaginateTypeDef

```python
# DescribeUsersRequestPaginateTypeDef definition

class DescribeUsersRequestPaginateTypeDef(TypedDict):
    AuthenticationToken: NotRequired[str],
    OrganizationId: NotRequired[str],
    UserIds: NotRequired[str],
    Query: NotRequired[str],
    Include: NotRequired[UserFilterTypeType],  # (1)
    Order: NotRequired[OrderTypeType],  # (2)
    Sort: NotRequired[UserSortTypeType],  # (3)
    Fields: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: UserFilterTypeType](./literals.md#userfiltertypetype) 
2. See [:material-code-brackets: OrderTypeType](./literals.md#ordertypetype) 
3. See [:material-code-brackets: UserSortTypeType](./literals.md#usersorttypetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeDocumentVersionsResponseTypeDef

```python
# DescribeDocumentVersionsResponseTypeDef definition

class DescribeDocumentVersionsResponseTypeDef(TypedDict):
    DocumentVersions: List[DocumentVersionMetadataTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentVersionMetadataTypeDef](./type_defs.md#documentversionmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentMetadataTypeDef

```python
# DocumentMetadataTypeDef definition

class DocumentMetadataTypeDef(TypedDict):
    Id: NotRequired[str],
    CreatorId: NotRequired[str],
    ParentFolderId: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    ModifiedTimestamp: NotRequired[datetime],
    LatestVersionMetadata: NotRequired[DocumentVersionMetadataTypeDef],  # (1)
    ResourceState: NotRequired[ResourceStateTypeType],  # (2)
    Labels: NotRequired[List[str]],
```

1. See [:material-code-braces: DocumentVersionMetadataTypeDef](./type_defs.md#documentversionmetadatatypedef) 
2. See [:material-code-brackets: ResourceStateTypeType](./literals.md#resourcestatetypetype) 
## GetDocumentVersionResponseTypeDef

```python
# GetDocumentVersionResponseTypeDef definition

class GetDocumentVersionResponseTypeDef(TypedDict):
    Metadata: DocumentVersionMetadataTypeDef,  # (1)
    CustomMetadata: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentVersionMetadataTypeDef](./type_defs.md#documentversionmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGroupsResponseTypeDef

```python
# DescribeGroupsResponseTypeDef definition

class DescribeGroupsResponseTypeDef(TypedDict):
    Groups: List[GroupMetadataTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupMetadataTypeDef](./type_defs.md#groupmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ParticipantsTypeDef

```python
# ParticipantsTypeDef definition

class ParticipantsTypeDef(TypedDict):
    Users: NotRequired[List[UserMetadataTypeDef]],  # (1)
    Groups: NotRequired[List[GroupMetadataTypeDef]],  # (2)
```

1. See [:material-code-braces: UserMetadataTypeDef](./type_defs.md#usermetadatatypedef) 
2. See [:material-code-braces: GroupMetadataTypeDef](./type_defs.md#groupmetadatatypedef) 
## PrincipalTypeDef

```python
# PrincipalTypeDef definition

class PrincipalTypeDef(TypedDict):
    Id: NotRequired[str],
    Type: NotRequired[PrincipalTypeType],  # (1)
    Roles: NotRequired[List[PermissionInfoTypeDef]],  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: PermissionInfoTypeDef](./type_defs.md#permissioninfotypedef) 
## ResourcePathTypeDef

```python
# ResourcePathTypeDef definition

class ResourcePathTypeDef(TypedDict):
    Components: NotRequired[List[ResourcePathComponentTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePathComponentTypeDef](./type_defs.md#resourcepathcomponenttypedef) 
## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    Id: NotRequired[str],
    Username: NotRequired[str],
    EmailAddress: NotRequired[str],
    GivenName: NotRequired[str],
    Surname: NotRequired[str],
    OrganizationId: NotRequired[str],
    RootFolderId: NotRequired[str],
    RecycleBinFolderId: NotRequired[str],
    Status: NotRequired[UserStatusTypeType],  # (1)
    Type: NotRequired[UserTypeType],  # (2)
    CreatedTimestamp: NotRequired[datetime],
    ModifiedTimestamp: NotRequired[datetime],
    TimeZoneId: NotRequired[str],
    Locale: NotRequired[LocaleTypeType],  # (3)
    Storage: NotRequired[UserStorageMetadataTypeDef],  # (4)
```

1. See [:material-code-brackets: UserStatusTypeType](./literals.md#userstatustypetype) 
2. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
3. See [:material-code-brackets: LocaleTypeType](./literals.md#localetypetype) 
4. See [:material-code-braces: UserStorageMetadataTypeDef](./type_defs.md#userstoragemetadatatypedef) 
## FiltersTypeDef

```python
# FiltersTypeDef definition

class FiltersTypeDef(TypedDict):
    TextLocales: NotRequired[Sequence[LanguageCodeTypeType]],  # (1)
    ContentCategories: NotRequired[Sequence[ContentCategoryTypeType]],  # (2)
    ResourceTypes: NotRequired[Sequence[SearchResourceTypeType]],  # (3)
    Labels: NotRequired[Sequence[str]],
    Principals: NotRequired[Sequence[SearchPrincipalTypeTypeDef]],  # (4)
    AncestorIds: NotRequired[Sequence[str]],
    SearchCollectionTypes: NotRequired[Sequence[SearchCollectionTypeType]],  # (5)
    SizeRange: NotRequired[LongRangeTypeTypeDef],  # (6)
    CreatedRange: NotRequired[DateRangeTypeTypeDef],  # (7)
    ModifiedRange: NotRequired[DateRangeTypeTypeDef],  # (7)
```

1. See [:material-code-brackets: LanguageCodeTypeType](./literals.md#languagecodetypetype) 
2. See [:material-code-brackets: ContentCategoryTypeType](./literals.md#contentcategorytypetype) 
3. See [:material-code-brackets: SearchResourceTypeType](./literals.md#searchresourcetypetype) 
4. See [:material-code-braces: SearchPrincipalTypeTypeDef](./type_defs.md#searchprincipaltypetypedef) 
5. See [:material-code-brackets: SearchCollectionTypeType](./literals.md#searchcollectiontypetype) 
6. See [:material-code-braces: LongRangeTypeTypeDef](./type_defs.md#longrangetypetypedef) 
7. See [:material-code-braces: DateRangeTypeTypeDef](./type_defs.md#daterangetypetypedef) 
8. See [:material-code-braces: DateRangeTypeTypeDef](./type_defs.md#daterangetypetypedef) 
## DescribeFolderContentsResponseTypeDef

```python
# DescribeFolderContentsResponseTypeDef definition

class DescribeFolderContentsResponseTypeDef(TypedDict):
    Folders: List[FolderMetadataTypeDef],  # (1)
    Documents: List[DocumentMetadataTypeDef],  # (2)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FolderMetadataTypeDef](./type_defs.md#foldermetadatatypedef) 
2. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDocumentResponseTypeDef

```python
# GetDocumentResponseTypeDef definition

class GetDocumentResponseTypeDef(TypedDict):
    Metadata: DocumentMetadataTypeDef,  # (1)
    CustomMetadata: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcesResponseTypeDef

```python
# GetResourcesResponseTypeDef definition

class GetResourcesResponseTypeDef(TypedDict):
    Folders: List[FolderMetadataTypeDef],  # (1)
    Documents: List[DocumentMetadataTypeDef],  # (2)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FolderMetadataTypeDef](./type_defs.md#foldermetadatatypedef) 
2. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InitiateDocumentVersionUploadResponseTypeDef

```python
# InitiateDocumentVersionUploadResponseTypeDef definition

class InitiateDocumentVersionUploadResponseTypeDef(TypedDict):
    Metadata: DocumentMetadataTypeDef,  # (1)
    UploadMetadata: UploadMetadataTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
2. See [:material-code-braces: UploadMetadataTypeDef](./type_defs.md#uploadmetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourcePermissionsResponseTypeDef

```python
# DescribeResourcePermissionsResponseTypeDef definition

class DescribeResourcePermissionsResponseTypeDef(TypedDict):
    Principals: List[PrincipalTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDocumentPathResponseTypeDef

```python
# GetDocumentPathResponseTypeDef definition

class GetDocumentPathResponseTypeDef(TypedDict):
    Path: ResourcePathTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePathTypeDef](./type_defs.md#resourcepathtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFolderPathResponseTypeDef

```python
# GetFolderPathResponseTypeDef definition

class GetFolderPathResponseTypeDef(TypedDict):
    Path: ResourcePathTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourcePathTypeDef](./type_defs.md#resourcepathtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActivateUserResponseTypeDef

```python
# ActivateUserResponseTypeDef definition

class ActivateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CommentMetadataTypeDef

```python
# CommentMetadataTypeDef definition

class CommentMetadataTypeDef(TypedDict):
    CommentId: NotRequired[str],
    Contributor: NotRequired[UserTypeDef],  # (1)
    CreatedTimestamp: NotRequired[datetime],
    CommentStatus: NotRequired[CommentStatusTypeType],  # (2)
    RecipientId: NotRequired[str],
    ContributorId: NotRequired[str],
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-brackets: CommentStatusTypeType](./literals.md#commentstatustypetype) 
## CommentTypeDef

```python
# CommentTypeDef definition

class CommentTypeDef(TypedDict):
    CommentId: str,
    ParentId: NotRequired[str],
    ThreadId: NotRequired[str],
    Text: NotRequired[str],
    Contributor: NotRequired[UserTypeDef],  # (1)
    CreatedTimestamp: NotRequired[datetime],
    Status: NotRequired[CommentStatusTypeType],  # (2)
    Visibility: NotRequired[CommentVisibilityTypeType],  # (3)
    RecipientId: NotRequired[str],
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-brackets: CommentStatusTypeType](./literals.md#commentstatustypetype) 
3. See [:material-code-brackets: CommentVisibilityTypeType](./literals.md#commentvisibilitytypetype) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUsersResponseTypeDef

```python
# DescribeUsersResponseTypeDef definition

class DescribeUsersResponseTypeDef(TypedDict):
    Users: List[UserTypeDef],  # (1)
    TotalNumberOfUsers: int,
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCurrentUserResponseTypeDef

```python
# GetCurrentUserResponseTypeDef definition

class GetCurrentUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserResponseTypeDef

```python
# UpdateUserResponseTypeDef definition

class UpdateUserResponseTypeDef(TypedDict):
    User: UserTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchResourcesRequestPaginateTypeDef

```python
# SearchResourcesRequestPaginateTypeDef definition

class SearchResourcesRequestPaginateTypeDef(TypedDict):
    AuthenticationToken: NotRequired[str],
    QueryText: NotRequired[str],
    QueryScopes: NotRequired[Sequence[SearchQueryScopeTypeType]],  # (1)
    OrganizationId: NotRequired[str],
    AdditionalResponseFields: NotRequired[Sequence[AdditionalResponseFieldTypeType]],  # (2)
    Filters: NotRequired[FiltersTypeDef],  # (3)
    OrderBy: NotRequired[Sequence[SearchSortResultTypeDef]],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: SearchQueryScopeTypeType](./literals.md#searchqueryscopetypetype) 
2. See [:material-code-brackets: AdditionalResponseFieldTypeType](./literals.md#additionalresponsefieldtypetype) 
3. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
4. See [:material-code-braces: SearchSortResultTypeDef](./type_defs.md#searchsortresulttypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchResourcesRequestRequestTypeDef

```python
# SearchResourcesRequestRequestTypeDef definition

class SearchResourcesRequestRequestTypeDef(TypedDict):
    AuthenticationToken: NotRequired[str],
    QueryText: NotRequired[str],
    QueryScopes: NotRequired[Sequence[SearchQueryScopeTypeType]],  # (1)
    OrganizationId: NotRequired[str],
    AdditionalResponseFields: NotRequired[Sequence[AdditionalResponseFieldTypeType]],  # (2)
    Filters: NotRequired[FiltersTypeDef],  # (3)
    OrderBy: NotRequired[Sequence[SearchSortResultTypeDef]],  # (4)
    Limit: NotRequired[int],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: SearchQueryScopeTypeType](./literals.md#searchqueryscopetypetype) 
2. See [:material-code-brackets: AdditionalResponseFieldTypeType](./literals.md#additionalresponsefieldtypetype) 
3. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
4. See [:material-code-braces: SearchSortResultTypeDef](./type_defs.md#searchsortresulttypedef) 
## ActivityTypeDef

```python
# ActivityTypeDef definition

class ActivityTypeDef(TypedDict):
    Type: NotRequired[ActivityTypeType],  # (1)
    TimeStamp: NotRequired[datetime],
    IsIndirectActivity: NotRequired[bool],
    OrganizationId: NotRequired[str],
    Initiator: NotRequired[UserMetadataTypeDef],  # (2)
    Participants: NotRequired[ParticipantsTypeDef],  # (3)
    ResourceMetadata: NotRequired[ResourceMetadataTypeDef],  # (4)
    OriginalParent: NotRequired[ResourceMetadataTypeDef],  # (4)
    CommentMetadata: NotRequired[CommentMetadataTypeDef],  # (6)
```

1. See [:material-code-brackets: ActivityTypeType](./literals.md#activitytypetype) 
2. See [:material-code-braces: UserMetadataTypeDef](./type_defs.md#usermetadatatypedef) 
3. See [:material-code-braces: ParticipantsTypeDef](./type_defs.md#participantstypedef) 
4. See [:material-code-braces: ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef) 
5. See [:material-code-braces: ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef) 
6. See [:material-code-braces: CommentMetadataTypeDef](./type_defs.md#commentmetadatatypedef) 
## ResponseItemTypeDef

```python
# ResponseItemTypeDef definition

class ResponseItemTypeDef(TypedDict):
    ResourceType: NotRequired[ResponseItemTypeType],  # (1)
    WebUrl: NotRequired[str],
    DocumentMetadata: NotRequired[DocumentMetadataTypeDef],  # (2)
    FolderMetadata: NotRequired[FolderMetadataTypeDef],  # (3)
    CommentMetadata: NotRequired[CommentMetadataTypeDef],  # (4)
    DocumentVersionMetadata: NotRequired[DocumentVersionMetadataTypeDef],  # (5)
```

1. See [:material-code-brackets: ResponseItemTypeType](./literals.md#responseitemtypetype) 
2. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
3. See [:material-code-braces: FolderMetadataTypeDef](./type_defs.md#foldermetadatatypedef) 
4. See [:material-code-braces: CommentMetadataTypeDef](./type_defs.md#commentmetadatatypedef) 
5. See [:material-code-braces: DocumentVersionMetadataTypeDef](./type_defs.md#documentversionmetadatatypedef) 
## CreateCommentResponseTypeDef

```python
# CreateCommentResponseTypeDef definition

class CreateCommentResponseTypeDef(TypedDict):
    Comment: CommentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCommentsResponseTypeDef

```python
# DescribeCommentsResponseTypeDef definition

class DescribeCommentsResponseTypeDef(TypedDict):
    Comments: List[CommentTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommentTypeDef](./type_defs.md#commenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeActivitiesResponseTypeDef

```python
# DescribeActivitiesResponseTypeDef definition

class DescribeActivitiesResponseTypeDef(TypedDict):
    UserActivities: List[ActivityTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActivityTypeDef](./type_defs.md#activitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchResourcesResponseTypeDef

```python
# SearchResourcesResponseTypeDef definition

class SearchResourcesResponseTypeDef(TypedDict):
    Items: List[ResponseItemTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseItemTypeDef](./type_defs.md#responseitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
