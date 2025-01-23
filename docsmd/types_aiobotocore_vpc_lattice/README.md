# VPCLattice module

> [Index](../README.md) > VPCLattice


!!! note ""

    Auto-generated documentation for [VPCLattice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#vpclattice)
    type annotations stubs module [types-aiobotocore-vpc-lattice](https://pypi.org/project/types-aiobotocore-vpc-lattice/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `VPCLattice` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `VPCLattice` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[vpc-lattice]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[vpc-lattice]'

# standalone installation
python -m pip install types-aiobotocore-vpc-lattice
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-vpc-lattice
```

## Usage

Code samples can be found in [Examples](./usage.md).

## VPCLatticeClient

Type annotations and code completion for  `#!python session.create_client("vpc-lattice")` as [VPCLatticeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client)

```python
# VPCLatticeClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_vpc_lattice.client import VPCLatticeClient


session = get_session()
async with session.create_client("vpc-lattice") as client:
    client: VPCLatticeClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("vpc-lattice").get_paginator("...")`.

```python
# ListAccessLogSubscriptionsPaginator usage example

from types_aiobotocore_vpc_lattice.paginator import ListAccessLogSubscriptionsPaginator

def get_list_access_log_subscriptions_paginator() -> ListAccessLogSubscriptionsPaginator:
    return client.get_paginator("list_access_log_subscriptions"))
```

- [ListAccessLogSubscriptionsPaginator](./paginators.md#listaccesslogsubscriptionspaginator)
- [ListListenersPaginator](./paginators.md#listlistenerspaginator)
- [ListResourceConfigurationsPaginator](./paginators.md#listresourceconfigurationspaginator)
- [ListResourceEndpointAssociationsPaginator](./paginators.md#listresourceendpointassociationspaginator)
- [ListResourceGatewaysPaginator](./paginators.md#listresourcegatewayspaginator)
- [ListRulesPaginator](./paginators.md#listrulespaginator)
- [ListServiceNetworkResourceAssociationsPaginator](./paginators.md#listservicenetworkresourceassociationspaginator)
- [ListServiceNetworkServiceAssociationsPaginator](./paginators.md#listservicenetworkserviceassociationspaginator)
- [ListServiceNetworkVpcAssociationsPaginator](./paginators.md#listservicenetworkvpcassociationspaginator)
- [ListServiceNetworkVpcEndpointAssociationsPaginator](./paginators.md#listservicenetworkvpcendpointassociationspaginator)
- [ListServiceNetworksPaginator](./paginators.md#listservicenetworkspaginator)
- [ListServicesPaginator](./paginators.md#listservicespaginator)
- [ListTargetGroupsPaginator](./paginators.md#listtargetgroupspaginator)
- [ListTargetsPaginator](./paginators.md#listtargetspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AuthPolicyStateType usage example

from types_aiobotocore_vpc_lattice.literals import AuthPolicyStateType

def get_value() -> AuthPolicyStateType:
    return "Active"
```

- [AuthPolicyStateType](./literals.md#authpolicystatetype)
- [AuthTypeType](./literals.md#authtypetype)
- [HealthCheckProtocolVersionType](./literals.md#healthcheckprotocolversiontype)
- [IpAddressTypeType](./literals.md#ipaddresstypetype)
- [LambdaEventStructureVersionType](./literals.md#lambdaeventstructureversiontype)
- [ListAccessLogSubscriptionsPaginatorName](./literals.md#listaccesslogsubscriptionspaginatorname)
- [ListListenersPaginatorName](./literals.md#listlistenerspaginatorname)
- [ListResourceConfigurationsPaginatorName](./literals.md#listresourceconfigurationspaginatorname)
- [ListResourceEndpointAssociationsPaginatorName](./literals.md#listresourceendpointassociationspaginatorname)
- [ListResourceGatewaysPaginatorName](./literals.md#listresourcegatewayspaginatorname)
- [ListRulesPaginatorName](./literals.md#listrulespaginatorname)
- [ListServiceNetworkResourceAssociationsPaginatorName](./literals.md#listservicenetworkresourceassociationspaginatorname)
- [ListServiceNetworkServiceAssociationsPaginatorName](./literals.md#listservicenetworkserviceassociationspaginatorname)
- [ListServiceNetworkVpcAssociationsPaginatorName](./literals.md#listservicenetworkvpcassociationspaginatorname)
- [ListServiceNetworkVpcEndpointAssociationsPaginatorName](./literals.md#listservicenetworkvpcendpointassociationspaginatorname)
- [ListServiceNetworksPaginatorName](./literals.md#listservicenetworkspaginatorname)
- [ListServicesPaginatorName](./literals.md#listservicespaginatorname)
- [ListTargetGroupsPaginatorName](./literals.md#listtargetgroupspaginatorname)
- [ListTargetsPaginatorName](./literals.md#listtargetspaginatorname)
- [ListenerProtocolType](./literals.md#listenerprotocoltype)
- [ProtocolTypeType](./literals.md#protocoltypetype)
- [ResourceConfigurationIpAddressTypeType](./literals.md#resourceconfigurationipaddresstypetype)
- [ResourceConfigurationStatusType](./literals.md#resourceconfigurationstatustype)
- [ResourceConfigurationTypeType](./literals.md#resourceconfigurationtypetype)
- [ResourceGatewayIpAddressTypeType](./literals.md#resourcegatewayipaddresstypetype)
- [ResourceGatewayStatusType](./literals.md#resourcegatewaystatustype)
- [ServiceNetworkLogTypeType](./literals.md#servicenetworklogtypetype)
- [ServiceNetworkResourceAssociationStatusType](./literals.md#servicenetworkresourceassociationstatustype)
- [ServiceNetworkServiceAssociationStatusType](./literals.md#servicenetworkserviceassociationstatustype)
- [ServiceNetworkVpcAssociationStatusType](./literals.md#servicenetworkvpcassociationstatustype)
- [ServiceStatusType](./literals.md#servicestatustype)
- [TargetGroupProtocolType](./literals.md#targetgroupprotocoltype)
- [TargetGroupProtocolVersionType](./literals.md#targetgroupprotocolversiontype)
- [TargetGroupStatusType](./literals.md#targetgroupstatustype)
- [TargetGroupTypeType](./literals.md#targetgrouptypetype)
- [TargetStatusType](./literals.md#targetstatustype)
- [VPCLatticeServiceName](./literals.md#vpclatticeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessLogSubscriptionSummaryTypeDef](./type_defs.md#accesslogsubscriptionsummarytypedef)
- [ArnResourceTypeDef](./type_defs.md#arnresourcetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [RuleUpdateFailureTypeDef](./type_defs.md#ruleupdatefailuretypedef)
- [CreateAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#createaccesslogsubscriptionrequestrequesttypedef)
- [CreateResourceGatewayRequestRequestTypeDef](./type_defs.md#createresourcegatewayrequestrequesttypedef)
- [SharingConfigTypeDef](./type_defs.md#sharingconfigtypedef)
- [CreateServiceNetworkResourceAssociationRequestRequestTypeDef](./type_defs.md#createservicenetworkresourceassociationrequestrequesttypedef)
- [CreateServiceNetworkServiceAssociationRequestRequestTypeDef](./type_defs.md#createservicenetworkserviceassociationrequestrequesttypedef)
- [DnsEntryTypeDef](./type_defs.md#dnsentrytypedef)
- [CreateServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#createservicenetworkvpcassociationrequestrequesttypedef)
- [CreateServiceRequestRequestTypeDef](./type_defs.md#createservicerequestrequesttypedef)
- [DeleteAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#deleteaccesslogsubscriptionrequestrequesttypedef)
- [DeleteAuthPolicyRequestRequestTypeDef](./type_defs.md#deleteauthpolicyrequestrequesttypedef)
- [DeleteListenerRequestRequestTypeDef](./type_defs.md#deletelistenerrequestrequesttypedef)
- [DeleteResourceConfigurationRequestRequestTypeDef](./type_defs.md#deleteresourceconfigurationrequestrequesttypedef)
- [DeleteResourceEndpointAssociationRequestRequestTypeDef](./type_defs.md#deleteresourceendpointassociationrequestrequesttypedef)
- [DeleteResourceGatewayRequestRequestTypeDef](./type_defs.md#deleteresourcegatewayrequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef)
- [DeleteServiceNetworkRequestRequestTypeDef](./type_defs.md#deleteservicenetworkrequestrequesttypedef)
- [DeleteServiceNetworkResourceAssociationRequestRequestTypeDef](./type_defs.md#deleteservicenetworkresourceassociationrequestrequesttypedef)
- [DeleteServiceNetworkServiceAssociationRequestRequestTypeDef](./type_defs.md#deleteservicenetworkserviceassociationrequestrequesttypedef)
- [DeleteServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#deleteservicenetworkvpcassociationrequestrequesttypedef)
- [DeleteServiceRequestRequestTypeDef](./type_defs.md#deleteservicerequestrequesttypedef)
- [DeleteTargetGroupRequestRequestTypeDef](./type_defs.md#deletetargetgrouprequestrequesttypedef)
- [TargetTypeDef](./type_defs.md#targettypedef)
- [TargetFailureTypeDef](./type_defs.md#targetfailuretypedef)
- [DnsResourceTypeDef](./type_defs.md#dnsresourcetypedef)
- [FixedResponseActionTypeDef](./type_defs.md#fixedresponseactiontypedef)
- [WeightedTargetGroupTypeDef](./type_defs.md#weightedtargetgrouptypedef)
- [GetAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#getaccesslogsubscriptionrequestrequesttypedef)
- [GetAuthPolicyRequestRequestTypeDef](./type_defs.md#getauthpolicyrequestrequesttypedef)
- [GetListenerRequestRequestTypeDef](./type_defs.md#getlistenerrequestrequesttypedef)
- [GetResourceConfigurationRequestRequestTypeDef](./type_defs.md#getresourceconfigurationrequestrequesttypedef)
- [GetResourceGatewayRequestRequestTypeDef](./type_defs.md#getresourcegatewayrequestrequesttypedef)
- [GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef)
- [GetRuleRequestRequestTypeDef](./type_defs.md#getrulerequestrequesttypedef)
- [GetServiceNetworkRequestRequestTypeDef](./type_defs.md#getservicenetworkrequestrequesttypedef)
- [GetServiceNetworkResourceAssociationRequestRequestTypeDef](./type_defs.md#getservicenetworkresourceassociationrequestrequesttypedef)
- [GetServiceNetworkServiceAssociationRequestRequestTypeDef](./type_defs.md#getservicenetworkserviceassociationrequestrequesttypedef)
- [GetServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#getservicenetworkvpcassociationrequestrequesttypedef)
- [GetServiceRequestRequestTypeDef](./type_defs.md#getservicerequestrequesttypedef)
- [GetTargetGroupRequestRequestTypeDef](./type_defs.md#gettargetgrouprequestrequesttypedef)
- [HeaderMatchTypeTypeDef](./type_defs.md#headermatchtypetypedef)
- [MatcherTypeDef](./type_defs.md#matchertypedef)
- [IpResourceTypeDef](./type_defs.md#ipresourcetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAccessLogSubscriptionsRequestRequestTypeDef](./type_defs.md#listaccesslogsubscriptionsrequestrequesttypedef)
- [ListListenersRequestRequestTypeDef](./type_defs.md#listlistenersrequestrequesttypedef)
- [ListenerSummaryTypeDef](./type_defs.md#listenersummarytypedef)
- [ListResourceConfigurationsRequestRequestTypeDef](./type_defs.md#listresourceconfigurationsrequestrequesttypedef)
- [ResourceConfigurationSummaryTypeDef](./type_defs.md#resourceconfigurationsummarytypedef)
- [ListResourceEndpointAssociationsRequestRequestTypeDef](./type_defs.md#listresourceendpointassociationsrequestrequesttypedef)
- [ResourceEndpointAssociationSummaryTypeDef](./type_defs.md#resourceendpointassociationsummarytypedef)
- [ListResourceGatewaysRequestRequestTypeDef](./type_defs.md#listresourcegatewaysrequestrequesttypedef)
- [ResourceGatewaySummaryTypeDef](./type_defs.md#resourcegatewaysummarytypedef)
- [ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef)
- [RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef)
- [ListServiceNetworkResourceAssociationsRequestRequestTypeDef](./type_defs.md#listservicenetworkresourceassociationsrequestrequesttypedef)
- [ListServiceNetworkServiceAssociationsRequestRequestTypeDef](./type_defs.md#listservicenetworkserviceassociationsrequestrequesttypedef)
- [ListServiceNetworkVpcAssociationsRequestRequestTypeDef](./type_defs.md#listservicenetworkvpcassociationsrequestrequesttypedef)
- [ServiceNetworkVpcAssociationSummaryTypeDef](./type_defs.md#servicenetworkvpcassociationsummarytypedef)
- [ListServiceNetworkVpcEndpointAssociationsRequestRequestTypeDef](./type_defs.md#listservicenetworkvpcendpointassociationsrequestrequesttypedef)
- [ServiceNetworkEndpointAssociationTypeDef](./type_defs.md#servicenetworkendpointassociationtypedef)
- [ListServiceNetworksRequestRequestTypeDef](./type_defs.md#listservicenetworksrequestrequesttypedef)
- [ServiceNetworkSummaryTypeDef](./type_defs.md#servicenetworksummarytypedef)
- [ListServicesRequestRequestTypeDef](./type_defs.md#listservicesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTargetGroupsRequestRequestTypeDef](./type_defs.md#listtargetgroupsrequestrequesttypedef)
- [TargetGroupSummaryTypeDef](./type_defs.md#targetgroupsummarytypedef)
- [TargetSummaryTypeDef](./type_defs.md#targetsummarytypedef)
- [PathMatchTypeTypeDef](./type_defs.md#pathmatchtypetypedef)
- [PutAuthPolicyRequestRequestTypeDef](./type_defs.md#putauthpolicyrequestrequesttypedef)
- [PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#updateaccesslogsubscriptionrequestrequesttypedef)
- [UpdateResourceGatewayRequestRequestTypeDef](./type_defs.md#updateresourcegatewayrequestrequesttypedef)
- [UpdateServiceNetworkRequestRequestTypeDef](./type_defs.md#updateservicenetworkrequestrequesttypedef)
- [UpdateServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#updateservicenetworkvpcassociationrequestrequesttypedef)
- [UpdateServiceRequestRequestTypeDef](./type_defs.md#updateservicerequestrequesttypedef)
- [CreateAccessLogSubscriptionResponseTypeDef](./type_defs.md#createaccesslogsubscriptionresponsetypedef)
- [CreateResourceGatewayResponseTypeDef](./type_defs.md#createresourcegatewayresponsetypedef)
- [CreateServiceNetworkResourceAssociationResponseTypeDef](./type_defs.md#createservicenetworkresourceassociationresponsetypedef)
- [CreateServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#createservicenetworkvpcassociationresponsetypedef)
- [DeleteResourceEndpointAssociationResponseTypeDef](./type_defs.md#deleteresourceendpointassociationresponsetypedef)
- [DeleteResourceGatewayResponseTypeDef](./type_defs.md#deleteresourcegatewayresponsetypedef)
- [DeleteServiceNetworkResourceAssociationResponseTypeDef](./type_defs.md#deleteservicenetworkresourceassociationresponsetypedef)
- [DeleteServiceNetworkServiceAssociationResponseTypeDef](./type_defs.md#deleteservicenetworkserviceassociationresponsetypedef)
- [DeleteServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#deleteservicenetworkvpcassociationresponsetypedef)
- [DeleteServiceResponseTypeDef](./type_defs.md#deleteserviceresponsetypedef)
- [DeleteTargetGroupResponseTypeDef](./type_defs.md#deletetargetgroupresponsetypedef)
- [GetAccessLogSubscriptionResponseTypeDef](./type_defs.md#getaccesslogsubscriptionresponsetypedef)
- [GetAuthPolicyResponseTypeDef](./type_defs.md#getauthpolicyresponsetypedef)
- [GetResourceGatewayResponseTypeDef](./type_defs.md#getresourcegatewayresponsetypedef)
- [GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)
- [GetServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#getservicenetworkvpcassociationresponsetypedef)
- [ListAccessLogSubscriptionsResponseTypeDef](./type_defs.md#listaccesslogsubscriptionsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutAuthPolicyResponseTypeDef](./type_defs.md#putauthpolicyresponsetypedef)
- [UpdateAccessLogSubscriptionResponseTypeDef](./type_defs.md#updateaccesslogsubscriptionresponsetypedef)
- [UpdateResourceGatewayResponseTypeDef](./type_defs.md#updateresourcegatewayresponsetypedef)
- [UpdateServiceNetworkResponseTypeDef](./type_defs.md#updateservicenetworkresponsetypedef)
- [UpdateServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#updateservicenetworkvpcassociationresponsetypedef)
- [UpdateServiceResponseTypeDef](./type_defs.md#updateserviceresponsetypedef)
- [CreateServiceNetworkRequestRequestTypeDef](./type_defs.md#createservicenetworkrequestrequesttypedef)
- [CreateServiceNetworkResponseTypeDef](./type_defs.md#createservicenetworkresponsetypedef)
- [GetServiceNetworkResponseTypeDef](./type_defs.md#getservicenetworkresponsetypedef)
- [CreateServiceNetworkServiceAssociationResponseTypeDef](./type_defs.md#createservicenetworkserviceassociationresponsetypedef)
- [CreateServiceResponseTypeDef](./type_defs.md#createserviceresponsetypedef)
- [GetServiceNetworkResourceAssociationResponseTypeDef](./type_defs.md#getservicenetworkresourceassociationresponsetypedef)
- [GetServiceNetworkServiceAssociationResponseTypeDef](./type_defs.md#getservicenetworkserviceassociationresponsetypedef)
- [GetServiceResponseTypeDef](./type_defs.md#getserviceresponsetypedef)
- [ServiceNetworkResourceAssociationSummaryTypeDef](./type_defs.md#servicenetworkresourceassociationsummarytypedef)
- [ServiceNetworkServiceAssociationSummaryTypeDef](./type_defs.md#servicenetworkserviceassociationsummarytypedef)
- [ServiceSummaryTypeDef](./type_defs.md#servicesummarytypedef)
- [DeregisterTargetsRequestRequestTypeDef](./type_defs.md#deregistertargetsrequestrequesttypedef)
- [ListTargetsRequestRequestTypeDef](./type_defs.md#listtargetsrequestrequesttypedef)
- [RegisterTargetsRequestRequestTypeDef](./type_defs.md#registertargetsrequestrequesttypedef)
- [DeregisterTargetsResponseTypeDef](./type_defs.md#deregistertargetsresponsetypedef)
- [RegisterTargetsResponseTypeDef](./type_defs.md#registertargetsresponsetypedef)
- [ForwardActionOutputTypeDef](./type_defs.md#forwardactionoutputtypedef)
- [ForwardActionTypeDef](./type_defs.md#forwardactiontypedef)
- [HeaderMatchTypeDef](./type_defs.md#headermatchtypedef)
- [HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef)
- [ResourceConfigurationDefinitionTypeDef](./type_defs.md#resourceconfigurationdefinitiontypedef)
- [ListAccessLogSubscriptionsRequestPaginateTypeDef](./type_defs.md#listaccesslogsubscriptionsrequestpaginatetypedef)
- [ListListenersRequestPaginateTypeDef](./type_defs.md#listlistenersrequestpaginatetypedef)
- [ListResourceConfigurationsRequestPaginateTypeDef](./type_defs.md#listresourceconfigurationsrequestpaginatetypedef)
- [ListResourceEndpointAssociationsRequestPaginateTypeDef](./type_defs.md#listresourceendpointassociationsrequestpaginatetypedef)
- [ListResourceGatewaysRequestPaginateTypeDef](./type_defs.md#listresourcegatewaysrequestpaginatetypedef)
- [ListRulesRequestPaginateTypeDef](./type_defs.md#listrulesrequestpaginatetypedef)
- [ListServiceNetworkResourceAssociationsRequestPaginateTypeDef](./type_defs.md#listservicenetworkresourceassociationsrequestpaginatetypedef)
- [ListServiceNetworkServiceAssociationsRequestPaginateTypeDef](./type_defs.md#listservicenetworkserviceassociationsrequestpaginatetypedef)
- [ListServiceNetworkVpcAssociationsRequestPaginateTypeDef](./type_defs.md#listservicenetworkvpcassociationsrequestpaginatetypedef)
- [ListServiceNetworkVpcEndpointAssociationsRequestPaginateTypeDef](./type_defs.md#listservicenetworkvpcendpointassociationsrequestpaginatetypedef)
- [ListServiceNetworksRequestPaginateTypeDef](./type_defs.md#listservicenetworksrequestpaginatetypedef)
- [ListServicesRequestPaginateTypeDef](./type_defs.md#listservicesrequestpaginatetypedef)
- [ListTargetGroupsRequestPaginateTypeDef](./type_defs.md#listtargetgroupsrequestpaginatetypedef)
- [ListTargetsRequestPaginateTypeDef](./type_defs.md#listtargetsrequestpaginatetypedef)
- [ListListenersResponseTypeDef](./type_defs.md#listlistenersresponsetypedef)
- [ListResourceConfigurationsResponseTypeDef](./type_defs.md#listresourceconfigurationsresponsetypedef)
- [ListResourceEndpointAssociationsResponseTypeDef](./type_defs.md#listresourceendpointassociationsresponsetypedef)
- [ListResourceGatewaysResponseTypeDef](./type_defs.md#listresourcegatewaysresponsetypedef)
- [ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef)
- [ListServiceNetworkVpcAssociationsResponseTypeDef](./type_defs.md#listservicenetworkvpcassociationsresponsetypedef)
- [ListServiceNetworkVpcEndpointAssociationsResponseTypeDef](./type_defs.md#listservicenetworkvpcendpointassociationsresponsetypedef)
- [ListServiceNetworksResponseTypeDef](./type_defs.md#listservicenetworksresponsetypedef)
- [ListTargetGroupsResponseTypeDef](./type_defs.md#listtargetgroupsresponsetypedef)
- [ListTargetsResponseTypeDef](./type_defs.md#listtargetsresponsetypedef)
- [PathMatchTypeDef](./type_defs.md#pathmatchtypedef)
- [ListServiceNetworkResourceAssociationsResponseTypeDef](./type_defs.md#listservicenetworkresourceassociationsresponsetypedef)
- [ListServiceNetworkServiceAssociationsResponseTypeDef](./type_defs.md#listservicenetworkserviceassociationsresponsetypedef)
- [ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef)
- [RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef)
- [ForwardActionUnionTypeDef](./type_defs.md#forwardactionuniontypedef)
- [TargetGroupConfigTypeDef](./type_defs.md#targetgroupconfigtypedef)
- [UpdateTargetGroupRequestRequestTypeDef](./type_defs.md#updatetargetgrouprequestrequesttypedef)
- [CreateResourceConfigurationRequestRequestTypeDef](./type_defs.md#createresourceconfigurationrequestrequesttypedef)
- [CreateResourceConfigurationResponseTypeDef](./type_defs.md#createresourceconfigurationresponsetypedef)
- [GetResourceConfigurationResponseTypeDef](./type_defs.md#getresourceconfigurationresponsetypedef)
- [UpdateResourceConfigurationRequestRequestTypeDef](./type_defs.md#updateresourceconfigurationrequestrequesttypedef)
- [UpdateResourceConfigurationResponseTypeDef](./type_defs.md#updateresourceconfigurationresponsetypedef)
- [HttpMatchOutputTypeDef](./type_defs.md#httpmatchoutputtypedef)
- [HttpMatchTypeDef](./type_defs.md#httpmatchtypedef)
- [CreateListenerResponseTypeDef](./type_defs.md#createlistenerresponsetypedef)
- [GetListenerResponseTypeDef](./type_defs.md#getlistenerresponsetypedef)
- [UpdateListenerResponseTypeDef](./type_defs.md#updatelistenerresponsetypedef)
- [RuleActionTypeDef](./type_defs.md#ruleactiontypedef)
- [CreateTargetGroupRequestRequestTypeDef](./type_defs.md#createtargetgrouprequestrequesttypedef)
- [CreateTargetGroupResponseTypeDef](./type_defs.md#createtargetgroupresponsetypedef)
- [GetTargetGroupResponseTypeDef](./type_defs.md#gettargetgroupresponsetypedef)
- [UpdateTargetGroupResponseTypeDef](./type_defs.md#updatetargetgroupresponsetypedef)
- [RuleMatchOutputTypeDef](./type_defs.md#rulematchoutputtypedef)
- [HttpMatchUnionTypeDef](./type_defs.md#httpmatchuniontypedef)
- [CreateListenerRequestRequestTypeDef](./type_defs.md#createlistenerrequestrequesttypedef)
- [RuleActionUnionTypeDef](./type_defs.md#ruleactionuniontypedef)
- [UpdateListenerRequestRequestTypeDef](./type_defs.md#updatelistenerrequestrequesttypedef)
- [CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef)
- [GetRuleResponseTypeDef](./type_defs.md#getruleresponsetypedef)
- [RuleUpdateSuccessTypeDef](./type_defs.md#ruleupdatesuccesstypedef)
- [UpdateRuleResponseTypeDef](./type_defs.md#updateruleresponsetypedef)
- [RuleMatchTypeDef](./type_defs.md#rulematchtypedef)
- [BatchUpdateRuleResponseTypeDef](./type_defs.md#batchupdateruleresponsetypedef)
- [CreateRuleRequestRequestTypeDef](./type_defs.md#createrulerequestrequesttypedef)
- [RuleMatchUnionTypeDef](./type_defs.md#rulematchuniontypedef)
- [UpdateRuleRequestRequestTypeDef](./type_defs.md#updaterulerequestrequesttypedef)
- [RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef)
- [BatchUpdateRuleRequestRequestTypeDef](./type_defs.md#batchupdaterulerequestrequesttypedef)

