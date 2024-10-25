# ChimeSDKVoiceClient

> [Index](../README.md) > [ChimeSDKVoice](./README.md) > ChimeSDKVoiceClient

!!! note ""

    Auto-generated documentation for [ChimeSDKVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice)
    type annotations stubs module [types-aiobotocore-chime-sdk-voice](https://pypi.org/project/types-aiobotocore-chime-sdk-voice/).

## ChimeSDKVoiceClient

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client)

```python
# ChimeSDKVoiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_chime_sdk_voice.client import ChimeSDKVoiceClient

session = get_session()
async with session.create_client("chime-sdk-voice") as client:
    client: ChimeSDKVoiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("chime-sdk-voice").exceptions` structure.

```python
# ChimeSDKVoiceClient.exceptions usage example

async with session.create_client("chime-sdk-voice") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.ForbiddenException,
        client.GoneException,
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
# ChimeSDKVoiceClient usage type checking example

from types_aiobotocore_chime_sdk_voice.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_phone\_numbers\_with\_voice\_connector

Associates phone numbers with the specified Amazon Chime SDK Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").associate_phone_numbers_with_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.associate_phone_numbers_with_voice_connector)

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

kwargs: AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "E164PhoneNumbers": ...,
}

parent.associate_phone_numbers_with_voice_connector(**kwargs)
```

