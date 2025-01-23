# QBusinessClient

> [Index](../README.md) > [QBusiness](./README.md) > QBusinessClient

!!! note ""

    Auto-generated documentation for [QBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#qbusiness)
    type annotations stubs module [types-aiobotocore-qbusiness](https://pypi.org/project/types-aiobotocore-qbusiness/).

## QBusinessClient

Type annotations and code completion for `#!python session.create_client("qbusiness")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client)

```python
# QBusinessClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_qbusiness.client import QBusinessClient

session = get_session()
async with session.create_client("qbusiness") as client:
    client: QBusinessClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("qbusiness").exceptions` structure.

```python
# QBusinessClient.exceptions usage example

async with session.create_client("qbusiness") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.ExternalResourceException,
        client.InternalServerException,
        client.LicenseNotFoundException,
        client.MediaTooLargeException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# QBusinessClient usage type checking example

from types_aiobotocore_qbusiness.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("qbusiness").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("qbusiness").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/generate_presigned_url.html)

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


### associate\_permission

Adds or updates a permission policy for a Q Business application, allowing
cross-account access for an ISV.

Type annotations and code completion for `#!python session.create_client("qbusiness").associate_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/associate_permission.html)

```python
# associate_permission method definition

await def associate_permission(
    self,
    *,
    applicationId: str,
    statementId: str,
    actions: Sequence[str],
    principal: str,
) -> AssociatePermissionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociatePermissionResponseTypeDef](./type_defs.md#associatepermissionresponsetypedef) 


```python
# associate_permission method usage example with argument unpacking

kwargs: AssociatePermissionRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "statementId": ...,
    "actions": ...,
    "principal": ...,
}

parent.associate_permission(**kwargs)
```

1. See [:material-code-braces: AssociatePermissionRequestRequestTypeDef](./type_defs.md#associatepermissionrequestrequesttypedef) 

### batch\_delete\_document

Asynchronously deletes one or more documents added using the
<code>BatchPutDocument</code> API from an Amazon Q Business index.

Type annotations and code completion for `#!python session.create_client("qbusiness").batch_delete_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/batch_delete_document.html)

```python
# batch_delete_document method definition

await def batch_delete_document(
    self,
    *,
    applicationId: str,
    indexId: str,
    documents: Sequence[DeleteDocumentTypeDef],  # (1)
    dataSourceSyncId: str = ...,
) -> BatchDeleteDocumentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeleteDocumentTypeDef](./type_defs.md#deletedocumenttypedef) 
2. See [:material-code-braces: BatchDeleteDocumentResponseTypeDef](./type_defs.md#batchdeletedocumentresponsetypedef) 


```python
# batch_delete_document method usage example with argument unpacking

kwargs: BatchDeleteDocumentRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "documents": ...,
}

parent.batch_delete_document(**kwargs)
```

1. See [:material-code-braces: BatchDeleteDocumentRequestRequestTypeDef](./type_defs.md#batchdeletedocumentrequestrequesttypedef) 

### batch\_put\_document

Adds one or more documents to an Amazon Q Business index.

Type annotations and code completion for `#!python session.create_client("qbusiness").batch_put_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/batch_put_document.html)

```python
# batch_put_document method definition

await def batch_put_document(
    self,
    *,
    applicationId: str,
    indexId: str,
    documents: Sequence[DocumentTypeDef],  # (1)
    roleArn: str = ...,
    dataSourceSyncId: str = ...,
) -> BatchPutDocumentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: BatchPutDocumentResponseTypeDef](./type_defs.md#batchputdocumentresponsetypedef) 


```python
# batch_put_document method usage example with argument unpacking

kwargs: BatchPutDocumentRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "documents": ...,
}

parent.batch_put_document(**kwargs)
```

1. See [:material-code-braces: BatchPutDocumentRequestRequestTypeDef](./type_defs.md#batchputdocumentrequestrequesttypedef) 

### chat

Starts or continues a streaming Amazon Q Business conversation.

Type annotations and code completion for `#!python session.create_client("qbusiness").chat` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/chat.html)

```python
# chat method definition

await def chat(
    self,
    *,
    applicationId: str,
    userId: str = ...,
    userGroups: Sequence[str] = ...,
    conversationId: str = ...,
    parentMessageId: str = ...,
    clientToken: str = ...,
    inputStream: AioEventStream[ChatInputStreamTypeDef] = ...,  # (1)
) -> ChatOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ChatInputStreamTypeDef](./type_defs.md#chatinputstreamtypedef) 
2. See [:material-code-braces: ChatOutputTypeDef](./type_defs.md#chatoutputtypedef) 


```python
# chat method usage example with argument unpacking

kwargs: ChatInputRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.chat(**kwargs)
```

1. See [:material-code-braces: ChatInputRequestTypeDef](./type_defs.md#chatinputrequesttypedef) 

### chat\_sync

Starts or continues a non-streaming Amazon Q Business conversation.

Type annotations and code completion for `#!python session.create_client("qbusiness").chat_sync` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/chat_sync.html)

```python
# chat_sync method definition

await def chat_sync(
    self,
    *,
    applicationId: str,
    userId: str = ...,
    userGroups: Sequence[str] = ...,
    userMessage: str = ...,
    attachments: Sequence[AttachmentInputTypeDef] = ...,  # (1)
    actionExecution: ActionExecutionTypeDef = ...,  # (2)
    authChallengeResponse: AuthChallengeResponseTypeDef = ...,  # (3)
    conversationId: str = ...,
    parentMessageId: str = ...,
    attributeFilter: AttributeFilterTypeDef = ...,  # (4)
    chatMode: ChatModeType = ...,  # (5)
    chatModeConfiguration: ChatModeConfigurationTypeDef = ...,  # (6)
    clientToken: str = ...,
) -> ChatSyncOutputTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: AttachmentInputTypeDef](./type_defs.md#attachmentinputtypedef) 
2. See [:material-code-braces: ActionExecutionTypeDef](./type_defs.md#actionexecutiontypedef) 
3. See [:material-code-braces: AuthChallengeResponseTypeDef](./type_defs.md#authchallengeresponsetypedef) 
4. See [:material-code-braces: AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef) 
5. See [:material-code-brackets: ChatModeType](./literals.md#chatmodetype) 
6. See [:material-code-braces: ChatModeConfigurationTypeDef](./type_defs.md#chatmodeconfigurationtypedef) 
7. See [:material-code-braces: ChatSyncOutputTypeDef](./type_defs.md#chatsyncoutputtypedef) 


```python
# chat_sync method usage example with argument unpacking

kwargs: ChatSyncInputRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.chat_sync(**kwargs)
```

1. See [:material-code-braces: ChatSyncInputRequestTypeDef](./type_defs.md#chatsyncinputrequesttypedef) 

### create\_application

Creates an Amazon Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/create_application.html)

```python
# create_application method definition

await def create_application(
    self,
    *,
    displayName: str,
    roleArn: str = ...,
    identityType: IdentityTypeType = ...,  # (1)
    iamIdentityProviderArn: str = ...,
    identityCenterInstanceArn: str = ...,
    clientIdsForOIDC: Sequence[str] = ...,
    description: str = ...,
    encryptionConfiguration: EncryptionConfigurationTypeDef = ...,  # (2)
    tags: Sequence[TagTypeDef] = ...,  # (3)
    clientToken: str = ...,
    attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,  # (4)
    qAppsConfiguration: QAppsConfigurationTypeDef = ...,  # (5)
    personalizationConfiguration: PersonalizationConfigurationTypeDef = ...,  # (6)
    quickSightConfiguration: QuickSightConfigurationTypeDef = ...,  # (7)
) -> CreateApplicationResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: AttachmentsConfigurationTypeDef](./type_defs.md#attachmentsconfigurationtypedef) 
5. See [:material-code-braces: QAppsConfigurationTypeDef](./type_defs.md#qappsconfigurationtypedef) 
6. See [:material-code-braces: PersonalizationConfigurationTypeDef](./type_defs.md#personalizationconfigurationtypedef) 
7. See [:material-code-braces: QuickSightConfigurationTypeDef](./type_defs.md#quicksightconfigurationtypedef) 
8. See [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 


```python
# create_application method usage example with argument unpacking

kwargs: CreateApplicationRequestRequestTypeDef = {  # (1)
    "displayName": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef) 

### create\_data\_accessor

Creates a new data accessor for an ISV to access data from a Q Business
application.

Type annotations and code completion for `#!python session.create_client("qbusiness").create_data_accessor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/create_data_accessor.html)

```python
# create_data_accessor method definition

await def create_data_accessor(
    self,
    *,
    applicationId: str,
    principal: str,
    actionConfigurations: Sequence[ActionConfigurationUnionTypeDef],  # (1)
    displayName: str,
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateDataAccessorResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ActionConfigurationTypeDef](./type_defs.md#actionconfigurationtypedef) [:material-code-braces: ActionConfigurationOutputTypeDef](./type_defs.md#actionconfigurationoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDataAccessorResponseTypeDef](./type_defs.md#createdataaccessorresponsetypedef) 


```python
# create_data_accessor method usage example with argument unpacking

kwargs: CreateDataAccessorRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "principal": ...,
    "actionConfigurations": ...,
    "displayName": ...,
}

parent.create_data_accessor(**kwargs)
```

1. See [:material-code-braces: CreateDataAccessorRequestRequestTypeDef](./type_defs.md#createdataaccessorrequestrequesttypedef) 

### create\_data\_source

Creates a data source connector for an Amazon Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").create_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/create_data_source.html)

```python
# create_data_source method definition

await def create_data_source(
    self,
    *,
    applicationId: str,
    indexId: str,
    displayName: str,
    configuration: Mapping[str, Any],
    vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,  # (1)
    description: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
    syncSchedule: str = ...,
    roleArn: str = ...,
    clientToken: str = ...,
    documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,  # (3)
    mediaExtractionConfiguration: MediaExtractionConfigurationTypeDef = ...,  # (4)
) -> CreateDataSourceResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef) 
4. See [:material-code-braces: MediaExtractionConfigurationTypeDef](./type_defs.md#mediaextractionconfigurationtypedef) 
5. See [:material-code-braces: CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef) 


```python
# create_data_source method usage example with argument unpacking

kwargs: CreateDataSourceRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "displayName": ...,
    "configuration": ...,
}

parent.create_data_source(**kwargs)
```

1. See [:material-code-braces: CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef) 

### create\_index

Creates an Amazon Q Business index.

Type annotations and code completion for `#!python session.create_client("qbusiness").create_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/create_index.html)

```python
# create_index method definition

await def create_index(
    self,
    *,
    applicationId: str,
    displayName: str,
    description: str = ...,
    type: IndexTypeType = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
    capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,  # (3)
    clientToken: str = ...,
) -> CreateIndexResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: IndexTypeType](./literals.md#indextypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef) 
4. See [:material-code-braces: CreateIndexResponseTypeDef](./type_defs.md#createindexresponsetypedef) 


```python
# create_index method usage example with argument unpacking

kwargs: CreateIndexRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "displayName": ...,
}

parent.create_index(**kwargs)
```

1. See [:material-code-braces: CreateIndexRequestRequestTypeDef](./type_defs.md#createindexrequestrequesttypedef) 

### create\_plugin

Creates an Amazon Q Business plugin.

Type annotations and code completion for `#!python session.create_client("qbusiness").create_plugin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/create_plugin.html)

```python
# create_plugin method definition

await def create_plugin(
    self,
    *,
    applicationId: str,
    displayName: str,
    type: PluginTypeType,  # (1)
    authConfiguration: PluginAuthConfigurationTypeDef,  # (2)
    serverUrl: str = ...,
    customPluginConfiguration: CustomPluginConfigurationTypeDef = ...,  # (3)
    tags: Sequence[TagTypeDef] = ...,  # (4)
    clientToken: str = ...,
) -> CreatePluginResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
2. See [:material-code-braces: PluginAuthConfigurationTypeDef](./type_defs.md#pluginauthconfigurationtypedef) 
3. See [:material-code-braces: CustomPluginConfigurationTypeDef](./type_defs.md#custompluginconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreatePluginResponseTypeDef](./type_defs.md#createpluginresponsetypedef) 


```python
# create_plugin method usage example with argument unpacking

kwargs: CreatePluginRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "displayName": ...,
    "type": ...,
    "authConfiguration": ...,
}

parent.create_plugin(**kwargs)
```

1. See [:material-code-braces: CreatePluginRequestRequestTypeDef](./type_defs.md#createpluginrequestrequesttypedef) 

### create\_retriever

Adds a retriever to your Amazon Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").create_retriever` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/create_retriever.html)

```python
# create_retriever method definition

await def create_retriever(
    self,
    *,
    applicationId: str,
    type: RetrieverTypeType,  # (1)
    displayName: str,
    configuration: RetrieverConfigurationTypeDef,  # (2)
    roleArn: str = ...,
    clientToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateRetrieverResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: RetrieverTypeType](./literals.md#retrievertypetype) 
2. See [:material-code-braces: RetrieverConfigurationTypeDef](./type_defs.md#retrieverconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateRetrieverResponseTypeDef](./type_defs.md#createretrieverresponsetypedef) 


```python
# create_retriever method usage example with argument unpacking

kwargs: CreateRetrieverRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "type": ...,
    "displayName": ...,
    "configuration": ...,
}

parent.create_retriever(**kwargs)
```

1. See [:material-code-braces: CreateRetrieverRequestRequestTypeDef](./type_defs.md#createretrieverrequestrequesttypedef) 

### create\_user

Creates a universally unique identifier (UUID) mapped to a list of local user
ids within an application.

Type annotations and code completion for `#!python session.create_client("qbusiness").create_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/create_user.html)

```python
# create_user method definition

await def create_user(
    self,
    *,
    applicationId: str,
    userId: str,
    userAliases: Sequence[UserAliasTypeDef] = ...,  # (1)
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 


```python
# create_user method usage example with argument unpacking

kwargs: CreateUserRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "userId": ...,
}

parent.create_user(**kwargs)
```

1. See [:material-code-braces: CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef) 

### create\_web\_experience

Creates an Amazon Q Business web experience.

Type annotations and code completion for `#!python session.create_client("qbusiness").create_web_experience` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/create_web_experience.html)

```python
# create_web_experience method definition

await def create_web_experience(
    self,
    *,
    applicationId: str,
    title: str = ...,
    subtitle: str = ...,
    welcomeMessage: str = ...,
    samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,  # (1)
    origins: Sequence[str] = ...,
    roleArn: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
    clientToken: str = ...,
    identityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...,  # (3)
    browserExtensionConfiguration: BrowserExtensionConfigurationTypeDef = ...,  # (4)
    customizationConfiguration: CustomizationConfigurationTypeDef = ...,  # (5)
) -> CreateWebExperienceResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: WebExperienceSamplePromptsControlModeType](./literals.md#webexperiencesamplepromptscontrolmodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: IdentityProviderConfigurationTypeDef](./type_defs.md#identityproviderconfigurationtypedef) 
4. See [:material-code-braces: BrowserExtensionConfigurationTypeDef](./type_defs.md#browserextensionconfigurationtypedef) 
5. See [:material-code-braces: CustomizationConfigurationTypeDef](./type_defs.md#customizationconfigurationtypedef) 
6. See [:material-code-braces: CreateWebExperienceResponseTypeDef](./type_defs.md#createwebexperienceresponsetypedef) 


```python
# create_web_experience method usage example with argument unpacking

kwargs: CreateWebExperienceRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.create_web_experience(**kwargs)
```

1. See [:material-code-braces: CreateWebExperienceRequestRequestTypeDef](./type_defs.md#createwebexperiencerequestrequesttypedef) 

### delete\_application

Deletes an Amazon Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_application.html)

```python
# delete_application method definition

await def delete_application(
    self,
    *,
    applicationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_application method usage example with argument unpacking

kwargs: DeleteApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef) 

### delete\_chat\_controls\_configuration

Deletes chat controls configured for an existing Amazon Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_chat_controls_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_chat_controls_configuration.html)

```python
# delete_chat_controls_configuration method definition

await def delete_chat_controls_configuration(
    self,
    *,
    applicationId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_chat_controls_configuration method usage example with argument unpacking

kwargs: DeleteChatControlsConfigurationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.delete_chat_controls_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteChatControlsConfigurationRequestRequestTypeDef](./type_defs.md#deletechatcontrolsconfigurationrequestrequesttypedef) 

### delete\_conversation

Deletes an Amazon Q Business web experience conversation.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_conversation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_conversation.html)

```python
# delete_conversation method definition

await def delete_conversation(
    self,
    *,
    conversationId: str,
    applicationId: str,
    userId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_conversation method usage example with argument unpacking

kwargs: DeleteConversationRequestRequestTypeDef = {  # (1)
    "conversationId": ...,
    "applicationId": ...,
}

parent.delete_conversation(**kwargs)
```

1. See [:material-code-braces: DeleteConversationRequestRequestTypeDef](./type_defs.md#deleteconversationrequestrequesttypedef) 

### delete\_data\_accessor

Deletes a specified data accessor.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_data_accessor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_data_accessor.html)

```python
# delete_data_accessor method definition

await def delete_data_accessor(
    self,
    *,
    applicationId: str,
    dataAccessorId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_data_accessor method usage example with argument unpacking

kwargs: DeleteDataAccessorRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "dataAccessorId": ...,
}

parent.delete_data_accessor(**kwargs)
```

1. See [:material-code-braces: DeleteDataAccessorRequestRequestTypeDef](./type_defs.md#deletedataaccessorrequestrequesttypedef) 

### delete\_data\_source

Deletes an Amazon Q Business data source connector.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_data_source.html)

```python
# delete_data_source method definition

await def delete_data_source(
    self,
    *,
    applicationId: str,
    indexId: str,
    dataSourceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_data_source method usage example with argument unpacking

kwargs: DeleteDataSourceRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "dataSourceId": ...,
}

parent.delete_data_source(**kwargs)
```

1. See [:material-code-braces: DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef) 

### delete\_group

Deletes a group so that all users and sub groups that belong to the group can
no longer access documents only available to that group.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_group.html)

```python
# delete_group method definition

await def delete_group(
    self,
    *,
    applicationId: str,
    indexId: str,
    groupName: str,
    dataSourceId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_group method usage example with argument unpacking

kwargs: DeleteGroupRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "groupName": ...,
}

parent.delete_group(**kwargs)
```

1. See [:material-code-braces: DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef) 

### delete\_index

Deletes an Amazon Q Business index.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_index.html)

```python
# delete_index method definition

await def delete_index(
    self,
    *,
    applicationId: str,
    indexId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_index method usage example with argument unpacking

kwargs: DeleteIndexRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
}

parent.delete_index(**kwargs)
```

1. See [:material-code-braces: DeleteIndexRequestRequestTypeDef](./type_defs.md#deleteindexrequestrequesttypedef) 

### delete\_plugin

Deletes an Amazon Q Business plugin.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_plugin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_plugin.html)

```python
# delete_plugin method definition

await def delete_plugin(
    self,
    *,
    applicationId: str,
    pluginId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_plugin method usage example with argument unpacking

kwargs: DeletePluginRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "pluginId": ...,
}

parent.delete_plugin(**kwargs)
```

1. See [:material-code-braces: DeletePluginRequestRequestTypeDef](./type_defs.md#deletepluginrequestrequesttypedef) 

### delete\_retriever

Deletes the retriever used by an Amazon Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_retriever` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_retriever.html)

```python
# delete_retriever method definition

await def delete_retriever(
    self,
    *,
    applicationId: str,
    retrieverId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_retriever method usage example with argument unpacking

kwargs: DeleteRetrieverRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "retrieverId": ...,
}

parent.delete_retriever(**kwargs)
```

1. See [:material-code-braces: DeleteRetrieverRequestRequestTypeDef](./type_defs.md#deleteretrieverrequestrequesttypedef) 

### delete\_user

Deletes a user by email id.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_user.html)

```python
# delete_user method definition

await def delete_user(
    self,
    *,
    applicationId: str,
    userId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_user method usage example with argument unpacking

kwargs: DeleteUserRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "userId": ...,
}

parent.delete_user(**kwargs)
```

1. See [:material-code-braces: DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef) 

### delete\_web\_experience

Deletes an Amazon Q Business web experience.

Type annotations and code completion for `#!python session.create_client("qbusiness").delete_web_experience` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/delete_web_experience.html)

```python
# delete_web_experience method definition

await def delete_web_experience(
    self,
    *,
    applicationId: str,
    webExperienceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_web_experience method usage example with argument unpacking

kwargs: DeleteWebExperienceRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "webExperienceId": ...,
}

parent.delete_web_experience(**kwargs)
```

1. See [:material-code-braces: DeleteWebExperienceRequestRequestTypeDef](./type_defs.md#deletewebexperiencerequestrequesttypedef) 

### disassociate\_permission

Removes a permission policy from a Q Business application, revoking the
cross-account access that was previously granted to an ISV.

Type annotations and code completion for `#!python session.create_client("qbusiness").disassociate_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/disassociate_permission.html)

```python
# disassociate_permission method definition

await def disassociate_permission(
    self,
    *,
    applicationId: str,
    statementId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_permission method usage example with argument unpacking

kwargs: DisassociatePermissionRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "statementId": ...,
}

parent.disassociate_permission(**kwargs)
```

1. See [:material-code-braces: DisassociatePermissionRequestRequestTypeDef](./type_defs.md#disassociatepermissionrequestrequesttypedef) 

### get\_application

Gets information about an existing Amazon Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_application.html)

```python
# get_application method definition

await def get_application(
    self,
    *,
    applicationId: str,
) -> GetApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApplicationResponseTypeDef](./type_defs.md#getapplicationresponsetypedef) 


```python
# get_application method usage example with argument unpacking

kwargs: GetApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.get_application(**kwargs)
```

1. See [:material-code-braces: GetApplicationRequestRequestTypeDef](./type_defs.md#getapplicationrequestrequesttypedef) 

### get\_chat\_controls\_configuration

Gets information about an chat controls configured for an existing Amazon Q
Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_chat_controls_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_chat_controls_configuration.html)

```python
# get_chat_controls_configuration method definition

await def get_chat_controls_configuration(
    self,
    *,
    applicationId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> GetChatControlsConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetChatControlsConfigurationResponseTypeDef](./type_defs.md#getchatcontrolsconfigurationresponsetypedef) 


```python
# get_chat_controls_configuration method usage example with argument unpacking

kwargs: GetChatControlsConfigurationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.get_chat_controls_configuration(**kwargs)
```

1. See [:material-code-braces: GetChatControlsConfigurationRequestRequestTypeDef](./type_defs.md#getchatcontrolsconfigurationrequestrequesttypedef) 

### get\_data\_accessor

Retrieves information about a specified data accessor.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_data_accessor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_data_accessor.html)

```python
# get_data_accessor method definition

await def get_data_accessor(
    self,
    *,
    applicationId: str,
    dataAccessorId: str,
) -> GetDataAccessorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataAccessorResponseTypeDef](./type_defs.md#getdataaccessorresponsetypedef) 


```python
# get_data_accessor method usage example with argument unpacking

kwargs: GetDataAccessorRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "dataAccessorId": ...,
}

parent.get_data_accessor(**kwargs)
```

1. See [:material-code-braces: GetDataAccessorRequestRequestTypeDef](./type_defs.md#getdataaccessorrequestrequesttypedef) 

### get\_data\_source

Gets information about an existing Amazon Q Business data source connector.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_data_source.html)

```python
# get_data_source method definition

await def get_data_source(
    self,
    *,
    applicationId: str,
    indexId: str,
    dataSourceId: str,
) -> GetDataSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef) 


```python
# get_data_source method usage example with argument unpacking

kwargs: GetDataSourceRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "dataSourceId": ...,
}

parent.get_data_source(**kwargs)
```

1. See [:material-code-braces: GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef) 

### get\_group

Describes a group by group name.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_group.html)

```python
# get_group method definition

await def get_group(
    self,
    *,
    applicationId: str,
    indexId: str,
    groupName: str,
    dataSourceId: str = ...,
) -> GetGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGroupResponseTypeDef](./type_defs.md#getgroupresponsetypedef) 


```python
# get_group method usage example with argument unpacking

kwargs: GetGroupRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "groupName": ...,
}

parent.get_group(**kwargs)
```

1. See [:material-code-braces: GetGroupRequestRequestTypeDef](./type_defs.md#getgrouprequestrequesttypedef) 

### get\_index

Gets information about an existing Amazon Q Business index.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_index.html)

```python
# get_index method definition

await def get_index(
    self,
    *,
    applicationId: str,
    indexId: str,
) -> GetIndexResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIndexResponseTypeDef](./type_defs.md#getindexresponsetypedef) 


```python
# get_index method usage example with argument unpacking

kwargs: GetIndexRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
}

parent.get_index(**kwargs)
```

1. See [:material-code-braces: GetIndexRequestRequestTypeDef](./type_defs.md#getindexrequestrequesttypedef) 

### get\_media

Returns the image bytes corresponding to a media object.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_media` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_media.html)

```python
# get_media method definition

await def get_media(
    self,
    *,
    applicationId: str,
    conversationId: str,
    messageId: str,
    mediaId: str,
) -> GetMediaResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMediaResponseTypeDef](./type_defs.md#getmediaresponsetypedef) 


```python
# get_media method usage example with argument unpacking

kwargs: GetMediaRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "conversationId": ...,
    "messageId": ...,
    "mediaId": ...,
}

parent.get_media(**kwargs)
```

1. See [:material-code-braces: GetMediaRequestRequestTypeDef](./type_defs.md#getmediarequestrequesttypedef) 

### get\_plugin

Gets information about an existing Amazon Q Business plugin.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_plugin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_plugin.html)

```python
# get_plugin method definition

await def get_plugin(
    self,
    *,
    applicationId: str,
    pluginId: str,
) -> GetPluginResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPluginResponseTypeDef](./type_defs.md#getpluginresponsetypedef) 


```python
# get_plugin method usage example with argument unpacking

kwargs: GetPluginRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "pluginId": ...,
}

parent.get_plugin(**kwargs)
```

1. See [:material-code-braces: GetPluginRequestRequestTypeDef](./type_defs.md#getpluginrequestrequesttypedef) 

### get\_policy

Retrieves the current permission policy for a Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_policy.html)

```python
# get_policy method definition

await def get_policy(
    self,
    *,
    applicationId: str,
) -> GetPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef) 


```python
# get_policy method usage example with argument unpacking

kwargs: GetPolicyRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.get_policy(**kwargs)
```

1. See [:material-code-braces: GetPolicyRequestRequestTypeDef](./type_defs.md#getpolicyrequestrequesttypedef) 

### get\_retriever

Gets information about an existing retriever used by an Amazon Q Business
application.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_retriever` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_retriever.html)

```python
# get_retriever method definition

await def get_retriever(
    self,
    *,
    applicationId: str,
    retrieverId: str,
) -> GetRetrieverResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRetrieverResponseTypeDef](./type_defs.md#getretrieverresponsetypedef) 


```python
# get_retriever method usage example with argument unpacking

kwargs: GetRetrieverRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "retrieverId": ...,
}

parent.get_retriever(**kwargs)
```

1. See [:material-code-braces: GetRetrieverRequestRequestTypeDef](./type_defs.md#getretrieverrequestrequesttypedef) 

### get\_user

Describes the universally unique identifier (UUID) associated with a local user
in a data source.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_user.html)

```python
# get_user method definition

await def get_user(
    self,
    *,
    applicationId: str,
    userId: str,
) -> GetUserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUserResponseTypeDef](./type_defs.md#getuserresponsetypedef) 


```python
# get_user method usage example with argument unpacking

kwargs: GetUserRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "userId": ...,
}

parent.get_user(**kwargs)
```

1. See [:material-code-braces: GetUserRequestRequestTypeDef](./type_defs.md#getuserrequestrequesttypedef) 

### get\_web\_experience

Gets information about an existing Amazon Q Business web experience.

Type annotations and code completion for `#!python session.create_client("qbusiness").get_web_experience` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/get_web_experience.html)

```python
# get_web_experience method definition

await def get_web_experience(
    self,
    *,
    applicationId: str,
    webExperienceId: str,
) -> GetWebExperienceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWebExperienceResponseTypeDef](./type_defs.md#getwebexperienceresponsetypedef) 


```python
# get_web_experience method usage example with argument unpacking

kwargs: GetWebExperienceRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "webExperienceId": ...,
}

parent.get_web_experience(**kwargs)
```

1. See [:material-code-braces: GetWebExperienceRequestRequestTypeDef](./type_defs.md#getwebexperiencerequestrequesttypedef) 

### list\_applications

Lists Amazon Q Business applications.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_applications.html)

```python
# list_applications method definition

await def list_applications(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListApplicationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python
# list_applications method usage example with argument unpacking

kwargs: ListApplicationsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef) 

### list\_attachments

Gets a list of attachments associated with an Amazon Q Business web experience
or a list of attachements associated with a specific Amazon Q Business
conversation.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_attachments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_attachments.html)

```python
# list_attachments method definition

await def list_attachments(
    self,
    *,
    applicationId: str,
    conversationId: str = ...,
    userId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAttachmentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAttachmentsResponseTypeDef](./type_defs.md#listattachmentsresponsetypedef) 


```python
# list_attachments method usage example with argument unpacking

kwargs: ListAttachmentsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_attachments(**kwargs)
```

1. See [:material-code-braces: ListAttachmentsRequestRequestTypeDef](./type_defs.md#listattachmentsrequestrequesttypedef) 

### list\_conversations

Lists one or more Amazon Q Business conversations.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_conversations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_conversations.html)

```python
# list_conversations method definition

await def list_conversations(
    self,
    *,
    applicationId: str,
    userId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListConversationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConversationsResponseTypeDef](./type_defs.md#listconversationsresponsetypedef) 


```python
# list_conversations method usage example with argument unpacking

kwargs: ListConversationsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_conversations(**kwargs)
```

1. See [:material-code-braces: ListConversationsRequestRequestTypeDef](./type_defs.md#listconversationsrequestrequesttypedef) 

### list\_data\_accessors

Lists the data accessors for a Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_data_accessors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_data_accessors.html)

```python
# list_data_accessors method definition

await def list_data_accessors(
    self,
    *,
    applicationId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDataAccessorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataAccessorsResponseTypeDef](./type_defs.md#listdataaccessorsresponsetypedef) 


```python
# list_data_accessors method usage example with argument unpacking

kwargs: ListDataAccessorsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_data_accessors(**kwargs)
```

1. See [:material-code-braces: ListDataAccessorsRequestRequestTypeDef](./type_defs.md#listdataaccessorsrequestrequesttypedef) 

### list\_data\_source\_sync\_jobs

Get information about an Amazon Q Business data source connector
synchronization.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_data_source_sync_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_data_source_sync_jobs.html)

```python
# list_data_source_sync_jobs method definition

await def list_data_source_sync_jobs(
    self,
    *,
    dataSourceId: str,
    applicationId: str,
    indexId: str,
    nextToken: str = ...,
    maxResults: int = ...,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    statusFilter: DataSourceSyncJobStatusType = ...,  # (1)
) -> ListDataSourceSyncJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype) 
2. See [:material-code-braces: ListDataSourceSyncJobsResponseTypeDef](./type_defs.md#listdatasourcesyncjobsresponsetypedef) 


```python
# list_data_source_sync_jobs method usage example with argument unpacking

kwargs: ListDataSourceSyncJobsRequestRequestTypeDef = {  # (1)
    "dataSourceId": ...,
    "applicationId": ...,
    "indexId": ...,
}

parent.list_data_source_sync_jobs(**kwargs)
```

1. See [:material-code-braces: ListDataSourceSyncJobsRequestRequestTypeDef](./type_defs.md#listdatasourcesyncjobsrequestrequesttypedef) 

### list\_data\_sources

Lists the Amazon Q Business data source connectors that you have created.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_data_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_data_sources.html)

```python
# list_data_sources method definition

await def list_data_sources(
    self,
    *,
    applicationId: str,
    indexId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDataSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


```python
# list_data_sources method usage example with argument unpacking

kwargs: ListDataSourcesRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
}

parent.list_data_sources(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef) 

### list\_documents

A list of documents attached to an index.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_documents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_documents.html)

