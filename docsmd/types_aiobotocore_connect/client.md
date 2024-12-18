# ConnectClient

> [Index](../README.md) > [Connect](./README.md) > ConnectClient

!!! note ""

    Auto-generated documentation for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#connect)
    type annotations stubs module [types-aiobotocore-connect](https://pypi.org/project/types-aiobotocore-connect/).

## ConnectClient

Type annotations and code completion for `#!python session.create_client("connect")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client)

```python
# ConnectClient usage example

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
# ConnectClient.exceptions usage example

async with session.create_client("connect") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConditionalOperationFailedException,
        client.ConflictException,
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
        client.OutputTypeNotFoundException,
        client.PropertyValidationException,
        client.ResourceConflictException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.ResourceNotReadyException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.TooManyRequestsException,
        client.UserNotFoundException,
    ) as e:
        print(e)
```

```python
# ConnectClient usage type checking example

from types_aiobotocore_connect.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("connect").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("connect").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("connect").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### activate\_evaluation\_form

Activates an evaluation form in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").activate_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/activate_evaluation_form.html)

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

### associate\_analytics\_data\_set

Associates the specified dataset for a Amazon Connect instance with the target
account.

Type annotations and code completion for `#!python session.create_client("connect").associate_analytics_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_analytics_data_set.html)

```python
# associate_analytics_data_set method definition