1. See [:material-code-braces: AssociatePhoneNumbersWithVoiceConnectorRequestRequestTypeDef](./type_defs.md#associatephonenumberswithvoiceconnectorrequestrequesttypedef) 

### associate\_phone\_numbers\_with\_voice\_connector\_group

Associates phone numbers with the specified Amazon Chime SDK Voice Connector
group.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").associate_phone_numbers_with_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.associate_phone_numbers_with_voice_connector_group)

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

kwargs: AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef = {  # (1)
    "VoiceConnectorGroupId": ...,
    "E164PhoneNumbers": ...,
}

parent.associate_phone_numbers_with_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: AssociatePhoneNumbersWithVoiceConnectorGroupRequestRequestTypeDef](./type_defs.md#associatephonenumberswithvoiceconnectorgrouprequestrequesttypedef) 

### batch\_delete\_phone\_number

Moves phone numbers into the **Deletion queue**.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").batch_delete_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.batch_delete_phone_number)

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

kwargs: BatchDeletePhoneNumberRequestRequestTypeDef = {  # (1)
    "PhoneNumberIds": ...,
}

parent.batch_delete_phone_number(**kwargs)
```

1. See [:material-code-braces: BatchDeletePhoneNumberRequestRequestTypeDef](./type_defs.md#batchdeletephonenumberrequestrequesttypedef) 

### batch\_update\_phone\_number

Updates phone number product types, calling names, or phone number names.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").batch_update_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.batch_update_phone_number)

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

kwargs: BatchUpdatePhoneNumberRequestRequestTypeDef = {  # (1)
    "UpdatePhoneNumberRequestItems": ...,
}

parent.batch_update_phone_number(**kwargs)
```

1. See [:material-code-braces: BatchUpdatePhoneNumberRequestRequestTypeDef](./type_defs.md#batchupdatephonenumberrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_phone\_number\_order

Creates an order for phone numbers to be provisioned.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").create_phone_number_order` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_phone_number_order)

```python
# create_phone_number_order method definition

await def create_phone_number_order(
    self,
    *,
    ProductType: PhoneNumberProductTypeType,  # (1)
    E164PhoneNumbers: Sequence[str],
    Name: str = ...,
) -> CreatePhoneNumberOrderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
2. See [:material-code-braces: CreatePhoneNumberOrderResponseTypeDef](./type_defs.md#createphonenumberorderresponsetypedef) 


```python
# create_phone_number_order method usage example with argument unpacking

kwargs: CreatePhoneNumberOrderRequestRequestTypeDef = {  # (1)
    "ProductType": ...,
    "E164PhoneNumbers": ...,
}

parent.create_phone_number_order(**kwargs)
```

1. See [:material-code-braces: CreatePhoneNumberOrderRequestRequestTypeDef](./type_defs.md#createphonenumberorderrequestrequesttypedef) 

### create\_proxy\_session

Creates a proxy session for the specified Amazon Chime SDK Voice Connector for
the specified participant phone
numbers.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").create_proxy_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_proxy_session)

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

kwargs: CreateProxySessionRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "ParticipantPhoneNumbers": ...,
    "Capabilities": ...,
}

parent.create_proxy_session(**kwargs)
```

1. See [:material-code-braces: CreateProxySessionRequestRequestTypeDef](./type_defs.md#createproxysessionrequestrequesttypedef) 

### create\_sip\_media\_application

Creates a SIP media application.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").create_sip_media_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_media_application)

```python
# create_sip_media_application method definition

await def create_sip_media_application(
    self,
    *,
    AwsRegion: str,
    Name: str,
    Endpoints: Sequence[SipMediaApplicationEndpointTypeDef],  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateSipMediaApplicationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SipMediaApplicationEndpointTypeDef](./type_defs.md#sipmediaapplicationendpointtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateSipMediaApplicationResponseTypeDef](./type_defs.md#createsipmediaapplicationresponsetypedef) 


```python
# create_sip_media_application method usage example with argument unpacking

kwargs: CreateSipMediaApplicationRequestRequestTypeDef = {  # (1)
    "AwsRegion": ...,
    "Name": ...,
    "Endpoints": ...,
}

parent.create_sip_media_application(**kwargs)
```

1. See [:material-code-braces: CreateSipMediaApplicationRequestRequestTypeDef](./type_defs.md#createsipmediaapplicationrequestrequesttypedef) 

### create\_sip\_media\_application\_call

Creates an outbound call to a phone number from the phone number specified in
the request, and it invokes the endpoint of the specified
`sipMediaApplicationId`.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").create_sip_media_application_call` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_media_application_call)

```python
# create_sip_media_application_call method definition

await def create_sip_media_application_call(
    self,
    *,
    FromPhoneNumber: str,
    ToPhoneNumber: str,
    SipMediaApplicationId: str,
    SipHeaders: Mapping[str, str] = ...,
    ArgumentsMap: Mapping[str, str] = ...,
) -> CreateSipMediaApplicationCallResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSipMediaApplicationCallResponseTypeDef](./type_defs.md#createsipmediaapplicationcallresponsetypedef) 


```python
# create_sip_media_application_call method usage example with argument unpacking

kwargs: CreateSipMediaApplicationCallRequestRequestTypeDef = {  # (1)
    "FromPhoneNumber": ...,
    "ToPhoneNumber": ...,
    "SipMediaApplicationId": ...,
}

parent.create_sip_media_application_call(**kwargs)
```

1. See [:material-code-braces: CreateSipMediaApplicationCallRequestRequestTypeDef](./type_defs.md#createsipmediaapplicationcallrequestrequesttypedef) 

### create\_sip\_rule

Creates a SIP rule, which can be used to run a SIP media application as a
target for a specific trigger
type.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").create_sip_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_sip_rule)

```python
# create_sip_rule method definition

await def create_sip_rule(
    self,
    *,
    Name: str,
    TriggerType: SipRuleTriggerTypeType,  # (1)
    TriggerValue: str,
    Disabled: bool = ...,
    TargetApplications: Sequence[SipRuleTargetApplicationTypeDef] = ...,  # (2)
) -> CreateSipRuleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SipRuleTriggerTypeType](./literals.md#sipruletriggertypetype) 
2. See [:material-code-braces: SipRuleTargetApplicationTypeDef](./type_defs.md#sipruletargetapplicationtypedef) 
3. See [:material-code-braces: CreateSipRuleResponseTypeDef](./type_defs.md#createsipruleresponsetypedef) 


```python
# create_sip_rule method usage example with argument unpacking

kwargs: CreateSipRuleRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "TriggerType": ...,
    "TriggerValue": ...,
}

parent.create_sip_rule(**kwargs)
```

1. See [:material-code-braces: CreateSipRuleRequestRequestTypeDef](./type_defs.md#createsiprulerequestrequesttypedef) 

### create\_voice\_connector

Creates an Amazon Chime SDK Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").create_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_connector)

```python
# create_voice_connector method definition

await def create_voice_connector(
    self,
    *,
    Name: str,
    RequireEncryption: bool,
    AwsRegion: VoiceConnectorAwsRegionType = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateVoiceConnectorResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: VoiceConnectorAwsRegionType](./literals.md#voiceconnectorawsregiontype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateVoiceConnectorResponseTypeDef](./type_defs.md#createvoiceconnectorresponsetypedef) 


```python
# create_voice_connector method usage example with argument unpacking

kwargs: CreateVoiceConnectorRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RequireEncryption": ...,
}

parent.create_voice_connector(**kwargs)
```

1. See [:material-code-braces: CreateVoiceConnectorRequestRequestTypeDef](./type_defs.md#createvoiceconnectorrequestrequesttypedef) 

### create\_voice\_connector\_group

Creates an Amazon Chime SDK Voice Connector group under the administrator's AWS
account.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").create_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_connector_group)

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

kwargs: CreateVoiceConnectorGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: CreateVoiceConnectorGroupRequestRequestTypeDef](./type_defs.md#createvoiceconnectorgrouprequestrequesttypedef) 

### create\_voice\_profile

Creates a voice profile, which consists of an enrolled user and their latest
voice
print.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").create_voice_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile)

```python
# create_voice_profile method definition

await def create_voice_profile(
    self,
    *,
    SpeakerSearchTaskId: str,
) -> CreateVoiceProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateVoiceProfileResponseTypeDef](./type_defs.md#createvoiceprofileresponsetypedef) 


```python
# create_voice_profile method usage example with argument unpacking

kwargs: CreateVoiceProfileRequestRequestTypeDef = {  # (1)
    "SpeakerSearchTaskId": ...,
}

parent.create_voice_profile(**kwargs)
```

1. See [:material-code-braces: CreateVoiceProfileRequestRequestTypeDef](./type_defs.md#createvoiceprofilerequestrequesttypedef) 

### create\_voice\_profile\_domain

Creates a voice profile domain, a collection of voice profiles, their voice
prints, and encrypted enrollment
audio.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").create_voice_profile_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.create_voice_profile_domain)

```python
# create_voice_profile_domain method definition

await def create_voice_profile_domain(
    self,
    *,
    Name: str,
    ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,  # (1)
    Description: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateVoiceProfileDomainResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateVoiceProfileDomainResponseTypeDef](./type_defs.md#createvoiceprofiledomainresponsetypedef) 


```python
# create_voice_profile_domain method usage example with argument unpacking

kwargs: CreateVoiceProfileDomainRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ServerSideEncryptionConfiguration": ...,
}

parent.create_voice_profile_domain(**kwargs)
```

1. See [:material-code-braces: CreateVoiceProfileDomainRequestRequestTypeDef](./type_defs.md#createvoiceprofiledomainrequestrequesttypedef) 

### delete\_phone\_number

Moves the specified phone number into the **Deletion queue**.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_phone_number)

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

kwargs: DeletePhoneNumberRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.delete_phone_number(**kwargs)
```

1. See [:material-code-braces: DeletePhoneNumberRequestRequestTypeDef](./type_defs.md#deletephonenumberrequestrequesttypedef) 

### delete\_proxy\_session

Deletes the specified proxy session from the specified Amazon Chime SDK Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_proxy_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_proxy_session)

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

kwargs: DeleteProxySessionRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "ProxySessionId": ...,
}

parent.delete_proxy_session(**kwargs)
```

1. See [:material-code-braces: DeleteProxySessionRequestRequestTypeDef](./type_defs.md#deleteproxysessionrequestrequesttypedef) 

### delete\_sip\_media\_application

Deletes a SIP media application.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_sip_media_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_sip_media_application)

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

kwargs: DeleteSipMediaApplicationRequestRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.delete_sip_media_application(**kwargs)
```

1. See [:material-code-braces: DeleteSipMediaApplicationRequestRequestTypeDef](./type_defs.md#deletesipmediaapplicationrequestrequesttypedef) 

### delete\_sip\_rule

Deletes a SIP rule.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_sip_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_sip_rule)

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

kwargs: DeleteSipRuleRequestRequestTypeDef = {  # (1)
    "SipRuleId": ...,
}

parent.delete_sip_rule(**kwargs)
```

1. See [:material-code-braces: DeleteSipRuleRequestRequestTypeDef](./type_defs.md#deletesiprulerequestrequesttypedef) 

### delete\_voice\_connector

Deletes an Amazon Chime SDK Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector)

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

kwargs: DeleteVoiceConnectorRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorRequestRequestTypeDef](./type_defs.md#deletevoiceconnectorrequestrequesttypedef) 

### delete\_voice\_connector\_emergency\_calling\_configuration

Deletes the emergency calling details from the specified Amazon Chime SDK Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_voice_connector_emergency_calling_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_emergency_calling_configuration)

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

kwargs: DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector_emergency_calling_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef](./type_defs.md#deletevoiceconnectoremergencycallingconfigurationrequestrequesttypedef) 

### delete\_voice\_connector\_group

Deletes an Amazon Chime SDK Voice Connector group.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_group)

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

kwargs: DeleteVoiceConnectorGroupRequestRequestTypeDef = {  # (1)
    "VoiceConnectorGroupId": ...,
}

parent.delete_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorGroupRequestRequestTypeDef](./type_defs.md#deletevoiceconnectorgrouprequestrequesttypedef) 

### delete\_voice\_connector\_origination

Deletes the origination settings for the specified Amazon Chime SDK Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_voice_connector_origination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_origination)

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

kwargs: DeleteVoiceConnectorOriginationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector_origination(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorOriginationRequestRequestTypeDef](./type_defs.md#deletevoiceconnectororiginationrequestrequesttypedef) 

### delete\_voice\_connector\_proxy

Deletes the proxy configuration from the specified Amazon Chime SDK Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_voice_connector_proxy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_proxy)

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

kwargs: DeleteVoiceConnectorProxyRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector_proxy(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorProxyRequestRequestTypeDef](./type_defs.md#deletevoiceconnectorproxyrequestrequesttypedef) 

### delete\_voice\_connector\_streaming\_configuration

Deletes a Voice Connector's streaming configuration.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_voice_connector_streaming_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_streaming_configuration)

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

kwargs: DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector_streaming_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorStreamingConfigurationRequestRequestTypeDef](./type_defs.md#deletevoiceconnectorstreamingconfigurationrequestrequesttypedef) 

### delete\_voice\_connector\_termination

Deletes the termination settings for the specified Amazon Chime SDK Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_voice_connector_termination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_termination)

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

kwargs: DeleteVoiceConnectorTerminationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.delete_voice_connector_termination(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorTerminationRequestRequestTypeDef](./type_defs.md#deletevoiceconnectorterminationrequestrequesttypedef) 

### delete\_voice\_connector\_termination\_credentials

Deletes the specified SIP credentials used by your equipment to authenticate
during call
termination.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_voice_connector_termination_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_connector_termination_credentials)

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

kwargs: DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "Usernames": ...,
}

parent.delete_voice_connector_termination_credentials(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceConnectorTerminationCredentialsRequestRequestTypeDef](./type_defs.md#deletevoiceconnectorterminationcredentialsrequestrequesttypedef) 

### delete\_voice\_profile

Deletes a voice profile, including its voice print and enrollment data.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_voice_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_profile)

```python
# delete_voice_profile method definition

await def delete_voice_profile(
    self,
    *,
    VoiceProfileId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_voice_profile method usage example with argument unpacking

kwargs: DeleteVoiceProfileRequestRequestTypeDef = {  # (1)
    "VoiceProfileId": ...,
}

parent.delete_voice_profile(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceProfileRequestRequestTypeDef](./type_defs.md#deletevoiceprofilerequestrequesttypedef) 

### delete\_voice\_profile\_domain

Deletes all voice profiles in the domain.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").delete_voice_profile_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.delete_voice_profile_domain)

```python
# delete_voice_profile_domain method definition

await def delete_voice_profile_domain(
    self,
    *,
    VoiceProfileDomainId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_voice_profile_domain method usage example with argument unpacking

kwargs: DeleteVoiceProfileDomainRequestRequestTypeDef = {  # (1)
    "VoiceProfileDomainId": ...,
}

parent.delete_voice_profile_domain(**kwargs)
```

1. See [:material-code-braces: DeleteVoiceProfileDomainRequestRequestTypeDef](./type_defs.md#deletevoiceprofiledomainrequestrequesttypedef) 

### disassociate\_phone\_numbers\_from\_voice\_connector

Disassociates the specified phone numbers from the specified Amazon Chime SDK
Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").disassociate_phone_numbers_from_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.disassociate_phone_numbers_from_voice_connector)

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

kwargs: DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "E164PhoneNumbers": ...,
}

parent.disassociate_phone_numbers_from_voice_connector(**kwargs)
```

1. See [:material-code-braces: DisassociatePhoneNumbersFromVoiceConnectorRequestRequestTypeDef](./type_defs.md#disassociatephonenumbersfromvoiceconnectorrequestrequesttypedef) 

### disassociate\_phone\_numbers\_from\_voice\_connector\_group

Disassociates the specified phone numbers from the specified Amazon Chime SDK
Voice Connector
group.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").disassociate_phone_numbers_from_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.disassociate_phone_numbers_from_voice_connector_group)

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

kwargs: DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef = {  # (1)
    "VoiceConnectorGroupId": ...,
    "E164PhoneNumbers": ...,
}

parent.disassociate_phone_numbers_from_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: DisassociatePhoneNumbersFromVoiceConnectorGroupRequestRequestTypeDef](./type_defs.md#disassociatephonenumbersfromvoiceconnectorgrouprequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.generate_presigned_url)

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


### get\_global\_settings

Retrieves the global settings for the Amazon Chime SDK Voice Connectors in an
AWS
account.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_global_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_global_settings)

```python
# get_global_settings method definition

await def get_global_settings(
    self,
) -> GetGlobalSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGlobalSettingsResponseTypeDef](./type_defs.md#getglobalsettingsresponsetypedef) 

### get\_phone\_number

Retrieves details for the specified phone number ID, such as associations,
capabilities, and product
type.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_phone_number)

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

kwargs: GetPhoneNumberRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.get_phone_number(**kwargs)
```

1. See [:material-code-braces: GetPhoneNumberRequestRequestTypeDef](./type_defs.md#getphonenumberrequestrequesttypedef) 

### get\_phone\_number\_order

Retrieves details for the specified phone number order, such as the order
creation timestamp, phone numbers in E.164 format, product type, and order
status.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_phone_number_order` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_phone_number_order)

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

kwargs: GetPhoneNumberOrderRequestRequestTypeDef = {  # (1)
    "PhoneNumberOrderId": ...,
}

parent.get_phone_number_order(**kwargs)
```

1. See [:material-code-braces: GetPhoneNumberOrderRequestRequestTypeDef](./type_defs.md#getphonenumberorderrequestrequesttypedef) 

### get\_phone\_number\_settings

Retrieves the phone number settings for the administrator's AWS account, such
as the default outbound calling
name.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_phone_number_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_phone_number_settings)

```python
# get_phone_number_settings method definition

await def get_phone_number_settings(
    self,
) -> GetPhoneNumberSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPhoneNumberSettingsResponseTypeDef](./type_defs.md#getphonenumbersettingsresponsetypedef) 

### get\_proxy\_session

Retrieves the specified proxy session details for the specified Amazon Chime
SDK Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_proxy_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_proxy_session)

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

kwargs: GetProxySessionRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "ProxySessionId": ...,
}

parent.get_proxy_session(**kwargs)
```

1. See [:material-code-braces: GetProxySessionRequestRequestTypeDef](./type_defs.md#getproxysessionrequestrequesttypedef) 

### get\_sip\_media\_application

Retrieves the information for a SIP media application, including name, AWS
Region, and
endpoints.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_sip_media_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_media_application)

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

kwargs: GetSipMediaApplicationRequestRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.get_sip_media_application(**kwargs)
```

1. See [:material-code-braces: GetSipMediaApplicationRequestRequestTypeDef](./type_defs.md#getsipmediaapplicationrequestrequesttypedef) 

### get\_sip\_media\_application\_alexa\_skill\_configuration

Gets the Alexa Skill configuration for the SIP media application.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_sip_media_application_alexa_skill_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_media_application_alexa_skill_configuration)

```python
# get_sip_media_application_alexa_skill_configuration method definition

await def get_sip_media_application_alexa_skill_configuration(
    self,
    *,
    SipMediaApplicationId: str,
) -> GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSipMediaApplicationAlexaSkillConfigurationResponseTypeDef](./type_defs.md#getsipmediaapplicationalexaskillconfigurationresponsetypedef) 


```python
# get_sip_media_application_alexa_skill_configuration method usage example with argument unpacking

kwargs: GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.get_sip_media_application_alexa_skill_configuration(**kwargs)
```

1. See [:material-code-braces: GetSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef](./type_defs.md#getsipmediaapplicationalexaskillconfigurationrequestrequesttypedef) 

### get\_sip\_media\_application\_logging\_configuration

Retrieves the logging configuration for the specified SIP media application.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_sip_media_application_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_media_application_logging_configuration)

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

kwargs: GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.get_sip_media_application_logging_configuration(**kwargs)
```

1. See [:material-code-braces: GetSipMediaApplicationLoggingConfigurationRequestRequestTypeDef](./type_defs.md#getsipmediaapplicationloggingconfigurationrequestrequesttypedef) 

### get\_sip\_rule

Retrieves the details of a SIP rule, such as the rule ID, name, triggers, and
target
endpoints.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_sip_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_sip_rule)

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

kwargs: GetSipRuleRequestRequestTypeDef = {  # (1)
    "SipRuleId": ...,
}

parent.get_sip_rule(**kwargs)
```

1. See [:material-code-braces: GetSipRuleRequestRequestTypeDef](./type_defs.md#getsiprulerequestrequesttypedef) 

### get\_speaker\_search\_task

Retrieves the details of the specified speaker search task.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_speaker_search_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_speaker_search_task)

```python
# get_speaker_search_task method definition

await def get_speaker_search_task(
    self,
    *,
    VoiceConnectorId: str,
    SpeakerSearchTaskId: str,
) -> GetSpeakerSearchTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSpeakerSearchTaskResponseTypeDef](./type_defs.md#getspeakersearchtaskresponsetypedef) 


```python
# get_speaker_search_task method usage example with argument unpacking

kwargs: GetSpeakerSearchTaskRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "SpeakerSearchTaskId": ...,
}

parent.get_speaker_search_task(**kwargs)
```

1. See [:material-code-braces: GetSpeakerSearchTaskRequestRequestTypeDef](./type_defs.md#getspeakersearchtaskrequestrequesttypedef) 

### get\_voice\_connector

Retrieves details for the specified Amazon Chime SDK Voice Connector, such as
timestamps,name, outbound host, and encryption
requirements.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector)

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

kwargs: GetVoiceConnectorRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorRequestRequestTypeDef](./type_defs.md#getvoiceconnectorrequestrequesttypedef) 

### get\_voice\_connector\_emergency\_calling\_configuration

Retrieves the emergency calling configuration details for the specified Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_connector_emergency_calling_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_emergency_calling_configuration)

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

