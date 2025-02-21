# ConnectParticipantClient

> [Index](../README.md) > [ConnectParticipant](./README.md) > ConnectParticipantClient

!!! note ""

    Auto-generated documentation for [ConnectParticipant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#connectparticipant)
    type annotations stubs module [types-aiobotocore-connectparticipant](https://pypi.org/project/types-aiobotocore-connectparticipant/).

## ConnectParticipantClient

Type annotations and code completion for `#!python session.create_client("connectparticipant")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant.Client)

```python
# ConnectParticipantClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_connectparticipant.client import ConnectParticipantClient

session = get_session()
async with session.create_client("connectparticipant") as client:
    client: ConnectParticipantClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("connectparticipant").exceptions` structure.

```python
# ConnectParticipantClient.exceptions usage example

async with session.create_client("connectparticipant") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# ConnectParticipantClient usage type checking example

from types_aiobotocore_connectparticipant.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("connectparticipant").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("connectparticipant").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/generate_presigned_url.html)

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


### cancel\_participant\_authentication

Cancels the authentication session.

Type annotations and code completion for `#!python session.create_client("connectparticipant").cancel_participant_authentication` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/cancel_participant_authentication.html)

```python
# cancel_participant_authentication method definition

await def cancel_participant_authentication(
    self,
    *,
    SessionId: str,
    ConnectionToken: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_participant_authentication method usage example with argument unpacking

kwargs: CancelParticipantAuthenticationRequestTypeDef = {  # (1)
    "SessionId": ...,
    "ConnectionToken": ...,
}

parent.cancel_participant_authentication(**kwargs)
```

