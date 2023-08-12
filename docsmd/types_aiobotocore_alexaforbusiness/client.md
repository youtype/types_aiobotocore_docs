# AlexaForBusinessClient

> [Index](../README.md) > [AlexaForBusiness](./README.md) > AlexaForBusinessClient

!!! note ""

    Auto-generated documentation for [AlexaForBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
    type annotations stubs module [types-aiobotocore-alexaforbusiness](https://pypi.org/project/types-aiobotocore-alexaforbusiness/).

## AlexaForBusinessClient

Type annotations and code completion for `#!python session.create_client("alexaforbusiness")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client)

```python
AlexaForBusinessClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_alexaforbusiness.client import AlexaForBusinessClient

session = get_session()
async with session.create_client("alexaforbusiness") as client:
    client: AlexaForBusinessClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("alexaforbusiness").exceptions` structure.

```python
AlexaForBusinessClient.exceptions usage example

async with session.create_client("alexaforbusiness") as client:
    try:
        do_something(client)
    except (
            client.AlreadyExistsException,
        client.ClientError,
        client.ConcurrentModificationException,
        client.DeviceNotRegisteredException,
        client.InvalidCertificateAuthorityException,
        client.InvalidDeviceException,
        client.InvalidSecretsManagerResourceException,
        client.InvalidServiceLinkedRoleStateException,
        client.InvalidUserStatusException,
        client.LimitExceededException,
        client.NameInUseException,
        client.NotFoundException,
        client.ResourceAssociatedException,
        client.ResourceInUseException,
        client.SkillNotLinkedException,
        client.UnauthorizedException,
    ) as e:
        print(e)
```

```python
AlexaForBusinessClient usage type checking example

from types_aiobotocore_alexaforbusiness.client import Exceptions

def handle_error(exc: Exceptions.AlreadyExistsException) -> None:
    ...
```


## Methods


### approve\_skill

Associates a skill with the organization under the customer's AWS account.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").approve_skill` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.approve_skill)

```python
# approve_skill method definition

await def approve_skill(
    self,
    *,
    SkillId: str,
) -> Dict[str, Any]:
    ...
```



```python
# approve_skill method usage example with argument unpacking

kwargs: ApproveSkillRequestRequestTypeDef = {  # (1)
    "SkillId": ...,
}

parent.approve_skill(**kwargs)
```

1. See [:material-code-braces: ApproveSkillRequestRequestTypeDef](./type_defs.md#approveskillrequestrequesttypedef) 

### associate\_contact\_with\_address\_book

Associates a contact with a given address book.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").associate_contact_with_address_book` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.associate_contact_with_address_book)

```python
# associate_contact_with_address_book method definition

await def associate_contact_with_address_book(
    self,
    *,
    ContactArn: str,
    AddressBookArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_contact_with_address_book method usage example with argument unpacking

kwargs: AssociateContactWithAddressBookRequestRequestTypeDef = {  # (1)
    "ContactArn": ...,
    "AddressBookArn": ...,
}

parent.associate_contact_with_address_book(**kwargs)
```

1. See [:material-code-braces: AssociateContactWithAddressBookRequestRequestTypeDef](./type_defs.md#associatecontactwithaddressbookrequestrequesttypedef) 

### associate\_device\_with\_network\_profile

Associates a device with the specified network profile.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").associate_device_with_network_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.associate_device_with_network_profile)

```python
# associate_device_with_network_profile method definition

await def associate_device_with_network_profile(
    self,
    *,
    DeviceArn: str,
    NetworkProfileArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_device_with_network_profile method usage example with argument unpacking

kwargs: AssociateDeviceWithNetworkProfileRequestRequestTypeDef = {  # (1)
    "DeviceArn": ...,
    "NetworkProfileArn": ...,
}

parent.associate_device_with_network_profile(**kwargs)
```

1. See [:material-code-braces: AssociateDeviceWithNetworkProfileRequestRequestTypeDef](./type_defs.md#associatedevicewithnetworkprofilerequestrequesttypedef) 

### associate\_device\_with\_room

Associates a device with a given room.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").associate_device_with_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.associate_device_with_room)

```python
# associate_device_with_room method definition

await def associate_device_with_room(
    self,
    *,
    DeviceArn: str = ...,
    RoomArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# associate_device_with_room method usage example with argument unpacking

kwargs: AssociateDeviceWithRoomRequestRequestTypeDef = {  # (1)
    "DeviceArn": ...,
}

parent.associate_device_with_room(**kwargs)
```

1. See [:material-code-braces: AssociateDeviceWithRoomRequestRequestTypeDef](./type_defs.md#associatedevicewithroomrequestrequesttypedef) 

### associate\_skill\_group\_with\_room

Associates a skill group with a given room.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").associate_skill_group_with_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.associate_skill_group_with_room)

```python
# associate_skill_group_with_room method definition

await def associate_skill_group_with_room(
    self,
    *,
    SkillGroupArn: str = ...,
    RoomArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# associate_skill_group_with_room method usage example with argument unpacking

kwargs: AssociateSkillGroupWithRoomRequestRequestTypeDef = {  # (1)
    "SkillGroupArn": ...,
}

parent.associate_skill_group_with_room(**kwargs)
```

1. See [:material-code-braces: AssociateSkillGroupWithRoomRequestRequestTypeDef](./type_defs.md#associateskillgroupwithroomrequestrequesttypedef) 

### associate\_skill\_with\_skill\_group

Associates a skill with a skill group.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").associate_skill_with_skill_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.associate_skill_with_skill_group)

```python
# associate_skill_with_skill_group method definition

await def associate_skill_with_skill_group(
    self,
    *,
    SkillId: str,
    SkillGroupArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# associate_skill_with_skill_group method usage example with argument unpacking

kwargs: AssociateSkillWithSkillGroupRequestRequestTypeDef = {  # (1)
    "SkillId": ...,
}

parent.associate_skill_with_skill_group(**kwargs)
```

1. See [:material-code-braces: AssociateSkillWithSkillGroupRequestRequestTypeDef](./type_defs.md#associateskillwithskillgrouprequestrequesttypedef) 

### associate\_skill\_with\_users

Makes a private skill available for enrolled users to enable on their devices.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").associate_skill_with_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.associate_skill_with_users)

```python
# associate_skill_with_users method definition

await def associate_skill_with_users(
    self,
    *,
    SkillId: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_skill_with_users method usage example with argument unpacking

kwargs: AssociateSkillWithUsersRequestRequestTypeDef = {  # (1)
    "SkillId": ...,
}

parent.associate_skill_with_users(**kwargs)
```

1. See [:material-code-braces: AssociateSkillWithUsersRequestRequestTypeDef](./type_defs.md#associateskillwithusersrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_address\_book

Creates an address book with the specified details.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").create_address_book` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_address_book)

```python
# create_address_book method definition

await def create_address_book(
    self,
    *,
    Name: str,
    Description: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateAddressBookResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateAddressBookResponseTypeDef](./type_defs.md#createaddressbookresponsetypedef) 


```python
# create_address_book method usage example with argument unpacking

kwargs: CreateAddressBookRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_address_book(**kwargs)
```

1. See [:material-code-braces: CreateAddressBookRequestRequestTypeDef](./type_defs.md#createaddressbookrequestrequesttypedef) 

### create\_business\_report\_schedule

Creates a recurring schedule for usage reports to deliver to the specified S3
location with a specified daily or weekly interval.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").create_business_report_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_business_report_schedule)

```python
# create_business_report_schedule method definition

await def create_business_report_schedule(
    self,
    *,
    Format: BusinessReportFormatType,  # (1)
    ContentRange: BusinessReportContentRangeTypeDef,  # (2)
    ScheduleName: str = ...,
    S3BucketName: str = ...,
    S3KeyPrefix: str = ...,
    Recurrence: BusinessReportRecurrenceTypeDef = ...,  # (3)
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateBusinessReportScheduleResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: BusinessReportFormatType](./literals.md#businessreportformattype) 
2. See [:material-code-braces: BusinessReportContentRangeTypeDef](./type_defs.md#businessreportcontentrangetypedef) 
3. See [:material-code-braces: BusinessReportRecurrenceTypeDef](./type_defs.md#businessreportrecurrencetypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateBusinessReportScheduleResponseTypeDef](./type_defs.md#createbusinessreportscheduleresponsetypedef) 


```python
# create_business_report_schedule method usage example with argument unpacking

kwargs: CreateBusinessReportScheduleRequestRequestTypeDef = {  # (1)
    "Format": ...,
    "ContentRange": ...,
}

parent.create_business_report_schedule(**kwargs)
```

1. See [:material-code-braces: CreateBusinessReportScheduleRequestRequestTypeDef](./type_defs.md#createbusinessreportschedulerequestrequesttypedef) 

### create\_conference\_provider

Adds a new conference provider under the user's AWS account.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").create_conference_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_conference_provider)

```python
# create_conference_provider method definition

await def create_conference_provider(
    self,
    *,
    ConferenceProviderName: str,
    ConferenceProviderType: ConferenceProviderTypeType,  # (1)
    MeetingSetting: MeetingSettingTypeDef,  # (2)
    IPDialIn: IPDialInTypeDef = ...,  # (3)
    PSTNDialIn: PSTNDialInTypeDef = ...,  # (4)
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreateConferenceProviderResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ConferenceProviderTypeType](./literals.md#conferenceprovidertypetype) 
2. See [:material-code-braces: MeetingSettingTypeDef](./type_defs.md#meetingsettingtypedef) 
3. See [:material-code-braces: IPDialInTypeDef](./type_defs.md#ipdialintypedef) 
4. See [:material-code-braces: PSTNDialInTypeDef](./type_defs.md#pstndialintypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateConferenceProviderResponseTypeDef](./type_defs.md#createconferenceproviderresponsetypedef) 


```python
# create_conference_provider method usage example with argument unpacking

kwargs: CreateConferenceProviderRequestRequestTypeDef = {  # (1)
    "ConferenceProviderName": ...,
    "ConferenceProviderType": ...,
    "MeetingSetting": ...,
}

parent.create_conference_provider(**kwargs)
```

1. See [:material-code-braces: CreateConferenceProviderRequestRequestTypeDef](./type_defs.md#createconferenceproviderrequestrequesttypedef) 

### create\_contact

Creates a contact with the specified details.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").create_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_contact)

```python
# create_contact method definition

await def create_contact(
    self,
    *,
    FirstName: str,
    DisplayName: str = ...,
    LastName: str = ...,
    PhoneNumber: str = ...,
    PhoneNumbers: Sequence[PhoneNumberTypeDef] = ...,  # (1)
    SipAddresses: Sequence[SipAddressTypeDef] = ...,  # (2)
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateContactResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: SipAddressTypeDef](./type_defs.md#sipaddresstypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateContactResponseTypeDef](./type_defs.md#createcontactresponsetypedef) 


```python
# create_contact method usage example with argument unpacking

kwargs: CreateContactRequestRequestTypeDef = {  # (1)
    "FirstName": ...,
}

parent.create_contact(**kwargs)
```

1. See [:material-code-braces: CreateContactRequestRequestTypeDef](./type_defs.md#createcontactrequestrequesttypedef) 

### create\_gateway\_group

Creates a gateway group with the specified details.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").create_gateway_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_gateway_group)

```python
# create_gateway_group method definition

await def create_gateway_group(
    self,
    *,
    Name: str,
    ClientRequestToken: str,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateGatewayGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateGatewayGroupResponseTypeDef](./type_defs.md#creategatewaygroupresponsetypedef) 


```python
# create_gateway_group method usage example with argument unpacking

kwargs: CreateGatewayGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ClientRequestToken": ...,
}

parent.create_gateway_group(**kwargs)
```

1. See [:material-code-braces: CreateGatewayGroupRequestRequestTypeDef](./type_defs.md#creategatewaygrouprequestrequesttypedef) 

### create\_network\_profile

Creates a network profile with the specified details.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").create_network_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_network_profile)

```python
# create_network_profile method definition

await def create_network_profile(
    self,
    *,
    NetworkProfileName: str,
    Ssid: str,
    SecurityType: NetworkSecurityTypeType,  # (1)
    ClientRequestToken: str,
    Description: str = ...,
    EapMethod: NetworkEapMethodType = ...,  # (2)
    CurrentPassword: str = ...,
    NextPassword: str = ...,
    CertificateAuthorityArn: str = ...,
    TrustAnchors: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateNetworkProfileResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: NetworkSecurityTypeType](./literals.md#networksecuritytypetype) 
2. See [:material-code-brackets: NetworkEapMethodType](./literals.md#networkeapmethodtype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateNetworkProfileResponseTypeDef](./type_defs.md#createnetworkprofileresponsetypedef) 


```python
# create_network_profile method usage example with argument unpacking

kwargs: CreateNetworkProfileRequestRequestTypeDef = {  # (1)
    "NetworkProfileName": ...,
    "Ssid": ...,
    "SecurityType": ...,
    "ClientRequestToken": ...,
}

parent.create_network_profile(**kwargs)
```

1. See [:material-code-braces: CreateNetworkProfileRequestRequestTypeDef](./type_defs.md#createnetworkprofilerequestrequesttypedef) 

### create\_profile

Creates a new room profile with the specified details.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").create_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_profile)

```python
# create_profile method definition

await def create_profile(
    self,
    *,
    ProfileName: str,
    Timezone: str,
    Address: str,
    DistanceUnit: DistanceUnitType,  # (1)
    TemperatureUnit: TemperatureUnitType,  # (2)
    WakeWord: WakeWordType,  # (3)
    Locale: str = ...,
    ClientRequestToken: str = ...,
    SetupModeDisabled: bool = ...,
    MaxVolumeLimit: int = ...,
    PSTNEnabled: bool = ...,
    DataRetentionOptIn: bool = ...,
    MeetingRoomConfiguration: CreateMeetingRoomConfigurationTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreateProfileResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
2. See [:material-code-brackets: TemperatureUnitType](./literals.md#temperatureunittype) 
3. See [:material-code-brackets: WakeWordType](./literals.md#wakewordtype) 
4. See [:material-code-braces: CreateMeetingRoomConfigurationTypeDef](./type_defs.md#createmeetingroomconfigurationtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateProfileResponseTypeDef](./type_defs.md#createprofileresponsetypedef) 


```python
# create_profile method usage example with argument unpacking

kwargs: CreateProfileRequestRequestTypeDef = {  # (1)
    "ProfileName": ...,
    "Timezone": ...,
    "Address": ...,
    "DistanceUnit": ...,
    "TemperatureUnit": ...,
    "WakeWord": ...,
}

parent.create_profile(**kwargs)
```

1. See [:material-code-braces: CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef) 

### create\_room

Creates a room with the specified details.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").create_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_room)

```python
# create_room method definition

await def create_room(
    self,
    *,
    RoomName: str,
    Description: str = ...,
    ProfileArn: str = ...,
    ProviderCalendarId: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateRoomResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateRoomResponseTypeDef](./type_defs.md#createroomresponsetypedef) 


```python
# create_room method usage example with argument unpacking

kwargs: CreateRoomRequestRequestTypeDef = {  # (1)
    "RoomName": ...,
}

parent.create_room(**kwargs)
```

1. See [:material-code-braces: CreateRoomRequestRequestTypeDef](./type_defs.md#createroomrequestrequesttypedef) 

### create\_skill\_group

Creates a skill group with a specified name and description.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").create_skill_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_skill_group)

```python
# create_skill_group method definition

await def create_skill_group(
    self,
    *,
    SkillGroupName: str,
    Description: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateSkillGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateSkillGroupResponseTypeDef](./type_defs.md#createskillgroupresponsetypedef) 


```python
# create_skill_group method usage example with argument unpacking

kwargs: CreateSkillGroupRequestRequestTypeDef = {  # (1)
    "SkillGroupName": ...,
}

parent.create_skill_group(**kwargs)
```

1. See [:material-code-braces: CreateSkillGroupRequestRequestTypeDef](./type_defs.md#createskillgrouprequestrequesttypedef) 

### create\_user

Creates a user.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.create_user)

```python
# create_user method definition

await def create_user(
    self,
    *,
    UserId: str,
    FirstName: str = ...,
    LastName: str = ...,
    Email: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateUserResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestRequestTypeDef = {  # (1)
    "UserId": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef) 

### delete\_address\_book

Deletes an address book by the address book ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_address_book` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_address_book)

```python
# delete_address_book method definition

await def delete_address_book(
    self,
    *,
    AddressBookArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_address_book method usage example with argument unpacking

kwargs: DeleteAddressBookRequestRequestTypeDef = {  # (1)
    "AddressBookArn": ...,
}

parent.delete_address_book(**kwargs)
```

1. See [:material-code-braces: DeleteAddressBookRequestRequestTypeDef](./type_defs.md#deleteaddressbookrequestrequesttypedef) 

### delete\_business\_report\_schedule

Deletes the recurring report delivery schedule with the specified schedule ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_business_report_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_business_report_schedule)

```python
# delete_business_report_schedule method definition

await def delete_business_report_schedule(
    self,
    *,
    ScheduleArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_business_report_schedule method usage example with argument unpacking

kwargs: DeleteBusinessReportScheduleRequestRequestTypeDef = {  # (1)
    "ScheduleArn": ...,
}

parent.delete_business_report_schedule(**kwargs)
```

1. See [:material-code-braces: DeleteBusinessReportScheduleRequestRequestTypeDef](./type_defs.md#deletebusinessreportschedulerequestrequesttypedef) 

### delete\_conference\_provider

Deletes a conference provider.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_conference_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_conference_provider)

```python
# delete_conference_provider method definition

await def delete_conference_provider(
    self,
    *,
    ConferenceProviderArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_conference_provider method usage example with argument unpacking

kwargs: DeleteConferenceProviderRequestRequestTypeDef = {  # (1)
    "ConferenceProviderArn": ...,
}

parent.delete_conference_provider(**kwargs)
```

1. See [:material-code-braces: DeleteConferenceProviderRequestRequestTypeDef](./type_defs.md#deleteconferenceproviderrequestrequesttypedef) 

### delete\_contact

Deletes a contact by the contact ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_contact)

```python
# delete_contact method definition

await def delete_contact(
    self,
    *,
    ContactArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_contact method usage example with argument unpacking

kwargs: DeleteContactRequestRequestTypeDef = {  # (1)
    "ContactArn": ...,
}

parent.delete_contact(**kwargs)
```

1. See [:material-code-braces: DeleteContactRequestRequestTypeDef](./type_defs.md#deletecontactrequestrequesttypedef) 

### delete\_device

Removes a device from Alexa For Business.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_device)

```python
# delete_device method definition

await def delete_device(
    self,
    *,
    DeviceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_device method usage example with argument unpacking

kwargs: DeleteDeviceRequestRequestTypeDef = {  # (1)
    "DeviceArn": ...,
}

parent.delete_device(**kwargs)
```

1. See [:material-code-braces: DeleteDeviceRequestRequestTypeDef](./type_defs.md#deletedevicerequestrequesttypedef) 

### delete\_device\_usage\_data

When this action is called for a specified shared device, it allows authorized
users to delete the device's entire previous history of voice input data and
associated response data.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_device_usage_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_device_usage_data)

```python
# delete_device_usage_data method definition

await def delete_device_usage_data(
    self,
    *,
    DeviceArn: str,
    DeviceUsageType: DeviceUsageTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: DeviceUsageTypeType](./literals.md#deviceusagetypetype) 


```python
# delete_device_usage_data method usage example with argument unpacking

kwargs: DeleteDeviceUsageDataRequestRequestTypeDef = {  # (1)
    "DeviceArn": ...,
    "DeviceUsageType": ...,
}

parent.delete_device_usage_data(**kwargs)
```

1. See [:material-code-braces: DeleteDeviceUsageDataRequestRequestTypeDef](./type_defs.md#deletedeviceusagedatarequestrequesttypedef) 

### delete\_gateway\_group

Deletes a gateway group.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_gateway_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_gateway_group)

```python
# delete_gateway_group method definition

await def delete_gateway_group(
    self,
    *,
    GatewayGroupArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_gateway_group method usage example with argument unpacking

kwargs: DeleteGatewayGroupRequestRequestTypeDef = {  # (1)
    "GatewayGroupArn": ...,
}

parent.delete_gateway_group(**kwargs)
```

1. See [:material-code-braces: DeleteGatewayGroupRequestRequestTypeDef](./type_defs.md#deletegatewaygrouprequestrequesttypedef) 

### delete\_network\_profile

Deletes a network profile by the network profile ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_network_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_network_profile)

```python
# delete_network_profile method definition

await def delete_network_profile(
    self,
    *,
    NetworkProfileArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_network_profile method usage example with argument unpacking

kwargs: DeleteNetworkProfileRequestRequestTypeDef = {  # (1)
    "NetworkProfileArn": ...,
}

parent.delete_network_profile(**kwargs)
```

1. See [:material-code-braces: DeleteNetworkProfileRequestRequestTypeDef](./type_defs.md#deletenetworkprofilerequestrequesttypedef) 

### delete\_profile

Deletes a room profile by the profile ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_profile)

```python
# delete_profile method definition

await def delete_profile(
    self,
    *,
    ProfileArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_profile method usage example with argument unpacking

kwargs: DeleteProfileRequestRequestTypeDef = {  # (1)
    "ProfileArn": ...,
}

parent.delete_profile(**kwargs)
```

1. See [:material-code-braces: DeleteProfileRequestRequestTypeDef](./type_defs.md#deleteprofilerequestrequesttypedef) 

### delete\_room

Deletes a room by the room ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_room)

```python
# delete_room method definition

await def delete_room(
    self,
    *,
    RoomArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_room method usage example with argument unpacking

kwargs: DeleteRoomRequestRequestTypeDef = {  # (1)
    "RoomArn": ...,
}

parent.delete_room(**kwargs)
```

1. See [:material-code-braces: DeleteRoomRequestRequestTypeDef](./type_defs.md#deleteroomrequestrequesttypedef) 

### delete\_room\_skill\_parameter

Deletes room skill parameter details by room, skill, and parameter key ID.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_room_skill_parameter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_room_skill_parameter)

```python
# delete_room_skill_parameter method definition

await def delete_room_skill_parameter(
    self,
    *,
    SkillId: str,
    ParameterKey: str,
    RoomArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_room_skill_parameter method usage example with argument unpacking

kwargs: DeleteRoomSkillParameterRequestRequestTypeDef = {  # (1)
    "SkillId": ...,
    "ParameterKey": ...,
}

parent.delete_room_skill_parameter(**kwargs)
```

1. See [:material-code-braces: DeleteRoomSkillParameterRequestRequestTypeDef](./type_defs.md#deleteroomskillparameterrequestrequesttypedef) 

### delete\_skill\_authorization

Unlinks a third-party account from a skill.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_skill_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_skill_authorization)

```python
# delete_skill_authorization method definition

await def delete_skill_authorization(
    self,
    *,
    SkillId: str,
    RoomArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_skill_authorization method usage example with argument unpacking

kwargs: DeleteSkillAuthorizationRequestRequestTypeDef = {  # (1)
    "SkillId": ...,
}

parent.delete_skill_authorization(**kwargs)
```

1. See [:material-code-braces: DeleteSkillAuthorizationRequestRequestTypeDef](./type_defs.md#deleteskillauthorizationrequestrequesttypedef) 

### delete\_skill\_group

Deletes a skill group by skill group ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_skill_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_skill_group)

```python
# delete_skill_group method definition

await def delete_skill_group(
    self,
    *,
    SkillGroupArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_skill_group method usage example with argument unpacking

kwargs: DeleteSkillGroupRequestRequestTypeDef = {  # (1)
    "SkillGroupArn": ...,
}

parent.delete_skill_group(**kwargs)
```

1. See [:material-code-braces: DeleteSkillGroupRequestRequestTypeDef](./type_defs.md#deleteskillgrouprequestrequesttypedef) 

### delete\_user

Deletes a specified user by user ARN and enrollment ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.delete_user)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    EnrollmentId: str,
    UserArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "EnrollmentId": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### disassociate\_contact\_from\_address\_book

Disassociates a contact from a given address book.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").disassociate_contact_from_address_book` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.disassociate_contact_from_address_book)

```python
# disassociate_contact_from_address_book method definition

await def disassociate_contact_from_address_book(
    self,
    *,
    ContactArn: str,
    AddressBookArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_contact_from_address_book method usage example with argument unpacking

kwargs: DisassociateContactFromAddressBookRequestRequestTypeDef = {  # (1)
    "ContactArn": ...,
    "AddressBookArn": ...,
}

parent.disassociate_contact_from_address_book(**kwargs)
```

1. See [:material-code-braces: DisassociateContactFromAddressBookRequestRequestTypeDef](./type_defs.md#disassociatecontactfromaddressbookrequestrequesttypedef) 

### disassociate\_device\_from\_room

Disassociates a device from its current room.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").disassociate_device_from_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.disassociate_device_from_room)

```python
# disassociate_device_from_room method definition

await def disassociate_device_from_room(
    self,
    *,
    DeviceArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_device_from_room method usage example with argument unpacking

kwargs: DisassociateDeviceFromRoomRequestRequestTypeDef = {  # (1)
    "DeviceArn": ...,
}

parent.disassociate_device_from_room(**kwargs)
```

1. See [:material-code-braces: DisassociateDeviceFromRoomRequestRequestTypeDef](./type_defs.md#disassociatedevicefromroomrequestrequesttypedef) 

### disassociate\_skill\_from\_skill\_group

Disassociates a skill from a skill group.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").disassociate_skill_from_skill_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.disassociate_skill_from_skill_group)

```python
# disassociate_skill_from_skill_group method definition

await def disassociate_skill_from_skill_group(
    self,
    *,
    SkillId: str,
    SkillGroupArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_skill_from_skill_group method usage example with argument unpacking

kwargs: DisassociateSkillFromSkillGroupRequestRequestTypeDef = {  # (1)
    "SkillId": ...,
}

parent.disassociate_skill_from_skill_group(**kwargs)
```

1. See [:material-code-braces: DisassociateSkillFromSkillGroupRequestRequestTypeDef](./type_defs.md#disassociateskillfromskillgrouprequestrequesttypedef) 

### disassociate\_skill\_from\_users

Makes a private skill unavailable for enrolled users and prevents them from
enabling it on their devices.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").disassociate_skill_from_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.disassociate_skill_from_users)

```python
# disassociate_skill_from_users method definition

await def disassociate_skill_from_users(
    self,
    *,
    SkillId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_skill_from_users method usage example with argument unpacking

kwargs: DisassociateSkillFromUsersRequestRequestTypeDef = {  # (1)
    "SkillId": ...,
}

parent.disassociate_skill_from_users(**kwargs)
```

1. See [:material-code-braces: DisassociateSkillFromUsersRequestRequestTypeDef](./type_defs.md#disassociateskillfromusersrequestrequesttypedef) 

### disassociate\_skill\_group\_from\_room

Disassociates a skill group from a specified room.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").disassociate_skill_group_from_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.disassociate_skill_group_from_room)

```python
# disassociate_skill_group_from_room method definition

await def disassociate_skill_group_from_room(
    self,
    *,
    SkillGroupArn: str = ...,
    RoomArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_skill_group_from_room method usage example with argument unpacking

kwargs: DisassociateSkillGroupFromRoomRequestRequestTypeDef = {  # (1)
    "SkillGroupArn": ...,
}

parent.disassociate_skill_group_from_room(**kwargs)
```

1. See [:material-code-braces: DisassociateSkillGroupFromRoomRequestRequestTypeDef](./type_defs.md#disassociateskillgroupfromroomrequestrequesttypedef) 

### forget\_smart\_home\_appliances

Forgets smart home appliances associated to a room.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").forget_smart_home_appliances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.forget_smart_home_appliances)

```python
# forget_smart_home_appliances method definition

await def forget_smart_home_appliances(
    self,
    *,
    RoomArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# forget_smart_home_appliances method usage example with argument unpacking

kwargs: ForgetSmartHomeAppliancesRequestRequestTypeDef = {  # (1)
    "RoomArn": ...,
}

parent.forget_smart_home_appliances(**kwargs)
```

1. See [:material-code-braces: ForgetSmartHomeAppliancesRequestRequestTypeDef](./type_defs.md#forgetsmarthomeappliancesrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.generate_presigned_url)

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


### get\_address\_book

Gets address the book details by the address book ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_address_book` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_address_book)

```python
# get_address_book method definition

await def get_address_book(
    self,
    *,
    AddressBookArn: str,
) -> GetAddressBookResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAddressBookResponseTypeDef](./type_defs.md#getaddressbookresponsetypedef) 


```python
# get_address_book method usage example with argument unpacking

kwargs: GetAddressBookRequestRequestTypeDef = {  # (1)
    "AddressBookArn": ...,
}

parent.get_address_book(**kwargs)
```

1. See [:material-code-braces: GetAddressBookRequestRequestTypeDef](./type_defs.md#getaddressbookrequestrequesttypedef) 

### get\_conference\_preference

Retrieves the existing conference preferences.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_conference_preference` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_conference_preference)

```python
# get_conference_preference method definition

await def get_conference_preference(
    self,
) -> GetConferencePreferenceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConferencePreferenceResponseTypeDef](./type_defs.md#getconferencepreferenceresponsetypedef) 

### get\_conference\_provider

Gets details about a specific conference provider.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_conference_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_conference_provider)

```python
# get_conference_provider method definition

await def get_conference_provider(
    self,
    *,
    ConferenceProviderArn: str,
) -> GetConferenceProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConferenceProviderResponseTypeDef](./type_defs.md#getconferenceproviderresponsetypedef) 


```python
# get_conference_provider method usage example with argument unpacking

kwargs: GetConferenceProviderRequestRequestTypeDef = {  # (1)
    "ConferenceProviderArn": ...,
}

parent.get_conference_provider(**kwargs)
```

1. See [:material-code-braces: GetConferenceProviderRequestRequestTypeDef](./type_defs.md#getconferenceproviderrequestrequesttypedef) 

### get\_contact

Gets the contact details by the contact ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_contact)

```python
# get_contact method definition

await def get_contact(
    self,
    *,
    ContactArn: str,
) -> GetContactResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContactResponseTypeDef](./type_defs.md#getcontactresponsetypedef) 


```python
# get_contact method usage example with argument unpacking

kwargs: GetContactRequestRequestTypeDef = {  # (1)
    "ContactArn": ...,
}

parent.get_contact(**kwargs)
```

1. See [:material-code-braces: GetContactRequestRequestTypeDef](./type_defs.md#getcontactrequestrequesttypedef) 

### get\_device

Gets the details of a device by device ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_device)

```python
# get_device method definition

await def get_device(
    self,
    *,
    DeviceArn: str = ...,
) -> GetDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceResponseTypeDef](./type_defs.md#getdeviceresponsetypedef) 


```python
# get_device method usage example with argument unpacking

kwargs: GetDeviceRequestRequestTypeDef = {  # (1)
    "DeviceArn": ...,
}

parent.get_device(**kwargs)
```

1. See [:material-code-braces: GetDeviceRequestRequestTypeDef](./type_defs.md#getdevicerequestrequesttypedef) 

### get\_gateway

Retrieves the details of a gateway.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_gateway)

```python
# get_gateway method definition

await def get_gateway(
    self,
    *,
    GatewayArn: str,
) -> GetGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGatewayResponseTypeDef](./type_defs.md#getgatewayresponsetypedef) 


```python
# get_gateway method usage example with argument unpacking

kwargs: GetGatewayRequestRequestTypeDef = {  # (1)
    "GatewayArn": ...,
}

parent.get_gateway(**kwargs)
```

1. See [:material-code-braces: GetGatewayRequestRequestTypeDef](./type_defs.md#getgatewayrequestrequesttypedef) 

### get\_gateway\_group

Retrieves the details of a gateway group.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_gateway_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_gateway_group)

```python
# get_gateway_group method definition

await def get_gateway_group(
    self,
    *,
    GatewayGroupArn: str,
) -> GetGatewayGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGatewayGroupResponseTypeDef](./type_defs.md#getgatewaygroupresponsetypedef) 


```python
# get_gateway_group method usage example with argument unpacking

kwargs: GetGatewayGroupRequestRequestTypeDef = {  # (1)
    "GatewayGroupArn": ...,
}

parent.get_gateway_group(**kwargs)
```

1. See [:material-code-braces: GetGatewayGroupRequestRequestTypeDef](./type_defs.md#getgatewaygrouprequestrequesttypedef) 

### get\_invitation\_configuration

Retrieves the configured values for the user enrollment invitation email
template.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_invitation_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_invitation_configuration)

```python
# get_invitation_configuration method definition

await def get_invitation_configuration(
    self,
) -> GetInvitationConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInvitationConfigurationResponseTypeDef](./type_defs.md#getinvitationconfigurationresponsetypedef) 

### get\_network\_profile

Gets the network profile details by the network profile ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_network_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_network_profile)

```python
# get_network_profile method definition

await def get_network_profile(
    self,
    *,
    NetworkProfileArn: str,
) -> GetNetworkProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNetworkProfileResponseTypeDef](./type_defs.md#getnetworkprofileresponsetypedef) 


```python
# get_network_profile method usage example with argument unpacking

kwargs: GetNetworkProfileRequestRequestTypeDef = {  # (1)
    "NetworkProfileArn": ...,
}

parent.get_network_profile(**kwargs)
```

1. See [:material-code-braces: GetNetworkProfileRequestRequestTypeDef](./type_defs.md#getnetworkprofilerequestrequesttypedef) 

### get\_profile

Gets the details of a room profile by profile ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_profile)

```python
# get_profile method definition

await def get_profile(
    self,
    *,
    ProfileArn: str = ...,
) -> GetProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProfileResponseTypeDef](./type_defs.md#getprofileresponsetypedef) 


```python
# get_profile method usage example with argument unpacking

kwargs: GetProfileRequestRequestTypeDef = {  # (1)
    "ProfileArn": ...,
}

parent.get_profile(**kwargs)
```

1. See [:material-code-braces: GetProfileRequestRequestTypeDef](./type_defs.md#getprofilerequestrequesttypedef) 

### get\_room

Gets room details by room ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_room)

```python
# get_room method definition

await def get_room(
    self,
    *,
    RoomArn: str = ...,
) -> GetRoomResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRoomResponseTypeDef](./type_defs.md#getroomresponsetypedef) 


```python
# get_room method usage example with argument unpacking

kwargs: GetRoomRequestRequestTypeDef = {  # (1)
    "RoomArn": ...,
}

parent.get_room(**kwargs)
```

1. See [:material-code-braces: GetRoomRequestRequestTypeDef](./type_defs.md#getroomrequestrequesttypedef) 

### get\_room\_skill\_parameter

Gets room skill parameter details by room, skill, and parameter key ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_room_skill_parameter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_room_skill_parameter)

```python
# get_room_skill_parameter method definition

await def get_room_skill_parameter(
    self,
    *,
    SkillId: str,
    ParameterKey: str,
    RoomArn: str = ...,
) -> GetRoomSkillParameterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRoomSkillParameterResponseTypeDef](./type_defs.md#getroomskillparameterresponsetypedef) 


```python
# get_room_skill_parameter method usage example with argument unpacking

kwargs: GetRoomSkillParameterRequestRequestTypeDef = {  # (1)
    "SkillId": ...,
    "ParameterKey": ...,
}

parent.get_room_skill_parameter(**kwargs)
```

1. See [:material-code-braces: GetRoomSkillParameterRequestRequestTypeDef](./type_defs.md#getroomskillparameterrequestrequesttypedef) 

### get\_skill\_group

Gets skill group details by skill group ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_skill_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.get_skill_group)

```python
# get_skill_group method definition

await def get_skill_group(
    self,
    *,
    SkillGroupArn: str = ...,
) -> GetSkillGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSkillGroupResponseTypeDef](./type_defs.md#getskillgroupresponsetypedef) 


```python
# get_skill_group method usage example with argument unpacking

kwargs: GetSkillGroupRequestRequestTypeDef = {  # (1)
    "SkillGroupArn": ...,
}

parent.get_skill_group(**kwargs)
```

1. See [:material-code-braces: GetSkillGroupRequestRequestTypeDef](./type_defs.md#getskillgrouprequestrequesttypedef) 

### list\_business\_report\_schedules

Lists the details of the schedules that a user configured.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").list_business_report_schedules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_business_report_schedules)

```python
# list_business_report_schedules method definition

await def list_business_report_schedules(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListBusinessReportSchedulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBusinessReportSchedulesResponseTypeDef](./type_defs.md#listbusinessreportschedulesresponsetypedef) 


```python
# list_business_report_schedules method usage example with argument unpacking

kwargs: ListBusinessReportSchedulesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_business_report_schedules(**kwargs)
```

1. See [:material-code-braces: ListBusinessReportSchedulesRequestRequestTypeDef](./type_defs.md#listbusinessreportschedulesrequestrequesttypedef) 

### list\_conference\_providers

Lists conference providers under a specific AWS account.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").list_conference_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_conference_providers)

```python
# list_conference_providers method definition

await def list_conference_providers(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListConferenceProvidersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConferenceProvidersResponseTypeDef](./type_defs.md#listconferenceprovidersresponsetypedef) 


```python
# list_conference_providers method usage example with argument unpacking

kwargs: ListConferenceProvidersRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_conference_providers(**kwargs)
```

1. See [:material-code-braces: ListConferenceProvidersRequestRequestTypeDef](./type_defs.md#listconferenceprovidersrequestrequesttypedef) 

### list\_device\_events

Lists the device event history, including device connection status, for up to 30
days.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").list_device_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_device_events)

```python
# list_device_events method definition

await def list_device_events(
    self,
    *,
    DeviceArn: str,
    EventType: DeviceEventTypeType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDeviceEventsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeviceEventTypeType](./literals.md#deviceeventtypetype) 
2. See [:material-code-braces: ListDeviceEventsResponseTypeDef](./type_defs.md#listdeviceeventsresponsetypedef) 


```python
# list_device_events method usage example with argument unpacking

kwargs: ListDeviceEventsRequestRequestTypeDef = {  # (1)
    "DeviceArn": ...,
}

parent.list_device_events(**kwargs)
```

1. See [:material-code-braces: ListDeviceEventsRequestRequestTypeDef](./type_defs.md#listdeviceeventsrequestrequesttypedef) 

### list\_gateway\_groups

Retrieves a list of gateway group summaries.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").list_gateway_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_gateway_groups)

```python
# list_gateway_groups method definition

await def list_gateway_groups(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListGatewayGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGatewayGroupsResponseTypeDef](./type_defs.md#listgatewaygroupsresponsetypedef) 


```python
# list_gateway_groups method usage example with argument unpacking

kwargs: ListGatewayGroupsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_gateway_groups(**kwargs)
```

1. See [:material-code-braces: ListGatewayGroupsRequestRequestTypeDef](./type_defs.md#listgatewaygroupsrequestrequesttypedef) 

### list\_gateways

Retrieves a list of gateway summaries.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").list_gateways` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_gateways)

```python
# list_gateways method definition

await def list_gateways(
    self,
    *,
    GatewayGroupArn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListGatewaysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef) 


```python
# list_gateways method usage example with argument unpacking

kwargs: ListGatewaysRequestRequestTypeDef = {  # (1)
    "GatewayGroupArn": ...,
}

parent.list_gateways(**kwargs)
```

1. See [:material-code-braces: ListGatewaysRequestRequestTypeDef](./type_defs.md#listgatewaysrequestrequesttypedef) 

### list\_skills

Lists all enabled skills in a specific skill group.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").list_skills` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_skills)

```python
# list_skills method definition

await def list_skills(
    self,
    *,
    SkillGroupArn: str = ...,
    EnablementType: EnablementTypeFilterType = ...,  # (1)
    SkillType: SkillTypeFilterType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSkillsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EnablementTypeFilterType](./literals.md#enablementtypefiltertype) 
2. See [:material-code-brackets: SkillTypeFilterType](./literals.md#skilltypefiltertype) 
3. See [:material-code-braces: ListSkillsResponseTypeDef](./type_defs.md#listskillsresponsetypedef) 


```python
# list_skills method usage example with argument unpacking

kwargs: ListSkillsRequestRequestTypeDef = {  # (1)
    "SkillGroupArn": ...,
}

parent.list_skills(**kwargs)
```

1. See [:material-code-braces: ListSkillsRequestRequestTypeDef](./type_defs.md#listskillsrequestrequesttypedef) 

### list\_skills\_store\_categories

Lists all categories in the Alexa skill store.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").list_skills_store_categories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_skills_store_categories)

```python
# list_skills_store_categories method definition

await def list_skills_store_categories(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSkillsStoreCategoriesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSkillsStoreCategoriesResponseTypeDef](./type_defs.md#listskillsstorecategoriesresponsetypedef) 


```python
# list_skills_store_categories method usage example with argument unpacking

kwargs: ListSkillsStoreCategoriesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_skills_store_categories(**kwargs)
```

1. See [:material-code-braces: ListSkillsStoreCategoriesRequestRequestTypeDef](./type_defs.md#listskillsstorecategoriesrequestrequesttypedef) 

### list\_skills\_store\_skills\_by\_category

Lists all skills in the Alexa skill store by category.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").list_skills_store_skills_by_category` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_skills_store_skills_by_category)

```python
# list_skills_store_skills_by_category method definition

await def list_skills_store_skills_by_category(
    self,
    *,
    CategoryId: int,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSkillsStoreSkillsByCategoryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSkillsStoreSkillsByCategoryResponseTypeDef](./type_defs.md#listskillsstoreskillsbycategoryresponsetypedef) 


```python
# list_skills_store_skills_by_category method usage example with argument unpacking

kwargs: ListSkillsStoreSkillsByCategoryRequestRequestTypeDef = {  # (1)
    "CategoryId": ...,
}

parent.list_skills_store_skills_by_category(**kwargs)
```

1. See [:material-code-braces: ListSkillsStoreSkillsByCategoryRequestRequestTypeDef](./type_defs.md#listskillsstoreskillsbycategoryrequestrequesttypedef) 

### list\_smart\_home\_appliances

Lists all of the smart home appliances associated with a room.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").list_smart_home_appliances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_smart_home_appliances)

```python
# list_smart_home_appliances method definition

await def list_smart_home_appliances(
    self,
    *,
    RoomArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSmartHomeAppliancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSmartHomeAppliancesResponseTypeDef](./type_defs.md#listsmarthomeappliancesresponsetypedef) 


```python
# list_smart_home_appliances method usage example with argument unpacking

kwargs: ListSmartHomeAppliancesRequestRequestTypeDef = {  # (1)
    "RoomArn": ...,
}

parent.list_smart_home_appliances(**kwargs)
```

1. See [:material-code-braces: ListSmartHomeAppliancesRequestRequestTypeDef](./type_defs.md#listsmarthomeappliancesrequestrequesttypedef) 

### list\_tags

Lists all tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").list_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.list_tags)

```python
# list_tags method definition

await def list_tags(
    self,
    *,
    Arn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


```python
# list_tags method usage example with argument unpacking

kwargs: ListTagsRequestRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.list_tags(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef) 

### put\_conference\_preference

Sets the conference preferences on a specific conference provider at the account
level.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").put_conference_preference` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.put_conference_preference)

```python
# put_conference_preference method definition

await def put_conference_preference(
    self,
    *,
    ConferencePreference: ConferencePreferenceTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ConferencePreferenceTypeDef](./type_defs.md#conferencepreferencetypedef) 


```python
# put_conference_preference method usage example with argument unpacking

kwargs: PutConferencePreferenceRequestRequestTypeDef = {  # (1)
    "ConferencePreference": ...,
}

parent.put_conference_preference(**kwargs)
```

1. See [:material-code-braces: PutConferencePreferenceRequestRequestTypeDef](./type_defs.md#putconferencepreferencerequestrequesttypedef) 

### put\_invitation\_configuration

Configures the email template for the user enrollment invitation with the
specified attributes.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").put_invitation_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.put_invitation_configuration)

```python
# put_invitation_configuration method definition

await def put_invitation_configuration(
    self,
    *,
    OrganizationName: str,
    ContactEmail: str = ...,
    PrivateSkillIds: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```



```python
# put_invitation_configuration method usage example with argument unpacking

kwargs: PutInvitationConfigurationRequestRequestTypeDef = {  # (1)
    "OrganizationName": ...,
}

parent.put_invitation_configuration(**kwargs)
```

1. See [:material-code-braces: PutInvitationConfigurationRequestRequestTypeDef](./type_defs.md#putinvitationconfigurationrequestrequesttypedef) 

### put\_room\_skill\_parameter

Updates room skill parameter details by room, skill, and parameter key ID.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").put_room_skill_parameter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.put_room_skill_parameter)

```python
# put_room_skill_parameter method definition

await def put_room_skill_parameter(
    self,
    *,
    SkillId: str,
    RoomSkillParameter: RoomSkillParameterTypeDef,  # (1)
    RoomArn: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: RoomSkillParameterTypeDef](./type_defs.md#roomskillparametertypedef) 


```python
# put_room_skill_parameter method usage example with argument unpacking

kwargs: PutRoomSkillParameterRequestRequestTypeDef = {  # (1)
    "SkillId": ...,
    "RoomSkillParameter": ...,
}

parent.put_room_skill_parameter(**kwargs)
```

1. See [:material-code-braces: PutRoomSkillParameterRequestRequestTypeDef](./type_defs.md#putroomskillparameterrequestrequesttypedef) 

### put\_skill\_authorization

Links a user's account to a third-party skill provider.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").put_skill_authorization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.put_skill_authorization)

```python
# put_skill_authorization method definition

await def put_skill_authorization(
    self,
    *,
    AuthorizationResult: Mapping[str, str],
    SkillId: str,
    RoomArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# put_skill_authorization method usage example with argument unpacking

kwargs: PutSkillAuthorizationRequestRequestTypeDef = {  # (1)
    "AuthorizationResult": ...,
    "SkillId": ...,
}

parent.put_skill_authorization(**kwargs)
```

1. See [:material-code-braces: PutSkillAuthorizationRequestRequestTypeDef](./type_defs.md#putskillauthorizationrequestrequesttypedef) 

### register\_avs\_device

Registers an Alexa-enabled device built by an Original Equipment Manufacturer
(OEM) using Alexa Voice Service (AVS).

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").register_avs_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.register_avs_device)

```python
# register_avs_device method definition

await def register_avs_device(
    self,
    *,
    ClientId: str,
    UserCode: str,
    ProductId: str,
    AmazonId: str,
    DeviceSerialNumber: str = ...,
    RoomArn: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> RegisterAVSDeviceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: RegisterAVSDeviceResponseTypeDef](./type_defs.md#registeravsdeviceresponsetypedef) 


```python
# register_avs_device method usage example with argument unpacking

kwargs: RegisterAVSDeviceRequestRequestTypeDef = {  # (1)
    "ClientId": ...,
    "UserCode": ...,
    "ProductId": ...,
    "AmazonId": ...,
}

parent.register_avs_device(**kwargs)
```

1. See [:material-code-braces: RegisterAVSDeviceRequestRequestTypeDef](./type_defs.md#registeravsdevicerequestrequesttypedef) 

### reject\_skill

Disassociates a skill from the organization under a user's AWS account.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").reject_skill` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.reject_skill)

```python
# reject_skill method definition

await def reject_skill(
    self,
    *,
    SkillId: str,
) -> Dict[str, Any]:
    ...
```



```python
# reject_skill method usage example with argument unpacking

kwargs: RejectSkillRequestRequestTypeDef = {  # (1)
    "SkillId": ...,
}

parent.reject_skill(**kwargs)
```

1. See [:material-code-braces: RejectSkillRequestRequestTypeDef](./type_defs.md#rejectskillrequestrequesttypedef) 

### resolve\_room

Determines the details for the room from which a skill request was invoked.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").resolve_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.resolve_room)

```python
# resolve_room method definition

await def resolve_room(
    self,
    *,
    UserId: str,
    SkillId: str,
) -> ResolveRoomResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResolveRoomResponseTypeDef](./type_defs.md#resolveroomresponsetypedef) 


```python
# resolve_room method usage example with argument unpacking

kwargs: ResolveRoomRequestRequestTypeDef = {  # (1)
    "UserId": ...,
    "SkillId": ...,
}

parent.resolve_room(**kwargs)
```

1. See [:material-code-braces: ResolveRoomRequestRequestTypeDef](./type_defs.md#resolveroomrequestrequesttypedef) 

### revoke\_invitation

Revokes an invitation and invalidates the enrollment URL.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").revoke_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.revoke_invitation)

```python
# revoke_invitation method definition

await def revoke_invitation(
    self,
    *,
    UserArn: str = ...,
    EnrollmentId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# revoke_invitation method usage example with argument unpacking

kwargs: RevokeInvitationRequestRequestTypeDef = {  # (1)
    "UserArn": ...,
}

parent.revoke_invitation(**kwargs)
```

1. See [:material-code-braces: RevokeInvitationRequestRequestTypeDef](./type_defs.md#revokeinvitationrequestrequesttypedef) 

### search\_address\_books

Searches address books and lists the ones that meet a set of filter and sort
criteria.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").search_address_books` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_address_books)

```python
# search_address_books method definition

await def search_address_books(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> SearchAddressBooksResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: SearchAddressBooksResponseTypeDef](./type_defs.md#searchaddressbooksresponsetypedef) 


```python
# search_address_books method usage example with argument unpacking

kwargs: SearchAddressBooksRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.search_address_books(**kwargs)
```

1. See [:material-code-braces: SearchAddressBooksRequestRequestTypeDef](./type_defs.md#searchaddressbooksrequestrequesttypedef) 

### search\_contacts

Searches contacts and lists the ones that meet a set of filter and sort
criteria.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").search_contacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_contacts)

```python
# search_contacts method definition

await def search_contacts(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> SearchContactsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: SearchContactsResponseTypeDef](./type_defs.md#searchcontactsresponsetypedef) 


```python
# search_contacts method usage example with argument unpacking

kwargs: SearchContactsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.search_contacts(**kwargs)
```

1. See [:material-code-braces: SearchContactsRequestRequestTypeDef](./type_defs.md#searchcontactsrequestrequesttypedef) 

### search\_devices

Searches devices and lists the ones that meet a set of filter criteria.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").search_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_devices)

```python
# search_devices method definition

await def search_devices(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
) -> SearchDevicesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef) 


```python
# search_devices method usage example with argument unpacking

kwargs: SearchDevicesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.search_devices(**kwargs)
```

1. See [:material-code-braces: SearchDevicesRequestRequestTypeDef](./type_defs.md#searchdevicesrequestrequesttypedef) 

### search\_network\_profiles

Searches network profiles and lists the ones that meet a set of filter and sort
criteria.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").search_network_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_network_profiles)

```python
# search_network_profiles method definition

await def search_network_profiles(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
) -> SearchNetworkProfilesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: SearchNetworkProfilesResponseTypeDef](./type_defs.md#searchnetworkprofilesresponsetypedef) 


```python
# search_network_profiles method usage example with argument unpacking

kwargs: SearchNetworkProfilesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.search_network_profiles(**kwargs)
```

1. See [:material-code-braces: SearchNetworkProfilesRequestRequestTypeDef](./type_defs.md#searchnetworkprofilesrequestrequesttypedef) 

### search\_profiles

Searches room profiles and lists the ones that meet a set of filter criteria.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").search_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_profiles)

```python
# search_profiles method definition

await def search_profiles(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
) -> SearchProfilesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: SearchProfilesResponseTypeDef](./type_defs.md#searchprofilesresponsetypedef) 


```python
# search_profiles method usage example with argument unpacking

kwargs: SearchProfilesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.search_profiles(**kwargs)
```

1. See [:material-code-braces: SearchProfilesRequestRequestTypeDef](./type_defs.md#searchprofilesrequestrequesttypedef) 

### search\_rooms

Searches rooms and lists the ones that meet a set of filter and sort criteria.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").search_rooms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_rooms)

```python
# search_rooms method definition

await def search_rooms(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
) -> SearchRoomsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: SearchRoomsResponseTypeDef](./type_defs.md#searchroomsresponsetypedef) 


```python
# search_rooms method usage example with argument unpacking

kwargs: SearchRoomsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.search_rooms(**kwargs)
```

1. See [:material-code-braces: SearchRoomsRequestRequestTypeDef](./type_defs.md#searchroomsrequestrequesttypedef) 

### search\_skill\_groups

Searches skill groups and lists the ones that meet a set of filter and sort
criteria.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").search_skill_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_skill_groups)

```python
# search_skill_groups method definition

await def search_skill_groups(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
) -> SearchSkillGroupsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: SearchSkillGroupsResponseTypeDef](./type_defs.md#searchskillgroupsresponsetypedef) 


```python
# search_skill_groups method usage example with argument unpacking

kwargs: SearchSkillGroupsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.search_skill_groups(**kwargs)
```

1. See [:material-code-braces: SearchSkillGroupsRequestRequestTypeDef](./type_defs.md#searchskillgroupsrequestrequesttypedef) 

### search\_users

Searches users and lists the ones that meet a set of filter and sort criteria.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").search_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.search_users)

```python
# search_users method definition

await def search_users(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
) -> SearchUsersResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: SearchUsersResponseTypeDef](./type_defs.md#searchusersresponsetypedef) 


```python
# search_users method usage example with argument unpacking

kwargs: SearchUsersRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.search_users(**kwargs)
```

1. See [:material-code-braces: SearchUsersRequestRequestTypeDef](./type_defs.md#searchusersrequestrequesttypedef) 

### send\_announcement

Triggers an asynchronous flow to send text, SSML, or audio announcements to
rooms that are identified by a search or filter.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").send_announcement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.send_announcement)

```python
# send_announcement method definition

await def send_announcement(
    self,
    *,
    RoomFilters: Sequence[FilterTypeDef],  # (1)
    Content: ContentTypeDef,  # (2)
    ClientRequestToken: str,
    TimeToLiveInSeconds: int = ...,
) -> SendAnnouncementResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
3. See [:material-code-braces: SendAnnouncementResponseTypeDef](./type_defs.md#sendannouncementresponsetypedef) 


```python
# send_announcement method usage example with argument unpacking

kwargs: SendAnnouncementRequestRequestTypeDef = {  # (1)
    "RoomFilters": ...,
    "Content": ...,
    "ClientRequestToken": ...,
}

parent.send_announcement(**kwargs)
```

1. See [:material-code-braces: SendAnnouncementRequestRequestTypeDef](./type_defs.md#sendannouncementrequestrequesttypedef) 

### send\_invitation

Sends an enrollment invitation email with a URL to a user.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").send_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.send_invitation)

```python
# send_invitation method definition

await def send_invitation(
    self,
    *,
    UserArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# send_invitation method usage example with argument unpacking

kwargs: SendInvitationRequestRequestTypeDef = {  # (1)
    "UserArn": ...,
}

parent.send_invitation(**kwargs)
```

1. See [:material-code-braces: SendInvitationRequestRequestTypeDef](./type_defs.md#sendinvitationrequestrequesttypedef) 

### start\_device\_sync

Resets a device and its account to the known default settings.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").start_device_sync` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.start_device_sync)

```python
# start_device_sync method definition

await def start_device_sync(
    self,
    *,
    Features: Sequence[FeatureType],  # (1)
    RoomArn: str = ...,
    DeviceArn: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: FeatureType](./literals.md#featuretype) 


```python
# start_device_sync method usage example with argument unpacking

kwargs: StartDeviceSyncRequestRequestTypeDef = {  # (1)
    "Features": ...,
}

parent.start_device_sync(**kwargs)
```

1. See [:material-code-braces: StartDeviceSyncRequestRequestTypeDef](./type_defs.md#startdevicesyncrequestrequesttypedef) 

### start\_smart\_home\_appliance\_discovery

Initiates the discovery of any smart home appliances associated with the room.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").start_smart_home_appliance_discovery` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.start_smart_home_appliance_discovery)

```python
# start_smart_home_appliance_discovery method definition

await def start_smart_home_appliance_discovery(
    self,
    *,
    RoomArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_smart_home_appliance_discovery method usage example with argument unpacking

kwargs: StartSmartHomeApplianceDiscoveryRequestRequestTypeDef = {  # (1)
    "RoomArn": ...,
}

parent.start_smart_home_appliance_discovery(**kwargs)
```

1. See [:material-code-braces: StartSmartHomeApplianceDiscoveryRequestRequestTypeDef](./type_defs.md#startsmarthomeappliancediscoveryrequestrequesttypedef) 

### tag\_resource

Adds metadata tags to a specified resource.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    Arn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "Arn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes metadata tags from a specified resource.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    Arn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "Arn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_address\_book

Updates address book details by the address book ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_address_book` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_address_book)

```python
# update_address_book method definition

await def update_address_book(
    self,
    *,
    AddressBookArn: str,
    Name: str = ...,
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_address_book method usage example with argument unpacking

kwargs: UpdateAddressBookRequestRequestTypeDef = {  # (1)
    "AddressBookArn": ...,
}

parent.update_address_book(**kwargs)
```

1. See [:material-code-braces: UpdateAddressBookRequestRequestTypeDef](./type_defs.md#updateaddressbookrequestrequesttypedef) 

### update\_business\_report\_schedule

Updates the configuration of the report delivery schedule with the specified
schedule ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_business_report_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_business_report_schedule)

```python
# update_business_report_schedule method definition

await def update_business_report_schedule(
    self,
    *,
    ScheduleArn: str,
    S3BucketName: str = ...,
    S3KeyPrefix: str = ...,
    Format: BusinessReportFormatType = ...,  # (1)
    ScheduleName: str = ...,
    Recurrence: BusinessReportRecurrenceTypeDef = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: BusinessReportFormatType](./literals.md#businessreportformattype) 
2. See [:material-code-braces: BusinessReportRecurrenceTypeDef](./type_defs.md#businessreportrecurrencetypedef) 


```python
# update_business_report_schedule method usage example with argument unpacking

kwargs: UpdateBusinessReportScheduleRequestRequestTypeDef = {  # (1)
    "ScheduleArn": ...,
}

parent.update_business_report_schedule(**kwargs)
```

1. See [:material-code-braces: UpdateBusinessReportScheduleRequestRequestTypeDef](./type_defs.md#updatebusinessreportschedulerequestrequesttypedef) 

### update\_conference\_provider

Updates an existing conference provider's settings.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_conference_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_conference_provider)

```python
# update_conference_provider method definition

await def update_conference_provider(
    self,
    *,
    ConferenceProviderArn: str,
    ConferenceProviderType: ConferenceProviderTypeType,  # (1)
    MeetingSetting: MeetingSettingTypeDef,  # (2)
    IPDialIn: IPDialInTypeDef = ...,  # (3)
    PSTNDialIn: PSTNDialInTypeDef = ...,  # (4)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ConferenceProviderTypeType](./literals.md#conferenceprovidertypetype) 
2. See [:material-code-braces: MeetingSettingTypeDef](./type_defs.md#meetingsettingtypedef) 
3. See [:material-code-braces: IPDialInTypeDef](./type_defs.md#ipdialintypedef) 
4. See [:material-code-braces: PSTNDialInTypeDef](./type_defs.md#pstndialintypedef) 


```python
# update_conference_provider method usage example with argument unpacking

kwargs: UpdateConferenceProviderRequestRequestTypeDef = {  # (1)
    "ConferenceProviderArn": ...,
    "ConferenceProviderType": ...,
    "MeetingSetting": ...,
}

parent.update_conference_provider(**kwargs)
```

1. See [:material-code-braces: UpdateConferenceProviderRequestRequestTypeDef](./type_defs.md#updateconferenceproviderrequestrequesttypedef) 

### update\_contact

Updates the contact details by the contact ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_contact)

```python
# update_contact method definition

await def update_contact(
    self,
    *,
    ContactArn: str,
    DisplayName: str = ...,
    FirstName: str = ...,
    LastName: str = ...,
    PhoneNumber: str = ...,
    PhoneNumbers: Sequence[PhoneNumberTypeDef] = ...,  # (1)
    SipAddresses: Sequence[SipAddressTypeDef] = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: PhoneNumberTypeDef](./type_defs.md#phonenumbertypedef) 
2. See [:material-code-braces: SipAddressTypeDef](./type_defs.md#sipaddresstypedef) 


```python
# update_contact method usage example with argument unpacking

kwargs: UpdateContactRequestRequestTypeDef = {  # (1)
    "ContactArn": ...,
}

parent.update_contact(**kwargs)
```

1. See [:material-code-braces: UpdateContactRequestRequestTypeDef](./type_defs.md#updatecontactrequestrequesttypedef) 

### update\_device

Updates the device name by device ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_device)

```python
# update_device method definition

await def update_device(
    self,
    *,
    DeviceArn: str = ...,
    DeviceName: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_device method usage example with argument unpacking

kwargs: UpdateDeviceRequestRequestTypeDef = {  # (1)
    "DeviceArn": ...,
}

parent.update_device(**kwargs)
```

1. See [:material-code-braces: UpdateDeviceRequestRequestTypeDef](./type_defs.md#updatedevicerequestrequesttypedef) 

### update\_gateway

Updates the details of a gateway.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_gateway)

```python
# update_gateway method definition

await def update_gateway(
    self,
    *,
    GatewayArn: str,
    Name: str = ...,
    Description: str = ...,
    SoftwareVersion: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_gateway method usage example with argument unpacking

kwargs: UpdateGatewayRequestRequestTypeDef = {  # (1)
    "GatewayArn": ...,
}

parent.update_gateway(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayRequestRequestTypeDef](./type_defs.md#updategatewayrequestrequesttypedef) 

### update\_gateway\_group

Updates the details of a gateway group.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_gateway_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_gateway_group)

```python
# update_gateway_group method definition

await def update_gateway_group(
    self,
    *,
    GatewayGroupArn: str,
    Name: str = ...,
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_gateway_group method usage example with argument unpacking

kwargs: UpdateGatewayGroupRequestRequestTypeDef = {  # (1)
    "GatewayGroupArn": ...,
}

parent.update_gateway_group(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayGroupRequestRequestTypeDef](./type_defs.md#updategatewaygrouprequestrequesttypedef) 

### update\_network\_profile

Updates a network profile by the network profile ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_network_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_network_profile)

```python
# update_network_profile method definition

await def update_network_profile(
    self,
    *,
    NetworkProfileArn: str,
    NetworkProfileName: str = ...,
    Description: str = ...,
    CurrentPassword: str = ...,
    NextPassword: str = ...,
    CertificateAuthorityArn: str = ...,
    TrustAnchors: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_network_profile method usage example with argument unpacking

kwargs: UpdateNetworkProfileRequestRequestTypeDef = {  # (1)
    "NetworkProfileArn": ...,
}

parent.update_network_profile(**kwargs)
```

1. See [:material-code-braces: UpdateNetworkProfileRequestRequestTypeDef](./type_defs.md#updatenetworkprofilerequestrequesttypedef) 

### update\_profile

Updates an existing room profile by room profile ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_profile)

```python
# update_profile method definition

await def update_profile(
    self,
    *,
    ProfileArn: str = ...,
    ProfileName: str = ...,
    IsDefault: bool = ...,
    Timezone: str = ...,
    Address: str = ...,
    DistanceUnit: DistanceUnitType = ...,  # (1)
    TemperatureUnit: TemperatureUnitType = ...,  # (2)
    WakeWord: WakeWordType = ...,  # (3)
    Locale: str = ...,
    SetupModeDisabled: bool = ...,
    MaxVolumeLimit: int = ...,
    PSTNEnabled: bool = ...,
    DataRetentionOptIn: bool = ...,
    MeetingRoomConfiguration: UpdateMeetingRoomConfigurationTypeDef = ...,  # (4)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: DistanceUnitType](./literals.md#distanceunittype) 
2. See [:material-code-brackets: TemperatureUnitType](./literals.md#temperatureunittype) 
3. See [:material-code-brackets: WakeWordType](./literals.md#wakewordtype) 
4. See [:material-code-braces: UpdateMeetingRoomConfigurationTypeDef](./type_defs.md#updatemeetingroomconfigurationtypedef) 


```python
# update_profile method usage example with argument unpacking

kwargs: UpdateProfileRequestRequestTypeDef = {  # (1)
    "ProfileArn": ...,
}

parent.update_profile(**kwargs)
```

1. See [:material-code-braces: UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef) 

### update\_room

Updates room details by room ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_room` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_room)

```python
# update_room method definition

await def update_room(
    self,
    *,
    RoomArn: str = ...,
    RoomName: str = ...,
    Description: str = ...,
    ProviderCalendarId: str = ...,
    ProfileArn: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_room method usage example with argument unpacking

kwargs: UpdateRoomRequestRequestTypeDef = {  # (1)
    "RoomArn": ...,
}

parent.update_room(**kwargs)
```

1. See [:material-code-braces: UpdateRoomRequestRequestTypeDef](./type_defs.md#updateroomrequestrequesttypedef) 

### update\_skill\_group

Updates skill group details by skill group ARN.

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").update_skill_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.update_skill_group)

```python
# update_skill_group method definition

await def update_skill_group(
    self,
    *,
    SkillGroupArn: str = ...,
    SkillGroupName: str = ...,
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_skill_group method usage example with argument unpacking

kwargs: UpdateSkillGroupRequestRequestTypeDef = {  # (1)
    "SkillGroupArn": ...,
}

parent.update_skill_group(**kwargs)
```

1. See [:material-code-braces: UpdateSkillGroupRequestRequestTypeDef](./type_defs.md#updateskillgrouprequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("alexaforbusiness").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> AlexaForBusinessClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("alexaforbusiness").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator` method with overloads.

- `client.get_paginator("list_business_report_schedules")` -> [ListBusinessReportSchedulesPaginator](./paginators.md#listbusinessreportschedulespaginator)
- `client.get_paginator("list_conference_providers")` -> [ListConferenceProvidersPaginator](./paginators.md#listconferenceproviderspaginator)
- `client.get_paginator("list_device_events")` -> [ListDeviceEventsPaginator](./paginators.md#listdeviceeventspaginator)
- `client.get_paginator("list_skills")` -> [ListSkillsPaginator](./paginators.md#listskillspaginator)
- `client.get_paginator("list_skills_store_categories")` -> [ListSkillsStoreCategoriesPaginator](./paginators.md#listskillsstorecategoriespaginator)
- `client.get_paginator("list_skills_store_skills_by_category")` -> [ListSkillsStoreSkillsByCategoryPaginator](./paginators.md#listskillsstoreskillsbycategorypaginator)
- `client.get_paginator("list_smart_home_appliances")` -> [ListSmartHomeAppliancesPaginator](./paginators.md#listsmarthomeappliancespaginator)
- `client.get_paginator("list_tags")` -> [ListTagsPaginator](./paginators.md#listtagspaginator)
- `client.get_paginator("search_devices")` -> [SearchDevicesPaginator](./paginators.md#searchdevicespaginator)
- `client.get_paginator("search_profiles")` -> [SearchProfilesPaginator](./paginators.md#searchprofilespaginator)
- `client.get_paginator("search_rooms")` -> [SearchRoomsPaginator](./paginators.md#searchroomspaginator)
- `client.get_paginator("search_skill_groups")` -> [SearchSkillGroupsPaginator](./paginators.md#searchskillgroupspaginator)
- `client.get_paginator("search_users")` -> [SearchUsersPaginator](./paginators.md#searchuserspaginator)



