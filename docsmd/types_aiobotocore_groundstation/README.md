# GroundStation module

> [Index](../README.md) > GroundStation


!!! note ""

    Auto-generated documentation for [GroundStation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
    type annotations stubs module [types-aiobotocore-groundstation](https://pypi.org/project/types-aiobotocore-groundstation/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `GroundStation` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[groundstation]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[groundstation]'


# standalone installation
python -m pip install types-aiobotocore-groundstation
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-groundstation
```

## Usage

Code samples can be found in [Examples](./usage.md).

## GroundStationClient

Type annotations and code completion for  `#!python session.create_client("groundstation")` as [GroundStationClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client)

```python
# GroundStationClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_groundstation.client import GroundStationClient


session = get_session()
async with session.create_client("groundstation") as client:
    client: GroundStationClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("groundstation").get_paginator("...")`.

```python
# ListConfigsPaginator usage example

from types_aiobotocore_groundstation.paginator import ListConfigsPaginator

def get_list_configs_paginator() -> ListConfigsPaginator:
    return client.get_paginator("list_configs"))
```

- [ListConfigsPaginator](./paginators.md#listconfigspaginator)
- [ListContactsPaginator](./paginators.md#listcontactspaginator)
- [ListDataflowEndpointGroupsPaginator](./paginators.md#listdataflowendpointgroupspaginator)
- [ListEphemeridesPaginator](./paginators.md#listephemeridespaginator)
- [ListGroundStationsPaginator](./paginators.md#listgroundstationspaginator)
- [ListMissionProfilesPaginator](./paginators.md#listmissionprofilespaginator)
- [ListSatellitesPaginator](./paginators.md#listsatellitespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("groundstation").get_waiter("...")`.

```python
# ContactScheduledWaiter usage example

from types_aiobotocore_groundstation.waiter import ContactScheduledWaiter

def get_contact_scheduled_waiter() -> ContactScheduledWaiter:
    return Session().client("groundstation").get_waiter("contact_scheduled")
```

- [ContactScheduledWaiter](./waiters.md#contactscheduledwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AgentStatusType usage example

from types_aiobotocore_groundstation.literals import AgentStatusType

def get_value() -> AgentStatusType:
    return "ACTIVE"
```

- [AgentStatusType](./literals.md#agentstatustype)
- [AngleUnitsType](./literals.md#angleunitstype)
- [AuditResultsType](./literals.md#auditresultstype)
- [BandwidthUnitsType](./literals.md#bandwidthunitstype)
- [CapabilityHealthReasonType](./literals.md#capabilityhealthreasontype)
- [CapabilityHealthType](./literals.md#capabilityhealthtype)
- [ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype)
- [ContactScheduledWaiterName](./literals.md#contactscheduledwaitername)
- [ContactStatusType](./literals.md#contactstatustype)
- [CriticalityType](./literals.md#criticalitytype)
- [EirpUnitsType](./literals.md#eirpunitstype)
- [EndpointStatusType](./literals.md#endpointstatustype)
- [EphemerisInvalidReasonType](./literals.md#ephemerisinvalidreasontype)
- [EphemerisSourceType](./literals.md#ephemerissourcetype)
- [EphemerisStatusType](./literals.md#ephemerisstatustype)
- [FrequencyUnitsType](./literals.md#frequencyunitstype)
- [ListConfigsPaginatorName](./literals.md#listconfigspaginatorname)
- [ListContactsPaginatorName](./literals.md#listcontactspaginatorname)
- [ListDataflowEndpointGroupsPaginatorName](./literals.md#listdataflowendpointgroupspaginatorname)
- [ListEphemeridesPaginatorName](./literals.md#listephemeridespaginatorname)
- [ListGroundStationsPaginatorName](./literals.md#listgroundstationspaginatorname)
- [ListMissionProfilesPaginatorName](./literals.md#listmissionprofilespaginatorname)
- [ListSatellitesPaginatorName](./literals.md#listsatellitespaginatorname)
- [PolarizationType](./literals.md#polarizationtype)
- [GroundStationServiceName](./literals.md#groundstationservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ComponentVersionTypeDef](./type_defs.md#componentversiontypedef)
- [AggregateStatusTypeDef](./type_defs.md#aggregatestatustypedef)
- [AntennaDemodDecodeDetailsTypeDef](./type_defs.md#antennademoddecodedetailstypedef)
- [DecodeConfigTypeDef](./type_defs.md#decodeconfigtypedef)
- [DemodulationConfigTypeDef](./type_defs.md#demodulationconfigtypedef)
- [EirpTypeDef](./type_defs.md#eirptypedef)
- [CancelContactRequestRequestTypeDef](./type_defs.md#cancelcontactrequestrequesttypedef)
- [ComponentStatusDataTypeDef](./type_defs.md#componentstatusdatatypedef)
- [S3RecordingDetailsTypeDef](./type_defs.md#s3recordingdetailstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ConfigListItemTypeDef](./type_defs.md#configlistitemtypedef)
- [DataflowEndpointConfigTypeDef](./type_defs.md#dataflowendpointconfigtypedef)
- [S3RecordingConfigTypeDef](./type_defs.md#s3recordingconfigtypedef)
- [TrackingConfigTypeDef](./type_defs.md#trackingconfigtypedef)
- [UplinkEchoConfigTypeDef](./type_defs.md#uplinkechoconfigtypedef)
- [SocketAddressTypeDef](./type_defs.md#socketaddresstypedef)
- [ElevationTypeDef](./type_defs.md#elevationtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [KmsKeyTypeDef](./type_defs.md#kmskeytypedef)
- [DataflowEndpointListItemTypeDef](./type_defs.md#dataflowendpointlistitemtypedef)
- [DeleteConfigRequestRequestTypeDef](./type_defs.md#deleteconfigrequestrequesttypedef)
- [DeleteDataflowEndpointGroupRequestRequestTypeDef](./type_defs.md#deletedataflowendpointgrouprequestrequesttypedef)
- [DeleteEphemerisRequestRequestTypeDef](./type_defs.md#deleteephemerisrequestrequesttypedef)
- [DeleteMissionProfileRequestRequestTypeDef](./type_defs.md#deletemissionprofilerequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeContactRequestRequestTypeDef](./type_defs.md#describecontactrequestrequesttypedef)
- [DescribeEphemerisRequestRequestTypeDef](./type_defs.md#describeephemerisrequestrequesttypedef)
- [DiscoveryDataTypeDef](./type_defs.md#discoverydatatypedef)
- [SecurityDetailsTypeDef](./type_defs.md#securitydetailstypedef)
- [S3ObjectTypeDef](./type_defs.md#s3objecttypedef)
- [EphemerisMetaDataTypeDef](./type_defs.md#ephemerismetadatatypedef)
- [FrequencyBandwidthTypeDef](./type_defs.md#frequencybandwidthtypedef)
- [FrequencyTypeDef](./type_defs.md#frequencytypedef)
- [GetAgentConfigurationRequestRequestTypeDef](./type_defs.md#getagentconfigurationrequestrequesttypedef)
- [GetConfigRequestRequestTypeDef](./type_defs.md#getconfigrequestrequesttypedef)
- [GetDataflowEndpointGroupRequestRequestTypeDef](./type_defs.md#getdataflowendpointgrouprequestrequesttypedef)
- [GetMinuteUsageRequestRequestTypeDef](./type_defs.md#getminuteusagerequestrequesttypedef)
- [GetMissionProfileRequestRequestTypeDef](./type_defs.md#getmissionprofilerequestrequesttypedef)
- [GetSatelliteRequestRequestTypeDef](./type_defs.md#getsatelliterequestrequesttypedef)
- [GroundStationDataTypeDef](./type_defs.md#groundstationdatatypedef)
- [IntegerRangeTypeDef](./type_defs.md#integerrangetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListConfigsRequestRequestTypeDef](./type_defs.md#listconfigsrequestrequesttypedef)
- [ListDataflowEndpointGroupsRequestRequestTypeDef](./type_defs.md#listdataflowendpointgroupsrequestrequesttypedef)
- [ListGroundStationsRequestRequestTypeDef](./type_defs.md#listgroundstationsrequestrequesttypedef)
- [ListMissionProfilesRequestRequestTypeDef](./type_defs.md#listmissionprofilesrequestrequesttypedef)
- [MissionProfileListItemTypeDef](./type_defs.md#missionprofilelistitemtypedef)
- [ListSatellitesRequestRequestTypeDef](./type_defs.md#listsatellitesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateEphemerisRequestRequestTypeDef](./type_defs.md#updateephemerisrequestrequesttypedef)
- [AgentDetailsTypeDef](./type_defs.md#agentdetailstypedef)
- [UpdateAgentStatusRequestRequestTypeDef](./type_defs.md#updateagentstatusrequestrequesttypedef)
- [ConfigIdResponseTypeDef](./type_defs.md#configidresponsetypedef)
- [ContactIdResponseTypeDef](./type_defs.md#contactidresponsetypedef)
- [DataflowEndpointGroupIdResponseTypeDef](./type_defs.md#dataflowendpointgroupidresponsetypedef)
- [EphemerisIdResponseTypeDef](./type_defs.md#ephemerisidresponsetypedef)
- [GetAgentConfigurationResponseTypeDef](./type_defs.md#getagentconfigurationresponsetypedef)
- [GetMinuteUsageResponseTypeDef](./type_defs.md#getminuteusageresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [MissionProfileIdResponseTypeDef](./type_defs.md#missionprofileidresponsetypedef)
- [RegisterAgentResponseTypeDef](./type_defs.md#registeragentresponsetypedef)
- [UpdateAgentStatusResponseTypeDef](./type_defs.md#updateagentstatusresponsetypedef)
- [ListConfigsResponseTypeDef](./type_defs.md#listconfigsresponsetypedef)
- [ConnectionDetailsTypeDef](./type_defs.md#connectiondetailstypedef)
- [DataflowEndpointTypeDef](./type_defs.md#dataflowendpointtypedef)
- [ContactDataTypeDef](./type_defs.md#contactdatatypedef)
- [ListContactsRequestRequestTypeDef](./type_defs.md#listcontactsrequestrequesttypedef)
- [ListEphemeridesRequestRequestTypeDef](./type_defs.md#listephemeridesrequestrequesttypedef)
- [ReserveContactRequestRequestTypeDef](./type_defs.md#reservecontactrequestrequesttypedef)
- [TimeRangeTypeDef](./type_defs.md#timerangetypedef)
- [CreateMissionProfileRequestRequestTypeDef](./type_defs.md#createmissionprofilerequestrequesttypedef)
- [GetMissionProfileResponseTypeDef](./type_defs.md#getmissionprofileresponsetypedef)
- [UpdateMissionProfileRequestRequestTypeDef](./type_defs.md#updatemissionprofilerequestrequesttypedef)
- [ListDataflowEndpointGroupsResponseTypeDef](./type_defs.md#listdataflowendpointgroupsresponsetypedef)
- [DescribeContactRequestContactScheduledWaitTypeDef](./type_defs.md#describecontactrequestcontactscheduledwaittypedef)
- [EphemerisDescriptionTypeDef](./type_defs.md#ephemerisdescriptiontypedef)
- [EphemerisItemTypeDef](./type_defs.md#ephemerisitemtypedef)
- [OEMEphemerisTypeDef](./type_defs.md#oemephemeristypedef)
- [GetSatelliteResponseTypeDef](./type_defs.md#getsatelliteresponsetypedef)
- [SatelliteListItemTypeDef](./type_defs.md#satellitelistitemtypedef)
- [SpectrumConfigTypeDef](./type_defs.md#spectrumconfigtypedef)
- [UplinkSpectrumConfigTypeDef](./type_defs.md#uplinkspectrumconfigtypedef)
- [ListGroundStationsResponseTypeDef](./type_defs.md#listgroundstationsresponsetypedef)
- [RangedSocketAddressTypeDef](./type_defs.md#rangedsocketaddresstypedef)
- [ListConfigsRequestListConfigsPaginateTypeDef](./type_defs.md#listconfigsrequestlistconfigspaginatetypedef)
- [ListContactsRequestListContactsPaginateTypeDef](./type_defs.md#listcontactsrequestlistcontactspaginatetypedef)
- [ListDataflowEndpointGroupsRequestListDataflowEndpointGroupsPaginateTypeDef](./type_defs.md#listdataflowendpointgroupsrequestlistdataflowendpointgroupspaginatetypedef)
- [ListEphemeridesRequestListEphemeridesPaginateTypeDef](./type_defs.md#listephemeridesrequestlistephemeridespaginatetypedef)
- [ListGroundStationsRequestListGroundStationsPaginateTypeDef](./type_defs.md#listgroundstationsrequestlistgroundstationspaginatetypedef)
- [ListMissionProfilesRequestListMissionProfilesPaginateTypeDef](./type_defs.md#listmissionprofilesrequestlistmissionprofilespaginatetypedef)
- [ListSatellitesRequestListSatellitesPaginateTypeDef](./type_defs.md#listsatellitesrequestlistsatellitespaginatetypedef)
- [ListMissionProfilesResponseTypeDef](./type_defs.md#listmissionprofilesresponsetypedef)
- [RegisterAgentRequestRequestTypeDef](./type_defs.md#registeragentrequestrequesttypedef)
- [ListContactsResponseTypeDef](./type_defs.md#listcontactsresponsetypedef)
- [TLEDataTypeDef](./type_defs.md#tledatatypedef)
- [EphemerisTypeDescriptionTypeDef](./type_defs.md#ephemeristypedescriptiontypedef)
- [ListEphemeridesResponseTypeDef](./type_defs.md#listephemeridesresponsetypedef)
- [ListSatellitesResponseTypeDef](./type_defs.md#listsatellitesresponsetypedef)
- [AntennaDownlinkConfigTypeDef](./type_defs.md#antennadownlinkconfigtypedef)
- [AntennaDownlinkDemodDecodeConfigTypeDef](./type_defs.md#antennadownlinkdemoddecodeconfigtypedef)
- [AntennaUplinkConfigTypeDef](./type_defs.md#antennauplinkconfigtypedef)
- [RangedConnectionDetailsTypeDef](./type_defs.md#rangedconnectiondetailstypedef)
- [TLEEphemerisTypeDef](./type_defs.md#tleephemeristypedef)
- [DescribeEphemerisResponseTypeDef](./type_defs.md#describeephemerisresponsetypedef)
- [ConfigTypeDataTypeDef](./type_defs.md#configtypedatatypedef)
- [AwsGroundStationAgentEndpointTypeDef](./type_defs.md#awsgroundstationagentendpointtypedef)
- [EphemerisDataTypeDef](./type_defs.md#ephemerisdatatypedef)
- [CreateConfigRequestRequestTypeDef](./type_defs.md#createconfigrequestrequesttypedef)
- [GetConfigResponseTypeDef](./type_defs.md#getconfigresponsetypedef)
- [UpdateConfigRequestRequestTypeDef](./type_defs.md#updateconfigrequestrequesttypedef)
- [EndpointDetailsTypeDef](./type_defs.md#endpointdetailstypedef)
- [CreateEphemerisRequestRequestTypeDef](./type_defs.md#createephemerisrequestrequesttypedef)
- [ConfigDetailsTypeDef](./type_defs.md#configdetailstypedef)
- [CreateDataflowEndpointGroupRequestRequestTypeDef](./type_defs.md#createdataflowendpointgrouprequestrequesttypedef)
- [GetDataflowEndpointGroupResponseTypeDef](./type_defs.md#getdataflowendpointgroupresponsetypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [DataflowDetailTypeDef](./type_defs.md#dataflowdetailtypedef)
- [DescribeContactResponseTypeDef](./type_defs.md#describecontactresponsetypedef)