```python
# list_documents method definition

await def list_documents(
    self,
    *,
    applicationId: str,
    indexId: str,
    dataSourceIds: Sequence[str] = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDocumentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDocumentsResponseTypeDef](./type_defs.md#listdocumentsresponsetypedef) 


```python
# list_documents method usage example with argument unpacking

kwargs: ListDocumentsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
}

parent.list_documents(**kwargs)
```

1. See [:material-code-braces: ListDocumentsRequestRequestTypeDef](./type_defs.md#listdocumentsrequestrequesttypedef) 

### list\_groups

Provides a list of groups that are mapped to users.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_groups.html)

```python
# list_groups method definition

await def list_groups(
    self,
    *,
    applicationId: str,
    indexId: str,
    updatedEarlierThan: TimestampTypeDef,
    dataSourceId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef) 


```python
# list_groups method usage example with argument unpacking

kwargs: ListGroupsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "updatedEarlierThan": ...,
}

parent.list_groups(**kwargs)
```

1. See [:material-code-braces: ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef) 

### list\_indices

Lists the Amazon Q Business indices you have created.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_indices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_indices.html)

```python
# list_indices method definition

await def list_indices(
    self,
    *,
    applicationId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListIndicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListIndicesResponseTypeDef](./type_defs.md#listindicesresponsetypedef) 


```python
# list_indices method usage example with argument unpacking

