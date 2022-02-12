<a id="type-annotations-for-aiobotocore-connectparticipant-module"></a>

# Type annotations for aiobotocore ConnectParticipant module

> [Index](..) > ConnectParticipant

Auto-generated documentation for
[ConnectParticipant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
type annotations stubs module
[types-aiobotocore-connectparticipant](https://pypi.org/project/types-aiobotocore-connectparticipant/).

- [Type annotations for aiobotocore ConnectParticipant module](#type-annotations-for-aiobotocore-connectparticipant-module)
  - [How to install](#how-to-install)
    - [VSCode extension](#vscode-extension)
    - [From PyPI with pip](#from-pypi-with-pip)
  - [How to uninstall](#how-to-uninstall)
  - [ConnectParticipantClient](#connectparticipantclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="how-to-install"></a>

## How to install

<a id="vscode-extension"></a>

### VSCode extension

Add
[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `ConnectParticipant`.

<a id="from-pypi-with-pip"></a>

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

<a id="how-to-uninstall"></a>

## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-connectparticipant
```

<a id="connectparticipantclient"></a>

## ConnectParticipantClient

Type annotations for `session.create_client("connectparticipant")` as
[ConnectParticipantClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_connectparticipant.client import ConnectParticipantClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [complete_attachment_upload](./client.md#complete_attachment_upload)
- [create_participant_connection](./client.md#create_participant_connection)
- [disconnect_participant](./client.md#disconnect_participant)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_attachment](./client.md#get_attachment)
- [get_transcript](./client.md#get_transcript)
- [send_event](./client.md#send_event)
- [send_message](./client.md#send_message)
- [start_attachment_upload](./client.md#start_attachment_upload)

<a id="exceptions"></a>

### Exceptions

ConnectParticipantClient [exceptions](./client.md#exceptions)

- AccessDeniedException
- ClientError
- ConflictException
- InternalServerException
- ServiceQuotaExceededException
- ThrottlingException
- ValidationException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_connectparticipant.literals import ArtifactStatusType, ...
```

- [ArtifactStatusType](./literals.md#artifactstatustype)
- [ChatItemTypeType](./literals.md#chatitemtypetype)
- [ConnectionTypeType](./literals.md#connectiontypetype)
- [ParticipantRoleType](./literals.md#participantroletype)
- [ScanDirectionType](./literals.md#scandirectiontype)
- [SortKeyType](./literals.md#sortkeytype)
- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_connectparticipant.type_defs import AttachmentItemTypeDef, ...
```

- [AttachmentItemTypeDef](./type_defs.md#attachmentitemtypedef)
- [CompleteAttachmentUploadRequestRequestTypeDef](./type_defs.md#completeattachmentuploadrequestrequesttypedef)
- [ConnectionCredentialsTypeDef](./type_defs.md#connectioncredentialstypedef)
- [CreateParticipantConnectionRequestRequestTypeDef](./type_defs.md#createparticipantconnectionrequestrequesttypedef)
- [CreateParticipantConnectionResponseTypeDef](./type_defs.md#createparticipantconnectionresponsetypedef)
- [DisconnectParticipantRequestRequestTypeDef](./type_defs.md#disconnectparticipantrequestrequesttypedef)
- [GetAttachmentRequestRequestTypeDef](./type_defs.md#getattachmentrequestrequesttypedef)
- [GetAttachmentResponseTypeDef](./type_defs.md#getattachmentresponsetypedef)
- [GetTranscriptRequestRequestTypeDef](./type_defs.md#gettranscriptrequestrequesttypedef)
- [GetTranscriptResponseTypeDef](./type_defs.md#gettranscriptresponsetypedef)
- [ItemTypeDef](./type_defs.md#itemtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SendEventRequestRequestTypeDef](./type_defs.md#sendeventrequestrequesttypedef)
- [SendEventResponseTypeDef](./type_defs.md#sendeventresponsetypedef)
- [SendMessageRequestRequestTypeDef](./type_defs.md#sendmessagerequestrequesttypedef)
- [SendMessageResponseTypeDef](./type_defs.md#sendmessageresponsetypedef)
- [StartAttachmentUploadRequestRequestTypeDef](./type_defs.md#startattachmentuploadrequestrequesttypedef)
- [StartAttachmentUploadResponseTypeDef](./type_defs.md#startattachmentuploadresponsetypedef)
- [StartPositionTypeDef](./type_defs.md#startpositiontypedef)
- [UploadMetadataTypeDef](./type_defs.md#uploadmetadatatypedef)
- [WebsocketTypeDef](./type_defs.md#websockettypedef)