1. See [:material-code-braces: CancelParticipantAuthenticationRequestTypeDef](./type_defs.md#cancelparticipantauthenticationrequesttypedef) 

### complete\_attachment\_upload

Allows you to confirm that the attachment has been uploaded using the
pre-signed URL provided in StartAttachmentUpload API.

Type annotations and code completion for `#!python session.create_client("connectparticipant").complete_attachment_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/complete_attachment_upload.html)

```python
# complete_attachment_upload method definition

await def complete_attachment_upload(
    self,
    *,
    AttachmentIds: Sequence[str],
    ClientToken: str,
    ConnectionToken: str,
) -> Dict[str, Any]:
    ...
```



```python
# complete_attachment_upload method usage example with argument unpacking

kwargs: CompleteAttachmentUploadRequestTypeDef = {  # (1)
    "AttachmentIds": ...,
    "ClientToken": ...,
    "ConnectionToken": ...,
}

parent.complete_attachment_upload(**kwargs)
```

1. See [:material-code-braces: CompleteAttachmentUploadRequestTypeDef](./type_defs.md#completeattachmentuploadrequesttypedef) 

### create\_participant\_connection

Creates the participant's connection.

Type annotations and code completion for `#!python session.create_client("connectparticipant").create_participant_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/create_participant_connection.html)

```python
# create_participant_connection method definition

await def create_participant_connection(
    self,
    *,
    ParticipantToken: str,
    Type: Sequence[ConnectionTypeType] = ...,  # (1)
    ConnectParticipant: bool = ...,
) -> CreateParticipantConnectionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-braces: CreateParticipantConnectionResponseTypeDef](./type_defs.md#createparticipantconnectionresponsetypedef) 


```python
# create_participant_connection method usage example with argument unpacking

kwargs: CreateParticipantConnectionRequestTypeDef = {  # (1)
    "ParticipantToken": ...,
}

parent.create_participant_connection(**kwargs)
```

1. See [:material-code-braces: CreateParticipantConnectionRequestTypeDef](./type_defs.md#createparticipantconnectionrequesttypedef) 

### describe\_view

Retrieves the view for the specified view token.

Type annotations and code completion for `#!python session.create_client("connectparticipant").describe_view` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/describe_view.html)

```python
# describe_view method definition

await def describe_view(
    self,
    *,
    ViewToken: str,
    ConnectionToken: str,
) -> DescribeViewResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeViewResponseTypeDef](./type_defs.md#describeviewresponsetypedef) 


```python
# describe_view method usage example with argument unpacking

kwargs: DescribeViewRequestTypeDef = {  # (1)
    "ViewToken": ...,
    "ConnectionToken": ...,
}

parent.describe_view(**kwargs)
```

1. See [:material-code-braces: DescribeViewRequestTypeDef](./type_defs.md#describeviewrequesttypedef) 

### disconnect\_participant

Disconnects a participant.

Type annotations and code completion for `#!python session.create_client("connectparticipant").disconnect_participant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/disconnect_participant.html)

```python
# disconnect_participant method definition

await def disconnect_participant(
    self,
    *,
    ConnectionToken: str,
    ClientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disconnect_participant method usage example with argument unpacking

kwargs: DisconnectParticipantRequestTypeDef = {  # (1)
    "ConnectionToken": ...,
}

parent.disconnect_participant(**kwargs)
```

1. See [:material-code-braces: DisconnectParticipantRequestTypeDef](./type_defs.md#disconnectparticipantrequesttypedef) 

### get\_attachment

Provides a pre-signed URL for download of a completed attachment.

Type annotations and code completion for `#!python session.create_client("connectparticipant").get_attachment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/get_attachment.html)

```python
# get_attachment method definition

await def get_attachment(
    self,
    *,
    AttachmentId: str,
    ConnectionToken: str,
    UrlExpiryInSeconds: int = ...,
) -> GetAttachmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAttachmentResponseTypeDef](./type_defs.md#getattachmentresponsetypedef) 


```python
# get_attachment method usage example with argument unpacking

kwargs: GetAttachmentRequestTypeDef = {  # (1)
    "AttachmentId": ...,
    "ConnectionToken": ...,
}

parent.get_attachment(**kwargs)
```

1. See [:material-code-braces: GetAttachmentRequestTypeDef](./type_defs.md#getattachmentrequesttypedef) 

### get\_authentication\_url

Retrieves the AuthenticationUrl for the current authentication session for the
AuthenticateCustomer flow block.

Type annotations and code completion for `#!python session.create_client("connectparticipant").get_authentication_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/get_authentication_url.html)

```python
# get_authentication_url method definition

await def get_authentication_url(
    self,
    *,
    SessionId: str,
    RedirectUri: str,
    ConnectionToken: str,
) -> GetAuthenticationUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAuthenticationUrlResponseTypeDef](./type_defs.md#getauthenticationurlresponsetypedef) 


```python
# get_authentication_url method usage example with argument unpacking

kwargs: GetAuthenticationUrlRequestTypeDef = {  # (1)
    "SessionId": ...,
    "RedirectUri": ...,
    "ConnectionToken": ...,
}

parent.get_authentication_url(**kwargs)
```

1. See [:material-code-braces: GetAuthenticationUrlRequestTypeDef](./type_defs.md#getauthenticationurlrequesttypedef) 

### get\_transcript

Retrieves a transcript of the session, including details about any attachments.

Type annotations and code completion for `#!python session.create_client("connectparticipant").get_transcript` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/get_transcript.html)

```python
# get_transcript method definition

await def get_transcript(
    self,
    *,
    ConnectionToken: str,
    ContactId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ScanDirection: ScanDirectionType = ...,  # (1)
    SortOrder: SortKeyType = ...,  # (2)
    StartPosition: StartPositionTypeDef = ...,  # (3)
) -> GetTranscriptResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ScanDirectionType](./literals.md#scandirectiontype) 
2. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
3. See [:material-code-braces: StartPositionTypeDef](./type_defs.md#startpositiontypedef) 
4. See [:material-code-braces: GetTranscriptResponseTypeDef](./type_defs.md#gettranscriptresponsetypedef) 


```python
# get_transcript method usage example with argument unpacking

kwargs: GetTranscriptRequestTypeDef = {  # (1)
    "ConnectionToken": ...,
}

parent.get_transcript(**kwargs)
```

1. See [:material-code-braces: GetTranscriptRequestTypeDef](./type_defs.md#gettranscriptrequesttypedef) 

### send\_event

The
<code>application/vnd.amazonaws.connect.event.connection.acknowledged</code>
ContentType will no longer be supported starting December 31, 2024.

Type annotations and code completion for `#!python session.create_client("connectparticipant").send_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/send_event.html)

```python
# send_event method definition

await def send_event(
    self,
    *,
    ContentType: str,
    ConnectionToken: str,
    Content: str = ...,
    ClientToken: str = ...,
) -> SendEventResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SendEventResponseTypeDef](./type_defs.md#sendeventresponsetypedef) 


```python
# send_event method usage example with argument unpacking

kwargs: SendEventRequestTypeDef = {  # (1)
    "ContentType": ...,
    "ConnectionToken": ...,
}

parent.send_event(**kwargs)
```

1. See [:material-code-braces: SendEventRequestTypeDef](./type_defs.md#sendeventrequesttypedef) 

### send\_message

Sends a message.

Type annotations and code completion for `#!python session.create_client("connectparticipant").send_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/send_message.html)

```python
# send_message method definition

await def send_message(
    self,
    *,
    ContentType: str,
    Content: str,
    ConnectionToken: str,
    ClientToken: str = ...,
) -> SendMessageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SendMessageResponseTypeDef](./type_defs.md#sendmessageresponsetypedef) 


```python
# send_message method usage example with argument unpacking

kwargs: SendMessageRequestTypeDef = {  # (1)
    "ContentType": ...,
    "Content": ...,
    "ConnectionToken": ...,
}

parent.send_message(**kwargs)
```

1. See [:material-code-braces: SendMessageRequestTypeDef](./type_defs.md#sendmessagerequesttypedef) 

### start\_attachment\_upload

Provides a pre-signed Amazon S3 URL in response for uploading the file directly
to S3.

Type annotations and code completion for `#!python session.create_client("connectparticipant").start_attachment_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant/client/start_attachment_upload.html)

```python
# start_attachment_upload method definition

await def start_attachment_upload(
    self,
    *,
    ContentType: str,
    AttachmentSizeInBytes: int,
    AttachmentName: str,
    ClientToken: str,
    ConnectionToken: str,
) -> StartAttachmentUploadResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartAttachmentUploadResponseTypeDef](./type_defs.md#startattachmentuploadresponsetypedef) 


```python
# start_attachment_upload method usage example with argument unpacking

kwargs: StartAttachmentUploadRequestTypeDef = {  # (1)
    "ContentType": ...,
    "AttachmentSizeInBytes": ...,
    "AttachmentName": ...,
    "ClientToken": ...,
    "ConnectionToken": ...,
}

parent.start_attachment_upload(**kwargs)
```

1. See [:material-code-braces: StartAttachmentUploadRequestTypeDef](./type_defs.md#startattachmentuploadrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("connectparticipant").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("connectparticipant").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant.Client)

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