kwargs: ListIndicesRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_indices(**kwargs)
```

1. See [:material-code-braces: ListIndicesRequestRequestTypeDef](./type_defs.md#listindicesrequestrequesttypedef) 

### list\_messages

Gets a list of messages associated with an Amazon Q Business web experience.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_messages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_messages.html)

```python
# list_messages method definition

await def list_messages(
    self,
    *,
    conversationId: str,
    applicationId: str,
    userId: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListMessagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMessagesResponseTypeDef](./type_defs.md#listmessagesresponsetypedef) 


```python
# list_messages method usage example with argument unpacking

kwargs: ListMessagesRequestRequestTypeDef = {  # (1)
    "conversationId": ...,
    "applicationId": ...,
}

parent.list_messages(**kwargs)
```

1. See [:material-code-braces: ListMessagesRequestRequestTypeDef](./type_defs.md#listmessagesrequestrequesttypedef) 

### list\_plugin\_actions

Lists configured Amazon Q Business actions for a specific plugin in an Amazon Q
Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_plugin_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_plugin_actions.html)

```python
# list_plugin_actions method definition

await def list_plugin_actions(
    self,
    *,
    applicationId: str,
    pluginId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPluginActionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPluginActionsResponseTypeDef](./type_defs.md#listpluginactionsresponsetypedef) 


```python
# list_plugin_actions method usage example with argument unpacking

kwargs: ListPluginActionsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "pluginId": ...,
}

