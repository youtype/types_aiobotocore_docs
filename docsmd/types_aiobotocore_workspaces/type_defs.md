# Type definitions

> [Index](../README.md) > [WorkSpaces](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#WorkSpaces)
    type annotations stubs module [types-aiobotocore-workspaces](https://pypi.org/project/types-aiobotocore-workspaces/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## WorkspacePropertiesUnionTypeDef

```python
# WorkspacePropertiesUnionTypeDef definition

WorkspacePropertiesUnionTypeDef = Union[
    WorkspacePropertiesTypeDef,  # (1)
    WorkspacePropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WorkspacePropertiesTypeDef](./type_defs.md#workspacepropertiestypedef) 
2. See [:material-code-braces: WorkspacePropertiesOutputTypeDef](./type_defs.md#workspacepropertiesoutputtypedef) 

## StandbyWorkspaceUnionTypeDef

```python
# StandbyWorkspaceUnionTypeDef definition

StandbyWorkspaceUnionTypeDef = Union[
    StandbyWorkspaceTypeDef,  # (1)
    StandbyWorkspaceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StandbyWorkspaceTypeDef](./type_defs.md#standbyworkspacetypedef) 
2. See [:material-code-braces: StandbyWorkspaceOutputTypeDef](./type_defs.md#standbyworkspaceoutputtypedef) 

## WorkspaceRequestUnionTypeDef

```python
# WorkspaceRequestUnionTypeDef definition

WorkspaceRequestUnionTypeDef = Union[
    WorkspaceRequestTypeDef,  # (1)
    WorkspaceRequestOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WorkspaceRequestTypeDef](./type_defs.md#workspacerequesttypedef) 
2. See [:material-code-braces: WorkspaceRequestOutputTypeDef](./type_defs.md#workspacerequestoutputtypedef) 



## AcceptAccountLinkInvitationRequestRequestTypeDef

```python
# AcceptAccountLinkInvitationRequestRequestTypeDef definition

class AcceptAccountLinkInvitationRequestRequestTypeDef(TypedDict):
    LinkId: str,
    ClientToken: NotRequired[str],
```

## AccountLinkTypeDef

```python
# AccountLinkTypeDef definition

class AccountLinkTypeDef(TypedDict):
    AccountLinkId: NotRequired[str],
    AccountLinkStatus: NotRequired[AccountLinkStatusEnumType],  # (1)
    SourceAccountId: NotRequired[str],
    TargetAccountId: NotRequired[str],
```

1. See [:material-code-brackets: AccountLinkStatusEnumType](./literals.md#accountlinkstatusenumtype) 
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

## AccountModificationTypeDef

```python
# AccountModificationTypeDef definition

class AccountModificationTypeDef(TypedDict):
    ModificationState: NotRequired[DedicatedTenancyModificationStateEnumType],  # (1)
    DedicatedTenancySupport: NotRequired[DedicatedTenancySupportResultEnumType],  # (2)
    DedicatedTenancyManagementCidrRange: NotRequired[str],
    StartTime: NotRequired[datetime],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: DedicatedTenancyModificationStateEnumType](./literals.md#dedicatedtenancymodificationstateenumtype) 
2. See [:material-code-brackets: DedicatedTenancySupportResultEnumType](./literals.md#dedicatedtenancysupportresultenumtype) 
## ActiveDirectoryConfigTypeDef

```python
# ActiveDirectoryConfigTypeDef definition

class ActiveDirectoryConfigTypeDef(TypedDict):
    DomainName: str,
    ServiceAccountSecretArn: str,
```

## AssociationStateReasonTypeDef

```python
# AssociationStateReasonTypeDef definition

class AssociationStateReasonTypeDef(TypedDict):
    ErrorCode: NotRequired[AssociationErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: AssociationErrorCodeType](./literals.md#associationerrorcodetype) 
## ApplicationSettingsRequestTypeDef

```python
# ApplicationSettingsRequestTypeDef definition

class ApplicationSettingsRequestTypeDef(TypedDict):
    Status: ApplicationSettingsStatusEnumType,  # (1)
    SettingsGroup: NotRequired[str],
```

1. See [:material-code-brackets: ApplicationSettingsStatusEnumType](./literals.md#applicationsettingsstatusenumtype) 
## ApplicationSettingsResponseTypeDef

```python
# ApplicationSettingsResponseTypeDef definition

class ApplicationSettingsResponseTypeDef(TypedDict):
    Status: ApplicationSettingsStatusEnumType,  # (1)
    SettingsGroup: NotRequired[str],
    S3BucketName: NotRequired[str],
```

1. See [:material-code-brackets: ApplicationSettingsStatusEnumType](./literals.md#applicationsettingsstatusenumtype) 
## AssociateConnectionAliasRequestRequestTypeDef

```python
# AssociateConnectionAliasRequestRequestTypeDef definition

class AssociateConnectionAliasRequestRequestTypeDef(TypedDict):
    AliasId: str,
    ResourceId: str,
```

## AssociateIpGroupsRequestRequestTypeDef

```python
# AssociateIpGroupsRequestRequestTypeDef definition

class AssociateIpGroupsRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    GroupIds: Sequence[str],
```

## AssociateWorkspaceApplicationRequestRequestTypeDef

```python
# AssociateWorkspaceApplicationRequestRequestTypeDef definition

class AssociateWorkspaceApplicationRequestRequestTypeDef(TypedDict):
    WorkspaceId: str,
    ApplicationId: str,
```

## IpRuleItemTypeDef

```python
# IpRuleItemTypeDef definition

class IpRuleItemTypeDef(TypedDict):
    ipRule: NotRequired[str],
    ruleDesc: NotRequired[str],
```

## CapacityStatusTypeDef

```python
# CapacityStatusTypeDef definition

class CapacityStatusTypeDef(TypedDict):
    AvailableUserSessions: int,
    DesiredUserSessions: int,
    ActualUserSessions: int,
    ActiveUserSessions: int,
```

## CapacityTypeDef

```python
# CapacityTypeDef definition

class CapacityTypeDef(TypedDict):
    DesiredUserSessions: int,
```

## CertificateBasedAuthPropertiesTypeDef

```python
# CertificateBasedAuthPropertiesTypeDef definition

class CertificateBasedAuthPropertiesTypeDef(TypedDict):
    Status: NotRequired[CertificateBasedAuthStatusEnumType],  # (1)
    CertificateAuthorityArn: NotRequired[str],
```

1. See [:material-code-brackets: CertificateBasedAuthStatusEnumType](./literals.md#certificatebasedauthstatusenumtype) 
## ClientPropertiesTypeDef

```python
# ClientPropertiesTypeDef definition

class ClientPropertiesTypeDef(TypedDict):
    ReconnectEnabled: NotRequired[ReconnectEnumType],  # (1)
    LogUploadEnabled: NotRequired[LogUploadEnumType],  # (2)
```

1. See [:material-code-brackets: ReconnectEnumType](./literals.md#reconnectenumtype) 
2. See [:material-code-brackets: LogUploadEnumType](./literals.md#loguploadenumtype) 
## ComputeTypeTypeDef

```python
# ComputeTypeTypeDef definition

class ComputeTypeTypeDef(TypedDict):
    Name: NotRequired[ComputeType],  # (1)
```

1. See [:material-code-brackets: ComputeType](./literals.md#computetype) 
## ConnectClientAddInTypeDef

```python
# ConnectClientAddInTypeDef definition

class ConnectClientAddInTypeDef(TypedDict):
    AddInId: NotRequired[str],
    ResourceId: NotRequired[str],
    Name: NotRequired[str],
    URL: NotRequired[str],
```

## ConnectionAliasAssociationTypeDef

```python
# ConnectionAliasAssociationTypeDef definition

class ConnectionAliasAssociationTypeDef(TypedDict):
    AssociationStatus: NotRequired[AssociationStatusType],  # (1)
    AssociatedAccountId: NotRequired[str],
    ResourceId: NotRequired[str],
    ConnectionIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: AssociationStatusType](./literals.md#associationstatustype) 
## ConnectionAliasPermissionTypeDef

```python
# ConnectionAliasPermissionTypeDef definition

class ConnectionAliasPermissionTypeDef(TypedDict):
    SharedAccountId: str,
    AllowAssociation: bool,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## CreateAccountLinkInvitationRequestRequestTypeDef

```python
# CreateAccountLinkInvitationRequestRequestTypeDef definition

class CreateAccountLinkInvitationRequestRequestTypeDef(TypedDict):
    TargetAccountId: str,
    ClientToken: NotRequired[str],
```

## CreateConnectClientAddInRequestRequestTypeDef

```python
# CreateConnectClientAddInRequestRequestTypeDef definition

class CreateConnectClientAddInRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    Name: str,
    URL: str,
```

## PendingCreateStandbyWorkspacesRequestTypeDef

```python
# PendingCreateStandbyWorkspacesRequestTypeDef definition

class PendingCreateStandbyWorkspacesRequestTypeDef(TypedDict):
    UserName: NotRequired[str],
    DirectoryId: NotRequired[str],
    State: NotRequired[WorkspaceStateType],  # (1)
    WorkspaceId: NotRequired[str],
```

1. See [:material-code-brackets: WorkspaceStateType](./literals.md#workspacestatetype) 
## RootStorageTypeDef

```python
# RootStorageTypeDef definition

class RootStorageTypeDef(TypedDict):
    Capacity: str,
```

## UserStorageTypeDef

```python
# UserStorageTypeDef definition

class UserStorageTypeDef(TypedDict):
    Capacity: str,
```

## OperatingSystemTypeDef

```python
# OperatingSystemTypeDef definition

class OperatingSystemTypeDef(TypedDict):
    Type: NotRequired[OperatingSystemTypeType],  # (1)
```

1. See [:material-code-brackets: OperatingSystemTypeType](./literals.md#operatingsystemtypetype) 
## TimeoutSettingsTypeDef

```python
# TimeoutSettingsTypeDef definition

class TimeoutSettingsTypeDef(TypedDict):
    DisconnectTimeoutInSeconds: NotRequired[int],
    IdleDisconnectTimeoutInSeconds: NotRequired[int],
    MaxUserDurationInSeconds: NotRequired[int],
```

## DataReplicationSettingsTypeDef

```python
# DataReplicationSettingsTypeDef definition

class DataReplicationSettingsTypeDef(TypedDict):
    DataReplication: NotRequired[DataReplicationType],  # (1)
    RecoverySnapshotTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DataReplicationType](./literals.md#datareplicationtype) 
## DefaultClientBrandingAttributesTypeDef

```python
# DefaultClientBrandingAttributesTypeDef definition

class DefaultClientBrandingAttributesTypeDef(TypedDict):
    LogoUrl: NotRequired[str],
    SupportEmail: NotRequired[str],
    SupportLink: NotRequired[str],
    ForgotPasswordLink: NotRequired[str],
    LoginMessage: NotRequired[Dict[str, str]],
```

## DefaultWorkspaceCreationPropertiesTypeDef

```python
# DefaultWorkspaceCreationPropertiesTypeDef definition

class DefaultWorkspaceCreationPropertiesTypeDef(TypedDict):
    EnableWorkDocs: NotRequired[bool],
    EnableInternetAccess: NotRequired[bool],
    DefaultOu: NotRequired[str],
    CustomSecurityGroupId: NotRequired[str],
    UserEnabledAsLocalAdministrator: NotRequired[bool],
    EnableMaintenanceMode: NotRequired[bool],
    InstanceIamRoleArn: NotRequired[str],
```

## DeleteAccountLinkInvitationRequestRequestTypeDef

```python
# DeleteAccountLinkInvitationRequestRequestTypeDef definition

class DeleteAccountLinkInvitationRequestRequestTypeDef(TypedDict):
    LinkId: str,
    ClientToken: NotRequired[str],
```

## DeleteClientBrandingRequestRequestTypeDef

```python
# DeleteClientBrandingRequestRequestTypeDef definition

class DeleteClientBrandingRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    Platforms: Sequence[ClientDeviceTypeType],  # (1)
```

1. See [:material-code-brackets: ClientDeviceTypeType](./literals.md#clientdevicetypetype) 
## DeleteConnectClientAddInRequestRequestTypeDef

```python
# DeleteConnectClientAddInRequestRequestTypeDef definition

class DeleteConnectClientAddInRequestRequestTypeDef(TypedDict):
    AddInId: str,
    ResourceId: str,
```

## DeleteConnectionAliasRequestRequestTypeDef

```python
# DeleteConnectionAliasRequestRequestTypeDef definition

class DeleteConnectionAliasRequestRequestTypeDef(TypedDict):
    AliasId: str,
```

## DeleteIpGroupRequestRequestTypeDef

```python
# DeleteIpGroupRequestRequestTypeDef definition

class DeleteIpGroupRequestRequestTypeDef(TypedDict):
    GroupId: str,
```

## DeleteTagsRequestRequestTypeDef

```python
# DeleteTagsRequestRequestTypeDef definition

class DeleteTagsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    TagKeys: Sequence[str],
```

## DeleteWorkspaceBundleRequestRequestTypeDef

```python
# DeleteWorkspaceBundleRequestRequestTypeDef definition

class DeleteWorkspaceBundleRequestRequestTypeDef(TypedDict):
    BundleId: NotRequired[str],
```

## DeleteWorkspaceImageRequestRequestTypeDef

```python
# DeleteWorkspaceImageRequestRequestTypeDef definition

class DeleteWorkspaceImageRequestRequestTypeDef(TypedDict):
    ImageId: str,
```

## DeployWorkspaceApplicationsRequestRequestTypeDef

```python
# DeployWorkspaceApplicationsRequestRequestTypeDef definition

class DeployWorkspaceApplicationsRequestRequestTypeDef(TypedDict):
    WorkspaceId: str,
    Force: NotRequired[bool],
```

## DeregisterWorkspaceDirectoryRequestRequestTypeDef

```python
# DeregisterWorkspaceDirectoryRequestRequestTypeDef definition

class DeregisterWorkspaceDirectoryRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAccountModificationsRequestRequestTypeDef

```python
# DescribeAccountModificationsRequestRequestTypeDef definition

class DescribeAccountModificationsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## DescribeApplicationAssociationsRequestRequestTypeDef

```python
# DescribeApplicationAssociationsRequestRequestTypeDef definition

class DescribeApplicationAssociationsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    AssociatedResourceTypes: Sequence[ApplicationAssociatedResourceTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ApplicationAssociatedResourceTypeType](./literals.md#applicationassociatedresourcetypetype) 
## DescribeApplicationsRequestRequestTypeDef

```python
# DescribeApplicationsRequestRequestTypeDef definition

class DescribeApplicationsRequestRequestTypeDef(TypedDict):
    ApplicationIds: NotRequired[Sequence[str]],
    ComputeTypeNames: NotRequired[Sequence[ComputeType]],  # (1)
    LicenseType: NotRequired[WorkSpaceApplicationLicenseTypeType],  # (2)
    OperatingSystemNames: NotRequired[Sequence[OperatingSystemNameType]],  # (3)
    Owner: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ComputeType](./literals.md#computetype) 
2. See [:material-code-brackets: WorkSpaceApplicationLicenseTypeType](./literals.md#workspaceapplicationlicensetypetype) 
3. See [:material-code-brackets: OperatingSystemNameType](./literals.md#operatingsystemnametype) 
## WorkSpaceApplicationTypeDef

```python
# WorkSpaceApplicationTypeDef definition

class WorkSpaceApplicationTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    Created: NotRequired[datetime],
    Description: NotRequired[str],
    LicenseType: NotRequired[WorkSpaceApplicationLicenseTypeType],  # (1)
    Name: NotRequired[str],
    Owner: NotRequired[str],
    State: NotRequired[WorkSpaceApplicationStateType],  # (2)
    SupportedComputeTypeNames: NotRequired[List[ComputeType]],  # (3)
    SupportedOperatingSystemNames: NotRequired[List[OperatingSystemNameType]],  # (4)
```

1. See [:material-code-brackets: WorkSpaceApplicationLicenseTypeType](./literals.md#workspaceapplicationlicensetypetype) 
2. See [:material-code-brackets: WorkSpaceApplicationStateType](./literals.md#workspaceapplicationstatetype) 
3. See [:material-code-brackets: ComputeType](./literals.md#computetype) 
4. See [:material-code-brackets: OperatingSystemNameType](./literals.md#operatingsystemnametype) 
## DescribeBundleAssociationsRequestRequestTypeDef

```python
# DescribeBundleAssociationsRequestRequestTypeDef definition

class DescribeBundleAssociationsRequestRequestTypeDef(TypedDict):
    BundleId: str,
    AssociatedResourceTypes: Sequence[BundleAssociatedResourceTypeType],  # (1)
```

1. See [:material-code-brackets: BundleAssociatedResourceTypeType](./literals.md#bundleassociatedresourcetypetype) 
## DescribeClientBrandingRequestRequestTypeDef

```python
# DescribeClientBrandingRequestRequestTypeDef definition

class DescribeClientBrandingRequestRequestTypeDef(TypedDict):
    ResourceId: str,
```

## IosClientBrandingAttributesTypeDef

```python
# IosClientBrandingAttributesTypeDef definition

class IosClientBrandingAttributesTypeDef(TypedDict):
    LogoUrl: NotRequired[str],
    Logo2xUrl: NotRequired[str],
    Logo3xUrl: NotRequired[str],
    SupportEmail: NotRequired[str],
    SupportLink: NotRequired[str],
    ForgotPasswordLink: NotRequired[str],
    LoginMessage: NotRequired[Dict[str, str]],
```

## DescribeClientPropertiesRequestRequestTypeDef

```python
# DescribeClientPropertiesRequestRequestTypeDef definition

class DescribeClientPropertiesRequestRequestTypeDef(TypedDict):
    ResourceIds: Sequence[str],
```

## DescribeConnectClientAddInsRequestRequestTypeDef

```python
# DescribeConnectClientAddInsRequestRequestTypeDef definition

class DescribeConnectClientAddInsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeConnectionAliasPermissionsRequestRequestTypeDef

```python
# DescribeConnectionAliasPermissionsRequestRequestTypeDef definition

class DescribeConnectionAliasPermissionsRequestRequestTypeDef(TypedDict):
    AliasId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeConnectionAliasesRequestRequestTypeDef

```python
# DescribeConnectionAliasesRequestRequestTypeDef definition

class DescribeConnectionAliasesRequestRequestTypeDef(TypedDict):
    AliasIds: NotRequired[Sequence[str]],
    ResourceId: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeImageAssociationsRequestRequestTypeDef

```python
# DescribeImageAssociationsRequestRequestTypeDef definition

class DescribeImageAssociationsRequestRequestTypeDef(TypedDict):
    ImageId: str,
    AssociatedResourceTypes: Sequence[ImageAssociatedResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ImageAssociatedResourceTypeType](./literals.md#imageassociatedresourcetypetype) 
## DescribeIpGroupsRequestRequestTypeDef

```python
# DescribeIpGroupsRequestRequestTypeDef definition

class DescribeIpGroupsRequestRequestTypeDef(TypedDict):
    GroupIds: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeTagsRequestRequestTypeDef

```python
# DescribeTagsRequestRequestTypeDef definition

class DescribeTagsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
```

## DescribeWorkspaceAssociationsRequestRequestTypeDef

```python
# DescribeWorkspaceAssociationsRequestRequestTypeDef definition

class DescribeWorkspaceAssociationsRequestRequestTypeDef(TypedDict):
    WorkspaceId: str,
    AssociatedResourceTypes: Sequence[WorkSpaceAssociatedResourceTypeType],  # (1)
```

1. See [:material-code-brackets: WorkSpaceAssociatedResourceTypeType](./literals.md#workspaceassociatedresourcetypetype) 
## DescribeWorkspaceBundlesRequestRequestTypeDef

```python
# DescribeWorkspaceBundlesRequestRequestTypeDef definition

class DescribeWorkspaceBundlesRequestRequestTypeDef(TypedDict):
    BundleIds: NotRequired[Sequence[str]],
    Owner: NotRequired[str],
    NextToken: NotRequired[str],
```

## DescribeWorkspaceDirectoriesFilterTypeDef

```python
# DescribeWorkspaceDirectoriesFilterTypeDef definition

class DescribeWorkspaceDirectoriesFilterTypeDef(TypedDict):
    Name: DescribeWorkspaceDirectoriesFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: DescribeWorkspaceDirectoriesFilterNameType](./literals.md#describeworkspacedirectoriesfilternametype) 
## DescribeWorkspaceImagePermissionsRequestRequestTypeDef

```python
# DescribeWorkspaceImagePermissionsRequestRequestTypeDef definition

class DescribeWorkspaceImagePermissionsRequestRequestTypeDef(TypedDict):
    ImageId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ImagePermissionTypeDef

```python
# ImagePermissionTypeDef definition

class ImagePermissionTypeDef(TypedDict):
    SharedAccountId: NotRequired[str],
```

## DescribeWorkspaceImagesRequestRequestTypeDef

```python
# DescribeWorkspaceImagesRequestRequestTypeDef definition

class DescribeWorkspaceImagesRequestRequestTypeDef(TypedDict):
    ImageIds: NotRequired[Sequence[str]],
    ImageType: NotRequired[ImageTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ImageTypeType](./literals.md#imagetypetype) 
## DescribeWorkspaceSnapshotsRequestRequestTypeDef

```python
# DescribeWorkspaceSnapshotsRequestRequestTypeDef definition

class DescribeWorkspaceSnapshotsRequestRequestTypeDef(TypedDict):
    WorkspaceId: str,
```

## SnapshotTypeDef

```python
# SnapshotTypeDef definition

class SnapshotTypeDef(TypedDict):
    SnapshotTime: NotRequired[datetime],
```

## DescribeWorkspacesConnectionStatusRequestRequestTypeDef

```python
# DescribeWorkspacesConnectionStatusRequestRequestTypeDef definition

class DescribeWorkspacesConnectionStatusRequestRequestTypeDef(TypedDict):
    WorkspaceIds: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
```

## WorkspaceConnectionStatusTypeDef

```python
# WorkspaceConnectionStatusTypeDef definition

class WorkspaceConnectionStatusTypeDef(TypedDict):
    WorkspaceId: NotRequired[str],
    ConnectionState: NotRequired[ConnectionStateType],  # (1)
    ConnectionStateCheckTimestamp: NotRequired[datetime],
    LastKnownUserConnectionTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
## DescribeWorkspacesPoolSessionsRequestRequestTypeDef

```python
# DescribeWorkspacesPoolSessionsRequestRequestTypeDef definition

class DescribeWorkspacesPoolSessionsRequestRequestTypeDef(TypedDict):
    PoolId: str,
    UserId: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeWorkspacesPoolsFilterTypeDef

```python
# DescribeWorkspacesPoolsFilterTypeDef definition

class DescribeWorkspacesPoolsFilterTypeDef(TypedDict):
    Name: DescribeWorkspacesPoolsFilterNameType,  # (1)
    Values: Sequence[str],
    Operator: DescribeWorkspacesPoolsFilterOperatorType,  # (2)
```

1. See [:material-code-brackets: DescribeWorkspacesPoolsFilterNameType](./literals.md#describeworkspacespoolsfilternametype) 
2. See [:material-code-brackets: DescribeWorkspacesPoolsFilterOperatorType](./literals.md#describeworkspacespoolsfilteroperatortype) 
## DescribeWorkspacesRequestRequestTypeDef

```python
# DescribeWorkspacesRequestRequestTypeDef definition

class DescribeWorkspacesRequestRequestTypeDef(TypedDict):
    WorkspaceIds: NotRequired[Sequence[str]],
    DirectoryId: NotRequired[str],
    UserName: NotRequired[str],
    BundleId: NotRequired[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
    WorkspaceName: NotRequired[str],
```

## DisassociateConnectionAliasRequestRequestTypeDef

```python
# DisassociateConnectionAliasRequestRequestTypeDef definition

class DisassociateConnectionAliasRequestRequestTypeDef(TypedDict):
    AliasId: str,
```

## DisassociateIpGroupsRequestRequestTypeDef

```python
# DisassociateIpGroupsRequestRequestTypeDef definition

class DisassociateIpGroupsRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    GroupIds: Sequence[str],
```

## DisassociateWorkspaceApplicationRequestRequestTypeDef

```python
# DisassociateWorkspaceApplicationRequestRequestTypeDef definition

class DisassociateWorkspaceApplicationRequestRequestTypeDef(TypedDict):
    WorkspaceId: str,
    ApplicationId: str,
```

## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    ErrorCode: NotRequired[WorkspaceImageErrorDetailCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: WorkspaceImageErrorDetailCodeType](./literals.md#workspaceimageerrordetailcodetype) 
## FailedWorkspaceChangeRequestTypeDef

```python
# FailedWorkspaceChangeRequestTypeDef definition

class FailedWorkspaceChangeRequestTypeDef(TypedDict):
    WorkspaceId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## GetAccountLinkRequestRequestTypeDef

```python
# GetAccountLinkRequestRequestTypeDef definition

class GetAccountLinkRequestRequestTypeDef(TypedDict):
    LinkId: NotRequired[str],
    LinkedAccountId: NotRequired[str],
```

## IDCConfigTypeDef

```python
# IDCConfigTypeDef definition

class IDCConfigTypeDef(TypedDict):
    InstanceArn: NotRequired[str],
    ApplicationArn: NotRequired[str],
```

## ListAccountLinksRequestRequestTypeDef

```python
# ListAccountLinksRequestRequestTypeDef definition

class ListAccountLinksRequestRequestTypeDef(TypedDict):
    LinkStatusFilter: NotRequired[Sequence[AccountLinkStatusEnumType]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: AccountLinkStatusEnumType](./literals.md#accountlinkstatusenumtype) 
## ListAvailableManagementCidrRangesRequestRequestTypeDef

```python
# ListAvailableManagementCidrRangesRequestRequestTypeDef definition

class ListAvailableManagementCidrRangesRequestRequestTypeDef(TypedDict):
    ManagementCidrRangeConstraint: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MicrosoftEntraConfigTypeDef

```python
# MicrosoftEntraConfigTypeDef definition

class MicrosoftEntraConfigTypeDef(TypedDict):
    TenantId: NotRequired[str],
    ApplicationConfigSecretArn: NotRequired[str],
```

## MigrateWorkspaceRequestRequestTypeDef

```python
# MigrateWorkspaceRequestRequestTypeDef definition

class MigrateWorkspaceRequestRequestTypeDef(TypedDict):
    SourceWorkspaceId: str,
    BundleId: str,
```

## ModificationStateTypeDef

```python
# ModificationStateTypeDef definition

class ModificationStateTypeDef(TypedDict):
    Resource: NotRequired[ModificationResourceEnumType],  # (1)
    State: NotRequired[ModificationStateEnumType],  # (2)
```

1. See [:material-code-brackets: ModificationResourceEnumType](./literals.md#modificationresourceenumtype) 
2. See [:material-code-brackets: ModificationStateEnumType](./literals.md#modificationstateenumtype) 
## ModifyAccountRequestRequestTypeDef

```python
# ModifyAccountRequestRequestTypeDef definition

class ModifyAccountRequestRequestTypeDef(TypedDict):
    DedicatedTenancySupport: NotRequired[DedicatedTenancySupportEnumType],  # (1)
    DedicatedTenancyManagementCidrRange: NotRequired[str],
```

1. See [:material-code-brackets: DedicatedTenancySupportEnumType](./literals.md#dedicatedtenancysupportenumtype) 
## SamlPropertiesTypeDef

```python
# SamlPropertiesTypeDef definition

class SamlPropertiesTypeDef(TypedDict):
    Status: NotRequired[SamlStatusEnumType],  # (1)
    UserAccessUrl: NotRequired[str],
    RelayStateParameterName: NotRequired[str],
```

1. See [:material-code-brackets: SamlStatusEnumType](./literals.md#samlstatusenumtype) 
## SelfservicePermissionsTypeDef

```python
# SelfservicePermissionsTypeDef definition

class SelfservicePermissionsTypeDef(TypedDict):
    RestartWorkspace: NotRequired[ReconnectEnumType],  # (1)
    IncreaseVolumeSize: NotRequired[ReconnectEnumType],  # (1)
    ChangeComputeType: NotRequired[ReconnectEnumType],  # (1)
    SwitchRunningMode: NotRequired[ReconnectEnumType],  # (1)
    RebuildWorkspace: NotRequired[ReconnectEnumType],  # (1)
```

1. See [:material-code-brackets: ReconnectEnumType](./literals.md#reconnectenumtype) 
2. See [:material-code-brackets: ReconnectEnumType](./literals.md#reconnectenumtype) 
3. See [:material-code-brackets: ReconnectEnumType](./literals.md#reconnectenumtype) 
4. See [:material-code-brackets: ReconnectEnumType](./literals.md#reconnectenumtype) 
5. See [:material-code-brackets: ReconnectEnumType](./literals.md#reconnectenumtype) 
## WorkspaceAccessPropertiesTypeDef

```python
# WorkspaceAccessPropertiesTypeDef definition

class WorkspaceAccessPropertiesTypeDef(TypedDict):
    DeviceTypeWindows: NotRequired[AccessPropertyValueType],  # (1)
    DeviceTypeOsx: NotRequired[AccessPropertyValueType],  # (1)
    DeviceTypeWeb: NotRequired[AccessPropertyValueType],  # (1)
    DeviceTypeIos: NotRequired[AccessPropertyValueType],  # (1)
    DeviceTypeAndroid: NotRequired[AccessPropertyValueType],  # (1)
    DeviceTypeChromeOs: NotRequired[AccessPropertyValueType],  # (1)
    DeviceTypeZeroClient: NotRequired[AccessPropertyValueType],  # (1)
    DeviceTypeLinux: NotRequired[AccessPropertyValueType],  # (1)
```

1. See [:material-code-brackets: AccessPropertyValueType](./literals.md#accesspropertyvaluetype) 
2. See [:material-code-brackets: AccessPropertyValueType](./literals.md#accesspropertyvaluetype) 
3. See [:material-code-brackets: AccessPropertyValueType](./literals.md#accesspropertyvaluetype) 
4. See [:material-code-brackets: AccessPropertyValueType](./literals.md#accesspropertyvaluetype) 
5. See [:material-code-brackets: AccessPropertyValueType](./literals.md#accesspropertyvaluetype) 
6. See [:material-code-brackets: AccessPropertyValueType](./literals.md#accesspropertyvaluetype) 
7. See [:material-code-brackets: AccessPropertyValueType](./literals.md#accesspropertyvaluetype) 
8. See [:material-code-brackets: AccessPropertyValueType](./literals.md#accesspropertyvaluetype) 
## WorkspaceCreationPropertiesTypeDef

```python
# WorkspaceCreationPropertiesTypeDef definition

class WorkspaceCreationPropertiesTypeDef(TypedDict):
    EnableWorkDocs: NotRequired[bool],
    EnableInternetAccess: NotRequired[bool],
    DefaultOu: NotRequired[str],
    CustomSecurityGroupId: NotRequired[str],
    UserEnabledAsLocalAdministrator: NotRequired[bool],
    EnableMaintenanceMode: NotRequired[bool],
    InstanceIamRoleArn: NotRequired[str],
```

## WorkspacePropertiesTypeDef

```python
# WorkspacePropertiesTypeDef definition

class WorkspacePropertiesTypeDef(TypedDict):
    RunningMode: NotRequired[RunningModeType],  # (1)
    RunningModeAutoStopTimeoutInMinutes: NotRequired[int],
    RootVolumeSizeGib: NotRequired[int],
    UserVolumeSizeGib: NotRequired[int],
    ComputeTypeName: NotRequired[ComputeType],  # (2)
    Protocols: NotRequired[Sequence[ProtocolType]],  # (3)
    OperatingSystemName: NotRequired[OperatingSystemNameType],  # (4)
```

1. See [:material-code-brackets: RunningModeType](./literals.md#runningmodetype) 
2. See [:material-code-brackets: ComputeType](./literals.md#computetype) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
4. See [:material-code-brackets: OperatingSystemNameType](./literals.md#operatingsystemnametype) 
## ModifyWorkspaceStateRequestRequestTypeDef

```python
# ModifyWorkspaceStateRequestRequestTypeDef definition

class ModifyWorkspaceStateRequestRequestTypeDef(TypedDict):
    WorkspaceId: str,
    WorkspaceState: TargetWorkspaceStateType,  # (1)
```

1. See [:material-code-brackets: TargetWorkspaceStateType](./literals.md#targetworkspacestatetype) 
## NetworkAccessConfigurationTypeDef

```python
# NetworkAccessConfigurationTypeDef definition

class NetworkAccessConfigurationTypeDef(TypedDict):
    EniPrivateIpAddress: NotRequired[str],
    EniId: NotRequired[str],
```

## RebootRequestTypeDef

```python
# RebootRequestTypeDef definition

class RebootRequestTypeDef(TypedDict):
    WorkspaceId: str,
```

## RebuildRequestTypeDef

```python
# RebuildRequestTypeDef definition

class RebuildRequestTypeDef(TypedDict):
    WorkspaceId: str,
```

## RejectAccountLinkInvitationRequestRequestTypeDef

```python
# RejectAccountLinkInvitationRequestRequestTypeDef definition

class RejectAccountLinkInvitationRequestRequestTypeDef(TypedDict):
    LinkId: str,
    ClientToken: NotRequired[str],
```

## RelatedWorkspacePropertiesTypeDef

```python
# RelatedWorkspacePropertiesTypeDef definition

class RelatedWorkspacePropertiesTypeDef(TypedDict):
    WorkspaceId: NotRequired[str],
    Region: NotRequired[str],
    State: NotRequired[WorkspaceStateType],  # (1)
    Type: NotRequired[StandbyWorkspaceRelationshipTypeType],  # (2)
```

1. See [:material-code-brackets: WorkspaceStateType](./literals.md#workspacestatetype) 
2. See [:material-code-brackets: StandbyWorkspaceRelationshipTypeType](./literals.md#standbyworkspacerelationshiptypetype) 
## RestoreWorkspaceRequestRequestTypeDef

```python
# RestoreWorkspaceRequestRequestTypeDef definition

class RestoreWorkspaceRequestRequestTypeDef(TypedDict):
    WorkspaceId: str,
```

## RevokeIpRulesRequestRequestTypeDef

```python
# RevokeIpRulesRequestRequestTypeDef definition

class RevokeIpRulesRequestRequestTypeDef(TypedDict):
    GroupId: str,
    UserRules: Sequence[str],
```

## StandbyWorkspacesPropertiesTypeDef

```python
# StandbyWorkspacesPropertiesTypeDef definition

class StandbyWorkspacesPropertiesTypeDef(TypedDict):
    StandbyWorkspaceId: NotRequired[str],
    DataReplication: NotRequired[DataReplicationType],  # (1)
    RecoverySnapshotTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DataReplicationType](./literals.md#datareplicationtype) 
## StartRequestTypeDef

```python
# StartRequestTypeDef definition

class StartRequestTypeDef(TypedDict):
    WorkspaceId: NotRequired[str],
```

## StartWorkspacesPoolRequestRequestTypeDef

```python
# StartWorkspacesPoolRequestRequestTypeDef definition

class StartWorkspacesPoolRequestRequestTypeDef(TypedDict):
    PoolId: str,
```

## StopRequestTypeDef

```python
# StopRequestTypeDef definition

class StopRequestTypeDef(TypedDict):
    WorkspaceId: NotRequired[str],
```

## StopWorkspacesPoolRequestRequestTypeDef

```python
# StopWorkspacesPoolRequestRequestTypeDef definition

class StopWorkspacesPoolRequestRequestTypeDef(TypedDict):
    PoolId: str,
```

## StorageConnectorTypeDef

```python
# StorageConnectorTypeDef definition

class StorageConnectorTypeDef(TypedDict):
    ConnectorType: StorageConnectorTypeEnumType,  # (1)
    Status: StorageConnectorStatusEnumType,  # (2)
```

1. See [:material-code-brackets: StorageConnectorTypeEnumType](./literals.md#storageconnectortypeenumtype) 
2. See [:material-code-brackets: StorageConnectorStatusEnumType](./literals.md#storageconnectorstatusenumtype) 
## UserSettingTypeDef

```python
# UserSettingTypeDef definition

class UserSettingTypeDef(TypedDict):
    Action: UserSettingActionEnumType,  # (1)
    Permission: UserSettingPermissionEnumType,  # (2)
    MaximumLength: NotRequired[int],
```

1. See [:material-code-brackets: UserSettingActionEnumType](./literals.md#usersettingactionenumtype) 
2. See [:material-code-brackets: UserSettingPermissionEnumType](./literals.md#usersettingpermissionenumtype) 
## TerminateRequestTypeDef

```python
# TerminateRequestTypeDef definition

class TerminateRequestTypeDef(TypedDict):
    WorkspaceId: str,
```

## TerminateWorkspacesPoolRequestRequestTypeDef

```python
# TerminateWorkspacesPoolRequestRequestTypeDef definition

class TerminateWorkspacesPoolRequestRequestTypeDef(TypedDict):
    PoolId: str,
```

## TerminateWorkspacesPoolSessionRequestRequestTypeDef

```python
# TerminateWorkspacesPoolSessionRequestRequestTypeDef definition

class TerminateWorkspacesPoolSessionRequestRequestTypeDef(TypedDict):
    SessionId: str,
```

## UpdateConnectClientAddInRequestRequestTypeDef

```python
# UpdateConnectClientAddInRequestRequestTypeDef definition

class UpdateConnectClientAddInRequestRequestTypeDef(TypedDict):
    AddInId: str,
    ResourceId: str,
    Name: NotRequired[str],
    URL: NotRequired[str],
```

## UpdateResultTypeDef

```python
# UpdateResultTypeDef definition

class UpdateResultTypeDef(TypedDict):
    UpdateAvailable: NotRequired[bool],
    Description: NotRequired[str],
```

## UpdateWorkspaceBundleRequestRequestTypeDef

```python
# UpdateWorkspaceBundleRequestRequestTypeDef definition

class UpdateWorkspaceBundleRequestRequestTypeDef(TypedDict):
    BundleId: NotRequired[str],
    ImageId: NotRequired[str],
```

## UpdateWorkspaceImagePermissionRequestRequestTypeDef

```python
# UpdateWorkspaceImagePermissionRequestRequestTypeDef definition

class UpdateWorkspaceImagePermissionRequestRequestTypeDef(TypedDict):
    ImageId: str,
    AllowCopyImage: bool,
    SharedAccountId: str,
```

## WorkspacePropertiesOutputTypeDef

```python
# WorkspacePropertiesOutputTypeDef definition

class WorkspacePropertiesOutputTypeDef(TypedDict):
    RunningMode: NotRequired[RunningModeType],  # (1)
    RunningModeAutoStopTimeoutInMinutes: NotRequired[int],
    RootVolumeSizeGib: NotRequired[int],
    UserVolumeSizeGib: NotRequired[int],
    ComputeTypeName: NotRequired[ComputeType],  # (2)
    Protocols: NotRequired[List[ProtocolType]],  # (3)
    OperatingSystemName: NotRequired[OperatingSystemNameType],  # (4)
```

1. See [:material-code-brackets: RunningModeType](./literals.md#runningmodetype) 
2. See [:material-code-brackets: ComputeType](./literals.md#computetype) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
4. See [:material-code-brackets: OperatingSystemNameType](./literals.md#operatingsystemnametype) 
## WorkspacesPoolErrorTypeDef

```python
# WorkspacesPoolErrorTypeDef definition

class WorkspacesPoolErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[WorkspacesPoolErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: WorkspacesPoolErrorCodeType](./literals.md#workspacespoolerrorcodetype) 
## AcceptAccountLinkInvitationResultTypeDef

```python
# AcceptAccountLinkInvitationResultTypeDef definition

class AcceptAccountLinkInvitationResultTypeDef(TypedDict):
    AccountLink: AccountLinkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountLinkTypeDef](./type_defs.md#accountlinktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateConnectionAliasResultTypeDef

```python
# AssociateConnectionAliasResultTypeDef definition

class AssociateConnectionAliasResultTypeDef(TypedDict):
    ConnectionIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyWorkspaceImageResultTypeDef

```python
# CopyWorkspaceImageResultTypeDef definition

class CopyWorkspaceImageResultTypeDef(TypedDict):
    ImageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAccountLinkInvitationResultTypeDef

```python
# CreateAccountLinkInvitationResultTypeDef definition

class CreateAccountLinkInvitationResultTypeDef(TypedDict):
    AccountLink: AccountLinkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountLinkTypeDef](./type_defs.md#accountlinktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConnectClientAddInResultTypeDef

```python
# CreateConnectClientAddInResultTypeDef definition

class CreateConnectClientAddInResultTypeDef(TypedDict):
    AddInId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConnectionAliasResultTypeDef

```python
# CreateConnectionAliasResultTypeDef definition

class CreateConnectionAliasResultTypeDef(TypedDict):
    AliasId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIpGroupResultTypeDef

```python
# CreateIpGroupResultTypeDef definition

class CreateIpGroupResultTypeDef(TypedDict):
    GroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUpdatedWorkspaceImageResultTypeDef

```python
# CreateUpdatedWorkspaceImageResultTypeDef definition

class CreateUpdatedWorkspaceImageResultTypeDef(TypedDict):
    ImageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAccountLinkInvitationResultTypeDef

```python
# DeleteAccountLinkInvitationResultTypeDef definition

class DeleteAccountLinkInvitationResultTypeDef(TypedDict):
    AccountLink: AccountLinkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountLinkTypeDef](./type_defs.md#accountlinktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountResultTypeDef

```python
# DescribeAccountResultTypeDef definition

class DescribeAccountResultTypeDef(TypedDict):
    DedicatedTenancySupport: DedicatedTenancySupportResultEnumType,  # (1)
    DedicatedTenancyManagementCidrRange: str,
    DedicatedTenancyAccountType: DedicatedTenancyAccountTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DedicatedTenancySupportResultEnumType](./literals.md#dedicatedtenancysupportresultenumtype) 
2. See [:material-code-brackets: DedicatedTenancyAccountTypeType](./literals.md#dedicatedtenancyaccounttypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountLinkResultTypeDef

```python
# GetAccountLinkResultTypeDef definition

class GetAccountLinkResultTypeDef(TypedDict):
    AccountLink: AccountLinkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountLinkTypeDef](./type_defs.md#accountlinktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportWorkspaceImageResultTypeDef

```python
# ImportWorkspaceImageResultTypeDef definition

class ImportWorkspaceImageResultTypeDef(TypedDict):
    ImageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccountLinksResultTypeDef

```python
# ListAccountLinksResultTypeDef definition

class ListAccountLinksResultTypeDef(TypedDict):
    AccountLinks: List[AccountLinkTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountLinkTypeDef](./type_defs.md#accountlinktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAvailableManagementCidrRangesResultTypeDef

```python
# ListAvailableManagementCidrRangesResultTypeDef definition

class ListAvailableManagementCidrRangesResultTypeDef(TypedDict):
    ManagementCidrRanges: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MigrateWorkspaceResultTypeDef

```python
# MigrateWorkspaceResultTypeDef definition

class MigrateWorkspaceResultTypeDef(TypedDict):
    SourceWorkspaceId: str,
    TargetWorkspaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterWorkspaceDirectoryResultTypeDef

```python
# RegisterWorkspaceDirectoryResultTypeDef definition

class RegisterWorkspaceDirectoryResultTypeDef(TypedDict):
    DirectoryId: str,
    State: WorkspaceDirectoryStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: WorkspaceDirectoryStateType](./literals.md#workspacedirectorystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectAccountLinkInvitationResultTypeDef

```python
# RejectAccountLinkInvitationResultTypeDef definition

class RejectAccountLinkInvitationResultTypeDef(TypedDict):
    AccountLink: AccountLinkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountLinkTypeDef](./type_defs.md#accountlinktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountModificationsResultTypeDef

```python
# DescribeAccountModificationsResultTypeDef definition

class DescribeAccountModificationsResultTypeDef(TypedDict):
    AccountModifications: List[AccountModificationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountModificationTypeDef](./type_defs.md#accountmodificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplicationResourceAssociationTypeDef

```python
# ApplicationResourceAssociationTypeDef definition

class ApplicationResourceAssociationTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    AssociatedResourceId: NotRequired[str],
    AssociatedResourceType: NotRequired[ApplicationAssociatedResourceTypeType],  # (1)
    Created: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    State: NotRequired[AssociationStateType],  # (2)
    StateReason: NotRequired[AssociationStateReasonTypeDef],  # (3)
```

1. See [:material-code-brackets: ApplicationAssociatedResourceTypeType](./literals.md#applicationassociatedresourcetypetype) 
2. See [:material-code-brackets: AssociationStateType](./literals.md#associationstatetype) 
3. See [:material-code-braces: AssociationStateReasonTypeDef](./type_defs.md#associationstatereasontypedef) 
## BundleResourceAssociationTypeDef

```python
# BundleResourceAssociationTypeDef definition

class BundleResourceAssociationTypeDef(TypedDict):
    AssociatedResourceId: NotRequired[str],
    AssociatedResourceType: NotRequired[BundleAssociatedResourceTypeType],  # (1)
    BundleId: NotRequired[str],
    Created: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    State: NotRequired[AssociationStateType],  # (2)
    StateReason: NotRequired[AssociationStateReasonTypeDef],  # (3)
```

1. See [:material-code-brackets: BundleAssociatedResourceTypeType](./literals.md#bundleassociatedresourcetypetype) 
2. See [:material-code-brackets: AssociationStateType](./literals.md#associationstatetype) 
3. See [:material-code-braces: AssociationStateReasonTypeDef](./type_defs.md#associationstatereasontypedef) 
## ImageResourceAssociationTypeDef

```python
# ImageResourceAssociationTypeDef definition

class ImageResourceAssociationTypeDef(TypedDict):
    AssociatedResourceId: NotRequired[str],
    AssociatedResourceType: NotRequired[ImageAssociatedResourceTypeType],  # (1)
    Created: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    ImageId: NotRequired[str],
    State: NotRequired[AssociationStateType],  # (2)
    StateReason: NotRequired[AssociationStateReasonTypeDef],  # (3)
```

1. See [:material-code-brackets: ImageAssociatedResourceTypeType](./literals.md#imageassociatedresourcetypetype) 
2. See [:material-code-brackets: AssociationStateType](./literals.md#associationstatetype) 
3. See [:material-code-braces: AssociationStateReasonTypeDef](./type_defs.md#associationstatereasontypedef) 
## WorkspaceResourceAssociationTypeDef

```python
# WorkspaceResourceAssociationTypeDef definition

class WorkspaceResourceAssociationTypeDef(TypedDict):
    AssociatedResourceId: NotRequired[str],
    AssociatedResourceType: NotRequired[WorkSpaceAssociatedResourceTypeType],  # (1)
    Created: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    State: NotRequired[AssociationStateType],  # (2)
    StateReason: NotRequired[AssociationStateReasonTypeDef],  # (3)
    WorkspaceId: NotRequired[str],
```

1. See [:material-code-brackets: WorkSpaceAssociatedResourceTypeType](./literals.md#workspaceassociatedresourcetypetype) 
2. See [:material-code-brackets: AssociationStateType](./literals.md#associationstatetype) 
3. See [:material-code-braces: AssociationStateReasonTypeDef](./type_defs.md#associationstatereasontypedef) 
## AuthorizeIpRulesRequestRequestTypeDef

```python
# AuthorizeIpRulesRequestRequestTypeDef definition

class AuthorizeIpRulesRequestRequestTypeDef(TypedDict):
    GroupId: str,
    UserRules: Sequence[IpRuleItemTypeDef],  # (1)
```

1. See [:material-code-braces: IpRuleItemTypeDef](./type_defs.md#ipruleitemtypedef) 
## UpdateRulesOfIpGroupRequestRequestTypeDef

```python
# UpdateRulesOfIpGroupRequestRequestTypeDef definition

class UpdateRulesOfIpGroupRequestRequestTypeDef(TypedDict):
    GroupId: str,
    UserRules: Sequence[IpRuleItemTypeDef],  # (1)
```

1. See [:material-code-braces: IpRuleItemTypeDef](./type_defs.md#ipruleitemtypedef) 
## WorkspacesIpGroupTypeDef

```python
# WorkspacesIpGroupTypeDef definition

class WorkspacesIpGroupTypeDef(TypedDict):
    groupId: NotRequired[str],
    groupName: NotRequired[str],
    groupDesc: NotRequired[str],
    userRules: NotRequired[List[IpRuleItemTypeDef]],  # (1)
```

1. See [:material-code-braces: IpRuleItemTypeDef](./type_defs.md#ipruleitemtypedef) 
## DefaultImportClientBrandingAttributesTypeDef

```python
# DefaultImportClientBrandingAttributesTypeDef definition

class DefaultImportClientBrandingAttributesTypeDef(TypedDict):
    Logo: NotRequired[BlobTypeDef],
    SupportEmail: NotRequired[str],
    SupportLink: NotRequired[str],
    ForgotPasswordLink: NotRequired[str],
    LoginMessage: NotRequired[Mapping[str, str]],
```

## IosImportClientBrandingAttributesTypeDef

```python
# IosImportClientBrandingAttributesTypeDef definition

class IosImportClientBrandingAttributesTypeDef(TypedDict):
    Logo: NotRequired[BlobTypeDef],
    Logo2x: NotRequired[BlobTypeDef],
    Logo3x: NotRequired[BlobTypeDef],
    SupportEmail: NotRequired[str],
    SupportLink: NotRequired[str],
    ForgotPasswordLink: NotRequired[str],
    LoginMessage: NotRequired[Mapping[str, str]],
```

## ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef

```python
# ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef definition

class ModifyCertificateBasedAuthPropertiesRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    CertificateBasedAuthProperties: NotRequired[CertificateBasedAuthPropertiesTypeDef],  # (1)
    PropertiesToDelete: NotRequired[Sequence[DeletableCertificateBasedAuthPropertyType]],  # (2)
```

1. See [:material-code-braces: CertificateBasedAuthPropertiesTypeDef](./type_defs.md#certificatebasedauthpropertiestypedef) 
2. See [:material-code-brackets: DeletableCertificateBasedAuthPropertyType](./literals.md#deletablecertificatebasedauthpropertytype) 
## ClientPropertiesResultTypeDef

```python
# ClientPropertiesResultTypeDef definition

class ClientPropertiesResultTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    ClientProperties: NotRequired[ClientPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: ClientPropertiesTypeDef](./type_defs.md#clientpropertiestypedef) 
## ModifyClientPropertiesRequestRequestTypeDef

```python
# ModifyClientPropertiesRequestRequestTypeDef definition

class ModifyClientPropertiesRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    ClientProperties: ClientPropertiesTypeDef,  # (1)
```

1. See [:material-code-braces: ClientPropertiesTypeDef](./type_defs.md#clientpropertiestypedef) 
## DescribeConnectClientAddInsResultTypeDef

```python
# DescribeConnectClientAddInsResultTypeDef definition

class DescribeConnectClientAddInsResultTypeDef(TypedDict):
    AddIns: List[ConnectClientAddInTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectClientAddInTypeDef](./type_defs.md#connectclientaddintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionAliasTypeDef

```python
# ConnectionAliasTypeDef definition

class ConnectionAliasTypeDef(TypedDict):
    ConnectionString: NotRequired[str],
    AliasId: NotRequired[str],
    State: NotRequired[ConnectionAliasStateType],  # (1)
    OwnerAccountId: NotRequired[str],
    Associations: NotRequired[List[ConnectionAliasAssociationTypeDef]],  # (2)
```

1. See [:material-code-brackets: ConnectionAliasStateType](./literals.md#connectionaliasstatetype) 
2. See [:material-code-braces: ConnectionAliasAssociationTypeDef](./type_defs.md#connectionaliasassociationtypedef) 
## DescribeConnectionAliasPermissionsResultTypeDef

```python
# DescribeConnectionAliasPermissionsResultTypeDef definition

class DescribeConnectionAliasPermissionsResultTypeDef(TypedDict):
    AliasId: str,
    ConnectionAliasPermissions: List[ConnectionAliasPermissionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectionAliasPermissionTypeDef](./type_defs.md#connectionaliaspermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConnectionAliasPermissionRequestRequestTypeDef

```python
# UpdateConnectionAliasPermissionRequestRequestTypeDef definition

class UpdateConnectionAliasPermissionRequestRequestTypeDef(TypedDict):
    AliasId: str,
    ConnectionAliasPermission: ConnectionAliasPermissionTypeDef,  # (1)
```

1. See [:material-code-braces: ConnectionAliasPermissionTypeDef](./type_defs.md#connectionaliaspermissiontypedef) 
## CopyWorkspaceImageRequestRequestTypeDef

```python
# CopyWorkspaceImageRequestRequestTypeDef definition

class CopyWorkspaceImageRequestRequestTypeDef(TypedDict):
    Name: str,
    SourceImageId: str,
    SourceRegion: str,
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateConnectionAliasRequestRequestTypeDef

```python
# CreateConnectionAliasRequestRequestTypeDef definition

class CreateConnectionAliasRequestRequestTypeDef(TypedDict):
    ConnectionString: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIpGroupRequestRequestTypeDef

```python
# CreateIpGroupRequestRequestTypeDef definition

class CreateIpGroupRequestRequestTypeDef(TypedDict):
    GroupName: str,
    GroupDesc: NotRequired[str],
    UserRules: NotRequired[Sequence[IpRuleItemTypeDef]],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: IpRuleItemTypeDef](./type_defs.md#ipruleitemtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTagsRequestRequestTypeDef

```python
# CreateTagsRequestRequestTypeDef definition

class CreateTagsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateUpdatedWorkspaceImageRequestRequestTypeDef

```python
# CreateUpdatedWorkspaceImageRequestRequestTypeDef definition

class CreateUpdatedWorkspaceImageRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: str,
    SourceImageId: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateWorkspaceImageRequestRequestTypeDef

```python
# CreateWorkspaceImageRequestRequestTypeDef definition

class CreateWorkspaceImageRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: str,
    WorkspaceId: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeTagsResultTypeDef

```python
# DescribeTagsResultTypeDef definition

class DescribeTagsResultTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportWorkspaceImageRequestRequestTypeDef

```python
# ImportWorkspaceImageRequestRequestTypeDef definition

class ImportWorkspaceImageRequestRequestTypeDef(TypedDict):
    Ec2ImageId: str,
    IngestionProcess: WorkspaceImageIngestionProcessType,  # (1)
    ImageName: str,
    ImageDescription: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    Applications: NotRequired[Sequence[ApplicationType]],  # (3)
```

1. See [:material-code-brackets: WorkspaceImageIngestionProcessType](./literals.md#workspaceimageingestionprocesstype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: ApplicationType](./literals.md#applicationtype) 
## StandbyWorkspaceOutputTypeDef

```python
# StandbyWorkspaceOutputTypeDef definition

class StandbyWorkspaceOutputTypeDef(TypedDict):
    PrimaryWorkspaceId: str,
    DirectoryId: str,
    VolumeEncryptionKey: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    DataReplication: NotRequired[DataReplicationType],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: DataReplicationType](./literals.md#datareplicationtype) 
## StandbyWorkspaceTypeDef

```python
# StandbyWorkspaceTypeDef definition

class StandbyWorkspaceTypeDef(TypedDict):
    PrimaryWorkspaceId: str,
    DirectoryId: str,
    VolumeEncryptionKey: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    DataReplication: NotRequired[DataReplicationType],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: DataReplicationType](./literals.md#datareplicationtype) 
## CreateWorkspaceBundleRequestRequestTypeDef

```python
# CreateWorkspaceBundleRequestRequestTypeDef definition

class CreateWorkspaceBundleRequestRequestTypeDef(TypedDict):
    BundleName: str,
    BundleDescription: str,
    ImageId: str,
    ComputeType: ComputeTypeTypeDef,  # (1)
    UserStorage: UserStorageTypeDef,  # (2)
    RootStorage: NotRequired[RootStorageTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: ComputeTypeTypeDef](./type_defs.md#computetypetypedef) 
2. See [:material-code-braces: UserStorageTypeDef](./type_defs.md#userstoragetypedef) 
3. See [:material-code-braces: RootStorageTypeDef](./type_defs.md#rootstoragetypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## WorkspaceBundleTypeDef

```python
# WorkspaceBundleTypeDef definition

class WorkspaceBundleTypeDef(TypedDict):
    BundleId: NotRequired[str],
    Name: NotRequired[str],
    Owner: NotRequired[str],
    Description: NotRequired[str],
    ImageId: NotRequired[str],
    RootStorage: NotRequired[RootStorageTypeDef],  # (1)
    UserStorage: NotRequired[UserStorageTypeDef],  # (2)
    ComputeType: NotRequired[ComputeTypeTypeDef],  # (3)
    LastUpdatedTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
    State: NotRequired[WorkspaceBundleStateType],  # (4)
    BundleType: NotRequired[BundleTypeType],  # (5)
```

1. See [:material-code-braces: RootStorageTypeDef](./type_defs.md#rootstoragetypedef) 
2. See [:material-code-braces: UserStorageTypeDef](./type_defs.md#userstoragetypedef) 
3. See [:material-code-braces: ComputeTypeTypeDef](./type_defs.md#computetypetypedef) 
4. See [:material-code-brackets: WorkspaceBundleStateType](./literals.md#workspacebundlestatetype) 
5. See [:material-code-brackets: BundleTypeType](./literals.md#bundletypetype) 
## CreateWorkspaceImageResultTypeDef

```python
# CreateWorkspaceImageResultTypeDef definition

class CreateWorkspaceImageResultTypeDef(TypedDict):
    ImageId: str,
    Name: str,
    Description: str,
    OperatingSystem: OperatingSystemTypeDef,  # (1)
    State: WorkspaceImageStateType,  # (2)
    RequiredTenancy: WorkspaceImageRequiredTenancyType,  # (3)
    Created: datetime,
    OwnerAccountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: OperatingSystemTypeDef](./type_defs.md#operatingsystemtypedef) 
2. See [:material-code-brackets: WorkspaceImageStateType](./literals.md#workspaceimagestatetype) 
3. See [:material-code-brackets: WorkspaceImageRequiredTenancyType](./literals.md#workspaceimagerequiredtenancytype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspacesPoolRequestRequestTypeDef

```python
# CreateWorkspacesPoolRequestRequestTypeDef definition

class CreateWorkspacesPoolRequestRequestTypeDef(TypedDict):
    PoolName: str,
    Description: str,
    BundleId: str,
    DirectoryId: str,
    Capacity: CapacityTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ApplicationSettings: NotRequired[ApplicationSettingsRequestTypeDef],  # (3)
    TimeoutSettings: NotRequired[TimeoutSettingsTypeDef],  # (4)
```

1. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ApplicationSettingsRequestTypeDef](./type_defs.md#applicationsettingsrequesttypedef) 
4. See [:material-code-braces: TimeoutSettingsTypeDef](./type_defs.md#timeoutsettingstypedef) 
## UpdateWorkspacesPoolRequestRequestTypeDef

```python
# UpdateWorkspacesPoolRequestRequestTypeDef definition

class UpdateWorkspacesPoolRequestRequestTypeDef(TypedDict):
    PoolId: str,
    Description: NotRequired[str],
    BundleId: NotRequired[str],
    DirectoryId: NotRequired[str],
    Capacity: NotRequired[CapacityTypeDef],  # (1)
    ApplicationSettings: NotRequired[ApplicationSettingsRequestTypeDef],  # (2)
    TimeoutSettings: NotRequired[TimeoutSettingsTypeDef],  # (3)
```

1. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
2. See [:material-code-braces: ApplicationSettingsRequestTypeDef](./type_defs.md#applicationsettingsrequesttypedef) 
3. See [:material-code-braces: TimeoutSettingsTypeDef](./type_defs.md#timeoutsettingstypedef) 
## DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef

```python
# DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef definition

class DescribeAccountModificationsRequestDescribeAccountModificationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef

```python
# DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef definition

class DescribeIpGroupsRequestDescribeIpGroupsPaginateTypeDef(TypedDict):
    GroupIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef

```python
# DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef definition

class DescribeWorkspaceBundlesRequestDescribeWorkspaceBundlesPaginateTypeDef(TypedDict):
    BundleIds: NotRequired[Sequence[str]],
    Owner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef

```python
# DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef definition

class DescribeWorkspaceImagesRequestDescribeWorkspaceImagesPaginateTypeDef(TypedDict):
    ImageIds: NotRequired[Sequence[str]],
    ImageType: NotRequired[ImageTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ImageTypeType](./literals.md#imagetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef

```python
# DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef definition

class DescribeWorkspacesConnectionStatusRequestDescribeWorkspacesConnectionStatusPaginateTypeDef(TypedDict):
    WorkspaceIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef

```python
# DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef definition

class DescribeWorkspacesRequestDescribeWorkspacesPaginateTypeDef(TypedDict):
    WorkspaceIds: NotRequired[Sequence[str]],
    DirectoryId: NotRequired[str],
    UserName: NotRequired[str],
    BundleId: NotRequired[str],
    WorkspaceName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountLinksRequestListAccountLinksPaginateTypeDef

```python
# ListAccountLinksRequestListAccountLinksPaginateTypeDef definition

class ListAccountLinksRequestListAccountLinksPaginateTypeDef(TypedDict):
    LinkStatusFilter: NotRequired[Sequence[AccountLinkStatusEnumType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AccountLinkStatusEnumType](./literals.md#accountlinkstatusenumtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef

```python
# ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef definition

class ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef(TypedDict):
    ManagementCidrRangeConstraint: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeApplicationsResultTypeDef

```python
# DescribeApplicationsResultTypeDef definition

class DescribeApplicationsResultTypeDef(TypedDict):
    Applications: List[WorkSpaceApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkSpaceApplicationTypeDef](./type_defs.md#workspaceapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeClientBrandingResultTypeDef

```python
# DescribeClientBrandingResultTypeDef definition

class DescribeClientBrandingResultTypeDef(TypedDict):
    DeviceTypeWindows: DefaultClientBrandingAttributesTypeDef,  # (1)
    DeviceTypeOsx: DefaultClientBrandingAttributesTypeDef,  # (1)
    DeviceTypeAndroid: DefaultClientBrandingAttributesTypeDef,  # (1)
    DeviceTypeIos: IosClientBrandingAttributesTypeDef,  # (4)
    DeviceTypeLinux: DefaultClientBrandingAttributesTypeDef,  # (1)
    DeviceTypeWeb: DefaultClientBrandingAttributesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef) 
2. See [:material-code-braces: DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef) 
3. See [:material-code-braces: DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef) 
4. See [:material-code-braces: IosClientBrandingAttributesTypeDef](./type_defs.md#iosclientbrandingattributestypedef) 
5. See [:material-code-braces: DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef) 
6. See [:material-code-braces: DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportClientBrandingResultTypeDef

```python
# ImportClientBrandingResultTypeDef definition

class ImportClientBrandingResultTypeDef(TypedDict):
    DeviceTypeWindows: DefaultClientBrandingAttributesTypeDef,  # (1)
    DeviceTypeOsx: DefaultClientBrandingAttributesTypeDef,  # (1)
    DeviceTypeAndroid: DefaultClientBrandingAttributesTypeDef,  # (1)
    DeviceTypeIos: IosClientBrandingAttributesTypeDef,  # (4)
    DeviceTypeLinux: DefaultClientBrandingAttributesTypeDef,  # (1)
    DeviceTypeWeb: DefaultClientBrandingAttributesTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef) 
2. See [:material-code-braces: DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef) 
3. See [:material-code-braces: DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef) 
4. See [:material-code-braces: IosClientBrandingAttributesTypeDef](./type_defs.md#iosclientbrandingattributestypedef) 
5. See [:material-code-braces: DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef) 
6. See [:material-code-braces: DefaultClientBrandingAttributesTypeDef](./type_defs.md#defaultclientbrandingattributestypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef

```python
# DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef definition

class DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef(TypedDict):
    DirectoryIds: NotRequired[Sequence[str]],
    WorkspaceDirectoryNames: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    Filters: NotRequired[Sequence[DescribeWorkspaceDirectoriesFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeWorkspaceDirectoriesFilterTypeDef](./type_defs.md#describeworkspacedirectoriesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeWorkspaceDirectoriesRequestRequestTypeDef

```python
# DescribeWorkspaceDirectoriesRequestRequestTypeDef definition

class DescribeWorkspaceDirectoriesRequestRequestTypeDef(TypedDict):
    DirectoryIds: NotRequired[Sequence[str]],
    WorkspaceDirectoryNames: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[DescribeWorkspaceDirectoriesFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: DescribeWorkspaceDirectoriesFilterTypeDef](./type_defs.md#describeworkspacedirectoriesfiltertypedef) 
## DescribeWorkspaceImagePermissionsResultTypeDef

```python
# DescribeWorkspaceImagePermissionsResultTypeDef definition

class DescribeWorkspaceImagePermissionsResultTypeDef(TypedDict):
    ImageId: str,
    ImagePermissions: List[ImagePermissionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImagePermissionTypeDef](./type_defs.md#imagepermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceSnapshotsResultTypeDef

```python
# DescribeWorkspaceSnapshotsResultTypeDef definition

class DescribeWorkspaceSnapshotsResultTypeDef(TypedDict):
    RebuildSnapshots: List[SnapshotTypeDef],  # (1)
    RestoreSnapshots: List[SnapshotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
2. See [:material-code-braces: SnapshotTypeDef](./type_defs.md#snapshottypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspacesConnectionStatusResultTypeDef

```python
# DescribeWorkspacesConnectionStatusResultTypeDef definition

class DescribeWorkspacesConnectionStatusResultTypeDef(TypedDict):
    WorkspacesConnectionStatus: List[WorkspaceConnectionStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceConnectionStatusTypeDef](./type_defs.md#workspaceconnectionstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspacesPoolsRequestRequestTypeDef

```python
# DescribeWorkspacesPoolsRequestRequestTypeDef definition

class DescribeWorkspacesPoolsRequestRequestTypeDef(TypedDict):
    PoolIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[DescribeWorkspacesPoolsFilterTypeDef]],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DescribeWorkspacesPoolsFilterTypeDef](./type_defs.md#describeworkspacespoolsfiltertypedef) 
## RebootWorkspacesResultTypeDef

```python
# RebootWorkspacesResultTypeDef definition

class RebootWorkspacesResultTypeDef(TypedDict):
    FailedRequests: List[FailedWorkspaceChangeRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedWorkspaceChangeRequestTypeDef](./type_defs.md#failedworkspacechangerequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RebuildWorkspacesResultTypeDef

```python
# RebuildWorkspacesResultTypeDef definition

class RebuildWorkspacesResultTypeDef(TypedDict):
    FailedRequests: List[FailedWorkspaceChangeRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedWorkspaceChangeRequestTypeDef](./type_defs.md#failedworkspacechangerequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartWorkspacesResultTypeDef

```python
# StartWorkspacesResultTypeDef definition

class StartWorkspacesResultTypeDef(TypedDict):
    FailedRequests: List[FailedWorkspaceChangeRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedWorkspaceChangeRequestTypeDef](./type_defs.md#failedworkspacechangerequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopWorkspacesResultTypeDef

```python
# StopWorkspacesResultTypeDef definition

class StopWorkspacesResultTypeDef(TypedDict):
    FailedRequests: List[FailedWorkspaceChangeRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedWorkspaceChangeRequestTypeDef](./type_defs.md#failedworkspacechangerequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TerminateWorkspacesResultTypeDef

```python
# TerminateWorkspacesResultTypeDef definition

class TerminateWorkspacesResultTypeDef(TypedDict):
    FailedRequests: List[FailedWorkspaceChangeRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedWorkspaceChangeRequestTypeDef](./type_defs.md#failedworkspacechangerequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterWorkspaceDirectoryRequestRequestTypeDef

```python
# RegisterWorkspaceDirectoryRequestRequestTypeDef definition

class RegisterWorkspaceDirectoryRequestRequestTypeDef(TypedDict):
    DirectoryId: NotRequired[str],
    SubnetIds: NotRequired[Sequence[str]],
    EnableWorkDocs: NotRequired[bool],
    EnableSelfService: NotRequired[bool],
    Tenancy: NotRequired[TenancyType],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    WorkspaceDirectoryName: NotRequired[str],
    WorkspaceDirectoryDescription: NotRequired[str],
    UserIdentityType: NotRequired[UserIdentityTypeType],  # (3)
    IdcInstanceArn: NotRequired[str],
    MicrosoftEntraConfig: NotRequired[MicrosoftEntraConfigTypeDef],  # (4)
    WorkspaceType: NotRequired[WorkspaceTypeType],  # (5)
    ActiveDirectoryConfig: NotRequired[ActiveDirectoryConfigTypeDef],  # (6)
```

1. See [:material-code-brackets: TenancyType](./literals.md#tenancytype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: UserIdentityTypeType](./literals.md#useridentitytypetype) 
4. See [:material-code-braces: MicrosoftEntraConfigTypeDef](./type_defs.md#microsoftentraconfigtypedef) 
5. See [:material-code-brackets: WorkspaceTypeType](./literals.md#workspacetypetype) 
6. See [:material-code-braces: ActiveDirectoryConfigTypeDef](./type_defs.md#activedirectoryconfigtypedef) 
## ModifySamlPropertiesRequestRequestTypeDef

```python
# ModifySamlPropertiesRequestRequestTypeDef definition

class ModifySamlPropertiesRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    SamlProperties: NotRequired[SamlPropertiesTypeDef],  # (1)
    PropertiesToDelete: NotRequired[Sequence[DeletableSamlPropertyType]],  # (2)
```

1. See [:material-code-braces: SamlPropertiesTypeDef](./type_defs.md#samlpropertiestypedef) 
2. See [:material-code-brackets: DeletableSamlPropertyType](./literals.md#deletablesamlpropertytype) 
## ModifySelfservicePermissionsRequestRequestTypeDef

```python
# ModifySelfservicePermissionsRequestRequestTypeDef definition

class ModifySelfservicePermissionsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    SelfservicePermissions: SelfservicePermissionsTypeDef,  # (1)
```

1. See [:material-code-braces: SelfservicePermissionsTypeDef](./type_defs.md#selfservicepermissionstypedef) 
## ModifyWorkspaceAccessPropertiesRequestRequestTypeDef

```python
# ModifyWorkspaceAccessPropertiesRequestRequestTypeDef definition

class ModifyWorkspaceAccessPropertiesRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    WorkspaceAccessProperties: WorkspaceAccessPropertiesTypeDef,  # (1)
```

1. See [:material-code-braces: WorkspaceAccessPropertiesTypeDef](./type_defs.md#workspaceaccesspropertiestypedef) 
## ModifyWorkspaceCreationPropertiesRequestRequestTypeDef

```python
# ModifyWorkspaceCreationPropertiesRequestRequestTypeDef definition

class ModifyWorkspaceCreationPropertiesRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    WorkspaceCreationProperties: WorkspaceCreationPropertiesTypeDef,  # (1)
```

1. See [:material-code-braces: WorkspaceCreationPropertiesTypeDef](./type_defs.md#workspacecreationpropertiestypedef) 
## ModifyWorkspacePropertiesRequestRequestTypeDef

```python
# ModifyWorkspacePropertiesRequestRequestTypeDef definition

class ModifyWorkspacePropertiesRequestRequestTypeDef(TypedDict):
    WorkspaceId: str,
    WorkspaceProperties: NotRequired[WorkspacePropertiesTypeDef],  # (1)
    DataReplication: NotRequired[DataReplicationType],  # (2)
```

1. See [:material-code-braces: WorkspacePropertiesTypeDef](./type_defs.md#workspacepropertiestypedef) 
2. See [:material-code-brackets: DataReplicationType](./literals.md#datareplicationtype) 
## WorkspacesPoolSessionTypeDef

```python
# WorkspacesPoolSessionTypeDef definition

class WorkspacesPoolSessionTypeDef(TypedDict):
    SessionId: str,
    PoolId: str,
    UserId: str,
    AuthenticationType: NotRequired[AuthenticationTypeType],  # (1)
    ConnectionState: NotRequired[SessionConnectionStateType],  # (2)
    InstanceId: NotRequired[str],
    ExpirationTime: NotRequired[datetime],
    NetworkAccessConfiguration: NotRequired[NetworkAccessConfigurationTypeDef],  # (3)
    StartTime: NotRequired[datetime],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-brackets: SessionConnectionStateType](./literals.md#sessionconnectionstatetype) 
3. See [:material-code-braces: NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef) 
## RebootWorkspacesRequestRequestTypeDef

```python
# RebootWorkspacesRequestRequestTypeDef definition

class RebootWorkspacesRequestRequestTypeDef(TypedDict):
    RebootWorkspaceRequests: Sequence[RebootRequestTypeDef],  # (1)
```

1. See [:material-code-braces: RebootRequestTypeDef](./type_defs.md#rebootrequesttypedef) 
## RebuildWorkspacesRequestRequestTypeDef

```python
# RebuildWorkspacesRequestRequestTypeDef definition

class RebuildWorkspacesRequestRequestTypeDef(TypedDict):
    RebuildWorkspaceRequests: Sequence[RebuildRequestTypeDef],  # (1)
```

1. See [:material-code-braces: RebuildRequestTypeDef](./type_defs.md#rebuildrequesttypedef) 
## StartWorkspacesRequestRequestTypeDef

```python
# StartWorkspacesRequestRequestTypeDef definition

class StartWorkspacesRequestRequestTypeDef(TypedDict):
    StartWorkspaceRequests: Sequence[StartRequestTypeDef],  # (1)
```

1. See [:material-code-braces: StartRequestTypeDef](./type_defs.md#startrequesttypedef) 
## StopWorkspacesRequestRequestTypeDef

```python
# StopWorkspacesRequestRequestTypeDef definition

class StopWorkspacesRequestRequestTypeDef(TypedDict):
    StopWorkspaceRequests: Sequence[StopRequestTypeDef],  # (1)
```

1. See [:material-code-braces: StopRequestTypeDef](./type_defs.md#stoprequesttypedef) 
## StreamingPropertiesOutputTypeDef

```python
# StreamingPropertiesOutputTypeDef definition

class StreamingPropertiesOutputTypeDef(TypedDict):
    StreamingExperiencePreferredProtocol: NotRequired[StreamingExperiencePreferredProtocolEnumType],  # (1)
    UserSettings: NotRequired[List[UserSettingTypeDef]],  # (2)
    StorageConnectors: NotRequired[List[StorageConnectorTypeDef]],  # (3)
```

1. See [:material-code-brackets: StreamingExperiencePreferredProtocolEnumType](./literals.md#streamingexperiencepreferredprotocolenumtype) 
2. See [:material-code-braces: UserSettingTypeDef](./type_defs.md#usersettingtypedef) 
3. See [:material-code-braces: StorageConnectorTypeDef](./type_defs.md#storageconnectortypedef) 
## StreamingPropertiesTypeDef

```python
# StreamingPropertiesTypeDef definition

class StreamingPropertiesTypeDef(TypedDict):
    StreamingExperiencePreferredProtocol: NotRequired[StreamingExperiencePreferredProtocolEnumType],  # (1)
    UserSettings: NotRequired[Sequence[UserSettingTypeDef]],  # (2)
    StorageConnectors: NotRequired[Sequence[StorageConnectorTypeDef]],  # (3)
```

1. See [:material-code-brackets: StreamingExperiencePreferredProtocolEnumType](./literals.md#streamingexperiencepreferredprotocolenumtype) 
2. See [:material-code-braces: UserSettingTypeDef](./type_defs.md#usersettingtypedef) 
3. See [:material-code-braces: StorageConnectorTypeDef](./type_defs.md#storageconnectortypedef) 
## TerminateWorkspacesRequestRequestTypeDef

```python
# TerminateWorkspacesRequestRequestTypeDef definition

class TerminateWorkspacesRequestRequestTypeDef(TypedDict):
    TerminateWorkspaceRequests: Sequence[TerminateRequestTypeDef],  # (1)
```

1. See [:material-code-braces: TerminateRequestTypeDef](./type_defs.md#terminaterequesttypedef) 
## WorkspaceImageTypeDef

```python
# WorkspaceImageTypeDef definition

class WorkspaceImageTypeDef(TypedDict):
    ImageId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    OperatingSystem: NotRequired[OperatingSystemTypeDef],  # (1)
    State: NotRequired[WorkspaceImageStateType],  # (2)
    RequiredTenancy: NotRequired[WorkspaceImageRequiredTenancyType],  # (3)
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
    Created: NotRequired[datetime],
    OwnerAccountId: NotRequired[str],
    Updates: NotRequired[UpdateResultTypeDef],  # (4)
    ErrorDetails: NotRequired[List[ErrorDetailsTypeDef]],  # (5)
```

1. See [:material-code-braces: OperatingSystemTypeDef](./type_defs.md#operatingsystemtypedef) 
2. See [:material-code-brackets: WorkspaceImageStateType](./literals.md#workspaceimagestatetype) 
3. See [:material-code-brackets: WorkspaceImageRequiredTenancyType](./literals.md#workspaceimagerequiredtenancytype) 
4. See [:material-code-braces: UpdateResultTypeDef](./type_defs.md#updateresulttypedef) 
5. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## WorkspaceRequestOutputTypeDef

```python
# WorkspaceRequestOutputTypeDef definition

class WorkspaceRequestOutputTypeDef(TypedDict):
    DirectoryId: str,
    UserName: str,
    BundleId: str,
    VolumeEncryptionKey: NotRequired[str],
    UserVolumeEncryptionEnabled: NotRequired[bool],
    RootVolumeEncryptionEnabled: NotRequired[bool],
    WorkspaceProperties: NotRequired[WorkspacePropertiesOutputTypeDef],  # (1)
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    WorkspaceName: NotRequired[str],
```

1. See [:material-code-braces: WorkspacePropertiesOutputTypeDef](./type_defs.md#workspacepropertiesoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## WorkspaceTypeDef

```python
# WorkspaceTypeDef definition

class WorkspaceTypeDef(TypedDict):
    WorkspaceId: NotRequired[str],
    DirectoryId: NotRequired[str],
    UserName: NotRequired[str],
    IpAddress: NotRequired[str],
    State: NotRequired[WorkspaceStateType],  # (1)
    BundleId: NotRequired[str],
    SubnetId: NotRequired[str],
    ErrorMessage: NotRequired[str],
    ErrorCode: NotRequired[str],
    ComputerName: NotRequired[str],
    VolumeEncryptionKey: NotRequired[str],
    UserVolumeEncryptionEnabled: NotRequired[bool],
    RootVolumeEncryptionEnabled: NotRequired[bool],
    WorkspaceName: NotRequired[str],
    WorkspaceProperties: NotRequired[WorkspacePropertiesOutputTypeDef],  # (2)
    ModificationStates: NotRequired[List[ModificationStateTypeDef]],  # (3)
    RelatedWorkspaces: NotRequired[List[RelatedWorkspacePropertiesTypeDef]],  # (4)
    DataReplicationSettings: NotRequired[DataReplicationSettingsTypeDef],  # (5)
    StandbyWorkspacesProperties: NotRequired[List[StandbyWorkspacesPropertiesTypeDef]],  # (6)
```

1. See [:material-code-brackets: WorkspaceStateType](./literals.md#workspacestatetype) 
2. See [:material-code-braces: WorkspacePropertiesOutputTypeDef](./type_defs.md#workspacepropertiesoutputtypedef) 
3. See [:material-code-braces: ModificationStateTypeDef](./type_defs.md#modificationstatetypedef) 
4. See [:material-code-braces: RelatedWorkspacePropertiesTypeDef](./type_defs.md#relatedworkspacepropertiestypedef) 
5. See [:material-code-braces: DataReplicationSettingsTypeDef](./type_defs.md#datareplicationsettingstypedef) 
6. See [:material-code-braces: StandbyWorkspacesPropertiesTypeDef](./type_defs.md#standbyworkspacespropertiestypedef) 
## WorkspacesPoolTypeDef

```python
# WorkspacesPoolTypeDef definition

class WorkspacesPoolTypeDef(TypedDict):
    PoolId: str,
    PoolArn: str,
    CapacityStatus: CapacityStatusTypeDef,  # (1)
    PoolName: str,
    State: WorkspacesPoolStateType,  # (2)
    CreatedAt: datetime,
    BundleId: str,
    DirectoryId: str,
    Description: NotRequired[str],
    Errors: NotRequired[List[WorkspacesPoolErrorTypeDef]],  # (3)
    ApplicationSettings: NotRequired[ApplicationSettingsResponseTypeDef],  # (4)
    TimeoutSettings: NotRequired[TimeoutSettingsTypeDef],  # (5)
```

1. See [:material-code-braces: CapacityStatusTypeDef](./type_defs.md#capacitystatustypedef) 
2. See [:material-code-brackets: WorkspacesPoolStateType](./literals.md#workspacespoolstatetype) 
3. See [:material-code-braces: WorkspacesPoolErrorTypeDef](./type_defs.md#workspacespoolerrortypedef) 
4. See [:material-code-braces: ApplicationSettingsResponseTypeDef](./type_defs.md#applicationsettingsresponsetypedef) 
5. See [:material-code-braces: TimeoutSettingsTypeDef](./type_defs.md#timeoutsettingstypedef) 
## DescribeApplicationAssociationsResultTypeDef

```python
# DescribeApplicationAssociationsResultTypeDef definition

class DescribeApplicationAssociationsResultTypeDef(TypedDict):
    Associations: List[ApplicationResourceAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationResourceAssociationTypeDef](./type_defs.md#applicationresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBundleAssociationsResultTypeDef

```python
# DescribeBundleAssociationsResultTypeDef definition

class DescribeBundleAssociationsResultTypeDef(TypedDict):
    Associations: List[BundleResourceAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BundleResourceAssociationTypeDef](./type_defs.md#bundleresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImageAssociationsResultTypeDef

```python
# DescribeImageAssociationsResultTypeDef definition

class DescribeImageAssociationsResultTypeDef(TypedDict):
    Associations: List[ImageResourceAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageResourceAssociationTypeDef](./type_defs.md#imageresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateWorkspaceApplicationResultTypeDef

```python
# AssociateWorkspaceApplicationResultTypeDef definition

class AssociateWorkspaceApplicationResultTypeDef(TypedDict):
    Association: WorkspaceResourceAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceResourceAssociationTypeDef](./type_defs.md#workspaceresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceAssociationsResultTypeDef

```python
# DescribeWorkspaceAssociationsResultTypeDef definition

class DescribeWorkspaceAssociationsResultTypeDef(TypedDict):
    Associations: List[WorkspaceResourceAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceResourceAssociationTypeDef](./type_defs.md#workspaceresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateWorkspaceApplicationResultTypeDef

```python
# DisassociateWorkspaceApplicationResultTypeDef definition

class DisassociateWorkspaceApplicationResultTypeDef(TypedDict):
    Association: WorkspaceResourceAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceResourceAssociationTypeDef](./type_defs.md#workspaceresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkSpaceApplicationDeploymentTypeDef

```python
# WorkSpaceApplicationDeploymentTypeDef definition

class WorkSpaceApplicationDeploymentTypeDef(TypedDict):
    Associations: NotRequired[List[WorkspaceResourceAssociationTypeDef]],  # (1)
```

1. See [:material-code-braces: WorkspaceResourceAssociationTypeDef](./type_defs.md#workspaceresourceassociationtypedef) 
## DescribeIpGroupsResultTypeDef

```python
# DescribeIpGroupsResultTypeDef definition

class DescribeIpGroupsResultTypeDef(TypedDict):
    Result: List[WorkspacesIpGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspacesIpGroupTypeDef](./type_defs.md#workspacesipgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportClientBrandingRequestRequestTypeDef

```python
# ImportClientBrandingRequestRequestTypeDef definition

class ImportClientBrandingRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    DeviceTypeWindows: NotRequired[DefaultImportClientBrandingAttributesTypeDef],  # (1)
    DeviceTypeOsx: NotRequired[DefaultImportClientBrandingAttributesTypeDef],  # (1)
    DeviceTypeAndroid: NotRequired[DefaultImportClientBrandingAttributesTypeDef],  # (1)
    DeviceTypeIos: NotRequired[IosImportClientBrandingAttributesTypeDef],  # (4)
    DeviceTypeLinux: NotRequired[DefaultImportClientBrandingAttributesTypeDef],  # (1)
    DeviceTypeWeb: NotRequired[DefaultImportClientBrandingAttributesTypeDef],  # (1)
```

1. See [:material-code-braces: DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef) 
2. See [:material-code-braces: DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef) 
3. See [:material-code-braces: DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef) 
4. See [:material-code-braces: IosImportClientBrandingAttributesTypeDef](./type_defs.md#iosimportclientbrandingattributestypedef) 
5. See [:material-code-braces: DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef) 
6. See [:material-code-braces: DefaultImportClientBrandingAttributesTypeDef](./type_defs.md#defaultimportclientbrandingattributestypedef) 
## DescribeClientPropertiesResultTypeDef

```python
# DescribeClientPropertiesResultTypeDef definition

class DescribeClientPropertiesResultTypeDef(TypedDict):
    ClientPropertiesList: List[ClientPropertiesResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClientPropertiesResultTypeDef](./type_defs.md#clientpropertiesresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConnectionAliasesResultTypeDef

```python
# DescribeConnectionAliasesResultTypeDef definition

class DescribeConnectionAliasesResultTypeDef(TypedDict):
    ConnectionAliases: List[ConnectionAliasTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectionAliasTypeDef](./type_defs.md#connectionaliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailedCreateStandbyWorkspacesRequestTypeDef

```python
# FailedCreateStandbyWorkspacesRequestTypeDef definition

class FailedCreateStandbyWorkspacesRequestTypeDef(TypedDict):
    StandbyWorkspaceRequest: NotRequired[StandbyWorkspaceOutputTypeDef],  # (1)
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-braces: StandbyWorkspaceOutputTypeDef](./type_defs.md#standbyworkspaceoutputtypedef) 
## CreateWorkspaceBundleResultTypeDef

```python
# CreateWorkspaceBundleResultTypeDef definition

class CreateWorkspaceBundleResultTypeDef(TypedDict):
    WorkspaceBundle: WorkspaceBundleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceBundleTypeDef](./type_defs.md#workspacebundletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceBundlesResultTypeDef

```python
# DescribeWorkspaceBundlesResultTypeDef definition

class DescribeWorkspaceBundlesResultTypeDef(TypedDict):
    Bundles: List[WorkspaceBundleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceBundleTypeDef](./type_defs.md#workspacebundletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspacesPoolSessionsResultTypeDef

```python
# DescribeWorkspacesPoolSessionsResultTypeDef definition

class DescribeWorkspacesPoolSessionsResultTypeDef(TypedDict):
    Sessions: List[WorkspacesPoolSessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspacesPoolSessionTypeDef](./type_defs.md#workspacespoolsessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkspaceDirectoryTypeDef

```python
# WorkspaceDirectoryTypeDef definition

class WorkspaceDirectoryTypeDef(TypedDict):
    DirectoryId: NotRequired[str],
    Alias: NotRequired[str],
    DirectoryName: NotRequired[str],
    RegistrationCode: NotRequired[str],
    SubnetIds: NotRequired[List[str]],
    DnsIpAddresses: NotRequired[List[str]],
    CustomerUserName: NotRequired[str],
    IamRoleId: NotRequired[str],
    DirectoryType: NotRequired[WorkspaceDirectoryTypeType],  # (1)
    WorkspaceSecurityGroupId: NotRequired[str],
    State: NotRequired[WorkspaceDirectoryStateType],  # (2)
    WorkspaceCreationProperties: NotRequired[DefaultWorkspaceCreationPropertiesTypeDef],  # (3)
    ipGroupIds: NotRequired[List[str]],
    WorkspaceAccessProperties: NotRequired[WorkspaceAccessPropertiesTypeDef],  # (4)
    Tenancy: NotRequired[TenancyType],  # (5)
    SelfservicePermissions: NotRequired[SelfservicePermissionsTypeDef],  # (6)
    SamlProperties: NotRequired[SamlPropertiesTypeDef],  # (7)
    CertificateBasedAuthProperties: NotRequired[CertificateBasedAuthPropertiesTypeDef],  # (8)
    MicrosoftEntraConfig: NotRequired[MicrosoftEntraConfigTypeDef],  # (9)
    WorkspaceDirectoryName: NotRequired[str],
    WorkspaceDirectoryDescription: NotRequired[str],
    UserIdentityType: NotRequired[UserIdentityTypeType],  # (10)
    WorkspaceType: NotRequired[WorkspaceTypeType],  # (11)
    IDCConfig: NotRequired[IDCConfigTypeDef],  # (12)
    ActiveDirectoryConfig: NotRequired[ActiveDirectoryConfigTypeDef],  # (13)
    StreamingProperties: NotRequired[StreamingPropertiesOutputTypeDef],  # (14)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: WorkspaceDirectoryTypeType](./literals.md#workspacedirectorytypetype) 
2. See [:material-code-brackets: WorkspaceDirectoryStateType](./literals.md#workspacedirectorystatetype) 
3. See [:material-code-braces: DefaultWorkspaceCreationPropertiesTypeDef](./type_defs.md#defaultworkspacecreationpropertiestypedef) 
4. See [:material-code-braces: WorkspaceAccessPropertiesTypeDef](./type_defs.md#workspaceaccesspropertiestypedef) 
5. See [:material-code-brackets: TenancyType](./literals.md#tenancytype) 
6. See [:material-code-braces: SelfservicePermissionsTypeDef](./type_defs.md#selfservicepermissionstypedef) 
7. See [:material-code-braces: SamlPropertiesTypeDef](./type_defs.md#samlpropertiestypedef) 
8. See [:material-code-braces: CertificateBasedAuthPropertiesTypeDef](./type_defs.md#certificatebasedauthpropertiestypedef) 
9. See [:material-code-braces: MicrosoftEntraConfigTypeDef](./type_defs.md#microsoftentraconfigtypedef) 
10. See [:material-code-brackets: UserIdentityTypeType](./literals.md#useridentitytypetype) 
11. See [:material-code-brackets: WorkspaceTypeType](./literals.md#workspacetypetype) 
12. See [:material-code-braces: IDCConfigTypeDef](./type_defs.md#idcconfigtypedef) 
13. See [:material-code-braces: ActiveDirectoryConfigTypeDef](./type_defs.md#activedirectoryconfigtypedef) 
14. See [:material-code-braces: StreamingPropertiesOutputTypeDef](./type_defs.md#streamingpropertiesoutputtypedef) 
## ModifyStreamingPropertiesRequestRequestTypeDef

```python
# ModifyStreamingPropertiesRequestRequestTypeDef definition

class ModifyStreamingPropertiesRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    StreamingProperties: NotRequired[StreamingPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: StreamingPropertiesTypeDef](./type_defs.md#streamingpropertiestypedef) 
## DescribeWorkspaceImagesResultTypeDef

```python
# DescribeWorkspaceImagesResultTypeDef definition

class DescribeWorkspaceImagesResultTypeDef(TypedDict):
    Images: List[WorkspaceImageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceImageTypeDef](./type_defs.md#workspaceimagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkspaceRequestTypeDef

```python
# WorkspaceRequestTypeDef definition

class WorkspaceRequestTypeDef(TypedDict):
    DirectoryId: str,
    UserName: str,
    BundleId: str,
    VolumeEncryptionKey: NotRequired[str],
    UserVolumeEncryptionEnabled: NotRequired[bool],
    RootVolumeEncryptionEnabled: NotRequired[bool],
    WorkspaceProperties: NotRequired[WorkspacePropertiesUnionTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    WorkspaceName: NotRequired[str],
```

1. See [:material-code-braces: WorkspacePropertiesTypeDef](./type_defs.md#workspacepropertiestypedef) [:material-code-braces: WorkspacePropertiesOutputTypeDef](./type_defs.md#workspacepropertiesoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## FailedCreateWorkspaceRequestTypeDef

```python
# FailedCreateWorkspaceRequestTypeDef definition

class FailedCreateWorkspaceRequestTypeDef(TypedDict):
    WorkspaceRequest: NotRequired[WorkspaceRequestOutputTypeDef],  # (1)
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceRequestOutputTypeDef](./type_defs.md#workspacerequestoutputtypedef) 
## DescribeWorkspacesResultTypeDef

```python
# DescribeWorkspacesResultTypeDef definition

class DescribeWorkspacesResultTypeDef(TypedDict):
    Workspaces: List[WorkspaceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceTypeDef](./type_defs.md#workspacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspacesPoolResultTypeDef

```python
# CreateWorkspacesPoolResultTypeDef definition

class CreateWorkspacesPoolResultTypeDef(TypedDict):
    WorkspacesPool: WorkspacesPoolTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspacesPoolTypeDef](./type_defs.md#workspacespooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspacesPoolsResultTypeDef

```python
# DescribeWorkspacesPoolsResultTypeDef definition

class DescribeWorkspacesPoolsResultTypeDef(TypedDict):
    WorkspacesPools: List[WorkspacesPoolTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspacesPoolTypeDef](./type_defs.md#workspacespooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkspacesPoolResultTypeDef

```python
# UpdateWorkspacesPoolResultTypeDef definition

class UpdateWorkspacesPoolResultTypeDef(TypedDict):
    WorkspacesPool: WorkspacesPoolTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspacesPoolTypeDef](./type_defs.md#workspacespooltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeployWorkspaceApplicationsResultTypeDef

```python
# DeployWorkspaceApplicationsResultTypeDef definition

class DeployWorkspaceApplicationsResultTypeDef(TypedDict):
    Deployment: WorkSpaceApplicationDeploymentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkSpaceApplicationDeploymentTypeDef](./type_defs.md#workspaceapplicationdeploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStandbyWorkspacesResultTypeDef

```python
# CreateStandbyWorkspacesResultTypeDef definition

class CreateStandbyWorkspacesResultTypeDef(TypedDict):
    FailedStandbyRequests: List[FailedCreateStandbyWorkspacesRequestTypeDef],  # (1)
    PendingStandbyRequests: List[PendingCreateStandbyWorkspacesRequestTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FailedCreateStandbyWorkspacesRequestTypeDef](./type_defs.md#failedcreatestandbyworkspacesrequesttypedef) 
2. See [:material-code-braces: PendingCreateStandbyWorkspacesRequestTypeDef](./type_defs.md#pendingcreatestandbyworkspacesrequesttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStandbyWorkspacesRequestRequestTypeDef

```python
# CreateStandbyWorkspacesRequestRequestTypeDef definition

class CreateStandbyWorkspacesRequestRequestTypeDef(TypedDict):
    PrimaryRegion: str,
    StandbyWorkspaces: Sequence[StandbyWorkspaceUnionTypeDef],  # (1)
```

1. See [:material-code-braces: StandbyWorkspaceTypeDef](./type_defs.md#standbyworkspacetypedef) [:material-code-braces: StandbyWorkspaceOutputTypeDef](./type_defs.md#standbyworkspaceoutputtypedef) 
## DescribeWorkspaceDirectoriesResultTypeDef

```python
# DescribeWorkspaceDirectoriesResultTypeDef definition

class DescribeWorkspaceDirectoriesResultTypeDef(TypedDict):
    Directories: List[WorkspaceDirectoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceDirectoryTypeDef](./type_defs.md#workspacedirectorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspacesResultTypeDef

```python
# CreateWorkspacesResultTypeDef definition

class CreateWorkspacesResultTypeDef(TypedDict):
    FailedRequests: List[FailedCreateWorkspaceRequestTypeDef],  # (1)
    PendingRequests: List[WorkspaceTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FailedCreateWorkspaceRequestTypeDef](./type_defs.md#failedcreateworkspacerequesttypedef) 
2. See [:material-code-braces: WorkspaceTypeDef](./type_defs.md#workspacetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspacesRequestRequestTypeDef

```python
# CreateWorkspacesRequestRequestTypeDef definition

class CreateWorkspacesRequestRequestTypeDef(TypedDict):
    Workspaces: Sequence[WorkspaceRequestUnionTypeDef],  # (1)
```

1. See [:material-code-braces: WorkspaceRequestTypeDef](./type_defs.md#workspacerequesttypedef) [:material-code-braces: WorkspaceRequestOutputTypeDef](./type_defs.md#workspacerequestoutputtypedef) 
