# UserNotificationsContactsClient

> [Index](../README.md) > [UserNotificationsContacts](./README.md) > UserNotificationsContactsClient

!!! note ""

    Auto-generated documentation for [UserNotificationsContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts.html#usernotificationscontacts)
    type annotations stubs module [types-aiobotocore-notificationscontacts](https://pypi.org/project/types-aiobotocore-notificationscontacts/).

## UserNotificationsContactsClient

Type annotations and code completion for `#!python session.create_client("notificationscontacts")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts.html#UserNotificationsContacts.Client)

```python
# UserNotificationsContactsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_notificationscontacts.client import UserNotificationsContactsClient

session = get_session()
async with session.create_client("notificationscontacts") as client:
    client: UserNotificationsContactsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("notificationscontacts").exceptions` structure.

```python
# UserNotificationsContactsClient.exceptions usage example

async with session.create_client("notificationscontacts") as client:
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
# UserNotificationsContactsClient usage type checking example

from types_aiobotocore_notificationscontacts.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("notificationscontacts").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("notificationscontacts").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/generate_presigned_url.html)

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


### activate\_email\_contact

Activates an email contact using an activation code.

Type annotations and code completion for `#!python session.create_client("notificationscontacts").activate_email_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/activate_email_contact.html)

```python
# activate_email_contact method definition

await def activate_email_contact(
    self,
    *,
    arn: str,
    code: str,
) -> Dict[str, Any]:
    ...
```



```python
# activate_email_contact method usage example with argument unpacking

kwargs: ActivateEmailContactRequestTypeDef = {  # (1)
    "arn": ...,
    "code": ...,
}

parent.activate_email_contact(**kwargs)
```

1. See [:material-code-braces: ActivateEmailContactRequestTypeDef](./type_defs.md#activateemailcontactrequesttypedef) 

### create\_email\_contact

Creates an email contact for the provided email address.

Type annotations and code completion for `#!python session.create_client("notificationscontacts").create_email_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/create_email_contact.html)

```python
# create_email_contact method definition

await def create_email_contact(
    self,
    *,
    name: str,
    emailAddress: str,
    tags: Mapping[str, str] = ...,
) -> CreateEmailContactResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateEmailContactResponseTypeDef](./type_defs.md#createemailcontactresponsetypedef) 


```python
# create_email_contact method usage example with argument unpacking

kwargs: CreateEmailContactRequestTypeDef = {  # (1)
    "name": ...,
    "emailAddress": ...,
}

parent.create_email_contact(**kwargs)
```

1. See [:material-code-braces: CreateEmailContactRequestTypeDef](./type_defs.md#createemailcontactrequesttypedef) 

### delete\_email\_contact

Deletes an email contact.

Type annotations and code completion for `#!python session.create_client("notificationscontacts").delete_email_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/delete_email_contact.html)

```python
# delete_email_contact method definition

await def delete_email_contact(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_email_contact method usage example with argument unpacking

kwargs: DeleteEmailContactRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_email_contact(**kwargs)
```

1. See [:material-code-braces: DeleteEmailContactRequestTypeDef](./type_defs.md#deleteemailcontactrequesttypedef) 

### get\_email\_contact

Returns an email contact.

Type annotations and code completion for `#!python session.create_client("notificationscontacts").get_email_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/get_email_contact.html)

```python
# get_email_contact method definition

await def get_email_contact(
    self,
    *,
    arn: str,
) -> GetEmailContactResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEmailContactResponseTypeDef](./type_defs.md#getemailcontactresponsetypedef) 


```python
# get_email_contact method usage example with argument unpacking

kwargs: GetEmailContactRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_email_contact(**kwargs)
```

1. See [:material-code-braces: GetEmailContactRequestTypeDef](./type_defs.md#getemailcontactrequesttypedef) 

### list\_email\_contacts

Lists all email contacts created under the Account.

Type annotations and code completion for `#!python session.create_client("notificationscontacts").list_email_contacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/list_email_contacts.html)

```python
# list_email_contacts method definition

await def list_email_contacts(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEmailContactsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEmailContactsResponseTypeDef](./type_defs.md#listemailcontactsresponsetypedef) 


```python
# list_email_contacts method usage example with argument unpacking

kwargs: ListEmailContactsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_email_contacts(**kwargs)
```

1. See [:material-code-braces: ListEmailContactsRequestTypeDef](./type_defs.md#listemailcontactsrequesttypedef) 

### list\_tags\_for\_resource

Lists all of the tags associated with the Amazon Resource Name (ARN) that you
specify.

Type annotations and code completion for `#!python session.create_client("notificationscontacts").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    arn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### send\_activation\_code

Sends an activation email to the email address associated with the specified
email contact.

Type annotations and code completion for `#!python session.create_client("notificationscontacts").send_activation_code` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/send_activation_code.html)

```python
# send_activation_code method definition

await def send_activation_code(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# send_activation_code method usage example with argument unpacking

kwargs: SendActivationCodeRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.send_activation_code(**kwargs)
```

1. See [:material-code-braces: SendActivationCodeRequestTypeDef](./type_defs.md#sendactivationcoderequesttypedef) 

### tag\_resource

Attaches a key-value pair to a resource, as identified by its Amazon Resource
Name (ARN).

Type annotations and code completion for `#!python session.create_client("notificationscontacts").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    arn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "arn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Detaches a key-value pair from a resource, as identified by its Amazon Resource
Name (ARN).

Type annotations and code completion for `#!python session.create_client("notificationscontacts").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    arn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "arn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("notificationscontacts").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts.html#UserNotificationsContacts.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("notificationscontacts").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts.html#UserNotificationsContacts.Client)

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

Type annotations and code completion for `#!python session.create_client("notificationscontacts").get_paginator` method with overloads.

- `client.get_paginator("list_email_contacts")` -> [ListEmailContactsPaginator](./paginators.md#listemailcontactspaginator)



