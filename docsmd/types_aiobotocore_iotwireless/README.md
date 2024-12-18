# IoTWireless module

> [Index](../README.md) > IoTWireless


!!! note ""

    Auto-generated documentation for [IoTWireless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#iotwireless)
    type annotations stubs module [types-aiobotocore-iotwireless](https://pypi.org/project/types-aiobotocore-iotwireless/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `IoTWireless` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `IoTWireless` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iotwireless]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iotwireless]'

# standalone installation
python -m pip install types-aiobotocore-iotwireless
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iotwireless
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTWirelessClient

Type annotations and code completion for  `#!python session.create_client("iotwireless")` as [IoTWirelessClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client)

```python
# IoTWirelessClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotwireless.client import IoTWirelessClient


session = get_session()
async with session.create_client("iotwireless") as client:
    client: IoTWirelessClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AggregationPeriodType usage example

from types_aiobotocore_iotwireless.literals import AggregationPeriodType

def get_value() -> AggregationPeriodType:
    return "OneDay"
```

- [AggregationPeriodType](./literals.md#aggregationperiodtype)
- [ApplicationConfigTypeType](./literals.md#applicationconfigtypetype)
- [BatteryLevelType](./literals.md#batteryleveltype)
- [ConnectionStatusType](./literals.md#connectionstatustype)
- [DeviceProfileTypeType](./literals.md#deviceprofiletypetype)
- [DeviceStateType](./literals.md#devicestatetype)
- [DimensionNameType](./literals.md#dimensionnametype)
- [DlClassType](./literals.md#dlclasstype)
- [DownlinkModeType](./literals.md#downlinkmodetype)
- [EventNotificationPartnerTypeType](./literals.md#eventnotificationpartnertypetype)
- [EventNotificationResourceTypeType](./literals.md#eventnotificationresourcetypetype)
- [EventNotificationTopicStatusType](./literals.md#eventnotificationtopicstatustype)
- [EventType](./literals.md#eventtype)
- [ExpressionTypeType](./literals.md#expressiontypetype)
- [FuotaDeviceStatusType](./literals.md#fuotadevicestatustype)
- [FuotaTaskEventType](./literals.md#fuotataskeventtype)
- [FuotaTaskStatusType](./literals.md#fuotataskstatustype)
- [FuotaTaskTypeType](./literals.md#fuotatasktypetype)
- [IdentifierTypeType](./literals.md#identifiertypetype)
- [ImportTaskStatusType](./literals.md#importtaskstatustype)
- [LogLevelType](./literals.md#logleveltype)
- [MessageTypeType](./literals.md#messagetypetype)
- [MetricNameType](./literals.md#metricnametype)
- [MetricQueryStatusType](./literals.md#metricquerystatustype)
- [MulticastFrameInfoType](./literals.md#multicastframeinfotype)
- [OnboardStatusType](./literals.md#onboardstatustype)
- [PartnerTypeType](./literals.md#partnertypetype)
- [PositionConfigurationFecType](./literals.md#positionconfigurationfectype)
- [PositionConfigurationStatusType](./literals.md#positionconfigurationstatustype)
- [PositionResourceTypeType](./literals.md#positionresourcetypetype)
- [PositionSolverProviderType](./literals.md#positionsolverprovidertype)
- [PositionSolverTypeType](./literals.md#positionsolvertypetype)
- [PositioningConfigStatusType](./literals.md#positioningconfigstatustype)
- [SigningAlgType](./literals.md#signingalgtype)
- [SummaryMetricConfigurationStatusType](./literals.md#summarymetricconfigurationstatustype)
- [SupportedRfRegionType](./literals.md#supportedrfregiontype)
- [WirelessDeviceEventType](./literals.md#wirelessdeviceeventtype)
- [WirelessDeviceFrameInfoType](./literals.md#wirelessdeviceframeinfotype)
- [WirelessDeviceIdTypeType](./literals.md#wirelessdeviceidtypetype)
- [WirelessDeviceSidewalkStatusType](./literals.md#wirelessdevicesidewalkstatustype)
- [WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype)
- [WirelessGatewayEventType](./literals.md#wirelessgatewayeventtype)
- [WirelessGatewayIdTypeType](./literals.md#wirelessgatewayidtypetype)
- [WirelessGatewayServiceTypeType](./literals.md#wirelessgatewayservicetypetype)
- [WirelessGatewayTaskDefinitionTypeType](./literals.md#wirelessgatewaytaskdefinitiontypetype)
- [WirelessGatewayTaskStatusType](./literals.md#wirelessgatewaytaskstatustype)
- [WirelessGatewayTypeType](./literals.md#wirelessgatewaytypetype)
- [IoTWirelessServiceName](./literals.md#iotwirelessservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [SessionKeysAbpV10XTypeDef](./type_defs.md#sessionkeysabpv10xtypedef)
- [SessionKeysAbpV11TypeDef](./type_defs.md#sessionkeysabpv11typedef)
- [AccuracyTypeDef](./type_defs.md#accuracytypedef)
- [ApplicationConfigTypeDef](./type_defs.md#applicationconfigtypedef)
- [SidewalkAccountInfoTypeDef](./type_defs.md#sidewalkaccountinfotypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef](./type_defs.md#associatemulticastgroupwithfuotataskrequestrequesttypedef)
- [AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef](./type_defs.md#associatewirelessdevicewithfuotataskrequestrequesttypedef)
- [AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef](./type_defs.md#associatewirelessdevicewithmulticastgrouprequestrequesttypedef)
- [AssociateWirelessDeviceWithThingRequestRequestTypeDef](./type_defs.md#associatewirelessdevicewiththingrequestrequesttypedef)
- [AssociateWirelessGatewayWithCertificateRequestRequestTypeDef](./type_defs.md#associatewirelessgatewaywithcertificaterequestrequesttypedef)
- [AssociateWirelessGatewayWithThingRequestRequestTypeDef](./type_defs.md#associatewirelessgatewaywiththingrequestrequesttypedef)
- [BeaconingOutputTypeDef](./type_defs.md#beaconingoutputtypedef)
- [BeaconingTypeDef](./type_defs.md#beaconingtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelMulticastGroupSessionRequestRequestTypeDef](./type_defs.md#cancelmulticastgroupsessionrequestrequesttypedef)
- [CdmaLocalIdTypeDef](./type_defs.md#cdmalocalidtypedef)
- [CdmaNmrObjTypeDef](./type_defs.md#cdmanmrobjtypedef)
- [CertificateListTypeDef](./type_defs.md#certificatelisttypedef)
- [LoRaWANConnectionStatusEventNotificationConfigurationsTypeDef](./type_defs.md#lorawanconnectionstatuseventnotificationconfigurationstypedef)
- [LoRaWANConnectionStatusResourceTypeEventConfigurationTypeDef](./type_defs.md#lorawanconnectionstatusresourcetypeeventconfigurationtypedef)
- [LoRaWANDeviceProfileTypeDef](./type_defs.md#lorawandeviceprofiletypedef)
- [LoRaWANFuotaTaskTypeDef](./type_defs.md#lorawanfuotatasktypedef)
- [TraceContentTypeDef](./type_defs.md#tracecontenttypedef)
- [LoRaWANServiceProfileTypeDef](./type_defs.md#lorawanserviceprofiletypedef)
- [SidewalkCreateWirelessDeviceTypeDef](./type_defs.md#sidewalkcreatewirelessdevicetypedef)
- [CreateWirelessGatewayTaskRequestRequestTypeDef](./type_defs.md#createwirelessgatewaytaskrequestrequesttypedef)
- [DakCertificateMetadataTypeDef](./type_defs.md#dakcertificatemetadatatypedef)
- [DeleteDestinationRequestRequestTypeDef](./type_defs.md#deletedestinationrequestrequesttypedef)
- [DeleteDeviceProfileRequestRequestTypeDef](./type_defs.md#deletedeviceprofilerequestrequesttypedef)
- [DeleteFuotaTaskRequestRequestTypeDef](./type_defs.md#deletefuotataskrequestrequesttypedef)
- [DeleteMulticastGroupRequestRequestTypeDef](./type_defs.md#deletemulticastgrouprequestrequesttypedef)
- [DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef](./type_defs.md#deletenetworkanalyzerconfigurationrequestrequesttypedef)
- [DeleteQueuedMessagesRequestRequestTypeDef](./type_defs.md#deletequeuedmessagesrequestrequesttypedef)
- [DeleteServiceProfileRequestRequestTypeDef](./type_defs.md#deleteserviceprofilerequestrequesttypedef)
- [DeleteWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#deletewirelessdeviceimporttaskrequestrequesttypedef)
- [DeleteWirelessDeviceRequestRequestTypeDef](./type_defs.md#deletewirelessdevicerequestrequesttypedef)
- [DeleteWirelessGatewayRequestRequestTypeDef](./type_defs.md#deletewirelessgatewayrequestrequesttypedef)
- [DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef](./type_defs.md#deletewirelessgatewaytaskdefinitionrequestrequesttypedef)
- [DeleteWirelessGatewayTaskRequestRequestTypeDef](./type_defs.md#deletewirelessgatewaytaskrequestrequesttypedef)
- [DeregisterWirelessDeviceRequestRequestTypeDef](./type_defs.md#deregisterwirelessdevicerequestrequesttypedef)
- [DestinationsTypeDef](./type_defs.md#destinationstypedef)
- [DeviceProfileTypeDef](./type_defs.md#deviceprofiletypedef)
- [SidewalkEventNotificationConfigurationsTypeDef](./type_defs.md#sidewalkeventnotificationconfigurationstypedef)
- [SidewalkResourceTypeEventConfigurationTypeDef](./type_defs.md#sidewalkresourcetypeeventconfigurationtypedef)
- [DimensionTypeDef](./type_defs.md#dimensiontypedef)
- [DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef](./type_defs.md#disassociateawsaccountfrompartneraccountrequestrequesttypedef)
- [DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef](./type_defs.md#disassociatemulticastgroupfromfuotataskrequestrequesttypedef)
- [DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef](./type_defs.md#disassociatewirelessdevicefromfuotataskrequestrequesttypedef)
- [DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef](./type_defs.md#disassociatewirelessdevicefrommulticastgrouprequestrequesttypedef)
- [DisassociateWirelessDeviceFromThingRequestRequestTypeDef](./type_defs.md#disassociatewirelessdevicefromthingrequestrequesttypedef)
- [DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef](./type_defs.md#disassociatewirelessgatewayfromcertificaterequestrequesttypedef)
- [DisassociateWirelessGatewayFromThingRequestRequestTypeDef](./type_defs.md#disassociatewirelessgatewayfromthingrequestrequesttypedef)
- [PositioningTypeDef](./type_defs.md#positioningtypedef)
- [FuotaTaskEventLogOptionTypeDef](./type_defs.md#fuotataskeventlogoptiontypedef)
- [FuotaTaskTypeDef](./type_defs.md#fuotatasktypedef)
- [GatewayListItemTypeDef](./type_defs.md#gatewaylistitemtypedef)
- [GetDestinationRequestRequestTypeDef](./type_defs.md#getdestinationrequestrequesttypedef)
- [GetDeviceProfileRequestRequestTypeDef](./type_defs.md#getdeviceprofilerequestrequesttypedef)
- [LoRaWANDeviceProfileOutputTypeDef](./type_defs.md#lorawandeviceprofileoutputtypedef)
- [GetFuotaTaskRequestRequestTypeDef](./type_defs.md#getfuotataskrequestrequesttypedef)
- [LoRaWANFuotaTaskGetInfoTypeDef](./type_defs.md#lorawanfuotataskgetinfotypedef)
- [SummaryMetricConfigurationTypeDef](./type_defs.md#summarymetricconfigurationtypedef)
- [GetMulticastGroupRequestRequestTypeDef](./type_defs.md#getmulticastgrouprequestrequesttypedef)
- [GetMulticastGroupSessionRequestRequestTypeDef](./type_defs.md#getmulticastgroupsessionrequestrequesttypedef)
- [LoRaWANMulticastSessionOutputTypeDef](./type_defs.md#lorawanmulticastsessionoutputtypedef)
- [GetNetworkAnalyzerConfigurationRequestRequestTypeDef](./type_defs.md#getnetworkanalyzerconfigurationrequestrequesttypedef)
- [GetPartnerAccountRequestRequestTypeDef](./type_defs.md#getpartneraccountrequestrequesttypedef)
- [SidewalkAccountInfoWithFingerprintTypeDef](./type_defs.md#sidewalkaccountinfowithfingerprinttypedef)
- [GetPositionConfigurationRequestRequestTypeDef](./type_defs.md#getpositionconfigurationrequestrequesttypedef)
- [GnssTypeDef](./type_defs.md#gnsstypedef)
- [IpTypeDef](./type_defs.md#iptypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [WiFiAccessPointTypeDef](./type_defs.md#wifiaccesspointtypedef)
- [GetPositionRequestRequestTypeDef](./type_defs.md#getpositionrequestrequesttypedef)
- [GetResourceEventConfigurationRequestRequestTypeDef](./type_defs.md#getresourceeventconfigurationrequestrequesttypedef)
- [GetResourceLogLevelRequestRequestTypeDef](./type_defs.md#getresourceloglevelrequestrequesttypedef)
- [GetResourcePositionRequestRequestTypeDef](./type_defs.md#getresourcepositionrequestrequesttypedef)
- [GetServiceEndpointRequestRequestTypeDef](./type_defs.md#getserviceendpointrequestrequesttypedef)
- [GetServiceProfileRequestRequestTypeDef](./type_defs.md#getserviceprofilerequestrequesttypedef)
- [LoRaWANGetServiceProfileInfoTypeDef](./type_defs.md#lorawangetserviceprofileinfotypedef)
- [GetWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#getwirelessdeviceimporttaskrequestrequesttypedef)
- [SidewalkGetStartImportInfoTypeDef](./type_defs.md#sidewalkgetstartimportinfotypedef)
- [GetWirelessDeviceRequestRequestTypeDef](./type_defs.md#getwirelessdevicerequestrequesttypedef)
- [GetWirelessDeviceStatisticsRequestRequestTypeDef](./type_defs.md#getwirelessdevicestatisticsrequestrequesttypedef)
- [SidewalkDeviceMetadataTypeDef](./type_defs.md#sidewalkdevicemetadatatypedef)
- [GetWirelessGatewayCertificateRequestRequestTypeDef](./type_defs.md#getwirelessgatewaycertificaterequestrequesttypedef)
- [GetWirelessGatewayFirmwareInformationRequestRequestTypeDef](./type_defs.md#getwirelessgatewayfirmwareinformationrequestrequesttypedef)
- [GetWirelessGatewayRequestRequestTypeDef](./type_defs.md#getwirelessgatewayrequestrequesttypedef)
- [GetWirelessGatewayStatisticsRequestRequestTypeDef](./type_defs.md#getwirelessgatewaystatisticsrequestrequesttypedef)
- [GetWirelessGatewayTaskDefinitionRequestRequestTypeDef](./type_defs.md#getwirelessgatewaytaskdefinitionrequestrequesttypedef)
- [GetWirelessGatewayTaskRequestRequestTypeDef](./type_defs.md#getwirelessgatewaytaskrequestrequesttypedef)
- [GlobalIdentityTypeDef](./type_defs.md#globalidentitytypedef)
- [GsmLocalIdTypeDef](./type_defs.md#gsmlocalidtypedef)
- [ImportedSidewalkDeviceTypeDef](./type_defs.md#importedsidewalkdevicetypedef)
- [LoRaWANJoinEventNotificationConfigurationsTypeDef](./type_defs.md#lorawanjoineventnotificationconfigurationstypedef)
- [LoRaWANJoinResourceTypeEventConfigurationTypeDef](./type_defs.md#lorawanjoinresourcetypeeventconfigurationtypedef)
- [ListDestinationsRequestRequestTypeDef](./type_defs.md#listdestinationsrequestrequesttypedef)
- [ListDeviceProfilesRequestRequestTypeDef](./type_defs.md#listdeviceprofilesrequestrequesttypedef)
- [ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#listdevicesforwirelessdeviceimporttaskrequestrequesttypedef)
- [ListEventConfigurationsRequestRequestTypeDef](./type_defs.md#listeventconfigurationsrequestrequesttypedef)
- [ListFuotaTasksRequestRequestTypeDef](./type_defs.md#listfuotatasksrequestrequesttypedef)
- [ListMulticastGroupsByFuotaTaskRequestRequestTypeDef](./type_defs.md#listmulticastgroupsbyfuotataskrequestrequesttypedef)
- [MulticastGroupByFuotaTaskTypeDef](./type_defs.md#multicastgroupbyfuotatasktypedef)
- [ListMulticastGroupsRequestRequestTypeDef](./type_defs.md#listmulticastgroupsrequestrequesttypedef)
- [MulticastGroupTypeDef](./type_defs.md#multicastgrouptypedef)
- [ListNetworkAnalyzerConfigurationsRequestRequestTypeDef](./type_defs.md#listnetworkanalyzerconfigurationsrequestrequesttypedef)
- [NetworkAnalyzerConfigurationsTypeDef](./type_defs.md#networkanalyzerconfigurationstypedef)
- [ListPartnerAccountsRequestRequestTypeDef](./type_defs.md#listpartneraccountsrequestrequesttypedef)
- [ListPositionConfigurationsRequestRequestTypeDef](./type_defs.md#listpositionconfigurationsrequestrequesttypedef)
- [ListQueuedMessagesRequestRequestTypeDef](./type_defs.md#listqueuedmessagesrequestrequesttypedef)
- [ListServiceProfilesRequestRequestTypeDef](./type_defs.md#listserviceprofilesrequestrequesttypedef)
- [ServiceProfileTypeDef](./type_defs.md#serviceprofiletypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWirelessDeviceImportTasksRequestRequestTypeDef](./type_defs.md#listwirelessdeviceimporttasksrequestrequesttypedef)
- [ListWirelessDevicesRequestRequestTypeDef](./type_defs.md#listwirelessdevicesrequestrequesttypedef)
- [ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef](./type_defs.md#listwirelessgatewaytaskdefinitionsrequestrequesttypedef)
- [ListWirelessGatewaysRequestRequestTypeDef](./type_defs.md#listwirelessgatewaysrequestrequesttypedef)
- [LoRaWANGatewayMetadataTypeDef](./type_defs.md#lorawangatewaymetadatatypedef)
- [LoRaWANPublicGatewayMetadataTypeDef](./type_defs.md#lorawanpublicgatewaymetadatatypedef)
- [OtaaV10XTypeDef](./type_defs.md#otaav10xtypedef)
- [OtaaV11TypeDef](./type_defs.md#otaav11typedef)
- [LoRaWANGatewayVersionTypeDef](./type_defs.md#lorawangatewayversiontypedef)
- [LoRaWANListDeviceTypeDef](./type_defs.md#lorawanlistdevicetypedef)
- [ParticipatingGatewaysMulticastOutputTypeDef](./type_defs.md#participatinggatewaysmulticastoutputtypedef)
- [LoRaWANMulticastMetadataTypeDef](./type_defs.md#lorawanmulticastmetadatatypedef)
- [UpdateAbpV10XTypeDef](./type_defs.md#updateabpv10xtypedef)
- [UpdateAbpV11TypeDef](./type_defs.md#updateabpv11typedef)
- [LteLocalIdTypeDef](./type_defs.md#ltelocalidtypedef)
- [LteNmrObjTypeDef](./type_defs.md#ltenmrobjtypedef)
- [MetricQueryValueTypeDef](./type_defs.md#metricqueryvaluetypedef)
- [ParticipatingGatewaysMulticastTypeDef](./type_defs.md#participatinggatewaysmulticasttypedef)
- [SemtechGnssConfigurationTypeDef](./type_defs.md#semtechgnssconfigurationtypedef)
- [SemtechGnssDetailTypeDef](./type_defs.md#semtechgnssdetailtypedef)
- [PutResourceLogLevelRequestRequestTypeDef](./type_defs.md#putresourceloglevelrequestrequesttypedef)
- [ResetResourceLogLevelRequestRequestTypeDef](./type_defs.md#resetresourceloglevelrequestrequesttypedef)
- [SidewalkSendDataToDeviceTypeDef](./type_defs.md#sidewalksenddatatodevicetypedef)
- [SidewalkSingleStartImportInfoTypeDef](./type_defs.md#sidewalksinglestartimportinfotypedef)
- [SidewalkStartImportInfoTypeDef](./type_defs.md#sidewalkstartimportinfotypedef)
- [SidewalkUpdateAccountTypeDef](./type_defs.md#sidewalkupdateaccounttypedef)
- [SidewalkUpdateImportInfoTypeDef](./type_defs.md#sidewalkupdateimportinfotypedef)
- [TdscdmaLocalIdTypeDef](./type_defs.md#tdscdmalocalidtypedef)
- [TdscdmaNmrObjTypeDef](./type_defs.md#tdscdmanmrobjtypedef)
- [TestWirelessDeviceRequestRequestTypeDef](./type_defs.md#testwirelessdevicerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDestinationRequestRequestTypeDef](./type_defs.md#updatedestinationrequestrequesttypedef)
- [UpdatePositionRequestRequestTypeDef](./type_defs.md#updatepositionrequestrequesttypedef)
- [UpdateWirelessGatewayRequestRequestTypeDef](./type_defs.md#updatewirelessgatewayrequestrequesttypedef)
- [WcdmaLocalIdTypeDef](./type_defs.md#wcdmalocalidtypedef)
- [WcdmaNmrObjTypeDef](./type_defs.md#wcdmanmrobjtypedef)
- [WirelessDeviceEventLogOptionTypeDef](./type_defs.md#wirelessdeviceeventlogoptiontypedef)
- [WirelessGatewayEventLogOptionTypeDef](./type_defs.md#wirelessgatewayeventlogoptiontypedef)
- [AbpV10XTypeDef](./type_defs.md#abpv10xtypedef)
- [AbpV11TypeDef](./type_defs.md#abpv11typedef)
- [AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef](./type_defs.md#associateawsaccountwithpartneraccountrequestrequesttypedef)
- [CreateDestinationRequestRequestTypeDef](./type_defs.md#createdestinationrequestrequesttypedef)
- [StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef](./type_defs.md#startbulkassociatewirelessdevicewithmulticastgrouprequestrequesttypedef)
- [StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef](./type_defs.md#startbulkdisassociatewirelessdevicefrommulticastgrouprequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [AssociateAwsAccountWithPartnerAccountResponseTypeDef](./type_defs.md#associateawsaccountwithpartneraccountresponsetypedef)
- [AssociateWirelessGatewayWithCertificateResponseTypeDef](./type_defs.md#associatewirelessgatewaywithcertificateresponsetypedef)
- [CreateDestinationResponseTypeDef](./type_defs.md#createdestinationresponsetypedef)
- [CreateDeviceProfileResponseTypeDef](./type_defs.md#createdeviceprofileresponsetypedef)
- [CreateFuotaTaskResponseTypeDef](./type_defs.md#createfuotataskresponsetypedef)
- [CreateMulticastGroupResponseTypeDef](./type_defs.md#createmulticastgroupresponsetypedef)
- [CreateNetworkAnalyzerConfigurationResponseTypeDef](./type_defs.md#createnetworkanalyzerconfigurationresponsetypedef)
- [CreateServiceProfileResponseTypeDef](./type_defs.md#createserviceprofileresponsetypedef)
- [CreateWirelessDeviceResponseTypeDef](./type_defs.md#createwirelessdeviceresponsetypedef)
- [CreateWirelessGatewayResponseTypeDef](./type_defs.md#createwirelessgatewayresponsetypedef)
- [CreateWirelessGatewayTaskDefinitionResponseTypeDef](./type_defs.md#createwirelessgatewaytaskdefinitionresponsetypedef)
- [CreateWirelessGatewayTaskResponseTypeDef](./type_defs.md#createwirelessgatewaytaskresponsetypedef)
- [GetDestinationResponseTypeDef](./type_defs.md#getdestinationresponsetypedef)
- [GetPositionEstimateResponseTypeDef](./type_defs.md#getpositionestimateresponsetypedef)
- [GetPositionResponseTypeDef](./type_defs.md#getpositionresponsetypedef)
- [GetResourceLogLevelResponseTypeDef](./type_defs.md#getresourceloglevelresponsetypedef)
- [GetResourcePositionResponseTypeDef](./type_defs.md#getresourcepositionresponsetypedef)
- [GetServiceEndpointResponseTypeDef](./type_defs.md#getserviceendpointresponsetypedef)
- [GetWirelessGatewayCertificateResponseTypeDef](./type_defs.md#getwirelessgatewaycertificateresponsetypedef)
- [GetWirelessGatewayStatisticsResponseTypeDef](./type_defs.md#getwirelessgatewaystatisticsresponsetypedef)
- [GetWirelessGatewayTaskResponseTypeDef](./type_defs.md#getwirelessgatewaytaskresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [SendDataToMulticastGroupResponseTypeDef](./type_defs.md#senddatatomulticastgroupresponsetypedef)
- [SendDataToWirelessDeviceResponseTypeDef](./type_defs.md#senddatatowirelessdeviceresponsetypedef)
- [StartSingleWirelessDeviceImportTaskResponseTypeDef](./type_defs.md#startsinglewirelessdeviceimporttaskresponsetypedef)
- [StartWirelessDeviceImportTaskResponseTypeDef](./type_defs.md#startwirelessdeviceimporttaskresponsetypedef)
- [TestWirelessDeviceResponseTypeDef](./type_defs.md#testwirelessdeviceresponsetypedef)
- [LoRaWANGatewayOutputTypeDef](./type_defs.md#lorawangatewayoutputtypedef)
- [BeaconingUnionTypeDef](./type_defs.md#beaconinguniontypedef)
- [UpdateResourcePositionRequestRequestTypeDef](./type_defs.md#updateresourcepositionrequestrequesttypedef)
- [CdmaObjTypeDef](./type_defs.md#cdmaobjtypedef)
- [SidewalkDeviceTypeDef](./type_defs.md#sidewalkdevicetypedef)
- [SidewalkListDeviceTypeDef](./type_defs.md#sidewalklistdevicetypedef)
- [ConnectionStatusEventConfigurationTypeDef](./type_defs.md#connectionstatuseventconfigurationtypedef)
- [ConnectionStatusResourceTypeEventConfigurationTypeDef](./type_defs.md#connectionstatusresourcetypeeventconfigurationtypedef)
- [CreateDeviceProfileRequestRequestTypeDef](./type_defs.md#createdeviceprofilerequestrequesttypedef)
- [CreateFuotaTaskRequestRequestTypeDef](./type_defs.md#createfuotataskrequestrequesttypedef)
- [UpdateFuotaTaskRequestRequestTypeDef](./type_defs.md#updatefuotataskrequestrequesttypedef)
- [CreateNetworkAnalyzerConfigurationRequestRequestTypeDef](./type_defs.md#createnetworkanalyzerconfigurationrequestrequesttypedef)
- [GetNetworkAnalyzerConfigurationResponseTypeDef](./type_defs.md#getnetworkanalyzerconfigurationresponsetypedef)
- [UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef](./type_defs.md#updatenetworkanalyzerconfigurationrequestrequesttypedef)
- [CreateServiceProfileRequestRequestTypeDef](./type_defs.md#createserviceprofilerequestrequesttypedef)
- [SidewalkGetDeviceProfileTypeDef](./type_defs.md#sidewalkgetdeviceprofiletypedef)
- [ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef)
- [ListDeviceProfilesResponseTypeDef](./type_defs.md#listdeviceprofilesresponsetypedef)
- [DeviceRegistrationStateEventConfigurationTypeDef](./type_defs.md#deviceregistrationstateeventconfigurationtypedef)
- [MessageDeliveryStatusEventConfigurationTypeDef](./type_defs.md#messagedeliverystatuseventconfigurationtypedef)
- [ProximityEventConfigurationTypeDef](./type_defs.md#proximityeventconfigurationtypedef)
- [DeviceRegistrationStateResourceTypeEventConfigurationTypeDef](./type_defs.md#deviceregistrationstateresourcetypeeventconfigurationtypedef)
- [MessageDeliveryStatusResourceTypeEventConfigurationTypeDef](./type_defs.md#messagedeliverystatusresourcetypeeventconfigurationtypedef)
- [ProximityResourceTypeEventConfigurationTypeDef](./type_defs.md#proximityresourcetypeeventconfigurationtypedef)
- [FPortsOutputTypeDef](./type_defs.md#fportsoutputtypedef)
- [FPortsTypeDef](./type_defs.md#fportstypedef)
- [UpdateFPortsTypeDef](./type_defs.md#updatefportstypedef)
- [FuotaTaskLogOptionOutputTypeDef](./type_defs.md#fuotatasklogoptionoutputtypedef)
- [FuotaTaskLogOptionTypeDef](./type_defs.md#fuotatasklogoptiontypedef)
- [ListFuotaTasksResponseTypeDef](./type_defs.md#listfuotatasksresponsetypedef)
- [ParticipatingGatewaysOutputTypeDef](./type_defs.md#participatinggatewaysoutputtypedef)
- [ParticipatingGatewaysTypeDef](./type_defs.md#participatinggatewaystypedef)
- [GetFuotaTaskResponseTypeDef](./type_defs.md#getfuotataskresponsetypedef)
- [GetMetricConfigurationResponseTypeDef](./type_defs.md#getmetricconfigurationresponsetypedef)
- [UpdateMetricConfigurationRequestRequestTypeDef](./type_defs.md#updatemetricconfigurationrequestrequesttypedef)
- [GetMulticastGroupSessionResponseTypeDef](./type_defs.md#getmulticastgroupsessionresponsetypedef)
- [GetPartnerAccountResponseTypeDef](./type_defs.md#getpartneraccountresponsetypedef)
- [ListPartnerAccountsResponseTypeDef](./type_defs.md#listpartneraccountsresponsetypedef)
- [LoRaWANMulticastSessionTypeDef](./type_defs.md#lorawanmulticastsessiontypedef)
- [LoRaWANStartFuotaTaskTypeDef](./type_defs.md#lorawanstartfuotatasktypedef)
- [SummaryMetricQueryTypeDef](./type_defs.md#summarymetricquerytypedef)
- [GetServiceProfileResponseTypeDef](./type_defs.md#getserviceprofileresponsetypedef)
- [GetWirelessDeviceImportTaskResponseTypeDef](./type_defs.md#getwirelessdeviceimporttaskresponsetypedef)
- [WirelessDeviceImportTaskTypeDef](./type_defs.md#wirelessdeviceimporttasktypedef)
- [GsmNmrObjTypeDef](./type_defs.md#gsmnmrobjtypedef)
- [ImportedWirelessDeviceTypeDef](./type_defs.md#importedwirelessdevicetypedef)
- [JoinEventConfigurationTypeDef](./type_defs.md#joineventconfigurationtypedef)
- [JoinResourceTypeEventConfigurationTypeDef](./type_defs.md#joinresourcetypeeventconfigurationtypedef)
- [ListMulticastGroupsByFuotaTaskResponseTypeDef](./type_defs.md#listmulticastgroupsbyfuotataskresponsetypedef)
- [ListMulticastGroupsResponseTypeDef](./type_defs.md#listmulticastgroupsresponsetypedef)
- [ListNetworkAnalyzerConfigurationsResponseTypeDef](./type_defs.md#listnetworkanalyzerconfigurationsresponsetypedef)
- [ListServiceProfilesResponseTypeDef](./type_defs.md#listserviceprofilesresponsetypedef)
- [LoRaWANDeviceMetadataTypeDef](./type_defs.md#lorawandevicemetadatatypedef)
- [LoRaWANGatewayCurrentVersionTypeDef](./type_defs.md#lorawangatewaycurrentversiontypedef)
- [LoRaWANUpdateGatewayTaskCreateTypeDef](./type_defs.md#lorawanupdategatewaytaskcreatetypedef)
- [LoRaWANUpdateGatewayTaskEntryTypeDef](./type_defs.md#lorawanupdategatewaytaskentrytypedef)
- [LoRaWANMulticastGetTypeDef](./type_defs.md#lorawanmulticastgettypedef)
- [MulticastWirelessMetadataTypeDef](./type_defs.md#multicastwirelessmetadatatypedef)
- [LteObjTypeDef](./type_defs.md#lteobjtypedef)
- [SummaryMetricQueryResultTypeDef](./type_defs.md#summarymetricqueryresulttypedef)
- [ParticipatingGatewaysMulticastUnionTypeDef](./type_defs.md#participatinggatewaysmulticastuniontypedef)
- [PositionSolverConfigurationsTypeDef](./type_defs.md#positionsolverconfigurationstypedef)
- [PositionSolverDetailsTypeDef](./type_defs.md#positionsolverdetailstypedef)
- [StartSingleWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#startsinglewirelessdeviceimporttaskrequestrequesttypedef)
- [StartWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#startwirelessdeviceimporttaskrequestrequesttypedef)
- [UpdatePartnerAccountRequestRequestTypeDef](./type_defs.md#updatepartneraccountrequestrequesttypedef)
- [UpdateWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#updatewirelessdeviceimporttaskrequestrequesttypedef)
- [TdscdmaObjTypeDef](./type_defs.md#tdscdmaobjtypedef)
- [WcdmaObjTypeDef](./type_defs.md#wcdmaobjtypedef)
- [WirelessDeviceLogOptionOutputTypeDef](./type_defs.md#wirelessdevicelogoptionoutputtypedef)
- [WirelessDeviceLogOptionTypeDef](./type_defs.md#wirelessdevicelogoptiontypedef)
- [WirelessGatewayLogOptionOutputTypeDef](./type_defs.md#wirelessgatewaylogoptionoutputtypedef)
- [WirelessGatewayLogOptionTypeDef](./type_defs.md#wirelessgatewaylogoptiontypedef)
- [GetWirelessGatewayResponseTypeDef](./type_defs.md#getwirelessgatewayresponsetypedef)
- [WirelessGatewayStatisticsTypeDef](./type_defs.md#wirelessgatewaystatisticstypedef)
- [LoRaWANGatewayTypeDef](./type_defs.md#lorawangatewaytypedef)
- [WirelessDeviceStatisticsTypeDef](./type_defs.md#wirelessdevicestatisticstypedef)
- [GetDeviceProfileResponseTypeDef](./type_defs.md#getdeviceprofileresponsetypedef)
- [LoRaWANDeviceOutputTypeDef](./type_defs.md#lorawandeviceoutputtypedef)
- [FPortsUnionTypeDef](./type_defs.md#fportsuniontypedef)
- [LoRaWANUpdateDeviceTypeDef](./type_defs.md#lorawanupdatedevicetypedef)
- [FuotaTaskLogOptionUnionTypeDef](./type_defs.md#fuotatasklogoptionuniontypedef)
- [LoRaWANSendDataToDeviceOutputTypeDef](./type_defs.md#lorawansenddatatodeviceoutputtypedef)
- [ParticipatingGatewaysUnionTypeDef](./type_defs.md#participatinggatewaysuniontypedef)
- [StartMulticastGroupSessionRequestRequestTypeDef](./type_defs.md#startmulticastgroupsessionrequestrequesttypedef)
- [StartFuotaTaskRequestRequestTypeDef](./type_defs.md#startfuotataskrequestrequesttypedef)
- [GetMetricsRequestRequestTypeDef](./type_defs.md#getmetricsrequestrequesttypedef)
- [ListWirelessDeviceImportTasksResponseTypeDef](./type_defs.md#listwirelessdeviceimporttasksresponsetypedef)
- [GsmObjTypeDef](./type_defs.md#gsmobjtypedef)
- [ListDevicesForWirelessDeviceImportTaskResponseTypeDef](./type_defs.md#listdevicesforwirelessdeviceimporttaskresponsetypedef)
- [EventNotificationItemConfigurationsTypeDef](./type_defs.md#eventnotificationitemconfigurationstypedef)
- [GetResourceEventConfigurationResponseTypeDef](./type_defs.md#getresourceeventconfigurationresponsetypedef)
- [UpdateResourceEventConfigurationRequestRequestTypeDef](./type_defs.md#updateresourceeventconfigurationrequestrequesttypedef)
- [GetEventConfigurationByResourceTypesResponseTypeDef](./type_defs.md#geteventconfigurationbyresourcetypesresponsetypedef)
- [UpdateEventConfigurationByResourceTypesRequestRequestTypeDef](./type_defs.md#updateeventconfigurationbyresourcetypesrequestrequesttypedef)
- [GetWirelessDeviceStatisticsResponseTypeDef](./type_defs.md#getwirelessdevicestatisticsresponsetypedef)
- [GetWirelessGatewayFirmwareInformationResponseTypeDef](./type_defs.md#getwirelessgatewayfirmwareinformationresponsetypedef)
- [UpdateWirelessGatewayTaskCreateTypeDef](./type_defs.md#updatewirelessgatewaytaskcreatetypedef)
- [UpdateWirelessGatewayTaskEntryTypeDef](./type_defs.md#updatewirelessgatewaytaskentrytypedef)
- [GetMulticastGroupResponseTypeDef](./type_defs.md#getmulticastgroupresponsetypedef)
- [SendDataToMulticastGroupRequestRequestTypeDef](./type_defs.md#senddatatomulticastgrouprequestrequesttypedef)
- [GetMetricsResponseTypeDef](./type_defs.md#getmetricsresponsetypedef)
- [LoRaWANMulticastTypeDef](./type_defs.md#lorawanmulticasttypedef)
- [PutPositionConfigurationRequestRequestTypeDef](./type_defs.md#putpositionconfigurationrequestrequesttypedef)
- [GetPositionConfigurationResponseTypeDef](./type_defs.md#getpositionconfigurationresponsetypedef)
- [PositionConfigurationItemTypeDef](./type_defs.md#positionconfigurationitemtypedef)
- [WirelessDeviceLogOptionUnionTypeDef](./type_defs.md#wirelessdevicelogoptionuniontypedef)
- [GetLogLevelsByResourceTypesResponseTypeDef](./type_defs.md#getloglevelsbyresourcetypesresponsetypedef)
- [WirelessGatewayLogOptionUnionTypeDef](./type_defs.md#wirelessgatewaylogoptionuniontypedef)
- [ListWirelessGatewaysResponseTypeDef](./type_defs.md#listwirelessgatewaysresponsetypedef)
- [CreateWirelessGatewayRequestRequestTypeDef](./type_defs.md#createwirelessgatewayrequestrequesttypedef)
- [ListWirelessDevicesResponseTypeDef](./type_defs.md#listwirelessdevicesresponsetypedef)
- [GetWirelessDeviceResponseTypeDef](./type_defs.md#getwirelessdeviceresponsetypedef)
- [LoRaWANDeviceTypeDef](./type_defs.md#lorawandevicetypedef)
- [UpdateWirelessDeviceRequestRequestTypeDef](./type_defs.md#updatewirelessdevicerequestrequesttypedef)
- [DownlinkQueueMessageTypeDef](./type_defs.md#downlinkqueuemessagetypedef)
- [LoRaWANSendDataToDeviceTypeDef](./type_defs.md#lorawansenddatatodevicetypedef)
- [CellTowersTypeDef](./type_defs.md#celltowerstypedef)
- [EventConfigurationItemTypeDef](./type_defs.md#eventconfigurationitemtypedef)
- [CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef](./type_defs.md#createwirelessgatewaytaskdefinitionrequestrequesttypedef)
- [GetWirelessGatewayTaskDefinitionResponseTypeDef](./type_defs.md#getwirelessgatewaytaskdefinitionresponsetypedef)
- [ListWirelessGatewayTaskDefinitionsResponseTypeDef](./type_defs.md#listwirelessgatewaytaskdefinitionsresponsetypedef)
- [CreateMulticastGroupRequestRequestTypeDef](./type_defs.md#createmulticastgrouprequestrequesttypedef)
- [UpdateMulticastGroupRequestRequestTypeDef](./type_defs.md#updatemulticastgrouprequestrequesttypedef)
- [ListPositionConfigurationsResponseTypeDef](./type_defs.md#listpositionconfigurationsresponsetypedef)
- [UpdateLogLevelsByResourceTypesRequestRequestTypeDef](./type_defs.md#updateloglevelsbyresourcetypesrequestrequesttypedef)
- [CreateWirelessDeviceRequestRequestTypeDef](./type_defs.md#createwirelessdevicerequestrequesttypedef)
- [ListQueuedMessagesResponseTypeDef](./type_defs.md#listqueuedmessagesresponsetypedef)
- [LoRaWANSendDataToDeviceUnionTypeDef](./type_defs.md#lorawansenddatatodeviceuniontypedef)
- [GetPositionEstimateRequestRequestTypeDef](./type_defs.md#getpositionestimaterequestrequesttypedef)
- [ListEventConfigurationsResponseTypeDef](./type_defs.md#listeventconfigurationsresponsetypedef)
- [WirelessMetadataTypeDef](./type_defs.md#wirelessmetadatatypedef)
- [SendDataToWirelessDeviceRequestRequestTypeDef](./type_defs.md#senddatatowirelessdevicerequestrequesttypedef)

