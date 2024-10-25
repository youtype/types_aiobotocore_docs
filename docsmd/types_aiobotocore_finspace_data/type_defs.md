# Type definitions

> [Index](../README.md) > [FinSpaceData](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [FinSpaceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
    type annotations stubs module [types-aiobotocore-finspace-data](https://pypi.org/project/types-aiobotocore-finspace-data/).

## SchemaDefinitionUnionTypeDef

```python
# SchemaDefinitionUnionTypeDef definition

SchemaDefinitionUnionTypeDef = Union[
    SchemaDefinitionTypeDef,  # (1)
    SchemaDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) 
2. See [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 



## AssociateUserToPermissionGroupRequestRequestTypeDef

```python
# AssociateUserToPermissionGroupRequestRequestTypeDef definition

class AssociateUserToPermissionGroupRequestRequestTypeDef(TypedDict):
    permissionGroupId: str,
    userId: str,
    clientToken: NotRequired[str],
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

## AwsCredentialsTypeDef

```python
# AwsCredentialsTypeDef definition

class AwsCredentialsTypeDef(TypedDict):
    accessKeyId: NotRequired[str],
    secretAccessKey: NotRequired[str],
    sessionToken: NotRequired[str],
    expiration: NotRequired[int],
```

## ChangesetErrorInfoTypeDef

```python
# ChangesetErrorInfoTypeDef definition

class ChangesetErrorInfoTypeDef(TypedDict):
    errorMessage: NotRequired[str],
    errorCategory: NotRequired[ErrorCategoryType],  # (1)
```

1. See [:material-code-brackets: ErrorCategoryType](./literals.md#errorcategorytype) 
## ColumnDefinitionTypeDef

```python
# ColumnDefinitionTypeDef definition

class ColumnDefinitionTypeDef(TypedDict):
    dataType: NotRequired[ColumnDataTypeType],  # (1)
    columnName: NotRequired[str],
    columnDescription: NotRequired[str],
```

1. See [:material-code-brackets: ColumnDataTypeType](./literals.md#columndatatypetype) 
## CreateChangesetRequestRequestTypeDef

```python
# CreateChangesetRequestRequestTypeDef definition

class CreateChangesetRequestRequestTypeDef(TypedDict):
    datasetId: str,
    changeType: ChangeTypeType,  # (1)
    sourceParams: Mapping[str, str],
    formatParams: Mapping[str, str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
## DataViewDestinationTypeParamsTypeDef

```python
# DataViewDestinationTypeParamsTypeDef definition

class DataViewDestinationTypeParamsTypeDef(TypedDict):
    destinationType: str,
    s3DestinationExportFileFormat: NotRequired[ExportFileFormatType],  # (1)
    s3DestinationExportFileFormatOptions: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ExportFileFormatType](./literals.md#exportfileformattype) 
## DatasetOwnerInfoTypeDef

```python
# DatasetOwnerInfoTypeDef definition

class DatasetOwnerInfoTypeDef(TypedDict):
    name: NotRequired[str],
    phoneNumber: NotRequired[str],
    email: NotRequired[str],
```

## CreatePermissionGroupRequestRequestTypeDef

```python
# CreatePermissionGroupRequestRequestTypeDef definition

class CreatePermissionGroupRequestRequestTypeDef(TypedDict):
    name: str,
    applicationPermissions: Sequence[ApplicationPermissionType],  # (1)
    description: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: ApplicationPermissionType](./literals.md#applicationpermissiontype) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    emailAddress: str,
    type: UserTypeType,  # (1)
    firstName: NotRequired[str],
    lastName: NotRequired[str],
    apiAccess: NotRequired[ApiAccessType],  # (2)
    apiAccessPrincipalArn: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-brackets: ApiAccessType](./literals.md#apiaccesstype) 
## CredentialsTypeDef

```python
# CredentialsTypeDef definition

class CredentialsTypeDef(TypedDict):
    accessKeyId: NotRequired[str],
    secretAccessKey: NotRequired[str],
    sessionToken: NotRequired[str],
```

## DataViewDestinationTypeParamsOutputTypeDef

```python
# DataViewDestinationTypeParamsOutputTypeDef definition

class DataViewDestinationTypeParamsOutputTypeDef(TypedDict):
    destinationType: str,
    s3DestinationExportFileFormat: NotRequired[ExportFileFormatType],  # (1)
    s3DestinationExportFileFormatOptions: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ExportFileFormatType](./literals.md#exportfileformattype) 
## DataViewErrorInfoTypeDef

```python
# DataViewErrorInfoTypeDef definition

class DataViewErrorInfoTypeDef(TypedDict):
    errorMessage: NotRequired[str],
    errorCategory: NotRequired[ErrorCategoryType],  # (1)
```

1. See [:material-code-brackets: ErrorCategoryType](./literals.md#errorcategorytype) 
## DeleteDatasetRequestRequestTypeDef

```python
# DeleteDatasetRequestRequestTypeDef definition

class DeleteDatasetRequestRequestTypeDef(TypedDict):
    datasetId: str,
    clientToken: NotRequired[str],
```

## DeletePermissionGroupRequestRequestTypeDef

```python
# DeletePermissionGroupRequestRequestTypeDef definition

class DeletePermissionGroupRequestRequestTypeDef(TypedDict):
    permissionGroupId: str,
    clientToken: NotRequired[str],
```

## DisableUserRequestRequestTypeDef

```python
# DisableUserRequestRequestTypeDef definition

class DisableUserRequestRequestTypeDef(TypedDict):
    userId: str,
    clientToken: NotRequired[str],
```

## DisassociateUserFromPermissionGroupRequestRequestTypeDef

```python
# DisassociateUserFromPermissionGroupRequestRequestTypeDef definition

class DisassociateUserFromPermissionGroupRequestRequestTypeDef(TypedDict):
    permissionGroupId: str,
    userId: str,
    clientToken: NotRequired[str],
```

## EnableUserRequestRequestTypeDef

```python
# EnableUserRequestRequestTypeDef definition

class EnableUserRequestRequestTypeDef(TypedDict):
    userId: str,
    clientToken: NotRequired[str],
```

## GetChangesetRequestRequestTypeDef

```python
# GetChangesetRequestRequestTypeDef definition

class GetChangesetRequestRequestTypeDef(TypedDict):
    datasetId: str,
    changesetId: str,
```

## GetDataViewRequestRequestTypeDef

```python
# GetDataViewRequestRequestTypeDef definition

class GetDataViewRequestRequestTypeDef(TypedDict):
    dataViewId: str,
    datasetId: str,
```

## GetDatasetRequestRequestTypeDef

```python
# GetDatasetRequestRequestTypeDef definition

class GetDatasetRequestRequestTypeDef(TypedDict):
    datasetId: str,
```

## GetExternalDataViewAccessDetailsRequestRequestTypeDef

```python
# GetExternalDataViewAccessDetailsRequestRequestTypeDef definition

class GetExternalDataViewAccessDetailsRequestRequestTypeDef(TypedDict):
    dataViewId: str,
    datasetId: str,
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucket: str,
    key: str,
```

## GetPermissionGroupRequestRequestTypeDef

```python
# GetPermissionGroupRequestRequestTypeDef definition

class GetPermissionGroupRequestRequestTypeDef(TypedDict):
    permissionGroupId: str,
```

## PermissionGroupTypeDef

```python
# PermissionGroupTypeDef definition

class PermissionGroupTypeDef(TypedDict):
    permissionGroupId: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    applicationPermissions: NotRequired[List[ApplicationPermissionType]],  # (1)
    createTime: NotRequired[int],
    lastModifiedTime: NotRequired[int],
    membershipStatus: NotRequired[PermissionGroupMembershipStatusType],  # (2)
```

1. See [:material-code-brackets: ApplicationPermissionType](./literals.md#applicationpermissiontype) 
2. See [:material-code-brackets: PermissionGroupMembershipStatusType](./literals.md#permissiongroupmembershipstatustype) 
## GetProgrammaticAccessCredentialsRequestRequestTypeDef

```python
# GetProgrammaticAccessCredentialsRequestRequestTypeDef definition

class GetProgrammaticAccessCredentialsRequestRequestTypeDef(TypedDict):
    environmentId: str,
    durationInMinutes: NotRequired[int],
```

## GetUserRequestRequestTypeDef

```python
# GetUserRequestRequestTypeDef definition

class GetUserRequestRequestTypeDef(TypedDict):
    userId: str,
```

## GetWorkingLocationRequestRequestTypeDef

```python
# GetWorkingLocationRequestRequestTypeDef definition

class GetWorkingLocationRequestRequestTypeDef(TypedDict):
    locationType: NotRequired[LocationTypeType],  # (1)
```

1. See [:material-code-brackets: LocationTypeType](./literals.md#locationtypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListChangesetsRequestRequestTypeDef

```python
# ListChangesetsRequestRequestTypeDef definition

class ListChangesetsRequestRequestTypeDef(TypedDict):
    datasetId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDataViewsRequestRequestTypeDef

```python
# ListDataViewsRequestRequestTypeDef definition

class ListDataViewsRequestRequestTypeDef(TypedDict):
    datasetId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDatasetsRequestRequestTypeDef

```python
# ListDatasetsRequestRequestTypeDef definition

class ListDatasetsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPermissionGroupsByUserRequestRequestTypeDef

```python
# ListPermissionGroupsByUserRequestRequestTypeDef definition

class ListPermissionGroupsByUserRequestRequestTypeDef(TypedDict):
    userId: str,
    maxResults: int,
    nextToken: NotRequired[str],
```

## PermissionGroupByUserTypeDef

```python
# PermissionGroupByUserTypeDef definition

class PermissionGroupByUserTypeDef(TypedDict):
    permissionGroupId: NotRequired[str],
    name: NotRequired[str],
    membershipStatus: NotRequired[PermissionGroupMembershipStatusType],  # (1)
```

1. See [:material-code-brackets: PermissionGroupMembershipStatusType](./literals.md#permissiongroupmembershipstatustype) 
## ListPermissionGroupsRequestRequestTypeDef

```python
# ListPermissionGroupsRequestRequestTypeDef definition

class ListPermissionGroupsRequestRequestTypeDef(TypedDict):
    maxResults: int,
    nextToken: NotRequired[str],
```

## ListUsersByPermissionGroupRequestRequestTypeDef

```python
# ListUsersByPermissionGroupRequestRequestTypeDef definition

class ListUsersByPermissionGroupRequestRequestTypeDef(TypedDict):
    permissionGroupId: str,
    maxResults: int,
    nextToken: NotRequired[str],
```

## UserByPermissionGroupTypeDef

```python
# UserByPermissionGroupTypeDef definition

class UserByPermissionGroupTypeDef(TypedDict):
    userId: NotRequired[str],
    status: NotRequired[UserStatusType],  # (1)
    firstName: NotRequired[str],
    lastName: NotRequired[str],
    emailAddress: NotRequired[str],
    type: NotRequired[UserTypeType],  # (2)
    apiAccess: NotRequired[ApiAccessType],  # (3)
    apiAccessPrincipalArn: NotRequired[str],
    membershipStatus: NotRequired[PermissionGroupMembershipStatusType],  # (4)
```

1. See [:material-code-brackets: UserStatusType](./literals.md#userstatustype) 
2. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
3. See [:material-code-brackets: ApiAccessType](./literals.md#apiaccesstype) 
4. See [:material-code-brackets: PermissionGroupMembershipStatusType](./literals.md#permissiongroupmembershipstatustype) 
## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    maxResults: int,
    nextToken: NotRequired[str],
```

## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    userId: NotRequired[str],
    status: NotRequired[UserStatusType],  # (1)
    firstName: NotRequired[str],
    lastName: NotRequired[str],
    emailAddress: NotRequired[str],
    type: NotRequired[UserTypeType],  # (2)
    apiAccess: NotRequired[ApiAccessType],  # (3)
    apiAccessPrincipalArn: NotRequired[str],
    createTime: NotRequired[int],
    lastEnabledTime: NotRequired[int],
    lastDisabledTime: NotRequired[int],
    lastModifiedTime: NotRequired[int],
    lastLoginTime: NotRequired[int],
```

1. See [:material-code-brackets: UserStatusType](./literals.md#userstatustype) 
2. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
3. See [:material-code-brackets: ApiAccessType](./literals.md#apiaccesstype) 
## ResourcePermissionTypeDef

```python
# ResourcePermissionTypeDef definition

class ResourcePermissionTypeDef(TypedDict):
    permission: NotRequired[str],
```

## ResetUserPasswordRequestRequestTypeDef

```python
# ResetUserPasswordRequestRequestTypeDef definition

class ResetUserPasswordRequestRequestTypeDef(TypedDict):
    userId: str,
    clientToken: NotRequired[str],
```

## UpdateChangesetRequestRequestTypeDef

```python
# UpdateChangesetRequestRequestTypeDef definition

class UpdateChangesetRequestRequestTypeDef(TypedDict):
    datasetId: str,
    changesetId: str,
    sourceParams: Mapping[str, str],
    formatParams: Mapping[str, str],
    clientToken: NotRequired[str],
```

## UpdatePermissionGroupRequestRequestTypeDef

```python
# UpdatePermissionGroupRequestRequestTypeDef definition

class UpdatePermissionGroupRequestRequestTypeDef(TypedDict):
    permissionGroupId: str,
    name: NotRequired[str],
    description: NotRequired[str],
    applicationPermissions: NotRequired[Sequence[ApplicationPermissionType]],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: ApplicationPermissionType](./literals.md#applicationpermissiontype) 
## UpdateUserRequestRequestTypeDef

```python
# UpdateUserRequestRequestTypeDef definition

class UpdateUserRequestRequestTypeDef(TypedDict):
    userId: str,
    type: NotRequired[UserTypeType],  # (1)
    firstName: NotRequired[str],
    lastName: NotRequired[str],
    apiAccess: NotRequired[ApiAccessType],  # (2)
    apiAccessPrincipalArn: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-brackets: ApiAccessType](./literals.md#apiaccesstype) 
## AssociateUserToPermissionGroupResponseTypeDef

```python
# AssociateUserToPermissionGroupResponseTypeDef definition

class AssociateUserToPermissionGroupResponseTypeDef(TypedDict):
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChangesetResponseTypeDef

```python
# CreateChangesetResponseTypeDef definition

class CreateChangesetResponseTypeDef(TypedDict):
    datasetId: str,
    changesetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataViewResponseTypeDef

```python
# CreateDataViewResponseTypeDef definition

class CreateDataViewResponseTypeDef(TypedDict):
    datasetId: str,
    dataViewId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetResponseTypeDef

```python
# CreateDatasetResponseTypeDef definition

class CreateDatasetResponseTypeDef(TypedDict):
    datasetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePermissionGroupResponseTypeDef

```python
# CreatePermissionGroupResponseTypeDef definition

class CreatePermissionGroupResponseTypeDef(TypedDict):
    permissionGroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    userId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDatasetResponseTypeDef

```python
# DeleteDatasetResponseTypeDef definition

class DeleteDatasetResponseTypeDef(TypedDict):
    datasetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePermissionGroupResponseTypeDef

```python
# DeletePermissionGroupResponseTypeDef definition

class DeletePermissionGroupResponseTypeDef(TypedDict):
    permissionGroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableUserResponseTypeDef

```python
# DisableUserResponseTypeDef definition

class DisableUserResponseTypeDef(TypedDict):
    userId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateUserFromPermissionGroupResponseTypeDef

```python
# DisassociateUserFromPermissionGroupResponseTypeDef definition

class DisassociateUserFromPermissionGroupResponseTypeDef(TypedDict):
    statusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableUserResponseTypeDef

```python
# EnableUserResponseTypeDef definition

class EnableUserResponseTypeDef(TypedDict):
    userId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserResponseTypeDef

```python
# GetUserResponseTypeDef definition

class GetUserResponseTypeDef(TypedDict):
    userId: str,
    status: UserStatusType,  # (1)
    firstName: str,
    lastName: str,
    emailAddress: str,
    type: UserTypeType,  # (2)
    apiAccess: ApiAccessType,  # (3)
    apiAccessPrincipalArn: str,
    createTime: int,
    lastEnabledTime: int,
    lastDisabledTime: int,
    lastModifiedTime: int,
    lastLoginTime: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: UserStatusType](./literals.md#userstatustype) 
2. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
3. See [:material-code-brackets: ApiAccessType](./literals.md#apiaccesstype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkingLocationResponseTypeDef

```python
# GetWorkingLocationResponseTypeDef definition

class GetWorkingLocationResponseTypeDef(TypedDict):
    s3Uri: str,
    s3Path: str,
    s3Bucket: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetUserPasswordResponseTypeDef

```python
# ResetUserPasswordResponseTypeDef definition

class ResetUserPasswordResponseTypeDef(TypedDict):
    userId: str,
    temporaryPassword: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChangesetResponseTypeDef

```python
# UpdateChangesetResponseTypeDef definition

class UpdateChangesetResponseTypeDef(TypedDict):
    changesetId: str,
    datasetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDatasetResponseTypeDef

```python
# UpdateDatasetResponseTypeDef definition

class UpdateDatasetResponseTypeDef(TypedDict):
    datasetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePermissionGroupResponseTypeDef

```python
# UpdatePermissionGroupResponseTypeDef definition

class UpdatePermissionGroupResponseTypeDef(TypedDict):
    permissionGroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserResponseTypeDef

```python
# UpdateUserResponseTypeDef definition

class UpdateUserResponseTypeDef(TypedDict):
    userId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChangesetSummaryTypeDef

```python
# ChangesetSummaryTypeDef definition

class ChangesetSummaryTypeDef(TypedDict):
    changesetId: NotRequired[str],
    changesetArn: NotRequired[str],
    datasetId: NotRequired[str],
    changeType: NotRequired[ChangeTypeType],  # (1)
    sourceParams: NotRequired[Dict[str, str]],
    formatParams: NotRequired[Dict[str, str]],
    createTime: NotRequired[int],
    status: NotRequired[IngestionStatusType],  # (2)
    errorInfo: NotRequired[ChangesetErrorInfoTypeDef],  # (3)
    activeUntilTimestamp: NotRequired[int],
    activeFromTimestamp: NotRequired[int],
    updatesChangesetId: NotRequired[str],
    updatedByChangesetId: NotRequired[str],
```

1. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
2. See [:material-code-brackets: IngestionStatusType](./literals.md#ingestionstatustype) 
3. See [:material-code-braces: ChangesetErrorInfoTypeDef](./type_defs.md#changeseterrorinfotypedef) 
## GetChangesetResponseTypeDef

```python
# GetChangesetResponseTypeDef definition

class GetChangesetResponseTypeDef(TypedDict):
    changesetId: str,
    changesetArn: str,
    datasetId: str,
    changeType: ChangeTypeType,  # (1)
    sourceParams: Dict[str, str],
    formatParams: Dict[str, str],
    createTime: int,
    status: IngestionStatusType,  # (2)
    errorInfo: ChangesetErrorInfoTypeDef,  # (3)
    activeUntilTimestamp: int,
    activeFromTimestamp: int,
    updatesChangesetId: str,
    updatedByChangesetId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
2. See [:material-code-brackets: IngestionStatusType](./literals.md#ingestionstatustype) 
3. See [:material-code-braces: ChangesetErrorInfoTypeDef](./type_defs.md#changeseterrorinfotypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SchemaDefinitionOutputTypeDef

```python
# SchemaDefinitionOutputTypeDef definition

class SchemaDefinitionOutputTypeDef(TypedDict):
    columns: NotRequired[List[ColumnDefinitionTypeDef]],  # (1)
    primaryKeyColumns: NotRequired[List[str]],
```

1. See [:material-code-braces: ColumnDefinitionTypeDef](./type_defs.md#columndefinitiontypedef) 
## SchemaDefinitionTypeDef

```python
# SchemaDefinitionTypeDef definition

class SchemaDefinitionTypeDef(TypedDict):
    columns: NotRequired[Sequence[ColumnDefinitionTypeDef]],  # (1)
    primaryKeyColumns: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ColumnDefinitionTypeDef](./type_defs.md#columndefinitiontypedef) 
## CreateDataViewRequestRequestTypeDef

```python
# CreateDataViewRequestRequestTypeDef definition

class CreateDataViewRequestRequestTypeDef(TypedDict):
    datasetId: str,
    destinationTypeParams: DataViewDestinationTypeParamsTypeDef,  # (1)
    clientToken: NotRequired[str],
    autoUpdate: NotRequired[bool],
    sortColumns: NotRequired[Sequence[str]],
    partitionColumns: NotRequired[Sequence[str]],
    asOfTimestamp: NotRequired[int],
```

1. See [:material-code-braces: DataViewDestinationTypeParamsTypeDef](./type_defs.md#dataviewdestinationtypeparamstypedef) 
## GetProgrammaticAccessCredentialsResponseTypeDef

```python
# GetProgrammaticAccessCredentialsResponseTypeDef definition

class GetProgrammaticAccessCredentialsResponseTypeDef(TypedDict):
    credentials: CredentialsTypeDef,  # (1)
    durationInMinutes: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataViewSummaryTypeDef

```python
# DataViewSummaryTypeDef definition

class DataViewSummaryTypeDef(TypedDict):
    dataViewId: NotRequired[str],
    dataViewArn: NotRequired[str],
    datasetId: NotRequired[str],
    asOfTimestamp: NotRequired[int],
    partitionColumns: NotRequired[List[str]],
    sortColumns: NotRequired[List[str]],
    status: NotRequired[DataViewStatusType],  # (1)
    errorInfo: NotRequired[DataViewErrorInfoTypeDef],  # (2)
    destinationTypeProperties: NotRequired[DataViewDestinationTypeParamsOutputTypeDef],  # (3)
    autoUpdate: NotRequired[bool],
    createTime: NotRequired[int],
    lastModifiedTime: NotRequired[int],
```

1. See [:material-code-brackets: DataViewStatusType](./literals.md#dataviewstatustype) 
2. See [:material-code-braces: DataViewErrorInfoTypeDef](./type_defs.md#dataviewerrorinfotypedef) 
3. See [:material-code-braces: DataViewDestinationTypeParamsOutputTypeDef](./type_defs.md#dataviewdestinationtypeparamsoutputtypedef) 
## GetDataViewResponseTypeDef

```python
# GetDataViewResponseTypeDef definition

class GetDataViewResponseTypeDef(TypedDict):
    autoUpdate: bool,
    partitionColumns: List[str],
    datasetId: str,
    asOfTimestamp: int,
    errorInfo: DataViewErrorInfoTypeDef,  # (1)
    lastModifiedTime: int,
    createTime: int,
    sortColumns: List[str],
    dataViewId: str,
    dataViewArn: str,
    destinationTypeParams: DataViewDestinationTypeParamsOutputTypeDef,  # (2)
    status: DataViewStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DataViewErrorInfoTypeDef](./type_defs.md#dataviewerrorinfotypedef) 
2. See [:material-code-braces: DataViewDestinationTypeParamsOutputTypeDef](./type_defs.md#dataviewdestinationtypeparamsoutputtypedef) 
3. See [:material-code-brackets: DataViewStatusType](./literals.md#dataviewstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExternalDataViewAccessDetailsResponseTypeDef

```python
# GetExternalDataViewAccessDetailsResponseTypeDef definition

class GetExternalDataViewAccessDetailsResponseTypeDef(TypedDict):
    credentials: AwsCredentialsTypeDef,  # (1)
    s3Location: S3LocationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AwsCredentialsTypeDef](./type_defs.md#awscredentialstypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPermissionGroupResponseTypeDef

```python
# GetPermissionGroupResponseTypeDef definition

class GetPermissionGroupResponseTypeDef(TypedDict):
    permissionGroup: PermissionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionGroupTypeDef](./type_defs.md#permissiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionGroupsResponseTypeDef

```python
# ListPermissionGroupsResponseTypeDef definition

class ListPermissionGroupsResponseTypeDef(TypedDict):
    permissionGroups: List[PermissionGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PermissionGroupTypeDef](./type_defs.md#permissiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChangesetsRequestListChangesetsPaginateTypeDef

```python
# ListChangesetsRequestListChangesetsPaginateTypeDef definition

class ListChangesetsRequestListChangesetsPaginateTypeDef(TypedDict):
    datasetId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataViewsRequestListDataViewsPaginateTypeDef

```python
# ListDataViewsRequestListDataViewsPaginateTypeDef definition

class ListDataViewsRequestListDataViewsPaginateTypeDef(TypedDict):
    datasetId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetsRequestListDatasetsPaginateTypeDef

```python
# ListDatasetsRequestListDatasetsPaginateTypeDef definition

class ListDatasetsRequestListDatasetsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef

```python
# ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef definition

class ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestListUsersPaginateTypeDef

```python
# ListUsersRequestListUsersPaginateTypeDef definition

class ListUsersRequestListUsersPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPermissionGroupsByUserResponseTypeDef

```python
# ListPermissionGroupsByUserResponseTypeDef definition

class ListPermissionGroupsByUserResponseTypeDef(TypedDict):
    permissionGroups: List[PermissionGroupByUserTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PermissionGroupByUserTypeDef](./type_defs.md#permissiongroupbyusertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersByPermissionGroupResponseTypeDef

```python
# ListUsersByPermissionGroupResponseTypeDef definition

class ListUsersByPermissionGroupResponseTypeDef(TypedDict):
    users: List[UserByPermissionGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UserByPermissionGroupTypeDef](./type_defs.md#userbypermissiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsersResponseTypeDef

```python
# ListUsersResponseTypeDef definition

class ListUsersResponseTypeDef(TypedDict):
    users: List[UserTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PermissionGroupParamsTypeDef

```python
# PermissionGroupParamsTypeDef definition

class PermissionGroupParamsTypeDef(TypedDict):
    permissionGroupId: NotRequired[str],
    datasetPermissions: NotRequired[Sequence[ResourcePermissionTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourcePermissionTypeDef](./type_defs.md#resourcepermissiontypedef) 
## ListChangesetsResponseTypeDef

```python
# ListChangesetsResponseTypeDef definition

class ListChangesetsResponseTypeDef(TypedDict):
    changesets: List[ChangesetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ChangesetSummaryTypeDef](./type_defs.md#changesetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SchemaUnionOutputTypeDef

```python
# SchemaUnionOutputTypeDef definition

class SchemaUnionOutputTypeDef(TypedDict):
    tabularSchemaConfig: NotRequired[SchemaDefinitionOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 
## ListDataViewsResponseTypeDef

```python
# ListDataViewsResponseTypeDef definition

class ListDataViewsResponseTypeDef(TypedDict):
    dataViews: List[DataViewSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataViewSummaryTypeDef](./type_defs.md#dataviewsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetTypeDef

```python
# DatasetTypeDef definition

class DatasetTypeDef(TypedDict):
    datasetId: NotRequired[str],
    datasetArn: NotRequired[str],
    datasetTitle: NotRequired[str],
    kind: NotRequired[DatasetKindType],  # (1)
    datasetDescription: NotRequired[str],
    ownerInfo: NotRequired[DatasetOwnerInfoTypeDef],  # (2)
    createTime: NotRequired[int],
    lastModifiedTime: NotRequired[int],
    schemaDefinition: NotRequired[SchemaUnionOutputTypeDef],  # (3)
    alias: NotRequired[str],
```

1. See [:material-code-brackets: DatasetKindType](./literals.md#datasetkindtype) 
2. See [:material-code-braces: DatasetOwnerInfoTypeDef](./type_defs.md#datasetownerinfotypedef) 
3. See [:material-code-braces: SchemaUnionOutputTypeDef](./type_defs.md#schemaunionoutputtypedef) 
## GetDatasetResponseTypeDef

```python
# GetDatasetResponseTypeDef definition

class GetDatasetResponseTypeDef(TypedDict):
    datasetId: str,
    datasetArn: str,
    datasetTitle: str,
    kind: DatasetKindType,  # (1)
    datasetDescription: str,
    createTime: int,
    lastModifiedTime: int,
    schemaDefinition: SchemaUnionOutputTypeDef,  # (2)
    alias: str,
    status: DatasetStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DatasetKindType](./literals.md#datasetkindtype) 
2. See [:material-code-braces: SchemaUnionOutputTypeDef](./type_defs.md#schemaunionoutputtypedef) 
3. See [:material-code-brackets: DatasetStatusType](./literals.md#datasetstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SchemaUnionTypeDef

```python
# SchemaUnionTypeDef definition

class SchemaUnionTypeDef(TypedDict):
    tabularSchemaConfig: NotRequired[SchemaDefinitionUnionTypeDef],  # (1)
```

1. See [:material-code-braces: SchemaDefinitionTypeDef](./type_defs.md#schemadefinitiontypedef) [:material-code-braces: SchemaDefinitionOutputTypeDef](./type_defs.md#schemadefinitionoutputtypedef) 
## ListDatasetsResponseTypeDef

```python
# ListDatasetsResponseTypeDef definition

class ListDatasetsResponseTypeDef(TypedDict):
    datasets: List[DatasetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetRequestRequestTypeDef

```python
# CreateDatasetRequestRequestTypeDef definition

class CreateDatasetRequestRequestTypeDef(TypedDict):
    datasetTitle: str,
    kind: DatasetKindType,  # (1)
    permissionGroupParams: PermissionGroupParamsTypeDef,  # (2)
    clientToken: NotRequired[str],
    datasetDescription: NotRequired[str],
    ownerInfo: NotRequired[DatasetOwnerInfoTypeDef],  # (3)
    alias: NotRequired[str],
    schemaDefinition: NotRequired[SchemaUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: DatasetKindType](./literals.md#datasetkindtype) 
2. See [:material-code-braces: PermissionGroupParamsTypeDef](./type_defs.md#permissiongroupparamstypedef) 
3. See [:material-code-braces: DatasetOwnerInfoTypeDef](./type_defs.md#datasetownerinfotypedef) 
4. See [:material-code-braces: SchemaUnionTypeDef](./type_defs.md#schemauniontypedef) 
## UpdateDatasetRequestRequestTypeDef

```python
# UpdateDatasetRequestRequestTypeDef definition

class UpdateDatasetRequestRequestTypeDef(TypedDict):
    datasetId: str,
    datasetTitle: str,
    kind: DatasetKindType,  # (1)
    clientToken: NotRequired[str],
    datasetDescription: NotRequired[str],
    alias: NotRequired[str],
    schemaDefinition: NotRequired[SchemaUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: DatasetKindType](./literals.md#datasetkindtype) 
2. See [:material-code-braces: SchemaUnionTypeDef](./type_defs.md#schemauniontypedef) 
