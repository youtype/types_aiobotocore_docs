# SSMContactsClient

> [Index](../README.md) > [SSMContacts](./README.md) > SSMContactsClient

!!! note ""

    Auto-generated documentation for [SSMContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#ssmcontacts)
    type annotations stubs module [types-aiobotocore-ssm-contacts](https://pypi.org/project/types-aiobotocore-ssm-contacts/).

## SSMContactsClient

Type annotations and code completion for `#!python session.create_client("ssm-contacts")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client)

```python
# SSMContactsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_ssm_contacts.client import SSMContactsClient

session = get_session()
async with session.create_client("ssm-contacts") as client:
    client: SSMContactsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("ssm-contacts").exceptions` structure.

```python
# SSMContactsClient.exceptions usage example

async with session.create_client("ssm-contacts") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.DataEncryptionException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SSMContactsClient usage type checking example

from types_aiobotocore_ssm_contacts.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("ssm-contacts").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("ssm-contacts").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("ssm-contacts").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### accept\_page

Used to acknowledge an engagement to a contact channel during an incident.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").accept_page` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/accept_page.html)

```python
# accept_page method definition

await def accept_page(
    self,
    *,
    PageId: str,
    AcceptType: AcceptTypeType,  # (1)
    AcceptCode: str,
    ContactChannelId: str = ...,
    Note: str = ...,
    AcceptCodeValidation: AcceptCodeValidationType = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: AcceptTypeType](./literals.md#accepttypetype) 
2. See [:material-code-brackets: AcceptCodeValidationType](./literals.md#acceptcodevalidationtype) 


```python
# accept_page method usage example with argument unpacking

kwargs: AcceptPageRequestRequestTypeDef = {  # (1)
    "PageId": ...,
    "AcceptType": ...,
    "AcceptCode": ...,
}

parent.accept_page(**kwargs)
```

1. See [:material-code-braces: AcceptPageRequestRequestTypeDef](./type_defs.md#acceptpagerequestrequesttypedef) 

### activate\_contact\_channel

Activates a contact's contact channel.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").activate_contact_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/activate_contact_channel.html)

```python
# activate_contact_channel method definition

await def activate_contact_channel(
    self,
    *,
    ContactChannelId: str,
    ActivationCode: str,
) -> Dict[str, Any]:
    ...
```



```python
# activate_contact_channel method usage example with argument unpacking

kwargs: ActivateContactChannelRequestRequestTypeDef = {  # (1)
    "ContactChannelId": ...,
    "ActivationCode": ...,
}

parent.activate_contact_channel(**kwargs)
```

1. See [:material-code-braces: ActivateContactChannelRequestRequestTypeDef](./type_defs.md#activatecontactchannelrequestrequesttypedef) 

### create\_contact

Contacts are either the contacts that Incident Manager engages during an
incident or the escalation plans that Incident Manager uses to engage contacts
in phases during an incident.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").create_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/create_contact.html)

```python
# create_contact method definition

await def create_contact(
    self,
    *,
    Alias: str,
    Type: ContactTypeType,  # (1)
    Plan: PlanTypeDef,  # (2)
    DisplayName: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    IdempotencyToken: str = ...,
) -> CreateContactResultTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ContactTypeType](./literals.md#contacttypetype) 
2. See [:material-code-braces: PlanTypeDef](./type_defs.md#plantypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateContactResultTypeDef](./type_defs.md#createcontactresulttypedef) 


```python
# create_contact method usage example with argument unpacking

kwargs: CreateContactRequestRequestTypeDef = {  # (1)
    "Alias": ...,
    "Type": ...,
    "Plan": ...,
}

parent.create_contact(**kwargs)
```

1. See [:material-code-braces: CreateContactRequestRequestTypeDef](./type_defs.md#createcontactrequestrequesttypedef) 

### create\_contact\_channel

A contact channel is the method that Incident Manager uses to engage your
contact.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").create_contact_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/create_contact_channel.html)

```python
# create_contact_channel method definition

await def create_contact_channel(
    self,
    *,
    ContactId: str,
    Name: str,
    Type: ChannelTypeType,  # (1)
    DeliveryAddress: ContactChannelAddressTypeDef,  # (2)
    DeferActivation: bool = ...,
    IdempotencyToken: str = ...,
) -> CreateContactChannelResultTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-braces: ContactChannelAddressTypeDef](./type_defs.md#contactchanneladdresstypedef) 
3. See [:material-code-braces: CreateContactChannelResultTypeDef](./type_defs.md#createcontactchannelresulttypedef) 


```python
# create_contact_channel method usage example with argument unpacking

kwargs: CreateContactChannelRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
    "Name": ...,
    "Type": ...,
    "DeliveryAddress": ...,
}

parent.create_contact_channel(**kwargs)
```

1. See [:material-code-braces: CreateContactChannelRequestRequestTypeDef](./type_defs.md#createcontactchannelrequestrequesttypedef) 

### create\_rotation

Creates a rotation in an on-call schedule.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").create_rotation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/create_rotation.html)

```python
# create_rotation method definition

await def create_rotation(
    self,
    *,
    Name: str,
    ContactIds: Sequence[str],
    TimeZoneId: str,
    Recurrence: RecurrenceSettingsTypeDef,  # (1)
    StartTime: TimestampTypeDef = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    IdempotencyToken: str = ...,
) -> CreateRotationResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RecurrenceSettingsTypeDef](./type_defs.md#recurrencesettingstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateRotationResultTypeDef](./type_defs.md#createrotationresulttypedef) 


```python
# create_rotation method usage example with argument unpacking

kwargs: CreateRotationRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ContactIds": ...,
    "TimeZoneId": ...,
    "Recurrence": ...,
}

parent.create_rotation(**kwargs)
```

1. See [:material-code-braces: CreateRotationRequestRequestTypeDef](./type_defs.md#createrotationrequestrequesttypedef) 

### create\_rotation\_override

Creates an override for a rotation in an on-call schedule.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").create_rotation_override` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/create_rotation_override.html)

```python
# create_rotation_override method definition

await def create_rotation_override(
    self,
    *,
    RotationId: str,
    NewContactIds: Sequence[str],
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    IdempotencyToken: str = ...,
) -> CreateRotationOverrideResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRotationOverrideResultTypeDef](./type_defs.md#createrotationoverrideresulttypedef) 


```python
# create_rotation_override method usage example with argument unpacking

kwargs: CreateRotationOverrideRequestRequestTypeDef = {  # (1)
    "RotationId": ...,
    "NewContactIds": ...,
    "StartTime": ...,
    "EndTime": ...,
}

parent.create_rotation_override(**kwargs)
```

1. See [:material-code-braces: CreateRotationOverrideRequestRequestTypeDef](./type_defs.md#createrotationoverriderequestrequesttypedef) 

### deactivate\_contact\_channel

To no longer receive Incident Manager engagements to a contact channel, you can
deactivate the channel.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").deactivate_contact_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/deactivate_contact_channel.html)

```python
# deactivate_contact_channel method definition

await def deactivate_contact_channel(
    self,
    *,
    ContactChannelId: str,
) -> Dict[str, Any]:
    ...
```



```python
# deactivate_contact_channel method usage example with argument unpacking

kwargs: DeactivateContactChannelRequestRequestTypeDef = {  # (1)
    "ContactChannelId": ...,
}

parent.deactivate_contact_channel(**kwargs)
```

1. See [:material-code-braces: DeactivateContactChannelRequestRequestTypeDef](./type_defs.md#deactivatecontactchannelrequestrequesttypedef) 

### delete\_contact

To remove a contact from Incident Manager, you can delete the contact.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").delete_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/delete_contact.html)

```python
# delete_contact method definition

await def delete_contact(
    self,
    *,
    ContactId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_contact method usage example with argument unpacking

kwargs: DeleteContactRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
}

parent.delete_contact(**kwargs)
```

1. See [:material-code-braces: DeleteContactRequestRequestTypeDef](./type_defs.md#deletecontactrequestrequesttypedef) 

### delete\_contact\_channel

To no longer receive engagements on a contact channel, you can delete the
channel from a contact.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").delete_contact_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/delete_contact_channel.html)

```python
# delete_contact_channel method definition

await def delete_contact_channel(
    self,
    *,
    ContactChannelId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_contact_channel method usage example with argument unpacking

kwargs: DeleteContactChannelRequestRequestTypeDef = {  # (1)
    "ContactChannelId": ...,
}

parent.delete_contact_channel(**kwargs)
```

1. See [:material-code-braces: DeleteContactChannelRequestRequestTypeDef](./type_defs.md#deletecontactchannelrequestrequesttypedef) 

### delete\_rotation

Deletes a rotation from the system.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").delete_rotation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/delete_rotation.html)

```python
# delete_rotation method definition

await def delete_rotation(
    self,
    *,
    RotationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_rotation method usage example with argument unpacking

kwargs: DeleteRotationRequestRequestTypeDef = {  # (1)
    "RotationId": ...,
}

parent.delete_rotation(**kwargs)
```

1. See [:material-code-braces: DeleteRotationRequestRequestTypeDef](./type_defs.md#deleterotationrequestrequesttypedef) 

### delete\_rotation\_override

Deletes an existing override for an on-call rotation.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").delete_rotation_override` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/delete_rotation_override.html)

```python
# delete_rotation_override method definition

await def delete_rotation_override(
    self,
    *,
    RotationId: str,
    RotationOverrideId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_rotation_override method usage example with argument unpacking

kwargs: DeleteRotationOverrideRequestRequestTypeDef = {  # (1)
    "RotationId": ...,
    "RotationOverrideId": ...,
}

parent.delete_rotation_override(**kwargs)
```

1. See [:material-code-braces: DeleteRotationOverrideRequestRequestTypeDef](./type_defs.md#deleterotationoverriderequestrequesttypedef) 

### describe\_engagement

Incident Manager uses engagements to engage contacts and escalation plans
during an incident.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").describe_engagement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/describe_engagement.html)

```python
# describe_engagement method definition

await def describe_engagement(
    self,
    *,
    EngagementId: str,
) -> DescribeEngagementResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEngagementResultTypeDef](./type_defs.md#describeengagementresulttypedef) 


```python
# describe_engagement method usage example with argument unpacking

kwargs: DescribeEngagementRequestRequestTypeDef = {  # (1)
    "EngagementId": ...,
}

parent.describe_engagement(**kwargs)
```

1. See [:material-code-braces: DescribeEngagementRequestRequestTypeDef](./type_defs.md#describeengagementrequestrequesttypedef) 

### describe\_page

Lists details of the engagement to a contact channel.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").describe_page` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/describe_page.html)

```python
# describe_page method definition

await def describe_page(
    self,
    *,
    PageId: str,
) -> DescribePageResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePageResultTypeDef](./type_defs.md#describepageresulttypedef) 


```python
# describe_page method usage example with argument unpacking

kwargs: DescribePageRequestRequestTypeDef = {  # (1)
    "PageId": ...,
}

parent.describe_page(**kwargs)
```

1. See [:material-code-braces: DescribePageRequestRequestTypeDef](./type_defs.md#describepagerequestrequesttypedef) 

### get\_contact

Retrieves information about the specified contact or escalation plan.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").get_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/get_contact.html)

```python
# get_contact method definition

await def get_contact(
    self,
    *,
    ContactId: str,
) -> GetContactResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContactResultTypeDef](./type_defs.md#getcontactresulttypedef) 


```python
# get_contact method usage example with argument unpacking

kwargs: GetContactRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
}

parent.get_contact(**kwargs)
```

1. See [:material-code-braces: GetContactRequestRequestTypeDef](./type_defs.md#getcontactrequestrequesttypedef) 

### get\_contact\_channel

List details about a specific contact channel.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").get_contact_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/get_contact_channel.html)

```python
# get_contact_channel method definition

await def get_contact_channel(
    self,
    *,
    ContactChannelId: str,
) -> GetContactChannelResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContactChannelResultTypeDef](./type_defs.md#getcontactchannelresulttypedef) 


```python
# get_contact_channel method usage example with argument unpacking

kwargs: GetContactChannelRequestRequestTypeDef = {  # (1)
    "ContactChannelId": ...,
}

parent.get_contact_channel(**kwargs)
```

1. See [:material-code-braces: GetContactChannelRequestRequestTypeDef](./type_defs.md#getcontactchannelrequestrequesttypedef) 

### get\_contact\_policy

Retrieves the resource policies attached to the specified contact or escalation
plan.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").get_contact_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/get_contact_policy.html)

```python
# get_contact_policy method definition

await def get_contact_policy(
    self,
    *,
    ContactArn: str,
) -> GetContactPolicyResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContactPolicyResultTypeDef](./type_defs.md#getcontactpolicyresulttypedef) 


```python
# get_contact_policy method usage example with argument unpacking

kwargs: GetContactPolicyRequestRequestTypeDef = {  # (1)
    "ContactArn": ...,
}

parent.get_contact_policy(**kwargs)
```

1. See [:material-code-braces: GetContactPolicyRequestRequestTypeDef](./type_defs.md#getcontactpolicyrequestrequesttypedef) 

### get\_rotation

Retrieves information about an on-call rotation.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").get_rotation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/get_rotation.html)

```python
# get_rotation method definition

await def get_rotation(
    self,
    *,
    RotationId: str,
) -> GetRotationResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRotationResultTypeDef](./type_defs.md#getrotationresulttypedef) 


```python
# get_rotation method usage example with argument unpacking

kwargs: GetRotationRequestRequestTypeDef = {  # (1)
    "RotationId": ...,
}

parent.get_rotation(**kwargs)
```

1. See [:material-code-braces: GetRotationRequestRequestTypeDef](./type_defs.md#getrotationrequestrequesttypedef) 

### get\_rotation\_override

Retrieves information about an override to an on-call rotation.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").get_rotation_override` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/get_rotation_override.html)

```python
# get_rotation_override method definition

await def get_rotation_override(
    self,
    *,
    RotationId: str,
    RotationOverrideId: str,
) -> GetRotationOverrideResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRotationOverrideResultTypeDef](./type_defs.md#getrotationoverrideresulttypedef) 


```python
# get_rotation_override method usage example with argument unpacking

kwargs: GetRotationOverrideRequestRequestTypeDef = {  # (1)
    "RotationId": ...,
    "RotationOverrideId": ...,
}

parent.get_rotation_override(**kwargs)
```

1. See [:material-code-braces: GetRotationOverrideRequestRequestTypeDef](./type_defs.md#getrotationoverriderequestrequesttypedef) 

### list\_contact\_channels

Lists all contact channels for the specified contact.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_contact_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_contact_channels.html)

```python
# list_contact_channels method definition

await def list_contact_channels(
    self,
    *,
    ContactId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListContactChannelsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListContactChannelsResultTypeDef](./type_defs.md#listcontactchannelsresulttypedef) 


```python
# list_contact_channels method usage example with argument unpacking

kwargs: ListContactChannelsRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
}

parent.list_contact_channels(**kwargs)
```

1. See [:material-code-braces: ListContactChannelsRequestRequestTypeDef](./type_defs.md#listcontactchannelsrequestrequesttypedef) 

### list\_contacts

Lists all contacts and escalation plans in Incident Manager.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_contacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_contacts.html)

```python
# list_contacts method definition

await def list_contacts(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    AliasPrefix: str = ...,
    Type: ContactTypeType = ...,  # (1)
) -> ListContactsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContactTypeType](./literals.md#contacttypetype) 
2. See [:material-code-braces: ListContactsResultTypeDef](./type_defs.md#listcontactsresulttypedef) 


```python
# list_contacts method usage example with argument unpacking

kwargs: ListContactsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_contacts(**kwargs)
```

1. See [:material-code-braces: ListContactsRequestRequestTypeDef](./type_defs.md#listcontactsrequestrequesttypedef) 

### list\_engagements

Lists all engagements that have happened in an incident.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_engagements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_engagements.html)

```python
# list_engagements method definition

await def list_engagements(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    IncidentId: str = ...,
    TimeRangeValue: TimeRangeTypeDef = ...,  # (1)
) -> ListEngagementsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-braces: ListEngagementsResultTypeDef](./type_defs.md#listengagementsresulttypedef) 


```python
# list_engagements method usage example with argument unpacking

kwargs: ListEngagementsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_engagements(**kwargs)
```

1. See [:material-code-braces: ListEngagementsRequestRequestTypeDef](./type_defs.md#listengagementsrequestrequesttypedef) 

### list\_page\_receipts

Lists all of the engagements to contact channels that have been acknowledged.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_page_receipts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_page_receipts.html)

```python
# list_page_receipts method definition

await def list_page_receipts(
    self,
    *,
    PageId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPageReceiptsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPageReceiptsResultTypeDef](./type_defs.md#listpagereceiptsresulttypedef) 


```python
# list_page_receipts method usage example with argument unpacking

kwargs: ListPageReceiptsRequestRequestTypeDef = {  # (1)
    "PageId": ...,
}

parent.list_page_receipts(**kwargs)
```

1. See [:material-code-braces: ListPageReceiptsRequestRequestTypeDef](./type_defs.md#listpagereceiptsrequestrequesttypedef) 

### list\_page\_resolutions

Returns the resolution path of an engagement.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_page_resolutions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_page_resolutions.html)

```python
# list_page_resolutions method definition

await def list_page_resolutions(
    self,
    *,
    PageId: str,
    NextToken: str = ...,
) -> ListPageResolutionsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPageResolutionsResultTypeDef](./type_defs.md#listpageresolutionsresulttypedef) 


```python
# list_page_resolutions method usage example with argument unpacking

kwargs: ListPageResolutionsRequestRequestTypeDef = {  # (1)
    "PageId": ...,
}

parent.list_page_resolutions(**kwargs)
```

1. See [:material-code-braces: ListPageResolutionsRequestRequestTypeDef](./type_defs.md#listpageresolutionsrequestrequesttypedef) 

### list\_pages\_by\_contact

Lists the engagements to a contact's contact channels.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_pages_by_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_pages_by_contact.html)

```python
# list_pages_by_contact method definition

await def list_pages_by_contact(
    self,
    *,
    ContactId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPagesByContactResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPagesByContactResultTypeDef](./type_defs.md#listpagesbycontactresulttypedef) 


```python
# list_pages_by_contact method usage example with argument unpacking

kwargs: ListPagesByContactRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
}

parent.list_pages_by_contact(**kwargs)
```

1. See [:material-code-braces: ListPagesByContactRequestRequestTypeDef](./type_defs.md#listpagesbycontactrequestrequesttypedef) 

### list\_pages\_by\_engagement

Lists the engagements to contact channels that occurred by engaging a contact.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_pages_by_engagement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_pages_by_engagement.html)

```python
# list_pages_by_engagement method definition

await def list_pages_by_engagement(
    self,
    *,
    EngagementId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPagesByEngagementResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPagesByEngagementResultTypeDef](./type_defs.md#listpagesbyengagementresulttypedef) 


```python
# list_pages_by_engagement method usage example with argument unpacking

kwargs: ListPagesByEngagementRequestRequestTypeDef = {  # (1)
    "EngagementId": ...,
}

parent.list_pages_by_engagement(**kwargs)
```

1. See [:material-code-braces: ListPagesByEngagementRequestRequestTypeDef](./type_defs.md#listpagesbyengagementrequestrequesttypedef) 

### list\_preview\_rotation\_shifts

Returns a list of shifts based on rotation configuration parameters.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_preview_rotation_shifts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_preview_rotation_shifts.html)

```python
# list_preview_rotation_shifts method definition

await def list_preview_rotation_shifts(
    self,
    *,
    EndTime: TimestampTypeDef,
    Members: Sequence[str],
    TimeZoneId: str,
    Recurrence: RecurrenceSettingsTypeDef,  # (1)
    RotationStartTime: TimestampTypeDef = ...,
    StartTime: TimestampTypeDef = ...,
    Overrides: Sequence[PreviewOverrideTypeDef] = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPreviewRotationShiftsResultTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RecurrenceSettingsTypeDef](./type_defs.md#recurrencesettingstypedef) 
2. See [:material-code-braces: PreviewOverrideTypeDef](./type_defs.md#previewoverridetypedef) 
3. See [:material-code-braces: ListPreviewRotationShiftsResultTypeDef](./type_defs.md#listpreviewrotationshiftsresulttypedef) 


```python
# list_preview_rotation_shifts method usage example with argument unpacking

kwargs: ListPreviewRotationShiftsRequestRequestTypeDef = {  # (1)
    "EndTime": ...,
    "Members": ...,
    "TimeZoneId": ...,
    "Recurrence": ...,
}

parent.list_preview_rotation_shifts(**kwargs)
```

1. See [:material-code-braces: ListPreviewRotationShiftsRequestRequestTypeDef](./type_defs.md#listpreviewrotationshiftsrequestrequesttypedef) 

### list\_rotation\_overrides

Retrieves a list of overrides currently specified for an on-call rotation.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_rotation_overrides` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_rotation_overrides.html)

```python
# list_rotation_overrides method definition

await def list_rotation_overrides(
    self,
    *,
    RotationId: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRotationOverridesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRotationOverridesResultTypeDef](./type_defs.md#listrotationoverridesresulttypedef) 


```python
# list_rotation_overrides method usage example with argument unpacking

kwargs: ListRotationOverridesRequestRequestTypeDef = {  # (1)
    "RotationId": ...,
    "StartTime": ...,
    "EndTime": ...,
}

parent.list_rotation_overrides(**kwargs)
```

1. See [:material-code-braces: ListRotationOverridesRequestRequestTypeDef](./type_defs.md#listrotationoverridesrequestrequesttypedef) 

### list\_rotation\_shifts

Returns a list of shifts generated by an existing rotation in the system.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_rotation_shifts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_rotation_shifts.html)

```python
# list_rotation_shifts method definition

await def list_rotation_shifts(
    self,
    *,
    RotationId: str,
    EndTime: TimestampTypeDef,
    StartTime: TimestampTypeDef = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRotationShiftsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRotationShiftsResultTypeDef](./type_defs.md#listrotationshiftsresulttypedef) 


```python
# list_rotation_shifts method usage example with argument unpacking

kwargs: ListRotationShiftsRequestRequestTypeDef = {  # (1)
    "RotationId": ...,
    "EndTime": ...,
}

parent.list_rotation_shifts(**kwargs)
```

1. See [:material-code-braces: ListRotationShiftsRequestRequestTypeDef](./type_defs.md#listrotationshiftsrequestrequesttypedef) 

### list\_rotations

Retrieves a list of on-call rotations.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_rotations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_rotations.html)

```python
# list_rotations method definition

await def list_rotations(
    self,
    *,
    RotationNamePrefix: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRotationsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRotationsResultTypeDef](./type_defs.md#listrotationsresulttypedef) 


```python
# list_rotations method usage example with argument unpacking

kwargs: ListRotationsRequestRequestTypeDef = {  # (1)
    "RotationNamePrefix": ...,
}

parent.list_rotations(**kwargs)
```

1. See [:material-code-braces: ListRotationsRequestRequestTypeDef](./type_defs.md#listrotationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags of an escalation plan or contact.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### put\_contact\_policy

Adds a resource policy to the specified contact or escalation plan.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").put_contact_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/put_contact_policy.html)

```python
# put_contact_policy method definition

await def put_contact_policy(
    self,
    *,
    ContactArn: str,
    Policy: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_contact_policy method usage example with argument unpacking

kwargs: PutContactPolicyRequestRequestTypeDef = {  # (1)
    "ContactArn": ...,
    "Policy": ...,
}

parent.put_contact_policy(**kwargs)
```

1. See [:material-code-braces: PutContactPolicyRequestRequestTypeDef](./type_defs.md#putcontactpolicyrequestrequesttypedef) 

### send\_activation\_code

Sends an activation code to a contact channel.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").send_activation_code` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/send_activation_code.html)

```python
# send_activation_code method definition

await def send_activation_code(
    self,
    *,
    ContactChannelId: str,
) -> Dict[str, Any]:
    ...
```



```python
# send_activation_code method usage example with argument unpacking

kwargs: SendActivationCodeRequestRequestTypeDef = {  # (1)
    "ContactChannelId": ...,
}

parent.send_activation_code(**kwargs)
```

1. See [:material-code-braces: SendActivationCodeRequestRequestTypeDef](./type_defs.md#sendactivationcoderequestrequesttypedef) 

### start\_engagement

Starts an engagement to a contact or escalation plan.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").start_engagement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/start_engagement.html)

```python
# start_engagement method definition

await def start_engagement(
    self,
    *,
    ContactId: str,
    Sender: str,
    Subject: str,
    Content: str,
    PublicSubject: str = ...,
    PublicContent: str = ...,
    IncidentId: str = ...,
    IdempotencyToken: str = ...,
) -> StartEngagementResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartEngagementResultTypeDef](./type_defs.md#startengagementresulttypedef) 


```python
# start_engagement method usage example with argument unpacking

kwargs: StartEngagementRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
    "Sender": ...,
    "Subject": ...,
    "Content": ...,
}

parent.start_engagement(**kwargs)
```

1. See [:material-code-braces: StartEngagementRequestRequestTypeDef](./type_defs.md#startengagementrequestrequesttypedef) 

### stop\_engagement

Stops an engagement before it finishes the final stage of the escalation plan
or engagement plan.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").stop_engagement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/stop_engagement.html)

```python
# stop_engagement method definition

await def stop_engagement(
    self,
    *,
    EngagementId: str,
    Reason: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# stop_engagement method usage example with argument unpacking

kwargs: StopEngagementRequestRequestTypeDef = {  # (1)
    "EngagementId": ...,
}

parent.stop_engagement(**kwargs)
```

1. See [:material-code-braces: StopEngagementRequestRequestTypeDef](./type_defs.md#stopengagementrequestrequesttypedef) 

### tag\_resource

Tags a contact or escalation plan.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_contact

Updates the contact or escalation plan specified.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").update_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/update_contact.html)

```python
# update_contact method definition

await def update_contact(
    self,
    *,
    ContactId: str,
    DisplayName: str = ...,
    Plan: PlanTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: PlanTypeDef](./type_defs.md#plantypedef) 


```python
# update_contact method usage example with argument unpacking

kwargs: UpdateContactRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
}

parent.update_contact(**kwargs)
```

1. See [:material-code-braces: UpdateContactRequestRequestTypeDef](./type_defs.md#updatecontactrequestrequesttypedef) 

### update\_contact\_channel

Updates a contact's contact channel.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").update_contact_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/update_contact_channel.html)

```python
# update_contact_channel method definition

await def update_contact_channel(
    self,
    *,
    ContactChannelId: str,
    Name: str = ...,
    DeliveryAddress: ContactChannelAddressTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ContactChannelAddressTypeDef](./type_defs.md#contactchanneladdresstypedef) 


```python
# update_contact_channel method usage example with argument unpacking

kwargs: UpdateContactChannelRequestRequestTypeDef = {  # (1)
    "ContactChannelId": ...,
}

parent.update_contact_channel(**kwargs)
```

1. See [:material-code-braces: UpdateContactChannelRequestRequestTypeDef](./type_defs.md#updatecontactchannelrequestrequesttypedef) 

### update\_rotation

Updates the information specified for an on-call rotation.

Type annotations and code completion for `#!python session.create_client("ssm-contacts").update_rotation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts/client/update_rotation.html)

```python
# update_rotation method definition

await def update_rotation(
    self,
    *,
    RotationId: str,
    Recurrence: RecurrenceSettingsTypeDef,  # (1)
    ContactIds: Sequence[str] = ...,
    StartTime: TimestampTypeDef = ...,
    TimeZoneId: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: RecurrenceSettingsTypeDef](./type_defs.md#recurrencesettingstypedef) 


```python
# update_rotation method usage example with argument unpacking

kwargs: UpdateRotationRequestRequestTypeDef = {  # (1)
    "RotationId": ...,
    "Recurrence": ...,
}

parent.update_rotation(**kwargs)
```

1. See [:material-code-braces: UpdateRotationRequestRequestTypeDef](./type_defs.md#updaterotationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("ssm-contacts").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "SSMContactsClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("ssm-contacts").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("ssm-contacts").get_paginator` method with overloads.

- `client.get_paginator("list_contact_channels")` -> [ListContactChannelsPaginator](./paginators.md#listcontactchannelspaginator)
- `client.get_paginator("list_contacts")` -> [ListContactsPaginator](./paginators.md#listcontactspaginator)
- `client.get_paginator("list_engagements")` -> [ListEngagementsPaginator](./paginators.md#listengagementspaginator)
- `client.get_paginator("list_page_receipts")` -> [ListPageReceiptsPaginator](./paginators.md#listpagereceiptspaginator)
- `client.get_paginator("list_page_resolutions")` -> [ListPageResolutionsPaginator](./paginators.md#listpageresolutionspaginator)
- `client.get_paginator("list_pages_by_contact")` -> [ListPagesByContactPaginator](./paginators.md#listpagesbycontactpaginator)
- `client.get_paginator("list_pages_by_engagement")` -> [ListPagesByEngagementPaginator](./paginators.md#listpagesbyengagementpaginator)
- `client.get_paginator("list_preview_rotation_shifts")` -> [ListPreviewRotationShiftsPaginator](./paginators.md#listpreviewrotationshiftspaginator)
- `client.get_paginator("list_rotation_overrides")` -> [ListRotationOverridesPaginator](./paginators.md#listrotationoverridespaginator)
- `client.get_paginator("list_rotation_shifts")` -> [ListRotationShiftsPaginator](./paginators.md#listrotationshiftspaginator)
- `client.get_paginator("list_rotations")` -> [ListRotationsPaginator](./paginators.md#listrotationspaginator)



