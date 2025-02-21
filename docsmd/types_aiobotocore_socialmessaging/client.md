# EndUserMessagingSocialClient

> [Index](../README.md) > [EndUserMessagingSocial](./README.md) > EndUserMessagingSocialClient

!!! note ""

    Auto-generated documentation for [EndUserMessagingSocial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#endusermessagingsocial)
    type annotations stubs module [types-aiobotocore-socialmessaging](https://pypi.org/project/types-aiobotocore-socialmessaging/).

## EndUserMessagingSocialClient

Type annotations and code completion for `#!python session.create_client("socialmessaging")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#EndUserMessagingSocial.Client)

```python
# EndUserMessagingSocialClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_socialmessaging.client import EndUserMessagingSocialClient

session = get_session()
async with session.create_client("socialmessaging") as client:
    client: EndUserMessagingSocialClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("socialmessaging").exceptions` structure.

```python
# EndUserMessagingSocialClient.exceptions usage example

async with session.create_client("socialmessaging") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedByMetaException,
        client.AccessDeniedException,
        client.ClientError,
        client.DependencyException,
        client.InternalServiceException,
        client.InvalidParametersException,
        client.ResourceNotFoundException,
        client.ThrottledRequestException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# EndUserMessagingSocialClient usage type checking example

from types_aiobotocore_socialmessaging.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedByMetaException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("socialmessaging").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("socialmessaging").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/generate_presigned_url.html)

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


### associate\_whatsapp\_business\_account

This is only used through the Amazon Web Services console during sign-up to
associate your WhatsApp Business Account to your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("socialmessaging").associate_whatsapp_business_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/associate_whatsapp_business_account.html)

```python
# associate_whatsapp_business_account method definition

await def associate_whatsapp_business_account(
    self,
    *,
    signupCallback: WhatsAppSignupCallbackTypeDef = ...,  # (1)
    setupFinalization: WhatsAppSetupFinalizationTypeDef = ...,  # (2)
) -> AssociateWhatsAppBusinessAccountOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: WhatsAppSignupCallbackTypeDef](./type_defs.md#whatsappsignupcallbacktypedef) 
2. See [:material-code-braces: WhatsAppSetupFinalizationTypeDef](./type_defs.md#whatsappsetupfinalizationtypedef) 
3. See [:material-code-braces: AssociateWhatsAppBusinessAccountOutputTypeDef](./type_defs.md#associatewhatsappbusinessaccountoutputtypedef) 


```python
# associate_whatsapp_business_account method usage example with argument unpacking

kwargs: AssociateWhatsAppBusinessAccountInputTypeDef = {  # (1)
    "signupCallback": ...,
}

parent.associate_whatsapp_business_account(**kwargs)
```

1. See [:material-code-braces: AssociateWhatsAppBusinessAccountInputTypeDef](./type_defs.md#associatewhatsappbusinessaccountinputtypedef) 

### delete\_whatsapp\_media\_message

Delete a media object from the WhatsApp service.

Type annotations and code completion for `#!python session.create_client("socialmessaging").delete_whatsapp_media_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/delete_whatsapp_media_message.html)

```python
# delete_whatsapp_media_message method definition

await def delete_whatsapp_media_message(
    self,
    *,
    mediaId: str,
    originationPhoneNumberId: str,
) -> DeleteWhatsAppMessageMediaOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWhatsAppMessageMediaOutputTypeDef](./type_defs.md#deletewhatsappmessagemediaoutputtypedef) 


```python
# delete_whatsapp_media_message method usage example with argument unpacking

kwargs: DeleteWhatsAppMessageMediaInputTypeDef = {  # (1)
    "mediaId": ...,
    "originationPhoneNumberId": ...,
}

parent.delete_whatsapp_media_message(**kwargs)
```

1. See [:material-code-braces: DeleteWhatsAppMessageMediaInputTypeDef](./type_defs.md#deletewhatsappmessagemediainputtypedef) 

### disassociate\_whatsapp\_business\_account

Disassociate a WhatsApp Business Account (WABA) from your Amazon Web Services
account.

Type annotations and code completion for `#!python session.create_client("socialmessaging").disassociate_whatsapp_business_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/disassociate_whatsapp_business_account.html)

```python
# disassociate_whatsapp_business_account method definition

await def disassociate_whatsapp_business_account(
    self,
    *,
    id: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_whatsapp_business_account method usage example with argument unpacking

kwargs: DisassociateWhatsAppBusinessAccountInputTypeDef = {  # (1)
    "id": ...,
}

parent.disassociate_whatsapp_business_account(**kwargs)
```

