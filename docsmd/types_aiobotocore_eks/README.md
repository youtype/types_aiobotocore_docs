# EKS module

> [Index](../README.md) > EKS


!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#eks)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
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
    return "AL2023_ARM_64_STANDARD"
```

- [AMITypesType](./literals.md#amitypestype)
- [AccessScopeTypeType](./literals.md#accessscopetypetype)
- [AddonActiveWaiterName](./literals.md#addonactivewaitername)
- [AddonDeletedWaiterName](./literals.md#addondeletedwaitername)
- [AddonIssueCodeType](./literals.md#addonissuecodetype)
- [AddonStatusType](./literals.md#addonstatustype)
- [AuthenticationModeType](./literals.md#authenticationmodetype)
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
- [IpFamilyType](./literals.md#ipfamilytype)
- [ListAccessEntriesPaginatorName](./literals.md#listaccessentriespaginatorname)
- [ListAccessPoliciesPaginatorName](./literals.md#listaccesspoliciespaginatorname)
- [ListAddonsPaginatorName](./literals.md#listaddonspaginatorname)
- [ListAssociatedAccessPoliciesPaginatorName](./literals.md#listassociatedaccesspoliciespaginatorname)
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
- [ResolveConflictsType](./literals.md#resolveconflictstype)
- [SupportTypeType](./literals.md#supporttypetype)
- [TaintEffectType](./literals.md#tainteffecttype)
- [UpdateParamTypeType](./literals.md#updateparamtypetype)
- [UpdateStatusType](./literals.md#updatestatustype)
- [UpdateTypeType](./literals.md#updatetypetype)
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
- [AddonPodIdentityAssociationsTypeDef](./type_defs.md#addonpodidentityassociationstypedef)
- [AddonPodIdentityConfigurationTypeDef](./type_defs.md#addonpodidentityconfigurationtypedef)
- [CompatibilityTypeDef](./type_defs.md#compatibilitytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [OidcIdentityProviderConfigRequestTypeDef](./type_defs.md#oidcidentityproviderconfigrequesttypedef)
- [AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef)
- [BlockStorageTypeDef](./type_defs.md#blockstoragetypedef)
- [CertificateTypeDef](./type_defs.md#certificatetypedef)
- [ClientStatTypeDef](./type_defs.md#clientstattypedef)
- [ClusterIssueTypeDef](./type_defs.md#clusterissuetypedef)
- [ComputeConfigResponseTypeDef](./type_defs.md#computeconfigresponsetypedef)
- [ConnectorConfigResponseTypeDef](./type_defs.md#connectorconfigresponsetypedef)
- [UpgradePolicyResponseTypeDef](./type_defs.md#upgradepolicyresponsetypedef)
- [VpcConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef)
- [ZonalShiftConfigResponseTypeDef](./type_defs.md#zonalshiftconfigresponsetypedef)
- [ClusterVersionInformationTypeDef](./type_defs.md#clusterversioninformationtypedef)
- [ComputeConfigRequestTypeDef](./type_defs.md#computeconfigrequesttypedef)
- [ConnectorConfigRequestTypeDef](./type_defs.md#connectorconfigrequesttypedef)
- [ControlPlanePlacementRequestTypeDef](./type_defs.md#controlplaneplacementrequesttypedef)
- [ControlPlanePlacementResponseTypeDef](./type_defs.md#controlplaneplacementresponsetypedef)
- [CreateAccessConfigRequestTypeDef](./type_defs.md#createaccessconfigrequesttypedef)
- [CreateAccessEntryRequestRequestTypeDef](./type_defs.md#createaccessentryrequestrequesttypedef)
- [UpgradePolicyRequestTypeDef](./type_defs.md#upgradepolicyrequesttypedef)
- [VpcConfigRequestTypeDef](./type_defs.md#vpcconfigrequesttypedef)
- [ZonalShiftConfigRequestTypeDef](./type_defs.md#zonalshiftconfigrequesttypedef)
- [EksAnywhereSubscriptionTermTypeDef](./type_defs.md#eksanywheresubscriptiontermtypedef)
- [LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef)
- [NodeRepairConfigTypeDef](./type_defs.md#noderepairconfigtypedef)
- [NodegroupScalingConfigTypeDef](./type_defs.md#nodegroupscalingconfigtypedef)
- [NodegroupUpdateConfigTypeDef](./type_defs.md#nodegroupupdateconfigtypedef)
- [RemoteAccessConfigTypeDef](./type_defs.md#remoteaccessconfigtypedef)
- [TaintTypeDef](./type_defs.md#tainttypedef)
- [CreatePodIdentityAssociationRequestRequestTypeDef](./type_defs.md#createpodidentityassociationrequestrequesttypedef)
- [PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef)
- [DeleteAccessEntryRequestRequestTypeDef](./type_defs.md#deleteaccessentryrequestrequesttypedef)
- [DeleteAddonRequestRequestTypeDef](./type_defs.md#deleteaddonrequestrequesttypedef)
- [DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef)
- [DeleteEksAnywhereSubscriptionRequestRequestTypeDef](./type_defs.md#deleteeksanywheresubscriptionrequestrequesttypedef)
- [DeleteFargateProfileRequestRequestTypeDef](./type_defs.md#deletefargateprofilerequestrequesttypedef)
- [DeleteNodegroupRequestRequestTypeDef](./type_defs.md#deletenodegrouprequestrequesttypedef)
- [DeletePodIdentityAssociationRequestRequestTypeDef](./type_defs.md#deletepodidentityassociationrequestrequesttypedef)
- [DeregisterClusterRequestRequestTypeDef](./type_defs.md#deregisterclusterrequestrequesttypedef)
- [DescribeAccessEntryRequestRequestTypeDef](./type_defs.md#describeaccessentryrequestrequesttypedef)
- [DescribeAddonConfigurationRequestRequestTypeDef](./type_defs.md#describeaddonconfigurationrequestrequesttypedef)
- [DescribeAddonRequestRequestTypeDef](./type_defs.md#describeaddonrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeAddonVersionsRequestRequestTypeDef](./type_defs.md#describeaddonversionsrequestrequesttypedef)
- [DescribeClusterRequestRequestTypeDef](./type_defs.md#describeclusterrequestrequesttypedef)
- [DescribeClusterVersionsRequestRequestTypeDef](./type_defs.md#describeclusterversionsrequestrequesttypedef)
- [DescribeEksAnywhereSubscriptionRequestRequestTypeDef](./type_defs.md#describeeksanywheresubscriptionrequestrequesttypedef)
- [DescribeFargateProfileRequestRequestTypeDef](./type_defs.md#describefargateprofilerequestrequesttypedef)
- [IdentityProviderConfigTypeDef](./type_defs.md#identityproviderconfigtypedef)
- [DescribeInsightRequestRequestTypeDef](./type_defs.md#describeinsightrequestrequesttypedef)
- [DescribeNodegroupRequestRequestTypeDef](./type_defs.md#describenodegrouprequestrequesttypedef)
- [DescribePodIdentityAssociationRequestRequestTypeDef](./type_defs.md#describepodidentityassociationrequestrequesttypedef)
- [DescribeUpdateRequestRequestTypeDef](./type_defs.md#describeupdaterequestrequesttypedef)
- [DisassociateAccessPolicyRequestRequestTypeDef](./type_defs.md#disassociateaccesspolicyrequestrequesttypedef)
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
- [ListAccessEntriesRequestRequestTypeDef](./type_defs.md#listaccessentriesrequestrequesttypedef)
- [ListAccessPoliciesRequestRequestTypeDef](./type_defs.md#listaccesspoliciesrequestrequesttypedef)
- [ListAddonsRequestRequestTypeDef](./type_defs.md#listaddonsrequestrequesttypedef)
- [ListAssociatedAccessPoliciesRequestRequestTypeDef](./type_defs.md#listassociatedaccesspoliciesrequestrequesttypedef)
- [ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef)
- [ListEksAnywhereSubscriptionsRequestRequestTypeDef](./type_defs.md#listeksanywheresubscriptionsrequestrequesttypedef)
- [ListFargateProfilesRequestRequestTypeDef](./type_defs.md#listfargateprofilesrequestrequesttypedef)
- [ListIdentityProviderConfigsRequestRequestTypeDef](./type_defs.md#listidentityproviderconfigsrequestrequesttypedef)
- [ListNodegroupsRequestRequestTypeDef](./type_defs.md#listnodegroupsrequestrequesttypedef)
- [ListPodIdentityAssociationsRequestRequestTypeDef](./type_defs.md#listpodidentityassociationsrequestrequesttypedef)
- [PodIdentityAssociationSummaryTypeDef](./type_defs.md#podidentityassociationsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListUpdatesRequestRequestTypeDef](./type_defs.md#listupdatesrequestrequesttypedef)
- [LogSetupOutputTypeDef](./type_defs.md#logsetupoutputtypedef)
- [LogSetupTypeDef](./type_defs.md#logsetuptypedef)
- [RemoteAccessConfigOutputTypeDef](./type_defs.md#remoteaccessconfigoutputtypedef)
- [RemoteNodeNetworkOutputTypeDef](./type_defs.md#remotenodenetworkoutputtypedef)
- [RemotePodNetworkOutputTypeDef](./type_defs.md#remotepodnetworkoutputtypedef)
- [RemoteNodeNetworkTypeDef](./type_defs.md#remotenodenetworktypedef)
- [RemotePodNetworkTypeDef](./type_defs.md#remotepodnetworktypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAccessConfigRequestTypeDef](./type_defs.md#updateaccessconfigrequesttypedef)
- [UpdateAccessEntryRequestRequestTypeDef](./type_defs.md#updateaccessentryrequestrequesttypedef)
- [UpdateClusterVersionRequestRequestTypeDef](./type_defs.md#updateclusterversionrequestrequesttypedef)
- [UpdateEksAnywhereSubscriptionRequestRequestTypeDef](./type_defs.md#updateeksanywheresubscriptionrequestrequesttypedef)
- [UpdateLabelsPayloadTypeDef](./type_defs.md#updatelabelspayloadtypedef)
- [UpdateParamTypeDef](./type_defs.md#updateparamtypedef)
- [UpdatePodIdentityAssociationRequestRequestTypeDef](./type_defs.md#updatepodidentityassociationrequestrequesttypedef)
- [AssociatedAccessPolicyTypeDef](./type_defs.md#associatedaccesspolicytypedef)
- [AssociateAccessPolicyRequestRequestTypeDef](./type_defs.md#associateaccesspolicyrequestrequesttypedef)
- [AddonHealthTypeDef](./type_defs.md#addonhealthtypedef)
- [CreateAddonRequestRequestTypeDef](./type_defs.md#createaddonrequestrequesttypedef)
- [UpdateAddonRequestRequestTypeDef](./type_defs.md#updateaddonrequestrequesttypedef)
- [AddonVersionInfoTypeDef](./type_defs.md#addonversioninfotypedef)
- [CreateAccessEntryResponseTypeDef](./type_defs.md#createaccessentryresponsetypedef)
- [DescribeAccessEntryResponseTypeDef](./type_defs.md#describeaccessentryresponsetypedef)
- [DescribeAddonConfigurationResponseTypeDef](./type_defs.md#describeaddonconfigurationresponsetypedef)
- [ListAccessEntriesResponseTypeDef](./type_defs.md#listaccessentriesresponsetypedef)
- [ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef)
- [ListAddonsResponseTypeDef](./type_defs.md#listaddonsresponsetypedef)
- [ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)
- [ListFargateProfilesResponseTypeDef](./type_defs.md#listfargateprofilesresponsetypedef)
- [ListNodegroupsResponseTypeDef](./type_defs.md#listnodegroupsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListUpdatesResponseTypeDef](./type_defs.md#listupdatesresponsetypedef)
- [UpdateAccessEntryResponseTypeDef](./type_defs.md#updateaccessentryresponsetypedef)
- [AssociateIdentityProviderConfigRequestRequestTypeDef](./type_defs.md#associateidentityproviderconfigrequestrequesttypedef)
- [NodegroupResourcesTypeDef](./type_defs.md#nodegroupresourcestypedef)
- [StorageConfigRequestTypeDef](./type_defs.md#storageconfigrequesttypedef)
- [StorageConfigResponseTypeDef](./type_defs.md#storageconfigresponsetypedef)
- [DeprecationDetailTypeDef](./type_defs.md#deprecationdetailtypedef)
- [ClusterHealthTypeDef](./type_defs.md#clusterhealthtypedef)
- [DescribeClusterVersionsResponseTypeDef](./type_defs.md#describeclusterversionsresponsetypedef)
- [RegisterClusterRequestRequestTypeDef](./type_defs.md#registerclusterrequestrequesttypedef)
- [OutpostConfigRequestTypeDef](./type_defs.md#outpostconfigrequesttypedef)
- [OutpostConfigResponseTypeDef](./type_defs.md#outpostconfigresponsetypedef)
- [CreateEksAnywhereSubscriptionRequestRequestTypeDef](./type_defs.md#createeksanywheresubscriptionrequestrequesttypedef)
- [EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef)
- [UpdateNodegroupVersionRequestRequestTypeDef](./type_defs.md#updatenodegroupversionrequestrequesttypedef)
- [CreateNodegroupRequestRequestTypeDef](./type_defs.md#createnodegrouprequestrequesttypedef)
- [UpdateTaintsPayloadTypeDef](./type_defs.md#updatetaintspayloadtypedef)
- [CreatePodIdentityAssociationResponseTypeDef](./type_defs.md#createpodidentityassociationresponsetypedef)
- [DeletePodIdentityAssociationResponseTypeDef](./type_defs.md#deletepodidentityassociationresponsetypedef)
- [DescribePodIdentityAssociationResponseTypeDef](./type_defs.md#describepodidentityassociationresponsetypedef)
- [UpdatePodIdentityAssociationResponseTypeDef](./type_defs.md#updatepodidentityassociationresponsetypedef)
- [DescribeAddonRequestWaitTypeDef](./type_defs.md#describeaddonrequestwaittypedef)
- [DescribeClusterRequestWaitTypeDef](./type_defs.md#describeclusterrequestwaittypedef)
- [DescribeFargateProfileRequestWaitTypeDef](./type_defs.md#describefargateprofilerequestwaittypedef)
- [DescribeNodegroupRequestWaitTypeDef](./type_defs.md#describenodegrouprequestwaittypedef)
- [DescribeAddonVersionsRequestPaginateTypeDef](./type_defs.md#describeaddonversionsrequestpaginatetypedef)
- [DescribeClusterVersionsRequestPaginateTypeDef](./type_defs.md#describeclusterversionsrequestpaginatetypedef)
- [ListAccessEntriesRequestPaginateTypeDef](./type_defs.md#listaccessentriesrequestpaginatetypedef)
- [ListAccessPoliciesRequestPaginateTypeDef](./type_defs.md#listaccesspoliciesrequestpaginatetypedef)
- [ListAddonsRequestPaginateTypeDef](./type_defs.md#listaddonsrequestpaginatetypedef)
- [ListAssociatedAccessPoliciesRequestPaginateTypeDef](./type_defs.md#listassociatedaccesspoliciesrequestpaginatetypedef)
- [ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef)
- [ListEksAnywhereSubscriptionsRequestPaginateTypeDef](./type_defs.md#listeksanywheresubscriptionsrequestpaginatetypedef)
- [ListFargateProfilesRequestPaginateTypeDef](./type_defs.md#listfargateprofilesrequestpaginatetypedef)
- [ListIdentityProviderConfigsRequestPaginateTypeDef](./type_defs.md#listidentityproviderconfigsrequestpaginatetypedef)
- [ListNodegroupsRequestPaginateTypeDef](./type_defs.md#listnodegroupsrequestpaginatetypedef)
- [ListPodIdentityAssociationsRequestPaginateTypeDef](./type_defs.md#listpodidentityassociationsrequestpaginatetypedef)
- [ListUpdatesRequestPaginateTypeDef](./type_defs.md#listupdatesrequestpaginatetypedef)
- [DescribeIdentityProviderConfigRequestRequestTypeDef](./type_defs.md#describeidentityproviderconfigrequestrequesttypedef)
- [DisassociateIdentityProviderConfigRequestRequestTypeDef](./type_defs.md#disassociateidentityproviderconfigrequestrequesttypedef)
- [ListIdentityProviderConfigsResponseTypeDef](./type_defs.md#listidentityproviderconfigsresponsetypedef)
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
- [ListInsightsRequestRequestTypeDef](./type_defs.md#listinsightsrequestrequesttypedef)
- [NodegroupHealthTypeDef](./type_defs.md#nodegrouphealthtypedef)
- [ListPodIdentityAssociationsResponseTypeDef](./type_defs.md#listpodidentityassociationsresponsetypedef)
- [LoggingOutputTypeDef](./type_defs.md#loggingoutputtypedef)
- [LogSetupUnionTypeDef](./type_defs.md#logsetupuniontypedef)
- [RemoteNetworkConfigResponseTypeDef](./type_defs.md#remotenetworkconfigresponsetypedef)
- [RemoteNodeNetworkUnionTypeDef](./type_defs.md#remotenodenetworkuniontypedef)
- [RemotePodNetworkUnionTypeDef](./type_defs.md#remotepodnetworkuniontypedef)
- [UpdateTypeDef](./type_defs.md#updatetypedef)
- [AssociateAccessPolicyResponseTypeDef](./type_defs.md#associateaccesspolicyresponsetypedef)
- [ListAssociatedAccessPoliciesResponseTypeDef](./type_defs.md#listassociatedaccesspoliciesresponsetypedef)
- [AddonTypeDef](./type_defs.md#addontypedef)
- [AddonInfoTypeDef](./type_defs.md#addoninfotypedef)
- [InsightCategorySpecificSummaryTypeDef](./type_defs.md#insightcategoryspecificsummarytypedef)
- [CreateEksAnywhereSubscriptionResponseTypeDef](./type_defs.md#createeksanywheresubscriptionresponsetypedef)
- [DeleteEksAnywhereSubscriptionResponseTypeDef](./type_defs.md#deleteeksanywheresubscriptionresponsetypedef)
- [DescribeEksAnywhereSubscriptionResponseTypeDef](./type_defs.md#describeeksanywheresubscriptionresponsetypedef)
- [ListEksAnywhereSubscriptionsResponseTypeDef](./type_defs.md#listeksanywheresubscriptionsresponsetypedef)
- [UpdateEksAnywhereSubscriptionResponseTypeDef](./type_defs.md#updateeksanywheresubscriptionresponsetypedef)
- [UpdateNodegroupConfigRequestRequestTypeDef](./type_defs.md#updatenodegroupconfigrequestrequesttypedef)
- [EncryptionConfigUnionTypeDef](./type_defs.md#encryptionconfiguniontypedef)
- [FargateProfileTypeDef](./type_defs.md#fargateprofiletypedef)
- [CreateFargateProfileRequestRequestTypeDef](./type_defs.md#createfargateprofilerequestrequesttypedef)
- [DescribeIdentityProviderConfigResponseTypeDef](./type_defs.md#describeidentityproviderconfigresponsetypedef)
- [ListInsightsResponseTypeDef](./type_defs.md#listinsightsresponsetypedef)
- [NodegroupTypeDef](./type_defs.md#nodegrouptypedef)
- [LoggingTypeDef](./type_defs.md#loggingtypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [RemoteNetworkConfigRequestTypeDef](./type_defs.md#remotenetworkconfigrequesttypedef)
- [AssociateEncryptionConfigResponseTypeDef](./type_defs.md#associateencryptionconfigresponsetypedef)
- [AssociateIdentityProviderConfigResponseTypeDef](./type_defs.md#associateidentityproviderconfigresponsetypedef)
- [DescribeUpdateResponseTypeDef](./type_defs.md#describeupdateresponsetypedef)
- [DisassociateIdentityProviderConfigResponseTypeDef](./type_defs.md#disassociateidentityproviderconfigresponsetypedef)
- [UpdateAddonResponseTypeDef](./type_defs.md#updateaddonresponsetypedef)
- [UpdateClusterConfigResponseTypeDef](./type_defs.md#updateclusterconfigresponsetypedef)
- [UpdateClusterVersionResponseTypeDef](./type_defs.md#updateclusterversionresponsetypedef)
- [UpdateNodegroupConfigResponseTypeDef](./type_defs.md#updatenodegroupconfigresponsetypedef)
- [UpdateNodegroupVersionResponseTypeDef](./type_defs.md#updatenodegroupversionresponsetypedef)
- [CreateAddonResponseTypeDef](./type_defs.md#createaddonresponsetypedef)
- [DeleteAddonResponseTypeDef](./type_defs.md#deleteaddonresponsetypedef)
- [DescribeAddonResponseTypeDef](./type_defs.md#describeaddonresponsetypedef)
- [DescribeAddonVersionsResponseTypeDef](./type_defs.md#describeaddonversionsresponsetypedef)
- [InsightTypeDef](./type_defs.md#insighttypedef)
- [AssociateEncryptionConfigRequestRequestTypeDef](./type_defs.md#associateencryptionconfigrequestrequesttypedef)
- [CreateFargateProfileResponseTypeDef](./type_defs.md#createfargateprofileresponsetypedef)
- [DeleteFargateProfileResponseTypeDef](./type_defs.md#deletefargateprofileresponsetypedef)
- [DescribeFargateProfileResponseTypeDef](./type_defs.md#describefargateprofileresponsetypedef)
- [CreateNodegroupResponseTypeDef](./type_defs.md#createnodegroupresponsetypedef)
- [DeleteNodegroupResponseTypeDef](./type_defs.md#deletenodegroupresponsetypedef)
- [DescribeNodegroupResponseTypeDef](./type_defs.md#describenodegroupresponsetypedef)
- [UpdateClusterConfigRequestRequestTypeDef](./type_defs.md#updateclusterconfigrequestrequesttypedef)
- [CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)
- [DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef)
- [DeregisterClusterResponseTypeDef](./type_defs.md#deregisterclusterresponsetypedef)
- [DescribeClusterResponseTypeDef](./type_defs.md#describeclusterresponsetypedef)
- [RegisterClusterResponseTypeDef](./type_defs.md#registerclusterresponsetypedef)
- [CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef)
- [DescribeInsightResponseTypeDef](./type_defs.md#describeinsightresponsetypedef)

