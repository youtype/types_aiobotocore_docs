# Type definitions

> [Index](../README.md) > [ManagedGrafana](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#ManagedGrafana)
    type annotations stubs module [types-aiobotocore-grafana](https://pypi.org/project/types-aiobotocore-grafana/).

## RoleValuesUnionTypeDef

```python
# RoleValuesUnionTypeDef definition

RoleValuesUnionTypeDef = Union[
    RoleValuesTypeDef,  # (1)
    RoleValuesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RoleValuesTypeDef](./type_defs.md#rolevaluestypedef) 
2. See [:material-code-braces: RoleValuesOutputTypeDef](./type_defs.md#rolevaluesoutputtypedef) 

## UpdateInstructionUnionTypeDef

```python
# UpdateInstructionUnionTypeDef definition

UpdateInstructionUnionTypeDef = Union[
    UpdateInstructionTypeDef,  # (1)
    UpdateInstructionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UpdateInstructionTypeDef](./type_defs.md#updateinstructiontypedef) 
2. See [:material-code-braces: UpdateInstructionOutputTypeDef](./type_defs.md#updateinstructionoutputtypedef) 



## AssertionAttributesTypeDef

```python
# AssertionAttributesTypeDef definition

class AssertionAttributesTypeDef(TypedDict):
    email: NotRequired[str],
    groups: NotRequired[str],
    login: NotRequired[str],
    name: NotRequired[str],
    org: NotRequired[str],
    role: NotRequired[str],
```

## AssociateLicenseRequestRequestTypeDef

```python
# AssociateLicenseRequestRequestTypeDef definition

class AssociateLicenseRequestRequestTypeDef(TypedDict):
    licenseType: LicenseTypeType,  # (1)
    workspaceId: str,
    grafanaToken: NotRequired[str],
```

1. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
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

## AwsSsoAuthenticationTypeDef

```python
# AwsSsoAuthenticationTypeDef definition

class AwsSsoAuthenticationTypeDef(TypedDict):
    ssoClientId: NotRequired[str],
```

## AuthenticationSummaryTypeDef

```python
# AuthenticationSummaryTypeDef definition

class AuthenticationSummaryTypeDef(TypedDict):
    providers: List[AuthenticationProviderTypesType],  # (1)
    samlConfigurationStatus: NotRequired[SamlConfigurationStatusType],  # (2)
```

1. See [:material-code-brackets: AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype) 
2. See [:material-code-brackets: SamlConfigurationStatusType](./literals.md#samlconfigurationstatustype) 
## CreateWorkspaceApiKeyRequestRequestTypeDef

```python
# CreateWorkspaceApiKeyRequestRequestTypeDef definition

class CreateWorkspaceApiKeyRequestRequestTypeDef(TypedDict):
    keyName: str,
    keyRole: str,
    secondsToLive: int,
    workspaceId: str,
```

## NetworkAccessConfigurationTypeDef

```python
# NetworkAccessConfigurationTypeDef definition

class NetworkAccessConfigurationTypeDef(TypedDict):
    prefixListIds: Sequence[str],
    vpceIds: Sequence[str],
```

## VpcConfigurationTypeDef

```python
# VpcConfigurationTypeDef definition

class VpcConfigurationTypeDef(TypedDict):
    securityGroupIds: Sequence[str],
    subnetIds: Sequence[str],
```

## CreateWorkspaceServiceAccountRequestRequestTypeDef

```python
# CreateWorkspaceServiceAccountRequestRequestTypeDef definition

class CreateWorkspaceServiceAccountRequestRequestTypeDef(TypedDict):
    grafanaRole: RoleType,  # (1)
    name: str,
    workspaceId: str,
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
## CreateWorkspaceServiceAccountTokenRequestRequestTypeDef

```python
# CreateWorkspaceServiceAccountTokenRequestRequestTypeDef definition

class CreateWorkspaceServiceAccountTokenRequestRequestTypeDef(TypedDict):
    name: str,
    secondsToLive: int,
    serviceAccountId: str,
    workspaceId: str,
```

## ServiceAccountTokenSummaryWithKeyTypeDef

```python
# ServiceAccountTokenSummaryWithKeyTypeDef definition

class ServiceAccountTokenSummaryWithKeyTypeDef(TypedDict):
    id: str,
    key: str,
    name: str,
```

## DeleteWorkspaceApiKeyRequestRequestTypeDef

```python
# DeleteWorkspaceApiKeyRequestRequestTypeDef definition

class DeleteWorkspaceApiKeyRequestRequestTypeDef(TypedDict):
    keyName: str,
    workspaceId: str,
```

## DeleteWorkspaceRequestRequestTypeDef

```python
# DeleteWorkspaceRequestRequestTypeDef definition

class DeleteWorkspaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DeleteWorkspaceServiceAccountRequestRequestTypeDef

```python
# DeleteWorkspaceServiceAccountRequestRequestTypeDef definition

class DeleteWorkspaceServiceAccountRequestRequestTypeDef(TypedDict):
    serviceAccountId: str,
    workspaceId: str,
```

## DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef

```python
# DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef definition

class DeleteWorkspaceServiceAccountTokenRequestRequestTypeDef(TypedDict):
    serviceAccountId: str,
    tokenId: str,
    workspaceId: str,
```

## DescribeWorkspaceAuthenticationRequestRequestTypeDef

```python
# DescribeWorkspaceAuthenticationRequestRequestTypeDef definition

class DescribeWorkspaceAuthenticationRequestRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DescribeWorkspaceConfigurationRequestRequestTypeDef

```python
# DescribeWorkspaceConfigurationRequestRequestTypeDef definition

class DescribeWorkspaceConfigurationRequestRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DescribeWorkspaceRequestRequestTypeDef

```python
# DescribeWorkspaceRequestRequestTypeDef definition

class DescribeWorkspaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
```

## DisassociateLicenseRequestRequestTypeDef

```python
# DisassociateLicenseRequestRequestTypeDef definition

class DisassociateLicenseRequestRequestTypeDef(TypedDict):
    licenseType: LicenseTypeType,  # (1)
    workspaceId: str,
```

1. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
## IdpMetadataTypeDef

```python
# IdpMetadataTypeDef definition

class IdpMetadataTypeDef(TypedDict):
    url: NotRequired[str],
    xml: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListPermissionsRequestRequestTypeDef

```python
# ListPermissionsRequestRequestTypeDef definition

class ListPermissionsRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    groupId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    userId: NotRequired[str],
    userType: NotRequired[UserTypeType],  # (1)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListVersionsRequestRequestTypeDef

```python
# ListVersionsRequestRequestTypeDef definition

class ListVersionsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    workspaceId: NotRequired[str],
```

## ListWorkspaceServiceAccountTokensRequestRequestTypeDef

```python
# ListWorkspaceServiceAccountTokensRequestRequestTypeDef definition

class ListWorkspaceServiceAccountTokensRequestRequestTypeDef(TypedDict):
    serviceAccountId: str,
    workspaceId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ServiceAccountTokenSummaryTypeDef

```python
# ServiceAccountTokenSummaryTypeDef definition

class ServiceAccountTokenSummaryTypeDef(TypedDict):
    createdAt: datetime,
    expiresAt: datetime,
    id: str,
    name: str,
    lastUsedAt: NotRequired[datetime],
```

## ListWorkspaceServiceAccountsRequestRequestTypeDef

```python
# ListWorkspaceServiceAccountsRequestRequestTypeDef definition

class ListWorkspaceServiceAccountsRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ServiceAccountSummaryTypeDef

```python
# ServiceAccountSummaryTypeDef definition

class ServiceAccountSummaryTypeDef(TypedDict):
    grafanaRole: RoleType,  # (1)
    id: str,
    isDisabled: str,
    name: str,
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
## ListWorkspacesRequestRequestTypeDef

```python
# ListWorkspacesRequestRequestTypeDef definition

class ListWorkspacesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## NetworkAccessConfigurationOutputTypeDef

```python
# NetworkAccessConfigurationOutputTypeDef definition

class NetworkAccessConfigurationOutputTypeDef(TypedDict):
    prefixListIds: List[str],
    vpceIds: List[str],
```

## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    id: str,
    type: UserTypeType,  # (1)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## RoleValuesOutputTypeDef

```python
# RoleValuesOutputTypeDef definition

class RoleValuesOutputTypeDef(TypedDict):
    admin: NotRequired[List[str]],
    editor: NotRequired[List[str]],
```

## RoleValuesTypeDef

```python
# RoleValuesTypeDef definition

class RoleValuesTypeDef(TypedDict):
    admin: NotRequired[Sequence[str]],
    editor: NotRequired[Sequence[str]],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateWorkspaceConfigurationRequestRequestTypeDef

```python
# UpdateWorkspaceConfigurationRequestRequestTypeDef definition

class UpdateWorkspaceConfigurationRequestRequestTypeDef(TypedDict):
    configuration: str,
    workspaceId: str,
    grafanaVersion: NotRequired[str],
```

## VpcConfigurationOutputTypeDef

```python
# VpcConfigurationOutputTypeDef definition

class VpcConfigurationOutputTypeDef(TypedDict):
    securityGroupIds: List[str],
    subnetIds: List[str],
```

## CreateWorkspaceApiKeyResponseTypeDef

```python
# CreateWorkspaceApiKeyResponseTypeDef definition

class CreateWorkspaceApiKeyResponseTypeDef(TypedDict):
    key: str,
    keyName: str,
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspaceServiceAccountResponseTypeDef

```python
# CreateWorkspaceServiceAccountResponseTypeDef definition

class CreateWorkspaceServiceAccountResponseTypeDef(TypedDict):
    grafanaRole: RoleType,  # (1)
    id: str,
    name: str,
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkspaceApiKeyResponseTypeDef

```python
# DeleteWorkspaceApiKeyResponseTypeDef definition

class DeleteWorkspaceApiKeyResponseTypeDef(TypedDict):
    keyName: str,
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkspaceServiceAccountResponseTypeDef

```python
# DeleteWorkspaceServiceAccountResponseTypeDef definition

class DeleteWorkspaceServiceAccountResponseTypeDef(TypedDict):
    serviceAccountId: str,
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkspaceServiceAccountTokenResponseTypeDef

```python
# DeleteWorkspaceServiceAccountTokenResponseTypeDef definition

class DeleteWorkspaceServiceAccountTokenResponseTypeDef(TypedDict):
    serviceAccountId: str,
    tokenId: str,
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceConfigurationResponseTypeDef

```python
# DescribeWorkspaceConfigurationResponseTypeDef definition

class DescribeWorkspaceConfigurationResponseTypeDef(TypedDict):
    configuration: str,
    grafanaVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVersionsResponseTypeDef

```python
# ListVersionsResponseTypeDef definition

class ListVersionsResponseTypeDef(TypedDict):
    grafanaVersions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkspaceSummaryTypeDef

```python
# WorkspaceSummaryTypeDef definition

class WorkspaceSummaryTypeDef(TypedDict):
    authentication: AuthenticationSummaryTypeDef,  # (1)
    created: datetime,
    endpoint: str,
    grafanaVersion: str,
    id: str,
    modified: datetime,
    status: WorkspaceStatusType,  # (4)
    description: NotRequired[str],
    grafanaToken: NotRequired[str],
    licenseType: NotRequired[LicenseTypeType],  # (2)
    name: NotRequired[str],
    notificationDestinations: NotRequired[List[NotificationDestinationTypeType]],  # (3)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AuthenticationSummaryTypeDef](./type_defs.md#authenticationsummarytypedef) 
2. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
3. See [:material-code-brackets: NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype) 
4. See [:material-code-brackets: WorkspaceStatusType](./literals.md#workspacestatustype) 
## CreateWorkspaceRequestRequestTypeDef

```python
# CreateWorkspaceRequestRequestTypeDef definition

class CreateWorkspaceRequestRequestTypeDef(TypedDict):
    accountAccessType: AccountAccessTypeType,  # (1)
    authenticationProviders: Sequence[AuthenticationProviderTypesType],  # (2)
    permissionType: PermissionTypeType,  # (3)
    clientToken: NotRequired[str],
    configuration: NotRequired[str],
    grafanaVersion: NotRequired[str],
    networkAccessControl: NotRequired[NetworkAccessConfigurationTypeDef],  # (4)
    organizationRoleName: NotRequired[str],
    stackSetName: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    vpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (5)
    workspaceDataSources: NotRequired[Sequence[DataSourceTypeType]],  # (6)
    workspaceDescription: NotRequired[str],
    workspaceName: NotRequired[str],
    workspaceNotificationDestinations: NotRequired[Sequence[NotificationDestinationTypeType]],  # (7)
    workspaceOrganizationalUnits: NotRequired[Sequence[str]],
    workspaceRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: AccountAccessTypeType](./literals.md#accountaccesstypetype) 
2. See [:material-code-brackets: AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype) 
3. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
4. See [:material-code-braces: NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef) 
5. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
6. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
7. See [:material-code-brackets: NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype) 
## UpdateWorkspaceRequestRequestTypeDef

```python
# UpdateWorkspaceRequestRequestTypeDef definition

class UpdateWorkspaceRequestRequestTypeDef(TypedDict):
    workspaceId: str,
    accountAccessType: NotRequired[AccountAccessTypeType],  # (1)
    networkAccessControl: NotRequired[NetworkAccessConfigurationTypeDef],  # (2)
    organizationRoleName: NotRequired[str],
    permissionType: NotRequired[PermissionTypeType],  # (3)
    removeNetworkAccessConfiguration: NotRequired[bool],
    removeVpcConfiguration: NotRequired[bool],
    stackSetName: NotRequired[str],
    vpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (4)
    workspaceDataSources: NotRequired[Sequence[DataSourceTypeType]],  # (5)
    workspaceDescription: NotRequired[str],
    workspaceName: NotRequired[str],
    workspaceNotificationDestinations: NotRequired[Sequence[NotificationDestinationTypeType]],  # (6)
    workspaceOrganizationalUnits: NotRequired[Sequence[str]],
    workspaceRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: AccountAccessTypeType](./literals.md#accountaccesstypetype) 
2. See [:material-code-braces: NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef) 
3. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
4. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
5. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
6. See [:material-code-brackets: NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype) 
## CreateWorkspaceServiceAccountTokenResponseTypeDef

```python
# CreateWorkspaceServiceAccountTokenResponseTypeDef definition

class CreateWorkspaceServiceAccountTokenResponseTypeDef(TypedDict):
    serviceAccountId: str,
    serviceAccountToken: ServiceAccountTokenSummaryWithKeyTypeDef,  # (1)
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceAccountTokenSummaryWithKeyTypeDef](./type_defs.md#serviceaccounttokensummarywithkeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionsRequestListPermissionsPaginateTypeDef

```python
# ListPermissionsRequestListPermissionsPaginateTypeDef definition

class ListPermissionsRequestListPermissionsPaginateTypeDef(TypedDict):
    workspaceId: str,
    groupId: NotRequired[str],
    userId: NotRequired[str],
    userType: NotRequired[UserTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVersionsRequestListVersionsPaginateTypeDef

```python
# ListVersionsRequestListVersionsPaginateTypeDef definition

class ListVersionsRequestListVersionsPaginateTypeDef(TypedDict):
    workspaceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkspaceServiceAccountTokensRequestListWorkspaceServiceAccountTokensPaginateTypeDef

```python
# ListWorkspaceServiceAccountTokensRequestListWorkspaceServiceAccountTokensPaginateTypeDef definition

class ListWorkspaceServiceAccountTokensRequestListWorkspaceServiceAccountTokensPaginateTypeDef(TypedDict):
    serviceAccountId: str,
    workspaceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkspaceServiceAccountsRequestListWorkspaceServiceAccountsPaginateTypeDef

```python
# ListWorkspaceServiceAccountsRequestListWorkspaceServiceAccountsPaginateTypeDef definition

class ListWorkspaceServiceAccountsRequestListWorkspaceServiceAccountsPaginateTypeDef(TypedDict):
    workspaceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkspacesRequestListWorkspacesPaginateTypeDef

```python
# ListWorkspacesRequestListWorkspacesPaginateTypeDef definition

class ListWorkspacesRequestListWorkspacesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkspaceServiceAccountTokensResponseTypeDef

```python
# ListWorkspaceServiceAccountTokensResponseTypeDef definition

class ListWorkspaceServiceAccountTokensResponseTypeDef(TypedDict):
    serviceAccountId: str,
    serviceAccountTokens: List[ServiceAccountTokenSummaryTypeDef],  # (1)
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceAccountTokenSummaryTypeDef](./type_defs.md#serviceaccounttokensummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkspaceServiceAccountsResponseTypeDef

```python
# ListWorkspaceServiceAccountsResponseTypeDef definition

class ListWorkspaceServiceAccountsResponseTypeDef(TypedDict):
    serviceAccounts: List[ServiceAccountSummaryTypeDef],  # (1)
    workspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceAccountSummaryTypeDef](./type_defs.md#serviceaccountsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PermissionEntryTypeDef

```python
# PermissionEntryTypeDef definition

class PermissionEntryTypeDef(TypedDict):
    role: RoleType,  # (1)
    user: UserTypeDef,  # (2)
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
2. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
## UpdateInstructionOutputTypeDef

```python
# UpdateInstructionOutputTypeDef definition

class UpdateInstructionOutputTypeDef(TypedDict):
    action: UpdateActionType,  # (1)
    role: RoleType,  # (2)
    users: List[UserTypeDef],  # (3)
```

1. See [:material-code-brackets: UpdateActionType](./literals.md#updateactiontype) 
2. See [:material-code-brackets: RoleType](./literals.md#roletype) 
3. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
## UpdateInstructionTypeDef

```python
# UpdateInstructionTypeDef definition

class UpdateInstructionTypeDef(TypedDict):
    action: UpdateActionType,  # (1)
    role: RoleType,  # (2)
    users: Sequence[UserTypeDef],  # (3)
```

1. See [:material-code-brackets: UpdateActionType](./literals.md#updateactiontype) 
2. See [:material-code-brackets: RoleType](./literals.md#roletype) 
3. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
## SamlConfigurationOutputTypeDef

```python
# SamlConfigurationOutputTypeDef definition

class SamlConfigurationOutputTypeDef(TypedDict):
    idpMetadata: IdpMetadataTypeDef,  # (2)
    allowedOrganizations: NotRequired[List[str]],
    assertionAttributes: NotRequired[AssertionAttributesTypeDef],  # (1)
    loginValidityDuration: NotRequired[int],
    roleValues: NotRequired[RoleValuesOutputTypeDef],  # (3)
```

1. See [:material-code-braces: AssertionAttributesTypeDef](./type_defs.md#assertionattributestypedef) 
2. See [:material-code-braces: IdpMetadataTypeDef](./type_defs.md#idpmetadatatypedef) 
3. See [:material-code-braces: RoleValuesOutputTypeDef](./type_defs.md#rolevaluesoutputtypedef) 
## WorkspaceDescriptionTypeDef

```python
# WorkspaceDescriptionTypeDef definition

class WorkspaceDescriptionTypeDef(TypedDict):
    authentication: AuthenticationSummaryTypeDef,  # (2)
    created: datetime,
    dataSources: List[DataSourceTypeType],  # (3)
    endpoint: str,
    grafanaVersion: str,
    id: str,
    modified: datetime,
    status: WorkspaceStatusType,  # (8)
    accountAccessType: NotRequired[AccountAccessTypeType],  # (1)
    description: NotRequired[str],
    freeTrialConsumed: NotRequired[bool],
    freeTrialExpiration: NotRequired[datetime],
    grafanaToken: NotRequired[str],
    licenseExpiration: NotRequired[datetime],
    licenseType: NotRequired[LicenseTypeType],  # (4)
    name: NotRequired[str],
    networkAccessControl: NotRequired[NetworkAccessConfigurationOutputTypeDef],  # (5)
    notificationDestinations: NotRequired[List[NotificationDestinationTypeType]],  # (6)
    organizationRoleName: NotRequired[str],
    organizationalUnits: NotRequired[List[str]],
    permissionType: NotRequired[PermissionTypeType],  # (7)
    stackSetName: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    vpcConfiguration: NotRequired[VpcConfigurationOutputTypeDef],  # (9)
    workspaceRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: AccountAccessTypeType](./literals.md#accountaccesstypetype) 
2. See [:material-code-braces: AuthenticationSummaryTypeDef](./type_defs.md#authenticationsummarytypedef) 
3. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
4. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
5. See [:material-code-braces: NetworkAccessConfigurationOutputTypeDef](./type_defs.md#networkaccessconfigurationoutputtypedef) 
6. See [:material-code-brackets: NotificationDestinationTypeType](./literals.md#notificationdestinationtypetype) 
7. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
8. See [:material-code-brackets: WorkspaceStatusType](./literals.md#workspacestatustype) 
9. See [:material-code-braces: VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef) 
## ListWorkspacesResponseTypeDef

```python
# ListWorkspacesResponseTypeDef definition

class ListWorkspacesResponseTypeDef(TypedDict):
    workspaces: List[WorkspaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceSummaryTypeDef](./type_defs.md#workspacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionsResponseTypeDef

```python
# ListPermissionsResponseTypeDef definition

class ListPermissionsResponseTypeDef(TypedDict):
    permissions: List[PermissionEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PermissionEntryTypeDef](./type_defs.md#permissionentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateErrorTypeDef

```python
# UpdateErrorTypeDef definition

class UpdateErrorTypeDef(TypedDict):
    causedBy: UpdateInstructionOutputTypeDef,  # (1)
    code: int,
    message: str,
```

1. See [:material-code-braces: UpdateInstructionOutputTypeDef](./type_defs.md#updateinstructionoutputtypedef) 
## SamlAuthenticationTypeDef

```python
# SamlAuthenticationTypeDef definition

class SamlAuthenticationTypeDef(TypedDict):
    status: SamlConfigurationStatusType,  # (2)
    configuration: NotRequired[SamlConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SamlConfigurationOutputTypeDef](./type_defs.md#samlconfigurationoutputtypedef) 
2. See [:material-code-brackets: SamlConfigurationStatusType](./literals.md#samlconfigurationstatustype) 
## SamlConfigurationTypeDef

```python
# SamlConfigurationTypeDef definition

class SamlConfigurationTypeDef(TypedDict):
    idpMetadata: IdpMetadataTypeDef,  # (2)
    allowedOrganizations: NotRequired[Sequence[str]],
    assertionAttributes: NotRequired[AssertionAttributesTypeDef],  # (1)
    loginValidityDuration: NotRequired[int],
    roleValues: NotRequired[RoleValuesUnionTypeDef],  # (3)
```

1. See [:material-code-braces: AssertionAttributesTypeDef](./type_defs.md#assertionattributestypedef) 
2. See [:material-code-braces: IdpMetadataTypeDef](./type_defs.md#idpmetadatatypedef) 
3. See [:material-code-braces: RoleValuesTypeDef](./type_defs.md#rolevaluestypedef) [:material-code-braces: RoleValuesOutputTypeDef](./type_defs.md#rolevaluesoutputtypedef) 
## AssociateLicenseResponseTypeDef

```python
# AssociateLicenseResponseTypeDef definition

class AssociateLicenseResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspaceResponseTypeDef

```python
# CreateWorkspaceResponseTypeDef definition

class CreateWorkspaceResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkspaceResponseTypeDef

```python
# DeleteWorkspaceResponseTypeDef definition

class DeleteWorkspaceResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceResponseTypeDef

```python
# DescribeWorkspaceResponseTypeDef definition

class DescribeWorkspaceResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateLicenseResponseTypeDef

```python
# DisassociateLicenseResponseTypeDef definition

class DisassociateLicenseResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkspaceResponseTypeDef

```python
# UpdateWorkspaceResponseTypeDef definition

class UpdateWorkspaceResponseTypeDef(TypedDict):
    workspace: WorkspaceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDescriptionTypeDef](./type_defs.md#workspacedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePermissionsResponseTypeDef

```python
# UpdatePermissionsResponseTypeDef definition

class UpdatePermissionsResponseTypeDef(TypedDict):
    errors: List[UpdateErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateErrorTypeDef](./type_defs.md#updateerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePermissionsRequestRequestTypeDef

```python
# UpdatePermissionsRequestRequestTypeDef definition

class UpdatePermissionsRequestRequestTypeDef(TypedDict):
    updateInstructionBatch: Sequence[UpdateInstructionUnionTypeDef],  # (1)
    workspaceId: str,
```

1. See [:material-code-braces: UpdateInstructionTypeDef](./type_defs.md#updateinstructiontypedef) [:material-code-braces: UpdateInstructionOutputTypeDef](./type_defs.md#updateinstructionoutputtypedef) 
## AuthenticationDescriptionTypeDef

```python
# AuthenticationDescriptionTypeDef definition

class AuthenticationDescriptionTypeDef(TypedDict):
    providers: List[AuthenticationProviderTypesType],  # (2)
    awsSso: NotRequired[AwsSsoAuthenticationTypeDef],  # (1)
    saml: NotRequired[SamlAuthenticationTypeDef],  # (3)
```

1. See [:material-code-braces: AwsSsoAuthenticationTypeDef](./type_defs.md#awsssoauthenticationtypedef) 
2. See [:material-code-brackets: AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype) 
3. See [:material-code-braces: SamlAuthenticationTypeDef](./type_defs.md#samlauthenticationtypedef) 
## UpdateWorkspaceAuthenticationRequestRequestTypeDef

```python
# UpdateWorkspaceAuthenticationRequestRequestTypeDef definition

class UpdateWorkspaceAuthenticationRequestRequestTypeDef(TypedDict):
    authenticationProviders: Sequence[AuthenticationProviderTypesType],  # (1)
    workspaceId: str,
    samlConfiguration: NotRequired[SamlConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthenticationProviderTypesType](./literals.md#authenticationprovidertypestype) 
2. See [:material-code-braces: SamlConfigurationTypeDef](./type_defs.md#samlconfigurationtypedef) 
## DescribeWorkspaceAuthenticationResponseTypeDef

```python
# DescribeWorkspaceAuthenticationResponseTypeDef definition

class DescribeWorkspaceAuthenticationResponseTypeDef(TypedDict):
    authentication: AuthenticationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthenticationDescriptionTypeDef](./type_defs.md#authenticationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkspaceAuthenticationResponseTypeDef

```python
# UpdateWorkspaceAuthenticationResponseTypeDef definition

class UpdateWorkspaceAuthenticationResponseTypeDef(TypedDict):
    authentication: AuthenticationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthenticationDescriptionTypeDef](./type_defs.md#authenticationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
