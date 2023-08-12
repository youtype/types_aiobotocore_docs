# ConnectClient

> [Index](../README.md) > [Connect](./README.md) > ConnectClient

!!! note ""

    Auto-generated documentation for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
    type annotations stubs module [types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

## ConnectClient

Type annotations and code completion for `#!python session.create_client("connect")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client)

```python
ConnectClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_connect.client import ConnectClient

session = get_session()
async with session.create_client("connect") as client:
    client: ConnectClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("connect").exceptions` structure.

```python
ConnectClient.exceptions usage example

async with session.create_client("connect") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ContactFlowNotPublishedException,
        client.ContactNotFoundException,
        client.DestinationNotAllowedException,
        client.DuplicateResourceException,
        client.IdempotencyException,
        client.InternalServiceException,
        client.InvalidContactFlowException,
        client.InvalidContactFlowModuleException,
        client.InvalidParameterException,
        client.InvalidRequestException,
        client.LimitExceededException,
        client.MaximumResultReturnedException,
        client.OutboundContactNotPermittedException,
        client.PropertyValidationException,
        client.ResourceConflictException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.ResourceNotReadyException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.UserNotFoundException,
    ) as e:
        print(e)
```

```python
ConnectClient usage type checking example

from types_aiobotocore_connect.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### activate\_evaluation\_form

Activates an evaluation form in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").activate_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.activate_evaluation_form)

```python
# activate_evaluation_form method definition

await def activate_evaluation_form(
    self,
    *,
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
) -> ActivateEvaluationFormResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ActivateEvaluationFormResponseTypeDef](./type_defs.md#activateevaluationformresponsetypedef) 


```python
# activate_evaluation_form method usage example with argument unpacking

kwargs: ActivateEvaluationFormRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationFormId": ...,
    "EvaluationFormVersion": ...,
}

parent.activate_evaluation_form(**kwargs)
```

1. See [:material-code-braces: ActivateEvaluationFormRequestRequestTypeDef](./type_defs.md#activateevaluationformrequestrequesttypedef) 

### associate\_approved\_origin

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").associate_approved_origin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_approved_origin)

```python
# associate_approved_origin method definition

await def associate_approved_origin(
    self,
    *,
    InstanceId: str,
    Origin: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_approved_origin method usage example with argument unpacking

kwargs: AssociateApprovedOriginRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Origin": ...,
}

parent.associate_approved_origin(**kwargs)
```

1. See [:material-code-braces: AssociateApprovedOriginRequestRequestTypeDef](./type_defs.md#associateapprovedoriginrequestrequesttypedef) 

### associate\_bot

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").associate_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_bot)

```python
# associate_bot method definition

await def associate_bot(
    self,
    *,
    InstanceId: str,
    LexBot: LexBotTypeDef = ...,  # (1)
    LexV2Bot: LexV2BotTypeDef = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: LexV2BotTypeDef](./type_defs.md#lexv2bottypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_bot method usage example with argument unpacking

kwargs: AssociateBotRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.associate_bot(**kwargs)
```

1. See [:material-code-braces: AssociateBotRequestRequestTypeDef](./type_defs.md#associatebotrequestrequesttypedef) 

### associate\_default\_vocabulary

Associates an existing vocabulary as the default.

Type annotations and code completion for `#!python session.create_client("connect").associate_default_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_default_vocabulary)

```python
# associate_default_vocabulary method definition

await def associate_default_vocabulary(
    self,
    *,
    InstanceId: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    VocabularyId: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 


```python
# associate_default_vocabulary method usage example with argument unpacking

kwargs: AssociateDefaultVocabularyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "LanguageCode": ...,
}

parent.associate_default_vocabulary(**kwargs)
```

1. See [:material-code-braces: AssociateDefaultVocabularyRequestRequestTypeDef](./type_defs.md#associatedefaultvocabularyrequestrequesttypedef) 

### associate\_instance\_storage\_config

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").associate_instance_storage_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_instance_storage_config)

```python
# associate_instance_storage_config method definition

