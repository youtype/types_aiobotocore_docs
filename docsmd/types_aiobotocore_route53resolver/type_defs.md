# Type definitions

> [Index](../README.md) > [Route53Resolver](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Route53Resolver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#route53resolver)
    type annotations stubs module [types-aiobotocore-route53resolver](https://pypi.org/project/types-aiobotocore-route53resolver/).



## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## FirewallRuleGroupAssociationTypeDef

```python
# FirewallRuleGroupAssociationTypeDef definition

class FirewallRuleGroupAssociationTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    FirewallRuleGroupId: NotRequired[str],
    VpcId: NotRequired[str],
    Name: NotRequired[str],
    Priority: NotRequired[int],
    MutationProtection: NotRequired[MutationProtectionStatusType],  # (1)
    ManagedOwnerName: NotRequired[str],
    Status: NotRequired[FirewallRuleGroupAssociationStatusType],  # (2)
    StatusMessage: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    CreationTime: NotRequired[str],
    ModificationTime: NotRequired[str],
```

1. See [:material-code-brackets: MutationProtectionStatusType](./literals.md#mutationprotectionstatustype) 
2. See [:material-code-brackets: FirewallRuleGroupAssociationStatusType](./literals.md#firewallrulegroupassociationstatustype) 
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

## IpAddressUpdateTypeDef

```python
# IpAddressUpdateTypeDef definition

class IpAddressUpdateTypeDef(TypedDict):
    IpId: NotRequired[str],
    SubnetId: NotRequired[str],
    Ip: NotRequired[str],
    Ipv6: NotRequired[str],
```

## ResolverEndpointTypeDef

```python
# ResolverEndpointTypeDef definition

class ResolverEndpointTypeDef(TypedDict):
    Id: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    SecurityGroupIds: NotRequired[List[str]],
    Direction: NotRequired[ResolverEndpointDirectionType],  # (1)
    IpAddressCount: NotRequired[int],
    HostVPCId: NotRequired[str],
    Status: NotRequired[ResolverEndpointStatusType],  # (2)
    StatusMessage: NotRequired[str],
    CreationTime: NotRequired[str],
    ModificationTime: NotRequired[str],
    OutpostArn: NotRequired[str],
    PreferredInstanceType: NotRequired[str],
    ResolverEndpointType: NotRequired[ResolverEndpointTypeType],  # (3)
    Protocols: NotRequired[List[ProtocolType]],  # (4)
```

1. See [:material-code-brackets: ResolverEndpointDirectionType](./literals.md#resolverendpointdirectiontype) 
2. See [:material-code-brackets: ResolverEndpointStatusType](./literals.md#resolverendpointstatustype) 
3. See [:material-code-brackets: ResolverEndpointTypeType](./literals.md#resolverendpointtypetype) 
4. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## AssociateResolverQueryLogConfigRequestRequestTypeDef

```python
# AssociateResolverQueryLogConfigRequestRequestTypeDef definition

class AssociateResolverQueryLogConfigRequestRequestTypeDef(TypedDict):
    ResolverQueryLogConfigId: str,
    ResourceId: str,
```

## ResolverQueryLogConfigAssociationTypeDef

```python
# ResolverQueryLogConfigAssociationTypeDef definition

class ResolverQueryLogConfigAssociationTypeDef(TypedDict):
    Id: NotRequired[str],
    ResolverQueryLogConfigId: NotRequired[str],
    ResourceId: NotRequired[str],
    Status: NotRequired[ResolverQueryLogConfigAssociationStatusType],  # (1)
    Error: NotRequired[ResolverQueryLogConfigAssociationErrorType],  # (2)
    ErrorMessage: NotRequired[str],
    CreationTime: NotRequired[str],
```

1. See [:material-code-brackets: ResolverQueryLogConfigAssociationStatusType](./literals.md#resolverquerylogconfigassociationstatustype) 
2. See [:material-code-brackets: ResolverQueryLogConfigAssociationErrorType](./literals.md#resolverquerylogconfigassociationerrortype) 
## AssociateResolverRuleRequestRequestTypeDef

```python
# AssociateResolverRuleRequestRequestTypeDef definition

class AssociateResolverRuleRequestRequestTypeDef(TypedDict):
    ResolverRuleId: str,
    VPCId: str,
    Name: NotRequired[str],
```

## ResolverRuleAssociationTypeDef

```python
# ResolverRuleAssociationTypeDef definition

class ResolverRuleAssociationTypeDef(TypedDict):
    Id: NotRequired[str],
    ResolverRuleId: NotRequired[str],
    Name: NotRequired[str],
    VPCId: NotRequired[str],
    Status: NotRequired[ResolverRuleAssociationStatusType],  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ResolverRuleAssociationStatusType](./literals.md#resolverruleassociationstatustype) 
## FirewallDomainListTypeDef

```python
# FirewallDomainListTypeDef definition

class FirewallDomainListTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    DomainCount: NotRequired[int],
    Status: NotRequired[FirewallDomainListStatusType],  # (1)
    StatusMessage: NotRequired[str],
    ManagedOwnerName: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    CreationTime: NotRequired[str],
    ModificationTime: NotRequired[str],
```

1. See [:material-code-brackets: FirewallDomainListStatusType](./literals.md#firewalldomainliststatustype) 
## FirewallRuleGroupTypeDef

```python
# FirewallRuleGroupTypeDef definition

class FirewallRuleGroupTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    RuleCount: NotRequired[int],
    Status: NotRequired[FirewallRuleGroupStatusType],  # (1)
    StatusMessage: NotRequired[str],
    OwnerId: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    ShareStatus: NotRequired[ShareStatusType],  # (2)
    CreationTime: NotRequired[str],
    ModificationTime: NotRequired[str],
```

1. See [:material-code-brackets: FirewallRuleGroupStatusType](./literals.md#firewallrulegroupstatustype) 
2. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## CreateFirewallRuleRequestRequestTypeDef

```python
# CreateFirewallRuleRequestRequestTypeDef definition

class CreateFirewallRuleRequestRequestTypeDef(TypedDict):
    CreatorRequestId: str,
    FirewallRuleGroupId: str,
    Priority: int,
    Action: ActionType,  # (1)
    Name: str,
    FirewallDomainListId: NotRequired[str],
    BlockResponse: NotRequired[BlockResponseType],  # (2)
    BlockOverrideDomain: NotRequired[str],
    BlockOverrideDnsType: NotRequired[BlockOverrideDnsTypeType],  # (3)
    BlockOverrideTtl: NotRequired[int],
    FirewallDomainRedirectionAction: NotRequired[FirewallDomainRedirectionActionType],  # (4)
    Qtype: NotRequired[str],
    DnsThreatProtection: NotRequired[DnsThreatProtectionType],  # (5)
    ConfidenceThreshold: NotRequired[ConfidenceThresholdType],  # (6)
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
2. See [:material-code-brackets: BlockResponseType](./literals.md#blockresponsetype) 
3. See [:material-code-brackets: BlockOverrideDnsTypeType](./literals.md#blockoverridednstypetype) 
4. See [:material-code-brackets: FirewallDomainRedirectionActionType](./literals.md#firewalldomainredirectionactiontype) 
5. See [:material-code-brackets: DnsThreatProtectionType](./literals.md#dnsthreatprotectiontype) 
6. See [:material-code-brackets: ConfidenceThresholdType](./literals.md#confidencethresholdtype) 
## FirewallRuleTypeDef

```python
# FirewallRuleTypeDef definition

class FirewallRuleTypeDef(TypedDict):
    FirewallRuleGroupId: NotRequired[str],
    FirewallDomainListId: NotRequired[str],
    FirewallThreatProtectionId: NotRequired[str],
    Name: NotRequired[str],
    Priority: NotRequired[int],
    Action: NotRequired[ActionType],  # (1)
    BlockResponse: NotRequired[BlockResponseType],  # (2)
    BlockOverrideDomain: NotRequired[str],
    BlockOverrideDnsType: NotRequired[BlockOverrideDnsTypeType],  # (3)
    BlockOverrideTtl: NotRequired[int],
    CreatorRequestId: NotRequired[str],
    CreationTime: NotRequired[str],
    ModificationTime: NotRequired[str],
    FirewallDomainRedirectionAction: NotRequired[FirewallDomainRedirectionActionType],  # (4)
    Qtype: NotRequired[str],
    DnsThreatProtection: NotRequired[DnsThreatProtectionType],  # (5)
    ConfidenceThreshold: NotRequired[ConfidenceThresholdType],  # (6)
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
2. See [:material-code-brackets: BlockResponseType](./literals.md#blockresponsetype) 
3. See [:material-code-brackets: BlockOverrideDnsTypeType](./literals.md#blockoverridednstypetype) 
4. See [:material-code-brackets: FirewallDomainRedirectionActionType](./literals.md#firewalldomainredirectionactiontype) 
5. See [:material-code-brackets: DnsThreatProtectionType](./literals.md#dnsthreatprotectiontype) 
6. See [:material-code-brackets: ConfidenceThresholdType](./literals.md#confidencethresholdtype) 
## OutpostResolverTypeDef

```python
# OutpostResolverTypeDef definition

class OutpostResolverTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreationTime: NotRequired[str],
    ModificationTime: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    Id: NotRequired[str],
    InstanceCount: NotRequired[int],
    PreferredInstanceType: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[OutpostResolverStatusType],  # (1)
    StatusMessage: NotRequired[str],
    OutpostArn: NotRequired[str],
```

1. See [:material-code-brackets: OutpostResolverStatusType](./literals.md#outpostresolverstatustype) 
## IpAddressRequestTypeDef

```python
# IpAddressRequestTypeDef definition

class IpAddressRequestTypeDef(TypedDict):
    SubnetId: str,
    Ip: NotRequired[str],
    Ipv6: NotRequired[str],
```

## ResolverQueryLogConfigTypeDef

```python
# ResolverQueryLogConfigTypeDef definition

class ResolverQueryLogConfigTypeDef(TypedDict):
    Id: NotRequired[str],
    OwnerId: NotRequired[str],
    Status: NotRequired[ResolverQueryLogConfigStatusType],  # (1)
    ShareStatus: NotRequired[ShareStatusType],  # (2)
    AssociationCount: NotRequired[int],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    DestinationArn: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    CreationTime: NotRequired[str],
```

1. See [:material-code-brackets: ResolverQueryLogConfigStatusType](./literals.md#resolverquerylogconfigstatustype) 
2. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## TargetAddressTypeDef

```python
# TargetAddressTypeDef definition

class TargetAddressTypeDef(TypedDict):
    Ip: NotRequired[str],
    Port: NotRequired[int],
    Ipv6: NotRequired[str],
    Protocol: NotRequired[ProtocolType],  # (1)
    ServerNameIndication: NotRequired[str],
```

1. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## DeleteFirewallDomainListRequestRequestTypeDef

```python
# DeleteFirewallDomainListRequestRequestTypeDef definition

class DeleteFirewallDomainListRequestRequestTypeDef(TypedDict):
    FirewallDomainListId: str,
```

## DeleteFirewallRuleGroupRequestRequestTypeDef

```python
# DeleteFirewallRuleGroupRequestRequestTypeDef definition

class DeleteFirewallRuleGroupRequestRequestTypeDef(TypedDict):
    FirewallRuleGroupId: str,
```

## DeleteFirewallRuleRequestRequestTypeDef

```python
# DeleteFirewallRuleRequestRequestTypeDef definition

class DeleteFirewallRuleRequestRequestTypeDef(TypedDict):
    FirewallRuleGroupId: str,
    FirewallDomainListId: NotRequired[str],
    FirewallThreatProtectionId: NotRequired[str],
    Qtype: NotRequired[str],
```

## DeleteOutpostResolverRequestRequestTypeDef

```python
# DeleteOutpostResolverRequestRequestTypeDef definition

class DeleteOutpostResolverRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteResolverEndpointRequestRequestTypeDef

```python
# DeleteResolverEndpointRequestRequestTypeDef definition

class DeleteResolverEndpointRequestRequestTypeDef(TypedDict):
    ResolverEndpointId: str,
```

## DeleteResolverQueryLogConfigRequestRequestTypeDef

```python
# DeleteResolverQueryLogConfigRequestRequestTypeDef definition

class DeleteResolverQueryLogConfigRequestRequestTypeDef(TypedDict):
    ResolverQueryLogConfigId: str,
```

## DeleteResolverRuleRequestRequestTypeDef

```python
# DeleteResolverRuleRequestRequestTypeDef definition

class DeleteResolverRuleRequestRequestTypeDef(TypedDict):
    ResolverRuleId: str,
```

## DisassociateFirewallRuleGroupRequestRequestTypeDef

```python
# DisassociateFirewallRuleGroupRequestRequestTypeDef definition

class DisassociateFirewallRuleGroupRequestRequestTypeDef(TypedDict):
    FirewallRuleGroupAssociationId: str,
```

## DisassociateResolverQueryLogConfigRequestRequestTypeDef

```python
# DisassociateResolverQueryLogConfigRequestRequestTypeDef definition

class DisassociateResolverQueryLogConfigRequestRequestTypeDef(TypedDict):
    ResolverQueryLogConfigId: str,
    ResourceId: str,
```

## DisassociateResolverRuleRequestRequestTypeDef

```python
# DisassociateResolverRuleRequestRequestTypeDef definition

class DisassociateResolverRuleRequestRequestTypeDef(TypedDict):
    VPCId: str,
    ResolverRuleId: str,
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## FirewallConfigTypeDef

```python
# FirewallConfigTypeDef definition

class FirewallConfigTypeDef(TypedDict):
    Id: NotRequired[str],
    ResourceId: NotRequired[str],
    OwnerId: NotRequired[str],
    FirewallFailOpen: NotRequired[FirewallFailOpenStatusType],  # (1)
```

1. See [:material-code-brackets: FirewallFailOpenStatusType](./literals.md#firewallfailopenstatustype) 
## FirewallDomainListMetadataTypeDef

```python
# FirewallDomainListMetadataTypeDef definition

class FirewallDomainListMetadataTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    ManagedOwnerName: NotRequired[str],
```

## FirewallRuleGroupMetadataTypeDef

```python
# FirewallRuleGroupMetadataTypeDef definition

class FirewallRuleGroupMetadataTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    OwnerId: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    ShareStatus: NotRequired[ShareStatusType],  # (1)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## GetFirewallConfigRequestRequestTypeDef

```python
# GetFirewallConfigRequestRequestTypeDef definition

class GetFirewallConfigRequestRequestTypeDef(TypedDict):
    ResourceId: str,
```

## GetFirewallDomainListRequestRequestTypeDef

```python
# GetFirewallDomainListRequestRequestTypeDef definition

class GetFirewallDomainListRequestRequestTypeDef(TypedDict):
    FirewallDomainListId: str,
```

## GetFirewallRuleGroupAssociationRequestRequestTypeDef

```python
# GetFirewallRuleGroupAssociationRequestRequestTypeDef definition

class GetFirewallRuleGroupAssociationRequestRequestTypeDef(TypedDict):
    FirewallRuleGroupAssociationId: str,
```

## GetFirewallRuleGroupPolicyRequestRequestTypeDef

```python
# GetFirewallRuleGroupPolicyRequestRequestTypeDef definition

class GetFirewallRuleGroupPolicyRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## GetFirewallRuleGroupRequestRequestTypeDef

```python
# GetFirewallRuleGroupRequestRequestTypeDef definition

class GetFirewallRuleGroupRequestRequestTypeDef(TypedDict):
    FirewallRuleGroupId: str,
```

## GetOutpostResolverRequestRequestTypeDef

```python
# GetOutpostResolverRequestRequestTypeDef definition

class GetOutpostResolverRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetResolverConfigRequestRequestTypeDef

```python
# GetResolverConfigRequestRequestTypeDef definition

class GetResolverConfigRequestRequestTypeDef(TypedDict):
    ResourceId: str,
```

## ResolverConfigTypeDef

```python
# ResolverConfigTypeDef definition

class ResolverConfigTypeDef(TypedDict):
    Id: NotRequired[str],
    ResourceId: NotRequired[str],
    OwnerId: NotRequired[str],
    AutodefinedReverse: NotRequired[ResolverAutodefinedReverseStatusType],  # (1)
```

1. See [:material-code-brackets: ResolverAutodefinedReverseStatusType](./literals.md#resolverautodefinedreversestatustype) 
## GetResolverDnssecConfigRequestRequestTypeDef

```python
# GetResolverDnssecConfigRequestRequestTypeDef definition

class GetResolverDnssecConfigRequestRequestTypeDef(TypedDict):
    ResourceId: str,
```

## ResolverDnssecConfigTypeDef

```python
# ResolverDnssecConfigTypeDef definition

class ResolverDnssecConfigTypeDef(TypedDict):
    Id: NotRequired[str],
    OwnerId: NotRequired[str],
    ResourceId: NotRequired[str],
    ValidationStatus: NotRequired[ResolverDNSSECValidationStatusType],  # (1)
```

1. See [:material-code-brackets: ResolverDNSSECValidationStatusType](./literals.md#resolverdnssecvalidationstatustype) 
## GetResolverEndpointRequestRequestTypeDef

```python
# GetResolverEndpointRequestRequestTypeDef definition

class GetResolverEndpointRequestRequestTypeDef(TypedDict):
    ResolverEndpointId: str,
```

## GetResolverQueryLogConfigAssociationRequestRequestTypeDef

```python
# GetResolverQueryLogConfigAssociationRequestRequestTypeDef definition

class GetResolverQueryLogConfigAssociationRequestRequestTypeDef(TypedDict):
    ResolverQueryLogConfigAssociationId: str,
```

## GetResolverQueryLogConfigPolicyRequestRequestTypeDef

```python
# GetResolverQueryLogConfigPolicyRequestRequestTypeDef definition

class GetResolverQueryLogConfigPolicyRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## GetResolverQueryLogConfigRequestRequestTypeDef

```python
# GetResolverQueryLogConfigRequestRequestTypeDef definition

class GetResolverQueryLogConfigRequestRequestTypeDef(TypedDict):
    ResolverQueryLogConfigId: str,
```

## GetResolverRuleAssociationRequestRequestTypeDef

```python
# GetResolverRuleAssociationRequestRequestTypeDef definition

class GetResolverRuleAssociationRequestRequestTypeDef(TypedDict):
    ResolverRuleAssociationId: str,
```

## GetResolverRulePolicyRequestRequestTypeDef

```python
# GetResolverRulePolicyRequestRequestTypeDef definition

class GetResolverRulePolicyRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## GetResolverRuleRequestRequestTypeDef

```python
# GetResolverRuleRequestRequestTypeDef definition

class GetResolverRuleRequestRequestTypeDef(TypedDict):
    ResolverRuleId: str,
```

## ImportFirewallDomainsRequestRequestTypeDef

```python
# ImportFirewallDomainsRequestRequestTypeDef definition

class ImportFirewallDomainsRequestRequestTypeDef(TypedDict):
    FirewallDomainListId: str,
    Operation: FirewallDomainImportOperationType,  # (1)
    DomainFileUrl: str,
```

1. See [:material-code-brackets: FirewallDomainImportOperationType](./literals.md#firewalldomainimportoperationtype) 
## IpAddressResponseTypeDef

```python
# IpAddressResponseTypeDef definition

class IpAddressResponseTypeDef(TypedDict):
    IpId: NotRequired[str],
    SubnetId: NotRequired[str],
    Ip: NotRequired[str],
    Ipv6: NotRequired[str],
    Status: NotRequired[IpAddressStatusType],  # (1)
    StatusMessage: NotRequired[str],
    CreationTime: NotRequired[str],
    ModificationTime: NotRequired[str],
```

1. See [:material-code-brackets: IpAddressStatusType](./literals.md#ipaddressstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListFirewallConfigsRequestRequestTypeDef

```python
# ListFirewallConfigsRequestRequestTypeDef definition

class ListFirewallConfigsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListFirewallDomainListsRequestRequestTypeDef

```python
# ListFirewallDomainListsRequestRequestTypeDef definition

class ListFirewallDomainListsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListFirewallDomainsRequestRequestTypeDef

```python
# ListFirewallDomainsRequestRequestTypeDef definition

class ListFirewallDomainsRequestRequestTypeDef(TypedDict):
    FirewallDomainListId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListFirewallRuleGroupAssociationsRequestRequestTypeDef

```python
# ListFirewallRuleGroupAssociationsRequestRequestTypeDef definition

class ListFirewallRuleGroupAssociationsRequestRequestTypeDef(TypedDict):
    FirewallRuleGroupId: NotRequired[str],
    VpcId: NotRequired[str],
    Priority: NotRequired[int],
    Status: NotRequired[FirewallRuleGroupAssociationStatusType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: FirewallRuleGroupAssociationStatusType](./literals.md#firewallrulegroupassociationstatustype) 
## ListFirewallRuleGroupsRequestRequestTypeDef

```python
# ListFirewallRuleGroupsRequestRequestTypeDef definition

class ListFirewallRuleGroupsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListFirewallRulesRequestRequestTypeDef

```python
# ListFirewallRulesRequestRequestTypeDef definition

class ListFirewallRulesRequestRequestTypeDef(TypedDict):
    FirewallRuleGroupId: str,
    Priority: NotRequired[int],
    Action: NotRequired[ActionType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## ListOutpostResolversRequestRequestTypeDef

```python
# ListOutpostResolversRequestRequestTypeDef definition

class ListOutpostResolversRequestRequestTypeDef(TypedDict):
    OutpostArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListResolverConfigsRequestRequestTypeDef

```python
# ListResolverConfigsRequestRequestTypeDef definition

class ListResolverConfigsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListResolverEndpointIpAddressesRequestRequestTypeDef

```python
# ListResolverEndpointIpAddressesRequestRequestTypeDef definition

class ListResolverEndpointIpAddressesRequestRequestTypeDef(TypedDict):
    ResolverEndpointId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PutFirewallRuleGroupPolicyRequestRequestTypeDef

```python
# PutFirewallRuleGroupPolicyRequestRequestTypeDef definition

class PutFirewallRuleGroupPolicyRequestRequestTypeDef(TypedDict):
    Arn: str,
    FirewallRuleGroupPolicy: str,
```

## PutResolverQueryLogConfigPolicyRequestRequestTypeDef

```python
# PutResolverQueryLogConfigPolicyRequestRequestTypeDef definition

class PutResolverQueryLogConfigPolicyRequestRequestTypeDef(TypedDict):
    Arn: str,
    ResolverQueryLogConfigPolicy: str,
```

## PutResolverRulePolicyRequestRequestTypeDef

```python
# PutResolverRulePolicyRequestRequestTypeDef definition

class PutResolverRulePolicyRequestRequestTypeDef(TypedDict):
    Arn: str,
    ResolverRulePolicy: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateFirewallConfigRequestRequestTypeDef

```python
# UpdateFirewallConfigRequestRequestTypeDef definition

class UpdateFirewallConfigRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    FirewallFailOpen: FirewallFailOpenStatusType,  # (1)
```

1. See [:material-code-brackets: FirewallFailOpenStatusType](./literals.md#firewallfailopenstatustype) 
## UpdateFirewallDomainsRequestRequestTypeDef

```python
# UpdateFirewallDomainsRequestRequestTypeDef definition

class UpdateFirewallDomainsRequestRequestTypeDef(TypedDict):
    FirewallDomainListId: str,
    Operation: FirewallDomainUpdateOperationType,  # (1)
    Domains: Sequence[str],
```

1. See [:material-code-brackets: FirewallDomainUpdateOperationType](./literals.md#firewalldomainupdateoperationtype) 
## UpdateFirewallRuleGroupAssociationRequestRequestTypeDef

```python
# UpdateFirewallRuleGroupAssociationRequestRequestTypeDef definition

class UpdateFirewallRuleGroupAssociationRequestRequestTypeDef(TypedDict):
    FirewallRuleGroupAssociationId: str,
    Priority: NotRequired[int],
    MutationProtection: NotRequired[MutationProtectionStatusType],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-brackets: MutationProtectionStatusType](./literals.md#mutationprotectionstatustype) 
## UpdateFirewallRuleRequestRequestTypeDef

```python
# UpdateFirewallRuleRequestRequestTypeDef definition

class UpdateFirewallRuleRequestRequestTypeDef(TypedDict):
    FirewallRuleGroupId: str,
    FirewallDomainListId: NotRequired[str],
    FirewallThreatProtectionId: NotRequired[str],
    Priority: NotRequired[int],
    Action: NotRequired[ActionType],  # (1)
    BlockResponse: NotRequired[BlockResponseType],  # (2)
    BlockOverrideDomain: NotRequired[str],
    BlockOverrideDnsType: NotRequired[BlockOverrideDnsTypeType],  # (3)
    BlockOverrideTtl: NotRequired[int],
    Name: NotRequired[str],
    FirewallDomainRedirectionAction: NotRequired[FirewallDomainRedirectionActionType],  # (4)
    Qtype: NotRequired[str],
    DnsThreatProtection: NotRequired[DnsThreatProtectionType],  # (5)
    ConfidenceThreshold: NotRequired[ConfidenceThresholdType],  # (6)
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
2. See [:material-code-brackets: BlockResponseType](./literals.md#blockresponsetype) 
3. See [:material-code-brackets: BlockOverrideDnsTypeType](./literals.md#blockoverridednstypetype) 
4. See [:material-code-brackets: FirewallDomainRedirectionActionType](./literals.md#firewalldomainredirectionactiontype) 
5. See [:material-code-brackets: DnsThreatProtectionType](./literals.md#dnsthreatprotectiontype) 
6. See [:material-code-brackets: ConfidenceThresholdType](./literals.md#confidencethresholdtype) 
## UpdateIpAddressTypeDef

```python
# UpdateIpAddressTypeDef definition

class UpdateIpAddressTypeDef(TypedDict):
    IpId: str,
    Ipv6: str,
```

## UpdateOutpostResolverRequestRequestTypeDef

```python
# UpdateOutpostResolverRequestRequestTypeDef definition

class UpdateOutpostResolverRequestRequestTypeDef(TypedDict):
    Id: str,
    Name: NotRequired[str],
    InstanceCount: NotRequired[int],
    PreferredInstanceType: NotRequired[str],
```

## UpdateResolverConfigRequestRequestTypeDef

```python
# UpdateResolverConfigRequestRequestTypeDef definition

class UpdateResolverConfigRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    AutodefinedReverseFlag: AutodefinedReverseFlagType,  # (1)
```

1. See [:material-code-brackets: AutodefinedReverseFlagType](./literals.md#autodefinedreverseflagtype) 
## UpdateResolverDnssecConfigRequestRequestTypeDef

```python
# UpdateResolverDnssecConfigRequestRequestTypeDef definition

class UpdateResolverDnssecConfigRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    Validation: ValidationType,  # (1)
```

1. See [:material-code-brackets: ValidationType](./literals.md#validationtype) 
## AssociateFirewallRuleGroupRequestRequestTypeDef

```python
# AssociateFirewallRuleGroupRequestRequestTypeDef definition

class AssociateFirewallRuleGroupRequestRequestTypeDef(TypedDict):
    CreatorRequestId: str,
    FirewallRuleGroupId: str,
    VpcId: str,
    Priority: int,
    Name: str,
    MutationProtection: NotRequired[MutationProtectionStatusType],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: MutationProtectionStatusType](./literals.md#mutationprotectionstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateFirewallDomainListRequestRequestTypeDef

```python
# CreateFirewallDomainListRequestRequestTypeDef definition

class CreateFirewallDomainListRequestRequestTypeDef(TypedDict):
    CreatorRequestId: str,
    Name: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateFirewallRuleGroupRequestRequestTypeDef

```python
# CreateFirewallRuleGroupRequestRequestTypeDef definition

class CreateFirewallRuleGroupRequestRequestTypeDef(TypedDict):
    CreatorRequestId: str,
    Name: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateOutpostResolverRequestRequestTypeDef

```python
# CreateOutpostResolverRequestRequestTypeDef definition

class CreateOutpostResolverRequestRequestTypeDef(TypedDict):
    CreatorRequestId: str,
    Name: str,
    PreferredInstanceType: str,
    OutpostArn: str,
    InstanceCount: NotRequired[int],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateResolverQueryLogConfigRequestRequestTypeDef

```python
# CreateResolverQueryLogConfigRequestRequestTypeDef definition

class CreateResolverQueryLogConfigRequestRequestTypeDef(TypedDict):
    Name: str,
    DestinationArn: str,
    CreatorRequestId: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AssociateFirewallRuleGroupResponseTypeDef

```python
# AssociateFirewallRuleGroupResponseTypeDef definition

class AssociateFirewallRuleGroupResponseTypeDef(TypedDict):
    FirewallRuleGroupAssociation: FirewallRuleGroupAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallRuleGroupAssociationTypeDef](./type_defs.md#firewallrulegroupassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateFirewallRuleGroupResponseTypeDef

```python
# DisassociateFirewallRuleGroupResponseTypeDef definition

class DisassociateFirewallRuleGroupResponseTypeDef(TypedDict):
    FirewallRuleGroupAssociation: FirewallRuleGroupAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallRuleGroupAssociationTypeDef](./type_defs.md#firewallrulegroupassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFirewallRuleGroupAssociationResponseTypeDef

```python
# GetFirewallRuleGroupAssociationResponseTypeDef definition

class GetFirewallRuleGroupAssociationResponseTypeDef(TypedDict):
    FirewallRuleGroupAssociation: FirewallRuleGroupAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallRuleGroupAssociationTypeDef](./type_defs.md#firewallrulegroupassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFirewallRuleGroupPolicyResponseTypeDef

```python
# GetFirewallRuleGroupPolicyResponseTypeDef definition

class GetFirewallRuleGroupPolicyResponseTypeDef(TypedDict):
    FirewallRuleGroupPolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResolverQueryLogConfigPolicyResponseTypeDef

```python
# GetResolverQueryLogConfigPolicyResponseTypeDef definition

class GetResolverQueryLogConfigPolicyResponseTypeDef(TypedDict):
    ResolverQueryLogConfigPolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResolverRulePolicyResponseTypeDef

```python
# GetResolverRulePolicyResponseTypeDef definition

class GetResolverRulePolicyResponseTypeDef(TypedDict):
    ResolverRulePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportFirewallDomainsResponseTypeDef

```python
# ImportFirewallDomainsResponseTypeDef definition

class ImportFirewallDomainsResponseTypeDef(TypedDict):
    Id: str,
    Name: str,
    Status: FirewallDomainListStatusType,  # (1)
    StatusMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FirewallDomainListStatusType](./literals.md#firewalldomainliststatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFirewallDomainsResponseTypeDef

```python
# ListFirewallDomainsResponseTypeDef definition

class ListFirewallDomainsResponseTypeDef(TypedDict):
    Domains: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFirewallRuleGroupAssociationsResponseTypeDef

```python
# ListFirewallRuleGroupAssociationsResponseTypeDef definition

class ListFirewallRuleGroupAssociationsResponseTypeDef(TypedDict):
    FirewallRuleGroupAssociations: List[FirewallRuleGroupAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FirewallRuleGroupAssociationTypeDef](./type_defs.md#firewallrulegroupassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutFirewallRuleGroupPolicyResponseTypeDef

```python
# PutFirewallRuleGroupPolicyResponseTypeDef definition

class PutFirewallRuleGroupPolicyResponseTypeDef(TypedDict):
    ReturnValue: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResolverQueryLogConfigPolicyResponseTypeDef

```python
# PutResolverQueryLogConfigPolicyResponseTypeDef definition

class PutResolverQueryLogConfigPolicyResponseTypeDef(TypedDict):
    ReturnValue: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResolverRulePolicyResponseTypeDef

```python
# PutResolverRulePolicyResponseTypeDef definition

class PutResolverRulePolicyResponseTypeDef(TypedDict):
    ReturnValue: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFirewallDomainsResponseTypeDef

```python
# UpdateFirewallDomainsResponseTypeDef definition

class UpdateFirewallDomainsResponseTypeDef(TypedDict):
    Id: str,
    Name: str,
    Status: FirewallDomainListStatusType,  # (1)
    StatusMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FirewallDomainListStatusType](./literals.md#firewalldomainliststatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFirewallRuleGroupAssociationResponseTypeDef

```python
# UpdateFirewallRuleGroupAssociationResponseTypeDef definition

class UpdateFirewallRuleGroupAssociationResponseTypeDef(TypedDict):
    FirewallRuleGroupAssociation: FirewallRuleGroupAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallRuleGroupAssociationTypeDef](./type_defs.md#firewallrulegroupassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateResolverEndpointIpAddressRequestRequestTypeDef

```python
# AssociateResolverEndpointIpAddressRequestRequestTypeDef definition

class AssociateResolverEndpointIpAddressRequestRequestTypeDef(TypedDict):
    ResolverEndpointId: str,
    IpAddress: IpAddressUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: IpAddressUpdateTypeDef](./type_defs.md#ipaddressupdatetypedef) 
## DisassociateResolverEndpointIpAddressRequestRequestTypeDef

```python
# DisassociateResolverEndpointIpAddressRequestRequestTypeDef definition

class DisassociateResolverEndpointIpAddressRequestRequestTypeDef(TypedDict):
    ResolverEndpointId: str,
    IpAddress: IpAddressUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: IpAddressUpdateTypeDef](./type_defs.md#ipaddressupdatetypedef) 
## AssociateResolverEndpointIpAddressResponseTypeDef

```python
# AssociateResolverEndpointIpAddressResponseTypeDef definition

class AssociateResolverEndpointIpAddressResponseTypeDef(TypedDict):
    ResolverEndpoint: ResolverEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverEndpointTypeDef](./type_defs.md#resolverendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResolverEndpointResponseTypeDef

```python
# CreateResolverEndpointResponseTypeDef definition

class CreateResolverEndpointResponseTypeDef(TypedDict):
    ResolverEndpoint: ResolverEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverEndpointTypeDef](./type_defs.md#resolverendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResolverEndpointResponseTypeDef

```python
# DeleteResolverEndpointResponseTypeDef definition

class DeleteResolverEndpointResponseTypeDef(TypedDict):
    ResolverEndpoint: ResolverEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverEndpointTypeDef](./type_defs.md#resolverendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateResolverEndpointIpAddressResponseTypeDef

```python
# DisassociateResolverEndpointIpAddressResponseTypeDef definition

class DisassociateResolverEndpointIpAddressResponseTypeDef(TypedDict):
    ResolverEndpoint: ResolverEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverEndpointTypeDef](./type_defs.md#resolverendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResolverEndpointResponseTypeDef

```python
# GetResolverEndpointResponseTypeDef definition

class GetResolverEndpointResponseTypeDef(TypedDict):
    ResolverEndpoint: ResolverEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverEndpointTypeDef](./type_defs.md#resolverendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResolverEndpointsResponseTypeDef

```python
# ListResolverEndpointsResponseTypeDef definition

class ListResolverEndpointsResponseTypeDef(TypedDict):
    MaxResults: int,
    ResolverEndpoints: List[ResolverEndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResolverEndpointTypeDef](./type_defs.md#resolverendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResolverEndpointResponseTypeDef

```python
# UpdateResolverEndpointResponseTypeDef definition

class UpdateResolverEndpointResponseTypeDef(TypedDict):
    ResolverEndpoint: ResolverEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverEndpointTypeDef](./type_defs.md#resolverendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateResolverQueryLogConfigResponseTypeDef

```python
# AssociateResolverQueryLogConfigResponseTypeDef definition

class AssociateResolverQueryLogConfigResponseTypeDef(TypedDict):
    ResolverQueryLogConfigAssociation: ResolverQueryLogConfigAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverQueryLogConfigAssociationTypeDef](./type_defs.md#resolverquerylogconfigassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateResolverQueryLogConfigResponseTypeDef

```python
# DisassociateResolverQueryLogConfigResponseTypeDef definition

class DisassociateResolverQueryLogConfigResponseTypeDef(TypedDict):
    ResolverQueryLogConfigAssociation: ResolverQueryLogConfigAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverQueryLogConfigAssociationTypeDef](./type_defs.md#resolverquerylogconfigassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResolverQueryLogConfigAssociationResponseTypeDef

```python
# GetResolverQueryLogConfigAssociationResponseTypeDef definition

class GetResolverQueryLogConfigAssociationResponseTypeDef(TypedDict):
    ResolverQueryLogConfigAssociation: ResolverQueryLogConfigAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverQueryLogConfigAssociationTypeDef](./type_defs.md#resolverquerylogconfigassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResolverQueryLogConfigAssociationsResponseTypeDef

```python
# ListResolverQueryLogConfigAssociationsResponseTypeDef definition

class ListResolverQueryLogConfigAssociationsResponseTypeDef(TypedDict):
    TotalCount: int,
    TotalFilteredCount: int,
    ResolverQueryLogConfigAssociations: List[ResolverQueryLogConfigAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResolverQueryLogConfigAssociationTypeDef](./type_defs.md#resolverquerylogconfigassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateResolverRuleResponseTypeDef

```python
# AssociateResolverRuleResponseTypeDef definition

class AssociateResolverRuleResponseTypeDef(TypedDict):
    ResolverRuleAssociation: ResolverRuleAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverRuleAssociationTypeDef](./type_defs.md#resolverruleassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateResolverRuleResponseTypeDef

```python
# DisassociateResolverRuleResponseTypeDef definition

class DisassociateResolverRuleResponseTypeDef(TypedDict):
    ResolverRuleAssociation: ResolverRuleAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverRuleAssociationTypeDef](./type_defs.md#resolverruleassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResolverRuleAssociationResponseTypeDef

```python
# GetResolverRuleAssociationResponseTypeDef definition

class GetResolverRuleAssociationResponseTypeDef(TypedDict):
    ResolverRuleAssociation: ResolverRuleAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverRuleAssociationTypeDef](./type_defs.md#resolverruleassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResolverRuleAssociationsResponseTypeDef

```python
# ListResolverRuleAssociationsResponseTypeDef definition

class ListResolverRuleAssociationsResponseTypeDef(TypedDict):
    MaxResults: int,
    ResolverRuleAssociations: List[ResolverRuleAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResolverRuleAssociationTypeDef](./type_defs.md#resolverruleassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFirewallDomainListResponseTypeDef

```python
# CreateFirewallDomainListResponseTypeDef definition

class CreateFirewallDomainListResponseTypeDef(TypedDict):
    FirewallDomainList: FirewallDomainListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallDomainListTypeDef](./type_defs.md#firewalldomainlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFirewallDomainListResponseTypeDef

```python
# DeleteFirewallDomainListResponseTypeDef definition

class DeleteFirewallDomainListResponseTypeDef(TypedDict):
    FirewallDomainList: FirewallDomainListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallDomainListTypeDef](./type_defs.md#firewalldomainlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFirewallDomainListResponseTypeDef

```python
# GetFirewallDomainListResponseTypeDef definition

class GetFirewallDomainListResponseTypeDef(TypedDict):
    FirewallDomainList: FirewallDomainListTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallDomainListTypeDef](./type_defs.md#firewalldomainlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFirewallRuleGroupResponseTypeDef

```python
# CreateFirewallRuleGroupResponseTypeDef definition

class CreateFirewallRuleGroupResponseTypeDef(TypedDict):
    FirewallRuleGroup: FirewallRuleGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallRuleGroupTypeDef](./type_defs.md#firewallrulegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFirewallRuleGroupResponseTypeDef

```python
# DeleteFirewallRuleGroupResponseTypeDef definition

class DeleteFirewallRuleGroupResponseTypeDef(TypedDict):
    FirewallRuleGroup: FirewallRuleGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallRuleGroupTypeDef](./type_defs.md#firewallrulegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFirewallRuleGroupResponseTypeDef

```python
# GetFirewallRuleGroupResponseTypeDef definition

class GetFirewallRuleGroupResponseTypeDef(TypedDict):
    FirewallRuleGroup: FirewallRuleGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallRuleGroupTypeDef](./type_defs.md#firewallrulegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFirewallRuleResponseTypeDef

```python
# CreateFirewallRuleResponseTypeDef definition

class CreateFirewallRuleResponseTypeDef(TypedDict):
    FirewallRule: FirewallRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallRuleTypeDef](./type_defs.md#firewallruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFirewallRuleResponseTypeDef

```python
# DeleteFirewallRuleResponseTypeDef definition

class DeleteFirewallRuleResponseTypeDef(TypedDict):
    FirewallRule: FirewallRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallRuleTypeDef](./type_defs.md#firewallruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFirewallRulesResponseTypeDef

```python
# ListFirewallRulesResponseTypeDef definition

class ListFirewallRulesResponseTypeDef(TypedDict):
    FirewallRules: List[FirewallRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FirewallRuleTypeDef](./type_defs.md#firewallruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFirewallRuleResponseTypeDef

```python
# UpdateFirewallRuleResponseTypeDef definition

class UpdateFirewallRuleResponseTypeDef(TypedDict):
    FirewallRule: FirewallRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallRuleTypeDef](./type_defs.md#firewallruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateOutpostResolverResponseTypeDef

```python
# CreateOutpostResolverResponseTypeDef definition

class CreateOutpostResolverResponseTypeDef(TypedDict):
    OutpostResolver: OutpostResolverTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutpostResolverTypeDef](./type_defs.md#outpostresolvertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteOutpostResolverResponseTypeDef

```python
# DeleteOutpostResolverResponseTypeDef definition

class DeleteOutpostResolverResponseTypeDef(TypedDict):
    OutpostResolver: OutpostResolverTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutpostResolverTypeDef](./type_defs.md#outpostresolvertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOutpostResolverResponseTypeDef

```python
# GetOutpostResolverResponseTypeDef definition

class GetOutpostResolverResponseTypeDef(TypedDict):
    OutpostResolver: OutpostResolverTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutpostResolverTypeDef](./type_defs.md#outpostresolvertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOutpostResolversResponseTypeDef

```python
# ListOutpostResolversResponseTypeDef definition

class ListOutpostResolversResponseTypeDef(TypedDict):
    OutpostResolvers: List[OutpostResolverTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OutpostResolverTypeDef](./type_defs.md#outpostresolvertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOutpostResolverResponseTypeDef

```python
# UpdateOutpostResolverResponseTypeDef definition

class UpdateOutpostResolverResponseTypeDef(TypedDict):
    OutpostResolver: OutpostResolverTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutpostResolverTypeDef](./type_defs.md#outpostresolvertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResolverEndpointRequestRequestTypeDef

```python
# CreateResolverEndpointRequestRequestTypeDef definition

class CreateResolverEndpointRequestRequestTypeDef(TypedDict):
    CreatorRequestId: str,
    SecurityGroupIds: Sequence[str],
    Direction: ResolverEndpointDirectionType,  # (1)
    IpAddresses: Sequence[IpAddressRequestTypeDef],  # (2)
    Name: NotRequired[str],
    OutpostArn: NotRequired[str],
    PreferredInstanceType: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    ResolverEndpointType: NotRequired[ResolverEndpointTypeType],  # (4)
    Protocols: NotRequired[Sequence[ProtocolType]],  # (5)
```

1. See [:material-code-brackets: ResolverEndpointDirectionType](./literals.md#resolverendpointdirectiontype) 
2. See [:material-code-braces: IpAddressRequestTypeDef](./type_defs.md#ipaddressrequesttypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: ResolverEndpointTypeType](./literals.md#resolverendpointtypetype) 
5. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## CreateResolverQueryLogConfigResponseTypeDef

```python
# CreateResolverQueryLogConfigResponseTypeDef definition

class CreateResolverQueryLogConfigResponseTypeDef(TypedDict):
    ResolverQueryLogConfig: ResolverQueryLogConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverQueryLogConfigTypeDef](./type_defs.md#resolverquerylogconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResolverQueryLogConfigResponseTypeDef

```python
# DeleteResolverQueryLogConfigResponseTypeDef definition

class DeleteResolverQueryLogConfigResponseTypeDef(TypedDict):
    ResolverQueryLogConfig: ResolverQueryLogConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverQueryLogConfigTypeDef](./type_defs.md#resolverquerylogconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResolverQueryLogConfigResponseTypeDef

```python
# GetResolverQueryLogConfigResponseTypeDef definition

class GetResolverQueryLogConfigResponseTypeDef(TypedDict):
    ResolverQueryLogConfig: ResolverQueryLogConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverQueryLogConfigTypeDef](./type_defs.md#resolverquerylogconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResolverQueryLogConfigsResponseTypeDef

```python
# ListResolverQueryLogConfigsResponseTypeDef definition

class ListResolverQueryLogConfigsResponseTypeDef(TypedDict):
    TotalCount: int,
    TotalFilteredCount: int,
    ResolverQueryLogConfigs: List[ResolverQueryLogConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResolverQueryLogConfigTypeDef](./type_defs.md#resolverquerylogconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResolverRuleRequestRequestTypeDef

```python
# CreateResolverRuleRequestRequestTypeDef definition

class CreateResolverRuleRequestRequestTypeDef(TypedDict):
    CreatorRequestId: str,
    RuleType: RuleTypeOptionType,  # (1)
    Name: NotRequired[str],
    DomainName: NotRequired[str],
    TargetIps: NotRequired[Sequence[TargetAddressTypeDef]],  # (2)
    ResolverEndpointId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: RuleTypeOptionType](./literals.md#ruletypeoptiontype) 
2. See [:material-code-braces: TargetAddressTypeDef](./type_defs.md#targetaddresstypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ResolverRuleConfigTypeDef

```python
# ResolverRuleConfigTypeDef definition

class ResolverRuleConfigTypeDef(TypedDict):
    Name: NotRequired[str],
    TargetIps: NotRequired[Sequence[TargetAddressTypeDef]],  # (1)
    ResolverEndpointId: NotRequired[str],
```

1. See [:material-code-braces: TargetAddressTypeDef](./type_defs.md#targetaddresstypedef) 
## ResolverRuleTypeDef

```python
# ResolverRuleTypeDef definition

class ResolverRuleTypeDef(TypedDict):
    Id: NotRequired[str],
    CreatorRequestId: NotRequired[str],
    Arn: NotRequired[str],
    DomainName: NotRequired[str],
    Status: NotRequired[ResolverRuleStatusType],  # (1)
    StatusMessage: NotRequired[str],
    RuleType: NotRequired[RuleTypeOptionType],  # (2)
    Name: NotRequired[str],
    TargetIps: NotRequired[List[TargetAddressTypeDef]],  # (3)
    ResolverEndpointId: NotRequired[str],
    OwnerId: NotRequired[str],
    ShareStatus: NotRequired[ShareStatusType],  # (4)
    CreationTime: NotRequired[str],
    ModificationTime: NotRequired[str],
```

1. See [:material-code-brackets: ResolverRuleStatusType](./literals.md#resolverrulestatustype) 
2. See [:material-code-brackets: RuleTypeOptionType](./literals.md#ruletypeoptiontype) 
3. See [:material-code-braces: TargetAddressTypeDef](./type_defs.md#targetaddresstypedef) 
4. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## ListResolverDnssecConfigsRequestRequestTypeDef

```python
# ListResolverDnssecConfigsRequestRequestTypeDef definition

class ListResolverDnssecConfigsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListResolverEndpointsRequestRequestTypeDef

```python
# ListResolverEndpointsRequestRequestTypeDef definition

class ListResolverEndpointsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListResolverQueryLogConfigAssociationsRequestRequestTypeDef

```python
# ListResolverQueryLogConfigAssociationsRequestRequestTypeDef definition

class ListResolverQueryLogConfigAssociationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListResolverQueryLogConfigsRequestRequestTypeDef

```python
# ListResolverQueryLogConfigsRequestRequestTypeDef definition

class ListResolverQueryLogConfigsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListResolverRuleAssociationsRequestRequestTypeDef

```python
# ListResolverRuleAssociationsRequestRequestTypeDef definition

class ListResolverRuleAssociationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListResolverRulesRequestRequestTypeDef

```python
# ListResolverRulesRequestRequestTypeDef definition

class ListResolverRulesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetFirewallConfigResponseTypeDef

```python
# GetFirewallConfigResponseTypeDef definition

class GetFirewallConfigResponseTypeDef(TypedDict):
    FirewallConfig: FirewallConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallConfigTypeDef](./type_defs.md#firewallconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFirewallConfigsResponseTypeDef

```python
# ListFirewallConfigsResponseTypeDef definition

class ListFirewallConfigsResponseTypeDef(TypedDict):
    FirewallConfigs: List[FirewallConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FirewallConfigTypeDef](./type_defs.md#firewallconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFirewallConfigResponseTypeDef

```python
# UpdateFirewallConfigResponseTypeDef definition

class UpdateFirewallConfigResponseTypeDef(TypedDict):
    FirewallConfig: FirewallConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallConfigTypeDef](./type_defs.md#firewallconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFirewallDomainListsResponseTypeDef

```python
# ListFirewallDomainListsResponseTypeDef definition

class ListFirewallDomainListsResponseTypeDef(TypedDict):
    FirewallDomainLists: List[FirewallDomainListMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FirewallDomainListMetadataTypeDef](./type_defs.md#firewalldomainlistmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFirewallRuleGroupsResponseTypeDef

```python
# ListFirewallRuleGroupsResponseTypeDef definition

class ListFirewallRuleGroupsResponseTypeDef(TypedDict):
    FirewallRuleGroups: List[FirewallRuleGroupMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FirewallRuleGroupMetadataTypeDef](./type_defs.md#firewallrulegroupmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResolverConfigResponseTypeDef

```python
# GetResolverConfigResponseTypeDef definition

class GetResolverConfigResponseTypeDef(TypedDict):
    ResolverConfig: ResolverConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverConfigTypeDef](./type_defs.md#resolverconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResolverConfigsResponseTypeDef

```python
# ListResolverConfigsResponseTypeDef definition

class ListResolverConfigsResponseTypeDef(TypedDict):
    ResolverConfigs: List[ResolverConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResolverConfigTypeDef](./type_defs.md#resolverconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResolverConfigResponseTypeDef

```python
# UpdateResolverConfigResponseTypeDef definition

class UpdateResolverConfigResponseTypeDef(TypedDict):
    ResolverConfig: ResolverConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverConfigTypeDef](./type_defs.md#resolverconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResolverDnssecConfigResponseTypeDef

```python
# GetResolverDnssecConfigResponseTypeDef definition

class GetResolverDnssecConfigResponseTypeDef(TypedDict):
    ResolverDNSSECConfig: ResolverDnssecConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverDnssecConfigTypeDef](./type_defs.md#resolverdnssecconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResolverDnssecConfigsResponseTypeDef

```python
# ListResolverDnssecConfigsResponseTypeDef definition

class ListResolverDnssecConfigsResponseTypeDef(TypedDict):
    ResolverDnssecConfigs: List[ResolverDnssecConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResolverDnssecConfigTypeDef](./type_defs.md#resolverdnssecconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResolverDnssecConfigResponseTypeDef

```python
# UpdateResolverDnssecConfigResponseTypeDef definition

class UpdateResolverDnssecConfigResponseTypeDef(TypedDict):
    ResolverDNSSECConfig: ResolverDnssecConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverDnssecConfigTypeDef](./type_defs.md#resolverdnssecconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResolverEndpointIpAddressesResponseTypeDef

```python
# ListResolverEndpointIpAddressesResponseTypeDef definition

class ListResolverEndpointIpAddressesResponseTypeDef(TypedDict):
    MaxResults: int,
    IpAddresses: List[IpAddressResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IpAddressResponseTypeDef](./type_defs.md#ipaddressresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFirewallConfigsRequestPaginateTypeDef

```python
# ListFirewallConfigsRequestPaginateTypeDef definition

class ListFirewallConfigsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFirewallDomainListsRequestPaginateTypeDef

```python
# ListFirewallDomainListsRequestPaginateTypeDef definition

class ListFirewallDomainListsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFirewallDomainsRequestPaginateTypeDef

```python
# ListFirewallDomainsRequestPaginateTypeDef definition

class ListFirewallDomainsRequestPaginateTypeDef(TypedDict):
    FirewallDomainListId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFirewallRuleGroupAssociationsRequestPaginateTypeDef

```python
# ListFirewallRuleGroupAssociationsRequestPaginateTypeDef definition

class ListFirewallRuleGroupAssociationsRequestPaginateTypeDef(TypedDict):
    FirewallRuleGroupId: NotRequired[str],
    VpcId: NotRequired[str],
    Priority: NotRequired[int],
    Status: NotRequired[FirewallRuleGroupAssociationStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FirewallRuleGroupAssociationStatusType](./literals.md#firewallrulegroupassociationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFirewallRuleGroupsRequestPaginateTypeDef

```python
# ListFirewallRuleGroupsRequestPaginateTypeDef definition

class ListFirewallRuleGroupsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFirewallRulesRequestPaginateTypeDef

```python
# ListFirewallRulesRequestPaginateTypeDef definition

class ListFirewallRulesRequestPaginateTypeDef(TypedDict):
    FirewallRuleGroupId: str,
    Priority: NotRequired[int],
    Action: NotRequired[ActionType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOutpostResolversRequestPaginateTypeDef

```python
# ListOutpostResolversRequestPaginateTypeDef definition

class ListOutpostResolversRequestPaginateTypeDef(TypedDict):
    OutpostArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResolverConfigsRequestPaginateTypeDef

```python
# ListResolverConfigsRequestPaginateTypeDef definition

class ListResolverConfigsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResolverDnssecConfigsRequestPaginateTypeDef

```python
# ListResolverDnssecConfigsRequestPaginateTypeDef definition

class ListResolverDnssecConfigsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResolverEndpointIpAddressesRequestPaginateTypeDef

```python
# ListResolverEndpointIpAddressesRequestPaginateTypeDef definition

class ListResolverEndpointIpAddressesRequestPaginateTypeDef(TypedDict):
    ResolverEndpointId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResolverEndpointsRequestPaginateTypeDef

```python
# ListResolverEndpointsRequestPaginateTypeDef definition

class ListResolverEndpointsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResolverQueryLogConfigAssociationsRequestPaginateTypeDef

```python
# ListResolverQueryLogConfigAssociationsRequestPaginateTypeDef definition

class ListResolverQueryLogConfigAssociationsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResolverQueryLogConfigsRequestPaginateTypeDef

```python
# ListResolverQueryLogConfigsRequestPaginateTypeDef definition

class ListResolverQueryLogConfigsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResolverRuleAssociationsRequestPaginateTypeDef

```python
# ListResolverRuleAssociationsRequestPaginateTypeDef definition

class ListResolverRuleAssociationsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResolverRulesRequestPaginateTypeDef

```python
# ListResolverRulesRequestPaginateTypeDef definition

class ListResolverRulesRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestPaginateTypeDef

```python
# ListTagsForResourceRequestPaginateTypeDef definition

class ListTagsForResourceRequestPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## UpdateResolverEndpointRequestRequestTypeDef

```python
# UpdateResolverEndpointRequestRequestTypeDef definition

class UpdateResolverEndpointRequestRequestTypeDef(TypedDict):
    ResolverEndpointId: str,
    Name: NotRequired[str],
    ResolverEndpointType: NotRequired[ResolverEndpointTypeType],  # (1)
    UpdateIpAddresses: NotRequired[Sequence[UpdateIpAddressTypeDef]],  # (2)
    Protocols: NotRequired[Sequence[ProtocolType]],  # (3)
```

1. See [:material-code-brackets: ResolverEndpointTypeType](./literals.md#resolverendpointtypetype) 
2. See [:material-code-braces: UpdateIpAddressTypeDef](./type_defs.md#updateipaddresstypedef) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## UpdateResolverRuleRequestRequestTypeDef

```python
# UpdateResolverRuleRequestRequestTypeDef definition

class UpdateResolverRuleRequestRequestTypeDef(TypedDict):
    ResolverRuleId: str,
    Config: ResolverRuleConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ResolverRuleConfigTypeDef](./type_defs.md#resolverruleconfigtypedef) 
## CreateResolverRuleResponseTypeDef

```python
# CreateResolverRuleResponseTypeDef definition

class CreateResolverRuleResponseTypeDef(TypedDict):
    ResolverRule: ResolverRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverRuleTypeDef](./type_defs.md#resolverruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResolverRuleResponseTypeDef

```python
# DeleteResolverRuleResponseTypeDef definition

class DeleteResolverRuleResponseTypeDef(TypedDict):
    ResolverRule: ResolverRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverRuleTypeDef](./type_defs.md#resolverruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResolverRuleResponseTypeDef

```python
# GetResolverRuleResponseTypeDef definition

class GetResolverRuleResponseTypeDef(TypedDict):
    ResolverRule: ResolverRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverRuleTypeDef](./type_defs.md#resolverruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResolverRulesResponseTypeDef

```python
# ListResolverRulesResponseTypeDef definition

class ListResolverRulesResponseTypeDef(TypedDict):
    MaxResults: int,
    ResolverRules: List[ResolverRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResolverRuleTypeDef](./type_defs.md#resolverruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResolverRuleResponseTypeDef

```python
# UpdateResolverRuleResponseTypeDef definition

class UpdateResolverRuleResponseTypeDef(TypedDict):
    ResolverRule: ResolverRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResolverRuleTypeDef](./type_defs.md#resolverruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
