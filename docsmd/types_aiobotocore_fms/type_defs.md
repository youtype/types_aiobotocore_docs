# Type definitions

> [Index](../README.md) > [FMS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [FMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
    type annotations stubs module [types-aiobotocore-fms](https://pypi.org/project/types-aiobotocore-fms/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AccountScopeTypeDef

```python
# AccountScopeTypeDef definition

class AccountScopeTypeDef(TypedDict):
    Accounts: NotRequired[List[str]],
    AllAccountsEnabled: NotRequired[bool],
    ExcludeSpecifiedAccounts: NotRequired[bool],
```

## ActionTargetTypeDef

```python
# ActionTargetTypeDef definition

class ActionTargetTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    Description: NotRequired[str],
```

## AdminAccountSummaryTypeDef

```python
# AdminAccountSummaryTypeDef definition

class AdminAccountSummaryTypeDef(TypedDict):
    AdminAccount: NotRequired[str],
    DefaultAdmin: NotRequired[bool],
    Status: NotRequired[OrganizationStatusType],  # (1)
```

1. See [:material-code-brackets: OrganizationStatusType](./literals.md#organizationstatustype) 
## OrganizationalUnitScopeTypeDef

```python
# OrganizationalUnitScopeTypeDef definition

class OrganizationalUnitScopeTypeDef(TypedDict):
    OrganizationalUnits: NotRequired[List[str]],
    AllOrganizationalUnitsEnabled: NotRequired[bool],
    ExcludeSpecifiedOrganizationalUnits: NotRequired[bool],
```

## PolicyTypeScopeTypeDef

```python
# PolicyTypeScopeTypeDef definition

class PolicyTypeScopeTypeDef(TypedDict):
    PolicyTypes: NotRequired[List[SecurityServiceTypeType]],  # (1)
    AllPolicyTypesEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: SecurityServiceTypeType](./literals.md#securityservicetypetype) 
## RegionScopeTypeDef

```python
# RegionScopeTypeDef definition

class RegionScopeTypeDef(TypedDict):
    Regions: NotRequired[List[str]],
    AllRegionsEnabled: NotRequired[bool],
```

## AppTypeDef

```python
# AppTypeDef definition

class AppTypeDef(TypedDict):
    AppName: str,
    Protocol: str,
    Port: int,
```

## AssociateAdminAccountRequestRequestTypeDef

```python
# AssociateAdminAccountRequestRequestTypeDef definition

class AssociateAdminAccountRequestRequestTypeDef(TypedDict):
    AdminAccount: str,
```

## AssociateThirdPartyFirewallRequestRequestTypeDef

```python
# AssociateThirdPartyFirewallRequestRequestTypeDef definition

class AssociateThirdPartyFirewallRequestRequestTypeDef(TypedDict):
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
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

## AwsEc2NetworkInterfaceViolationTypeDef

```python
# AwsEc2NetworkInterfaceViolationTypeDef definition

class AwsEc2NetworkInterfaceViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    ViolatingSecurityGroups: NotRequired[List[str]],
```

## PartialMatchTypeDef

```python
# PartialMatchTypeDef definition

class PartialMatchTypeDef(TypedDict):
    Reference: NotRequired[str],
    TargetViolationReasons: NotRequired[List[str]],
```

## BatchAssociateResourceRequestRequestTypeDef

```python
# BatchAssociateResourceRequestRequestTypeDef definition

class BatchAssociateResourceRequestRequestTypeDef(TypedDict):
    ResourceSetIdentifier: str,
    Items: Sequence[str],
```

## FailedItemTypeDef

```python
# FailedItemTypeDef definition

class FailedItemTypeDef(TypedDict):
    URI: NotRequired[str],
    Reason: NotRequired[FailedItemReasonType],  # (1)
```

1. See [:material-code-brackets: FailedItemReasonType](./literals.md#faileditemreasontype) 
## BatchDisassociateResourceRequestRequestTypeDef

```python
# BatchDisassociateResourceRequestRequestTypeDef definition

class BatchDisassociateResourceRequestRequestTypeDef(TypedDict):
    ResourceSetIdentifier: str,
    Items: Sequence[str],
```

## ComplianceViolatorTypeDef

```python
# ComplianceViolatorTypeDef definition

class ComplianceViolatorTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    ViolationReason: NotRequired[ViolationReasonType],  # (1)
    ResourceType: NotRequired[str],
    Metadata: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ViolationReasonType](./literals.md#violationreasontype) 
## DeleteAppsListRequestRequestTypeDef

```python
# DeleteAppsListRequestRequestTypeDef definition

class DeleteAppsListRequestRequestTypeDef(TypedDict):
    ListId: str,
```

## DeletePolicyRequestRequestTypeDef

```python
# DeletePolicyRequestRequestTypeDef definition

class DeletePolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    DeleteAllPolicyResources: NotRequired[bool],
```

## DeleteProtocolsListRequestRequestTypeDef

```python
# DeleteProtocolsListRequestRequestTypeDef definition

class DeleteProtocolsListRequestRequestTypeDef(TypedDict):
    ListId: str,
```

## DeleteResourceSetRequestRequestTypeDef

```python
# DeleteResourceSetRequestRequestTypeDef definition

class DeleteResourceSetRequestRequestTypeDef(TypedDict):
    Identifier: str,
```

## DisassociateThirdPartyFirewallRequestRequestTypeDef

```python
# DisassociateThirdPartyFirewallRequestRequestTypeDef definition

class DisassociateThirdPartyFirewallRequestRequestTypeDef(TypedDict):
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
## DiscoveredResourceTypeDef

```python
# DiscoveredResourceTypeDef definition

class DiscoveredResourceTypeDef(TypedDict):
    URI: NotRequired[str],
    AccountId: NotRequired[str],
    Type: NotRequired[str],
    Name: NotRequired[str],
```

## DnsDuplicateRuleGroupViolationTypeDef

```python
# DnsDuplicateRuleGroupViolationTypeDef definition

class DnsDuplicateRuleGroupViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    ViolationTargetDescription: NotRequired[str],
```

## DnsRuleGroupLimitExceededViolationTypeDef

```python
# DnsRuleGroupLimitExceededViolationTypeDef definition

class DnsRuleGroupLimitExceededViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    ViolationTargetDescription: NotRequired[str],
    NumberOfRuleGroupsAlreadyAssociated: NotRequired[int],
```

## DnsRuleGroupPriorityConflictViolationTypeDef

```python
# DnsRuleGroupPriorityConflictViolationTypeDef definition

class DnsRuleGroupPriorityConflictViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    ViolationTargetDescription: NotRequired[str],
    ConflictingPriority: NotRequired[int],
    ConflictingPolicyId: NotRequired[str],
    UnavailablePriorities: NotRequired[List[int]],
```

## EvaluationResultTypeDef

```python
# EvaluationResultTypeDef definition

class EvaluationResultTypeDef(TypedDict):
    ComplianceStatus: NotRequired[PolicyComplianceStatusTypeType],  # (1)
    ViolatorCount: NotRequired[int],
    EvaluationLimitExceeded: NotRequired[bool],
```

1. See [:material-code-brackets: PolicyComplianceStatusTypeType](./literals.md#policycompliancestatustypetype) 
## ExpectedRouteTypeDef

```python
# ExpectedRouteTypeDef definition

class ExpectedRouteTypeDef(TypedDict):
    IpV4Cidr: NotRequired[str],
    PrefixListId: NotRequired[str],
    IpV6Cidr: NotRequired[str],
    ContributingSubnets: NotRequired[List[str]],
    AllowedTargets: NotRequired[List[str]],
    RouteTableId: NotRequired[str],
```

## FMSPolicyUpdateFirewallCreationConfigActionTypeDef

```python
# FMSPolicyUpdateFirewallCreationConfigActionTypeDef definition

class FMSPolicyUpdateFirewallCreationConfigActionTypeDef(TypedDict):
    Description: NotRequired[str],
    FirewallCreationConfig: NotRequired[str],
```

## FirewallSubnetIsOutOfScopeViolationTypeDef

```python
# FirewallSubnetIsOutOfScopeViolationTypeDef definition

class FirewallSubnetIsOutOfScopeViolationTypeDef(TypedDict):
    FirewallSubnetId: NotRequired[str],
    VpcId: NotRequired[str],
    SubnetAvailabilityZone: NotRequired[str],
    SubnetAvailabilityZoneId: NotRequired[str],
    VpcEndpointId: NotRequired[str],
```

## FirewallSubnetMissingVPCEndpointViolationTypeDef

```python
# FirewallSubnetMissingVPCEndpointViolationTypeDef definition

class FirewallSubnetMissingVPCEndpointViolationTypeDef(TypedDict):
    FirewallSubnetId: NotRequired[str],
    VpcId: NotRequired[str],
    SubnetAvailabilityZone: NotRequired[str],
    SubnetAvailabilityZoneId: NotRequired[str],
```

## GetAdminScopeRequestRequestTypeDef

```python
# GetAdminScopeRequestRequestTypeDef definition

class GetAdminScopeRequestRequestTypeDef(TypedDict):
    AdminAccount: str,
```

## GetAppsListRequestRequestTypeDef

```python
# GetAppsListRequestRequestTypeDef definition

class GetAppsListRequestRequestTypeDef(TypedDict):
    ListId: str,
    DefaultList: NotRequired[bool],
```

## GetComplianceDetailRequestRequestTypeDef

```python
# GetComplianceDetailRequestRequestTypeDef definition

class GetComplianceDetailRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    MemberAccount: str,
```

## GetPolicyRequestRequestTypeDef

```python
# GetPolicyRequestRequestTypeDef definition

class GetPolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
```

## GetProtocolsListRequestRequestTypeDef

```python
# GetProtocolsListRequestRequestTypeDef definition

class GetProtocolsListRequestRequestTypeDef(TypedDict):
    ListId: str,
    DefaultList: NotRequired[bool],
```

## ProtocolsListDataTypeDef

```python
# ProtocolsListDataTypeDef definition

class ProtocolsListDataTypeDef(TypedDict):
    ListName: str,
    ProtocolsList: List[str],
    ListId: NotRequired[str],
    ListUpdateToken: NotRequired[str],
    CreateTime: NotRequired[datetime],
    LastUpdateTime: NotRequired[datetime],
    PreviousProtocolsList: NotRequired[Dict[str, List[str]]],
```

## GetResourceSetRequestRequestTypeDef

```python
# GetResourceSetRequestRequestTypeDef definition

class GetResourceSetRequestRequestTypeDef(TypedDict):
    Identifier: str,
```

## ResourceSetTypeDef

```python
# ResourceSetTypeDef definition

class ResourceSetTypeDef(TypedDict):
    Name: str,
    ResourceTypeList: List[str],
    Id: NotRequired[str],
    Description: NotRequired[str],
    UpdateToken: NotRequired[str],
    LastUpdateTime: NotRequired[datetime],
    ResourceSetStatus: NotRequired[ResourceSetStatusType],  # (1)
```

1. See [:material-code-brackets: ResourceSetStatusType](./literals.md#resourcesetstatustype) 
## GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef

```python
# GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef definition

class GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef(TypedDict):
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
## GetViolationDetailsRequestRequestTypeDef

```python
# GetViolationDetailsRequestRequestTypeDef definition

class GetViolationDetailsRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    MemberAccount: str,
    ResourceId: str,
    ResourceType: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAdminAccountsForOrganizationRequestRequestTypeDef

```python
# ListAdminAccountsForOrganizationRequestRequestTypeDef definition

class ListAdminAccountsForOrganizationRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAdminsManagingAccountRequestRequestTypeDef

```python
# ListAdminsManagingAccountRequestRequestTypeDef definition

class ListAdminsManagingAccountRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListAppsListsRequestRequestTypeDef

```python
# ListAppsListsRequestRequestTypeDef definition

class ListAppsListsRequestRequestTypeDef(TypedDict):
    MaxResults: int,
    DefaultLists: NotRequired[bool],
    NextToken: NotRequired[str],
```

## ListComplianceStatusRequestRequestTypeDef

```python
# ListComplianceStatusRequestRequestTypeDef definition

class ListComplianceStatusRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDiscoveredResourcesRequestRequestTypeDef

```python
# ListDiscoveredResourcesRequestRequestTypeDef definition

class ListDiscoveredResourcesRequestRequestTypeDef(TypedDict):
    MemberAccountIds: Sequence[str],
    ResourceType: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListMemberAccountsRequestRequestTypeDef

```python
# ListMemberAccountsRequestRequestTypeDef definition

class ListMemberAccountsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPoliciesRequestRequestTypeDef

```python
# ListPoliciesRequestRequestTypeDef definition

class ListPoliciesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PolicySummaryTypeDef

```python
# PolicySummaryTypeDef definition

class PolicySummaryTypeDef(TypedDict):
    PolicyArn: NotRequired[str],
    PolicyId: NotRequired[str],
    PolicyName: NotRequired[str],
    ResourceType: NotRequired[str],
    SecurityServiceType: NotRequired[SecurityServiceTypeType],  # (1)
    RemediationEnabled: NotRequired[bool],
    DeleteUnusedFMManagedResources: NotRequired[bool],
    PolicyStatus: NotRequired[CustomerPolicyStatusType],  # (2)
```

1. See [:material-code-brackets: SecurityServiceTypeType](./literals.md#securityservicetypetype) 
2. See [:material-code-brackets: CustomerPolicyStatusType](./literals.md#customerpolicystatustype) 
## ListProtocolsListsRequestRequestTypeDef

```python
# ListProtocolsListsRequestRequestTypeDef definition

class ListProtocolsListsRequestRequestTypeDef(TypedDict):
    MaxResults: int,
    DefaultLists: NotRequired[bool],
    NextToken: NotRequired[str],
```

## ProtocolsListDataSummaryTypeDef

```python
# ProtocolsListDataSummaryTypeDef definition

class ProtocolsListDataSummaryTypeDef(TypedDict):
    ListArn: NotRequired[str],
    ListId: NotRequired[str],
    ListName: NotRequired[str],
    ProtocolsList: NotRequired[List[str]],
```

## ListResourceSetResourcesRequestRequestTypeDef

```python
# ListResourceSetResourcesRequestRequestTypeDef definition

class ListResourceSetResourcesRequestRequestTypeDef(TypedDict):
    Identifier: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    URI: str,
    AccountId: NotRequired[str],
```

## ListResourceSetsRequestRequestTypeDef

```python
# ListResourceSetsRequestRequestTypeDef definition

class ListResourceSetsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ResourceSetSummaryTypeDef

```python
# ResourceSetSummaryTypeDef definition

class ResourceSetSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    LastUpdateTime: NotRequired[datetime],
    ResourceSetStatus: NotRequired[ResourceSetStatusType],  # (1)
```

1. See [:material-code-brackets: ResourceSetStatusType](./literals.md#resourcesetstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef

```python
# ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef definition

class ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef(TypedDict):
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
    MaxResults: int,
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
## ThirdPartyFirewallFirewallPolicyTypeDef

```python
# ThirdPartyFirewallFirewallPolicyTypeDef definition

class ThirdPartyFirewallFirewallPolicyTypeDef(TypedDict):
    FirewallPolicyId: NotRequired[str],
    FirewallPolicyName: NotRequired[str],
```

## RouteTypeDef

```python
# RouteTypeDef definition

class RouteTypeDef(TypedDict):
    DestinationType: NotRequired[DestinationTypeType],  # (1)
    TargetType: NotRequired[TargetTypeType],  # (2)
    Destination: NotRequired[str],
    Target: NotRequired[str],
```

1. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
2. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
## NetworkFirewallMissingExpectedRTViolationTypeDef

```python
# NetworkFirewallMissingExpectedRTViolationTypeDef definition

class NetworkFirewallMissingExpectedRTViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    VPC: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    CurrentRouteTable: NotRequired[str],
    ExpectedRouteTable: NotRequired[str],
```

## NetworkFirewallMissingFirewallViolationTypeDef

```python
# NetworkFirewallMissingFirewallViolationTypeDef definition

class NetworkFirewallMissingFirewallViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    VPC: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    TargetViolationReason: NotRequired[str],
```

## NetworkFirewallMissingSubnetViolationTypeDef

```python
# NetworkFirewallMissingSubnetViolationTypeDef definition

class NetworkFirewallMissingSubnetViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    VPC: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    TargetViolationReason: NotRequired[str],
```

## StatefulEngineOptionsTypeDef

```python
# StatefulEngineOptionsTypeDef definition

class StatefulEngineOptionsTypeDef(TypedDict):
    RuleOrder: NotRequired[RuleOrderType],  # (1)
```

1. See [:material-code-brackets: RuleOrderType](./literals.md#ruleordertype) 
## StatelessRuleGroupTypeDef

```python
# StatelessRuleGroupTypeDef definition

class StatelessRuleGroupTypeDef(TypedDict):
    RuleGroupName: NotRequired[str],
    ResourceId: NotRequired[str],
    Priority: NotRequired[int],
```

## NetworkFirewallPolicyTypeDef

```python
# NetworkFirewallPolicyTypeDef definition

class NetworkFirewallPolicyTypeDef(TypedDict):
    FirewallDeploymentModel: NotRequired[FirewallDeploymentModelType],  # (1)
```

1. See [:material-code-brackets: FirewallDeploymentModelType](./literals.md#firewalldeploymentmodeltype) 
## NetworkFirewallStatefulRuleGroupOverrideTypeDef

```python
# NetworkFirewallStatefulRuleGroupOverrideTypeDef definition

class NetworkFirewallStatefulRuleGroupOverrideTypeDef(TypedDict):
    Action: NotRequired[NetworkFirewallOverrideActionType],  # (1)
```

1. See [:material-code-brackets: NetworkFirewallOverrideActionType](./literals.md#networkfirewalloverrideactiontype) 
## ThirdPartyFirewallPolicyTypeDef

```python
# ThirdPartyFirewallPolicyTypeDef definition

class ThirdPartyFirewallPolicyTypeDef(TypedDict):
    FirewallDeploymentModel: NotRequired[FirewallDeploymentModelType],  # (1)
```

1. See [:material-code-brackets: FirewallDeploymentModelType](./literals.md#firewalldeploymentmodeltype) 
## ResourceTagTypeDef

```python
# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## PutNotificationChannelRequestRequestTypeDef

```python
# PutNotificationChannelRequestRequestTypeDef definition

class PutNotificationChannelRequestRequestTypeDef(TypedDict):
    SnsTopicArn: str,
    SnsRoleName: str,
```

## ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef

```python
# ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef definition

class ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    VPC: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    CurrentRouteTable: NotRequired[str],
    ExpectedRouteTable: NotRequired[str],
```

## ThirdPartyFirewallMissingFirewallViolationTypeDef

```python
# ThirdPartyFirewallMissingFirewallViolationTypeDef definition

class ThirdPartyFirewallMissingFirewallViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    VPC: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    TargetViolationReason: NotRequired[str],
```

## ThirdPartyFirewallMissingSubnetViolationTypeDef

```python
# ThirdPartyFirewallMissingSubnetViolationTypeDef definition

class ThirdPartyFirewallMissingSubnetViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    VPC: NotRequired[str],
    AvailabilityZone: NotRequired[str],
    TargetViolationReason: NotRequired[str],
```

## SecurityGroupRuleDescriptionTypeDef

```python
# SecurityGroupRuleDescriptionTypeDef definition

class SecurityGroupRuleDescriptionTypeDef(TypedDict):
    IPV4Range: NotRequired[str],
    IPV6Range: NotRequired[str],
    PrefixListId: NotRequired[str],
    Protocol: NotRequired[str],
    FromPort: NotRequired[int],
    ToPort: NotRequired[int],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## EC2AssociateRouteTableActionTypeDef

```python
# EC2AssociateRouteTableActionTypeDef definition

class EC2AssociateRouteTableActionTypeDef(TypedDict):
    RouteTableId: ActionTargetTypeDef,  # (1)
    Description: NotRequired[str],
    SubnetId: NotRequired[ActionTargetTypeDef],  # (1)
    GatewayId: NotRequired[ActionTargetTypeDef],  # (1)
```

1. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
2. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
3. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## EC2CopyRouteTableActionTypeDef

```python
# EC2CopyRouteTableActionTypeDef definition

class EC2CopyRouteTableActionTypeDef(TypedDict):
    VpcId: ActionTargetTypeDef,  # (1)
    RouteTableId: ActionTargetTypeDef,  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
2. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## EC2CreateRouteActionTypeDef

```python
# EC2CreateRouteActionTypeDef definition

class EC2CreateRouteActionTypeDef(TypedDict):
    RouteTableId: ActionTargetTypeDef,  # (1)
    Description: NotRequired[str],
    DestinationCidrBlock: NotRequired[str],
    DestinationPrefixListId: NotRequired[str],
    DestinationIpv6CidrBlock: NotRequired[str],
    VpcEndpointId: NotRequired[ActionTargetTypeDef],  # (1)
    GatewayId: NotRequired[ActionTargetTypeDef],  # (1)
```

1. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
2. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
3. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## EC2CreateRouteTableActionTypeDef

```python
# EC2CreateRouteTableActionTypeDef definition

class EC2CreateRouteTableActionTypeDef(TypedDict):
    VpcId: ActionTargetTypeDef,  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## EC2DeleteRouteActionTypeDef

```python
# EC2DeleteRouteActionTypeDef definition

class EC2DeleteRouteActionTypeDef(TypedDict):
    RouteTableId: ActionTargetTypeDef,  # (1)
    Description: NotRequired[str],
    DestinationCidrBlock: NotRequired[str],
    DestinationPrefixListId: NotRequired[str],
    DestinationIpv6CidrBlock: NotRequired[str],
```

1. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## EC2ReplaceRouteActionTypeDef

```python
# EC2ReplaceRouteActionTypeDef definition

class EC2ReplaceRouteActionTypeDef(TypedDict):
    RouteTableId: ActionTargetTypeDef,  # (1)
    Description: NotRequired[str],
    DestinationCidrBlock: NotRequired[str],
    DestinationPrefixListId: NotRequired[str],
    DestinationIpv6CidrBlock: NotRequired[str],
    GatewayId: NotRequired[ActionTargetTypeDef],  # (1)
```

1. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
2. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## EC2ReplaceRouteTableAssociationActionTypeDef

```python
# EC2ReplaceRouteTableAssociationActionTypeDef definition

class EC2ReplaceRouteTableAssociationActionTypeDef(TypedDict):
    AssociationId: ActionTargetTypeDef,  # (1)
    RouteTableId: ActionTargetTypeDef,  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
2. See [:material-code-braces: ActionTargetTypeDef](./type_defs.md#actiontargettypedef) 
## AdminScopeTypeDef

```python
# AdminScopeTypeDef definition

class AdminScopeTypeDef(TypedDict):
    AccountScope: NotRequired[AccountScopeTypeDef],  # (1)
    OrganizationalUnitScope: NotRequired[OrganizationalUnitScopeTypeDef],  # (2)
    RegionScope: NotRequired[RegionScopeTypeDef],  # (3)
    PolicyTypeScope: NotRequired[PolicyTypeScopeTypeDef],  # (4)
```

1. See [:material-code-braces: AccountScopeTypeDef](./type_defs.md#accountscopetypedef) 
2. See [:material-code-braces: OrganizationalUnitScopeTypeDef](./type_defs.md#organizationalunitscopetypedef) 
3. See [:material-code-braces: RegionScopeTypeDef](./type_defs.md#regionscopetypedef) 
4. See [:material-code-braces: PolicyTypeScopeTypeDef](./type_defs.md#policytypescopetypedef) 
## AppsListDataSummaryTypeDef

```python
# AppsListDataSummaryTypeDef definition

class AppsListDataSummaryTypeDef(TypedDict):
    ListArn: NotRequired[str],
    ListId: NotRequired[str],
    ListName: NotRequired[str],
    AppsList: NotRequired[List[AppTypeDef]],  # (1)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
## AppsListDataTypeDef

```python
# AppsListDataTypeDef definition

class AppsListDataTypeDef(TypedDict):
    ListName: str,
    AppsList: List[AppTypeDef],  # (1)
    ListId: NotRequired[str],
    ListUpdateToken: NotRequired[str],
    CreateTime: NotRequired[datetime],
    LastUpdateTime: NotRequired[datetime],
    PreviousAppsList: NotRequired[Dict[str, List[AppTypeDef]]],  # (2)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
## AssociateThirdPartyFirewallResponseTypeDef

```python
# AssociateThirdPartyFirewallResponseTypeDef definition

class AssociateThirdPartyFirewallResponseTypeDef(TypedDict):
    ThirdPartyFirewallStatus: ThirdPartyFirewallAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ThirdPartyFirewallAssociationStatusType](./literals.md#thirdpartyfirewallassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateThirdPartyFirewallResponseTypeDef

```python
# DisassociateThirdPartyFirewallResponseTypeDef definition

class DisassociateThirdPartyFirewallResponseTypeDef(TypedDict):
    ThirdPartyFirewallStatus: ThirdPartyFirewallAssociationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ThirdPartyFirewallAssociationStatusType](./literals.md#thirdpartyfirewallassociationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAdminAccountResponseTypeDef

```python
# GetAdminAccountResponseTypeDef definition

class GetAdminAccountResponseTypeDef(TypedDict):
    AdminAccount: str,
    RoleStatus: AccountRoleStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AccountRoleStatusType](./literals.md#accountrolestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNotificationChannelResponseTypeDef

```python
# GetNotificationChannelResponseTypeDef definition

class GetNotificationChannelResponseTypeDef(TypedDict):
    SnsTopicArn: str,
    SnsRoleName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProtectionStatusResponseTypeDef

```python
# GetProtectionStatusResponseTypeDef definition

class GetProtectionStatusResponseTypeDef(TypedDict):
    AdminAccountId: str,
    ServiceType: SecurityServiceTypeType,  # (1)
    Data: str,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SecurityServiceTypeType](./literals.md#securityservicetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetThirdPartyFirewallAssociationStatusResponseTypeDef

```python
# GetThirdPartyFirewallAssociationStatusResponseTypeDef definition

class GetThirdPartyFirewallAssociationStatusResponseTypeDef(TypedDict):
    ThirdPartyFirewallStatus: ThirdPartyFirewallAssociationStatusType,  # (1)
    MarketplaceOnboardingStatus: MarketplaceSubscriptionOnboardingStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ThirdPartyFirewallAssociationStatusType](./literals.md#thirdpartyfirewallassociationstatustype) 
2. See [:material-code-brackets: MarketplaceSubscriptionOnboardingStatusType](./literals.md#marketplacesubscriptiononboardingstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAdminAccountsForOrganizationResponseTypeDef

```python
# ListAdminAccountsForOrganizationResponseTypeDef definition

class ListAdminAccountsForOrganizationResponseTypeDef(TypedDict):
    AdminAccounts: List[AdminAccountSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AdminAccountSummaryTypeDef](./type_defs.md#adminaccountsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAdminsManagingAccountResponseTypeDef

```python
# ListAdminsManagingAccountResponseTypeDef definition

class ListAdminsManagingAccountResponseTypeDef(TypedDict):
    AdminAccounts: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMemberAccountsResponseTypeDef

```python
# ListMemberAccountsResponseTypeDef definition

class ListMemberAccountsResponseTypeDef(TypedDict):
    MemberAccounts: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AwsEc2InstanceViolationTypeDef

```python
# AwsEc2InstanceViolationTypeDef definition

class AwsEc2InstanceViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    AwsEc2NetworkInterfaceViolations: NotRequired[List[AwsEc2NetworkInterfaceViolationTypeDef]],  # (1)
```

1. See [:material-code-braces: AwsEc2NetworkInterfaceViolationTypeDef](./type_defs.md#awsec2networkinterfaceviolationtypedef) 
## BatchAssociateResourceResponseTypeDef

```python
# BatchAssociateResourceResponseTypeDef definition

class BatchAssociateResourceResponseTypeDef(TypedDict):
    ResourceSetIdentifier: str,
    FailedItems: List[FailedItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedItemTypeDef](./type_defs.md#faileditemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateResourceResponseTypeDef

```python
# BatchDisassociateResourceResponseTypeDef definition

class BatchDisassociateResourceResponseTypeDef(TypedDict):
    ResourceSetIdentifier: str,
    FailedItems: List[FailedItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedItemTypeDef](./type_defs.md#faileditemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyComplianceDetailTypeDef

```python
# PolicyComplianceDetailTypeDef definition

class PolicyComplianceDetailTypeDef(TypedDict):
    PolicyOwner: NotRequired[str],
    PolicyId: NotRequired[str],
    MemberAccount: NotRequired[str],
    Violators: NotRequired[List[ComplianceViolatorTypeDef]],  # (1)
    EvaluationLimitExceeded: NotRequired[bool],
    ExpiredAt: NotRequired[datetime],
    IssueInfoMap: NotRequired[Dict[DependentServiceNameType, str]],  # (2)
```

1. See [:material-code-braces: ComplianceViolatorTypeDef](./type_defs.md#complianceviolatortypedef) 
2. See [:material-code-brackets: DependentServiceNameType](./literals.md#dependentservicenametype) 
## ListDiscoveredResourcesResponseTypeDef

```python
# ListDiscoveredResourcesResponseTypeDef definition

class ListDiscoveredResourcesResponseTypeDef(TypedDict):
    Items: List[DiscoveredResourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DiscoveredResourceTypeDef](./type_defs.md#discoveredresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyComplianceStatusTypeDef

```python
# PolicyComplianceStatusTypeDef definition

class PolicyComplianceStatusTypeDef(TypedDict):
    PolicyOwner: NotRequired[str],
    PolicyId: NotRequired[str],
    PolicyName: NotRequired[str],
    MemberAccount: NotRequired[str],
    EvaluationResults: NotRequired[List[EvaluationResultTypeDef]],  # (1)
    LastUpdated: NotRequired[datetime],
    IssueInfoMap: NotRequired[Dict[DependentServiceNameType, str]],  # (2)
```

1. See [:material-code-braces: EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef) 
2. See [:material-code-brackets: DependentServiceNameType](./literals.md#dependentservicenametype) 
## NetworkFirewallMissingExpectedRoutesViolationTypeDef

```python
# NetworkFirewallMissingExpectedRoutesViolationTypeDef definition

class NetworkFirewallMissingExpectedRoutesViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    ExpectedRoutes: NotRequired[List[ExpectedRouteTypeDef]],  # (1)
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: ExpectedRouteTypeDef](./type_defs.md#expectedroutetypedef) 
## GetProtectionStatusRequestRequestTypeDef

```python
# GetProtectionStatusRequestRequestTypeDef definition

class GetProtectionStatusRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    MemberAccountId: NotRequired[str],
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetProtocolsListResponseTypeDef

```python
# GetProtocolsListResponseTypeDef definition

class GetProtocolsListResponseTypeDef(TypedDict):
    ProtocolsList: ProtocolsListDataTypeDef,  # (1)
    ProtocolsListArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtocolsListDataTypeDef](./type_defs.md#protocolslistdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProtocolsListResponseTypeDef

```python
# PutProtocolsListResponseTypeDef definition

class PutProtocolsListResponseTypeDef(TypedDict):
    ProtocolsList: ProtocolsListDataTypeDef,  # (1)
    ProtocolsListArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtocolsListDataTypeDef](./type_defs.md#protocolslistdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceSetResponseTypeDef

```python
# GetResourceSetResponseTypeDef definition

class GetResourceSetResponseTypeDef(TypedDict):
    ResourceSet: ResourceSetTypeDef,  # (1)
    ResourceSetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSetTypeDef](./type_defs.md#resourcesettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourceSetResponseTypeDef

```python
# PutResourceSetResponseTypeDef definition

class PutResourceSetResponseTypeDef(TypedDict):
    ResourceSet: ResourceSetTypeDef,  # (1)
    ResourceSetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSetTypeDef](./type_defs.md#resourcesettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef

```python
# ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef definition

class ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef

```python
# ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef definition

class ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAppsListsRequestListAppsListsPaginateTypeDef

```python
# ListAppsListsRequestListAppsListsPaginateTypeDef definition

class ListAppsListsRequestListAppsListsPaginateTypeDef(TypedDict):
    DefaultLists: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComplianceStatusRequestListComplianceStatusPaginateTypeDef

```python
# ListComplianceStatusRequestListComplianceStatusPaginateTypeDef definition

class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(TypedDict):
    PolicyId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMemberAccountsRequestListMemberAccountsPaginateTypeDef

```python
# ListMemberAccountsRequestListMemberAccountsPaginateTypeDef definition

class ListMemberAccountsRequestListMemberAccountsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPoliciesRequestListPoliciesPaginateTypeDef

```python
# ListPoliciesRequestListPoliciesPaginateTypeDef definition

class ListPoliciesRequestListPoliciesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtocolsListsRequestListProtocolsListsPaginateTypeDef

```python
# ListProtocolsListsRequestListProtocolsListsPaginateTypeDef definition

class ListProtocolsListsRequestListProtocolsListsPaginateTypeDef(TypedDict):
    DefaultLists: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef

```python
# ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef definition

class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(TypedDict):
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPoliciesResponseTypeDef

```python
# ListPoliciesResponseTypeDef definition

class ListPoliciesResponseTypeDef(TypedDict):
    PolicyList: List[PolicySummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicySummaryTypeDef](./type_defs.md#policysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProtocolsListsResponseTypeDef

```python
# ListProtocolsListsResponseTypeDef definition

class ListProtocolsListsResponseTypeDef(TypedDict):
    ProtocolsLists: List[ProtocolsListDataSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtocolsListDataSummaryTypeDef](./type_defs.md#protocolslistdatasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceSetResourcesResponseTypeDef

```python
# ListResourceSetResourcesResponseTypeDef definition

class ListResourceSetResourcesResponseTypeDef(TypedDict):
    Items: List[ResourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceSetsResponseTypeDef

```python
# ListResourceSetsResponseTypeDef definition

class ListResourceSetsResponseTypeDef(TypedDict):
    ResourceSets: List[ResourceSetSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSetSummaryTypeDef](./type_defs.md#resourcesetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    TagList: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutProtocolsListRequestRequestTypeDef

```python
# PutProtocolsListRequestRequestTypeDef definition

class PutProtocolsListRequestRequestTypeDef(TypedDict):
    ProtocolsList: ProtocolsListDataTypeDef,  # (1)
    TagList: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ProtocolsListDataTypeDef](./type_defs.md#protocolslistdatatypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutResourceSetRequestRequestTypeDef

```python
# PutResourceSetRequestRequestTypeDef definition

class PutResourceSetRequestRequestTypeDef(TypedDict):
    ResourceSet: ResourceSetTypeDef,  # (1)
    TagList: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ResourceSetTypeDef](./type_defs.md#resourcesettypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagList: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListThirdPartyFirewallFirewallPoliciesResponseTypeDef

```python
# ListThirdPartyFirewallFirewallPoliciesResponseTypeDef definition

class ListThirdPartyFirewallFirewallPoliciesResponseTypeDef(TypedDict):
    ThirdPartyFirewallFirewallPolicies: List[ThirdPartyFirewallFirewallPolicyTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThirdPartyFirewallFirewallPolicyTypeDef](./type_defs.md#thirdpartyfirewallfirewallpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkFirewallBlackHoleRouteDetectedViolationTypeDef

```python
# NetworkFirewallBlackHoleRouteDetectedViolationTypeDef definition

class NetworkFirewallBlackHoleRouteDetectedViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    RouteTableId: NotRequired[str],
    VpcId: NotRequired[str],
    ViolatingRoutes: NotRequired[List[RouteTypeDef]],  # (1)
```

1. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
## NetworkFirewallInternetTrafficNotInspectedViolationTypeDef

```python
# NetworkFirewallInternetTrafficNotInspectedViolationTypeDef definition

class NetworkFirewallInternetTrafficNotInspectedViolationTypeDef(TypedDict):
    SubnetId: NotRequired[str],
    SubnetAvailabilityZone: NotRequired[str],
    RouteTableId: NotRequired[str],
    ViolatingRoutes: NotRequired[List[RouteTypeDef]],  # (1)
    IsRouteTableUsedInDifferentAZ: NotRequired[bool],
    CurrentFirewallSubnetRouteTable: NotRequired[str],
    ExpectedFirewallEndpoint: NotRequired[str],
    FirewallSubnetId: NotRequired[str],
    ExpectedFirewallSubnetRoutes: NotRequired[List[ExpectedRouteTypeDef]],  # (2)
    ActualFirewallSubnetRoutes: NotRequired[List[RouteTypeDef]],  # (1)
    InternetGatewayId: NotRequired[str],
    CurrentInternetGatewayRouteTable: NotRequired[str],
    ExpectedInternetGatewayRoutes: NotRequired[List[ExpectedRouteTypeDef]],  # (2)
    ActualInternetGatewayRoutes: NotRequired[List[RouteTypeDef]],  # (1)
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
2. See [:material-code-braces: ExpectedRouteTypeDef](./type_defs.md#expectedroutetypedef) 
3. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
4. See [:material-code-braces: ExpectedRouteTypeDef](./type_defs.md#expectedroutetypedef) 
5. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
## NetworkFirewallInvalidRouteConfigurationViolationTypeDef

```python
# NetworkFirewallInvalidRouteConfigurationViolationTypeDef definition

class NetworkFirewallInvalidRouteConfigurationViolationTypeDef(TypedDict):
    AffectedSubnets: NotRequired[List[str]],
    RouteTableId: NotRequired[str],
    IsRouteTableUsedInDifferentAZ: NotRequired[bool],
    ViolatingRoute: NotRequired[RouteTypeDef],  # (1)
    CurrentFirewallSubnetRouteTable: NotRequired[str],
    ExpectedFirewallEndpoint: NotRequired[str],
    ActualFirewallEndpoint: NotRequired[str],
    ExpectedFirewallSubnetId: NotRequired[str],
    ActualFirewallSubnetId: NotRequired[str],
    ExpectedFirewallSubnetRoutes: NotRequired[List[ExpectedRouteTypeDef]],  # (2)
    ActualFirewallSubnetRoutes: NotRequired[List[RouteTypeDef]],  # (3)
    InternetGatewayId: NotRequired[str],
    CurrentInternetGatewayRouteTable: NotRequired[str],
    ExpectedInternetGatewayRoutes: NotRequired[List[ExpectedRouteTypeDef]],  # (2)
    ActualInternetGatewayRoutes: NotRequired[List[RouteTypeDef]],  # (3)
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
2. See [:material-code-braces: ExpectedRouteTypeDef](./type_defs.md#expectedroutetypedef) 
3. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
4. See [:material-code-braces: ExpectedRouteTypeDef](./type_defs.md#expectedroutetypedef) 
5. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
## NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef

```python
# NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef definition

class NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef(TypedDict):
    FirewallSubnetId: NotRequired[str],
    ViolatingRoutes: NotRequired[List[RouteTypeDef]],  # (1)
    RouteTableId: NotRequired[str],
    FirewallEndpoint: NotRequired[str],
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
## NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef

```python
# NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef definition

class NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef(TypedDict):
    GatewayId: NotRequired[str],
    ViolatingRoutes: NotRequired[List[RouteTypeDef]],  # (1)
    RouteTableId: NotRequired[str],
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
## RouteHasOutOfScopeEndpointViolationTypeDef

```python
# RouteHasOutOfScopeEndpointViolationTypeDef definition

class RouteHasOutOfScopeEndpointViolationTypeDef(TypedDict):
    SubnetId: NotRequired[str],
    VpcId: NotRequired[str],
    RouteTableId: NotRequired[str],
    ViolatingRoutes: NotRequired[List[RouteTypeDef]],  # (1)
    SubnetAvailabilityZone: NotRequired[str],
    SubnetAvailabilityZoneId: NotRequired[str],
    CurrentFirewallSubnetRouteTable: NotRequired[str],
    FirewallSubnetId: NotRequired[str],
    FirewallSubnetRoutes: NotRequired[List[RouteTypeDef]],  # (1)
    InternetGatewayId: NotRequired[str],
    CurrentInternetGatewayRouteTable: NotRequired[str],
    InternetGatewayRoutes: NotRequired[List[RouteTypeDef]],  # (1)
```

1. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
2. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
3. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
## StatefulRuleGroupTypeDef

```python
# StatefulRuleGroupTypeDef definition

class StatefulRuleGroupTypeDef(TypedDict):
    RuleGroupName: NotRequired[str],
    ResourceId: NotRequired[str],
    Priority: NotRequired[int],
    Override: NotRequired[NetworkFirewallStatefulRuleGroupOverrideTypeDef],  # (1)
```

1. See [:material-code-braces: NetworkFirewallStatefulRuleGroupOverrideTypeDef](./type_defs.md#networkfirewallstatefulrulegroupoverridetypedef) 
## PolicyOptionTypeDef

```python
# PolicyOptionTypeDef definition

class PolicyOptionTypeDef(TypedDict):
    NetworkFirewallPolicy: NotRequired[NetworkFirewallPolicyTypeDef],  # (1)
    ThirdPartyFirewallPolicy: NotRequired[ThirdPartyFirewallPolicyTypeDef],  # (2)
```

1. See [:material-code-braces: NetworkFirewallPolicyTypeDef](./type_defs.md#networkfirewallpolicytypedef) 
2. See [:material-code-braces: ThirdPartyFirewallPolicyTypeDef](./type_defs.md#thirdpartyfirewallpolicytypedef) 
## SecurityGroupRemediationActionTypeDef

```python
# SecurityGroupRemediationActionTypeDef definition

class SecurityGroupRemediationActionTypeDef(TypedDict):
    RemediationActionType: NotRequired[RemediationActionTypeType],  # (1)
    Description: NotRequired[str],
    RemediationResult: NotRequired[SecurityGroupRuleDescriptionTypeDef],  # (2)
    IsDefaultAction: NotRequired[bool],
```

1. See [:material-code-brackets: RemediationActionTypeType](./literals.md#remediationactiontypetype) 
2. See [:material-code-braces: SecurityGroupRuleDescriptionTypeDef](./type_defs.md#securitygroupruledescriptiontypedef) 
## RemediationActionTypeDef

```python
# RemediationActionTypeDef definition

class RemediationActionTypeDef(TypedDict):
    Description: NotRequired[str],
    EC2CreateRouteAction: NotRequired[EC2CreateRouteActionTypeDef],  # (1)
    EC2ReplaceRouteAction: NotRequired[EC2ReplaceRouteActionTypeDef],  # (2)
    EC2DeleteRouteAction: NotRequired[EC2DeleteRouteActionTypeDef],  # (3)
    EC2CopyRouteTableAction: NotRequired[EC2CopyRouteTableActionTypeDef],  # (4)
    EC2ReplaceRouteTableAssociationAction: NotRequired[EC2ReplaceRouteTableAssociationActionTypeDef],  # (5)
    EC2AssociateRouteTableAction: NotRequired[EC2AssociateRouteTableActionTypeDef],  # (6)
    EC2CreateRouteTableAction: NotRequired[EC2CreateRouteTableActionTypeDef],  # (7)
    FMSPolicyUpdateFirewallCreationConfigAction: NotRequired[FMSPolicyUpdateFirewallCreationConfigActionTypeDef],  # (8)
```

1. See [:material-code-braces: EC2CreateRouteActionTypeDef](./type_defs.md#ec2createrouteactiontypedef) 
2. See [:material-code-braces: EC2ReplaceRouteActionTypeDef](./type_defs.md#ec2replacerouteactiontypedef) 
3. See [:material-code-braces: EC2DeleteRouteActionTypeDef](./type_defs.md#ec2deleterouteactiontypedef) 
4. See [:material-code-braces: EC2CopyRouteTableActionTypeDef](./type_defs.md#ec2copyroutetableactiontypedef) 
5. See [:material-code-braces: EC2ReplaceRouteTableAssociationActionTypeDef](./type_defs.md#ec2replaceroutetableassociationactiontypedef) 
6. See [:material-code-braces: EC2AssociateRouteTableActionTypeDef](./type_defs.md#ec2associateroutetableactiontypedef) 
7. See [:material-code-braces: EC2CreateRouteTableActionTypeDef](./type_defs.md#ec2createroutetableactiontypedef) 
8. See [:material-code-braces: FMSPolicyUpdateFirewallCreationConfigActionTypeDef](./type_defs.md#fmspolicyupdatefirewallcreationconfigactiontypedef) 
## GetAdminScopeResponseTypeDef

```python
# GetAdminScopeResponseTypeDef definition

class GetAdminScopeResponseTypeDef(TypedDict):
    AdminScope: AdminScopeTypeDef,  # (1)
    Status: OrganizationStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AdminScopeTypeDef](./type_defs.md#adminscopetypedef) 
2. See [:material-code-brackets: OrganizationStatusType](./literals.md#organizationstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAdminAccountRequestRequestTypeDef

```python
# PutAdminAccountRequestRequestTypeDef definition

class PutAdminAccountRequestRequestTypeDef(TypedDict):
    AdminAccount: str,
    AdminScope: NotRequired[AdminScopeTypeDef],  # (1)
```

1. See [:material-code-braces: AdminScopeTypeDef](./type_defs.md#adminscopetypedef) 
## ListAppsListsResponseTypeDef

```python
# ListAppsListsResponseTypeDef definition

class ListAppsListsResponseTypeDef(TypedDict):
    AppsLists: List[AppsListDataSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppsListDataSummaryTypeDef](./type_defs.md#appslistdatasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppsListResponseTypeDef

```python
# GetAppsListResponseTypeDef definition

class GetAppsListResponseTypeDef(TypedDict):
    AppsList: AppsListDataTypeDef,  # (1)
    AppsListArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppsListDataTypeDef](./type_defs.md#appslistdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAppsListRequestRequestTypeDef

```python
# PutAppsListRequestRequestTypeDef definition

class PutAppsListRequestRequestTypeDef(TypedDict):
    AppsList: AppsListDataTypeDef,  # (1)
    TagList: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: AppsListDataTypeDef](./type_defs.md#appslistdatatypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutAppsListResponseTypeDef

```python
# PutAppsListResponseTypeDef definition

class PutAppsListResponseTypeDef(TypedDict):
    AppsList: AppsListDataTypeDef,  # (1)
    AppsListArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppsListDataTypeDef](./type_defs.md#appslistdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComplianceDetailResponseTypeDef

```python
# GetComplianceDetailResponseTypeDef definition

class GetComplianceDetailResponseTypeDef(TypedDict):
    PolicyComplianceDetail: PolicyComplianceDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyComplianceDetailTypeDef](./type_defs.md#policycompliancedetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListComplianceStatusResponseTypeDef

```python
# ListComplianceStatusResponseTypeDef definition

class ListComplianceStatusResponseTypeDef(TypedDict):
    PolicyComplianceStatusList: List[PolicyComplianceStatusTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyComplianceStatusTypeDef](./type_defs.md#policycompliancestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkFirewallPolicyDescriptionTypeDef

```python
# NetworkFirewallPolicyDescriptionTypeDef definition

class NetworkFirewallPolicyDescriptionTypeDef(TypedDict):
    StatelessRuleGroups: NotRequired[List[StatelessRuleGroupTypeDef]],  # (1)
    StatelessDefaultActions: NotRequired[List[str]],
    StatelessFragmentDefaultActions: NotRequired[List[str]],
    StatelessCustomActions: NotRequired[List[str]],
    StatefulRuleGroups: NotRequired[List[StatefulRuleGroupTypeDef]],  # (2)
    StatefulDefaultActions: NotRequired[List[str]],
    StatefulEngineOptions: NotRequired[StatefulEngineOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: StatelessRuleGroupTypeDef](./type_defs.md#statelessrulegrouptypedef) 
2. See [:material-code-braces: StatefulRuleGroupTypeDef](./type_defs.md#statefulrulegrouptypedef) 
3. See [:material-code-braces: StatefulEngineOptionsTypeDef](./type_defs.md#statefulengineoptionstypedef) 
## SecurityServicePolicyDataTypeDef

```python
# SecurityServicePolicyDataTypeDef definition

class SecurityServicePolicyDataTypeDef(TypedDict):
    Type: SecurityServiceTypeType,  # (1)
    ManagedServiceData: NotRequired[str],
    PolicyOption: NotRequired[PolicyOptionTypeDef],  # (2)
```

1. See [:material-code-brackets: SecurityServiceTypeType](./literals.md#securityservicetypetype) 
2. See [:material-code-braces: PolicyOptionTypeDef](./type_defs.md#policyoptiontypedef) 
## AwsVPCSecurityGroupViolationTypeDef

```python
# AwsVPCSecurityGroupViolationTypeDef definition

class AwsVPCSecurityGroupViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    ViolationTargetDescription: NotRequired[str],
    PartialMatches: NotRequired[List[PartialMatchTypeDef]],  # (1)
    PossibleSecurityGroupRemediationActions: NotRequired[List[SecurityGroupRemediationActionTypeDef]],  # (2)
```

1. See [:material-code-braces: PartialMatchTypeDef](./type_defs.md#partialmatchtypedef) 
2. See [:material-code-braces: SecurityGroupRemediationActionTypeDef](./type_defs.md#securitygroupremediationactiontypedef) 
## RemediationActionWithOrderTypeDef

```python
# RemediationActionWithOrderTypeDef definition

class RemediationActionWithOrderTypeDef(TypedDict):
    RemediationAction: NotRequired[RemediationActionTypeDef],  # (1)
    Order: NotRequired[int],
```

1. See [:material-code-braces: RemediationActionTypeDef](./type_defs.md#remediationactiontypedef) 
## NetworkFirewallPolicyModifiedViolationTypeDef

```python
# NetworkFirewallPolicyModifiedViolationTypeDef definition

class NetworkFirewallPolicyModifiedViolationTypeDef(TypedDict):
    ViolationTarget: NotRequired[str],
    CurrentPolicyDescription: NotRequired[NetworkFirewallPolicyDescriptionTypeDef],  # (1)
    ExpectedPolicyDescription: NotRequired[NetworkFirewallPolicyDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: NetworkFirewallPolicyDescriptionTypeDef](./type_defs.md#networkfirewallpolicydescriptiontypedef) 
2. See [:material-code-braces: NetworkFirewallPolicyDescriptionTypeDef](./type_defs.md#networkfirewallpolicydescriptiontypedef) 
## PolicyTypeDef

```python
# PolicyTypeDef definition

class PolicyTypeDef(TypedDict):
    PolicyName: str,
    SecurityServicePolicyData: SecurityServicePolicyDataTypeDef,  # (1)
    ResourceType: str,
    ExcludeResourceTags: bool,
    RemediationEnabled: bool,
    PolicyId: NotRequired[str],
    PolicyUpdateToken: NotRequired[str],
    ResourceTypeList: NotRequired[List[str]],
    ResourceTags: NotRequired[List[ResourceTagTypeDef]],  # (2)
    DeleteUnusedFMManagedResources: NotRequired[bool],
    IncludeMap: NotRequired[Dict[CustomerPolicyScopeIdTypeType, List[str]]],  # (3)
    ExcludeMap: NotRequired[Dict[CustomerPolicyScopeIdTypeType, List[str]]],  # (3)
    ResourceSetIds: NotRequired[List[str]],
    PolicyDescription: NotRequired[str],
    PolicyStatus: NotRequired[CustomerPolicyStatusType],  # (5)
```

1. See [:material-code-braces: SecurityServicePolicyDataTypeDef](./type_defs.md#securityservicepolicydatatypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
3. See [:material-code-brackets: CustomerPolicyScopeIdTypeType](./literals.md#customerpolicyscopeidtypetype) 
4. See [:material-code-brackets: CustomerPolicyScopeIdTypeType](./literals.md#customerpolicyscopeidtypetype) 
5. See [:material-code-brackets: CustomerPolicyStatusType](./literals.md#customerpolicystatustype) 
## PossibleRemediationActionTypeDef

```python
# PossibleRemediationActionTypeDef definition

class PossibleRemediationActionTypeDef(TypedDict):
    OrderedRemediationActions: List[RemediationActionWithOrderTypeDef],  # (1)
    Description: NotRequired[str],
    IsDefaultAction: NotRequired[bool],
```

1. See [:material-code-braces: RemediationActionWithOrderTypeDef](./type_defs.md#remediationactionwithordertypedef) 
## GetPolicyResponseTypeDef

```python
# GetPolicyResponseTypeDef definition

class GetPolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    PolicyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPolicyRequestRequestTypeDef

```python
# PutPolicyRequestRequestTypeDef definition

class PutPolicyRequestRequestTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    TagList: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutPolicyResponseTypeDef

```python
# PutPolicyResponseTypeDef definition

class PutPolicyResponseTypeDef(TypedDict):
    Policy: PolicyTypeDef,  # (1)
    PolicyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PolicyTypeDef](./type_defs.md#policytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PossibleRemediationActionsTypeDef

```python
# PossibleRemediationActionsTypeDef definition

class PossibleRemediationActionsTypeDef(TypedDict):
    Description: NotRequired[str],
    Actions: NotRequired[List[PossibleRemediationActionTypeDef]],  # (1)
```

1. See [:material-code-braces: PossibleRemediationActionTypeDef](./type_defs.md#possibleremediationactiontypedef) 
## ResourceViolationTypeDef

```python
# ResourceViolationTypeDef definition

class ResourceViolationTypeDef(TypedDict):
    AwsVPCSecurityGroupViolation: NotRequired[AwsVPCSecurityGroupViolationTypeDef],  # (1)
    AwsEc2NetworkInterfaceViolation: NotRequired[AwsEc2NetworkInterfaceViolationTypeDef],  # (2)
    AwsEc2InstanceViolation: NotRequired[AwsEc2InstanceViolationTypeDef],  # (3)
    NetworkFirewallMissingFirewallViolation: NotRequired[NetworkFirewallMissingFirewallViolationTypeDef],  # (4)
    NetworkFirewallMissingSubnetViolation: NotRequired[NetworkFirewallMissingSubnetViolationTypeDef],  # (5)
    NetworkFirewallMissingExpectedRTViolation: NotRequired[NetworkFirewallMissingExpectedRTViolationTypeDef],  # (6)
    NetworkFirewallPolicyModifiedViolation: NotRequired[NetworkFirewallPolicyModifiedViolationTypeDef],  # (7)
    NetworkFirewallInternetTrafficNotInspectedViolation: NotRequired[NetworkFirewallInternetTrafficNotInspectedViolationTypeDef],  # (8)
    NetworkFirewallInvalidRouteConfigurationViolation: NotRequired[NetworkFirewallInvalidRouteConfigurationViolationTypeDef],  # (9)
    NetworkFirewallBlackHoleRouteDetectedViolation: NotRequired[NetworkFirewallBlackHoleRouteDetectedViolationTypeDef],  # (10)
    NetworkFirewallUnexpectedFirewallRoutesViolation: NotRequired[NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef],  # (11)
    NetworkFirewallUnexpectedGatewayRoutesViolation: NotRequired[NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef],  # (12)
    NetworkFirewallMissingExpectedRoutesViolation: NotRequired[NetworkFirewallMissingExpectedRoutesViolationTypeDef],  # (13)
    DnsRuleGroupPriorityConflictViolation: NotRequired[DnsRuleGroupPriorityConflictViolationTypeDef],  # (14)
    DnsDuplicateRuleGroupViolation: NotRequired[DnsDuplicateRuleGroupViolationTypeDef],  # (15)
    DnsRuleGroupLimitExceededViolation: NotRequired[DnsRuleGroupLimitExceededViolationTypeDef],  # (16)
    PossibleRemediationActions: NotRequired[PossibleRemediationActionsTypeDef],  # (17)
    FirewallSubnetIsOutOfScopeViolation: NotRequired[FirewallSubnetIsOutOfScopeViolationTypeDef],  # (18)
    RouteHasOutOfScopeEndpointViolation: NotRequired[RouteHasOutOfScopeEndpointViolationTypeDef],  # (19)
    ThirdPartyFirewallMissingFirewallViolation: NotRequired[ThirdPartyFirewallMissingFirewallViolationTypeDef],  # (20)
    ThirdPartyFirewallMissingSubnetViolation: NotRequired[ThirdPartyFirewallMissingSubnetViolationTypeDef],  # (21)
    ThirdPartyFirewallMissingExpectedRouteTableViolation: NotRequired[ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef],  # (22)
    FirewallSubnetMissingVPCEndpointViolation: NotRequired[FirewallSubnetMissingVPCEndpointViolationTypeDef],  # (23)
```

1. See [:material-code-braces: AwsVPCSecurityGroupViolationTypeDef](./type_defs.md#awsvpcsecuritygroupviolationtypedef) 
2. See [:material-code-braces: AwsEc2NetworkInterfaceViolationTypeDef](./type_defs.md#awsec2networkinterfaceviolationtypedef) 
3. See [:material-code-braces: AwsEc2InstanceViolationTypeDef](./type_defs.md#awsec2instanceviolationtypedef) 
4. See [:material-code-braces: NetworkFirewallMissingFirewallViolationTypeDef](./type_defs.md#networkfirewallmissingfirewallviolationtypedef) 
5. See [:material-code-braces: NetworkFirewallMissingSubnetViolationTypeDef](./type_defs.md#networkfirewallmissingsubnetviolationtypedef) 
6. See [:material-code-braces: NetworkFirewallMissingExpectedRTViolationTypeDef](./type_defs.md#networkfirewallmissingexpectedrtviolationtypedef) 
7. See [:material-code-braces: NetworkFirewallPolicyModifiedViolationTypeDef](./type_defs.md#networkfirewallpolicymodifiedviolationtypedef) 
8. See [:material-code-braces: NetworkFirewallInternetTrafficNotInspectedViolationTypeDef](./type_defs.md#networkfirewallinternettrafficnotinspectedviolationtypedef) 
9. See [:material-code-braces: NetworkFirewallInvalidRouteConfigurationViolationTypeDef](./type_defs.md#networkfirewallinvalidrouteconfigurationviolationtypedef) 
10. See [:material-code-braces: NetworkFirewallBlackHoleRouteDetectedViolationTypeDef](./type_defs.md#networkfirewallblackholeroutedetectedviolationtypedef) 
11. See [:material-code-braces: NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef](./type_defs.md#networkfirewallunexpectedfirewallroutesviolationtypedef) 
12. See [:material-code-braces: NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef](./type_defs.md#networkfirewallunexpectedgatewayroutesviolationtypedef) 
13. See [:material-code-braces: NetworkFirewallMissingExpectedRoutesViolationTypeDef](./type_defs.md#networkfirewallmissingexpectedroutesviolationtypedef) 
14. See [:material-code-braces: DnsRuleGroupPriorityConflictViolationTypeDef](./type_defs.md#dnsrulegrouppriorityconflictviolationtypedef) 
15. See [:material-code-braces: DnsDuplicateRuleGroupViolationTypeDef](./type_defs.md#dnsduplicaterulegroupviolationtypedef) 
16. See [:material-code-braces: DnsRuleGroupLimitExceededViolationTypeDef](./type_defs.md#dnsrulegrouplimitexceededviolationtypedef) 
17. See [:material-code-braces: PossibleRemediationActionsTypeDef](./type_defs.md#possibleremediationactionstypedef) 
18. See [:material-code-braces: FirewallSubnetIsOutOfScopeViolationTypeDef](./type_defs.md#firewallsubnetisoutofscopeviolationtypedef) 
19. See [:material-code-braces: RouteHasOutOfScopeEndpointViolationTypeDef](./type_defs.md#routehasoutofscopeendpointviolationtypedef) 
20. See [:material-code-braces: ThirdPartyFirewallMissingFirewallViolationTypeDef](./type_defs.md#thirdpartyfirewallmissingfirewallviolationtypedef) 
21. See [:material-code-braces: ThirdPartyFirewallMissingSubnetViolationTypeDef](./type_defs.md#thirdpartyfirewallmissingsubnetviolationtypedef) 
22. See [:material-code-braces: ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef](./type_defs.md#thirdpartyfirewallmissingexpectedroutetableviolationtypedef) 
23. See [:material-code-braces: FirewallSubnetMissingVPCEndpointViolationTypeDef](./type_defs.md#firewallsubnetmissingvpcendpointviolationtypedef) 
## ViolationDetailTypeDef

```python
# ViolationDetailTypeDef definition

class ViolationDetailTypeDef(TypedDict):
    PolicyId: str,
    MemberAccount: str,
    ResourceId: str,
    ResourceType: str,
    ResourceViolations: List[ResourceViolationTypeDef],  # (1)
    ResourceTags: NotRequired[List[TagTypeDef]],  # (2)
    ResourceDescription: NotRequired[str],
```

1. See [:material-code-braces: ResourceViolationTypeDef](./type_defs.md#resourceviolationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetViolationDetailsResponseTypeDef

```python
# GetViolationDetailsResponseTypeDef definition

class GetViolationDetailsResponseTypeDef(TypedDict):
    ViolationDetail: ViolationDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ViolationDetailTypeDef](./type_defs.md#violationdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
