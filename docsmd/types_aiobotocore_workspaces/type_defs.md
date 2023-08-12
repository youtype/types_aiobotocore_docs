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
## AssociateConnectionAliasRequestRequestTypeDef

```python
# AssociateConnectionAliasRequestRequestTypeDef definition

class AssociateConnectionAliasRequestRequestTypeDef(TypedDict):
    AliasId: str,
    ResourceId: str,
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

## AssociateIpGroupsRequestRequestTypeDef

```python
# AssociateIpGroupsRequestRequestTypeDef definition

class AssociateIpGroupsRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    GroupIds: Sequence[str],
```

## IpRuleItemTypeDef

```python
# IpRuleItemTypeDef definition

class IpRuleItemTypeDef(TypedDict):
    ipRule: NotRequired[str],
    ruleDesc: NotRequired[str],
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
    Capacity: NotRequired[str],
```

## UserStorageTypeDef

```python
# UserStorageTypeDef definition

class UserStorageTypeDef(TypedDict):
    Capacity: NotRequired[str],
```

## OperatingSystemTypeDef

```python
# OperatingSystemTypeDef definition

class OperatingSystemTypeDef(TypedDict):
    Type: NotRequired[OperatingSystemTypeType],  # (1)
```

1. See [:material-code-brackets: OperatingSystemTypeType](./literals.md#operatingsystemtypetype) 
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

## DescribeWorkspaceBundlesRequestRequestTypeDef

```python
# DescribeWorkspaceBundlesRequestRequestTypeDef definition

class DescribeWorkspaceBundlesRequestRequestTypeDef(TypedDict):
    BundleIds: NotRequired[Sequence[str]],
    Owner: NotRequired[str],
    NextToken: NotRequired[str],
```

## DescribeWorkspaceDirectoriesRequestRequestTypeDef

```python
# DescribeWorkspaceDirectoriesRequestRequestTypeDef definition

class DescribeWorkspaceDirectoriesRequestRequestTypeDef(TypedDict):
    DirectoryIds: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

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

## FailedWorkspaceChangeRequestTypeDef

```python
# FailedWorkspaceChangeRequestTypeDef definition

class FailedWorkspaceChangeRequestTypeDef(TypedDict):
    WorkspaceId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## ListAvailableManagementCidrRangesRequestRequestTypeDef

```python
# ListAvailableManagementCidrRangesRequestRequestTypeDef definition

class ListAvailableManagementCidrRangesRequestRequestTypeDef(TypedDict):
    ManagementCidrRangeConstraint: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
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
```

1. See [:material-code-brackets: RunningModeType](./literals.md#runningmodetype) 
2. See [:material-code-brackets: ComputeType](./literals.md#computetype) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## ModifyWorkspaceStateRequestRequestTypeDef

```python
# ModifyWorkspaceStateRequestRequestTypeDef definition

class ModifyWorkspaceStateRequestRequestTypeDef(TypedDict):
    WorkspaceId: str,
    WorkspaceState: TargetWorkspaceStateType,  # (1)
```

1. See [:material-code-brackets: TargetWorkspaceStateType](./literals.md#targetworkspacestatetype) 
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

## StartRequestTypeDef

```python
# StartRequestTypeDef definition

class StartRequestTypeDef(TypedDict):
    WorkspaceId: NotRequired[str],
```

## StopRequestTypeDef

```python
# StopRequestTypeDef definition

class StopRequestTypeDef(TypedDict):
    WorkspaceId: NotRequired[str],
```

## TerminateRequestTypeDef

```python
# TerminateRequestTypeDef definition

class TerminateRequestTypeDef(TypedDict):
    WorkspaceId: str,
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
## DescribeAccountModificationsResultTypeDef

```python
# DescribeAccountModificationsResultTypeDef definition

class DescribeAccountModificationsResultTypeDef(TypedDict):
    AccountModifications: List[AccountModificationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountModificationTypeDef](./type_defs.md#accountmodificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountResultTypeDef

```python
# DescribeAccountResultTypeDef definition

