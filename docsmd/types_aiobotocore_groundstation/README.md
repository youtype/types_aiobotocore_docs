# GroundStation module

> [Index](../README.md) > GroundStation


!!! note ""

    Auto-generated documentation for [GroundStation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#groundstation)
    type annotations stubs module [types-aiobotocore-groundstation](https://pypi.org/project/types-aiobotocore-groundstation/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `GroundStation` service.
1. Use provided commands to install generated packages.



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
- [EphemerisErrorCodeType](./literals.md#ephemeriserrorcodetype)
- [EphemerisInvalidReasonType](./literals.md#ephemerisinvalidreasontype)
- [EphemerisSourceType](./literals.md#ephemerissourcetype)
- [EphemerisStatusType](./literals.md#ephemerisstatustype)
- [EphemerisTypeType](./literals.md#ephemeristypetype)
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
- [AzElEphemerisFilterTypeDef](./type_defs.md#azelephemerisfiltertypedef)
- [AzElProgramTrackSettingsTypeDef](./type_defs.md#azelprogramtracksettingstypedef)
- [TimeAzElTypeDef](./type_defs.md#timeazeltypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [S3ObjectTypeDef](./type_defs.md#s3objecttypedef)
- [CancelContactRequestTypeDef](./type_defs.md#cancelcontactrequesttypedef)
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
- [EphemerisResponseDataTypeDef](./type_defs.md#ephemerisresponsedatatypedef)
- [KmsKeyTypeDef](./type_defs.md#kmskeytypedef)
- [DataflowEndpointListItemTypeDef](./type_defs.md#dataflowendpointlistitemtypedef)
- [DeleteConfigRequestTypeDef](./type_defs.md#deleteconfigrequesttypedef)
- [DeleteDataflowEndpointGroupRequestTypeDef](./type_defs.md#deletedataflowendpointgrouprequesttypedef)
- [DeleteEphemerisRequestTypeDef](./type_defs.md#deleteephemerisrequesttypedef)
- [DeleteMissionProfileRequestTypeDef](./type_defs.md#deletemissionprofilerequesttypedef)
- [DescribeContactRequestTypeDef](./type_defs.md#describecontactrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeEphemerisRequestTypeDef](./type_defs.md#describeephemerisrequesttypedef)
- [EphemerisErrorReasonTypeDef](./type_defs.md#ephemeriserrorreasontypedef)
- [DiscoveryDataTypeDef](./type_defs.md#discoverydatatypedef)
- [SecurityDetailsOutputTypeDef](./type_defs.md#securitydetailsoutputtypedef)
- [EphemerisMetaDataTypeDef](./type_defs.md#ephemerismetadatatypedef)
- [FrequencyBandwidthTypeDef](./type_defs.md#frequencybandwidthtypedef)
- [FrequencyTypeDef](./type_defs.md#frequencytypedef)
- [GetAgentConfigurationRequestTypeDef](./type_defs.md#getagentconfigurationrequesttypedef)
- [GetAgentTaskResponseUrlRequestTypeDef](./type_defs.md#getagenttaskresponseurlrequesttypedef)
- [GetConfigRequestTypeDef](./type_defs.md#getconfigrequesttypedef)
- [GetDataflowEndpointGroupRequestTypeDef](./type_defs.md#getdataflowendpointgrouprequesttypedef)
- [GetMinuteUsageRequestTypeDef](./type_defs.md#getminuteusagerequesttypedef)
- [GetMissionProfileRequestTypeDef](./type_defs.md#getmissionprofilerequesttypedef)
- [GetSatelliteRequestTypeDef](./type_defs.md#getsatelliterequesttypedef)
- [GroundStationDataTypeDef](./type_defs.md#groundstationdatatypedef)
- [IntegerRangeTypeDef](./type_defs.md#integerrangetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListConfigsRequestTypeDef](./type_defs.md#listconfigsrequesttypedef)
- [ListDataflowEndpointGroupsRequestTypeDef](./type_defs.md#listdataflowendpointgroupsrequesttypedef)
- [ListGroundStationsRequestTypeDef](./type_defs.md#listgroundstationsrequesttypedef)
- [ListMissionProfilesRequestTypeDef](./type_defs.md#listmissionprofilesrequesttypedef)
- [MissionProfileListItemTypeDef](./type_defs.md#missionprofilelistitemtypedef)
- [ListSatellitesRequestTypeDef](./type_defs.md#listsatellitesrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [SecurityDetailsTypeDef](./type_defs.md#securitydetailstypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateEphemerisRequestTypeDef](./type_defs.md#updateephemerisrequesttypedef)
- [AgentDetailsTypeDef](./type_defs.md#agentdetailstypedef)
- [EphemerisFilterTypeDef](./type_defs.md#ephemerisfiltertypedef)
- [ProgramTrackSettingsTypeDef](./type_defs.md#programtracksettingstypedef)
- [ISO8601TimeRangeTypeDef](./type_defs.md#iso8601timerangetypedef)
- [ListEphemeridesRequestTypeDef](./type_defs.md#listephemeridesrequesttypedef)
- [TimeRangeTypeDef](./type_defs.md#timerangetypedef)
- [EphemerisDescriptionTypeDef](./type_defs.md#ephemerisdescriptiontypedef)
- [EphemerisItemTypeDef](./type_defs.md#ephemerisitemtypedef)
- [OEMEphemerisTypeDef](./type_defs.md#oemephemeristypedef)
- [UpdateAgentStatusRequestTypeDef](./type_defs.md#updateagentstatusrequesttypedef)
- [ConfigIdResponseTypeDef](./type_defs.md#configidresponsetypedef)
- [ContactIdResponseTypeDef](./type_defs.md#contactidresponsetypedef)
- [CreateDataflowEndpointGroupV2ResponseTypeDef](./type_defs.md#createdataflowendpointgroupv2responsetypedef)
- [DataflowEndpointGroupIdResponseTypeDef](./type_defs.md#dataflowendpointgroupidresponsetypedef)
- [EphemerisIdResponseTypeDef](./type_defs.md#ephemerisidresponsetypedef)
- [GetAgentConfigurationResponseTypeDef](./type_defs.md#getagentconfigurationresponsetypedef)
- [GetAgentTaskResponseUrlResponseTypeDef](./type_defs.md#getagenttaskresponseurlresponsetypedef)
- [GetMinuteUsageResponseTypeDef](./type_defs.md#getminuteusageresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [MissionProfileIdResponseTypeDef](./type_defs.md#missionprofileidresponsetypedef)
- [RegisterAgentResponseTypeDef](./type_defs.md#registeragentresponsetypedef)
- [UpdateAgentStatusResponseTypeDef](./type_defs.md#updateagentstatusresponsetypedef)
- [ListConfigsResponseTypeDef](./type_defs.md#listconfigsresponsetypedef)
- [ConnectionDetailsTypeDef](./type_defs.md#connectiondetailstypedef)
- [DataflowEndpointTypeDef](./type_defs.md#dataflowendpointtypedef)
- [ContactDataTypeDef](./type_defs.md#contactdatatypedef)
- [CreateMissionProfileRequestTypeDef](./type_defs.md#createmissionprofilerequesttypedef)
- [GetMissionProfileResponseTypeDef](./type_defs.md#getmissionprofileresponsetypedef)
- [UpdateMissionProfileRequestTypeDef](./type_defs.md#updatemissionprofilerequesttypedef)
- [ListDataflowEndpointGroupsResponseTypeDef](./type_defs.md#listdataflowendpointgroupsresponsetypedef)
- [DescribeContactRequestWaitTypeDef](./type_defs.md#describecontactrequestwaittypedef)
- [GetSatelliteResponseTypeDef](./type_defs.md#getsatelliteresponsetypedef)
- [SatelliteListItemTypeDef](./type_defs.md#satellitelistitemtypedef)
- [SpectrumConfigTypeDef](./type_defs.md#spectrumconfigtypedef)
- [UplinkSpectrumConfigTypeDef](./type_defs.md#uplinkspectrumconfigtypedef)
- [ListGroundStationsResponseTypeDef](./type_defs.md#listgroundstationsresponsetypedef)
- [RangedSocketAddressTypeDef](./type_defs.md#rangedsocketaddresstypedef)
- [ListConfigsRequestPaginateTypeDef](./type_defs.md#listconfigsrequestpaginatetypedef)
- [ListDataflowEndpointGroupsRequestPaginateTypeDef](./type_defs.md#listdataflowendpointgroupsrequestpaginatetypedef)
- [ListEphemeridesRequestPaginateTypeDef](./type_defs.md#listephemeridesrequestpaginatetypedef)
- [ListGroundStationsRequestPaginateTypeDef](./type_defs.md#listgroundstationsrequestpaginatetypedef)
- [ListMissionProfilesRequestPaginateTypeDef](./type_defs.md#listmissionprofilesrequestpaginatetypedef)
- [ListSatellitesRequestPaginateTypeDef](./type_defs.md#listsatellitesrequestpaginatetypedef)
- [ListMissionProfilesResponseTypeDef](./type_defs.md#listmissionprofilesresponsetypedef)
- [SecurityDetailsUnionTypeDef](./type_defs.md#securitydetailsuniontypedef)
- [RegisterAgentRequestTypeDef](./type_defs.md#registeragentrequesttypedef)
- [ListContactsRequestPaginateTypeDef](./type_defs.md#listcontactsrequestpaginatetypedef)
- [ListContactsRequestTypeDef](./type_defs.md#listcontactsrequesttypedef)
- [TrackingOverridesTypeDef](./type_defs.md#trackingoverridestypedef)
- [AzElSegmentTypeDef](./type_defs.md#azelsegmenttypedef)
- [TLEDataTypeDef](./type_defs.md#tledatatypedef)
- [EphemerisTypeDescriptionTypeDef](./type_defs.md#ephemeristypedescriptiontypedef)
- [ListEphemeridesResponseTypeDef](./type_defs.md#listephemeridesresponsetypedef)
- [ListContactsResponseTypeDef](./type_defs.md#listcontactsresponsetypedef)
- [ListSatellitesResponseTypeDef](./type_defs.md#listsatellitesresponsetypedef)
- [AntennaDownlinkConfigTypeDef](./type_defs.md#antennadownlinkconfigtypedef)
- [AntennaDownlinkDemodDecodeConfigTypeDef](./type_defs.md#antennadownlinkdemoddecodeconfigtypedef)
- [AntennaUplinkConfigTypeDef](./type_defs.md#antennauplinkconfigtypedef)
- [RangedConnectionDetailsTypeDef](./type_defs.md#rangedconnectiondetailstypedef)
- [ReserveContactRequestTypeDef](./type_defs.md#reservecontactrequesttypedef)
- [AzElSegmentsTypeDef](./type_defs.md#azelsegmentstypedef)
- [TLEEphemerisTypeDef](./type_defs.md#tleephemeristypedef)
- [DescribeEphemerisResponseTypeDef](./type_defs.md#describeephemerisresponsetypedef)
- [ConfigTypeDataTypeDef](./type_defs.md#configtypedatatypedef)
- [AwsGroundStationAgentEndpointTypeDef](./type_defs.md#awsgroundstationagentendpointtypedef)
- [DownlinkConnectionDetailsTypeDef](./type_defs.md#downlinkconnectiondetailstypedef)
- [UplinkConnectionDetailsTypeDef](./type_defs.md#uplinkconnectiondetailstypedef)
- [AzElSegmentsDataTypeDef](./type_defs.md#azelsegmentsdatatypedef)
- [CreateConfigRequestTypeDef](./type_defs.md#createconfigrequesttypedef)
- [GetConfigResponseTypeDef](./type_defs.md#getconfigresponsetypedef)
- [UpdateConfigRequestTypeDef](./type_defs.md#updateconfigrequesttypedef)
- [DownlinkDataflowDetailsTypeDef](./type_defs.md#downlinkdataflowdetailstypedef)
- [UplinkDataflowDetailsTypeDef](./type_defs.md#uplinkdataflowdetailstypedef)
- [AzElEphemerisTypeDef](./type_defs.md#azelephemeristypedef)
- [DownlinkAwsGroundStationAgentEndpointDetailsTypeDef](./type_defs.md#downlinkawsgroundstationagentendpointdetailstypedef)
- [DownlinkAwsGroundStationAgentEndpointTypeDef](./type_defs.md#downlinkawsgroundstationagentendpointtypedef)
- [UplinkAwsGroundStationAgentEndpointDetailsTypeDef](./type_defs.md#uplinkawsgroundstationagentendpointdetailstypedef)
- [UplinkAwsGroundStationAgentEndpointTypeDef](./type_defs.md#uplinkawsgroundstationagentendpointtypedef)
- [EphemerisDataTypeDef](./type_defs.md#ephemerisdatatypedef)
- [EndpointDetailsOutputTypeDef](./type_defs.md#endpointdetailsoutputtypedef)
- [EndpointDetailsTypeDef](./type_defs.md#endpointdetailstypedef)
- [CreateEndpointDetailsTypeDef](./type_defs.md#createendpointdetailstypedef)
- [CreateEphemerisRequestTypeDef](./type_defs.md#createephemerisrequesttypedef)
- [ConfigDetailsTypeDef](./type_defs.md#configdetailstypedef)
- [GetDataflowEndpointGroupResponseTypeDef](./type_defs.md#getdataflowendpointgroupresponsetypedef)
- [EndpointDetailsUnionTypeDef](./type_defs.md#endpointdetailsuniontypedef)
- [CreateDataflowEndpointGroupV2RequestTypeDef](./type_defs.md#createdataflowendpointgroupv2requesttypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [CreateDataflowEndpointGroupRequestTypeDef](./type_defs.md#createdataflowendpointgrouprequesttypedef)
- [DataflowDetailTypeDef](./type_defs.md#dataflowdetailtypedef)
- [DescribeContactResponseTypeDef](./type_defs.md#describecontactresponsetypedef)

