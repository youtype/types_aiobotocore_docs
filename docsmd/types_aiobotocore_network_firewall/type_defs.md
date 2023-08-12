# Type definitions

> [Index](../README.md) > [NetworkFirewall](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [NetworkFirewall](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
    type annotations stubs module [types-aiobotocore-network-firewall](https://pypi.org/project/types-aiobotocore-network-firewall/).



## AddressTypeDef

```python
# AddressTypeDef definition

class AddressTypeDef(TypedDict):
    AddressDefinition: str,
```

## AssociateFirewallPolicyRequestRequestTypeDef

```python
# AssociateFirewallPolicyRequestRequestTypeDef definition

class AssociateFirewallPolicyRequestRequestTypeDef(TypedDict):
    FirewallPolicyArn: str,
    UpdateToken: NotRequired[str],
    FirewallArn: NotRequired[str],
    FirewallName: NotRequired[str],
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

## SubnetMappingTypeDef

```python
# SubnetMappingTypeDef definition

class SubnetMappingTypeDef(TypedDict):
    SubnetId: str,
    IPAddressType: NotRequired[IPAddressTypeType],  # (1)
```

1. See [:material-code-brackets: IPAddressTypeType](./literals.md#ipaddresstypetype) 
## AttachmentTypeDef

```python
# AttachmentTypeDef definition

class AttachmentTypeDef(TypedDict):
    SubnetId: NotRequired[str],
    EndpointId: NotRequired[str],
    Status: NotRequired[AttachmentStatusType],  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: AttachmentStatusType](./literals.md#attachmentstatustype) 
## IPSetMetadataTypeDef

```python
# IPSetMetadataTypeDef definition

class IPSetMetadataTypeDef(TypedDict):
    ResolvedCIDRCount: NotRequired[int],
```

## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    Type: EncryptionTypeType,  # (1)
    KeyId: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## SourceMetadataTypeDef

```python
# SourceMetadataTypeDef definition

class SourceMetadataTypeDef(TypedDict):
    SourceArn: NotRequired[str],
    SourceUpdateToken: NotRequired[str],
```

## DeleteFirewallPolicyRequestRequestTypeDef

```python
# DeleteFirewallPolicyRequestRequestTypeDef definition

class DeleteFirewallPolicyRequestRequestTypeDef(TypedDict):
    FirewallPolicyName: NotRequired[str],
    FirewallPolicyArn: NotRequired[str],
```

## DeleteFirewallRequestRequestTypeDef

```python
# DeleteFirewallRequestRequestTypeDef definition

class DeleteFirewallRequestRequestTypeDef(TypedDict):
    FirewallName: NotRequired[str],
    FirewallArn: NotRequired[str],
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DeleteRuleGroupRequestRequestTypeDef

```python
# DeleteRuleGroupRequestRequestTypeDef definition

class DeleteRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupName: NotRequired[str],
    RuleGroupArn: NotRequired[str],
    Type: NotRequired[RuleGroupTypeType],  # (1)
```

1. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype) 
## DeleteTLSInspectionConfigurationRequestRequestTypeDef

```python
# DeleteTLSInspectionConfigurationRequestRequestTypeDef definition

class DeleteTLSInspectionConfigurationRequestRequestTypeDef(TypedDict):
    TLSInspectionConfigurationArn: NotRequired[str],
    TLSInspectionConfigurationName: NotRequired[str],
```

## DescribeFirewallPolicyRequestRequestTypeDef

```python
# DescribeFirewallPolicyRequestRequestTypeDef definition

class DescribeFirewallPolicyRequestRequestTypeDef(TypedDict):
    FirewallPolicyName: NotRequired[str],
    FirewallPolicyArn: NotRequired[str],
```

## DescribeFirewallRequestRequestTypeDef

```python
# DescribeFirewallRequestRequestTypeDef definition

class DescribeFirewallRequestRequestTypeDef(TypedDict):
    FirewallName: NotRequired[str],
    FirewallArn: NotRequired[str],
```

## DescribeLoggingConfigurationRequestRequestTypeDef

```python
# DescribeLoggingConfigurationRequestRequestTypeDef definition

class DescribeLoggingConfigurationRequestRequestTypeDef(TypedDict):
    FirewallArn: NotRequired[str],
    FirewallName: NotRequired[str],
```

## DescribeResourcePolicyRequestRequestTypeDef

```python
# DescribeResourcePolicyRequestRequestTypeDef definition

class DescribeResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DescribeRuleGroupMetadataRequestRequestTypeDef

```python
# DescribeRuleGroupMetadataRequestRequestTypeDef definition

class DescribeRuleGroupMetadataRequestRequestTypeDef(TypedDict):
    RuleGroupName: NotRequired[str],
    RuleGroupArn: NotRequired[str],
    Type: NotRequired[RuleGroupTypeType],  # (1)
```

1. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype) 
## StatefulRuleOptionsTypeDef

```python
# StatefulRuleOptionsTypeDef definition

class StatefulRuleOptionsTypeDef(TypedDict):
    RuleOrder: NotRequired[RuleOrderType],  # (1)
```

1. See [:material-code-brackets: RuleOrderType](./literals.md#ruleordertype) 
## DescribeRuleGroupRequestRequestTypeDef

```python
# DescribeRuleGroupRequestRequestTypeDef definition

class DescribeRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupName: NotRequired[str],
    RuleGroupArn: NotRequired[str],
    Type: NotRequired[RuleGroupTypeType],  # (1)
```

1. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype) 
## DescribeTLSInspectionConfigurationRequestRequestTypeDef

```python
# DescribeTLSInspectionConfigurationRequestRequestTypeDef definition

class DescribeTLSInspectionConfigurationRequestRequestTypeDef(TypedDict):
    TLSInspectionConfigurationArn: NotRequired[str],
    TLSInspectionConfigurationName: NotRequired[str],
```

## DimensionTypeDef

```python
# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    Value: str,
```

## DisassociateSubnetsRequestRequestTypeDef

```python
# DisassociateSubnetsRequestRequestTypeDef definition

class DisassociateSubnetsRequestRequestTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    UpdateToken: NotRequired[str],
    FirewallArn: NotRequired[str],
    FirewallName: NotRequired[str],
```

## FirewallMetadataTypeDef

```python
# FirewallMetadataTypeDef definition

class FirewallMetadataTypeDef(TypedDict):
    FirewallName: NotRequired[str],
    FirewallArn: NotRequired[str],
```

## FirewallPolicyMetadataTypeDef

```python
# FirewallPolicyMetadataTypeDef definition

class FirewallPolicyMetadataTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
```

## StatefulEngineOptionsTypeDef

```python
# StatefulEngineOptionsTypeDef definition

class StatefulEngineOptionsTypeDef(TypedDict):
    RuleOrder: NotRequired[RuleOrderType],  # (1)
    StreamExceptionPolicy: NotRequired[StreamExceptionPolicyType],  # (2)
```

1. See [:material-code-brackets: RuleOrderType](./literals.md#ruleordertype) 
2. See [:material-code-brackets: StreamExceptionPolicyType](./literals.md#streamexceptionpolicytype) 
## StatelessRuleGroupReferenceTypeDef

```python
# StatelessRuleGroupReferenceTypeDef definition

class StatelessRuleGroupReferenceTypeDef(TypedDict):
    ResourceArn: str,
    Priority: int,
```

## HeaderTypeDef

```python
# HeaderTypeDef definition

class HeaderTypeDef(TypedDict):
    Protocol: StatefulRuleProtocolType,  # (1)
    Source: str,
    SourcePort: str,
    Direction: StatefulRuleDirectionType,  # (2)
    Destination: str,
    DestinationPort: str,
```

1. See [:material-code-brackets: StatefulRuleProtocolType](./literals.md#statefulruleprotocoltype) 
2. See [:material-code-brackets: StatefulRuleDirectionType](./literals.md#statefulruledirectiontype) 
## IPSetReferenceTypeDef

```python
# IPSetReferenceTypeDef definition

class IPSetReferenceTypeDef(TypedDict):
    ReferenceArn: NotRequired[str],
```

## IPSetTypeDef

```python
# IPSetTypeDef definition

class IPSetTypeDef(TypedDict):
    Definition: Sequence[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListFirewallPoliciesRequestRequestTypeDef

```python
# ListFirewallPoliciesRequestRequestTypeDef definition

class ListFirewallPoliciesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListFirewallsRequestRequestTypeDef

```python
# ListFirewallsRequestRequestTypeDef definition

class ListFirewallsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    VpcIds: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
```

## ListRuleGroupsRequestRequestTypeDef

```python
# ListRuleGroupsRequestRequestTypeDef definition

class ListRuleGroupsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Scope: NotRequired[ResourceManagedStatusType],  # (1)
    ManagedType: NotRequired[ResourceManagedTypeType],  # (2)
    Type: NotRequired[RuleGroupTypeType],  # (3)
```

1. See [:material-code-brackets: ResourceManagedStatusType](./literals.md#resourcemanagedstatustype) 
2. See [:material-code-brackets: ResourceManagedTypeType](./literals.md#resourcemanagedtypetype) 
3. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype) 
## RuleGroupMetadataTypeDef

```python
# RuleGroupMetadataTypeDef definition

class RuleGroupMetadataTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
```

## ListTLSInspectionConfigurationsRequestRequestTypeDef

```python
# ListTLSInspectionConfigurationsRequestRequestTypeDef definition

class ListTLSInspectionConfigurationsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## TLSInspectionConfigurationMetadataTypeDef

```python
# TLSInspectionConfigurationMetadataTypeDef definition

class TLSInspectionConfigurationMetadataTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## LogDestinationConfigTypeDef

```python
# LogDestinationConfigTypeDef definition

class LogDestinationConfigTypeDef(TypedDict):
    LogType: LogTypeType,  # (1)
    LogDestinationType: LogDestinationTypeType,  # (2)
    LogDestination: Dict[str, str],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
2. See [:material-code-brackets: LogDestinationTypeType](./literals.md#logdestinationtypetype) 
## PortRangeTypeDef

```python
# PortRangeTypeDef definition

class PortRangeTypeDef(TypedDict):
    FromPort: int,
    ToPort: int,
```

## TCPFlagFieldTypeDef

```python
# TCPFlagFieldTypeDef definition

class TCPFlagFieldTypeDef(TypedDict):
    Flags: Sequence[TCPFlagType],  # (1)
    Masks: NotRequired[Sequence[TCPFlagType]],  # (1)
```

1. See [:material-code-brackets: TCPFlagType](./literals.md#tcpflagtype) 
2. See [:material-code-brackets: TCPFlagType](./literals.md#tcpflagtype) 
## PerObjectStatusTypeDef

```python
# PerObjectStatusTypeDef definition

class PerObjectStatusTypeDef(TypedDict):
    SyncStatus: NotRequired[PerObjectSyncStatusType],  # (1)
    UpdateToken: NotRequired[str],
```

1. See [:material-code-brackets: PerObjectSyncStatusType](./literals.md#perobjectsyncstatustype) 
## PortSetTypeDef

```python
# PortSetTypeDef definition

class PortSetTypeDef(TypedDict):
    Definition: NotRequired[Sequence[str]],
```

## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
```

## RuleOptionTypeDef

```python
# RuleOptionTypeDef definition

class RuleOptionTypeDef(TypedDict):
    Keyword: str,
    Settings: NotRequired[Sequence[str]],
```

## RulesSourceListTypeDef

```python
# RulesSourceListTypeDef definition

class RulesSourceListTypeDef(TypedDict):
    Targets: Sequence[str],
    TargetTypes: Sequence[TargetTypeType],  # (1)
    GeneratedRulesType: GeneratedRulesTypeType,  # (2)
```

1. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
2. See [:material-code-brackets: GeneratedRulesTypeType](./literals.md#generatedrulestypetype) 
## ServerCertificateTypeDef

```python
# ServerCertificateTypeDef definition

class ServerCertificateTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
```

## StatefulRuleGroupOverrideTypeDef

```python
# StatefulRuleGroupOverrideTypeDef definition

class StatefulRuleGroupOverrideTypeDef(TypedDict):
    Action: NotRequired[OverrideActionType],  # (1)
```

1. See [:material-code-brackets: OverrideActionType](./literals.md#overrideactiontype) 
## TlsCertificateDataTypeDef

```python
# TlsCertificateDataTypeDef definition

class TlsCertificateDataTypeDef(TypedDict):
    CertificateArn: NotRequired[str],
    CertificateSerial: NotRequired[str],
    Status: NotRequired[str],
    StatusMessage: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateFirewallDeleteProtectionRequestRequestTypeDef

```python
# UpdateFirewallDeleteProtectionRequestRequestTypeDef definition

class UpdateFirewallDeleteProtectionRequestRequestTypeDef(TypedDict):
    DeleteProtection: bool,
    UpdateToken: NotRequired[str],
    FirewallArn: NotRequired[str],
    FirewallName: NotRequired[str],
```

## UpdateFirewallDescriptionRequestRequestTypeDef

```python
# UpdateFirewallDescriptionRequestRequestTypeDef definition

class UpdateFirewallDescriptionRequestRequestTypeDef(TypedDict):
    UpdateToken: NotRequired[str],
    FirewallArn: NotRequired[str],
    FirewallName: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef

```python
# UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef definition

class UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef(TypedDict):
    FirewallPolicyChangeProtection: bool,
    UpdateToken: NotRequired[str],
    FirewallArn: NotRequired[str],
    FirewallName: NotRequired[str],
```

## UpdateSubnetChangeProtectionRequestRequestTypeDef

```python
# UpdateSubnetChangeProtectionRequestRequestTypeDef definition

class UpdateSubnetChangeProtectionRequestRequestTypeDef(TypedDict):
    SubnetChangeProtection: bool,
    UpdateToken: NotRequired[str],
    FirewallArn: NotRequired[str],
    FirewallName: NotRequired[str],
```

## AssociateFirewallPolicyResponseTypeDef

```python
# AssociateFirewallPolicyResponseTypeDef definition

class AssociateFirewallPolicyResponseTypeDef(TypedDict):
    FirewallArn: str,
    FirewallName: str,
    FirewallPolicyArn: str,
    UpdateToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeResourcePolicyResponseTypeDef

```python
# DescribeResourcePolicyResponseTypeDef definition

class DescribeResourcePolicyResponseTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFirewallDeleteProtectionResponseTypeDef

```python
# UpdateFirewallDeleteProtectionResponseTypeDef definition

class UpdateFirewallDeleteProtectionResponseTypeDef(TypedDict):
    FirewallArn: str,
    FirewallName: str,
    DeleteProtection: bool,
    UpdateToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFirewallDescriptionResponseTypeDef

```python
# UpdateFirewallDescriptionResponseTypeDef definition

class UpdateFirewallDescriptionResponseTypeDef(TypedDict):
    FirewallArn: str,
    FirewallName: str,
    Description: str,
    UpdateToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFirewallPolicyChangeProtectionResponseTypeDef

```python
# UpdateFirewallPolicyChangeProtectionResponseTypeDef definition

class UpdateFirewallPolicyChangeProtectionResponseTypeDef(TypedDict):
    UpdateToken: str,
    FirewallArn: str,
    FirewallName: str,
    FirewallPolicyChangeProtection: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSubnetChangeProtectionResponseTypeDef

```python
# UpdateSubnetChangeProtectionResponseTypeDef definition

class UpdateSubnetChangeProtectionResponseTypeDef(TypedDict):
    UpdateToken: str,
    FirewallArn: str,
    FirewallName: str,
    SubnetChangeProtection: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateSubnetsRequestRequestTypeDef

```python
# AssociateSubnetsRequestRequestTypeDef definition

class AssociateSubnetsRequestRequestTypeDef(TypedDict):
    SubnetMappings: Sequence[SubnetMappingTypeDef],  # (1)
    UpdateToken: NotRequired[str],
    FirewallArn: NotRequired[str],
    FirewallName: NotRequired[str],
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
## AssociateSubnetsResponseTypeDef

```python
# AssociateSubnetsResponseTypeDef definition

class AssociateSubnetsResponseTypeDef(TypedDict):
    FirewallArn: str,
    FirewallName: str,
    SubnetMappings: List[SubnetMappingTypeDef],  # (1)
    UpdateToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateSubnetsResponseTypeDef

```python
# DisassociateSubnetsResponseTypeDef definition

class DisassociateSubnetsResponseTypeDef(TypedDict):
    FirewallArn: str,
    FirewallName: str,
    SubnetMappings: List[SubnetMappingTypeDef],  # (1)
    UpdateToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CIDRSummaryTypeDef

```python
# CIDRSummaryTypeDef definition

class CIDRSummaryTypeDef(TypedDict):
    AvailableCIDRCount: NotRequired[int],
    UtilizedCIDRCount: NotRequired[int],
    IPSetReferences: NotRequired[Dict[str, IPSetMetadataTypeDef]],  # (1)
```

1. See [:material-code-braces: IPSetMetadataTypeDef](./type_defs.md#ipsetmetadatatypedef) 
## UpdateFirewallEncryptionConfigurationRequestRequestTypeDef

```python
# UpdateFirewallEncryptionConfigurationRequestRequestTypeDef definition

class UpdateFirewallEncryptionConfigurationRequestRequestTypeDef(TypedDict):
    UpdateToken: NotRequired[str],
    FirewallArn: NotRequired[str],
    FirewallName: NotRequired[str],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## UpdateFirewallEncryptionConfigurationResponseTypeDef

```python
# UpdateFirewallEncryptionConfigurationResponseTypeDef definition

class UpdateFirewallEncryptionConfigurationResponseTypeDef(TypedDict):
    FirewallArn: str,
    FirewallName: str,
    UpdateToken: str,
    EncryptionConfiguration: EncryptionConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFirewallRequestRequestTypeDef

```python
# CreateFirewallRequestRequestTypeDef definition

class CreateFirewallRequestRequestTypeDef(TypedDict):
    FirewallName: str,
    FirewallPolicyArn: str,
    VpcId: str,
    SubnetMappings: Sequence[SubnetMappingTypeDef],  # (1)
    DeleteProtection: NotRequired[bool],
    SubnetChangeProtection: NotRequired[bool],
    FirewallPolicyChangeProtection: NotRequired[bool],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## FirewallPolicyResponseTypeDef

```python
# FirewallPolicyResponseTypeDef definition

class FirewallPolicyResponseTypeDef(TypedDict):
    FirewallPolicyName: str,
    FirewallPolicyArn: str,
    FirewallPolicyId: str,
    Description: NotRequired[str],
    FirewallPolicyStatus: NotRequired[ResourceStatusType],  # (1)
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    ConsumedStatelessRuleCapacity: NotRequired[int],
    ConsumedStatefulRuleCapacity: NotRequired[int],
    NumberOfAssociations: NotRequired[int],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## FirewallTypeDef

```python
# FirewallTypeDef definition

class FirewallTypeDef(TypedDict):
    FirewallPolicyArn: str,
    VpcId: str,
    SubnetMappings: List[SubnetMappingTypeDef],  # (1)
    FirewallId: str,
    FirewallName: NotRequired[str],
    FirewallArn: NotRequired[str],
    DeleteProtection: NotRequired[bool],
    SubnetChangeProtection: NotRequired[bool],
    FirewallPolicyChangeProtection: NotRequired[bool],
    Description: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    NextToken: str,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RuleGroupResponseTypeDef

```python
# RuleGroupResponseTypeDef definition

class RuleGroupResponseTypeDef(TypedDict):
    RuleGroupArn: str,
    RuleGroupName: str,
    RuleGroupId: str,
    Description: NotRequired[str],
    Type: NotRequired[RuleGroupTypeType],  # (1)
    Capacity: NotRequired[int],
    RuleGroupStatus: NotRequired[ResourceStatusType],  # (2)
    Tags: NotRequired[List[TagTypeDef]],  # (3)
    ConsumedCapacity: NotRequired[int],
    NumberOfAssociations: NotRequired[int],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (4)
    SourceMetadata: NotRequired[SourceMetadataTypeDef],  # (5)
    SnsTopic: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
5. See [:material-code-braces: SourceMetadataTypeDef](./type_defs.md#sourcemetadatatypedef) 
## DescribeRuleGroupMetadataResponseTypeDef

```python
# DescribeRuleGroupMetadataResponseTypeDef definition

class DescribeRuleGroupMetadataResponseTypeDef(TypedDict):
    RuleGroupArn: str,
    RuleGroupName: str,
    Description: str,
    Type: RuleGroupTypeType,  # (1)
    Capacity: int,
    StatefulRuleOptions: StatefulRuleOptionsTypeDef,  # (2)
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype) 
2. See [:material-code-braces: StatefulRuleOptionsTypeDef](./type_defs.md#statefulruleoptionstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishMetricActionTypeDef

```python
# PublishMetricActionTypeDef definition

class PublishMetricActionTypeDef(TypedDict):
    Dimensions: Sequence[DimensionTypeDef],  # (1)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## ListFirewallsResponseTypeDef

```python
# ListFirewallsResponseTypeDef definition

class ListFirewallsResponseTypeDef(TypedDict):
    NextToken: str,
    Firewalls: List[FirewallMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallMetadataTypeDef](./type_defs.md#firewallmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFirewallPoliciesResponseTypeDef

```python
# ListFirewallPoliciesResponseTypeDef definition

class ListFirewallPoliciesResponseTypeDef(TypedDict):
    NextToken: str,
    FirewallPolicies: List[FirewallPolicyMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallPolicyMetadataTypeDef](./type_defs.md#firewallpolicymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReferenceSetsTypeDef

```python
# ReferenceSetsTypeDef definition

class ReferenceSetsTypeDef(TypedDict):
    IPSetReferences: NotRequired[Mapping[str, IPSetReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: IPSetReferenceTypeDef](./type_defs.md#ipsetreferencetypedef) 
## PolicyVariablesTypeDef

```python
# PolicyVariablesTypeDef definition

class PolicyVariablesTypeDef(TypedDict):
    RuleVariables: NotRequired[Mapping[str, IPSetTypeDef]],  # (1)
```

1. See [:material-code-braces: IPSetTypeDef](./type_defs.md#ipsettypedef) 
## ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef

```python
# ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef definition

class ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFirewallsRequestListFirewallsPaginateTypeDef

```python
# ListFirewallsRequestListFirewallsPaginateTypeDef definition

class ListFirewallsRequestListFirewallsPaginateTypeDef(TypedDict):
    VpcIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRuleGroupsRequestListRuleGroupsPaginateTypeDef

```python
# ListRuleGroupsRequestListRuleGroupsPaginateTypeDef definition

class ListRuleGroupsRequestListRuleGroupsPaginateTypeDef(TypedDict):
    Scope: NotRequired[ResourceManagedStatusType],  # (1)
    ManagedType: NotRequired[ResourceManagedTypeType],  # (2)
    Type: NotRequired[RuleGroupTypeType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ResourceManagedStatusType](./literals.md#resourcemanagedstatustype) 
2. See [:material-code-brackets: ResourceManagedTypeType](./literals.md#resourcemanagedtypetype) 
3. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef

```python
# ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef definition

class ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceRequestListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRuleGroupsResponseTypeDef

```python
# ListRuleGroupsResponseTypeDef definition

class ListRuleGroupsResponseTypeDef(TypedDict):
    NextToken: str,
    RuleGroups: List[RuleGroupMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupMetadataTypeDef](./type_defs.md#rulegroupmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTLSInspectionConfigurationsResponseTypeDef

```python
# ListTLSInspectionConfigurationsResponseTypeDef definition

class ListTLSInspectionConfigurationsResponseTypeDef(TypedDict):
    NextToken: str,
    TLSInspectionConfigurations: List[TLSInspectionConfigurationMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TLSInspectionConfigurationMetadataTypeDef](./type_defs.md#tlsinspectionconfigurationmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingConfigurationTypeDef

```python
# LoggingConfigurationTypeDef definition

class LoggingConfigurationTypeDef(TypedDict):
    LogDestinationConfigs: List[LogDestinationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: LogDestinationConfigTypeDef](./type_defs.md#logdestinationconfigtypedef) 
## ServerCertificateScopeTypeDef

```python
# ServerCertificateScopeTypeDef definition

class ServerCertificateScopeTypeDef(TypedDict):
    Sources: NotRequired[Sequence[AddressTypeDef]],  # (1)
    Destinations: NotRequired[Sequence[AddressTypeDef]],  # (1)
    SourcePorts: NotRequired[Sequence[PortRangeTypeDef]],  # (3)
    DestinationPorts: NotRequired[Sequence[PortRangeTypeDef]],  # (3)
    Protocols: NotRequired[Sequence[int]],
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
4. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
## MatchAttributesTypeDef

```python
# MatchAttributesTypeDef definition

class MatchAttributesTypeDef(TypedDict):
    Sources: NotRequired[Sequence[AddressTypeDef]],  # (1)
    Destinations: NotRequired[Sequence[AddressTypeDef]],  # (1)
    SourcePorts: NotRequired[Sequence[PortRangeTypeDef]],  # (3)
    DestinationPorts: NotRequired[Sequence[PortRangeTypeDef]],  # (3)
    Protocols: NotRequired[Sequence[int]],
    TCPFlags: NotRequired[Sequence[TCPFlagFieldTypeDef]],  # (5)
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
4. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
5. See [:material-code-braces: TCPFlagFieldTypeDef](./type_defs.md#tcpflagfieldtypedef) 
## SyncStateTypeDef

```python
# SyncStateTypeDef definition

class SyncStateTypeDef(TypedDict):
    Attachment: NotRequired[AttachmentTypeDef],  # (1)
    Config: NotRequired[Dict[str, PerObjectStatusTypeDef]],  # (2)
```

1. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) 
2. See [:material-code-braces: PerObjectStatusTypeDef](./type_defs.md#perobjectstatustypedef) 
## RuleVariablesTypeDef

```python
# RuleVariablesTypeDef definition

class RuleVariablesTypeDef(TypedDict):
    IPSets: NotRequired[Mapping[str, IPSetTypeDef]],  # (1)
    PortSets: NotRequired[Mapping[str, PortSetTypeDef]],  # (2)
```

1. See [:material-code-braces: IPSetTypeDef](./type_defs.md#ipsettypedef) 
2. See [:material-code-braces: PortSetTypeDef](./type_defs.md#portsettypedef) 
## StatefulRuleTypeDef

```python
# StatefulRuleTypeDef definition

class StatefulRuleTypeDef(TypedDict):
    Action: StatefulActionType,  # (1)
    Header: HeaderTypeDef,  # (2)
    RuleOptions: Sequence[RuleOptionTypeDef],  # (3)
```

1. See [:material-code-brackets: StatefulActionType](./literals.md#statefulactiontype) 
2. See [:material-code-braces: HeaderTypeDef](./type_defs.md#headertypedef) 
3. See [:material-code-braces: RuleOptionTypeDef](./type_defs.md#ruleoptiontypedef) 
## StatefulRuleGroupReferenceTypeDef

```python
# StatefulRuleGroupReferenceTypeDef definition

class StatefulRuleGroupReferenceTypeDef(TypedDict):
    ResourceArn: str,
    Priority: NotRequired[int],
    Override: NotRequired[StatefulRuleGroupOverrideTypeDef],  # (1)
```

1. See [:material-code-braces: StatefulRuleGroupOverrideTypeDef](./type_defs.md#statefulrulegroupoverridetypedef) 
## TLSInspectionConfigurationResponseTypeDef

```python
# TLSInspectionConfigurationResponseTypeDef definition

class TLSInspectionConfigurationResponseTypeDef(TypedDict):
    TLSInspectionConfigurationArn: str,
    TLSInspectionConfigurationName: str,
    TLSInspectionConfigurationId: str,
    TLSInspectionConfigurationStatus: NotRequired[ResourceStatusType],  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    LastModifiedTime: NotRequired[datetime],
    NumberOfAssociations: NotRequired[int],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
    Certificates: NotRequired[List[TlsCertificateDataTypeDef]],  # (4)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: TlsCertificateDataTypeDef](./type_defs.md#tlscertificatedatatypedef) 
## CapacityUsageSummaryTypeDef

```python
# CapacityUsageSummaryTypeDef definition

class CapacityUsageSummaryTypeDef(TypedDict):
    CIDRs: NotRequired[CIDRSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: CIDRSummaryTypeDef](./type_defs.md#cidrsummarytypedef) 
## CreateFirewallPolicyResponseTypeDef

```python
# CreateFirewallPolicyResponseTypeDef definition

class CreateFirewallPolicyResponseTypeDef(TypedDict):
    UpdateToken: str,
    FirewallPolicyResponse: FirewallPolicyResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallPolicyResponseTypeDef](./type_defs.md#firewallpolicyresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFirewallPolicyResponseTypeDef

```python
# DeleteFirewallPolicyResponseTypeDef definition

class DeleteFirewallPolicyResponseTypeDef(TypedDict):
    FirewallPolicyResponse: FirewallPolicyResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallPolicyResponseTypeDef](./type_defs.md#firewallpolicyresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFirewallPolicyResponseTypeDef

```python
# UpdateFirewallPolicyResponseTypeDef definition

class UpdateFirewallPolicyResponseTypeDef(TypedDict):
    UpdateToken: str,
    FirewallPolicyResponse: FirewallPolicyResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FirewallPolicyResponseTypeDef](./type_defs.md#firewallpolicyresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleGroupResponseTypeDef

```python
# CreateRuleGroupResponseTypeDef definition

class CreateRuleGroupResponseTypeDef(TypedDict):
    UpdateToken: str,
    RuleGroupResponse: RuleGroupResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupResponseTypeDef](./type_defs.md#rulegroupresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRuleGroupResponseTypeDef

```python
# DeleteRuleGroupResponseTypeDef definition

class DeleteRuleGroupResponseTypeDef(TypedDict):
    RuleGroupResponse: RuleGroupResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupResponseTypeDef](./type_defs.md#rulegroupresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRuleGroupResponseTypeDef

```python
# UpdateRuleGroupResponseTypeDef definition

class UpdateRuleGroupResponseTypeDef(TypedDict):
    UpdateToken: str,
    RuleGroupResponse: RuleGroupResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleGroupResponseTypeDef](./type_defs.md#rulegroupresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActionDefinitionTypeDef

```python
# ActionDefinitionTypeDef definition

class ActionDefinitionTypeDef(TypedDict):
    PublishMetricAction: NotRequired[PublishMetricActionTypeDef],  # (1)
```

1. See [:material-code-braces: PublishMetricActionTypeDef](./type_defs.md#publishmetricactiontypedef) 
## DescribeLoggingConfigurationResponseTypeDef

```python
# DescribeLoggingConfigurationResponseTypeDef definition

class DescribeLoggingConfigurationResponseTypeDef(TypedDict):
    FirewallArn: str,
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLoggingConfigurationRequestRequestTypeDef

```python
# UpdateLoggingConfigurationRequestRequestTypeDef definition

class UpdateLoggingConfigurationRequestRequestTypeDef(TypedDict):
    FirewallArn: NotRequired[str],
    FirewallName: NotRequired[str],
    LoggingConfiguration: NotRequired[LoggingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
## UpdateLoggingConfigurationResponseTypeDef

```python
# UpdateLoggingConfigurationResponseTypeDef definition

class UpdateLoggingConfigurationResponseTypeDef(TypedDict):
    FirewallArn: str,
    FirewallName: str,
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServerCertificateConfigurationTypeDef

```python
# ServerCertificateConfigurationTypeDef definition

class ServerCertificateConfigurationTypeDef(TypedDict):
    ServerCertificates: NotRequired[Sequence[ServerCertificateTypeDef]],  # (1)
    Scopes: NotRequired[Sequence[ServerCertificateScopeTypeDef]],  # (2)
```

1. See [:material-code-braces: ServerCertificateTypeDef](./type_defs.md#servercertificatetypedef) 
2. See [:material-code-braces: ServerCertificateScopeTypeDef](./type_defs.md#servercertificatescopetypedef) 
## RuleDefinitionTypeDef

```python
# RuleDefinitionTypeDef definition

class RuleDefinitionTypeDef(TypedDict):
    MatchAttributes: MatchAttributesTypeDef,  # (1)
    Actions: Sequence[str],
```

1. See [:material-code-braces: MatchAttributesTypeDef](./type_defs.md#matchattributestypedef) 
## CreateTLSInspectionConfigurationResponseTypeDef

```python
# CreateTLSInspectionConfigurationResponseTypeDef definition

class CreateTLSInspectionConfigurationResponseTypeDef(TypedDict):
    UpdateToken: str,
    TLSInspectionConfigurationResponse: TLSInspectionConfigurationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TLSInspectionConfigurationResponseTypeDef](./type_defs.md#tlsinspectionconfigurationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTLSInspectionConfigurationResponseTypeDef

```python
# DeleteTLSInspectionConfigurationResponseTypeDef definition

class DeleteTLSInspectionConfigurationResponseTypeDef(TypedDict):
    TLSInspectionConfigurationResponse: TLSInspectionConfigurationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TLSInspectionConfigurationResponseTypeDef](./type_defs.md#tlsinspectionconfigurationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTLSInspectionConfigurationResponseTypeDef

```python
# UpdateTLSInspectionConfigurationResponseTypeDef definition

class UpdateTLSInspectionConfigurationResponseTypeDef(TypedDict):
    UpdateToken: str,
    TLSInspectionConfigurationResponse: TLSInspectionConfigurationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TLSInspectionConfigurationResponseTypeDef](./type_defs.md#tlsinspectionconfigurationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FirewallStatusTypeDef

```python
# FirewallStatusTypeDef definition

class FirewallStatusTypeDef(TypedDict):
    Status: FirewallStatusValueType,  # (1)
    ConfigurationSyncStateSummary: ConfigurationSyncStateType,  # (2)
    SyncStates: NotRequired[Dict[str, SyncStateTypeDef]],  # (3)
    CapacityUsageSummary: NotRequired[CapacityUsageSummaryTypeDef],  # (4)
```

1. See [:material-code-brackets: FirewallStatusValueType](./literals.md#firewallstatusvaluetype) 
2. See [:material-code-brackets: ConfigurationSyncStateType](./literals.md#configurationsyncstatetype) 
3. See [:material-code-braces: SyncStateTypeDef](./type_defs.md#syncstatetypedef) 
4. See [:material-code-braces: CapacityUsageSummaryTypeDef](./type_defs.md#capacityusagesummarytypedef) 
## CustomActionTypeDef

```python
# CustomActionTypeDef definition

class CustomActionTypeDef(TypedDict):
    ActionName: str,
    ActionDefinition: ActionDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: ActionDefinitionTypeDef](./type_defs.md#actiondefinitiontypedef) 
## TLSInspectionConfigurationTypeDef

```python
# TLSInspectionConfigurationTypeDef definition

class TLSInspectionConfigurationTypeDef(TypedDict):
    ServerCertificateConfigurations: NotRequired[Sequence[ServerCertificateConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerCertificateConfigurationTypeDef](./type_defs.md#servercertificateconfigurationtypedef) 
## StatelessRuleTypeDef

```python
# StatelessRuleTypeDef definition

class StatelessRuleTypeDef(TypedDict):
    RuleDefinition: RuleDefinitionTypeDef,  # (1)
    Priority: int,
```

1. See [:material-code-braces: RuleDefinitionTypeDef](./type_defs.md#ruledefinitiontypedef) 
## CreateFirewallResponseTypeDef

```python
# CreateFirewallResponseTypeDef definition

class CreateFirewallResponseTypeDef(TypedDict):
    Firewall: FirewallTypeDef,  # (1)
    FirewallStatus: FirewallStatusTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FirewallTypeDef](./type_defs.md#firewalltypedef) 
2. See [:material-code-braces: FirewallStatusTypeDef](./type_defs.md#firewallstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFirewallResponseTypeDef

```python
# DeleteFirewallResponseTypeDef definition

class DeleteFirewallResponseTypeDef(TypedDict):
    Firewall: FirewallTypeDef,  # (1)
    FirewallStatus: FirewallStatusTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FirewallTypeDef](./type_defs.md#firewalltypedef) 
2. See [:material-code-braces: FirewallStatusTypeDef](./type_defs.md#firewallstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFirewallResponseTypeDef

```python
# DescribeFirewallResponseTypeDef definition

class DescribeFirewallResponseTypeDef(TypedDict):
    UpdateToken: str,
    Firewall: FirewallTypeDef,  # (1)
    FirewallStatus: FirewallStatusTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FirewallTypeDef](./type_defs.md#firewalltypedef) 
2. See [:material-code-braces: FirewallStatusTypeDef](./type_defs.md#firewallstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FirewallPolicyTypeDef

```python
# FirewallPolicyTypeDef definition

class FirewallPolicyTypeDef(TypedDict):
    StatelessDefaultActions: Sequence[str],
    StatelessFragmentDefaultActions: Sequence[str],
    StatelessRuleGroupReferences: NotRequired[Sequence[StatelessRuleGroupReferenceTypeDef]],  # (1)
    StatelessCustomActions: NotRequired[Sequence[CustomActionTypeDef]],  # (2)
    StatefulRuleGroupReferences: NotRequired[Sequence[StatefulRuleGroupReferenceTypeDef]],  # (3)
    StatefulDefaultActions: NotRequired[Sequence[str]],
    StatefulEngineOptions: NotRequired[StatefulEngineOptionsTypeDef],  # (4)
    TLSInspectionConfigurationArn: NotRequired[str],
    PolicyVariables: NotRequired[PolicyVariablesTypeDef],  # (5)
```

1. See [:material-code-braces: StatelessRuleGroupReferenceTypeDef](./type_defs.md#statelessrulegroupreferencetypedef) 
2. See [:material-code-braces: CustomActionTypeDef](./type_defs.md#customactiontypedef) 
3. See [:material-code-braces: StatefulRuleGroupReferenceTypeDef](./type_defs.md#statefulrulegroupreferencetypedef) 
4. See [:material-code-braces: StatefulEngineOptionsTypeDef](./type_defs.md#statefulengineoptionstypedef) 
5. See [:material-code-braces: PolicyVariablesTypeDef](./type_defs.md#policyvariablestypedef) 
## CreateTLSInspectionConfigurationRequestRequestTypeDef

```python
# CreateTLSInspectionConfigurationRequestRequestTypeDef definition

class CreateTLSInspectionConfigurationRequestRequestTypeDef(TypedDict):
    TLSInspectionConfigurationName: str,
    TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: TLSInspectionConfigurationTypeDef](./type_defs.md#tlsinspectionconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## DescribeTLSInspectionConfigurationResponseTypeDef

```python
# DescribeTLSInspectionConfigurationResponseTypeDef definition

class DescribeTLSInspectionConfigurationResponseTypeDef(TypedDict):
    UpdateToken: str,
    TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,  # (1)
    TLSInspectionConfigurationResponse: TLSInspectionConfigurationResponseTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TLSInspectionConfigurationTypeDef](./type_defs.md#tlsinspectionconfigurationtypedef) 
2. See [:material-code-braces: TLSInspectionConfigurationResponseTypeDef](./type_defs.md#tlsinspectionconfigurationresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTLSInspectionConfigurationRequestRequestTypeDef

```python
# UpdateTLSInspectionConfigurationRequestRequestTypeDef definition

class UpdateTLSInspectionConfigurationRequestRequestTypeDef(TypedDict):
    TLSInspectionConfiguration: TLSInspectionConfigurationTypeDef,  # (1)
    UpdateToken: str,
    TLSInspectionConfigurationArn: NotRequired[str],
    TLSInspectionConfigurationName: NotRequired[str],
    Description: NotRequired[str],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: TLSInspectionConfigurationTypeDef](./type_defs.md#tlsinspectionconfigurationtypedef) 
2. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## StatelessRulesAndCustomActionsTypeDef

```python
# StatelessRulesAndCustomActionsTypeDef definition

class StatelessRulesAndCustomActionsTypeDef(TypedDict):
    StatelessRules: Sequence[StatelessRuleTypeDef],  # (1)
    CustomActions: NotRequired[Sequence[CustomActionTypeDef]],  # (2)
```

1. See [:material-code-braces: StatelessRuleTypeDef](./type_defs.md#statelessruletypedef) 
2. See [:material-code-braces: CustomActionTypeDef](./type_defs.md#customactiontypedef) 
## CreateFirewallPolicyRequestRequestTypeDef

```python
# CreateFirewallPolicyRequestRequestTypeDef definition

class CreateFirewallPolicyRequestRequestTypeDef(TypedDict):
    FirewallPolicyName: str,
    FirewallPolicy: FirewallPolicyTypeDef,  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    DryRun: NotRequired[bool],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: FirewallPolicyTypeDef](./type_defs.md#firewallpolicytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## DescribeFirewallPolicyResponseTypeDef

```python
# DescribeFirewallPolicyResponseTypeDef definition

class DescribeFirewallPolicyResponseTypeDef(TypedDict):
    UpdateToken: str,
    FirewallPolicyResponse: FirewallPolicyResponseTypeDef,  # (1)
    FirewallPolicy: FirewallPolicyTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FirewallPolicyResponseTypeDef](./type_defs.md#firewallpolicyresponsetypedef) 
2. See [:material-code-braces: FirewallPolicyTypeDef](./type_defs.md#firewallpolicytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFirewallPolicyRequestRequestTypeDef

```python
# UpdateFirewallPolicyRequestRequestTypeDef definition

class UpdateFirewallPolicyRequestRequestTypeDef(TypedDict):
    UpdateToken: str,
    FirewallPolicy: FirewallPolicyTypeDef,  # (1)
    FirewallPolicyArn: NotRequired[str],
    FirewallPolicyName: NotRequired[str],
    Description: NotRequired[str],
    DryRun: NotRequired[bool],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FirewallPolicyTypeDef](./type_defs.md#firewallpolicytypedef) 
2. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## RulesSourceTypeDef

```python
# RulesSourceTypeDef definition

class RulesSourceTypeDef(TypedDict):
    RulesString: NotRequired[str],
    RulesSourceList: NotRequired[RulesSourceListTypeDef],  # (1)
    StatefulRules: NotRequired[Sequence[StatefulRuleTypeDef]],  # (2)
    StatelessRulesAndCustomActions: NotRequired[StatelessRulesAndCustomActionsTypeDef],  # (3)
```

1. See [:material-code-braces: RulesSourceListTypeDef](./type_defs.md#rulessourcelisttypedef) 
2. See [:material-code-braces: StatefulRuleTypeDef](./type_defs.md#statefulruletypedef) 
3. See [:material-code-braces: StatelessRulesAndCustomActionsTypeDef](./type_defs.md#statelessrulesandcustomactionstypedef) 
## RuleGroupTypeDef

```python
# RuleGroupTypeDef definition

class RuleGroupTypeDef(TypedDict):
    RulesSource: RulesSourceTypeDef,  # (3)
    RuleVariables: NotRequired[RuleVariablesTypeDef],  # (1)
    ReferenceSets: NotRequired[ReferenceSetsTypeDef],  # (2)
    StatefulRuleOptions: NotRequired[StatefulRuleOptionsTypeDef],  # (4)
```

1. See [:material-code-braces: RuleVariablesTypeDef](./type_defs.md#rulevariablestypedef) 
2. See [:material-code-braces: ReferenceSetsTypeDef](./type_defs.md#referencesetstypedef) 
3. See [:material-code-braces: RulesSourceTypeDef](./type_defs.md#rulessourcetypedef) 
4. See [:material-code-braces: StatefulRuleOptionsTypeDef](./type_defs.md#statefulruleoptionstypedef) 
## CreateRuleGroupRequestRequestTypeDef

```python
# CreateRuleGroupRequestRequestTypeDef definition

class CreateRuleGroupRequestRequestTypeDef(TypedDict):
    RuleGroupName: str,
    Type: RuleGroupTypeType,  # (1)
    Capacity: int,
    RuleGroup: NotRequired[RuleGroupTypeDef],  # (2)
    Rules: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    DryRun: NotRequired[bool],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (4)
    SourceMetadata: NotRequired[SourceMetadataTypeDef],  # (5)
```

1. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype) 
2. See [:material-code-braces: RuleGroupTypeDef](./type_defs.md#rulegrouptypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
5. See [:material-code-braces: SourceMetadataTypeDef](./type_defs.md#sourcemetadatatypedef) 
## DescribeRuleGroupResponseTypeDef

```python
# DescribeRuleGroupResponseTypeDef definition

class DescribeRuleGroupResponseTypeDef(TypedDict):
    UpdateToken: str,
    RuleGroup: RuleGroupTypeDef,  # (1)
    RuleGroupResponse: RuleGroupResponseTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RuleGroupTypeDef](./type_defs.md#rulegrouptypedef) 
2. See [:material-code-braces: RuleGroupResponseTypeDef](./type_defs.md#rulegroupresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRuleGroupRequestRequestTypeDef

```python
# UpdateRuleGroupRequestRequestTypeDef definition

class UpdateRuleGroupRequestRequestTypeDef(TypedDict):
    UpdateToken: str,
    RuleGroupArn: NotRequired[str],
    RuleGroupName: NotRequired[str],
    RuleGroup: NotRequired[RuleGroupTypeDef],  # (1)
    Rules: NotRequired[str],
    Type: NotRequired[RuleGroupTypeType],  # (2)
    Description: NotRequired[str],
    DryRun: NotRequired[bool],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (3)
    SourceMetadata: NotRequired[SourceMetadataTypeDef],  # (4)
```

1. See [:material-code-braces: RuleGroupTypeDef](./type_defs.md#rulegrouptypedef) 
2. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype) 
3. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
4. See [:material-code-braces: SourceMetadataTypeDef](./type_defs.md#sourcemetadatatypedef) 