await def associate_analytics_data_set(
    self,
    *,
    InstanceId: str,
    DataSetId: str,
    TargetAccountId: str = ...,
) -> AssociateAnalyticsDataSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateAnalyticsDataSetResponseTypeDef](./type_defs.md#associateanalyticsdatasetresponsetypedef) 


```python
# associate_analytics_data_set method usage example with argument unpacking

kwargs: AssociateAnalyticsDataSetRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "DataSetId": ...,
}

parent.associate_analytics_data_set(**kwargs)
```

1. See [:material-code-braces: AssociateAnalyticsDataSetRequestRequestTypeDef](./type_defs.md#associateanalyticsdatasetrequestrequesttypedef) 

### associate\_approved\_origin

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").associate_approved_origin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_approved_origin.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_bot.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_default_vocabulary.html)

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

### associate\_flow

Associates a connect resource to a flow.

Type annotations and code completion for `#!python session.create_client("connect").associate_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_flow.html)

```python
# associate_flow method definition

await def associate_flow(
    self,
    *,
    InstanceId: str,
    ResourceId: str,
    FlowId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 


```python
# associate_flow method usage example with argument unpacking

kwargs: AssociateFlowRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ResourceId": ...,
    "FlowId": ...,
    "ResourceType": ...,
}

parent.associate_flow(**kwargs)
```

1. See [:material-code-braces: AssociateFlowRequestRequestTypeDef](./type_defs.md#associateflowrequestrequesttypedef) 

### associate\_instance\_storage\_config

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").associate_instance_storage_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_instance_storage_config.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_lambda_function.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_lex_bot.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_phone_number_contact_flow.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_queue_quick_connects.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_routing_profile_queues.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_security_key.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_traffic_distribution_group_user.html)

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

### associate\_user\_proficiencies

&gt;Associates a set of proficiencies with a user.

Type annotations and code completion for `#!python session.create_client("connect").associate_user_proficiencies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/associate_user_proficiencies.html)

```python
# associate_user_proficiencies method definition

await def associate_user_proficiencies(
    self,
    *,
    InstanceId: str,
    UserId: str,
    UserProficiencies: Sequence[UserProficiencyTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UserProficiencyTypeDef](./type_defs.md#userproficiencytypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_user_proficiencies method usage example with argument unpacking

kwargs: AssociateUserProficienciesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "UserId": ...,
    "UserProficiencies": ...,
}

parent.associate_user_proficiencies(**kwargs)
```

1. See [:material-code-braces: AssociateUserProficienciesRequestRequestTypeDef](./type_defs.md#associateuserproficienciesrequestrequesttypedef) 

### batch\_associate\_analytics\_data\_set

Associates a list of analytics datasets for a given Amazon Connect instance to
a target account.

Type annotations and code completion for `#!python session.create_client("connect").batch_associate_analytics_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/batch_associate_analytics_data_set.html)

```python
# batch_associate_analytics_data_set method definition

await def batch_associate_analytics_data_set(
    self,
    *,
    InstanceId: str,
    DataSetIds: Sequence[str],
    TargetAccountId: str = ...,
) -> BatchAssociateAnalyticsDataSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchAssociateAnalyticsDataSetResponseTypeDef](./type_defs.md#batchassociateanalyticsdatasetresponsetypedef) 


```python
# batch_associate_analytics_data_set method usage example with argument unpacking

kwargs: BatchAssociateAnalyticsDataSetRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "DataSetIds": ...,
}

parent.batch_associate_analytics_data_set(**kwargs)
```

1. See [:material-code-braces: BatchAssociateAnalyticsDataSetRequestRequestTypeDef](./type_defs.md#batchassociateanalyticsdatasetrequestrequesttypedef) 

### batch\_disassociate\_analytics\_data\_set

Removes a list of analytics datasets associated with a given Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").batch_disassociate_analytics_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/batch_disassociate_analytics_data_set.html)

```python
# batch_disassociate_analytics_data_set method definition

await def batch_disassociate_analytics_data_set(
    self,
    *,
    InstanceId: str,
    DataSetIds: Sequence[str],
    TargetAccountId: str = ...,
) -> BatchDisassociateAnalyticsDataSetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDisassociateAnalyticsDataSetResponseTypeDef](./type_defs.md#batchdisassociateanalyticsdatasetresponsetypedef) 


```python
# batch_disassociate_analytics_data_set method usage example with argument unpacking

kwargs: BatchDisassociateAnalyticsDataSetRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "DataSetIds": ...,
}

parent.batch_disassociate_analytics_data_set(**kwargs)
```

1. See [:material-code-braces: BatchDisassociateAnalyticsDataSetRequestRequestTypeDef](./type_defs.md#batchdisassociateanalyticsdatasetrequestrequesttypedef) 

### batch\_get\_attached\_file\_metadata

Allows you to retrieve metadata about multiple attached files on an associated
resource.

Type annotations and code completion for `#!python session.create_client("connect").batch_get_attached_file_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/batch_get_attached_file_metadata.html)

```python
# batch_get_attached_file_metadata method definition

await def batch_get_attached_file_metadata(
    self,
    *,
    FileIds: Sequence[str],
    InstanceId: str,
    AssociatedResourceArn: str,
) -> BatchGetAttachedFileMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetAttachedFileMetadataResponseTypeDef](./type_defs.md#batchgetattachedfilemetadataresponsetypedef) 


```python
# batch_get_attached_file_metadata method usage example with argument unpacking

kwargs: BatchGetAttachedFileMetadataRequestRequestTypeDef = {  # (1)
    "FileIds": ...,
    "InstanceId": ...,
    "AssociatedResourceArn": ...,
}

parent.batch_get_attached_file_metadata(**kwargs)
```

1. See [:material-code-braces: BatchGetAttachedFileMetadataRequestRequestTypeDef](./type_defs.md#batchgetattachedfilemetadatarequestrequesttypedef) 

### batch\_get\_flow\_association

Retrieve the flow associations for the given resources.

Type annotations and code completion for `#!python session.create_client("connect").batch_get_flow_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/batch_get_flow_association.html)

```python
# batch_get_flow_association method definition

await def batch_get_flow_association(
    self,
    *,
    InstanceId: str,
    ResourceIds: Sequence[str],
    ResourceType: ListFlowAssociationResourceTypeType = ...,  # (1)
) -> BatchGetFlowAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype) 
2. See [:material-code-braces: BatchGetFlowAssociationResponseTypeDef](./type_defs.md#batchgetflowassociationresponsetypedef) 


```python
# batch_get_flow_association method usage example with argument unpacking

kwargs: BatchGetFlowAssociationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ResourceIds": ...,
}

parent.batch_get_flow_association(**kwargs)
```

1. See [:material-code-braces: BatchGetFlowAssociationRequestRequestTypeDef](./type_defs.md#batchgetflowassociationrequestrequesttypedef) 

### batch\_put\_contact

Only the Amazon Connect outbound campaigns service principal is allowed to
assume a role in your account and call this API.

Type annotations and code completion for `#!python session.create_client("connect").batch_put_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/batch_put_contact.html)

```python
# batch_put_contact method definition

await def batch_put_contact(
    self,
    *,
    InstanceId: str,
    ContactDataRequestList: Sequence[ContactDataRequestTypeDef],  # (1)
    ClientToken: str = ...,
) -> BatchPutContactResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ContactDataRequestTypeDef](./type_defs.md#contactdatarequesttypedef) 
2. See [:material-code-braces: BatchPutContactResponseTypeDef](./type_defs.md#batchputcontactresponsetypedef) 


```python
# batch_put_contact method usage example with argument unpacking

kwargs: BatchPutContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactDataRequestList": ...,
}

parent.batch_put_contact(**kwargs)
```

1. See [:material-code-braces: BatchPutContactRequestRequestTypeDef](./type_defs.md#batchputcontactrequestrequesttypedef) 

### claim\_phone\_number

Claims an available phone number to your Amazon Connect instance or traffic
distribution group.

Type annotations and code completion for `#!python session.create_client("connect").claim_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/claim_phone_number.html)

```python
# claim_phone_number method definition

await def claim_phone_number(
    self,
    *,
    PhoneNumber: str,
    TargetArn: str = ...,
    InstanceId: str = ...,
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
    "PhoneNumber": ...,
}

parent.claim_phone_number(**kwargs)
```

1. See [:material-code-braces: ClaimPhoneNumberRequestRequestTypeDef](./type_defs.md#claimphonenumberrequestrequesttypedef) 

### complete\_attached\_file\_upload

Allows you to confirm that the attached file has been uploaded using the
pre-signed URL provided in the StartAttachedFileUpload API.

Type annotations and code completion for `#!python session.create_client("connect").complete_attached_file_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/complete_attached_file_upload.html)

```python
# complete_attached_file_upload method definition

await def complete_attached_file_upload(
    self,
    *,
    InstanceId: str,
    FileId: str,
    AssociatedResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# complete_attached_file_upload method usage example with argument unpacking

kwargs: CompleteAttachedFileUploadRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "FileId": ...,
    "AssociatedResourceArn": ...,
}

parent.complete_attached_file_upload(**kwargs)
```

1. See [:material-code-braces: CompleteAttachedFileUploadRequestRequestTypeDef](./type_defs.md#completeattachedfileuploadrequestrequesttypedef) 

### create\_agent\_status

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").create_agent_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_agent_status.html)

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

### create\_contact

Creates a new contact.

Type annotations and code completion for `#!python session.create_client("connect").create_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_contact.html)

```python
# create_contact method definition

await def create_contact(
    self,
    *,
    InstanceId: str,
    Channel: ChannelType,  # (1)
    InitiationMethod: ContactInitiationMethodType,  # (2)
    ClientToken: str = ...,
    RelatedContactId: str = ...,
    Attributes: Mapping[str, str] = ...,
    References: Mapping[str, ReferenceTypeDef] = ...,  # (3)
    ExpiryDurationInMinutes: int = ...,
    UserInfo: UserInfoTypeDef = ...,  # (4)
    InitiateAs: InitiateAsType = ...,  # (5)
    Name: str = ...,
    Description: str = ...,
    SegmentAttributes: Mapping[str, SegmentAttributeValueUnionTypeDef] = ...,  # (6)
) -> CreateContactResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: ChannelType](./literals.md#channeltype) 
2. See [:material-code-brackets: ContactInitiationMethodType](./literals.md#contactinitiationmethodtype) 
3. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
4. See [:material-code-braces: UserInfoTypeDef](./type_defs.md#userinfotypedef) 
5. See [:material-code-brackets: InitiateAsType](./literals.md#initiateastype) 
6. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) [:material-code-braces: SegmentAttributeValueOutputTypeDef](./type_defs.md#segmentattributevalueoutputtypedef) 
7. See [:material-code-braces: CreateContactResponseTypeDef](./type_defs.md#createcontactresponsetypedef) 


```python
# create_contact method usage example with argument unpacking

kwargs: CreateContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Channel": ...,
    "InitiationMethod": ...,
}

parent.create_contact(**kwargs)
```

1. See [:material-code-braces: CreateContactRequestRequestTypeDef](./type_defs.md#createcontactrequestrequesttypedef) 

### create\_contact\_flow

Creates a flow for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_contact_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_contact_flow.html)

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
    Status: ContactFlowStatusType = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> CreateContactFlowResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ContactFlowTypeType](./literals.md#contactflowtypetype) 
2. See [:material-code-brackets: ContactFlowStatusType](./literals.md#contactflowstatustype) 
3. See [:material-code-braces: CreateContactFlowResponseTypeDef](./type_defs.md#createcontactflowresponsetypedef) 


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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_contact_flow_module.html)

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

### create\_contact\_flow\_version

Publishes a new version of the flow provided.

Type annotations and code completion for `#!python session.create_client("connect").create_contact_flow_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_contact_flow_version.html)

```python
# create_contact_flow_version method definition

await def create_contact_flow_version(
    self,
    *,
    InstanceId: str,
    ContactFlowId: str,
    Description: str = ...,
    FlowContentSha256: str = ...,
    LastModifiedTime: TimestampTypeDef = ...,
    LastModifiedRegion: str = ...,
) -> CreateContactFlowVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateContactFlowVersionResponseTypeDef](./type_defs.md#createcontactflowversionresponsetypedef) 


```python
# create_contact_flow_version method usage example with argument unpacking

kwargs: CreateContactFlowVersionRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowId": ...,
}

parent.create_contact_flow_version(**kwargs)
```

1. See [:material-code-braces: CreateContactFlowVersionRequestRequestTypeDef](./type_defs.md#createcontactflowversionrequestrequesttypedef) 

### create\_email\_address

Create new email address in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_email_address` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_email_address.html)

```python
# create_email_address method definition

await def create_email_address(
    self,
    *,
    InstanceId: str,
    EmailAddress: str,
    Description: str = ...,
    DisplayName: str = ...,
    Tags: Mapping[str, str] = ...,
    ClientToken: str = ...,
) -> CreateEmailAddressResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateEmailAddressResponseTypeDef](./type_defs.md#createemailaddressresponsetypedef) 


```python
# create_email_address method usage example with argument unpacking

kwargs: CreateEmailAddressRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EmailAddress": ...,
}

parent.create_email_address(**kwargs)
```

1. See [:material-code-braces: CreateEmailAddressRequestRequestTypeDef](./type_defs.md#createemailaddressrequestrequesttypedef) 

### create\_evaluation\_form

Creates an evaluation form in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_evaluation_form.html)

```python
# create_evaluation_form method definition

await def create_evaluation_form(
    self,
    *,
    InstanceId: str,
    Title: str,
    Items: Sequence[EvaluationFormItemUnionTypeDef],  # (1)
    Description: str = ...,
    ScoringStrategy: EvaluationFormScoringStrategyTypeDef = ...,  # (2)
    ClientToken: str = ...,
) -> CreateEvaluationFormResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EvaluationFormItemTypeDef](./type_defs.md#evaluationformitemtypedef) [:material-code-braces: EvaluationFormItemOutputTypeDef](./type_defs.md#evaluationformitemoutputtypedef) 
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_hours_of_operation.html)

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

### create\_hours\_of\_operation\_override

Creates an hours of operation override in an Amazon Connect hours of operation
resource.

Type annotations and code completion for `#!python session.create_client("connect").create_hours_of_operation_override` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_hours_of_operation_override.html)

```python
# create_hours_of_operation_override method definition

await def create_hours_of_operation_override(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
    Name: str,
    Config: Sequence[HoursOfOperationOverrideConfigTypeDef],  # (1)
    EffectiveFrom: str,
    EffectiveTill: str,
    Description: str = ...,
) -> CreateHoursOfOperationOverrideResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HoursOfOperationOverrideConfigTypeDef](./type_defs.md#hoursofoperationoverrideconfigtypedef) 
2. See [:material-code-braces: CreateHoursOfOperationOverrideResponseTypeDef](./type_defs.md#createhoursofoperationoverrideresponsetypedef) 


```python
# create_hours_of_operation_override method usage example with argument unpacking

kwargs: CreateHoursOfOperationOverrideRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
    "Name": ...,
    "Config": ...,
    "EffectiveFrom": ...,
    "EffectiveTill": ...,
}

parent.create_hours_of_operation_override(**kwargs)
```

1. See [:material-code-braces: CreateHoursOfOperationOverrideRequestRequestTypeDef](./type_defs.md#createhoursofoperationoverriderequestrequesttypedef) 

### create\_instance

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").create_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_instance.html)

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
    Tags: Mapping[str, str] = ...,
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_integration_association.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_participant.html)

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

### create\_persistent\_contact\_association

Enables rehydration of chats for the lifespan of a contact.

Type annotations and code completion for `#!python session.create_client("connect").create_persistent_contact_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_persistent_contact_association.html)

```python
# create_persistent_contact_association method definition

await def create_persistent_contact_association(
    self,
    *,
    InstanceId: str,
    InitialContactId: str,
    RehydrationType: RehydrationTypeType,  # (1)
    SourceContactId: str,
    ClientToken: str = ...,
) -> CreatePersistentContactAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RehydrationTypeType](./literals.md#rehydrationtypetype) 
2. See [:material-code-braces: CreatePersistentContactAssociationResponseTypeDef](./type_defs.md#createpersistentcontactassociationresponsetypedef) 


```python
# create_persistent_contact_association method usage example with argument unpacking

kwargs: CreatePersistentContactAssociationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "InitialContactId": ...,
    "RehydrationType": ...,
    "SourceContactId": ...,
}

parent.create_persistent_contact_association(**kwargs)
```

1. See [:material-code-braces: CreatePersistentContactAssociationRequestRequestTypeDef](./type_defs.md#createpersistentcontactassociationrequestrequesttypedef) 

### create\_predefined\_attribute

Creates a new predefined attribute for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_predefined_attribute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_predefined_attribute.html)

```python
# create_predefined_attribute method definition

await def create_predefined_attribute(
    self,
    *,
    InstanceId: str,
    Name: str,
    Values: PredefinedAttributeValuesTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PredefinedAttributeValuesTypeDef](./type_defs.md#predefinedattributevaluestypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_predefined_attribute method usage example with argument unpacking

kwargs: CreatePredefinedAttributeRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
    "Values": ...,
}

parent.create_predefined_attribute(**kwargs)
```

1. See [:material-code-braces: CreatePredefinedAttributeRequestRequestTypeDef](./type_defs.md#createpredefinedattributerequestrequesttypedef) 

### create\_prompt

Creates a prompt.

Type annotations and code completion for `#!python session.create_client("connect").create_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_prompt.html)

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

### create\_push\_notification\_registration

Creates registration for a device token and a chat contact to receive real-time
push notifications.

Type annotations and code completion for `#!python session.create_client("connect").create_push_notification_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_push_notification_registration.html)

```python
# create_push_notification_registration method definition

await def create_push_notification_registration(
    self,
    *,
    InstanceId: str,
    PinpointAppArn: str,
    DeviceToken: str,
    DeviceType: DeviceTypeType,  # (1)
    ContactConfiguration: ContactConfigurationTypeDef,  # (2)
    ClientToken: str = ...,
) -> CreatePushNotificationRegistrationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DeviceTypeType](./literals.md#devicetypetype) 
2. See [:material-code-braces: ContactConfigurationTypeDef](./type_defs.md#contactconfigurationtypedef) 
3. See [:material-code-braces: CreatePushNotificationRegistrationResponseTypeDef](./type_defs.md#createpushnotificationregistrationresponsetypedef) 


```python
# create_push_notification_registration method usage example with argument unpacking

kwargs: CreatePushNotificationRegistrationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "PinpointAppArn": ...,
    "DeviceToken": ...,
    "DeviceType": ...,
    "ContactConfiguration": ...,
}

parent.create_push_notification_registration(**kwargs)
```

1. See [:material-code-braces: CreatePushNotificationRegistrationRequestRequestTypeDef](./type_defs.md#createpushnotificationregistrationrequestrequesttypedef) 

### create\_queue

Creates a new queue for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_queue.html)

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
    OutboundEmailConfig: OutboundEmailConfigTypeDef = ...,  # (2)
    MaxContacts: int = ...,
    QuickConnectIds: Sequence[str] = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateQueueResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef) 
2. See [:material-code-braces: OutboundEmailConfigTypeDef](./type_defs.md#outboundemailconfigtypedef) 
3. See [:material-code-braces: CreateQueueResponseTypeDef](./type_defs.md#createqueueresponsetypedef) 


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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_quick_connect.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_routing_profile.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_rule.html)

```python
# create_rule method definition

await def create_rule(
    self,
    *,
    InstanceId: str,
    Name: str,
    TriggerEventSource: RuleTriggerEventSourceTypeDef,  # (1)
    Function: str,
    Actions: Sequence[RuleActionUnionTypeDef],  # (2)
    PublishStatus: RulePublishStatusType,  # (3)
    ClientToken: str = ...,
) -> CreateRuleResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RuleTriggerEventSourceTypeDef](./type_defs.md#ruletriggereventsourcetypedef) 
2. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) [:material-code-braces: RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef) 
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

Creates a security profile.

Type annotations and code completion for `#!python session.create_client("connect").create_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_security_profile.html)

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
    Applications: Sequence[ApplicationUnionTypeDef] = ...,  # (1)
    HierarchyRestrictedResources: Sequence[str] = ...,
    AllowedAccessControlHierarchyGroupId: str = ...,
) -> CreateSecurityProfileResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 
2. See [:material-code-braces: CreateSecurityProfileResponseTypeDef](./type_defs.md#createsecurityprofileresponsetypedef) 


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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_task_template.html)

```python
# create_task_template method definition

await def create_task_template(
    self,
    *,
    InstanceId: str,
    Name: str,
    Fields: Sequence[TaskTemplateFieldUnionTypeDef],  # (1)
    Description: str = ...,
    ContactFlowId: str = ...,
    SelfAssignFlowId: str = ...,
    Constraints: TaskTemplateConstraintsTypeDef = ...,  # (2)
    Defaults: TaskTemplateDefaultsTypeDef = ...,  # (3)
    Status: TaskTemplateStatusType = ...,  # (4)
    ClientToken: str = ...,
) -> CreateTaskTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: TaskTemplateFieldTypeDef](./type_defs.md#tasktemplatefieldtypedef) [:material-code-braces: TaskTemplateFieldOutputTypeDef](./type_defs.md#tasktemplatefieldoutputtypedef) 
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_traffic_distribution_group.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_use_case.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_user.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_user_hierarchy_group.html)

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

### create\_view

Creates a new view with the possible status of <code>SAVED</code> or
<code>PUBLISHED</code>.

Type annotations and code completion for `#!python session.create_client("connect").create_view` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_view.html)

```python
# create_view method definition

await def create_view(
    self,
    *,
    InstanceId: str,
    Status: ViewStatusType,  # (1)
    Content: ViewInputContentTypeDef,  # (2)
    Name: str,
    ClientToken: str = ...,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateViewResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ViewStatusType](./literals.md#viewstatustype) 
2. See [:material-code-braces: ViewInputContentTypeDef](./type_defs.md#viewinputcontenttypedef) 
3. See [:material-code-braces: CreateViewResponseTypeDef](./type_defs.md#createviewresponsetypedef) 


```python
# create_view method usage example with argument unpacking

kwargs: CreateViewRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Status": ...,
    "Content": ...,
    "Name": ...,
}

parent.create_view(**kwargs)
```

1. See [:material-code-braces: CreateViewRequestRequestTypeDef](./type_defs.md#createviewrequestrequesttypedef) 

### create\_view\_version

Publishes a new version of the view identifier.

Type annotations and code completion for `#!python session.create_client("connect").create_view_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_view_version.html)

```python
# create_view_version method definition

await def create_view_version(
    self,
    *,
    InstanceId: str,
    ViewId: str,
    VersionDescription: str = ...,
    ViewContentSha256: str = ...,
) -> CreateViewVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateViewVersionResponseTypeDef](./type_defs.md#createviewversionresponsetypedef) 


```python
# create_view_version method usage example with argument unpacking

kwargs: CreateViewVersionRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ViewId": ...,
}

parent.create_view_version(**kwargs)
```

1. See [:material-code-braces: CreateViewVersionRequestRequestTypeDef](./type_defs.md#createviewversionrequestrequesttypedef) 

### create\_vocabulary

Creates a custom vocabulary associated with your Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").create_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/create_vocabulary.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/deactivate_evaluation_form.html)

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

### delete\_attached\_file

Deletes an attached file along with the underlying S3 Object.

Type annotations and code completion for `#!python session.create_client("connect").delete_attached_file` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_attached_file.html)

```python
# delete_attached_file method definition

await def delete_attached_file(
    self,
    *,
    InstanceId: str,
    FileId: str,
    AssociatedResourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_attached_file method usage example with argument unpacking

kwargs: DeleteAttachedFileRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "FileId": ...,
    "AssociatedResourceArn": ...,
}

parent.delete_attached_file(**kwargs)
```

1. See [:material-code-braces: DeleteAttachedFileRequestRequestTypeDef](./type_defs.md#deleteattachedfilerequestrequesttypedef) 

### delete\_contact\_evaluation

Deletes a contact evaluation in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").delete_contact_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_contact_evaluation.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_contact_flow.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_contact_flow_module.html)

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

### delete\_email\_address

Deletes email address from the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").delete_email_address` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_email_address.html)

```python
# delete_email_address method definition

await def delete_email_address(
    self,
    *,
    InstanceId: str,
    EmailAddressId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_email_address method usage example with argument unpacking

kwargs: DeleteEmailAddressRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EmailAddressId": ...,
}

parent.delete_email_address(**kwargs)
```

1. See [:material-code-braces: DeleteEmailAddressRequestRequestTypeDef](./type_defs.md#deleteemailaddressrequestrequesttypedef) 

### delete\_evaluation\_form

Deletes an evaluation form in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").delete_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_evaluation_form.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_hours_of_operation.html)

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

### delete\_hours\_of\_operation\_override

Deletes an hours of operation override in an Amazon Connect hours of operation
resource.

Type annotations and code completion for `#!python session.create_client("connect").delete_hours_of_operation_override` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_hours_of_operation_override.html)

```python
# delete_hours_of_operation_override method definition

await def delete_hours_of_operation_override(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
    HoursOfOperationOverrideId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_hours_of_operation_override method usage example with argument unpacking

kwargs: DeleteHoursOfOperationOverrideRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
    "HoursOfOperationOverrideId": ...,
}

parent.delete_hours_of_operation_override(**kwargs)
```

1. See [:material-code-braces: DeleteHoursOfOperationOverrideRequestRequestTypeDef](./type_defs.md#deletehoursofoperationoverriderequestrequesttypedef) 

### delete\_instance

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").delete_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_instance.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_integration_association.html)

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

### delete\_predefined\_attribute

Deletes a predefined attribute from the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").delete_predefined_attribute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_predefined_attribute.html)

```python
# delete_predefined_attribute method definition

await def delete_predefined_attribute(
    self,
    *,
    InstanceId: str,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_predefined_attribute method usage example with argument unpacking

kwargs: DeletePredefinedAttributeRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
}

parent.delete_predefined_attribute(**kwargs)
```

1. See [:material-code-braces: DeletePredefinedAttributeRequestRequestTypeDef](./type_defs.md#deletepredefinedattributerequestrequesttypedef) 

### delete\_prompt

Deletes a prompt.

Type annotations and code completion for `#!python session.create_client("connect").delete_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_prompt.html)

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

### delete\_push\_notification\_registration

Deletes registration for a device token and a chat contact.

Type annotations and code completion for `#!python session.create_client("connect").delete_push_notification_registration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_push_notification_registration.html)

```python
# delete_push_notification_registration method definition

await def delete_push_notification_registration(
    self,
    *,
    InstanceId: str,
    RegistrationId: str,
    ContactId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_push_notification_registration method usage example with argument unpacking

kwargs: DeletePushNotificationRegistrationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "RegistrationId": ...,
    "ContactId": ...,
}

parent.delete_push_notification_registration(**kwargs)
```

1. See [:material-code-braces: DeletePushNotificationRegistrationRequestRequestTypeDef](./type_defs.md#deletepushnotificationregistrationrequestrequesttypedef) 

### delete\_queue

Deletes a queue.

Type annotations and code completion for `#!python session.create_client("connect").delete_queue` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_queue.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_quick_connect.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_routing_profile.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_rule.html)

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

Deletes a security profile.

Type annotations and code completion for `#!python session.create_client("connect").delete_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_security_profile.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_task_template.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_traffic_distribution_group.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_use_case.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_user.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_user_hierarchy_group.html)

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

### delete\_view

Deletes the view entirely.

Type annotations and code completion for `#!python session.create_client("connect").delete_view` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_view.html)

```python
# delete_view method definition

await def delete_view(
    self,
    *,
    InstanceId: str,
    ViewId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_view method usage example with argument unpacking

kwargs: DeleteViewRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ViewId": ...,
}

parent.delete_view(**kwargs)
```

1. See [:material-code-braces: DeleteViewRequestRequestTypeDef](./type_defs.md#deleteviewrequestrequesttypedef) 

### delete\_view\_version

Deletes the particular version specified in <code>ViewVersion</code> identifier.

Type annotations and code completion for `#!python session.create_client("connect").delete_view_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_view_version.html)

```python
# delete_view_version method definition

await def delete_view_version(
    self,
    *,
    InstanceId: str,
    ViewId: str,
    ViewVersion: int,
) -> Dict[str, Any]:
    ...
```



```python
# delete_view_version method usage example with argument unpacking

kwargs: DeleteViewVersionRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ViewId": ...,
    "ViewVersion": ...,
}

parent.delete_view_version(**kwargs)
```

1. See [:material-code-braces: DeleteViewVersionRequestRequestTypeDef](./type_defs.md#deleteviewversionrequestrequesttypedef) 

### delete\_vocabulary

Deletes the vocabulary that has the given identifier.

Type annotations and code completion for `#!python session.create_client("connect").delete_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/delete_vocabulary.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_agent_status.html)

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

### describe\_authentication\_profile

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_authentication_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_authentication_profile.html)

```python
# describe_authentication_profile method definition

await def describe_authentication_profile(
    self,
    *,
    AuthenticationProfileId: str,
    InstanceId: str,
) -> DescribeAuthenticationProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAuthenticationProfileResponseTypeDef](./type_defs.md#describeauthenticationprofileresponsetypedef) 


```python
# describe_authentication_profile method usage example with argument unpacking

kwargs: DescribeAuthenticationProfileRequestRequestTypeDef = {  # (1)
    "AuthenticationProfileId": ...,
    "InstanceId": ...,
}

parent.describe_authentication_profile(**kwargs)
```

1. See [:material-code-braces: DescribeAuthenticationProfileRequestRequestTypeDef](./type_defs.md#describeauthenticationprofilerequestrequesttypedef) 

### describe\_contact

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_contact.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_contact_evaluation.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_contact_flow.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_contact_flow_module.html)

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

### describe\_email\_address

Describe email address form the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").describe_email_address` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_email_address.html)

```python
# describe_email_address method definition

await def describe_email_address(
    self,
    *,
    InstanceId: str,
    EmailAddressId: str,
) -> DescribeEmailAddressResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEmailAddressResponseTypeDef](./type_defs.md#describeemailaddressresponsetypedef) 


```python
# describe_email_address method usage example with argument unpacking

kwargs: DescribeEmailAddressRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EmailAddressId": ...,
}

parent.describe_email_address(**kwargs)
```

1. See [:material-code-braces: DescribeEmailAddressRequestRequestTypeDef](./type_defs.md#describeemailaddressrequestrequesttypedef) 

### describe\_evaluation\_form

Describes an evaluation form in the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").describe_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_evaluation_form.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_hours_of_operation.html)

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

### describe\_hours\_of\_operation\_override

Describes the hours of operation override.

Type annotations and code completion for `#!python session.create_client("connect").describe_hours_of_operation_override` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_hours_of_operation_override.html)

```python
# describe_hours_of_operation_override method definition

await def describe_hours_of_operation_override(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
    HoursOfOperationOverrideId: str,
) -> DescribeHoursOfOperationOverrideResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHoursOfOperationOverrideResponseTypeDef](./type_defs.md#describehoursofoperationoverrideresponsetypedef) 


```python
# describe_hours_of_operation_override method usage example with argument unpacking

kwargs: DescribeHoursOfOperationOverrideRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
    "HoursOfOperationOverrideId": ...,
}

parent.describe_hours_of_operation_override(**kwargs)
```

1. See [:material-code-braces: DescribeHoursOfOperationOverrideRequestRequestTypeDef](./type_defs.md#describehoursofoperationoverriderequestrequesttypedef) 

### describe\_instance

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").describe_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_instance.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_instance_attribute.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_instance_storage_config.html)

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

Gets details and status of a phone number that's claimed to your Amazon Connect
instance or traffic distribution group.

Type annotations and code completion for `#!python session.create_client("connect").describe_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_phone_number.html)

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

### describe\_predefined\_attribute

Describes a predefined attribute for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").describe_predefined_attribute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_predefined_attribute.html)

```python
# describe_predefined_attribute method definition

await def describe_predefined_attribute(
    self,
    *,
    InstanceId: str,
    Name: str,
) -> DescribePredefinedAttributeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePredefinedAttributeResponseTypeDef](./type_defs.md#describepredefinedattributeresponsetypedef) 


```python
# describe_predefined_attribute method usage example with argument unpacking

kwargs: DescribePredefinedAttributeRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
}

parent.describe_predefined_attribute(**kwargs)
```

1. See [:material-code-braces: DescribePredefinedAttributeRequestRequestTypeDef](./type_defs.md#describepredefinedattributerequestrequesttypedef) 

### describe\_prompt

Describes the prompt.

Type annotations and code completion for `#!python session.create_client("connect").describe_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_prompt.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_queue.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_quick_connect.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_routing_profile.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_rule.html)

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

Gets basic information about the security profile.

Type annotations and code completion for `#!python session.create_client("connect").describe_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_security_profile.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_traffic_distribution_group.html)

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

Describes the specified user.

Type annotations and code completion for `#!python session.create_client("connect").describe_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_user.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_user_hierarchy_group.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_user_hierarchy_structure.html)

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

### describe\_view

Retrieves the view for the specified Amazon Connect instance and view
identifier.

Type annotations and code completion for `#!python session.create_client("connect").describe_view` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_view.html)

```python
# describe_view method definition

await def describe_view(
    self,
    *,
    InstanceId: str,
    ViewId: str,
) -> DescribeViewResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeViewResponseTypeDef](./type_defs.md#describeviewresponsetypedef) 


```python
# describe_view method usage example with argument unpacking

kwargs: DescribeViewRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ViewId": ...,
}

parent.describe_view(**kwargs)
```

1. See [:material-code-braces: DescribeViewRequestRequestTypeDef](./type_defs.md#describeviewrequestrequesttypedef) 

### describe\_vocabulary

Describes the specified vocabulary.

Type annotations and code completion for `#!python session.create_client("connect").describe_vocabulary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/describe_vocabulary.html)

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

### disassociate\_analytics\_data\_set

Removes the dataset ID associated with a given Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_analytics_data_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_analytics_data_set.html)

```python
# disassociate_analytics_data_set method definition

await def disassociate_analytics_data_set(
    self,
    *,
    InstanceId: str,
    DataSetId: str,
    TargetAccountId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_analytics_data_set method usage example with argument unpacking

kwargs: DisassociateAnalyticsDataSetRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "DataSetId": ...,
}

parent.disassociate_analytics_data_set(**kwargs)
```

1. See [:material-code-braces: DisassociateAnalyticsDataSetRequestRequestTypeDef](./type_defs.md#disassociateanalyticsdatasetrequestrequesttypedef) 

### disassociate\_approved\_origin

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_approved_origin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_approved_origin.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_bot.html)

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

### disassociate\_flow

Disassociates a connect resource from a flow.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_flow.html)

```python
# disassociate_flow method definition

await def disassociate_flow(
    self,
    *,
    InstanceId: str,
    ResourceId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 


```python
# disassociate_flow method usage example with argument unpacking

kwargs: DisassociateFlowRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ResourceId": ...,
    "ResourceType": ...,
}

parent.disassociate_flow(**kwargs)
```

1. See [:material-code-braces: DisassociateFlowRequestRequestTypeDef](./type_defs.md#disassociateflowrequestrequesttypedef) 

### disassociate\_instance\_storage\_config

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_instance_storage_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_instance_storage_config.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_lambda_function.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_lex_bot.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_phone_number_contact_flow.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_queue_quick_connects.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_routing_profile_queues.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_security_key.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_traffic_distribution_group_user.html)

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

### disassociate\_user\_proficiencies

Disassociates a set of proficiencies from a user.

Type annotations and code completion for `#!python session.create_client("connect").disassociate_user_proficiencies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/disassociate_user_proficiencies.html)

```python
# disassociate_user_proficiencies method definition

await def disassociate_user_proficiencies(
    self,
    *,
    InstanceId: str,
    UserId: str,
    UserProficiencies: Sequence[UserProficiencyDisassociateTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UserProficiencyDisassociateTypeDef](./type_defs.md#userproficiencydisassociatetypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_user_proficiencies method usage example with argument unpacking

kwargs: DisassociateUserProficienciesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "UserId": ...,
    "UserProficiencies": ...,
}

parent.disassociate_user_proficiencies(**kwargs)
```

1. See [:material-code-braces: DisassociateUserProficienciesRequestRequestTypeDef](./type_defs.md#disassociateuserproficienciesrequestrequesttypedef) 

### dismiss\_user\_contact

Dismisses contacts from an agent's CCP and returns the agent to an available
state, which allows the agent to receive a new routed contact.

Type annotations and code completion for `#!python session.create_client("connect").dismiss_user_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/dismiss_user_contact.html)

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

### get\_attached\_file

Provides a pre-signed URL for download of an approved attached file.

Type annotations and code completion for `#!python session.create_client("connect").get_attached_file` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_attached_file.html)

```python
# get_attached_file method definition

await def get_attached_file(
    self,
    *,
    InstanceId: str,
    FileId: str,
    AssociatedResourceArn: str,
    UrlExpiryInSeconds: int = ...,
) -> GetAttachedFileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAttachedFileResponseTypeDef](./type_defs.md#getattachedfileresponsetypedef) 


```python
# get_attached_file method usage example with argument unpacking

kwargs: GetAttachedFileRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "FileId": ...,
    "AssociatedResourceArn": ...,
}

parent.get_attached_file(**kwargs)
```

1. See [:material-code-braces: GetAttachedFileRequestRequestTypeDef](./type_defs.md#getattachedfilerequestrequesttypedef) 

### get\_contact\_attributes

Retrieves the contact attributes for the specified contact.

Type annotations and code completion for `#!python session.create_client("connect").get_contact_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_contact_attributes.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_current_metric_data.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_current_user_data.html)

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

### get\_effective\_hours\_of\_operations

Get the hours of operations with the effective override applied.

Type annotations and code completion for `#!python session.create_client("connect").get_effective_hours_of_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_effective_hours_of_operations.html)

```python
# get_effective_hours_of_operations method definition

await def get_effective_hours_of_operations(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
    FromDate: str,
    ToDate: str,
) -> GetEffectiveHoursOfOperationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEffectiveHoursOfOperationsResponseTypeDef](./type_defs.md#geteffectivehoursofoperationsresponsetypedef) 


```python
# get_effective_hours_of_operations method usage example with argument unpacking

kwargs: GetEffectiveHoursOfOperationsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
    "FromDate": ...,
    "ToDate": ...,
}

parent.get_effective_hours_of_operations(**kwargs)
```

1. See [:material-code-braces: GetEffectiveHoursOfOperationsRequestRequestTypeDef](./type_defs.md#geteffectivehoursofoperationsrequestrequesttypedef) 

### get\_federation\_token

Supports SAML sign-in for Amazon Connect.

Type annotations and code completion for `#!python session.create_client("connect").get_federation_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_federation_token.html)

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

### get\_flow\_association

Retrieves the flow associated for a given resource.

Type annotations and code completion for `#!python session.create_client("connect").get_flow_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_flow_association.html)

```python
# get_flow_association method definition

await def get_flow_association(
    self,
    *,
    InstanceId: str,
    ResourceId: str,
    ResourceType: FlowAssociationResourceTypeType,  # (1)
) -> GetFlowAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FlowAssociationResourceTypeType](./literals.md#flowassociationresourcetypetype) 
2. See [:material-code-braces: GetFlowAssociationResponseTypeDef](./type_defs.md#getflowassociationresponsetypedef) 


```python
# get_flow_association method usage example with argument unpacking

kwargs: GetFlowAssociationRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ResourceId": ...,
    "ResourceType": ...,
}

parent.get_flow_association(**kwargs)
```

1. See [:material-code-braces: GetFlowAssociationRequestRequestTypeDef](./type_defs.md#getflowassociationrequestrequesttypedef) 

### get\_metric\_data

Gets historical metric data from the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").get_metric_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_metric_data.html)

```python
# get_metric_data method definition

await def get_metric_data(
    self,
    *,
    InstanceId: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_metric_data_v2.html)

```python
# get_metric_data_v2 method definition

await def get_metric_data_v2(
    self,
    *,
    ResourceArn: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Filters: Sequence[FilterV2TypeDef],  # (1)
    Metrics: Sequence[MetricV2UnionTypeDef],  # (2)
    Interval: IntervalDetailsTypeDef = ...,  # (3)
    Groupings: Sequence[str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetMetricDataV2ResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: FilterV2TypeDef](./type_defs.md#filterv2typedef) 
2. See [:material-code-braces: MetricV2TypeDef](./type_defs.md#metricv2typedef) [:material-code-braces: MetricV2OutputTypeDef](./type_defs.md#metricv2outputtypedef) 
3. See [:material-code-braces: IntervalDetailsTypeDef](./type_defs.md#intervaldetailstypedef) 
4. See [:material-code-braces: GetMetricDataV2ResponseTypeDef](./type_defs.md#getmetricdatav2responsetypedef) 


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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_prompt_file.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_task_template.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/get_traffic_distribution.html)

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

### import\_phone\_number

Imports a claimed phone number from an external service, such as Amazon Web
Services End User Messaging, into an Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").import_phone_number` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/import_phone_number.html)

```python
# import_phone_number method definition

await def import_phone_number(
    self,
    *,
    InstanceId: str,
    SourcePhoneNumberArn: str,
    PhoneNumberDescription: str = ...,
    Tags: Mapping[str, str] = ...,
    ClientToken: str = ...,
) -> ImportPhoneNumberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ImportPhoneNumberResponseTypeDef](./type_defs.md#importphonenumberresponsetypedef) 


```python
# import_phone_number method usage example with argument unpacking

kwargs: ImportPhoneNumberRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "SourcePhoneNumberArn": ...,
}

parent.import_phone_number(**kwargs)
```

1. See [:material-code-braces: ImportPhoneNumberRequestRequestTypeDef](./type_defs.md#importphonenumberrequestrequesttypedef) 

### list\_agent\_statuses

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_agent_statuses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_agent_statuses.html)

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

### list\_analytics\_data\_associations

Lists the association status of requested dataset ID for a given Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").list_analytics_data_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_analytics_data_associations.html)

```python
# list_analytics_data_associations method definition

await def list_analytics_data_associations(
    self,
    *,
    InstanceId: str,
    DataSetId: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAnalyticsDataAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAnalyticsDataAssociationsResponseTypeDef](./type_defs.md#listanalyticsdataassociationsresponsetypedef) 


```python
# list_analytics_data_associations method usage example with argument unpacking

kwargs: ListAnalyticsDataAssociationsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_analytics_data_associations(**kwargs)
```

1. See [:material-code-braces: ListAnalyticsDataAssociationsRequestRequestTypeDef](./type_defs.md#listanalyticsdataassociationsrequestrequesttypedef) 

### list\_approved\_origins

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_approved_origins` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_approved_origins.html)

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

### list\_associated\_contacts

Provides information about contact tree, a list of associated contacts with a
unique identifier.

Type annotations and code completion for `#!python session.create_client("connect").list_associated_contacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_associated_contacts.html)

```python
# list_associated_contacts method definition

await def list_associated_contacts(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAssociatedContactsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssociatedContactsResponseTypeDef](./type_defs.md#listassociatedcontactsresponsetypedef) 


```python
# list_associated_contacts method usage example with argument unpacking

kwargs: ListAssociatedContactsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
}

parent.list_associated_contacts(**kwargs)
```

1. See [:material-code-braces: ListAssociatedContactsRequestRequestTypeDef](./type_defs.md#listassociatedcontactsrequestrequesttypedef) 

### list\_authentication\_profiles

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_authentication_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_authentication_profiles.html)

```python
# list_authentication_profiles method definition

await def list_authentication_profiles(
    self,
    *,
    InstanceId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAuthenticationProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAuthenticationProfilesResponseTypeDef](./type_defs.md#listauthenticationprofilesresponsetypedef) 


```python
# list_authentication_profiles method usage example with argument unpacking

kwargs: ListAuthenticationProfilesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_authentication_profiles(**kwargs)
```

1. See [:material-code-braces: ListAuthenticationProfilesRequestRequestTypeDef](./type_defs.md#listauthenticationprofilesrequestrequesttypedef) 

### list\_bots

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").list_bots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_bots.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_contact_evaluations.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_contact_flow_modules.html)

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

### list\_contact\_flow\_versions

Returns all the available versions for the specified Amazon Connect instance
and flow identifier.

Type annotations and code completion for `#!python session.create_client("connect").list_contact_flow_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_contact_flow_versions.html)

```python
# list_contact_flow_versions method definition

await def list_contact_flow_versions(
    self,
    *,
    InstanceId: str,
    ContactFlowId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListContactFlowVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListContactFlowVersionsResponseTypeDef](./type_defs.md#listcontactflowversionsresponsetypedef) 


```python
# list_contact_flow_versions method usage example with argument unpacking

kwargs: ListContactFlowVersionsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactFlowId": ...,
}

parent.list_contact_flow_versions(**kwargs)
```

1. See [:material-code-braces: ListContactFlowVersionsRequestRequestTypeDef](./type_defs.md#listcontactflowversionsrequestrequesttypedef) 

### list\_contact\_flows

Provides information about the flows for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_contact_flows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_contact_flows.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_contact_references.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_default_vocabularies.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_evaluation_form_versions.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_evaluation_forms.html)

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

### list\_flow\_associations

List the flow association based on the filters.

Type annotations and code completion for `#!python session.create_client("connect").list_flow_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_flow_associations.html)

```python
# list_flow_associations method definition

await def list_flow_associations(
    self,
    *,
    InstanceId: str,
    ResourceType: ListFlowAssociationResourceTypeType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListFlowAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ListFlowAssociationResourceTypeType](./literals.md#listflowassociationresourcetypetype) 
2. See [:material-code-braces: ListFlowAssociationsResponseTypeDef](./type_defs.md#listflowassociationsresponsetypedef) 


```python
# list_flow_associations method usage example with argument unpacking

kwargs: ListFlowAssociationsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_flow_associations(**kwargs)
```

1. See [:material-code-braces: ListFlowAssociationsRequestRequestTypeDef](./type_defs.md#listflowassociationsrequestrequesttypedef) 

### list\_hours\_of\_operation\_overrides

List the hours of operation overrides.

Type annotations and code completion for `#!python session.create_client("connect").list_hours_of_operation_overrides` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_hours_of_operation_overrides.html)

```python
# list_hours_of_operation_overrides method definition

await def list_hours_of_operation_overrides(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListHoursOfOperationOverridesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListHoursOfOperationOverridesResponseTypeDef](./type_defs.md#listhoursofoperationoverridesresponsetypedef) 


```python
# list_hours_of_operation_overrides method usage example with argument unpacking

kwargs: ListHoursOfOperationOverridesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
}

parent.list_hours_of_operation_overrides(**kwargs)
```

1. See [:material-code-braces: ListHoursOfOperationOverridesRequestRequestTypeDef](./type_defs.md#listhoursofoperationoverridesrequestrequesttypedef) 

### list\_hours\_of\_operations

Provides information about the hours of operation for the specified Amazon
Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_hours_of_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_hours_of_operations.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_instance_attributes.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_instance_storage_configs.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_instances.html)

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

Provides summary information about the Amazon Web Services resource
associations for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_integration_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_integration_associations.html)

```python
# list_integration_associations method definition

await def list_integration_associations(
    self,
    *,
    InstanceId: str,
    IntegrationType: IntegrationTypeType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    IntegrationArn: str = ...,
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_lambda_functions.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_lex_bots.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_phone_numbers.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_phone_numbers_v2.html)

```python
# list_phone_numbers_v2 method definition

await def list_phone_numbers_v2(
    self,
    *,
    TargetArn: str = ...,
    InstanceId: str = ...,
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

### list\_predefined\_attributes

Lists predefined attributes for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_predefined_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_predefined_attributes.html)

```python
# list_predefined_attributes method definition

await def list_predefined_attributes(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPredefinedAttributesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPredefinedAttributesResponseTypeDef](./type_defs.md#listpredefinedattributesresponsetypedef) 


```python
# list_predefined_attributes method usage example with argument unpacking

kwargs: ListPredefinedAttributesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_predefined_attributes(**kwargs)
```

1. See [:material-code-braces: ListPredefinedAttributesRequestRequestTypeDef](./type_defs.md#listpredefinedattributesrequestrequesttypedef) 

### list\_prompts

Provides information about the prompts for the specified Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").list_prompts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_prompts.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_queue_quick_connects.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_queues.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_quick_connects.html)

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

### list\_realtime\_contact\_analysis\_segments\_v2

Provides a list of analysis segments for a real-time analysis session.

Type annotations and code completion for `#!python session.create_client("connect").list_realtime_contact_analysis_segments_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_realtime_contact_analysis_segments_v2.html)

```python
# list_realtime_contact_analysis_segments_v2 method definition

await def list_realtime_contact_analysis_segments_v2(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    OutputType: RealTimeContactAnalysisOutputTypeType,  # (1)
    SegmentTypes: Sequence[RealTimeContactAnalysisSegmentTypeType],  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RealTimeContactAnalysisOutputTypeType](./literals.md#realtimecontactanalysisoutputtypetype) 
2. See [:material-code-brackets: RealTimeContactAnalysisSegmentTypeType](./literals.md#realtimecontactanalysissegmenttypetype) 
3. See [:material-code-braces: ListRealtimeContactAnalysisSegmentsV2ResponseTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsv2responsetypedef) 


```python
# list_realtime_contact_analysis_segments_v2 method usage example with argument unpacking

kwargs: ListRealtimeContactAnalysisSegmentsV2RequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "OutputType": ...,
    "SegmentTypes": ...,
}

parent.list_realtime_contact_analysis_segments_v2(**kwargs)
```

1. See [:material-code-braces: ListRealtimeContactAnalysisSegmentsV2RequestRequestTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsv2requestrequesttypedef) 

### list\_routing\_profile\_queues

Lists the queues associated with a routing profile.

Type annotations and code completion for `#!python session.create_client("connect").list_routing_profile_queues` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_routing_profile_queues.html)

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

Provides summary information about the routing profiles for the specified
Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_routing_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_routing_profiles.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_rules.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_security_keys.html)

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

### list\_security\_profile\_applications

Returns a list of third-party applications in a specific security profile.

Type annotations and code completion for `#!python session.create_client("connect").list_security_profile_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_security_profile_applications.html)

```python
# list_security_profile_applications method definition

await def list_security_profile_applications(
    self,
    *,
    SecurityProfileId: str,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSecurityProfileApplicationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSecurityProfileApplicationsResponseTypeDef](./type_defs.md#listsecurityprofileapplicationsresponsetypedef) 


```python
# list_security_profile_applications method usage example with argument unpacking

kwargs: ListSecurityProfileApplicationsRequestRequestTypeDef = {  # (1)
    "SecurityProfileId": ...,
    "InstanceId": ...,
}

parent.list_security_profile_applications(**kwargs)
```

1. See [:material-code-braces: ListSecurityProfileApplicationsRequestRequestTypeDef](./type_defs.md#listsecurityprofileapplicationsrequestrequesttypedef) 

### list\_security\_profile\_permissions

Lists the permissions granted to a security profile.

Type annotations and code completion for `#!python session.create_client("connect").list_security_profile_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_security_profile_permissions.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_security_profiles.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_tags_for_resource.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_task_templates.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_traffic_distribution_group_users.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_traffic_distribution_groups.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_use_cases.html)

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

Provides summary information about the hierarchy groups for the specified
Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").list_user_hierarchy_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_user_hierarchy_groups.html)

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

### list\_user\_proficiencies

Lists proficiencies associated with a user.

Type annotations and code completion for `#!python session.create_client("connect").list_user_proficiencies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_user_proficiencies.html)

```python
# list_user_proficiencies method definition

await def list_user_proficiencies(
    self,
    *,
    InstanceId: str,
    UserId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListUserProficienciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUserProficienciesResponseTypeDef](./type_defs.md#listuserproficienciesresponsetypedef) 


```python
# list_user_proficiencies method usage example with argument unpacking

kwargs: ListUserProficienciesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "UserId": ...,
}

parent.list_user_proficiencies(**kwargs)
```

1. See [:material-code-braces: ListUserProficienciesRequestRequestTypeDef](./type_defs.md#listuserproficienciesrequestrequesttypedef) 

### list\_users

Provides summary information about the users for the specified Amazon Connect
instance.

Type annotations and code completion for `#!python session.create_client("connect").list_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_users.html)

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

### list\_view\_versions

Returns all the available versions for the specified Amazon Connect instance
and view identifier.

Type annotations and code completion for `#!python session.create_client("connect").list_view_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_view_versions.html)

```python
# list_view_versions method definition

await def list_view_versions(
    self,
    *,
    InstanceId: str,
    ViewId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListViewVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListViewVersionsResponseTypeDef](./type_defs.md#listviewversionsresponsetypedef) 


```python
# list_view_versions method usage example with argument unpacking

kwargs: ListViewVersionsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ViewId": ...,
}

parent.list_view_versions(**kwargs)
```

1. See [:material-code-braces: ListViewVersionsRequestRequestTypeDef](./type_defs.md#listviewversionsrequestrequesttypedef) 

### list\_views

Returns views in the given instance.

Type annotations and code completion for `#!python session.create_client("connect").list_views` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/list_views.html)

```python
# list_views method definition

await def list_views(
    self,
    *,
    InstanceId: str,
    Type: ViewTypeType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListViewsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ViewTypeType](./literals.md#viewtypetype) 
2. See [:material-code-braces: ListViewsResponseTypeDef](./type_defs.md#listviewsresponsetypedef) 


```python
# list_views method usage example with argument unpacking

kwargs: ListViewsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.list_views(**kwargs)
```

1. See [:material-code-braces: ListViewsRequestRequestTypeDef](./type_defs.md#listviewsrequestrequesttypedef) 

### monitor\_contact

Initiates silent monitoring of a contact.

Type annotations and code completion for `#!python session.create_client("connect").monitor_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/monitor_contact.html)

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

### pause\_contact

Allows pausing an ongoing task contact.

Type annotations and code completion for `#!python session.create_client("connect").pause_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/pause_contact.html)

```python
# pause_contact method definition

await def pause_contact(
    self,
    *,
    ContactId: str,
    InstanceId: str,
    ContactFlowId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# pause_contact method usage example with argument unpacking

kwargs: PauseContactRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
    "InstanceId": ...,
}

parent.pause_contact(**kwargs)
```

1. See [:material-code-braces: PauseContactRequestRequestTypeDef](./type_defs.md#pausecontactrequestrequesttypedef) 

### put\_user\_status

Changes the current status of a user or agent in Amazon Connect.

Type annotations and code completion for `#!python session.create_client("connect").put_user_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/put_user_status.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/release_phone_number.html)

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
Region and copies configuration information for Amazon Connect resources across
Amazon Web Services Regions.

Type annotations and code completion for `#!python session.create_client("connect").replicate_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/replicate_instance.html)

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

### resume\_contact

Allows resuming a task contact in a paused state.

Type annotations and code completion for `#!python session.create_client("connect").resume_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/resume_contact.html)

```python
# resume_contact method definition

await def resume_contact(
    self,
    *,
    ContactId: str,
    InstanceId: str,
    ContactFlowId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# resume_contact method usage example with argument unpacking

kwargs: ResumeContactRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
    "InstanceId": ...,
}

parent.resume_contact(**kwargs)
```

1. See [:material-code-braces: ResumeContactRequestRequestTypeDef](./type_defs.md#resumecontactrequestrequesttypedef) 

### resume\_contact\_recording

When a contact is being recorded, and the recording has been suspended using
SuspendContactRecording, this API resumes recording whatever recording is
selected in the flow configuration: call, screen, or both.

Type annotations and code completion for `#!python session.create_client("connect").resume_contact_recording` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/resume_contact_recording.html)

```python
# resume_contact_recording method definition

await def resume_contact_recording(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
    ContactRecordingType: ContactRecordingTypeType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ContactRecordingTypeType](./literals.md#contactrecordingtypetype) 


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

### search\_agent\_statuses

Searches AgentStatuses in an Amazon Connect instance, with optional filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_agent_statuses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_agent_statuses.html)

```python
# search_agent_statuses method definition

await def search_agent_statuses(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: AgentStatusSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: AgentStatusSearchCriteriaTypeDef = ...,  # (2)
) -> SearchAgentStatusesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AgentStatusSearchFilterTypeDef](./type_defs.md#agentstatussearchfiltertypedef) 
2. See [:material-code-braces: AgentStatusSearchCriteriaTypeDef](./type_defs.md#agentstatussearchcriteriatypedef) 
3. See [:material-code-braces: SearchAgentStatusesResponseTypeDef](./type_defs.md#searchagentstatusesresponsetypedef) 


```python
# search_agent_statuses method usage example with argument unpacking

kwargs: SearchAgentStatusesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_agent_statuses(**kwargs)
```

1. See [:material-code-braces: SearchAgentStatusesRequestRequestTypeDef](./type_defs.md#searchagentstatusesrequestrequesttypedef) 

### search\_available\_phone\_numbers

Searches for available phone numbers that you can claim to your Amazon Connect
instance or traffic distribution group.

Type annotations and code completion for `#!python session.create_client("connect").search_available_phone_numbers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_available_phone_numbers.html)

```python
# search_available_phone_numbers method definition

await def search_available_phone_numbers(
    self,
    *,
    PhoneNumberCountryCode: PhoneNumberCountryCodeType,  # (1)
    PhoneNumberType: PhoneNumberTypeType,  # (2)
    TargetArn: str = ...,
    InstanceId: str = ...,
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
    "PhoneNumberCountryCode": ...,
    "PhoneNumberType": ...,
}

parent.search_available_phone_numbers(**kwargs)
```

1. See [:material-code-braces: SearchAvailablePhoneNumbersRequestRequestTypeDef](./type_defs.md#searchavailablephonenumbersrequestrequesttypedef) 

### search\_contact\_flow\_modules

Searches the flow modules in an Amazon Connect instance, with optional
filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_contact_flow_modules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_contact_flow_modules.html)

```python
# search_contact_flow_modules method definition

await def search_contact_flow_modules(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: ContactFlowModuleSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: ContactFlowModuleSearchCriteriaTypeDef = ...,  # (2)
) -> SearchContactFlowModulesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ContactFlowModuleSearchFilterTypeDef](./type_defs.md#contactflowmodulesearchfiltertypedef) 
2. See [:material-code-braces: ContactFlowModuleSearchCriteriaTypeDef](./type_defs.md#contactflowmodulesearchcriteriatypedef) 
3. See [:material-code-braces: SearchContactFlowModulesResponseTypeDef](./type_defs.md#searchcontactflowmodulesresponsetypedef) 


```python
# search_contact_flow_modules method usage example with argument unpacking

kwargs: SearchContactFlowModulesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_contact_flow_modules(**kwargs)
```

1. See [:material-code-braces: SearchContactFlowModulesRequestRequestTypeDef](./type_defs.md#searchcontactflowmodulesrequestrequesttypedef) 

### search\_contact\_flows

Searches the flows in an Amazon Connect instance, with optional filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_contact_flows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_contact_flows.html)

```python
# search_contact_flows method definition

await def search_contact_flows(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: ContactFlowSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: ContactFlowSearchCriteriaTypeDef = ...,  # (2)
) -> SearchContactFlowsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ContactFlowSearchFilterTypeDef](./type_defs.md#contactflowsearchfiltertypedef) 
2. See [:material-code-braces: ContactFlowSearchCriteriaTypeDef](./type_defs.md#contactflowsearchcriteriatypedef) 
3. See [:material-code-braces: SearchContactFlowsResponseTypeDef](./type_defs.md#searchcontactflowsresponsetypedef) 


```python
# search_contact_flows method usage example with argument unpacking

kwargs: SearchContactFlowsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_contact_flows(**kwargs)
```

1. See [:material-code-braces: SearchContactFlowsRequestRequestTypeDef](./type_defs.md#searchcontactflowsrequestrequesttypedef) 

### search\_contacts

Searches contacts in an Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").search_contacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_contacts.html)

```python
# search_contacts method definition

await def search_contacts(
    self,
    *,
    InstanceId: str,
    TimeRange: SearchContactsTimeRangeTypeDef,  # (1)
    SearchCriteria: SearchCriteriaTypeDef = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
    Sort: SortTypeDef = ...,  # (3)
) -> SearchContactsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SearchContactsTimeRangeTypeDef](./type_defs.md#searchcontactstimerangetypedef) 
2. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef) 
3. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
4. See [:material-code-braces: SearchContactsResponseTypeDef](./type_defs.md#searchcontactsresponsetypedef) 


```python
# search_contacts method usage example with argument unpacking

kwargs: SearchContactsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "TimeRange": ...,
}

parent.search_contacts(**kwargs)
```

1. See [:material-code-braces: SearchContactsRequestRequestTypeDef](./type_defs.md#searchcontactsrequestrequesttypedef) 

### search\_email\_addresses

Searches email address in an instance, with optional filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_email_addresses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_email_addresses.html)

```python
# search_email_addresses method definition

await def search_email_addresses(
    self,
    *,
    InstanceId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    SearchCriteria: EmailAddressSearchCriteriaTypeDef = ...,  # (1)
    SearchFilter: EmailAddressSearchFilterTypeDef = ...,  # (2)
) -> SearchEmailAddressesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EmailAddressSearchCriteriaTypeDef](./type_defs.md#emailaddresssearchcriteriatypedef) 
2. See [:material-code-braces: EmailAddressSearchFilterTypeDef](./type_defs.md#emailaddresssearchfiltertypedef) 
3. See [:material-code-braces: SearchEmailAddressesResponseTypeDef](./type_defs.md#searchemailaddressesresponsetypedef) 


```python
# search_email_addresses method usage example with argument unpacking

kwargs: SearchEmailAddressesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_email_addresses(**kwargs)
```

1. See [:material-code-braces: SearchEmailAddressesRequestRequestTypeDef](./type_defs.md#searchemailaddressesrequestrequesttypedef) 

### search\_hours\_of\_operation\_overrides

Searches the hours of operation overrides.

Type annotations and code completion for `#!python session.create_client("connect").search_hours_of_operation_overrides` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_hours_of_operation_overrides.html)

```python
# search_hours_of_operation_overrides method definition

await def search_hours_of_operation_overrides(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: HoursOfOperationSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: HoursOfOperationOverrideSearchCriteriaTypeDef = ...,  # (2)
) -> SearchHoursOfOperationOverridesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: HoursOfOperationSearchFilterTypeDef](./type_defs.md#hoursofoperationsearchfiltertypedef) 
2. See [:material-code-braces: HoursOfOperationOverrideSearchCriteriaTypeDef](./type_defs.md#hoursofoperationoverridesearchcriteriatypedef) 
3. See [:material-code-braces: SearchHoursOfOperationOverridesResponseTypeDef](./type_defs.md#searchhoursofoperationoverridesresponsetypedef) 


```python
# search_hours_of_operation_overrides method usage example with argument unpacking

kwargs: SearchHoursOfOperationOverridesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_hours_of_operation_overrides(**kwargs)
```

1. See [:material-code-braces: SearchHoursOfOperationOverridesRequestRequestTypeDef](./type_defs.md#searchhoursofoperationoverridesrequestrequesttypedef) 

### search\_hours\_of\_operations

Searches the hours of operation in an Amazon Connect instance, with optional
filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_hours_of_operations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_hours_of_operations.html)

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

### search\_predefined\_attributes

Searches predefined attributes that meet certain criteria.

Type annotations and code completion for `#!python session.create_client("connect").search_predefined_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_predefined_attributes.html)

```python
# search_predefined_attributes method definition

await def search_predefined_attributes(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchCriteria: PredefinedAttributeSearchCriteriaTypeDef = ...,  # (1)
) -> SearchPredefinedAttributesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PredefinedAttributeSearchCriteriaTypeDef](./type_defs.md#predefinedattributesearchcriteriatypedef) 
2. See [:material-code-braces: SearchPredefinedAttributesResponseTypeDef](./type_defs.md#searchpredefinedattributesresponsetypedef) 


```python
# search_predefined_attributes method usage example with argument unpacking

kwargs: SearchPredefinedAttributesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_predefined_attributes(**kwargs)
```

1. See [:material-code-braces: SearchPredefinedAttributesRequestRequestTypeDef](./type_defs.md#searchpredefinedattributesrequestrequesttypedef) 

### search\_prompts

Searches prompts in an Amazon Connect instance, with optional filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_prompts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_prompts.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_queues.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_quick_connects.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_resource_tags.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_routing_profiles.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_security_profiles.html)

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

### search\_user\_hierarchy\_groups

Searches UserHierarchyGroups in an Amazon Connect instance, with optional
filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_user_hierarchy_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_user_hierarchy_groups.html)

```python
# search_user_hierarchy_groups method definition

await def search_user_hierarchy_groups(
    self,
    *,
    InstanceId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    SearchFilter: UserHierarchyGroupSearchFilterTypeDef = ...,  # (1)
    SearchCriteria: UserHierarchyGroupSearchCriteriaTypeDef = ...,  # (2)
) -> SearchUserHierarchyGroupsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UserHierarchyGroupSearchFilterTypeDef](./type_defs.md#userhierarchygroupsearchfiltertypedef) 
2. See [:material-code-braces: UserHierarchyGroupSearchCriteriaTypeDef](./type_defs.md#userhierarchygroupsearchcriteriatypedef) 
3. See [:material-code-braces: SearchUserHierarchyGroupsResponseTypeDef](./type_defs.md#searchuserhierarchygroupsresponsetypedef) 


```python
# search_user_hierarchy_groups method usage example with argument unpacking

kwargs: SearchUserHierarchyGroupsRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
}

parent.search_user_hierarchy_groups(**kwargs)
```

1. See [:material-code-braces: SearchUserHierarchyGroupsRequestRequestTypeDef](./type_defs.md#searchuserhierarchygroupsrequestrequesttypedef) 

### search\_users

Searches users in an Amazon Connect instance, with optional filtering.

Type annotations and code completion for `#!python session.create_client("connect").search_users` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_users.html)

```python
# search_users method definition

await def search_users(
    self,
    *,
    InstanceId: str,
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
<code>State</code>, <code>NameStartsWith</code>, and <code>LanguageCode</code>.

Type annotations and code completion for `#!python session.create_client("connect").search_vocabularies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/search_vocabularies.html)

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

### send\_chat\_integration\_event

Processes chat integration events from Amazon Web Services or external
integrations to Amazon Connect.

Type annotations and code completion for `#!python session.create_client("connect").send_chat_integration_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/send_chat_integration_event.html)

```python
# send_chat_integration_event method definition

await def send_chat_integration_event(
    self,
    *,
    SourceId: str,
    DestinationId: str,
    Event: ChatEventTypeDef,  # (1)
    Subtype: str = ...,
    NewSessionDetails: NewSessionDetailsTypeDef = ...,  # (2)
) -> SendChatIntegrationEventResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ChatEventTypeDef](./type_defs.md#chateventtypedef) 
2. See [:material-code-braces: NewSessionDetailsTypeDef](./type_defs.md#newsessiondetailstypedef) 
3. See [:material-code-braces: SendChatIntegrationEventResponseTypeDef](./type_defs.md#sendchatintegrationeventresponsetypedef) 


```python
# send_chat_integration_event method usage example with argument unpacking

kwargs: SendChatIntegrationEventRequestRequestTypeDef = {  # (1)
    "SourceId": ...,
    "DestinationId": ...,
    "Event": ...,
}

parent.send_chat_integration_event(**kwargs)
```

1. See [:material-code-braces: SendChatIntegrationEventRequestRequestTypeDef](./type_defs.md#sendchatintegrationeventrequestrequesttypedef) 

### send\_outbound\_email

Send outbound email for outbound campaigns.

Type annotations and code completion for `#!python session.create_client("connect").send_outbound_email` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/send_outbound_email.html)

```python
# send_outbound_email method definition

await def send_outbound_email(
    self,
    *,
    InstanceId: str,
    FromEmailAddress: EmailAddressInfoTypeDef,  # (1)
    DestinationEmailAddress: EmailAddressInfoTypeDef,  # (1)
    EmailMessage: OutboundEmailContentTypeDef,  # (3)
    TrafficType: TrafficTypeType,  # (4)
    AdditionalRecipients: OutboundAdditionalRecipientsTypeDef = ...,  # (5)
    SourceCampaign: SourceCampaignTypeDef = ...,  # (6)
    ClientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
2. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
3. See [:material-code-braces: OutboundEmailContentTypeDef](./type_defs.md#outboundemailcontenttypedef) 
4. See [:material-code-brackets: TrafficTypeType](./literals.md#traffictypetype) 
5. See [:material-code-braces: OutboundAdditionalRecipientsTypeDef](./type_defs.md#outboundadditionalrecipientstypedef) 
6. See [:material-code-braces: SourceCampaignTypeDef](./type_defs.md#sourcecampaigntypedef) 


```python
# send_outbound_email method usage example with argument unpacking

kwargs: SendOutboundEmailRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "FromEmailAddress": ...,
    "DestinationEmailAddress": ...,
    "EmailMessage": ...,
    "TrafficType": ...,
}

parent.send_outbound_email(**kwargs)
```

1. See [:material-code-braces: SendOutboundEmailRequestRequestTypeDef](./type_defs.md#sendoutboundemailrequestrequesttypedef) 

### start\_attached\_file\_upload

Provides a pre-signed Amazon S3 URL in response for uploading your content.

Type annotations and code completion for `#!python session.create_client("connect").start_attached_file_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_attached_file_upload.html)

```python
# start_attached_file_upload method definition

await def start_attached_file_upload(
    self,
    *,
    InstanceId: str,
    FileName: str,
    FileSizeInBytes: int,
    FileUseCaseType: FileUseCaseTypeType,  # (1)
    AssociatedResourceArn: str,
    ClientToken: str = ...,
    UrlExpiryInSeconds: int = ...,
    CreatedBy: CreatedByInfoTypeDef = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> StartAttachedFileUploadResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: FileUseCaseTypeType](./literals.md#fileusecasetypetype) 
2. See [:material-code-braces: CreatedByInfoTypeDef](./type_defs.md#createdbyinfotypedef) 
3. See [:material-code-braces: StartAttachedFileUploadResponseTypeDef](./type_defs.md#startattachedfileuploadresponsetypedef) 


```python
# start_attached_file_upload method usage example with argument unpacking

kwargs: StartAttachedFileUploadRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "FileName": ...,
    "FileSizeInBytes": ...,
    "FileUseCaseType": ...,
    "AssociatedResourceArn": ...,
}

parent.start_attached_file_upload(**kwargs)
```

1. See [:material-code-braces: StartAttachedFileUploadRequestRequestTypeDef](./type_defs.md#startattachedfileuploadrequestrequesttypedef) 

### start\_chat\_contact

Initiates a flow to start a new chat for the customer.

Type annotations and code completion for `#!python session.create_client("connect").start_chat_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_chat_contact.html)

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
    SegmentAttributes: Mapping[str, SegmentAttributeValueTypeDef] = ...,  # (4)
) -> StartChatContactResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
2. See [:material-code-braces: ChatMessageTypeDef](./type_defs.md#chatmessagetypedef) 
3. See [:material-code-braces: PersistentChatTypeDef](./type_defs.md#persistentchattypedef) 
4. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) 
5. See [:material-code-braces: StartChatContactResponseTypeDef](./type_defs.md#startchatcontactresponsetypedef) 


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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_contact_evaluation.html)

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

Starts recording the contact:.

Type annotations and code completion for `#!python session.create_client("connect").start_contact_recording` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_contact_recording.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_contact_streaming.html)

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

### start\_email\_contact

Creates an inbound email contact and initiates a flow to start the email
contact for the customer.

Type annotations and code completion for `#!python session.create_client("connect").start_email_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_email_contact.html)

```python
# start_email_contact method definition

await def start_email_contact(
    self,
    *,
    InstanceId: str,
    FromEmailAddress: EmailAddressInfoTypeDef,  # (1)
    DestinationEmailAddress: str,
    EmailMessage: InboundEmailContentTypeDef,  # (2)
    Description: str = ...,
    References: Mapping[str, ReferenceTypeDef] = ...,  # (3)
    Name: str = ...,
    AdditionalRecipients: InboundAdditionalRecipientsTypeDef = ...,  # (4)
    Attachments: Sequence[EmailAttachmentTypeDef] = ...,  # (5)
    ContactFlowId: str = ...,
    RelatedContactId: str = ...,
    Attributes: Mapping[str, str] = ...,
    SegmentAttributes: Mapping[str, SegmentAttributeValueTypeDef] = ...,  # (6)
    ClientToken: str = ...,
) -> StartEmailContactResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
2. See [:material-code-braces: InboundEmailContentTypeDef](./type_defs.md#inboundemailcontenttypedef) 
3. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
4. See [:material-code-braces: InboundAdditionalRecipientsTypeDef](./type_defs.md#inboundadditionalrecipientstypedef) 
5. See [:material-code-braces: EmailAttachmentTypeDef](./type_defs.md#emailattachmenttypedef) 
6. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) 
7. See [:material-code-braces: StartEmailContactResponseTypeDef](./type_defs.md#startemailcontactresponsetypedef) 


```python
# start_email_contact method usage example with argument unpacking

kwargs: StartEmailContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "FromEmailAddress": ...,
    "DestinationEmailAddress": ...,
    "EmailMessage": ...,
}

parent.start_email_contact(**kwargs)
```

1. See [:material-code-braces: StartEmailContactRequestRequestTypeDef](./type_defs.md#startemailcontactrequestrequesttypedef) 

### start\_outbound\_chat\_contact

Initiates a new outbound SMS contact to a customer.

Type annotations and code completion for `#!python session.create_client("connect").start_outbound_chat_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_outbound_chat_contact.html)

```python
# start_outbound_chat_contact method definition

await def start_outbound_chat_contact(
    self,
    *,
    SourceEndpoint: EndpointTypeDef,  # (1)
    DestinationEndpoint: EndpointTypeDef,  # (1)
    InstanceId: str,
    SegmentAttributes: Mapping[str, SegmentAttributeValueTypeDef],  # (3)
    ContactFlowId: str,
    Attributes: Mapping[str, str] = ...,
    ChatDurationInMinutes: int = ...,
    ParticipantDetails: ParticipantDetailsTypeDef = ...,  # (4)
    InitialSystemMessage: ChatMessageTypeDef = ...,  # (5)
    RelatedContactId: str = ...,
    SupportedMessagingContentTypes: Sequence[str] = ...,
    ClientToken: str = ...,
) -> StartOutboundChatContactResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
3. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) 
4. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
5. See [:material-code-braces: ChatMessageTypeDef](./type_defs.md#chatmessagetypedef) 
6. See [:material-code-braces: StartOutboundChatContactResponseTypeDef](./type_defs.md#startoutboundchatcontactresponsetypedef) 


```python
# start_outbound_chat_contact method usage example with argument unpacking

kwargs: StartOutboundChatContactRequestRequestTypeDef = {  # (1)
    "SourceEndpoint": ...,
    "DestinationEndpoint": ...,
    "InstanceId": ...,
    "SegmentAttributes": ...,
    "ContactFlowId": ...,
}

parent.start_outbound_chat_contact(**kwargs)
```

1. See [:material-code-braces: StartOutboundChatContactRequestRequestTypeDef](./type_defs.md#startoutboundchatcontactrequestrequesttypedef) 

### start\_outbound\_email\_contact

Initiates a flow to send an agent reply or outbound email contact (created from
the CreateContact API) to a customer.

Type annotations and code completion for `#!python session.create_client("connect").start_outbound_email_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_outbound_email_contact.html)

```python
# start_outbound_email_contact method definition

await def start_outbound_email_contact(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    DestinationEmailAddress: EmailAddressInfoTypeDef,  # (1)
    EmailMessage: OutboundEmailContentTypeDef,  # (2)
    FromEmailAddress: EmailAddressInfoTypeDef = ...,  # (1)
    AdditionalRecipients: OutboundAdditionalRecipientsTypeDef = ...,  # (4)
    ClientToken: str = ...,
) -> StartOutboundEmailContactResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
2. See [:material-code-braces: OutboundEmailContentTypeDef](./type_defs.md#outboundemailcontenttypedef) 
3. See [:material-code-braces: EmailAddressInfoTypeDef](./type_defs.md#emailaddressinfotypedef) 
4. See [:material-code-braces: OutboundAdditionalRecipientsTypeDef](./type_defs.md#outboundadditionalrecipientstypedef) 
5. See [:material-code-braces: StartOutboundEmailContactResponseTypeDef](./type_defs.md#startoutboundemailcontactresponsetypedef) 


```python
# start_outbound_email_contact method usage example with argument unpacking

kwargs: StartOutboundEmailContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
    "DestinationEmailAddress": ...,
    "EmailMessage": ...,
}

parent.start_outbound_email_contact(**kwargs)
```

1. See [:material-code-braces: StartOutboundEmailContactRequestRequestTypeDef](./type_defs.md#startoutboundemailcontactrequestrequesttypedef) 

### start\_outbound\_voice\_contact

Places an outbound call to a contact, and then initiates the flow.

Type annotations and code completion for `#!python session.create_client("connect").start_outbound_voice_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_outbound_voice_contact.html)

```python
# start_outbound_voice_contact method definition

await def start_outbound_voice_contact(
    self,
    *,
    DestinationPhoneNumber: str,
    ContactFlowId: str,
    InstanceId: str,
    Name: str = ...,
    Description: str = ...,
    References: Mapping[str, ReferenceTypeDef] = ...,  # (1)
    RelatedContactId: str = ...,
    ClientToken: str = ...,
    SourcePhoneNumber: str = ...,
    QueueId: str = ...,
    Attributes: Mapping[str, str] = ...,
    AnswerMachineDetectionConfig: AnswerMachineDetectionConfigTypeDef = ...,  # (2)
    CampaignId: str = ...,
    TrafficType: TrafficTypeType = ...,  # (3)
) -> StartOutboundVoiceContactResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
2. See [:material-code-braces: AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef) 
3. See [:material-code-brackets: TrafficTypeType](./literals.md#traffictypetype) 
4. See [:material-code-braces: StartOutboundVoiceContactResponseTypeDef](./type_defs.md#startoutboundvoicecontactresponsetypedef) 


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

### start\_screen\_sharing

Starts screen sharing for a contact.

Type annotations and code completion for `#!python session.create_client("connect").start_screen_sharing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_screen_sharing.html)

```python
# start_screen_sharing method definition

await def start_screen_sharing(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    ClientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# start_screen_sharing method usage example with argument unpacking

kwargs: StartScreenSharingRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
}

parent.start_screen_sharing(**kwargs)
```

1. See [:material-code-braces: StartScreenSharingRequestRequestTypeDef](./type_defs.md#startscreensharingrequestrequesttypedef) 

### start\_task\_contact

Initiates a flow to start a new task contact.

Type annotations and code completion for `#!python session.create_client("connect").start_task_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_task_contact.html)

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
    ScheduledTime: TimestampTypeDef = ...,
    TaskTemplateId: str = ...,
    QuickConnectId: str = ...,
    RelatedContactId: str = ...,
    SegmentAttributes: Mapping[str, SegmentAttributeValueTypeDef] = ...,  # (2)
) -> StartTaskContactResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
2. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) 
3. See [:material-code-braces: StartTaskContactResponseTypeDef](./type_defs.md#starttaskcontactresponsetypedef) 


```python
# start_task_contact method usage example with argument unpacking

kwargs: StartTaskContactRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
}

parent.start_task_contact(**kwargs)
```

1. See [:material-code-braces: StartTaskContactRequestRequestTypeDef](./type_defs.md#starttaskcontactrequestrequesttypedef) 

### start\_web\_rtc\_contact

Places an inbound in-app, web, or video call to a contact, and then initiates
the flow.

Type annotations and code completion for `#!python session.create_client("connect").start_web_rtc_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/start_web_rtc_contact.html)

```python
# start_web_rtc_contact method definition

await def start_web_rtc_contact(
    self,
    *,
    ContactFlowId: str,
    InstanceId: str,
    ParticipantDetails: ParticipantDetailsTypeDef,  # (1)
    Attributes: Mapping[str, str] = ...,
    ClientToken: str = ...,
    AllowedCapabilities: AllowedCapabilitiesTypeDef = ...,  # (2)
    RelatedContactId: str = ...,
    References: Mapping[str, ReferenceTypeDef] = ...,  # (3)
    Description: str = ...,
) -> StartWebRTCContactResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef) 
2. See [:material-code-braces: AllowedCapabilitiesTypeDef](./type_defs.md#allowedcapabilitiestypedef) 
3. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
4. See [:material-code-braces: StartWebRTCContactResponseTypeDef](./type_defs.md#startwebrtccontactresponsetypedef) 


```python
# start_web_rtc_contact method usage example with argument unpacking

kwargs: StartWebRTCContactRequestRequestTypeDef = {  # (1)
    "ContactFlowId": ...,
    "InstanceId": ...,
    "ParticipantDetails": ...,
}

parent.start_web_rtc_contact(**kwargs)
```

1. See [:material-code-braces: StartWebRTCContactRequestRequestTypeDef](./type_defs.md#startwebrtccontactrequestrequesttypedef) 

### stop\_contact

Ends the specified contact.

Type annotations and code completion for `#!python session.create_client("connect").stop_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/stop_contact.html)

```python
# stop_contact method definition

await def stop_contact(
    self,
    *,
    ContactId: str,
    InstanceId: str,
    DisconnectReason: DisconnectReasonTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: DisconnectReasonTypeDef](./type_defs.md#disconnectreasontypedef) 


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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/stop_contact_recording.html)

```python
# stop_contact_recording method definition

await def stop_contact_recording(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
    ContactRecordingType: ContactRecordingTypeType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ContactRecordingTypeType](./literals.md#contactrecordingtypetype) 


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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/stop_contact_streaming.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/submit_contact_evaluation.html)

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

When a contact is being recorded, this API suspends recording whatever is
selected in the flow configuration: call, screen, or both.

Type annotations and code completion for `#!python session.create_client("connect").suspend_contact_recording` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/suspend_contact_recording.html)

```python
# suspend_contact_recording method definition

await def suspend_contact_recording(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    InitialContactId: str,
    ContactRecordingType: ContactRecordingTypeType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ContactRecordingTypeType](./literals.md#contactrecordingtypetype) 


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

### tag\_contact

Adds the specified tags to the contact resource.

Type annotations and code completion for `#!python session.create_client("connect").tag_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/tag_contact.html)

```python
# tag_contact method definition

await def tag_contact(
    self,
    *,
    ContactId: str,
    InstanceId: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_contact method usage example with argument unpacking

kwargs: TagContactRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
    "InstanceId": ...,
    "Tags": ...,
}

parent.tag_contact(**kwargs)
```

1. See [:material-code-braces: TagContactRequestRequestTypeDef](./type_defs.md#tagcontactrequestrequesttypedef) 

### tag\_resource

Adds the specified tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("connect").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/tag_resource.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/transfer_contact.html)

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

### untag\_contact

Removes the specified tags from the contact resource.

Type annotations and code completion for `#!python session.create_client("connect").untag_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/untag_contact.html)

```python
# untag_contact method definition

await def untag_contact(
    self,
    *,
    ContactId: str,
    InstanceId: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_contact method usage example with argument unpacking

kwargs: UntagContactRequestRequestTypeDef = {  # (1)
    "ContactId": ...,
    "InstanceId": ...,
    "TagKeys": ...,
}

parent.untag_contact(**kwargs)
```

1. See [:material-code-braces: UntagContactRequestRequestTypeDef](./type_defs.md#untagcontactrequestrequesttypedef) 

### untag\_resource

Removes the specified tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("connect").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/untag_resource.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_agent_status.html)

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

### update\_authentication\_profile

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_authentication_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_authentication_profile.html)

```python
# update_authentication_profile method definition

await def update_authentication_profile(
    self,
    *,
    AuthenticationProfileId: str,
    InstanceId: str,
    Name: str = ...,
    Description: str = ...,
    AllowedIps: Sequence[str] = ...,
    BlockedIps: Sequence[str] = ...,
    PeriodicSessionDuration: int = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_authentication_profile method usage example with argument unpacking

kwargs: UpdateAuthenticationProfileRequestRequestTypeDef = {  # (1)
    "AuthenticationProfileId": ...,
    "InstanceId": ...,
}

parent.update_authentication_profile(**kwargs)
```

1. See [:material-code-braces: UpdateAuthenticationProfileRequestRequestTypeDef](./type_defs.md#updateauthenticationprofilerequestrequesttypedef) 

### update\_contact

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_contact.html)

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
    SegmentAttributes: Mapping[str, SegmentAttributeValueTypeDef] = ...,  # (2)
    QueueInfo: QueueInfoInputTypeDef = ...,  # (3)
    UserInfo: UserInfoTypeDef = ...,  # (4)
    CustomerEndpoint: EndpointTypeDef = ...,  # (5)
    SystemEndpoint: EndpointTypeDef = ...,  # (5)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
2. See [:material-code-braces: SegmentAttributeValueTypeDef](./type_defs.md#segmentattributevaluetypedef) 
3. See [:material-code-braces: QueueInfoInputTypeDef](./type_defs.md#queueinfoinputtypedef) 
4. See [:material-code-braces: UserInfoTypeDef](./type_defs.md#userinfotypedef) 
5. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
6. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 


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

Creates or updates user-defined contact attributes associated with the
specified contact.

Type annotations and code completion for `#!python session.create_client("connect").update_contact_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_contact_attributes.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_contact_evaluation.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_contact_flow_content.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_contact_flow_metadata.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_contact_flow_module_content.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_contact_flow_module_metadata.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_contact_flow_name.html)

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

### update\_contact\_routing\_data

Updates routing priority and age on the contact (<b>QueuePriority</b> and
<b>QueueTimeAdjustmentInSeconds</b>).

Type annotations and code completion for `#!python session.create_client("connect").update_contact_routing_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_contact_routing_data.html)

```python
# update_contact_routing_data method definition

await def update_contact_routing_data(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    QueueTimeAdjustmentSeconds: int = ...,
    QueuePriority: int = ...,
    RoutingCriteria: RoutingCriteriaInputTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: RoutingCriteriaInputTypeDef](./type_defs.md#routingcriteriainputtypedef) 


```python
# update_contact_routing_data method usage example with argument unpacking

kwargs: UpdateContactRoutingDataRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
}

parent.update_contact_routing_data(**kwargs)
```

1. See [:material-code-braces: UpdateContactRoutingDataRequestRequestTypeDef](./type_defs.md#updatecontactroutingdatarequestrequesttypedef) 

### update\_contact\_schedule

Updates the scheduled time of a task contact that is already scheduled.

Type annotations and code completion for `#!python session.create_client("connect").update_contact_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_contact_schedule.html)

```python
# update_contact_schedule method definition

await def update_contact_schedule(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    ScheduledTime: TimestampTypeDef,
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

### update\_email\_address\_metadata

Updates an email address metadata.

Type annotations and code completion for `#!python session.create_client("connect").update_email_address_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_email_address_metadata.html)

```python
# update_email_address_metadata method definition

await def update_email_address_metadata(
    self,
    *,
    InstanceId: str,
    EmailAddressId: str,
    Description: str = ...,
    DisplayName: str = ...,
    ClientToken: str = ...,
) -> UpdateEmailAddressMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateEmailAddressMetadataResponseTypeDef](./type_defs.md#updateemailaddressmetadataresponsetypedef) 


```python
# update_email_address_metadata method usage example with argument unpacking

kwargs: UpdateEmailAddressMetadataRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "EmailAddressId": ...,
}

parent.update_email_address_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateEmailAddressMetadataRequestRequestTypeDef](./type_defs.md#updateemailaddressmetadatarequestrequesttypedef) 

### update\_evaluation\_form

Updates details about a specific evaluation form version in the specified
Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").update_evaluation_form` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_evaluation_form.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_hours_of_operation.html)

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

### update\_hours\_of\_operation\_override

Update the hours of operation override.

Type annotations and code completion for `#!python session.create_client("connect").update_hours_of_operation_override` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_hours_of_operation_override.html)

```python
# update_hours_of_operation_override method definition

await def update_hours_of_operation_override(
    self,
    *,
    InstanceId: str,
    HoursOfOperationId: str,
    HoursOfOperationOverrideId: str,
    Name: str = ...,
    Description: str = ...,
    Config: Sequence[HoursOfOperationOverrideConfigTypeDef] = ...,  # (1)
    EffectiveFrom: str = ...,
    EffectiveTill: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HoursOfOperationOverrideConfigTypeDef](./type_defs.md#hoursofoperationoverrideconfigtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_hours_of_operation_override method usage example with argument unpacking

kwargs: UpdateHoursOfOperationOverrideRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "HoursOfOperationId": ...,
    "HoursOfOperationOverrideId": ...,
}

parent.update_hours_of_operation_override(**kwargs)
```

1. See [:material-code-braces: UpdateHoursOfOperationOverrideRequestRequestTypeDef](./type_defs.md#updatehoursofoperationoverriderequestrequesttypedef) 

### update\_instance\_attribute

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_instance_attribute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_instance_attribute.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_instance_storage_config.html)

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

Updates timeouts for when human chat participants are to be considered idle,
and when agents are automatically disconnected from a chat due to idleness.

Type annotations and code completion for `#!python session.create_client("connect").update_participant_role_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_participant_role_config.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_phone_number.html)

```python
# update_phone_number method definition

await def update_phone_number(
    self,
    *,
    PhoneNumberId: str,
    TargetArn: str = ...,
    InstanceId: str = ...,
    ClientToken: str = ...,
) -> UpdatePhoneNumberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdatePhoneNumberResponseTypeDef](./type_defs.md#updatephonenumberresponsetypedef) 


```python
# update_phone_number method usage example with argument unpacking

kwargs: UpdatePhoneNumberRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.update_phone_number(**kwargs)
```

1. See [:material-code-braces: UpdatePhoneNumberRequestRequestTypeDef](./type_defs.md#updatephonenumberrequestrequesttypedef) 

### update\_phone\_number\_metadata

Updates a phone number's metadata.

Type annotations and code completion for `#!python session.create_client("connect").update_phone_number_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_phone_number_metadata.html)

```python
# update_phone_number_metadata method definition

await def update_phone_number_metadata(
    self,
    *,
    PhoneNumberId: str,
    PhoneNumberDescription: str = ...,
    ClientToken: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_phone_number_metadata method usage example with argument unpacking

kwargs: UpdatePhoneNumberMetadataRequestRequestTypeDef = {  # (1)
    "PhoneNumberId": ...,
}

parent.update_phone_number_metadata(**kwargs)
```

1. See [:material-code-braces: UpdatePhoneNumberMetadataRequestRequestTypeDef](./type_defs.md#updatephonenumbermetadatarequestrequesttypedef) 

### update\_predefined\_attribute

Updates a predefined attribute for the specified Amazon Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").update_predefined_attribute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_predefined_attribute.html)

```python
# update_predefined_attribute method definition

await def update_predefined_attribute(
    self,
    *,
    InstanceId: str,
    Name: str,
    Values: PredefinedAttributeValuesTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PredefinedAttributeValuesTypeDef](./type_defs.md#predefinedattributevaluestypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_predefined_attribute method usage example with argument unpacking

kwargs: UpdatePredefinedAttributeRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "Name": ...,
}

parent.update_predefined_attribute(**kwargs)
```

1. See [:material-code-braces: UpdatePredefinedAttributeRequestRequestTypeDef](./type_defs.md#updatepredefinedattributerequestrequesttypedef) 

### update\_prompt

Updates a prompt.

Type annotations and code completion for `#!python session.create_client("connect").update_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_prompt.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_queue_hours_of_operation.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_queue_max_contacts.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_queue_name.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_queue_outbound_caller_config.html)

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

### update\_queue\_outbound\_email\_config

Updates the outbound email address Id for a specified queue.

Type annotations and code completion for `#!python session.create_client("connect").update_queue_outbound_email_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_queue_outbound_email_config.html)

```python
# update_queue_outbound_email_config method definition

await def update_queue_outbound_email_config(
    self,
    *,
    InstanceId: str,
    QueueId: str,
    OutboundEmailConfig: OutboundEmailConfigTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OutboundEmailConfigTypeDef](./type_defs.md#outboundemailconfigtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_queue_outbound_email_config method usage example with argument unpacking

kwargs: UpdateQueueOutboundEmailConfigRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "QueueId": ...,
    "OutboundEmailConfig": ...,
}

parent.update_queue_outbound_email_config(**kwargs)
```

1. See [:material-code-braces: UpdateQueueOutboundEmailConfigRequestRequestTypeDef](./type_defs.md#updatequeueoutboundemailconfigrequestrequesttypedef) 

### update\_queue\_status

This API is in preview release for Amazon Connect and is subject to change.

Type annotations and code completion for `#!python session.create_client("connect").update_queue_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_queue_status.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_quick_connect_config.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_quick_connect_name.html)

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
calculated based on <i>time since their last inbound contact</i> or <i>longest
idle time</i>.

Type annotations and code completion for `#!python session.create_client("connect").update_routing_profile_agent_availability_timer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_routing_profile_agent_availability_timer.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_routing_profile_concurrency.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_routing_profile_default_outbound_queue.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_routing_profile_name.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_routing_profile_queues.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_rule.html)

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

Updates a security profile.

Type annotations and code completion for `#!python session.create_client("connect").update_security_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_security_profile.html)

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
    Applications: Sequence[ApplicationTypeDef] = ...,  # (1)
    HierarchyRestrictedResources: Sequence[str] = ...,
    AllowedAccessControlHierarchyGroupId: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_task_template.html)

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
    SelfAssignFlowId: str = ...,
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_traffic_distribution.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_user_hierarchy.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_user_hierarchy_group_name.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_user_hierarchy_structure.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_user_identity_info.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_user_phone_config.html)

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

### update\_user\_proficiencies

Updates the properties associated with the proficiencies of a user.

Type annotations and code completion for `#!python session.create_client("connect").update_user_proficiencies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_user_proficiencies.html)

```python
# update_user_proficiencies method definition

await def update_user_proficiencies(
    self,
    *,
    InstanceId: str,
    UserId: str,
    UserProficiencies: Sequence[UserProficiencyTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UserProficiencyTypeDef](./type_defs.md#userproficiencytypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_user_proficiencies method usage example with argument unpacking

kwargs: UpdateUserProficienciesRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "UserId": ...,
    "UserProficiencies": ...,
}

parent.update_user_proficiencies(**kwargs)
```

1. See [:material-code-braces: UpdateUserProficienciesRequestRequestTypeDef](./type_defs.md#updateuserproficienciesrequestrequesttypedef) 

### update\_user\_routing\_profile

Assigns the specified routing profile to the specified user.

Type annotations and code completion for `#!python session.create_client("connect").update_user_routing_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_user_routing_profile.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_user_security_profiles.html)

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

### update\_view\_content

Updates the view content of the given view identifier in the specified Amazon
Connect instance.

Type annotations and code completion for `#!python session.create_client("connect").update_view_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_view_content.html)

```python
# update_view_content method definition

await def update_view_content(
    self,
    *,
    InstanceId: str,
    ViewId: str,
    Status: ViewStatusType,  # (1)
    Content: ViewInputContentTypeDef,  # (2)
) -> UpdateViewContentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ViewStatusType](./literals.md#viewstatustype) 
2. See [:material-code-braces: ViewInputContentTypeDef](./type_defs.md#viewinputcontenttypedef) 
3. See [:material-code-braces: UpdateViewContentResponseTypeDef](./type_defs.md#updateviewcontentresponsetypedef) 


```python
# update_view_content method usage example with argument unpacking

kwargs: UpdateViewContentRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ViewId": ...,
    "Status": ...,
    "Content": ...,
}

parent.update_view_content(**kwargs)
```

1. See [:material-code-braces: UpdateViewContentRequestRequestTypeDef](./type_defs.md#updateviewcontentrequestrequesttypedef) 

### update\_view\_metadata

Updates the view metadata.

Type annotations and code completion for `#!python session.create_client("connect").update_view_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect/client/update_view_metadata.html)

```python
# update_view_metadata method definition

await def update_view_metadata(
    self,
    *,
    InstanceId: str,
    ViewId: str,
    Name: str = ...,
    Description: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_view_metadata method usage example with argument unpacking

kwargs: UpdateViewMetadataRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ViewId": ...,
}

parent.update_view_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateViewMetadataRequestRequestTypeDef](./type_defs.md#updateviewmetadatarequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("connect").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ConnectClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("connect").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client)

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
- `client.get_paginator("list_authentication_profiles")` -> [ListAuthenticationProfilesPaginator](./paginators.md#listauthenticationprofilespaginator)
- `client.get_paginator("list_bots")` -> [ListBotsPaginator](./paginators.md#listbotspaginator)
- `client.get_paginator("list_contact_evaluations")` -> [ListContactEvaluationsPaginator](./paginators.md#listcontactevaluationspaginator)
- `client.get_paginator("list_contact_flow_modules")` -> [ListContactFlowModulesPaginator](./paginators.md#listcontactflowmodulespaginator)
- `client.get_paginator("list_contact_flow_versions")` -> [ListContactFlowVersionsPaginator](./paginators.md#listcontactflowversionspaginator)
- `client.get_paginator("list_contact_flows")` -> [ListContactFlowsPaginator](./paginators.md#listcontactflowspaginator)
- `client.get_paginator("list_contact_references")` -> [ListContactReferencesPaginator](./paginators.md#listcontactreferencespaginator)
- `client.get_paginator("list_default_vocabularies")` -> [ListDefaultVocabulariesPaginator](./paginators.md#listdefaultvocabulariespaginator)
- `client.get_paginator("list_evaluation_form_versions")` -> [ListEvaluationFormVersionsPaginator](./paginators.md#listevaluationformversionspaginator)
- `client.get_paginator("list_evaluation_forms")` -> [ListEvaluationFormsPaginator](./paginators.md#listevaluationformspaginator)
- `client.get_paginator("list_flow_associations")` -> [ListFlowAssociationsPaginator](./paginators.md#listflowassociationspaginator)
- `client.get_paginator("list_hours_of_operation_overrides")` -> [ListHoursOfOperationOverridesPaginator](./paginators.md#listhoursofoperationoverridespaginator)
- `client.get_paginator("list_hours_of_operations")` -> [ListHoursOfOperationsPaginator](./paginators.md#listhoursofoperationspaginator)
- `client.get_paginator("list_instance_attributes")` -> [ListInstanceAttributesPaginator](./paginators.md#listinstanceattributespaginator)
- `client.get_paginator("list_instance_storage_configs")` -> [ListInstanceStorageConfigsPaginator](./paginators.md#listinstancestorageconfigspaginator)
- `client.get_paginator("list_instances")` -> [ListInstancesPaginator](./paginators.md#listinstancespaginator)
- `client.get_paginator("list_integration_associations")` -> [ListIntegrationAssociationsPaginator](./paginators.md#listintegrationassociationspaginator)
- `client.get_paginator("list_lambda_functions")` -> [ListLambdaFunctionsPaginator](./paginators.md#listlambdafunctionspaginator)
- `client.get_paginator("list_lex_bots")` -> [ListLexBotsPaginator](./paginators.md#listlexbotspaginator)
- `client.get_paginator("list_phone_numbers")` -> [ListPhoneNumbersPaginator](./paginators.md#listphonenumberspaginator)
- `client.get_paginator("list_phone_numbers_v2")` -> [ListPhoneNumbersV2Paginator](./paginators.md#listphonenumbersv2paginator)
- `client.get_paginator("list_predefined_attributes")` -> [ListPredefinedAttributesPaginator](./paginators.md#listpredefinedattributespaginator)
- `client.get_paginator("list_prompts")` -> [ListPromptsPaginator](./paginators.md#listpromptspaginator)
- `client.get_paginator("list_queue_quick_connects")` -> [ListQueueQuickConnectsPaginator](./paginators.md#listqueuequickconnectspaginator)
- `client.get_paginator("list_queues")` -> [ListQueuesPaginator](./paginators.md#listqueuespaginator)
- `client.get_paginator("list_quick_connects")` -> [ListQuickConnectsPaginator](./paginators.md#listquickconnectspaginator)
- `client.get_paginator("list_routing_profile_queues")` -> [ListRoutingProfileQueuesPaginator](./paginators.md#listroutingprofilequeuespaginator)
- `client.get_paginator("list_routing_profiles")` -> [ListRoutingProfilesPaginator](./paginators.md#listroutingprofilespaginator)
- `client.get_paginator("list_rules")` -> [ListRulesPaginator](./paginators.md#listrulespaginator)
- `client.get_paginator("list_security_keys")` -> [ListSecurityKeysPaginator](./paginators.md#listsecuritykeyspaginator)
- `client.get_paginator("list_security_profile_applications")` -> [ListSecurityProfileApplicationsPaginator](./paginators.md#listsecurityprofileapplicationspaginator)
- `client.get_paginator("list_security_profile_permissions")` -> [ListSecurityProfilePermissionsPaginator](./paginators.md#listsecurityprofilepermissionspaginator)
- `client.get_paginator("list_security_profiles")` -> [ListSecurityProfilesPaginator](./paginators.md#listsecurityprofilespaginator)
- `client.get_paginator("list_task_templates")` -> [ListTaskTemplatesPaginator](./paginators.md#listtasktemplatespaginator)
- `client.get_paginator("list_traffic_distribution_group_users")` -> [ListTrafficDistributionGroupUsersPaginator](./paginators.md#listtrafficdistributiongroupuserspaginator)
- `client.get_paginator("list_traffic_distribution_groups")` -> [ListTrafficDistributionGroupsPaginator](./paginators.md#listtrafficdistributiongroupspaginator)
- `client.get_paginator("list_use_cases")` -> [ListUseCasesPaginator](./paginators.md#listusecasespaginator)
- `client.get_paginator("list_user_hierarchy_groups")` -> [ListUserHierarchyGroupsPaginator](./paginators.md#listuserhierarchygroupspaginator)
- `client.get_paginator("list_user_proficiencies")` -> [ListUserProficienciesPaginator](./paginators.md#listuserproficienciespaginator)
- `client.get_paginator("list_users")` -> [ListUsersPaginator](./paginators.md#listuserspaginator)
- `client.get_paginator("list_view_versions")` -> [ListViewVersionsPaginator](./paginators.md#listviewversionspaginator)
- `client.get_paginator("list_views")` -> [ListViewsPaginator](./paginators.md#listviewspaginator)
- `client.get_paginator("search_agent_statuses")` -> [SearchAgentStatusesPaginator](./paginators.md#searchagentstatusespaginator)
- `client.get_paginator("search_available_phone_numbers")` -> [SearchAvailablePhoneNumbersPaginator](./paginators.md#searchavailablephonenumberspaginator)
- `client.get_paginator("search_contact_flow_modules")` -> [SearchContactFlowModulesPaginator](./paginators.md#searchcontactflowmodulespaginator)
- `client.get_paginator("search_contact_flows")` -> [SearchContactFlowsPaginator](./paginators.md#searchcontactflowspaginator)
- `client.get_paginator("search_contacts")` -> [SearchContactsPaginator](./paginators.md#searchcontactspaginator)
- `client.get_paginator("search_hours_of_operation_overrides")` -> [SearchHoursOfOperationOverridesPaginator](./paginators.md#searchhoursofoperationoverridespaginator)
- `client.get_paginator("search_hours_of_operations")` -> [SearchHoursOfOperationsPaginator](./paginators.md#searchhoursofoperationspaginator)
- `client.get_paginator("search_predefined_attributes")` -> [SearchPredefinedAttributesPaginator](./paginators.md#searchpredefinedattributespaginator)
- `client.get_paginator("search_prompts")` -> [SearchPromptsPaginator](./paginators.md#searchpromptspaginator)
- `client.get_paginator("search_queues")` -> [SearchQueuesPaginator](./paginators.md#searchqueuespaginator)
- `client.get_paginator("search_quick_connects")` -> [SearchQuickConnectsPaginator](./paginators.md#searchquickconnectspaginator)
- `client.get_paginator("search_resource_tags")` -> [SearchResourceTagsPaginator](./paginators.md#searchresourcetagspaginator)
- `client.get_paginator("search_routing_profiles")` -> [SearchRoutingProfilesPaginator](./paginators.md#searchroutingprofilespaginator)
- `client.get_paginator("search_security_profiles")` -> [SearchSecurityProfilesPaginator](./paginators.md#searchsecurityprofilespaginator)
- `client.get_paginator("search_user_hierarchy_groups")` -> [SearchUserHierarchyGroupsPaginator](./paginators.md#searchuserhierarchygroupspaginator)
- `client.get_paginator("search_users")` -> [SearchUsersPaginator](./paginators.md#searchuserspaginator)
- `client.get_paginator("search_vocabularies")` -> [SearchVocabulariesPaginator](./paginators.md#searchvocabulariespaginator)



