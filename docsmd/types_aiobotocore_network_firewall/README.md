# NetworkFirewall module

> [Index](../README.md) > NetworkFirewall


!!! note ""

    Auto-generated documentation for [NetworkFirewall](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#networkfirewall)
    type annotations stubs module [types-aiobotocore-network-firewall](https://pypi.org/project/types-aiobotocore-network-firewall/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `NetworkFirewall` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `NetworkFirewall` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[network-firewall]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[network-firewall]'

# standalone installation
python -m pip install types-aiobotocore-network-firewall
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-network-firewall
```

## Usage

Code samples can be found in [Examples](./usage.md).

## NetworkFirewallClient

Type annotations and code completion for  `#!python session.create_client("network-firewall")` as [NetworkFirewallClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Client)

```python
# NetworkFirewallClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.client import NetworkFirewallClient


session = get_session()
async with session.create_client("network-firewall") as client:
    client: NetworkFirewallClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("network-firewall").get_paginator("...")`.

```python
# ListFirewallPoliciesPaginator usage example

from types_aiobotocore_network_firewall.paginator import ListFirewallPoliciesPaginator

def get_list_firewall_policies_paginator() -> ListFirewallPoliciesPaginator:
    return client.get_paginator("list_firewall_policies"))
```

- [ListFirewallPoliciesPaginator](./paginators.md#listfirewallpoliciespaginator)
- [ListFirewallsPaginator](./paginators.md#listfirewallspaginator)
- [ListRuleGroupsPaginator](./paginators.md#listrulegroupspaginator)
- [ListTLSInspectionConfigurationsPaginator](./paginators.md#listtlsinspectionconfigurationspaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AttachmentStatusType usage example

from types_aiobotocore_network_firewall.literals import AttachmentStatusType

def get_value() -> AttachmentStatusType:
    return "CREATING"
```

- [AttachmentStatusType](./literals.md#attachmentstatustype)
- [ConfigurationSyncStateType](./literals.md#configurationsyncstatetype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [FirewallStatusValueType](./literals.md#firewallstatusvaluetype)
- [GeneratedRulesTypeType](./literals.md#generatedrulestypetype)
- [IPAddressTypeType](./literals.md#ipaddresstypetype)
- [IdentifiedTypeType](./literals.md#identifiedtypetype)
- [ListFirewallPoliciesPaginatorName](./literals.md#listfirewallpoliciespaginatorname)
- [ListFirewallsPaginatorName](./literals.md#listfirewallspaginatorname)
- [ListRuleGroupsPaginatorName](./literals.md#listrulegroupspaginatorname)
- [ListTLSInspectionConfigurationsPaginatorName](./literals.md#listtlsinspectionconfigurationspaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [LogDestinationTypeType](./literals.md#logdestinationtypetype)
- [LogTypeType](./literals.md#logtypetype)
- [OverrideActionType](./literals.md#overrideactiontype)
- [PerObjectSyncStatusType](./literals.md#perobjectsyncstatustype)
- [ResourceManagedStatusType](./literals.md#resourcemanagedstatustype)
- [ResourceManagedTypeType](./literals.md#resourcemanagedtypetype)
- [ResourceStatusType](./literals.md#resourcestatustype)
- [RevocationCheckActionType](./literals.md#revocationcheckactiontype)
- [RuleGroupTypeType](./literals.md#rulegrouptypetype)
- [RuleOrderType](./literals.md#ruleordertype)
- [StatefulActionType](./literals.md#statefulactiontype)
- [StatefulRuleDirectionType](./literals.md#statefulruledirectiontype)
- [StatefulRuleProtocolType](./literals.md#statefulruleprotocoltype)
- [StreamExceptionPolicyType](./literals.md#streamexceptionpolicytype)
- [TCPFlagType](./literals.md#tcpflagtype)
- [TargetTypeType](./literals.md#targettypetype)
- [NetworkFirewallServiceName](./literals.md#networkfirewallservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddressTypeDef](./type_defs.md#addresstypedef)
- [AnalysisResultTypeDef](./type_defs.md#analysisresulttypedef)
- [AssociateFirewallPolicyRequestRequestTypeDef](./type_defs.md#associatefirewallpolicyrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SubnetMappingTypeDef](./type_defs.md#subnetmappingtypedef)
- [AttachmentTypeDef](./type_defs.md#attachmenttypedef)
- [IPSetMetadataTypeDef](./type_defs.md#ipsetmetadatatypedef)
- [CheckCertificateRevocationStatusActionsTypeDef](./type_defs.md#checkcertificaterevocationstatusactionstypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [SourceMetadataTypeDef](./type_defs.md#sourcemetadatatypedef)
- [DeleteFirewallPolicyRequestRequestTypeDef](./type_defs.md#deletefirewallpolicyrequestrequesttypedef)
- [DeleteFirewallRequestRequestTypeDef](./type_defs.md#deletefirewallrequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteRuleGroupRequestRequestTypeDef](./type_defs.md#deleterulegrouprequestrequesttypedef)
- [DeleteTLSInspectionConfigurationRequestRequestTypeDef](./type_defs.md#deletetlsinspectionconfigurationrequestrequesttypedef)
- [DescribeFirewallPolicyRequestRequestTypeDef](./type_defs.md#describefirewallpolicyrequestrequesttypedef)
- [DescribeFirewallRequestRequestTypeDef](./type_defs.md#describefirewallrequestrequesttypedef)
- [DescribeLoggingConfigurationRequestRequestTypeDef](./type_defs.md#describeloggingconfigurationrequestrequesttypedef)
- [DescribeResourcePolicyRequestRequestTypeDef](./type_defs.md#describeresourcepolicyrequestrequesttypedef)
- [DescribeRuleGroupMetadataRequestRequestTypeDef](./type_defs.md#describerulegroupmetadatarequestrequesttypedef)
- [StatefulRuleOptionsTypeDef](./type_defs.md#statefulruleoptionstypedef)
- [DescribeRuleGroupRequestRequestTypeDef](./type_defs.md#describerulegrouprequestrequesttypedef)
- [DescribeTLSInspectionConfigurationRequestRequestTypeDef](./type_defs.md#describetlsinspectionconfigurationrequestrequesttypedef)
- [DimensionTypeDef](./type_defs.md#dimensiontypedef)
- [DisassociateSubnetsRequestRequestTypeDef](./type_defs.md#disassociatesubnetsrequestrequesttypedef)
- [FirewallMetadataTypeDef](./type_defs.md#firewallmetadatatypedef)
- [FirewallPolicyMetadataTypeDef](./type_defs.md#firewallpolicymetadatatypedef)
- [StatelessRuleGroupReferenceTypeDef](./type_defs.md#statelessrulegroupreferencetypedef)
- [FlowTimeoutsTypeDef](./type_defs.md#flowtimeoutstypedef)
- [HeaderTypeDef](./type_defs.md#headertypedef)
- [IPSetOutputTypeDef](./type_defs.md#ipsetoutputtypedef)
- [IPSetReferenceTypeDef](./type_defs.md#ipsetreferencetypedef)
- [IPSetTypeDef](./type_defs.md#ipsettypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListFirewallPoliciesRequestRequestTypeDef](./type_defs.md#listfirewallpoliciesrequestrequesttypedef)
- [ListFirewallsRequestRequestTypeDef](./type_defs.md#listfirewallsrequestrequesttypedef)
- [ListRuleGroupsRequestRequestTypeDef](./type_defs.md#listrulegroupsrequestrequesttypedef)
- [RuleGroupMetadataTypeDef](./type_defs.md#rulegroupmetadatatypedef)
- [ListTLSInspectionConfigurationsRequestRequestTypeDef](./type_defs.md#listtlsinspectionconfigurationsrequestrequesttypedef)
- [TLSInspectionConfigurationMetadataTypeDef](./type_defs.md#tlsinspectionconfigurationmetadatatypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [LogDestinationConfigOutputTypeDef](./type_defs.md#logdestinationconfigoutputtypedef)
- [LogDestinationConfigTypeDef](./type_defs.md#logdestinationconfigtypedef)
- [PortRangeTypeDef](./type_defs.md#portrangetypedef)
- [TCPFlagFieldOutputTypeDef](./type_defs.md#tcpflagfieldoutputtypedef)
- [PerObjectStatusTypeDef](./type_defs.md#perobjectstatustypedef)
- [PortSetOutputTypeDef](./type_defs.md#portsetoutputtypedef)
- [PortSetTypeDef](./type_defs.md#portsettypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [RuleOptionOutputTypeDef](./type_defs.md#ruleoptionoutputtypedef)
- [RuleOptionTypeDef](./type_defs.md#ruleoptiontypedef)
- [RulesSourceListOutputTypeDef](./type_defs.md#rulessourcelistoutputtypedef)
- [RulesSourceListTypeDef](./type_defs.md#rulessourcelisttypedef)
- [ServerCertificateTypeDef](./type_defs.md#servercertificatetypedef)
- [StatefulRuleGroupOverrideTypeDef](./type_defs.md#statefulrulegroupoverridetypedef)
- [TCPFlagFieldTypeDef](./type_defs.md#tcpflagfieldtypedef)
- [TlsCertificateDataTypeDef](./type_defs.md#tlscertificatedatatypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateFirewallDeleteProtectionRequestRequestTypeDef](./type_defs.md#updatefirewalldeleteprotectionrequestrequesttypedef)
- [UpdateFirewallDescriptionRequestRequestTypeDef](./type_defs.md#updatefirewalldescriptionrequestrequesttypedef)
- [UpdateFirewallPolicyChangeProtectionRequestRequestTypeDef](./type_defs.md#updatefirewallpolicychangeprotectionrequestrequesttypedef)
- [UpdateSubnetChangeProtectionRequestRequestTypeDef](./type_defs.md#updatesubnetchangeprotectionrequestrequesttypedef)
- [AssociateFirewallPolicyResponseTypeDef](./type_defs.md#associatefirewallpolicyresponsetypedef)
- [DescribeResourcePolicyResponseTypeDef](./type_defs.md#describeresourcepolicyresponsetypedef)
- [UpdateFirewallDeleteProtectionResponseTypeDef](./type_defs.md#updatefirewalldeleteprotectionresponsetypedef)
- [UpdateFirewallDescriptionResponseTypeDef](./type_defs.md#updatefirewalldescriptionresponsetypedef)
- [UpdateFirewallPolicyChangeProtectionResponseTypeDef](./type_defs.md#updatefirewallpolicychangeprotectionresponsetypedef)
- [UpdateSubnetChangeProtectionResponseTypeDef](./type_defs.md#updatesubnetchangeprotectionresponsetypedef)
- [AssociateSubnetsRequestRequestTypeDef](./type_defs.md#associatesubnetsrequestrequesttypedef)
- [AssociateSubnetsResponseTypeDef](./type_defs.md#associatesubnetsresponsetypedef)
- [DisassociateSubnetsResponseTypeDef](./type_defs.md#disassociatesubnetsresponsetypedef)
- [CIDRSummaryTypeDef](./type_defs.md#cidrsummarytypedef)
- [UpdateFirewallEncryptionConfigurationRequestRequestTypeDef](./type_defs.md#updatefirewallencryptionconfigurationrequestrequesttypedef)
- [UpdateFirewallEncryptionConfigurationResponseTypeDef](./type_defs.md#updatefirewallencryptionconfigurationresponsetypedef)
- [CreateFirewallRequestRequestTypeDef](./type_defs.md#createfirewallrequestrequesttypedef)
- [FirewallPolicyResponseTypeDef](./type_defs.md#firewallpolicyresponsetypedef)
- [FirewallTypeDef](./type_defs.md#firewalltypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [RuleGroupResponseTypeDef](./type_defs.md#rulegroupresponsetypedef)
- [DescribeRuleGroupMetadataResponseTypeDef](./type_defs.md#describerulegroupmetadataresponsetypedef)
- [PublishMetricActionOutputTypeDef](./type_defs.md#publishmetricactionoutputtypedef)
- [PublishMetricActionTypeDef](./type_defs.md#publishmetricactiontypedef)
- [ListFirewallsResponseTypeDef](./type_defs.md#listfirewallsresponsetypedef)
- [ListFirewallPoliciesResponseTypeDef](./type_defs.md#listfirewallpoliciesresponsetypedef)
- [StatefulEngineOptionsTypeDef](./type_defs.md#statefulengineoptionstypedef)
- [PolicyVariablesOutputTypeDef](./type_defs.md#policyvariablesoutputtypedef)
- [ReferenceSetsOutputTypeDef](./type_defs.md#referencesetsoutputtypedef)
- [ReferenceSetsTypeDef](./type_defs.md#referencesetstypedef)
- [IPSetUnionTypeDef](./type_defs.md#ipsetuniontypedef)
- [ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef](./type_defs.md#listfirewallpoliciesrequestlistfirewallpoliciespaginatetypedef)
- [ListFirewallsRequestListFirewallsPaginateTypeDef](./type_defs.md#listfirewallsrequestlistfirewallspaginatetypedef)
- [ListRuleGroupsRequestListRuleGroupsPaginateTypeDef](./type_defs.md#listrulegroupsrequestlistrulegroupspaginatetypedef)
- [ListTLSInspectionConfigurationsRequestListTLSInspectionConfigurationsPaginateTypeDef](./type_defs.md#listtlsinspectionconfigurationsrequestlisttlsinspectionconfigurationspaginatetypedef)
- [ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef)
- [ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef)
- [ListTLSInspectionConfigurationsResponseTypeDef](./type_defs.md#listtlsinspectionconfigurationsresponsetypedef)
- [LoggingConfigurationOutputTypeDef](./type_defs.md#loggingconfigurationoutputtypedef)
- [LogDestinationConfigUnionTypeDef](./type_defs.md#logdestinationconfiguniontypedef)
- [ServerCertificateScopeOutputTypeDef](./type_defs.md#servercertificatescopeoutputtypedef)
- [ServerCertificateScopeTypeDef](./type_defs.md#servercertificatescopetypedef)
- [MatchAttributesOutputTypeDef](./type_defs.md#matchattributesoutputtypedef)
- [SyncStateTypeDef](./type_defs.md#syncstatetypedef)
- [RuleVariablesOutputTypeDef](./type_defs.md#rulevariablesoutputtypedef)
- [PortSetUnionTypeDef](./type_defs.md#portsetuniontypedef)
- [StatefulRuleOutputTypeDef](./type_defs.md#statefulruleoutputtypedef)
- [RuleOptionUnionTypeDef](./type_defs.md#ruleoptionuniontypedef)
- [RulesSourceListUnionTypeDef](./type_defs.md#rulessourcelistuniontypedef)
- [StatefulRuleGroupReferenceTypeDef](./type_defs.md#statefulrulegroupreferencetypedef)
- [TCPFlagFieldUnionTypeDef](./type_defs.md#tcpflagfielduniontypedef)
- [TLSInspectionConfigurationResponseTypeDef](./type_defs.md#tlsinspectionconfigurationresponsetypedef)
- [CapacityUsageSummaryTypeDef](./type_defs.md#capacityusagesummarytypedef)
- [CreateFirewallPolicyResponseTypeDef](./type_defs.md#createfirewallpolicyresponsetypedef)
- [DeleteFirewallPolicyResponseTypeDef](./type_defs.md#deletefirewallpolicyresponsetypedef)
- [UpdateFirewallPolicyResponseTypeDef](./type_defs.md#updatefirewallpolicyresponsetypedef)
- [CreateRuleGroupResponseTypeDef](./type_defs.md#createrulegroupresponsetypedef)
- [DeleteRuleGroupResponseTypeDef](./type_defs.md#deleterulegroupresponsetypedef)
- [UpdateRuleGroupResponseTypeDef](./type_defs.md#updaterulegroupresponsetypedef)
- [ActionDefinitionOutputTypeDef](./type_defs.md#actiondefinitionoutputtypedef)
- [PublishMetricActionUnionTypeDef](./type_defs.md#publishmetricactionuniontypedef)
- [ReferenceSetsUnionTypeDef](./type_defs.md#referencesetsuniontypedef)
- [PolicyVariablesTypeDef](./type_defs.md#policyvariablestypedef)
- [DescribeLoggingConfigurationResponseTypeDef](./type_defs.md#describeloggingconfigurationresponsetypedef)
- [UpdateLoggingConfigurationResponseTypeDef](./type_defs.md#updateloggingconfigurationresponsetypedef)
- [LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef)
- [ServerCertificateConfigurationOutputTypeDef](./type_defs.md#servercertificateconfigurationoutputtypedef)
- [ServerCertificateScopeUnionTypeDef](./type_defs.md#servercertificatescopeuniontypedef)
- [RuleDefinitionOutputTypeDef](./type_defs.md#ruledefinitionoutputtypedef)
- [RuleVariablesTypeDef](./type_defs.md#rulevariablestypedef)
- [StatefulRuleTypeDef](./type_defs.md#statefulruletypedef)
- [MatchAttributesTypeDef](./type_defs.md#matchattributestypedef)
- [CreateTLSInspectionConfigurationResponseTypeDef](./type_defs.md#createtlsinspectionconfigurationresponsetypedef)
- [DeleteTLSInspectionConfigurationResponseTypeDef](./type_defs.md#deletetlsinspectionconfigurationresponsetypedef)
- [UpdateTLSInspectionConfigurationResponseTypeDef](./type_defs.md#updatetlsinspectionconfigurationresponsetypedef)
- [FirewallStatusTypeDef](./type_defs.md#firewallstatustypedef)
- [CustomActionOutputTypeDef](./type_defs.md#customactionoutputtypedef)
- [ActionDefinitionTypeDef](./type_defs.md#actiondefinitiontypedef)
- [PolicyVariablesUnionTypeDef](./type_defs.md#policyvariablesuniontypedef)
- [UpdateLoggingConfigurationRequestRequestTypeDef](./type_defs.md#updateloggingconfigurationrequestrequesttypedef)
- [TLSInspectionConfigurationOutputTypeDef](./type_defs.md#tlsinspectionconfigurationoutputtypedef)
- [ServerCertificateConfigurationTypeDef](./type_defs.md#servercertificateconfigurationtypedef)
- [StatelessRuleOutputTypeDef](./type_defs.md#statelessruleoutputtypedef)
- [RuleVariablesUnionTypeDef](./type_defs.md#rulevariablesuniontypedef)
- [StatefulRuleUnionTypeDef](./type_defs.md#statefulruleuniontypedef)
- [MatchAttributesUnionTypeDef](./type_defs.md#matchattributesuniontypedef)
- [CreateFirewallResponseTypeDef](./type_defs.md#createfirewallresponsetypedef)
- [DeleteFirewallResponseTypeDef](./type_defs.md#deletefirewallresponsetypedef)
- [DescribeFirewallResponseTypeDef](./type_defs.md#describefirewallresponsetypedef)
- [FirewallPolicyOutputTypeDef](./type_defs.md#firewallpolicyoutputtypedef)
- [ActionDefinitionUnionTypeDef](./type_defs.md#actiondefinitionuniontypedef)
- [DescribeTLSInspectionConfigurationResponseTypeDef](./type_defs.md#describetlsinspectionconfigurationresponsetypedef)
- [ServerCertificateConfigurationUnionTypeDef](./type_defs.md#servercertificateconfigurationuniontypedef)
- [StatelessRulesAndCustomActionsOutputTypeDef](./type_defs.md#statelessrulesandcustomactionsoutputtypedef)
- [RuleDefinitionTypeDef](./type_defs.md#ruledefinitiontypedef)
- [DescribeFirewallPolicyResponseTypeDef](./type_defs.md#describefirewallpolicyresponsetypedef)
- [CustomActionTypeDef](./type_defs.md#customactiontypedef)
- [TLSInspectionConfigurationTypeDef](./type_defs.md#tlsinspectionconfigurationtypedef)
- [RulesSourceOutputTypeDef](./type_defs.md#rulessourceoutputtypedef)
- [RuleDefinitionUnionTypeDef](./type_defs.md#ruledefinitionuniontypedef)
- [CustomActionUnionTypeDef](./type_defs.md#customactionuniontypedef)
- [CreateTLSInspectionConfigurationRequestRequestTypeDef](./type_defs.md#createtlsinspectionconfigurationrequestrequesttypedef)
- [UpdateTLSInspectionConfigurationRequestRequestTypeDef](./type_defs.md#updatetlsinspectionconfigurationrequestrequesttypedef)
- [RuleGroupOutputTypeDef](./type_defs.md#rulegroupoutputtypedef)
- [StatelessRuleTypeDef](./type_defs.md#statelessruletypedef)
- [FirewallPolicyTypeDef](./type_defs.md#firewallpolicytypedef)
- [DescribeRuleGroupResponseTypeDef](./type_defs.md#describerulegroupresponsetypedef)
- [StatelessRuleUnionTypeDef](./type_defs.md#statelessruleuniontypedef)
- [CreateFirewallPolicyRequestRequestTypeDef](./type_defs.md#createfirewallpolicyrequestrequesttypedef)
- [UpdateFirewallPolicyRequestRequestTypeDef](./type_defs.md#updatefirewallpolicyrequestrequesttypedef)
- [StatelessRulesAndCustomActionsTypeDef](./type_defs.md#statelessrulesandcustomactionstypedef)
- [StatelessRulesAndCustomActionsUnionTypeDef](./type_defs.md#statelessrulesandcustomactionsuniontypedef)
- [RulesSourceTypeDef](./type_defs.md#rulessourcetypedef)
- [RulesSourceUnionTypeDef](./type_defs.md#rulessourceuniontypedef)
- [RuleGroupTypeDef](./type_defs.md#rulegrouptypedef)
- [CreateRuleGroupRequestRequestTypeDef](./type_defs.md#createrulegrouprequestrequesttypedef)
- [UpdateRuleGroupRequestRequestTypeDef](./type_defs.md#updaterulegrouprequestrequesttypedef)