1. See [:material-code-braces: DisassociateWhatsAppBusinessAccountInputTypeDef](./type_defs.md#disassociatewhatsappbusinessaccountinputtypedef) 

### get\_linked\_whatsapp\_business\_account

Get the details of your linked WhatsApp Business Account.

Type annotations and code completion for `#!python session.create_client("socialmessaging").get_linked_whatsapp_business_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/get_linked_whatsapp_business_account.html)

```python
# get_linked_whatsapp_business_account method definition

await def get_linked_whatsapp_business_account(
    self,
    *,
    id: str,
) -> GetLinkedWhatsAppBusinessAccountOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLinkedWhatsAppBusinessAccountOutputTypeDef](./type_defs.md#getlinkedwhatsappbusinessaccountoutputtypedef) 


```python
# get_linked_whatsapp_business_account method usage example with argument unpacking

kwargs: GetLinkedWhatsAppBusinessAccountInputTypeDef = {  # (1)
    "id": ...,
}

parent.get_linked_whatsapp_business_account(**kwargs)
```

1. See [:material-code-braces: GetLinkedWhatsAppBusinessAccountInputTypeDef](./type_defs.md#getlinkedwhatsappbusinessaccountinputtypedef) 

### get\_linked\_whatsapp\_business\_account\_phone\_number

Use your WhatsApp phone number id to get the WABA account id and phone number
details.

Type annotations and code completion for `#!python session.create_client("socialmessaging").get_linked_whatsapp_business_account_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/get_linked_whatsapp_business_account_phone_number.html)

```python
# get_linked_whatsapp_business_account_phone_number method definition

await def get_linked_whatsapp_business_account_phone_number(
    self,
    *,
    id: str,
) -> GetLinkedWhatsAppBusinessAccountPhoneNumberOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLinkedWhatsAppBusinessAccountPhoneNumberOutputTypeDef](./type_defs.md#getlinkedwhatsappbusinessaccountphonenumberoutputtypedef) 


```python
# get_linked_whatsapp_business_account_phone_number method usage example with argument unpacking

kwargs: GetLinkedWhatsAppBusinessAccountPhoneNumberInputTypeDef = {  # (1)
    "id": ...,
}

parent.get_linked_whatsapp_business_account_phone_number(**kwargs)
```

1. See [:material-code-braces: GetLinkedWhatsAppBusinessAccountPhoneNumberInputTypeDef](./type_defs.md#getlinkedwhatsappbusinessaccountphonenumberinputtypedef) 

### get\_whatsapp\_message\_media

Get a media file from the WhatsApp service.

Type annotations and code completion for `#!python session.create_client("socialmessaging").get_whatsapp_message_media` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/get_whatsapp_message_media.html)

```python
# get_whatsapp_message_media method definition

await def get_whatsapp_message_media(
    self,
    *,
    mediaId: str,
    originationPhoneNumberId: str,
    metadataOnly: bool = ...,
    destinationS3PresignedUrl: S3PresignedUrlTypeDef = ...,  # (1)
    destinationS3File: S3FileTypeDef = ...,  # (2)
) -> GetWhatsAppMessageMediaOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: S3PresignedUrlTypeDef](./type_defs.md#s3presignedurltypedef) 
2. See [:material-code-braces: S3FileTypeDef](./type_defs.md#s3filetypedef) 
3. See [:material-code-braces: GetWhatsAppMessageMediaOutputTypeDef](./type_defs.md#getwhatsappmessagemediaoutputtypedef) 


```python
# get_whatsapp_message_media method usage example with argument unpacking

kwargs: GetWhatsAppMessageMediaInputTypeDef = {  # (1)
    "mediaId": ...,
    "originationPhoneNumberId": ...,
}

parent.get_whatsapp_message_media(**kwargs)
```

1. See [:material-code-braces: GetWhatsAppMessageMediaInputTypeDef](./type_defs.md#getwhatsappmessagemediainputtypedef) 

### list\_linked\_whatsapp\_business\_accounts

List all WhatsApp Business Accounts linked to your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("socialmessaging").list_linked_whatsapp_business_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/list_linked_whatsapp_business_accounts.html)

```python
# list_linked_whatsapp_business_accounts method definition

await def list_linked_whatsapp_business_accounts(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListLinkedWhatsAppBusinessAccountsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLinkedWhatsAppBusinessAccountsOutputTypeDef](./type_defs.md#listlinkedwhatsappbusinessaccountsoutputtypedef) 


```python
# list_linked_whatsapp_business_accounts method usage example with argument unpacking

kwargs: ListLinkedWhatsAppBusinessAccountsInputTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_linked_whatsapp_business_accounts(**kwargs)
```

1. See [:material-code-braces: ListLinkedWhatsAppBusinessAccountsInputTypeDef](./type_defs.md#listlinkedwhatsappbusinessaccountsinputtypedef) 

### list\_tags\_for\_resource

List all tags associated with a resource, such as a phone number or WABA.

Type annotations and code completion for `#!python session.create_client("socialmessaging").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef) 

### post\_whatsapp\_message\_media

Upload a media file to the WhatsApp service.

Type annotations and code completion for `#!python session.create_client("socialmessaging").post_whatsapp_message_media` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/post_whatsapp_message_media.html)

```python
# post_whatsapp_message_media method definition

await def post_whatsapp_message_media(
    self,
    *,
    originationPhoneNumberId: str,
    sourceS3PresignedUrl: S3PresignedUrlTypeDef = ...,  # (1)
    sourceS3File: S3FileTypeDef = ...,  # (2)
) -> PostWhatsAppMessageMediaOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: S3PresignedUrlTypeDef](./type_defs.md#s3presignedurltypedef) 
2. See [:material-code-braces: S3FileTypeDef](./type_defs.md#s3filetypedef) 
3. See [:material-code-braces: PostWhatsAppMessageMediaOutputTypeDef](./type_defs.md#postwhatsappmessagemediaoutputtypedef) 


```python
# post_whatsapp_message_media method usage example with argument unpacking

kwargs: PostWhatsAppMessageMediaInputTypeDef = {  # (1)
    "originationPhoneNumberId": ...,
}

parent.post_whatsapp_message_media(**kwargs)
```

1. See [:material-code-braces: PostWhatsAppMessageMediaInputTypeDef](./type_defs.md#postwhatsappmessagemediainputtypedef) 

### put\_whatsapp\_business\_account\_event\_destinations

Add an event destination to log event data from WhatsApp for a WhatsApp
Business Account (WABA).

Type annotations and code completion for `#!python session.create_client("socialmessaging").put_whatsapp_business_account_event_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/put_whatsapp_business_account_event_destinations.html)

```python
# put_whatsapp_business_account_event_destinations method definition

await def put_whatsapp_business_account_event_destinations(
    self,
    *,
    id: str,
    eventDestinations: Sequence[WhatsAppBusinessAccountEventDestinationTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: WhatsAppBusinessAccountEventDestinationTypeDef](./type_defs.md#whatsappbusinessaccounteventdestinationtypedef) 


```python
# put_whatsapp_business_account_event_destinations method usage example with argument unpacking

kwargs: PutWhatsAppBusinessAccountEventDestinationsInputTypeDef = {  # (1)
    "id": ...,
    "eventDestinations": ...,
}

parent.put_whatsapp_business_account_event_destinations(**kwargs)
```

1. See [:material-code-braces: PutWhatsAppBusinessAccountEventDestinationsInputTypeDef](./type_defs.md#putwhatsappbusinessaccounteventdestinationsinputtypedef) 

### send\_whatsapp\_message

Send a WhatsApp message.

Type annotations and code completion for `#!python session.create_client("socialmessaging").send_whatsapp_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/send_whatsapp_message.html)

```python
# send_whatsapp_message method definition

await def send_whatsapp_message(
    self,
    *,
    originationPhoneNumberId: str,
    message: BlobTypeDef,
    metaApiVersion: str,
) -> SendWhatsAppMessageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SendWhatsAppMessageOutputTypeDef](./type_defs.md#sendwhatsappmessageoutputtypedef) 


```python
# send_whatsapp_message method usage example with argument unpacking

kwargs: SendWhatsAppMessageInputTypeDef = {  # (1)
    "originationPhoneNumberId": ...,
    "message": ...,
    "metaApiVersion": ...,
}

parent.send_whatsapp_message(**kwargs)
```

1. See [:material-code-braces: SendWhatsAppMessageInputTypeDef](./type_defs.md#sendwhatsappmessageinputtypedef) 

### tag\_resource

Adds or overwrites only the specified tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("socialmessaging").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> TagResourceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: TagResourceOutputTypeDef](./type_defs.md#tagresourceoutputtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef) 

### untag\_resource

Removes the specified tags from a resource.

Type annotations and code completion for `#!python session.create_client("socialmessaging").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> UntagResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UntagResourceOutputTypeDef](./type_defs.md#untagresourceoutputtypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("socialmessaging").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#EndUserMessagingSocial.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("socialmessaging").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#EndUserMessagingSocial.Client)

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

Type annotations and code completion for `#!python session.create_client("socialmessaging").get_paginator` method with overloads.

- `client.get_paginator("list_linked_whatsapp_business_accounts")` -> [ListLinkedWhatsAppBusinessAccountsPaginator](./paginators.md#listlinkedwhatsappbusinessaccountspaginator)