await def associate_instance_storage_config(
    self,
    *,
    InstanceId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    StorageConfig: InstanceStorageConfigTypeDef,  # (2)
) -> AssociateInstanceStorageConfigResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef) 
3. See [:material-code-braces: AssociateInstanceStorageConfigResponseTypeDef](./type_defs.md#associateinstancestorageconfigresponsetypedef) 


```python
# associate_instance_storage_config method usage example with argument unpacking

kwargs: AssociateInstanceStorageConfigRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ResourceType": ...,
    "StorageConfig": ...,
}

parent.associate_instance_storage_config(**kwargs)
```

1. See [:material-code-braces: AssociateInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#associateinstancestorageconfigrequestrequesttypedef) 

### associate\_lambda\_function

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").associate_lambda_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_lambda_function)

```python
# associate_lambda_function method definition

await def associate_lambda_function(
    self,
    *,
    InstanceId: str,
    FunctionArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_lambda_function method usage example with argument unpacking

kwargs: AssociateLambdaFunctionRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "FunctionArn": ...,
}

parent.associate_lambda_function(**kwargs)
```

1. See [:material-code-braces: AssociateLambdaFunctionRequestRequestTypeDef](./type_defs.md#associatelambdafunctionrequestrequesttypedef) 

### associate\_lex\_bot

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").associate_lex_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_lex_bot)

```python
# associate_lex_bot method definition

await def associate_lex_bot(
    self,
    *,
    InstanceId: str,
    LexBot: LexBotTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_lex_bot method usage example with argument unpacking

kwargs: AssociateLexBotRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "LexBot": ...,
}

parent.associate_lex_bot(**kwargs)
```

1. See [:material-code-braces: AssociateLexBotRequestRequestTypeDef](./type_defs.md#associatelexbotrequestrequesttypedef) 

### associate\_phone\_number\_contact\_flow

Associates a flow with a phone number claimed to your Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").associate_phone_number_contact_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_phone_number_contact_flow)

```python
# associate_phone_number_contact_flow method definition

await def associate_phone_number_contact_flow(
    self,
    *,
    PhoneNumberId: str,
    InstanceId: str,
    ContactFlowId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_phone_number_contact_flow method usage example with argument unpacking

kwargs: AssociatePhoneNumberContactFlowRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
    "InstanceId": ...,
    "ContactFlowId": ...,
}

parent.associate_phone_number_contact_flow(**kwargs)
```

1. See [:material-code-braces: AssociatePhoneNumberContactFlowRequestRequestTypeDef](./type_defs.md#associatephonenumbercontactflowrequestrequesttypedef) 

### associate\_queue\_quick\_connects

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").associate_queue_quick_connects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_queue_quick_connects)

```python
# associate_queue_quick_connects method definition

await def associate_queue_quick_connects(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    QuickConnectIds: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_queue_quick_connects method usage example with argument unpacking

kwargs: AssociateQueueQuickConnectsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
    "QuickConnectIds": ...,
}

parent.associate_queue_quick_connects(**kwargs)
```

1. See [:material-code-braces: AssociateQueueQuickConnectsRequestRequestTypeDef](./type_defs.md#associatequeuequickconnectsrequestrequesttypedef) 

### associate\_routing\_profile\_queues

Associates a set of queues with a routing profile.

Type annotations and code completion for `#!python session.create_client("connect").associate_routing_profile_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_routing_profile_queues)

```python
# associate_routing_profile_queues method definition

await def associate_routing_profile_queues(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_routing_profile_queues method usage example with argument unpacking

kwargs: AssociateRoutingProfileQueuesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
    "QueueConfigs": ...,
}

parent.associate_routing_profile_queues(**kwargs)
```

1. See [:material-code-braces: AssociateRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#associateroutingprofilequeuesrequestrequesttypedef) 

### associate\_security\_key

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").associate_security_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_security_key)

```python
# associate_security_key method definition

await def associate_security_key(
    self,
    *,
    InstanceId: str,
    Key: str,
) -> AssociateSecurityKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateSecurityKeyResponseTypeDef](./type_defs.md#associatesecuritykeyresponsetypedef) 


```python
# associate_security_key method usage example with argument unpacking

kwargs: AssociateSecurityKeyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Key": ...,
}

parent.associate_security_key(**kwargs)
```

1. See [:material-code-braces: AssociateSecurityKeyRequestRequestTypeDef](./type_defs.md#associatesecuritykeyrequestrequesttypedef) 

### associate\_traffic\_distribution\_group\_user

Associates an agent with a traffic distribution group.

Type annotations and code completion for `#!python session.create_client("connect").associate_traffic_distribution_group_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.associate_traffic_distribution_group_user)

```python
# associate_traffic_distribution_group_user method definition

await def associate_traffic_distribution_group_user(
    self,
    *,
    TrafficDistributionGroupId: str,
    UserId: str,
    InstanceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_traffic_distribution_group_user method usage example with argument unpacking

kwargs: AssociateTrafficDistributionGroupUserRequestRequestTypeDef = {  # (1)
    "TrafficDistributionGroupId": ...,
    "UserId": ...,
    "InstanceId": ...,
}

parent.associate_traffic_distribution_group_user(**kwargs)
```

1. See [:material-code-braces: AssociateTrafficDistributionGroupUserRequestRequestTypeDef](./type_defs.md#associatetrafficdistributiongroupuserrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("connect").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### claim\_phone\_number

Claims an available phone number to your Amazon Connect instance or traffic
distribution group.

Type annotations and code completion for `#!python session.create_client("connect").claim_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.claim_phone_number)

```python
# claim_phone_number method definition

await def claim_phone_number(
    self,
    *,
    TargetArn: str,
    PhoneNumber: str,
    PhoneNumberDescription: str = ...,
    Tags: Mapping[str, str] = ...,
    ClientToken: str = ...,
) -> ClaimPhoneNumberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClaimPhoneNumberResponseTypeDef](./type_defs.md#claimphonenumberresponsetypedef) 


```python
# claim_phone_number method usage example with argument unpacking

kwargs: ClaimPhoneNumberRequestRequestTypeDef = {  # (1)
    "TargetArn": ...,
    "PhoneNumber": ...,
}

parent.claim_phone_number(**kwargs)
```

1. See [:material-code-braces: ClaimPhoneNumberRequestRequestTypeDef](./type_defs.md#claimphonenumberrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("connect").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_agent\_status

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").create_agent_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_agent_status)

```python
# create_agent_status method definition

await def create_agent_status(
    self,
    *,
    InstanceId: str,
    Name: str,
    State: AgentStatusStateType,  # (1)
    Description: str = ...,
    DisplayOrder: int = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateAgentStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AgentStatusStateType](./literals.md#agentstatusstatetype) 
2. See [:material-code-braces: CreateAgentStatusResponseTypeDef](./type_defs.md#createagentstatusresponsetypedef) 


```python
# create_agent_status method usage example with argument unpacking

kwargs: CreateAgentStatusRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "State": ...,
}

parent.create_agent_status(**kwargs)
```

1. See [:material-code-braces: CreateAgentStatusRequestRequestTypeDef](./type_defs.md#createagentstatusrequestrequesttypedef) 

### create\_contact\_flow

Creates a flow for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_contact_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow)

```python
# create_contact_flow method definition

await def create_contact_flow(
    self,
    *,
    InstanceId: str,
    Name: str,
    Type: ContactFlowTypeType,  # (1)
    Content: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateContactFlowResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-braces: CreateContactFlowResponseTypeDef](./type_defs.md#createcontactflowresponsetypedef) 


```python
# create_contact_flow method usage example with argument unpacking

kwargs: CreateContactFlowRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "Type": ...,
    "Content": ...,
}

parent.create_contact_flow(**kwargs)
```

1. See [:material-code-braces: CreateContactFlowRequestRequestTypeDef](./type_defs.md#createcontactflowrequestrequesttypedef) 

### create\_contact\_flow\_module

Creates a flow module for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_contact_flow_module` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_contact_flow_module)

```python
# create_contact_flow_module method definition

await def create_contact_flow_module(
    self,
    *,
    InstanceId: str,
    Name: str,
    Content: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
    ClientToken: str = ...,
) -> CreateContactFlowModuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateContactFlowModuleResponseTypeDef](./type_defs.md#createcontactflowmoduleresponsetypedef) 


```python
# create_contact_flow_module method usage example with argument unpacking

kwargs: CreateContactFlowModuleRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "Content": ...,
}

parent.create_contact_flow_module(**kwargs)
```

1. See [:material-code-braces: CreateContactFlowModuleRequestRequestTypeDef](./type_defs.md#createcontactflowmodulerequestrequesttypedef) 

### create\_evaluation\_form

Creates an evaluation form in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_evaluation_form)

```python
# create_evaluation_form method definition

await def create_evaluation_form(
    self,
    *,
    InstanceId: str,
    Title: str,
    Items: Sequence[EvaluationFormItemTypeDef],  # (1)
    Description: str = ...,
    ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,  # (2)
    ClientToken: str = ...,
) -> CreateEvaluationFormResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) 
2. See [:material-code-braces: EvaluationFormScoringStrategyTypeDef](./type_defs.md#evaluationformscoringstrategytypedef) 
3. See [:material-code-braces: CreateEvaluationFormResponseTypeDef](./type_defs.md#createevaluationformresponsetypedef) 


```python
# create_evaluation_form method usage example with argument unpacking

kwargs: CreateEvaluationFormRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Title": ...,
    "Items": ...,
}

parent.create_evaluation_form(**kwargs)
```

1. See [:material-code-braces: CreateEvaluationFormRequestRequestTypeDef](./type_defs.md#createevaluationformrequestrequesttypedef) 

### create\_hours\_of\_operation

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").create_hours_of_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_hours_of_operation)

```python
# create_hours_of_operation method definition

await def create_hours_of_operation(
    self,
    *,
    InstanceId: str,
    Name: str,
    TimeZone: str,
    Config: Sequence[HoursOfOperationConfigTypeDef],  # (1)
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateHoursOfOperationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HoursOfOperationConfigTypeDef](./type_defs.md#hoursofoperationconfigtypedef) 
2. See [:material-code-braces: CreateHoursOfOperationResponseTypeDef](./type_defs.md#createhoursofoperationresponsetypedef) 


```python
# create_hours_of_operation method usage example with argument unpacking

kwargs: CreateHoursOfOperationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "TimeZone": ...,
    "Config": ...,
}

parent.create_hours_of_operation(**kwargs)
```

1. See [:material-code-braces: CreateHoursOfOperationRequestRequestTypeDef](./type_defs.md#createhoursofoperationrequestrequesttypedef) 

### create\_instance

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").create_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_instance)

```python
# create_instance method definition

await def create_instance(
    self,
    *,
    IdentityManagementType: DirectoryTypeType,  # (1)
    InboundCallsEnabled: bool,
    OutboundCallsEnabled: bool,
    ClientToken: str = ...,
    InstanceAlias: str = ...,
    DirectoryId: str = ...,
) -> CreateInstanceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DirectoryTypeType](./literals.md#directorytypetype) 
2. See [:material-code-braces: CreateInstanceResponseTypeDef](./type_defs.md#createinstanceresponsetypedef) 


```python
# create_instance method usage example with argument unpacking

kwargs: CreateInstanceRequestRequestTypeDef = {  # (1)
    "IdentityManagementType": ...,
    "InboundCallsEnabled": ...,
    "OutboundCallsEnabled": ...,
}

parent.create_instance(**kwargs)
```

1. See [:material-code-braces: CreateInstanceRequestRequestTypeDef](./type_defs.md#createinstancerequestrequesttypedef) 

### create\_integration\_association

Creates an Amazon Web Services resource association with an Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").create_integration_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_integration_association)

```python
# create_integration_association method definition

await def create_integration_association(
    self,
    *,
    InstanceId: str,
    IntegrationType: IntegrationTypeType,  # (1)
    IntegrationArn: str,
    SourceApplicationUrl: str = ...,
    SourceApplicationName: str = ...,
    SourceType: SourceTypeType = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> CreateIntegrationAssociationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
3. See [:material-code-braces: CreateIntegrationAssociationResponseTypeDef](./type_defs.md#createintegrationassociationresponsetypedef) 


```python
# create_integration_association method usage example with argument unpacking

kwargs: CreateIntegrationAssociationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "IntegrationType": ...,
    "IntegrationArn": ...,
}

parent.create_integration_association(**kwargs)
```

1. See [:material-code-braces: CreateIntegrationAssociationRequestRequestTypeDef](./type_defs.md#createintegrationassociationrequestrequesttypedef) 

### create\_participant

Adds a new participant into an on-going chat contact.

Type annotations and code completion for `#!python session.create_client("connect").create_participant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_participant)

```python
# create_participant method definition

await def create_participant(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    ParticipantDetails: ParticipantDetailsToAddTypeDef,  # (1)
    ClientToken: str = ...,
) -> CreateParticipantResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ParticipantDetailsToAddTypeDef](./type_defs.md#participantdetailstoaddtypedef) 
2. See [:material-code-braces: CreateParticipantResponseTypeDef](./type_defs.md#createparticipantresponsetypedef) 


```python
# create_participant method usage example with argument unpacking

kwargs: CreateParticipantRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "ParticipantDetails": ...,
}

parent.create_participant(**kwargs)
```

1. See [:material-code-braces: CreateParticipantRequestRequestTypeDef](./type_defs.md#createparticipantrequestrequesttypedef) 

### create\_prompt

Creates a prompt.

Type annotations and code completion for `#!python session.create_client("connect").create_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_prompt)

```python
# create_prompt method definition

await def create_prompt(
    self,
    *,
    InstanceId: str,
    Name: str,
    S3Uri: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreatePromptResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePromptResponseTypeDef](./type_defs.md#createpromptresponsetypedef) 


```python
# create_prompt method usage example with argument unpacking

kwargs: CreatePromptRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "S3Uri": ...,
}

parent.create_prompt(**kwargs)
```

1. See [:material-code-braces: CreatePromptRequestRequestTypeDef](./type_defs.md#createpromptrequestrequesttypedef) 

### create\_queue

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").create_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_queue)

```python
# create_queue method definition

await def create_queue(
    self,
    *,
    InstanceId: str,
    Name: str,
    HoursOfOperationId: str,
    Description: str = ...,
    OutboundCallerConfig: OutboundCallerConfigTypeDef = ...,  # (1)
    MaxContacts: int = ...,
    QuickConnectIds: Sequence[str] = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateQueueResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef) 
2. See [:material-code-braces: CreateQueueResponseTypeDef](./type_defs.md#createqueueresponsetypedef) 


```python
# create_queue method usage example with argument unpacking

kwargs: CreateQueueRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "HoursOfOperationId": ...,
}

parent.create_queue(**kwargs)
```

1. See [:material-code-braces: CreateQueueRequestRequestTypeDef](./type_defs.md#createqueuerequestrequesttypedef) 

### create\_quick\_connect

Creates a quick connect for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_quick_connect` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_quick_connect)

```python
# create_quick_connect method definition

await def create_quick_connect(
    self,
    *,
    InstanceId: str,
    Name: str,
    QuickConnectConfig: QuickConnectConfigTypeDef,  # (1)
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateQuickConnectResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: QuickConnectConfigTypeDef](./type_defs.md#quickconnectconfigtypedef) 
2. See [:material-code-braces: CreateQuickConnectResponseTypeDef](./type_defs.md#createquickconnectresponsetypedef) 


```python
# create_quick_connect method usage example with argument unpacking

kwargs: CreateQuickConnectRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "QuickConnectConfig": ...,
}

parent.create_quick_connect(**kwargs)
```

1. See [:material-code-braces: CreateQuickConnectRequestRequestTypeDef](./type_defs.md#createquickconnectrequestrequesttypedef) 

### create\_routing\_profile

Creates a new routing profile.

Type annotations and code completion for `#!python session.create_client("connect").create_routing_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_routing_profile)

```python
# create_routing_profile method definition

await def create_routing_profile(
    self,
    *,
    InstanceId: str,
    Name: str,
    Description: str,
    DefaultOutboundQueueId: str,
    MediaConcurrencies: Sequence[MediaConcurrencyTypeDef],  # (1)
    QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef] = ...,  # (2)
    Tags: Mapping[str, str] = ...,
    AgentAvailabilityTimer: AgentAvailabilityTimerType = ...,  # (3)
) -> CreateRoutingProfileResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: MediaConcurrencyTypeDef](./type_defs.md#mediaconcurrencytypedef) 
2. See [:material-code-braces: RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef) 
3. See [:material-code-brackets: AgentAvailabilityTimerType](./literals.md#agentavailabilitytimertype) 
4. See [:material-code-braces: CreateRoutingProfileResponseTypeDef](./type_defs.md#createroutingprofileresponsetypedef) 


```python
# create_routing_profile method usage example with argument unpacking

kwargs: CreateRoutingProfileRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "Description": ...,
    "DefaultOutboundQueueId": ...,
    "MediaConcurrencies": ...,
}

parent.create_routing_profile(**kwargs)
```

1. See [:material-code-braces: CreateRoutingProfileRequestRequestTypeDef](./type_defs.md#createroutingprofilerequestrequesttypedef) 

### create\_rule

Creates a rule for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_rule)

```python
# create_rule method definition

await def create_rule(
    self,
    *,
    InstanceId: str,
    Name: str,
    TriggerEventSource: RuleTriggerEventSourceTypeDef,  # (1)
    Function: str,
    Actions: Sequence[RuleActionTypeDef],  # (2)
    PublishStatus: RulePublishStatusType,  # (3)
    ClientToken: str = ...,
) -> CreateRuleResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RuleTriggerEventSourceTypeDef](./type_defs.md#ruletriggereventsourcetypedef) 
2. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
3. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
4. See [:material-code-braces: CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef) 


```python
# create_rule method usage example with argument unpacking

kwargs: CreateRuleRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "TriggerEventSource": ...,
    "Function": ...,
    "Actions": ...,
    "PublishStatus": ...,
}

parent.create_rule(**kwargs)
```

1. See [:material-code-braces: CreateRuleRequestRequestTypeDef](./type_defs.md#createrulerequestrequesttypedef) 

### create\_security\_profile

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").create_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_security_profile)

```python
# create_security_profile method definition

await def create_security_profile(
    self,
    *,
    SecurityProfileName: str,
    InstanceId: str,
    Description: str = ...,
    Permissions: Sequence[str] = ...,
    Tags: Mapping[str, str] = ...,
    AllowedAccessControlTags: Mapping[str, str] = ...,
    TagRestrictedResources: Sequence[str] = ...,
) -> CreateSecurityProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSecurityProfileResponseTypeDef](./type_defs.md#createsecurityprofileresponsetypedef) 


```python
# create_security_profile method usage example with argument unpacking

kwargs: CreateSecurityProfileRequestRequestTypeDef = {  # (1)
    "SecurityProfileName": ...,
    "InstanceId": ...,
}

parent.create_security_profile(**kwargs)
```

1. See [:material-code-braces: CreateSecurityProfileRequestRequestTypeDef](./type_defs.md#createsecurityprofilerequestrequesttypedef) 

### create\_task\_template

Creates a new task template in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_task_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_task_template)

```python
# create_task_template method definition

await def create_task_template(
    self,
    *,
    InstanceId: str,
    Name: str,
    Fields: Sequence[TaskTemplateFieldTypeDef],  # (1)
    Description: str = ...,
    ContactFlowId: str = ...,
    Constraints: TaskTemplateConstraintsTypeDef = ...,  # (2)
    Defaults: TaskTemplateDefaultsTypeDef = ...,  # (3)
    Status: TaskTemplateStatusType = ...,  # (4)
    ClientToken: str = ...,
) -> CreateTaskTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: TaskTemplateFieldTypeDef](./type_defs.md#tasktemplatefieldtypedef) 
2. See [:material-code-braces: TaskTemplateConstraintsTypeDef](./type_defs.md#tasktemplateconstraintstypedef) 
3. See [:material-code-braces: TaskTemplateDefaultsTypeDef](./type_defs.md#tasktemplatedefaultstypedef) 
4. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
5. See [:material-code-braces: CreateTaskTemplateResponseTypeDef](./type_defs.md#createtasktemplateresponsetypedef) 


```python
# create_task_template method usage example with argument unpacking

kwargs: CreateTaskTemplateRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "Fields": ...,
}

parent.create_task_template(**kwargs)
```

1. See [:material-code-braces: CreateTaskTemplateRequestRequestTypeDef](./type_defs.md#createtasktemplaterequestrequesttypedef) 

### create\_traffic\_distribution\_group

Creates a traffic distribution group given an Amazon Connect instance that has
been replicated.

Type annotations and code completion for `#!python session.create_client("connect").create_traffic_distribution_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_traffic_distribution_group)

```python
# create_traffic_distribution_group method definition

await def create_traffic_distribution_group(
    self,
    *,
    Name: str,
    InstanceId: str,
    Description: str = ...,
    ClientToken: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateTrafficDistributionGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateTrafficDistributionGroupResponseTypeDef](./type_defs.md#createtrafficdistributiongroupresponsetypedef) 


```python
# create_traffic_distribution_group method usage example with argument unpacking

kwargs: CreateTrafficDistributionGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "InstanceId": ...,
}

parent.create_traffic_distribution_group(**kwargs)
```

1. See [:material-code-braces: CreateTrafficDistributionGroupRequestRequestTypeDef](./type_defs.md#createtrafficdistributiongrouprequestrequesttypedef) 

### create\_use\_case

Creates a use case for an integration association.

Type annotations and code completion for `#!python session.create_client("connect").create_use_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_use_case)

```python
# create_use_case method definition

await def create_use_case(
    self,
    *,
    InstanceId: str,
    IntegrationAssociationId: str,
    UseCaseType: UseCaseTypeType,  # (1)
    Tags: Mapping[str, str] = ...,
) -> CreateUseCaseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UseCaseTypeType](./literals.md#usecasetypetype) 
2. See [:material-code-braces: CreateUseCaseResponseTypeDef](./type_defs.md#createusecaseresponsetypedef) 


```python
# create_use_case method usage example with argument unpacking

kwargs: CreateUseCaseRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "IntegrationAssociationId": ...,
    "UseCaseType": ...,
}

parent.create_use_case(**kwargs)
```

1. See [:material-code-braces: CreateUseCaseRequestRequestTypeDef](./type_defs.md#createusecaserequestrequesttypedef) 

### create\_user

Creates a user account for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user)

```python
# create_user method definition

await def create_user(
    self,
    *,
    Username: str,
    PhoneConfig: UserPhoneConfigTypeDef,  # (1)
    SecurityProfileIds: Sequence[str],
    RoutingProfileId: str,
    InstanceId: str,
    Password: str = ...,
    IdentityInfo: UserIdentityInfoTypeDef = ...,  # (2)
    DirectoryUserId: str = ...,
    HierarchyGroupId: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateUserResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef) 
2. See [:material-code-braces: UserIdentityInfoTypeDef](./type_defs.md#useridentityinfotypedef) 
3. See [:material-code-braces: CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestRequestTypeDef = {  # (1)
    "Username": ...,
    "PhoneConfig": ...,
    "SecurityProfileIds": ...,
    "RoutingProfileId": ...,
    "InstanceId": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef) 

### create\_user\_hierarchy\_group

Creates a new user hierarchy group.

Type annotations and code completion for `#!python session.create_client("connect").create_user_hierarchy_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_user_hierarchy_group)

```python
# create_user_hierarchy_group method definition

await def create_user_hierarchy_group(
    self,
    *,
    Name: str,
    InstanceId: str,
    ParentGroupId: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateUserHierarchyGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateUserHierarchyGroupResponseTypeDef](./type_defs.md#createuserhierarchygroupresponsetypedef) 


```python
# create_user_hierarchy_group method usage example with argument unpacking

kwargs: CreateUserHierarchyGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "InstanceId": ...,
}

parent.create_user_hierarchy_group(**kwargs)
```

1. See [:material-code-braces: CreateUserHierarchyGroupRequestRequestTypeDef](./type_defs.md#createuserhierarchygrouprequestrequesttypedef) 

### create\_vocabulary

Creates a custom vocabulary associated with your Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.create_vocabulary)

```python
# create_vocabulary method definition

await def create_vocabulary(
    self,
    *,
    InstanceId: str,
    VocabularyName: str,
    LanguageCode: VocabularyLanguageCodeType,  # (1)
    Content: str,
    ClientToken: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateVocabularyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
2. See [:material-code-braces: CreateVocabularyResponseTypeDef](./type_defs.md#createvocabularyresponsetypedef) 


```python
# create_vocabulary method usage example with argument unpacking

kwargs: CreateVocabularyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "VocabularyName": ...,
    "LanguageCode": ...,
    "Content": ...,
}

parent.create_vocabulary(**kwargs)
```

1. See [:material-code-braces: CreateVocabularyRequestRequestTypeDef](./type_defs.md#createvocabularyrequestrequesttypedef) 

### deactivate\_evaluation\_form

Deactivates an evaluation form in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").deactivate_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.deactivate_evaluation_form)

```python
# deactivate_evaluation_form method definition

await def deactivate_evaluation_form(
    self,
    *,
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
) -> DeactivateEvaluationFormResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeactivateEvaluationFormResponseTypeDef](./type_defs.md#deactivateevaluationformresponsetypedef) 


```python
# deactivate_evaluation_form method usage example with argument unpacking

kwargs: DeactivateEvaluationFormRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationFormId": ...,
    "EvaluationFormVersion": ...,
}

parent.deactivate_evaluation_form(**kwargs)
```

1. See [:material-code-braces: DeactivateEvaluationFormRequestRequestTypeDef](./type_defs.md#deactivateevaluationformrequestrequesttypedef) 

### delete\_contact\_evaluation

Deletes a contact evaluation in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").delete_contact_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_contact_evaluation)

```python
# delete_contact_evaluation method definition

await def delete_contact_evaluation(
    self,
    *,
    InstanceId: str,
    EvaluationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_contact_evaluation method usage example with argument unpacking

kwargs: DeleteContactEvaluationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationId": ...,
}

parent.delete_contact_evaluation(**kwargs)
```

1. See [:material-code-braces: DeleteContactEvaluationRequestRequestTypeDef](./type_defs.md#deletecontactevaluationrequestrequesttypedef) 

### delete\_contact\_flow

Deletes a flow for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").delete_contact_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_contact_flow)

```python
# delete_contact_flow method definition

await def delete_contact_flow(
    self,
    *,
    InstanceId: str,
    ContactFlowId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_contact_flow method usage example with argument unpacking

kwargs: DeleteContactFlowRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowId": ...,
}

parent.delete_contact_flow(**kwargs)
```

1. See [:material-code-braces: DeleteContactFlowRequestRequestTypeDef](./type_defs.md#deletecontactflowrequestrequesttypedef) 

### delete\_contact\_flow\_module

Deletes the specified flow module.

Type annotations and code completion for `#!python session.create_client("connect").delete_contact_flow_module` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_contact_flow_module)

```python
# delete_contact_flow_module method definition

await def delete_contact_flow_module(
    self,
    *,
    InstanceId: str,
    ContactFlowModuleId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_contact_flow_module method usage example with argument unpacking

kwargs: DeleteContactFlowModuleRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowModuleId": ...,
}

parent.delete_contact_flow_module(**kwargs)
```

1. See [:material-code-braces: DeleteContactFlowModuleRequestRequestTypeDef](./type_defs.md#deletecontactflowmodulerequestrequesttypedef) 

### delete\_evaluation\_form

Deletes an evaluation form in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").delete_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_evaluation_form)

```python
# delete_evaluation_form method definition

await def delete_evaluation_form(
    self,
    *,
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_evaluation_form method usage example with argument unpacking

kwargs: DeleteEvaluationFormRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationFormId": ...,
}

parent.delete_evaluation_form(**kwargs)
```

1. See [:material-code-braces: DeleteEvaluationFormRequestRequestTypeDef](./type_defs.md#deleteevaluationformrequestrequesttypedef) 

### delete\_hours\_of\_operation

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").delete_hours_of_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_hours_of_operation)

```python
# delete_hours_of_operation method definition

await def delete_hours_of_operation(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_hours_of_operation method usage example with argument unpacking

kwargs: DeleteHoursOfOperationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
}

parent.delete_hours_of_operation(**kwargs)
```

1. See [:material-code-braces: DeleteHoursOfOperationRequestRequestTypeDef](./type_defs.md#deletehoursofoperationrequestrequesttypedef) 

### delete\_instance

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").delete_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_instance)

```python
# delete_instance method definition

await def delete_instance(
    self,
    *,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_instance method usage example with argument unpacking

kwargs: DeleteInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.delete_instance(**kwargs)
```

1. See [:material-code-braces: DeleteInstanceRequestRequestTypeDef](./type_defs.md#deleteinstancerequestrequesttypedef) 

### delete\_integration\_association

Deletes an Amazon Web Services resource association from an Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").delete_integration_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_integration_association)

```python
# delete_integration_association method definition

await def delete_integration_association(
    self,
    *,
    InstanceId: str,
    IntegrationAssociationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_integration_association method usage example with argument unpacking

kwargs: DeleteIntegrationAssociationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "IntegrationAssociationId": ...,
}

parent.delete_integration_association(**kwargs)
```

1. See [:material-code-braces: DeleteIntegrationAssociationRequestRequestTypeDef](./type_defs.md#deleteintegrationassociationrequestrequesttypedef) 

### delete\_prompt

Deletes a prompt.

Type annotations and code completion for `#!python session.create_client("connect").delete_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_prompt)

```python
# delete_prompt method definition

await def delete_prompt(
    self,
    *,
    InstanceId: str,
    PromptId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_prompt method usage example with argument unpacking

kwargs: DeletePromptRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "PromptId": ...,
}

parent.delete_prompt(**kwargs)
```

1. See [:material-code-braces: DeletePromptRequestRequestTypeDef](./type_defs.md#deletepromptrequestrequesttypedef) 

### delete\_queue

Deletes a queue.

Type annotations and code completion for `#!python session.create_client("connect").delete_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_queue)

```python
# delete_queue method definition

await def delete_queue(
    self,
    *,
    InstanceId: str,
    QueueId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_queue method usage example with argument unpacking

kwargs: DeleteQueueRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
}

parent.delete_queue(**kwargs)
```

1. See [:material-code-braces: DeleteQueueRequestRequestTypeDef](./type_defs.md#deletequeuerequestrequesttypedef) 

### delete\_quick\_connect

Deletes a quick connect.

Type annotations and code completion for `#!python session.create_client("connect").delete_quick_connect` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_quick_connect)

```python
# delete_quick_connect method definition

await def delete_quick_connect(
    self,
    *,
    InstanceId: str,
    QuickConnectId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_quick_connect method usage example with argument unpacking

kwargs: DeleteQuickConnectRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QuickConnectId": ...,
}

parent.delete_quick_connect(**kwargs)
```

1. See [:material-code-braces: DeleteQuickConnectRequestRequestTypeDef](./type_defs.md#deletequickconnectrequestrequesttypedef) 

### delete\_routing\_profile

Deletes a routing profile.

Type annotations and code completion for `#!python session.create_client("connect").delete_routing_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_routing_profile)

```python
# delete_routing_profile method definition

await def delete_routing_profile(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_routing_profile method usage example with argument unpacking

kwargs: DeleteRoutingProfileRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
}

parent.delete_routing_profile(**kwargs)
```

1. See [:material-code-braces: DeleteRoutingProfileRequestRequestTypeDef](./type_defs.md#deleteroutingprofilerequestrequesttypedef) 

### delete\_rule

Deletes a rule for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").delete_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_rule)

```python
# delete_rule method definition

await def delete_rule(
    self,
    *,
    InstanceId: str,
    RuleId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_rule method usage example with argument unpacking

kwargs: DeleteRuleRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RuleId": ...,
}

parent.delete_rule(**kwargs)
```

1. See [:material-code-braces: DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef) 

### delete\_security\_profile

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").delete_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_security_profile)

```python
# delete_security_profile method definition

await def delete_security_profile(
    self,
    *,
    InstanceId: str,
    SecurityProfileId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_security_profile method usage example with argument unpacking

kwargs: DeleteSecurityProfileRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "SecurityProfileId": ...,
}

parent.delete_security_profile(**kwargs)
```

1. See [:material-code-braces: DeleteSecurityProfileRequestRequestTypeDef](./type_defs.md#deletesecurityprofilerequestrequesttypedef) 

### delete\_task\_template

Deletes the task template.

Type annotations and code completion for `#!python session.create_client("connect").delete_task_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_task_template)

```python
# delete_task_template method definition

await def delete_task_template(
    self,
    *,
    InstanceId: str,
    TaskTemplateId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_task_template method usage example with argument unpacking

kwargs: DeleteTaskTemplateRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "TaskTemplateId": ...,
}

parent.delete_task_template(**kwargs)
```

1. See [:material-code-braces: DeleteTaskTemplateRequestRequestTypeDef](./type_defs.md#deletetasktemplaterequestrequesttypedef) 

### delete\_traffic\_distribution\_group

Deletes a traffic distribution group.

Type annotations and code completion for `#!python session.create_client("connect").delete_traffic_distribution_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_traffic_distribution_group)

```python
# delete_traffic_distribution_group method definition

await def delete_traffic_distribution_group(
    self,
    *,
    TrafficDistributionGroupId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_traffic_distribution_group method usage example with argument unpacking

kwargs: DeleteTrafficDistributionGroupRequestRequestTypeDef = {  # (1)
    "TrafficDistributionGroupId": ...,
}

parent.delete_traffic_distribution_group(**kwargs)
```

1. See [:material-code-braces: DeleteTrafficDistributionGroupRequestRequestTypeDef](./type_defs.md#deletetrafficdistributiongrouprequestrequesttypedef) 

### delete\_use\_case

Deletes a use case from an integration association.

Type annotations and code completion for `#!python session.create_client("connect").delete_use_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_use_case)

```python
# delete_use_case method definition

await def delete_use_case(
    self,
    *,
    InstanceId: str,
    IntegrationAssociationId: str,
    UseCaseId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_use_case method usage example with argument unpacking

kwargs: DeleteUseCaseRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "IntegrationAssociationId": ...,
    "UseCaseId": ...,
}

parent.delete_use_case(**kwargs)
```

1. See [:material-code-braces: DeleteUseCaseRequestRequestTypeDef](./type_defs.md#deleteusecaserequestrequesttypedef) 

### delete\_user

Deletes a user account from the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_user)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    InstanceId: str,
    UserId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "UserId": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### delete\_user\_hierarchy\_group

Deletes an existing user hierarchy group.

Type annotations and code completion for `#!python session.create_client("connect").delete_user_hierarchy_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_user_hierarchy_group)

```python
# delete_user_hierarchy_group method definition

await def delete_user_hierarchy_group(
    self,
    *,
    HierarchyGroupId: str,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user_hierarchy_group method usage example with argument unpacking

kwargs: DeleteUserHierarchyGroupRequestRequestTypeDef = {  # (1)
    "HierarchyGroupId": ...,
    "InstanceId": ...,
}

parent.delete_user_hierarchy_group(**kwargs)
```

1. See [:material-code-braces: DeleteUserHierarchyGroupRequestRequestTypeDef](./type_defs.md#deleteuserhierarchygrouprequestrequesttypedef) 

### delete\_vocabulary

Deletes the vocabulary that has the given identifier.

Type annotations and code completion for `#!python session.create_client("connect").delete_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.delete_vocabulary)

```python
# delete_vocabulary method definition

await def delete_vocabulary(
    self,
    *,
    InstanceId: str,
    VocabularyId: str,
) -> DeleteVocabularyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVocabularyResponseTypeDef](./type_defs.md#deletevocabularyresponsetypedef) 


```python
# delete_vocabulary method usage example with argument unpacking

kwargs: DeleteVocabularyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "VocabularyId": ...,
}

parent.delete_vocabulary(**kwargs)
```

1. See [:material-code-braces: DeleteVocabularyRequestRequestTypeDef](./type_defs.md#deletevocabularyrequestrequesttypedef) 

### describe\_agent\_status

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_agent_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_agent_status)

```python
# describe_agent_status method definition

await def describe_agent_status(
    self,
    *,
    InstanceId: str,
    AgentStatusId: str,
) -> DescribeAgentStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAgentStatusResponseTypeDef](./type_defs.md#describeagentstatusresponsetypedef) 


```python
# describe_agent_status method usage example with argument unpacking

kwargs: DescribeAgentStatusRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "AgentStatusId": ...,
}

parent.describe_agent_status(**kwargs)
```

1. See [:material-code-braces: DescribeAgentStatusRequestRequestTypeDef](./type_defs.md#describeagentstatusrequestrequesttypedef) 

### describe\_contact

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact)

```python
# describe_contact method definition

await def describe_contact(
    self,
    *,
    InstanceId: str,
    ContactId: str,
) -> DescribeContactResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeContactResponseTypeDef](./type_defs.md#describecontactresponsetypedef) 


```python
# describe_contact method usage example with argument unpacking

kwargs: DescribeContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
}

parent.describe_contact(**kwargs)
```

1. See [:material-code-braces: DescribeContactRequestRequestTypeDef](./type_defs.md#describecontactrequestrequesttypedef) 

### describe\_contact\_evaluation

Describes a contact evaluation in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").describe_contact_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_evaluation)

```python
# describe_contact_evaluation method definition

await def describe_contact_evaluation(
    self,
    *,
    InstanceId: str,
    EvaluationId: str,
) -> DescribeContactEvaluationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeContactEvaluationResponseTypeDef](./type_defs.md#describecontactevaluationresponsetypedef) 


```python
# describe_contact_evaluation method usage example with argument unpacking

kwargs: DescribeContactEvaluationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationId": ...,
}

parent.describe_contact_evaluation(**kwargs)
```

1. See [:material-code-braces: DescribeContactEvaluationRequestRequestTypeDef](./type_defs.md#describecontactevaluationrequestrequesttypedef) 

### describe\_contact\_flow

Describes the specified flow.

Type annotations and code completion for `#!python session.create_client("connect").describe_contact_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_flow)

```python
# describe_contact_flow method definition

await def describe_contact_flow(
    self,
    *,
    InstanceId: str,
    ContactFlowId: str,
) -> DescribeContactFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeContactFlowResponseTypeDef](./type_defs.md#describecontactflowresponsetypedef) 


```python
# describe_contact_flow method usage example with argument unpacking

kwargs: DescribeContactFlowRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowId": ...,
}

parent.describe_contact_flow(**kwargs)
```

1. See [:material-code-braces: DescribeContactFlowRequestRequestTypeDef](./type_defs.md#describecontactflowrequestrequesttypedef) 

### describe\_contact\_flow\_module

Describes the specified flow module.

Type annotations and code completion for `#!python session.create_client("connect").describe_contact_flow_module` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_contact_flow_module)

```python
# describe_contact_flow_module method definition

await def describe_contact_flow_module(
    self,
    *,
    InstanceId: str,
    ContactFlowModuleId: str,
) -> DescribeContactFlowModuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeContactFlowModuleResponseTypeDef](./type_defs.md#describecontactflowmoduleresponsetypedef) 


```python
# describe_contact_flow_module method usage example with argument unpacking

kwargs: DescribeContactFlowModuleRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowModuleId": ...,
}

parent.describe_contact_flow_module(**kwargs)
```

1. See [:material-code-braces: DescribeContactFlowModuleRequestRequestTypeDef](./type_defs.md#describecontactflowmodulerequestrequesttypedef) 

### describe\_evaluation\_form

Describes an evaluation form in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").describe_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_evaluation_form)

```python
# describe_evaluation_form method definition

await def describe_evaluation_form(
    self,
    *,
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int = ...,
) -> DescribeEvaluationFormResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEvaluationFormResponseTypeDef](./type_defs.md#describeevaluationformresponsetypedef) 


```python
# describe_evaluation_form method usage example with argument unpacking

kwargs: DescribeEvaluationFormRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationFormId": ...,
}

parent.describe_evaluation_form(**kwargs)
```

1. See [:material-code-braces: DescribeEvaluationFormRequestRequestTypeDef](./type_defs.md#describeevaluationformrequestrequesttypedef) 

### describe\_hours\_of\_operation

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_hours_of_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_hours_of_operation)

```python
# describe_hours_of_operation method definition

await def describe_hours_of_operation(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
) -> DescribeHoursOfOperationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHoursOfOperationResponseTypeDef](./type_defs.md#describehoursofoperationresponsetypedef) 


```python
# describe_hours_of_operation method usage example with argument unpacking

kwargs: DescribeHoursOfOperationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
}

parent.describe_hours_of_operation(**kwargs)
```

1. See [:material-code-braces: DescribeHoursOfOperationRequestRequestTypeDef](./type_defs.md#describehoursofoperationrequestrequesttypedef) 

### describe\_instance

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance)

```python
# describe_instance method definition

await def describe_instance(
    self,
    *,
    InstanceId: str,
) -> DescribeInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInstanceResponseTypeDef](./type_defs.md#describeinstanceresponsetypedef) 


```python
# describe_instance method usage example with argument unpacking

kwargs: DescribeInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.describe_instance(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceRequestRequestTypeDef](./type_defs.md#describeinstancerequestrequesttypedef) 

### describe\_instance\_attribute

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_instance_attribute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_attribute)

```python
# describe_instance_attribute method definition

await def describe_instance_attribute(
    self,
    *,
    InstanceId: str,
    AttributeType: InstanceAttributeTypeType,  # (1)
) -> DescribeInstanceAttributeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InstanceAttributeTypeType](./literals.md#instanceattributetypetype) 
2. See [:material-code-braces: DescribeInstanceAttributeResponseTypeDef](./type_defs.md#describeinstanceattributeresponsetypedef) 


```python
# describe_instance_attribute method usage example with argument unpacking

kwargs: DescribeInstanceAttributeRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "AttributeType": ...,
}

parent.describe_instance_attribute(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceAttributeRequestRequestTypeDef](./type_defs.md#describeinstanceattributerequestrequesttypedef) 

### describe\_instance\_storage\_config

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_instance_storage_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_instance_storage_config)

```python
# describe_instance_storage_config method definition

await def describe_instance_storage_config(
    self,
    *,
    InstanceId: str,
    AssociationId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
) -> DescribeInstanceStorageConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: DescribeInstanceStorageConfigResponseTypeDef](./type_defs.md#describeinstancestorageconfigresponsetypedef) 


```python
# describe_instance_storage_config method usage example with argument unpacking

kwargs: DescribeInstanceStorageConfigRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "AssociationId": ...,
    "ResourceType": ...,
}

parent.describe_instance_storage_config(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#describeinstancestorageconfigrequestrequesttypedef) 

### describe\_phone\_number

Gets details and status of a phone number that’s claimed to your Amazon Connect
instance or traffic distribution group.

Type annotations and code completion for `#!python session.create_client("connect").describe_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_phone_number)

```python
# describe_phone_number method definition

await def describe_phone_number(
    self,
    *,
    PhoneNumberId: str,
) -> DescribePhoneNumberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePhoneNumberResponseTypeDef](./type_defs.md#describephonenumberresponsetypedef) 


```python
# describe_phone_number method usage example with argument unpacking

kwargs: DescribePhoneNumberRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.describe_phone_number(**kwargs)
```

1. See [:material-code-braces: DescribePhoneNumberRequestRequestTypeDef](./type_defs.md#describephonenumberrequestrequesttypedef) 

### describe\_prompt

Describes the prompt.

Type annotations and code completion for `#!python session.create_client("connect").describe_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_prompt)

```python
# describe_prompt method definition

await def describe_prompt(
    self,
    *,
    InstanceId: str,
    PromptId: str,
) -> DescribePromptResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePromptResponseTypeDef](./type_defs.md#describepromptresponsetypedef) 


```python
# describe_prompt method usage example with argument unpacking

kwargs: DescribePromptRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "PromptId": ...,
}

parent.describe_prompt(**kwargs)
```

1. See [:material-code-braces: DescribePromptRequestRequestTypeDef](./type_defs.md#describepromptrequestrequesttypedef) 

### describe\_queue

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_queue)

```python
# describe_queue method definition

await def describe_queue(
    self,
    *,
    InstanceId: str,
    QueueId: str,
) -> DescribeQueueResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeQueueResponseTypeDef](./type_defs.md#describequeueresponsetypedef) 


```python
# describe_queue method usage example with argument unpacking

kwargs: DescribeQueueRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
}

parent.describe_queue(**kwargs)
```

1. See [:material-code-braces: DescribeQueueRequestRequestTypeDef](./type_defs.md#describequeuerequestrequesttypedef) 

### describe\_quick\_connect

Describes the quick connect.

Type annotations and code completion for `#!python session.create_client("connect").describe_quick_connect` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_quick_connect)

```python
# describe_quick_connect method definition

await def describe_quick_connect(
    self,
    *,
    InstanceId: str,
    QuickConnectId: str,
) -> DescribeQuickConnectResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeQuickConnectResponseTypeDef](./type_defs.md#describequickconnectresponsetypedef) 


```python
# describe_quick_connect method usage example with argument unpacking

kwargs: DescribeQuickConnectRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QuickConnectId": ...,
}

parent.describe_quick_connect(**kwargs)
```

1. See [:material-code-braces: DescribeQuickConnectRequestRequestTypeDef](./type_defs.md#describequickconnectrequestrequesttypedef) 

### describe\_routing\_profile

Describes the specified routing profile.

Type annotations and code completion for `#!python session.create_client("connect").describe_routing_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_routing_profile)

```python
# describe_routing_profile method definition

await def describe_routing_profile(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
) -> DescribeRoutingProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRoutingProfileResponseTypeDef](./type_defs.md#describeroutingprofileresponsetypedef) 


```python
# describe_routing_profile method usage example with argument unpacking

kwargs: DescribeRoutingProfileRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
}

parent.describe_routing_profile(**kwargs)
```

1. See [:material-code-braces: DescribeRoutingProfileRequestRequestTypeDef](./type_defs.md#describeroutingprofilerequestrequesttypedef) 

### describe\_rule

Describes a rule for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").describe_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_rule)

```python
# describe_rule method definition

await def describe_rule(
    self,
    *,
    InstanceId: str,
    RuleId: str,
) -> DescribeRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRuleResponseTypeDef](./type_defs.md#describeruleresponsetypedef) 


```python
# describe_rule method usage example with argument unpacking

kwargs: DescribeRuleRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RuleId": ...,
}

parent.describe_rule(**kwargs)
```

1. See [:material-code-braces: DescribeRuleRequestRequestTypeDef](./type_defs.md#describerulerequestrequesttypedef) 

### describe\_security\_profile

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_security_profile)

```python
# describe_security_profile method definition

await def describe_security_profile(
    self,
    *,
    SecurityProfileId: str,
    InstanceId: str,
) -> DescribeSecurityProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSecurityProfileResponseTypeDef](./type_defs.md#describesecurityprofileresponsetypedef) 


```python
# describe_security_profile method usage example with argument unpacking

kwargs: DescribeSecurityProfileRequestRequestTypeDef = {  # (1)
    "SecurityProfileId": ...,
    "InstanceId": ...,
}

parent.describe_security_profile(**kwargs)
```

1. See [:material-code-braces: DescribeSecurityProfileRequestRequestTypeDef](./type_defs.md#describesecurityprofilerequestrequesttypedef) 

### describe\_traffic\_distribution\_group

Gets details and status of a traffic distribution group.

Type annotations and code completion for `#!python session.create_client("connect").describe_traffic_distribution_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_traffic_distribution_group)

```python
# describe_traffic_distribution_group method definition

await def describe_traffic_distribution_group(
    self,
    *,
    TrafficDistributionGroupId: str,
) -> DescribeTrafficDistributionGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrafficDistributionGroupResponseTypeDef](./type_defs.md#describetrafficdistributiongroupresponsetypedef) 


```python
# describe_traffic_distribution_group method usage example with argument unpacking

kwargs: DescribeTrafficDistributionGroupRequestRequestTypeDef = {  # (1)
    "TrafficDistributionGroupId": ...,
}

parent.describe_traffic_distribution_group(**kwargs)
```

1. See [:material-code-braces: DescribeTrafficDistributionGroupRequestRequestTypeDef](./type_defs.md#describetrafficdistributiongrouprequestrequesttypedef) 

### describe\_user

Describes the specified user account.

Type annotations and code completion for `#!python session.create_client("connect").describe_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user)

```python
# describe_user method definition

await def describe_user(
    self,
    *,
    UserId: str,
    InstanceId: str,
) -> DescribeUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef) 


```python
# describe_user method usage example with argument unpacking

kwargs: DescribeUserRequestRequestTypeDef = {  # (1)
    "UserId": ...,
    "InstanceId": ...,
}

parent.describe_user(**kwargs)
```

1. See [:material-code-braces: DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef) 

### describe\_user\_hierarchy\_group

Describes the specified hierarchy group.

Type annotations and code completion for `#!python session.create_client("connect").describe_user_hierarchy_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user_hierarchy_group)

```python
# describe_user_hierarchy_group method definition

await def describe_user_hierarchy_group(
    self,
    *,
    HierarchyGroupId: str,
    InstanceId: str,
) -> DescribeUserHierarchyGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserHierarchyGroupResponseTypeDef](./type_defs.md#describeuserhierarchygroupresponsetypedef) 


```python
# describe_user_hierarchy_group method usage example with argument unpacking

kwargs: DescribeUserHierarchyGroupRequestRequestTypeDef = {  # (1)
    "HierarchyGroupId": ...,
    "InstanceId": ...,
}

parent.describe_user_hierarchy_group(**kwargs)
```

1. See [:material-code-braces: DescribeUserHierarchyGroupRequestRequestTypeDef](./type_defs.md#describeuserhierarchygrouprequestrequesttypedef) 

### describe\_user\_hierarchy\_structure

Describes the hierarchy structure of the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").describe_user_hierarchy_structure` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_user_hierarchy_structure)

```python
# describe_user_hierarchy_structure method definition

await def describe_user_hierarchy_structure(
    self,
    *,
    InstanceId: str,
) -> DescribeUserHierarchyStructureResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserHierarchyStructureResponseTypeDef](./type_defs.md#describeuserhierarchystructureresponsetypedef) 


```python
# describe_user_hierarchy_structure method usage example with argument unpacking

kwargs: DescribeUserHierarchyStructureRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.describe_user_hierarchy_structure(**kwargs)
```

1. See [:material-code-braces: DescribeUserHierarchyStructureRequestRequestTypeDef](./type_defs.md#describeuserhierarchystructurerequestrequesttypedef) 

### describe\_vocabulary

Describes the specified vocabulary.

Type annotations and code completion for `#!python session.create_client("connect").describe_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.describe_vocabulary)

```python
# describe_vocabulary method definition

await def describe_vocabulary(
    self,
    *,
    InstanceId: str,
    VocabularyId: str,
) -> DescribeVocabularyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVocabularyResponseTypeDef](./type_defs.md#describevocabularyresponsetypedef) 


```python
# describe_vocabulary method usage example with argument unpacking

kwargs: DescribeVocabularyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "VocabularyId": ...,
}

parent.describe_vocabulary(**kwargs)
```

1. See [:material-code-braces: DescribeVocabularyRequestRequestTypeDef](./type_defs.md#describevocabularyrequestrequesttypedef) 

### disassociate\_approved\_origin

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_approved_origin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_approved_origin)

```python
# disassociate_approved_origin method definition

await def disassociate_approved_origin(
    self,
    *,
    InstanceId: str,
    Origin: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_approved_origin method usage example with argument unpacking

kwargs: DisassociateApprovedOriginRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Origin": ...,
}

parent.disassociate_approved_origin(**kwargs)
```

1. See [:material-code-braces: DisassociateApprovedOriginRequestRequestTypeDef](./type_defs.md#disassociateapprovedoriginrequestrequesttypedef) 

### disassociate\_bot

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_bot)

```python
# disassociate_bot method definition

await def disassociate_bot(
    self,
    *,
    InstanceId: str,
    LexBot: LexBotTypeDef = ...,  # (1)
    LexV2Bot: LexV2BotTypeDef = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LexBotTypeDef](./type_defs.md#lexbottypedef) 
2. See [:material-code-braces: LexV2BotTypeDef](./type_defs.md#lexv2bottypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_bot method usage example with argument unpacking

kwargs: DisassociateBotRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.disassociate_bot(**kwargs)
```

1. See [:material-code-braces: DisassociateBotRequestRequestTypeDef](./type_defs.md#disassociatebotrequestrequesttypedef) 

### disassociate\_instance\_storage\_config

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_instance_storage_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_instance_storage_config)

```python
# disassociate_instance_storage_config method definition

await def disassociate_instance_storage_config(
    self,
    *,
    InstanceId: str,
    AssociationId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_instance_storage_config method usage example with argument unpacking

kwargs: DisassociateInstanceStorageConfigRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "AssociationId": ...,
    "ResourceType": ...,
}

parent.disassociate_instance_storage_config(**kwargs)
```

1. See [:material-code-braces: DisassociateInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#disassociateinstancestorageconfigrequestrequesttypedef) 

### disassociate\_lambda\_function

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_lambda_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_lambda_function)

```python
# disassociate_lambda_function method definition

await def disassociate_lambda_function(
    self,
    *,
    InstanceId: str,
    FunctionArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_lambda_function method usage example with argument unpacking

kwargs: DisassociateLambdaFunctionRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "FunctionArn": ...,
}

parent.disassociate_lambda_function(**kwargs)
```

1. See [:material-code-braces: DisassociateLambdaFunctionRequestRequestTypeDef](./type_defs.md#disassociatelambdafunctionrequestrequesttypedef) 

### disassociate\_lex\_bot

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_lex_bot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_lex_bot)

```python
# disassociate_lex_bot method definition

await def disassociate_lex_bot(
    self,
    *,
    InstanceId: str,
    BotName: str,
    LexRegion: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_lex_bot method usage example with argument unpacking

kwargs: DisassociateLexBotRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "BotName": ...,
    "LexRegion": ...,
}

parent.disassociate_lex_bot(**kwargs)
```

1. See [:material-code-braces: DisassociateLexBotRequestRequestTypeDef](./type_defs.md#disassociatelexbotrequestrequesttypedef) 

### disassociate\_phone\_number\_contact\_flow

Removes the flow association from a phone number claimed to your Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_phone_number_contact_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_phone_number_contact_flow)

```python
# disassociate_phone_number_contact_flow method definition

await def disassociate_phone_number_contact_flow(
    self,
    *,
    PhoneNumberId: str,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_phone_number_contact_flow method usage example with argument unpacking

kwargs: DisassociatePhoneNumberContactFlowRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
    "InstanceId": ...,
}

parent.disassociate_phone_number_contact_flow(**kwargs)
```

1. See [:material-code-braces: DisassociatePhoneNumberContactFlowRequestRequestTypeDef](./type_defs.md#disassociatephonenumbercontactflowrequestrequesttypedef) 

### disassociate\_queue\_quick\_connects

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_queue_quick_connects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_queue_quick_connects)

```python
# disassociate_queue_quick_connects method definition

await def disassociate_queue_quick_connects(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    QuickConnectIds: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_queue_quick_connects method usage example with argument unpacking

kwargs: DisassociateQueueQuickConnectsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
    "QuickConnectIds": ...,
}

parent.disassociate_queue_quick_connects(**kwargs)
```

1. See [:material-code-braces: DisassociateQueueQuickConnectsRequestRequestTypeDef](./type_defs.md#disassociatequeuequickconnectsrequestrequesttypedef) 

### disassociate\_routing\_profile\_queues

Disassociates a set of queues from a routing profile.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_routing_profile_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_routing_profile_queues)

```python
# disassociate_routing_profile_queues method definition

await def disassociate_routing_profile_queues(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    QueueReferences: Sequence[RoutingProfileQueueReferenceTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RoutingProfileQueueReferenceTypeDef](./type_defs.md#routingprofilequeuereferencetypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_routing_profile_queues method usage example with argument unpacking

kwargs: DisassociateRoutingProfileQueuesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
    "QueueReferences": ...,
}

parent.disassociate_routing_profile_queues(**kwargs)
```

1. See [:material-code-braces: DisassociateRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#disassociateroutingprofilequeuesrequestrequesttypedef) 

### disassociate\_security\_key

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_security_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_security_key)

```python
# disassociate_security_key method definition

await def disassociate_security_key(
    self,
    *,
    InstanceId: str,
    AssociationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_security_key method usage example with argument unpacking

kwargs: DisassociateSecurityKeyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "AssociationId": ...,
}

parent.disassociate_security_key(**kwargs)
```

1. See [:material-code-braces: DisassociateSecurityKeyRequestRequestTypeDef](./type_defs.md#disassociatesecuritykeyrequestrequesttypedef) 

### disassociate\_traffic\_distribution\_group\_user

Disassociates an agent from a traffic distribution group.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_traffic_distribution_group_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.disassociate_traffic_distribution_group_user)

```python
# disassociate_traffic_distribution_group_user method definition

await def disassociate_traffic_distribution_group_user(
    self,
    *,
    TrafficDistributionGroupId: str,
    UserId: str,
    InstanceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_traffic_distribution_group_user method usage example with argument unpacking

kwargs: DisassociateTrafficDistributionGroupUserRequestRequestTypeDef = {  # (1)
    "TrafficDistributionGroupId": ...,
    "UserId": ...,
    "InstanceId": ...,
}

parent.disassociate_traffic_distribution_group_user(**kwargs)
```

1. See [:material-code-braces: DisassociateTrafficDistributionGroupUserRequestRequestTypeDef](./type_defs.md#disassociatetrafficdistributiongroupuserrequestrequesttypedef) 

### dismiss\_user\_contact

Dismisses contacts from an agent’s CCP and returns the agent to an available
state, which allows the agent to receive a new routed contact.

Type annotations and code completion for `#!python session.create_client("connect").dismiss_user_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.dismiss_user_contact)

```python
# dismiss_user_contact method definition

await def dismiss_user_contact(
    self,
    *,
    UserId: str,
    InstanceId: str,
    ContactId: str,
) -> Dict[str, Any]:
    ...
```



```python
# dismiss_user_contact method usage example with argument unpacking

kwargs: DismissUserContactRequestRequestTypeDef = {  # (1)
    "UserId": ...,
    "InstanceId": ...,
    "ContactId": ...,
}

parent.dismiss_user_contact(**kwargs)
```

1. See [:material-code-braces: DismissUserContactRequestRequestTypeDef](./type_defs.md#dismissusercontactrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("connect").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.generate_presigned_url)

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


### get\_contact\_attributes

Retrieves the contact attributes for the specified contact.

Type annotations and code completion for `#!python session.create_client("connect").get_contact_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_contact_attributes)

```python
# get_contact_attributes method definition

await def get_contact_attributes(
    self,
    *,
    InstanceId: str,
    InitialContactId: str,
) -> GetContactAttributesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContactAttributesResponseTypeDef](./type_defs.md#getcontactattributesresponsetypedef) 


```python
# get_contact_attributes method usage example with argument unpacking

kwargs: GetContactAttributesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "InitialContactId": ...,
}

parent.get_contact_attributes(**kwargs)
```

1. See [:material-code-braces: GetContactAttributesRequestRequestTypeDef](./type_defs.md#getcontactattributesrequestrequesttypedef) 

### get\_current\_metric\_data

Gets the real-time metric data from the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").get_current_metric_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_metric_data)

```python
# get_current_metric_data method definition

await def get_current_metric_data(
    self,
    *,
    InstanceId: str,
    Filters: FiltersTypeDef,  # (1)
    CurrentMetrics: Sequence[CurrentMetricTypeDef],  # (2)
    Groupings: Sequence[GroupingType] = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
    SortCriteria: Sequence[CurrentMetricSortCriteriaTypeDef] = ...,  # (4)
) -> GetCurrentMetricDataResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: CurrentMetricTypeDef](./type_defs.md#currentmetrictypedef) 
3. See [:material-code-brackets: GroupingType](./literals.md#groupingtype) 
4. See [:material-code-braces: CurrentMetricSortCriteriaTypeDef](./type_defs.md#currentmetricsortcriteriatypedef) 
5. See [:material-code-braces: GetCurrentMetricDataResponseTypeDef](./type_defs.md#getcurrentmetricdataresponsetypedef) 


```python
# get_current_metric_data method usage example with argument unpacking

kwargs: GetCurrentMetricDataRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Filters": ...,
    "CurrentMetrics": ...,
}

parent.get_current_metric_data(**kwargs)
```

1. See [:material-code-braces: GetCurrentMetricDataRequestRequestTypeDef](./type_defs.md#getcurrentmetricdatarequestrequesttypedef) 

### get\_current\_user\_data

Gets the real-time active user data from the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").get_current_user_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_current_user_data)

```python
# get_current_user_data method definition

await def get_current_user_data(
    self,
    *,
    InstanceId: str,
    Filters: UserDataFiltersTypeDef,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetCurrentUserDataResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UserDataFiltersTypeDef](./type_defs.md#userdatafilterstypedef) 
2. See [:material-code-braces: GetCurrentUserDataResponseTypeDef](./type_defs.md#getcurrentuserdataresponsetypedef) 


```python
# get_current_user_data method usage example with argument unpacking

kwargs: GetCurrentUserDataRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Filters": ...,
}

parent.get_current_user_data(**kwargs)
```

1. See [:material-code-braces: GetCurrentUserDataRequestRequestTypeDef](./type_defs.md#getcurrentuserdatarequestrequesttypedef) 

### get\_federation\_token

Retrieves a token for federation.

Type annotations and code completion for `#!python session.create_client("connect").get_federation_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_federation_token)

```python
# get_federation_token method definition

await def get_federation_token(
    self,
    *,
    InstanceId: str,
) -> GetFederationTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFederationTokenResponseTypeDef](./type_defs.md#getfederationtokenresponsetypedef) 


```python
# get_federation_token method usage example with argument unpacking

kwargs: GetFederationTokenRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.get_federation_token(**kwargs)
```

1. See [:material-code-braces: GetFederationTokenRequestRequestTypeDef](./type_defs.md#getfederationtokenrequestrequesttypedef) 

### get\_metric\_data

Gets historical metric data from the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").get_metric_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data)

```python
# get_metric_data method definition

await def get_metric_data(
    self,
    *,
    InstanceId: str,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    Filters: FiltersTypeDef,  # (1)
    HistoricalMetrics: Sequence[HistoricalMetricTypeDef],  # (2)
    Groupings: Sequence[GroupingType] = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetMetricDataResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef) 
3. See [:material-code-brackets: GroupingType](./literals.md#groupingtype) 
4. See [:material-code-braces: GetMetricDataResponseTypeDef](./type_defs.md#getmetricdataresponsetypedef) 


```python
# get_metric_data method usage example with argument unpacking

kwargs: GetMetricDataRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "StartTime": ...,
    "EndTime": ...,
    "Filters": ...,
    "HistoricalMetrics": ...,
}

parent.get_metric_data(**kwargs)
```

1. See [:material-code-braces: GetMetricDataRequestRequestTypeDef](./type_defs.md#getmetricdatarequestrequesttypedef) 

### get\_metric\_data\_v2

Gets metric data from the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").get_metric_data_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_metric_data_v2)

```python
# get_metric_data_v2 method definition

await def get_metric_data_v2(
    self,
    *,
    ResourceArn: str,
    StartTime: Union[datetime, str],
    EndTime: Union[datetime, str],
    Filters: Sequence[FilterV2TypeDef],  # (1)
    Metrics: Sequence[MetricV2TypeDef],  # (2)
    Groupings: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetMetricDataV2ResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterV2TypeDef](./type_defs.md#filterv2typedef) 
2. See [:material-code-braces: MetricV2TypeDef](./type_defs.md#metricv2typedef) 
3. See [:material-code-braces: GetMetricDataV2ResponseTypeDef](./type_defs.md#getmetricdatav2responsetypedef) 


```python
# get_metric_data_v2 method usage example with argument unpacking

kwargs: GetMetricDataV2RequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "StartTime": ...,
    "EndTime": ...,
    "Filters": ...,
    "Metrics": ...,
}

parent.get_metric_data_v2(**kwargs)
```

1. See [:material-code-braces: GetMetricDataV2RequestRequestTypeDef](./type_defs.md#getmetricdatav2requestrequesttypedef) 

### get\_prompt\_file

Gets the prompt file.

Type annotations and code completion for `#!python session.create_client("connect").get_prompt_file` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_prompt_file)

```python
# get_prompt_file method definition

await def get_prompt_file(
    self,
    *,
    InstanceId: str,
    PromptId: str,
) -> GetPromptFileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPromptFileResponseTypeDef](./type_defs.md#getpromptfileresponsetypedef) 


```python
# get_prompt_file method usage example with argument unpacking

kwargs: GetPromptFileRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "PromptId": ...,
}

parent.get_prompt_file(**kwargs)
```

1. See [:material-code-braces: GetPromptFileRequestRequestTypeDef](./type_defs.md#getpromptfilerequestrequesttypedef) 

### get\_task\_template

Gets details about a specific task template in the specified Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").get_task_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_task_template)

```python
# get_task_template method definition

await def get_task_template(
    self,
    *,
    InstanceId: str,
    TaskTemplateId: str,
    SnapshotVersion: str = ...,
) -> GetTaskTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTaskTemplateResponseTypeDef](./type_defs.md#gettasktemplateresponsetypedef) 


```python
# get_task_template method usage example with argument unpacking

kwargs: GetTaskTemplateRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "TaskTemplateId": ...,
}

parent.get_task_template(**kwargs)
```

1. See [:material-code-braces: GetTaskTemplateRequestRequestTypeDef](./type_defs.md#gettasktemplaterequestrequesttypedef) 

### get\_traffic\_distribution

Retrieves the current traffic distribution for a given traffic distribution
group.

Type annotations and code completion for `#!python session.create_client("connect").get_traffic_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.get_traffic_distribution)

```python
# get_traffic_distribution method definition

await def get_traffic_distribution(
    self,
    *,
    Id: str,
) -> GetTrafficDistributionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrafficDistributionResponseTypeDef](./type_defs.md#gettrafficdistributionresponsetypedef) 


```python
# get_traffic_distribution method usage example with argument unpacking

kwargs: GetTrafficDistributionRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_traffic_distribution(**kwargs)
```

1. See [:material-code-braces: GetTrafficDistributionRequestRequestTypeDef](./type_defs.md#gettrafficdistributionrequestrequesttypedef) 

### list\_agent\_statuses

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_agent_statuses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_agent_statuses)

```python
# list_agent_statuses method definition

await def list_agent_statuses(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    AgentStatusTypes: Sequence[AgentStatusTypeType] = ...,  # (1)
) -> ListAgentStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AgentStatusTypeType](./literals.md#agentstatustypetype) 
2. See [:material-code-braces: ListAgentStatusResponseTypeDef](./type_defs.md#listagentstatusresponsetypedef) 


```python
# list_agent_statuses method usage example with argument unpacking

kwargs: ListAgentStatusRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_agent_statuses(**kwargs)
```

1. See [:material-code-braces: ListAgentStatusRequestRequestTypeDef](./type_defs.md#listagentstatusrequestrequesttypedef) 

### list\_approved\_origins

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_approved_origins` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_approved_origins)

```python
# list_approved_origins method definition

await def list_approved_origins(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListApprovedOriginsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApprovedOriginsResponseTypeDef](./type_defs.md#listapprovedoriginsresponsetypedef) 


```python
# list_approved_origins method usage example with argument unpacking

kwargs: ListApprovedOriginsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_approved_origins(**kwargs)
```

1. See [:material-code-braces: ListApprovedOriginsRequestRequestTypeDef](./type_defs.md#listapprovedoriginsrequestrequesttypedef) 

### list\_bots

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_bots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_bots)

```python
# list_bots method definition

await def list_bots(
    self,
    *,
    InstanceId: str,
    LexVersion: LexVersionType,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListBotsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LexVersionType](./literals.md#lexversiontype) 
2. See [:material-code-braces: ListBotsResponseTypeDef](./type_defs.md#listbotsresponsetypedef) 


```python
# list_bots method usage example with argument unpacking

kwargs: ListBotsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "LexVersion": ...,
}

parent.list_bots(**kwargs)
```

1. See [:material-code-braces: ListBotsRequestRequestTypeDef](./type_defs.md#listbotsrequestrequesttypedef) 

### list\_contact\_evaluations

Lists contact evaluations in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_contact_evaluations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_evaluations)

```python
# list_contact_evaluations method definition

await def list_contact_evaluations(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    NextToken: str = ...,
) -> ListContactEvaluationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListContactEvaluationsResponseTypeDef](./type_defs.md#listcontactevaluationsresponsetypedef) 


```python
# list_contact_evaluations method usage example with argument unpacking

kwargs: ListContactEvaluationsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
}

parent.list_contact_evaluations(**kwargs)
```

1. See [:material-code-braces: ListContactEvaluationsRequestRequestTypeDef](./type_defs.md#listcontactevaluationsrequestrequesttypedef) 

### list\_contact\_flow\_modules

Provides information about the flow modules for the specified Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").list_contact_flow_modules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flow_modules)

```python
# list_contact_flow_modules method definition

await def list_contact_flow_modules(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    ContactFlowModuleState: ContactFlowModuleStateType = ...,  # (1)
) -> ListContactFlowModulesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 
2. See [:material-code-braces: ListContactFlowModulesResponseTypeDef](./type_defs.md#listcontactflowmodulesresponsetypedef) 


```python
# list_contact_flow_modules method usage example with argument unpacking

kwargs: ListContactFlowModulesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_contact_flow_modules(**kwargs)
```

1. See [:material-code-braces: ListContactFlowModulesRequestRequestTypeDef](./type_defs.md#listcontactflowmodulesrequestrequesttypedef) 

### list\_contact\_flows

Provides information about the flows for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_contact_flows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_flows)

```python
# list_contact_flows method definition

await def list_contact_flows(
    self,
    *,
    InstanceId: str,
    ContactFlowTypes: Sequence[ContactFlowTypeType] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListContactFlowsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-braces: ListContactFlowsResponseTypeDef](./type_defs.md#listcontactflowsresponsetypedef) 


```python
# list_contact_flows method usage example with argument unpacking

kwargs: ListContactFlowsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_contact_flows(**kwargs)
```

1. See [:material-code-braces: ListContactFlowsRequestRequestTypeDef](./type_defs.md#listcontactflowsrequestrequesttypedef) 

### list\_contact\_references

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_contact_references` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_contact_references)

```python
# list_contact_references method definition

await def list_contact_references(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    ReferenceTypes: Sequence[ReferenceTypeType],  # (1)
    NextToken: str = ...,
) -> ListContactReferencesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReferenceTypeType](./literals.md#referencetypetype) 
2. See [:material-code-braces: ListContactReferencesResponseTypeDef](./type_defs.md#listcontactreferencesresponsetypedef) 


```python
# list_contact_references method usage example with argument unpacking

kwargs: ListContactReferencesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "ReferenceTypes": ...,
}

parent.list_contact_references(**kwargs)
```

1. See [:material-code-braces: ListContactReferencesRequestRequestTypeDef](./type_defs.md#listcontactreferencesrequestrequesttypedef) 

### list\_default\_vocabularies

Lists the default vocabularies for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_default_vocabularies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_default_vocabularies)

```python
# list_default_vocabularies method definition

await def list_default_vocabularies(
    self,
    *,
    InstanceId: str,
    LanguageCode: VocabularyLanguageCodeType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDefaultVocabulariesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
2. See [:material-code-braces: ListDefaultVocabulariesResponseTypeDef](./type_defs.md#listdefaultvocabulariesresponsetypedef) 


```python
# list_default_vocabularies method usage example with argument unpacking

kwargs: ListDefaultVocabulariesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_default_vocabularies(**kwargs)
```

1. See [:material-code-braces: ListDefaultVocabulariesRequestRequestTypeDef](./type_defs.md#listdefaultvocabulariesrequestrequesttypedef) 

### list\_evaluation\_form\_versions

Lists versions of an evaluation form in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_evaluation_form_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_evaluation_form_versions)

```python
# list_evaluation_form_versions method definition

await def list_evaluation_form_versions(
    self,
    *,
    InstanceId: str,
    EvaluationFormId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListEvaluationFormVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEvaluationFormVersionsResponseTypeDef](./type_defs.md#listevaluationformversionsresponsetypedef) 


```python
# list_evaluation_form_versions method usage example with argument unpacking

kwargs: ListEvaluationFormVersionsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationFormId": ...,
}

parent.list_evaluation_form_versions(**kwargs)
```

1. See [:material-code-braces: ListEvaluationFormVersionsRequestRequestTypeDef](./type_defs.md#listevaluationformversionsrequestrequesttypedef) 

### list\_evaluation\_forms

Lists evaluation forms in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_evaluation_forms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_evaluation_forms)

```python
# list_evaluation_forms method definition

await def list_evaluation_forms(
    self,
    *,
    InstanceId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListEvaluationFormsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEvaluationFormsResponseTypeDef](./type_defs.md#listevaluationformsresponsetypedef) 


```python
# list_evaluation_forms method usage example with argument unpacking

kwargs: ListEvaluationFormsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_evaluation_forms(**kwargs)
```

1. See [:material-code-braces: ListEvaluationFormsRequestRequestTypeDef](./type_defs.md#listevaluationformsrequestrequesttypedef) 

### list\_hours\_of\_operations

Provides information about the hours of operation for the specified Amazon
Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_hours_of_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_hours_of_operations)

```python
# list_hours_of_operations method definition

await def list_hours_of_operations(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListHoursOfOperationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListHoursOfOperationsResponseTypeDef](./type_defs.md#listhoursofoperationsresponsetypedef) 


```python
# list_hours_of_operations method usage example with argument unpacking

kwargs: ListHoursOfOperationsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_hours_of_operations(**kwargs)
```

1. See [:material-code-braces: ListHoursOfOperationsRequestRequestTypeDef](./type_defs.md#listhoursofoperationsrequestrequesttypedef) 

### list\_instance\_attributes

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_instance_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_attributes)

```python
# list_instance_attributes method definition

await def list_instance_attributes(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListInstanceAttributesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInstanceAttributesResponseTypeDef](./type_defs.md#listinstanceattributesresponsetypedef) 


```python
# list_instance_attributes method usage example with argument unpacking

kwargs: ListInstanceAttributesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_instance_attributes(**kwargs)
```

1. See [:material-code-braces: ListInstanceAttributesRequestRequestTypeDef](./type_defs.md#listinstanceattributesrequestrequesttypedef) 

### list\_instance\_storage\_configs

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_instance_storage_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instance_storage_configs)

```python
# list_instance_storage_configs method definition

await def list_instance_storage_configs(
    self,
    *,
    InstanceId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListInstanceStorageConfigsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: ListInstanceStorageConfigsResponseTypeDef](./type_defs.md#listinstancestorageconfigsresponsetypedef) 


```python
# list_instance_storage_configs method usage example with argument unpacking

kwargs: ListInstanceStorageConfigsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ResourceType": ...,
}

parent.list_instance_storage_configs(**kwargs)
```

1. See [:material-code-braces: ListInstanceStorageConfigsRequestRequestTypeDef](./type_defs.md#listinstancestorageconfigsrequestrequesttypedef) 

### list\_instances

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_instances)

```python
# list_instances method definition

await def list_instances(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListInstancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


```python
# list_instances method usage example with argument unpacking

kwargs: ListInstancesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_instances(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestRequestTypeDef](./type_defs.md#listinstancesrequestrequesttypedef) 

### list\_integration\_associations

Provides summary information about the Amazon Web Services resource associations
for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_integration_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_integration_associations)

```python
# list_integration_associations method definition

await def list_integration_associations(
    self,
    *,
    InstanceId: str,
    IntegrationType: IntegrationTypeType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListIntegrationAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-braces: ListIntegrationAssociationsResponseTypeDef](./type_defs.md#listintegrationassociationsresponsetypedef) 


```python
# list_integration_associations method usage example with argument unpacking

kwargs: ListIntegrationAssociationsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_integration_associations(**kwargs)
```

1. See [:material-code-braces: ListIntegrationAssociationsRequestRequestTypeDef](./type_defs.md#listintegrationassociationsrequestrequesttypedef) 

### list\_lambda\_functions

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_lambda_functions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_lambda_functions)

```python
# list_lambda_functions method definition

await def list_lambda_functions(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLambdaFunctionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLambdaFunctionsResponseTypeDef](./type_defs.md#listlambdafunctionsresponsetypedef) 


```python
# list_lambda_functions method usage example with argument unpacking

kwargs: ListLambdaFunctionsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_lambda_functions(**kwargs)
```

1. See [:material-code-braces: ListLambdaFunctionsRequestRequestTypeDef](./type_defs.md#listlambdafunctionsrequestrequesttypedef) 

### list\_lex\_bots

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_lex_bots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_lex_bots)

```python
# list_lex_bots method definition

await def list_lex_bots(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLexBotsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLexBotsResponseTypeDef](./type_defs.md#listlexbotsresponsetypedef) 


```python
# list_lex_bots method usage example with argument unpacking

kwargs: ListLexBotsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_lex_bots(**kwargs)
```

1. See [:material-code-braces: ListLexBotsRequestRequestTypeDef](./type_defs.md#listlexbotsrequestrequesttypedef) 

### list\_phone\_numbers

Provides information about the phone numbers for the specified Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").list_phone_numbers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers)

```python
# list_phone_numbers method definition

await def list_phone_numbers(
    self,
    *,
    InstanceId: str,
    PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,  # (1)
    PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPhoneNumbersResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
2. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
3. See [:material-code-braces: ListPhoneNumbersResponseTypeDef](./type_defs.md#listphonenumbersresponsetypedef) 


```python
# list_phone_numbers method usage example with argument unpacking

kwargs: ListPhoneNumbersRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_phone_numbers(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumbersRequestRequestTypeDef](./type_defs.md#listphonenumbersrequestrequesttypedef) 

### list\_phone\_numbers\_v2

Lists phone numbers claimed to your Amazon Connect instance or traffic
distribution group.

Type annotations and code completion for `#!python session.create_client("connect").list_phone_numbers_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_phone_numbers_v2)

```python
# list_phone_numbers_v2 method definition

await def list_phone_numbers_v2(
    self,
    *,
    TargetArn: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    PhoneNumberCountryCodes: Sequence[PhoneNumberCountryCodeType] = ...,  # (1)
    PhoneNumberTypes: Sequence[PhoneNumberTypeType] = ...,  # (2)
    PhoneNumberPrefix: str = ...,
) -> ListPhoneNumbersV2ResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
3. See [:material-code-braces: ListPhoneNumbersV2ResponseTypeDef](./type_defs.md#listphonenumbersv2responsetypedef) 


```python
# list_phone_numbers_v2 method usage example with argument unpacking

kwargs: ListPhoneNumbersV2RequestRequestTypeDef = {  # (1)
    "TargetArn": ...,
}

parent.list_phone_numbers_v2(**kwargs)
```

1. See [:material-code-braces: ListPhoneNumbersV2RequestRequestTypeDef](./type_defs.md#listphonenumbersv2requestrequesttypedef) 

### list\_prompts

Provides information about the prompts for the specified Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").list_prompts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_prompts)

```python
# list_prompts method definition

await def list_prompts(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPromptsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPromptsResponseTypeDef](./type_defs.md#listpromptsresponsetypedef) 


```python
# list_prompts method usage example with argument unpacking

kwargs: ListPromptsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_prompts(**kwargs)
```

1. See [:material-code-braces: ListPromptsRequestRequestTypeDef](./type_defs.md#listpromptsrequestrequesttypedef) 

### list\_queue\_quick\_connects

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_queue_quick_connects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queue_quick_connects)

```python
# list_queue_quick_connects method definition

await def list_queue_quick_connects(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListQueueQuickConnectsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQueueQuickConnectsResponseTypeDef](./type_defs.md#listqueuequickconnectsresponsetypedef) 


```python
# list_queue_quick_connects method usage example with argument unpacking

kwargs: ListQueueQuickConnectsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
}

parent.list_queue_quick_connects(**kwargs)
```

1. See [:material-code-braces: ListQueueQuickConnectsRequestRequestTypeDef](./type_defs.md#listqueuequickconnectsrequestrequesttypedef) 

### list\_queues

Provides information about the queues for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_queues)

```python
# list_queues method definition

await def list_queues(
    self,
    *,
    InstanceId: str,
    QueueTypes: Sequence[QueueTypeType] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListQueuesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueueTypeType](./literals.md#queuetypetype) 
2. See [:material-code-braces: ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef) 


```python
# list_queues method usage example with argument unpacking

kwargs: ListQueuesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_queues(**kwargs)
```

1. See [:material-code-braces: ListQueuesRequestRequestTypeDef](./type_defs.md#listqueuesrequestrequesttypedef) 

### list\_quick\_connects

Provides information about the quick connects for the specified Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").list_quick_connects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_quick_connects)

```python
# list_quick_connects method definition

await def list_quick_connects(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    QuickConnectTypes: Sequence[QuickConnectTypeType] = ...,  # (1)
) -> ListQuickConnectsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QuickConnectTypeType](./literals.md#quickconnecttypetype) 
2. See [:material-code-braces: ListQuickConnectsResponseTypeDef](./type_defs.md#listquickconnectsresponsetypedef) 


```python
# list_quick_connects method usage example with argument unpacking

kwargs: ListQuickConnectsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_quick_connects(**kwargs)
```

1. See [:material-code-braces: ListQuickConnectsRequestRequestTypeDef](./type_defs.md#listquickconnectsrequestrequesttypedef) 

### list\_routing\_profile\_queues

Lists the queues associated with a routing profile.

Type annotations and code completion for `#!python session.create_client("connect").list_routing_profile_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_routing_profile_queues)

```python
# list_routing_profile_queues method definition

await def list_routing_profile_queues(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRoutingProfileQueuesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRoutingProfileQueuesResponseTypeDef](./type_defs.md#listroutingprofilequeuesresponsetypedef) 


```python
# list_routing_profile_queues method usage example with argument unpacking

kwargs: ListRoutingProfileQueuesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
}

parent.list_routing_profile_queues(**kwargs)
```

1. See [:material-code-braces: ListRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#listroutingprofilequeuesrequestrequesttypedef) 

### list\_routing\_profiles

Provides summary information about the routing profiles for the specified Amazon
Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_routing_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_routing_profiles)

```python
# list_routing_profiles method definition

await def list_routing_profiles(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListRoutingProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRoutingProfilesResponseTypeDef](./type_defs.md#listroutingprofilesresponsetypedef) 


```python
# list_routing_profiles method usage example with argument unpacking

kwargs: ListRoutingProfilesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_routing_profiles(**kwargs)
```

1. See [:material-code-braces: ListRoutingProfilesRequestRequestTypeDef](./type_defs.md#listroutingprofilesrequestrequesttypedef) 

### list\_rules

List all rules for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_rules)

```python
# list_rules method definition

await def list_rules(
    self,
    *,
    InstanceId: str,
    PublishStatus: RulePublishStatusType = ...,  # (1)
    EventSourceName: EventSourceNameType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRulesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
2. See [:material-code-brackets: EventSourceNameType](./literals.md#eventsourcenametype) 
3. See [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


```python
# list_rules method usage example with argument unpacking

kwargs: ListRulesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_rules(**kwargs)
```

1. See [:material-code-braces: ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef) 

### list\_security\_keys

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_security_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_keys)

```python
# list_security_keys method definition

await def list_security_keys(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSecurityKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSecurityKeysResponseTypeDef](./type_defs.md#listsecuritykeysresponsetypedef) 


```python
# list_security_keys method usage example with argument unpacking

kwargs: ListSecurityKeysRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_security_keys(**kwargs)
```

1. See [:material-code-braces: ListSecurityKeysRequestRequestTypeDef](./type_defs.md#listsecuritykeysrequestrequesttypedef) 

### list\_security\_profile\_permissions

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_security_profile_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profile_permissions)

```python
# list_security_profile_permissions method definition

await def list_security_profile_permissions(
    self,
    *,
    SecurityProfileId: str,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSecurityProfilePermissionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSecurityProfilePermissionsResponseTypeDef](./type_defs.md#listsecurityprofilepermissionsresponsetypedef) 


```python
# list_security_profile_permissions method usage example with argument unpacking

kwargs: ListSecurityProfilePermissionsRequestRequestTypeDef = {  # (1)
    "SecurityProfileId": ...,
    "InstanceId": ...,
}

parent.list_security_profile_permissions(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilePermissionsRequestRequestTypeDef](./type_defs.md#listsecurityprofilepermissionsrequestrequesttypedef) 

### list\_security\_profiles

Provides summary information about the security profiles for the specified
Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_security_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_security_profiles)

```python
# list_security_profiles method definition

await def list_security_profiles(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSecurityProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSecurityProfilesResponseTypeDef](./type_defs.md#listsecurityprofilesresponsetypedef) 


```python
# list_security_profiles method usage example with argument unpacking

kwargs: ListSecurityProfilesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_security_profiles(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfilesRequestRequestTypeDef](./type_defs.md#listsecurityprofilesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("connect").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_tags_for_resource)

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

### list\_task\_templates

Lists task templates for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_task_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_task_templates)

```python
# list_task_templates method definition

await def list_task_templates(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    Status: TaskTemplateStatusType = ...,  # (1)
    Name: str = ...,
) -> ListTaskTemplatesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
2. See [:material-code-braces: ListTaskTemplatesResponseTypeDef](./type_defs.md#listtasktemplatesresponsetypedef) 


```python
# list_task_templates method usage example with argument unpacking

kwargs: ListTaskTemplatesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_task_templates(**kwargs)
```

1. See [:material-code-braces: ListTaskTemplatesRequestRequestTypeDef](./type_defs.md#listtasktemplatesrequestrequesttypedef) 

### list\_traffic\_distribution\_group\_users

Lists traffic distribution group users.

Type annotations and code completion for `#!python session.create_client("connect").list_traffic_distribution_group_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_traffic_distribution_group_users)

```python
# list_traffic_distribution_group_users method definition

await def list_traffic_distribution_group_users(
    self,
    *,
    TrafficDistributionGroupId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTrafficDistributionGroupUsersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrafficDistributionGroupUsersResponseTypeDef](./type_defs.md#listtrafficdistributiongroupusersresponsetypedef) 


```python
# list_traffic_distribution_group_users method usage example with argument unpacking

kwargs: ListTrafficDistributionGroupUsersRequestRequestTypeDef = {  # (1)
    "TrafficDistributionGroupId": ...,
}

parent.list_traffic_distribution_group_users(**kwargs)
```

1. See [:material-code-braces: ListTrafficDistributionGroupUsersRequestRequestTypeDef](./type_defs.md#listtrafficdistributiongroupusersrequestrequesttypedef) 

### list\_traffic\_distribution\_groups

Lists traffic distribution groups.

Type annotations and code completion for `#!python session.create_client("connect").list_traffic_distribution_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_traffic_distribution_groups)

```python
# list_traffic_distribution_groups method definition

await def list_traffic_distribution_groups(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    InstanceId: str = ...,
) -> ListTrafficDistributionGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrafficDistributionGroupsResponseTypeDef](./type_defs.md#listtrafficdistributiongroupsresponsetypedef) 


```python
# list_traffic_distribution_groups method usage example with argument unpacking

kwargs: ListTrafficDistributionGroupsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_traffic_distribution_groups(**kwargs)
```

1. See [:material-code-braces: ListTrafficDistributionGroupsRequestRequestTypeDef](./type_defs.md#listtrafficdistributiongroupsrequestrequesttypedef) 

### list\_use\_cases

Lists the use cases for the integration association.

Type annotations and code completion for `#!python session.create_client("connect").list_use_cases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_use_cases)

```python
# list_use_cases method definition

await def list_use_cases(
    self,
    *,
    InstanceId: str,
    IntegrationAssociationId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListUseCasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUseCasesResponseTypeDef](./type_defs.md#listusecasesresponsetypedef) 


```python
# list_use_cases method usage example with argument unpacking

kwargs: ListUseCasesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "IntegrationAssociationId": ...,
}

parent.list_use_cases(**kwargs)
```

1. See [:material-code-braces: ListUseCasesRequestRequestTypeDef](./type_defs.md#listusecasesrequestrequesttypedef) 

### list\_user\_hierarchy\_groups

Provides summary information about the hierarchy groups for the specified Amazon
Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_user_hierarchy_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_user_hierarchy_groups)

```python
# list_user_hierarchy_groups method definition

await def list_user_hierarchy_groups(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListUserHierarchyGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUserHierarchyGroupsResponseTypeDef](./type_defs.md#listuserhierarchygroupsresponsetypedef) 


```python
# list_user_hierarchy_groups method usage example with argument unpacking

kwargs: ListUserHierarchyGroupsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_user_hierarchy_groups(**kwargs)
```

1. See [:material-code-braces: ListUserHierarchyGroupsRequestRequestTypeDef](./type_defs.md#listuserhierarchygroupsrequestrequesttypedef) 

### list\_users

Provides summary information about the users for the specified Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.list_users)

```python
# list_users method definition

await def list_users(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListUsersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef) 


```python
# list_users method usage example with argument unpacking

kwargs: ListUsersRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_users(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef) 

### monitor\_contact

Initiates silent monitoring of a contact.

Type annotations and code completion for `#!python session.create_client("connect").monitor_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.monitor_contact)

```python
# monitor_contact method definition

await def monitor_contact(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    UserId: str,
    AllowedMonitorCapabilities: Sequence[MonitorCapabilityType] = ...,  # (1)
    ClientToken: str = ...,
) -> MonitorContactResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MonitorCapabilityType](./literals.md#monitorcapabilitytype) 
2. See [:material-code-braces: MonitorContactResponseTypeDef](./type_defs.md#monitorcontactresponsetypedef) 


```python
# monitor_contact method usage example with argument unpacking

kwargs: MonitorContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "UserId": ...,
}

parent.monitor_contact(**kwargs)
```

1. See [:material-code-braces: MonitorContactRequestRequestTypeDef](./type_defs.md#monitorcontactrequestrequesttypedef) 

### put\_user\_status

Changes the current status of a user or agent in Amazon Connect.

Type annotations and code completion for `#!python session.create_client("connect").put_user_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.put_user_status)

```python
# put_user_status method definition

await def put_user_status(
    self,
    *,
    UserId: str,
    InstanceId: str,
    AgentStatusId: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_user_status method usage example with argument unpacking

kwargs: PutUserStatusRequestRequestTypeDef = {  # (1)
    "UserId": ...,
    "InstanceId": ...,
    "AgentStatusId": ...,
}

parent.put_user_status(**kwargs)
```

1. See [:material-code-braces: PutUserStatusRequestRequestTypeDef](./type_defs.md#putuserstatusrequestrequesttypedef) 

### release\_phone\_number

Releases a phone number previously claimed to an Amazon Connect instance or
traffic distribution group.

Type annotations and code completion for `#!python session.create_client("connect").release_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.release_phone_number)

```python
# release_phone_number method definition

await def release_phone_number(
    self,
    *,
    PhoneNumberId: str,
    ClientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# release_phone_number method usage example with argument unpacking

kwargs: ReleasePhoneNumberRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.release_phone_number(**kwargs)
```

1. See [:material-code-braces: ReleasePhoneNumberRequestRequestTypeDef](./type_defs.md#releasephonenumberrequestrequesttypedef) 

### replicate\_instance

Replicates an Amazon Connect instance in the specified Amazon Web Services
Region.

Type annotations and code completion for `#!python session.create_client("connect").replicate_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.replicate_instance)

```python
# replicate_instance method definition

await def replicate_instance(
    self,
    *,
    InstanceId: str,
    ReplicaRegion: str,
    ReplicaAlias: str,
    ClientToken: str = ...,
) -> ReplicateInstanceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ReplicateInstanceResponseTypeDef](./type_defs.md#replicateinstanceresponsetypedef) 


```python
# replicate_instance method usage example with argument unpacking

kwargs: ReplicateInstanceRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ReplicaRegion": ...,
    "ReplicaAlias": ...,
}

parent.replicate_instance(**kwargs)
```

1. See [:material-code-braces: ReplicateInstanceRequestRequestTypeDef](./type_defs.md#replicateinstancerequestrequesttypedef) 

### resume\_contact\_recording

When a contact is being recorded, and the recording has been suspended using
SuspendContactRecording, this API resumes recording the call or screen.

Type annotations and code completion for `#!python session.create_client("connect").resume_contact_recording` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.resume_contact_recording)

```python
# resume_contact_recording method definition

await def resume_contact_recording(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
) -> Dict[str, Any]:
    ...
```



```python
# resume_contact_recording method usage example with argument unpacking

kwargs: ResumeContactRecordingRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "InitialContactId": ...,
}

parent.resume_contact_recording(**kwargs)
```

1. See [:material-code-braces: ResumeContactRecordingRequestRequestTypeDef](./type_defs.md#resumecontactrecordingrequestrequesttypedef) 

### search\_available\_phone\_numbers

Searches for available phone numbers that you can claim to your Amazon Connect
instance or traffic distribution group.

Type annotations and code completion for `#!python session.create_client("connect").search_available_phone_numbers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_available_phone_numbers)

```python
# search_available_phone_numbers method definition

await def search_available_phone_numbers(
    self,
    *,
    TargetArn: str,
    PhoneNumberCountryCode: PhoneNumberCountryCodeType,  # (1)
    PhoneNumberType: PhoneNumberTypeType,  # (2)
    PhoneNumberPrefix: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> SearchAvailablePhoneNumbersResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype) 
2. See [:material-code-brackets: PhoneNumberTypeType](./literals.md#phonenumbertypetype) 
3. See [:material-code-braces: SearchAvailablePhoneNumbersResponseTypeDef](./type_defs.md#searchavailablephonenumbersresponsetypedef) 


```python
# search_available_phone_numbers method usage example with argument unpacking

kwargs: SearchAvailablePhoneNumbersRequestRequestTypeDef = {  # (1)
    "TargetArn": ...,
    "PhoneNumberCountryCode": ...,
    "PhoneNumberType": ...,
}

parent.search_available_phone_numbers(**kwargs)
```

1. See [:material-code-braces: SearchAvailablePhoneNumbersRequestRequestTypeDef](./type_defs.md#searchavailablephonenumbersrequestrequesttypedef) 

### search\_hours\_of\_operations

Searches the hours of operation in an Amazon Connect instance, with optional
filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_hours_of_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_hours_of_operations)

```python
# search_hours_of_operations method definition

await def search_hours_of_operations(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: HoursOfOperationSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: HoursOfOperationSearchCriteriaTypeDef = ...,  # (2)
) -> SearchHoursOfOperationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: HoursOfOperationSearchFilterTypeDef](./type_defs.md#hoursofoperationsearchfiltertypedef) 
2. See [:material-code-braces: HoursOfOperationSearchCriteriaTypeDef](./type_defs.md#hoursofoperationsearchcriteriatypedef) 
3. See [:material-code-braces: SearchHoursOfOperationsResponseTypeDef](./type_defs.md#searchhoursofoperationsresponsetypedef) 


```python
# search_hours_of_operations method usage example with argument unpacking

kwargs: SearchHoursOfOperationsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_hours_of_operations(**kwargs)
```

1. See [:material-code-braces: SearchHoursOfOperationsRequestRequestTypeDef](./type_defs.md#searchhoursofoperationsrequestrequesttypedef) 

### search\_prompts

Searches prompts in an Amazon Connect instance, with optional filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_prompts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_prompts)

```python
# search_prompts method definition

await def search_prompts(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: PromptSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: PromptSearchCriteriaTypeDef = ...,  # (2)
) -> SearchPromptsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PromptSearchFilterTypeDef](./type_defs.md#promptsearchfiltertypedef) 
2. See [:material-code-braces: PromptSearchCriteriaTypeDef](./type_defs.md#promptsearchcriteriatypedef) 
3. See [:material-code-braces: SearchPromptsResponseTypeDef](./type_defs.md#searchpromptsresponsetypedef) 


```python
# search_prompts method usage example with argument unpacking

kwargs: SearchPromptsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_prompts(**kwargs)
```

1. See [:material-code-braces: SearchPromptsRequestRequestTypeDef](./type_defs.md#searchpromptsrequestrequesttypedef) 

### search\_queues

Searches queues in an Amazon Connect instance, with optional filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_queues)

```python
# search_queues method definition

await def search_queues(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: QueueSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: QueueSearchCriteriaTypeDef = ...,  # (2)
) -> SearchQueuesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: QueueSearchFilterTypeDef](./type_defs.md#queuesearchfiltertypedef) 
2. See [:material-code-braces: QueueSearchCriteriaTypeDef](./type_defs.md#queuesearchcriteriatypedef) 
3. See [:material-code-braces: SearchQueuesResponseTypeDef](./type_defs.md#searchqueuesresponsetypedef) 


```python
# search_queues method usage example with argument unpacking

kwargs: SearchQueuesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_queues(**kwargs)
```

1. See [:material-code-braces: SearchQueuesRequestRequestTypeDef](./type_defs.md#searchqueuesrequestrequesttypedef) 

### search\_quick\_connects

Searches quick connects in an Amazon Connect instance, with optional filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_quick_connects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_quick_connects)

```python
# search_quick_connects method definition

await def search_quick_connects(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: QuickConnectSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: QuickConnectSearchCriteriaTypeDef = ...,  # (2)
) -> SearchQuickConnectsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: QuickConnectSearchFilterTypeDef](./type_defs.md#quickconnectsearchfiltertypedef) 
2. See [:material-code-braces: QuickConnectSearchCriteriaTypeDef](./type_defs.md#quickconnectsearchcriteriatypedef) 
3. See [:material-code-braces: SearchQuickConnectsResponseTypeDef](./type_defs.md#searchquickconnectsresponsetypedef) 


```python
# search_quick_connects method usage example with argument unpacking

kwargs: SearchQuickConnectsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_quick_connects(**kwargs)
```

1. See [:material-code-braces: SearchQuickConnectsRequestRequestTypeDef](./type_defs.md#searchquickconnectsrequestrequesttypedef) 

### search\_resource\_tags

Searches tags used in an Amazon Connect instance using optional search criteria.

Type annotations and code completion for `#!python session.create_client("connect").search_resource_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_resource_tags)

```python
# search_resource_tags method definition

await def search_resource_tags(
    self,
    *,
    InstanceId: str,
    ResourceTypes: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchCriteria: ResourceTagsSearchCriteriaTypeDef = ...,  # (1)
) -> SearchResourceTagsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ResourceTagsSearchCriteriaTypeDef](./type_defs.md#resourcetagssearchcriteriatypedef) 
2. See [:material-code-braces: SearchResourceTagsResponseTypeDef](./type_defs.md#searchresourcetagsresponsetypedef) 


```python
# search_resource_tags method usage example with argument unpacking

kwargs: SearchResourceTagsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_resource_tags(**kwargs)
```

1. See [:material-code-braces: SearchResourceTagsRequestRequestTypeDef](./type_defs.md#searchresourcetagsrequestrequesttypedef) 

### search\_routing\_profiles

Searches routing profiles in an Amazon Connect instance, with optional
filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_routing_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_routing_profiles)

```python
# search_routing_profiles method definition

await def search_routing_profiles(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: RoutingProfileSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: RoutingProfileSearchCriteriaTypeDef = ...,  # (2)
) -> SearchRoutingProfilesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RoutingProfileSearchFilterTypeDef](./type_defs.md#routingprofilesearchfiltertypedef) 
2. See [:material-code-braces: RoutingProfileSearchCriteriaTypeDef](./type_defs.md#routingprofilesearchcriteriatypedef) 
3. See [:material-code-braces: SearchRoutingProfilesResponseTypeDef](./type_defs.md#searchroutingprofilesresponsetypedef) 


```python
# search_routing_profiles method usage example with argument unpacking

kwargs: SearchRoutingProfilesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_routing_profiles(**kwargs)
```

1. See [:material-code-braces: SearchRoutingProfilesRequestRequestTypeDef](./type_defs.md#searchroutingprofilesrequestrequesttypedef) 

### search\_security\_profiles

Searches security profiles in an Amazon Connect instance, with optional
filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_security_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_security_profiles)

```python
# search_security_profiles method definition

await def search_security_profiles(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchCriteria: SecurityProfileSearchCriteriaTypeDef = ...,  # (1)
    SearchFilter: SecurityProfilesSearchFilterTypeDef = ...,  # (2)
) -> SearchSecurityProfilesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SecurityProfileSearchCriteriaTypeDef](./type_defs.md#securityprofilesearchcriteriatypedef) 
2. See [:material-code-braces: SecurityProfilesSearchFilterTypeDef](./type_defs.md#securityprofilessearchfiltertypedef) 
3. See [:material-code-braces: SearchSecurityProfilesResponseTypeDef](./type_defs.md#searchsecurityprofilesresponsetypedef) 


```python
# search_security_profiles method usage example with argument unpacking

kwargs: SearchSecurityProfilesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_security_profiles(**kwargs)
```

1. See [:material-code-braces: SearchSecurityProfilesRequestRequestTypeDef](./type_defs.md#searchsecurityprofilesrequestrequesttypedef) 

### search\_users

Searches users in an Amazon Connect instance, with optional filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_users)

```python
# search_users method definition

await def search_users(
    self,
    *,
    InstanceId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: UserSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: UserSearchCriteriaTypeDef = ...,  # (2)
) -> SearchUsersResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UserSearchFilterTypeDef](./type_defs.md#usersearchfiltertypedef) 
2. See [:material-code-braces: UserSearchCriteriaTypeDef](./type_defs.md#usersearchcriteriatypedef) 
3. See [:material-code-braces: SearchUsersResponseTypeDef](./type_defs.md#searchusersresponsetypedef) 


```python
# search_users method usage example with argument unpacking

kwargs: SearchUsersRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_users(**kwargs)
```

1. See [:material-code-braces: SearchUsersRequestRequestTypeDef](./type_defs.md#searchusersrequestrequesttypedef) 

### search\_vocabularies

Searches for vocabularies within a specific Amazon Connect instance using
`State`, `NameStartsWith`, and `LanguageCode`.

Type annotations and code completion for `#!python session.create_client("connect").search_vocabularies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.search_vocabularies)

```python
# search_vocabularies method definition

await def search_vocabularies(
    self,
    *,
    InstanceId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    State: VocabularyStateType = ...,  # (1)
    NameStartsWith: str = ...,
    LanguageCode: VocabularyLanguageCodeType = ...,  # (2)
) -> SearchVocabulariesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: VocabularyStateType](./literals.md#vocabularystatetype) 
2. See [:material-code-brackets: VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype) 
3. See [:material-code-braces: SearchVocabulariesResponseTypeDef](./type_defs.md#searchvocabulariesresponsetypedef) 


```python
# search_vocabularies method usage example with argument unpacking

kwargs: SearchVocabulariesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_vocabularies(**kwargs)
```

1. See [:material-code-braces: SearchVocabulariesRequestRequestTypeDef](./type_defs.md#searchvocabulariesrequestrequesttypedef) 

### start\_chat\_contact

Initiates a flow to start a new chat for the customer.

Type annotations and code completion for `#!python session.create_client("connect").start_chat_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_chat_contact)

```python
# start_chat_contact method definition

await def start_chat_contact(
    self,
    *,
    InstanceId: str,
    ContactFlowId: str,
    ParticipantDetails: ParticipantDetailsTypeDef,  # (1)
    Attributes: Mapping[str, str] = ...,
    InitialMessage: ChatMessageTypeDef = ...,  # (2)
    ClientToken: str = ...,
    ChatDurationInMinutes: int = ...,
    SupportedMessagingContentTypes: Sequence[str] = ...,
    PersistentChat: PersistentChatTypeDef = ...,  # (3)
    RelatedContactId: str = ...,
) -> StartChatContactResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
2. See [:material-code-braces: ChatMessageTypeDef](./type_defs.md#chatmessagetypedef) 
3. See [:material-code-braces: PersistentChatTypeDef](./type_defs.md#persistentchattypedef) 
4. See [:material-code-braces: StartChatContactResponseTypeDef](./type_defs.md#startchatcontactresponsetypedef) 


```python
# start_chat_contact method usage example with argument unpacking

kwargs: StartChatContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowId": ...,
    "ParticipantDetails": ...,
}

parent.start_chat_contact(**kwargs)
```

1. See [:material-code-braces: StartChatContactRequestRequestTypeDef](./type_defs.md#startchatcontactrequestrequesttypedef) 

### start\_contact\_evaluation

Starts an empty evaluation in the specified Amazon Connect instance, using the
given evaluation form for the particular contact.

Type annotations and code completion for `#!python session.create_client("connect").start_contact_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_evaluation)

```python
# start_contact_evaluation method definition

await def start_contact_evaluation(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    EvaluationFormId: str,
    ClientToken: str = ...,
) -> StartContactEvaluationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartContactEvaluationResponseTypeDef](./type_defs.md#startcontactevaluationresponsetypedef) 


```python
# start_contact_evaluation method usage example with argument unpacking

kwargs: StartContactEvaluationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "EvaluationFormId": ...,
}

parent.start_contact_evaluation(**kwargs)
```

1. See [:material-code-braces: StartContactEvaluationRequestRequestTypeDef](./type_defs.md#startcontactevaluationrequestrequesttypedef) 

### start\_contact\_recording

Starts recording the contact: * If the API is called *before* the agent joins
the call, recording starts when the agent joins the call.

Type annotations and code completion for `#!python session.create_client("connect").start_contact_recording` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_recording)

```python
# start_contact_recording method definition

await def start_contact_recording(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
    VoiceRecordingConfiguration: VoiceRecordingConfigurationTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: VoiceRecordingConfigurationTypeDef](./type_defs.md#voicerecordingconfigurationtypedef) 


```python
# start_contact_recording method usage example with argument unpacking

kwargs: StartContactRecordingRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "InitialContactId": ...,
    "VoiceRecordingConfiguration": ...,
}

parent.start_contact_recording(**kwargs)
```

1. See [:material-code-braces: StartContactRecordingRequestRequestTypeDef](./type_defs.md#startcontactrecordingrequestrequesttypedef) 

### start\_contact\_streaming

Initiates real-time message streaming for a new chat contact.

Type annotations and code completion for `#!python session.create_client("connect").start_contact_streaming` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_contact_streaming)

```python
# start_contact_streaming method definition

await def start_contact_streaming(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    ChatStreamingConfiguration: ChatStreamingConfigurationTypeDef,  # (1)
    ClientToken: str,
) -> StartContactStreamingResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ChatStreamingConfigurationTypeDef](./type_defs.md#chatstreamingconfigurationtypedef) 
2. See [:material-code-braces: StartContactStreamingResponseTypeDef](./type_defs.md#startcontactstreamingresponsetypedef) 


```python
# start_contact_streaming method usage example with argument unpacking

kwargs: StartContactStreamingRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "ChatStreamingConfiguration": ...,
    "ClientToken": ...,
}

parent.start_contact_streaming(**kwargs)
```

1. See [:material-code-braces: StartContactStreamingRequestRequestTypeDef](./type_defs.md#startcontactstreamingrequestrequesttypedef) 

### start\_outbound\_voice\_contact

Places an outbound call to a contact, and then initiates the flow.

Type annotations and code completion for `#!python session.create_client("connect").start_outbound_voice_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_outbound_voice_contact)

```python
# start_outbound_voice_contact method definition

await def start_outbound_voice_contact(
    self,
    *,
    DestinationPhoneNumber: str,
    ContactFlowId: str,
    InstanceId: str,
    ClientToken: str = ...,
    SourcePhoneNumber: str = ...,
    QueueId: str = ...,
    Attributes: Mapping[str, str] = ...,
    AnswerMachineDetectionConfig: AnswerMachineDetectionConfigTypeDef = ...,  # (1)
    CampaignId: str = ...,
    TrafficType: TrafficTypeType = ...,  # (2)
) -> StartOutboundVoiceContactResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef) 
2. See [:material-code-brackets: TrafficTypeType](./literals.md#traffictypetype) 
3. See [:material-code-braces: StartOutboundVoiceContactResponseTypeDef](./type_defs.md#startoutboundvoicecontactresponsetypedef) 


```python
# start_outbound_voice_contact method usage example with argument unpacking

kwargs: StartOutboundVoiceContactRequestRequestTypeDef = {  # (1)
    "DestinationPhoneNumber": ...,
    "ContactFlowId": ...,
    "InstanceId": ...,
}

parent.start_outbound_voice_contact(**kwargs)
```

1. See [:material-code-braces: StartOutboundVoiceContactRequestRequestTypeDef](./type_defs.md#startoutboundvoicecontactrequestrequesttypedef) 

### start\_task\_contact

Initiates a flow to start a new task.

Type annotations and code completion for `#!python session.create_client("connect").start_task_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.start_task_contact)

```python
# start_task_contact method definition

await def start_task_contact(
    self,
    *,
    InstanceId: str,
    Name: str,
    PreviousContactId: str = ...,
    ContactFlowId: str = ...,
    Attributes: Mapping[str, str] = ...,
    References: Mapping[str, ReferenceTypeDef] = ...,  # (1)
    Description: str = ...,
    ClientToken: str = ...,
    ScheduledTime: Union[datetime, str] = ...,
    TaskTemplateId: str = ...,
    QuickConnectId: str = ...,
    RelatedContactId: str = ...,
) -> StartTaskContactResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
2. See [:material-code-braces: StartTaskContactResponseTypeDef](./type_defs.md#starttaskcontactresponsetypedef) 


```python
# start_task_contact method usage example with argument unpacking

kwargs: StartTaskContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
}

parent.start_task_contact(**kwargs)
```

1. See [:material-code-braces: StartTaskContactRequestRequestTypeDef](./type_defs.md#starttaskcontactrequestrequesttypedef) 

### stop\_contact

Ends the specified contact.

Type annotations and code completion for `#!python session.create_client("connect").stop_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.stop_contact)

```python
# stop_contact method definition

await def stop_contact(
    self,
    *,
    ContactId: str,
    InstanceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_contact method usage example with argument unpacking

kwargs: StopContactRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
    "InstanceId": ...,
}

parent.stop_contact(**kwargs)
```

1. See [:material-code-braces: StopContactRequestRequestTypeDef](./type_defs.md#stopcontactrequestrequesttypedef) 

### stop\_contact\_recording

Stops recording a call when a contact is being recorded.

Type annotations and code completion for `#!python session.create_client("connect").stop_contact_recording` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.stop_contact_recording)

```python
# stop_contact_recording method definition

await def stop_contact_recording(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_contact_recording method usage example with argument unpacking

kwargs: StopContactRecordingRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "InitialContactId": ...,
}

parent.stop_contact_recording(**kwargs)
```

1. See [:material-code-braces: StopContactRecordingRequestRequestTypeDef](./type_defs.md#stopcontactrecordingrequestrequesttypedef) 

### stop\_contact\_streaming

Ends message streaming on a specified contact.

Type annotations and code completion for `#!python session.create_client("connect").stop_contact_streaming` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.stop_contact_streaming)

```python
# stop_contact_streaming method definition

await def stop_contact_streaming(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    StreamingId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_contact_streaming method usage example with argument unpacking

kwargs: StopContactStreamingRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "StreamingId": ...,
}

parent.stop_contact_streaming(**kwargs)
```

1. See [:material-code-braces: StopContactStreamingRequestRequestTypeDef](./type_defs.md#stopcontactstreamingrequestrequesttypedef) 

### submit\_contact\_evaluation

Submits a contact evaluation in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").submit_contact_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.submit_contact_evaluation)

```python
# submit_contact_evaluation method definition

await def submit_contact_evaluation(
    self,
    *,
    InstanceId: str,
    EvaluationId: str,
    Answers: Mapping[str, EvaluationAnswerInputTypeDef] = ...,  # (1)
    Notes: Mapping[str, EvaluationNoteTypeDef] = ...,  # (2)
) -> SubmitContactEvaluationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EvaluationAnswerInputTypeDef](./type_defs.md#evaluationanswerinputtypedef) 
2. See [:material-code-braces: EvaluationNoteTypeDef](./type_defs.md#evaluationnotetypedef) 
3. See [:material-code-braces: SubmitContactEvaluationResponseTypeDef](./type_defs.md#submitcontactevaluationresponsetypedef) 


```python
# submit_contact_evaluation method usage example with argument unpacking

kwargs: SubmitContactEvaluationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationId": ...,
}

parent.submit_contact_evaluation(**kwargs)
```

1. See [:material-code-braces: SubmitContactEvaluationRequestRequestTypeDef](./type_defs.md#submitcontactevaluationrequestrequesttypedef) 

### suspend\_contact\_recording

When a contact is being recorded, this API suspends recording the call or
screen.

Type annotations and code completion for `#!python session.create_client("connect").suspend_contact_recording` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.suspend_contact_recording)

```python
# suspend_contact_recording method definition

await def suspend_contact_recording(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
) -> Dict[str, Any]:
    ...
```



```python
# suspend_contact_recording method usage example with argument unpacking

kwargs: SuspendContactRecordingRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "InitialContactId": ...,
}

parent.suspend_contact_recording(**kwargs)
```

1. See [:material-code-braces: SuspendContactRecordingRequestRequestTypeDef](./type_defs.md#suspendcontactrecordingrequestrequesttypedef) 

### tag\_resource

Adds the specified tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("connect").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### transfer\_contact

Transfers contacts from one agent or queue to another agent or queue at any
point after a contact is created.

Type annotations and code completion for `#!python session.create_client("connect").transfer_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.transfer_contact)

```python
# transfer_contact method definition

await def transfer_contact(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    ContactFlowId: str,
    QueueId: str = ...,
    UserId: str = ...,
    ClientToken: str = ...,
) -> TransferContactResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TransferContactResponseTypeDef](./type_defs.md#transfercontactresponsetypedef) 


```python
# transfer_contact method usage example with argument unpacking

kwargs: TransferContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "ContactFlowId": ...,
}

parent.transfer_contact(**kwargs)
```

1. See [:material-code-braces: TransferContactRequestRequestTypeDef](./type_defs.md#transfercontactrequestrequesttypedef) 

### untag\_resource

Removes the specified tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("connect").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_agent\_status

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_agent_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_agent_status)

```python
# update_agent_status method definition

await def update_agent_status(
    self,
    *,
    InstanceId: str,
    AgentStatusId: str,
    Name: str = ...,
    Description: str = ...,
    State: AgentStatusStateType = ...,  # (1)
    DisplayOrder: int = ...,
    ResetOrderNumber: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AgentStatusStateType](./literals.md#agentstatusstatetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_agent_status method usage example with argument unpacking

kwargs: UpdateAgentStatusRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "AgentStatusId": ...,
}

parent.update_agent_status(**kwargs)
```

1. See [:material-code-braces: UpdateAgentStatusRequestRequestTypeDef](./type_defs.md#updateagentstatusrequestrequesttypedef) 

### update\_contact

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact)

```python
# update_contact method definition

await def update_contact(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    Name: str = ...,
    Description: str = ...,
    References: Mapping[str, ReferenceTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 


```python
# update_contact method usage example with argument unpacking

kwargs: UpdateContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
}

parent.update_contact(**kwargs)
```

1. See [:material-code-braces: UpdateContactRequestRequestTypeDef](./type_defs.md#updatecontactrequestrequesttypedef) 

### update\_contact\_attributes

Creates or updates user-defined contact attributes associated with the specified
contact.

Type annotations and code completion for `#!python session.create_client("connect").update_contact_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_attributes)

```python
# update_contact_attributes method definition

await def update_contact_attributes(
    self,
    *,
    InitialContactId: str,
    InstanceId: str,
    Attributes: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# update_contact_attributes method usage example with argument unpacking

kwargs: UpdateContactAttributesRequestRequestTypeDef = {  # (1)
    "InitialContactId": ...,
    "InstanceId": ...,
    "Attributes": ...,
}

parent.update_contact_attributes(**kwargs)
```

1. See [:material-code-braces: UpdateContactAttributesRequestRequestTypeDef](./type_defs.md#updatecontactattributesrequestrequesttypedef) 

### update\_contact\_evaluation

Updates details about a contact evaluation in the specified Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").update_contact_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_evaluation)

```python
# update_contact_evaluation method definition

await def update_contact_evaluation(
    self,
    *,
    InstanceId: str,
    EvaluationId: str,
    Answers: Mapping[str, EvaluationAnswerInputTypeDef] = ...,  # (1)
    Notes: Mapping[str, EvaluationNoteTypeDef] = ...,  # (2)
) -> UpdateContactEvaluationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EvaluationAnswerInputTypeDef](./type_defs.md#evaluationanswerinputtypedef) 
2. See [:material-code-braces: EvaluationNoteTypeDef](./type_defs.md#evaluationnotetypedef) 
3. See [:material-code-braces: UpdateContactEvaluationResponseTypeDef](./type_defs.md#updatecontactevaluationresponsetypedef) 


```python
# update_contact_evaluation method usage example with argument unpacking

kwargs: UpdateContactEvaluationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationId": ...,
}

parent.update_contact_evaluation(**kwargs)
```

1. See [:material-code-braces: UpdateContactEvaluationRequestRequestTypeDef](./type_defs.md#updatecontactevaluationrequestrequesttypedef) 

### update\_contact\_flow\_content

Updates the specified flow.

Type annotations and code completion for `#!python session.create_client("connect").update_contact_flow_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_flow_content)

```python
# update_contact_flow_content method definition

await def update_contact_flow_content(
    self,
    *,
    InstanceId: str,
    ContactFlowId: str,
    Content: str,
) -> Dict[str, Any]:
    ...
```



```python
# update_contact_flow_content method usage example with argument unpacking

kwargs: UpdateContactFlowContentRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowId": ...,
    "Content": ...,
}

parent.update_contact_flow_content(**kwargs)
```

1. See [:material-code-braces: UpdateContactFlowContentRequestRequestTypeDef](./type_defs.md#updatecontactflowcontentrequestrequesttypedef) 

### update\_contact\_flow\_metadata

Updates metadata about specified flow.

Type annotations and code completion for `#!python session.create_client("connect").update_contact_flow_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_flow_metadata)

```python
# update_contact_flow_metadata method definition

await def update_contact_flow_metadata(
    self,
    *,
    InstanceId: str,
    ContactFlowId: str,
    Name: str = ...,
    Description: str = ...,
    ContactFlowState: ContactFlowStateType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ContactFlowStateType](./literals.md#contactflowstatetype) 


```python
# update_contact_flow_metadata method usage example with argument unpacking

kwargs: UpdateContactFlowMetadataRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowId": ...,
}

parent.update_contact_flow_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateContactFlowMetadataRequestRequestTypeDef](./type_defs.md#updatecontactflowmetadatarequestrequesttypedef) 

### update\_contact\_flow\_module\_content

Updates specified flow module for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").update_contact_flow_module_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_flow_module_content)

```python
# update_contact_flow_module_content method definition

await def update_contact_flow_module_content(
    self,
    *,
    InstanceId: str,
    ContactFlowModuleId: str,
    Content: str,
) -> Dict[str, Any]:
    ...
```



```python
# update_contact_flow_module_content method usage example with argument unpacking

kwargs: UpdateContactFlowModuleContentRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowModuleId": ...,
    "Content": ...,
}

parent.update_contact_flow_module_content(**kwargs)
```

1. See [:material-code-braces: UpdateContactFlowModuleContentRequestRequestTypeDef](./type_defs.md#updatecontactflowmodulecontentrequestrequesttypedef) 

### update\_contact\_flow\_module\_metadata

Updates metadata about specified flow module.

Type annotations and code completion for `#!python session.create_client("connect").update_contact_flow_module_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_flow_module_metadata)

```python
# update_contact_flow_module_metadata method definition

await def update_contact_flow_module_metadata(
    self,
    *,
    InstanceId: str,
    ContactFlowModuleId: str,
    Name: str = ...,
    Description: str = ...,
    State: ContactFlowModuleStateType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype) 


```python
# update_contact_flow_module_metadata method usage example with argument unpacking

kwargs: UpdateContactFlowModuleMetadataRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowModuleId": ...,
}

parent.update_contact_flow_module_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateContactFlowModuleMetadataRequestRequestTypeDef](./type_defs.md#updatecontactflowmodulemetadatarequestrequesttypedef) 

### update\_contact\_flow\_name

The name of the flow.

Type annotations and code completion for `#!python session.create_client("connect").update_contact_flow_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_flow_name)

```python
# update_contact_flow_name method definition

await def update_contact_flow_name(
    self,
    *,
    InstanceId: str,
    ContactFlowId: str,
    Name: str = ...,
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_contact_flow_name method usage example with argument unpacking

kwargs: UpdateContactFlowNameRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowId": ...,
}

parent.update_contact_flow_name(**kwargs)
```

1. See [:material-code-braces: UpdateContactFlowNameRequestRequestTypeDef](./type_defs.md#updatecontactflownamerequestrequesttypedef) 

### update\_contact\_schedule

Updates the scheduled time of a task contact that is already scheduled.

Type annotations and code completion for `#!python session.create_client("connect").update_contact_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_contact_schedule)

```python
# update_contact_schedule method definition

await def update_contact_schedule(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    ScheduledTime: Union[datetime, str],
) -> Dict[str, Any]:
    ...
```



```python
# update_contact_schedule method usage example with argument unpacking

kwargs: UpdateContactScheduleRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "ScheduledTime": ...,
}

parent.update_contact_schedule(**kwargs)
```

1. See [:material-code-braces: UpdateContactScheduleRequestRequestTypeDef](./type_defs.md#updatecontactschedulerequestrequesttypedef) 

### update\_evaluation\_form

Updates details about a specific evaluation form version in the specified Amazon
Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").update_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_evaluation_form)

```python
# update_evaluation_form method definition

await def update_evaluation_form(
    self,
    *,
    InstanceId: str,
    EvaluationFormId: str,
    EvaluationFormVersion: int,
    Title: str,
    Items: Sequence[EvaluationFormItemTypeDef],  # (1)
    CreateNewVersion: bool = ...,
    Description: str = ...,
    ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,  # (2)
    ClientToken: str = ...,
) -> UpdateEvaluationFormResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) 
2. See [:material-code-braces: EvaluationFormScoringStrategyTypeDef](./type_defs.md#evaluationformscoringstrategytypedef) 
3. See [:material-code-braces: UpdateEvaluationFormResponseTypeDef](./type_defs.md#updateevaluationformresponsetypedef) 


```python
# update_evaluation_form method usage example with argument unpacking

kwargs: UpdateEvaluationFormRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EvaluationFormId": ...,
    "EvaluationFormVersion": ...,
    "Title": ...,
    "Items": ...,
}

parent.update_evaluation_form(**kwargs)
```

1. See [:material-code-braces: UpdateEvaluationFormRequestRequestTypeDef](./type_defs.md#updateevaluationformrequestrequesttypedef) 

### update\_hours\_of\_operation

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_hours_of_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_hours_of_operation)

```python
# update_hours_of_operation method definition

await def update_hours_of_operation(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
    Name: str = ...,
    Description: str = ...,
    TimeZone: str = ...,
    Config: Sequence[HoursOfOperationConfigTypeDef] = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HoursOfOperationConfigTypeDef](./type_defs.md#hoursofoperationconfigtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_hours_of_operation method usage example with argument unpacking

kwargs: UpdateHoursOfOperationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
}

parent.update_hours_of_operation(**kwargs)
```

1. See [:material-code-braces: UpdateHoursOfOperationRequestRequestTypeDef](./type_defs.md#updatehoursofoperationrequestrequesttypedef) 

### update\_instance\_attribute

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_instance_attribute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_instance_attribute)

```python
# update_instance_attribute method definition

await def update_instance_attribute(
    self,
    *,
    InstanceId: str,
    AttributeType: InstanceAttributeTypeType,  # (1)
    Value: str,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InstanceAttributeTypeType](./literals.md#instanceattributetypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_instance_attribute method usage example with argument unpacking

kwargs: UpdateInstanceAttributeRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "AttributeType": ...,
    "Value": ...,
}

parent.update_instance_attribute(**kwargs)
```

1. See [:material-code-braces: UpdateInstanceAttributeRequestRequestTypeDef](./type_defs.md#updateinstanceattributerequestrequesttypedef) 

### update\_instance\_storage\_config

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_instance_storage_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_instance_storage_config)

```python
# update_instance_storage_config method definition

await def update_instance_storage_config(
    self,
    *,
    InstanceId: str,
    AssociationId: str,
    ResourceType: InstanceStorageResourceTypeType,  # (1)
    StorageConfig: InstanceStorageConfigTypeDef,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype) 
2. See [:material-code-braces: InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_instance_storage_config method usage example with argument unpacking

kwargs: UpdateInstanceStorageConfigRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "AssociationId": ...,
    "ResourceType": ...,
    "StorageConfig": ...,
}

parent.update_instance_storage_config(**kwargs)
```

1. See [:material-code-braces: UpdateInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#updateinstancestorageconfigrequestrequesttypedef) 

### update\_participant\_role\_config

Updates timeouts for when human chat participants are to be considered idle, and
when agents are automatically disconnected from a chat due to idleness.

Type annotations and code completion for `#!python session.create_client("connect").update_participant_role_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_participant_role_config)

```python
# update_participant_role_config method definition

await def update_participant_role_config(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    ChannelConfiguration: UpdateParticipantRoleConfigChannelInfoTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: UpdateParticipantRoleConfigChannelInfoTypeDef](./type_defs.md#updateparticipantroleconfigchannelinfotypedef) 


```python
# update_participant_role_config method usage example with argument unpacking

kwargs: UpdateParticipantRoleConfigRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "ChannelConfiguration": ...,
}

parent.update_participant_role_config(**kwargs)
```

1. See [:material-code-braces: UpdateParticipantRoleConfigRequestRequestTypeDef](./type_defs.md#updateparticipantroleconfigrequestrequesttypedef) 

### update\_phone\_number

Updates your claimed phone number from its current Amazon Connect instance or
traffic distribution group to another Amazon Connect instance or traffic
distribution group in the same Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("connect").update_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_phone_number)

```python
# update_phone_number method definition

await def update_phone_number(
    self,
    *,
    PhoneNumberId: str,
    TargetArn: str,
    ClientToken: str = ...,
) -> UpdatePhoneNumberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdatePhoneNumberResponseTypeDef](./type_defs.md#updatephonenumberresponsetypedef) 


```python
# update_phone_number method usage example with argument unpacking

kwargs: UpdatePhoneNumberRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
    "TargetArn": ...,
}

parent.update_phone_number(**kwargs)
```

1. See [:material-code-braces: UpdatePhoneNumberRequestRequestTypeDef](./type_defs.md#updatephonenumberrequestrequesttypedef) 

### update\_prompt

Updates a prompt.

Type annotations and code completion for `#!python session.create_client("connect").update_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_prompt)

```python
# update_prompt method definition

await def update_prompt(
    self,
    *,
    InstanceId: str,
    PromptId: str,
    Name: str = ...,
    Description: str = ...,
    S3Uri: str = ...,
) -> UpdatePromptResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdatePromptResponseTypeDef](./type_defs.md#updatepromptresponsetypedef) 


```python
# update_prompt method usage example with argument unpacking

kwargs: UpdatePromptRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "PromptId": ...,
}

parent.update_prompt(**kwargs)
```

1. See [:material-code-braces: UpdatePromptRequestRequestTypeDef](./type_defs.md#updatepromptrequestrequesttypedef) 

### update\_queue\_hours\_of\_operation

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_queue_hours_of_operation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_queue_hours_of_operation)

```python
# update_queue_hours_of_operation method definition

await def update_queue_hours_of_operation(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    HoursOfOperationId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_queue_hours_of_operation method usage example with argument unpacking

kwargs: UpdateQueueHoursOfOperationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
    "HoursOfOperationId": ...,
}

parent.update_queue_hours_of_operation(**kwargs)
```

1. See [:material-code-braces: UpdateQueueHoursOfOperationRequestRequestTypeDef](./type_defs.md#updatequeuehoursofoperationrequestrequesttypedef) 

### update\_queue\_max\_contacts

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_queue_max_contacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_queue_max_contacts)

```python
# update_queue_max_contacts method definition

await def update_queue_max_contacts(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    MaxContacts: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_queue_max_contacts method usage example with argument unpacking

kwargs: UpdateQueueMaxContactsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
}

parent.update_queue_max_contacts(**kwargs)
```

1. See [:material-code-braces: UpdateQueueMaxContactsRequestRequestTypeDef](./type_defs.md#updatequeuemaxcontactsrequestrequesttypedef) 

### update\_queue\_name

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_queue_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_queue_name)

```python
# update_queue_name method definition

await def update_queue_name(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    Name: str = ...,
    Description: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_queue_name method usage example with argument unpacking

kwargs: UpdateQueueNameRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
}

parent.update_queue_name(**kwargs)
```

1. See [:material-code-braces: UpdateQueueNameRequestRequestTypeDef](./type_defs.md#updatequeuenamerequestrequesttypedef) 

### update\_queue\_outbound\_caller\_config

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_queue_outbound_caller_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_queue_outbound_caller_config)

```python
# update_queue_outbound_caller_config method definition

await def update_queue_outbound_caller_config(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    OutboundCallerConfig: OutboundCallerConfigTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_queue_outbound_caller_config method usage example with argument unpacking

kwargs: UpdateQueueOutboundCallerConfigRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
    "OutboundCallerConfig": ...,
}

parent.update_queue_outbound_caller_config(**kwargs)
```

1. See [:material-code-braces: UpdateQueueOutboundCallerConfigRequestRequestTypeDef](./type_defs.md#updatequeueoutboundcallerconfigrequestrequesttypedef) 

### update\_queue\_status

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_queue_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_queue_status)

```python
# update_queue_status method definition

await def update_queue_status(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    Status: QueueStatusType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueueStatusType](./literals.md#queuestatustype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_queue_status method usage example with argument unpacking

kwargs: UpdateQueueStatusRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
    "Status": ...,
}

parent.update_queue_status(**kwargs)
```

1. See [:material-code-braces: UpdateQueueStatusRequestRequestTypeDef](./type_defs.md#updatequeuestatusrequestrequesttypedef) 

### update\_quick\_connect\_config

Updates the configuration settings for the specified quick connect.

Type annotations and code completion for `#!python session.create_client("connect").update_quick_connect_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_quick_connect_config)

```python
# update_quick_connect_config method definition

await def update_quick_connect_config(
    self,
    *,
    InstanceId: str,
    QuickConnectId: str,
    QuickConnectConfig: QuickConnectConfigTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: QuickConnectConfigTypeDef](./type_defs.md#quickconnectconfigtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_quick_connect_config method usage example with argument unpacking

kwargs: UpdateQuickConnectConfigRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QuickConnectId": ...,
    "QuickConnectConfig": ...,
}

parent.update_quick_connect_config(**kwargs)
```

1. See [:material-code-braces: UpdateQuickConnectConfigRequestRequestTypeDef](./type_defs.md#updatequickconnectconfigrequestrequesttypedef) 

### update\_quick\_connect\_name

Updates the name and description of a quick connect.

Type annotations and code completion for `#!python session.create_client("connect").update_quick_connect_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_quick_connect_name)

```python
# update_quick_connect_name method definition

await def update_quick_connect_name(
    self,
    *,
    InstanceId: str,
    QuickConnectId: str,
    Name: str = ...,
    Description: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_quick_connect_name method usage example with argument unpacking

kwargs: UpdateQuickConnectNameRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QuickConnectId": ...,
}

parent.update_quick_connect_name(**kwargs)
```

1. See [:material-code-braces: UpdateQuickConnectNameRequestRequestTypeDef](./type_defs.md#updatequickconnectnamerequestrequesttypedef) 

### update\_routing\_profile\_agent\_availability\_timer

Whether agents with this routing profile will have their routing order
calculated based on *time since their last inbound contact* or *longest idle
time*.

Type annotations and code completion for `#!python session.create_client("connect").update_routing_profile_agent_availability_timer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_agent_availability_timer)

```python
# update_routing_profile_agent_availability_timer method definition

await def update_routing_profile_agent_availability_timer(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    AgentAvailabilityTimer: AgentAvailabilityTimerType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AgentAvailabilityTimerType](./literals.md#agentavailabilitytimertype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_routing_profile_agent_availability_timer method usage example with argument unpacking

kwargs: UpdateRoutingProfileAgentAvailabilityTimerRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
    "AgentAvailabilityTimer": ...,
}

parent.update_routing_profile_agent_availability_timer(**kwargs)
```

1. See [:material-code-braces: UpdateRoutingProfileAgentAvailabilityTimerRequestRequestTypeDef](./type_defs.md#updateroutingprofileagentavailabilitytimerrequestrequesttypedef) 

### update\_routing\_profile\_concurrency

Updates the channels that agents can handle in the Contact Control Panel (CCP)
for a routing profile.

Type annotations and code completion for `#!python session.create_client("connect").update_routing_profile_concurrency` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_concurrency)

```python
# update_routing_profile_concurrency method definition

await def update_routing_profile_concurrency(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    MediaConcurrencies: Sequence[MediaConcurrencyTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MediaConcurrencyTypeDef](./type_defs.md#mediaconcurrencytypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_routing_profile_concurrency method usage example with argument unpacking

kwargs: UpdateRoutingProfileConcurrencyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
    "MediaConcurrencies": ...,
}

parent.update_routing_profile_concurrency(**kwargs)
```

1. See [:material-code-braces: UpdateRoutingProfileConcurrencyRequestRequestTypeDef](./type_defs.md#updateroutingprofileconcurrencyrequestrequesttypedef) 

### update\_routing\_profile\_default\_outbound\_queue

Updates the default outbound queue of a routing profile.

Type annotations and code completion for `#!python session.create_client("connect").update_routing_profile_default_outbound_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_default_outbound_queue)

```python
# update_routing_profile_default_outbound_queue method definition

await def update_routing_profile_default_outbound_queue(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    DefaultOutboundQueueId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_routing_profile_default_outbound_queue method usage example with argument unpacking

kwargs: UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
    "DefaultOutboundQueueId": ...,
}

parent.update_routing_profile_default_outbound_queue(**kwargs)
```

1. See [:material-code-braces: UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef](./type_defs.md#updateroutingprofiledefaultoutboundqueuerequestrequesttypedef) 

### update\_routing\_profile\_name

Updates the name and description of a routing profile.

Type annotations and code completion for `#!python session.create_client("connect").update_routing_profile_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_name)

```python
# update_routing_profile_name method definition

await def update_routing_profile_name(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    Name: str = ...,
    Description: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_routing_profile_name method usage example with argument unpacking

kwargs: UpdateRoutingProfileNameRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
}

parent.update_routing_profile_name(**kwargs)
```

1. See [:material-code-braces: UpdateRoutingProfileNameRequestRequestTypeDef](./type_defs.md#updateroutingprofilenamerequestrequesttypedef) 

### update\_routing\_profile\_queues

Updates the properties associated with a set of queues for a routing profile.

Type annotations and code completion for `#!python session.create_client("connect").update_routing_profile_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_routing_profile_queues)

```python
# update_routing_profile_queues method definition

await def update_routing_profile_queues(
    self,
    *,
    InstanceId: str,
    RoutingProfileId: str,
    QueueConfigs: Sequence[RoutingProfileQueueConfigTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_routing_profile_queues method usage example with argument unpacking

kwargs: UpdateRoutingProfileQueuesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RoutingProfileId": ...,
    "QueueConfigs": ...,
}

parent.update_routing_profile_queues(**kwargs)
```

1. See [:material-code-braces: UpdateRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#updateroutingprofilequeuesrequestrequesttypedef) 

### update\_rule

Updates a rule for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").update_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_rule)

```python
# update_rule method definition

await def update_rule(
    self,
    *,
    RuleId: str,
    InstanceId: str,
    Name: str,
    Function: str,
    Actions: Sequence[RuleActionTypeDef],  # (1)
    PublishStatus: RulePublishStatusType,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-brackets: RulePublishStatusType](./literals.md#rulepublishstatustype) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_rule method usage example with argument unpacking

kwargs: UpdateRuleRequestRequestTypeDef = {  # (1)
    "RuleId": ...,
    "InstanceId": ...,
    "Name": ...,
    "Function": ...,
    "Actions": ...,
    "PublishStatus": ...,
}

parent.update_rule(**kwargs)
```

1. See [:material-code-braces: UpdateRuleRequestRequestTypeDef](./type_defs.md#updaterulerequestrequesttypedef) 

### update\_security\_profile

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_security_profile)

```python
# update_security_profile method definition

await def update_security_profile(
    self,
    *,
    SecurityProfileId: str,
    InstanceId: str,
    Description: str = ...,
    Permissions: Sequence[str] = ...,
    AllowedAccessControlTags: Mapping[str, str] = ...,
    TagRestrictedResources: Sequence[str] = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_security_profile method usage example with argument unpacking

kwargs: UpdateSecurityProfileRequestRequestTypeDef = {  # (1)
    "SecurityProfileId": ...,
    "InstanceId": ...,
}

parent.update_security_profile(**kwargs)
```

1. See [:material-code-braces: UpdateSecurityProfileRequestRequestTypeDef](./type_defs.md#updatesecurityprofilerequestrequesttypedef) 

### update\_task\_template

Updates details about a specific task template in the specified Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").update_task_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_task_template)

```python
# update_task_template method definition

await def update_task_template(
    self,
    *,
    TaskTemplateId: str,
    InstanceId: str,
    Name: str = ...,
    Description: str = ...,
    ContactFlowId: str = ...,
    Constraints: TaskTemplateConstraintsTypeDef = ...,  # (1)
    Defaults: TaskTemplateDefaultsTypeDef = ...,  # (2)
    Status: TaskTemplateStatusType = ...,  # (3)
    Fields: Sequence[TaskTemplateFieldTypeDef] = ...,  # (4)
) -> UpdateTaskTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: TaskTemplateConstraintsTypeDef](./type_defs.md#tasktemplateconstraintstypedef) 
2. See [:material-code-braces: TaskTemplateDefaultsTypeDef](./type_defs.md#tasktemplatedefaultstypedef) 
3. See [:material-code-brackets: TaskTemplateStatusType](./literals.md#tasktemplatestatustype) 
4. See [:material-code-braces: TaskTemplateFieldTypeDef](./type_defs.md#tasktemplatefieldtypedef) 
5. See [:material-code-braces: UpdateTaskTemplateResponseTypeDef](./type_defs.md#updatetasktemplateresponsetypedef) 


```python
# update_task_template method usage example with argument unpacking

kwargs: UpdateTaskTemplateRequestRequestTypeDef = {  # (1)
    "TaskTemplateId": ...,
    "InstanceId": ...,
}

parent.update_task_template(**kwargs)
```

1. See [:material-code-braces: UpdateTaskTemplateRequestRequestTypeDef](./type_defs.md#updatetasktemplaterequestrequesttypedef) 

### update\_traffic\_distribution

Updates the traffic distribution for a given traffic distribution group.

Type annotations and code completion for `#!python session.create_client("connect").update_traffic_distribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_traffic_distribution)

```python
# update_traffic_distribution method definition

await def update_traffic_distribution(
    self,
    *,
    Id: str,
    TelephonyConfig: TelephonyConfigTypeDef = ...,  # (1)
    SignInConfig: SignInConfigTypeDef = ...,  # (2)
    AgentConfig: AgentConfigTypeDef = ...,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TelephonyConfigTypeDef](./type_defs.md#telephonyconfigtypedef) 
2. See [:material-code-braces: SignInConfigTypeDef](./type_defs.md#signinconfigtypedef) 
3. See [:material-code-braces: AgentConfigTypeDef](./type_defs.md#agentconfigtypedef) 


```python
# update_traffic_distribution method usage example with argument unpacking

kwargs: UpdateTrafficDistributionRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.update_traffic_distribution(**kwargs)
```

1. See [:material-code-braces: UpdateTrafficDistributionRequestRequestTypeDef](./type_defs.md#updatetrafficdistributionrequestrequesttypedef) 

### update\_user\_hierarchy

Assigns the specified hierarchy group to the specified user.

Type annotations and code completion for `#!python session.create_client("connect").update_user_hierarchy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_user_hierarchy)

```python
# update_user_hierarchy method definition

await def update_user_hierarchy(
    self,
    *,
    UserId: str,
    InstanceId: str,
    HierarchyGroupId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user_hierarchy method usage example with argument unpacking

kwargs: UpdateUserHierarchyRequestRequestTypeDef = {  # (1)
    "UserId": ...,
    "InstanceId": ...,
}

parent.update_user_hierarchy(**kwargs)
```

1. See [:material-code-braces: UpdateUserHierarchyRequestRequestTypeDef](./type_defs.md#updateuserhierarchyrequestrequesttypedef) 

### update\_user\_hierarchy\_group\_name

Updates the name of the user hierarchy group.

Type annotations and code completion for `#!python session.create_client("connect").update_user_hierarchy_group_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_user_hierarchy_group_name)

```python
# update_user_hierarchy_group_name method definition

await def update_user_hierarchy_group_name(
    self,
    *,
    Name: str,
    HierarchyGroupId: str,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user_hierarchy_group_name method usage example with argument unpacking

kwargs: UpdateUserHierarchyGroupNameRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "HierarchyGroupId": ...,
    "InstanceId": ...,
}

parent.update_user_hierarchy_group_name(**kwargs)
```

1. See [:material-code-braces: UpdateUserHierarchyGroupNameRequestRequestTypeDef](./type_defs.md#updateuserhierarchygroupnamerequestrequesttypedef) 

### update\_user\_hierarchy\_structure

Updates the user hierarchy structure: add, remove, and rename user hierarchy
levels.

Type annotations and code completion for `#!python session.create_client("connect").update_user_hierarchy_structure` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_user_hierarchy_structure)

```python
# update_user_hierarchy_structure method definition

await def update_user_hierarchy_structure(
    self,
    *,
    HierarchyStructure: HierarchyStructureUpdateTypeDef,  # (1)
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HierarchyStructureUpdateTypeDef](./type_defs.md#hierarchystructureupdatetypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user_hierarchy_structure method usage example with argument unpacking

kwargs: UpdateUserHierarchyStructureRequestRequestTypeDef = {  # (1)
    "HierarchyStructure": ...,
    "InstanceId": ...,
}

parent.update_user_hierarchy_structure(**kwargs)
```

1. See [:material-code-braces: UpdateUserHierarchyStructureRequestRequestTypeDef](./type_defs.md#updateuserhierarchystructurerequestrequesttypedef) 

### update\_user\_identity\_info

Updates the identity information for the specified user.

Type annotations and code completion for `#!python session.create_client("connect").update_user_identity_info` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_user_identity_info)

```python
# update_user_identity_info method definition

await def update_user_identity_info(
    self,
    *,
    IdentityInfo: UserIdentityInfoTypeDef,  # (1)
    UserId: str,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UserIdentityInfoTypeDef](./type_defs.md#useridentityinfotypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user_identity_info method usage example with argument unpacking

kwargs: UpdateUserIdentityInfoRequestRequestTypeDef = {  # (1)
    "IdentityInfo": ...,
    "UserId": ...,
    "InstanceId": ...,
}

parent.update_user_identity_info(**kwargs)
```

1. See [:material-code-braces: UpdateUserIdentityInfoRequestRequestTypeDef](./type_defs.md#updateuseridentityinforequestrequesttypedef) 

### update\_user\_phone\_config

Updates the phone configuration settings for the specified user.

Type annotations and code completion for `#!python session.create_client("connect").update_user_phone_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_user_phone_config)

```python
# update_user_phone_config method definition

await def update_user_phone_config(
    self,
    *,
    PhoneConfig: UserPhoneConfigTypeDef,  # (1)
    UserId: str,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user_phone_config method usage example with argument unpacking

kwargs: UpdateUserPhoneConfigRequestRequestTypeDef = {  # (1)
    "PhoneConfig": ...,
    "UserId": ...,
    "InstanceId": ...,
}

parent.update_user_phone_config(**kwargs)
```

1. See [:material-code-braces: UpdateUserPhoneConfigRequestRequestTypeDef](./type_defs.md#updateuserphoneconfigrequestrequesttypedef) 

### update\_user\_routing\_profile

Assigns the specified routing profile to the specified user.

Type annotations and code completion for `#!python session.create_client("connect").update_user_routing_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_user_routing_profile)

```python
# update_user_routing_profile method definition

await def update_user_routing_profile(
    self,
    *,
    RoutingProfileId: str,
    UserId: str,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user_routing_profile method usage example with argument unpacking

kwargs: UpdateUserRoutingProfileRequestRequestTypeDef = {  # (1)
    "RoutingProfileId": ...,
    "UserId": ...,
    "InstanceId": ...,
}

parent.update_user_routing_profile(**kwargs)
```

1. See [:material-code-braces: UpdateUserRoutingProfileRequestRequestTypeDef](./type_defs.md#updateuserroutingprofilerequestrequesttypedef) 

### update\_user\_security\_profiles

Assigns the specified security profiles to the specified user.

Type annotations and code completion for `#!python session.create_client("connect").update_user_security_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.update_user_security_profiles)

```python
# update_user_security_profiles method definition

await def update_user_security_profiles(
    self,
    *,
    SecurityProfileIds: Sequence[str],
    UserId: str,
    InstanceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user_security_profiles method usage example with argument unpacking

kwargs: UpdateUserSecurityProfilesRequestRequestTypeDef = {  # (1)
    "SecurityProfileIds": ...,
    "UserId": ...,
    "InstanceId": ...,
}

parent.update_user_security_profiles(**kwargs)
```

1. See [:material-code-braces: UpdateUserSecurityProfilesRequestRequestTypeDef](./type_defs.md#updateusersecurityprofilesrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("connect").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> ConnectClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("connect").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("connect").get_paginator` method with overloads.

- `client.get_paginator("get_metric_data")` -> [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
- `client.get_paginator("list_agent_statuses")` -> [ListAgentStatusesPaginator](./paginators.md#listagentstatusespaginator)
- `client.get_paginator("list_approved_origins")` -> [ListApprovedOriginsPaginator](./paginators.md#listapprovedoriginspaginator)
- `client.get_paginator("list_bots")` -> [ListBotsPaginator](./paginators.md#listbotspaginator)
- `client.get_paginator("list_contact_evaluations")` -> [ListContactEvaluationsPaginator](./paginators.md#listcontactevaluationspaginator)
- `client.get_paginator("list_contact_flow_modules")` -> [ListContactFlowModulesPaginator](./paginators.md#listcontactflowmodulespaginator)
- `client.get_paginator("list_contact_flows")` -> [ListContactFlowsPaginator](./paginators.md#listcontactflowspaginator)
- `client.get_paginator("list_contact_references")` -> [ListContactReferencesPaginator](./paginators.md#listcontactreferencespaginator)
- `client.get_paginator("list_default_vocabularies")` -> [ListDefaultVocabulariesPaginator](./paginators.md#listdefaultvocabulariespaginator)
- `client.get_paginator("list_evaluation_form_versions")` -> [ListEvaluationFormVersionsPaginator](./paginators.md#listevaluationformversionspaginator)
- `client.get_paginator("list_evaluation_forms")` -> [ListEvaluationFormsPaginator](./paginators.md#listevaluationformspaginator)
- `client.get_paginator("list_hours_of_operations")` -> [ListHoursOfOperationsPaginator](./paginators.md#listhoursofoperationspaginator)
- `client.get_paginator("list_instance_attributes")` -> [ListInstanceAttributesPaginator](./paginators.md#listinstanceattributespaginator)
- `client.get_paginator("list_instance_storage_configs")` -> [ListInstanceStorageConfigsPaginator](./paginators.md#listinstancestorageconfigspaginator)
- `client.get_paginator("list_instances")` -> [ListInstancesPaginator](./paginators.md#listinstancespaginator)
- `client.get_paginator("list_integration_associations")` -> [ListIntegrationAssociationsPaginator](./paginators.md#listintegrationassociationspaginator)
- `client.get_paginator("list_lambda_functions")` -> [ListLambdaFunctionsPaginator](./paginators.md#listlambdafunctionspaginator)
- `client.get_paginator("list_lex_bots")` -> [ListLexBotsPaginator](./paginators.md#listlexbotspaginator)
- `client.get_paginator("list_phone_numbers")` -> [ListPhoneNumbersPaginator](./paginators.md#listphonenumberspaginator)
- `client.get_paginator("list_phone_numbers_v2")` -> [ListPhoneNumbersV2Paginator](./paginators.md#listphonenumbersv2paginator)
- `client.get_paginator("list_prompts")` -> [ListPromptsPaginator](./paginators.md#listpromptspaginator)
- `client.get_paginator("list_queue_quick_connects")` -> [ListQueueQuickConnectsPaginator](./paginators.md#listqueuequickconnectspaginator)
- `client.get_paginator("list_queues")` -> [ListQueuesPaginator](./paginators.md#listqueuespaginator)
- `client.get_paginator("list_quick_connects")` -> [ListQuickConnectsPaginator](./paginators.md#listquickconnectspaginator)
- `client.get_paginator("list_routing_profile_queues")` -> [ListRoutingProfileQueuesPaginator](./paginators.md#listroutingprofilequeuespaginator)
- `client.get_paginator("list_routing_profiles")` -> [ListRoutingProfilesPaginator](./paginators.md#listroutingprofilespaginator)
- `client.get_paginator("list_rules")` -> [ListRulesPaginator](./paginators.md#listrulespaginator)
- `client.get_paginator("list_security_keys")` -> [ListSecurityKeysPaginator](./paginators.md#listsecuritykeyspaginator)
- `client.get_paginator("list_security_profile_permissions")` -> [ListSecurityProfilePermissionsPaginator](./paginators.md#listsecurityprofilepermissionspaginator)
- `client.get_paginator("list_security_profiles")` -> [ListSecurityProfilesPaginator](./paginators.md#listsecurityprofilespaginator)
- `client.get_paginator("list_task_templates")` -> [ListTaskTemplatesPaginator](./paginators.md#listtasktemplatespaginator)
- `client.get_paginator("list_traffic_distribution_group_users")` -> [ListTrafficDistributionGroupUsersPaginator](./paginators.md#listtrafficdistributiongroupuserspaginator)
- `client.get_paginator("list_traffic_distribution_groups")` -> [ListTrafficDistributionGroupsPaginator](./paginators.md#listtrafficdistributiongroupspaginator)
- `client.get_paginator("list_use_cases")` -> [ListUseCasesPaginator](./paginators.md#listusecasespaginator)
- `client.get_paginator("list_user_hierarchy_groups")` -> [ListUserHierarchyGroupsPaginator](./paginators.md#listuserhierarchygroupspaginator)
- `client.get_paginator("list_users")` -> [ListUsersPaginator](./paginators.md#listuserspaginator)
- `client.get_paginator("search_available_phone_numbers")` -> [SearchAvailablePhoneNumbersPaginator](./paginators.md#searchavailablephonenumberspaginator)
- `client.get_paginator("search_hours_of_operations")` -> [SearchHoursOfOperationsPaginator](./paginators.md#searchhoursofoperationspaginator)
- `client.get_paginator("search_prompts")` -> [SearchPromptsPaginator](./paginators.md#searchpromptspaginator)
- `client.get_paginator("search_queues")` -> [SearchQueuesPaginator](./paginators.md#searchqueuespaginator)
- `client.get_paginator("search_quick_connects")` -> [SearchQuickConnectsPaginator](./paginators.md#searchquickconnectspaginator)
- `client.get_paginator("search_resource_tags")` -> [SearchResourceTagsPaginator](./paginators.md#searchresourcetagspaginator)
- `client.get_paginator("search_routing_profiles")` -> [SearchRoutingProfilesPaginator](./paginators.md#searchroutingprofilespaginator)
- `client.get_paginator("search_security_profiles")` -> [SearchSecurityProfilesPaginator](./paginators.md#searchsecurityprofilespaginator)
- `client.get_paginator("search_users")` -> [SearchUsersPaginator](./paginators.md#searchuserspaginator)
- `client.get_paginator("search_vocabularies")` -> [SearchVocabulariesPaginator](./paginators.md#searchvocabulariespaginator)



