# ChimeClient

> [Index](../README.md) > [Chime](./README.md) > ChimeClient

!!! note ""

    Auto-generated documentation for [Chime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#chime)
    type annotations stubs module [types-aiobotocore-chime](https://pypi.org/project/types-aiobotocore-chime/).

## ChimeClient

Type annotations and code completion for `#!python session.create_client("chime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client)

```python
# ChimeClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_chime.client import ChimeClient

session = get_session()
async with session.create_client("chime") as client:
    client: ChimeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("chime").exceptions` structure.

```python
# ChimeClient.exceptions usage example

async with session.create_client("chime") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.ForbiddenException,
        client.NotFoundException,
        client.ResourceLimitExceededException,
        client.ServiceFailureException,
        client.ServiceUnavailableException,
        client.ThrottledClientException,
        client.UnauthorizedClientException,
        client.UnprocessableEntityException,
    ) as e:
        print(e)
```

```python
# ChimeClient usage type checking example

from types_aiobotocore_chime.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("chime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("chime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/generate_presigned_url.html)

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


### associate\_phone\_number\_with\_user

Associates a phone number with the specified Amazon Chime user.

Type annotations and code completion for `#!python session.create_client("chime").associate_phone_number_with_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/associate_phone_number_with_user.html)

```python
# associate_phone_number_with_user method definition

await def associate_phone_number_with_user(
    self,
    *,
    AccountId: str,
    UserId: str,
    E164PhoneNumber: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_phone_number_with_user method usage example with argument unpacking

kwargs: AssociatePhoneNumberWithUserRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserId": ...,
    "E164PhoneNumber": ...,
}

parent.associate_phone_number_with_user(**kwargs)
```

1. See [:material-code-braces: AssociatePhoneNumberWithUserRequestTypeDef](./type_defs.md#associatephonenumberwithuserrequesttypedef) 

### associate\_phone\_numbers\_with\_voice\_connector

Associates phone numbers with the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").associate_phone_numbers_with_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/associate_phone_numbers_with_voice_connector.html)

```python
# associate_phone_numbers_with_voice_connector method definition

await def associate_phone_numbers_with_voice_connector(
    self,
    *,
    VoiceConnectorId: str,
    E164PhoneNumbers: Sequence[str],
    ForceAssociate: bool = ...,
) -> AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef](./type_defs.md#associatephonenumberswithvoiceconnectorresponsetypedef) 


```python
# associate_phone_numbers_with_voice_connector method usage example with argument unpacking

kwargs: AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "E164PhoneNumbers": ...,
}

parent.associate_phone_numbers_with_voice_connector(**kwargs)
```

1. See [:material-code-braces: AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef](./type_defs.md#associatephonenumberswithvoiceconnectorrequesttypedef) 

### associate\_phone\_numbers\_with\_voice\_connector\_group

Associates phone numbers with the specified Amazon Chime Voice Connector group.

Type annotations and code completion for `#!python session.create_client("chime").associate_phone_numbers_with_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/associate_phone_numbers_with_voice_connector_group.html)

```python
# associate_phone_numbers_with_voice_connector_group method definition

await def associate_phone_numbers_with_voice_connector_group(
    self,
    *,
    VoiceConnectorGroupId: str,
    E164PhoneNumbers: Sequence[str],
    ForceAssociate: bool = ...,
) -> AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociatePhoneNumbersWithVoiceConnectorGroupResponseTypeDef](./type_defs.md#associatephonenumberswithvoiceconnectorgroupresponsetypedef) 


```python
# associate_phone_numbers_with_voice_connector_group method usage example with argument unpacking

kwargs: AssociatePhoneNumbersWithVoiceConnectorGroupRequestTypeDef = {  # (1)
    "VoiceConnectorGroupId": ...,
    "E164PhoneNumbers": ...,
}

parent.associate_phone_numbers_with_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: AssociatePhoneNumbersWithVoiceConnectorGroupRequestTypeDef](./type_defs.md#associatephonenumberswithvoiceconnectorgrouprequesttypedef) 

### associate\_signin\_delegate\_groups\_with\_account

Associates the specified sign-in delegate groups with the specified Amazon
Chime account.

Type annotations and code completion for `#!python session.create_client("chime").associate_signin_delegate_groups_with_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/associate_signin_delegate_groups_with_account.html)

```python
# associate_signin_delegate_groups_with_account method definition

await def associate_signin_delegate_groups_with_account(
    self,
    *,
    AccountId: str,
    SigninDelegateGroups: Sequence[SigninDelegateGroupTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: SigninDelegateGroupTypeDef](./type_defs.md#signindelegategrouptypedef) 


```python
# associate_signin_delegate_groups_with_account method usage example with argument unpacking

kwargs: AssociateSigninDelegateGroupsWithAccountRequestTypeDef = {  # (1)
    "AccountId": ...,
    "SigninDelegateGroups": ...,
}

parent.associate_signin_delegate_groups_with_account(**kwargs)
```

1. See [:material-code-braces: AssociateSigninDelegateGroupsWithAccountRequestTypeDef](./type_defs.md#associatesignindelegategroupswithaccountrequesttypedef) 

### batch\_create\_attendee

Creates up to 100 new attendees for an active Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.create_client("chime").batch_create_attendee` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/batch_create_attendee.html)

```python
# batch_create_attendee method definition

await def batch_create_attendee(
    self,
    *,
    MeetingId: str,
    Attendees: Sequence[CreateAttendeeRequestItemTypeDef],  # (1)
) -> BatchCreateAttendeeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CreateAttendeeRequestItemTypeDef](./type_defs.md#createattendeerequestitemtypedef) 
2. See [:material-code-braces: BatchCreateAttendeeResponseTypeDef](./type_defs.md#batchcreateattendeeresponsetypedef) 


```python
# batch_create_attendee method usage example with argument unpacking

kwargs: BatchCreateAttendeeRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "Attendees": ...,
}

parent.batch_create_attendee(**kwargs)
```

1. See [:material-code-braces: BatchCreateAttendeeRequestTypeDef](./type_defs.md#batchcreateattendeerequesttypedef) 

### batch\_create\_channel\_membership

Adds a specified number of users to a channel.

Type annotations and code completion for `#!python session.create_client("chime").batch_create_channel_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/batch_create_channel_membership.html)

```python
# batch_create_channel_membership method definition

await def batch_create_channel_membership(
    self,
    *,
    ChannelArn: str,
    MemberArns: Sequence[str],
    Type: ChannelMembershipTypeType = ...,  # (1)
    ChimeBearer: str = ...,
) -> BatchCreateChannelMembershipResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
2. See [:material-code-braces: BatchCreateChannelMembershipResponseTypeDef](./type_defs.md#batchcreatechannelmembershipresponsetypedef) 


```python
# batch_create_channel_membership method usage example with argument unpacking

kwargs: BatchCreateChannelMembershipRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MemberArns": ...,
}

parent.batch_create_channel_membership(**kwargs)
```

1. See [:material-code-braces: BatchCreateChannelMembershipRequestTypeDef](./type_defs.md#batchcreatechannelmembershiprequesttypedef) 

### batch\_create\_room\_membership

Adds up to 50 members to a chat room in an Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").batch_create_room_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/batch_create_room_membership.html)

```python
# batch_create_room_membership method definition