kwargs: GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_emergency_calling_configuration(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef](./type_defs.md#getvoiceconnectoremergencycallingconfigurationrequestrequesttypedef) 

### get\_voice\_connector\_group

Retrieves details for the specified Amazon Chime SDK Voice Connector group,
such as timestamps,name, and associated
`VoiceConnectorItems`.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_group)

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

kwargs: GetVoiceConnectorGroupRequestRequestTypeDef = {  # (1)
    "VoiceConnectorGroupId": ...,
}

parent.get_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorGroupRequestRequestTypeDef](./type_defs.md#getvoiceconnectorgrouprequestrequesttypedef) 

### get\_voice\_connector\_logging\_configuration

Retrieves the logging configuration settings for the specified Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_connector_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_logging_configuration)

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

kwargs: GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_logging_configuration(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorLoggingConfigurationRequestRequestTypeDef](./type_defs.md#getvoiceconnectorloggingconfigurationrequestrequesttypedef) 

### get\_voice\_connector\_origination

Retrieves the origination settings for the specified Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_connector_origination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_origination)

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

kwargs: GetVoiceConnectorOriginationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_origination(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorOriginationRequestRequestTypeDef](./type_defs.md#getvoiceconnectororiginationrequestrequesttypedef) 

### get\_voice\_connector\_proxy

Retrieves the proxy configuration details for the specified Amazon Chime SDK
Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_connector_proxy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_proxy)

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

kwargs: GetVoiceConnectorProxyRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_proxy(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorProxyRequestRequestTypeDef](./type_defs.md#getvoiceconnectorproxyrequestrequesttypedef) 

### get\_voice\_connector\_streaming\_configuration

Retrieves the streaming configuration details for the specified Amazon Chime
SDK Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_connector_streaming_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_streaming_configuration)

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

kwargs: GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_streaming_configuration(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef](./type_defs.md#getvoiceconnectorstreamingconfigurationrequestrequesttypedef) 

### get\_voice\_connector\_termination

Retrieves the termination setting details for the specified Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_connector_termination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_termination)

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

kwargs: GetVoiceConnectorTerminationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_termination(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorTerminationRequestRequestTypeDef](./type_defs.md#getvoiceconnectorterminationrequestrequesttypedef) 

### get\_voice\_connector\_termination\_health

Retrieves information about the last time a `SIP OPTIONS` ping was received
from your SIP infrastructure for the specified Amazon Chime SDK Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_connector_termination_health` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_connector_termination_health)

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

kwargs: GetVoiceConnectorTerminationHealthRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.get_voice_connector_termination_health(**kwargs)
```

1. See [:material-code-braces: GetVoiceConnectorTerminationHealthRequestRequestTypeDef](./type_defs.md#getvoiceconnectorterminationhealthrequestrequesttypedef) 

### get\_voice\_profile

Retrieves the details of the specified voice profile.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_profile)

```python
# get_voice_profile method definition

await def get_voice_profile(
    self,
    *,
    VoiceProfileId: str,
) -> GetVoiceProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceProfileResponseTypeDef](./type_defs.md#getvoiceprofileresponsetypedef) 


```python
# get_voice_profile method usage example with argument unpacking

kwargs: GetVoiceProfileRequestRequestTypeDef = {  # (1)
    "VoiceProfileId": ...,
}

parent.get_voice_profile(**kwargs)
```

1. See [:material-code-braces: GetVoiceProfileRequestRequestTypeDef](./type_defs.md#getvoiceprofilerequestrequesttypedef) 

### get\_voice\_profile\_domain

Retrieves the details of the specified voice profile domain.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_profile_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_profile_domain)

```python
# get_voice_profile_domain method definition

await def get_voice_profile_domain(
    self,
    *,
    VoiceProfileDomainId: str,
) -> GetVoiceProfileDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceProfileDomainResponseTypeDef](./type_defs.md#getvoiceprofiledomainresponsetypedef) 


```python
# get_voice_profile_domain method usage example with argument unpacking

kwargs: GetVoiceProfileDomainRequestRequestTypeDef = {  # (1)
    "VoiceProfileDomainId": ...,
}

parent.get_voice_profile_domain(**kwargs)
```

1. See [:material-code-braces: GetVoiceProfileDomainRequestRequestTypeDef](./type_defs.md#getvoiceprofiledomainrequestrequesttypedef) 

### get\_voice\_tone\_analysis\_task

Retrieves the details of a voice tone analysis task.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_voice_tone_analysis_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.get_voice_tone_analysis_task)

```python
# get_voice_tone_analysis_task method definition

await def get_voice_tone_analysis_task(
    self,
    *,
    VoiceConnectorId: str,
    VoiceToneAnalysisTaskId: str,
    IsCaller: bool,
) -> GetVoiceToneAnalysisTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVoiceToneAnalysisTaskResponseTypeDef](./type_defs.md#getvoicetoneanalysistaskresponsetypedef) 


```python
# get_voice_tone_analysis_task method usage example with argument unpacking

kwargs: GetVoiceToneAnalysisTaskRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "VoiceToneAnalysisTaskId": ...,
    "IsCaller": ...,
}

