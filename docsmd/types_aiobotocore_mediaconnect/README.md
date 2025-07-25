# MediaConnect module

> [Index](../README.md) > MediaConnect


!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#mediaconnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.23.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MediaConnect` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MediaConnect` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[mediaconnect]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[mediaconnect]'

# standalone installation
python -m pip install types-aiobotocore-mediaconnect
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mediaconnect
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MediaConnectClient

Type annotations and code completion for  `#!python session.create_client("mediaconnect")` as [MediaConnectClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client)

```python
# MediaConnectClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.client import MediaConnectClient


session = get_session()
async with session.create_client("mediaconnect") as client:
    client: MediaConnectClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("mediaconnect").get_paginator("...")`.

```python
# ListBridgesPaginator usage example

from types_aiobotocore_mediaconnect.paginator import ListBridgesPaginator

def get_list_bridges_paginator() -> ListBridgesPaginator:
    return client.get_paginator("list_bridges"))
```

- [ListBridgesPaginator](./paginators.md#listbridgespaginator)
- [ListEntitlementsPaginator](./paginators.md#listentitlementspaginator)
- [ListFlowsPaginator](./paginators.md#listflowspaginator)
- [ListGatewayInstancesPaginator](./paginators.md#listgatewayinstancespaginator)
- [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
- [ListOfferingsPaginator](./paginators.md#listofferingspaginator)
- [ListReservationsPaginator](./paginators.md#listreservationspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("mediaconnect").get_waiter("...")`.

```python
# FlowActiveWaiter usage example

from types_aiobotocore_mediaconnect.waiter import FlowActiveWaiter

def get_flow_active_waiter() -> FlowActiveWaiter:
    return Session().client("mediaconnect").get_waiter("flow_active")
```

- [FlowActiveWaiter](./waiters.md#flowactivewaiter)
- [FlowDeletedWaiter](./waiters.md#flowdeletedwaiter)
- [FlowStandbyWaiter](./waiters.md#flowstandbywaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AlgorithmType usage example

from types_aiobotocore_mediaconnect.literals import AlgorithmType

def get_value() -> AlgorithmType:
    return "aes128"
```

- [AlgorithmType](./literals.md#algorithmtype)
- [BridgePlacementType](./literals.md#bridgeplacementtype)
- [BridgeStateType](./literals.md#bridgestatetype)
- [ColorimetryType](./literals.md#colorimetrytype)
- [ConnectionStatusType](./literals.md#connectionstatustype)
- [ContentQualityAnalysisStateType](./literals.md#contentqualityanalysisstatetype)
- [DesiredStateType](./literals.md#desiredstatetype)
- [DurationUnitsType](./literals.md#durationunitstype)
- [EncoderProfileType](./literals.md#encoderprofiletype)
- [EncodingNameType](./literals.md#encodingnametype)
- [EntitlementStatusType](./literals.md#entitlementstatustype)
- [FailoverModeType](./literals.md#failovermodetype)
- [FlowActiveWaiterName](./literals.md#flowactivewaitername)
- [FlowDeletedWaiterName](./literals.md#flowdeletedwaitername)
- [FlowSizeType](./literals.md#flowsizetype)
- [FlowStandbyWaiterName](./literals.md#flowstandbywaitername)
- [GatewayStateType](./literals.md#gatewaystatetype)
- [InstanceStateType](./literals.md#instancestatetype)
- [KeyTypeType](./literals.md#keytypetype)
- [ListBridgesPaginatorName](./literals.md#listbridgespaginatorname)
- [ListEntitlementsPaginatorName](./literals.md#listentitlementspaginatorname)
- [ListFlowsPaginatorName](./literals.md#listflowspaginatorname)
- [ListGatewayInstancesPaginatorName](./literals.md#listgatewayinstancespaginatorname)
- [ListGatewaysPaginatorName](./literals.md#listgatewayspaginatorname)
- [ListOfferingsPaginatorName](./literals.md#listofferingspaginatorname)
- [ListReservationsPaginatorName](./literals.md#listreservationspaginatorname)
- [MaintenanceDayType](./literals.md#maintenancedaytype)
- [MediaStreamTypeType](./literals.md#mediastreamtypetype)
- [NdiStateType](./literals.md#ndistatetype)
- [NetworkInterfaceTypeType](./literals.md#networkinterfacetypetype)
- [OutputStatusType](./literals.md#outputstatustype)
- [PriceUnitsType](./literals.md#priceunitstype)
- [ProtocolType](./literals.md#protocoltype)
- [RangeType](./literals.md#rangetype)
- [ReservationStateType](./literals.md#reservationstatetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [ScanModeType](./literals.md#scanmodetype)
- [SourceTypeType](./literals.md#sourcetypetype)
- [StateType](./literals.md#statetype)
- [StatusType](./literals.md#statustype)
- [TcsType](./literals.md#tcstype)
- [ThumbnailStateType](./literals.md#thumbnailstatetype)
- [MediaConnectServiceName](./literals.md#mediaconnectservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [VpcInterfaceAttachmentTypeDef](./type_defs.md#vpcinterfaceattachmenttypedef)
- [AddBridgeNetworkOutputRequestTypeDef](./type_defs.md#addbridgenetworkoutputrequesttypedef)
- [MulticastSourceSettingsTypeDef](./type_defs.md#multicastsourcesettingstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AddEgressGatewayBridgeRequestTypeDef](./type_defs.md#addegressgatewaybridgerequesttypedef)
- [VpcInterfaceRequestTypeDef](./type_defs.md#vpcinterfacerequesttypedef)
- [VpcInterfaceTypeDef](./type_defs.md#vpcinterfacetypedef)
- [AddIngressGatewayBridgeRequestTypeDef](./type_defs.md#addingressgatewaybridgerequesttypedef)
- [AddMaintenanceTypeDef](./type_defs.md#addmaintenancetypedef)
- [EncryptionTypeDef](./type_defs.md#encryptiontypedef)
- [SilentAudioTypeDef](./type_defs.md#silentaudiotypedef)
- [BlackFramesTypeDef](./type_defs.md#blackframestypedef)
- [BridgeFlowOutputTypeDef](./type_defs.md#bridgeflowoutputtypedef)
- [BridgeNetworkOutputTypeDef](./type_defs.md#bridgenetworkoutputtypedef)
- [EgressGatewayBridgeTypeDef](./type_defs.md#egressgatewaybridgetypedef)
- [IngressGatewayBridgeTypeDef](./type_defs.md#ingressgatewaybridgetypedef)
- [MessageDetailTypeDef](./type_defs.md#messagedetailtypedef)
- [GatewayNetworkTypeDef](./type_defs.md#gatewaynetworktypedef)
- [DeleteBridgeRequestTypeDef](./type_defs.md#deletebridgerequesttypedef)
- [DeleteFlowRequestTypeDef](./type_defs.md#deleteflowrequesttypedef)
- [DeleteGatewayRequestTypeDef](./type_defs.md#deletegatewayrequesttypedef)
- [DeregisterGatewayInstanceRequestTypeDef](./type_defs.md#deregistergatewayinstancerequesttypedef)
- [DescribeBridgeRequestTypeDef](./type_defs.md#describebridgerequesttypedef)
- [DescribeFlowRequestTypeDef](./type_defs.md#describeflowrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [MessagesTypeDef](./type_defs.md#messagestypedef)
- [DescribeFlowSourceMetadataRequestTypeDef](./type_defs.md#describeflowsourcemetadatarequesttypedef)
- [DescribeFlowSourceThumbnailRequestTypeDef](./type_defs.md#describeflowsourcethumbnailrequesttypedef)
- [DescribeGatewayInstanceRequestTypeDef](./type_defs.md#describegatewayinstancerequesttypedef)
- [DescribeGatewayRequestTypeDef](./type_defs.md#describegatewayrequesttypedef)
- [DescribeOfferingRequestTypeDef](./type_defs.md#describeofferingrequesttypedef)
- [DescribeReservationRequestTypeDef](./type_defs.md#describereservationrequesttypedef)
- [InterfaceRequestTypeDef](./type_defs.md#interfacerequesttypedef)
- [InterfaceTypeDef](./type_defs.md#interfacetypedef)
- [EncodingParametersRequestTypeDef](./type_defs.md#encodingparametersrequesttypedef)
- [EncodingParametersTypeDef](./type_defs.md#encodingparameterstypedef)
- [SourcePriorityTypeDef](./type_defs.md#sourceprioritytypedef)
- [MaintenanceTypeDef](./type_defs.md#maintenancetypedef)
- [FmtpRequestTypeDef](./type_defs.md#fmtprequesttypedef)
- [FmtpTypeDef](./type_defs.md#fmtptypedef)
- [FrameResolutionTypeDef](./type_defs.md#frameresolutiontypedef)
- [FrozenFramesTypeDef](./type_defs.md#frozenframestypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBridgesRequestTypeDef](./type_defs.md#listbridgesrequesttypedef)
- [ListedBridgeTypeDef](./type_defs.md#listedbridgetypedef)
- [ListEntitlementsRequestTypeDef](./type_defs.md#listentitlementsrequesttypedef)
- [ListedEntitlementTypeDef](./type_defs.md#listedentitlementtypedef)
- [ListFlowsRequestTypeDef](./type_defs.md#listflowsrequesttypedef)
- [ListGatewayInstancesRequestTypeDef](./type_defs.md#listgatewayinstancesrequesttypedef)
- [ListedGatewayInstanceTypeDef](./type_defs.md#listedgatewayinstancetypedef)
- [ListGatewaysRequestTypeDef](./type_defs.md#listgatewaysrequesttypedef)
- [ListedGatewayTypeDef](./type_defs.md#listedgatewaytypedef)
- [ListOfferingsRequestTypeDef](./type_defs.md#listofferingsrequesttypedef)
- [ListReservationsRequestTypeDef](./type_defs.md#listreservationsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [NdiDiscoveryServerConfigTypeDef](./type_defs.md#ndidiscoveryserverconfigtypedef)
- [ResourceSpecificationTypeDef](./type_defs.md#resourcespecificationtypedef)
- [TransportTypeDef](./type_defs.md#transporttypedef)
- [PurchaseOfferingRequestTypeDef](./type_defs.md#purchaseofferingrequesttypedef)
- [RemoveBridgeOutputRequestTypeDef](./type_defs.md#removebridgeoutputrequesttypedef)
- [RemoveBridgeSourceRequestTypeDef](./type_defs.md#removebridgesourcerequesttypedef)
- [RemoveFlowMediaStreamRequestTypeDef](./type_defs.md#removeflowmediastreamrequesttypedef)
- [RemoveFlowOutputRequestTypeDef](./type_defs.md#removeflowoutputrequesttypedef)
- [RemoveFlowSourceRequestTypeDef](./type_defs.md#removeflowsourcerequesttypedef)
- [RemoveFlowVpcInterfaceRequestTypeDef](./type_defs.md#removeflowvpcinterfacerequesttypedef)
- [RevokeFlowEntitlementRequestTypeDef](./type_defs.md#revokeflowentitlementrequesttypedef)
- [StartFlowRequestTypeDef](./type_defs.md#startflowrequesttypedef)
- [StopFlowRequestTypeDef](./type_defs.md#stopflowrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateBridgeNetworkOutputRequestTypeDef](./type_defs.md#updatebridgenetworkoutputrequesttypedef)
- [UpdateEgressGatewayBridgeRequestTypeDef](./type_defs.md#updateegressgatewaybridgerequesttypedef)
- [UpdateIngressGatewayBridgeRequestTypeDef](./type_defs.md#updateingressgatewaybridgerequesttypedef)
- [UpdateBridgeStateRequestTypeDef](./type_defs.md#updatebridgestaterequesttypedef)
- [UpdateEncryptionTypeDef](./type_defs.md#updateencryptiontypedef)
- [UpdateMaintenanceTypeDef](./type_defs.md#updatemaintenancetypedef)
- [UpdateGatewayInstanceRequestTypeDef](./type_defs.md#updategatewayinstancerequesttypedef)
- [AddBridgeFlowSourceRequestTypeDef](./type_defs.md#addbridgeflowsourcerequesttypedef)
- [BridgeFlowSourceTypeDef](./type_defs.md#bridgeflowsourcetypedef)
- [GatewayBridgeSourceTypeDef](./type_defs.md#gatewaybridgesourcetypedef)
- [SetGatewayBridgeSourceRequestTypeDef](./type_defs.md#setgatewaybridgesourcerequesttypedef)
- [UpdateBridgeFlowSourceRequestTypeDef](./type_defs.md#updatebridgeflowsourcerequesttypedef)
- [UpdateGatewayBridgeSourceRequestTypeDef](./type_defs.md#updategatewaybridgesourcerequesttypedef)
- [AddBridgeOutputRequestTypeDef](./type_defs.md#addbridgeoutputrequesttypedef)
- [AddBridgeNetworkSourceRequestTypeDef](./type_defs.md#addbridgenetworksourcerequesttypedef)
- [BridgeNetworkSourceTypeDef](./type_defs.md#bridgenetworksourcetypedef)
- [UpdateBridgeNetworkSourceRequestTypeDef](./type_defs.md#updatebridgenetworksourcerequesttypedef)
- [DeleteBridgeResponseTypeDef](./type_defs.md#deletebridgeresponsetypedef)
- [DeleteFlowResponseTypeDef](./type_defs.md#deleteflowresponsetypedef)
- [DeleteGatewayResponseTypeDef](./type_defs.md#deletegatewayresponsetypedef)
- [DeregisterGatewayInstanceResponseTypeDef](./type_defs.md#deregistergatewayinstanceresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [RemoveBridgeOutputResponseTypeDef](./type_defs.md#removebridgeoutputresponsetypedef)
- [RemoveBridgeSourceResponseTypeDef](./type_defs.md#removebridgesourceresponsetypedef)
- [RemoveFlowMediaStreamResponseTypeDef](./type_defs.md#removeflowmediastreamresponsetypedef)
- [RemoveFlowOutputResponseTypeDef](./type_defs.md#removeflowoutputresponsetypedef)
- [RemoveFlowSourceResponseTypeDef](./type_defs.md#removeflowsourceresponsetypedef)
- [RemoveFlowVpcInterfaceResponseTypeDef](./type_defs.md#removeflowvpcinterfaceresponsetypedef)
- [RevokeFlowEntitlementResponseTypeDef](./type_defs.md#revokeflowentitlementresponsetypedef)
- [StartFlowResponseTypeDef](./type_defs.md#startflowresponsetypedef)
- [StopFlowResponseTypeDef](./type_defs.md#stopflowresponsetypedef)
- [UpdateBridgeStateResponseTypeDef](./type_defs.md#updatebridgestateresponsetypedef)
- [UpdateGatewayInstanceResponseTypeDef](./type_defs.md#updategatewayinstanceresponsetypedef)
- [AddFlowVpcInterfacesRequestTypeDef](./type_defs.md#addflowvpcinterfacesrequesttypedef)
- [AddFlowVpcInterfacesResponseTypeDef](./type_defs.md#addflowvpcinterfacesresponsetypedef)
- [EntitlementTypeDef](./type_defs.md#entitlementtypedef)
- [GrantEntitlementRequestTypeDef](./type_defs.md#grantentitlementrequesttypedef)
- [AudioMonitoringSettingTypeDef](./type_defs.md#audiomonitoringsettingtypedef)
- [BridgeOutputTypeDef](./type_defs.md#bridgeoutputtypedef)
- [GatewayInstanceTypeDef](./type_defs.md#gatewayinstancetypedef)
- [ThumbnailDetailsTypeDef](./type_defs.md#thumbnaildetailstypedef)
- [CreateGatewayRequestTypeDef](./type_defs.md#creategatewayrequesttypedef)
- [GatewayTypeDef](./type_defs.md#gatewaytypedef)
- [DescribeFlowRequestWaitExtraExtraTypeDef](./type_defs.md#describeflowrequestwaitextraextratypedef)
- [DescribeFlowRequestWaitExtraTypeDef](./type_defs.md#describeflowrequestwaitextratypedef)
- [DescribeFlowRequestWaitTypeDef](./type_defs.md#describeflowrequestwaittypedef)
- [DestinationConfigurationRequestTypeDef](./type_defs.md#destinationconfigurationrequesttypedef)
- [InputConfigurationRequestTypeDef](./type_defs.md#inputconfigurationrequesttypedef)
- [DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef)
- [InputConfigurationTypeDef](./type_defs.md#inputconfigurationtypedef)
- [FailoverConfigTypeDef](./type_defs.md#failoverconfigtypedef)
- [UpdateFailoverConfigTypeDef](./type_defs.md#updatefailoverconfigtypedef)
- [ListedFlowTypeDef](./type_defs.md#listedflowtypedef)
- [MediaStreamAttributesRequestTypeDef](./type_defs.md#mediastreamattributesrequesttypedef)
- [MediaStreamAttributesTypeDef](./type_defs.md#mediastreamattributestypedef)
- [TransportStreamTypeDef](./type_defs.md#transportstreamtypedef)
- [VideoMonitoringSettingTypeDef](./type_defs.md#videomonitoringsettingtypedef)
- [ListBridgesRequestPaginateTypeDef](./type_defs.md#listbridgesrequestpaginatetypedef)
- [ListEntitlementsRequestPaginateTypeDef](./type_defs.md#listentitlementsrequestpaginatetypedef)
- [ListFlowsRequestPaginateTypeDef](./type_defs.md#listflowsrequestpaginatetypedef)
- [ListGatewayInstancesRequestPaginateTypeDef](./type_defs.md#listgatewayinstancesrequestpaginatetypedef)
- [ListGatewaysRequestPaginateTypeDef](./type_defs.md#listgatewaysrequestpaginatetypedef)
- [ListOfferingsRequestPaginateTypeDef](./type_defs.md#listofferingsrequestpaginatetypedef)
- [ListReservationsRequestPaginateTypeDef](./type_defs.md#listreservationsrequestpaginatetypedef)
- [ListBridgesResponseTypeDef](./type_defs.md#listbridgesresponsetypedef)
- [ListEntitlementsResponseTypeDef](./type_defs.md#listentitlementsresponsetypedef)
- [ListGatewayInstancesResponseTypeDef](./type_defs.md#listgatewayinstancesresponsetypedef)
- [ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef)
- [NdiConfigOutputTypeDef](./type_defs.md#ndiconfigoutputtypedef)
- [NdiConfigTypeDef](./type_defs.md#ndiconfigtypedef)
- [OfferingTypeDef](./type_defs.md#offeringtypedef)
- [ReservationTypeDef](./type_defs.md#reservationtypedef)
- [UpdateBridgeOutputRequestTypeDef](./type_defs.md#updatebridgeoutputrequesttypedef)
- [UpdateFlowEntitlementRequestTypeDef](./type_defs.md#updateflowentitlementrequesttypedef)
- [AddBridgeOutputsRequestTypeDef](./type_defs.md#addbridgeoutputsrequesttypedef)
- [AddBridgeSourceRequestTypeDef](./type_defs.md#addbridgesourcerequesttypedef)
- [BridgeSourceTypeDef](./type_defs.md#bridgesourcetypedef)
- [UpdateBridgeSourceRequestTypeDef](./type_defs.md#updatebridgesourcerequesttypedef)
- [GrantFlowEntitlementsResponseTypeDef](./type_defs.md#grantflowentitlementsresponsetypedef)
- [UpdateFlowEntitlementResponseTypeDef](./type_defs.md#updateflowentitlementresponsetypedef)
- [GrantFlowEntitlementsRequestTypeDef](./type_defs.md#grantflowentitlementsrequesttypedef)
- [AddBridgeOutputsResponseTypeDef](./type_defs.md#addbridgeoutputsresponsetypedef)
- [UpdateBridgeOutputResponseTypeDef](./type_defs.md#updatebridgeoutputresponsetypedef)
- [DescribeGatewayInstanceResponseTypeDef](./type_defs.md#describegatewayinstanceresponsetypedef)
- [DescribeFlowSourceThumbnailResponseTypeDef](./type_defs.md#describeflowsourcethumbnailresponsetypedef)
- [CreateGatewayResponseTypeDef](./type_defs.md#creategatewayresponsetypedef)
- [DescribeGatewayResponseTypeDef](./type_defs.md#describegatewayresponsetypedef)
- [MediaStreamOutputConfigurationRequestTypeDef](./type_defs.md#mediastreamoutputconfigurationrequesttypedef)
- [MediaStreamSourceConfigurationRequestTypeDef](./type_defs.md#mediastreamsourceconfigurationrequesttypedef)
- [MediaStreamOutputConfigurationTypeDef](./type_defs.md#mediastreamoutputconfigurationtypedef)
- [MediaStreamSourceConfigurationTypeDef](./type_defs.md#mediastreamsourceconfigurationtypedef)
- [UpdateBridgeRequestTypeDef](./type_defs.md#updatebridgerequesttypedef)
- [ListFlowsResponseTypeDef](./type_defs.md#listflowsresponsetypedef)
- [AddMediaStreamRequestTypeDef](./type_defs.md#addmediastreamrequesttypedef)
- [UpdateFlowMediaStreamRequestTypeDef](./type_defs.md#updateflowmediastreamrequesttypedef)
- [MediaStreamTypeDef](./type_defs.md#mediastreamtypedef)
- [TransportStreamProgramTypeDef](./type_defs.md#transportstreamprogramtypedef)
- [MonitoringConfigOutputTypeDef](./type_defs.md#monitoringconfigoutputtypedef)
- [MonitoringConfigTypeDef](./type_defs.md#monitoringconfigtypedef)
- [NdiConfigUnionTypeDef](./type_defs.md#ndiconfiguniontypedef)
- [DescribeOfferingResponseTypeDef](./type_defs.md#describeofferingresponsetypedef)
- [ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef)
- [DescribeReservationResponseTypeDef](./type_defs.md#describereservationresponsetypedef)
- [ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef)
- [PurchaseOfferingResponseTypeDef](./type_defs.md#purchaseofferingresponsetypedef)
- [AddBridgeSourcesRequestTypeDef](./type_defs.md#addbridgesourcesrequesttypedef)
- [CreateBridgeRequestTypeDef](./type_defs.md#createbridgerequesttypedef)
- [AddBridgeSourcesResponseTypeDef](./type_defs.md#addbridgesourcesresponsetypedef)
- [BridgeTypeDef](./type_defs.md#bridgetypedef)
- [UpdateBridgeSourceResponseTypeDef](./type_defs.md#updatebridgesourceresponsetypedef)
- [AddOutputRequestTypeDef](./type_defs.md#addoutputrequesttypedef)
- [UpdateFlowOutputRequestTypeDef](./type_defs.md#updateflowoutputrequesttypedef)
- [SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef)
- [UpdateFlowSourceRequestTypeDef](./type_defs.md#updateflowsourcerequesttypedef)
- [OutputTypeDef](./type_defs.md#outputtypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [AddFlowMediaStreamsRequestTypeDef](./type_defs.md#addflowmediastreamsrequesttypedef)
- [AddFlowMediaStreamsResponseTypeDef](./type_defs.md#addflowmediastreamsresponsetypedef)
- [UpdateFlowMediaStreamResponseTypeDef](./type_defs.md#updateflowmediastreamresponsetypedef)
- [TransportMediaInfoTypeDef](./type_defs.md#transportmediainfotypedef)
- [MonitoringConfigUnionTypeDef](./type_defs.md#monitoringconfiguniontypedef)
- [CreateBridgeResponseTypeDef](./type_defs.md#createbridgeresponsetypedef)
- [DescribeBridgeResponseTypeDef](./type_defs.md#describebridgeresponsetypedef)
- [UpdateBridgeResponseTypeDef](./type_defs.md#updatebridgeresponsetypedef)
- [AddFlowOutputsRequestTypeDef](./type_defs.md#addflowoutputsrequesttypedef)
- [AddFlowSourcesRequestTypeDef](./type_defs.md#addflowsourcesrequesttypedef)
- [AddFlowOutputsResponseTypeDef](./type_defs.md#addflowoutputsresponsetypedef)
- [UpdateFlowOutputResponseTypeDef](./type_defs.md#updateflowoutputresponsetypedef)
- [AddFlowSourcesResponseTypeDef](./type_defs.md#addflowsourcesresponsetypedef)
- [FlowTypeDef](./type_defs.md#flowtypedef)
- [UpdateFlowSourceResponseTypeDef](./type_defs.md#updateflowsourceresponsetypedef)
- [DescribeFlowSourceMetadataResponseTypeDef](./type_defs.md#describeflowsourcemetadataresponsetypedef)
- [CreateFlowRequestTypeDef](./type_defs.md#createflowrequesttypedef)
- [UpdateFlowRequestTypeDef](./type_defs.md#updateflowrequesttypedef)
- [CreateFlowResponseTypeDef](./type_defs.md#createflowresponsetypedef)
- [DescribeFlowResponseTypeDef](./type_defs.md#describeflowresponsetypedef)
- [UpdateFlowResponseTypeDef](./type_defs.md#updateflowresponsetypedef)

