# VPCLattice module

> [Index](../README.md) > VPCLattice


!!! note ""

    Auto-generated documentation for [VPCLattice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
    type annotations stubs module [types-aiobotocore-vpc-lattice](https://pypi.org/project/types-aiobotocore-vpc-lattice/).

## How to install



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
- [ListRulesPaginator](./paginators.md#listrulespaginator)
- [ListServiceNetworkServiceAssociationsPaginator](./paginators.md#listservicenetworkserviceassociationspaginator)
- [ListServiceNetworkVpcAssociationsPaginator](./paginators.md#listservicenetworkvpcassociationspaginator)
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
- [ListAccessLogSubscriptionsPaginatorName](./literals.md#listaccesslogsubscriptionspaginatorname)
- [ListListenersPaginatorName](./literals.md#listlistenerspaginatorname)
- [ListRulesPaginatorName](./literals.md#listrulespaginatorname)
- [ListServiceNetworkServiceAssociationsPaginatorName](./literals.md#listservicenetworkserviceassociationspaginatorname)
- [ListServiceNetworkVpcAssociationsPaginatorName](./literals.md#listservicenetworkvpcassociationspaginatorname)
- [ListServiceNetworksPaginatorName](./literals.md#listservicenetworkspaginatorname)
- [ListServicesPaginatorName](./literals.md#listservicespaginatorname)
- [ListTargetGroupsPaginatorName](./literals.md#listtargetgroupspaginatorname)
- [ListTargetsPaginatorName](./literals.md#listtargetspaginatorname)
- [ListenerProtocolType](./literals.md#listenerprotocoltype)
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
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [RuleUpdateFailureTypeDef](./type_defs.md#ruleupdatefailuretypedef)
- [CreateAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#createaccesslogsubscriptionrequestrequesttypedef)
- [CreateServiceNetworkRequestRequestTypeDef](./type_defs.md#createservicenetworkrequestrequesttypedef)
- [CreateServiceNetworkServiceAssociationRequestRequestTypeDef](./type_defs.md#createservicenetworkserviceassociationrequestrequesttypedef)
- [DnsEntryTypeDef](./type_defs.md#dnsentrytypedef)
- [CreateServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#createservicenetworkvpcassociationrequestrequesttypedef)
- [CreateServiceRequestRequestTypeDef](./type_defs.md#createservicerequestrequesttypedef)
- [DeleteAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#deleteaccesslogsubscriptionrequestrequesttypedef)
- [DeleteAuthPolicyRequestRequestTypeDef](./type_defs.md#deleteauthpolicyrequestrequesttypedef)
- [DeleteListenerRequestRequestTypeDef](./type_defs.md#deletelistenerrequestrequesttypedef)
- [DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef)
- [DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef)
- [DeleteServiceNetworkRequestRequestTypeDef](./type_defs.md#deleteservicenetworkrequestrequesttypedef)
- [DeleteServiceNetworkServiceAssociationRequestRequestTypeDef](./type_defs.md#deleteservicenetworkserviceassociationrequestrequesttypedef)
- [DeleteServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#deleteservicenetworkvpcassociationrequestrequesttypedef)
- [DeleteServiceRequestRequestTypeDef](./type_defs.md#deleteservicerequestrequesttypedef)
- [DeleteTargetGroupRequestRequestTypeDef](./type_defs.md#deletetargetgrouprequestrequesttypedef)
- [TargetTypeDef](./type_defs.md#targettypedef)
- [TargetFailureTypeDef](./type_defs.md#targetfailuretypedef)
- [FixedResponseActionTypeDef](./type_defs.md#fixedresponseactiontypedef)
- [WeightedTargetGroupTypeDef](./type_defs.md#weightedtargetgrouptypedef)
- [GetAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#getaccesslogsubscriptionrequestrequesttypedef)
- [GetAuthPolicyRequestRequestTypeDef](./type_defs.md#getauthpolicyrequestrequesttypedef)
- [GetListenerRequestRequestTypeDef](./type_defs.md#getlistenerrequestrequesttypedef)
- [GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef)
- [GetRuleRequestRequestTypeDef](./type_defs.md#getrulerequestrequesttypedef)
- [GetServiceNetworkRequestRequestTypeDef](./type_defs.md#getservicenetworkrequestrequesttypedef)
- [GetServiceNetworkServiceAssociationRequestRequestTypeDef](./type_defs.md#getservicenetworkserviceassociationrequestrequesttypedef)
- [GetServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#getservicenetworkvpcassociationrequestrequesttypedef)
- [GetServiceRequestRequestTypeDef](./type_defs.md#getservicerequestrequesttypedef)
- [GetTargetGroupRequestRequestTypeDef](./type_defs.md#gettargetgrouprequestrequesttypedef)
- [HeaderMatchTypeTypeDef](./type_defs.md#headermatchtypetypedef)
- [MatcherTypeDef](./type_defs.md#matchertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAccessLogSubscriptionsRequestRequestTypeDef](./type_defs.md#listaccesslogsubscriptionsrequestrequesttypedef)
- [ListListenersRequestRequestTypeDef](./type_defs.md#listlistenersrequestrequesttypedef)
- [ListenerSummaryTypeDef](./type_defs.md#listenersummarytypedef)
- [ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef)
- [RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef)
- [ListServiceNetworkServiceAssociationsRequestRequestTypeDef](./type_defs.md#listservicenetworkserviceassociationsrequestrequesttypedef)
- [ListServiceNetworkVpcAssociationsRequestRequestTypeDef](./type_defs.md#listservicenetworkvpcassociationsrequestrequesttypedef)
- [ServiceNetworkVpcAssociationSummaryTypeDef](./type_defs.md#servicenetworkvpcassociationsummarytypedef)
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
- [UpdateServiceNetworkRequestRequestTypeDef](./type_defs.md#updateservicenetworkrequestrequesttypedef)
- [UpdateServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#updateservicenetworkvpcassociationrequestrequesttypedef)
- [UpdateServiceRequestRequestTypeDef](./type_defs.md#updateservicerequestrequesttypedef)
- [CreateAccessLogSubscriptionResponseTypeDef](./type_defs.md#createaccesslogsubscriptionresponsetypedef)
- [CreateServiceNetworkResponseTypeDef](./type_defs.md#createservicenetworkresponsetypedef)
- [CreateServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#createservicenetworkvpcassociationresponsetypedef)
- [DeleteServiceNetworkServiceAssociationResponseTypeDef](./type_defs.md#deleteservicenetworkserviceassociationresponsetypedef)
- [DeleteServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#deleteservicenetworkvpcassociationresponsetypedef)
- [DeleteServiceResponseTypeDef](./type_defs.md#deleteserviceresponsetypedef)
- [DeleteTargetGroupResponseTypeDef](./type_defs.md#deletetargetgroupresponsetypedef)
- [GetAccessLogSubscriptionResponseTypeDef](./type_defs.md#getaccesslogsubscriptionresponsetypedef)
- [GetAuthPolicyResponseTypeDef](./type_defs.md#getauthpolicyresponsetypedef)
- [GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)
- [GetServiceNetworkResponseTypeDef](./type_defs.md#getservicenetworkresponsetypedef)
- [GetServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#getservicenetworkvpcassociationresponsetypedef)
- [ListAccessLogSubscriptionsResponseTypeDef](./type_defs.md#listaccesslogsubscriptionsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutAuthPolicyResponseTypeDef](./type_defs.md#putauthpolicyresponsetypedef)
- [UpdateAccessLogSubscriptionResponseTypeDef](./type_defs.md#updateaccesslogsubscriptionresponsetypedef)
- [UpdateServiceNetworkResponseTypeDef](./type_defs.md#updateservicenetworkresponsetypedef)
- [UpdateServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#updateservicenetworkvpcassociationresponsetypedef)
- [UpdateServiceResponseTypeDef](./type_defs.md#updateserviceresponsetypedef)
- [CreateServiceNetworkServiceAssociationResponseTypeDef](./type_defs.md#createservicenetworkserviceassociationresponsetypedef)
- [CreateServiceResponseTypeDef](./type_defs.md#createserviceresponsetypedef)
- [GetServiceNetworkServiceAssociationResponseTypeDef](./type_defs.md#getservicenetworkserviceassociationresponsetypedef)
- [GetServiceResponseTypeDef](./type_defs.md#getserviceresponsetypedef)
- [ServiceNetworkServiceAssociationSummaryTypeDef](./type_defs.md#servicenetworkserviceassociationsummarytypedef)
- [ServiceSummaryTypeDef](./type_defs.md#servicesummarytypedef)
- [DeregisterTargetsRequestRequestTypeDef](./type_defs.md#deregistertargetsrequestrequesttypedef)
- [ListTargetsRequestRequestTypeDef](./type_defs.md#listtargetsrequestrequesttypedef)
- [RegisterTargetsRequestRequestTypeDef](./type_defs.md#registertargetsrequestrequesttypedef)
- [DeregisterTargetsResponseTypeDef](./type_defs.md#deregistertargetsresponsetypedef)
- [RegisterTargetsResponseTypeDef](./type_defs.md#registertargetsresponsetypedef)
- [ForwardActionTypeDef](./type_defs.md#forwardactiontypedef)
- [HeaderMatchTypeDef](./type_defs.md#headermatchtypedef)
- [HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef)
- [ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef](./type_defs.md#listaccesslogsubscriptionsrequestlistaccesslogsubscriptionspaginatetypedef)
- [ListListenersRequestListListenersPaginateTypeDef](./type_defs.md#listlistenersrequestlistlistenerspaginatetypedef)
- [ListRulesRequestListRulesPaginateTypeDef](./type_defs.md#listrulesrequestlistrulespaginatetypedef)
- [ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef](./type_defs.md#listservicenetworkserviceassociationsrequestlistservicenetworkserviceassociationspaginatetypedef)
- [ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef](./type_defs.md#listservicenetworkvpcassociationsrequestlistservicenetworkvpcassociationspaginatetypedef)
- [ListServiceNetworksRequestListServiceNetworksPaginateTypeDef](./type_defs.md#listservicenetworksrequestlistservicenetworkspaginatetypedef)
- [ListServicesRequestListServicesPaginateTypeDef](./type_defs.md#listservicesrequestlistservicespaginatetypedef)
- [ListTargetGroupsRequestListTargetGroupsPaginateTypeDef](./type_defs.md#listtargetgroupsrequestlisttargetgroupspaginatetypedef)
- [ListTargetsRequestListTargetsPaginateTypeDef](./type_defs.md#listtargetsrequestlisttargetspaginatetypedef)
- [ListListenersResponseTypeDef](./type_defs.md#listlistenersresponsetypedef)
- [ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef)
- [ListServiceNetworkVpcAssociationsResponseTypeDef](./type_defs.md#listservicenetworkvpcassociationsresponsetypedef)
- [ListServiceNetworksResponseTypeDef](./type_defs.md#listservicenetworksresponsetypedef)
- [ListTargetGroupsResponseTypeDef](./type_defs.md#listtargetgroupsresponsetypedef)
- [ListTargetsResponseTypeDef](./type_defs.md#listtargetsresponsetypedef)
- [PathMatchTypeDef](./type_defs.md#pathmatchtypedef)
- [ListServiceNetworkServiceAssociationsResponseTypeDef](./type_defs.md#listservicenetworkserviceassociationsresponsetypedef)
- [ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef)
- [RuleActionTypeDef](./type_defs.md#ruleactiontypedef)
- [TargetGroupConfigTypeDef](./type_defs.md#targetgroupconfigtypedef)
- [UpdateTargetGroupRequestRequestTypeDef](./type_defs.md#updatetargetgrouprequestrequesttypedef)
- [HttpMatchTypeDef](./type_defs.md#httpmatchtypedef)
- [CreateListenerRequestRequestTypeDef](./type_defs.md#createlistenerrequestrequesttypedef)
- [CreateListenerResponseTypeDef](./type_defs.md#createlistenerresponsetypedef)
- [GetListenerResponseTypeDef](./type_defs.md#getlistenerresponsetypedef)
- [UpdateListenerRequestRequestTypeDef](./type_defs.md#updatelistenerrequestrequesttypedef)
- [UpdateListenerResponseTypeDef](./type_defs.md#updatelistenerresponsetypedef)
- [CreateTargetGroupRequestRequestTypeDef](./type_defs.md#createtargetgrouprequestrequesttypedef)
- [CreateTargetGroupResponseTypeDef](./type_defs.md#createtargetgroupresponsetypedef)
- [GetTargetGroupResponseTypeDef](./type_defs.md#gettargetgroupresponsetypedef)
- [UpdateTargetGroupResponseTypeDef](./type_defs.md#updatetargetgroupresponsetypedef)
- [RuleMatchTypeDef](./type_defs.md#rulematchtypedef)
- [CreateRuleRequestRequestTypeDef](./type_defs.md#createrulerequestrequesttypedef)
- [CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef)
- [GetRuleResponseTypeDef](./type_defs.md#getruleresponsetypedef)
- [RuleUpdateSuccessTypeDef](./type_defs.md#ruleupdatesuccesstypedef)
- [RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef)
- [UpdateRuleRequestRequestTypeDef](./type_defs.md#updaterulerequestrequesttypedef)
- [UpdateRuleResponseTypeDef](./type_defs.md#updateruleresponsetypedef)
- [BatchUpdateRuleResponseTypeDef](./type_defs.md#batchupdateruleresponsetypedef)
- [BatchUpdateRuleRequestRequestTypeDef](./type_defs.md#batchupdaterulerequestrequesttypedef)