parent.get_voice_tone_analysis_task(**kwargs)
```

1. See [:material-code-braces: GetVoiceToneAnalysisTaskRequestRequestTypeDef](./type_defs.md#getvoicetoneanalysistaskrequestrequesttypedef) 

### list\_available\_voice\_connector\_regions

Lists the available AWS Regions in which you can create an Amazon Chime SDK
Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_available_voice_connector_regions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_available_voice_connector_regions)

```python
# list_available_voice_connector_regions method definition

await def list_available_voice_connector_regions(
    self,
) -> ListAvailableVoiceConnectorRegionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAvailableVoiceConnectorRegionsResponseTypeDef](./type_defs.md#listavailablevoiceconnectorregionsresponsetypedef) 

### list\_phone\_number\_orders

Lists the phone numbers for an administrator's Amazon Chime SDK account.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_phone_number_orders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_phone_number_orders)

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

kwargs: ListPhoneNumberOrdersRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_phone_number_orders(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumberOrdersRequestRequestTypeDef](./type_defs.md#listphonenumberordersrequestrequesttypedef) 

### list\_phone\_numbers

Lists the phone numbers for the specified Amazon Chime SDK account, Amazon
Chime SDK user, Amazon Chime SDK Voice Connector, or Amazon Chime SDK Voice
Connector
group.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_phone_numbers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_phone_numbers)

```python
# list_phone_numbers method definition

await def list_phone_numbers(
    self,
    *,
    Status: str = ...,
    ProductType: PhoneNumberProductTypeType = ...,  # (1)
    FilterName: PhoneNumberAssociationNameType = ...,  # (2)
    FilterValue: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPhoneNumbersResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
2. See [:material-code-brackets: PhoneNumberAssociationNameType](./literals.md#phonenumberassociationnametype) 
3. See [:material-code-braces: ListPhoneNumbersResponseTypeDef](./type_defs.md#listphonenumbersresponsetypedef) 


```python
# list_phone_numbers method usage example with argument unpacking

kwargs: ListPhoneNumbersRequestRequestTypeDef = {  # (1)
    "Status": ...,
}

parent.list_phone_numbers(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumbersRequestRequestTypeDef](./type_defs.md#listphonenumbersrequestrequesttypedef) 

### list\_proxy\_sessions

Lists the proxy sessions for the specified Amazon Chime SDK Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_proxy_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_proxy_sessions)

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

kwargs: ListProxySessionsRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.list_proxy_sessions(**kwargs)
```

1. See [:material-code-braces: ListProxySessionsRequestRequestTypeDef](./type_defs.md#listproxysessionsrequestrequesttypedef) 

### list\_sip\_media\_applications

Lists the SIP media applications under the administrator's AWS account.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_sip_media_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_sip_media_applications)

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

kwargs: ListSipMediaApplicationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_sip_media_applications(**kwargs)
```

1. See [:material-code-braces: ListSipMediaApplicationsRequestRequestTypeDef](./type_defs.md#listsipmediaapplicationsrequestrequesttypedef) 

### list\_sip\_rules

Lists the SIP rules under the administrator's AWS account.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_sip_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_sip_rules)

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

kwargs: ListSipRulesRequestRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.list_sip_rules(**kwargs)
```

1. See [:material-code-braces: ListSipRulesRequestRequestTypeDef](./type_defs.md#listsiprulesrequestrequesttypedef) 

### list\_supported\_phone\_number\_countries

Lists the countries that you can order phone numbers from.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_supported_phone_number_countries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_supported_phone_number_countries)

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

kwargs: ListSupportedPhoneNumberCountriesRequestRequestTypeDef = {  # (1)
    "ProductType": ...,
}

parent.list_supported_phone_number_countries(**kwargs)
```

1. See [:material-code-braces: ListSupportedPhoneNumberCountriesRequestRequestTypeDef](./type_defs.md#listsupportedphonenumbercountriesrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of the tags in a given resource.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_tags_for_resource)

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

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_voice\_connector\_groups

Lists the Amazon Chime SDK Voice Connector groups in the administrator's AWS
account.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_voice_connector_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connector_groups)

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

kwargs: ListVoiceConnectorGroupsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_voice_connector_groups(**kwargs)
```

1. See [:material-code-braces: ListVoiceConnectorGroupsRequestRequestTypeDef](./type_defs.md#listvoiceconnectorgroupsrequestrequesttypedef) 

### list\_voice\_connector\_termination\_credentials

Lists the SIP credentials for the specified Amazon Chime SDK Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_voice_connector_termination_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connector_termination_credentials)

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

kwargs: ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.list_voice_connector_termination_credentials(**kwargs)
```

1. See [:material-code-braces: ListVoiceConnectorTerminationCredentialsRequestRequestTypeDef](./type_defs.md#listvoiceconnectorterminationcredentialsrequestrequesttypedef) 

### list\_voice\_connectors

Lists the Amazon Chime SDK Voice Connectors in the administrators AWS account.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_voice_connectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_connectors)

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

kwargs: ListVoiceConnectorsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_voice_connectors(**kwargs)
```

1. See [:material-code-braces: ListVoiceConnectorsRequestRequestTypeDef](./type_defs.md#listvoiceconnectorsrequestrequesttypedef) 

### list\_voice\_profile\_domains

Lists the specified voice profile domains in the administrator's AWS account.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_voice_profile_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profile_domains)

```python
# list_voice_profile_domains method definition

await def list_voice_profile_domains(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListVoiceProfileDomainsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVoiceProfileDomainsResponseTypeDef](./type_defs.md#listvoiceprofiledomainsresponsetypedef) 


```python
# list_voice_profile_domains method usage example with argument unpacking

kwargs: ListVoiceProfileDomainsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_voice_profile_domains(**kwargs)
```

1. See [:material-code-braces: ListVoiceProfileDomainsRequestRequestTypeDef](./type_defs.md#listvoiceprofiledomainsrequestrequesttypedef) 

### list\_voice\_profiles

Lists the voice profiles in a voice profile domain.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").list_voice_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.list_voice_profiles)

```python
# list_voice_profiles method definition

await def list_voice_profiles(
    self,
    *,
    VoiceProfileDomainId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListVoiceProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVoiceProfilesResponseTypeDef](./type_defs.md#listvoiceprofilesresponsetypedef) 


```python
# list_voice_profiles method usage example with argument unpacking

kwargs: ListVoiceProfilesRequestRequestTypeDef = {  # (1)
    "VoiceProfileDomainId": ...,
}

parent.list_voice_profiles(**kwargs)
```

1. See [:material-code-braces: ListVoiceProfilesRequestRequestTypeDef](./type_defs.md#listvoiceprofilesrequestrequesttypedef) 

### put\_sip\_media\_application\_alexa\_skill\_configuration

Updates the Alexa Skill configuration for the SIP media application.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").put_sip_media_application_alexa_skill_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_alexa_skill_configuration)

```python
# put_sip_media_application_alexa_skill_configuration method definition

await def put_sip_media_application_alexa_skill_configuration(
    self,
    *,
    SipMediaApplicationId: str,
    SipMediaApplicationAlexaSkillConfiguration: SipMediaApplicationAlexaSkillConfigurationTypeDef = ...,  # (1)
) -> PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SipMediaApplicationAlexaSkillConfigurationTypeDef](./type_defs.md#sipmediaapplicationalexaskillconfigurationtypedef) 
2. See [:material-code-braces: PutSipMediaApplicationAlexaSkillConfigurationResponseTypeDef](./type_defs.md#putsipmediaapplicationalexaskillconfigurationresponsetypedef) 


```python
# put_sip_media_application_alexa_skill_configuration method usage example with argument unpacking

kwargs: PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.put_sip_media_application_alexa_skill_configuration(**kwargs)
```

1. See [:material-code-braces: PutSipMediaApplicationAlexaSkillConfigurationRequestRequestTypeDef](./type_defs.md#putsipmediaapplicationalexaskillconfigurationrequestrequesttypedef) 

### put\_sip\_media\_application\_logging\_configuration

Updates the logging configuration for the specified SIP media application.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").put_sip_media_application_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_sip_media_application_logging_configuration)

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

kwargs: PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.put_sip_media_application_logging_configuration(**kwargs)
```

1. See [:material-code-braces: PutSipMediaApplicationLoggingConfigurationRequestRequestTypeDef](./type_defs.md#putsipmediaapplicationloggingconfigurationrequestrequesttypedef) 

### put\_voice\_connector\_emergency\_calling\_configuration

Updates a Voice Connector's emergency calling configuration.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").put_voice_connector_emergency_calling_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_emergency_calling_configuration)

```python
# put_voice_connector_emergency_calling_configuration method definition

await def put_voice_connector_emergency_calling_configuration(
    self,
    *,
    VoiceConnectorId: str,
    EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef,  # (1)
) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EmergencyCallingConfigurationTypeDef](./type_defs.md#emergencycallingconfigurationtypedef) 
2. See [:material-code-braces: PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef](./type_defs.md#putvoiceconnectoremergencycallingconfigurationresponsetypedef) 


```python
# put_voice_connector_emergency_calling_configuration method usage example with argument unpacking

kwargs: PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "EmergencyCallingConfiguration": ...,
}

parent.put_voice_connector_emergency_calling_configuration(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef](./type_defs.md#putvoiceconnectoremergencycallingconfigurationrequestrequesttypedef) 

### put\_voice\_connector\_logging\_configuration

Updates a Voice Connector's logging configuration.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").put_voice_connector_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_logging_configuration)

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

kwargs: PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "LoggingConfiguration": ...,
}

parent.put_voice_connector_logging_configuration(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef](./type_defs.md#putvoiceconnectorloggingconfigurationrequestrequesttypedef) 

### put\_voice\_connector\_origination

Updates a Voice Connector's origination settings.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").put_voice_connector_origination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_origination)

```python
# put_voice_connector_origination method definition

await def put_voice_connector_origination(
    self,
    *,
    VoiceConnectorId: str,
    Origination: OriginationTypeDef,  # (1)
) -> PutVoiceConnectorOriginationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OriginationTypeDef](./type_defs.md#originationtypedef) 
2. See [:material-code-braces: PutVoiceConnectorOriginationResponseTypeDef](./type_defs.md#putvoiceconnectororiginationresponsetypedef) 


```python
# put_voice_connector_origination method usage example with argument unpacking

kwargs: PutVoiceConnectorOriginationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "Origination": ...,
}

parent.put_voice_connector_origination(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorOriginationRequestRequestTypeDef](./type_defs.md#putvoiceconnectororiginationrequestrequesttypedef) 

### put\_voice\_connector\_proxy

Puts the specified proxy configuration to the specified Amazon Chime SDK Voice
Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").put_voice_connector_proxy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_proxy)

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

kwargs: PutVoiceConnectorProxyRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "DefaultSessionExpiryMinutes": ...,
    "PhoneNumberPoolCountries": ...,
}

parent.put_voice_connector_proxy(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorProxyRequestRequestTypeDef](./type_defs.md#putvoiceconnectorproxyrequestrequesttypedef) 

### put\_voice\_connector\_streaming\_configuration

Updates a Voice Connector's streaming configuration settings.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").put_voice_connector_streaming_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_streaming_configuration)

```python
# put_voice_connector_streaming_configuration method definition

await def put_voice_connector_streaming_configuration(
    self,
    *,
    VoiceConnectorId: str,
    StreamingConfiguration: StreamingConfigurationTypeDef,  # (1)
) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamingConfigurationTypeDef](./type_defs.md#streamingconfigurationtypedef) 
2. See [:material-code-braces: PutVoiceConnectorStreamingConfigurationResponseTypeDef](./type_defs.md#putvoiceconnectorstreamingconfigurationresponsetypedef) 


```python
# put_voice_connector_streaming_configuration method usage example with argument unpacking

kwargs: PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "StreamingConfiguration": ...,
}

parent.put_voice_connector_streaming_configuration(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef](./type_defs.md#putvoiceconnectorstreamingconfigurationrequestrequesttypedef) 

### put\_voice\_connector\_termination

Updates a Voice Connector's termination settings.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").put_voice_connector_termination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_termination)

```python
# put_voice_connector_termination method definition

await def put_voice_connector_termination(
    self,
    *,
    VoiceConnectorId: str,
    Termination: TerminationTypeDef,  # (1)
) -> PutVoiceConnectorTerminationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TerminationTypeDef](./type_defs.md#terminationtypedef) 
2. See [:material-code-braces: PutVoiceConnectorTerminationResponseTypeDef](./type_defs.md#putvoiceconnectorterminationresponsetypedef) 


```python
# put_voice_connector_termination method usage example with argument unpacking

kwargs: PutVoiceConnectorTerminationRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "Termination": ...,
}

parent.put_voice_connector_termination(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorTerminationRequestRequestTypeDef](./type_defs.md#putvoiceconnectorterminationrequestrequesttypedef) 

### put\_voice\_connector\_termination\_credentials

Updates a Voice Connector's termination credentials.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").put_voice_connector_termination_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.put_voice_connector_termination_credentials)

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

kwargs: PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
}

parent.put_voice_connector_termination_credentials(**kwargs)
```

1. See [:material-code-braces: PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef](./type_defs.md#putvoiceconnectorterminationcredentialsrequestrequesttypedef) 

### restore\_phone\_number

Restores a deleted phone number.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").restore_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.restore_phone_number)

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

kwargs: RestorePhoneNumberRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.restore_phone_number(**kwargs)
```

1. See [:material-code-braces: RestorePhoneNumberRequestRequestTypeDef](./type_defs.md#restorephonenumberrequestrequesttypedef) 

### search\_available\_phone\_numbers

Searches the provisioned phone numbers in an organization.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").search_available_phone_numbers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.search_available_phone_numbers)

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

kwargs: SearchAvailablePhoneNumbersRequestRequestTypeDef = {  # (1)
    "AreaCode": ...,
}

parent.search_available_phone_numbers(**kwargs)
```

1. See [:material-code-braces: SearchAvailablePhoneNumbersRequestRequestTypeDef](./type_defs.md#searchavailablephonenumbersrequestrequesttypedef) 

### start\_speaker\_search\_task

Starts a speaker search task.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").start_speaker_search_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_speaker_search_task)

```python
# start_speaker_search_task method definition

await def start_speaker_search_task(
    self,
    *,
    VoiceConnectorId: str,
    TransactionId: str,
    VoiceProfileDomainId: str,
    ClientRequestToken: str = ...,
    CallLeg: CallLegTypeType = ...,  # (1)
) -> StartSpeakerSearchTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CallLegTypeType](./literals.md#calllegtypetype) 
2. See [:material-code-braces: StartSpeakerSearchTaskResponseTypeDef](./type_defs.md#startspeakersearchtaskresponsetypedef) 


```python
# start_speaker_search_task method usage example with argument unpacking

kwargs: StartSpeakerSearchTaskRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "TransactionId": ...,
    "VoiceProfileDomainId": ...,
}

parent.start_speaker_search_task(**kwargs)
```

1. See [:material-code-braces: StartSpeakerSearchTaskRequestRequestTypeDef](./type_defs.md#startspeakersearchtaskrequestrequesttypedef) 

### start\_voice\_tone\_analysis\_task

Starts a voice tone analysis task.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").start_voice_tone_analysis_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.start_voice_tone_analysis_task)

```python
# start_voice_tone_analysis_task method definition

await def start_voice_tone_analysis_task(
    self,
    *,
    VoiceConnectorId: str,
    TransactionId: str,
    LanguageCode: LanguageCodeType,  # (1)
    ClientRequestToken: str = ...,
) -> StartVoiceToneAnalysisTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: StartVoiceToneAnalysisTaskResponseTypeDef](./type_defs.md#startvoicetoneanalysistaskresponsetypedef) 


```python
# start_voice_tone_analysis_task method usage example with argument unpacking

kwargs: StartVoiceToneAnalysisTaskRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "TransactionId": ...,
    "LanguageCode": ...,
}

parent.start_voice_tone_analysis_task(**kwargs)
```

1. See [:material-code-braces: StartVoiceToneAnalysisTaskRequestRequestTypeDef](./type_defs.md#startvoicetoneanalysistaskrequestrequesttypedef) 

### stop\_speaker\_search\_task

Stops a speaker search task.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").stop_speaker_search_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.stop_speaker_search_task)

```python
# stop_speaker_search_task method definition

await def stop_speaker_search_task(
    self,
    *,
    VoiceConnectorId: str,
    SpeakerSearchTaskId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_speaker_search_task method usage example with argument unpacking

kwargs: StopSpeakerSearchTaskRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "SpeakerSearchTaskId": ...,
}

parent.stop_speaker_search_task(**kwargs)
```

1. See [:material-code-braces: StopSpeakerSearchTaskRequestRequestTypeDef](./type_defs.md#stopspeakersearchtaskrequestrequesttypedef) 

### stop\_voice\_tone\_analysis\_task

Stops a voice tone analysis task.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").stop_voice_tone_analysis_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.stop_voice_tone_analysis_task)

```python
# stop_voice_tone_analysis_task method definition

await def stop_voice_tone_analysis_task(
    self,
    *,
    VoiceConnectorId: str,
    VoiceToneAnalysisTaskId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_voice_tone_analysis_task method usage example with argument unpacking

kwargs: StopVoiceToneAnalysisTaskRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "VoiceToneAnalysisTaskId": ...,
}

parent.stop_voice_tone_analysis_task(**kwargs)
```

1. See [:material-code-braces: StopVoiceToneAnalysisTaskRequestRequestTypeDef](./type_defs.md#stopvoicetoneanalysistaskrequestrequesttypedef) 

### tag\_resource

Adds a tag to the specified resource.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.tag_resource)

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

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from a resource.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.untag_resource)

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

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_global\_settings

Updates global settings for the Amazon Chime SDK Voice Connectors in an AWS
account.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_global_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_global_settings)

```python
# update_global_settings method definition

await def update_global_settings(
    self,
    *,
    VoiceConnector: VoiceConnectorSettingsTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VoiceConnectorSettingsTypeDef](./type_defs.md#voiceconnectorsettingstypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_global_settings method usage example with argument unpacking

kwargs: UpdateGlobalSettingsRequestRequestTypeDef = {  # (1)
    "VoiceConnector": ...,
}

parent.update_global_settings(**kwargs)
```

1. See [:material-code-braces: UpdateGlobalSettingsRequestRequestTypeDef](./type_defs.md#updateglobalsettingsrequestrequesttypedef) 

### update\_phone\_number

Updates phone number details, such as product type, calling name, or phone
number name for the specified phone number
ID.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_phone_number)

```python
# update_phone_number method definition

await def update_phone_number(
    self,
    *,
    PhoneNumberId: str,
    ProductType: PhoneNumberProductTypeType = ...,  # (1)
    CallingName: str = ...,
    Name: str = ...,
) -> UpdatePhoneNumberResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PhoneNumberProductTypeType](./literals.md#phonenumberproducttypetype) 
2. See [:material-code-braces: UpdatePhoneNumberResponseTypeDef](./type_defs.md#updatephonenumberresponsetypedef) 


```python
# update_phone_number method usage example with argument unpacking

kwargs: UpdatePhoneNumberRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.update_phone_number(**kwargs)
```

1. See [:material-code-braces: UpdatePhoneNumberRequestRequestTypeDef](./type_defs.md#updatephonenumberrequestrequesttypedef) 

### update\_phone\_number\_settings

Updates the phone number settings for the administrator's AWS account, such as
the default outbound calling
name.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_phone_number_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_phone_number_settings)

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

kwargs: UpdatePhoneNumberSettingsRequestRequestTypeDef = {  # (1)
    "CallingName": ...,
}

parent.update_phone_number_settings(**kwargs)
```

1. See [:material-code-braces: UpdatePhoneNumberSettingsRequestRequestTypeDef](./type_defs.md#updatephonenumbersettingsrequestrequesttypedef) 

### update\_proxy\_session

Updates the specified proxy session details, such as voice or SMS capabilities.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_proxy_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_proxy_session)

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

kwargs: UpdateProxySessionRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "ProxySessionId": ...,
    "Capabilities": ...,
}

parent.update_proxy_session(**kwargs)
```

1. See [:material-code-braces: UpdateProxySessionRequestRequestTypeDef](./type_defs.md#updateproxysessionrequestrequesttypedef) 

### update\_sip\_media\_application

Updates the details of the specified SIP media application.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_sip_media_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_media_application)

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

kwargs: UpdateSipMediaApplicationRequestRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.update_sip_media_application(**kwargs)
```

1. See [:material-code-braces: UpdateSipMediaApplicationRequestRequestTypeDef](./type_defs.md#updatesipmediaapplicationrequestrequesttypedef) 

### update\_sip\_media\_application\_call

Invokes the AWS Lambda function associated with the SIP media application and
transaction ID in an update
request.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_sip_media_application_call` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_media_application_call)

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

kwargs: UpdateSipMediaApplicationCallRequestRequestTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
    "TransactionId": ...,
    "Arguments": ...,
}

parent.update_sip_media_application_call(**kwargs)
```

1. See [:material-code-braces: UpdateSipMediaApplicationCallRequestRequestTypeDef](./type_defs.md#updatesipmediaapplicationcallrequestrequesttypedef) 

### update\_sip\_rule

Updates the details of the specified SIP rule.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_sip_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_sip_rule)

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

kwargs: UpdateSipRuleRequestRequestTypeDef = {  # (1)
    "SipRuleId": ...,
    "Name": ...,
}

parent.update_sip_rule(**kwargs)
```

1. See [:material-code-braces: UpdateSipRuleRequestRequestTypeDef](./type_defs.md#updatesiprulerequestrequesttypedef) 

### update\_voice\_connector

Updates the details for the specified Amazon Chime SDK Voice Connector.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_voice_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_connector)

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

kwargs: UpdateVoiceConnectorRequestRequestTypeDef = {  # (1)
    "VoiceConnectorId": ...,
    "Name": ...,
    "RequireEncryption": ...,
}

parent.update_voice_connector(**kwargs)
```

1. See [:material-code-braces: UpdateVoiceConnectorRequestRequestTypeDef](./type_defs.md#updatevoiceconnectorrequestrequesttypedef) 

### update\_voice\_connector\_group

Updates the settings for the specified Amazon Chime SDK Voice Connector group.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_voice_connector_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_connector_group)

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

kwargs: UpdateVoiceConnectorGroupRequestRequestTypeDef = {  # (1)
    "VoiceConnectorGroupId": ...,
    "Name": ...,
    "VoiceConnectorItems": ...,
}

parent.update_voice_connector_group(**kwargs)
```

1. See [:material-code-braces: UpdateVoiceConnectorGroupRequestRequestTypeDef](./type_defs.md#updatevoiceconnectorgrouprequestrequesttypedef) 

### update\_voice\_profile

Updates the specified voice profile's voice print and refreshes its expiration
timestamp.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_voice_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile)

```python
# update_voice_profile method definition

await def update_voice_profile(
    self,
    *,
    VoiceProfileId: str,
    SpeakerSearchTaskId: str,
) -> UpdateVoiceProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateVoiceProfileResponseTypeDef](./type_defs.md#updatevoiceprofileresponsetypedef) 


```python
# update_voice_profile method usage example with argument unpacking

kwargs: UpdateVoiceProfileRequestRequestTypeDef = {  # (1)
    "VoiceProfileId": ...,
    "SpeakerSearchTaskId": ...,
}

parent.update_voice_profile(**kwargs)
```

1. See [:material-code-braces: UpdateVoiceProfileRequestRequestTypeDef](./type_defs.md#updatevoiceprofilerequestrequesttypedef) 

### update\_voice\_profile\_domain

Updates the settings for the specified voice profile domain.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").update_voice_profile_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.update_voice_profile_domain)

```python
# update_voice_profile_domain method definition

await def update_voice_profile_domain(
    self,
    *,
    VoiceProfileDomainId: str,
    Name: str = ...,
    Description: str = ...,
) -> UpdateVoiceProfileDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateVoiceProfileDomainResponseTypeDef](./type_defs.md#updatevoiceprofiledomainresponsetypedef) 


```python
# update_voice_profile_domain method usage example with argument unpacking

kwargs: UpdateVoiceProfileDomainRequestRequestTypeDef = {  # (1)
    "VoiceProfileDomainId": ...,
}

parent.update_voice_profile_domain(**kwargs)
```

1. See [:material-code-braces: UpdateVoiceProfileDomainRequestRequestTypeDef](./type_defs.md#updatevoiceprofiledomainrequestrequesttypedef) 

### validate\_e911\_address

Validates an address to be used for 911 calls made with Amazon Chime SDK Voice
Connectors.

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").validate_e911_address` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.validate_e911_address)

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

kwargs: ValidateE911AddressRequestRequestTypeDef = {  # (1)
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

1. See [:material-code-braces: ValidateE911AddressRequestRequestTypeDef](./type_defs.md#validatee911addressrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ChimeSDKVoiceClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#ChimeSDKVoice.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_paginator` method with overloads.

- `client.get_paginator("list_sip_media_applications")` -> [ListSipMediaApplicationsPaginator](./paginators.md#listsipmediaapplicationspaginator)
- `client.get_paginator("list_sip_rules")` -> [ListSipRulesPaginator](./paginators.md#listsiprulespaginator)



