# IvsrealtimeClient

> [Index](../README.md) > [Ivsrealtime](./README.md) > IvsrealtimeClient

!!! note ""

    Auto-generated documentation for [Ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).

## IvsrealtimeClient

Type annotations and code completion for `#!python session.create_client("ivs-realtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client)

```python
# IvsrealtimeClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_ivs_realtime.client import IvsrealtimeClient

session = get_session()
async with session.create_client("ivs-realtime") as client:
    client: IvsrealtimeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("ivs-realtime").exceptions` structure.

```python
# IvsrealtimeClient.exceptions usage example

async with session.create_client("ivs-realtime") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.PendingVerification,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# IvsrealtimeClient usage type checking example

from types_aiobotocore_ivs_realtime.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("ivs-realtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("ivs-realtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### create\_encoder\_configuration

Creates an EncoderConfiguration object.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").create_encoder_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/create_encoder_configuration.html)

```python
# create_encoder_configuration method definition

await def create_encoder_configuration(
    self,
    *,
    name: str = ...,
    video: VideoTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateEncoderConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VideoTypeDef](./type_defs.md#videotypedef) 
2. See [:material-code-braces: CreateEncoderConfigurationResponseTypeDef](./type_defs.md#createencoderconfigurationresponsetypedef) 


```python
# create_encoder_configuration method usage example with argument unpacking

kwargs: CreateEncoderConfigurationRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_encoder_configuration(**kwargs)
```

1. See [:material-code-braces: CreateEncoderConfigurationRequestRequestTypeDef](./type_defs.md#createencoderconfigurationrequestrequesttypedef) 

### create\_ingest\_configuration

Creates a new IngestConfiguration resource, used to specify the ingest protocol
for a stage.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").create_ingest_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/create_ingest_configuration.html)

```python
# create_ingest_configuration method definition

await def create_ingest_configuration(
    self,
    *,
    ingestProtocol: IngestProtocolType,  # (1)
    name: str = ...,
    stageArn: str = ...,
    userId: str = ...,
    attributes: Mapping[str, str] = ...,
    insecureIngest: bool = ...,
    tags: Mapping[str, str] = ...,
) -> CreateIngestConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IngestProtocolType](./literals.md#ingestprotocoltype) 
2. See [:material-code-braces: CreateIngestConfigurationResponseTypeDef](./type_defs.md#createingestconfigurationresponsetypedef) 


```python
# create_ingest_configuration method usage example with argument unpacking

kwargs: CreateIngestConfigurationRequestRequestTypeDef = {  # (1)
    "ingestProtocol": ...,
}

parent.create_ingest_configuration(**kwargs)
```

1. See [:material-code-braces: CreateIngestConfigurationRequestRequestTypeDef](./type_defs.md#createingestconfigurationrequestrequesttypedef) 

### create\_participant\_token

Creates an additional token for a specified stage.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").create_participant_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/create_participant_token.html)

```python
# create_participant_token method definition

await def create_participant_token(
    self,
    *,
    stageArn: str,
    duration: int = ...,
    userId: str = ...,
    attributes: Mapping[str, str] = ...,
    capabilities: Sequence[ParticipantTokenCapabilityType] = ...,  # (1)
) -> CreateParticipantTokenResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ParticipantTokenCapabilityType](./literals.md#participanttokencapabilitytype) 
2. See [:material-code-braces: CreateParticipantTokenResponseTypeDef](./type_defs.md#createparticipanttokenresponsetypedef) 


```python
# create_participant_token method usage example with argument unpacking

kwargs: CreateParticipantTokenRequestRequestTypeDef = {  # (1)
    "stageArn": ...,
}

parent.create_participant_token(**kwargs)
```

1. See [:material-code-braces: CreateParticipantTokenRequestRequestTypeDef](./type_defs.md#createparticipanttokenrequestrequesttypedef) 

### create\_stage

Creates a new stage (and optionally participant tokens).

Type annotations and code completion for `#!python session.create_client("ivs-realtime").create_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/create_stage.html)

```python
# create_stage method definition

await def create_stage(
    self,
    *,
    name: str = ...,
    participantTokenConfigurations: Sequence[ParticipantTokenConfigurationTypeDef] = ...,  # (1)
    tags: Mapping[str, str] = ...,
    autoParticipantRecordingConfiguration: AutoParticipantRecordingConfigurationTypeDef = ...,  # (2)
) -> CreateStageResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ParticipantTokenConfigurationTypeDef](./type_defs.md#participanttokenconfigurationtypedef) 
2. See [:material-code-braces: AutoParticipantRecordingConfigurationTypeDef](./type_defs.md#autoparticipantrecordingconfigurationtypedef) 
3. See [:material-code-braces: CreateStageResponseTypeDef](./type_defs.md#createstageresponsetypedef) 


```python
# create_stage method usage example with argument unpacking

kwargs: CreateStageRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_stage(**kwargs)
```

1. See [:material-code-braces: CreateStageRequestRequestTypeDef](./type_defs.md#createstagerequestrequesttypedef) 

### create\_storage\_configuration

Creates a new storage configuration, used to enable recording to Amazon S3.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").create_storage_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/create_storage_configuration.html)

```python
# create_storage_configuration method definition

await def create_storage_configuration(
    self,
    *,
    s3: S3StorageConfigurationTypeDef,  # (1)
    name: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateStorageConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: S3StorageConfigurationTypeDef](./type_defs.md#s3storageconfigurationtypedef) 
2. See [:material-code-braces: CreateStorageConfigurationResponseTypeDef](./type_defs.md#createstorageconfigurationresponsetypedef) 


```python
# create_storage_configuration method usage example with argument unpacking

kwargs: CreateStorageConfigurationRequestRequestTypeDef = {  # (1)
    "s3": ...,
}

parent.create_storage_configuration(**kwargs)
```

1. See [:material-code-braces: CreateStorageConfigurationRequestRequestTypeDef](./type_defs.md#createstorageconfigurationrequestrequesttypedef) 

### delete\_encoder\_configuration

Deletes an EncoderConfiguration resource.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").delete_encoder_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/delete_encoder_configuration.html)

```python
# delete_encoder_configuration method definition

await def delete_encoder_configuration(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_encoder_configuration method usage example with argument unpacking

kwargs: DeleteEncoderConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_encoder_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteEncoderConfigurationRequestRequestTypeDef](./type_defs.md#deleteencoderconfigurationrequestrequesttypedef) 

### delete\_ingest\_configuration

Deletes a specified IngestConfiguration, so it can no longer be used to
broadcast.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").delete_ingest_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/delete_ingest_configuration.html)

```python
# delete_ingest_configuration method definition

await def delete_ingest_configuration(
    self,
    *,
    arn: str,
    force: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ingest_configuration method usage example with argument unpacking

kwargs: DeleteIngestConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_ingest_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteIngestConfigurationRequestRequestTypeDef](./type_defs.md#deleteingestconfigurationrequestrequesttypedef) 

### delete\_public\_key

Deletes the specified public key used to sign stage participant tokens.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").delete_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/delete_public_key.html)

```python
# delete_public_key method definition

await def delete_public_key(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_public_key method usage example with argument unpacking

kwargs: DeletePublicKeyRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_public_key(**kwargs)
```

1. See [:material-code-braces: DeletePublicKeyRequestRequestTypeDef](./type_defs.md#deletepublickeyrequestrequesttypedef) 

### delete\_stage

Shuts down and deletes the specified stage (disconnecting all participants).

Type annotations and code completion for `#!python session.create_client("ivs-realtime").delete_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/delete_stage.html)

```python
# delete_stage method definition

await def delete_stage(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_stage method usage example with argument unpacking

kwargs: DeleteStageRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_stage(**kwargs)
```

1. See [:material-code-braces: DeleteStageRequestRequestTypeDef](./type_defs.md#deletestagerequestrequesttypedef) 

### delete\_storage\_configuration

Deletes the storage configuration for the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").delete_storage_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/delete_storage_configuration.html)

```python
# delete_storage_configuration method definition

await def delete_storage_configuration(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_storage_configuration method usage example with argument unpacking

kwargs: DeleteStorageConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_storage_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteStorageConfigurationRequestRequestTypeDef](./type_defs.md#deletestorageconfigurationrequestrequesttypedef) 

### disconnect\_participant

Disconnects a specified participant from a specified stage.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").disconnect_participant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/disconnect_participant.html)

```python
# disconnect_participant method definition

await def disconnect_participant(
    self,
    *,
    stageArn: str,
    participantId: str,
    reason: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disconnect_participant method usage example with argument unpacking

kwargs: DisconnectParticipantRequestRequestTypeDef = {  # (1)
    "stageArn": ...,
    "participantId": ...,
}

parent.disconnect_participant(**kwargs)
```

1. See [:material-code-braces: DisconnectParticipantRequestRequestTypeDef](./type_defs.md#disconnectparticipantrequestrequesttypedef) 

### get\_composition

Get information about the specified Composition resource.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_composition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/get_composition.html)

```python
# get_composition method definition

await def get_composition(
    self,
    *,
    arn: str,
) -> GetCompositionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCompositionResponseTypeDef](./type_defs.md#getcompositionresponsetypedef) 


```python
# get_composition method usage example with argument unpacking

kwargs: GetCompositionRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_composition(**kwargs)
```

1. See [:material-code-braces: GetCompositionRequestRequestTypeDef](./type_defs.md#getcompositionrequestrequesttypedef) 

### get\_encoder\_configuration

Gets information about the specified EncoderConfiguration resource.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_encoder_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/get_encoder_configuration.html)

```python
# get_encoder_configuration method definition

await def get_encoder_configuration(
    self,
    *,
    arn: str,
) -> GetEncoderConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEncoderConfigurationResponseTypeDef](./type_defs.md#getencoderconfigurationresponsetypedef) 


```python
# get_encoder_configuration method usage example with argument unpacking

kwargs: GetEncoderConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_encoder_configuration(**kwargs)
```

1. See [:material-code-braces: GetEncoderConfigurationRequestRequestTypeDef](./type_defs.md#getencoderconfigurationrequestrequesttypedef) 

### get\_ingest\_configuration

Gets information about the specified IngestConfiguration.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_ingest_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/get_ingest_configuration.html)

```python
# get_ingest_configuration method definition

await def get_ingest_configuration(
    self,
    *,
    arn: str,
) -> GetIngestConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIngestConfigurationResponseTypeDef](./type_defs.md#getingestconfigurationresponsetypedef) 


```python
# get_ingest_configuration method usage example with argument unpacking

kwargs: GetIngestConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_ingest_configuration(**kwargs)
```

1. See [:material-code-braces: GetIngestConfigurationRequestRequestTypeDef](./type_defs.md#getingestconfigurationrequestrequesttypedef) 

### get\_participant

Gets information about the specified participant token.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_participant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/get_participant.html)

```python
# get_participant method definition

await def get_participant(
    self,
    *,
    stageArn: str,
    sessionId: str,
    participantId: str,
) -> GetParticipantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetParticipantResponseTypeDef](./type_defs.md#getparticipantresponsetypedef) 


```python
# get_participant method usage example with argument unpacking

kwargs: GetParticipantRequestRequestTypeDef = {  # (1)
    "stageArn": ...,
    "sessionId": ...,
    "participantId": ...,
}

parent.get_participant(**kwargs)
```

1. See [:material-code-braces: GetParticipantRequestRequestTypeDef](./type_defs.md#getparticipantrequestrequesttypedef) 

### get\_public\_key

Gets information for the specified public key.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/get_public_key.html)

```python
# get_public_key method definition

await def get_public_key(
    self,
    *,
    arn: str,
) -> GetPublicKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPublicKeyResponseTypeDef](./type_defs.md#getpublickeyresponsetypedef) 


```python
# get_public_key method usage example with argument unpacking

kwargs: GetPublicKeyRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_public_key(**kwargs)
```

1. See [:material-code-braces: GetPublicKeyRequestRequestTypeDef](./type_defs.md#getpublickeyrequestrequesttypedef) 

### get\_stage

Gets information for the specified stage.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/get_stage.html)

```python
# get_stage method definition

await def get_stage(
    self,
    *,
    arn: str,
) -> GetStageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStageResponseTypeDef](./type_defs.md#getstageresponsetypedef) 


```python
# get_stage method usage example with argument unpacking

kwargs: GetStageRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_stage(**kwargs)
```

1. See [:material-code-braces: GetStageRequestRequestTypeDef](./type_defs.md#getstagerequestrequesttypedef) 

### get\_stage\_session

Gets information for the specified stage session.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_stage_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/get_stage_session.html)

```python
# get_stage_session method definition

await def get_stage_session(
    self,
    *,
    stageArn: str,
    sessionId: str,
) -> GetStageSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStageSessionResponseTypeDef](./type_defs.md#getstagesessionresponsetypedef) 


```python
# get_stage_session method usage example with argument unpacking

kwargs: GetStageSessionRequestRequestTypeDef = {  # (1)
    "stageArn": ...,
    "sessionId": ...,
}

parent.get_stage_session(**kwargs)
```

1. See [:material-code-braces: GetStageSessionRequestRequestTypeDef](./type_defs.md#getstagesessionrequestrequesttypedef) 

### get\_storage\_configuration

Gets the storage configuration for the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_storage_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/get_storage_configuration.html)

```python
# get_storage_configuration method definition

await def get_storage_configuration(
    self,
    *,
    arn: str,
) -> GetStorageConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStorageConfigurationResponseTypeDef](./type_defs.md#getstorageconfigurationresponsetypedef) 


```python
# get_storage_configuration method usage example with argument unpacking

kwargs: GetStorageConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_storage_configuration(**kwargs)
```

1. See [:material-code-braces: GetStorageConfigurationRequestRequestTypeDef](./type_defs.md#getstorageconfigurationrequestrequesttypedef) 

### import\_public\_key

Import a public key to be used for signing stage participant tokens.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").import_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/import_public_key.html)

```python
# import_public_key method definition

await def import_public_key(
    self,
    *,
    publicKeyMaterial: str,
    name: str = ...,
    tags: Mapping[str, str] = ...,
) -> ImportPublicKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ImportPublicKeyResponseTypeDef](./type_defs.md#importpublickeyresponsetypedef) 


```python
# import_public_key method usage example with argument unpacking

kwargs: ImportPublicKeyRequestRequestTypeDef = {  # (1)
    "publicKeyMaterial": ...,
}

parent.import_public_key(**kwargs)
```

1. See [:material-code-braces: ImportPublicKeyRequestRequestTypeDef](./type_defs.md#importpublickeyrequestrequesttypedef) 

### list\_compositions

Gets summary information about all Compositions in your account, in the AWS
region where the API request is processed.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_compositions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/list_compositions.html)

```python
# list_compositions method definition

await def list_compositions(
    self,
    *,
    filterByStageArn: str = ...,
    filterByEncoderConfigurationArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCompositionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCompositionsResponseTypeDef](./type_defs.md#listcompositionsresponsetypedef) 


```python
# list_compositions method usage example with argument unpacking

kwargs: ListCompositionsRequestRequestTypeDef = {  # (1)
    "filterByStageArn": ...,
}

parent.list_compositions(**kwargs)
```

1. See [:material-code-braces: ListCompositionsRequestRequestTypeDef](./type_defs.md#listcompositionsrequestrequesttypedef) 

### list\_encoder\_configurations

Gets summary information about all EncoderConfigurations in your account, in
the AWS region where the API request is processed.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_encoder_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/list_encoder_configurations.html)

```python
# list_encoder_configurations method definition

await def list_encoder_configurations(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListEncoderConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEncoderConfigurationsResponseTypeDef](./type_defs.md#listencoderconfigurationsresponsetypedef) 


```python
# list_encoder_configurations method usage example with argument unpacking

kwargs: ListEncoderConfigurationsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_encoder_configurations(**kwargs)
```

1. See [:material-code-braces: ListEncoderConfigurationsRequestRequestTypeDef](./type_defs.md#listencoderconfigurationsrequestrequesttypedef) 

### list\_ingest\_configurations

Lists all IngestConfigurations in your account, in the AWS region where the API
request is processed.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_ingest_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/list_ingest_configurations.html)

```python
# list_ingest_configurations method definition

await def list_ingest_configurations(
    self,
    *,
    filterByStageArn: str = ...,
    filterByState: IngestConfigurationStateType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListIngestConfigurationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IngestConfigurationStateType](./literals.md#ingestconfigurationstatetype) 
2. See [:material-code-braces: ListIngestConfigurationsResponseTypeDef](./type_defs.md#listingestconfigurationsresponsetypedef) 


```python
# list_ingest_configurations method usage example with argument unpacking

kwargs: ListIngestConfigurationsRequestRequestTypeDef = {  # (1)
    "filterByStageArn": ...,
}

parent.list_ingest_configurations(**kwargs)
```

1. See [:material-code-braces: ListIngestConfigurationsRequestRequestTypeDef](./type_defs.md#listingestconfigurationsrequestrequesttypedef) 

### list\_participant\_events

Lists events for a specified participant that occurred during a specified stage
session.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_participant_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/list_participant_events.html)

```python
# list_participant_events method definition

await def list_participant_events(
    self,
    *,
    stageArn: str,
    sessionId: str,
    participantId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListParticipantEventsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListParticipantEventsResponseTypeDef](./type_defs.md#listparticipanteventsresponsetypedef) 


```python
# list_participant_events method usage example with argument unpacking

kwargs: ListParticipantEventsRequestRequestTypeDef = {  # (1)
    "stageArn": ...,
    "sessionId": ...,
    "participantId": ...,
}

parent.list_participant_events(**kwargs)
```

1. See [:material-code-braces: ListParticipantEventsRequestRequestTypeDef](./type_defs.md#listparticipanteventsrequestrequesttypedef) 

### list\_participants

Lists all participants in a specified stage session.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_participants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/list_participants.html)

```python
# list_participants method definition

await def list_participants(
    self,
    *,
    stageArn: str,
    sessionId: str,
    filterByUserId: str = ...,
    filterByPublished: bool = ...,
    filterByState: ParticipantStateType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
    filterByRecordingState: ParticipantRecordingFilterByRecordingStateType = ...,  # (2)
) -> ListParticipantsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
2. See [:material-code-brackets: ParticipantRecordingFilterByRecordingStateType](./literals.md#participantrecordingfilterbyrecordingstatetype) 
3. See [:material-code-braces: ListParticipantsResponseTypeDef](./type_defs.md#listparticipantsresponsetypedef) 


```python
# list_participants method usage example with argument unpacking

kwargs: ListParticipantsRequestRequestTypeDef = {  # (1)
    "stageArn": ...,
    "sessionId": ...,
}

parent.list_participants(**kwargs)
```

1. See [:material-code-braces: ListParticipantsRequestRequestTypeDef](./type_defs.md#listparticipantsrequestrequesttypedef) 

### list\_public\_keys

Gets summary information about all public keys in your account, in the AWS
region where the API request is processed.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_public_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/list_public_keys.html)

```python
# list_public_keys method definition

await def list_public_keys(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPublicKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPublicKeysResponseTypeDef](./type_defs.md#listpublickeysresponsetypedef) 


```python
# list_public_keys method usage example with argument unpacking

kwargs: ListPublicKeysRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_public_keys(**kwargs)
```

1. See [:material-code-braces: ListPublicKeysRequestRequestTypeDef](./type_defs.md#listpublickeysrequestrequesttypedef) 

### list\_stage\_sessions

Gets all sessions for a specified stage.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_stage_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/list_stage_sessions.html)

```python
# list_stage_sessions method definition

await def list_stage_sessions(
    self,
    *,
    stageArn: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListStageSessionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStageSessionsResponseTypeDef](./type_defs.md#liststagesessionsresponsetypedef) 


```python
# list_stage_sessions method usage example with argument unpacking

kwargs: ListStageSessionsRequestRequestTypeDef = {  # (1)
    "stageArn": ...,
}

parent.list_stage_sessions(**kwargs)
```

1. See [:material-code-braces: ListStageSessionsRequestRequestTypeDef](./type_defs.md#liststagesessionsrequestrequesttypedef) 

### list\_stages

Gets summary information about all stages in your account, in the AWS region
where the API request is processed.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_stages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/list_stages.html)

```python
# list_stages method definition

await def list_stages(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListStagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStagesResponseTypeDef](./type_defs.md#liststagesresponsetypedef) 


```python
# list_stages method usage example with argument unpacking

kwargs: ListStagesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_stages(**kwargs)
```

1. See [:material-code-braces: ListStagesRequestRequestTypeDef](./type_defs.md#liststagesrequestrequesttypedef) 

### list\_storage\_configurations

Gets summary information about all storage configurations in your account, in
the AWS region where the API request is processed.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_storage_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/list_storage_configurations.html)

```python
# list_storage_configurations method definition

await def list_storage_configurations(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListStorageConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStorageConfigurationsResponseTypeDef](./type_defs.md#liststorageconfigurationsresponsetypedef) 


```python
# list_storage_configurations method usage example with argument unpacking

kwargs: ListStorageConfigurationsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_storage_configurations(**kwargs)
```

1. See [:material-code-braces: ListStorageConfigurationsRequestRequestTypeDef](./type_defs.md#liststorageconfigurationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Gets information about AWS tags for the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### start\_composition

Starts a Composition from a stage based on the configuration provided in the
request.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").start_composition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/start_composition.html)

```python
# start_composition method definition

await def start_composition(
    self,
    *,
    stageArn: str,
    destinations: Sequence[DestinationConfigurationUnionTypeDef],  # (1)
    idempotencyToken: str = ...,
    layout: LayoutConfigurationTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> StartCompositionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DestinationConfigurationTypeDef](./type_defs.md#destinationconfigurationtypedef) [:material-code-braces: DestinationConfigurationOutputTypeDef](./type_defs.md#destinationconfigurationoutputtypedef) 
2. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
3. See [:material-code-braces: StartCompositionResponseTypeDef](./type_defs.md#startcompositionresponsetypedef) 


```python
# start_composition method usage example with argument unpacking

kwargs: StartCompositionRequestRequestTypeDef = {  # (1)
    "stageArn": ...,
    "destinations": ...,
}

parent.start_composition(**kwargs)
```

1. See [:material-code-braces: StartCompositionRequestRequestTypeDef](./type_defs.md#startcompositionrequestrequesttypedef) 

### stop\_composition

Stops and deletes a Composition resource.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").stop_composition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/stop_composition.html)

```python
# stop_composition method definition

await def stop_composition(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_composition method usage example with argument unpacking

kwargs: StopCompositionRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.stop_composition(**kwargs)
```

1. See [:material-code-braces: StopCompositionRequestRequestTypeDef](./type_defs.md#stopcompositionrequestrequesttypedef) 

### tag\_resource

Adds or updates tags for the AWS resource with the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from the resource with the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_ingest\_configuration

Updates a specified IngestConfiguration.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").update_ingest_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/update_ingest_configuration.html)

```python
# update_ingest_configuration method definition

await def update_ingest_configuration(
    self,
    *,
    arn: str,
    stageArn: str = ...,
) -> UpdateIngestConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateIngestConfigurationResponseTypeDef](./type_defs.md#updateingestconfigurationresponsetypedef) 


```python
# update_ingest_configuration method usage example with argument unpacking

kwargs: UpdateIngestConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_ingest_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateIngestConfigurationRequestRequestTypeDef](./type_defs.md#updateingestconfigurationrequestrequesttypedef) 

### update\_stage

Updates a stage's configuration.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").update_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime/client/update_stage.html)

```python
# update_stage method definition

await def update_stage(
    self,
    *,
    arn: str,
    name: str = ...,
    autoParticipantRecordingConfiguration: AutoParticipantRecordingConfigurationTypeDef = ...,  # (1)
) -> UpdateStageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AutoParticipantRecordingConfigurationTypeDef](./type_defs.md#autoparticipantrecordingconfigurationtypedef) 
2. See [:material-code-braces: UpdateStageResponseTypeDef](./type_defs.md#updatestageresponsetypedef) 


```python
# update_stage method usage example with argument unpacking

kwargs: UpdateStageRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_stage(**kwargs)
```

1. See [:material-code-braces: UpdateStageRequestRequestTypeDef](./type_defs.md#updatestagerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("ivs-realtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("ivs-realtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#Ivsrealtime.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_paginator` method with overloads.

- `client.get_paginator("list_ingest_configurations")` -> [ListIngestConfigurationsPaginator](./paginators.md#listingestconfigurationspaginator)
- `client.get_paginator("list_public_keys")` -> [ListPublicKeysPaginator](./paginators.md#listpublickeyspaginator)



