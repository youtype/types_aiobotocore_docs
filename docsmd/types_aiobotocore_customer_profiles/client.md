# CustomerProfilesClient

> [Index](../README.md) > [CustomerProfiles](./README.md) > CustomerProfilesClient

!!! note ""

    Auto-generated documentation for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
    type annotations stubs module [types-aiobotocore-customer-profiles](https://pypi.org/project/types-aiobotocore-customer-profiles/).

## CustomerProfilesClient

Type annotations and code completion for `#!python session.create_client("customer-profiles")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client)

```python
# CustomerProfilesClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_customer_profiles.client import CustomerProfilesClient

session = get_session()
async with session.create_client("customer-profiles") as client:
    client: CustomerProfilesClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("customer-profiles").exceptions` structure.

```python
# CustomerProfilesClient.exceptions usage example

async with session.create_client("customer-profiles") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
        client.ClientError,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python
# CustomerProfilesClient usage type checking example

from types_aiobotocore_customer_profiles.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### add\_profile\_key

Associates a new key value with a specific profile, such as a Contact Record
ContactId.

Type annotations and code completion for `#!python session.create_client("customer-profiles").add_profile_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.add_profile_key)

```python
# add_profile_key method definition

await def add_profile_key(
    self,
    *,
    ProfileId: str,
    KeyName: str,
    Values: Sequence[str],
    DomainName: str,
) -> AddProfileKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AddProfileKeyResponseTypeDef](./type_defs.md#addprofilekeyresponsetypedef) 


```python
# add_profile_key method usage example with argument unpacking

kwargs: AddProfileKeyRequestRequestTypeDef = {  # (1)
    "ProfileId": ...,
    "KeyName": ...,
    "Values": ...,
    "DomainName": ...,
}

parent.add_profile_key(**kwargs)
```

1. See [:material-code-braces: AddProfileKeyRequestRequestTypeDef](./type_defs.md#addprofilekeyrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("customer-profiles").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("customer-profiles").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_calculated\_attribute\_definition

Creates a new calculated attribute definition.

Type annotations and code completion for `#!python session.create_client("customer-profiles").create_calculated_attribute_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_calculated_attribute_definition)

```python
# create_calculated_attribute_definition method definition

await def create_calculated_attribute_definition(
    self,
    *,
    DomainName: str,
    CalculatedAttributeName: str,
    AttributeDetails: AttributeDetailsTypeDef,  # (1)
    Statistic: StatisticType,  # (2)
    DisplayName: str = ...,
    Description: str = ...,
    Conditions: ConditionsTypeDef = ...,  # (3)
    Tags: Mapping[str, str] = ...,
) -> CreateCalculatedAttributeDefinitionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AttributeDetailsTypeDef](./type_defs.md#attributedetailstypedef) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-braces: ConditionsTypeDef](./type_defs.md#conditionstypedef) 
4. See [:material-code-braces: CreateCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#createcalculatedattributedefinitionresponsetypedef) 


```python
# create_calculated_attribute_definition method usage example with argument unpacking

kwargs: CreateCalculatedAttributeDefinitionRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "CalculatedAttributeName": ...,
    "AttributeDetails": ...,
    "Statistic": ...,
}

parent.create_calculated_attribute_definition(**kwargs)
```

1. See [:material-code-braces: CreateCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#createcalculatedattributedefinitionrequestrequesttypedef) 

### create\_domain

Creates a domain, which is a container for all customer data, such as customer
profile attributes, object types, profile keys, and encryption
keys.

Type annotations and code completion for `#!python session.create_client("customer-profiles").create_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_domain)

```python
# create_domain method definition

await def create_domain(
    self,
    *,
    DomainName: str,
    DefaultExpirationDays: int,
    DefaultEncryptionKey: str = ...,
    DeadLetterQueueUrl: str = ...,
    Matching: MatchingRequestTypeDef = ...,  # (1)
    RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> CreateDomainResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MatchingRequestTypeDef](./type_defs.md#matchingrequesttypedef) 
2. See [:material-code-braces: RuleBasedMatchingRequestTypeDef](./type_defs.md#rulebasedmatchingrequesttypedef) 
3. See [:material-code-braces: CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef) 


```python
# create_domain method usage example with argument unpacking

kwargs: CreateDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "DefaultExpirationDays": ...,
}

parent.create_domain(**kwargs)
```

1. See [:material-code-braces: CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef) 

### create\_event\_stream

Creates an event stream, which is a subscription to real-time events, such as
when profiles are created and updated through Amazon Connect Customer
Profiles.

Type annotations and code completion for `#!python session.create_client("customer-profiles").create_event_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_event_stream)

```python
# create_event_stream method definition

await def create_event_stream(
    self,
    *,
    DomainName: str,
    Uri: str,
    EventStreamName: str,
    Tags: Mapping[str, str] = ...,
) -> CreateEventStreamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateEventStreamResponseTypeDef](./type_defs.md#createeventstreamresponsetypedef) 


```python
# create_event_stream method usage example with argument unpacking

kwargs: CreateEventStreamRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Uri": ...,
    "EventStreamName": ...,
}

parent.create_event_stream(**kwargs)
```

1. See [:material-code-braces: CreateEventStreamRequestRequestTypeDef](./type_defs.md#createeventstreamrequestrequesttypedef) 

### create\_integration\_workflow

Creates an integration workflow.

Type annotations and code completion for `#!python session.create_client("customer-profiles").create_integration_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_integration_workflow)

```python
# create_integration_workflow method definition

await def create_integration_workflow(
    self,
    *,
    DomainName: str,
    WorkflowType: WorkflowTypeType,  # (1)
    IntegrationConfig: IntegrationConfigTypeDef,  # (2)
    ObjectTypeName: str,
    RoleArn: str,
    Tags: Mapping[str, str] = ...,
) -> CreateIntegrationWorkflowResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-braces: IntegrationConfigTypeDef](./type_defs.md#integrationconfigtypedef) 
3. See [:material-code-braces: CreateIntegrationWorkflowResponseTypeDef](./type_defs.md#createintegrationworkflowresponsetypedef) 


```python
# create_integration_workflow method usage example with argument unpacking

kwargs: CreateIntegrationWorkflowRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "WorkflowType": ...,
    "IntegrationConfig": ...,
    "ObjectTypeName": ...,
    "RoleArn": ...,
}

parent.create_integration_workflow(**kwargs)
```

1. See [:material-code-braces: CreateIntegrationWorkflowRequestRequestTypeDef](./type_defs.md#createintegrationworkflowrequestrequesttypedef) 

### create\_profile

Creates a standard profile.

Type annotations and code completion for `#!python session.create_client("customer-profiles").create_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_profile)

```python
# create_profile method definition

await def create_profile(
    self,
    *,
    DomainName: str,
    AccountNumber: str = ...,
    AdditionalInformation: str = ...,
    PartyType: PartyTypeType = ...,  # (1)
    BusinessName: str = ...,
    FirstName: str = ...,
    MiddleName: str = ...,
    LastName: str = ...,
    BirthDate: str = ...,
    Gender: GenderType = ...,  # (2)
    PhoneNumber: str = ...,
    MobilePhoneNumber: str = ...,
    HomePhoneNumber: str = ...,
    BusinessPhoneNumber: str = ...,
    EmailAddress: str = ...,
    PersonalEmailAddress: str = ...,
    BusinessEmailAddress: str = ...,
    Address: AddressTypeDef = ...,  # (3)
    ShippingAddress: AddressTypeDef = ...,  # (3)
    MailingAddress: AddressTypeDef = ...,  # (3)
    BillingAddress: AddressTypeDef = ...,  # (3)
    Attributes: Mapping[str, str] = ...,
    PartyTypeString: str = ...,
    GenderString: str = ...,
) -> CreateProfileResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: PartyTypeType](./literals.md#partytypetype) 
2. See [:material-code-brackets: GenderType](./literals.md#gendertype) 
3. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
4. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
5. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
6. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
7. See [:material-code-braces: CreateProfileResponseTypeDef](./type_defs.md#createprofileresponsetypedef) 


```python
# create_profile method usage example with argument unpacking

kwargs: CreateProfileRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.create_profile(**kwargs)
```

1. See [:material-code-braces: CreateProfileRequestRequestTypeDef](./type_defs.md#createprofilerequestrequesttypedef) 

### delete\_calculated\_attribute\_definition

Deletes an existing calculated attribute definition.

Type annotations and code completion for `#!python session.create_client("customer-profiles").delete_calculated_attribute_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_calculated_attribute_definition)

```python
# delete_calculated_attribute_definition method definition

await def delete_calculated_attribute_definition(
    self,
    *,
    DomainName: str,
    CalculatedAttributeName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_calculated_attribute_definition method usage example with argument unpacking

kwargs: DeleteCalculatedAttributeDefinitionRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "CalculatedAttributeName": ...,
}

parent.delete_calculated_attribute_definition(**kwargs)
```

1. See [:material-code-braces: DeleteCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#deletecalculatedattributedefinitionrequestrequesttypedef) 

### delete\_domain

Deletes a specific domain and all of its customer data, such as customer
profile attributes and their related
objects.

Type annotations and code completion for `#!python session.create_client("customer-profiles").delete_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_domain)

```python
# delete_domain method definition

await def delete_domain(
    self,
    *,
    DomainName: str,
) -> DeleteDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDomainResponseTypeDef](./type_defs.md#deletedomainresponsetypedef) 


```python
# delete_domain method usage example with argument unpacking

kwargs: DeleteDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.delete_domain(**kwargs)
```

1. See [:material-code-braces: DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef) 

### delete\_event\_stream

Disables and deletes the specified event stream.

Type annotations and code completion for `#!python session.create_client("customer-profiles").delete_event_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_event_stream)

```python
# delete_event_stream method definition

await def delete_event_stream(
    self,
    *,
    DomainName: str,
    EventStreamName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_event_stream method usage example with argument unpacking

kwargs: DeleteEventStreamRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "EventStreamName": ...,
}

parent.delete_event_stream(**kwargs)
```

1. See [:material-code-braces: DeleteEventStreamRequestRequestTypeDef](./type_defs.md#deleteeventstreamrequestrequesttypedef) 

### delete\_integration

Removes an integration from a specific domain.

Type annotations and code completion for `#!python session.create_client("customer-profiles").delete_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_integration)

```python
# delete_integration method definition

await def delete_integration(
    self,
    *,
    DomainName: str,
    Uri: str,
) -> DeleteIntegrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteIntegrationResponseTypeDef](./type_defs.md#deleteintegrationresponsetypedef) 


```python
# delete_integration method usage example with argument unpacking

kwargs: DeleteIntegrationRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Uri": ...,
}

parent.delete_integration(**kwargs)
```

1. See [:material-code-braces: DeleteIntegrationRequestRequestTypeDef](./type_defs.md#deleteintegrationrequestrequesttypedef) 

### delete\_profile

Deletes the standard customer profile and all data pertaining to the profile.

Type annotations and code completion for `#!python session.create_client("customer-profiles").delete_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile)

```python
# delete_profile method definition

await def delete_profile(
    self,
    *,
    ProfileId: str,
    DomainName: str,
) -> DeleteProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteProfileResponseTypeDef](./type_defs.md#deleteprofileresponsetypedef) 


```python
# delete_profile method usage example with argument unpacking

kwargs: DeleteProfileRequestRequestTypeDef = {  # (1)
    "ProfileId": ...,
    "DomainName": ...,
}

parent.delete_profile(**kwargs)
```

1. See [:material-code-braces: DeleteProfileRequestRequestTypeDef](./type_defs.md#deleteprofilerequestrequesttypedef) 

### delete\_profile\_key

Removes a searchable key from a customer profile.

Type annotations and code completion for `#!python session.create_client("customer-profiles").delete_profile_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile_key)

```python
# delete_profile_key method definition

await def delete_profile_key(
    self,
    *,
    ProfileId: str,
    KeyName: str,
    Values: Sequence[str],
    DomainName: str,
) -> DeleteProfileKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteProfileKeyResponseTypeDef](./type_defs.md#deleteprofilekeyresponsetypedef) 


```python
# delete_profile_key method usage example with argument unpacking

kwargs: DeleteProfileKeyRequestRequestTypeDef = {  # (1)
    "ProfileId": ...,
    "KeyName": ...,
    "Values": ...,
    "DomainName": ...,
}

parent.delete_profile_key(**kwargs)
```

1. See [:material-code-braces: DeleteProfileKeyRequestRequestTypeDef](./type_defs.md#deleteprofilekeyrequestrequesttypedef) 

### delete\_profile\_object

Removes an object associated with a profile of a given ProfileObjectType.

Type annotations and code completion for `#!python session.create_client("customer-profiles").delete_profile_object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile_object)

```python
# delete_profile_object method definition

await def delete_profile_object(
    self,
    *,
    ProfileId: str,
    ProfileObjectUniqueKey: str,
    ObjectTypeName: str,
    DomainName: str,
) -> DeleteProfileObjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteProfileObjectResponseTypeDef](./type_defs.md#deleteprofileobjectresponsetypedef) 


```python
# delete_profile_object method usage example with argument unpacking

kwargs: DeleteProfileObjectRequestRequestTypeDef = {  # (1)
    "ProfileId": ...,
    "ProfileObjectUniqueKey": ...,
    "ObjectTypeName": ...,
    "DomainName": ...,
}

parent.delete_profile_object(**kwargs)
```

1. See [:material-code-braces: DeleteProfileObjectRequestRequestTypeDef](./type_defs.md#deleteprofileobjectrequestrequesttypedef) 

### delete\_profile\_object\_type

Removes a ProfileObjectType from a specific domain as well as removes all the
ProfileObjects of that
type.

Type annotations and code completion for `#!python session.create_client("customer-profiles").delete_profile_object_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_profile_object_type)

```python
# delete_profile_object_type method definition

await def delete_profile_object_type(
    self,
    *,
    DomainName: str,
    ObjectTypeName: str,
) -> DeleteProfileObjectTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteProfileObjectTypeResponseTypeDef](./type_defs.md#deleteprofileobjecttyperesponsetypedef) 


```python
# delete_profile_object_type method usage example with argument unpacking

kwargs: DeleteProfileObjectTypeRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ObjectTypeName": ...,
}

parent.delete_profile_object_type(**kwargs)
```

1. See [:material-code-braces: DeleteProfileObjectTypeRequestRequestTypeDef](./type_defs.md#deleteprofileobjecttyperequestrequesttypedef) 

### delete\_workflow

Deletes the specified workflow and all its corresponding resources.

Type annotations and code completion for `#!python session.create_client("customer-profiles").delete_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.delete_workflow)

```python
# delete_workflow method definition

await def delete_workflow(
    self,
    *,
    DomainName: str,
    WorkflowId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_workflow method usage example with argument unpacking

kwargs: DeleteWorkflowRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "WorkflowId": ...,
}

parent.delete_workflow(**kwargs)
```

1. See [:material-code-braces: DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef) 

### detect\_profile\_object\_type

The process of detecting profile object type mapping by using given objects.

Type annotations and code completion for `#!python session.create_client("customer-profiles").detect_profile_object_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.detect_profile_object_type)

```python
# detect_profile_object_type method definition

await def detect_profile_object_type(
    self,
    *,
    Objects: Sequence[str],
    DomainName: str,
) -> DetectProfileObjectTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DetectProfileObjectTypeResponseTypeDef](./type_defs.md#detectprofileobjecttyperesponsetypedef) 


```python
# detect_profile_object_type method usage example with argument unpacking

kwargs: DetectProfileObjectTypeRequestRequestTypeDef = {  # (1)
    "Objects": ...,
    "DomainName": ...,
}

parent.detect_profile_object_type(**kwargs)
```

1. See [:material-code-braces: DetectProfileObjectTypeRequestRequestTypeDef](./type_defs.md#detectprofileobjecttyperequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("customer-profiles").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.generate_presigned_url)

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


### get\_auto\_merging\_preview

Tests the auto-merging settings of your Identity Resolution Job without merging
your
data.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_auto_merging_preview` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_auto_merging_preview)

```python
# get_auto_merging_preview method definition

await def get_auto_merging_preview(
    self,
    *,
    DomainName: str,
    Consolidation: ConsolidationTypeDef,  # (1)
    ConflictResolution: ConflictResolutionTypeDef,  # (2)
    MinAllowedConfidenceScoreForMerging: float = ...,
) -> GetAutoMergingPreviewResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ConsolidationTypeDef](./type_defs.md#consolidationtypedef) 
2. See [:material-code-braces: ConflictResolutionTypeDef](./type_defs.md#conflictresolutiontypedef) 
3. See [:material-code-braces: GetAutoMergingPreviewResponseTypeDef](./type_defs.md#getautomergingpreviewresponsetypedef) 


```python
# get_auto_merging_preview method usage example with argument unpacking

kwargs: GetAutoMergingPreviewRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Consolidation": ...,
    "ConflictResolution": ...,
}

parent.get_auto_merging_preview(**kwargs)
```

1. See [:material-code-braces: GetAutoMergingPreviewRequestRequestTypeDef](./type_defs.md#getautomergingpreviewrequestrequesttypedef) 

### get\_calculated\_attribute\_definition

Provides more information on a calculated attribute definition for Customer
Profiles.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_calculated_attribute_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_calculated_attribute_definition)

```python
# get_calculated_attribute_definition method definition

await def get_calculated_attribute_definition(
    self,
    *,
    DomainName: str,
    CalculatedAttributeName: str,
) -> GetCalculatedAttributeDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#getcalculatedattributedefinitionresponsetypedef) 


```python
# get_calculated_attribute_definition method usage example with argument unpacking

kwargs: GetCalculatedAttributeDefinitionRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "CalculatedAttributeName": ...,
}

parent.get_calculated_attribute_definition(**kwargs)
```

1. See [:material-code-braces: GetCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#getcalculatedattributedefinitionrequestrequesttypedef) 

### get\_calculated\_attribute\_for\_profile

Retrieve a calculated attribute for a customer profile.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_calculated_attribute_for_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_calculated_attribute_for_profile)

```python
# get_calculated_attribute_for_profile method definition

await def get_calculated_attribute_for_profile(
    self,
    *,
    DomainName: str,
    ProfileId: str,
    CalculatedAttributeName: str,
) -> GetCalculatedAttributeForProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCalculatedAttributeForProfileResponseTypeDef](./type_defs.md#getcalculatedattributeforprofileresponsetypedef) 


```python
# get_calculated_attribute_for_profile method usage example with argument unpacking

kwargs: GetCalculatedAttributeForProfileRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ProfileId": ...,
    "CalculatedAttributeName": ...,
}

parent.get_calculated_attribute_for_profile(**kwargs)
```

1. See [:material-code-braces: GetCalculatedAttributeForProfileRequestRequestTypeDef](./type_defs.md#getcalculatedattributeforprofilerequestrequesttypedef) 

### get\_domain

Returns information about a specific domain.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_domain)

```python
# get_domain method definition

await def get_domain(
    self,
    *,
    DomainName: str,
) -> GetDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDomainResponseTypeDef](./type_defs.md#getdomainresponsetypedef) 


```python
# get_domain method usage example with argument unpacking

kwargs: GetDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.get_domain(**kwargs)
```

1. See [:material-code-braces: GetDomainRequestRequestTypeDef](./type_defs.md#getdomainrequestrequesttypedef) 

### get\_event\_stream

Returns information about the specified event stream in a specific domain.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_event_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_event_stream)

```python
# get_event_stream method definition

await def get_event_stream(
    self,
    *,
    DomainName: str,
    EventStreamName: str,
) -> GetEventStreamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventStreamResponseTypeDef](./type_defs.md#geteventstreamresponsetypedef) 


```python
# get_event_stream method usage example with argument unpacking

kwargs: GetEventStreamRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "EventStreamName": ...,
}

parent.get_event_stream(**kwargs)
```

1. See [:material-code-braces: GetEventStreamRequestRequestTypeDef](./type_defs.md#geteventstreamrequestrequesttypedef) 

### get\_identity\_resolution\_job

Returns information about an Identity Resolution Job in a specific domain.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_identity_resolution_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_identity_resolution_job)

```python
# get_identity_resolution_job method definition

await def get_identity_resolution_job(
    self,
    *,
    DomainName: str,
    JobId: str,
) -> GetIdentityResolutionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIdentityResolutionJobResponseTypeDef](./type_defs.md#getidentityresolutionjobresponsetypedef) 


```python
# get_identity_resolution_job method usage example with argument unpacking

kwargs: GetIdentityResolutionJobRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "JobId": ...,
}

parent.get_identity_resolution_job(**kwargs)
```

1. See [:material-code-braces: GetIdentityResolutionJobRequestRequestTypeDef](./type_defs.md#getidentityresolutionjobrequestrequesttypedef) 

### get\_integration

Returns an integration for a domain.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_integration)

```python
# get_integration method definition

await def get_integration(
    self,
    *,
    DomainName: str,
    Uri: str,
) -> GetIntegrationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIntegrationResponseTypeDef](./type_defs.md#getintegrationresponsetypedef) 


```python
# get_integration method usage example with argument unpacking

kwargs: GetIntegrationRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Uri": ...,
}

parent.get_integration(**kwargs)
```

1. See [:material-code-braces: GetIntegrationRequestRequestTypeDef](./type_defs.md#getintegrationrequestrequesttypedef) 

### get\_matches

Before calling this API, use
[CreateDomain](https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_CreateDomain.html)
or
[UpdateDomain](https://docs.aws.amazon.com/customerprofiles/latest/APIReference/API_UpdateDomain.html)
to enable identity resolution: set `Matching` to
tr...

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_matches` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_matches)

```python
# get_matches method definition

await def get_matches(
    self,
    *,
    DomainName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetMatchesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMatchesResponseTypeDef](./type_defs.md#getmatchesresponsetypedef) 


```python
# get_matches method usage example with argument unpacking

kwargs: GetMatchesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.get_matches(**kwargs)
```

1. See [:material-code-braces: GetMatchesRequestRequestTypeDef](./type_defs.md#getmatchesrequestrequesttypedef) 

### get\_profile\_object\_type

Returns the object types for a specific domain.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_profile_object_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_profile_object_type)

```python
# get_profile_object_type method definition

await def get_profile_object_type(
    self,
    *,
    DomainName: str,
    ObjectTypeName: str,
) -> GetProfileObjectTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProfileObjectTypeResponseTypeDef](./type_defs.md#getprofileobjecttyperesponsetypedef) 


```python
# get_profile_object_type method usage example with argument unpacking

kwargs: GetProfileObjectTypeRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ObjectTypeName": ...,
}

parent.get_profile_object_type(**kwargs)
```

1. See [:material-code-braces: GetProfileObjectTypeRequestRequestTypeDef](./type_defs.md#getprofileobjecttyperequestrequesttypedef) 

### get\_profile\_object\_type\_template

Returns the template information for a specific object type.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_profile_object_type_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_profile_object_type_template)

```python
# get_profile_object_type_template method definition

await def get_profile_object_type_template(
    self,
    *,
    TemplateId: str,
) -> GetProfileObjectTypeTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProfileObjectTypeTemplateResponseTypeDef](./type_defs.md#getprofileobjecttypetemplateresponsetypedef) 


```python
# get_profile_object_type_template method usage example with argument unpacking

kwargs: GetProfileObjectTypeTemplateRequestRequestTypeDef = {  # (1)
    "TemplateId": ...,
}

parent.get_profile_object_type_template(**kwargs)
```

1. See [:material-code-braces: GetProfileObjectTypeTemplateRequestRequestTypeDef](./type_defs.md#getprofileobjecttypetemplaterequestrequesttypedef) 

### get\_similar\_profiles

Returns a set of profiles that belong to the same matching group using the
`matchId` or
`profileId`.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_similar_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_similar_profiles)

```python
# get_similar_profiles method definition

await def get_similar_profiles(
    self,
    *,
    DomainName: str,
    MatchType: MatchTypeType,  # (1)
    SearchKey: str,
    SearchValue: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetSimilarProfilesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MatchTypeType](./literals.md#matchtypetype) 
2. See [:material-code-braces: GetSimilarProfilesResponseTypeDef](./type_defs.md#getsimilarprofilesresponsetypedef) 


```python
# get_similar_profiles method usage example with argument unpacking

kwargs: GetSimilarProfilesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "MatchType": ...,
    "SearchKey": ...,
    "SearchValue": ...,
}

parent.get_similar_profiles(**kwargs)
```

1. See [:material-code-braces: GetSimilarProfilesRequestRequestTypeDef](./type_defs.md#getsimilarprofilesrequestrequesttypedef) 

### get\_workflow

Get details of specified workflow.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_workflow)

```python
# get_workflow method definition

await def get_workflow(
    self,
    *,
    DomainName: str,
    WorkflowId: str,
) -> GetWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef) 


```python
# get_workflow method usage example with argument unpacking

kwargs: GetWorkflowRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "WorkflowId": ...,
}

parent.get_workflow(**kwargs)
```

1. See [:material-code-braces: GetWorkflowRequestRequestTypeDef](./type_defs.md#getworkflowrequestrequesttypedef) 

### get\_workflow\_steps

Get granular list of steps in workflow.

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_workflow_steps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.get_workflow_steps)

```python
# get_workflow_steps method definition

await def get_workflow_steps(
    self,
    *,
    DomainName: str,
    WorkflowId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetWorkflowStepsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowStepsResponseTypeDef](./type_defs.md#getworkflowstepsresponsetypedef) 


```python
# get_workflow_steps method usage example with argument unpacking

kwargs: GetWorkflowStepsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "WorkflowId": ...,
}

parent.get_workflow_steps(**kwargs)
```

1. See [:material-code-braces: GetWorkflowStepsRequestRequestTypeDef](./type_defs.md#getworkflowstepsrequestrequesttypedef) 

### list\_account\_integrations

Lists all of the integrations associated to a specific URI in the AWS account.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_account_integrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_account_integrations)

```python
# list_account_integrations method definition

await def list_account_integrations(
    self,
    *,
    Uri: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    IncludeHidden: bool = ...,
) -> ListAccountIntegrationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccountIntegrationsResponseTypeDef](./type_defs.md#listaccountintegrationsresponsetypedef) 


```python
# list_account_integrations method usage example with argument unpacking

kwargs: ListAccountIntegrationsRequestRequestTypeDef = {  # (1)
    "Uri": ...,
}

parent.list_account_integrations(**kwargs)
```

1. See [:material-code-braces: ListAccountIntegrationsRequestRequestTypeDef](./type_defs.md#listaccountintegrationsrequestrequesttypedef) 

### list\_calculated\_attribute\_definitions

Lists calculated attribute definitions for Customer Profiles See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/customer-profiles-2020-08-15/ListCalculatedAttributeDefinitions).

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_calculated_attribute_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_calculated_attribute_definitions)

```python
# list_calculated_attribute_definitions method definition

await def list_calculated_attribute_definitions(
    self,
    *,
    DomainName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCalculatedAttributeDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCalculatedAttributeDefinitionsResponseTypeDef](./type_defs.md#listcalculatedattributedefinitionsresponsetypedef) 


```python
# list_calculated_attribute_definitions method usage example with argument unpacking

kwargs: ListCalculatedAttributeDefinitionsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_calculated_attribute_definitions(**kwargs)
```

1. See [:material-code-braces: ListCalculatedAttributeDefinitionsRequestRequestTypeDef](./type_defs.md#listcalculatedattributedefinitionsrequestrequesttypedef) 

### list\_calculated\_attributes\_for\_profile

Retrieve a list of calculated attributes for a customer profile.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_calculated_attributes_for_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_calculated_attributes_for_profile)

```python
# list_calculated_attributes_for_profile method definition

await def list_calculated_attributes_for_profile(
    self,
    *,
    DomainName: str,
    ProfileId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListCalculatedAttributesForProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCalculatedAttributesForProfileResponseTypeDef](./type_defs.md#listcalculatedattributesforprofileresponsetypedef) 


```python
# list_calculated_attributes_for_profile method usage example with argument unpacking

kwargs: ListCalculatedAttributesForProfileRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ProfileId": ...,
}

parent.list_calculated_attributes_for_profile(**kwargs)
```

1. See [:material-code-braces: ListCalculatedAttributesForProfileRequestRequestTypeDef](./type_defs.md#listcalculatedattributesforprofilerequestrequesttypedef) 

### list\_domains

Returns a list of all the domains for an AWS account that have been created.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_domains)

```python
# list_domains method definition

await def list_domains(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDomainsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 


```python
# list_domains method usage example with argument unpacking

kwargs: ListDomainsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_domains(**kwargs)
```

1. See [:material-code-braces: ListDomainsRequestRequestTypeDef](./type_defs.md#listdomainsrequestrequesttypedef) 

### list\_event\_streams

Returns a list of all the event streams in a specific domain.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_event_streams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_event_streams)

```python
# list_event_streams method definition

await def list_event_streams(
    self,
    *,
    DomainName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEventStreamsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventStreamsResponseTypeDef](./type_defs.md#listeventstreamsresponsetypedef) 


```python
# list_event_streams method usage example with argument unpacking

kwargs: ListEventStreamsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_event_streams(**kwargs)
```

1. See [:material-code-braces: ListEventStreamsRequestRequestTypeDef](./type_defs.md#listeventstreamsrequestrequesttypedef) 

### list\_identity\_resolution\_jobs

Lists all of the Identity Resolution Jobs in your domain.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_identity_resolution_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_identity_resolution_jobs)

```python
# list_identity_resolution_jobs method definition

await def list_identity_resolution_jobs(
    self,
    *,
    DomainName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListIdentityResolutionJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIdentityResolutionJobsResponseTypeDef](./type_defs.md#listidentityresolutionjobsresponsetypedef) 


```python
# list_identity_resolution_jobs method usage example with argument unpacking

kwargs: ListIdentityResolutionJobsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_identity_resolution_jobs(**kwargs)
```

1. See [:material-code-braces: ListIdentityResolutionJobsRequestRequestTypeDef](./type_defs.md#listidentityresolutionjobsrequestrequesttypedef) 

### list\_integrations

Lists all of the integrations in your domain.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_integrations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_integrations)

```python
# list_integrations method definition

await def list_integrations(
    self,
    *,
    DomainName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    IncludeHidden: bool = ...,
) -> ListIntegrationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIntegrationsResponseTypeDef](./type_defs.md#listintegrationsresponsetypedef) 


```python
# list_integrations method usage example with argument unpacking

kwargs: ListIntegrationsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_integrations(**kwargs)
```

1. See [:material-code-braces: ListIntegrationsRequestRequestTypeDef](./type_defs.md#listintegrationsrequestrequesttypedef) 

### list\_profile\_object\_type\_templates

Lists all of the template information for object types.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_profile_object_type_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_object_type_templates)

```python
# list_profile_object_type_templates method definition

await def list_profile_object_type_templates(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListProfileObjectTypeTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProfileObjectTypeTemplatesResponseTypeDef](./type_defs.md#listprofileobjecttypetemplatesresponsetypedef) 


```python
# list_profile_object_type_templates method usage example with argument unpacking

kwargs: ListProfileObjectTypeTemplatesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_profile_object_type_templates(**kwargs)
```

1. See [:material-code-braces: ListProfileObjectTypeTemplatesRequestRequestTypeDef](./type_defs.md#listprofileobjecttypetemplatesrequestrequesttypedef) 

### list\_profile\_object\_types

Lists all of the templates available within the service.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_profile_object_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_object_types)

```python
# list_profile_object_types method definition

await def list_profile_object_types(
    self,
    *,
    DomainName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListProfileObjectTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListProfileObjectTypesResponseTypeDef](./type_defs.md#listprofileobjecttypesresponsetypedef) 


```python
# list_profile_object_types method usage example with argument unpacking

kwargs: ListProfileObjectTypesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_profile_object_types(**kwargs)
```

1. See [:material-code-braces: ListProfileObjectTypesRequestRequestTypeDef](./type_defs.md#listprofileobjecttypesrequestrequesttypedef) 

### list\_profile\_objects

Returns a list of objects associated with a profile of a given
ProfileObjectType.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_profile_objects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_profile_objects)

```python
# list_profile_objects method definition

await def list_profile_objects(
    self,
    *,
    DomainName: str,
    ObjectTypeName: str,
    ProfileId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    ObjectFilter: ObjectFilterTypeDef = ...,  # (1)
) -> ListProfileObjectsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ObjectFilterTypeDef](./type_defs.md#objectfiltertypedef) 
2. See [:material-code-braces: ListProfileObjectsResponseTypeDef](./type_defs.md#listprofileobjectsresponsetypedef) 


```python
# list_profile_objects method usage example with argument unpacking

kwargs: ListProfileObjectsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ObjectTypeName": ...,
    "ProfileId": ...,
}

parent.list_profile_objects(**kwargs)
```

1. See [:material-code-braces: ListProfileObjectsRequestRequestTypeDef](./type_defs.md#listprofileobjectsrequestrequesttypedef) 

### list\_rule\_based\_matches

Returns a set of `MatchIds` that belong to the given domain.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_rule_based_matches` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_rule_based_matches)

```python
# list_rule_based_matches method definition

await def list_rule_based_matches(
    self,
    *,
    DomainName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRuleBasedMatchesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRuleBasedMatchesResponseTypeDef](./type_defs.md#listrulebasedmatchesresponsetypedef) 


```python
# list_rule_based_matches method usage example with argument unpacking

kwargs: ListRuleBasedMatchesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_rule_based_matches(**kwargs)
```

1. See [:material-code-braces: ListRuleBasedMatchesRequestRequestTypeDef](./type_defs.md#listrulebasedmatchesrequestrequesttypedef) 

### list\_tags\_for\_resource

Displays the tags associated with an Amazon Connect Customer Profiles resource.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_tags_for_resource)

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

### list\_workflows

Query to list all workflows.

Type annotations and code completion for `#!python session.create_client("customer-profiles").list_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.list_workflows)

```python
# list_workflows method definition

await def list_workflows(
    self,
    *,
    DomainName: str,
    WorkflowType: WorkflowTypeType = ...,  # (1)
    Status: StatusType = ...,  # (2)
    QueryStartDate: TimestampTypeDef = ...,
    QueryEndDate: TimestampTypeDef = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListWorkflowsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


```python
# list_workflows method usage example with argument unpacking

kwargs: ListWorkflowsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_workflows(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef) 

### merge\_profiles

Runs an AWS Lambda job that does the following: * All the profileKeys in the
`ProfileToBeMerged` will be moved to the main
profile.

Type annotations and code completion for `#!python session.create_client("customer-profiles").merge_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.merge_profiles)

```python
# merge_profiles method definition

await def merge_profiles(
    self,
    *,
    DomainName: str,
    MainProfileId: str,
    ProfileIdsToBeMerged: Sequence[str],
    FieldSourceProfileIds: FieldSourceProfileIdsTypeDef = ...,  # (1)
) -> MergeProfilesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FieldSourceProfileIdsTypeDef](./type_defs.md#fieldsourceprofileidstypedef) 
2. See [:material-code-braces: MergeProfilesResponseTypeDef](./type_defs.md#mergeprofilesresponsetypedef) 


```python
# merge_profiles method usage example with argument unpacking

kwargs: MergeProfilesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "MainProfileId": ...,
    "ProfileIdsToBeMerged": ...,
}

parent.merge_profiles(**kwargs)
```

1. See [:material-code-braces: MergeProfilesRequestRequestTypeDef](./type_defs.md#mergeprofilesrequestrequesttypedef) 

### put\_integration

Adds an integration between the service and a third-party service, which
includes Amazon AppFlow and Amazon
Connect.

Type annotations and code completion for `#!python session.create_client("customer-profiles").put_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_integration)

```python
# put_integration method definition

await def put_integration(
    self,
    *,
    DomainName: str,
    Uri: str = ...,
    ObjectTypeName: str = ...,
    Tags: Mapping[str, str] = ...,
    FlowDefinition: FlowDefinitionTypeDef = ...,  # (1)
    ObjectTypeNames: Mapping[str, str] = ...,
    RoleArn: str = ...,
) -> PutIntegrationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef) 
2. See [:material-code-braces: PutIntegrationResponseTypeDef](./type_defs.md#putintegrationresponsetypedef) 


```python
# put_integration method usage example with argument unpacking

kwargs: PutIntegrationRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.put_integration(**kwargs)
```

1. See [:material-code-braces: PutIntegrationRequestRequestTypeDef](./type_defs.md#putintegrationrequestrequesttypedef) 

### put\_profile\_object

Adds additional objects to customer profiles of a given ObjectType.

Type annotations and code completion for `#!python session.create_client("customer-profiles").put_profile_object` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object)

```python
# put_profile_object method definition

await def put_profile_object(
    self,
    *,
    ObjectTypeName: str,
    Object: str,
    DomainName: str,
) -> PutProfileObjectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutProfileObjectResponseTypeDef](./type_defs.md#putprofileobjectresponsetypedef) 


```python
# put_profile_object method usage example with argument unpacking

kwargs: PutProfileObjectRequestRequestTypeDef = {  # (1)
    "ObjectTypeName": ...,
    "Object": ...,
    "DomainName": ...,
}

parent.put_profile_object(**kwargs)
```

1. See [:material-code-braces: PutProfileObjectRequestRequestTypeDef](./type_defs.md#putprofileobjectrequestrequesttypedef) 

### put\_profile\_object\_type

Defines a ProfileObjectType.

Type annotations and code completion for `#!python session.create_client("customer-profiles").put_profile_object_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)

```python
# put_profile_object_type method definition

await def put_profile_object_type(
    self,
    *,
    DomainName: str,
    ObjectTypeName: str,
    Description: str,
    TemplateId: str = ...,
    ExpirationDays: int = ...,
    EncryptionKey: str = ...,
    AllowProfileCreation: bool = ...,
    SourceLastUpdatedTimestampFormat: str = ...,
    MaxProfileObjectCount: int = ...,
    Fields: Mapping[str, ObjectTypeFieldTypeDef] = ...,  # (1)
    Keys: Mapping[str, Sequence[ObjectTypeKeyUnionTypeDef]] = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> PutProfileObjectTypeResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ObjectTypeFieldTypeDef](./type_defs.md#objecttypefieldtypedef) 
2. See [:material-code-braces: ObjectTypeKeyTypeDef](./type_defs.md#objecttypekeytypedef) [:material-code-braces: ObjectTypeKeyOutputTypeDef](./type_defs.md#objecttypekeyoutputtypedef) 
3. See [:material-code-braces: PutProfileObjectTypeResponseTypeDef](./type_defs.md#putprofileobjecttyperesponsetypedef) 


```python
# put_profile_object_type method usage example with argument unpacking

kwargs: PutProfileObjectTypeRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ObjectTypeName": ...,
    "Description": ...,
}

parent.put_profile_object_type(**kwargs)
```

1. See [:material-code-braces: PutProfileObjectTypeRequestRequestTypeDef](./type_defs.md#putprofileobjecttyperequestrequesttypedef) 

### search\_profiles

Searches for profiles within a specific domain using one or more predefined
search keys (e.g., _fullName, _phone, _email, _account, etc.) and/or
custom-defined search
keys.

Type annotations and code completion for `#!python session.create_client("customer-profiles").search_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.search_profiles)

```python
# search_profiles method definition

await def search_profiles(
    self,
    *,
    DomainName: str,
    KeyName: str,
    Values: Sequence[str],
    NextToken: str = ...,
    MaxResults: int = ...,
    AdditionalSearchKeys: Sequence[AdditionalSearchKeyTypeDef] = ...,  # (1)
    LogicalOperator: LogicalOperatorType = ...,  # (2)
) -> SearchProfilesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AdditionalSearchKeyTypeDef](./type_defs.md#additionalsearchkeytypedef) 
2. See [:material-code-brackets: LogicalOperatorType](./literals.md#logicaloperatortype) 
3. See [:material-code-braces: SearchProfilesResponseTypeDef](./type_defs.md#searchprofilesresponsetypedef) 


```python
# search_profiles method usage example with argument unpacking

kwargs: SearchProfilesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "KeyName": ...,
    "Values": ...,
}

parent.search_profiles(**kwargs)
```

1. See [:material-code-braces: SearchProfilesRequestRequestTypeDef](./type_defs.md#searchprofilesrequestrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified Amazon Connect
Customer Profiles
resource.

Type annotations and code completion for `#!python session.create_client("customer-profiles").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.tag_resource)

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

Removes one or more tags from the specified Amazon Connect Customer Profiles
resource.

Type annotations and code completion for `#!python session.create_client("customer-profiles").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.untag_resource)

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

### update\_calculated\_attribute\_definition

Updates an existing calculated attribute definition.

Type annotations and code completion for `#!python session.create_client("customer-profiles").update_calculated_attribute_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_calculated_attribute_definition)

```python
# update_calculated_attribute_definition method definition

await def update_calculated_attribute_definition(
    self,
    *,
    DomainName: str,
    CalculatedAttributeName: str,
    DisplayName: str = ...,
    Description: str = ...,
    Conditions: ConditionsTypeDef = ...,  # (1)
) -> UpdateCalculatedAttributeDefinitionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConditionsTypeDef](./type_defs.md#conditionstypedef) 
2. See [:material-code-braces: UpdateCalculatedAttributeDefinitionResponseTypeDef](./type_defs.md#updatecalculatedattributedefinitionresponsetypedef) 


```python
# update_calculated_attribute_definition method usage example with argument unpacking

kwargs: UpdateCalculatedAttributeDefinitionRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "CalculatedAttributeName": ...,
}

parent.update_calculated_attribute_definition(**kwargs)
```

1. See [:material-code-braces: UpdateCalculatedAttributeDefinitionRequestRequestTypeDef](./type_defs.md#updatecalculatedattributedefinitionrequestrequesttypedef) 

### update\_domain

Updates the properties of a domain, including creating or selecting a dead
letter queue or an encryption
key.

Type annotations and code completion for `#!python session.create_client("customer-profiles").update_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_domain)

```python
# update_domain method definition

await def update_domain(
    self,
    *,
    DomainName: str,
    DefaultExpirationDays: int = ...,
    DefaultEncryptionKey: str = ...,
    DeadLetterQueueUrl: str = ...,
    Matching: MatchingRequestTypeDef = ...,  # (1)
    RuleBasedMatching: RuleBasedMatchingRequestTypeDef = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> UpdateDomainResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MatchingRequestTypeDef](./type_defs.md#matchingrequesttypedef) 
2. See [:material-code-braces: RuleBasedMatchingRequestTypeDef](./type_defs.md#rulebasedmatchingrequesttypedef) 
3. See [:material-code-braces: UpdateDomainResponseTypeDef](./type_defs.md#updatedomainresponsetypedef) 


```python
# update_domain method usage example with argument unpacking

kwargs: UpdateDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.update_domain(**kwargs)
```

1. See [:material-code-braces: UpdateDomainRequestRequestTypeDef](./type_defs.md#updatedomainrequestrequesttypedef) 

### update\_profile

Updates the properties of a profile.

Type annotations and code completion for `#!python session.create_client("customer-profiles").update_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_profile)

```python
# update_profile method definition

await def update_profile(
    self,
    *,
    DomainName: str,
    ProfileId: str,
    AdditionalInformation: str = ...,
    AccountNumber: str = ...,
    PartyType: PartyTypeType = ...,  # (1)
    BusinessName: str = ...,
    FirstName: str = ...,
    MiddleName: str = ...,
    LastName: str = ...,
    BirthDate: str = ...,
    Gender: GenderType = ...,  # (2)
    PhoneNumber: str = ...,
    MobilePhoneNumber: str = ...,
    HomePhoneNumber: str = ...,
    BusinessPhoneNumber: str = ...,
    EmailAddress: str = ...,
    PersonalEmailAddress: str = ...,
    BusinessEmailAddress: str = ...,
    Address: UpdateAddressTypeDef = ...,  # (3)
    ShippingAddress: UpdateAddressTypeDef = ...,  # (3)
    MailingAddress: UpdateAddressTypeDef = ...,  # (3)
    BillingAddress: UpdateAddressTypeDef = ...,  # (3)
    Attributes: Mapping[str, str] = ...,
    PartyTypeString: str = ...,
    GenderString: str = ...,
) -> UpdateProfileResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: PartyTypeType](./literals.md#partytypetype) 
2. See [:material-code-brackets: GenderType](./literals.md#gendertype) 
3. See [:material-code-braces: UpdateAddressTypeDef](./type_defs.md#updateaddresstypedef) 
4. See [:material-code-braces: UpdateAddressTypeDef](./type_defs.md#updateaddresstypedef) 
5. See [:material-code-braces: UpdateAddressTypeDef](./type_defs.md#updateaddresstypedef) 
6. See [:material-code-braces: UpdateAddressTypeDef](./type_defs.md#updateaddresstypedef) 
7. See [:material-code-braces: UpdateProfileResponseTypeDef](./type_defs.md#updateprofileresponsetypedef) 


```python
# update_profile method usage example with argument unpacking

kwargs: UpdateProfileRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ProfileId": ...,
}

parent.update_profile(**kwargs)
```

1. See [:material-code-braces: UpdateProfileRequestRequestTypeDef](./type_defs.md#updateprofilerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("customer-profiles").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CustomerProfilesClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("customer-profiles").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator` method with overloads.

- `client.get_paginator("list_event_streams")` -> [ListEventStreamsPaginator](./paginators.md#listeventstreamspaginator)