class DescribeAccountResultTypeDef(TypedDict):
    DedicatedTenancySupport: DedicatedTenancySupportResultEnumType,  # (1)
    DedicatedTenancyManagementCidrRange: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DedicatedTenancySupportResultEnumType](./literals.md#dedicatedtenancysupportresultenumtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportWorkspaceImageResultTypeDef

```python
# ImportWorkspaceImageResultTypeDef definition

class ImportWorkspaceImageResultTypeDef(TypedDict):
    ImageId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAvailableManagementCidrRangesResultTypeDef

```python
# ListAvailableManagementCidrRangesResultTypeDef definition

class ListAvailableManagementCidrRangesResultTypeDef(TypedDict):
    ManagementCidrRanges: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
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
    Logo: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    SupportEmail: NotRequired[str],
    SupportLink: NotRequired[str],
    ForgotPasswordLink: NotRequired[str],
    LoginMessage: NotRequired[Mapping[str, str]],
```

## IosImportClientBrandingAttributesTypeDef

```python
# IosImportClientBrandingAttributesTypeDef definition

class IosImportClientBrandingAttributesTypeDef(TypedDict):
    Logo: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    Logo2x: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    Logo3x: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
## RegisterWorkspaceDirectoryRequestRequestTypeDef

```python
# RegisterWorkspaceDirectoryRequestRequestTypeDef definition

class RegisterWorkspaceDirectoryRequestRequestTypeDef(TypedDict):
    DirectoryId: str,
    EnableWorkDocs: bool,
    SubnetIds: NotRequired[Sequence[str]],
    EnableSelfService: NotRequired[bool],
    Tenancy: NotRequired[TenancyType],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: TenancyType](./literals.md#tenancytype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StandbyWorkspaceTypeDef

```python
# StandbyWorkspaceTypeDef definition

class StandbyWorkspaceTypeDef(TypedDict):
    PrimaryWorkspaceId: str,
    DirectoryId: str,
    VolumeEncryptionKey: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
## DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef

```python
# DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef definition

class DescribeWorkspaceDirectoriesRequestDescribeWorkspaceDirectoriesPaginateTypeDef(TypedDict):
    DirectoryIds: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
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
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef

```python
# ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef definition

class ListAvailableManagementCidrRangesRequestListAvailableManagementCidrRangesPaginateTypeDef(TypedDict):
    ManagementCidrRangeConstraint: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
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
## DescribeWorkspaceImagePermissionsResultTypeDef

```python
# DescribeWorkspaceImagePermissionsResultTypeDef definition

class DescribeWorkspaceImagePermissionsResultTypeDef(TypedDict):
    ImageId: str,
    ImagePermissions: List[ImagePermissionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceConnectionStatusTypeDef](./type_defs.md#workspaceconnectionstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
```

1. See [:material-code-brackets: WorkspaceDirectoryTypeType](./literals.md#workspacedirectorytypetype) 
2. See [:material-code-brackets: WorkspaceDirectoryStateType](./literals.md#workspacedirectorystatetype) 
3. See [:material-code-braces: DefaultWorkspaceCreationPropertiesTypeDef](./type_defs.md#defaultworkspacecreationpropertiestypedef) 
4. See [:material-code-braces: WorkspaceAccessPropertiesTypeDef](./type_defs.md#workspaceaccesspropertiestypedef) 
5. See [:material-code-brackets: TenancyType](./literals.md#tenancytype) 
6. See [:material-code-braces: SelfservicePermissionsTypeDef](./type_defs.md#selfservicepermissionstypedef) 
7. See [:material-code-braces: SamlPropertiesTypeDef](./type_defs.md#samlpropertiestypedef) 
8. See [:material-code-braces: CertificateBasedAuthPropertiesTypeDef](./type_defs.md#certificatebasedauthpropertiestypedef) 
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
    WorkspaceProperties: WorkspacePropertiesTypeDef,  # (1)
```

1. See [:material-code-braces: WorkspacePropertiesTypeDef](./type_defs.md#workspacepropertiestypedef) 
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
    WorkspaceProperties: NotRequired[WorkspacePropertiesTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: WorkspacePropertiesTypeDef](./type_defs.md#workspacepropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
    WorkspaceProperties: NotRequired[WorkspacePropertiesTypeDef],  # (2)
    ModificationStates: NotRequired[List[ModificationStateTypeDef]],  # (3)
    RelatedWorkspaces: NotRequired[List[RelatedWorkspacePropertiesTypeDef]],  # (4)
```

1. See [:material-code-brackets: WorkspaceStateType](./literals.md#workspacestatetype) 
2. See [:material-code-braces: WorkspacePropertiesTypeDef](./type_defs.md#workspacepropertiestypedef) 
3. See [:material-code-braces: ModificationStateTypeDef](./type_defs.md#modificationstatetypedef) 
4. See [:material-code-braces: RelatedWorkspacePropertiesTypeDef](./type_defs.md#relatedworkspacepropertiestypedef) 
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
```

1. See [:material-code-braces: OperatingSystemTypeDef](./type_defs.md#operatingsystemtypedef) 
2. See [:material-code-brackets: WorkspaceImageStateType](./literals.md#workspaceimagestatetype) 
3. See [:material-code-brackets: WorkspaceImageRequiredTenancyType](./literals.md#workspaceimagerequiredtenancytype) 
4. See [:material-code-braces: UpdateResultTypeDef](./type_defs.md#updateresulttypedef) 
## DescribeIpGroupsResultTypeDef

```python
# DescribeIpGroupsResultTypeDef definition

class DescribeIpGroupsResultTypeDef(TypedDict):
    Result: List[WorkspacesIpGroupTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionAliasTypeDef](./type_defs.md#connectionaliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStandbyWorkspacesRequestRequestTypeDef

```python
# CreateStandbyWorkspacesRequestRequestTypeDef definition

class CreateStandbyWorkspacesRequestRequestTypeDef(TypedDict):
    PrimaryRegion: str,
    StandbyWorkspaces: Sequence[StandbyWorkspaceTypeDef],  # (1)
```

1. See [:material-code-braces: StandbyWorkspaceTypeDef](./type_defs.md#standbyworkspacetypedef) 
## FailedCreateStandbyWorkspacesRequestTypeDef

```python
# FailedCreateStandbyWorkspacesRequestTypeDef definition

class FailedCreateStandbyWorkspacesRequestTypeDef(TypedDict):
    StandbyWorkspaceRequest: NotRequired[StandbyWorkspaceTypeDef],  # (1)
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-braces: StandbyWorkspaceTypeDef](./type_defs.md#standbyworkspacetypedef) 
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceBundleTypeDef](./type_defs.md#workspacebundletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceDirectoriesResultTypeDef

```python
# DescribeWorkspaceDirectoriesResultTypeDef definition

class DescribeWorkspaceDirectoriesResultTypeDef(TypedDict):
    Directories: List[WorkspaceDirectoryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceDirectoryTypeDef](./type_defs.md#workspacedirectorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkspacesRequestRequestTypeDef

```python
# CreateWorkspacesRequestRequestTypeDef definition

class CreateWorkspacesRequestRequestTypeDef(TypedDict):
    Workspaces: Sequence[WorkspaceRequestTypeDef],  # (1)
```

1. See [:material-code-braces: WorkspaceRequestTypeDef](./type_defs.md#workspacerequesttypedef) 
## FailedCreateWorkspaceRequestTypeDef

```python
# FailedCreateWorkspaceRequestTypeDef definition

class FailedCreateWorkspaceRequestTypeDef(TypedDict):
    WorkspaceRequest: NotRequired[WorkspaceRequestTypeDef],  # (1)
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-braces: WorkspaceRequestTypeDef](./type_defs.md#workspacerequesttypedef) 
## DescribeWorkspacesResultTypeDef

```python
# DescribeWorkspacesResultTypeDef definition

class DescribeWorkspacesResultTypeDef(TypedDict):
    Workspaces: List[WorkspaceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceTypeDef](./type_defs.md#workspacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorkspaceImagesResultTypeDef

```python
# DescribeWorkspaceImagesResultTypeDef definition

class DescribeWorkspaceImagesResultTypeDef(TypedDict):
    Images: List[WorkspaceImageTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkspaceImageTypeDef](./type_defs.md#workspaceimagetypedef) 
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
