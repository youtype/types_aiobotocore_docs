# Type definitions

> [Index](../README.md) > [AppStream](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AppStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#appstream)
    type annotations stubs module [types-aiobotocore-appstream](https://pypi.org/project/types-aiobotocore-appstream/).

## StorageConnectorUnionTypeDef

```python
# StorageConnectorUnionTypeDef definition

StorageConnectorUnionTypeDef = Union[
    StorageConnectorTypeDef,  # (1)
    StorageConnectorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StorageConnectorTypeDef](./type_defs.md#storageconnectortypedef) 
2. See [:material-code-braces: StorageConnectorOutputTypeDef](./type_defs.md#storageconnectoroutputtypedef) 



## AccessEndpointTypeDef

```python
# AccessEndpointTypeDef definition

class AccessEndpointTypeDef(TypedDict):
    EndpointType: AccessEndpointTypeType,  # (1)
    VpceId: NotRequired[str],
```

1. See [:material-code-brackets: AccessEndpointTypeType](./literals.md#accessendpointtypetype) 
## AppBlockBuilderAppBlockAssociationTypeDef

```python
# AppBlockBuilderAppBlockAssociationTypeDef definition

class AppBlockBuilderAppBlockAssociationTypeDef(TypedDict):
    AppBlockArn: str,
    AppBlockBuilderName: str,
```

## AppBlockBuilderStateChangeReasonTypeDef

```python
# AppBlockBuilderStateChangeReasonTypeDef definition

class AppBlockBuilderStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[AppBlockBuilderStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: AppBlockBuilderStateChangeReasonCodeType](./literals.md#appblockbuilderstatechangereasoncodetype) 
## ResourceErrorTypeDef

```python
# ResourceErrorTypeDef definition

class ResourceErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[FleetErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
    ErrorTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: FleetErrorCodeType](./literals.md#fleeterrorcodetype) 
## VpcConfigOutputTypeDef

```python
# VpcConfigOutputTypeDef definition

class VpcConfigOutputTypeDef(TypedDict):
    SubnetIds: NotRequired[List[str]],
    SecurityGroupIds: NotRequired[List[str]],
```

## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    S3Bucket: str,
    S3Key: NotRequired[str],
```

## ApplicationFleetAssociationTypeDef

```python
# ApplicationFleetAssociationTypeDef definition

class ApplicationFleetAssociationTypeDef(TypedDict):
    FleetName: str,
    ApplicationArn: str,
```

## ApplicationSettingsResponseTypeDef

```python
# ApplicationSettingsResponseTypeDef definition

class ApplicationSettingsResponseTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    SettingsGroup: NotRequired[str],
    S3BucketName: NotRequired[str],
```

## ApplicationSettingsTypeDef

```python
# ApplicationSettingsTypeDef definition

class ApplicationSettingsTypeDef(TypedDict):
    Enabled: bool,
    SettingsGroup: NotRequired[str],
```

## AssociateAppBlockBuilderAppBlockRequestRequestTypeDef

```python
# AssociateAppBlockBuilderAppBlockRequestRequestTypeDef definition

class AssociateAppBlockBuilderAppBlockRequestRequestTypeDef(TypedDict):
    AppBlockArn: str,
    AppBlockBuilderName: str,
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

## AssociateApplicationFleetRequestRequestTypeDef

```python
# AssociateApplicationFleetRequestRequestTypeDef definition

class AssociateApplicationFleetRequestRequestTypeDef(TypedDict):
    FleetName: str,
    ApplicationArn: str,
```

## AssociateApplicationToEntitlementRequestRequestTypeDef

```python
# AssociateApplicationToEntitlementRequestRequestTypeDef definition

class AssociateApplicationToEntitlementRequestRequestTypeDef(TypedDict):
    StackName: str,
    EntitlementName: str,
    ApplicationIdentifier: str,
```

## AssociateFleetRequestRequestTypeDef

```python
# AssociateFleetRequestRequestTypeDef definition

class AssociateFleetRequestRequestTypeDef(TypedDict):
    FleetName: str,
    StackName: str,
```

## UserStackAssociationTypeDef

```python
# UserStackAssociationTypeDef definition

class UserStackAssociationTypeDef(TypedDict):
    StackName: str,
    UserName: str,
    AuthenticationType: AuthenticationTypeType,  # (1)
    SendEmailNotification: NotRequired[bool],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## CertificateBasedAuthPropertiesTypeDef

```python
# CertificateBasedAuthPropertiesTypeDef definition

class CertificateBasedAuthPropertiesTypeDef(TypedDict):
    Status: NotRequired[CertificateBasedAuthStatusType],  # (1)
    CertificateAuthorityArn: NotRequired[str],
```

1. See [:material-code-brackets: CertificateBasedAuthStatusType](./literals.md#certificatebasedauthstatustype) 
## ComputeCapacityStatusTypeDef

```python
# ComputeCapacityStatusTypeDef definition

class ComputeCapacityStatusTypeDef(TypedDict):
    Desired: int,
    Running: NotRequired[int],
    InUse: NotRequired[int],
    Available: NotRequired[int],
    DesiredUserSessions: NotRequired[int],
    AvailableUserSessions: NotRequired[int],
    ActiveUserSessions: NotRequired[int],
    ActualUserSessions: NotRequired[int],
```

## ComputeCapacityTypeDef

```python
# ComputeCapacityTypeDef definition

class ComputeCapacityTypeDef(TypedDict):
    DesiredInstances: NotRequired[int],
    DesiredSessions: NotRequired[int],
```

## CopyImageRequestRequestTypeDef

```python
# CopyImageRequestRequestTypeDef definition

class CopyImageRequestRequestTypeDef(TypedDict):
    SourceImageName: str,
    DestinationImageName: str,
    DestinationRegion: str,
    DestinationImageDescription: NotRequired[str],
```

## VpcConfigTypeDef

```python
# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    SubnetIds: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
```

## CreateAppBlockBuilderStreamingURLRequestRequestTypeDef

```python
# CreateAppBlockBuilderStreamingURLRequestRequestTypeDef definition

class CreateAppBlockBuilderStreamingURLRequestRequestTypeDef(TypedDict):
    AppBlockBuilderName: str,
    Validity: NotRequired[int],
```

## ServiceAccountCredentialsTypeDef

```python
# ServiceAccountCredentialsTypeDef definition

class ServiceAccountCredentialsTypeDef(TypedDict):
    AccountName: str,
    AccountPassword: str,
```

## EntitlementAttributeTypeDef

```python
# EntitlementAttributeTypeDef definition

class EntitlementAttributeTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## DomainJoinInfoTypeDef

```python
# DomainJoinInfoTypeDef definition

class DomainJoinInfoTypeDef(TypedDict):
    DirectoryName: NotRequired[str],
    OrganizationalUnitDistinguishedName: NotRequired[str],
```

## CreateImageBuilderStreamingURLRequestRequestTypeDef

```python
# CreateImageBuilderStreamingURLRequestRequestTypeDef definition

class CreateImageBuilderStreamingURLRequestRequestTypeDef(TypedDict):
    Name: str,
    Validity: NotRequired[int],
```

## StreamingExperienceSettingsTypeDef

```python
# StreamingExperienceSettingsTypeDef definition

class StreamingExperienceSettingsTypeDef(TypedDict):
    PreferredProtocol: NotRequired[PreferredProtocolType],  # (1)
```

1. See [:material-code-brackets: PreferredProtocolType](./literals.md#preferredprotocoltype) 
## UserSettingTypeDef

```python
# UserSettingTypeDef definition

class UserSettingTypeDef(TypedDict):
    Action: ActionType,  # (1)
    Permission: PermissionType,  # (2)
    MaximumLength: NotRequired[int],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## CreateStreamingURLRequestRequestTypeDef

```python
# CreateStreamingURLRequestRequestTypeDef definition

class CreateStreamingURLRequestRequestTypeDef(TypedDict):
    StackName: str,
    FleetName: str,
    UserId: str,
    ApplicationId: NotRequired[str],
    Validity: NotRequired[int],
    SessionContext: NotRequired[str],
```

## ThemeFooterLinkTypeDef

```python
# ThemeFooterLinkTypeDef definition

class ThemeFooterLinkTypeDef(TypedDict):
    DisplayName: NotRequired[str],
    FooterLinkURL: NotRequired[str],
```

## CreateUpdatedImageRequestRequestTypeDef

```python
# CreateUpdatedImageRequestRequestTypeDef definition

class CreateUpdatedImageRequestRequestTypeDef(TypedDict):
    existingImageName: str,
    newImageName: str,
    newImageDescription: NotRequired[str],
    newImageDisplayName: NotRequired[str],
    newImageTags: NotRequired[Mapping[str, str]],
    dryRun: NotRequired[bool],
```

## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    AuthenticationType: AuthenticationTypeType,  # (1)
    MessageAction: NotRequired[MessageActionType],  # (2)
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-brackets: MessageActionType](./literals.md#messageactiontype) 
## DeleteAppBlockBuilderRequestRequestTypeDef

```python
# DeleteAppBlockBuilderRequestRequestTypeDef definition

class DeleteAppBlockBuilderRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteAppBlockRequestRequestTypeDef

```python
# DeleteAppBlockRequestRequestTypeDef definition

class DeleteAppBlockRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteDirectoryConfigRequestRequestTypeDef

```python
# DeleteDirectoryConfigRequestRequestTypeDef definition

class DeleteDirectoryConfigRequestRequestTypeDef(TypedDict):
    DirectoryName: str,
```

## DeleteEntitlementRequestRequestTypeDef

```python
# DeleteEntitlementRequestRequestTypeDef definition

class DeleteEntitlementRequestRequestTypeDef(TypedDict):
    Name: str,
    StackName: str,
```

## DeleteFleetRequestRequestTypeDef

```python
# DeleteFleetRequestRequestTypeDef definition

class DeleteFleetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteImageBuilderRequestRequestTypeDef

```python
# DeleteImageBuilderRequestRequestTypeDef definition

class DeleteImageBuilderRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteImagePermissionsRequestRequestTypeDef

```python
# DeleteImagePermissionsRequestRequestTypeDef definition

class DeleteImagePermissionsRequestRequestTypeDef(TypedDict):
    Name: str,
    SharedAccountId: str,
```

## DeleteImageRequestRequestTypeDef

```python
# DeleteImageRequestRequestTypeDef definition

class DeleteImageRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteStackRequestRequestTypeDef

```python
# DeleteStackRequestRequestTypeDef definition

class DeleteStackRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteThemeForStackRequestRequestTypeDef

```python
# DeleteThemeForStackRequestRequestTypeDef definition

class DeleteThemeForStackRequestRequestTypeDef(TypedDict):
    StackName: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    AuthenticationType: AuthenticationTypeType,  # (1)
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef

```python
# DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef definition

class DescribeAppBlockBuilderAppBlockAssociationsRequestRequestTypeDef(TypedDict):
    AppBlockArn: NotRequired[str],
    AppBlockBuilderName: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeAppBlockBuildersRequestRequestTypeDef

```python
# DescribeAppBlockBuildersRequestRequestTypeDef definition

class DescribeAppBlockBuildersRequestRequestTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeAppBlocksRequestRequestTypeDef

```python
# DescribeAppBlocksRequestRequestTypeDef definition

class DescribeAppBlocksRequestRequestTypeDef(TypedDict):
    Arns: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeApplicationFleetAssociationsRequestRequestTypeDef

```python
# DescribeApplicationFleetAssociationsRequestRequestTypeDef definition

class DescribeApplicationFleetAssociationsRequestRequestTypeDef(TypedDict):
    FleetName: NotRequired[str],
    ApplicationArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeApplicationsRequestRequestTypeDef

```python
# DescribeApplicationsRequestRequestTypeDef definition

class DescribeApplicationsRequestRequestTypeDef(TypedDict):
    Arns: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeDirectoryConfigsRequestRequestTypeDef

```python
# DescribeDirectoryConfigsRequestRequestTypeDef definition

class DescribeDirectoryConfigsRequestRequestTypeDef(TypedDict):
    DirectoryNames: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeEntitlementsRequestRequestTypeDef

```python
# DescribeEntitlementsRequestRequestTypeDef definition

class DescribeEntitlementsRequestRequestTypeDef(TypedDict):
    StackName: str,
    Name: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeFleetsRequestRequestTypeDef

```python
# DescribeFleetsRequestRequestTypeDef definition

class DescribeFleetsRequestRequestTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeImageBuildersRequestRequestTypeDef

```python
# DescribeImageBuildersRequestRequestTypeDef definition

class DescribeImageBuildersRequestRequestTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeImagePermissionsRequestRequestTypeDef

```python
# DescribeImagePermissionsRequestRequestTypeDef definition

class DescribeImagePermissionsRequestRequestTypeDef(TypedDict):
    Name: str,
    MaxResults: NotRequired[int],
    SharedAwsAccountIds: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
```

## DescribeImagesRequestRequestTypeDef

```python
# DescribeImagesRequestRequestTypeDef definition

class DescribeImagesRequestRequestTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    Arns: NotRequired[Sequence[str]],
    Type: NotRequired[VisibilityTypeType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: VisibilityTypeType](./literals.md#visibilitytypetype) 
## DescribeSessionsRequestRequestTypeDef

```python
# DescribeSessionsRequestRequestTypeDef definition

class DescribeSessionsRequestRequestTypeDef(TypedDict):
    StackName: str,
    FleetName: str,
    UserId: NotRequired[str],
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
    AuthenticationType: NotRequired[AuthenticationTypeType],  # (1)
    InstanceId: NotRequired[str],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## DescribeStacksRequestRequestTypeDef

```python
# DescribeStacksRequestRequestTypeDef definition

class DescribeStacksRequestRequestTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
```

## DescribeThemeForStackRequestRequestTypeDef

```python
# DescribeThemeForStackRequestRequestTypeDef definition

class DescribeThemeForStackRequestRequestTypeDef(TypedDict):
    StackName: str,
```

## DescribeUsageReportSubscriptionsRequestRequestTypeDef

```python
# DescribeUsageReportSubscriptionsRequestRequestTypeDef definition

class DescribeUsageReportSubscriptionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeUserStackAssociationsRequestRequestTypeDef

```python
# DescribeUserStackAssociationsRequestRequestTypeDef definition

class DescribeUserStackAssociationsRequestRequestTypeDef(TypedDict):
    StackName: NotRequired[str],
    UserName: NotRequired[str],
    AuthenticationType: NotRequired[AuthenticationTypeType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## DescribeUsersRequestRequestTypeDef

```python
# DescribeUsersRequestRequestTypeDef definition

class DescribeUsersRequestRequestTypeDef(TypedDict):
    AuthenticationType: AuthenticationTypeType,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    AuthenticationType: AuthenticationTypeType,  # (1)
    Arn: NotRequired[str],
    UserName: NotRequired[str],
    Enabled: NotRequired[bool],
    Status: NotRequired[str],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## DisableUserRequestRequestTypeDef

```python
# DisableUserRequestRequestTypeDef definition

class DisableUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    AuthenticationType: AuthenticationTypeType,  # (1)
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef

```python
# DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef definition

class DisassociateAppBlockBuilderAppBlockRequestRequestTypeDef(TypedDict):
    AppBlockArn: str,
    AppBlockBuilderName: str,
```

## DisassociateApplicationFleetRequestRequestTypeDef

```python
# DisassociateApplicationFleetRequestRequestTypeDef definition

class DisassociateApplicationFleetRequestRequestTypeDef(TypedDict):
    FleetName: str,
    ApplicationArn: str,
```

## DisassociateApplicationFromEntitlementRequestRequestTypeDef

```python
# DisassociateApplicationFromEntitlementRequestRequestTypeDef definition

class DisassociateApplicationFromEntitlementRequestRequestTypeDef(TypedDict):
    StackName: str,
    EntitlementName: str,
    ApplicationIdentifier: str,
```

## DisassociateFleetRequestRequestTypeDef

```python
# DisassociateFleetRequestRequestTypeDef definition

class DisassociateFleetRequestRequestTypeDef(TypedDict):
    FleetName: str,
    StackName: str,
```

## EnableUserRequestRequestTypeDef

```python
# EnableUserRequestRequestTypeDef definition

class EnableUserRequestRequestTypeDef(TypedDict):
    UserName: str,
    AuthenticationType: AuthenticationTypeType,  # (1)
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## EntitledApplicationTypeDef

```python
# EntitledApplicationTypeDef definition

class EntitledApplicationTypeDef(TypedDict):
    ApplicationIdentifier: str,
```

## ExpireSessionRequestRequestTypeDef

```python
# ExpireSessionRequestRequestTypeDef definition

class ExpireSessionRequestRequestTypeDef(TypedDict):
    SessionId: str,
```

## FleetErrorTypeDef

```python
# FleetErrorTypeDef definition

class FleetErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[FleetErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: FleetErrorCodeType](./literals.md#fleeterrorcodetype) 
## ImageBuilderStateChangeReasonTypeDef

```python
# ImageBuilderStateChangeReasonTypeDef definition

class ImageBuilderStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[ImageBuilderStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: ImageBuilderStateChangeReasonCodeType](./literals.md#imagebuilderstatechangereasoncodetype) 
## NetworkAccessConfigurationTypeDef

```python
# NetworkAccessConfigurationTypeDef definition

class NetworkAccessConfigurationTypeDef(TypedDict):
    EniPrivateIpAddress: NotRequired[str],
    EniId: NotRequired[str],
```

## ImagePermissionsTypeDef

```python
# ImagePermissionsTypeDef definition

class ImagePermissionsTypeDef(TypedDict):
    allowFleet: NotRequired[bool],
    allowImageBuilder: NotRequired[bool],
```

## ImageStateChangeReasonTypeDef

```python
# ImageStateChangeReasonTypeDef definition

class ImageStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[ImageStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: ImageStateChangeReasonCodeType](./literals.md#imagestatechangereasoncodetype) 
## LastReportGenerationExecutionErrorTypeDef

```python
# LastReportGenerationExecutionErrorTypeDef definition

class LastReportGenerationExecutionErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[UsageReportExecutionErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: UsageReportExecutionErrorCodeType](./literals.md#usagereportexecutionerrorcodetype) 
## ListAssociatedFleetsRequestRequestTypeDef

```python
# ListAssociatedFleetsRequestRequestTypeDef definition

class ListAssociatedFleetsRequestRequestTypeDef(TypedDict):
    StackName: str,
    NextToken: NotRequired[str],
```

## ListAssociatedStacksRequestRequestTypeDef

```python
# ListAssociatedStacksRequestRequestTypeDef definition

class ListAssociatedStacksRequestRequestTypeDef(TypedDict):
    FleetName: str,
    NextToken: NotRequired[str],
```

## ListEntitledApplicationsRequestRequestTypeDef

```python
# ListEntitledApplicationsRequestRequestTypeDef definition

class ListEntitledApplicationsRequestRequestTypeDef(TypedDict):
    StackName: str,
    EntitlementName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## StackErrorTypeDef

```python
# StackErrorTypeDef definition

class StackErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[StackErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: StackErrorCodeType](./literals.md#stackerrorcodetype) 
## StorageConnectorOutputTypeDef

```python
# StorageConnectorOutputTypeDef definition

class StorageConnectorOutputTypeDef(TypedDict):
    ConnectorType: StorageConnectorTypeType,  # (1)
    ResourceIdentifier: NotRequired[str],
    Domains: NotRequired[List[str]],
```

1. See [:material-code-brackets: StorageConnectorTypeType](./literals.md#storageconnectortypetype) 
## StartAppBlockBuilderRequestRequestTypeDef

```python
# StartAppBlockBuilderRequestRequestTypeDef definition

class StartAppBlockBuilderRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StartFleetRequestRequestTypeDef

```python
# StartFleetRequestRequestTypeDef definition

class StartFleetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StartImageBuilderRequestRequestTypeDef

```python
# StartImageBuilderRequestRequestTypeDef definition

class StartImageBuilderRequestRequestTypeDef(TypedDict):
    Name: str,
    AppstreamAgentVersion: NotRequired[str],
```

## StopAppBlockBuilderRequestRequestTypeDef

```python
# StopAppBlockBuilderRequestRequestTypeDef definition

class StopAppBlockBuilderRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StopFleetRequestRequestTypeDef

```python
# StopFleetRequestRequestTypeDef definition

class StopFleetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StopImageBuilderRequestRequestTypeDef

```python
# StopImageBuilderRequestRequestTypeDef definition

class StopImageBuilderRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StorageConnectorTypeDef

```python
# StorageConnectorTypeDef definition

class StorageConnectorTypeDef(TypedDict):
    ConnectorType: StorageConnectorTypeType,  # (1)
    ResourceIdentifier: NotRequired[str],
    Domains: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: StorageConnectorTypeType](./literals.md#storageconnectortypetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## AppBlockBuilderTypeDef

```python
# AppBlockBuilderTypeDef definition

class AppBlockBuilderTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Platform: AppBlockBuilderPlatformTypeType,  # (1)
    InstanceType: str,
    VpcConfig: VpcConfigOutputTypeDef,  # (2)
    State: AppBlockBuilderStateType,  # (3)
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    EnableDefaultInternetAccess: NotRequired[bool],
    IamRoleArn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    AppBlockBuilderErrors: NotRequired[List[ResourceErrorTypeDef]],  # (4)
    StateChangeReason: NotRequired[AppBlockBuilderStateChangeReasonTypeDef],  # (5)
    AccessEndpoints: NotRequired[List[AccessEndpointTypeDef]],  # (6)
```

1. See [:material-code-brackets: AppBlockBuilderPlatformTypeType](./literals.md#appblockbuilderplatformtypetype) 
2. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
3. See [:material-code-brackets: AppBlockBuilderStateType](./literals.md#appblockbuilderstatetype) 
4. See [:material-code-braces: ResourceErrorTypeDef](./type_defs.md#resourceerrortypedef) 
5. See [:material-code-braces: AppBlockBuilderStateChangeReasonTypeDef](./type_defs.md#appblockbuilderstatechangereasontypedef) 
6. See [:material-code-braces: AccessEndpointTypeDef](./type_defs.md#accessendpointtypedef) 
## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    Name: NotRequired[str],
    DisplayName: NotRequired[str],
    IconURL: NotRequired[str],
    LaunchPath: NotRequired[str],
    LaunchParameters: NotRequired[str],
    Enabled: NotRequired[bool],
    Metadata: NotRequired[Dict[str, str]],
    WorkingDirectory: NotRequired[str],
    Description: NotRequired[str],
    Arn: NotRequired[str],
    AppBlockArn: NotRequired[str],
    IconS3Location: NotRequired[S3LocationTypeDef],  # (1)
    Platforms: NotRequired[List[PlatformTypeType]],  # (2)
    InstanceFamilies: NotRequired[List[str]],
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    Name: str,
    IconS3Location: S3LocationTypeDef,  # (1)
    LaunchPath: str,
    Platforms: Sequence[PlatformTypeType],  # (2)
    InstanceFamilies: Sequence[str],
    AppBlockArn: str,
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    WorkingDirectory: NotRequired[str],
    LaunchParameters: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
## ScriptDetailsTypeDef

```python
# ScriptDetailsTypeDef definition

class ScriptDetailsTypeDef(TypedDict):
    ScriptS3Location: S3LocationTypeDef,  # (1)
    ExecutablePath: str,
    TimeoutInSeconds: int,
    ExecutableParameters: NotRequired[str],
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    Name: str,
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    IconS3Location: NotRequired[S3LocationTypeDef],  # (1)
    LaunchPath: NotRequired[str],
    WorkingDirectory: NotRequired[str],
    LaunchParameters: NotRequired[str],
    AppBlockArn: NotRequired[str],
    AttributesToDelete: NotRequired[Sequence[ApplicationAttributeType]],  # (2)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-brackets: ApplicationAttributeType](./literals.md#applicationattributetype) 
## AssociateAppBlockBuilderAppBlockResultTypeDef

```python
# AssociateAppBlockBuilderAppBlockResultTypeDef definition

class AssociateAppBlockBuilderAppBlockResultTypeDef(TypedDict):
    AppBlockBuilderAppBlockAssociation: AppBlockBuilderAppBlockAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppBlockBuilderAppBlockAssociationTypeDef](./type_defs.md#appblockbuilderappblockassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateApplicationFleetResultTypeDef

```python
# AssociateApplicationFleetResultTypeDef definition

class AssociateApplicationFleetResultTypeDef(TypedDict):
    ApplicationFleetAssociation: ApplicationFleetAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationFleetAssociationTypeDef](./type_defs.md#applicationfleetassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyImageResponseTypeDef

```python
# CopyImageResponseTypeDef definition

class CopyImageResponseTypeDef(TypedDict):
    DestinationImageName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppBlockBuilderStreamingURLResultTypeDef

```python
# CreateAppBlockBuilderStreamingURLResultTypeDef definition

class CreateAppBlockBuilderStreamingURLResultTypeDef(TypedDict):
    StreamingURL: str,
    Expires: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateImageBuilderStreamingURLResultTypeDef

```python
# CreateImageBuilderStreamingURLResultTypeDef definition

class CreateImageBuilderStreamingURLResultTypeDef(TypedDict):
    StreamingURL: str,
    Expires: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStreamingURLResultTypeDef

```python
# CreateStreamingURLResultTypeDef definition

class CreateStreamingURLResultTypeDef(TypedDict):
    StreamingURL: str,
    Expires: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUsageReportSubscriptionResultTypeDef

```python
# CreateUsageReportSubscriptionResultTypeDef definition

class CreateUsageReportSubscriptionResultTypeDef(TypedDict):
    S3BucketName: str,
    Schedule: UsageReportScheduleType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: UsageReportScheduleType](./literals.md#usagereportscheduletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef

```python
# DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef definition

class DescribeAppBlockBuilderAppBlockAssociationsResultTypeDef(TypedDict):
    AppBlockBuilderAppBlockAssociations: List[AppBlockBuilderAppBlockAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AppBlockBuilderAppBlockAssociationTypeDef](./type_defs.md#appblockbuilderappblockassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicationFleetAssociationsResultTypeDef

```python
# DescribeApplicationFleetAssociationsResultTypeDef definition

class DescribeApplicationFleetAssociationsResultTypeDef(TypedDict):
    ApplicationFleetAssociations: List[ApplicationFleetAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationFleetAssociationTypeDef](./type_defs.md#applicationfleetassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssociatedFleetsResultTypeDef

```python
# ListAssociatedFleetsResultTypeDef definition

class ListAssociatedFleetsResultTypeDef(TypedDict):
    Names: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssociatedStacksResultTypeDef

```python
# ListAssociatedStacksResultTypeDef definition

class ListAssociatedStacksResultTypeDef(TypedDict):
    Names: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchAssociateUserStackRequestRequestTypeDef

```python
# BatchAssociateUserStackRequestRequestTypeDef definition

class BatchAssociateUserStackRequestRequestTypeDef(TypedDict):
    UserStackAssociations: Sequence[UserStackAssociationTypeDef],  # (1)
```

1. See [:material-code-braces: UserStackAssociationTypeDef](./type_defs.md#userstackassociationtypedef) 
## BatchDisassociateUserStackRequestRequestTypeDef

```python
# BatchDisassociateUserStackRequestRequestTypeDef definition

class BatchDisassociateUserStackRequestRequestTypeDef(TypedDict):
    UserStackAssociations: Sequence[UserStackAssociationTypeDef],  # (1)
```

1. See [:material-code-braces: UserStackAssociationTypeDef](./type_defs.md#userstackassociationtypedef) 
## DescribeUserStackAssociationsResultTypeDef

```python
# DescribeUserStackAssociationsResultTypeDef definition

class DescribeUserStackAssociationsResultTypeDef(TypedDict):
    UserStackAssociations: List[UserStackAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserStackAssociationTypeDef](./type_defs.md#userstackassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UserStackAssociationErrorTypeDef

```python
# UserStackAssociationErrorTypeDef definition

class UserStackAssociationErrorTypeDef(TypedDict):
    UserStackAssociation: NotRequired[UserStackAssociationTypeDef],  # (1)
    ErrorCode: NotRequired[UserStackAssociationErrorCodeType],  # (2)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-braces: UserStackAssociationTypeDef](./type_defs.md#userstackassociationtypedef) 
2. See [:material-code-brackets: UserStackAssociationErrorCodeType](./literals.md#userstackassociationerrorcodetype) 
## CreateAppBlockBuilderRequestRequestTypeDef

```python
# CreateAppBlockBuilderRequestRequestTypeDef definition

class CreateAppBlockBuilderRequestRequestTypeDef(TypedDict):
    Name: str,
    Platform: AppBlockBuilderPlatformTypeType,  # (1)
    InstanceType: str,
    VpcConfig: VpcConfigTypeDef,  # (2)
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    EnableDefaultInternetAccess: NotRequired[bool],
    IamRoleArn: NotRequired[str],
    AccessEndpoints: NotRequired[Sequence[AccessEndpointTypeDef]],  # (3)
```

1. See [:material-code-brackets: AppBlockBuilderPlatformTypeType](./literals.md#appblockbuilderplatformtypetype) 
2. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
3. See [:material-code-braces: AccessEndpointTypeDef](./type_defs.md#accessendpointtypedef) 
## UpdateAppBlockBuilderRequestRequestTypeDef

```python
# UpdateAppBlockBuilderRequestRequestTypeDef definition

class UpdateAppBlockBuilderRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    Platform: NotRequired[PlatformTypeType],  # (1)
    InstanceType: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (2)
    EnableDefaultInternetAccess: NotRequired[bool],
    IamRoleArn: NotRequired[str],
    AccessEndpoints: NotRequired[Sequence[AccessEndpointTypeDef]],  # (3)
    AttributesToDelete: NotRequired[Sequence[AppBlockBuilderAttributeType]],  # (4)
```

1. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
2. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
3. See [:material-code-braces: AccessEndpointTypeDef](./type_defs.md#accessendpointtypedef) 
4. See [:material-code-brackets: AppBlockBuilderAttributeType](./literals.md#appblockbuilderattributetype) 
## CreateDirectoryConfigRequestRequestTypeDef

```python
# CreateDirectoryConfigRequestRequestTypeDef definition

class CreateDirectoryConfigRequestRequestTypeDef(TypedDict):
    DirectoryName: str,
    OrganizationalUnitDistinguishedNames: Sequence[str],
    ServiceAccountCredentials: NotRequired[ServiceAccountCredentialsTypeDef],  # (1)
    CertificateBasedAuthProperties: NotRequired[CertificateBasedAuthPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: ServiceAccountCredentialsTypeDef](./type_defs.md#serviceaccountcredentialstypedef) 
2. See [:material-code-braces: CertificateBasedAuthPropertiesTypeDef](./type_defs.md#certificatebasedauthpropertiestypedef) 
## DirectoryConfigTypeDef

```python
# DirectoryConfigTypeDef definition

class DirectoryConfigTypeDef(TypedDict):
    DirectoryName: str,
    OrganizationalUnitDistinguishedNames: NotRequired[List[str]],
    ServiceAccountCredentials: NotRequired[ServiceAccountCredentialsTypeDef],  # (1)
    CreatedTime: NotRequired[datetime],
    CertificateBasedAuthProperties: NotRequired[CertificateBasedAuthPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: ServiceAccountCredentialsTypeDef](./type_defs.md#serviceaccountcredentialstypedef) 
2. See [:material-code-braces: CertificateBasedAuthPropertiesTypeDef](./type_defs.md#certificatebasedauthpropertiestypedef) 
## UpdateDirectoryConfigRequestRequestTypeDef

```python
# UpdateDirectoryConfigRequestRequestTypeDef definition

class UpdateDirectoryConfigRequestRequestTypeDef(TypedDict):
    DirectoryName: str,
    OrganizationalUnitDistinguishedNames: NotRequired[Sequence[str]],
    ServiceAccountCredentials: NotRequired[ServiceAccountCredentialsTypeDef],  # (1)
    CertificateBasedAuthProperties: NotRequired[CertificateBasedAuthPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: ServiceAccountCredentialsTypeDef](./type_defs.md#serviceaccountcredentialstypedef) 
2. See [:material-code-braces: CertificateBasedAuthPropertiesTypeDef](./type_defs.md#certificatebasedauthpropertiestypedef) 
## CreateEntitlementRequestRequestTypeDef

```python
# CreateEntitlementRequestRequestTypeDef definition

class CreateEntitlementRequestRequestTypeDef(TypedDict):
    Name: str,
    StackName: str,
    AppVisibility: AppVisibilityType,  # (1)
    Attributes: Sequence[EntitlementAttributeTypeDef],  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: AppVisibilityType](./literals.md#appvisibilitytype) 
2. See [:material-code-braces: EntitlementAttributeTypeDef](./type_defs.md#entitlementattributetypedef) 
## EntitlementTypeDef

```python
# EntitlementTypeDef definition

class EntitlementTypeDef(TypedDict):
    Name: str,
    StackName: str,
    AppVisibility: AppVisibilityType,  # (1)
    Attributes: List[EntitlementAttributeTypeDef],  # (2)
    Description: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: AppVisibilityType](./literals.md#appvisibilitytype) 
2. See [:material-code-braces: EntitlementAttributeTypeDef](./type_defs.md#entitlementattributetypedef) 
## UpdateEntitlementRequestRequestTypeDef

```python
# UpdateEntitlementRequestRequestTypeDef definition

class UpdateEntitlementRequestRequestTypeDef(TypedDict):
    Name: str,
    StackName: str,
    Description: NotRequired[str],
    AppVisibility: NotRequired[AppVisibilityType],  # (1)
    Attributes: NotRequired[Sequence[EntitlementAttributeTypeDef]],  # (2)
```

1. See [:material-code-brackets: AppVisibilityType](./literals.md#appvisibilitytype) 
2. See [:material-code-braces: EntitlementAttributeTypeDef](./type_defs.md#entitlementattributetypedef) 
## CreateFleetRequestRequestTypeDef

```python
# CreateFleetRequestRequestTypeDef definition

class CreateFleetRequestRequestTypeDef(TypedDict):
    Name: str,
    InstanceType: str,
    ImageName: NotRequired[str],
    ImageArn: NotRequired[str],
    FleetType: NotRequired[FleetTypeType],  # (1)
    ComputeCapacity: NotRequired[ComputeCapacityTypeDef],  # (2)
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (3)
    MaxUserDurationInSeconds: NotRequired[int],
    DisconnectTimeoutInSeconds: NotRequired[int],
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    EnableDefaultInternetAccess: NotRequired[bool],
    DomainJoinInfo: NotRequired[DomainJoinInfoTypeDef],  # (4)
    Tags: NotRequired[Mapping[str, str]],
    IdleDisconnectTimeoutInSeconds: NotRequired[int],
    IamRoleArn: NotRequired[str],
    StreamView: NotRequired[StreamViewType],  # (5)
    Platform: NotRequired[PlatformTypeType],  # (6)
    MaxConcurrentSessions: NotRequired[int],
    UsbDeviceFilterStrings: NotRequired[Sequence[str]],
    SessionScriptS3Location: NotRequired[S3LocationTypeDef],  # (7)
    MaxSessionsPerInstance: NotRequired[int],
```

1. See [:material-code-brackets: FleetTypeType](./literals.md#fleettypetype) 
2. See [:material-code-braces: ComputeCapacityTypeDef](./type_defs.md#computecapacitytypedef) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
4. See [:material-code-braces: DomainJoinInfoTypeDef](./type_defs.md#domainjoininfotypedef) 
5. See [:material-code-brackets: StreamViewType](./literals.md#streamviewtype) 
6. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
7. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## CreateImageBuilderRequestRequestTypeDef

```python
# CreateImageBuilderRequestRequestTypeDef definition

class CreateImageBuilderRequestRequestTypeDef(TypedDict):
    Name: str,
    InstanceType: str,
    ImageName: NotRequired[str],
    ImageArn: NotRequired[str],
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (1)
    IamRoleArn: NotRequired[str],
    EnableDefaultInternetAccess: NotRequired[bool],
    DomainJoinInfo: NotRequired[DomainJoinInfoTypeDef],  # (2)
    AppstreamAgentVersion: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    AccessEndpoints: NotRequired[Sequence[AccessEndpointTypeDef]],  # (3)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
2. See [:material-code-braces: DomainJoinInfoTypeDef](./type_defs.md#domainjoininfotypedef) 
3. See [:material-code-braces: AccessEndpointTypeDef](./type_defs.md#accessendpointtypedef) 
## UpdateFleetRequestRequestTypeDef

```python
# UpdateFleetRequestRequestTypeDef definition

class UpdateFleetRequestRequestTypeDef(TypedDict):
    ImageName: NotRequired[str],
    ImageArn: NotRequired[str],
    Name: NotRequired[str],
    InstanceType: NotRequired[str],
    ComputeCapacity: NotRequired[ComputeCapacityTypeDef],  # (1)
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (2)
    MaxUserDurationInSeconds: NotRequired[int],
    DisconnectTimeoutInSeconds: NotRequired[int],
    DeleteVpcConfig: NotRequired[bool],
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    EnableDefaultInternetAccess: NotRequired[bool],
    DomainJoinInfo: NotRequired[DomainJoinInfoTypeDef],  # (3)
    IdleDisconnectTimeoutInSeconds: NotRequired[int],
    AttributesToDelete: NotRequired[Sequence[FleetAttributeType]],  # (4)
    IamRoleArn: NotRequired[str],
    StreamView: NotRequired[StreamViewType],  # (5)
    Platform: NotRequired[PlatformTypeType],  # (6)
    MaxConcurrentSessions: NotRequired[int],
    UsbDeviceFilterStrings: NotRequired[Sequence[str]],
    SessionScriptS3Location: NotRequired[S3LocationTypeDef],  # (7)
    MaxSessionsPerInstance: NotRequired[int],
```

1. See [:material-code-braces: ComputeCapacityTypeDef](./type_defs.md#computecapacitytypedef) 
2. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
3. See [:material-code-braces: DomainJoinInfoTypeDef](./type_defs.md#domainjoininfotypedef) 
4. See [:material-code-brackets: FleetAttributeType](./literals.md#fleetattributetype) 
5. See [:material-code-brackets: StreamViewType](./literals.md#streamviewtype) 
6. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
7. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## CreateThemeForStackRequestRequestTypeDef

```python
# CreateThemeForStackRequestRequestTypeDef definition

class CreateThemeForStackRequestRequestTypeDef(TypedDict):
    StackName: str,
    TitleText: str,
    ThemeStyling: ThemeStylingType,  # (1)
    OrganizationLogoS3Location: S3LocationTypeDef,  # (2)
    FaviconS3Location: S3LocationTypeDef,  # (2)
    FooterLinks: NotRequired[Sequence[ThemeFooterLinkTypeDef]],  # (4)
```

1. See [:material-code-brackets: ThemeStylingType](./literals.md#themestylingtype) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: ThemeFooterLinkTypeDef](./type_defs.md#themefooterlinktypedef) 
## ThemeTypeDef

```python
# ThemeTypeDef definition

class ThemeTypeDef(TypedDict):
    StackName: NotRequired[str],
    State: NotRequired[ThemeStateType],  # (1)
    ThemeTitleText: NotRequired[str],
    ThemeStyling: NotRequired[ThemeStylingType],  # (2)
    ThemeFooterLinks: NotRequired[List[ThemeFooterLinkTypeDef]],  # (3)
    ThemeOrganizationLogoURL: NotRequired[str],
    ThemeFaviconURL: NotRequired[str],
    CreatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ThemeStateType](./literals.md#themestatetype) 
2. See [:material-code-brackets: ThemeStylingType](./literals.md#themestylingtype) 
3. See [:material-code-braces: ThemeFooterLinkTypeDef](./type_defs.md#themefooterlinktypedef) 
## UpdateThemeForStackRequestRequestTypeDef

```python
# UpdateThemeForStackRequestRequestTypeDef definition

class UpdateThemeForStackRequestRequestTypeDef(TypedDict):
    StackName: str,
    FooterLinks: NotRequired[Sequence[ThemeFooterLinkTypeDef]],  # (1)
    TitleText: NotRequired[str],
    ThemeStyling: NotRequired[ThemeStylingType],  # (2)
    OrganizationLogoS3Location: NotRequired[S3LocationTypeDef],  # (3)
    FaviconS3Location: NotRequired[S3LocationTypeDef],  # (3)
    State: NotRequired[ThemeStateType],  # (5)
    AttributesToDelete: NotRequired[Sequence[ThemeAttributeType]],  # (6)
```

1. See [:material-code-braces: ThemeFooterLinkTypeDef](./type_defs.md#themefooterlinktypedef) 
2. See [:material-code-brackets: ThemeStylingType](./literals.md#themestylingtype) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
5. See [:material-code-brackets: ThemeStateType](./literals.md#themestatetype) 
6. See [:material-code-brackets: ThemeAttributeType](./literals.md#themeattributetype) 
## DescribeDirectoryConfigsRequestPaginateTypeDef

```python
# DescribeDirectoryConfigsRequestPaginateTypeDef definition

class DescribeDirectoryConfigsRequestPaginateTypeDef(TypedDict):
    DirectoryNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeFleetsRequestPaginateTypeDef

```python
# DescribeFleetsRequestPaginateTypeDef definition

class DescribeFleetsRequestPaginateTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeImageBuildersRequestPaginateTypeDef

```python
# DescribeImageBuildersRequestPaginateTypeDef definition

class DescribeImageBuildersRequestPaginateTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeImagesRequestPaginateTypeDef

```python
# DescribeImagesRequestPaginateTypeDef definition

class DescribeImagesRequestPaginateTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    Arns: NotRequired[Sequence[str]],
    Type: NotRequired[VisibilityTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: VisibilityTypeType](./literals.md#visibilitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeSessionsRequestPaginateTypeDef

```python
# DescribeSessionsRequestPaginateTypeDef definition

class DescribeSessionsRequestPaginateTypeDef(TypedDict):
    StackName: str,
    FleetName: str,
    UserId: NotRequired[str],
    AuthenticationType: NotRequired[AuthenticationTypeType],  # (1)
    InstanceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeStacksRequestPaginateTypeDef

```python
# DescribeStacksRequestPaginateTypeDef definition

class DescribeStacksRequestPaginateTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeUserStackAssociationsRequestPaginateTypeDef

```python
# DescribeUserStackAssociationsRequestPaginateTypeDef definition

class DescribeUserStackAssociationsRequestPaginateTypeDef(TypedDict):
    StackName: NotRequired[str],
    UserName: NotRequired[str],
    AuthenticationType: NotRequired[AuthenticationTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeUsersRequestPaginateTypeDef

```python
# DescribeUsersRequestPaginateTypeDef definition

class DescribeUsersRequestPaginateTypeDef(TypedDict):
    AuthenticationType: AuthenticationTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociatedFleetsRequestPaginateTypeDef

```python
# ListAssociatedFleetsRequestPaginateTypeDef definition

class ListAssociatedFleetsRequestPaginateTypeDef(TypedDict):
    StackName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociatedStacksRequestPaginateTypeDef

```python
# ListAssociatedStacksRequestPaginateTypeDef definition

class ListAssociatedStacksRequestPaginateTypeDef(TypedDict):
    FleetName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeFleetsRequestWaitTypeDef

```python
# DescribeFleetsRequestWaitTypeDef definition

class DescribeFleetsRequestWaitTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeUsersResultTypeDef

```python
# DescribeUsersResultTypeDef definition

class DescribeUsersResultTypeDef(TypedDict):
    Users: List[UserTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserTypeDef](./type_defs.md#usertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEntitledApplicationsResultTypeDef

```python
# ListEntitledApplicationsResultTypeDef definition

class ListEntitledApplicationsResultTypeDef(TypedDict):
    EntitledApplications: List[EntitledApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EntitledApplicationTypeDef](./type_defs.md#entitledapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FleetTypeDef

```python
# FleetTypeDef definition

class FleetTypeDef(TypedDict):
    Arn: str,
    Name: str,
    InstanceType: str,
    ComputeCapacityStatus: ComputeCapacityStatusTypeDef,  # (2)
    State: FleetStateType,  # (3)
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    ImageName: NotRequired[str],
    ImageArn: NotRequired[str],
    FleetType: NotRequired[FleetTypeType],  # (1)
    MaxUserDurationInSeconds: NotRequired[int],
    DisconnectTimeoutInSeconds: NotRequired[int],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (4)
    CreatedTime: NotRequired[datetime],
    FleetErrors: NotRequired[List[FleetErrorTypeDef]],  # (5)
    EnableDefaultInternetAccess: NotRequired[bool],
    DomainJoinInfo: NotRequired[DomainJoinInfoTypeDef],  # (6)
    IdleDisconnectTimeoutInSeconds: NotRequired[int],
    IamRoleArn: NotRequired[str],
    StreamView: NotRequired[StreamViewType],  # (7)
    Platform: NotRequired[PlatformTypeType],  # (8)
    MaxConcurrentSessions: NotRequired[int],
    UsbDeviceFilterStrings: NotRequired[List[str]],
    SessionScriptS3Location: NotRequired[S3LocationTypeDef],  # (9)
    MaxSessionsPerInstance: NotRequired[int],
```

1. See [:material-code-brackets: FleetTypeType](./literals.md#fleettypetype) 
2. See [:material-code-braces: ComputeCapacityStatusTypeDef](./type_defs.md#computecapacitystatustypedef) 
3. See [:material-code-brackets: FleetStateType](./literals.md#fleetstatetype) 
4. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
5. See [:material-code-braces: FleetErrorTypeDef](./type_defs.md#fleeterrortypedef) 
6. See [:material-code-braces: DomainJoinInfoTypeDef](./type_defs.md#domainjoininfotypedef) 
7. See [:material-code-brackets: StreamViewType](./literals.md#streamviewtype) 
8. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
9. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ImageBuilderTypeDef

```python
# ImageBuilderTypeDef definition

class ImageBuilderTypeDef(TypedDict):
    Name: str,
    Arn: NotRequired[str],
    ImageArn: NotRequired[str],
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (1)
    InstanceType: NotRequired[str],
    Platform: NotRequired[PlatformTypeType],  # (2)
    IamRoleArn: NotRequired[str],
    State: NotRequired[ImageBuilderStateType],  # (3)
    StateChangeReason: NotRequired[ImageBuilderStateChangeReasonTypeDef],  # (4)
    CreatedTime: NotRequired[datetime],
    EnableDefaultInternetAccess: NotRequired[bool],
    DomainJoinInfo: NotRequired[DomainJoinInfoTypeDef],  # (5)
    NetworkAccessConfiguration: NotRequired[NetworkAccessConfigurationTypeDef],  # (6)
    ImageBuilderErrors: NotRequired[List[ResourceErrorTypeDef]],  # (7)
    AppstreamAgentVersion: NotRequired[str],
    AccessEndpoints: NotRequired[List[AccessEndpointTypeDef]],  # (8)
    LatestAppstreamAgentVersion: NotRequired[LatestAppstreamAgentVersionType],  # (9)
```

1. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
2. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
3. See [:material-code-brackets: ImageBuilderStateType](./literals.md#imagebuilderstatetype) 
4. See [:material-code-braces: ImageBuilderStateChangeReasonTypeDef](./type_defs.md#imagebuilderstatechangereasontypedef) 
5. See [:material-code-braces: DomainJoinInfoTypeDef](./type_defs.md#domainjoininfotypedef) 
6. See [:material-code-braces: NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef) 
7. See [:material-code-braces: ResourceErrorTypeDef](./type_defs.md#resourceerrortypedef) 
8. See [:material-code-braces: AccessEndpointTypeDef](./type_defs.md#accessendpointtypedef) 
9. See [:material-code-brackets: LatestAppstreamAgentVersionType](./literals.md#latestappstreamagentversiontype) 
## SessionTypeDef

```python
# SessionTypeDef definition

class SessionTypeDef(TypedDict):
    Id: str,
    UserId: str,
    StackName: str,
    FleetName: str,
    State: SessionStateType,  # (1)
    ConnectionState: NotRequired[SessionConnectionStateType],  # (2)
    StartTime: NotRequired[datetime],
    MaxExpirationTime: NotRequired[datetime],
    AuthenticationType: NotRequired[AuthenticationTypeType],  # (3)
    NetworkAccessConfiguration: NotRequired[NetworkAccessConfigurationTypeDef],  # (4)
    InstanceId: NotRequired[str],
```

1. See [:material-code-brackets: SessionStateType](./literals.md#sessionstatetype) 
2. See [:material-code-brackets: SessionConnectionStateType](./literals.md#sessionconnectionstatetype) 
3. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
4. See [:material-code-braces: NetworkAccessConfigurationTypeDef](./type_defs.md#networkaccessconfigurationtypedef) 
## SharedImagePermissionsTypeDef

```python
# SharedImagePermissionsTypeDef definition

class SharedImagePermissionsTypeDef(TypedDict):
    sharedAccountId: str,
    imagePermissions: ImagePermissionsTypeDef,  # (1)
```

1. See [:material-code-braces: ImagePermissionsTypeDef](./type_defs.md#imagepermissionstypedef) 
## UpdateImagePermissionsRequestRequestTypeDef

```python
# UpdateImagePermissionsRequestRequestTypeDef definition

class UpdateImagePermissionsRequestRequestTypeDef(TypedDict):
    Name: str,
    SharedAccountId: str,
    ImagePermissions: ImagePermissionsTypeDef,  # (1)
```

1. See [:material-code-braces: ImagePermissionsTypeDef](./type_defs.md#imagepermissionstypedef) 
## UsageReportSubscriptionTypeDef

```python
# UsageReportSubscriptionTypeDef definition

class UsageReportSubscriptionTypeDef(TypedDict):
    S3BucketName: NotRequired[str],
    Schedule: NotRequired[UsageReportScheduleType],  # (1)
    LastGeneratedReportDate: NotRequired[datetime],
    SubscriptionErrors: NotRequired[List[LastReportGenerationExecutionErrorTypeDef]],  # (2)
```

1. See [:material-code-brackets: UsageReportScheduleType](./literals.md#usagereportscheduletype) 
2. See [:material-code-braces: LastReportGenerationExecutionErrorTypeDef](./type_defs.md#lastreportgenerationexecutionerrortypedef) 
## StackTypeDef

```python
# StackTypeDef definition

class StackTypeDef(TypedDict):
    Name: str,
    Arn: NotRequired[str],
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    StorageConnectors: NotRequired[List[StorageConnectorOutputTypeDef]],  # (1)
    RedirectURL: NotRequired[str],
    FeedbackURL: NotRequired[str],
    StackErrors: NotRequired[List[StackErrorTypeDef]],  # (2)
    UserSettings: NotRequired[List[UserSettingTypeDef]],  # (3)
    ApplicationSettings: NotRequired[ApplicationSettingsResponseTypeDef],  # (4)
    AccessEndpoints: NotRequired[List[AccessEndpointTypeDef]],  # (5)
    EmbedHostDomains: NotRequired[List[str]],
    StreamingExperienceSettings: NotRequired[StreamingExperienceSettingsTypeDef],  # (6)
```

1. See [:material-code-braces: StorageConnectorOutputTypeDef](./type_defs.md#storageconnectoroutputtypedef) 
2. See [:material-code-braces: StackErrorTypeDef](./type_defs.md#stackerrortypedef) 
3. See [:material-code-braces: UserSettingTypeDef](./type_defs.md#usersettingtypedef) 
4. See [:material-code-braces: ApplicationSettingsResponseTypeDef](./type_defs.md#applicationsettingsresponsetypedef) 
5. See [:material-code-braces: AccessEndpointTypeDef](./type_defs.md#accessendpointtypedef) 
6. See [:material-code-braces: StreamingExperienceSettingsTypeDef](./type_defs.md#streamingexperiencesettingstypedef) 
## UpdateStackRequestRequestTypeDef

```python
# UpdateStackRequestRequestTypeDef definition

class UpdateStackRequestRequestTypeDef(TypedDict):
    Name: str,
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    StorageConnectors: NotRequired[Sequence[StorageConnectorTypeDef]],  # (1)
    DeleteStorageConnectors: NotRequired[bool],
    RedirectURL: NotRequired[str],
    FeedbackURL: NotRequired[str],
    AttributesToDelete: NotRequired[Sequence[StackAttributeType]],  # (2)
    UserSettings: NotRequired[Sequence[UserSettingTypeDef]],  # (3)
    ApplicationSettings: NotRequired[ApplicationSettingsTypeDef],  # (4)
    AccessEndpoints: NotRequired[Sequence[AccessEndpointTypeDef]],  # (5)
    EmbedHostDomains: NotRequired[Sequence[str]],
    StreamingExperienceSettings: NotRequired[StreamingExperienceSettingsTypeDef],  # (6)
```

1. See [:material-code-braces: StorageConnectorTypeDef](./type_defs.md#storageconnectortypedef) 
2. See [:material-code-brackets: StackAttributeType](./literals.md#stackattributetype) 
3. See [:material-code-braces: UserSettingTypeDef](./type_defs.md#usersettingtypedef) 
4. See [:material-code-braces: ApplicationSettingsTypeDef](./type_defs.md#applicationsettingstypedef) 
5. See [:material-code-braces: AccessEndpointTypeDef](./type_defs.md#accessendpointtypedef) 
6. See [:material-code-braces: StreamingExperienceSettingsTypeDef](./type_defs.md#streamingexperiencesettingstypedef) 
## CreateAppBlockBuilderResultTypeDef

```python
# CreateAppBlockBuilderResultTypeDef definition

class CreateAppBlockBuilderResultTypeDef(TypedDict):
    AppBlockBuilder: AppBlockBuilderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppBlockBuilderTypeDef](./type_defs.md#appblockbuildertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppBlockBuildersResultTypeDef

```python
# DescribeAppBlockBuildersResultTypeDef definition

class DescribeAppBlockBuildersResultTypeDef(TypedDict):
    AppBlockBuilders: List[AppBlockBuilderTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AppBlockBuilderTypeDef](./type_defs.md#appblockbuildertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAppBlockBuilderResultTypeDef

```python
# StartAppBlockBuilderResultTypeDef definition

class StartAppBlockBuilderResultTypeDef(TypedDict):
    AppBlockBuilder: AppBlockBuilderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppBlockBuilderTypeDef](./type_defs.md#appblockbuildertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopAppBlockBuilderResultTypeDef

```python
# StopAppBlockBuilderResultTypeDef definition

class StopAppBlockBuilderResultTypeDef(TypedDict):
    AppBlockBuilder: AppBlockBuilderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppBlockBuilderTypeDef](./type_defs.md#appblockbuildertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppBlockBuilderResultTypeDef

```python
# UpdateAppBlockBuilderResultTypeDef definition

class UpdateAppBlockBuilderResultTypeDef(TypedDict):
    AppBlockBuilder: AppBlockBuilderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppBlockBuilderTypeDef](./type_defs.md#appblockbuildertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationResultTypeDef

```python
# CreateApplicationResultTypeDef definition

class CreateApplicationResultTypeDef(TypedDict):
    Application: ApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicationsResultTypeDef

```python
# DescribeApplicationsResultTypeDef definition

class DescribeApplicationsResultTypeDef(TypedDict):
    Applications: List[ApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImageTypeDef

```python
# ImageTypeDef definition

class ImageTypeDef(TypedDict):
    Name: str,
    Arn: NotRequired[str],
    BaseImageArn: NotRequired[str],
    DisplayName: NotRequired[str],
    State: NotRequired[ImageStateType],  # (1)
    Visibility: NotRequired[VisibilityTypeType],  # (2)
    ImageBuilderSupported: NotRequired[bool],
    ImageBuilderName: NotRequired[str],
    Platform: NotRequired[PlatformTypeType],  # (3)
    Description: NotRequired[str],
    StateChangeReason: NotRequired[ImageStateChangeReasonTypeDef],  # (4)
    Applications: NotRequired[List[ApplicationTypeDef]],  # (5)
    CreatedTime: NotRequired[datetime],
    PublicBaseImageReleasedDate: NotRequired[datetime],
    AppstreamAgentVersion: NotRequired[str],
    ImagePermissions: NotRequired[ImagePermissionsTypeDef],  # (6)
    ImageErrors: NotRequired[List[ResourceErrorTypeDef]],  # (7)
    LatestAppstreamAgentVersion: NotRequired[LatestAppstreamAgentVersionType],  # (8)
    SupportedInstanceFamilies: NotRequired[List[str]],
    DynamicAppProvidersEnabled: NotRequired[DynamicAppProvidersEnabledType],  # (9)
    ImageSharedWithOthers: NotRequired[ImageSharedWithOthersType],  # (10)
```

1. See [:material-code-brackets: ImageStateType](./literals.md#imagestatetype) 
2. See [:material-code-brackets: VisibilityTypeType](./literals.md#visibilitytypetype) 
3. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
4. See [:material-code-braces: ImageStateChangeReasonTypeDef](./type_defs.md#imagestatechangereasontypedef) 
5. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
6. See [:material-code-braces: ImagePermissionsTypeDef](./type_defs.md#imagepermissionstypedef) 
7. See [:material-code-braces: ResourceErrorTypeDef](./type_defs.md#resourceerrortypedef) 
8. See [:material-code-brackets: LatestAppstreamAgentVersionType](./literals.md#latestappstreamagentversiontype) 
9. See [:material-code-brackets: DynamicAppProvidersEnabledType](./literals.md#dynamicappprovidersenabledtype) 
10. See [:material-code-brackets: ImageSharedWithOthersType](./literals.md#imagesharedwithotherstype) 
## UpdateApplicationResultTypeDef

```python
# UpdateApplicationResultTypeDef definition

class UpdateApplicationResultTypeDef(TypedDict):
    Application: ApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AppBlockTypeDef

```python
# AppBlockTypeDef definition

class AppBlockTypeDef(TypedDict):
    Name: str,
    Arn: str,
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    SourceS3Location: NotRequired[S3LocationTypeDef],  # (1)
    SetupScriptDetails: NotRequired[ScriptDetailsTypeDef],  # (2)
    CreatedTime: NotRequired[datetime],
    PostSetupScriptDetails: NotRequired[ScriptDetailsTypeDef],  # (2)
    PackagingType: NotRequired[PackagingTypeType],  # (4)
    State: NotRequired[AppBlockStateType],  # (5)
    AppBlockErrors: NotRequired[List[ErrorDetailsTypeDef]],  # (6)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: ScriptDetailsTypeDef](./type_defs.md#scriptdetailstypedef) 
3. See [:material-code-braces: ScriptDetailsTypeDef](./type_defs.md#scriptdetailstypedef) 
4. See [:material-code-brackets: PackagingTypeType](./literals.md#packagingtypetype) 
5. See [:material-code-brackets: AppBlockStateType](./literals.md#appblockstatetype) 
6. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## CreateAppBlockRequestRequestTypeDef

```python
# CreateAppBlockRequestRequestTypeDef definition

class CreateAppBlockRequestRequestTypeDef(TypedDict):
    Name: str,
    SourceS3Location: S3LocationTypeDef,  # (1)
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    SetupScriptDetails: NotRequired[ScriptDetailsTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
    PostSetupScriptDetails: NotRequired[ScriptDetailsTypeDef],  # (2)
    PackagingType: NotRequired[PackagingTypeType],  # (4)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: ScriptDetailsTypeDef](./type_defs.md#scriptdetailstypedef) 
3. See [:material-code-braces: ScriptDetailsTypeDef](./type_defs.md#scriptdetailstypedef) 
4. See [:material-code-brackets: PackagingTypeType](./literals.md#packagingtypetype) 
## BatchAssociateUserStackResultTypeDef

```python
# BatchAssociateUserStackResultTypeDef definition

class BatchAssociateUserStackResultTypeDef(TypedDict):
    errors: List[UserStackAssociationErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserStackAssociationErrorTypeDef](./type_defs.md#userstackassociationerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateUserStackResultTypeDef

```python
# BatchDisassociateUserStackResultTypeDef definition

class BatchDisassociateUserStackResultTypeDef(TypedDict):
    errors: List[UserStackAssociationErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserStackAssociationErrorTypeDef](./type_defs.md#userstackassociationerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDirectoryConfigResultTypeDef

```python
# CreateDirectoryConfigResultTypeDef definition

class CreateDirectoryConfigResultTypeDef(TypedDict):
    DirectoryConfig: DirectoryConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectoryConfigTypeDef](./type_defs.md#directoryconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDirectoryConfigsResultTypeDef

```python
# DescribeDirectoryConfigsResultTypeDef definition

class DescribeDirectoryConfigsResultTypeDef(TypedDict):
    DirectoryConfigs: List[DirectoryConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DirectoryConfigTypeDef](./type_defs.md#directoryconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDirectoryConfigResultTypeDef

```python
# UpdateDirectoryConfigResultTypeDef definition

class UpdateDirectoryConfigResultTypeDef(TypedDict):
    DirectoryConfig: DirectoryConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DirectoryConfigTypeDef](./type_defs.md#directoryconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEntitlementResultTypeDef

```python
# CreateEntitlementResultTypeDef definition

class CreateEntitlementResultTypeDef(TypedDict):
    Entitlement: EntitlementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEntitlementsResultTypeDef

```python
# DescribeEntitlementsResultTypeDef definition

class DescribeEntitlementsResultTypeDef(TypedDict):
    Entitlements: List[EntitlementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEntitlementResultTypeDef

```python
# UpdateEntitlementResultTypeDef definition

class UpdateEntitlementResultTypeDef(TypedDict):
    Entitlement: EntitlementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateThemeForStackResultTypeDef

```python
# CreateThemeForStackResultTypeDef definition

class CreateThemeForStackResultTypeDef(TypedDict):
    Theme: ThemeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeTypeDef](./type_defs.md#themetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeThemeForStackResultTypeDef

```python
# DescribeThemeForStackResultTypeDef definition

class DescribeThemeForStackResultTypeDef(TypedDict):
    Theme: ThemeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeTypeDef](./type_defs.md#themetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateThemeForStackResultTypeDef

```python
# UpdateThemeForStackResultTypeDef definition

class UpdateThemeForStackResultTypeDef(TypedDict):
    Theme: ThemeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThemeTypeDef](./type_defs.md#themetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetResultTypeDef

```python
# CreateFleetResultTypeDef definition

class CreateFleetResultTypeDef(TypedDict):
    Fleet: FleetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FleetTypeDef](./type_defs.md#fleettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFleetsResultTypeDef

```python
# DescribeFleetsResultTypeDef definition

class DescribeFleetsResultTypeDef(TypedDict):
    Fleets: List[FleetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetTypeDef](./type_defs.md#fleettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFleetResultTypeDef

```python
# UpdateFleetResultTypeDef definition

class UpdateFleetResultTypeDef(TypedDict):
    Fleet: FleetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FleetTypeDef](./type_defs.md#fleettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateImageBuilderResultTypeDef

```python
# CreateImageBuilderResultTypeDef definition

class CreateImageBuilderResultTypeDef(TypedDict):
    ImageBuilder: ImageBuilderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageBuilderTypeDef](./type_defs.md#imagebuildertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteImageBuilderResultTypeDef

```python
# DeleteImageBuilderResultTypeDef definition

class DeleteImageBuilderResultTypeDef(TypedDict):
    ImageBuilder: ImageBuilderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageBuilderTypeDef](./type_defs.md#imagebuildertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImageBuildersResultTypeDef

```python
# DescribeImageBuildersResultTypeDef definition

class DescribeImageBuildersResultTypeDef(TypedDict):
    ImageBuilders: List[ImageBuilderTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImageBuilderTypeDef](./type_defs.md#imagebuildertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImageBuilderResultTypeDef

```python
# StartImageBuilderResultTypeDef definition

class StartImageBuilderResultTypeDef(TypedDict):
    ImageBuilder: ImageBuilderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageBuilderTypeDef](./type_defs.md#imagebuildertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopImageBuilderResultTypeDef

```python
# StopImageBuilderResultTypeDef definition

class StopImageBuilderResultTypeDef(TypedDict):
    ImageBuilder: ImageBuilderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageBuilderTypeDef](./type_defs.md#imagebuildertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSessionsResultTypeDef

```python
# DescribeSessionsResultTypeDef definition

class DescribeSessionsResultTypeDef(TypedDict):
    Sessions: List[SessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImagePermissionsResultTypeDef

```python
# DescribeImagePermissionsResultTypeDef definition

class DescribeImagePermissionsResultTypeDef(TypedDict):
    Name: str,
    SharedImagePermissionsList: List[SharedImagePermissionsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SharedImagePermissionsTypeDef](./type_defs.md#sharedimagepermissionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUsageReportSubscriptionsResultTypeDef

```python
# DescribeUsageReportSubscriptionsResultTypeDef definition

class DescribeUsageReportSubscriptionsResultTypeDef(TypedDict):
    UsageReportSubscriptions: List[UsageReportSubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UsageReportSubscriptionTypeDef](./type_defs.md#usagereportsubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStackResultTypeDef

```python
# CreateStackResultTypeDef definition

class CreateStackResultTypeDef(TypedDict):
    Stack: StackTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StackTypeDef](./type_defs.md#stacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStacksResultTypeDef

```python
# DescribeStacksResultTypeDef definition

class DescribeStacksResultTypeDef(TypedDict):
    Stacks: List[StackTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StackTypeDef](./type_defs.md#stacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStackResultTypeDef

```python
# UpdateStackResultTypeDef definition

class UpdateStackResultTypeDef(TypedDict):
    Stack: StackTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StackTypeDef](./type_defs.md#stacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStackRequestRequestTypeDef

```python
# CreateStackRequestRequestTypeDef definition

class CreateStackRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    StorageConnectors: NotRequired[Sequence[StorageConnectorUnionTypeDef]],  # (1)
    RedirectURL: NotRequired[str],
    FeedbackURL: NotRequired[str],
    UserSettings: NotRequired[Sequence[UserSettingTypeDef]],  # (2)
    ApplicationSettings: NotRequired[ApplicationSettingsTypeDef],  # (3)
    Tags: NotRequired[Mapping[str, str]],
    AccessEndpoints: NotRequired[Sequence[AccessEndpointTypeDef]],  # (4)
    EmbedHostDomains: NotRequired[Sequence[str]],
    StreamingExperienceSettings: NotRequired[StreamingExperienceSettingsTypeDef],  # (5)
```

1. See [:material-code-braces: StorageConnectorTypeDef](./type_defs.md#storageconnectortypedef) [:material-code-braces: StorageConnectorOutputTypeDef](./type_defs.md#storageconnectoroutputtypedef) 
2. See [:material-code-braces: UserSettingTypeDef](./type_defs.md#usersettingtypedef) 
3. See [:material-code-braces: ApplicationSettingsTypeDef](./type_defs.md#applicationsettingstypedef) 
4. See [:material-code-braces: AccessEndpointTypeDef](./type_defs.md#accessendpointtypedef) 
5. See [:material-code-braces: StreamingExperienceSettingsTypeDef](./type_defs.md#streamingexperiencesettingstypedef) 
## CreateUpdatedImageResultTypeDef

```python
# CreateUpdatedImageResultTypeDef definition

class CreateUpdatedImageResultTypeDef(TypedDict):
    image: ImageTypeDef,  # (1)
    canUpdateImage: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteImageResultTypeDef

```python
# DeleteImageResultTypeDef definition

class DeleteImageResultTypeDef(TypedDict):
    Image: ImageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImagesResultTypeDef

```python
# DescribeImagesResultTypeDef definition

class DescribeImagesResultTypeDef(TypedDict):
    Images: List[ImageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppBlockResultTypeDef

```python
# CreateAppBlockResultTypeDef definition

class CreateAppBlockResultTypeDef(TypedDict):
    AppBlock: AppBlockTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppBlockTypeDef](./type_defs.md#appblocktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAppBlocksResultTypeDef

```python
# DescribeAppBlocksResultTypeDef definition

class DescribeAppBlocksResultTypeDef(TypedDict):
    AppBlocks: List[AppBlockTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AppBlockTypeDef](./type_defs.md#appblocktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
