# Ivsrealtime module

> [Index](../README.md) > Ivsrealtime


!!! note ""

    Auto-generated documentation for [Ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Ivsrealtime` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ivs-realtime]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ivs-realtime]'


# standalone installation
python -m pip install types-aiobotocore-ivs-realtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ivs-realtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IvsrealtimeClient

Type annotations and code completion for  `#!python session.create_client("ivs-realtime")` as [IvsrealtimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client)

```python
# IvsrealtimeClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ivs_realtime.client import IvsrealtimeClient


session = get_session()
async with session.create_client("ivs-realtime") as client:
    client: IvsrealtimeClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("ivs-realtime").get_paginator("...")`.

```python
# ListIngestConfigurationsPaginator usage example

from types_aiobotocore_ivs_realtime.paginator import ListIngestConfigurationsPaginator

def get_list_ingest_configurations_paginator() -> ListIngestConfigurationsPaginator:
    return client.get_paginator("list_ingest_configurations"))
```

- [ListIngestConfigurationsPaginator](./paginators.md#listingestconfigurationspaginator)
- [ListPublicKeysPaginator](./paginators.md#listpublickeyspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CompositionStateType usage example

from types_aiobotocore_ivs_realtime.literals import CompositionStateType

def get_value() -> CompositionStateType:
    return "ACTIVE"
```

- [CompositionStateType](./literals.md#compositionstatetype)
- [DestinationStateType](./literals.md#destinationstatetype)
- [EventErrorCodeType](./literals.md#eventerrorcodetype)
- [EventNameType](./literals.md#eventnametype)
- [IngestConfigurationStateType](./literals.md#ingestconfigurationstatetype)
- [IngestProtocolType](./literals.md#ingestprotocoltype)
- [ListIngestConfigurationsPaginatorName](./literals.md#listingestconfigurationspaginatorname)
- [ListPublicKeysPaginatorName](./literals.md#listpublickeyspaginatorname)
- [ParticipantProtocolType](./literals.md#participantprotocoltype)
- [ParticipantRecordingFilterByRecordingStateType](./literals.md#participantrecordingfilterbyrecordingstatetype)
- [ParticipantRecordingMediaTypeType](./literals.md#participantrecordingmediatypetype)
- [ParticipantRecordingStateType](./literals.md#participantrecordingstatetype)
- [ParticipantStateType](./literals.md#participantstatetype)
- [ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype)
- [PipBehaviorType](./literals.md#pipbehaviortype)
- [PipPositionType](./literals.md#pippositiontype)
- [RecordingConfigurationFormatType](./literals.md#recordingconfigurationformattype)
- [VideoAspectRatioType](./literals.md#videoaspectratiotype)
- [VideoFillModeType](./literals.md#videofillmodetype)
- [IvsrealtimeServiceName](./literals.md#ivsrealtimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AutoParticipantRecordingConfigurationOutputTypeDef](./type_defs.md#autoparticipantrecordingconfigurationoutputtypedef)
- [AutoParticipantRecordingConfigurationTypeDef](./type_defs.md#autoparticipantrecordingconfigurationtypedef)
- [ChannelDestinationConfigurationTypeDef](./type_defs.md#channeldestinationconfigurationtypedef)
- [DestinationSummaryTypeDef](./type_defs.md#destinationsummarytypedef)
- [VideoTypeDef](./type_defs.md#videotypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateIngestConfigurationRequestRequestTypeDef](./type_defs.md#createingestconfigurationrequestrequesttypedef)
- [IngestConfigurationTypeDef](./type_defs.md#ingestconfigurationtypedef)
- [CreateParticipantTokenRequestRequestTypeDef](./type_defs.md#createparticipanttokenrequestrequesttypedef)
- [ParticipantTokenTypeDef](./type_defs.md#participanttokentypedef)
- [ParticipantTokenConfigurationTypeDef](./type_defs.md#participanttokenconfigurationtypedef)
- [S3StorageConfigurationTypeDef](./type_defs.md#s3storageconfigurationtypedef)
- [DeleteEncoderConfigurationRequestRequestTypeDef](./type_defs.md#deleteencoderconfigurationrequestrequesttypedef)
- [DeleteIngestConfigurationRequestRequestTypeDef](./type_defs.md#deleteingestconfigurationrequestrequesttypedef)
- [DeletePublicKeyRequestRequestTypeDef](./type_defs.md#deletepublickeyrequestrequesttypedef)
- [DeleteStageRequestRequestTypeDef](./type_defs.md#deletestagerequestrequesttypedef)
- [DeleteStorageConfigurationRequestRequestTypeDef](./type_defs.md#deletestorageconfigurationrequestrequesttypedef)
- [S3DetailTypeDef](./type_defs.md#s3detailtypedef)
- [DisconnectParticipantRequestRequestTypeDef](./type_defs.md#disconnectparticipantrequestrequesttypedef)
- [EncoderConfigurationSummaryTypeDef](./type_defs.md#encoderconfigurationsummarytypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [GetCompositionRequestRequestTypeDef](./type_defs.md#getcompositionrequestrequesttypedef)
- [GetEncoderConfigurationRequestRequestTypeDef](./type_defs.md#getencoderconfigurationrequestrequesttypedef)
- [GetIngestConfigurationRequestRequestTypeDef](./type_defs.md#getingestconfigurationrequestrequesttypedef)
- [GetParticipantRequestRequestTypeDef](./type_defs.md#getparticipantrequestrequesttypedef)
- [ParticipantTypeDef](./type_defs.md#participanttypedef)
- [GetPublicKeyRequestRequestTypeDef](./type_defs.md#getpublickeyrequestrequesttypedef)
- [PublicKeyTypeDef](./type_defs.md#publickeytypedef)
- [GetStageRequestRequestTypeDef](./type_defs.md#getstagerequestrequesttypedef)
- [GetStageSessionRequestRequestTypeDef](./type_defs.md#getstagesessionrequestrequesttypedef)
- [StageSessionTypeDef](./type_defs.md#stagesessiontypedef)
- [GetStorageConfigurationRequestRequestTypeDef](./type_defs.md#getstorageconfigurationrequestrequesttypedef)
- [GridConfigurationTypeDef](./type_defs.md#gridconfigurationtypedef)
- [ImportPublicKeyRequestRequestTypeDef](./type_defs.md#importpublickeyrequestrequesttypedef)
- [IngestConfigurationSummaryTypeDef](./type_defs.md#ingestconfigurationsummarytypedef)
- [PipConfigurationTypeDef](./type_defs.md#pipconfigurationtypedef)
- [ListCompositionsRequestRequestTypeDef](./type_defs.md#listcompositionsrequestrequesttypedef)
- [ListEncoderConfigurationsRequestRequestTypeDef](./type_defs.md#listencoderconfigurationsrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListIngestConfigurationsRequestRequestTypeDef](./type_defs.md#listingestconfigurationsrequestrequesttypedef)
- [ListParticipantEventsRequestRequestTypeDef](./type_defs.md#listparticipanteventsrequestrequesttypedef)
- [ListParticipantsRequestRequestTypeDef](./type_defs.md#listparticipantsrequestrequesttypedef)
- [ParticipantSummaryTypeDef](./type_defs.md#participantsummarytypedef)
- [ListPublicKeysRequestRequestTypeDef](./type_defs.md#listpublickeysrequestrequesttypedef)
- [PublicKeySummaryTypeDef](./type_defs.md#publickeysummarytypedef)
- [ListStageSessionsRequestRequestTypeDef](./type_defs.md#liststagesessionsrequestrequesttypedef)
- [StageSessionSummaryTypeDef](./type_defs.md#stagesessionsummarytypedef)
- [ListStagesRequestRequestTypeDef](./type_defs.md#liststagesrequestrequesttypedef)
- [StageSummaryTypeDef](./type_defs.md#stagesummarytypedef)
- [ListStorageConfigurationsRequestRequestTypeDef](./type_defs.md#liststorageconfigurationsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RecordingConfigurationTypeDef](./type_defs.md#recordingconfigurationtypedef)
- [StageEndpointsTypeDef](./type_defs.md#stageendpointstypedef)
- [StopCompositionRequestRequestTypeDef](./type_defs.md#stopcompositionrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateIngestConfigurationRequestRequestTypeDef](./type_defs.md#updateingestconfigurationrequestrequesttypedef)
- [UpdateStageRequestRequestTypeDef](./type_defs.md#updatestagerequestrequesttypedef)
- [CompositionSummaryTypeDef](./type_defs.md#compositionsummarytypedef)
- [CreateEncoderConfigurationRequestRequestTypeDef](./type_defs.md#createencoderconfigurationrequestrequesttypedef)
- [EncoderConfigurationTypeDef](./type_defs.md#encoderconfigurationtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateIngestConfigurationResponseTypeDef](./type_defs.md#createingestconfigurationresponsetypedef)
- [GetIngestConfigurationResponseTypeDef](./type_defs.md#getingestconfigurationresponsetypedef)
- [UpdateIngestConfigurationResponseTypeDef](./type_defs.md#updateingestconfigurationresponsetypedef)
- [CreateParticipantTokenResponseTypeDef](./type_defs.md#createparticipanttokenresponsetypedef)
- [CreateStageRequestRequestTypeDef](./type_defs.md#createstagerequestrequesttypedef)
- [CreateStorageConfigurationRequestRequestTypeDef](./type_defs.md#createstorageconfigurationrequestrequesttypedef)
- [StorageConfigurationSummaryTypeDef](./type_defs.md#storageconfigurationsummarytypedef)
- [StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef)
- [DestinationDetailTypeDef](./type_defs.md#destinationdetailtypedef)
- [ListEncoderConfigurationsResponseTypeDef](./type_defs.md#listencoderconfigurationsresponsetypedef)
- [ListParticipantEventsResponseTypeDef](./type_defs.md#listparticipanteventsresponsetypedef)
- [GetParticipantResponseTypeDef](./type_defs.md#getparticipantresponsetypedef)
- [GetPublicKeyResponseTypeDef](./type_defs.md#getpublickeyresponsetypedef)
- [ImportPublicKeyResponseTypeDef](./type_defs.md#importpublickeyresponsetypedef)
- [GetStageSessionResponseTypeDef](./type_defs.md#getstagesessionresponsetypedef)
- [ListIngestConfigurationsResponseTypeDef](./type_defs.md#listingestconfigurationsresponsetypedef)
- [LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef)
- [ListIngestConfigurationsRequestListIngestConfigurationsPaginateTypeDef](./type_defs.md#listingestconfigurationsrequestlistingestconfigurationspaginatetypedef)
- [ListPublicKeysRequestListPublicKeysPaginateTypeDef](./type_defs.md#listpublickeysrequestlistpublickeyspaginatetypedef)
- [ListParticipantsResponseTypeDef](./type_defs.md#listparticipantsresponsetypedef)
- [ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef)
- [ListStageSessionsResponseTypeDef](./type_defs.md#liststagesessionsresponsetypedef)
- [ListStagesResponseTypeDef](./type_defs.md#liststagesresponsetypedef)
- [S3DestinationConfigurationOutputTypeDef](./type_defs.md#s3destinationconfigurationoutputtypedef)
- [S3DestinationConfigurationTypeDef](./type_defs.md#s3destinationconfigurationtypedef)
- [StageTypeDef](./type_defs.md#stagetypedef)
- [ListCompositionsResponseTypeDef](./type_defs.md#listcompositionsresponsetypedef)
- [CreateEncoderConfigurationResponseTypeDef](./type_defs.md#createencoderconfigurationresponsetypedef)
- [GetEncoderConfigurationResponseTypeDef](./type_defs.md#getencoderconfigurationresponsetypedef)
- [ListStorageConfigurationsResponseTypeDef](./type_defs.md#liststorageconfigurationsresponsetypedef)
- [CreateStorageConfigurationResponseTypeDef](./type_defs.md#createstorageconfigurationresponsetypedef)
- [GetStorageConfigurationResponseTypeDef](./type_defs.md#getstorageconfigurationresponsetypedef)
- [DestinationConfigurationOutputTypeDef](./type_defs.md#destinationconfigurationoutputtypedef)
- [S3DestinationConfigurationUnionTypeDef](./type_defs.md#s3destinationconfigurationuniontypedef)
- [CreateStageResponseTypeDef](./type_defs.md#createstageresponsetypedef)
- [GetStageResponseTypeDef](./type_defs.md#getstageresponsetypedef)
- [UpdateStageResponseTypeDef](./type_defs.md#updatestageresponsetypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef)
- [CompositionTypeDef](./type_defs.md#compositiontypedef)
- [DestinationConfigurationUnionTypeDef](./type_defs.md#destinationconfigurationuniontypedef)
- [GetCompositionResponseTypeDef](./type_defs.md#getcompositionresponsetypedef)
- [StartCompositionResponseTypeDef](./type_defs.md#startcompositionresponsetypedef)
- [StartCompositionRequestRequestTypeDef](./type_defs.md#startcompositionrequestrequesttypedef)

