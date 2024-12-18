# MediaConnect module

> [Index](../README.md) > MediaConnect


!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#mediaconnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
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
- [DesiredStateType](./literals.md#desiredstatetype)
- [DurationUnitsType](./literals.md#durationunitstype)
- [EncoderProfileType](./literals.md#encoderprofiletype)
- [EncodingNameType](./literals.md#encodingnametype)
- [EntitlementStatusType](./literals.md#entitlementstatustype)
- [FailoverModeType](./literals.md#failovermodetype)
- [FlowActiveWaiterName](./literals.md#flowactivewaitername)
- [FlowDeletedWaiterName](./literals.md#flowdeletedwaitername)
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
- [BridgeFlowOutputTypeDef](./type_defs.md#bridgeflowoutputtypedef)
- [BridgeNetworkOutputTypeDef](./type_defs.md#bridgenetworkoutputtypedef)
- [EgressGatewayBridgeTypeDef](./type_defs.md#egressgatewaybridgetypedef)
- [IngressGatewayBridgeTypeDef](./type_defs.md#ingressgatewaybridgetypedef)
- [MessageDetailTypeDef](./type_defs.md#messagedetailtypedef)
- [MonitoringConfigTypeDef](./type_defs.md#monitoringconfigtypedef)
- [GatewayNetworkTypeDef](./type_defs.md#gatewaynetworktypedef)
- [DeleteBridgeRequestRequestTypeDef](./type_defs.md#deletebridgerequestrequesttypedef)
- [DeleteFlowRequestRequestTypeDef](./type_defs.md#deleteflowrequestrequesttypedef)
- [DeleteGatewayRequestRequestTypeDef](./type_defs.md#deletegatewayrequestrequesttypedef)
- [DeregisterGatewayInstanceRequestRequestTypeDef](./type_defs.md#deregistergatewayinstancerequestrequesttypedef)
- [DescribeBridgeRequestRequestTypeDef](./type_defs.md#describebridgerequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeFlowRequestRequestTypeDef](./type_defs.md#describeflowrequestrequesttypedef)
- [MessagesTypeDef](./type_defs.md#messagestypedef)
- [DescribeFlowSourceMetadataRequestRequestTypeDef](./type_defs.md#describeflowsourcemetadatarequestrequesttypedef)
- [DescribeFlowSourceThumbnailRequestRequestTypeDef](./type_defs.md#describeflowsourcethumbnailrequestrequesttypedef)
- [DescribeGatewayInstanceRequestRequestTypeDef](./type_defs.md#describegatewayinstancerequestrequesttypedef)
- [DescribeGatewayRequestRequestTypeDef](./type_defs.md#describegatewayrequestrequesttypedef)
- [DescribeOfferingRequestRequestTypeDef](./type_defs.md#describeofferingrequestrequesttypedef)
- [DescribeReservationRequestRequestTypeDef](./type_defs.md#describereservationrequestrequesttypedef)
- [InterfaceRequestTypeDef](./type_defs.md#interfacerequesttypedef)
- [InterfaceTypeDef](./type_defs.md#interfacetypedef)
- [EncodingParametersRequestTypeDef](./type_defs.md#encodingparametersrequesttypedef)
- [EncodingParametersTypeDef](./type_defs.md#encodingparameterstypedef)
- [SourcePriorityTypeDef](./type_defs.md#sourceprioritytypedef)
- [MaintenanceTypeDef](./type_defs.md#maintenancetypedef)
- [FmtpRequestTypeDef](./type_defs.md#fmtprequesttypedef)
- [FmtpTypeDef](./type_defs.md#fmtptypedef)
- [FrameResolutionTypeDef](./type_defs.md#frameresolutiontypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBridgesRequestRequestTypeDef](./type_defs.md#listbridgesrequestrequesttypedef)
- [ListedBridgeTypeDef](./type_defs.md#listedbridgetypedef)
- [ListEntitlementsRequestRequestTypeDef](./type_defs.md#listentitlementsrequestrequesttypedef)
- [ListedEntitlementTypeDef](./type_defs.md#listedentitlementtypedef)
- [ListFlowsRequestRequestTypeDef](./type_defs.md#listflowsrequestrequesttypedef)
- [ListGatewayInstancesRequestRequestTypeDef](./type_defs.md#listgatewayinstancesrequestrequesttypedef)
- [ListedGatewayInstanceTypeDef](./type_defs.md#listedgatewayinstancetypedef)
- [ListGatewaysRequestRequestTypeDef](./type_defs.md#listgatewaysrequestrequesttypedef)
- [ListedGatewayTypeDef](./type_defs.md#listedgatewaytypedef)
- [ListOfferingsRequestRequestTypeDef](./type_defs.md#listofferingsrequestrequesttypedef)
- [ListReservationsRequestRequestTypeDef](./type_defs.md#listreservationsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ResourceSpecificationTypeDef](./type_defs.md#resourcespecificationtypedef)
- [TransportTypeDef](./type_defs.md#transporttypedef)
- [PurchaseOfferingRequestRequestTypeDef](./type_defs.md#purchaseofferingrequestrequesttypedef)
- [RemoveBridgeOutputRequestRequestTypeDef](./type_defs.md#removebridgeoutputrequestrequesttypedef)
- [RemoveBridgeSourceRequestRequestTypeDef](./type_defs.md#removebridgesourcerequestrequesttypedef)
- [RemoveFlowMediaStreamRequestRequestTypeDef](./type_defs.md#removeflowmediastreamrequestrequesttypedef)
- [RemoveFlowOutputRequestRequestTypeDef](./type_defs.md#removeflowoutputrequestrequesttypedef)
- [RemoveFlowSourceRequestRequestTypeDef](./type_defs.md#removeflowsourcerequestrequesttypedef)
- [RemoveFlowVpcInterfaceRequestRequestTypeDef](./type_defs.md#removeflowvpcinterfacerequestrequesttypedef)
- [RevokeFlowEntitlementRequestRequestTypeDef](./type_defs.md#revokeflowentitlementrequestrequesttypedef)
- [StartFlowRequestRequestTypeDef](./type_defs.md#startflowrequestrequesttypedef)
- [StopFlowRequestRequestTypeDef](./type_defs.md#stopflowrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateBridgeNetworkOutputRequestTypeDef](./type_defs.md#updatebridgenetworkoutputrequesttypedef)
- [UpdateEgressGatewayBridgeRequestTypeDef](./type_defs.md#updateegressgatewaybridgerequesttypedef)
- [UpdateIngressGatewayBridgeRequestTypeDef](./type_defs.md#updateingressgatewaybridgerequesttypedef)
- [UpdateBridgeStateRequestRequestTypeDef](./type_defs.md#updatebridgestaterequestrequesttypedef)
- [UpdateEncryptionTypeDef](./type_defs.md#updateencryptiontypedef)
- [UpdateMaintenanceTypeDef](./type_defs.md#updatemaintenancetypedef)
- [UpdateGatewayInstanceRequestRequestTypeDef](./type_defs.md#updategatewayinstancerequestrequesttypedef)
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
- [AddFlowVpcInterfacesRequestRequestTypeDef](./type_defs.md#addflowvpcinterfacesrequestrequesttypedef)
- [AddFlowVpcInterfacesResponseTypeDef](./type_defs.md#addflowvpcinterfacesresponsetypedef)
- [EntitlementTypeDef](./type_defs.md#entitlementtypedef)
- [GrantEntitlementRequestTypeDef](./type_defs.md#grantentitlementrequesttypedef)
- [BridgeOutputTypeDef](./type_defs.md#bridgeoutputtypedef)
- [GatewayInstanceTypeDef](./type_defs.md#gatewayinstancetypedef)
- [ThumbnailDetailsTypeDef](./type_defs.md#thumbnaildetailstypedef)
- [CreateGatewayRequestRequestTypeDef](./type_defs.md#creategatewayrequestrequesttypedef)
- [GatewayTypeDef](./type_defs.md#gatewaytypedef)
- [DescribeFlowRequestFlowActiveWaitTypeDef](./type_defs.md#describeflowrequestflowactivewaittypedef)
- [DescribeFlowRequestFlowDeletedWaitTypeDef](./type_defs.md#describeflowrequestflowdeletedwaittypedef)
- [DescribeFlowRequestFlowStandbyWaitTypeDef](./type_defs.md#describeflowrequestflowstandbywaittypedef)
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
- [ListBridgesRequestListBridgesPaginateTypeDef](./type_defs.md#listbridgesrequestlistbridgespaginatetypedef)
- [ListEntitlementsRequestListEntitlementsPaginateTypeDef](./type_defs.md#listentitlementsrequestlistentitlementspaginatetypedef)
- [ListFlowsRequestListFlowsPaginateTypeDef](./type_defs.md#listflowsrequestlistflowspaginatetypedef)
- [ListGatewayInstancesRequestListGatewayInstancesPaginateTypeDef](./type_defs.md#listgatewayinstancesrequestlistgatewayinstancespaginatetypedef)
- [ListGatewaysRequestListGatewaysPaginateTypeDef](./type_defs.md#listgatewaysrequestlistgatewayspaginatetypedef)
- [ListOfferingsRequestListOfferingsPaginateTypeDef](./type_defs.md#listofferingsrequestlistofferingspaginatetypedef)
- [ListReservationsRequestListReservationsPaginateTypeDef](./type_defs.md#listreservationsrequestlistreservationspaginatetypedef)
- [ListBridgesResponseTypeDef](./type_defs.md#listbridgesresponsetypedef)
- [ListEntitlementsResponseTypeDef](./type_defs.md#listentitlementsresponsetypedef)
- [ListGatewayInstancesResponseTypeDef](./type_defs.md#listgatewayinstancesresponsetypedef)
- [ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef)
- [OfferingTypeDef](./type_defs.md#offeringtypedef)
- [ReservationTypeDef](./type_defs.md#reservationtypedef)
- [UpdateBridgeOutputRequestRequestTypeDef](./type_defs.md#updatebridgeoutputrequestrequesttypedef)
- [UpdateFlowEntitlementRequestRequestTypeDef](./type_defs.md#updateflowentitlementrequestrequesttypedef)
- [AddBridgeOutputsRequestRequestTypeDef](./type_defs.md#addbridgeoutputsrequestrequesttypedef)
- [AddBridgeSourceRequestTypeDef](./type_defs.md#addbridgesourcerequesttypedef)
- [BridgeSourceTypeDef](./type_defs.md#bridgesourcetypedef)
- [UpdateBridgeSourceRequestRequestTypeDef](./type_defs.md#updatebridgesourcerequestrequesttypedef)
- [GrantFlowEntitlementsResponseTypeDef](./type_defs.md#grantflowentitlementsresponsetypedef)
- [UpdateFlowEntitlementResponseTypeDef](./type_defs.md#updateflowentitlementresponsetypedef)
- [GrantFlowEntitlementsRequestRequestTypeDef](./type_defs.md#grantflowentitlementsrequestrequesttypedef)
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
- [UpdateBridgeRequestRequestTypeDef](./type_defs.md#updatebridgerequestrequesttypedef)
- [UpdateFlowRequestRequestTypeDef](./type_defs.md#updateflowrequestrequesttypedef)
- [ListFlowsResponseTypeDef](./type_defs.md#listflowsresponsetypedef)
- [AddMediaStreamRequestTypeDef](./type_defs.md#addmediastreamrequesttypedef)
- [UpdateFlowMediaStreamRequestRequestTypeDef](./type_defs.md#updateflowmediastreamrequestrequesttypedef)
- [MediaStreamTypeDef](./type_defs.md#mediastreamtypedef)
- [TransportStreamProgramTypeDef](./type_defs.md#transportstreamprogramtypedef)
- [DescribeOfferingResponseTypeDef](./type_defs.md#describeofferingresponsetypedef)
- [ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef)
- [DescribeReservationResponseTypeDef](./type_defs.md#describereservationresponsetypedef)
- [ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef)
- [PurchaseOfferingResponseTypeDef](./type_defs.md#purchaseofferingresponsetypedef)
- [AddBridgeSourcesRequestRequestTypeDef](./type_defs.md#addbridgesourcesrequestrequesttypedef)
- [CreateBridgeRequestRequestTypeDef](./type_defs.md#createbridgerequestrequesttypedef)
- [AddBridgeSourcesResponseTypeDef](./type_defs.md#addbridgesourcesresponsetypedef)
- [BridgeTypeDef](./type_defs.md#bridgetypedef)
- [UpdateBridgeSourceResponseTypeDef](./type_defs.md#updatebridgesourceresponsetypedef)
- [AddOutputRequestTypeDef](./type_defs.md#addoutputrequesttypedef)
- [UpdateFlowOutputRequestRequestTypeDef](./type_defs.md#updateflowoutputrequestrequesttypedef)
- [SetSourceRequestTypeDef](./type_defs.md#setsourcerequesttypedef)
- [UpdateFlowSourceRequestRequestTypeDef](./type_defs.md#updateflowsourcerequestrequesttypedef)
- [OutputTypeDef](./type_defs.md#outputtypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [AddFlowMediaStreamsRequestRequestTypeDef](./type_defs.md#addflowmediastreamsrequestrequesttypedef)
- [AddFlowMediaStreamsResponseTypeDef](./type_defs.md#addflowmediastreamsresponsetypedef)
- [UpdateFlowMediaStreamResponseTypeDef](./type_defs.md#updateflowmediastreamresponsetypedef)
- [TransportMediaInfoTypeDef](./type_defs.md#transportmediainfotypedef)
- [CreateBridgeResponseTypeDef](./type_defs.md#createbridgeresponsetypedef)
- [DescribeBridgeResponseTypeDef](./type_defs.md#describebridgeresponsetypedef)
- [UpdateBridgeResponseTypeDef](./type_defs.md#updatebridgeresponsetypedef)
- [AddFlowOutputsRequestRequestTypeDef](./type_defs.md#addflowoutputsrequestrequesttypedef)
- [AddFlowSourcesRequestRequestTypeDef](./type_defs.md#addflowsourcesrequestrequesttypedef)
- [CreateFlowRequestRequestTypeDef](./type_defs.md#createflowrequestrequesttypedef)
- [AddFlowOutputsResponseTypeDef](./type_defs.md#addflowoutputsresponsetypedef)
- [UpdateFlowOutputResponseTypeDef](./type_defs.md#updateflowoutputresponsetypedef)
- [AddFlowSourcesResponseTypeDef](./type_defs.md#addflowsourcesresponsetypedef)
- [FlowTypeDef](./type_defs.md#flowtypedef)
- [UpdateFlowSourceResponseTypeDef](./type_defs.md#updateflowsourceresponsetypedef)
- [DescribeFlowSourceMetadataResponseTypeDef](./type_defs.md#describeflowsourcemetadataresponsetypedef)
- [CreateFlowResponseTypeDef](./type_defs.md#createflowresponsetypedef)
- [DescribeFlowResponseTypeDef](./type_defs.md#describeflowresponsetypedef)
- [UpdateFlowResponseTypeDef](./type_defs.md#updateflowresponsetypedef)

