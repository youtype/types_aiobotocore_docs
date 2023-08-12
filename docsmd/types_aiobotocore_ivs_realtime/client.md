# ivsrealtimeClient

> [Index](../README.md) > [ivsrealtime](./README.md) > ivsrealtimeClient

!!! note ""

    Auto-generated documentation for [ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).

## ivsrealtimeClient

Type annotations and code completion for `#!python session.create_client("ivs-realtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client)

```python
ivsrealtimeClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_ivs_realtime.client import ivsrealtimeClient

session = get_session()
async with session.create_client("ivs-realtime") as client:
    client: ivsrealtimeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("ivs-realtime").exceptions` structure.

```python
ivsrealtimeClient.exceptions usage example

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
ivsrealtimeClient usage type checking example

from types_aiobotocore_ivs_realtime.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_participant\_token

Creates an additional token for a specified stage.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").create_participant_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_participant_token)

```python
# create_participant_token method definition

await def create_participant_token(
    self,
    *,
    stageArn: str,
    attributes: Mapping[str, str] = ...,
    capabilities: Sequence[ParticipantTokenCapabilityType] = ...,  # (1)
    duration: int = ...,
    userId: str = ...,
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.create_stage)

```python
# create_stage method definition

await def create_stage(
    self,
    *,
    name: str = ...,
    participantTokenConfigurations: Sequence[ParticipantTokenConfigurationTypeDef] = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateStageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ParticipantTokenConfigurationTypeDef](./type_defs.md#participanttokenconfigurationtypedef) 
2. See [:material-code-braces: CreateStageResponseTypeDef](./type_defs.md#createstageresponsetypedef) 


```python
# create_stage method usage example with argument unpacking

kwargs: CreateStageRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_stage(**kwargs)
```

1. See [:material-code-braces: CreateStageRequestRequestTypeDef](./type_defs.md#createstagerequestrequesttypedef) 

### delete\_stage

Shuts down and deletes the specified stage (disconnecting all participants).

Type annotations and code completion for `#!python session.create_client("ivs-realtime").delete_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.delete_stage)

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

### disconnect\_participant

Disconnects a specified participant and revokes the participant permanently from
a specified stage.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").disconnect_participant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.disconnect_participant)

```python
# disconnect_participant method definition

await def disconnect_participant(
    self,
    *,
    participantId: str,
    stageArn: str,
    reason: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disconnect_participant method usage example with argument unpacking

kwargs: DisconnectParticipantRequestRequestTypeDef = {  # (1)
    "participantId": ...,
    "stageArn": ...,
}

parent.disconnect_participant(**kwargs)
```

1. See [:material-code-braces: DisconnectParticipantRequestRequestTypeDef](./type_defs.md#disconnectparticipantrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.generate_presigned_url)

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


### get\_participant

Gets information about the specified participant token.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_participant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_participant)

```python
# get_participant method definition

await def get_participant(
    self,
    *,
    participantId: str,
    sessionId: str,
    stageArn: str,
) -> GetParticipantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetParticipantResponseTypeDef](./type_defs.md#getparticipantresponsetypedef) 


```python
# get_participant method usage example with argument unpacking

kwargs: GetParticipantRequestRequestTypeDef = {  # (1)
    "participantId": ...,
    "sessionId": ...,
    "stageArn": ...,
}

parent.get_participant(**kwargs)
```

1. See [:material-code-braces: GetParticipantRequestRequestTypeDef](./type_defs.md#getparticipantrequestrequesttypedef) 

### get\_stage

Gets information for the specified stage.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").get_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_stage)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.get_stage_session)

```python
# get_stage_session method definition

await def get_stage_session(
    self,
    *,
    sessionId: str,
    stageArn: str,
) -> GetStageSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetStageSessionResponseTypeDef](./type_defs.md#getstagesessionresponsetypedef) 


```python
# get_stage_session method usage example with argument unpacking

kwargs: GetStageSessionRequestRequestTypeDef = {  # (1)
    "sessionId": ...,
    "stageArn": ...,
}

parent.get_stage_session(**kwargs)
```

1. See [:material-code-braces: GetStageSessionRequestRequestTypeDef](./type_defs.md#getstagesessionrequestrequesttypedef) 

### list\_participant\_events

Lists events for a specified participant that occurred during a specified stage
session.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_participant_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participant_events)

```python
# list_participant_events method definition

await def list_participant_events(
    self,
    *,
    participantId: str,
    sessionId: str,
    stageArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListParticipantEventsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListParticipantEventsResponseTypeDef](./type_defs.md#listparticipanteventsresponsetypedef) 


```python
# list_participant_events method usage example with argument unpacking

kwargs: ListParticipantEventsRequestRequestTypeDef = {  # (1)
    "participantId": ...,
    "sessionId": ...,
    "stageArn": ...,
}

parent.list_participant_events(**kwargs)
```

1. See [:material-code-braces: ListParticipantEventsRequestRequestTypeDef](./type_defs.md#listparticipanteventsrequestrequesttypedef) 

### list\_participants

Lists all participants in a specified stage session.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_participants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_participants)

```python
# list_participants method definition

await def list_participants(
    self,
    *,
    sessionId: str,
    stageArn: str,
    filterByPublished: bool = ...,
    filterByState: ParticipantStateType = ...,  # (1)
    filterByUserId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListParticipantsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ParticipantStateType](./literals.md#participantstatetype) 
2. See [:material-code-braces: ListParticipantsResponseTypeDef](./type_defs.md#listparticipantsresponsetypedef) 


```python
# list_participants method usage example with argument unpacking

kwargs: ListParticipantsRequestRequestTypeDef = {  # (1)
    "sessionId": ...,
    "stageArn": ...,
}

parent.list_participants(**kwargs)
```

1. See [:material-code-braces: ListParticipantsRequestRequestTypeDef](./type_defs.md#listparticipantsrequestrequesttypedef) 

### list\_stage\_sessions

Gets all sessions for a specified stage.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_stage_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_stage_sessions)

```python
# list_stage_sessions method definition

await def list_stage_sessions(
    self,
    *,
    stageArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_stages)

```python
# list_stages method definition

await def list_stages(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListStagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStagesResponseTypeDef](./type_defs.md#liststagesresponsetypedef) 


```python
# list_stages method usage example with argument unpacking

kwargs: ListStagesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_stages(**kwargs)
```

1. See [:material-code-braces: ListStagesRequestRequestTypeDef](./type_defs.md#liststagesrequestrequesttypedef) 

### list\_tags\_for\_resource

Gets information about AWS tags for the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.list_tags_for_resource)

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

### tag\_resource

Adds or updates tags for the AWS resource with the specified ARN.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.tag_resource)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.untag_resource)

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

### update\_stage

Updates a stage’s configuration.

Type annotations and code completion for `#!python session.create_client("ivs-realtime").update_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.update_stage)

```python
# update_stage method definition

await def update_stage(
    self,
    *,
    arn: str,
    name: str = ...,
) -> UpdateStageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateStageResponseTypeDef](./type_defs.md#updatestageresponsetypedef) 


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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> ivsrealtimeClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("ivs-realtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





