# EKS module

> [Index](../README.md) > EKS


!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#eks)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `EKS` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `EKS` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[eks]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[eks]'

# standalone installation
python -m pip install types-aiobotocore-eks
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-eks
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EKSClient

Type annotations and code completion for  `#!python session.create_client("eks")` as [EKSClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS.Client)

```python
# EKSClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_eks.client import EKSClient


session = get_session()
async with session.create_client("eks") as client:
    client: EKSClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("eks").get_paginator("...")`.

```python
# DescribeAddonVersionsPaginator usage example

from types_aiobotocore_eks.paginator import DescribeAddonVersionsPaginator

def get_describe_addon_versions_paginator() -> DescribeAddonVersionsPaginator:
    return client.get_paginator("describe_addon_versions"))
```

- [DescribeAddonVersionsPaginator](./paginators.md#describeaddonversionspaginator)
- [DescribeClusterVersionsPaginator](./paginators.md#describeclusterversionspaginator)
- [ListAccessEntriesPaginator](./paginators.md#listaccessentriespaginator)
- [ListAccessPoliciesPaginator](./paginators.md#listaccesspoliciespaginator)
- [ListAddonsPaginator](./paginators.md#listaddonspaginator)
- [ListAssociatedAccessPoliciesPaginator](./paginators.md#listassociatedaccesspoliciespaginator)
- [ListCapabilitiesPaginator](./paginators.md#listcapabilitiespaginator)
- [ListClustersPaginator](./paginators.md#listclusterspaginator)
- [ListEksAnywhereSubscriptionsPaginator](./paginators.md#listeksanywheresubscriptionspaginator)
- [ListFargateProfilesPaginator](./paginators.md#listfargateprofilespaginator)
- [ListIdentityProviderConfigsPaginator](./paginators.md#listidentityproviderconfigspaginator)
- [ListInsightsPaginator](./paginators.md#listinsightspaginator)
- [ListNodegroupsPaginator](./paginators.md#listnodegroupspaginator)
- [ListPodIdentityAssociationsPaginator](./paginators.md#listpodidentityassociationspaginator)
- [ListUpdatesPaginator](./paginators.md#listupdatespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("eks").get_waiter("...")`.

```python
# AddonActiveWaiter usage example

from types_aiobotocore_eks.waiter import AddonActiveWaiter

def get_addon_active_waiter() -> AddonActiveWaiter:
    return Session().client("eks").get_waiter("addon_active")
```

- [AddonActiveWaiter](./waiters.md#addonactivewaiter)
- [AddonDeletedWaiter](./waiters.md#addondeletedwaiter)
- [ClusterActiveWaiter](./waiters.md#clusteractivewaiter)
- [ClusterDeletedWaiter](./waiters.md#clusterdeletedwaiter)
- [FargateProfileActiveWaiter](./waiters.md#fargateprofileactivewaiter)
- [FargateProfileDeletedWaiter](./waiters.md#fargateprofiledeletedwaiter)
- [NodegroupActiveWaiter](./waiters.md#nodegroupactivewaiter)
- [NodegroupDeletedWaiter](./waiters.md#nodegroupdeletedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AMITypesType usage example

from types_aiobotocore_eks.literals import AMITypesType

def get_value() -> AMITypesType:
    return "AL2023_ARM_64_NVIDIA"
```

- [AMITypesType](./literals.md#amitypestype)
- [AccessScopeTypeType](./literals.md#accessscopetypetype)
- [AddonActiveWaiterName](./literals.md#addonactivewaitername)
- [AddonDeletedWaiterName](./literals.md#addondeletedwaitername)
- [AddonIssueCodeType](./literals.md#addonissuecodetype)
- [AddonStatusType](./literals.md#addonstatustype)
- [ArgoCdRoleType](./literals.md#argocdroletype)
- [AuthenticationModeType](./literals.md#authenticationmodetype)
- [CapabilityDeletePropagationPolicyType](./literals.md#capabilitydeletepropagationpolicytype)
- [CapabilityIssueCodeType](./literals.md#capabilityissuecodetype)
- [CapabilityStatusType](./literals.md#capabilitystatustype)
- [CapabilityTypeType](./literals.md#capabilitytypetype)
- [CapacityTypesType](./literals.md#capacitytypestype)
- [CategoryType](./literals.md#categorytype)
- [ClusterActiveWaiterName](./literals.md#clusteractivewaitername)
- [ClusterDeletedWaiterName](./literals.md#clusterdeletedwaitername)
- [ClusterIssueCodeType](./literals.md#clusterissuecodetype)
- [ClusterStatusType](./literals.md#clusterstatustype)
- [ClusterVersionStatusType](./literals.md#clusterversionstatustype)
- [ConfigStatusType](./literals.md#configstatustype)
- [ConnectorConfigProviderType](./literals.md#connectorconfigprovidertype)
- [DescribeAddonVersionsPaginatorName](./literals.md#describeaddonversionspaginatorname)
- [DescribeClusterVersionsPaginatorName](./literals.md#describeclusterversionspaginatorname)
- [EksAnywhereSubscriptionLicenseTypeType](./literals.md#eksanywheresubscriptionlicensetypetype)
- [EksAnywhereSubscriptionStatusType](./literals.md#eksanywheresubscriptionstatustype)
- [EksAnywhereSubscriptionTermUnitType](./literals.md#eksanywheresubscriptiontermunittype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [FargateProfileActiveWaiterName](./literals.md#fargateprofileactivewaitername)
- [FargateProfileDeletedWaiterName](./literals.md#fargateprofiledeletedwaitername)
- [FargateProfileIssueCodeType](./literals.md#fargateprofileissuecodetype)
- [FargateProfileStatusType](./literals.md#fargateprofilestatustype)
- [InsightStatusValueType](./literals.md#insightstatusvaluetype)
- [InsightsRefreshStatusType](./literals.md#insightsrefreshstatustype)
- [IpFamilyType](./literals.md#ipfamilytype)
- [ListAccessEntriesPaginatorName](./literals.md#listaccessentriespaginatorname)
- [ListAccessPoliciesPaginatorName](./literals.md#listaccesspoliciespaginatorname)
- [ListAddonsPaginatorName](./literals.md#listaddonspaginatorname)
- [ListAssociatedAccessPoliciesPaginatorName](./literals.md#listassociatedaccesspoliciespaginatorname)
- [ListCapabilitiesPaginatorName](./literals.md#listcapabilitiespaginatorname)
- [ListClustersPaginatorName](./literals.md#listclusterspaginatorname)
- [ListEksAnywhereSubscriptionsPaginatorName](./literals.md#listeksanywheresubscriptionspaginatorname)
- [ListFargateProfilesPaginatorName](./literals.md#listfargateprofilespaginatorname)
- [ListIdentityProviderConfigsPaginatorName](./literals.md#listidentityproviderconfigspaginatorname)
- [ListInsightsPaginatorName](./literals.md#listinsightspaginatorname)
- [ListNodegroupsPaginatorName](./literals.md#listnodegroupspaginatorname)
- [ListPodIdentityAssociationsPaginatorName](./literals.md#listpodidentityassociationspaginatorname)
- [ListUpdatesPaginatorName](./literals.md#listupdatespaginatorname)
- [LogTypeType](./literals.md#logtypetype)
- [NodegroupActiveWaiterName](./literals.md#nodegroupactivewaitername)
- [NodegroupDeletedWaiterName](./literals.md#nodegroupdeletedwaitername)
- [NodegroupIssueCodeType](./literals.md#nodegroupissuecodetype)
- [NodegroupStatusType](./literals.md#nodegroupstatustype)
- [NodegroupUpdateStrategiesType](./literals.md#nodegroupupdatestrategiestype)
- [ProvisionedControlPlaneTierType](./literals.md#provisionedcontrolplanetiertype)
- [RepairActionType](./literals.md#repairactiontype)
- [ResolveConflictsType](./literals.md#resolveconflictstype)
- [SsoIdentityTypeType](./literals.md#ssoidentitytypetype)
- [SupportTypeType](./literals.md#supporttypetype)
- [TaintEffectType](./literals.md#tainteffecttype)
- [UpdateParamTypeType](./literals.md#updateparamtypetype)
- [UpdateStatusType](./literals.md#updatestatustype)
- [UpdateTypeType](./literals.md#updatetypetype)
- [VersionStatusType](./literals.md#versionstatustype)
- [EKSServiceName](./literals.md#eksservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessConfigResponseTypeDef](./type_defs.md#accessconfigresponsetypedef)
- [AccessEntryTypeDef](./type_defs.md#accessentrytypedef)
- [AccessPolicyTypeDef](./type_defs.md#accesspolicytypedef)
- [AccessScopeOutputTypeDef](./type_defs.md#accessscopeoutputtypedef)
- [AccessScopeTypeDef](./type_defs.md#accessscopetypedef)
- [AddonCompatibilityDetailTypeDef](./type_defs.md#addoncompatibilitydetailtypedef)
- [AddonIssueTypeDef](./type_defs.md#addonissuetypedef)
- [MarketplaceInformationTypeDef](./type_defs.md#marketplaceinformationtypedef)
- [AddonNamespaceConfigRequestTypeDef](./type_defs.md#addonnamespaceconfigrequesttypedef)
- [AddonNamespaceConfigResponseTypeDef](./type_defs.md#addonnamespaceconfigresponsetypedef)
- [AddonPodIdentityAssociationsTypeDef](./type_defs.md#addonpodidentityassociationstypedef)
- [AddonPodIdentityConfigurationTypeDef](./type_defs.md#addonpodidentityconfigurationtypedef)
- [CompatibilityTypeDef](./type_defs.md#compatibilitytypedef)
- [ArgoCdAwsIdcConfigRequestTypeDef](./type_defs.md#argocdawsidcconfigrequesttypedef)
- [ArgoCdAwsIdcConfigResponseTypeDef](./type_defs.md#argocdawsidcconfigresponsetypedef)
- [ArgoCdNetworkAccessConfigRequestTypeDef](./type_defs.md#argocdnetworkaccessconfigrequesttypedef)
- [ArgoCdNetworkAccessConfigResponseTypeDef](./type_defs.md#argocdnetworkaccessconfigresponsetypedef)
- [SsoIdentityTypeDef](./type_defs.md#ssoidentitytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [OidcIdentityProviderConfigRequestTypeDef](./type_defs.md#oidcidentityproviderconfigrequesttypedef)
- [AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef)
- [BlockStorageTypeDef](./type_defs.md#blockstoragetypedef)
- [CapabilityIssueTypeDef](./type_defs.md#capabilityissuetypedef)
- [CapabilitySummaryTypeDef](./type_defs.md#capabilitysummarytypedef)
- [CertificateTypeDef](./type_defs.md#certificatetypedef)
- [ClientStatTypeDef](./type_defs.md#clientstattypedef)
- [ClusterIssueTypeDef](./type_defs.md#clusterissuetypedef)
- [ComputeConfigResponseTypeDef](./type_defs.md#computeconfigresponsetypedef)
- [ConnectorConfigResponseTypeDef](./type_defs.md#connectorconfigresponsetypedef)
- [ControlPlaneScalingConfigTypeDef](./type_defs.md#controlplanescalingconfigtypedef)
- [UpgradePolicyResponseTypeDef](./type_defs.md#upgradepolicyresponsetypedef)
- [VpcConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef)
- [ZonalShiftConfigResponseTypeDef](./type_defs.md#zonalshiftconfigresponsetypedef)
- [ClusterVersionInformationTypeDef](./type_defs.md#clusterversioninformationtypedef)
- [ComputeConfigRequestTypeDef](./type_defs.md#computeconfigrequesttypedef)
- [ConnectorConfigRequestTypeDef](./type_defs.md#connectorconfigrequesttypedef)
- [ControlPlanePlacementRequestTypeDef](./type_defs.md#controlplaneplacementrequesttypedef)
- [ControlPlanePlacementResponseTypeDef](./type_defs.md#controlplaneplacementresponsetypedef)
- [CreateAccessConfigRequestTypeDef](./type_defs.md#createaccessconfigrequesttypedef)
- [CreateAccessEntryRequestTypeDef](./type_defs.md#createaccessentryrequesttypedef)
- [UpgradePolicyRequestTypeDef](./type_defs.md#upgradepolicyrequesttypedef)
- [VpcConfigRequestTypeDef](./type_defs.md#vpcconfigrequesttypedef)
- [ZonalShiftConfigRequestTypeDef](./type_defs.md#zonalshiftconfigrequesttypedef)
- [EksAnywhereSubscriptionTermTypeDef](./type_defs.md#eksanywheresubscriptiontermtypedef)
- [LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef)
- [NodegroupScalingConfigTypeDef](./type_defs.md#nodegroupscalingconfigtypedef)
- [NodegroupUpdateConfigTypeDef](./type_defs.md#nodegroupupdateconfigtypedef)
- [TaintTypeDef](./type_defs.md#tainttypedef)
- [CreatePodIdentityAssociationRequestTypeDef](./type_defs.md#createpodidentityassociationrequesttypedef)
- [PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef)
- [DeleteAccessEntryRequestTypeDef](./type_defs.md#deleteaccessentryrequesttypedef)
- [DeleteAddonRequestTypeDef](./type_defs.md#deleteaddonrequesttypedef)
- [DeleteCapabilityRequestTypeDef](./type_defs.md#deletecapabilityrequesttypedef)
- [DeleteClusterRequestTypeDef](./type_defs.md#deleteclusterrequesttypedef)
- [DeleteEksAnywhereSubscriptionRequestTypeDef](./type_defs.md#deleteeksanywheresubscriptionrequesttypedef)
- [DeleteFargateProfileRequestTypeDef](./type_defs.md#deletefargateprofilerequesttypedef)
- [DeleteNodegroupRequestTypeDef](./type_defs.md#deletenodegrouprequesttypedef)
- [DeletePodIdentityAssociationRequestTypeDef](./type_defs.md#deletepodidentityassociationrequesttypedef)
- [DeregisterClusterRequestTypeDef](./type_defs.md#deregisterclusterrequesttypedef)
- [DescribeAccessEntryRequestTypeDef](./type_defs.md#describeaccessentryrequesttypedef)
- [DescribeAddonConfigurationRequestTypeDef](./type_defs.md#describeaddonconfigurationrequesttypedef)
- [DescribeAddonRequestTypeDef](./type_defs.md#describeaddonrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeAddonVersionsRequestTypeDef](./type_defs.md#describeaddonversionsrequesttypedef)
- [DescribeCapabilityRequestTypeDef](./type_defs.md#describecapabilityrequesttypedef)
- [DescribeClusterRequestTypeDef](./type_defs.md#describeclusterrequesttypedef)
- [DescribeClusterVersionsRequestTypeDef](./type_defs.md#describeclusterversionsrequesttypedef)
- [DescribeEksAnywhereSubscriptionRequestTypeDef](./type_defs.md#describeeksanywheresubscriptionrequesttypedef)
- [DescribeFargateProfileRequestTypeDef](./type_defs.md#describefargateprofilerequesttypedef)
- [IdentityProviderConfigTypeDef](./type_defs.md#identityproviderconfigtypedef)
- [DescribeInsightRequestTypeDef](./type_defs.md#describeinsightrequesttypedef)
- [DescribeInsightsRefreshRequestTypeDef](./type_defs.md#describeinsightsrefreshrequesttypedef)
- [DescribeNodegroupRequestTypeDef](./type_defs.md#describenodegrouprequesttypedef)
- [DescribePodIdentityAssociationRequestTypeDef](./type_defs.md#describepodidentityassociationrequesttypedef)
- [DescribeUpdateRequestTypeDef](./type_defs.md#describeupdaterequesttypedef)
- [DisassociateAccessPolicyRequestTypeDef](./type_defs.md#disassociateaccesspolicyrequesttypedef)
- [LicenseTypeDef](./type_defs.md#licensetypedef)
- [ElasticLoadBalancingTypeDef](./type_defs.md#elasticloadbalancingtypedef)
- [ProviderTypeDef](./type_defs.md#providertypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [FargateProfileIssueTypeDef](./type_defs.md#fargateprofileissuetypedef)
- [FargateProfileSelectorOutputTypeDef](./type_defs.md#fargateprofileselectoroutputtypedef)
- [FargateProfileSelectorTypeDef](./type_defs.md#fargateprofileselectortypedef)
- [OidcIdentityProviderConfigTypeDef](./type_defs.md#oidcidentityproviderconfigtypedef)
- [OIDCTypeDef](./type_defs.md#oidctypedef)
- [InsightStatusTypeDef](./type_defs.md#insightstatustypedef)
- [InsightsFilterTypeDef](./type_defs.md#insightsfiltertypedef)
- [IssueTypeDef](./type_defs.md#issuetypedef)
- [ListAccessEntriesRequestTypeDef](./type_defs.md#listaccessentriesrequesttypedef)
- [ListAccessPoliciesRequestTypeDef](./type_defs.md#listaccesspoliciesrequesttypedef)
- [ListAddonsRequestTypeDef](./type_defs.md#listaddonsrequesttypedef)
- [ListAssociatedAccessPoliciesRequestTypeDef](./type_defs.md#listassociatedaccesspoliciesrequesttypedef)
- [ListCapabilitiesRequestTypeDef](./type_defs.md#listcapabilitiesrequesttypedef)
- [ListClustersRequestTypeDef](./type_defs.md#listclustersrequesttypedef)
- [ListEksAnywhereSubscriptionsRequestTypeDef](./type_defs.md#listeksanywheresubscriptionsrequesttypedef)
- [ListFargateProfilesRequestTypeDef](./type_defs.md#listfargateprofilesrequesttypedef)
- [ListIdentityProviderConfigsRequestTypeDef](./type_defs.md#listidentityproviderconfigsrequesttypedef)
- [ListNodegroupsRequestTypeDef](./type_defs.md#listnodegroupsrequesttypedef)
- [ListPodIdentityAssociationsRequestTypeDef](./type_defs.md#listpodidentityassociationsrequesttypedef)
- [PodIdentityAssociationSummaryTypeDef](./type_defs.md#podidentityassociationsummarytypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListUpdatesRequestTypeDef](./type_defs.md#listupdatesrequesttypedef)
- [LogSetupOutputTypeDef](./type_defs.md#logsetupoutputtypedef)
- [LogSetupTypeDef](./type_defs.md#logsetuptypedef)
- [NodeRepairConfigOverridesTypeDef](./type_defs.md#noderepairconfigoverridestypedef)
- [RemoteAccessConfigOutputTypeDef](./type_defs.md#remoteaccessconfigoutputtypedef)
- [RemoteAccessConfigTypeDef](./type_defs.md#remoteaccessconfigtypedef)
- [RemoteNodeNetworkOutputTypeDef](./type_defs.md#remotenodenetworkoutputtypedef)
- [RemotePodNetworkOutputTypeDef](./type_defs.md#remotepodnetworkoutputtypedef)
- [RemoteNodeNetworkTypeDef](./type_defs.md#remotenodenetworktypedef)
- [RemotePodNetworkTypeDef](./type_defs.md#remotepodnetworktypedef)
- [StartInsightsRefreshRequestTypeDef](./type_defs.md#startinsightsrefreshrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateAccessConfigRequestTypeDef](./type_defs.md#updateaccessconfigrequesttypedef)
- [UpdateAccessEntryRequestTypeDef](./type_defs.md#updateaccessentryrequesttypedef)
- [UpdateClusterVersionRequestTypeDef](./type_defs.md#updateclusterversionrequesttypedef)
- [UpdateEksAnywhereSubscriptionRequestTypeDef](./type_defs.md#updateeksanywheresubscriptionrequesttypedef)
- [UpdateLabelsPayloadTypeDef](./type_defs.md#updatelabelspayloadtypedef)
- [UpdateParamTypeDef](./type_defs.md#updateparamtypedef)
- [UpdatePodIdentityAssociationRequestTypeDef](./type_defs.md#updatepodidentityassociationrequesttypedef)
- [AssociatedAccessPolicyTypeDef](./type_defs.md#associatedaccesspolicytypedef)
- [AccessScopeUnionTypeDef](./type_defs.md#accessscopeuniontypedef)
- [AddonHealthTypeDef](./type_defs.md#addonhealthtypedef)
- [CreateAddonRequestTypeDef](./type_defs.md#createaddonrequesttypedef)
- [UpdateAddonRequestTypeDef](./type_defs.md#updateaddonrequesttypedef)
- [AddonVersionInfoTypeDef](./type_defs.md#addonversioninfotypedef)
- [ArgoCdRoleMappingOutputTypeDef](./type_defs.md#argocdrolemappingoutputtypedef)
- [ArgoCdRoleMappingTypeDef](./type_defs.md#argocdrolemappingtypedef)
- [CreateAccessEntryResponseTypeDef](./type_defs.md#createaccessentryresponsetypedef)
- [DescribeAccessEntryResponseTypeDef](./type_defs.md#describeaccessentryresponsetypedef)
- [DescribeAddonConfigurationResponseTypeDef](./type_defs.md#describeaddonconfigurationresponsetypedef)
- [DescribeInsightsRefreshResponseTypeDef](./type_defs.md#describeinsightsrefreshresponsetypedef)
- [ListAccessEntriesResponseTypeDef](./type_defs.md#listaccessentriesresponsetypedef)
- [ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef)
- [ListAddonsResponseTypeDef](./type_defs.md#listaddonsresponsetypedef)
- [ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)
- [ListFargateProfilesResponseTypeDef](./type_defs.md#listfargateprofilesresponsetypedef)
- [ListNodegroupsResponseTypeDef](./type_defs.md#listnodegroupsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListUpdatesResponseTypeDef](./type_defs.md#listupdatesresponsetypedef)
- [StartInsightsRefreshResponseTypeDef](./type_defs.md#startinsightsrefreshresponsetypedef)
- [UpdateAccessEntryResponseTypeDef](./type_defs.md#updateaccessentryresponsetypedef)
- [AssociateIdentityProviderConfigRequestTypeDef](./type_defs.md#associateidentityproviderconfigrequesttypedef)
- [NodegroupResourcesTypeDef](./type_defs.md#nodegroupresourcestypedef)
- [StorageConfigRequestTypeDef](./type_defs.md#storageconfigrequesttypedef)
- [StorageConfigResponseTypeDef](./type_defs.md#storageconfigresponsetypedef)
- [CapabilityHealthTypeDef](./type_defs.md#capabilityhealthtypedef)
- [ListCapabilitiesResponseTypeDef](./type_defs.md#listcapabilitiesresponsetypedef)
- [DeprecationDetailTypeDef](./type_defs.md#deprecationdetailtypedef)
- [ClusterHealthTypeDef](./type_defs.md#clusterhealthtypedef)
- [DescribeClusterVersionsResponseTypeDef](./type_defs.md#describeclusterversionsresponsetypedef)
- [RegisterClusterRequestTypeDef](./type_defs.md#registerclusterrequesttypedef)
- [OutpostConfigRequestTypeDef](./type_defs.md#outpostconfigrequesttypedef)
- [OutpostConfigResponseTypeDef](./type_defs.md#outpostconfigresponsetypedef)
- [CreateEksAnywhereSubscriptionRequestTypeDef](./type_defs.md#createeksanywheresubscriptionrequesttypedef)
- [UpdateNodegroupVersionRequestTypeDef](./type_defs.md#updatenodegroupversionrequesttypedef)
- [UpdateTaintsPayloadTypeDef](./type_defs.md#updatetaintspayloadtypedef)
- [CreatePodIdentityAssociationResponseTypeDef](./type_defs.md#createpodidentityassociationresponsetypedef)
- [DeletePodIdentityAssociationResponseTypeDef](./type_defs.md#deletepodidentityassociationresponsetypedef)
- [DescribePodIdentityAssociationResponseTypeDef](./type_defs.md#describepodidentityassociationresponsetypedef)
- [UpdatePodIdentityAssociationResponseTypeDef](./type_defs.md#updatepodidentityassociationresponsetypedef)
- [DescribeAddonRequestWaitExtraTypeDef](./type_defs.md#describeaddonrequestwaitextratypedef)
- [DescribeAddonRequestWaitTypeDef](./type_defs.md#describeaddonrequestwaittypedef)
- [DescribeClusterRequestWaitExtraTypeDef](./type_defs.md#describeclusterrequestwaitextratypedef)
- [DescribeClusterRequestWaitTypeDef](./type_defs.md#describeclusterrequestwaittypedef)
- [DescribeFargateProfileRequestWaitExtraTypeDef](./type_defs.md#describefargateprofilerequestwaitextratypedef)
- [DescribeFargateProfileRequestWaitTypeDef](./type_defs.md#describefargateprofilerequestwaittypedef)
- [DescribeNodegroupRequestWaitExtraTypeDef](./type_defs.md#describenodegrouprequestwaitextratypedef)
- [DescribeNodegroupRequestWaitTypeDef](./type_defs.md#describenodegrouprequestwaittypedef)
- [DescribeAddonVersionsRequestPaginateTypeDef](./type_defs.md#describeaddonversionsrequestpaginatetypedef)
- [DescribeClusterVersionsRequestPaginateTypeDef](./type_defs.md#describeclusterversionsrequestpaginatetypedef)
- [ListAccessEntriesRequestPaginateTypeDef](./type_defs.md#listaccessentriesrequestpaginatetypedef)
- [ListAccessPoliciesRequestPaginateTypeDef](./type_defs.md#listaccesspoliciesrequestpaginatetypedef)
- [ListAddonsRequestPaginateTypeDef](./type_defs.md#listaddonsrequestpaginatetypedef)
- [ListAssociatedAccessPoliciesRequestPaginateTypeDef](./type_defs.md#listassociatedaccesspoliciesrequestpaginatetypedef)
- [ListCapabilitiesRequestPaginateTypeDef](./type_defs.md#listcapabilitiesrequestpaginatetypedef)
- [ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef)
- [ListEksAnywhereSubscriptionsRequestPaginateTypeDef](./type_defs.md#listeksanywheresubscriptionsrequestpaginatetypedef)
- [ListFargateProfilesRequestPaginateTypeDef](./type_defs.md#listfargateprofilesrequestpaginatetypedef)
- [ListIdentityProviderConfigsRequestPaginateTypeDef](./type_defs.md#listidentityproviderconfigsrequestpaginatetypedef)
- [ListNodegroupsRequestPaginateTypeDef](./type_defs.md#listnodegroupsrequestpaginatetypedef)
- [ListPodIdentityAssociationsRequestPaginateTypeDef](./type_defs.md#listpodidentityassociationsrequestpaginatetypedef)
- [ListUpdatesRequestPaginateTypeDef](./type_defs.md#listupdatesrequestpaginatetypedef)
- [DescribeIdentityProviderConfigRequestTypeDef](./type_defs.md#describeidentityproviderconfigrequesttypedef)
- [DisassociateIdentityProviderConfigRequestTypeDef](./type_defs.md#disassociateidentityproviderconfigrequesttypedef)
- [ListIdentityProviderConfigsResponseTypeDef](./type_defs.md#listidentityproviderconfigsresponsetypedef)
- [EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef)
- [KubernetesNetworkConfigRequestTypeDef](./type_defs.md#kubernetesnetworkconfigrequesttypedef)
- [KubernetesNetworkConfigResponseTypeDef](./type_defs.md#kubernetesnetworkconfigresponsetypedef)
- [EncryptionConfigOutputTypeDef](./type_defs.md#encryptionconfigoutputtypedef)
- [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- [FargateProfileHealthTypeDef](./type_defs.md#fargateprofilehealthtypedef)
- [FargateProfileSelectorUnionTypeDef](./type_defs.md#fargateprofileselectoruniontypedef)
- [IdentityProviderConfigResponseTypeDef](./type_defs.md#identityproviderconfigresponsetypedef)
- [IdentityTypeDef](./type_defs.md#identitytypedef)
- [InsightResourceDetailTypeDef](./type_defs.md#insightresourcedetailtypedef)
- [InsightSummaryTypeDef](./type_defs.md#insightsummarytypedef)
- [ListInsightsRequestPaginateTypeDef](./type_defs.md#listinsightsrequestpaginatetypedef)
- [ListInsightsRequestTypeDef](./type_defs.md#listinsightsrequesttypedef)
- [NodegroupHealthTypeDef](./type_defs.md#nodegrouphealthtypedef)
- [ListPodIdentityAssociationsResponseTypeDef](./type_defs.md#listpodidentityassociationsresponsetypedef)
- [LoggingOutputTypeDef](./type_defs.md#loggingoutputtypedef)
- [LoggingTypeDef](./type_defs.md#loggingtypedef)
- [NodeRepairConfigOutputTypeDef](./type_defs.md#noderepairconfigoutputtypedef)
- [NodeRepairConfigTypeDef](./type_defs.md#noderepairconfigtypedef)
- [RemoteAccessConfigUnionTypeDef](./type_defs.md#remoteaccessconfiguniontypedef)
- [RemoteNetworkConfigResponseTypeDef](./type_defs.md#remotenetworkconfigresponsetypedef)
- [RemoteNodeNetworkUnionTypeDef](./type_defs.md#remotenodenetworkuniontypedef)
- [RemotePodNetworkUnionTypeDef](./type_defs.md#remotepodnetworkuniontypedef)
- [UpdateTypeDef](./type_defs.md#updatetypedef)
- [AssociateAccessPolicyResponseTypeDef](./type_defs.md#associateaccesspolicyresponsetypedef)
- [ListAssociatedAccessPoliciesResponseTypeDef](./type_defs.md#listassociatedaccesspoliciesresponsetypedef)
- [AssociateAccessPolicyRequestTypeDef](./type_defs.md#associateaccesspolicyrequesttypedef)
- [AddonTypeDef](./type_defs.md#addontypedef)
- [AddonInfoTypeDef](./type_defs.md#addoninfotypedef)
- [ArgoCdConfigResponseTypeDef](./type_defs.md#argocdconfigresponsetypedef)
- [ArgoCdRoleMappingUnionTypeDef](./type_defs.md#argocdrolemappinguniontypedef)
- [InsightCategorySpecificSummaryTypeDef](./type_defs.md#insightcategoryspecificsummarytypedef)
- [CreateEksAnywhereSubscriptionResponseTypeDef](./type_defs.md#createeksanywheresubscriptionresponsetypedef)
- [DeleteEksAnywhereSubscriptionResponseTypeDef](./type_defs.md#deleteeksanywheresubscriptionresponsetypedef)
- [DescribeEksAnywhereSubscriptionResponseTypeDef](./type_defs.md#describeeksanywheresubscriptionresponsetypedef)
- [ListEksAnywhereSubscriptionsResponseTypeDef](./type_defs.md#listeksanywheresubscriptionsresponsetypedef)
- [UpdateEksAnywhereSubscriptionResponseTypeDef](./type_defs.md#updateeksanywheresubscriptionresponsetypedef)
- [EncryptionConfigUnionTypeDef](./type_defs.md#encryptionconfiguniontypedef)
- [FargateProfileTypeDef](./type_defs.md#fargateprofiletypedef)
- [CreateFargateProfileRequestTypeDef](./type_defs.md#createfargateprofilerequesttypedef)
- [DescribeIdentityProviderConfigResponseTypeDef](./type_defs.md#describeidentityproviderconfigresponsetypedef)
- [ListInsightsResponseTypeDef](./type_defs.md#listinsightsresponsetypedef)
- [LoggingUnionTypeDef](./type_defs.md#logginguniontypedef)
- [NodegroupTypeDef](./type_defs.md#nodegrouptypedef)
- [NodeRepairConfigUnionTypeDef](./type_defs.md#noderepairconfiguniontypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [RemoteNetworkConfigRequestTypeDef](./type_defs.md#remotenetworkconfigrequesttypedef)
- [AssociateEncryptionConfigResponseTypeDef](./type_defs.md#associateencryptionconfigresponsetypedef)
- [AssociateIdentityProviderConfigResponseTypeDef](./type_defs.md#associateidentityproviderconfigresponsetypedef)
- [DescribeUpdateResponseTypeDef](./type_defs.md#describeupdateresponsetypedef)
- [DisassociateIdentityProviderConfigResponseTypeDef](./type_defs.md#disassociateidentityproviderconfigresponsetypedef)
- [UpdateAddonResponseTypeDef](./type_defs.md#updateaddonresponsetypedef)
- [UpdateCapabilityResponseTypeDef](./type_defs.md#updatecapabilityresponsetypedef)
- [UpdateClusterConfigResponseTypeDef](./type_defs.md#updateclusterconfigresponsetypedef)
- [UpdateClusterVersionResponseTypeDef](./type_defs.md#updateclusterversionresponsetypedef)
- [UpdateNodegroupConfigResponseTypeDef](./type_defs.md#updatenodegroupconfigresponsetypedef)
- [UpdateNodegroupVersionResponseTypeDef](./type_defs.md#updatenodegroupversionresponsetypedef)
- [CreateAddonResponseTypeDef](./type_defs.md#createaddonresponsetypedef)
- [DeleteAddonResponseTypeDef](./type_defs.md#deleteaddonresponsetypedef)
- [DescribeAddonResponseTypeDef](./type_defs.md#describeaddonresponsetypedef)
- [DescribeAddonVersionsResponseTypeDef](./type_defs.md#describeaddonversionsresponsetypedef)
- [CapabilityConfigurationResponseTypeDef](./type_defs.md#capabilityconfigurationresponsetypedef)
- [ArgoCdConfigRequestTypeDef](./type_defs.md#argocdconfigrequesttypedef)
- [UpdateRoleMappingsTypeDef](./type_defs.md#updaterolemappingstypedef)
- [InsightTypeDef](./type_defs.md#insighttypedef)
- [AssociateEncryptionConfigRequestTypeDef](./type_defs.md#associateencryptionconfigrequesttypedef)
- [CreateFargateProfileResponseTypeDef](./type_defs.md#createfargateprofileresponsetypedef)
- [DeleteFargateProfileResponseTypeDef](./type_defs.md#deletefargateprofileresponsetypedef)
- [DescribeFargateProfileResponseTypeDef](./type_defs.md#describefargateprofileresponsetypedef)
- [CreateNodegroupResponseTypeDef](./type_defs.md#createnodegroupresponsetypedef)
- [DeleteNodegroupResponseTypeDef](./type_defs.md#deletenodegroupresponsetypedef)
- [DescribeNodegroupResponseTypeDef](./type_defs.md#describenodegroupresponsetypedef)
- [CreateNodegroupRequestTypeDef](./type_defs.md#createnodegrouprequesttypedef)
- [UpdateNodegroupConfigRequestTypeDef](./type_defs.md#updatenodegroupconfigrequesttypedef)
- [CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)
- [DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef)
- [DeregisterClusterResponseTypeDef](./type_defs.md#deregisterclusterresponsetypedef)
- [DescribeClusterResponseTypeDef](./type_defs.md#describeclusterresponsetypedef)
- [RegisterClusterResponseTypeDef](./type_defs.md#registerclusterresponsetypedef)
- [CreateClusterRequestTypeDef](./type_defs.md#createclusterrequesttypedef)
- [UpdateClusterConfigRequestTypeDef](./type_defs.md#updateclusterconfigrequesttypedef)
- [CapabilityTypeDef](./type_defs.md#capabilitytypedef)
- [CapabilityConfigurationRequestTypeDef](./type_defs.md#capabilityconfigurationrequesttypedef)
- [UpdateArgoCdConfigTypeDef](./type_defs.md#updateargocdconfigtypedef)
- [DescribeInsightResponseTypeDef](./type_defs.md#describeinsightresponsetypedef)
- [CreateCapabilityResponseTypeDef](./type_defs.md#createcapabilityresponsetypedef)
- [DeleteCapabilityResponseTypeDef](./type_defs.md#deletecapabilityresponsetypedef)
- [DescribeCapabilityResponseTypeDef](./type_defs.md#describecapabilityresponsetypedef)
- [CreateCapabilityRequestTypeDef](./type_defs.md#createcapabilityrequesttypedef)
- [UpdateCapabilityConfigurationTypeDef](./type_defs.md#updatecapabilityconfigurationtypedef)
- [UpdateCapabilityRequestTypeDef](./type_defs.md#updatecapabilityrequesttypedef)

