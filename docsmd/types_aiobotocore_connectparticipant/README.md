# ConnectParticipant module

> [Index](../README.md) > ConnectParticipant


!!! note ""

    Auto-generated documentation for [ConnectParticipant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
    type annotations stubs module [types-aiobotocore-connectparticipant](https://pypi.org/project/types-aiobotocore-connectparticipant/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ConnectParticipant` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[connectparticipant]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[connectparticipant]'


# standalone installation
python -m pip install types-aiobotocore-connectparticipant
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-connectparticipant
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ConnectParticipantClient

Type annotations and code completion for  `#!python session.create_client("connectparticipant")` as [ConnectParticipantClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_connectparticipant.client import ConnectParticipantClient


session = get_session()
async with session.create_client("connectparticipant") as client:
    client: ConnectParticipantClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_connectparticipant.literals import ArtifactStatusType

def get_value() -> ArtifactStatusType:
    return "APPROVED"
```

- [ArtifactStatusType](./literals.md#artifactstatustype)
- [ChatItemTypeType](./literals.md#chatitemtypetype)
- [ConnectionTypeType](./literals.md#connectiontypetype)
- [ParticipantRoleType](./literals.md#participantroletype)
- [ScanDirectionType](./literals.md#scandirectiontype)
- [SortKeyType](./literals.md#sortkeytype)
- [ConnectParticipantServiceName](./literals.md#connectparticipantservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_connectparticipant.type_defs import AttachmentItemTypeDef

def get_value() -> AttachmentItemTypeDef:
    return {
        "ContentType": ...,
    }
```

- [AttachmentItemTypeDef](./type_defs.md#attachmentitemtypedef)
- [CompleteAttachmentUploadRequestRequestTypeDef](./type_defs.md#completeattachmentuploadrequestrequesttypedef)
- [ConnectionCredentialsTypeDef](./type_defs.md#connectioncredentialstypedef)
- [CreateParticipantConnectionRequestRequestTypeDef](./type_defs.md#createparticipantconnectionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [WebsocketTypeDef](./type_defs.md#websockettypedef)
- [DisconnectParticipantRequestRequestTypeDef](./type_defs.md#disconnectparticipantrequestrequesttypedef)
- [GetAttachmentRequestRequestTypeDef](./type_defs.md#getattachmentrequestrequesttypedef)
- [StartPositionTypeDef](./type_defs.md#startpositiontypedef)
- [SendEventRequestRequestTypeDef](./type_defs.md#sendeventrequestrequesttypedef)
- [SendMessageRequestRequestTypeDef](./type_defs.md#sendmessagerequestrequesttypedef)
- [StartAttachmentUploadRequestRequestTypeDef](./type_defs.md#startattachmentuploadrequestrequesttypedef)
- [UploadMetadataTypeDef](./type_defs.md#uploadmetadatatypedef)
- [ItemTypeDef](./type_defs.md#itemtypedef)
- [GetAttachmentResponseTypeDef](./type_defs.md#getattachmentresponsetypedef)
- [SendEventResponseTypeDef](./type_defs.md#sendeventresponsetypedef)
- [SendMessageResponseTypeDef](./type_defs.md#sendmessageresponsetypedef)
- [CreateParticipantConnectionResponseTypeDef](./type_defs.md#createparticipantconnectionresponsetypedef)
- [GetTranscriptRequestRequestTypeDef](./type_defs.md#gettranscriptrequestrequesttypedef)
- [StartAttachmentUploadResponseTypeDef](./type_defs.md#startattachmentuploadresponsetypedef)
- [GetTranscriptResponseTypeDef](./type_defs.md#gettranscriptresponsetypedef)

