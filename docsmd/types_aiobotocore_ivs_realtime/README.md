# ivsrealtime module

> [Index](../README.md) > ivsrealtime


!!! note ""

    Auto-generated documentation for [ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ivsrealtime` service.

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

## ivsrealtimeClient

Type annotations and code completion for  `#!python session.create_client("ivs-realtime")` as [ivsrealtimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client)

```python
# ivsrealtimeClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ivs_realtime.client import ivsrealtimeClient


session = get_session()
async with session.create_client("ivs-realtime") as client:
    client: ivsrealtimeClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# EventErrorCodeType usage example

from types_aiobotocore_ivs_realtime.literals import EventErrorCodeType

def get_value() -> EventErrorCodeType:
    return "INSUFFICIENT_CAPABILITIES"
```

- [EventErrorCodeType](./literals.md#eventerrorcodetype)
- [EventNameType](./literals.md#eventnametype)
- [ParticipantStateType](./literals.md#participantstatetype)
- [ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype)
- [ivsrealtimeServiceName](./literals.md#ivsrealtimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CreateParticipantTokenRequestRequestTypeDef](./type_defs.md#createparticipanttokenrequestrequesttypedef)
- [ParticipantTokenTypeDef](./type_defs.md#participanttokentypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ParticipantTokenConfigurationTypeDef](./type_defs.md#participanttokenconfigurationtypedef)
- [StageTypeDef](./type_defs.md#stagetypedef)
- [DeleteStageRequestRequestTypeDef](./type_defs.md#deletestagerequestrequesttypedef)
- [DisconnectParticipantRequestRequestTypeDef](./type_defs.md#disconnectparticipantrequestrequesttypedef)
- [EventTypeDef](./type_defs.md#eventtypedef)
- [GetParticipantRequestRequestTypeDef](./type_defs.md#getparticipantrequestrequesttypedef)
- [ParticipantTypeDef](./type_defs.md#participanttypedef)
- [GetStageRequestRequestTypeDef](./type_defs.md#getstagerequestrequesttypedef)
- [GetStageSessionRequestRequestTypeDef](./type_defs.md#getstagesessionrequestrequesttypedef)
- [StageSessionTypeDef](./type_defs.md#stagesessiontypedef)
- [ListParticipantEventsRequestRequestTypeDef](./type_defs.md#listparticipanteventsrequestrequesttypedef)
- [ListParticipantsRequestRequestTypeDef](./type_defs.md#listparticipantsrequestrequesttypedef)
- [ParticipantSummaryTypeDef](./type_defs.md#participantsummarytypedef)
- [ListStageSessionsRequestRequestTypeDef](./type_defs.md#liststagesessionsrequestrequesttypedef)
- [StageSessionSummaryTypeDef](./type_defs.md#stagesessionsummarytypedef)
- [ListStagesRequestRequestTypeDef](./type_defs.md#liststagesrequestrequesttypedef)
- [StageSummaryTypeDef](./type_defs.md#stagesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateStageRequestRequestTypeDef](./type_defs.md#updatestagerequestrequesttypedef)
- [CreateParticipantTokenResponseTypeDef](./type_defs.md#createparticipanttokenresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateStageRequestRequestTypeDef](./type_defs.md#createstagerequestrequesttypedef)
- [CreateStageResponseTypeDef](./type_defs.md#createstageresponsetypedef)
- [GetStageResponseTypeDef](./type_defs.md#getstageresponsetypedef)
- [UpdateStageResponseTypeDef](./type_defs.md#updatestageresponsetypedef)
- [ListParticipantEventsResponseTypeDef](./type_defs.md#listparticipanteventsresponsetypedef)
- [GetParticipantResponseTypeDef](./type_defs.md#getparticipantresponsetypedef)
- [GetStageSessionResponseTypeDef](./type_defs.md#getstagesessionresponsetypedef)
- [ListParticipantsResponseTypeDef](./type_defs.md#listparticipantsresponsetypedef)
- [ListStageSessionsResponseTypeDef](./type_defs.md#liststagesessionsresponsetypedef)
- [ListStagesResponseTypeDef](./type_defs.md#liststagesresponsetypedef)

