# Type definitions

> [Index](../README.md) > [WorkMail](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WorkMail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#WorkMail)
    type annotations stubs module [types-aiobotocore-workmail](https://pypi.org/project/types-aiobotocore-workmail/).



## AccessControlRuleTypeDef

```python
# AccessControlRuleTypeDef definition

class AccessControlRuleTypeDef(TypedDict):
    Name: NotRequired[str],
    Effect: NotRequired[AccessControlRuleEffectType],  # (1)
    Description: NotRequired[str],
    IpRanges: NotRequired[List[str]],
    NotIpRanges: NotRequired[List[str]],
    Actions: NotRequired[List[str]],
    NotActions: NotRequired[List[str]],
    UserIds: NotRequired[List[str]],
    NotUserIds: NotRequired[List[str]],
    DateCreated: NotRequired[datetime],
    DateModified: NotRequired[datetime],
    ImpersonationRoleIds: NotRequired[List[str]],
    NotImpersonationRoleIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: AccessControlRuleEffectType](./literals.md#accesscontrolruleeffecttype) 
## AssociateDelegateToResourceRequestRequestTypeDef

```python
# AssociateDelegateToResourceRequestRequestTypeDef definition

class AssociateDelegateToResourceRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ResourceId: str,
    EntityId: str,
```

## AssociateMemberToGroupRequestRequestTypeDef

```python
# AssociateMemberToGroupRequestRequestTypeDef definition

class AssociateMemberToGroupRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    GroupId: str,
    MemberId: str,
```

## AssumeImpersonationRoleRequestRequestTypeDef

```python
# AssumeImpersonationRoleRequestRequestTypeDef definition

class AssumeImpersonationRoleRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ImpersonationRoleId: str,
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

## LambdaAvailabilityProviderTypeDef

```python
# LambdaAvailabilityProviderTypeDef definition

class LambdaAvailabilityProviderTypeDef(TypedDict):
    LambdaArn: str,
```

## RedactedEwsAvailabilityProviderTypeDef

```python
# RedactedEwsAvailabilityProviderTypeDef definition

class RedactedEwsAvailabilityProviderTypeDef(TypedDict):
    EwsEndpoint: NotRequired[str],
    EwsUsername: NotRequired[str],
```

## BookingOptionsTypeDef

```python
# BookingOptionsTypeDef definition

class BookingOptionsTypeDef(TypedDict):
    AutoAcceptRequests: NotRequired[bool],
    AutoDeclineRecurringRequests: NotRequired[bool],
    AutoDeclineConflictingRequests: NotRequired[bool],
```

## CancelMailboxExportJobRequestRequestTypeDef

```python
# CancelMailboxExportJobRequestRequestTypeDef definition

class CancelMailboxExportJobRequestRequestTypeDef(TypedDict):
    ClientToken: str,
    JobId: str,
    OrganizationId: str,
```

## CreateAliasRequestRequestTypeDef

```python
# CreateAliasRequestRequestTypeDef definition

class CreateAliasRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
    Alias: str,
```

## EwsAvailabilityProviderTypeDef

```python
# EwsAvailabilityProviderTypeDef definition

class EwsAvailabilityProviderTypeDef(TypedDict):
    EwsEndpoint: str,
    EwsUsername: str,
    EwsPassword: str,
```

## CreateGroupRequestRequestTypeDef

```python
# CreateGroupRequestRequestTypeDef definition

class CreateGroupRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Name: str,
```

## ImpersonationRuleTypeDef

```python
# ImpersonationRuleTypeDef definition

class ImpersonationRuleTypeDef(TypedDict):
    ImpersonationRuleId: str,
    Effect: AccessEffectType,  # (1)
    Name: NotRequired[str],
    Description: NotRequired[str],
    TargetUsers: NotRequired[Sequence[str]],
    NotTargetUsers: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AccessEffectType](./literals.md#accesseffecttype) 
## CreateMobileDeviceAccessRuleRequestRequestTypeDef

```python
# CreateMobileDeviceAccessRuleRequestRequestTypeDef definition

class CreateMobileDeviceAccessRuleRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Name: str,
    Effect: MobileDeviceAccessRuleEffectType,  # (1)
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    DeviceTypes: NotRequired[Sequence[str]],
    NotDeviceTypes: NotRequired[Sequence[str]],
    DeviceModels: NotRequired[Sequence[str]],
    NotDeviceModels: NotRequired[Sequence[str]],
    DeviceOperatingSystems: NotRequired[Sequence[str]],
    NotDeviceOperatingSystems: NotRequired[Sequence[str]],
    DeviceUserAgents: NotRequired[Sequence[str]],
    NotDeviceUserAgents: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype) 
## DomainTypeDef

```python
# DomainTypeDef definition

class DomainTypeDef(TypedDict):
    DomainName: NotRequired[str],
    HostedZoneId: NotRequired[str],
```

## CreateResourceRequestRequestTypeDef

```python
# CreateResourceRequestRequestTypeDef definition

class CreateResourceRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Name: str,
    Type: ResourceTypeType,  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## CreateUserRequestRequestTypeDef

```python
# CreateUserRequestRequestTypeDef definition

class CreateUserRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Name: str,
    DisplayName: str,
    Password: str,
```

## DelegateTypeDef

```python
# DelegateTypeDef definition

class DelegateTypeDef(TypedDict):
    Id: str,
    Type: MemberTypeType,  # (1)
```

1. See [:material-code-brackets: MemberTypeType](./literals.md#membertypetype) 
## DeleteAccessControlRuleRequestRequestTypeDef

```python
# DeleteAccessControlRuleRequestRequestTypeDef definition

class DeleteAccessControlRuleRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Name: str,
```

## DeleteAliasRequestRequestTypeDef

```python
# DeleteAliasRequestRequestTypeDef definition

class DeleteAliasRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
    Alias: str,
```

## DeleteAvailabilityConfigurationRequestRequestTypeDef

```python
# DeleteAvailabilityConfigurationRequestRequestTypeDef definition

class DeleteAvailabilityConfigurationRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    DomainName: str,
```

## DeleteEmailMonitoringConfigurationRequestRequestTypeDef

```python
# DeleteEmailMonitoringConfigurationRequestRequestTypeDef definition

class DeleteEmailMonitoringConfigurationRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
```

## DeleteGroupRequestRequestTypeDef

```python
# DeleteGroupRequestRequestTypeDef definition

class DeleteGroupRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    GroupId: str,
```

## DeleteImpersonationRoleRequestRequestTypeDef

```python
# DeleteImpersonationRoleRequestRequestTypeDef definition

class DeleteImpersonationRoleRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ImpersonationRoleId: str,
```

## DeleteMailboxPermissionsRequestRequestTypeDef

```python
# DeleteMailboxPermissionsRequestRequestTypeDef definition

class DeleteMailboxPermissionsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
    GranteeId: str,
```

## DeleteMobileDeviceAccessOverrideRequestRequestTypeDef

```python
# DeleteMobileDeviceAccessOverrideRequestRequestTypeDef definition

class DeleteMobileDeviceAccessOverrideRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    UserId: str,
    DeviceId: str,
```

## DeleteMobileDeviceAccessRuleRequestRequestTypeDef

```python
# DeleteMobileDeviceAccessRuleRequestRequestTypeDef definition

class DeleteMobileDeviceAccessRuleRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    MobileDeviceAccessRuleId: str,
```

## DeleteOrganizationRequestRequestTypeDef

```python
# DeleteOrganizationRequestRequestTypeDef definition

class DeleteOrganizationRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    DeleteDirectory: bool,
    ClientToken: NotRequired[str],
```

## DeleteResourceRequestRequestTypeDef

```python
# DeleteResourceRequestRequestTypeDef definition

class DeleteResourceRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ResourceId: str,
```

## DeleteRetentionPolicyRequestRequestTypeDef

```python
# DeleteRetentionPolicyRequestRequestTypeDef definition

class DeleteRetentionPolicyRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Id: str,
```

## DeleteUserRequestRequestTypeDef

```python
# DeleteUserRequestRequestTypeDef definition

class DeleteUserRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    UserId: str,
```

## DeregisterFromWorkMailRequestRequestTypeDef

```python
# DeregisterFromWorkMailRequestRequestTypeDef definition

class DeregisterFromWorkMailRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
```

## DeregisterMailDomainRequestRequestTypeDef

```python
# DeregisterMailDomainRequestRequestTypeDef definition

class DeregisterMailDomainRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    DomainName: str,
```

## DescribeEmailMonitoringConfigurationRequestRequestTypeDef

```python
# DescribeEmailMonitoringConfigurationRequestRequestTypeDef definition

class DescribeEmailMonitoringConfigurationRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
```

## DescribeGroupRequestRequestTypeDef

```python
# DescribeGroupRequestRequestTypeDef definition

class DescribeGroupRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    GroupId: str,
```

## DescribeInboundDmarcSettingsRequestRequestTypeDef

```python
# DescribeInboundDmarcSettingsRequestRequestTypeDef definition

class DescribeInboundDmarcSettingsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
```

## DescribeMailboxExportJobRequestRequestTypeDef

```python
# DescribeMailboxExportJobRequestRequestTypeDef definition

class DescribeMailboxExportJobRequestRequestTypeDef(TypedDict):
    JobId: str,
    OrganizationId: str,
```

## DescribeOrganizationRequestRequestTypeDef

```python
# DescribeOrganizationRequestRequestTypeDef definition

class DescribeOrganizationRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
```

## DescribeResourceRequestRequestTypeDef

```python
# DescribeResourceRequestRequestTypeDef definition

class DescribeResourceRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ResourceId: str,
```

## DescribeUserRequestRequestTypeDef

```python
# DescribeUserRequestRequestTypeDef definition

class DescribeUserRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    UserId: str,
```

## DisassociateDelegateFromResourceRequestRequestTypeDef

```python
# DisassociateDelegateFromResourceRequestRequestTypeDef definition

class DisassociateDelegateFromResourceRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ResourceId: str,
    EntityId: str,
```

## DisassociateMemberFromGroupRequestRequestTypeDef

```python
# DisassociateMemberFromGroupRequestRequestTypeDef definition

class DisassociateMemberFromGroupRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    GroupId: str,
    MemberId: str,
```

## DnsRecordTypeDef

```python
# DnsRecordTypeDef definition

class DnsRecordTypeDef(TypedDict):
    Type: NotRequired[str],
    Hostname: NotRequired[str],
    Value: NotRequired[str],
```

## FolderConfigurationTypeDef

```python
# FolderConfigurationTypeDef definition

class FolderConfigurationTypeDef(TypedDict):
    Name: FolderNameType,  # (1)
    Action: RetentionActionType,  # (2)
    Period: NotRequired[int],
```

1. See [:material-code-brackets: FolderNameType](./literals.md#foldernametype) 
2. See [:material-code-brackets: RetentionActionType](./literals.md#retentionactiontype) 
## GetAccessControlEffectRequestRequestTypeDef

```python
# GetAccessControlEffectRequestRequestTypeDef definition

class GetAccessControlEffectRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    IpAddress: str,
    Action: str,
    UserId: NotRequired[str],
    ImpersonationRoleId: NotRequired[str],
```

## GetDefaultRetentionPolicyRequestRequestTypeDef

```python
# GetDefaultRetentionPolicyRequestRequestTypeDef definition

class GetDefaultRetentionPolicyRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
```

## GetImpersonationRoleEffectRequestRequestTypeDef

```python
# GetImpersonationRoleEffectRequestRequestTypeDef definition

class GetImpersonationRoleEffectRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ImpersonationRoleId: str,
    TargetUser: str,
```

## ImpersonationMatchedRuleTypeDef

```python
# ImpersonationMatchedRuleTypeDef definition

class ImpersonationMatchedRuleTypeDef(TypedDict):
    ImpersonationRuleId: NotRequired[str],
    Name: NotRequired[str],
```

## GetImpersonationRoleRequestRequestTypeDef

```python
# GetImpersonationRoleRequestRequestTypeDef definition

class GetImpersonationRoleRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ImpersonationRoleId: str,
```

## GetMailDomainRequestRequestTypeDef

```python
# GetMailDomainRequestRequestTypeDef definition

class GetMailDomainRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    DomainName: str,
```

## GetMailboxDetailsRequestRequestTypeDef

```python
# GetMailboxDetailsRequestRequestTypeDef definition

class GetMailboxDetailsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    UserId: str,
```

## GetMobileDeviceAccessEffectRequestRequestTypeDef

```python
# GetMobileDeviceAccessEffectRequestRequestTypeDef definition

class GetMobileDeviceAccessEffectRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    DeviceType: NotRequired[str],
    DeviceModel: NotRequired[str],
    DeviceOperatingSystem: NotRequired[str],
    DeviceUserAgent: NotRequired[str],
```

## MobileDeviceAccessMatchedRuleTypeDef

```python
# MobileDeviceAccessMatchedRuleTypeDef definition

class MobileDeviceAccessMatchedRuleTypeDef(TypedDict):
    MobileDeviceAccessRuleId: NotRequired[str],
    Name: NotRequired[str],
```

## GetMobileDeviceAccessOverrideRequestRequestTypeDef

```python
# GetMobileDeviceAccessOverrideRequestRequestTypeDef definition

class GetMobileDeviceAccessOverrideRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    UserId: str,
    DeviceId: str,
```

## GroupTypeDef

```python
# GroupTypeDef definition

class GroupTypeDef(TypedDict):
    Id: NotRequired[str],
    Email: NotRequired[str],
    Name: NotRequired[str],
    State: NotRequired[EntityStateType],  # (1)
    EnabledDate: NotRequired[datetime],
    DisabledDate: NotRequired[datetime],
```

1. See [:material-code-brackets: EntityStateType](./literals.md#entitystatetype) 
## ImpersonationRoleTypeDef

```python
# ImpersonationRoleTypeDef definition

class ImpersonationRoleTypeDef(TypedDict):
    ImpersonationRoleId: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[ImpersonationRoleTypeType],  # (1)
    DateCreated: NotRequired[datetime],
    DateModified: NotRequired[datetime],
```

1. See [:material-code-brackets: ImpersonationRoleTypeType](./literals.md#impersonationroletypetype) 
## ListAccessControlRulesRequestRequestTypeDef

```python
# ListAccessControlRulesRequestRequestTypeDef definition

class ListAccessControlRulesRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAliasesRequestRequestTypeDef

```python
# ListAliasesRequestRequestTypeDef definition

class ListAliasesRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAvailabilityConfigurationsRequestRequestTypeDef

```python
# ListAvailabilityConfigurationsRequestRequestTypeDef definition

class ListAvailabilityConfigurationsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListGroupMembersRequestRequestTypeDef

```python
# ListGroupMembersRequestRequestTypeDef definition

class ListGroupMembersRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    GroupId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MemberTypeDef

```python
# MemberTypeDef definition

class MemberTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[MemberTypeType],  # (1)
    State: NotRequired[EntityStateType],  # (2)
    EnabledDate: NotRequired[datetime],
    DisabledDate: NotRequired[datetime],
```

1. See [:material-code-brackets: MemberTypeType](./literals.md#membertypetype) 
2. See [:material-code-brackets: EntityStateType](./literals.md#entitystatetype) 
## ListGroupsRequestRequestTypeDef

```python
# ListGroupsRequestRequestTypeDef definition

class ListGroupsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListImpersonationRolesRequestRequestTypeDef

```python
# ListImpersonationRolesRequestRequestTypeDef definition

class ListImpersonationRolesRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListMailDomainsRequestRequestTypeDef

```python
# ListMailDomainsRequestRequestTypeDef definition

class ListMailDomainsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MailDomainSummaryTypeDef

```python
# MailDomainSummaryTypeDef definition

class MailDomainSummaryTypeDef(TypedDict):
    DomainName: NotRequired[str],
    DefaultDomain: NotRequired[bool],
```

## ListMailboxExportJobsRequestRequestTypeDef

```python
# ListMailboxExportJobsRequestRequestTypeDef definition

class ListMailboxExportJobsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MailboxExportJobTypeDef

```python
# MailboxExportJobTypeDef definition

class MailboxExportJobTypeDef(TypedDict):
    JobId: NotRequired[str],
    EntityId: NotRequired[str],
    Description: NotRequired[str],
    S3BucketName: NotRequired[str],
    S3Path: NotRequired[str],
    EstimatedProgress: NotRequired[int],
    State: NotRequired[MailboxExportJobStateType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: MailboxExportJobStateType](./literals.md#mailboxexportjobstatetype) 
## ListMailboxPermissionsRequestRequestTypeDef

```python
# ListMailboxPermissionsRequestRequestTypeDef definition

class ListMailboxPermissionsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PermissionTypeDef

```python
# PermissionTypeDef definition

class PermissionTypeDef(TypedDict):
    GranteeId: str,
    GranteeType: MemberTypeType,  # (1)
    PermissionValues: List[PermissionTypeType],  # (2)
```

1. See [:material-code-brackets: MemberTypeType](./literals.md#membertypetype) 
2. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
## ListMobileDeviceAccessOverridesRequestRequestTypeDef

```python
# ListMobileDeviceAccessOverridesRequestRequestTypeDef definition

class ListMobileDeviceAccessOverridesRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    UserId: NotRequired[str],
    DeviceId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MobileDeviceAccessOverrideTypeDef

```python
# MobileDeviceAccessOverrideTypeDef definition

class MobileDeviceAccessOverrideTypeDef(TypedDict):
    UserId: NotRequired[str],
    DeviceId: NotRequired[str],
    Effect: NotRequired[MobileDeviceAccessRuleEffectType],  # (1)
    Description: NotRequired[str],
    DateCreated: NotRequired[datetime],
    DateModified: NotRequired[datetime],
```

1. See [:material-code-brackets: MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype) 
## ListMobileDeviceAccessRulesRequestRequestTypeDef

```python
# ListMobileDeviceAccessRulesRequestRequestTypeDef definition

class ListMobileDeviceAccessRulesRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
```

## MobileDeviceAccessRuleTypeDef

```python
# MobileDeviceAccessRuleTypeDef definition

class MobileDeviceAccessRuleTypeDef(TypedDict):
    MobileDeviceAccessRuleId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Effect: NotRequired[MobileDeviceAccessRuleEffectType],  # (1)
    DeviceTypes: NotRequired[List[str]],
    NotDeviceTypes: NotRequired[List[str]],
    DeviceModels: NotRequired[List[str]],
    NotDeviceModels: NotRequired[List[str]],
    DeviceOperatingSystems: NotRequired[List[str]],
    NotDeviceOperatingSystems: NotRequired[List[str]],
    DeviceUserAgents: NotRequired[List[str]],
    NotDeviceUserAgents: NotRequired[List[str]],
    DateCreated: NotRequired[datetime],
    DateModified: NotRequired[datetime],
```

1. See [:material-code-brackets: MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype) 
## ListOrganizationsRequestRequestTypeDef

```python
# ListOrganizationsRequestRequestTypeDef definition

class ListOrganizationsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## OrganizationSummaryTypeDef

```python
# OrganizationSummaryTypeDef definition

class OrganizationSummaryTypeDef(TypedDict):
    OrganizationId: NotRequired[str],
    Alias: NotRequired[str],
    DefaultMailDomain: NotRequired[str],
    ErrorMessage: NotRequired[str],
    State: NotRequired[str],
```

## ListResourceDelegatesRequestRequestTypeDef

```python
# ListResourceDelegatesRequestRequestTypeDef definition

class ListResourceDelegatesRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ResourceId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListResourcesRequestRequestTypeDef

```python
# ListResourcesRequestRequestTypeDef definition

class ListResourcesRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    Id: NotRequired[str],
    Email: NotRequired[str],
    Name: NotRequired[str],
    Type: NotRequired[ResourceTypeType],  # (1)
    State: NotRequired[EntityStateType],  # (2)
    EnabledDate: NotRequired[datetime],
    DisabledDate: NotRequired[datetime],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: EntityStateType](./literals.md#entitystatetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ListUsersRequestRequestTypeDef

```python
# ListUsersRequestRequestTypeDef definition

class ListUsersRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## UserTypeDef

```python
# UserTypeDef definition

class UserTypeDef(TypedDict):
    Id: NotRequired[str],
    Email: NotRequired[str],
    Name: NotRequired[str],
    DisplayName: NotRequired[str],
    State: NotRequired[EntityStateType],  # (1)
    UserRole: NotRequired[UserRoleType],  # (2)
    EnabledDate: NotRequired[datetime],
    DisabledDate: NotRequired[datetime],
```

1. See [:material-code-brackets: EntityStateType](./literals.md#entitystatetype) 
2. See [:material-code-brackets: UserRoleType](./literals.md#userroletype) 
## PutAccessControlRuleRequestRequestTypeDef

```python
# PutAccessControlRuleRequestRequestTypeDef definition

class PutAccessControlRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    Effect: AccessControlRuleEffectType,  # (1)
    Description: str,
    OrganizationId: str,
    IpRanges: NotRequired[Sequence[str]],
    NotIpRanges: NotRequired[Sequence[str]],
    Actions: NotRequired[Sequence[str]],
    NotActions: NotRequired[Sequence[str]],
    UserIds: NotRequired[Sequence[str]],
    NotUserIds: NotRequired[Sequence[str]],
    ImpersonationRoleIds: NotRequired[Sequence[str]],
    NotImpersonationRoleIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AccessControlRuleEffectType](./literals.md#accesscontrolruleeffecttype) 
## PutEmailMonitoringConfigurationRequestRequestTypeDef

```python
# PutEmailMonitoringConfigurationRequestRequestTypeDef definition

class PutEmailMonitoringConfigurationRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    RoleArn: str,
    LogGroupArn: str,
```

## PutInboundDmarcSettingsRequestRequestTypeDef

```python
# PutInboundDmarcSettingsRequestRequestTypeDef definition

class PutInboundDmarcSettingsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Enforced: bool,
```

## PutMailboxPermissionsRequestRequestTypeDef

```python
# PutMailboxPermissionsRequestRequestTypeDef definition

class PutMailboxPermissionsRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
    GranteeId: str,
    PermissionValues: Sequence[PermissionTypeType],  # (1)
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
## PutMobileDeviceAccessOverrideRequestRequestTypeDef

```python
# PutMobileDeviceAccessOverrideRequestRequestTypeDef definition

class PutMobileDeviceAccessOverrideRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    UserId: str,
    DeviceId: str,
    Effect: MobileDeviceAccessRuleEffectType,  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype) 
## RegisterMailDomainRequestRequestTypeDef

```python
# RegisterMailDomainRequestRequestTypeDef definition

class RegisterMailDomainRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    DomainName: str,
    ClientToken: NotRequired[str],
```

## RegisterToWorkMailRequestRequestTypeDef

```python
# RegisterToWorkMailRequestRequestTypeDef definition

class RegisterToWorkMailRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
    Email: str,
```

## ResetPasswordRequestRequestTypeDef

```python
# ResetPasswordRequestRequestTypeDef definition

class ResetPasswordRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    UserId: str,
    Password: str,
```

## StartMailboxExportJobRequestRequestTypeDef

```python
# StartMailboxExportJobRequestRequestTypeDef definition

class StartMailboxExportJobRequestRequestTypeDef(TypedDict):
    ClientToken: str,
    OrganizationId: str,
    EntityId: str,
    RoleArn: str,
    KmsKeyArn: str,
    S3BucketName: str,
    S3Prefix: str,
    Description: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateDefaultMailDomainRequestRequestTypeDef

```python
# UpdateDefaultMailDomainRequestRequestTypeDef definition

class UpdateDefaultMailDomainRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    DomainName: str,
```

## UpdateMailboxQuotaRequestRequestTypeDef

```python
# UpdateMailboxQuotaRequestRequestTypeDef definition

class UpdateMailboxQuotaRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    UserId: str,
    MailboxQuota: int,
```

## UpdateMobileDeviceAccessRuleRequestRequestTypeDef

```python
# UpdateMobileDeviceAccessRuleRequestRequestTypeDef definition

class UpdateMobileDeviceAccessRuleRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    MobileDeviceAccessRuleId: str,
    Name: str,
    Effect: MobileDeviceAccessRuleEffectType,  # (1)
    Description: NotRequired[str],
    DeviceTypes: NotRequired[Sequence[str]],
    NotDeviceTypes: NotRequired[Sequence[str]],
    DeviceModels: NotRequired[Sequence[str]],
    NotDeviceModels: NotRequired[Sequence[str]],
    DeviceOperatingSystems: NotRequired[Sequence[str]],
    NotDeviceOperatingSystems: NotRequired[Sequence[str]],
    DeviceUserAgents: NotRequired[Sequence[str]],
    NotDeviceUserAgents: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype) 
## UpdatePrimaryEmailAddressRequestRequestTypeDef

```python
# UpdatePrimaryEmailAddressRequestRequestTypeDef definition

class UpdatePrimaryEmailAddressRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
    Email: str,
```

## AssumeImpersonationRoleResponseTypeDef

```python
# AssumeImpersonationRoleResponseTypeDef definition

class AssumeImpersonationRoleResponseTypeDef(TypedDict):
    Token: str,
    ExpiresIn: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupResponseTypeDef

```python
# CreateGroupResponseTypeDef definition

class CreateGroupResponseTypeDef(TypedDict):
    GroupId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateImpersonationRoleResponseTypeDef

```python
# CreateImpersonationRoleResponseTypeDef definition

class CreateImpersonationRoleResponseTypeDef(TypedDict):
    ImpersonationRoleId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMobileDeviceAccessRuleResponseTypeDef

```python
# CreateMobileDeviceAccessRuleResponseTypeDef definition

class CreateMobileDeviceAccessRuleResponseTypeDef(TypedDict):
    MobileDeviceAccessRuleId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOrganizationResponseTypeDef

```python
# CreateOrganizationResponseTypeDef definition

class CreateOrganizationResponseTypeDef(TypedDict):
    OrganizationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceResponseTypeDef

```python
# CreateResourceResponseTypeDef definition

class CreateResourceResponseTypeDef(TypedDict):
    ResourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserResponseTypeDef

```python
# CreateUserResponseTypeDef definition

class CreateUserResponseTypeDef(TypedDict):
    UserId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteOrganizationResponseTypeDef

```python
# DeleteOrganizationResponseTypeDef definition

class DeleteOrganizationResponseTypeDef(TypedDict):
    OrganizationId: str,
    State: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEmailMonitoringConfigurationResponseTypeDef

```python
# DescribeEmailMonitoringConfigurationResponseTypeDef definition

class DescribeEmailMonitoringConfigurationResponseTypeDef(TypedDict):
    RoleArn: str,
    LogGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGroupResponseTypeDef

```python
# DescribeGroupResponseTypeDef definition

class DescribeGroupResponseTypeDef(TypedDict):
    GroupId: str,
    Name: str,
    Email: str,
    State: EntityStateType,  # (1)
    EnabledDate: datetime,
    DisabledDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EntityStateType](./literals.md#entitystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInboundDmarcSettingsResponseTypeDef

```python
# DescribeInboundDmarcSettingsResponseTypeDef definition

class DescribeInboundDmarcSettingsResponseTypeDef(TypedDict):
    Enforced: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMailboxExportJobResponseTypeDef

```python
# DescribeMailboxExportJobResponseTypeDef definition

class DescribeMailboxExportJobResponseTypeDef(TypedDict):
    EntityId: str,
    Description: str,
    RoleArn: str,
    KmsKeyArn: str,
    S3BucketName: str,
    S3Prefix: str,
    S3Path: str,
    EstimatedProgress: int,
    State: MailboxExportJobStateType,  # (1)
    ErrorInfo: str,
    StartTime: datetime,
    EndTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MailboxExportJobStateType](./literals.md#mailboxexportjobstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationResponseTypeDef

```python
# DescribeOrganizationResponseTypeDef definition

class DescribeOrganizationResponseTypeDef(TypedDict):
    OrganizationId: str,
    Alias: str,
    State: str,
    DirectoryId: str,
    DirectoryType: str,
    DefaultMailDomain: str,
    CompletedDate: datetime,
    ErrorMessage: str,
    ARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserResponseTypeDef

```python
# DescribeUserResponseTypeDef definition

class DescribeUserResponseTypeDef(TypedDict):
    UserId: str,
    Name: str,
    Email: str,
    DisplayName: str,
    State: EntityStateType,  # (1)
    UserRole: UserRoleType,  # (2)
    EnabledDate: datetime,
    DisabledDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EntityStateType](./literals.md#entitystatetype) 
2. See [:material-code-brackets: UserRoleType](./literals.md#userroletype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccessControlEffectResponseTypeDef

```python
# GetAccessControlEffectResponseTypeDef definition

class GetAccessControlEffectResponseTypeDef(TypedDict):
    Effect: AccessControlRuleEffectType,  # (1)
    MatchedRules: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AccessControlRuleEffectType](./literals.md#accesscontrolruleeffecttype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMailboxDetailsResponseTypeDef

```python
# GetMailboxDetailsResponseTypeDef definition

class GetMailboxDetailsResponseTypeDef(TypedDict):
    MailboxQuota: int,
    MailboxSize: float,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMobileDeviceAccessOverrideResponseTypeDef

```python
# GetMobileDeviceAccessOverrideResponseTypeDef definition

class GetMobileDeviceAccessOverrideResponseTypeDef(TypedDict):
    UserId: str,
    DeviceId: str,
    Effect: MobileDeviceAccessRuleEffectType,  # (1)
    Description: str,
    DateCreated: datetime,
    DateModified: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessControlRulesResponseTypeDef

```python
# ListAccessControlRulesResponseTypeDef definition

class ListAccessControlRulesResponseTypeDef(TypedDict):
    Rules: List[AccessControlRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessControlRuleTypeDef](./type_defs.md#accesscontrolruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAliasesResponseTypeDef

```python
# ListAliasesResponseTypeDef definition

class ListAliasesResponseTypeDef(TypedDict):
    Aliases: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMailboxExportJobResponseTypeDef

```python
# StartMailboxExportJobResponseTypeDef definition

class StartMailboxExportJobResponseTypeDef(TypedDict):
    JobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestAvailabilityConfigurationResponseTypeDef

```python
# TestAvailabilityConfigurationResponseTypeDef definition

class TestAvailabilityConfigurationResponseTypeDef(TypedDict):
    TestPassed: bool,
    FailureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AvailabilityConfigurationTypeDef

```python
# AvailabilityConfigurationTypeDef definition

class AvailabilityConfigurationTypeDef(TypedDict):
    DomainName: NotRequired[str],
    ProviderType: NotRequired[AvailabilityProviderTypeType],  # (1)
    EwsProvider: NotRequired[RedactedEwsAvailabilityProviderTypeDef],  # (2)
    LambdaProvider: NotRequired[LambdaAvailabilityProviderTypeDef],  # (3)
    DateCreated: NotRequired[datetime],
    DateModified: NotRequired[datetime],
```

1. See [:material-code-brackets: AvailabilityProviderTypeType](./literals.md#availabilityprovidertypetype) 
2. See [:material-code-braces: RedactedEwsAvailabilityProviderTypeDef](./type_defs.md#redactedewsavailabilityprovidertypedef) 
3. See [:material-code-braces: LambdaAvailabilityProviderTypeDef](./type_defs.md#lambdaavailabilityprovidertypedef) 
## DescribeResourceResponseTypeDef

```python
# DescribeResourceResponseTypeDef definition

class DescribeResourceResponseTypeDef(TypedDict):
    ResourceId: str,
    Email: str,
    Name: str,
    Type: ResourceTypeType,  # (1)
    BookingOptions: BookingOptionsTypeDef,  # (2)
    State: EntityStateType,  # (3)
    EnabledDate: datetime,
    DisabledDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: BookingOptionsTypeDef](./type_defs.md#bookingoptionstypedef) 
3. See [:material-code-brackets: EntityStateType](./literals.md#entitystatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResourceRequestRequestTypeDef

```python
# UpdateResourceRequestRequestTypeDef definition

class UpdateResourceRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ResourceId: str,
    Name: NotRequired[str],
    BookingOptions: NotRequired[BookingOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: BookingOptionsTypeDef](./type_defs.md#bookingoptionstypedef) 
## CreateAvailabilityConfigurationRequestRequestTypeDef

```python
# CreateAvailabilityConfigurationRequestRequestTypeDef definition

class CreateAvailabilityConfigurationRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    DomainName: str,
    ClientToken: NotRequired[str],
    EwsProvider: NotRequired[EwsAvailabilityProviderTypeDef],  # (1)
    LambdaProvider: NotRequired[LambdaAvailabilityProviderTypeDef],  # (2)
```

1. See [:material-code-braces: EwsAvailabilityProviderTypeDef](./type_defs.md#ewsavailabilityprovidertypedef) 
2. See [:material-code-braces: LambdaAvailabilityProviderTypeDef](./type_defs.md#lambdaavailabilityprovidertypedef) 
## TestAvailabilityConfigurationRequestRequestTypeDef

```python
# TestAvailabilityConfigurationRequestRequestTypeDef definition

class TestAvailabilityConfigurationRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    DomainName: NotRequired[str],
    EwsProvider: NotRequired[EwsAvailabilityProviderTypeDef],  # (1)
    LambdaProvider: NotRequired[LambdaAvailabilityProviderTypeDef],  # (2)
```

1. See [:material-code-braces: EwsAvailabilityProviderTypeDef](./type_defs.md#ewsavailabilityprovidertypedef) 
2. See [:material-code-braces: LambdaAvailabilityProviderTypeDef](./type_defs.md#lambdaavailabilityprovidertypedef) 
## UpdateAvailabilityConfigurationRequestRequestTypeDef

```python
# UpdateAvailabilityConfigurationRequestRequestTypeDef definition

class UpdateAvailabilityConfigurationRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    DomainName: str,
    EwsProvider: NotRequired[EwsAvailabilityProviderTypeDef],  # (1)
    LambdaProvider: NotRequired[LambdaAvailabilityProviderTypeDef],  # (2)
```

1. See [:material-code-braces: EwsAvailabilityProviderTypeDef](./type_defs.md#ewsavailabilityprovidertypedef) 
2. See [:material-code-braces: LambdaAvailabilityProviderTypeDef](./type_defs.md#lambdaavailabilityprovidertypedef) 
## CreateImpersonationRoleRequestRequestTypeDef

```python
# CreateImpersonationRoleRequestRequestTypeDef definition

class CreateImpersonationRoleRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Name: str,
    Type: ImpersonationRoleTypeType,  # (1)
    Rules: Sequence[ImpersonationRuleTypeDef],  # (2)
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ImpersonationRoleTypeType](./literals.md#impersonationroletypetype) 
2. See [:material-code-braces: ImpersonationRuleTypeDef](./type_defs.md#impersonationruletypedef) 
## GetImpersonationRoleResponseTypeDef

```python
# GetImpersonationRoleResponseTypeDef definition

class GetImpersonationRoleResponseTypeDef(TypedDict):
    ImpersonationRoleId: str,
    Name: str,
    Type: ImpersonationRoleTypeType,  # (1)
    Description: str,
    Rules: List[ImpersonationRuleTypeDef],  # (2)
    DateCreated: datetime,
    DateModified: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ImpersonationRoleTypeType](./literals.md#impersonationroletypetype) 
2. See [:material-code-braces: ImpersonationRuleTypeDef](./type_defs.md#impersonationruletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateImpersonationRoleRequestRequestTypeDef

```python
# UpdateImpersonationRoleRequestRequestTypeDef definition

class UpdateImpersonationRoleRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    ImpersonationRoleId: str,
    Name: str,
    Type: ImpersonationRoleTypeType,  # (1)
    Rules: Sequence[ImpersonationRuleTypeDef],  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ImpersonationRoleTypeType](./literals.md#impersonationroletypetype) 
2. See [:material-code-braces: ImpersonationRuleTypeDef](./type_defs.md#impersonationruletypedef) 
## CreateOrganizationRequestRequestTypeDef

```python
# CreateOrganizationRequestRequestTypeDef definition

class CreateOrganizationRequestRequestTypeDef(TypedDict):
    Alias: str,
    DirectoryId: NotRequired[str],
    ClientToken: NotRequired[str],
    Domains: NotRequired[Sequence[DomainTypeDef]],  # (1)
    KmsKeyArn: NotRequired[str],
    EnableInteroperability: NotRequired[bool],
```

1. See [:material-code-braces: DomainTypeDef](./type_defs.md#domaintypedef) 
## ListResourceDelegatesResponseTypeDef

```python
# ListResourceDelegatesResponseTypeDef definition

class ListResourceDelegatesResponseTypeDef(TypedDict):
    Delegates: List[DelegateTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DelegateTypeDef](./type_defs.md#delegatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMailDomainResponseTypeDef

```python
# GetMailDomainResponseTypeDef definition

class GetMailDomainResponseTypeDef(TypedDict):
    Records: List[DnsRecordTypeDef],  # (1)
    IsTestDomain: bool,
    IsDefault: bool,
    OwnershipVerificationStatus: DnsRecordVerificationStatusType,  # (2)
    DkimVerificationStatus: DnsRecordVerificationStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DnsRecordTypeDef](./type_defs.md#dnsrecordtypedef) 
2. See [:material-code-brackets: DnsRecordVerificationStatusType](./literals.md#dnsrecordverificationstatustype) 
3. See [:material-code-brackets: DnsRecordVerificationStatusType](./literals.md#dnsrecordverificationstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDefaultRetentionPolicyResponseTypeDef

```python
# GetDefaultRetentionPolicyResponseTypeDef definition

class GetDefaultRetentionPolicyResponseTypeDef(TypedDict):
    Id: str,
    Name: str,
    Description: str,
    FolderConfigurations: List[FolderConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FolderConfigurationTypeDef](./type_defs.md#folderconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRetentionPolicyRequestRequestTypeDef

```python
# PutRetentionPolicyRequestRequestTypeDef definition

class PutRetentionPolicyRequestRequestTypeDef(TypedDict):
    OrganizationId: str,
    Name: str,
    FolderConfigurations: Sequence[FolderConfigurationTypeDef],  # (1)
    Id: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-braces: FolderConfigurationTypeDef](./type_defs.md#folderconfigurationtypedef) 
## GetImpersonationRoleEffectResponseTypeDef

```python
# GetImpersonationRoleEffectResponseTypeDef definition

class GetImpersonationRoleEffectResponseTypeDef(TypedDict):
    Type: ImpersonationRoleTypeType,  # (1)
    Effect: AccessEffectType,  # (2)
    MatchedRules: List[ImpersonationMatchedRuleTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ImpersonationRoleTypeType](./literals.md#impersonationroletypetype) 
2. See [:material-code-brackets: AccessEffectType](./literals.md#accesseffecttype) 
3. See [:material-code-braces: ImpersonationMatchedRuleTypeDef](./type_defs.md#impersonationmatchedruletypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMobileDeviceAccessEffectResponseTypeDef

```python
# GetMobileDeviceAccessEffectResponseTypeDef definition

class GetMobileDeviceAccessEffectResponseTypeDef(TypedDict):
    Effect: MobileDeviceAccessRuleEffectType,  # (1)
    MatchedRules: List[MobileDeviceAccessMatchedRuleTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MobileDeviceAccessRuleEffectType](./literals.md#mobiledeviceaccessruleeffecttype) 
2. See [:material-code-braces: MobileDeviceAccessMatchedRuleTypeDef](./type_defs.md#mobiledeviceaccessmatchedruletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## ListImpersonationRolesResponseTypeDef

```python
# ListImpersonationRolesResponseTypeDef definition

class ListImpersonationRolesResponseTypeDef(TypedDict):
    Roles: List[ImpersonationRoleTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImpersonationRoleTypeDef](./type_defs.md#impersonationroletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAliasesRequestListAliasesPaginateTypeDef

```python
# ListAliasesRequestListAliasesPaginateTypeDef definition

class ListAliasesRequestListAliasesPaginateTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef

```python
# ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef definition

class ListAvailabilityConfigurationsRequestListAvailabilityConfigurationsPaginateTypeDef(TypedDict):
    OrganizationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupMembersRequestListGroupMembersPaginateTypeDef

```python
# ListGroupMembersRequestListGroupMembersPaginateTypeDef definition

class ListGroupMembersRequestListGroupMembersPaginateTypeDef(TypedDict):
    OrganizationId: str,
    GroupId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupsRequestListGroupsPaginateTypeDef

```python
# ListGroupsRequestListGroupsPaginateTypeDef definition

class ListGroupsRequestListGroupsPaginateTypeDef(TypedDict):
    OrganizationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef

```python
# ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef definition

class ListMailboxPermissionsRequestListMailboxPermissionsPaginateTypeDef(TypedDict):
    OrganizationId: str,
    EntityId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationsRequestListOrganizationsPaginateTypeDef

```python
# ListOrganizationsRequestListOrganizationsPaginateTypeDef definition

class ListOrganizationsRequestListOrganizationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef

```python
# ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef definition

class ListResourceDelegatesRequestListResourceDelegatesPaginateTypeDef(TypedDict):
    OrganizationId: str,
    ResourceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourcesRequestListResourcesPaginateTypeDef

```python
# ListResourcesRequestListResourcesPaginateTypeDef definition

class ListResourcesRequestListResourcesPaginateTypeDef(TypedDict):
    OrganizationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsersRequestListUsersPaginateTypeDef

```python
# ListUsersRequestListUsersPaginateTypeDef definition

class ListUsersRequestListUsersPaginateTypeDef(TypedDict):
    OrganizationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupMembersResponseTypeDef

```python
# ListGroupMembersResponseTypeDef definition

class ListGroupMembersResponseTypeDef(TypedDict):
    Members: List[MemberTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMailDomainsResponseTypeDef

```python
# ListMailDomainsResponseTypeDef definition

class ListMailDomainsResponseTypeDef(TypedDict):
    MailDomains: List[MailDomainSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MailDomainSummaryTypeDef](./type_defs.md#maildomainsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMailboxExportJobsResponseTypeDef

```python
# ListMailboxExportJobsResponseTypeDef definition

class ListMailboxExportJobsResponseTypeDef(TypedDict):
    Jobs: List[MailboxExportJobTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MailboxExportJobTypeDef](./type_defs.md#mailboxexportjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMailboxPermissionsResponseTypeDef

```python
# ListMailboxPermissionsResponseTypeDef definition

class ListMailboxPermissionsResponseTypeDef(TypedDict):
    Permissions: List[PermissionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionTypeDef](./type_defs.md#permissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMobileDeviceAccessOverridesResponseTypeDef

```python
# ListMobileDeviceAccessOverridesResponseTypeDef definition

class ListMobileDeviceAccessOverridesResponseTypeDef(TypedDict):
    Overrides: List[MobileDeviceAccessOverrideTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MobileDeviceAccessOverrideTypeDef](./type_defs.md#mobiledeviceaccessoverridetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMobileDeviceAccessRulesResponseTypeDef

```python
# ListMobileDeviceAccessRulesResponseTypeDef definition

class ListMobileDeviceAccessRulesResponseTypeDef(TypedDict):
    Rules: List[MobileDeviceAccessRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MobileDeviceAccessRuleTypeDef](./type_defs.md#mobiledeviceaccessruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrganizationsResponseTypeDef

```python
# ListOrganizationsResponseTypeDef definition

class ListOrganizationsResponseTypeDef(TypedDict):
    OrganizationSummaries: List[OrganizationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationSummaryTypeDef](./type_defs.md#organizationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesResponseTypeDef

```python
# ListResourcesResponseTypeDef definition

class ListResourcesResponseTypeDef(TypedDict):
    Resources: List[ResourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
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
## ListAvailabilityConfigurationsResponseTypeDef

```python
# ListAvailabilityConfigurationsResponseTypeDef definition

class ListAvailabilityConfigurationsResponseTypeDef(TypedDict):
    AvailabilityConfigurations: List[AvailabilityConfigurationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AvailabilityConfigurationTypeDef](./type_defs.md#availabilityconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