await def batch_create_room_membership(
    self,
    *,
    AccountId: str,
    RoomId: str,
    MembershipItemList: Sequence[MembershipItemTypeDef],  # (1)
) -> BatchCreateRoomMembershipResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MembershipItemTypeDef](./type_defs.md#membershipitemtypedef) 
2. See [:material-code-braces: BatchCreateRoomMembershipResponseTypeDef](./type_defs.md#batchcreateroommembershipresponsetypedef) 


```python
# batch_create_room_membership method usage example with argument unpacking

kwargs: BatchCreateRoomMembershipRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RoomId": ...,
    "MembershipItemList": ...,
}

parent.batch_create_room_membership(**kwargs)
```

1. See [:material-code-braces: BatchCreateRoomMembershipRequestTypeDef](./type_defs.md#batchcreateroommembershiprequesttypedef) 

### batch\_delete\_phone\_number

Moves phone numbers into the <b>Deletion queue</b>.

Type annotations and code completion for `#!python session.create_client("chime").batch_delete_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/batch_delete_phone_number.html)

```python
# batch_delete_phone_number method definition

await def batch_delete_phone_number(
    self,
    *,
    PhoneNumberIds: Sequence[str],
) -> BatchDeletePhoneNumberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeletePhoneNumberResponseTypeDef](./type_defs.md#batchdeletephonenumberresponsetypedef) 


```python
# batch_delete_phone_number method usage example with argument unpacking

kwargs: BatchDeletePhoneNumberRequestTypeDef = {  # (1)
    "PhoneNumberIds": ...,
}

parent.batch_delete_phone_number(**kwargs)
```

1. See [:material-code-braces: BatchDeletePhoneNumberRequestTypeDef](./type_defs.md#batchdeletephonenumberrequesttypedef) 

### batch\_suspend\_user

Suspends up to 50 users from a <code>Team</code> or <code>EnterpriseLWA</code>
Amazon Chime account.

Type annotations and code completion for `#!python session.create_client("chime").batch_suspend_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/batch_suspend_user.html)

```python
# batch_suspend_user method definition

await def batch_suspend_user(
    self,
    *,
    AccountId: str,
    UserIdList: Sequence[str],
) -> BatchSuspendUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchSuspendUserResponseTypeDef](./type_defs.md#batchsuspenduserresponsetypedef) 


```python
# batch_suspend_user method usage example with argument unpacking

kwargs: BatchSuspendUserRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserIdList": ...,
}

parent.batch_suspend_user(**kwargs)
```

1. See [:material-code-braces: BatchSuspendUserRequestTypeDef](./type_defs.md#batchsuspenduserrequesttypedef) 

### batch\_unsuspend\_user

Removes the suspension from up to 50 previously suspended users for the
specified Amazon Chime <code>EnterpriseLWA</code> account.

Type annotations and code completion for `#!python session.create_client("chime").batch_unsuspend_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/batch_unsuspend_user.html)

```python
# batch_unsuspend_user method definition

await def batch_unsuspend_user(
    self,
    *,
    AccountId: str,
    UserIdList: Sequence[str],
) -> BatchUnsuspendUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchUnsuspendUserResponseTypeDef](./type_defs.md#batchunsuspenduserresponsetypedef) 


```python
# batch_unsuspend_user method usage example with argument unpacking

kwargs: BatchUnsuspendUserRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserIdList": ...,
}

parent.batch_unsuspend_user(**kwargs)
```

1. See [:material-code-braces: BatchUnsuspendUserRequestTypeDef](./type_defs.md#batchunsuspenduserrequesttypedef) 

### batch\_update\_phone\_number

Updates phone number product types or calling names.

Type annotations and code completion for `#!python session.create_client("chime").batch_update_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/batch_update_phone_number.html)

```python
# batch_update_phone_number method definition

await def batch_update_phone_number(
    self,
    *,
    UpdatePhoneNumberRequestItems: Sequence[UpdatePhoneNumberRequestItemTypeDef],  # (1)
) -> BatchUpdatePhoneNumberResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdatePhoneNumberRequestItemTypeDef](./type_defs.md#updatephonenumberrequestitemtypedef) 
2. See [:material-code-braces: BatchUpdatePhoneNumberResponseTypeDef](./type_defs.md#batchupdatephonenumberresponsetypedef) 


```python
# batch_update_phone_number method usage example with argument unpacking

kwargs: BatchUpdatePhoneNumberRequestTypeDef = {  # (1)
    "UpdatePhoneNumberRequestItems": ...,
}

parent.batch_update_phone_number(**kwargs)
```

1. See [:material-code-braces: BatchUpdatePhoneNumberRequestTypeDef](./type_defs.md#batchupdatephonenumberrequesttypedef) 

### batch\_update\_user

Updates user details within the <a>UpdateUserRequestItem</a> object for up to
20 users for the specified Amazon Chime account.

Type annotations and code completion for `#!python session.create_client("chime").batch_update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/batch_update_user.html)

```python
# batch_update_user method definition

await def batch_update_user(
    self,
    *,
    AccountId: str,
    UpdateUserRequestItems: Sequence[UpdateUserRequestItemTypeDef],  # (1)
) -> BatchUpdateUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateUserRequestItemTypeDef](./type_defs.md#updateuserrequestitemtypedef) 
2. See [:material-code-braces: BatchUpdateUserResponseTypeDef](./type_defs.md#batchupdateuserresponsetypedef) 


```python
# batch_update_user method usage example with argument unpacking

kwargs: BatchUpdateUserRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UpdateUserRequestItems": ...,
}

parent.batch_update_user(**kwargs)
```

1. See [:material-code-braces: BatchUpdateUserRequestTypeDef](./type_defs.md#batchupdateuserrequesttypedef) 

### create\_account

Creates an Amazon Chime account under the administrator's AWS account.

Type annotations and code completion for `#!python session.create_client("chime").create_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_account.html)

```python
# create_account method definition

await def create_account(
    self,
    *,
    Name: str,
) -> CreateAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAccountResponseTypeDef](./type_defs.md#createaccountresponsetypedef) 


```python
# create_account method usage example with argument unpacking

kwargs: CreateAccountRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_account(**kwargs)
```

1. See [:material-code-braces: CreateAccountRequestTypeDef](./type_defs.md#createaccountrequesttypedef) 

### create\_app\_instance

Creates an Amazon Chime SDK messaging <code>AppInstance</code> under an AWS
account.

Type annotations and code completion for `#!python session.create_client("chime").create_app_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_app_instance.html)

```python
# create_app_instance method definition

await def create_app_instance(
    self,
    *,
    Name: str,
    ClientRequestToken: str,
    Metadata: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateAppInstanceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateAppInstanceResponseTypeDef](./type_defs.md#createappinstanceresponsetypedef) 


```python
# create_app_instance method usage example with argument unpacking

kwargs: CreateAppInstanceRequestTypeDef = {  # (1)
    "Name": ...,
    "ClientRequestToken": ...,
}

parent.create_app_instance(**kwargs)
```

1. See [:material-code-braces: CreateAppInstanceRequestTypeDef](./type_defs.md#createappinstancerequesttypedef) 

### create\_app\_instance\_admin

Promotes an <code>AppInstanceUser</code> to an <code>AppInstanceAdmin</code>.

Type annotations and code completion for `#!python session.create_client("chime").create_app_instance_admin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_app_instance_admin.html)

```python
# create_app_instance_admin method definition

await def create_app_instance_admin(
    self,
    *,
    AppInstanceAdminArn: str,
    AppInstanceArn: str,
) -> CreateAppInstanceAdminResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAppInstanceAdminResponseTypeDef](./type_defs.md#createappinstanceadminresponsetypedef) 


```python
# create_app_instance_admin method usage example with argument unpacking

kwargs: CreateAppInstanceAdminRequestTypeDef = {  # (1)
    "AppInstanceAdminArn": ...,
    "AppInstanceArn": ...,
}

parent.create_app_instance_admin(**kwargs)
```

1. See [:material-code-braces: CreateAppInstanceAdminRequestTypeDef](./type_defs.md#createappinstanceadminrequesttypedef) 

### create\_app\_instance\_user

Creates a user under an Amazon Chime <code>AppInstance</code>.

Type annotations and code completion for `#!python session.create_client("chime").create_app_instance_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_app_instance_user.html)

```python
# create_app_instance_user method definition

await def create_app_instance_user(
    self,
    *,
    AppInstanceArn: str,
    AppInstanceUserId: str,
    Name: str,
    ClientRequestToken: str,
    Metadata: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateAppInstanceUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateAppInstanceUserResponseTypeDef](./type_defs.md#createappinstanceuserresponsetypedef) 


```python
# create_app_instance_user method usage example with argument unpacking

kwargs: CreateAppInstanceUserRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
    "AppInstanceUserId": ...,
    "Name": ...,
    "ClientRequestToken": ...,
}

parent.create_app_instance_user(**kwargs)
```

1. See [:material-code-braces: CreateAppInstanceUserRequestTypeDef](./type_defs.md#createappinstanceuserrequesttypedef) 

### create\_attendee

Creates a new attendee for an active Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.create_client("chime").create_attendee` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_attendee.html)

```python
# create_attendee method definition

await def create_attendee(
    self,
    *,
    MeetingId: str,
    ExternalUserId: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateAttendeeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateAttendeeResponseTypeDef](./type_defs.md#createattendeeresponsetypedef) 


```python
# create_attendee method usage example with argument unpacking

kwargs: CreateAttendeeRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "ExternalUserId": ...,
}

parent.create_attendee(**kwargs)
```

1. See [:material-code-braces: CreateAttendeeRequestTypeDef](./type_defs.md#createattendeerequesttypedef) 

### create\_bot

Creates a bot for an Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").create_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_bot.html)

```python
# create_bot method definition

await def create_bot(
    self,
    *,
    AccountId: str,
    DisplayName: str,
    Domain: str = ...,
) -> CreateBotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateBotResponseTypeDef](./type_defs.md#createbotresponsetypedef) 


```python
# create_bot method usage example with argument unpacking

kwargs: CreateBotRequestTypeDef = {  # (1)
    "AccountId": ...,
    "DisplayName": ...,
}

parent.create_bot(**kwargs)
```

1. See [:material-code-braces: CreateBotRequestTypeDef](./type_defs.md#createbotrequesttypedef) 

### create\_channel

Creates a channel to which you can add users and send messages.

Type annotations and code completion for `#!python session.create_client("chime").create_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_channel.html)

```python
# create_channel method definition

await def create_channel(
    self,
    *,
    AppInstanceArn: str,
    Name: str,
    ClientRequestToken: str,
    Mode: ChannelModeType = ...,  # (1)
    Privacy: ChannelPrivacyType = ...,  # (2)
    Metadata: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    ChimeBearer: str = ...,
) -> CreateChannelResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
2. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef) 


```python
# create_channel method usage example with argument unpacking

kwargs: CreateChannelRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
    "Name": ...,
    "ClientRequestToken": ...,
}

parent.create_channel(**kwargs)
```

1. See [:material-code-braces: CreateChannelRequestTypeDef](./type_defs.md#createchannelrequesttypedef) 

### create\_channel\_ban

Permanently bans a member from a channel.

Type annotations and code completion for `#!python session.create_client("chime").create_channel_ban` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_channel_ban.html)

```python
# create_channel_ban method definition

await def create_channel_ban(
    self,
    *,
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str = ...,
) -> CreateChannelBanResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateChannelBanResponseTypeDef](./type_defs.md#createchannelbanresponsetypedef) 


```python
# create_channel_ban method usage example with argument unpacking

kwargs: CreateChannelBanRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MemberArn": ...,
}

parent.create_channel_ban(**kwargs)
```

1. See [:material-code-braces: CreateChannelBanRequestTypeDef](./type_defs.md#createchannelbanrequesttypedef) 

### create\_channel\_membership

Adds a user to a channel.

Type annotations and code completion for `#!python session.create_client("chime").create_channel_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_channel_membership.html)

```python
# create_channel_membership method definition

await def create_channel_membership(
    self,
    *,
    ChannelArn: str,
    MemberArn: str,
    Type: ChannelMembershipTypeType,  # (1)
    ChimeBearer: str = ...,
) -> CreateChannelMembershipResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
2. See [:material-code-braces: CreateChannelMembershipResponseTypeDef](./type_defs.md#createchannelmembershipresponsetypedef) 


```python
# create_channel_membership method usage example with argument unpacking

kwargs: CreateChannelMembershipRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MemberArn": ...,
    "Type": ...,
}

parent.create_channel_membership(**kwargs)
```

1. See [:material-code-braces: CreateChannelMembershipRequestTypeDef](./type_defs.md#createchannelmembershiprequesttypedef) 

### create\_channel\_moderator

Creates a new <code>ChannelModerator</code>.

Type annotations and code completion for `#!python session.create_client("chime").create_channel_moderator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_channel_moderator.html)

```python
# create_channel_moderator method definition

await def create_channel_moderator(
    self,
    *,
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: str = ...,
) -> CreateChannelModeratorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateChannelModeratorResponseTypeDef](./type_defs.md#createchannelmoderatorresponsetypedef) 


```python
# create_channel_moderator method usage example with argument unpacking

kwargs: CreateChannelModeratorRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "ChannelModeratorArn": ...,
}

parent.create_channel_moderator(**kwargs)
```

1. See [:material-code-braces: CreateChannelModeratorRequestTypeDef](./type_defs.md#createchannelmoderatorrequesttypedef) 

### create\_media\_capture\_pipeline

Creates a media capture pipeline.

Type annotations and code completion for `#!python session.create_client("chime").create_media_capture_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_media_capture_pipeline.html)

```python
# create_media_capture_pipeline method definition

await def create_media_capture_pipeline(
    self,
    *,
    SourceType: MediaPipelineSourceTypeType,  # (1)
    SourceArn: str,
    SinkType: MediaPipelineSinkTypeType,  # (2)
    SinkArn: str,
    ClientRequestToken: str = ...,
    ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...,  # (3)
) -> CreateMediaCapturePipelineResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: MediaPipelineSourceTypeType](./literals.md#mediapipelinesourcetypetype) 
2. See [:material-code-brackets: MediaPipelineSinkTypeType](./literals.md#mediapipelinesinktypetype) 
3. See [:material-code-braces: ChimeSdkMeetingConfigurationTypeDef](./type_defs.md#chimesdkmeetingconfigurationtypedef) [:material-code-braces: ChimeSdkMeetingConfigurationOutputTypeDef](./type_defs.md#chimesdkmeetingconfigurationoutputtypedef) 
4. See [:material-code-braces: CreateMediaCapturePipelineResponseTypeDef](./type_defs.md#createmediacapturepipelineresponsetypedef) 


```python
# create_media_capture_pipeline method usage example with argument unpacking

kwargs: CreateMediaCapturePipelineRequestTypeDef = {  # (1)
    "SourceType": ...,
    "SourceArn": ...,
    "SinkType": ...,
    "SinkArn": ...,
}

parent.create_media_capture_pipeline(**kwargs)
```

1. See [:material-code-braces: CreateMediaCapturePipelineRequestTypeDef](./type_defs.md#createmediacapturepipelinerequesttypedef) 

### create\_meeting

Creates a new Amazon Chime SDK meeting in the specified media Region with no
initial attendees.

Type annotations and code completion for `#!python session.create_client("chime").create_meeting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_meeting.html)

```python
# create_meeting method definition

await def create_meeting(
    self,
    *,
    ClientRequestToken: str,
    ExternalMeetingId: str = ...,
    MeetingHostId: str = ...,
    MediaRegion: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    NotificationsConfiguration: MeetingNotificationConfigurationTypeDef = ...,  # (2)
) -> CreateMeetingResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: MeetingNotificationConfigurationTypeDef](./type_defs.md#meetingnotificationconfigurationtypedef) 
3. See [:material-code-braces: CreateMeetingResponseTypeDef](./type_defs.md#createmeetingresponsetypedef) 


```python
# create_meeting method usage example with argument unpacking

kwargs: CreateMeetingRequestTypeDef = {  # (1)
    "ClientRequestToken": ...,
}

parent.create_meeting(**kwargs)
```

1. See [:material-code-braces: CreateMeetingRequestTypeDef](./type_defs.md#createmeetingrequesttypedef) 

### create\_meeting\_dial\_out

Uses the join token and call metadata in a meeting request (From number, To
number, and so forth) to initiate an outbound call to a public switched
telephone network (PSTN) and join them into a Chime meeting.

Type annotations and code completion for `#!python session.create_client("chime").create_meeting_dial_out` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_meeting_dial_out.html)

```python
# create_meeting_dial_out method definition

await def create_meeting_dial_out(
    self,
    *,
    MeetingId: str,
    FromPhoneNumber: str,
    ToPhoneNumber: str,
    JoinToken: str,
) -> CreateMeetingDialOutResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateMeetingDialOutResponseTypeDef](./type_defs.md#createmeetingdialoutresponsetypedef) 


```python
# create_meeting_dial_out method usage example with argument unpacking

kwargs: CreateMeetingDialOutRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "FromPhoneNumber": ...,
    "ToPhoneNumber": ...,
    "JoinToken": ...,
}

parent.create_meeting_dial_out(**kwargs)
```

1. See [:material-code-braces: CreateMeetingDialOutRequestTypeDef](./type_defs.md#createmeetingdialoutrequesttypedef) 

### create\_meeting\_with\_attendees

Creates a new Amazon Chime SDK meeting in the specified media Region, with
attendees.

Type annotations and code completion for `#!python session.create_client("chime").create_meeting_with_attendees` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_meeting_with_attendees.html)

```python
# create_meeting_with_attendees method definition

await def create_meeting_with_attendees(
    self,
    *,
    ClientRequestToken: str,
    ExternalMeetingId: str = ...,
    MeetingHostId: str = ...,
    MediaRegion: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    NotificationsConfiguration: MeetingNotificationConfigurationTypeDef = ...,  # (2)
    Attendees: Sequence[CreateAttendeeRequestItemTypeDef] = ...,  # (3)
) -> CreateMeetingWithAttendeesResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: MeetingNotificationConfigurationTypeDef](./type_defs.md#meetingnotificationconfigurationtypedef) 
3. See [:material-code-braces: CreateAttendeeRequestItemTypeDef](./type_defs.md#createattendeerequestitemtypedef) 
4. See [:material-code-braces: CreateMeetingWithAttendeesResponseTypeDef](./type_defs.md#createmeetingwithattendeesresponsetypedef) 


```python
# create_meeting_with_attendees method usage example with argument unpacking

kwargs: CreateMeetingWithAttendeesRequestTypeDef = {  # (1)
    "ClientRequestToken": ...,
}

parent.create_meeting_with_attendees(**kwargs)
```

1. See [:material-code-braces: CreateMeetingWithAttendeesRequestTypeDef](./type_defs.md#createmeetingwithattendeesrequesttypedef) 

### create\_phone\_number\_order

Creates an order for phone numbers to be provisioned.

Type annotations and code completion for `#!python session.create_client("chime").create_phone_number_order` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_phone_number_order.html)

```python
# create_phone_number_order method definition

await def create_phone_number_order(
    self,
    *,
    ProductType: PhoneNumberProductTypeType,  # (1)
    E164PhoneNumbers: Sequence[str],
) -> CreatePhoneNumberOrderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
2. See [:material-code-braces: CreatePhoneNumberOrderResponseTypeDef](./type_defs.md#createphonenumberorderresponsetypedef) 


```python
# create_phone_number_order method usage example with argument unpacking

kwargs: CreatePhoneNumberOrderRequestTypeDef = {  # (1)
    "ProductType": ...,
    "E164PhoneNumbers": ...,
}

parent.create_phone_number_order(**kwargs)
```

1. See [:material-code-braces: CreatePhoneNumberOrderRequestTypeDef](./type_defs.md#createphonenumberorderrequesttypedef) 

### create\_proxy\_session

Creates a proxy session on the specified Amazon Chime Voice Connector for the
specified participant phone numbers.

Type annotations and code completion for `#!python session.create_client("chime").create_proxy_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_proxy_session.html)

```python
# create_proxy_session method definition

await def create_proxy_session(
    self,
    *,
    VoiceConnectorId: str,
    ParticipantPhoneNumbers: Sequence[str],
    Capabilities: Sequence[CapabilityType],  # (1)
    Name: str = ...,
    ExpiryMinutes: int = ...,
    NumberSelectionBehavior: NumberSelectionBehaviorType = ...,  # (2)
    GeoMatchLevel: GeoMatchLevelType = ...,  # (3)
    GeoMatchParams: GeoMatchParamsTypeDef = ...,  # (4)
) -> CreateProxySessionResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: CapabilityType](./literals.md#capabilitytype) 
2. See [:material-code-brackets: NumberSelectionBehaviorType](./literals.md#numberselectionbehaviortype) 
3. See [:material-code-brackets: GeoMatchLevelType](./literals.md#geomatchleveltype) 
4. See [:material-code-braces: GeoMatchParamsTypeDef](./type_defs.md#geomatchparamstypedef) 
5. See [:material-code-braces: CreateProxySessionResponseTypeDef](./type_defs.md#createproxysessionresponsetypedef) 


```python
# create_proxy_session method usage example with argument unpacking

kwargs: CreateProxySessionRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "ParticipantPhoneNumbers": ...,
    "Capabilities": ...,
}

parent.create_proxy_session(**kwargs)
```

1. See [:material-code-braces: CreateProxySessionRequestTypeDef](./type_defs.md#createproxysessionrequesttypedef) 

### create\_room

Creates a chat room for the specified Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").create_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_room.html)

```python
# create_room method definition

await def create_room(
    self,
    *,
    AccountId: str,
    Name: str,
    ClientRequestToken: str = ...,
) -> CreateRoomResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateRoomResponseTypeDef](./type_defs.md#createroomresponsetypedef) 


```python
# create_room method usage example with argument unpacking

kwargs: CreateRoomRequestTypeDef = {  # (1)
    "AccountId": ...,
    "Name": ...,
}

parent.create_room(**kwargs)
```

1. See [:material-code-braces: CreateRoomRequestTypeDef](./type_defs.md#createroomrequesttypedef) 

### create\_room\_membership

Adds a member to a chat room in an Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").create_room_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_room_membership.html)

```python
# create_room_membership method definition

await def create_room_membership(
    self,
    *,
    AccountId: str,
    RoomId: str,
    MemberId: str,
    Role: RoomMembershipRoleType = ...,  # (1)
) -> CreateRoomMembershipResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoomMembershipRoleType](./literals.md#roommembershiproletype) 
2. See [:material-code-braces: CreateRoomMembershipResponseTypeDef](./type_defs.md#createroommembershipresponsetypedef) 


```python
# create_room_membership method usage example with argument unpacking

kwargs: CreateRoomMembershipRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RoomId": ...,
    "MemberId": ...,
}

parent.create_room_membership(**kwargs)
```

1. See [:material-code-braces: CreateRoomMembershipRequestTypeDef](./type_defs.md#createroommembershiprequesttypedef) 

### create\_sip\_media\_application

Creates a SIP media application.

Type annotations and code completion for `#!python session.create_client("chime").create_sip_media_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_sip_media_application.html)

```python
# create_sip_media_application method definition

await def create_sip_media_application(
    self,
    *,
    AwsRegion: str,
    Name: str,
    Endpoints: Sequence[SipMediaApplicationEndpointTypeDef],  # (1)
) -> CreateSipMediaApplicationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SipMediaApplicationEndpointTypeDef](./type_defs.md#sipmediaapplicationendpointtypedef) 
2. See [:material-code-braces: CreateSipMediaApplicationResponseTypeDef](./type_defs.md#createsipmediaapplicationresponsetypedef) 


```python
# create_sip_media_application method usage example with argument unpacking

kwargs: CreateSipMediaApplicationRequestTypeDef = {  # (1)
    "AwsRegion": ...,
    "Name": ...,
    "Endpoints": ...,
}

parent.create_sip_media_application(**kwargs)
```

1. See [:material-code-braces: CreateSipMediaApplicationRequestTypeDef](./type_defs.md#createsipmediaapplicationrequesttypedef) 

### create\_sip\_media\_application\_call

Creates an outbound call to a phone number from the phone number specified in
the request, and it invokes the endpoint of the specified
<code>sipMediaApplicationId</code>.

Type annotations and code completion for `#!python session.create_client("chime").create_sip_media_application_call` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_sip_media_application_call.html)

```python
# create_sip_media_application_call method definition

await def create_sip_media_application_call(
    self,
    *,
    FromPhoneNumber: str,
    ToPhoneNumber: str,
    SipMediaApplicationId: str,
    SipHeaders: Mapping[str, str] = ...,
) -> CreateSipMediaApplicationCallResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSipMediaApplicationCallResponseTypeDef](./type_defs.md#createsipmediaapplicationcallresponsetypedef) 


```python
# create_sip_media_application_call method usage example with argument unpacking

kwargs: CreateSipMediaApplicationCallRequestTypeDef = {  # (1)
    "FromPhoneNumber": ...,
    "ToPhoneNumber": ...,
    "SipMediaApplicationId": ...,
}

parent.create_sip_media_application_call(**kwargs)
```

1. See [:material-code-braces: CreateSipMediaApplicationCallRequestTypeDef](./type_defs.md#createsipmediaapplicationcallrequesttypedef) 

### create\_sip\_rule

Creates a SIP rule which can be used to run a SIP media application as a target
for a specific trigger type.

Type annotations and code completion for `#!python session.create_client("chime").create_sip_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_sip_rule.html)

```python
# create_sip_rule method definition

await def create_sip_rule(
    self,
    *,
    Name: str,
    TriggerType: SipRuleTriggerTypeType,  # (1)
    TriggerValue: str,
    TargetApplications: Sequence[SipRuleTargetApplicationTypeDef],  # (2)
    Disabled: bool = ...,
) -> CreateSipRuleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SipRuleTriggerTypeType](./literals.md#sipruletriggertypetype) 
2. See [:material-code-braces: SipRuleTargetApplicationTypeDef](./type_defs.md#sipruletargetapplicationtypedef) 
3. See [:material-code-braces: CreateSipRuleResponseTypeDef](./type_defs.md#createsipruleresponsetypedef) 


```python
# create_sip_rule method usage example with argument unpacking

kwargs: CreateSipRuleRequestTypeDef = {  # (1)
    "Name": ...,
    "TriggerType": ...,
    "TriggerValue": ...,
    "TargetApplications": ...,
}

parent.create_sip_rule(**kwargs)
```

1. See [:material-code-braces: CreateSipRuleRequestTypeDef](./type_defs.md#createsiprulerequesttypedef) 

### create\_user

Creates a user under the specified Amazon Chime account.

Type annotations and code completion for `#!python session.create_client("chime").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_user.html)

```python
# create_user method definition

await def create_user(
    self,
    *,
    AccountId: str,
    Username: str = ...,
    Email: str = ...,
    UserType: UserTypeType = ...,  # (1)
) -> CreateUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestTypeDef](./type_defs.md#createuserrequesttypedef) 

### create\_voice\_connector

Creates an Amazon Chime Voice Connector under the administrator's AWS account.

Type annotations and code completion for `#!python session.create_client("chime").create_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_voice_connector.html)

```python
# create_voice_connector method definition

await def create_voice_connector(
    self,
    *,
    Name: str,
    RequireEncryption: bool,
    AwsRegion: VoiceConnectorAwsRegionType = ...,  # (1)
) -> CreateVoiceConnectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: VoiceConnectorAwsRegionType](./literals.md#voiceconnectorawsregiontype) 
2. See [:material-code-braces: CreateVoiceConnectorResponseTypeDef](./type_defs.md#createvoiceconnectorresponsetypedef) 


```python
# create_voice_connector method usage example with argument unpacking

kwargs: CreateVoiceConnectorRequestTypeDef = {  # (1)
    "Name": ...,
    "RequireEncryption": ...,
}

parent.create_voice_connector(**kwargs)
```

1. See [:material-code-braces: CreateVoiceConnectorRequestTypeDef](./type_defs.md#createvoiceconnectorrequesttypedef) 

### create\_voice\_connector\_group

Creates an Amazon Chime Voice Connector group under the administrator's AWS
account.

Type annotations and code completion for `#!python session.create_client("chime").create_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/create_voice_connector_group.html)

```python
# create_voice_connector_group method definition

await def create_voice_connector_group(
    self,
    *,
    Name: str,
    VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef] = ...,  # (1)
) -> CreateVoiceConnectorGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VoiceConnectorItemTypeDef](./type_defs.md#voiceconnectoritemtypedef) 
2. See [:material-code-braces: CreateVoiceConnectorGroupResponseTypeDef](./type_defs.md#createvoiceconnectorgroupresponsetypedef) 


```python
# create_voice_connector_group method usage example with argument unpacking

kwargs: CreateVoiceConnectorGroupRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: CreateVoiceConnectorGroupRequestTypeDef](./type_defs.md#createvoiceconnectorgrouprequesttypedef) 

### delete\_account

Deletes the specified Amazon Chime account.

Type annotations and code completion for `#!python session.create_client("chime").delete_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_account.html)

```python
# delete_account method definition

await def delete_account(
    self,
    *,
    AccountId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_account method usage example with argument unpacking

kwargs: DeleteAccountRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.delete_account(**kwargs)
```

1. See [:material-code-braces: DeleteAccountRequestTypeDef](./type_defs.md#deleteaccountrequesttypedef) 

### delete\_app\_instance

Deletes an <code>AppInstance</code> and all associated data asynchronously.

Type annotations and code completion for `#!python session.create_client("chime").delete_app_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_app_instance.html)

```python
# delete_app_instance method definition

await def delete_app_instance(
    self,
    *,
    AppInstanceArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_app_instance method usage example with argument unpacking

kwargs: DeleteAppInstanceRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
}

parent.delete_app_instance(**kwargs)
```

1. See [:material-code-braces: DeleteAppInstanceRequestTypeDef](./type_defs.md#deleteappinstancerequesttypedef) 

### delete\_app\_instance\_admin

Demotes an <code>AppInstanceAdmin</code> to an <code>AppInstanceUser</code>.

Type annotations and code completion for `#!python session.create_client("chime").delete_app_instance_admin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_app_instance_admin.html)

```python
# delete_app_instance_admin method definition

await def delete_app_instance_admin(
    self,
    *,
    AppInstanceAdminArn: str,
    AppInstanceArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_app_instance_admin method usage example with argument unpacking

kwargs: DeleteAppInstanceAdminRequestTypeDef = {  # (1)
    "AppInstanceAdminArn": ...,
    "AppInstanceArn": ...,
}

parent.delete_app_instance_admin(**kwargs)
```

1. See [:material-code-braces: DeleteAppInstanceAdminRequestTypeDef](./type_defs.md#deleteappinstanceadminrequesttypedef) 

### delete\_app\_instance\_streaming\_configurations

Deletes the streaming configurations of an <code>AppInstance</code>.

Type annotations and code completion for `#!python session.create_client("chime").delete_app_instance_streaming_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_app_instance_streaming_configurations.html)

```python
# delete_app_instance_streaming_configurations method definition

await def delete_app_instance_streaming_configurations(
    self,
    *,
    AppInstanceArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_app_instance_streaming_configurations method usage example with argument unpacking

kwargs: DeleteAppInstanceStreamingConfigurationsRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
}

parent.delete_app_instance_streaming_configurations(**kwargs)
```

1. See [:material-code-braces: DeleteAppInstanceStreamingConfigurationsRequestTypeDef](./type_defs.md#deleteappinstancestreamingconfigurationsrequesttypedef) 

### delete\_app\_instance\_user

Deletes an <code>AppInstanceUser</code>.

Type annotations and code completion for `#!python session.create_client("chime").delete_app_instance_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_app_instance_user.html)

```python
# delete_app_instance_user method definition

await def delete_app_instance_user(
    self,
    *,
    AppInstanceUserArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_app_instance_user method usage example with argument unpacking

kwargs: DeleteAppInstanceUserRequestTypeDef = {  # (1)
    "AppInstanceUserArn": ...,
}

parent.delete_app_instance_user(**kwargs)
```

1. See [:material-code-braces: DeleteAppInstanceUserRequestTypeDef](./type_defs.md#deleteappinstanceuserrequesttypedef) 

### delete\_attendee

Deletes an attendee from the specified Amazon Chime SDK meeting and deletes
their <code>JoinToken</code>.

Type annotations and code completion for `#!python session.create_client("chime").delete_attendee` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_attendee.html)

```python
# delete_attendee method definition

await def delete_attendee(
    self,
    *,
    MeetingId: str,
    AttendeeId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_attendee method usage example with argument unpacking

kwargs: DeleteAttendeeRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "AttendeeId": ...,
}

parent.delete_attendee(**kwargs)
```

1. See [:material-code-braces: DeleteAttendeeRequestTypeDef](./type_defs.md#deleteattendeerequesttypedef) 

### delete\_channel

Immediately makes a channel and its memberships inaccessible and marks them for
deletion.

Type annotations and code completion for `#!python session.create_client("chime").delete_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_channel.html)

```python
# delete_channel method definition

await def delete_channel(
    self,
    *,
    ChannelArn: str,
    ChimeBearer: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_channel method usage example with argument unpacking

kwargs: DeleteChannelRequestTypeDef = {  # (1)
    "ChannelArn": ...,
}

parent.delete_channel(**kwargs)
```

1. See [:material-code-braces: DeleteChannelRequestTypeDef](./type_defs.md#deletechannelrequesttypedef) 

### delete\_channel\_ban

Removes a user from a channel's ban list.

Type annotations and code completion for `#!python session.create_client("chime").delete_channel_ban` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_channel_ban.html)

```python
# delete_channel_ban method definition

await def delete_channel_ban(
    self,
    *,
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_channel_ban method usage example with argument unpacking

kwargs: DeleteChannelBanRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MemberArn": ...,
}

parent.delete_channel_ban(**kwargs)
```

1. See [:material-code-braces: DeleteChannelBanRequestTypeDef](./type_defs.md#deletechannelbanrequesttypedef) 

### delete\_channel\_membership

Removes a member from a channel.

Type annotations and code completion for `#!python session.create_client("chime").delete_channel_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_channel_membership.html)

```python
# delete_channel_membership method definition

await def delete_channel_membership(
    self,
    *,
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_channel_membership method usage example with argument unpacking

kwargs: DeleteChannelMembershipRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MemberArn": ...,
}

parent.delete_channel_membership(**kwargs)
```

1. See [:material-code-braces: DeleteChannelMembershipRequestTypeDef](./type_defs.md#deletechannelmembershiprequesttypedef) 

### delete\_channel\_message

Deletes a channel message.

Type annotations and code completion for `#!python session.create_client("chime").delete_channel_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_channel_message.html)

```python
# delete_channel_message method definition

await def delete_channel_message(
    self,
    *,
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_channel_message method usage example with argument unpacking

kwargs: DeleteChannelMessageRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MessageId": ...,
}

parent.delete_channel_message(**kwargs)
```

1. See [:material-code-braces: DeleteChannelMessageRequestTypeDef](./type_defs.md#deletechannelmessagerequesttypedef) 

### delete\_channel\_moderator

Deletes a channel moderator.

Type annotations and code completion for `#!python session.create_client("chime").delete_channel_moderator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_channel_moderator.html)

```python
# delete_channel_moderator method definition

await def delete_channel_moderator(
    self,
    *,
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_channel_moderator method usage example with argument unpacking

kwargs: DeleteChannelModeratorRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "ChannelModeratorArn": ...,
}

parent.delete_channel_moderator(**kwargs)
```

1. See [:material-code-braces: DeleteChannelModeratorRequestTypeDef](./type_defs.md#deletechannelmoderatorrequesttypedef) 

### delete\_events\_configuration

Deletes the events configuration that allows a bot to receive outgoing events.

Type annotations and code completion for `#!python session.create_client("chime").delete_events_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_events_configuration.html)

```python
# delete_events_configuration method definition

await def delete_events_configuration(
    self,
    *,
    AccountId: str,
    BotId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_events_configuration method usage example with argument unpacking

kwargs: DeleteEventsConfigurationRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BotId": ...,
}

parent.delete_events_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteEventsConfigurationRequestTypeDef](./type_defs.md#deleteeventsconfigurationrequesttypedef) 

### delete\_media\_capture\_pipeline

Deletes the media capture pipeline.

Type annotations and code completion for `#!python session.create_client("chime").delete_media_capture_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_media_capture_pipeline.html)

```python
# delete_media_capture_pipeline method definition

await def delete_media_capture_pipeline(
    self,
    *,
    MediaPipelineId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_media_capture_pipeline method usage example with argument unpacking

kwargs: DeleteMediaCapturePipelineRequestTypeDef = {  # (1)
    "MediaPipelineId": ...,
}

parent.delete_media_capture_pipeline(**kwargs)
```

1. See [:material-code-braces: DeleteMediaCapturePipelineRequestTypeDef](./type_defs.md#deletemediacapturepipelinerequesttypedef) 

### delete\_meeting

Deletes the specified Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.create_client("chime").delete_meeting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_meeting.html)

```python
# delete_meeting method definition

await def delete_meeting(
    self,
    *,
    MeetingId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_meeting method usage example with argument unpacking

kwargs: DeleteMeetingRequestTypeDef = {  # (1)
    "MeetingId": ...,
}

parent.delete_meeting(**kwargs)
```

1. See [:material-code-braces: DeleteMeetingRequestTypeDef](./type_defs.md#deletemeetingrequesttypedef) 

### delete\_phone\_number

Moves the specified phone number into the <b>Deletion queue</b>.

Type annotations and code completion for `#!python session.create_client("chime").delete_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_phone_number.html)

```python
# delete_phone_number method definition

await def delete_phone_number(
    self,
    *,
    PhoneNumberId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_phone_number method usage example with argument unpacking

kwargs: DeletePhoneNumberRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.delete_phone_number(**kwargs)
```

1. See [:material-code-braces: DeletePhoneNumberRequestTypeDef](./type_defs.md#deletephonenumberrequesttypedef) 

### delete\_proxy\_session

Deletes the specified proxy session from the specified Amazon Chime Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime").delete_proxy_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_proxy_session.html)

```python
# delete_proxy_session method definition

await def delete_proxy_session(
    self,
    *,
    VoiceConnectorId: str,
    ProxySessionId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_proxy_session method usage example with argument unpacking

kwargs: DeleteProxySessionRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "ProxySessionId": ...,
}

parent.delete_proxy_session(**kwargs)
```

1. See [:material-code-braces: DeleteProxySessionRequestTypeDef](./type_defs.md#deleteproxysessionrequesttypedef) 

### delete\_room

Deletes a chat room in an Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").delete_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_room.html)

```python
# delete_room method definition

await def delete_room(
    self,
    *,
    AccountId: str,
    RoomId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_room method usage example with argument unpacking

kwargs: DeleteRoomRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RoomId": ...,
}

parent.delete_room(**kwargs)
```

1. See [:material-code-braces: DeleteRoomRequestTypeDef](./type_defs.md#deleteroomrequesttypedef) 

### delete\_room\_membership

Removes a member from a chat room in an Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").delete_room_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_room_membership.html)

```python
# delete_room_membership method definition

await def delete_room_membership(
    self,
    *,
    AccountId: str,
    RoomId: str,
    MemberId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_room_membership method usage example with argument unpacking

kwargs: DeleteRoomMembershipRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RoomId": ...,
    "MemberId": ...,
}

parent.delete_room_membership(**kwargs)
```

1. See [:material-code-braces: DeleteRoomMembershipRequestTypeDef](./type_defs.md#deleteroommembershiprequesttypedef) 

### delete\_sip\_media\_application

Deletes a SIP media application.

Type annotations and code completion for `#!python session.create_client("chime").delete_sip_media_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_sip_media_application.html)

```python
# delete_sip_media_application method definition

await def delete_sip_media_application(
    self,
    *,
    SipMediaApplicationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_sip_media_application method usage example with argument unpacking

kwargs: DeleteSipMediaApplicationRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.delete_sip_media_application(**kwargs)
```

1. See [:material-code-braces: DeleteSipMediaApplicationRequestTypeDef](./type_defs.md#deletesipmediaapplicationrequesttypedef) 

### delete\_sip\_rule

Deletes a SIP rule.

Type annotations and code completion for `#!python session.create_client("chime").delete_sip_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_sip_rule.html)

```python
# delete_sip_rule method definition

await def delete_sip_rule(
    self,
    *,
    SipRuleId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_sip_rule method usage example with argument unpacking

kwargs: DeleteSipRuleRequestTypeDef = {  # (1)
    "SipRuleId": ...,
}

parent.delete_sip_rule(**kwargs)
```

1. See [:material-code-braces: DeleteSipRuleRequestTypeDef](./type_defs.md#deletesiprulerequesttypedef) 

### delete\_voice\_connector

Deletes the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").delete_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_voice_connector.html)

```python
# delete_voice_connector method definition

await def delete_voice_connector(
    self,
    *,
    VoiceConnectorId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_voice_connector method usage example with argument unpacking

kwargs: DeleteVoiceConnectorRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorRequestTypeDef](./type_defs.md#deletevoiceconnectorrequesttypedef) 

### delete\_voice\_connector\_emergency\_calling\_configuration

Deletes the emergency calling configuration details from the specified Amazon
Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").delete_voice_connector_emergency_calling_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_voice_connector_emergency_calling_configuration.html)

```python
# delete_voice_connector_emergency_calling_configuration method definition

await def delete_voice_connector_emergency_calling_configuration(
    self,
    *,
    VoiceConnectorId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_voice_connector_emergency_calling_configuration method usage example with argument unpacking

kwargs: DeleteVoiceConnectorEmergencyCallingConfigurationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector_emergency_calling_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorEmergencyCallingConfigurationRequestTypeDef](./type_defs.md#deletevoiceconnectoremergencycallingconfigurationrequesttypedef) 

### delete\_voice\_connector\_group

Deletes the specified Amazon Chime Voice Connector group.

Type annotations and code completion for `#!python session.create_client("chime").delete_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_voice_connector_group.html)

```python
# delete_voice_connector_group method definition

await def delete_voice_connector_group(
    self,
    *,
    VoiceConnectorGroupId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_voice_connector_group method usage example with argument unpacking

kwargs: DeleteVoiceConnectorGroupRequestTypeDef = {  # (1)
    "VoiceConnectorGroupId": ...,
}

parent.delete_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorGroupRequestTypeDef](./type_defs.md#deletevoiceconnectorgrouprequesttypedef) 

### delete\_voice\_connector\_origination

Deletes the origination settings for the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").delete_voice_connector_origination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_voice_connector_origination.html)

```python
# delete_voice_connector_origination method definition

await def delete_voice_connector_origination(
    self,
    *,
    VoiceConnectorId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_voice_connector_origination method usage example with argument unpacking

kwargs: DeleteVoiceConnectorOriginationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector_origination(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorOriginationRequestTypeDef](./type_defs.md#deletevoiceconnectororiginationrequesttypedef) 

### delete\_voice\_connector\_proxy

Deletes the proxy configuration from the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").delete_voice_connector_proxy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_voice_connector_proxy.html)

```python
# delete_voice_connector_proxy method definition

await def delete_voice_connector_proxy(
    self,
    *,
    VoiceConnectorId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_voice_connector_proxy method usage example with argument unpacking

kwargs: DeleteVoiceConnectorProxyRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector_proxy(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorProxyRequestTypeDef](./type_defs.md#deletevoiceconnectorproxyrequesttypedef) 

### delete\_voice\_connector\_streaming\_configuration

Deletes the streaming configuration for the specified Amazon Chime Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime").delete_voice_connector_streaming_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_voice_connector_streaming_configuration.html)

```python
# delete_voice_connector_streaming_configuration method definition

await def delete_voice_connector_streaming_configuration(
    self,
    *,
    VoiceConnectorId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_voice_connector_streaming_configuration method usage example with argument unpacking

kwargs: DeleteVoiceConnectorStreamingConfigurationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector_streaming_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorStreamingConfigurationRequestTypeDef](./type_defs.md#deletevoiceconnectorstreamingconfigurationrequesttypedef) 

### delete\_voice\_connector\_termination

Deletes the termination settings for the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").delete_voice_connector_termination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_voice_connector_termination.html)

```python
# delete_voice_connector_termination method definition

await def delete_voice_connector_termination(
    self,
    *,
    VoiceConnectorId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_voice_connector_termination method usage example with argument unpacking

kwargs: DeleteVoiceConnectorTerminationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector_termination(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorTerminationRequestTypeDef](./type_defs.md#deletevoiceconnectorterminationrequesttypedef) 

### delete\_voice\_connector\_termination\_credentials

Deletes the specified SIP credentials used by your equipment to authenticate
during call termination.

Type annotations and code completion for `#!python session.create_client("chime").delete_voice_connector_termination_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/delete_voice_connector_termination_credentials.html)

```python
# delete_voice_connector_termination_credentials method definition

await def delete_voice_connector_termination_credentials(
    self,
    *,
    VoiceConnectorId: str,
    Usernames: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_voice_connector_termination_credentials method usage example with argument unpacking

kwargs: DeleteVoiceConnectorTerminationCredentialsRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "Usernames": ...,
}

parent.delete_voice_connector_termination_credentials(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorTerminationCredentialsRequestTypeDef](./type_defs.md#deletevoiceconnectorterminationcredentialsrequesttypedef) 

### describe\_app\_instance

Returns the full details of an <code>AppInstance</code>.

Type annotations and code completion for `#!python session.create_client("chime").describe_app_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/describe_app_instance.html)

```python
# describe_app_instance method definition

await def describe_app_instance(
    self,
    *,
    AppInstanceArn: str,
) -> DescribeAppInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppInstanceResponseTypeDef](./type_defs.md#describeappinstanceresponsetypedef) 


```python
# describe_app_instance method usage example with argument unpacking

kwargs: DescribeAppInstanceRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
}

parent.describe_app_instance(**kwargs)
```

1. See [:material-code-braces: DescribeAppInstanceRequestTypeDef](./type_defs.md#describeappinstancerequesttypedef) 

### describe\_app\_instance\_admin

Returns the full details of an <code>AppInstanceAdmin</code>.

Type annotations and code completion for `#!python session.create_client("chime").describe_app_instance_admin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/describe_app_instance_admin.html)

```python
# describe_app_instance_admin method definition

await def describe_app_instance_admin(
    self,
    *,
    AppInstanceAdminArn: str,
    AppInstanceArn: str,
) -> DescribeAppInstanceAdminResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppInstanceAdminResponseTypeDef](./type_defs.md#describeappinstanceadminresponsetypedef) 


```python
# describe_app_instance_admin method usage example with argument unpacking

kwargs: DescribeAppInstanceAdminRequestTypeDef = {  # (1)
    "AppInstanceAdminArn": ...,
    "AppInstanceArn": ...,
}

parent.describe_app_instance_admin(**kwargs)
```

1. See [:material-code-braces: DescribeAppInstanceAdminRequestTypeDef](./type_defs.md#describeappinstanceadminrequesttypedef) 

### describe\_app\_instance\_user

Returns the full details of an <code>AppInstanceUser</code>.

Type annotations and code completion for `#!python session.create_client("chime").describe_app_instance_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/describe_app_instance_user.html)

```python
# describe_app_instance_user method definition

await def describe_app_instance_user(
    self,
    *,
    AppInstanceUserArn: str,
) -> DescribeAppInstanceUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppInstanceUserResponseTypeDef](./type_defs.md#describeappinstanceuserresponsetypedef) 


```python
# describe_app_instance_user method usage example with argument unpacking

kwargs: DescribeAppInstanceUserRequestTypeDef = {  # (1)
    "AppInstanceUserArn": ...,
}

parent.describe_app_instance_user(**kwargs)
```

1. See [:material-code-braces: DescribeAppInstanceUserRequestTypeDef](./type_defs.md#describeappinstanceuserrequesttypedef) 

### describe\_channel

Returns the full details of a channel in an Amazon Chime
<code>AppInstance</code>.

Type annotations and code completion for `#!python session.create_client("chime").describe_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/describe_channel.html)

```python
# describe_channel method definition

await def describe_channel(
    self,
    *,
    ChannelArn: str,
    ChimeBearer: str = ...,
) -> DescribeChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelResponseTypeDef](./type_defs.md#describechannelresponsetypedef) 


```python
# describe_channel method usage example with argument unpacking

kwargs: DescribeChannelRequestTypeDef = {  # (1)
    "ChannelArn": ...,
}

parent.describe_channel(**kwargs)
```

1. See [:material-code-braces: DescribeChannelRequestTypeDef](./type_defs.md#describechannelrequesttypedef) 

### describe\_channel\_ban

Returns the full details of a channel ban.

Type annotations and code completion for `#!python session.create_client("chime").describe_channel_ban` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/describe_channel_ban.html)

```python
# describe_channel_ban method definition

await def describe_channel_ban(
    self,
    *,
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str = ...,
) -> DescribeChannelBanResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelBanResponseTypeDef](./type_defs.md#describechannelbanresponsetypedef) 


```python
# describe_channel_ban method usage example with argument unpacking

kwargs: DescribeChannelBanRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MemberArn": ...,
}

parent.describe_channel_ban(**kwargs)
```

1. See [:material-code-braces: DescribeChannelBanRequestTypeDef](./type_defs.md#describechannelbanrequesttypedef) 

### describe\_channel\_membership

Returns the full details of a user's channel membership.

Type annotations and code completion for `#!python session.create_client("chime").describe_channel_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/describe_channel_membership.html)

```python
# describe_channel_membership method definition

await def describe_channel_membership(
    self,
    *,
    ChannelArn: str,
    MemberArn: str,
    ChimeBearer: str = ...,
) -> DescribeChannelMembershipResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelMembershipResponseTypeDef](./type_defs.md#describechannelmembershipresponsetypedef) 


```python
# describe_channel_membership method usage example with argument unpacking

kwargs: DescribeChannelMembershipRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MemberArn": ...,
}

parent.describe_channel_membership(**kwargs)
```

1. See [:material-code-braces: DescribeChannelMembershipRequestTypeDef](./type_defs.md#describechannelmembershiprequesttypedef) 

### describe\_channel\_membership\_for\_app\_instance\_user

Returns the details of a channel based on the membership of the specified
<code>AppInstanceUser</code>.

Type annotations and code completion for `#!python session.create_client("chime").describe_channel_membership_for_app_instance_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/describe_channel_membership_for_app_instance_user.html)

```python
# describe_channel_membership_for_app_instance_user method definition

await def describe_channel_membership_for_app_instance_user(
    self,
    *,
    ChannelArn: str,
    AppInstanceUserArn: str,
    ChimeBearer: str = ...,
) -> DescribeChannelMembershipForAppInstanceUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelMembershipForAppInstanceUserResponseTypeDef](./type_defs.md#describechannelmembershipforappinstanceuserresponsetypedef) 


```python
# describe_channel_membership_for_app_instance_user method usage example with argument unpacking

kwargs: DescribeChannelMembershipForAppInstanceUserRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "AppInstanceUserArn": ...,
}

parent.describe_channel_membership_for_app_instance_user(**kwargs)
```

1. See [:material-code-braces: DescribeChannelMembershipForAppInstanceUserRequestTypeDef](./type_defs.md#describechannelmembershipforappinstanceuserrequesttypedef) 

### describe\_channel\_moderated\_by\_app\_instance\_user

Returns the full details of a channel moderated by the specified
<code>AppInstanceUser</code>.

Type annotations and code completion for `#!python session.create_client("chime").describe_channel_moderated_by_app_instance_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/describe_channel_moderated_by_app_instance_user.html)

```python
# describe_channel_moderated_by_app_instance_user method definition

await def describe_channel_moderated_by_app_instance_user(
    self,
    *,
    ChannelArn: str,
    AppInstanceUserArn: str,
    ChimeBearer: str = ...,
) -> DescribeChannelModeratedByAppInstanceUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelModeratedByAppInstanceUserResponseTypeDef](./type_defs.md#describechannelmoderatedbyappinstanceuserresponsetypedef) 


```python
# describe_channel_moderated_by_app_instance_user method usage example with argument unpacking

kwargs: DescribeChannelModeratedByAppInstanceUserRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "AppInstanceUserArn": ...,
}

parent.describe_channel_moderated_by_app_instance_user(**kwargs)
```

1. See [:material-code-braces: DescribeChannelModeratedByAppInstanceUserRequestTypeDef](./type_defs.md#describechannelmoderatedbyappinstanceuserrequesttypedef) 

### describe\_channel\_moderator

Returns the full details of a single ChannelModerator.

Type annotations and code completion for `#!python session.create_client("chime").describe_channel_moderator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/describe_channel_moderator.html)

```python
# describe_channel_moderator method definition

await def describe_channel_moderator(
    self,
    *,
    ChannelArn: str,
    ChannelModeratorArn: str,
    ChimeBearer: str = ...,
) -> DescribeChannelModeratorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelModeratorResponseTypeDef](./type_defs.md#describechannelmoderatorresponsetypedef) 


```python
# describe_channel_moderator method usage example with argument unpacking

kwargs: DescribeChannelModeratorRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "ChannelModeratorArn": ...,
}

parent.describe_channel_moderator(**kwargs)
```

1. See [:material-code-braces: DescribeChannelModeratorRequestTypeDef](./type_defs.md#describechannelmoderatorrequesttypedef) 

### disassociate\_phone\_number\_from\_user

Disassociates the primary provisioned phone number from the specified Amazon
Chime user.

Type annotations and code completion for `#!python session.create_client("chime").disassociate_phone_number_from_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/disassociate_phone_number_from_user.html)

```python
# disassociate_phone_number_from_user method definition

await def disassociate_phone_number_from_user(
    self,
    *,
    AccountId: str,
    UserId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_phone_number_from_user method usage example with argument unpacking

kwargs: DisassociatePhoneNumberFromUserRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserId": ...,
}

parent.disassociate_phone_number_from_user(**kwargs)
```

1. See [:material-code-braces: DisassociatePhoneNumberFromUserRequestTypeDef](./type_defs.md#disassociatephonenumberfromuserrequesttypedef) 

### disassociate\_phone\_numbers\_from\_voice\_connector

Disassociates the specified phone numbers from the specified Amazon Chime Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime").disassociate_phone_numbers_from_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/disassociate_phone_numbers_from_voice_connector.html)

```python
# disassociate_phone_numbers_from_voice_connector method definition

await def disassociate_phone_numbers_from_voice_connector(
    self,
    *,
    VoiceConnectorId: str,
    E164PhoneNumbers: Sequence[str],
) -> DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef](./type_defs.md#disassociatephonenumbersfromvoiceconnectorresponsetypedef) 


```python
# disassociate_phone_numbers_from_voice_connector method usage example with argument unpacking

kwargs: DisassociatePhoneNumbersFromVoiceConnectorRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "E164PhoneNumbers": ...,
}

parent.disassociate_phone_numbers_from_voice_connector(**kwargs)
```

1. See [:material-code-braces: DisassociatePhoneNumbersFromVoiceConnectorRequestTypeDef](./type_defs.md#disassociatephonenumbersfromvoiceconnectorrequesttypedef) 

### disassociate\_phone\_numbers\_from\_voice\_connector\_group

Disassociates the specified phone numbers from the specified Amazon Chime Voice
Connector group.

Type annotations and code completion for `#!python session.create_client("chime").disassociate_phone_numbers_from_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/disassociate_phone_numbers_from_voice_connector_group.html)

```python
# disassociate_phone_numbers_from_voice_connector_group method definition

await def disassociate_phone_numbers_from_voice_connector_group(
    self,
    *,
    VoiceConnectorGroupId: str,
    E164PhoneNumbers: Sequence[str],
) -> DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef](./type_defs.md#disassociatephonenumbersfromvoiceconnectorgroupresponsetypedef) 


```python
# disassociate_phone_numbers_from_voice_connector_group method usage example with argument unpacking

kwargs: DisassociatePhoneNumbersFromVoiceConnectorGroupRequestTypeDef = {  # (1)
    "VoiceConnectorGroupId": ...,
    "E164PhoneNumbers": ...,
}

parent.disassociate_phone_numbers_from_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: DisassociatePhoneNumbersFromVoiceConnectorGroupRequestTypeDef](./type_defs.md#disassociatephonenumbersfromvoiceconnectorgrouprequesttypedef) 

### disassociate\_signin\_delegate\_groups\_from\_account

Disassociates the specified sign-in delegate groups from the specified Amazon
Chime account.

Type annotations and code completion for `#!python session.create_client("chime").disassociate_signin_delegate_groups_from_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/disassociate_signin_delegate_groups_from_account.html)

```python
# disassociate_signin_delegate_groups_from_account method definition

await def disassociate_signin_delegate_groups_from_account(
    self,
    *,
    AccountId: str,
    GroupNames: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_signin_delegate_groups_from_account method usage example with argument unpacking

kwargs: DisassociateSigninDelegateGroupsFromAccountRequestTypeDef = {  # (1)
    "AccountId": ...,
    "GroupNames": ...,
}

parent.disassociate_signin_delegate_groups_from_account(**kwargs)
```

1. See [:material-code-braces: DisassociateSigninDelegateGroupsFromAccountRequestTypeDef](./type_defs.md#disassociatesignindelegategroupsfromaccountrequesttypedef) 

### get\_account

Retrieves details for the specified Amazon Chime account, such as account type
and supported licenses.

Type annotations and code completion for `#!python session.create_client("chime").get_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_account.html)

```python
# get_account method definition

await def get_account(
    self,
    *,
    AccountId: str,
) -> GetAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountResponseTypeDef](./type_defs.md#getaccountresponsetypedef) 


```python
# get_account method usage example with argument unpacking

kwargs: GetAccountRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.get_account(**kwargs)
```

1. See [:material-code-braces: GetAccountRequestTypeDef](./type_defs.md#getaccountrequesttypedef) 

### get\_account\_settings

Retrieves account settings for the specified Amazon Chime account ID, such as
remote control and dialout settings.

Type annotations and code completion for `#!python session.create_client("chime").get_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_account_settings.html)

```python
# get_account_settings method definition

await def get_account_settings(
    self,
    *,
    AccountId: str,
) -> GetAccountSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountSettingsResponseTypeDef](./type_defs.md#getaccountsettingsresponsetypedef) 


```python
# get_account_settings method usage example with argument unpacking

kwargs: GetAccountSettingsRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.get_account_settings(**kwargs)
```

1. See [:material-code-braces: GetAccountSettingsRequestTypeDef](./type_defs.md#getaccountsettingsrequesttypedef) 

### get\_app\_instance\_retention\_settings

Gets the retention settings for an <code>AppInstance</code>.

Type annotations and code completion for `#!python session.create_client("chime").get_app_instance_retention_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_app_instance_retention_settings.html)

```python
# get_app_instance_retention_settings method definition

await def get_app_instance_retention_settings(
    self,
    *,
    AppInstanceArn: str,
) -> GetAppInstanceRetentionSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAppInstanceRetentionSettingsResponseTypeDef](./type_defs.md#getappinstanceretentionsettingsresponsetypedef) 


```python
# get_app_instance_retention_settings method usage example with argument unpacking

kwargs: GetAppInstanceRetentionSettingsRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
}

parent.get_app_instance_retention_settings(**kwargs)
```

1. See [:material-code-braces: GetAppInstanceRetentionSettingsRequestTypeDef](./type_defs.md#getappinstanceretentionsettingsrequesttypedef) 

### get\_app\_instance\_streaming\_configurations

Gets the streaming settings for an <code>AppInstance</code>.

Type annotations and code completion for `#!python session.create_client("chime").get_app_instance_streaming_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_app_instance_streaming_configurations.html)

```python
# get_app_instance_streaming_configurations method definition

await def get_app_instance_streaming_configurations(
    self,
    *,
    AppInstanceArn: str,
) -> GetAppInstanceStreamingConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAppInstanceStreamingConfigurationsResponseTypeDef](./type_defs.md#getappinstancestreamingconfigurationsresponsetypedef) 


```python
# get_app_instance_streaming_configurations method usage example with argument unpacking

kwargs: GetAppInstanceStreamingConfigurationsRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
}

parent.get_app_instance_streaming_configurations(**kwargs)
```

1. See [:material-code-braces: GetAppInstanceStreamingConfigurationsRequestTypeDef](./type_defs.md#getappinstancestreamingconfigurationsrequesttypedef) 

### get\_attendee

Gets the Amazon Chime SDK attendee details for a specified meeting ID and
attendee ID.

Type annotations and code completion for `#!python session.create_client("chime").get_attendee` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_attendee.html)

```python
# get_attendee method definition

await def get_attendee(
    self,
    *,
    MeetingId: str,
    AttendeeId: str,
) -> GetAttendeeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAttendeeResponseTypeDef](./type_defs.md#getattendeeresponsetypedef) 


```python
# get_attendee method usage example with argument unpacking

kwargs: GetAttendeeRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "AttendeeId": ...,
}

parent.get_attendee(**kwargs)
```

1. See [:material-code-braces: GetAttendeeRequestTypeDef](./type_defs.md#getattendeerequesttypedef) 

### get\_bot

Retrieves details for the specified bot, such as bot email address, bot type,
status, and display name.

Type annotations and code completion for `#!python session.create_client("chime").get_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_bot.html)

```python
# get_bot method definition

await def get_bot(
    self,
    *,
    AccountId: str,
    BotId: str,
) -> GetBotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBotResponseTypeDef](./type_defs.md#getbotresponsetypedef) 


```python
# get_bot method usage example with argument unpacking

kwargs: GetBotRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BotId": ...,
}

parent.get_bot(**kwargs)
```

1. See [:material-code-braces: GetBotRequestTypeDef](./type_defs.md#getbotrequesttypedef) 

### get\_channel\_message

Gets the full details of a channel message.

Type annotations and code completion for `#!python session.create_client("chime").get_channel_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_channel_message.html)

```python
# get_channel_message method definition

await def get_channel_message(
    self,
    *,
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: str = ...,
) -> GetChannelMessageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChannelMessageResponseTypeDef](./type_defs.md#getchannelmessageresponsetypedef) 


```python
# get_channel_message method usage example with argument unpacking

kwargs: GetChannelMessageRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MessageId": ...,
}

parent.get_channel_message(**kwargs)
```

1. See [:material-code-braces: GetChannelMessageRequestTypeDef](./type_defs.md#getchannelmessagerequesttypedef) 

### get\_events\_configuration

Gets details for an events configuration that allows a bot to receive outgoing
events, such as an HTTPS endpoint or Lambda function ARN.

Type annotations and code completion for `#!python session.create_client("chime").get_events_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_events_configuration.html)

```python
# get_events_configuration method definition

await def get_events_configuration(
    self,
    *,
    AccountId: str,
    BotId: str,
) -> GetEventsConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventsConfigurationResponseTypeDef](./type_defs.md#geteventsconfigurationresponsetypedef) 


```python
# get_events_configuration method usage example with argument unpacking

kwargs: GetEventsConfigurationRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BotId": ...,
}

parent.get_events_configuration(**kwargs)
```

1. See [:material-code-braces: GetEventsConfigurationRequestTypeDef](./type_defs.md#geteventsconfigurationrequesttypedef) 

### get\_global\_settings

Retrieves global settings for the administrator's AWS account, such as Amazon
Chime Business Calling and Amazon Chime Voice Connector settings.

Type annotations and code completion for `#!python session.create_client("chime").get_global_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_global_settings.html)

```python
# get_global_settings method definition

await def get_global_settings(
    self,
) -> GetGlobalSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGlobalSettingsResponseTypeDef](./type_defs.md#getglobalsettingsresponsetypedef) 

### get\_media\_capture\_pipeline

Gets an existing media capture pipeline.

Type annotations and code completion for `#!python session.create_client("chime").get_media_capture_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_media_capture_pipeline.html)

```python
# get_media_capture_pipeline method definition

await def get_media_capture_pipeline(
    self,
    *,
    MediaPipelineId: str,
) -> GetMediaCapturePipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMediaCapturePipelineResponseTypeDef](./type_defs.md#getmediacapturepipelineresponsetypedef) 


```python
# get_media_capture_pipeline method usage example with argument unpacking

kwargs: GetMediaCapturePipelineRequestTypeDef = {  # (1)
    "MediaPipelineId": ...,
}

parent.get_media_capture_pipeline(**kwargs)
```

1. See [:material-code-braces: GetMediaCapturePipelineRequestTypeDef](./type_defs.md#getmediacapturepipelinerequesttypedef) 

### get\_meeting

<b>This API is is no longer supported and will not be updated.</b> We recommend
using the latest version, <a
href="https://docs.aws.amazon.com/chime-sdk/latest/APIReference/API_meeting-chime_GetMeeting.html">GetMeeting</a>,
in the Amazon Chime SDK.

Type annotations and code completion for `#!python session.create_client("chime").get_meeting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_meeting.html)

```python
# get_meeting method definition

await def get_meeting(
    self,
    *,
    MeetingId: str,
) -> GetMeetingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMeetingResponseTypeDef](./type_defs.md#getmeetingresponsetypedef) 


```python
# get_meeting method usage example with argument unpacking

kwargs: GetMeetingRequestTypeDef = {  # (1)
    "MeetingId": ...,
}

parent.get_meeting(**kwargs)
```

1. See [:material-code-braces: GetMeetingRequestTypeDef](./type_defs.md#getmeetingrequesttypedef) 

### get\_messaging\_session\_endpoint

The details of the endpoint for the messaging session.

Type annotations and code completion for `#!python session.create_client("chime").get_messaging_session_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_messaging_session_endpoint.html)

```python
# get_messaging_session_endpoint method definition

await def get_messaging_session_endpoint(
    self,
) -> GetMessagingSessionEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMessagingSessionEndpointResponseTypeDef](./type_defs.md#getmessagingsessionendpointresponsetypedef) 

### get\_phone\_number

Retrieves details for the specified phone number ID, such as associations,
capabilities, and product type.

Type annotations and code completion for `#!python session.create_client("chime").get_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_phone_number.html)

```python
# get_phone_number method definition

await def get_phone_number(
    self,
    *,
    PhoneNumberId: str,
) -> GetPhoneNumberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPhoneNumberResponseTypeDef](./type_defs.md#getphonenumberresponsetypedef) 


```python
# get_phone_number method usage example with argument unpacking

kwargs: GetPhoneNumberRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.get_phone_number(**kwargs)
```

1. See [:material-code-braces: GetPhoneNumberRequestTypeDef](./type_defs.md#getphonenumberrequesttypedef) 

### get\_phone\_number\_order

Retrieves details for the specified phone number order, such as the order
creation timestamp, phone numbers in E.164 format, product type, and order
status.

Type annotations and code completion for `#!python session.create_client("chime").get_phone_number_order` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_phone_number_order.html)

```python
# get_phone_number_order method definition

await def get_phone_number_order(
    self,
    *,
    PhoneNumberOrderId: str,
) -> GetPhoneNumberOrderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPhoneNumberOrderResponseTypeDef](./type_defs.md#getphonenumberorderresponsetypedef) 


```python
# get_phone_number_order method usage example with argument unpacking

kwargs: GetPhoneNumberOrderRequestTypeDef = {  # (1)
    "PhoneNumberOrderId": ...,
}

parent.get_phone_number_order(**kwargs)
```

1. See [:material-code-braces: GetPhoneNumberOrderRequestTypeDef](./type_defs.md#getphonenumberorderrequesttypedef) 

### get\_phone\_number\_settings

Retrieves the phone number settings for the administrator's AWS account, such
as the default outbound calling name.

Type annotations and code completion for `#!python session.create_client("chime").get_phone_number_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_phone_number_settings.html)

```python
# get_phone_number_settings method definition

await def get_phone_number_settings(
    self,
) -> GetPhoneNumberSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPhoneNumberSettingsResponseTypeDef](./type_defs.md#getphonenumbersettingsresponsetypedef) 

### get\_proxy\_session

Gets the specified proxy session details for the specified Amazon Chime Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime").get_proxy_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_proxy_session.html)

```python
# get_proxy_session method definition

await def get_proxy_session(
    self,
    *,
    VoiceConnectorId: str,
    ProxySessionId: str,
) -> GetProxySessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProxySessionResponseTypeDef](./type_defs.md#getproxysessionresponsetypedef) 


```python
# get_proxy_session method usage example with argument unpacking

kwargs: GetProxySessionRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "ProxySessionId": ...,
}

parent.get_proxy_session(**kwargs)
```

1. See [:material-code-braces: GetProxySessionRequestTypeDef](./type_defs.md#getproxysessionrequesttypedef) 

### get\_retention\_settings

Gets the retention settings for the specified Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").get_retention_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_retention_settings.html)

```python
# get_retention_settings method definition

await def get_retention_settings(
    self,
    *,
    AccountId: str,
) -> GetRetentionSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRetentionSettingsResponseTypeDef](./type_defs.md#getretentionsettingsresponsetypedef) 


```python
# get_retention_settings method usage example with argument unpacking

kwargs: GetRetentionSettingsRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.get_retention_settings(**kwargs)
```

1. See [:material-code-braces: GetRetentionSettingsRequestTypeDef](./type_defs.md#getretentionsettingsrequesttypedef) 

### get\_room

Retrieves room details, such as the room name, for a room in an Amazon Chime
Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").get_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_room.html)

```python
# get_room method definition

await def get_room(
    self,
    *,
    AccountId: str,
    RoomId: str,
) -> GetRoomResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRoomResponseTypeDef](./type_defs.md#getroomresponsetypedef) 


```python
# get_room method usage example with argument unpacking

kwargs: GetRoomRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RoomId": ...,
}

parent.get_room(**kwargs)
```

1. See [:material-code-braces: GetRoomRequestTypeDef](./type_defs.md#getroomrequesttypedef) 

### get\_sip\_media\_application

Retrieves the information for a SIP media application, including name, AWS
Region, and endpoints.

Type annotations and code completion for `#!python session.create_client("chime").get_sip_media_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_sip_media_application.html)

```python
# get_sip_media_application method definition

await def get_sip_media_application(
    self,
    *,
    SipMediaApplicationId: str,
) -> GetSipMediaApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSipMediaApplicationResponseTypeDef](./type_defs.md#getsipmediaapplicationresponsetypedef) 


```python
# get_sip_media_application method usage example with argument unpacking

kwargs: GetSipMediaApplicationRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.get_sip_media_application(**kwargs)
```

1. See [:material-code-braces: GetSipMediaApplicationRequestTypeDef](./type_defs.md#getsipmediaapplicationrequesttypedef) 

### get\_sip\_media\_application\_logging\_configuration

Returns the logging configuration for the specified SIP media application.

Type annotations and code completion for `#!python session.create_client("chime").get_sip_media_application_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_sip_media_application_logging_configuration.html)

```python
# get_sip_media_application_logging_configuration method definition

await def get_sip_media_application_logging_configuration(
    self,
    *,
    SipMediaApplicationId: str,
) -> GetSipMediaApplicationLoggingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSipMediaApplicationLoggingConfigurationResponseTypeDef](./type_defs.md#getsipmediaapplicationloggingconfigurationresponsetypedef) 


```python
# get_sip_media_application_logging_configuration method usage example with argument unpacking

kwargs: GetSipMediaApplicationLoggingConfigurationRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.get_sip_media_application_logging_configuration(**kwargs)
```

1. See [:material-code-braces: GetSipMediaApplicationLoggingConfigurationRequestTypeDef](./type_defs.md#getsipmediaapplicationloggingconfigurationrequesttypedef) 

### get\_sip\_rule

Retrieves the details of a SIP rule, such as the rule ID, name, triggers, and
target endpoints.

Type annotations and code completion for `#!python session.create_client("chime").get_sip_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_sip_rule.html)

```python
# get_sip_rule method definition

await def get_sip_rule(
    self,
    *,
    SipRuleId: str,
) -> GetSipRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSipRuleResponseTypeDef](./type_defs.md#getsipruleresponsetypedef) 


```python
# get_sip_rule method usage example with argument unpacking

kwargs: GetSipRuleRequestTypeDef = {  # (1)
    "SipRuleId": ...,
}

parent.get_sip_rule(**kwargs)
```

1. See [:material-code-braces: GetSipRuleRequestTypeDef](./type_defs.md#getsiprulerequesttypedef) 

### get\_user

Retrieves details for the specified user ID, such as primary email address,
license type,and personal meeting PIN.

Type annotations and code completion for `#!python session.create_client("chime").get_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_user.html)

```python
# get_user method definition

await def get_user(
    self,
    *,
    AccountId: str,
    UserId: str,
) -> GetUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef) 


```python
# get_user method usage example with argument unpacking

kwargs: GetUserRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserId": ...,
}

parent.get_user(**kwargs)
```

1. See [:material-code-braces: GetUserRequestTypeDef](./type_defs.md#getuserrequesttypedef) 

### get\_user\_settings

Retrieves settings for the specified user ID, such as any associated phone
number settings.

Type annotations and code completion for `#!python session.create_client("chime").get_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_user_settings.html)

```python
# get_user_settings method definition

await def get_user_settings(
    self,
    *,
    AccountId: str,
    UserId: str,
) -> GetUserSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserSettingsResponseTypeDef](./type_defs.md#getusersettingsresponsetypedef) 


```python
# get_user_settings method usage example with argument unpacking

kwargs: GetUserSettingsRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserId": ...,
}

parent.get_user_settings(**kwargs)
```

1. See [:material-code-braces: GetUserSettingsRequestTypeDef](./type_defs.md#getusersettingsrequesttypedef) 

### get\_voice\_connector

Retrieves details for the specified Amazon Chime Voice Connector, such as
timestamps,name, outbound host, and encryption requirements.

Type annotations and code completion for `#!python session.create_client("chime").get_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_voice_connector.html)

```python
# get_voice_connector method definition

await def get_voice_connector(
    self,
    *,
    VoiceConnectorId: str,
) -> GetVoiceConnectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceConnectorResponseTypeDef](./type_defs.md#getvoiceconnectorresponsetypedef) 


```python
# get_voice_connector method usage example with argument unpacking

kwargs: GetVoiceConnectorRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorRequestTypeDef](./type_defs.md#getvoiceconnectorrequesttypedef) 

### get\_voice\_connector\_emergency\_calling\_configuration

Gets the emergency calling configuration details for the specified Amazon Chime
Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").get_voice_connector_emergency_calling_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_voice_connector_emergency_calling_configuration.html)

```python
# get_voice_connector_emergency_calling_configuration method definition

await def get_voice_connector_emergency_calling_configuration(
    self,
    *,
    VoiceConnectorId: str,
) -> GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef](./type_defs.md#getvoiceconnectoremergencycallingconfigurationresponsetypedef) 


```python
# get_voice_connector_emergency_calling_configuration method usage example with argument unpacking

kwargs: GetVoiceConnectorEmergencyCallingConfigurationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_emergency_calling_configuration(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorEmergencyCallingConfigurationRequestTypeDef](./type_defs.md#getvoiceconnectoremergencycallingconfigurationrequesttypedef) 

### get\_voice\_connector\_group

Retrieves details for the specified Amazon Chime Voice Connector group, such as
timestamps,name, and associated <code>VoiceConnectorItems</code>.

Type annotations and code completion for `#!python session.create_client("chime").get_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_voice_connector_group.html)

```python
# get_voice_connector_group method definition

await def get_voice_connector_group(
    self,
    *,
    VoiceConnectorGroupId: str,
) -> GetVoiceConnectorGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceConnectorGroupResponseTypeDef](./type_defs.md#getvoiceconnectorgroupresponsetypedef) 


```python
# get_voice_connector_group method usage example with argument unpacking

kwargs: GetVoiceConnectorGroupRequestTypeDef = {  # (1)
    "VoiceConnectorGroupId": ...,
}

parent.get_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorGroupRequestTypeDef](./type_defs.md#getvoiceconnectorgrouprequesttypedef) 

### get\_voice\_connector\_logging\_configuration

Retrieves the logging configuration details for the specified Amazon Chime
Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").get_voice_connector_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_voice_connector_logging_configuration.html)

```python
# get_voice_connector_logging_configuration method definition

await def get_voice_connector_logging_configuration(
    self,
    *,
    VoiceConnectorId: str,
) -> GetVoiceConnectorLoggingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceConnectorLoggingConfigurationResponseTypeDef](./type_defs.md#getvoiceconnectorloggingconfigurationresponsetypedef) 


```python
# get_voice_connector_logging_configuration method usage example with argument unpacking

kwargs: GetVoiceConnectorLoggingConfigurationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_logging_configuration(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorLoggingConfigurationRequestTypeDef](./type_defs.md#getvoiceconnectorloggingconfigurationrequesttypedef) 

### get\_voice\_connector\_origination

Retrieves origination setting details for the specified Amazon Chime Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime").get_voice_connector_origination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_voice_connector_origination.html)

```python
# get_voice_connector_origination method definition

await def get_voice_connector_origination(
    self,
    *,
    VoiceConnectorId: str,
) -> GetVoiceConnectorOriginationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceConnectorOriginationResponseTypeDef](./type_defs.md#getvoiceconnectororiginationresponsetypedef) 


```python
# get_voice_connector_origination method usage example with argument unpacking

kwargs: GetVoiceConnectorOriginationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_origination(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorOriginationRequestTypeDef](./type_defs.md#getvoiceconnectororiginationrequesttypedef) 

### get\_voice\_connector\_proxy

Gets the proxy configuration details for the specified Amazon Chime Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime").get_voice_connector_proxy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_voice_connector_proxy.html)

```python
# get_voice_connector_proxy method definition

await def get_voice_connector_proxy(
    self,
    *,
    VoiceConnectorId: str,
) -> GetVoiceConnectorProxyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceConnectorProxyResponseTypeDef](./type_defs.md#getvoiceconnectorproxyresponsetypedef) 


```python
# get_voice_connector_proxy method usage example with argument unpacking

kwargs: GetVoiceConnectorProxyRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_proxy(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorProxyRequestTypeDef](./type_defs.md#getvoiceconnectorproxyrequesttypedef) 

### get\_voice\_connector\_streaming\_configuration

Retrieves the streaming configuration details for the specified Amazon Chime
Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").get_voice_connector_streaming_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_voice_connector_streaming_configuration.html)

```python
# get_voice_connector_streaming_configuration method definition

await def get_voice_connector_streaming_configuration(
    self,
    *,
    VoiceConnectorId: str,
) -> GetVoiceConnectorStreamingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceConnectorStreamingConfigurationResponseTypeDef](./type_defs.md#getvoiceconnectorstreamingconfigurationresponsetypedef) 


```python
# get_voice_connector_streaming_configuration method usage example with argument unpacking

kwargs: GetVoiceConnectorStreamingConfigurationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_streaming_configuration(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorStreamingConfigurationRequestTypeDef](./type_defs.md#getvoiceconnectorstreamingconfigurationrequesttypedef) 

### get\_voice\_connector\_termination

Retrieves termination setting details for the specified Amazon Chime Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime").get_voice_connector_termination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_voice_connector_termination.html)

```python
# get_voice_connector_termination method definition

await def get_voice_connector_termination(
    self,
    *,
    VoiceConnectorId: str,
) -> GetVoiceConnectorTerminationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceConnectorTerminationResponseTypeDef](./type_defs.md#getvoiceconnectorterminationresponsetypedef) 


```python
# get_voice_connector_termination method usage example with argument unpacking

kwargs: GetVoiceConnectorTerminationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_termination(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorTerminationRequestTypeDef](./type_defs.md#getvoiceconnectorterminationrequesttypedef) 

### get\_voice\_connector\_termination\_health

<b>This API is is no longer supported and will not be updated.</b> We recommend
using the latest version, <a
href="https://docs.aws.amazon.com/chime-sdk/latest/APIReference/API_voice-chime_GetVoiceConnectorTerminationHealth.html">GetVoiceConnectorTerminationHealth</a>,
in the Amazon Chime SDK.

Type annotations and code completion for `#!python session.create_client("chime").get_voice_connector_termination_health` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/get_voice_connector_termination_health.html)

```python
# get_voice_connector_termination_health method definition

await def get_voice_connector_termination_health(
    self,
    *,
    VoiceConnectorId: str,
) -> GetVoiceConnectorTerminationHealthResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceConnectorTerminationHealthResponseTypeDef](./type_defs.md#getvoiceconnectorterminationhealthresponsetypedef) 


```python
# get_voice_connector_termination_health method usage example with argument unpacking

kwargs: GetVoiceConnectorTerminationHealthRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_termination_health(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorTerminationHealthRequestTypeDef](./type_defs.md#getvoiceconnectorterminationhealthrequesttypedef) 

### invite\_users

Sends email to a maximum of 50 users, inviting them to the specified Amazon
Chime <code>Team</code> account.

Type annotations and code completion for `#!python session.create_client("chime").invite_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/invite_users.html)

```python
# invite_users method definition

await def invite_users(
    self,
    *,
    AccountId: str,
    UserEmailList: Sequence[str],
    UserType: UserTypeType = ...,  # (1)
) -> InviteUsersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: InviteUsersResponseTypeDef](./type_defs.md#inviteusersresponsetypedef) 


```python
# invite_users method usage example with argument unpacking

kwargs: InviteUsersRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserEmailList": ...,
}

parent.invite_users(**kwargs)
```

1. See [:material-code-braces: InviteUsersRequestTypeDef](./type_defs.md#inviteusersrequesttypedef) 

### list\_accounts

Lists the Amazon Chime accounts under the administrator's AWS account.

Type annotations and code completion for `#!python session.create_client("chime").list_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_accounts.html)

```python
# list_accounts method definition

await def list_accounts(
    self,
    *,
    Name: str = ...,
    UserEmail: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef) 


```python
# list_accounts method usage example with argument unpacking

kwargs: ListAccountsRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.list_accounts(**kwargs)
```

1. See [:material-code-braces: ListAccountsRequestTypeDef](./type_defs.md#listaccountsrequesttypedef) 

### list\_app\_instance\_admins

Returns a list of the administrators in the <code>AppInstance</code>.

Type annotations and code completion for `#!python session.create_client("chime").list_app_instance_admins` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_app_instance_admins.html)

```python
# list_app_instance_admins method definition

await def list_app_instance_admins(
    self,
    *,
    AppInstanceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAppInstanceAdminsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppInstanceAdminsResponseTypeDef](./type_defs.md#listappinstanceadminsresponsetypedef) 


```python
# list_app_instance_admins method usage example with argument unpacking

kwargs: ListAppInstanceAdminsRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
}

parent.list_app_instance_admins(**kwargs)
```

1. See [:material-code-braces: ListAppInstanceAdminsRequestTypeDef](./type_defs.md#listappinstanceadminsrequesttypedef) 

### list\_app\_instance\_users

List all <code>AppInstanceUsers</code> created under a single
<code>AppInstance</code>.

Type annotations and code completion for `#!python session.create_client("chime").list_app_instance_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_app_instance_users.html)

```python
# list_app_instance_users method definition

await def list_app_instance_users(
    self,
    *,
    AppInstanceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAppInstanceUsersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppInstanceUsersResponseTypeDef](./type_defs.md#listappinstanceusersresponsetypedef) 


```python
# list_app_instance_users method usage example with argument unpacking

kwargs: ListAppInstanceUsersRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
}

parent.list_app_instance_users(**kwargs)
```

1. See [:material-code-braces: ListAppInstanceUsersRequestTypeDef](./type_defs.md#listappinstanceusersrequesttypedef) 

### list\_app\_instances

Lists all Amazon Chime <code>AppInstance</code>s created under a single AWS
account.

Type annotations and code completion for `#!python session.create_client("chime").list_app_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_app_instances.html)

```python
# list_app_instances method definition

await def list_app_instances(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAppInstancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAppInstancesResponseTypeDef](./type_defs.md#listappinstancesresponsetypedef) 


```python
# list_app_instances method usage example with argument unpacking

kwargs: ListAppInstancesRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_app_instances(**kwargs)
```

1. See [:material-code-braces: ListAppInstancesRequestTypeDef](./type_defs.md#listappinstancesrequesttypedef) 

### list\_attendee\_tags

Lists the tags applied to an Amazon Chime SDK attendee resource.

Type annotations and code completion for `#!python session.create_client("chime").list_attendee_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_attendee_tags.html)

```python
# list_attendee_tags method definition

await def list_attendee_tags(
    self,
    *,
    MeetingId: str,
    AttendeeId: str,
) -> ListAttendeeTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAttendeeTagsResponseTypeDef](./type_defs.md#listattendeetagsresponsetypedef) 


```python
# list_attendee_tags method usage example with argument unpacking

kwargs: ListAttendeeTagsRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "AttendeeId": ...,
}

parent.list_attendee_tags(**kwargs)
```

1. See [:material-code-braces: ListAttendeeTagsRequestTypeDef](./type_defs.md#listattendeetagsrequesttypedef) 

### list\_attendees

Lists the attendees for the specified Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.create_client("chime").list_attendees` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_attendees.html)

```python
# list_attendees method definition

await def list_attendees(
    self,
    *,
    MeetingId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAttendeesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAttendeesResponseTypeDef](./type_defs.md#listattendeesresponsetypedef) 


```python
# list_attendees method usage example with argument unpacking

kwargs: ListAttendeesRequestTypeDef = {  # (1)
    "MeetingId": ...,
}

parent.list_attendees(**kwargs)
```

1. See [:material-code-braces: ListAttendeesRequestTypeDef](./type_defs.md#listattendeesrequesttypedef) 

### list\_bots

Lists the bots associated with the administrator's Amazon Chime Enterprise
account ID.

Type annotations and code completion for `#!python session.create_client("chime").list_bots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_bots.html)

```python
# list_bots method definition

await def list_bots(
    self,
    *,
    AccountId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListBotsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBotsResponseTypeDef](./type_defs.md#listbotsresponsetypedef) 


```python
# list_bots method usage example with argument unpacking

kwargs: ListBotsRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_bots(**kwargs)
```

1. See [:material-code-braces: ListBotsRequestTypeDef](./type_defs.md#listbotsrequesttypedef) 

### list\_channel\_bans

Lists all the users banned from a particular channel.

Type annotations and code completion for `#!python session.create_client("chime").list_channel_bans` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_channel_bans.html)

```python
# list_channel_bans method definition

await def list_channel_bans(
    self,
    *,
    ChannelArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    ChimeBearer: str = ...,
) -> ListChannelBansResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelBansResponseTypeDef](./type_defs.md#listchannelbansresponsetypedef) 


```python
# list_channel_bans method usage example with argument unpacking

kwargs: ListChannelBansRequestTypeDef = {  # (1)
    "ChannelArn": ...,
}

parent.list_channel_bans(**kwargs)
```

1. See [:material-code-braces: ListChannelBansRequestTypeDef](./type_defs.md#listchannelbansrequesttypedef) 

### list\_channel\_memberships

Lists all channel memberships in a channel.

Type annotations and code completion for `#!python session.create_client("chime").list_channel_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_channel_memberships.html)

```python
# list_channel_memberships method definition

await def list_channel_memberships(
    self,
    *,
    ChannelArn: str,
    Type: ChannelMembershipTypeType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
    ChimeBearer: str = ...,
) -> ListChannelMembershipsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ChannelMembershipTypeType](./literals.md#channelmembershiptypetype) 
2. See [:material-code-braces: ListChannelMembershipsResponseTypeDef](./type_defs.md#listchannelmembershipsresponsetypedef) 


```python
# list_channel_memberships method usage example with argument unpacking

kwargs: ListChannelMembershipsRequestTypeDef = {  # (1)
    "ChannelArn": ...,
}

parent.list_channel_memberships(**kwargs)
```

1. See [:material-code-braces: ListChannelMembershipsRequestTypeDef](./type_defs.md#listchannelmembershipsrequesttypedef) 

### list\_channel\_memberships\_for\_app\_instance\_user

Lists all channels that a particular <code>AppInstanceUser</code> is a part of.

Type annotations and code completion for `#!python session.create_client("chime").list_channel_memberships_for_app_instance_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_channel_memberships_for_app_instance_user.html)

```python
# list_channel_memberships_for_app_instance_user method definition

await def list_channel_memberships_for_app_instance_user(
    self,
    *,
    AppInstanceUserArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ChimeBearer: str = ...,
) -> ListChannelMembershipsForAppInstanceUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelMembershipsForAppInstanceUserResponseTypeDef](./type_defs.md#listchannelmembershipsforappinstanceuserresponsetypedef) 


```python
# list_channel_memberships_for_app_instance_user method usage example with argument unpacking

kwargs: ListChannelMembershipsForAppInstanceUserRequestTypeDef = {  # (1)
    "AppInstanceUserArn": ...,
}

parent.list_channel_memberships_for_app_instance_user(**kwargs)
```

1. See [:material-code-braces: ListChannelMembershipsForAppInstanceUserRequestTypeDef](./type_defs.md#listchannelmembershipsforappinstanceuserrequesttypedef) 

### list\_channel\_messages

List all the messages in a channel.

Type annotations and code completion for `#!python session.create_client("chime").list_channel_messages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_channel_messages.html)

```python
# list_channel_messages method definition

await def list_channel_messages(
    self,
    *,
    ChannelArn: str,
    SortOrder: SortOrderType = ...,  # (1)
    NotBefore: TimestampTypeDef = ...,
    NotAfter: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ChimeBearer: str = ...,
) -> ListChannelMessagesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: ListChannelMessagesResponseTypeDef](./type_defs.md#listchannelmessagesresponsetypedef) 


```python
# list_channel_messages method usage example with argument unpacking

kwargs: ListChannelMessagesRequestTypeDef = {  # (1)
    "ChannelArn": ...,
}

parent.list_channel_messages(**kwargs)
```

1. See [:material-code-braces: ListChannelMessagesRequestTypeDef](./type_defs.md#listchannelmessagesrequesttypedef) 

### list\_channel\_moderators

Lists all the moderators for a channel.

Type annotations and code completion for `#!python session.create_client("chime").list_channel_moderators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_channel_moderators.html)

```python
# list_channel_moderators method definition

await def list_channel_moderators(
    self,
    *,
    ChannelArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    ChimeBearer: str = ...,
) -> ListChannelModeratorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelModeratorsResponseTypeDef](./type_defs.md#listchannelmoderatorsresponsetypedef) 


```python
# list_channel_moderators method usage example with argument unpacking

kwargs: ListChannelModeratorsRequestTypeDef = {  # (1)
    "ChannelArn": ...,
}

parent.list_channel_moderators(**kwargs)
```

1. See [:material-code-braces: ListChannelModeratorsRequestTypeDef](./type_defs.md#listchannelmoderatorsrequesttypedef) 

### list\_channels

Lists all Channels created under a single Chime App as a paginated list.

Type annotations and code completion for `#!python session.create_client("chime").list_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_channels.html)

```python
# list_channels method definition

await def list_channels(
    self,
    *,
    AppInstanceArn: str,
    Privacy: ChannelPrivacyType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
    ChimeBearer: str = ...,
) -> ListChannelsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ChannelPrivacyType](./literals.md#channelprivacytype) 
2. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# list_channels method usage example with argument unpacking

kwargs: ListChannelsRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
}

parent.list_channels(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestTypeDef](./type_defs.md#listchannelsrequesttypedef) 

### list\_channels\_moderated\_by\_app\_instance\_user

A list of the channels moderated by an <code>AppInstanceUser</code>.

Type annotations and code completion for `#!python session.create_client("chime").list_channels_moderated_by_app_instance_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_channels_moderated_by_app_instance_user.html)

```python
# list_channels_moderated_by_app_instance_user method definition

await def list_channels_moderated_by_app_instance_user(
    self,
    *,
    AppInstanceUserArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ChimeBearer: str = ...,
) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelsModeratedByAppInstanceUserResponseTypeDef](./type_defs.md#listchannelsmoderatedbyappinstanceuserresponsetypedef) 


```python
# list_channels_moderated_by_app_instance_user method usage example with argument unpacking

kwargs: ListChannelsModeratedByAppInstanceUserRequestTypeDef = {  # (1)
    "AppInstanceUserArn": ...,
}

parent.list_channels_moderated_by_app_instance_user(**kwargs)
```

1. See [:material-code-braces: ListChannelsModeratedByAppInstanceUserRequestTypeDef](./type_defs.md#listchannelsmoderatedbyappinstanceuserrequesttypedef) 

### list\_media\_capture\_pipelines

Returns a list of media capture pipelines.

Type annotations and code completion for `#!python session.create_client("chime").list_media_capture_pipelines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_media_capture_pipelines.html)

```python
# list_media_capture_pipelines method definition

await def list_media_capture_pipelines(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMediaCapturePipelinesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMediaCapturePipelinesResponseTypeDef](./type_defs.md#listmediacapturepipelinesresponsetypedef) 


```python
# list_media_capture_pipelines method usage example with argument unpacking

kwargs: ListMediaCapturePipelinesRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_media_capture_pipelines(**kwargs)
```

1. See [:material-code-braces: ListMediaCapturePipelinesRequestTypeDef](./type_defs.md#listmediacapturepipelinesrequesttypedef) 

### list\_meeting\_tags

Lists the tags applied to an Amazon Chime SDK meeting resource.

Type annotations and code completion for `#!python session.create_client("chime").list_meeting_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_meeting_tags.html)

```python
# list_meeting_tags method definition

await def list_meeting_tags(
    self,
    *,
    MeetingId: str,
) -> ListMeetingTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMeetingTagsResponseTypeDef](./type_defs.md#listmeetingtagsresponsetypedef) 


```python
# list_meeting_tags method usage example with argument unpacking

kwargs: ListMeetingTagsRequestTypeDef = {  # (1)
    "MeetingId": ...,
}

parent.list_meeting_tags(**kwargs)
```

1. See [:material-code-braces: ListMeetingTagsRequestTypeDef](./type_defs.md#listmeetingtagsrequesttypedef) 

### list\_meetings

Lists up to 100 active Amazon Chime SDK meetings.

Type annotations and code completion for `#!python session.create_client("chime").list_meetings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_meetings.html)

```python
# list_meetings method definition

await def list_meetings(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMeetingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMeetingsResponseTypeDef](./type_defs.md#listmeetingsresponsetypedef) 


```python
# list_meetings method usage example with argument unpacking

kwargs: ListMeetingsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_meetings(**kwargs)
```

1. See [:material-code-braces: ListMeetingsRequestTypeDef](./type_defs.md#listmeetingsrequesttypedef) 

### list\_phone\_number\_orders

Lists the phone number orders for the administrator's Amazon Chime account.

Type annotations and code completion for `#!python session.create_client("chime").list_phone_number_orders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_phone_number_orders.html)

```python
# list_phone_number_orders method definition

await def list_phone_number_orders(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPhoneNumberOrdersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPhoneNumberOrdersResponseTypeDef](./type_defs.md#listphonenumberordersresponsetypedef) 


```python
# list_phone_number_orders method usage example with argument unpacking

kwargs: ListPhoneNumberOrdersRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_phone_number_orders(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumberOrdersRequestTypeDef](./type_defs.md#listphonenumberordersrequesttypedef) 

### list\_phone\_numbers

Lists the phone numbers for the specified Amazon Chime account, Amazon Chime
user, Amazon Chime Voice Connector, or Amazon Chime Voice Connector group.

Type annotations and code completion for `#!python session.create_client("chime").list_phone_numbers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_phone_numbers.html)

```python
# list_phone_numbers method definition

await def list_phone_numbers(
    self,
    *,
    Status: PhoneNumberStatusType = ...,  # (1)
    ProductType: PhoneNumberProductTypeType = ...,  # (2)
    FilterName: PhoneNumberAssociationNameType = ...,  # (3)
    FilterValue: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPhoneNumbersResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: PhoneNumberStatusType](./literals.md#phonenumberstatustype) 
2. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
3. See [:material-code-brackets: PhoneNumberAssociationNameType](./literals.md#phonenumberassociationnametype) 
4. See [:material-code-braces: ListPhoneNumbersResponseTypeDef](./type_defs.md#listphonenumbersresponsetypedef) 


```python
# list_phone_numbers method usage example with argument unpacking

kwargs: ListPhoneNumbersRequestTypeDef = {  # (1)
    "Status": ...,
}

parent.list_phone_numbers(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumbersRequestTypeDef](./type_defs.md#listphonenumbersrequesttypedef) 

### list\_proxy\_sessions

Lists the proxy sessions for the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").list_proxy_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_proxy_sessions.html)

```python
# list_proxy_sessions method definition

await def list_proxy_sessions(
    self,
    *,
    VoiceConnectorId: str,
    Status: ProxySessionStatusType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListProxySessionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ProxySessionStatusType](./literals.md#proxysessionstatustype) 
2. See [:material-code-braces: ListProxySessionsResponseTypeDef](./type_defs.md#listproxysessionsresponsetypedef) 


```python
# list_proxy_sessions method usage example with argument unpacking

kwargs: ListProxySessionsRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.list_proxy_sessions(**kwargs)
```

1. See [:material-code-braces: ListProxySessionsRequestTypeDef](./type_defs.md#listproxysessionsrequesttypedef) 

### list\_room\_memberships

Lists the membership details for the specified room in an Amazon Chime
Enterprise account, such as the members' IDs, email addresses, and names.

Type annotations and code completion for `#!python session.create_client("chime").list_room_memberships` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_room_memberships.html)

```python
# list_room_memberships method definition

await def list_room_memberships(
    self,
    *,
    AccountId: str,
    RoomId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRoomMembershipsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRoomMembershipsResponseTypeDef](./type_defs.md#listroommembershipsresponsetypedef) 


```python
# list_room_memberships method usage example with argument unpacking

kwargs: ListRoomMembershipsRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RoomId": ...,
}

parent.list_room_memberships(**kwargs)
```

1. See [:material-code-braces: ListRoomMembershipsRequestTypeDef](./type_defs.md#listroommembershipsrequesttypedef) 

### list\_rooms

Lists the room details for the specified Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").list_rooms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_rooms.html)

```python
# list_rooms method definition

await def list_rooms(
    self,
    *,
    AccountId: str,
    MemberId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRoomsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRoomsResponseTypeDef](./type_defs.md#listroomsresponsetypedef) 


```python
# list_rooms method usage example with argument unpacking

kwargs: ListRoomsRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_rooms(**kwargs)
```

1. See [:material-code-braces: ListRoomsRequestTypeDef](./type_defs.md#listroomsrequesttypedef) 

### list\_sip\_media\_applications

Lists the SIP media applications under the administrator's AWS account.

Type annotations and code completion for `#!python session.create_client("chime").list_sip_media_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_sip_media_applications.html)

```python
# list_sip_media_applications method definition

await def list_sip_media_applications(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSipMediaApplicationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSipMediaApplicationsResponseTypeDef](./type_defs.md#listsipmediaapplicationsresponsetypedef) 


```python
# list_sip_media_applications method usage example with argument unpacking

kwargs: ListSipMediaApplicationsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_sip_media_applications(**kwargs)
```

1. See [:material-code-braces: ListSipMediaApplicationsRequestTypeDef](./type_defs.md#listsipmediaapplicationsrequesttypedef) 

### list\_sip\_rules

Lists the SIP rules under the administrator's AWS account.

Type annotations and code completion for `#!python session.create_client("chime").list_sip_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_sip_rules.html)

```python
# list_sip_rules method definition

await def list_sip_rules(
    self,
    *,
    SipMediaApplicationId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSipRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSipRulesResponseTypeDef](./type_defs.md#listsiprulesresponsetypedef) 


```python
# list_sip_rules method usage example with argument unpacking

kwargs: ListSipRulesRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.list_sip_rules(**kwargs)
```

1. See [:material-code-braces: ListSipRulesRequestTypeDef](./type_defs.md#listsiprulesrequesttypedef) 

### list\_supported\_phone\_number\_countries

Lists supported phone number countries.

Type annotations and code completion for `#!python session.create_client("chime").list_supported_phone_number_countries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_supported_phone_number_countries.html)

```python
# list_supported_phone_number_countries method definition

await def list_supported_phone_number_countries(
    self,
    *,
    ProductType: PhoneNumberProductTypeType,  # (1)
) -> ListSupportedPhoneNumberCountriesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
2. See [:material-code-braces: ListSupportedPhoneNumberCountriesResponseTypeDef](./type_defs.md#listsupportedphonenumbercountriesresponsetypedef) 


```python
# list_supported_phone_number_countries method usage example with argument unpacking

kwargs: ListSupportedPhoneNumberCountriesRequestTypeDef = {  # (1)
    "ProductType": ...,
}

parent.list_supported_phone_number_countries(**kwargs)
```

1. See [:material-code-braces: ListSupportedPhoneNumberCountriesRequestTypeDef](./type_defs.md#listsupportedphonenumbercountriesrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags applied to an Amazon Chime SDK meeting and messaging resources.

Type annotations and code completion for `#!python session.create_client("chime").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### list\_users

Lists the users that belong to the specified Amazon Chime account.

Type annotations and code completion for `#!python session.create_client("chime").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_users.html)

```python
# list_users method definition

await def list_users(
    self,
    *,
    AccountId: str,
    UserEmail: str = ...,
    UserType: UserTypeType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListUsersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
2. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# list_users method usage example with argument unpacking

kwargs: ListUsersRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.list_users(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestTypeDef](./type_defs.md#listusersrequesttypedef) 

### list\_voice\_connector\_groups

Lists the Amazon Chime Voice Connector groups for the administrator's AWS
account.

Type annotations and code completion for `#!python session.create_client("chime").list_voice_connector_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_voice_connector_groups.html)

```python
# list_voice_connector_groups method definition

await def list_voice_connector_groups(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListVoiceConnectorGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVoiceConnectorGroupsResponseTypeDef](./type_defs.md#listvoiceconnectorgroupsresponsetypedef) 


```python
# list_voice_connector_groups method usage example with argument unpacking

kwargs: ListVoiceConnectorGroupsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_voice_connector_groups(**kwargs)
```

1. See [:material-code-braces: ListVoiceConnectorGroupsRequestTypeDef](./type_defs.md#listvoiceconnectorgroupsrequesttypedef) 

### list\_voice\_connector\_termination\_credentials

Lists the SIP credentials for the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").list_voice_connector_termination_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_voice_connector_termination_credentials.html)

```python
# list_voice_connector_termination_credentials method definition

await def list_voice_connector_termination_credentials(
    self,
    *,
    VoiceConnectorId: str,
) -> ListVoiceConnectorTerminationCredentialsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVoiceConnectorTerminationCredentialsResponseTypeDef](./type_defs.md#listvoiceconnectorterminationcredentialsresponsetypedef) 


```python
# list_voice_connector_termination_credentials method usage example with argument unpacking

kwargs: ListVoiceConnectorTerminationCredentialsRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.list_voice_connector_termination_credentials(**kwargs)
```

1. See [:material-code-braces: ListVoiceConnectorTerminationCredentialsRequestTypeDef](./type_defs.md#listvoiceconnectorterminationcredentialsrequesttypedef) 

### list\_voice\_connectors

Lists the Amazon Chime Voice Connectors for the administrator's AWS account.

Type annotations and code completion for `#!python session.create_client("chime").list_voice_connectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/list_voice_connectors.html)

```python
# list_voice_connectors method definition

await def list_voice_connectors(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListVoiceConnectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVoiceConnectorsResponseTypeDef](./type_defs.md#listvoiceconnectorsresponsetypedef) 


```python
# list_voice_connectors method usage example with argument unpacking

kwargs: ListVoiceConnectorsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_voice_connectors(**kwargs)
```

1. See [:material-code-braces: ListVoiceConnectorsRequestTypeDef](./type_defs.md#listvoiceconnectorsrequesttypedef) 

### logout\_user

Logs out the specified user from all of the devices they are currently logged
into.

Type annotations and code completion for `#!python session.create_client("chime").logout_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/logout_user.html)

```python
# logout_user method definition

await def logout_user(
    self,
    *,
    AccountId: str,
    UserId: str,
) -> Dict[str, Any]:
    ...
```



```python
# logout_user method usage example with argument unpacking

kwargs: LogoutUserRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserId": ...,
}

parent.logout_user(**kwargs)
```

1. See [:material-code-braces: LogoutUserRequestTypeDef](./type_defs.md#logoutuserrequesttypedef) 

### put\_app\_instance\_retention\_settings

Sets the amount of time in days that a given <code>AppInstance</code> retains
data.

Type annotations and code completion for `#!python session.create_client("chime").put_app_instance_retention_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_app_instance_retention_settings.html)

```python
# put_app_instance_retention_settings method definition

await def put_app_instance_retention_settings(
    self,
    *,
    AppInstanceArn: str,
    AppInstanceRetentionSettings: AppInstanceRetentionSettingsTypeDef,  # (1)
) -> PutAppInstanceRetentionSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AppInstanceRetentionSettingsTypeDef](./type_defs.md#appinstanceretentionsettingstypedef) 
2. See [:material-code-braces: PutAppInstanceRetentionSettingsResponseTypeDef](./type_defs.md#putappinstanceretentionsettingsresponsetypedef) 


```python
# put_app_instance_retention_settings method usage example with argument unpacking

kwargs: PutAppInstanceRetentionSettingsRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
    "AppInstanceRetentionSettings": ...,
}

parent.put_app_instance_retention_settings(**kwargs)
```

1. See [:material-code-braces: PutAppInstanceRetentionSettingsRequestTypeDef](./type_defs.md#putappinstanceretentionsettingsrequesttypedef) 

### put\_app\_instance\_streaming\_configurations

The data streaming configurations of an <code>AppInstance</code>.

Type annotations and code completion for `#!python session.create_client("chime").put_app_instance_streaming_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_app_instance_streaming_configurations.html)

```python
# put_app_instance_streaming_configurations method definition

await def put_app_instance_streaming_configurations(
    self,
    *,
    AppInstanceArn: str,
    AppInstanceStreamingConfigurations: Sequence[AppInstanceStreamingConfigurationTypeDef],  # (1)
) -> PutAppInstanceStreamingConfigurationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AppInstanceStreamingConfigurationTypeDef](./type_defs.md#appinstancestreamingconfigurationtypedef) 
2. See [:material-code-braces: PutAppInstanceStreamingConfigurationsResponseTypeDef](./type_defs.md#putappinstancestreamingconfigurationsresponsetypedef) 


```python
# put_app_instance_streaming_configurations method usage example with argument unpacking

kwargs: PutAppInstanceStreamingConfigurationsRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
    "AppInstanceStreamingConfigurations": ...,
}

parent.put_app_instance_streaming_configurations(**kwargs)
```

1. See [:material-code-braces: PutAppInstanceStreamingConfigurationsRequestTypeDef](./type_defs.md#putappinstancestreamingconfigurationsrequesttypedef) 

### put\_events\_configuration

Creates an events configuration that allows a bot to receive outgoing events
sent by Amazon Chime.

Type annotations and code completion for `#!python session.create_client("chime").put_events_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_events_configuration.html)

```python
# put_events_configuration method definition

await def put_events_configuration(
    self,
    *,
    AccountId: str,
    BotId: str,
    OutboundEventsHTTPSEndpoint: str = ...,
    LambdaFunctionArn: str = ...,
) -> PutEventsConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutEventsConfigurationResponseTypeDef](./type_defs.md#puteventsconfigurationresponsetypedef) 


```python
# put_events_configuration method usage example with argument unpacking

kwargs: PutEventsConfigurationRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BotId": ...,
}

parent.put_events_configuration(**kwargs)
```

1. See [:material-code-braces: PutEventsConfigurationRequestTypeDef](./type_defs.md#puteventsconfigurationrequesttypedef) 

### put\_retention\_settings

Puts retention settings for the specified Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").put_retention_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_retention_settings.html)

```python
# put_retention_settings method definition

await def put_retention_settings(
    self,
    *,
    AccountId: str,
    RetentionSettings: RetentionSettingsTypeDef,  # (1)
) -> PutRetentionSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RetentionSettingsTypeDef](./type_defs.md#retentionsettingstypedef) 
2. See [:material-code-braces: PutRetentionSettingsResponseTypeDef](./type_defs.md#putretentionsettingsresponsetypedef) 


```python
# put_retention_settings method usage example with argument unpacking

kwargs: PutRetentionSettingsRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RetentionSettings": ...,
}

parent.put_retention_settings(**kwargs)
```

1. See [:material-code-braces: PutRetentionSettingsRequestTypeDef](./type_defs.md#putretentionsettingsrequesttypedef) 

### put\_sip\_media\_application\_logging\_configuration

Updates the logging configuration for the specified SIP media application.

Type annotations and code completion for `#!python session.create_client("chime").put_sip_media_application_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_sip_media_application_logging_configuration.html)

```python
# put_sip_media_application_logging_configuration method definition

await def put_sip_media_application_logging_configuration(
    self,
    *,
    SipMediaApplicationId: str,
    SipMediaApplicationLoggingConfiguration: SipMediaApplicationLoggingConfigurationTypeDef = ...,  # (1)
) -> PutSipMediaApplicationLoggingConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SipMediaApplicationLoggingConfigurationTypeDef](./type_defs.md#sipmediaapplicationloggingconfigurationtypedef) 
2. See [:material-code-braces: PutSipMediaApplicationLoggingConfigurationResponseTypeDef](./type_defs.md#putsipmediaapplicationloggingconfigurationresponsetypedef) 


```python
# put_sip_media_application_logging_configuration method usage example with argument unpacking

kwargs: PutSipMediaApplicationLoggingConfigurationRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.put_sip_media_application_logging_configuration(**kwargs)
```

1. See [:material-code-braces: PutSipMediaApplicationLoggingConfigurationRequestTypeDef](./type_defs.md#putsipmediaapplicationloggingconfigurationrequesttypedef) 

### put\_voice\_connector\_emergency\_calling\_configuration

Puts emergency calling configuration details to the specified Amazon Chime
Voice Connector, such as emergency phone numbers and calling countries.

Type annotations and code completion for `#!python session.create_client("chime").put_voice_connector_emergency_calling_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_voice_connector_emergency_calling_configuration.html)

```python
# put_voice_connector_emergency_calling_configuration method definition

await def put_voice_connector_emergency_calling_configuration(
    self,
    *,
    VoiceConnectorId: str,
    EmergencyCallingConfiguration: EmergencyCallingConfigurationUnionTypeDef,  # (1)
) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EmergencyCallingConfigurationTypeDef](./type_defs.md#emergencycallingconfigurationtypedef) [:material-code-braces: EmergencyCallingConfigurationOutputTypeDef](./type_defs.md#emergencycallingconfigurationoutputtypedef) 
2. See [:material-code-braces: PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef](./type_defs.md#putvoiceconnectoremergencycallingconfigurationresponsetypedef) 


```python
# put_voice_connector_emergency_calling_configuration method usage example with argument unpacking

kwargs: PutVoiceConnectorEmergencyCallingConfigurationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "EmergencyCallingConfiguration": ...,
}

parent.put_voice_connector_emergency_calling_configuration(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorEmergencyCallingConfigurationRequestTypeDef](./type_defs.md#putvoiceconnectoremergencycallingconfigurationrequesttypedef) 

### put\_voice\_connector\_logging\_configuration

Adds a logging configuration for the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").put_voice_connector_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_voice_connector_logging_configuration.html)

```python
# put_voice_connector_logging_configuration method definition

await def put_voice_connector_logging_configuration(
    self,
    *,
    VoiceConnectorId: str,
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (1)
) -> PutVoiceConnectorLoggingConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
2. See [:material-code-braces: PutVoiceConnectorLoggingConfigurationResponseTypeDef](./type_defs.md#putvoiceconnectorloggingconfigurationresponsetypedef) 


```python
# put_voice_connector_logging_configuration method usage example with argument unpacking

kwargs: PutVoiceConnectorLoggingConfigurationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "LoggingConfiguration": ...,
}

parent.put_voice_connector_logging_configuration(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorLoggingConfigurationRequestTypeDef](./type_defs.md#putvoiceconnectorloggingconfigurationrequesttypedef) 

### put\_voice\_connector\_origination

Adds origination settings for the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").put_voice_connector_origination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_voice_connector_origination.html)

```python
# put_voice_connector_origination method definition

await def put_voice_connector_origination(
    self,
    *,
    VoiceConnectorId: str,
    Origination: OriginationUnionTypeDef,  # (1)
) -> PutVoiceConnectorOriginationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OriginationTypeDef](./type_defs.md#originationtypedef) [:material-code-braces: OriginationOutputTypeDef](./type_defs.md#originationoutputtypedef) 
2. See [:material-code-braces: PutVoiceConnectorOriginationResponseTypeDef](./type_defs.md#putvoiceconnectororiginationresponsetypedef) 


```python
# put_voice_connector_origination method usage example with argument unpacking

kwargs: PutVoiceConnectorOriginationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "Origination": ...,
}

parent.put_voice_connector_origination(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorOriginationRequestTypeDef](./type_defs.md#putvoiceconnectororiginationrequesttypedef) 

### put\_voice\_connector\_proxy

Puts the specified proxy configuration to the specified Amazon Chime Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime").put_voice_connector_proxy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_voice_connector_proxy.html)

```python
# put_voice_connector_proxy method definition

await def put_voice_connector_proxy(
    self,
    *,
    VoiceConnectorId: str,
    DefaultSessionExpiryMinutes: int,
    PhoneNumberPoolCountries: Sequence[str],
    FallBackPhoneNumber: str = ...,
    Disabled: bool = ...,
) -> PutVoiceConnectorProxyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutVoiceConnectorProxyResponseTypeDef](./type_defs.md#putvoiceconnectorproxyresponsetypedef) 


```python
# put_voice_connector_proxy method usage example with argument unpacking

kwargs: PutVoiceConnectorProxyRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "DefaultSessionExpiryMinutes": ...,
    "PhoneNumberPoolCountries": ...,
}

parent.put_voice_connector_proxy(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorProxyRequestTypeDef](./type_defs.md#putvoiceconnectorproxyrequesttypedef) 

### put\_voice\_connector\_streaming\_configuration

Adds a streaming configuration for the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").put_voice_connector_streaming_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_voice_connector_streaming_configuration.html)

```python
# put_voice_connector_streaming_configuration method definition

await def put_voice_connector_streaming_configuration(
    self,
    *,
    VoiceConnectorId: str,
    StreamingConfiguration: StreamingConfigurationUnionTypeDef,  # (1)
) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamingConfigurationTypeDef](./type_defs.md#streamingconfigurationtypedef) [:material-code-braces: StreamingConfigurationOutputTypeDef](./type_defs.md#streamingconfigurationoutputtypedef) 
2. See [:material-code-braces: PutVoiceConnectorStreamingConfigurationResponseTypeDef](./type_defs.md#putvoiceconnectorstreamingconfigurationresponsetypedef) 


```python
# put_voice_connector_streaming_configuration method usage example with argument unpacking

kwargs: PutVoiceConnectorStreamingConfigurationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "StreamingConfiguration": ...,
}

parent.put_voice_connector_streaming_configuration(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorStreamingConfigurationRequestTypeDef](./type_defs.md#putvoiceconnectorstreamingconfigurationrequesttypedef) 

### put\_voice\_connector\_termination

Adds termination settings for the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").put_voice_connector_termination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_voice_connector_termination.html)

```python
# put_voice_connector_termination method definition

await def put_voice_connector_termination(
    self,
    *,
    VoiceConnectorId: str,
    Termination: TerminationUnionTypeDef,  # (1)
) -> PutVoiceConnectorTerminationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TerminationTypeDef](./type_defs.md#terminationtypedef) [:material-code-braces: TerminationOutputTypeDef](./type_defs.md#terminationoutputtypedef) 
2. See [:material-code-braces: PutVoiceConnectorTerminationResponseTypeDef](./type_defs.md#putvoiceconnectorterminationresponsetypedef) 


```python
# put_voice_connector_termination method usage example with argument unpacking

kwargs: PutVoiceConnectorTerminationRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "Termination": ...,
}

parent.put_voice_connector_termination(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorTerminationRequestTypeDef](./type_defs.md#putvoiceconnectorterminationrequesttypedef) 

### put\_voice\_connector\_termination\_credentials

Adds termination SIP credentials for the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").put_voice_connector_termination_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/put_voice_connector_termination_credentials.html)

```python
# put_voice_connector_termination_credentials method definition

await def put_voice_connector_termination_credentials(
    self,
    *,
    VoiceConnectorId: str,
    Credentials: Sequence[CredentialTypeDef] = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CredentialTypeDef](./type_defs.md#credentialtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_voice_connector_termination_credentials method usage example with argument unpacking

kwargs: PutVoiceConnectorTerminationCredentialsRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.put_voice_connector_termination_credentials(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorTerminationCredentialsRequestTypeDef](./type_defs.md#putvoiceconnectorterminationcredentialsrequesttypedef) 

### redact\_channel\_message

Redacts message content, but not metadata.

Type annotations and code completion for `#!python session.create_client("chime").redact_channel_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/redact_channel_message.html)

```python
# redact_channel_message method definition

await def redact_channel_message(
    self,
    *,
    ChannelArn: str,
    MessageId: str,
    ChimeBearer: str = ...,
) -> RedactChannelMessageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RedactChannelMessageResponseTypeDef](./type_defs.md#redactchannelmessageresponsetypedef) 


```python
# redact_channel_message method usage example with argument unpacking

kwargs: RedactChannelMessageRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MessageId": ...,
}

parent.redact_channel_message(**kwargs)
```

1. See [:material-code-braces: RedactChannelMessageRequestTypeDef](./type_defs.md#redactchannelmessagerequesttypedef) 

### redact\_conversation\_message

Redacts the specified message from the specified Amazon Chime conversation.

Type annotations and code completion for `#!python session.create_client("chime").redact_conversation_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/redact_conversation_message.html)

```python
# redact_conversation_message method definition

await def redact_conversation_message(
    self,
    *,
    AccountId: str,
    ConversationId: str,
    MessageId: str,
) -> Dict[str, Any]:
    ...
```



```python
# redact_conversation_message method usage example with argument unpacking

kwargs: RedactConversationMessageRequestTypeDef = {  # (1)
    "AccountId": ...,
    "ConversationId": ...,
    "MessageId": ...,
}

parent.redact_conversation_message(**kwargs)
```

1. See [:material-code-braces: RedactConversationMessageRequestTypeDef](./type_defs.md#redactconversationmessagerequesttypedef) 

### redact\_room\_message

Redacts the specified message from the specified Amazon Chime channel.

Type annotations and code completion for `#!python session.create_client("chime").redact_room_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/redact_room_message.html)

```python
# redact_room_message method definition

await def redact_room_message(
    self,
    *,
    AccountId: str,
    RoomId: str,
    MessageId: str,
) -> Dict[str, Any]:
    ...
```



```python
# redact_room_message method usage example with argument unpacking

kwargs: RedactRoomMessageRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RoomId": ...,
    "MessageId": ...,
}

parent.redact_room_message(**kwargs)
```

1. See [:material-code-braces: RedactRoomMessageRequestTypeDef](./type_defs.md#redactroommessagerequesttypedef) 

### regenerate\_security\_token

Regenerates the security token for a bot.

Type annotations and code completion for `#!python session.create_client("chime").regenerate_security_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/regenerate_security_token.html)

```python
# regenerate_security_token method definition

await def regenerate_security_token(
    self,
    *,
    AccountId: str,
    BotId: str,
) -> RegenerateSecurityTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegenerateSecurityTokenResponseTypeDef](./type_defs.md#regeneratesecuritytokenresponsetypedef) 


```python
# regenerate_security_token method usage example with argument unpacking

kwargs: RegenerateSecurityTokenRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BotId": ...,
}

parent.regenerate_security_token(**kwargs)
```

1. See [:material-code-braces: RegenerateSecurityTokenRequestTypeDef](./type_defs.md#regeneratesecuritytokenrequesttypedef) 

### reset\_personal\_pin

Resets the personal meeting PIN for the specified user on an Amazon Chime
account.

Type annotations and code completion for `#!python session.create_client("chime").reset_personal_pin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/reset_personal_pin.html)

```python
# reset_personal_pin method definition

await def reset_personal_pin(
    self,
    *,
    AccountId: str,
    UserId: str,
) -> ResetPersonalPINResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResetPersonalPINResponseTypeDef](./type_defs.md#resetpersonalpinresponsetypedef) 


```python
# reset_personal_pin method usage example with argument unpacking

kwargs: ResetPersonalPINRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserId": ...,
}

parent.reset_personal_pin(**kwargs)
```

1. See [:material-code-braces: ResetPersonalPINRequestTypeDef](./type_defs.md#resetpersonalpinrequesttypedef) 

### restore\_phone\_number

Moves a phone number from the <b>Deletion queue</b> back into the phone number
<b>Inventory</b>.

Type annotations and code completion for `#!python session.create_client("chime").restore_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/restore_phone_number.html)

```python
# restore_phone_number method definition

await def restore_phone_number(
    self,
    *,
    PhoneNumberId: str,
) -> RestorePhoneNumberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestorePhoneNumberResponseTypeDef](./type_defs.md#restorephonenumberresponsetypedef) 


```python
# restore_phone_number method usage example with argument unpacking

kwargs: RestorePhoneNumberRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.restore_phone_number(**kwargs)
```

1. See [:material-code-braces: RestorePhoneNumberRequestTypeDef](./type_defs.md#restorephonenumberrequesttypedef) 

### search\_available\_phone\_numbers

Searches for phone numbers that can be ordered.

Type annotations and code completion for `#!python session.create_client("chime").search_available_phone_numbers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/search_available_phone_numbers.html)

```python
# search_available_phone_numbers method definition

await def search_available_phone_numbers(
    self,
    *,
    AreaCode: str = ...,
    City: str = ...,
    Country: str = ...,
    State: str = ...,
    TollFreePrefix: str = ...,
    PhoneNumberType: PhoneNumberTypeType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> SearchAvailablePhoneNumbersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
2. See [:material-code-braces: SearchAvailablePhoneNumbersResponseTypeDef](./type_defs.md#searchavailablephonenumbersresponsetypedef) 


```python
# search_available_phone_numbers method usage example with argument unpacking

kwargs: SearchAvailablePhoneNumbersRequestTypeDef = {  # (1)
    "AreaCode": ...,
}

parent.search_available_phone_numbers(**kwargs)
```

1. See [:material-code-braces: SearchAvailablePhoneNumbersRequestTypeDef](./type_defs.md#searchavailablephonenumbersrequesttypedef) 

### send\_channel\_message

Sends a message to a particular channel that the member is a part of.

Type annotations and code completion for `#!python session.create_client("chime").send_channel_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/send_channel_message.html)

```python
# send_channel_message method definition

await def send_channel_message(
    self,
    *,
    ChannelArn: str,
    Content: str,
    Type: ChannelMessageTypeType,  # (1)
    Persistence: ChannelMessagePersistenceTypeType,  # (2)
    ClientRequestToken: str,
    Metadata: str = ...,
    ChimeBearer: str = ...,
) -> SendChannelMessageResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ChannelMessageTypeType](./literals.md#channelmessagetypetype) 
2. See [:material-code-brackets: ChannelMessagePersistenceTypeType](./literals.md#channelmessagepersistencetypetype) 
3. See [:material-code-braces: SendChannelMessageResponseTypeDef](./type_defs.md#sendchannelmessageresponsetypedef) 


```python
# send_channel_message method usage example with argument unpacking

kwargs: SendChannelMessageRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "Content": ...,
    "Type": ...,
    "Persistence": ...,
    "ClientRequestToken": ...,
}

parent.send_channel_message(**kwargs)
```

1. See [:material-code-braces: SendChannelMessageRequestTypeDef](./type_defs.md#sendchannelmessagerequesttypedef) 

### start\_meeting\_transcription

Starts transcription for the specified <code>meetingId</code>.

Type annotations and code completion for `#!python session.create_client("chime").start_meeting_transcription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/start_meeting_transcription.html)

```python
# start_meeting_transcription method definition

await def start_meeting_transcription(
    self,
    *,
    MeetingId: str,
    TranscriptionConfiguration: TranscriptionConfigurationTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TranscriptionConfigurationTypeDef](./type_defs.md#transcriptionconfigurationtypedef) 


```python
# start_meeting_transcription method usage example with argument unpacking

kwargs: StartMeetingTranscriptionRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "TranscriptionConfiguration": ...,
}

parent.start_meeting_transcription(**kwargs)
```

1. See [:material-code-braces: StartMeetingTranscriptionRequestTypeDef](./type_defs.md#startmeetingtranscriptionrequesttypedef) 

### stop\_meeting\_transcription

Stops transcription for the specified <code>meetingId</code>.

Type annotations and code completion for `#!python session.create_client("chime").stop_meeting_transcription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/stop_meeting_transcription.html)

```python
# stop_meeting_transcription method definition

await def stop_meeting_transcription(
    self,
    *,
    MeetingId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_meeting_transcription method usage example with argument unpacking

kwargs: StopMeetingTranscriptionRequestTypeDef = {  # (1)
    "MeetingId": ...,
}

parent.stop_meeting_transcription(**kwargs)
```

1. See [:material-code-braces: StopMeetingTranscriptionRequestTypeDef](./type_defs.md#stopmeetingtranscriptionrequesttypedef) 

### tag\_attendee

Applies the specified tags to the specified Amazon Chime attendee.

Type annotations and code completion for `#!python session.create_client("chime").tag_attendee` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/tag_attendee.html)

```python
# tag_attendee method definition

await def tag_attendee(
    self,
    *,
    MeetingId: str,
    AttendeeId: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_attendee method usage example with argument unpacking

kwargs: TagAttendeeRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "AttendeeId": ...,
    "Tags": ...,
}

parent.tag_attendee(**kwargs)
```

1. See [:material-code-braces: TagAttendeeRequestTypeDef](./type_defs.md#tagattendeerequesttypedef) 

### tag\_meeting

Applies the specified tags to the specified Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.create_client("chime").tag_meeting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/tag_meeting.html)

```python
# tag_meeting method definition

await def tag_meeting(
    self,
    *,
    MeetingId: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_meeting method usage example with argument unpacking

kwargs: TagMeetingRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "Tags": ...,
}

parent.tag_meeting(**kwargs)
```

1. See [:material-code-braces: TagMeetingRequestTypeDef](./type_defs.md#tagmeetingrequesttypedef) 

### tag\_resource

Applies the specified tags to the specified Amazon Chime SDK meeting resource.

Type annotations and code completion for `#!python session.create_client("chime").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_attendee

Untags the specified tags from the specified Amazon Chime SDK attendee.

Type annotations and code completion for `#!python session.create_client("chime").untag_attendee` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/untag_attendee.html)

```python
# untag_attendee method definition

await def untag_attendee(
    self,
    *,
    MeetingId: str,
    AttendeeId: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_attendee method usage example with argument unpacking

kwargs: UntagAttendeeRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "AttendeeId": ...,
    "TagKeys": ...,
}

parent.untag_attendee(**kwargs)
```

1. See [:material-code-braces: UntagAttendeeRequestTypeDef](./type_defs.md#untagattendeerequesttypedef) 

### untag\_meeting

Untags the specified tags from the specified Amazon Chime SDK meeting.

Type annotations and code completion for `#!python session.create_client("chime").untag_meeting` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/untag_meeting.html)

```python
# untag_meeting method definition

await def untag_meeting(
    self,
    *,
    MeetingId: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_meeting method usage example with argument unpacking

kwargs: UntagMeetingRequestTypeDef = {  # (1)
    "MeetingId": ...,
    "TagKeys": ...,
}

parent.untag_meeting(**kwargs)
```

1. See [:material-code-braces: UntagMeetingRequestTypeDef](./type_defs.md#untagmeetingrequesttypedef) 

### untag\_resource

Untags the specified tags from the specified Amazon Chime SDK meeting resource.

Type annotations and code completion for `#!python session.create_client("chime").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_account

Updates account details for the specified Amazon Chime account.

Type annotations and code completion for `#!python session.create_client("chime").update_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_account.html)

```python
# update_account method definition

await def update_account(
    self,
    *,
    AccountId: str,
    Name: str = ...,
    DefaultLicense: LicenseType = ...,  # (1)
) -> UpdateAccountResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LicenseType](./literals.md#licensetype) 
2. See [:material-code-braces: UpdateAccountResponseTypeDef](./type_defs.md#updateaccountresponsetypedef) 


```python
# update_account method usage example with argument unpacking

kwargs: UpdateAccountRequestTypeDef = {  # (1)
    "AccountId": ...,
}

parent.update_account(**kwargs)
```

1. See [:material-code-braces: UpdateAccountRequestTypeDef](./type_defs.md#updateaccountrequesttypedef) 

### update\_account\_settings

Updates the settings for the specified Amazon Chime account.

Type annotations and code completion for `#!python session.create_client("chime").update_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_account_settings.html)

```python
# update_account_settings method definition

await def update_account_settings(
    self,
    *,
    AccountId: str,
    AccountSettings: AccountSettingsTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 


```python
# update_account_settings method usage example with argument unpacking

kwargs: UpdateAccountSettingsRequestTypeDef = {  # (1)
    "AccountId": ...,
    "AccountSettings": ...,
}

parent.update_account_settings(**kwargs)
```

1. See [:material-code-braces: UpdateAccountSettingsRequestTypeDef](./type_defs.md#updateaccountsettingsrequesttypedef) 

### update\_app\_instance

Updates <code>AppInstance</code> metadata.

Type annotations and code completion for `#!python session.create_client("chime").update_app_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_app_instance.html)

```python
# update_app_instance method definition

await def update_app_instance(
    self,
    *,
    AppInstanceArn: str,
    Name: str,
    Metadata: str = ...,
) -> UpdateAppInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAppInstanceResponseTypeDef](./type_defs.md#updateappinstanceresponsetypedef) 


```python
# update_app_instance method usage example with argument unpacking

kwargs: UpdateAppInstanceRequestTypeDef = {  # (1)
    "AppInstanceArn": ...,
    "Name": ...,
}

parent.update_app_instance(**kwargs)
```

1. See [:material-code-braces: UpdateAppInstanceRequestTypeDef](./type_defs.md#updateappinstancerequesttypedef) 

### update\_app\_instance\_user

Updates the details of an <code>AppInstanceUser</code>.

Type annotations and code completion for `#!python session.create_client("chime").update_app_instance_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_app_instance_user.html)

```python
# update_app_instance_user method definition

await def update_app_instance_user(
    self,
    *,
    AppInstanceUserArn: str,
    Name: str,
    Metadata: str = ...,
) -> UpdateAppInstanceUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAppInstanceUserResponseTypeDef](./type_defs.md#updateappinstanceuserresponsetypedef) 


```python
# update_app_instance_user method usage example with argument unpacking

kwargs: UpdateAppInstanceUserRequestTypeDef = {  # (1)
    "AppInstanceUserArn": ...,
    "Name": ...,
}

parent.update_app_instance_user(**kwargs)
```

1. See [:material-code-braces: UpdateAppInstanceUserRequestTypeDef](./type_defs.md#updateappinstanceuserrequesttypedef) 

### update\_bot

Updates the status of the specified bot, such as starting or stopping the bot
from running in your Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").update_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_bot.html)

```python
# update_bot method definition

await def update_bot(
    self,
    *,
    AccountId: str,
    BotId: str,
    Disabled: bool = ...,
) -> UpdateBotResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateBotResponseTypeDef](./type_defs.md#updatebotresponsetypedef) 


```python
# update_bot method usage example with argument unpacking

kwargs: UpdateBotRequestTypeDef = {  # (1)
    "AccountId": ...,
    "BotId": ...,
}

parent.update_bot(**kwargs)
```

1. See [:material-code-braces: UpdateBotRequestTypeDef](./type_defs.md#updatebotrequesttypedef) 

### update\_channel

Update a channel's attributes.

Type annotations and code completion for `#!python session.create_client("chime").update_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_channel.html)

```python
# update_channel method definition

await def update_channel(
    self,
    *,
    ChannelArn: str,
    Name: str,
    Mode: ChannelModeType,  # (1)
    Metadata: str = ...,
    ChimeBearer: str = ...,
) -> UpdateChannelResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ChannelModeType](./literals.md#channelmodetype) 
2. See [:material-code-braces: UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef) 


```python
# update_channel method usage example with argument unpacking

kwargs: UpdateChannelRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "Name": ...,
    "Mode": ...,
}

parent.update_channel(**kwargs)
```

1. See [:material-code-braces: UpdateChannelRequestTypeDef](./type_defs.md#updatechannelrequesttypedef) 

### update\_channel\_message

Updates the content of a message.

Type annotations and code completion for `#!python session.create_client("chime").update_channel_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_channel_message.html)

```python
# update_channel_message method definition

await def update_channel_message(
    self,
    *,
    ChannelArn: str,
    MessageId: str,
    Content: str = ...,
    Metadata: str = ...,
    ChimeBearer: str = ...,
) -> UpdateChannelMessageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateChannelMessageResponseTypeDef](./type_defs.md#updatechannelmessageresponsetypedef) 


```python
# update_channel_message method usage example with argument unpacking

kwargs: UpdateChannelMessageRequestTypeDef = {  # (1)
    "ChannelArn": ...,
    "MessageId": ...,
}

parent.update_channel_message(**kwargs)
```

1. See [:material-code-braces: UpdateChannelMessageRequestTypeDef](./type_defs.md#updatechannelmessagerequesttypedef) 

### update\_channel\_read\_marker

The details of the time when a user last read messages in a channel.

Type annotations and code completion for `#!python session.create_client("chime").update_channel_read_marker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_channel_read_marker.html)

```python
# update_channel_read_marker method definition

await def update_channel_read_marker(
    self,
    *,
    ChannelArn: str,
    ChimeBearer: str = ...,
) -> UpdateChannelReadMarkerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateChannelReadMarkerResponseTypeDef](./type_defs.md#updatechannelreadmarkerresponsetypedef) 


```python
# update_channel_read_marker method usage example with argument unpacking

kwargs: UpdateChannelReadMarkerRequestTypeDef = {  # (1)
    "ChannelArn": ...,
}

parent.update_channel_read_marker(**kwargs)
```

1. See [:material-code-braces: UpdateChannelReadMarkerRequestTypeDef](./type_defs.md#updatechannelreadmarkerrequesttypedef) 

### update\_global\_settings

Updates global settings for the administrator's AWS account, such as Amazon
Chime Business Calling and Amazon Chime Voice Connector settings.

Type annotations and code completion for `#!python session.create_client("chime").update_global_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_global_settings.html)

```python
# update_global_settings method definition

await def update_global_settings(
    self,
    *,
    BusinessCalling: BusinessCallingSettingsTypeDef = ...,  # (1)
    VoiceConnector: VoiceConnectorSettingsTypeDef = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: BusinessCallingSettingsTypeDef](./type_defs.md#businesscallingsettingstypedef) 
2. See [:material-code-braces: VoiceConnectorSettingsTypeDef](./type_defs.md#voiceconnectorsettingstypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_global_settings method usage example with argument unpacking

kwargs: UpdateGlobalSettingsRequestTypeDef = {  # (1)
    "BusinessCalling": ...,
}

parent.update_global_settings(**kwargs)
```

1. See [:material-code-braces: UpdateGlobalSettingsRequestTypeDef](./type_defs.md#updateglobalsettingsrequesttypedef) 

### update\_phone\_number

Updates phone number details, such as product type or calling name, for the
specified phone number ID.

Type annotations and code completion for `#!python session.create_client("chime").update_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_phone_number.html)

```python
# update_phone_number method definition

await def update_phone_number(
    self,
    *,
    PhoneNumberId: str,
    ProductType: PhoneNumberProductTypeType = ...,  # (1)
    CallingName: str = ...,
) -> UpdatePhoneNumberResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
2. See [:material-code-braces: UpdatePhoneNumberResponseTypeDef](./type_defs.md#updatephonenumberresponsetypedef) 


```python
# update_phone_number method usage example with argument unpacking

kwargs: UpdatePhoneNumberRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.update_phone_number(**kwargs)
```

1. See [:material-code-braces: UpdatePhoneNumberRequestTypeDef](./type_defs.md#updatephonenumberrequesttypedef) 

### update\_phone\_number\_settings

Updates the phone number settings for the administrator's AWS account, such as
the default outbound calling name.

Type annotations and code completion for `#!python session.create_client("chime").update_phone_number_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_phone_number_settings.html)

```python
# update_phone_number_settings method definition

await def update_phone_number_settings(
    self,
    *,
    CallingName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_phone_number_settings method usage example with argument unpacking

kwargs: UpdatePhoneNumberSettingsRequestTypeDef = {  # (1)
    "CallingName": ...,
}

parent.update_phone_number_settings(**kwargs)
```

1. See [:material-code-braces: UpdatePhoneNumberSettingsRequestTypeDef](./type_defs.md#updatephonenumbersettingsrequesttypedef) 

### update\_proxy\_session

Updates the specified proxy session details, such as voice or SMS capabilities.

Type annotations and code completion for `#!python session.create_client("chime").update_proxy_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_proxy_session.html)

```python
# update_proxy_session method definition

await def update_proxy_session(
    self,
    *,
    VoiceConnectorId: str,
    ProxySessionId: str,
    Capabilities: Sequence[CapabilityType],  # (1)
    ExpiryMinutes: int = ...,
) -> UpdateProxySessionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CapabilityType](./literals.md#capabilitytype) 
2. See [:material-code-braces: UpdateProxySessionResponseTypeDef](./type_defs.md#updateproxysessionresponsetypedef) 


```python
# update_proxy_session method usage example with argument unpacking

kwargs: UpdateProxySessionRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "ProxySessionId": ...,
    "Capabilities": ...,
}

parent.update_proxy_session(**kwargs)
```

1. See [:material-code-braces: UpdateProxySessionRequestTypeDef](./type_defs.md#updateproxysessionrequesttypedef) 

### update\_room

Updates room details, such as the room name, for a room in an Amazon Chime
Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").update_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_room.html)

```python
# update_room method definition

await def update_room(
    self,
    *,
    AccountId: str,
    RoomId: str,
    Name: str = ...,
) -> UpdateRoomResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateRoomResponseTypeDef](./type_defs.md#updateroomresponsetypedef) 


```python
# update_room method usage example with argument unpacking

kwargs: UpdateRoomRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RoomId": ...,
}

parent.update_room(**kwargs)
```

1. See [:material-code-braces: UpdateRoomRequestTypeDef](./type_defs.md#updateroomrequesttypedef) 

### update\_room\_membership

Updates room membership details, such as the member role, for a room in an
Amazon Chime Enterprise account.

Type annotations and code completion for `#!python session.create_client("chime").update_room_membership` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_room_membership.html)

```python
# update_room_membership method definition

await def update_room_membership(
    self,
    *,
    AccountId: str,
    RoomId: str,
    MemberId: str,
    Role: RoomMembershipRoleType = ...,  # (1)
) -> UpdateRoomMembershipResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RoomMembershipRoleType](./literals.md#roommembershiproletype) 
2. See [:material-code-braces: UpdateRoomMembershipResponseTypeDef](./type_defs.md#updateroommembershipresponsetypedef) 


```python
# update_room_membership method usage example with argument unpacking

kwargs: UpdateRoomMembershipRequestTypeDef = {  # (1)
    "AccountId": ...,
    "RoomId": ...,
    "MemberId": ...,
}

parent.update_room_membership(**kwargs)
```

1. See [:material-code-braces: UpdateRoomMembershipRequestTypeDef](./type_defs.md#updateroommembershiprequesttypedef) 

### update\_sip\_media\_application

Updates the details of the specified SIP media application.

Type annotations and code completion for `#!python session.create_client("chime").update_sip_media_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_sip_media_application.html)

```python
# update_sip_media_application method definition

await def update_sip_media_application(
    self,
    *,
    SipMediaApplicationId: str,
    Name: str = ...,
    Endpoints: Sequence[SipMediaApplicationEndpointTypeDef] = ...,  # (1)
) -> UpdateSipMediaApplicationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SipMediaApplicationEndpointTypeDef](./type_defs.md#sipmediaapplicationendpointtypedef) 
2. See [:material-code-braces: UpdateSipMediaApplicationResponseTypeDef](./type_defs.md#updatesipmediaapplicationresponsetypedef) 


```python
# update_sip_media_application method usage example with argument unpacking

kwargs: UpdateSipMediaApplicationRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.update_sip_media_application(**kwargs)
```

1. See [:material-code-braces: UpdateSipMediaApplicationRequestTypeDef](./type_defs.md#updatesipmediaapplicationrequesttypedef) 

### update\_sip\_media\_application\_call

Invokes the AWS Lambda function associated with the SIP media application and
transaction ID in an update request.

Type annotations and code completion for `#!python session.create_client("chime").update_sip_media_application_call` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_sip_media_application_call.html)

```python
# update_sip_media_application_call method definition

await def update_sip_media_application_call(
    self,
    *,
    SipMediaApplicationId: str,
    TransactionId: str,
    Arguments: Mapping[str, str],
) -> UpdateSipMediaApplicationCallResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSipMediaApplicationCallResponseTypeDef](./type_defs.md#updatesipmediaapplicationcallresponsetypedef) 


```python
# update_sip_media_application_call method usage example with argument unpacking

kwargs: UpdateSipMediaApplicationCallRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
    "TransactionId": ...,
    "Arguments": ...,
}

parent.update_sip_media_application_call(**kwargs)
```

1. See [:material-code-braces: UpdateSipMediaApplicationCallRequestTypeDef](./type_defs.md#updatesipmediaapplicationcallrequesttypedef) 

### update\_sip\_rule

Updates the details of the specified SIP rule.

Type annotations and code completion for `#!python session.create_client("chime").update_sip_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_sip_rule.html)

```python
# update_sip_rule method definition

await def update_sip_rule(
    self,
    *,
    SipRuleId: str,
    Name: str,
    Disabled: bool = ...,
    TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...,  # (1)
) -> UpdateSipRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SipRuleTargetApplicationTypeDef](./type_defs.md#sipruletargetapplicationtypedef) 
2. See [:material-code-braces: UpdateSipRuleResponseTypeDef](./type_defs.md#updatesipruleresponsetypedef) 


```python
# update_sip_rule method usage example with argument unpacking

kwargs: UpdateSipRuleRequestTypeDef = {  # (1)
    "SipRuleId": ...,
    "Name": ...,
}

parent.update_sip_rule(**kwargs)
```

1. See [:material-code-braces: UpdateSipRuleRequestTypeDef](./type_defs.md#updatesiprulerequesttypedef) 

### update\_user

Updates user details for a specified user ID.

Type annotations and code completion for `#!python session.create_client("chime").update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_user.html)

```python
# update_user method definition

await def update_user(
    self,
    *,
    AccountId: str,
    UserId: str,
    LicenseType: LicenseType = ...,  # (1)
    UserType: UserTypeType = ...,  # (2)
    AlexaForBusinessMetadata: AlexaForBusinessMetadataTypeDef = ...,  # (3)
) -> UpdateUserResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: LicenseType](./literals.md#licensetype) 
2. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
3. See [:material-code-braces: AlexaForBusinessMetadataTypeDef](./type_defs.md#alexaforbusinessmetadatatypedef) 
4. See [:material-code-braces: UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef) 


```python
# update_user method usage example with argument unpacking

kwargs: UpdateUserRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserId": ...,
}

parent.update_user(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestTypeDef](./type_defs.md#updateuserrequesttypedef) 

### update\_user\_settings

Updates the settings for the specified user, such as phone number settings.

Type annotations and code completion for `#!python session.create_client("chime").update_user_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_user_settings.html)

```python
# update_user_settings method definition

await def update_user_settings(
    self,
    *,
    AccountId: str,
    UserId: str,
    UserSettings: UserSettingsTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user_settings method usage example with argument unpacking

kwargs: UpdateUserSettingsRequestTypeDef = {  # (1)
    "AccountId": ...,
    "UserId": ...,
    "UserSettings": ...,
}

parent.update_user_settings(**kwargs)
```

1. See [:material-code-braces: UpdateUserSettingsRequestTypeDef](./type_defs.md#updateusersettingsrequesttypedef) 

### update\_voice\_connector

Updates details for the specified Amazon Chime Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime").update_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_voice_connector.html)

```python
# update_voice_connector method definition

await def update_voice_connector(
    self,
    *,
    VoiceConnectorId: str,
    Name: str,
    RequireEncryption: bool,
) -> UpdateVoiceConnectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateVoiceConnectorResponseTypeDef](./type_defs.md#updatevoiceconnectorresponsetypedef) 


```python
# update_voice_connector method usage example with argument unpacking

kwargs: UpdateVoiceConnectorRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "Name": ...,
    "RequireEncryption": ...,
}

parent.update_voice_connector(**kwargs)
```

1. See [:material-code-braces: UpdateVoiceConnectorRequestTypeDef](./type_defs.md#updatevoiceconnectorrequesttypedef) 

### update\_voice\_connector\_group

Updates details of the specified Amazon Chime Voice Connector group, such as
the name and Amazon Chime Voice Connector priority ranking.

Type annotations and code completion for `#!python session.create_client("chime").update_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/update_voice_connector_group.html)

```python
# update_voice_connector_group method definition

await def update_voice_connector_group(
    self,
    *,
    VoiceConnectorGroupId: str,
    Name: str,
    VoiceConnectorItems: Sequence[VoiceConnectorItemTypeDef],  # (1)
) -> UpdateVoiceConnectorGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VoiceConnectorItemTypeDef](./type_defs.md#voiceconnectoritemtypedef) 
2. See [:material-code-braces: UpdateVoiceConnectorGroupResponseTypeDef](./type_defs.md#updatevoiceconnectorgroupresponsetypedef) 


```python
# update_voice_connector_group method usage example with argument unpacking

kwargs: UpdateVoiceConnectorGroupRequestTypeDef = {  # (1)
    "VoiceConnectorGroupId": ...,
    "Name": ...,
    "VoiceConnectorItems": ...,
}

parent.update_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: UpdateVoiceConnectorGroupRequestTypeDef](./type_defs.md#updatevoiceconnectorgrouprequesttypedef) 

### validate\_e911\_address

Validates an address to be used for 911 calls made with Amazon Chime Voice
Connectors.

Type annotations and code completion for `#!python session.create_client("chime").validate_e911_address` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime/client/validate_e911_address.html)

```python
# validate_e911_address method definition

await def validate_e911_address(
    self,
    *,
    AwsAccountId: str,
    StreetNumber: str,
    StreetInfo: str,
    City: str,
    State: str,
    Country: str,
    PostalCode: str,
) -> ValidateE911AddressResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ValidateE911AddressResponseTypeDef](./type_defs.md#validatee911addressresponsetypedef) 


```python
# validate_e911_address method usage example with argument unpacking

kwargs: ValidateE911AddressRequestTypeDef = {  # (1)
    "AwsAccountId": ...,
    "StreetNumber": ...,
    "StreetInfo": ...,
    "City": ...,
    "State": ...,
    "Country": ...,
    "PostalCode": ...,
}

parent.validate_e911_address(**kwargs)
```

1. See [:material-code-braces: ValidateE911AddressRequestTypeDef](./type_defs.md#validatee911addressrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("chime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("chime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client)

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

Type annotations and code completion for `#!python session.create_client("chime").get_paginator` method with overloads.

- `client.get_paginator("list_accounts")` -> [ListAccountsPaginator](./paginators.md#listaccountspaginator)
- `client.get_paginator("list_users")` -> [ListUsersPaginator](./paginators.md#listuserspaginator)



