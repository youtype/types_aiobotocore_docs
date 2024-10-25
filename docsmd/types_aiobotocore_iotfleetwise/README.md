# IoTFleetWise module

> [Index](../README.md) > IoTFleetWise


!!! note ""

    Auto-generated documentation for [IoTFleetWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
    type annotations stubs module [types-aiobotocore-iotfleetwise](https://pypi.org/project/types-aiobotocore-iotfleetwise/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `IoTFleetWise` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iotfleetwise]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iotfleetwise]'


# standalone installation
python -m pip install types-aiobotocore-iotfleetwise
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iotfleetwise
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTFleetWiseClient

Type annotations and code completion for  `#!python session.create_client("iotfleetwise")` as [IoTFleetWiseClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Client)

```python
# IoTFleetWiseClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.client import IoTFleetWiseClient


session = get_session()
async with session.create_client("iotfleetwise") as client:
    client: IoTFleetWiseClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("iotfleetwise").get_paginator("...")`.

```python
# GetVehicleStatusPaginator usage example

from types_aiobotocore_iotfleetwise.paginator import GetVehicleStatusPaginator

def get_get_vehicle_status_paginator() -> GetVehicleStatusPaginator:
    return client.get_paginator("get_vehicle_status"))
```

- [GetVehicleStatusPaginator](./paginators.md#getvehiclestatuspaginator)
- [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
- [ListDecoderManifestNetworkInterfacesPaginator](./paginators.md#listdecodermanifestnetworkinterfacespaginator)
- [ListDecoderManifestSignalsPaginator](./paginators.md#listdecodermanifestsignalspaginator)
- [ListDecoderManifestsPaginator](./paginators.md#listdecodermanifestspaginator)
- [ListFleetsPaginator](./paginators.md#listfleetspaginator)
- [ListFleetsForVehiclePaginator](./paginators.md#listfleetsforvehiclepaginator)
- [ListModelManifestNodesPaginator](./paginators.md#listmodelmanifestnodespaginator)
- [ListModelManifestsPaginator](./paginators.md#listmodelmanifestspaginator)
- [ListSignalCatalogNodesPaginator](./paginators.md#listsignalcatalognodespaginator)
- [ListSignalCatalogsPaginator](./paginators.md#listsignalcatalogspaginator)
- [ListVehiclesPaginator](./paginators.md#listvehiclespaginator)
- [ListVehiclesInFleetPaginator](./paginators.md#listvehiclesinfleetpaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CampaignStatusType usage example

from types_aiobotocore_iotfleetwise.literals import CampaignStatusType

def get_value() -> CampaignStatusType:
    return "CREATING"
```

- [CampaignStatusType](./literals.md#campaignstatustype)
- [CompressionType](./literals.md#compressiontype)
- [DataFormatType](./literals.md#dataformattype)
- [DiagnosticsModeType](./literals.md#diagnosticsmodetype)
- [EncryptionStatusType](./literals.md#encryptionstatustype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [GetVehicleStatusPaginatorName](./literals.md#getvehiclestatuspaginatorname)
- [ListCampaignsPaginatorName](./literals.md#listcampaignspaginatorname)
- [ListDecoderManifestNetworkInterfacesPaginatorName](./literals.md#listdecodermanifestnetworkinterfacespaginatorname)
- [ListDecoderManifestSignalsPaginatorName](./literals.md#listdecodermanifestsignalspaginatorname)
- [ListDecoderManifestsPaginatorName](./literals.md#listdecodermanifestspaginatorname)
- [ListFleetsForVehiclePaginatorName](./literals.md#listfleetsforvehiclepaginatorname)
- [ListFleetsPaginatorName](./literals.md#listfleetspaginatorname)
- [ListModelManifestNodesPaginatorName](./literals.md#listmodelmanifestnodespaginatorname)
- [ListModelManifestsPaginatorName](./literals.md#listmodelmanifestspaginatorname)
- [ListSignalCatalogNodesPaginatorName](./literals.md#listsignalcatalognodespaginatorname)
- [ListSignalCatalogsPaginatorName](./literals.md#listsignalcatalogspaginatorname)
- [ListVehiclesInFleetPaginatorName](./literals.md#listvehiclesinfleetpaginatorname)
- [ListVehiclesPaginatorName](./literals.md#listvehiclespaginatorname)
- [LogTypeType](./literals.md#logtypetype)
- [ManifestStatusType](./literals.md#manifeststatustype)
- [NetworkInterfaceTypeType](./literals.md#networkinterfacetypetype)
- [NodeDataEncodingType](./literals.md#nodedataencodingtype)
- [NodeDataTypeType](./literals.md#nodedatatypetype)
- [ROS2PrimitiveTypeType](./literals.md#ros2primitivetypetype)
- [RegistrationStatusType](./literals.md#registrationstatustype)
- [SignalDecoderTypeType](./literals.md#signaldecodertypetype)
- [SignalNodeTypeType](./literals.md#signalnodetypetype)
- [SpoolingModeType](./literals.md#spoolingmodetype)
- [StorageCompressionFormatType](./literals.md#storagecompressionformattype)
- [StructuredMessageListTypeType](./literals.md#structuredmessagelisttypetype)
- [TriggerModeType](./literals.md#triggermodetype)
- [UpdateCampaignActionType](./literals.md#updatecampaignactiontype)
- [UpdateModeType](./literals.md#updatemodetype)
- [VehicleAssociationBehaviorType](./literals.md#vehicleassociationbehaviortype)
- [VehicleMiddlewareProtocolType](./literals.md#vehiclemiddlewareprotocoltype)
- [VehicleStateType](./literals.md#vehiclestatetype)
- [IoTFleetWiseServiceName](./literals.md#iotfleetwiseservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActuatorOutputTypeDef](./type_defs.md#actuatoroutputtypedef)
- [ActuatorTypeDef](./type_defs.md#actuatortypedef)
- [AssociateVehicleFleetRequestRequestTypeDef](./type_defs.md#associatevehiclefleetrequestrequesttypedef)
- [AttributeOutputTypeDef](./type_defs.md#attributeoutputtypedef)
- [AttributeTypeDef](./type_defs.md#attributetypedef)
- [CreateVehicleErrorTypeDef](./type_defs.md#createvehicleerrortypedef)
- [CreateVehicleResponseItemTypeDef](./type_defs.md#createvehicleresponseitemtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [UpdateVehicleRequestItemTypeDef](./type_defs.md#updatevehiclerequestitemtypedef)
- [UpdateVehicleErrorTypeDef](./type_defs.md#updatevehicleerrortypedef)
- [UpdateVehicleResponseItemTypeDef](./type_defs.md#updatevehicleresponseitemtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [BranchTypeDef](./type_defs.md#branchtypedef)
- [CampaignSummaryTypeDef](./type_defs.md#campaignsummarytypedef)
- [CanInterfaceTypeDef](./type_defs.md#caninterfacetypedef)
- [CanSignalTypeDef](./type_defs.md#cansignaltypedef)
- [CloudWatchLogDeliveryOptionsTypeDef](./type_defs.md#cloudwatchlogdeliveryoptionstypedef)
- [ConditionBasedCollectionSchemeTypeDef](./type_defs.md#conditionbasedcollectionschemetypedef)
- [TimeBasedCollectionSchemeTypeDef](./type_defs.md#timebasedcollectionschemetypedef)
- [SignalInformationTypeDef](./type_defs.md#signalinformationtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [CustomPropertyTypeDef](./type_defs.md#custompropertytypedef)
- [CustomStructTypeDef](./type_defs.md#customstructtypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [TimestreamConfigTypeDef](./type_defs.md#timestreamconfigtypedef)
- [DecoderManifestSummaryTypeDef](./type_defs.md#decodermanifestsummarytypedef)
- [DeleteCampaignRequestRequestTypeDef](./type_defs.md#deletecampaignrequestrequesttypedef)
- [DeleteDecoderManifestRequestRequestTypeDef](./type_defs.md#deletedecodermanifestrequestrequesttypedef)
- [DeleteFleetRequestRequestTypeDef](./type_defs.md#deletefleetrequestrequesttypedef)
- [DeleteModelManifestRequestRequestTypeDef](./type_defs.md#deletemodelmanifestrequestrequesttypedef)
- [DeleteSignalCatalogRequestRequestTypeDef](./type_defs.md#deletesignalcatalogrequestrequesttypedef)
- [DeleteVehicleRequestRequestTypeDef](./type_defs.md#deletevehiclerequestrequesttypedef)
- [DisassociateVehicleFleetRequestRequestTypeDef](./type_defs.md#disassociatevehiclefleetrequestrequesttypedef)
- [FleetSummaryTypeDef](./type_defs.md#fleetsummarytypedef)
- [FormattedVssTypeDef](./type_defs.md#formattedvsstypedef)
- [GetCampaignRequestRequestTypeDef](./type_defs.md#getcampaignrequestrequesttypedef)
- [GetDecoderManifestRequestRequestTypeDef](./type_defs.md#getdecodermanifestrequestrequesttypedef)
- [GetFleetRequestRequestTypeDef](./type_defs.md#getfleetrequestrequesttypedef)
- [GetModelManifestRequestRequestTypeDef](./type_defs.md#getmodelmanifestrequestrequesttypedef)
- [IamRegistrationResponseTypeDef](./type_defs.md#iamregistrationresponsetypedef)
- [TimestreamRegistrationResponseTypeDef](./type_defs.md#timestreamregistrationresponsetypedef)
- [GetSignalCatalogRequestRequestTypeDef](./type_defs.md#getsignalcatalogrequestrequesttypedef)
- [NodeCountsTypeDef](./type_defs.md#nodecountstypedef)
- [GetVehicleRequestRequestTypeDef](./type_defs.md#getvehiclerequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetVehicleStatusRequestRequestTypeDef](./type_defs.md#getvehiclestatusrequestrequesttypedef)
- [VehicleStatusTypeDef](./type_defs.md#vehiclestatustypedef)
- [IamResourcesTypeDef](./type_defs.md#iamresourcestypedef)
- [ListCampaignsRequestRequestTypeDef](./type_defs.md#listcampaignsrequestrequesttypedef)
- [ListDecoderManifestNetworkInterfacesRequestRequestTypeDef](./type_defs.md#listdecodermanifestnetworkinterfacesrequestrequesttypedef)
- [ListDecoderManifestSignalsRequestRequestTypeDef](./type_defs.md#listdecodermanifestsignalsrequestrequesttypedef)
- [ListDecoderManifestsRequestRequestTypeDef](./type_defs.md#listdecodermanifestsrequestrequesttypedef)
- [ListFleetsForVehicleRequestRequestTypeDef](./type_defs.md#listfleetsforvehiclerequestrequesttypedef)
- [ListFleetsRequestRequestTypeDef](./type_defs.md#listfleetsrequestrequesttypedef)
- [ListModelManifestNodesRequestRequestTypeDef](./type_defs.md#listmodelmanifestnodesrequestrequesttypedef)
- [ListModelManifestsRequestRequestTypeDef](./type_defs.md#listmodelmanifestsrequestrequesttypedef)
- [ModelManifestSummaryTypeDef](./type_defs.md#modelmanifestsummarytypedef)
- [ListSignalCatalogNodesRequestRequestTypeDef](./type_defs.md#listsignalcatalognodesrequestrequesttypedef)
- [ListSignalCatalogsRequestRequestTypeDef](./type_defs.md#listsignalcatalogsrequestrequesttypedef)
- [SignalCatalogSummaryTypeDef](./type_defs.md#signalcatalogsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListVehiclesInFleetRequestRequestTypeDef](./type_defs.md#listvehiclesinfleetrequestrequesttypedef)
- [ListVehiclesRequestRequestTypeDef](./type_defs.md#listvehiclesrequestrequesttypedef)
- [VehicleSummaryTypeDef](./type_defs.md#vehiclesummarytypedef)
- [ObdInterfaceTypeDef](./type_defs.md#obdinterfacetypedef)
- [VehicleMiddlewareTypeDef](./type_defs.md#vehiclemiddlewaretypedef)
- [SensorOutputTypeDef](./type_defs.md#sensoroutputtypedef)
- [ObdSignalTypeDef](./type_defs.md#obdsignaltypedef)
- [ROS2PrimitiveMessageDefinitionTypeDef](./type_defs.md#ros2primitivemessagedefinitiontypedef)
- [PutEncryptionConfigurationRequestRequestTypeDef](./type_defs.md#putencryptionconfigurationrequestrequesttypedef)
- [TimestreamResourcesTypeDef](./type_defs.md#timestreamresourcestypedef)
- [SensorTypeDef](./type_defs.md#sensortypedef)
- [StructuredMessageFieldNameAndDataTypePairOutputTypeDef](./type_defs.md#structuredmessagefieldnameanddatatypepairoutputtypedef)
- [StructuredMessageFieldNameAndDataTypePairPaginatorTypeDef](./type_defs.md#structuredmessagefieldnameanddatatypepairpaginatortypedef)
- [StructuredMessageFieldNameAndDataTypePairTypeDef](./type_defs.md#structuredmessagefieldnameanddatatypepairtypedef)
- [StructuredMessageListDefinitionOutputTypeDef](./type_defs.md#structuredmessagelistdefinitionoutputtypedef)
- [StructuredMessageListDefinitionPaginatorTypeDef](./type_defs.md#structuredmessagelistdefinitionpaginatortypedef)
- [StructuredMessageListDefinitionTypeDef](./type_defs.md#structuredmessagelistdefinitiontypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateCampaignRequestRequestTypeDef](./type_defs.md#updatecampaignrequestrequesttypedef)
- [UpdateFleetRequestRequestTypeDef](./type_defs.md#updatefleetrequestrequesttypedef)
- [UpdateModelManifestRequestRequestTypeDef](./type_defs.md#updatemodelmanifestrequestrequesttypedef)
- [UpdateVehicleRequestRequestTypeDef](./type_defs.md#updatevehiclerequestrequesttypedef)
- [ActuatorUnionTypeDef](./type_defs.md#actuatoruniontypedef)
- [AttributeUnionTypeDef](./type_defs.md#attributeuniontypedef)
- [BatchCreateVehicleResponseTypeDef](./type_defs.md#batchcreatevehicleresponsetypedef)
- [CreateCampaignResponseTypeDef](./type_defs.md#createcampaignresponsetypedef)
- [CreateDecoderManifestResponseTypeDef](./type_defs.md#createdecodermanifestresponsetypedef)
- [CreateFleetResponseTypeDef](./type_defs.md#createfleetresponsetypedef)
- [CreateModelManifestResponseTypeDef](./type_defs.md#createmodelmanifestresponsetypedef)
- [CreateSignalCatalogResponseTypeDef](./type_defs.md#createsignalcatalogresponsetypedef)
- [CreateVehicleResponseTypeDef](./type_defs.md#createvehicleresponsetypedef)
- [DeleteCampaignResponseTypeDef](./type_defs.md#deletecampaignresponsetypedef)
- [DeleteDecoderManifestResponseTypeDef](./type_defs.md#deletedecodermanifestresponsetypedef)
- [DeleteFleetResponseTypeDef](./type_defs.md#deletefleetresponsetypedef)
- [DeleteModelManifestResponseTypeDef](./type_defs.md#deletemodelmanifestresponsetypedef)
- [DeleteSignalCatalogResponseTypeDef](./type_defs.md#deletesignalcatalogresponsetypedef)
- [DeleteVehicleResponseTypeDef](./type_defs.md#deletevehicleresponsetypedef)
- [GetDecoderManifestResponseTypeDef](./type_defs.md#getdecodermanifestresponsetypedef)
- [GetEncryptionConfigurationResponseTypeDef](./type_defs.md#getencryptionconfigurationresponsetypedef)
- [GetFleetResponseTypeDef](./type_defs.md#getfleetresponsetypedef)
- [GetModelManifestResponseTypeDef](./type_defs.md#getmodelmanifestresponsetypedef)
- [GetVehicleResponseTypeDef](./type_defs.md#getvehicleresponsetypedef)
- [ImportDecoderManifestResponseTypeDef](./type_defs.md#importdecodermanifestresponsetypedef)
- [ImportSignalCatalogResponseTypeDef](./type_defs.md#importsignalcatalogresponsetypedef)
- [ListFleetsForVehicleResponseTypeDef](./type_defs.md#listfleetsforvehicleresponsetypedef)
- [ListVehiclesInFleetResponseTypeDef](./type_defs.md#listvehiclesinfleetresponsetypedef)
- [PutEncryptionConfigurationResponseTypeDef](./type_defs.md#putencryptionconfigurationresponsetypedef)
- [UpdateCampaignResponseTypeDef](./type_defs.md#updatecampaignresponsetypedef)
- [UpdateDecoderManifestResponseTypeDef](./type_defs.md#updatedecodermanifestresponsetypedef)
- [UpdateFleetResponseTypeDef](./type_defs.md#updatefleetresponsetypedef)
- [UpdateModelManifestResponseTypeDef](./type_defs.md#updatemodelmanifestresponsetypedef)
- [UpdateSignalCatalogResponseTypeDef](./type_defs.md#updatesignalcatalogresponsetypedef)
- [UpdateVehicleResponseTypeDef](./type_defs.md#updatevehicleresponsetypedef)
- [BatchUpdateVehicleRequestRequestTypeDef](./type_defs.md#batchupdatevehiclerequestrequesttypedef)
- [BatchUpdateVehicleResponseTypeDef](./type_defs.md#batchupdatevehicleresponsetypedef)
- [CanDbcDefinitionTypeDef](./type_defs.md#candbcdefinitiontypedef)
- [ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef)
- [GetLoggingOptionsResponseTypeDef](./type_defs.md#getloggingoptionsresponsetypedef)
- [PutLoggingOptionsRequestRequestTypeDef](./type_defs.md#putloggingoptionsrequestrequesttypedef)
- [CollectionSchemeTypeDef](./type_defs.md#collectionschemetypedef)
- [CreateFleetRequestRequestTypeDef](./type_defs.md#createfleetrequestrequesttypedef)
- [CreateModelManifestRequestRequestTypeDef](./type_defs.md#createmodelmanifestrequestrequesttypedef)
- [CreateVehicleRequestItemTypeDef](./type_defs.md#createvehiclerequestitemtypedef)
- [CreateVehicleRequestRequestTypeDef](./type_defs.md#createvehiclerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [DataDestinationConfigTypeDef](./type_defs.md#datadestinationconfigtypedef)
- [ListDecoderManifestsResponseTypeDef](./type_defs.md#listdecodermanifestsresponsetypedef)
- [ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef)
- [ImportSignalCatalogRequestRequestTypeDef](./type_defs.md#importsignalcatalogrequestrequesttypedef)
- [GetRegisterAccountStatusResponseTypeDef](./type_defs.md#getregisteraccountstatusresponsetypedef)
- [GetSignalCatalogResponseTypeDef](./type_defs.md#getsignalcatalogresponsetypedef)
- [GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef](./type_defs.md#getvehiclestatusrequestgetvehiclestatuspaginatetypedef)
- [ListCampaignsRequestListCampaignsPaginateTypeDef](./type_defs.md#listcampaignsrequestlistcampaignspaginatetypedef)
- [ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef](./type_defs.md#listdecodermanifestnetworkinterfacesrequestlistdecodermanifestnetworkinterfacespaginatetypedef)
- [ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef](./type_defs.md#listdecodermanifestsignalsrequestlistdecodermanifestsignalspaginatetypedef)
- [ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef](./type_defs.md#listdecodermanifestsrequestlistdecodermanifestspaginatetypedef)
- [ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef](./type_defs.md#listfleetsforvehiclerequestlistfleetsforvehiclepaginatetypedef)
- [ListFleetsRequestListFleetsPaginateTypeDef](./type_defs.md#listfleetsrequestlistfleetspaginatetypedef)
- [ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef](./type_defs.md#listmodelmanifestnodesrequestlistmodelmanifestnodespaginatetypedef)
- [ListModelManifestsRequestListModelManifestsPaginateTypeDef](./type_defs.md#listmodelmanifestsrequestlistmodelmanifestspaginatetypedef)
- [ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef](./type_defs.md#listsignalcatalognodesrequestlistsignalcatalognodespaginatetypedef)
- [ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef](./type_defs.md#listsignalcatalogsrequestlistsignalcatalogspaginatetypedef)
- [ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef](./type_defs.md#listvehiclesinfleetrequestlistvehiclesinfleetpaginatetypedef)
- [ListVehiclesRequestListVehiclesPaginateTypeDef](./type_defs.md#listvehiclesrequestlistvehiclespaginatetypedef)
- [GetVehicleStatusResponseTypeDef](./type_defs.md#getvehiclestatusresponsetypedef)
- [ListModelManifestsResponseTypeDef](./type_defs.md#listmodelmanifestsresponsetypedef)
- [ListSignalCatalogsResponseTypeDef](./type_defs.md#listsignalcatalogsresponsetypedef)
- [ListVehiclesResponseTypeDef](./type_defs.md#listvehiclesresponsetypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [NodeOutputTypeDef](./type_defs.md#nodeoutputtypedef)
- [PrimitiveMessageDefinitionTypeDef](./type_defs.md#primitivemessagedefinitiontypedef)
- [RegisterAccountRequestRequestTypeDef](./type_defs.md#registeraccountrequestrequesttypedef)
- [RegisterAccountResponseTypeDef](./type_defs.md#registeraccountresponsetypedef)
- [SensorUnionTypeDef](./type_defs.md#sensoruniontypedef)
- [StructuredMessageFieldNameAndDataTypePairUnionTypeDef](./type_defs.md#structuredmessagefieldnameanddatatypepairuniontypedef)
- [StructuredMessageListDefinitionUnionTypeDef](./type_defs.md#structuredmessagelistdefinitionuniontypedef)
- [NetworkFileDefinitionTypeDef](./type_defs.md#networkfiledefinitiontypedef)
- [BatchCreateVehicleRequestRequestTypeDef](./type_defs.md#batchcreatevehiclerequestrequesttypedef)
- [CreateCampaignRequestRequestTypeDef](./type_defs.md#createcampaignrequestrequesttypedef)
- [GetCampaignResponseTypeDef](./type_defs.md#getcampaignresponsetypedef)
- [ListDecoderManifestNetworkInterfacesResponseTypeDef](./type_defs.md#listdecodermanifestnetworkinterfacesresponsetypedef)
- [ListModelManifestNodesResponseTypeDef](./type_defs.md#listmodelmanifestnodesresponsetypedef)
- [ListSignalCatalogNodesResponseTypeDef](./type_defs.md#listsignalcatalognodesresponsetypedef)
- [StructuredMessageOutputTypeDef](./type_defs.md#structuredmessageoutputtypedef)
- [StructuredMessagePaginatorTypeDef](./type_defs.md#structuredmessagepaginatortypedef)
- [NodeTypeDef](./type_defs.md#nodetypedef)
- [StructuredMessageTypeDef](./type_defs.md#structuredmessagetypedef)
- [ImportDecoderManifestRequestRequestTypeDef](./type_defs.md#importdecodermanifestrequestrequesttypedef)
- [MessageSignalOutputTypeDef](./type_defs.md#messagesignaloutputtypedef)
- [MessageSignalPaginatorTypeDef](./type_defs.md#messagesignalpaginatortypedef)
- [NodeUnionTypeDef](./type_defs.md#nodeuniontypedef)
- [UpdateSignalCatalogRequestRequestTypeDef](./type_defs.md#updatesignalcatalogrequestrequesttypedef)
- [StructuredMessageUnionTypeDef](./type_defs.md#structuredmessageuniontypedef)
- [SignalDecoderOutputTypeDef](./type_defs.md#signaldecoderoutputtypedef)
- [SignalDecoderPaginatorTypeDef](./type_defs.md#signaldecoderpaginatortypedef)
- [CreateSignalCatalogRequestRequestTypeDef](./type_defs.md#createsignalcatalogrequestrequesttypedef)
- [MessageSignalTypeDef](./type_defs.md#messagesignaltypedef)
- [ListDecoderManifestSignalsResponseTypeDef](./type_defs.md#listdecodermanifestsignalsresponsetypedef)
- [ListDecoderManifestSignalsResponsePaginatorTypeDef](./type_defs.md#listdecodermanifestsignalsresponsepaginatortypedef)
- [MessageSignalUnionTypeDef](./type_defs.md#messagesignaluniontypedef)
- [SignalDecoderTypeDef](./type_defs.md#signaldecodertypedef)
- [SignalDecoderUnionTypeDef](./type_defs.md#signaldecoderuniontypedef)
- [UpdateDecoderManifestRequestRequestTypeDef](./type_defs.md#updatedecodermanifestrequestrequesttypedef)
- [CreateDecoderManifestRequestRequestTypeDef](./type_defs.md#createdecodermanifestrequestrequesttypedef)

