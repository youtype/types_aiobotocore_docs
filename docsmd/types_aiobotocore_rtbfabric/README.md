# RTBFabric module

> [Index](../README.md) > RTBFabric


!!! note ""

    Auto-generated documentation for [RTBFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#rtbfabric)
    type annotations stubs module [types-aiobotocore-rtbfabric](https://pypi.org/project/types-aiobotocore-rtbfabric/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `RTBFabric` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `RTBFabric` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[rtbfabric]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[rtbfabric]'

# standalone installation
python -m pip install types-aiobotocore-rtbfabric
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-rtbfabric
```

## Usage

Code samples can be found in [Examples](./usage.md).

## RTBFabricClient

Type annotations and code completion for  `#!python session.create_client("rtbfabric")` as [RTBFabricClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#RTBFabric.Client)

```python
# RTBFabricClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_rtbfabric.client import RTBFabricClient


session = get_session()
async with session.create_client("rtbfabric") as client:
    client: RTBFabricClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("rtbfabric").get_paginator("...")`.

```python
# ListLinksPaginator usage example

from types_aiobotocore_rtbfabric.paginator import ListLinksPaginator

def get_list_links_paginator() -> ListLinksPaginator:
    return client.get_paginator("list_links"))
```

- [ListLinksPaginator](./paginators.md#listlinkspaginator)
- [ListRequesterGatewaysPaginator](./paginators.md#listrequestergatewayspaginator)
- [ListResponderGatewaysPaginator](./paginators.md#listrespondergatewayspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("rtbfabric").get_waiter("...")`.

```python
# InboundExternalLinkActiveWaiter usage example

from types_aiobotocore_rtbfabric.waiter import InboundExternalLinkActiveWaiter

def get_inbound_external_link_active_waiter() -> InboundExternalLinkActiveWaiter:
    return Session().client("rtbfabric").get_waiter("inbound_external_link_active")
```

- [InboundExternalLinkActiveWaiter](./waiters.md#inboundexternallinkactivewaiter)
- [LinkAcceptedWaiter](./waiters.md#linkacceptedwaiter)
- [LinkActiveWaiter](./waiters.md#linkactivewaiter)
- [OutboundExternalLinkActiveWaiter](./waiters.md#outboundexternallinkactivewaiter)
- [RequesterGatewayActiveWaiter](./waiters.md#requestergatewayactivewaiter)
- [RequesterGatewayDeletedWaiter](./waiters.md#requestergatewaydeletedwaiter)
- [ResponderGatewayActiveWaiter](./waiters.md#respondergatewayactivewaiter)
- [ResponderGatewayDeletedWaiter](./waiters.md#respondergatewaydeletedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# FilterTypeType usage example

from types_aiobotocore_rtbfabric.literals import FilterTypeType

def get_value() -> FilterTypeType:
    return "EXCLUDE"
```

- [FilterTypeType](./literals.md#filtertypetype)
- [InboundExternalLinkActiveWaiterName](./literals.md#inboundexternallinkactivewaitername)
- [LinkAcceptedWaiterName](./literals.md#linkacceptedwaitername)
- [LinkActiveWaiterName](./literals.md#linkactivewaitername)
- [LinkDirectionType](./literals.md#linkdirectiontype)
- [LinkStatusType](./literals.md#linkstatustype)
- [ListLinksPaginatorName](./literals.md#listlinkspaginatorname)
- [ListRequesterGatewaysPaginatorName](./literals.md#listrequestergatewayspaginatorname)
- [ListResponderGatewaysPaginatorName](./literals.md#listrespondergatewayspaginatorname)
- [OutboundExternalLinkActiveWaiterName](./literals.md#outboundexternallinkactivewaitername)
- [ProtocolType](./literals.md#protocoltype)
- [RequesterGatewayActiveWaiterName](./literals.md#requestergatewayactivewaitername)
- [RequesterGatewayDeletedWaiterName](./literals.md#requestergatewaydeletedwaitername)
- [RequesterGatewayStatusType](./literals.md#requestergatewaystatustype)
- [ResponderErrorMaskingActionType](./literals.md#respondererrormaskingactiontype)
- [ResponderErrorMaskingLoggingTypeType](./literals.md#respondererrormaskingloggingtypetype)
- [ResponderGatewayActiveWaiterName](./literals.md#respondergatewayactivewaitername)
- [ResponderGatewayDeletedWaiterName](./literals.md#respondergatewaydeletedwaitername)
- [ResponderGatewayStatusType](./literals.md#respondergatewaystatustype)
- [RTBFabricServiceName](./literals.md#rtbfabricservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [HeaderTagActionTypeDef](./type_defs.md#headertagactiontypedef)
- [NoBidActionTypeDef](./type_defs.md#nobidactiontypedef)
- [AutoScalingGroupsConfigurationOutputTypeDef](./type_defs.md#autoscalinggroupsconfigurationoutputtypedef)
- [AutoScalingGroupsConfigurationTypeDef](./type_defs.md#autoscalinggroupsconfigurationtypedef)
- [CreateRequesterGatewayRequestTypeDef](./type_defs.md#createrequestergatewayrequesttypedef)
- [DeleteInboundExternalLinkRequestTypeDef](./type_defs.md#deleteinboundexternallinkrequesttypedef)
- [DeleteLinkRequestTypeDef](./type_defs.md#deletelinkrequesttypedef)
- [DeleteOutboundExternalLinkRequestTypeDef](./type_defs.md#deleteoutboundexternallinkrequesttypedef)
- [DeleteRequesterGatewayRequestTypeDef](./type_defs.md#deleterequestergatewayrequesttypedef)
- [DeleteResponderGatewayRequestTypeDef](./type_defs.md#deleterespondergatewayrequesttypedef)
- [EksEndpointsConfigurationTypeDef](./type_defs.md#eksendpointsconfigurationtypedef)
- [FilterCriterionOutputTypeDef](./type_defs.md#filtercriterionoutputtypedef)
- [FilterCriterionTypeDef](./type_defs.md#filtercriteriontypedef)
- [GetInboundExternalLinkRequestTypeDef](./type_defs.md#getinboundexternallinkrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetLinkRequestTypeDef](./type_defs.md#getlinkrequesttypedef)
- [GetOutboundExternalLinkRequestTypeDef](./type_defs.md#getoutboundexternallinkrequesttypedef)
- [GetRequesterGatewayRequestTypeDef](./type_defs.md#getrequestergatewayrequesttypedef)
- [GetResponderGatewayRequestTypeDef](./type_defs.md#getrespondergatewayrequesttypedef)
- [TrustStoreConfigurationOutputTypeDef](./type_defs.md#truststoreconfigurationoutputtypedef)
- [LinkApplicationLogSamplingTypeDef](./type_defs.md#linkapplicationlogsamplingtypedef)
- [ResponderErrorMaskingForHttpCodeOutputTypeDef](./type_defs.md#respondererrormaskingforhttpcodeoutputtypedef)
- [ResponderErrorMaskingForHttpCodeTypeDef](./type_defs.md#respondererrormaskingforhttpcodetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListLinksRequestTypeDef](./type_defs.md#listlinksrequesttypedef)
- [ListRequesterGatewaysRequestTypeDef](./type_defs.md#listrequestergatewaysrequesttypedef)
- [ListResponderGatewaysRequestTypeDef](./type_defs.md#listrespondergatewaysrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [NoBidModuleParametersTypeDef](./type_defs.md#nobidmoduleparameterstypedef)
- [RateLimiterModuleParametersTypeDef](./type_defs.md#ratelimitermoduleparameterstypedef)
- [RejectLinkRequestTypeDef](./type_defs.md#rejectlinkrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [TrustStoreConfigurationTypeDef](./type_defs.md#truststoreconfigurationtypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateRequesterGatewayRequestTypeDef](./type_defs.md#updaterequestergatewayrequesttypedef)
- [CreateInboundExternalLinkResponseTypeDef](./type_defs.md#createinboundexternallinkresponsetypedef)
- [CreateOutboundExternalLinkResponseTypeDef](./type_defs.md#createoutboundexternallinkresponsetypedef)
- [CreateRequesterGatewayResponseTypeDef](./type_defs.md#createrequestergatewayresponsetypedef)
- [CreateResponderGatewayResponseTypeDef](./type_defs.md#createrespondergatewayresponsetypedef)
- [DeleteInboundExternalLinkResponseTypeDef](./type_defs.md#deleteinboundexternallinkresponsetypedef)
- [DeleteLinkResponseTypeDef](./type_defs.md#deletelinkresponsetypedef)
- [DeleteOutboundExternalLinkResponseTypeDef](./type_defs.md#deleteoutboundexternallinkresponsetypedef)
- [DeleteRequesterGatewayResponseTypeDef](./type_defs.md#deleterequestergatewayresponsetypedef)
- [DeleteResponderGatewayResponseTypeDef](./type_defs.md#deleterespondergatewayresponsetypedef)
- [GetRequesterGatewayResponseTypeDef](./type_defs.md#getrequestergatewayresponsetypedef)
- [ListRequesterGatewaysResponseTypeDef](./type_defs.md#listrequestergatewaysresponsetypedef)
- [ListResponderGatewaysResponseTypeDef](./type_defs.md#listrespondergatewaysresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateLinkModuleFlowResponseTypeDef](./type_defs.md#updatelinkmoduleflowresponsetypedef)
- [UpdateLinkResponseTypeDef](./type_defs.md#updatelinkresponsetypedef)
- [UpdateRequesterGatewayResponseTypeDef](./type_defs.md#updaterequestergatewayresponsetypedef)
- [UpdateResponderGatewayResponseTypeDef](./type_defs.md#updaterespondergatewayresponsetypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [ManagedEndpointConfigurationOutputTypeDef](./type_defs.md#managedendpointconfigurationoutputtypedef)
- [ManagedEndpointConfigurationTypeDef](./type_defs.md#managedendpointconfigurationtypedef)
- [FilterOutputTypeDef](./type_defs.md#filteroutputtypedef)
- [FilterCriterionUnionTypeDef](./type_defs.md#filtercriterionuniontypedef)
- [GetInboundExternalLinkRequestWaitTypeDef](./type_defs.md#getinboundexternallinkrequestwaittypedef)
- [GetLinkRequestWaitExtraTypeDef](./type_defs.md#getlinkrequestwaitextratypedef)
- [GetLinkRequestWaitTypeDef](./type_defs.md#getlinkrequestwaittypedef)
- [GetOutboundExternalLinkRequestWaitTypeDef](./type_defs.md#getoutboundexternallinkrequestwaittypedef)
- [GetRequesterGatewayRequestWaitExtraTypeDef](./type_defs.md#getrequestergatewayrequestwaitextratypedef)
- [GetRequesterGatewayRequestWaitTypeDef](./type_defs.md#getrequestergatewayrequestwaittypedef)
- [GetResponderGatewayRequestWaitExtraTypeDef](./type_defs.md#getrespondergatewayrequestwaitextratypedef)
- [GetResponderGatewayRequestWaitTypeDef](./type_defs.md#getrespondergatewayrequestwaittypedef)
- [LinkApplicationLogConfigurationTypeDef](./type_defs.md#linkapplicationlogconfigurationtypedef)
- [LinkAttributesOutputTypeDef](./type_defs.md#linkattributesoutputtypedef)
- [LinkAttributesTypeDef](./type_defs.md#linkattributestypedef)
- [ListLinksRequestPaginateTypeDef](./type_defs.md#listlinksrequestpaginatetypedef)
- [ListRequesterGatewaysRequestPaginateTypeDef](./type_defs.md#listrequestergatewaysrequestpaginatetypedef)
- [ListResponderGatewaysRequestPaginateTypeDef](./type_defs.md#listrespondergatewaysrequestpaginatetypedef)
- [TrustStoreConfigurationUnionTypeDef](./type_defs.md#truststoreconfigurationuniontypedef)
- [GetResponderGatewayResponseTypeDef](./type_defs.md#getrespondergatewayresponsetypedef)
- [ManagedEndpointConfigurationUnionTypeDef](./type_defs.md#managedendpointconfigurationuniontypedef)
- [OpenRtbAttributeModuleParametersOutputTypeDef](./type_defs.md#openrtbattributemoduleparametersoutputtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [LinkLogSettingsTypeDef](./type_defs.md#linklogsettingstypedef)
- [LinkAttributesUnionTypeDef](./type_defs.md#linkattributesuniontypedef)
- [CreateResponderGatewayRequestTypeDef](./type_defs.md#createrespondergatewayrequesttypedef)
- [UpdateResponderGatewayRequestTypeDef](./type_defs.md#updaterespondergatewayrequesttypedef)
- [ModuleParametersOutputTypeDef](./type_defs.md#moduleparametersoutputtypedef)
- [FilterUnionTypeDef](./type_defs.md#filteruniontypedef)
- [GetOutboundExternalLinkResponseTypeDef](./type_defs.md#getoutboundexternallinkresponsetypedef)
- [UpdateLinkRequestTypeDef](./type_defs.md#updatelinkrequesttypedef)
- [AcceptLinkRequestTypeDef](./type_defs.md#acceptlinkrequesttypedef)
- [CreateInboundExternalLinkRequestTypeDef](./type_defs.md#createinboundexternallinkrequesttypedef)
- [CreateLinkRequestTypeDef](./type_defs.md#createlinkrequesttypedef)
- [CreateOutboundExternalLinkRequestTypeDef](./type_defs.md#createoutboundexternallinkrequesttypedef)
- [ModuleConfigurationOutputTypeDef](./type_defs.md#moduleconfigurationoutputtypedef)
- [OpenRtbAttributeModuleParametersTypeDef](./type_defs.md#openrtbattributemoduleparameterstypedef)
- [AcceptLinkResponseTypeDef](./type_defs.md#acceptlinkresponsetypedef)
- [CreateLinkResponseTypeDef](./type_defs.md#createlinkresponsetypedef)
- [GetInboundExternalLinkResponseTypeDef](./type_defs.md#getinboundexternallinkresponsetypedef)
- [GetLinkResponseTypeDef](./type_defs.md#getlinkresponsetypedef)
- [ListLinksResponseStructureTypeDef](./type_defs.md#listlinksresponsestructuretypedef)
- [RejectLinkResponseTypeDef](./type_defs.md#rejectlinkresponsetypedef)
- [OpenRtbAttributeModuleParametersUnionTypeDef](./type_defs.md#openrtbattributemoduleparametersuniontypedef)
- [ListLinksResponseTypeDef](./type_defs.md#listlinksresponsetypedef)
- [ModuleParametersTypeDef](./type_defs.md#moduleparameterstypedef)
- [ModuleParametersUnionTypeDef](./type_defs.md#moduleparametersuniontypedef)
- [ModuleConfigurationTypeDef](./type_defs.md#moduleconfigurationtypedef)
- [ModuleConfigurationUnionTypeDef](./type_defs.md#moduleconfigurationuniontypedef)
- [UpdateLinkModuleFlowRequestTypeDef](./type_defs.md#updatelinkmoduleflowrequesttypedef)