parent.list_plugin_actions(**kwargs)
```

1. See [:material-code-braces: ListPluginActionsRequestRequestTypeDef](./type_defs.md#listpluginactionsrequestrequesttypedef) 

### list\_plugin\_type\_actions

Lists configured Amazon Q Business actions for any plugin type—both built-in
and custom.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_plugin_type_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_plugin_type_actions.html)

```python
# list_plugin_type_actions method definition

await def list_plugin_type_actions(
    self,
    *,
    pluginType: PluginTypeType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPluginTypeActionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PluginTypeType](./literals.md#plugintypetype) 
2. See [:material-code-braces: ListPluginTypeActionsResponseTypeDef](./type_defs.md#listplugintypeactionsresponsetypedef) 


```python
# list_plugin_type_actions method usage example with argument unpacking

kwargs: ListPluginTypeActionsRequestRequestTypeDef = {  # (1)
    "pluginType": ...,
}

parent.list_plugin_type_actions(**kwargs)
```

1. See [:material-code-braces: ListPluginTypeActionsRequestRequestTypeDef](./type_defs.md#listplugintypeactionsrequestrequesttypedef) 

### list\_plugin\_type\_metadata

Lists metadata for all Amazon Q Business plugin types.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_plugin_type_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_plugin_type_metadata.html)

```python
# list_plugin_type_metadata method definition

await def list_plugin_type_metadata(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPluginTypeMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPluginTypeMetadataResponseTypeDef](./type_defs.md#listplugintypemetadataresponsetypedef) 


```python
# list_plugin_type_metadata method usage example with argument unpacking

kwargs: ListPluginTypeMetadataRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_plugin_type_metadata(**kwargs)
```

1. See [:material-code-braces: ListPluginTypeMetadataRequestRequestTypeDef](./type_defs.md#listplugintypemetadatarequestrequesttypedef) 

### list\_plugins

Lists configured Amazon Q Business plugins.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_plugins` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_plugins.html)

```python
# list_plugins method definition

await def list_plugins(
    self,
    *,
    applicationId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPluginsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPluginsResponseTypeDef](./type_defs.md#listpluginsresponsetypedef) 


```python
# list_plugins method usage example with argument unpacking

kwargs: ListPluginsRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_plugins(**kwargs)
```

1. See [:material-code-braces: ListPluginsRequestRequestTypeDef](./type_defs.md#listpluginsrequestrequesttypedef) 

### list\_retrievers

Lists the retriever used by an Amazon Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_retrievers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_retrievers.html)

```python
# list_retrievers method definition

await def list_retrievers(
    self,
    *,
    applicationId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListRetrieversResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRetrieversResponseTypeDef](./type_defs.md#listretrieversresponsetypedef) 


```python
# list_retrievers method usage example with argument unpacking

kwargs: ListRetrieversRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_retrievers(**kwargs)
```

1. See [:material-code-braces: ListRetrieversRequestRequestTypeDef](./type_defs.md#listretrieversrequestrequesttypedef) 

### list\_tags\_for\_resource

Gets a list of tags associated with a specified resource.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_web\_experiences

Lists one or more Amazon Q Business Web Experiences.

Type annotations and code completion for `#!python session.create_client("qbusiness").list_web_experiences` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/list_web_experiences.html)

```python
# list_web_experiences method definition

await def list_web_experiences(
    self,
    *,
    applicationId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListWebExperiencesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWebExperiencesResponseTypeDef](./type_defs.md#listwebexperiencesresponsetypedef) 


```python
# list_web_experiences method usage example with argument unpacking

kwargs: ListWebExperiencesRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.list_web_experiences(**kwargs)
```

1. See [:material-code-braces: ListWebExperiencesRequestRequestTypeDef](./type_defs.md#listwebexperiencesrequestrequesttypedef) 

### put\_feedback

Enables your end user to provide feedback on their Amazon Q Business generated
chat responses.

Type annotations and code completion for `#!python session.create_client("qbusiness").put_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/put_feedback.html)

```python
# put_feedback method definition

await def put_feedback(
    self,
    *,
    applicationId: str,
    conversationId: str,
    messageId: str,
    userId: str = ...,
    messageCopiedAt: TimestampTypeDef = ...,
    messageUsefulness: MessageUsefulnessFeedbackTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MessageUsefulnessFeedbackTypeDef](./type_defs.md#messageusefulnessfeedbacktypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_feedback method usage example with argument unpacking

kwargs: PutFeedbackRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "conversationId": ...,
    "messageId": ...,
}

parent.put_feedback(**kwargs)
```

1. See [:material-code-braces: PutFeedbackRequestRequestTypeDef](./type_defs.md#putfeedbackrequestrequesttypedef) 

### put\_group

Create, or updates, a mapping of users—who have access to a document—to groups.

Type annotations and code completion for `#!python session.create_client("qbusiness").put_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/put_group.html)

```python
# put_group method definition

await def put_group(
    self,
    *,
    applicationId: str,
    indexId: str,
    groupName: str,
    type: MembershipTypeType,  # (1)
    groupMembers: GroupMembersTypeDef,  # (2)
    dataSourceId: str = ...,
    roleArn: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: MembershipTypeType](./literals.md#membershiptypetype) 
2. See [:material-code-braces: GroupMembersTypeDef](./type_defs.md#groupmemberstypedef) 


```python
# put_group method usage example with argument unpacking

kwargs: PutGroupRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "groupName": ...,
    "type": ...,
    "groupMembers": ...,
}

parent.put_group(**kwargs)
```

1. See [:material-code-braces: PutGroupRequestRequestTypeDef](./type_defs.md#putgrouprequestrequesttypedef) 

### search\_relevant\_content

Searches for relevant content in a Q Business application based on a query.

Type annotations and code completion for `#!python session.create_client("qbusiness").search_relevant_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/search_relevant_content.html)

```python
# search_relevant_content method definition

await def search_relevant_content(
    self,
    *,
    applicationId: str,
    queryText: str,
    contentSource: ContentSourceTypeDef,  # (1)
    attributeFilter: AttributeFilterTypeDef = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchRelevantContentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ContentSourceTypeDef](./type_defs.md#contentsourcetypedef) 
2. See [:material-code-braces: AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef) 
3. See [:material-code-braces: SearchRelevantContentResponseTypeDef](./type_defs.md#searchrelevantcontentresponsetypedef) 


```python
# search_relevant_content method usage example with argument unpacking

kwargs: SearchRelevantContentRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "queryText": ...,
    "contentSource": ...,
}

parent.search_relevant_content(**kwargs)
```

1. See [:material-code-braces: SearchRelevantContentRequestRequestTypeDef](./type_defs.md#searchrelevantcontentrequestrequesttypedef) 

### start\_data\_source\_sync\_job

Starts a data source connector synchronization job.

Type annotations and code completion for `#!python session.create_client("qbusiness").start_data_source_sync_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/start_data_source_sync_job.html)

```python
# start_data_source_sync_job method definition

await def start_data_source_sync_job(
    self,
    *,
    dataSourceId: str,
    applicationId: str,
    indexId: str,
) -> StartDataSourceSyncJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartDataSourceSyncJobResponseTypeDef](./type_defs.md#startdatasourcesyncjobresponsetypedef) 


```python
# start_data_source_sync_job method usage example with argument unpacking

kwargs: StartDataSourceSyncJobRequestRequestTypeDef = {  # (1)
    "dataSourceId": ...,
    "applicationId": ...,
    "indexId": ...,
}

parent.start_data_source_sync_job(**kwargs)
```

1. See [:material-code-braces: StartDataSourceSyncJobRequestRequestTypeDef](./type_defs.md#startdatasourcesyncjobrequestrequesttypedef) 

### stop\_data\_source\_sync\_job

Stops an Amazon Q Business data source connector synchronization job already in
progress.

Type annotations and code completion for `#!python session.create_client("qbusiness").stop_data_source_sync_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/stop_data_source_sync_job.html)

```python
# stop_data_source_sync_job method definition

await def stop_data_source_sync_job(
    self,
    *,
    dataSourceId: str,
    applicationId: str,
    indexId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_data_source_sync_job method usage example with argument unpacking

kwargs: StopDataSourceSyncJobRequestRequestTypeDef = {  # (1)
    "dataSourceId": ...,
    "applicationId": ...,
    "indexId": ...,
}

parent.stop_data_source_sync_job(**kwargs)
```

1. See [:material-code-braces: StopDataSourceSyncJobRequestRequestTypeDef](./type_defs.md#stopdatasourcesyncjobrequestrequesttypedef) 

### tag\_resource

Adds the specified tag to the specified Amazon Q Business application or data
source resource.

Type annotations and code completion for `#!python session.create_client("qbusiness").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceARN: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a tag from an Amazon Q Business application or a data source.

Type annotations and code completion for `#!python session.create_client("qbusiness").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceARN: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_application

Updates an existing Amazon Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/update_application.html)

```python
# update_application method definition

await def update_application(
    self,
    *,
    applicationId: str,
    identityCenterInstanceArn: str = ...,
    displayName: str = ...,
    description: str = ...,
    roleArn: str = ...,
    attachmentsConfiguration: AttachmentsConfigurationTypeDef = ...,  # (1)
    qAppsConfiguration: QAppsConfigurationTypeDef = ...,  # (2)
    personalizationConfiguration: PersonalizationConfigurationTypeDef = ...,  # (3)
    autoSubscriptionConfiguration: AutoSubscriptionConfigurationTypeDef = ...,  # (4)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: AttachmentsConfigurationTypeDef](./type_defs.md#attachmentsconfigurationtypedef) 
2. See [:material-code-braces: QAppsConfigurationTypeDef](./type_defs.md#qappsconfigurationtypedef) 
3. See [:material-code-braces: PersonalizationConfigurationTypeDef](./type_defs.md#personalizationconfigurationtypedef) 
4. See [:material-code-braces: AutoSubscriptionConfigurationTypeDef](./type_defs.md#autosubscriptionconfigurationtypedef) 


```python
# update_application method usage example with argument unpacking

kwargs: UpdateApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef) 

### update\_chat\_controls\_configuration

Updates an set of chat controls configured for an existing Amazon Q Business
application.

Type annotations and code completion for `#!python session.create_client("qbusiness").update_chat_controls_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/update_chat_controls_configuration.html)

```python
# update_chat_controls_configuration method definition

await def update_chat_controls_configuration(
    self,
    *,
    applicationId: str,
    clientToken: str = ...,
    responseScope: ResponseScopeType = ...,  # (1)
    blockedPhrasesConfigurationUpdate: BlockedPhrasesConfigurationUpdateTypeDef = ...,  # (2)
    topicConfigurationsToCreateOrUpdate: Sequence[TopicConfigurationUnionTypeDef] = ...,  # (3)
    topicConfigurationsToDelete: Sequence[TopicConfigurationTypeDef] = ...,  # (4)
    creatorModeConfiguration: CreatorModeConfigurationTypeDef = ...,  # (5)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ResponseScopeType](./literals.md#responsescopetype) 
2. See [:material-code-braces: BlockedPhrasesConfigurationUpdateTypeDef](./type_defs.md#blockedphrasesconfigurationupdatetypedef) 
3. See [:material-code-braces: TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef) [:material-code-braces: TopicConfigurationOutputTypeDef](./type_defs.md#topicconfigurationoutputtypedef) 
4. See [:material-code-braces: TopicConfigurationTypeDef](./type_defs.md#topicconfigurationtypedef) 
5. See [:material-code-braces: CreatorModeConfigurationTypeDef](./type_defs.md#creatormodeconfigurationtypedef) 


```python
# update_chat_controls_configuration method usage example with argument unpacking

kwargs: UpdateChatControlsConfigurationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.update_chat_controls_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateChatControlsConfigurationRequestRequestTypeDef](./type_defs.md#updatechatcontrolsconfigurationrequestrequesttypedef) 

### update\_data\_accessor

Updates an existing data accessor.

Type annotations and code completion for `#!python session.create_client("qbusiness").update_data_accessor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/update_data_accessor.html)

```python
# update_data_accessor method definition

await def update_data_accessor(
    self,
    *,
    applicationId: str,
    dataAccessorId: str,
    actionConfigurations: Sequence[ActionConfigurationTypeDef],  # (1)
    displayName: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ActionConfigurationTypeDef](./type_defs.md#actionconfigurationtypedef) 


```python
# update_data_accessor method usage example with argument unpacking

kwargs: UpdateDataAccessorRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "dataAccessorId": ...,
    "actionConfigurations": ...,
}

parent.update_data_accessor(**kwargs)
```

1. See [:material-code-braces: UpdateDataAccessorRequestRequestTypeDef](./type_defs.md#updatedataaccessorrequestrequesttypedef) 

### update\_data\_source

Updates an existing Amazon Q Business data source connector.

Type annotations and code completion for `#!python session.create_client("qbusiness").update_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/update_data_source.html)

```python
# update_data_source method definition

await def update_data_source(
    self,
    *,
    applicationId: str,
    indexId: str,
    dataSourceId: str,
    displayName: str = ...,
    configuration: Mapping[str, Any] = ...,
    vpcConfiguration: DataSourceVpcConfigurationTypeDef = ...,  # (1)
    description: str = ...,
    syncSchedule: str = ...,
    roleArn: str = ...,
    documentEnrichmentConfiguration: DocumentEnrichmentConfigurationTypeDef = ...,  # (2)
    mediaExtractionConfiguration: MediaExtractionConfigurationTypeDef = ...,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) 
2. See [:material-code-braces: DocumentEnrichmentConfigurationTypeDef](./type_defs.md#documentenrichmentconfigurationtypedef) 
3. See [:material-code-braces: MediaExtractionConfigurationTypeDef](./type_defs.md#mediaextractionconfigurationtypedef) 


```python
# update_data_source method usage example with argument unpacking

kwargs: UpdateDataSourceRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
    "dataSourceId": ...,
}

parent.update_data_source(**kwargs)
```

1. See [:material-code-braces: UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef) 

### update\_index

Updates an Amazon Q Business index.

Type annotations and code completion for `#!python session.create_client("qbusiness").update_index` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/update_index.html)

```python
# update_index method definition

await def update_index(
    self,
    *,
    applicationId: str,
    indexId: str,
    displayName: str = ...,
    description: str = ...,
    capacityConfiguration: IndexCapacityConfigurationTypeDef = ...,  # (1)
    documentAttributeConfigurations: Sequence[DocumentAttributeConfigurationTypeDef] = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: IndexCapacityConfigurationTypeDef](./type_defs.md#indexcapacityconfigurationtypedef) 
2. See [:material-code-braces: DocumentAttributeConfigurationTypeDef](./type_defs.md#documentattributeconfigurationtypedef) 


```python
# update_index method usage example with argument unpacking

kwargs: UpdateIndexRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "indexId": ...,
}

parent.update_index(**kwargs)
```

1. See [:material-code-braces: UpdateIndexRequestRequestTypeDef](./type_defs.md#updateindexrequestrequesttypedef) 

### update\_plugin

Updates an Amazon Q Business plugin.

Type annotations and code completion for `#!python session.create_client("qbusiness").update_plugin` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/update_plugin.html)

```python
# update_plugin method definition

await def update_plugin(
    self,
    *,
    applicationId: str,
    pluginId: str,
    displayName: str = ...,
    state: PluginStateType = ...,  # (1)
    serverUrl: str = ...,
    customPluginConfiguration: CustomPluginConfigurationTypeDef = ...,  # (2)
    authConfiguration: PluginAuthConfigurationTypeDef = ...,  # (3)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PluginStateType](./literals.md#pluginstatetype) 
2. See [:material-code-braces: CustomPluginConfigurationTypeDef](./type_defs.md#custompluginconfigurationtypedef) 
3. See [:material-code-braces: PluginAuthConfigurationTypeDef](./type_defs.md#pluginauthconfigurationtypedef) 


```python
# update_plugin method usage example with argument unpacking

kwargs: UpdatePluginRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "pluginId": ...,
}

parent.update_plugin(**kwargs)
```

1. See [:material-code-braces: UpdatePluginRequestRequestTypeDef](./type_defs.md#updatepluginrequestrequesttypedef) 

### update\_retriever

Updates the retriever used for your Amazon Q Business application.

Type annotations and code completion for `#!python session.create_client("qbusiness").update_retriever` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/update_retriever.html)

```python
# update_retriever method definition

await def update_retriever(
    self,
    *,
    applicationId: str,
    retrieverId: str,
    configuration: RetrieverConfigurationTypeDef = ...,  # (1)
    displayName: str = ...,
    roleArn: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: RetrieverConfigurationTypeDef](./type_defs.md#retrieverconfigurationtypedef) 


```python
# update_retriever method usage example with argument unpacking

kwargs: UpdateRetrieverRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "retrieverId": ...,
}

parent.update_retriever(**kwargs)
```

1. See [:material-code-braces: UpdateRetrieverRequestRequestTypeDef](./type_defs.md#updateretrieverrequestrequesttypedef) 

### update\_user

Updates a information associated with a user id.

Type annotations and code completion for `#!python session.create_client("qbusiness").update_user` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/update_user.html)

```python
# update_user method definition

await def update_user(
    self,
    *,
    applicationId: str,
    userId: str,
    userAliasesToUpdate: Sequence[UserAliasTypeDef] = ...,  # (1)
    userAliasesToDelete: Sequence[UserAliasTypeDef] = ...,  # (1)
) -> UpdateUserResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
2. See [:material-code-braces: UserAliasTypeDef](./type_defs.md#useraliastypedef) 
3. See [:material-code-braces: UpdateUserResponseTypeDef](./type_defs.md#updateuserresponsetypedef) 


```python
# update_user method usage example with argument unpacking

kwargs: UpdateUserRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "userId": ...,
}

parent.update_user(**kwargs)
```

1. See [:material-code-braces: UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef) 

### update\_web\_experience

Updates an Amazon Q Business web experience.

Type annotations and code completion for `#!python session.create_client("qbusiness").update_web_experience` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness/client/update_web_experience.html)

```python
# update_web_experience method definition

await def update_web_experience(
    self,
    *,
    applicationId: str,
    webExperienceId: str,
    roleArn: str = ...,
    authenticationConfiguration: WebExperienceAuthConfigurationTypeDef = ...,  # (1)
    title: str = ...,
    subtitle: str = ...,
    welcomeMessage: str = ...,
    samplePromptsControlMode: WebExperienceSamplePromptsControlModeType = ...,  # (2)
    identityProviderConfiguration: IdentityProviderConfigurationTypeDef = ...,  # (3)
    origins: Sequence[str] = ...,
    browserExtensionConfiguration: BrowserExtensionConfigurationTypeDef = ...,  # (4)
    customizationConfiguration: CustomizationConfigurationTypeDef = ...,  # (5)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: WebExperienceAuthConfigurationTypeDef](./type_defs.md#webexperienceauthconfigurationtypedef) 
2. See [:material-code-brackets: WebExperienceSamplePromptsControlModeType](./literals.md#webexperiencesamplepromptscontrolmodetype) 
3. See [:material-code-braces: IdentityProviderConfigurationTypeDef](./type_defs.md#identityproviderconfigurationtypedef) 
4. See [:material-code-braces: BrowserExtensionConfigurationTypeDef](./type_defs.md#browserextensionconfigurationtypedef) 
5. See [:material-code-braces: CustomizationConfigurationTypeDef](./type_defs.md#customizationconfigurationtypedef) 


```python
# update_web_experience method usage example with argument unpacking

kwargs: UpdateWebExperienceRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
    "webExperienceId": ...,
}

parent.update_web_experience(**kwargs)
```

1. See [:material-code-braces: UpdateWebExperienceRequestRequestTypeDef](./type_defs.md#updatewebexperiencerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("qbusiness").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("qbusiness").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness.Client)

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

Type annotations and code completion for `#!python session.create_client("qbusiness").get_paginator` method with overloads.

- `client.get_paginator("get_chat_controls_configuration")` -> [GetChatControlsConfigurationPaginator](./paginators.md#getchatcontrolsconfigurationpaginator)
- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
- `client.get_paginator("list_attachments")` -> [ListAttachmentsPaginator](./paginators.md#listattachmentspaginator)
- `client.get_paginator("list_conversations")` -> [ListConversationsPaginator](./paginators.md#listconversationspaginator)
- `client.get_paginator("list_data_accessors")` -> [ListDataAccessorsPaginator](./paginators.md#listdataaccessorspaginator)
- `client.get_paginator("list_data_source_sync_jobs")` -> [ListDataSourceSyncJobsPaginator](./paginators.md#listdatasourcesyncjobspaginator)
- `client.get_paginator("list_data_sources")` -> [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- `client.get_paginator("list_documents")` -> [ListDocumentsPaginator](./paginators.md#listdocumentspaginator)
- `client.get_paginator("list_groups")` -> [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- `client.get_paginator("list_indices")` -> [ListIndicesPaginator](./paginators.md#listindicespaginator)
- `client.get_paginator("list_messages")` -> [ListMessagesPaginator](./paginators.md#listmessagespaginator)
- `client.get_paginator("list_plugin_actions")` -> [ListPluginActionsPaginator](./paginators.md#listpluginactionspaginator)
- `client.get_paginator("list_plugin_type_actions")` -> [ListPluginTypeActionsPaginator](./paginators.md#listplugintypeactionspaginator)
- `client.get_paginator("list_plugin_type_metadata")` -> [ListPluginTypeMetadataPaginator](./paginators.md#listplugintypemetadatapaginator)
- `client.get_paginator("list_plugins")` -> [ListPluginsPaginator](./paginators.md#listpluginspaginator)
- `client.get_paginator("list_retrievers")` -> [ListRetrieversPaginator](./paginators.md#listretrieverspaginator)
- `client.get_paginator("list_web_experiences")` -> [ListWebExperiencesPaginator](./paginators.md#listwebexperiencespaginator)
- `client.get_paginator("search_relevant_content")` -> [SearchRelevantContentPaginator](./paginators.md#searchrelevantcontentpaginator)



