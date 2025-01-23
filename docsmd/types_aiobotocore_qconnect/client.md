# QConnectClient

> [Index](../README.md) > [QConnect](./README.md) > QConnectClient

!!! note ""

    Auto-generated documentation for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#qconnect)
    type annotations stubs module [types-aiobotocore-qconnect](https://pypi.org/project/types-aiobotocore-qconnect/).

## QConnectClient

Type annotations and code completion for `#!python session.create_client("qconnect")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client)

```python
# QConnectClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_qconnect.client import QConnectClient

session = get_session()
async with session.create_client("qconnect") as client:
    client: QConnectClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("qconnect").exceptions` structure.

```python
# QConnectClient.exceptions usage example

async with session.create_client("qconnect") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.PreconditionFailedException,
        client.RequestTimeoutException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.TooManyTagsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# QConnectClient usage type checking example

from types_aiobotocore_qconnect.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("qconnect").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("qconnect").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/generate_presigned_url.html)

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


### activate\_message\_template

Activates a specific version of the Amazon Q in Connect message template.

Type annotations and code completion for `#!python session.create_client("qconnect").activate_message_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/activate_message_template.html)

```python
# activate_message_template method definition

await def activate_message_template(
    self,
    *,
    knowledgeBaseId: str,
    messageTemplateId: str,
    versionNumber: int,
) -> ActivateMessageTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ActivateMessageTemplateResponseTypeDef](./type_defs.md#activatemessagetemplateresponsetypedef) 


```python
# activate_message_template method usage example with argument unpacking

kwargs: ActivateMessageTemplateRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
    "versionNumber": ...,
}

parent.activate_message_template(**kwargs)
```

1. See [:material-code-braces: ActivateMessageTemplateRequestRequestTypeDef](./type_defs.md#activatemessagetemplaterequestrequesttypedef) 

### create\_ai\_agent

Creates an Amazon Q in Connect AI Agent.

Type annotations and code completion for `#!python session.create_client("qconnect").create_ai_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_ai_agent.html)

```python
# create_ai_agent method definition

await def create_ai_agent(
    self,
    *,
    assistantId: str,
    configuration: AIAgentConfigurationTypeDef,  # (1)
    name: str,
    type: AIAgentTypeType,  # (2)
    visibilityStatus: VisibilityStatusType,  # (3)
    clientToken: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAIAgentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AIAgentConfigurationTypeDef](./type_defs.md#aiagentconfigurationtypedef) 
2. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) 
3. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
4. See [:material-code-braces: CreateAIAgentResponseTypeDef](./type_defs.md#createaiagentresponsetypedef) 


```python
# create_ai_agent method usage example with argument unpacking

kwargs: CreateAIAgentRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "configuration": ...,
    "name": ...,
    "type": ...,
    "visibilityStatus": ...,
}

parent.create_ai_agent(**kwargs)
```

1. See [:material-code-braces: CreateAIAgentRequestRequestTypeDef](./type_defs.md#createaiagentrequestrequesttypedef) 

### create\_ai\_agent\_version

Creates and Amazon Q in Connect AI Agent version.

Type annotations and code completion for `#!python session.create_client("qconnect").create_ai_agent_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_ai_agent_version.html)

```python
# create_ai_agent_version method definition

await def create_ai_agent_version(
    self,
    *,
    aiAgentId: str,
    assistantId: str,
    clientToken: str = ...,
    modifiedTime: TimestampTypeDef = ...,
) -> CreateAIAgentVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAIAgentVersionResponseTypeDef](./type_defs.md#createaiagentversionresponsetypedef) 


```python
# create_ai_agent_version method usage example with argument unpacking

kwargs: CreateAIAgentVersionRequestRequestTypeDef = {  # (1)
    "aiAgentId": ...,
    "assistantId": ...,
}

parent.create_ai_agent_version(**kwargs)
```

1. See [:material-code-braces: CreateAIAgentVersionRequestRequestTypeDef](./type_defs.md#createaiagentversionrequestrequesttypedef) 

### create\_ai\_guardrail

Creates an Amazon Q in Connect AI Guardrail.

Type annotations and code completion for `#!python session.create_client("qconnect").create_ai_guardrail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_ai_guardrail.html)

```python
# create_ai_guardrail method definition

await def create_ai_guardrail(
    self,
    *,
    assistantId: str,
    blockedInputMessaging: str,
    blockedOutputsMessaging: str,
    name: str,
    visibilityStatus: VisibilityStatusType,  # (1)
    clientToken: str = ...,
    contentPolicyConfig: AIGuardrailContentPolicyConfigTypeDef = ...,  # (2)
    contextualGroundingPolicyConfig: AIGuardrailContextualGroundingPolicyConfigTypeDef = ...,  # (3)
    description: str = ...,
    sensitiveInformationPolicyConfig: AIGuardrailSensitiveInformationPolicyConfigTypeDef = ...,  # (4)
    tags: Mapping[str, str] = ...,
    topicPolicyConfig: AIGuardrailTopicPolicyConfigTypeDef = ...,  # (5)
    wordPolicyConfig: AIGuardrailWordPolicyConfigTypeDef = ...,  # (6)
) -> CreateAIGuardrailResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
2. See [:material-code-braces: AIGuardrailContentPolicyConfigTypeDef](./type_defs.md#aiguardrailcontentpolicyconfigtypedef) 
3. See [:material-code-braces: AIGuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#aiguardrailcontextualgroundingpolicyconfigtypedef) 
4. See [:material-code-braces: AIGuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#aiguardrailsensitiveinformationpolicyconfigtypedef) 
5. See [:material-code-braces: AIGuardrailTopicPolicyConfigTypeDef](./type_defs.md#aiguardrailtopicpolicyconfigtypedef) 
6. See [:material-code-braces: AIGuardrailWordPolicyConfigTypeDef](./type_defs.md#aiguardrailwordpolicyconfigtypedef) 
7. See [:material-code-braces: CreateAIGuardrailResponseTypeDef](./type_defs.md#createaiguardrailresponsetypedef) 


```python
# create_ai_guardrail method usage example with argument unpacking

kwargs: CreateAIGuardrailRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "blockedInputMessaging": ...,
    "blockedOutputsMessaging": ...,
    "name": ...,
    "visibilityStatus": ...,
}

parent.create_ai_guardrail(**kwargs)
```

1. See [:material-code-braces: CreateAIGuardrailRequestRequestTypeDef](./type_defs.md#createaiguardrailrequestrequesttypedef) 

### create\_ai\_guardrail\_version

Creates an Amazon Q in Connect AI Guardrail version.

Type annotations and code completion for `#!python session.create_client("qconnect").create_ai_guardrail_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_ai_guardrail_version.html)

```python
# create_ai_guardrail_version method definition

await def create_ai_guardrail_version(
    self,
    *,
    aiGuardrailId: str,
    assistantId: str,
    clientToken: str = ...,
    modifiedTime: TimestampTypeDef = ...,
) -> CreateAIGuardrailVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAIGuardrailVersionResponseTypeDef](./type_defs.md#createaiguardrailversionresponsetypedef) 


```python
# create_ai_guardrail_version method usage example with argument unpacking

kwargs: CreateAIGuardrailVersionRequestRequestTypeDef = {  # (1)
    "aiGuardrailId": ...,
    "assistantId": ...,
}

parent.create_ai_guardrail_version(**kwargs)
```

1. See [:material-code-braces: CreateAIGuardrailVersionRequestRequestTypeDef](./type_defs.md#createaiguardrailversionrequestrequesttypedef) 

### create\_ai\_prompt

Creates an Amazon Q in Connect AI Prompt.

Type annotations and code completion for `#!python session.create_client("qconnect").create_ai_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_ai_prompt.html)

```python
# create_ai_prompt method definition

await def create_ai_prompt(
    self,
    *,
    apiFormat: AIPromptAPIFormatType,  # (1)
    assistantId: str,
    modelId: str,
    name: str,
    templateConfiguration: AIPromptTemplateConfigurationTypeDef,  # (2)
    templateType: AIPromptTemplateTypeType,  # (3)
    type: AIPromptTypeType,  # (4)
    visibilityStatus: VisibilityStatusType,  # (5)
    clientToken: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAIPromptResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: AIPromptAPIFormatType](./literals.md#aipromptapiformattype) 
2. See [:material-code-braces: AIPromptTemplateConfigurationTypeDef](./type_defs.md#aiprompttemplateconfigurationtypedef) 
3. See [:material-code-brackets: AIPromptTemplateTypeType](./literals.md#aiprompttemplatetypetype) 
4. See [:material-code-brackets: AIPromptTypeType](./literals.md#aiprompttypetype) 
5. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
6. See [:material-code-braces: CreateAIPromptResponseTypeDef](./type_defs.md#createaipromptresponsetypedef) 


```python
# create_ai_prompt method usage example with argument unpacking

kwargs: CreateAIPromptRequestRequestTypeDef = {  # (1)
    "apiFormat": ...,
    "assistantId": ...,
    "modelId": ...,
    "name": ...,
    "templateConfiguration": ...,
    "templateType": ...,
    "type": ...,
    "visibilityStatus": ...,
}

parent.create_ai_prompt(**kwargs)
```

1. See [:material-code-braces: CreateAIPromptRequestRequestTypeDef](./type_defs.md#createaipromptrequestrequesttypedef) 

### create\_ai\_prompt\_version

Creates an Amazon Q in Connect AI Prompt version.

Type annotations and code completion for `#!python session.create_client("qconnect").create_ai_prompt_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_ai_prompt_version.html)

```python
# create_ai_prompt_version method definition

await def create_ai_prompt_version(
    self,
    *,
    aiPromptId: str,
    assistantId: str,
    clientToken: str = ...,
    modifiedTime: TimestampTypeDef = ...,
) -> CreateAIPromptVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAIPromptVersionResponseTypeDef](./type_defs.md#createaipromptversionresponsetypedef) 


```python
# create_ai_prompt_version method usage example with argument unpacking

kwargs: CreateAIPromptVersionRequestRequestTypeDef = {  # (1)
    "aiPromptId": ...,
    "assistantId": ...,
}

parent.create_ai_prompt_version(**kwargs)
```

1. See [:material-code-braces: CreateAIPromptVersionRequestRequestTypeDef](./type_defs.md#createaipromptversionrequestrequesttypedef) 

### create\_assistant

Creates an Amazon Q in Connect assistant.

Type annotations and code completion for `#!python session.create_client("qconnect").create_assistant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_assistant.html)

```python
# create_assistant method definition

await def create_assistant(
    self,
    *,
    name: str,
    type: AssistantTypeType,  # (1)
    clientToken: str = ...,
    description: str = ...,
    serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> CreateAssistantResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AssistantTypeType](./literals.md#assistanttypetype) 
2. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
3. See [:material-code-braces: CreateAssistantResponseTypeDef](./type_defs.md#createassistantresponsetypedef) 


```python
# create_assistant method usage example with argument unpacking

kwargs: CreateAssistantRequestRequestTypeDef = {  # (1)
    "name": ...,
    "type": ...,
}

parent.create_assistant(**kwargs)
```

1. See [:material-code-braces: CreateAssistantRequestRequestTypeDef](./type_defs.md#createassistantrequestrequesttypedef) 

### create\_assistant\_association

Creates an association between an Amazon Q in Connect assistant and another
resource.

Type annotations and code completion for `#!python session.create_client("qconnect").create_assistant_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_assistant_association.html)

```python
# create_assistant_association method definition

await def create_assistant_association(
    self,
    *,
    assistantId: str,
    association: AssistantAssociationInputDataTypeDef,  # (1)
    associationType: AssociationTypeType,  # (2)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAssistantAssociationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AssistantAssociationInputDataTypeDef](./type_defs.md#assistantassociationinputdatatypedef) 
2. See [:material-code-brackets: AssociationTypeType](./literals.md#associationtypetype) 
3. See [:material-code-braces: CreateAssistantAssociationResponseTypeDef](./type_defs.md#createassistantassociationresponsetypedef) 


```python
# create_assistant_association method usage example with argument unpacking

kwargs: CreateAssistantAssociationRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "association": ...,
    "associationType": ...,
}

parent.create_assistant_association(**kwargs)
```

1. See [:material-code-braces: CreateAssistantAssociationRequestRequestTypeDef](./type_defs.md#createassistantassociationrequestrequesttypedef) 

### create\_content

Creates Amazon Q in Connect content.

Type annotations and code completion for `#!python session.create_client("qconnect").create_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_content.html)

```python
# create_content method definition

await def create_content(
    self,
    *,
    knowledgeBaseId: str,
    name: str,
    uploadId: str,
    clientToken: str = ...,
    metadata: Mapping[str, str] = ...,
    overrideLinkOutUri: str = ...,
    tags: Mapping[str, str] = ...,
    title: str = ...,
) -> CreateContentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateContentResponseTypeDef](./type_defs.md#createcontentresponsetypedef) 


```python
# create_content method usage example with argument unpacking

kwargs: CreateContentRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "name": ...,
    "uploadId": ...,
}

parent.create_content(**kwargs)
```

1. See [:material-code-braces: CreateContentRequestRequestTypeDef](./type_defs.md#createcontentrequestrequesttypedef) 

### create\_content\_association

Creates an association between a content resource in a knowledge base and <a
href="https://docs.aws.amazon.com/connect/latest/adminguide/step-by-step-guided-experiences.html">step-by-step
guides</a>.

Type annotations and code completion for `#!python session.create_client("qconnect").create_content_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_content_association.html)

```python
# create_content_association method definition

await def create_content_association(
    self,
    *,
    association: ContentAssociationContentsTypeDef,  # (1)
    associationType: ContentAssociationTypeType,  # (2)
    contentId: str,
    knowledgeBaseId: str,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateContentAssociationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ContentAssociationContentsTypeDef](./type_defs.md#contentassociationcontentstypedef) 
2. See [:material-code-brackets: ContentAssociationTypeType](./literals.md#contentassociationtypetype) 
3. See [:material-code-braces: CreateContentAssociationResponseTypeDef](./type_defs.md#createcontentassociationresponsetypedef) 


```python
# create_content_association method usage example with argument unpacking

kwargs: CreateContentAssociationRequestRequestTypeDef = {  # (1)
    "association": ...,
    "associationType": ...,
    "contentId": ...,
    "knowledgeBaseId": ...,
}

parent.create_content_association(**kwargs)
```

1. See [:material-code-braces: CreateContentAssociationRequestRequestTypeDef](./type_defs.md#createcontentassociationrequestrequesttypedef) 

### create\_knowledge\_base

Creates a knowledge base.

Type annotations and code completion for `#!python session.create_client("qconnect").create_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_knowledge_base.html)

```python
# create_knowledge_base method definition

await def create_knowledge_base(
    self,
    *,
    knowledgeBaseType: KnowledgeBaseTypeType,  # (1)
    name: str,
    clientToken: str = ...,
    description: str = ...,
    renderingConfiguration: RenderingConfigurationTypeDef = ...,  # (2)
    serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,  # (3)
    sourceConfiguration: SourceConfigurationTypeDef = ...,  # (4)
    tags: Mapping[str, str] = ...,
    vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,  # (5)
) -> CreateKnowledgeBaseResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype) 
2. See [:material-code-braces: RenderingConfigurationTypeDef](./type_defs.md#renderingconfigurationtypedef) 
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
4. See [:material-code-braces: SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef) 
5. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
6. See [:material-code-braces: CreateKnowledgeBaseResponseTypeDef](./type_defs.md#createknowledgebaseresponsetypedef) 


```python
# create_knowledge_base method usage example with argument unpacking

kwargs: CreateKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseType": ...,
    "name": ...,
}

parent.create_knowledge_base(**kwargs)
```

1. See [:material-code-braces: CreateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#createknowledgebaserequestrequesttypedef) 

### create\_message\_template

Creates an Amazon Q in Connect message template.

Type annotations and code completion for `#!python session.create_client("qconnect").create_message_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_message_template.html)

```python
# create_message_template method definition

await def create_message_template(
    self,
    *,
    channelSubtype: ChannelSubtypeType,  # (1)
    content: MessageTemplateContentProviderTypeDef,  # (2)
    knowledgeBaseId: str,
    name: str,
    clientToken: str = ...,
    defaultAttributes: MessageTemplateAttributesTypeDef = ...,  # (3)
    description: str = ...,
    groupingConfiguration: GroupingConfigurationTypeDef = ...,  # (4)
    language: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateMessageTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ChannelSubtypeType](./literals.md#channelsubtypetype) 
2. See [:material-code-braces: MessageTemplateContentProviderTypeDef](./type_defs.md#messagetemplatecontentprovidertypedef) 
3. See [:material-code-braces: MessageTemplateAttributesTypeDef](./type_defs.md#messagetemplateattributestypedef) 
4. See [:material-code-braces: GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef) 
5. See [:material-code-braces: CreateMessageTemplateResponseTypeDef](./type_defs.md#createmessagetemplateresponsetypedef) 


```python
# create_message_template method usage example with argument unpacking

kwargs: CreateMessageTemplateRequestRequestTypeDef = {  # (1)
    "channelSubtype": ...,
    "content": ...,
    "knowledgeBaseId": ...,
    "name": ...,
}

parent.create_message_template(**kwargs)
```

1. See [:material-code-braces: CreateMessageTemplateRequestRequestTypeDef](./type_defs.md#createmessagetemplaterequestrequesttypedef) 

### create\_message\_template\_attachment

Uploads an attachment file to the specified Amazon Q in Connect message
template.

Type annotations and code completion for `#!python session.create_client("qconnect").create_message_template_attachment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_message_template_attachment.html)

```python
# create_message_template_attachment method definition

await def create_message_template_attachment(
    self,
    *,
    body: str,
    contentDisposition: ContentDispositionType,  # (1)
    knowledgeBaseId: str,
    messageTemplateId: str,
    name: str,
    clientToken: str = ...,
) -> CreateMessageTemplateAttachmentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContentDispositionType](./literals.md#contentdispositiontype) 
2. See [:material-code-braces: CreateMessageTemplateAttachmentResponseTypeDef](./type_defs.md#createmessagetemplateattachmentresponsetypedef) 


```python
# create_message_template_attachment method usage example with argument unpacking

kwargs: CreateMessageTemplateAttachmentRequestRequestTypeDef = {  # (1)
    "body": ...,
    "contentDisposition": ...,
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
    "name": ...,
}

parent.create_message_template_attachment(**kwargs)
```

1. See [:material-code-braces: CreateMessageTemplateAttachmentRequestRequestTypeDef](./type_defs.md#createmessagetemplateattachmentrequestrequesttypedef) 

### create\_message\_template\_version

Creates a new Amazon Q in Connect message template version from the current
content and configuration of a message template.

Type annotations and code completion for `#!python session.create_client("qconnect").create_message_template_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_message_template_version.html)

```python
# create_message_template_version method definition

await def create_message_template_version(
    self,
    *,
    knowledgeBaseId: str,
    messageTemplateId: str,
    messageTemplateContentSha256: str = ...,
) -> CreateMessageTemplateVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateMessageTemplateVersionResponseTypeDef](./type_defs.md#createmessagetemplateversionresponsetypedef) 


```python
# create_message_template_version method usage example with argument unpacking

kwargs: CreateMessageTemplateVersionRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
}

parent.create_message_template_version(**kwargs)
```

1. See [:material-code-braces: CreateMessageTemplateVersionRequestRequestTypeDef](./type_defs.md#createmessagetemplateversionrequestrequesttypedef) 

### create\_quick\_response

Creates an Amazon Q in Connect quick response.

Type annotations and code completion for `#!python session.create_client("qconnect").create_quick_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_quick_response.html)

```python
# create_quick_response method definition

await def create_quick_response(
    self,
    *,
    content: QuickResponseDataProviderTypeDef,  # (1)
    knowledgeBaseId: str,
    name: str,
    channels: Sequence[str] = ...,
    clientToken: str = ...,
    contentType: str = ...,
    description: str = ...,
    groupingConfiguration: GroupingConfigurationTypeDef = ...,  # (2)
    isActive: bool = ...,
    language: str = ...,
    shortcutKey: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateQuickResponseResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: QuickResponseDataProviderTypeDef](./type_defs.md#quickresponsedataprovidertypedef) 
2. See [:material-code-braces: GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef) 
3. See [:material-code-braces: CreateQuickResponseResponseTypeDef](./type_defs.md#createquickresponseresponsetypedef) 


```python
# create_quick_response method usage example with argument unpacking

kwargs: CreateQuickResponseRequestRequestTypeDef = {  # (1)
    "content": ...,
    "knowledgeBaseId": ...,
    "name": ...,
}

parent.create_quick_response(**kwargs)
```

1. See [:material-code-braces: CreateQuickResponseRequestRequestTypeDef](./type_defs.md#createquickresponserequestrequesttypedef) 

### create\_session

Creates a session.

Type annotations and code completion for `#!python session.create_client("qconnect").create_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/create_session.html)

```python
# create_session method definition

await def create_session(
    self,
    *,
    assistantId: str,
    name: str,
    aiAgentConfiguration: Mapping[AIAgentTypeType, AIAgentConfigurationDataTypeDef] = ...,  # (1)
    clientToken: str = ...,
    description: str = ...,
    tagFilter: TagFilterTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> CreateSessionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) [:material-code-braces: AIAgentConfigurationDataTypeDef](./type_defs.md#aiagentconfigurationdatatypedef) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
3. See [:material-code-braces: CreateSessionResponseTypeDef](./type_defs.md#createsessionresponsetypedef) 


```python
# create_session method usage example with argument unpacking

kwargs: CreateSessionRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "name": ...,
}

parent.create_session(**kwargs)
```

1. See [:material-code-braces: CreateSessionRequestRequestTypeDef](./type_defs.md#createsessionrequestrequesttypedef) 

### deactivate\_message\_template

Deactivates a specific version of the Amazon Q in Connect message template.

Type annotations and code completion for `#!python session.create_client("qconnect").deactivate_message_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/deactivate_message_template.html)

```python
# deactivate_message_template method definition

await def deactivate_message_template(
    self,
    *,
    knowledgeBaseId: str,
    messageTemplateId: str,
    versionNumber: int,
) -> DeactivateMessageTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeactivateMessageTemplateResponseTypeDef](./type_defs.md#deactivatemessagetemplateresponsetypedef) 


```python
# deactivate_message_template method usage example with argument unpacking

kwargs: DeactivateMessageTemplateRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
    "versionNumber": ...,
}

parent.deactivate_message_template(**kwargs)
```

1. See [:material-code-braces: DeactivateMessageTemplateRequestRequestTypeDef](./type_defs.md#deactivatemessagetemplaterequestrequesttypedef) 

### delete\_ai\_agent

Deletes an Amazon Q in Connect AI Agent.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_ai_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_ai_agent.html)

```python
# delete_ai_agent method definition

await def delete_ai_agent(
    self,
    *,
    aiAgentId: str,
    assistantId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ai_agent method usage example with argument unpacking

kwargs: DeleteAIAgentRequestRequestTypeDef = {  # (1)
    "aiAgentId": ...,
    "assistantId": ...,
}

parent.delete_ai_agent(**kwargs)
```

1. See [:material-code-braces: DeleteAIAgentRequestRequestTypeDef](./type_defs.md#deleteaiagentrequestrequesttypedef) 

### delete\_ai\_agent\_version

Deletes an Amazon Q in Connect AI Agent Version.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_ai_agent_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_ai_agent_version.html)

```python
# delete_ai_agent_version method definition

await def delete_ai_agent_version(
    self,
    *,
    aiAgentId: str,
    assistantId: str,
    versionNumber: int,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ai_agent_version method usage example with argument unpacking

kwargs: DeleteAIAgentVersionRequestRequestTypeDef = {  # (1)
    "aiAgentId": ...,
    "assistantId": ...,
    "versionNumber": ...,
}

parent.delete_ai_agent_version(**kwargs)
```

1. See [:material-code-braces: DeleteAIAgentVersionRequestRequestTypeDef](./type_defs.md#deleteaiagentversionrequestrequesttypedef) 

### delete\_ai\_guardrail

Deletes an Amazon Q in Connect AI Guardrail.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_ai_guardrail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_ai_guardrail.html)

```python
# delete_ai_guardrail method definition

await def delete_ai_guardrail(
    self,
    *,
    aiGuardrailId: str,
    assistantId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ai_guardrail method usage example with argument unpacking

kwargs: DeleteAIGuardrailRequestRequestTypeDef = {  # (1)
    "aiGuardrailId": ...,
    "assistantId": ...,
}

parent.delete_ai_guardrail(**kwargs)
```

1. See [:material-code-braces: DeleteAIGuardrailRequestRequestTypeDef](./type_defs.md#deleteaiguardrailrequestrequesttypedef) 

### delete\_ai\_guardrail\_version

Delete and Amazon Q in Connect AI Guardrail version.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_ai_guardrail_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_ai_guardrail_version.html)

```python
# delete_ai_guardrail_version method definition

await def delete_ai_guardrail_version(
    self,
    *,
    aiGuardrailId: str,
    assistantId: str,
    versionNumber: int,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ai_guardrail_version method usage example with argument unpacking

kwargs: DeleteAIGuardrailVersionRequestRequestTypeDef = {  # (1)
    "aiGuardrailId": ...,
    "assistantId": ...,
    "versionNumber": ...,
}

parent.delete_ai_guardrail_version(**kwargs)
```

1. See [:material-code-braces: DeleteAIGuardrailVersionRequestRequestTypeDef](./type_defs.md#deleteaiguardrailversionrequestrequesttypedef) 

### delete\_ai\_prompt

Deletes an Amazon Q in Connect AI Prompt.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_ai_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_ai_prompt.html)

```python
# delete_ai_prompt method definition

await def delete_ai_prompt(
    self,
    *,
    aiPromptId: str,
    assistantId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ai_prompt method usage example with argument unpacking

kwargs: DeleteAIPromptRequestRequestTypeDef = {  # (1)
    "aiPromptId": ...,
    "assistantId": ...,
}

parent.delete_ai_prompt(**kwargs)
```

1. See [:material-code-braces: DeleteAIPromptRequestRequestTypeDef](./type_defs.md#deleteaipromptrequestrequesttypedef) 

### delete\_ai\_prompt\_version

Delete and Amazon Q in Connect AI Prompt version.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_ai_prompt_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_ai_prompt_version.html)

```python
# delete_ai_prompt_version method definition

await def delete_ai_prompt_version(
    self,
    *,
    aiPromptId: str,
    assistantId: str,
    versionNumber: int,
) -> Dict[str, Any]:
    ...
```



```python
# delete_ai_prompt_version method usage example with argument unpacking

kwargs: DeleteAIPromptVersionRequestRequestTypeDef = {  # (1)
    "aiPromptId": ...,
    "assistantId": ...,
    "versionNumber": ...,
}

parent.delete_ai_prompt_version(**kwargs)
```

1. See [:material-code-braces: DeleteAIPromptVersionRequestRequestTypeDef](./type_defs.md#deleteaipromptversionrequestrequesttypedef) 

### delete\_assistant

Deletes an assistant.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_assistant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_assistant.html)

```python
# delete_assistant method definition

await def delete_assistant(
    self,
    *,
    assistantId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_assistant method usage example with argument unpacking

kwargs: DeleteAssistantRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
}

parent.delete_assistant(**kwargs)
```

1. See [:material-code-braces: DeleteAssistantRequestRequestTypeDef](./type_defs.md#deleteassistantrequestrequesttypedef) 

### delete\_assistant\_association

Deletes an assistant association.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_assistant_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_assistant_association.html)

```python
# delete_assistant_association method definition

await def delete_assistant_association(
    self,
    *,
    assistantAssociationId: str,
    assistantId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_assistant_association method usage example with argument unpacking

kwargs: DeleteAssistantAssociationRequestRequestTypeDef = {  # (1)
    "assistantAssociationId": ...,
    "assistantId": ...,
}

parent.delete_assistant_association(**kwargs)
```

1. See [:material-code-braces: DeleteAssistantAssociationRequestRequestTypeDef](./type_defs.md#deleteassistantassociationrequestrequesttypedef) 

### delete\_content

Deletes the content.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_content.html)

```python
# delete_content method definition

await def delete_content(
    self,
    *,
    contentId: str,
    knowledgeBaseId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_content method usage example with argument unpacking

kwargs: DeleteContentRequestRequestTypeDef = {  # (1)
    "contentId": ...,
    "knowledgeBaseId": ...,
}

parent.delete_content(**kwargs)
```

1. See [:material-code-braces: DeleteContentRequestRequestTypeDef](./type_defs.md#deletecontentrequestrequesttypedef) 

### delete\_content\_association

Deletes the content association.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_content_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_content_association.html)

```python
# delete_content_association method definition

await def delete_content_association(
    self,
    *,
    contentAssociationId: str,
    contentId: str,
    knowledgeBaseId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_content_association method usage example with argument unpacking

kwargs: DeleteContentAssociationRequestRequestTypeDef = {  # (1)
    "contentAssociationId": ...,
    "contentId": ...,
    "knowledgeBaseId": ...,
}

parent.delete_content_association(**kwargs)
```

1. See [:material-code-braces: DeleteContentAssociationRequestRequestTypeDef](./type_defs.md#deletecontentassociationrequestrequesttypedef) 

### delete\_import\_job

Deletes the quick response import job.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_import_job.html)

```python
# delete_import_job method definition

await def delete_import_job(
    self,
    *,
    importJobId: str,
    knowledgeBaseId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_import_job method usage example with argument unpacking

kwargs: DeleteImportJobRequestRequestTypeDef = {  # (1)
    "importJobId": ...,
    "knowledgeBaseId": ...,
}

parent.delete_import_job(**kwargs)
```

1. See [:material-code-braces: DeleteImportJobRequestRequestTypeDef](./type_defs.md#deleteimportjobrequestrequesttypedef) 

### delete\_knowledge\_base

Deletes the knowledge base.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_knowledge_base.html)

```python
# delete_knowledge_base method definition

await def delete_knowledge_base(
    self,
    *,
    knowledgeBaseId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_knowledge_base method usage example with argument unpacking

kwargs: DeleteKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.delete_knowledge_base(**kwargs)
```

1. See [:material-code-braces: DeleteKnowledgeBaseRequestRequestTypeDef](./type_defs.md#deleteknowledgebaserequestrequesttypedef) 

### delete\_message\_template

Deletes an Amazon Q in Connect message template entirely or a specific version
of the message template if version is supplied in the request.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_message_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_message_template.html)

```python
# delete_message_template method definition

await def delete_message_template(
    self,
    *,
    knowledgeBaseId: str,
    messageTemplateId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_message_template method usage example with argument unpacking

kwargs: DeleteMessageTemplateRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
}

parent.delete_message_template(**kwargs)
```

1. See [:material-code-braces: DeleteMessageTemplateRequestRequestTypeDef](./type_defs.md#deletemessagetemplaterequestrequesttypedef) 

### delete\_message\_template\_attachment

Deletes the attachment file from the Amazon Q in Connect message template that
is referenced by <code>$LATEST</code> qualifier.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_message_template_attachment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_message_template_attachment.html)

```python
# delete_message_template_attachment method definition

await def delete_message_template_attachment(
    self,
    *,
    attachmentId: str,
    knowledgeBaseId: str,
    messageTemplateId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_message_template_attachment method usage example with argument unpacking

kwargs: DeleteMessageTemplateAttachmentRequestRequestTypeDef = {  # (1)
    "attachmentId": ...,
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
}

parent.delete_message_template_attachment(**kwargs)
```

1. See [:material-code-braces: DeleteMessageTemplateAttachmentRequestRequestTypeDef](./type_defs.md#deletemessagetemplateattachmentrequestrequesttypedef) 

### delete\_quick\_response

Deletes a quick response.

Type annotations and code completion for `#!python session.create_client("qconnect").delete_quick_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/delete_quick_response.html)

```python
# delete_quick_response method definition

await def delete_quick_response(
    self,
    *,
    knowledgeBaseId: str,
    quickResponseId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_quick_response method usage example with argument unpacking

kwargs: DeleteQuickResponseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "quickResponseId": ...,
}

parent.delete_quick_response(**kwargs)
```

1. See [:material-code-braces: DeleteQuickResponseRequestRequestTypeDef](./type_defs.md#deletequickresponserequestrequesttypedef) 

### get\_ai\_agent

Gets an Amazon Q in Connect AI Agent.

Type annotations and code completion for `#!python session.create_client("qconnect").get_ai_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_ai_agent.html)

```python
# get_ai_agent method definition

await def get_ai_agent(
    self,
    *,
    aiAgentId: str,
    assistantId: str,
) -> GetAIAgentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAIAgentResponseTypeDef](./type_defs.md#getaiagentresponsetypedef) 


```python
# get_ai_agent method usage example with argument unpacking

kwargs: GetAIAgentRequestRequestTypeDef = {  # (1)
    "aiAgentId": ...,
    "assistantId": ...,
}

parent.get_ai_agent(**kwargs)
```

1. See [:material-code-braces: GetAIAgentRequestRequestTypeDef](./type_defs.md#getaiagentrequestrequesttypedef) 

### get\_ai\_guardrail

Gets the Amazon Q in Connect AI Guardrail.

Type annotations and code completion for `#!python session.create_client("qconnect").get_ai_guardrail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_ai_guardrail.html)

```python
# get_ai_guardrail method definition

await def get_ai_guardrail(
    self,
    *,
    aiGuardrailId: str,
    assistantId: str,
) -> GetAIGuardrailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAIGuardrailResponseTypeDef](./type_defs.md#getaiguardrailresponsetypedef) 


```python
# get_ai_guardrail method usage example with argument unpacking

kwargs: GetAIGuardrailRequestRequestTypeDef = {  # (1)
    "aiGuardrailId": ...,
    "assistantId": ...,
}

parent.get_ai_guardrail(**kwargs)
```

1. See [:material-code-braces: GetAIGuardrailRequestRequestTypeDef](./type_defs.md#getaiguardrailrequestrequesttypedef) 

### get\_ai\_prompt

Gets and Amazon Q in Connect AI Prompt.

Type annotations and code completion for `#!python session.create_client("qconnect").get_ai_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_ai_prompt.html)

```python
# get_ai_prompt method definition

await def get_ai_prompt(
    self,
    *,
    aiPromptId: str,
    assistantId: str,
) -> GetAIPromptResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAIPromptResponseTypeDef](./type_defs.md#getaipromptresponsetypedef) 


```python
# get_ai_prompt method usage example with argument unpacking

kwargs: GetAIPromptRequestRequestTypeDef = {  # (1)
    "aiPromptId": ...,
    "assistantId": ...,
}

parent.get_ai_prompt(**kwargs)
```

1. See [:material-code-braces: GetAIPromptRequestRequestTypeDef](./type_defs.md#getaipromptrequestrequesttypedef) 

### get\_assistant

Retrieves information about an assistant.

Type annotations and code completion for `#!python session.create_client("qconnect").get_assistant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_assistant.html)

```python
# get_assistant method definition

await def get_assistant(
    self,
    *,
    assistantId: str,
) -> GetAssistantResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssistantResponseTypeDef](./type_defs.md#getassistantresponsetypedef) 


```python
# get_assistant method usage example with argument unpacking

kwargs: GetAssistantRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
}

parent.get_assistant(**kwargs)
```

1. See [:material-code-braces: GetAssistantRequestRequestTypeDef](./type_defs.md#getassistantrequestrequesttypedef) 

### get\_assistant\_association

Retrieves information about an assistant association.

Type annotations and code completion for `#!python session.create_client("qconnect").get_assistant_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_assistant_association.html)

```python
# get_assistant_association method definition

await def get_assistant_association(
    self,
    *,
    assistantAssociationId: str,
    assistantId: str,
) -> GetAssistantAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssistantAssociationResponseTypeDef](./type_defs.md#getassistantassociationresponsetypedef) 


```python
# get_assistant_association method usage example with argument unpacking

kwargs: GetAssistantAssociationRequestRequestTypeDef = {  # (1)
    "assistantAssociationId": ...,
    "assistantId": ...,
}

parent.get_assistant_association(**kwargs)
```

1. See [:material-code-braces: GetAssistantAssociationRequestRequestTypeDef](./type_defs.md#getassistantassociationrequestrequesttypedef) 

### get\_content

Retrieves content, including a pre-signed URL to download the content.

Type annotations and code completion for `#!python session.create_client("qconnect").get_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_content.html)

```python
# get_content method definition

await def get_content(
    self,
    *,
    contentId: str,
    knowledgeBaseId: str,
) -> GetContentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContentResponseTypeDef](./type_defs.md#getcontentresponsetypedef) 


```python
# get_content method usage example with argument unpacking

kwargs: GetContentRequestRequestTypeDef = {  # (1)
    "contentId": ...,
    "knowledgeBaseId": ...,
}

parent.get_content(**kwargs)
```

1. See [:material-code-braces: GetContentRequestRequestTypeDef](./type_defs.md#getcontentrequestrequesttypedef) 

### get\_content\_association

Returns the content association.

Type annotations and code completion for `#!python session.create_client("qconnect").get_content_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_content_association.html)

```python
# get_content_association method definition

await def get_content_association(
    self,
    *,
    contentAssociationId: str,
    contentId: str,
    knowledgeBaseId: str,
) -> GetContentAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContentAssociationResponseTypeDef](./type_defs.md#getcontentassociationresponsetypedef) 


```python
# get_content_association method usage example with argument unpacking

kwargs: GetContentAssociationRequestRequestTypeDef = {  # (1)
    "contentAssociationId": ...,
    "contentId": ...,
    "knowledgeBaseId": ...,
}

parent.get_content_association(**kwargs)
```

1. See [:material-code-braces: GetContentAssociationRequestRequestTypeDef](./type_defs.md#getcontentassociationrequestrequesttypedef) 

### get\_content\_summary

Retrieves summary information about the content.

Type annotations and code completion for `#!python session.create_client("qconnect").get_content_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_content_summary.html)

```python
# get_content_summary method definition

await def get_content_summary(
    self,
    *,
    contentId: str,
    knowledgeBaseId: str,
) -> GetContentSummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContentSummaryResponseTypeDef](./type_defs.md#getcontentsummaryresponsetypedef) 


```python
# get_content_summary method usage example with argument unpacking

kwargs: GetContentSummaryRequestRequestTypeDef = {  # (1)
    "contentId": ...,
    "knowledgeBaseId": ...,
}

parent.get_content_summary(**kwargs)
```

1. See [:material-code-braces: GetContentSummaryRequestRequestTypeDef](./type_defs.md#getcontentsummaryrequestrequesttypedef) 

### get\_import\_job

Retrieves the started import job.

Type annotations and code completion for `#!python session.create_client("qconnect").get_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_import_job.html)

```python
# get_import_job method definition

await def get_import_job(
    self,
    *,
    importJobId: str,
    knowledgeBaseId: str,
) -> GetImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImportJobResponseTypeDef](./type_defs.md#getimportjobresponsetypedef) 


```python
# get_import_job method usage example with argument unpacking

kwargs: GetImportJobRequestRequestTypeDef = {  # (1)
    "importJobId": ...,
    "knowledgeBaseId": ...,
}

parent.get_import_job(**kwargs)
```

1. See [:material-code-braces: GetImportJobRequestRequestTypeDef](./type_defs.md#getimportjobrequestrequesttypedef) 

### get\_knowledge\_base

Retrieves information about the knowledge base.

Type annotations and code completion for `#!python session.create_client("qconnect").get_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_knowledge_base.html)

```python
# get_knowledge_base method definition

await def get_knowledge_base(
    self,
    *,
    knowledgeBaseId: str,
) -> GetKnowledgeBaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKnowledgeBaseResponseTypeDef](./type_defs.md#getknowledgebaseresponsetypedef) 


```python
# get_knowledge_base method usage example with argument unpacking

kwargs: GetKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.get_knowledge_base(**kwargs)
```

1. See [:material-code-braces: GetKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getknowledgebaserequestrequesttypedef) 

### get\_message\_template

Retrieves the Amazon Q in Connect message template.

Type annotations and code completion for `#!python session.create_client("qconnect").get_message_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_message_template.html)

```python
# get_message_template method definition

await def get_message_template(
    self,
    *,
    knowledgeBaseId: str,
    messageTemplateId: str,
) -> GetMessageTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMessageTemplateResponseTypeDef](./type_defs.md#getmessagetemplateresponsetypedef) 


```python
# get_message_template method usage example with argument unpacking

kwargs: GetMessageTemplateRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
}

parent.get_message_template(**kwargs)
```

1. See [:material-code-braces: GetMessageTemplateRequestRequestTypeDef](./type_defs.md#getmessagetemplaterequestrequesttypedef) 

### get\_next\_message

Retrieves next message on an Amazon Q in Connect session.

Type annotations and code completion for `#!python session.create_client("qconnect").get_next_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_next_message.html)

```python
# get_next_message method definition

await def get_next_message(
    self,
    *,
    assistantId: str,
    nextMessageToken: str,
    sessionId: str,
) -> GetNextMessageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNextMessageResponseTypeDef](./type_defs.md#getnextmessageresponsetypedef) 


```python
# get_next_message method usage example with argument unpacking

kwargs: GetNextMessageRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "nextMessageToken": ...,
    "sessionId": ...,
}

parent.get_next_message(**kwargs)
```

1. See [:material-code-braces: GetNextMessageRequestRequestTypeDef](./type_defs.md#getnextmessagerequestrequesttypedef) 

### get\_quick\_response

Retrieves the quick response.

Type annotations and code completion for `#!python session.create_client("qconnect").get_quick_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_quick_response.html)

```python
# get_quick_response method definition

await def get_quick_response(
    self,
    *,
    knowledgeBaseId: str,
    quickResponseId: str,
) -> GetQuickResponseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQuickResponseResponseTypeDef](./type_defs.md#getquickresponseresponsetypedef) 


```python
# get_quick_response method usage example with argument unpacking

kwargs: GetQuickResponseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "quickResponseId": ...,
}

parent.get_quick_response(**kwargs)
```

1. See [:material-code-braces: GetQuickResponseRequestRequestTypeDef](./type_defs.md#getquickresponserequestrequesttypedef) 

### get\_recommendations

This API will be discontinued starting June 1, 2024.

Type annotations and code completion for `#!python session.create_client("qconnect").get_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_recommendations.html)

```python
# get_recommendations method definition

await def get_recommendations(
    self,
    *,
    assistantId: str,
    sessionId: str,
    maxResults: int = ...,
    waitTimeSeconds: int = ...,
) -> GetRecommendationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRecommendationsResponseTypeDef](./type_defs.md#getrecommendationsresponsetypedef) 


```python
# get_recommendations method usage example with argument unpacking

kwargs: GetRecommendationsRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "sessionId": ...,
}

parent.get_recommendations(**kwargs)
```

1. See [:material-code-braces: GetRecommendationsRequestRequestTypeDef](./type_defs.md#getrecommendationsrequestrequesttypedef) 

### get\_session

Retrieves information for a specified session.

Type annotations and code completion for `#!python session.create_client("qconnect").get_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/get_session.html)

```python
# get_session method definition

await def get_session(
    self,
    *,
    assistantId: str,
    sessionId: str,
) -> GetSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef) 


```python
# get_session method usage example with argument unpacking

kwargs: GetSessionRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "sessionId": ...,
}

parent.get_session(**kwargs)
```

1. See [:material-code-braces: GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef) 

### list\_ai\_agent\_versions

List AI Agent versions.

Type annotations and code completion for `#!python session.create_client("qconnect").list_ai_agent_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_ai_agent_versions.html)

```python
# list_ai_agent_versions method definition

await def list_ai_agent_versions(
    self,
    *,
    aiAgentId: str,
    assistantId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    origin: OriginType = ...,  # (1)
) -> ListAIAgentVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: ListAIAgentVersionsResponseTypeDef](./type_defs.md#listaiagentversionsresponsetypedef) 


```python
# list_ai_agent_versions method usage example with argument unpacking

kwargs: ListAIAgentVersionsRequestRequestTypeDef = {  # (1)
    "aiAgentId": ...,
    "assistantId": ...,
}

parent.list_ai_agent_versions(**kwargs)
```

1. See [:material-code-braces: ListAIAgentVersionsRequestRequestTypeDef](./type_defs.md#listaiagentversionsrequestrequesttypedef) 

### list\_ai\_agents

Lists AI Agents.

Type annotations and code completion for `#!python session.create_client("qconnect").list_ai_agents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_ai_agents.html)

```python
# list_ai_agents method definition

await def list_ai_agents(
    self,
    *,
    assistantId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    origin: OriginType = ...,  # (1)
) -> ListAIAgentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: ListAIAgentsResponseTypeDef](./type_defs.md#listaiagentsresponsetypedef) 


```python
# list_ai_agents method usage example with argument unpacking

kwargs: ListAIAgentsRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
}

parent.list_ai_agents(**kwargs)
```

1. See [:material-code-braces: ListAIAgentsRequestRequestTypeDef](./type_defs.md#listaiagentsrequestrequesttypedef) 

### list\_ai\_guardrail\_versions

Lists AI Guardrail versions.

Type annotations and code completion for `#!python session.create_client("qconnect").list_ai_guardrail_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_ai_guardrail_versions.html)

```python
# list_ai_guardrail_versions method definition

await def list_ai_guardrail_versions(
    self,
    *,
    aiGuardrailId: str,
    assistantId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAIGuardrailVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAIGuardrailVersionsResponseTypeDef](./type_defs.md#listaiguardrailversionsresponsetypedef) 


```python
# list_ai_guardrail_versions method usage example with argument unpacking

kwargs: ListAIGuardrailVersionsRequestRequestTypeDef = {  # (1)
    "aiGuardrailId": ...,
    "assistantId": ...,
}

parent.list_ai_guardrail_versions(**kwargs)
```

1. See [:material-code-braces: ListAIGuardrailVersionsRequestRequestTypeDef](./type_defs.md#listaiguardrailversionsrequestrequesttypedef) 

### list\_ai\_guardrails

Lists the AI Guardrails available on the Amazon Q in Connect assistant.

Type annotations and code completion for `#!python session.create_client("qconnect").list_ai_guardrails` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_ai_guardrails.html)

```python
# list_ai_guardrails method definition

await def list_ai_guardrails(
    self,
    *,
    assistantId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAIGuardrailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAIGuardrailsResponseTypeDef](./type_defs.md#listaiguardrailsresponsetypedef) 


```python
# list_ai_guardrails method usage example with argument unpacking

kwargs: ListAIGuardrailsRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
}

parent.list_ai_guardrails(**kwargs)
```

1. See [:material-code-braces: ListAIGuardrailsRequestRequestTypeDef](./type_defs.md#listaiguardrailsrequestrequesttypedef) 

### list\_ai\_prompt\_versions

Lists AI Prompt versions.

Type annotations and code completion for `#!python session.create_client("qconnect").list_ai_prompt_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_ai_prompt_versions.html)

```python
# list_ai_prompt_versions method definition

await def list_ai_prompt_versions(
    self,
    *,
    aiPromptId: str,
    assistantId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    origin: OriginType = ...,  # (1)
) -> ListAIPromptVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: ListAIPromptVersionsResponseTypeDef](./type_defs.md#listaipromptversionsresponsetypedef) 


```python
# list_ai_prompt_versions method usage example with argument unpacking

kwargs: ListAIPromptVersionsRequestRequestTypeDef = {  # (1)
    "aiPromptId": ...,
    "assistantId": ...,
}

parent.list_ai_prompt_versions(**kwargs)
```

1. See [:material-code-braces: ListAIPromptVersionsRequestRequestTypeDef](./type_defs.md#listaipromptversionsrequestrequesttypedef) 

### list\_ai\_prompts

Lists the AI Prompts available on the Amazon Q in Connect assistant.

Type annotations and code completion for `#!python session.create_client("qconnect").list_ai_prompts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_ai_prompts.html)

```python
# list_ai_prompts method definition

await def list_ai_prompts(
    self,
    *,
    assistantId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    origin: OriginType = ...,  # (1)
) -> ListAIPromptsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: ListAIPromptsResponseTypeDef](./type_defs.md#listaipromptsresponsetypedef) 


```python
# list_ai_prompts method usage example with argument unpacking

kwargs: ListAIPromptsRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
}

parent.list_ai_prompts(**kwargs)
```

1. See [:material-code-braces: ListAIPromptsRequestRequestTypeDef](./type_defs.md#listaipromptsrequestrequesttypedef) 

### list\_assistant\_associations

Lists information about assistant associations.

Type annotations and code completion for `#!python session.create_client("qconnect").list_assistant_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_assistant_associations.html)

```python
# list_assistant_associations method definition

await def list_assistant_associations(
    self,
    *,
    assistantId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAssistantAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssistantAssociationsResponseTypeDef](./type_defs.md#listassistantassociationsresponsetypedef) 


```python
# list_assistant_associations method usage example with argument unpacking

kwargs: ListAssistantAssociationsRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
}

parent.list_assistant_associations(**kwargs)
```

1. See [:material-code-braces: ListAssistantAssociationsRequestRequestTypeDef](./type_defs.md#listassistantassociationsrequestrequesttypedef) 

### list\_assistants

Lists information about assistants.

Type annotations and code completion for `#!python session.create_client("qconnect").list_assistants` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_assistants.html)

```python
# list_assistants method definition

await def list_assistants(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAssistantsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssistantsResponseTypeDef](./type_defs.md#listassistantsresponsetypedef) 


```python
# list_assistants method usage example with argument unpacking

kwargs: ListAssistantsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_assistants(**kwargs)
```

1. See [:material-code-braces: ListAssistantsRequestRequestTypeDef](./type_defs.md#listassistantsrequestrequesttypedef) 

### list\_content\_associations

Lists the content associations.

Type annotations and code completion for `#!python session.create_client("qconnect").list_content_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_content_associations.html)

```python
# list_content_associations method definition

await def list_content_associations(
    self,
    *,
    contentId: str,
    knowledgeBaseId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListContentAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListContentAssociationsResponseTypeDef](./type_defs.md#listcontentassociationsresponsetypedef) 


```python
# list_content_associations method usage example with argument unpacking

kwargs: ListContentAssociationsRequestRequestTypeDef = {  # (1)
    "contentId": ...,
    "knowledgeBaseId": ...,
}

parent.list_content_associations(**kwargs)
```

1. See [:material-code-braces: ListContentAssociationsRequestRequestTypeDef](./type_defs.md#listcontentassociationsrequestrequesttypedef) 

### list\_contents

Lists the content.

Type annotations and code completion for `#!python session.create_client("qconnect").list_contents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_contents.html)

```python
# list_contents method definition

await def list_contents(
    self,
    *,
    knowledgeBaseId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListContentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListContentsResponseTypeDef](./type_defs.md#listcontentsresponsetypedef) 


```python
# list_contents method usage example with argument unpacking

kwargs: ListContentsRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.list_contents(**kwargs)
```

1. See [:material-code-braces: ListContentsRequestRequestTypeDef](./type_defs.md#listcontentsrequestrequesttypedef) 

### list\_import\_jobs

Lists information about import jobs.

Type annotations and code completion for `#!python session.create_client("qconnect").list_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_import_jobs.html)

```python
# list_import_jobs method definition

await def list_import_jobs(
    self,
    *,
    knowledgeBaseId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListImportJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListImportJobsResponseTypeDef](./type_defs.md#listimportjobsresponsetypedef) 


```python
# list_import_jobs method usage example with argument unpacking

kwargs: ListImportJobsRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.list_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListImportJobsRequestRequestTypeDef](./type_defs.md#listimportjobsrequestrequesttypedef) 

### list\_knowledge\_bases

Lists the knowledge bases.

Type annotations and code completion for `#!python session.create_client("qconnect").list_knowledge_bases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_knowledge_bases.html)

```python
# list_knowledge_bases method definition

await def list_knowledge_bases(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListKnowledgeBasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef) 


```python
# list_knowledge_bases method usage example with argument unpacking

kwargs: ListKnowledgeBasesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_knowledge_bases(**kwargs)
```

1. See [:material-code-braces: ListKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listknowledgebasesrequestrequesttypedef) 

### list\_message\_template\_versions

Lists all the available versions for the specified Amazon Q in Connect message
template.

Type annotations and code completion for `#!python session.create_client("qconnect").list_message_template_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_message_template_versions.html)

```python
# list_message_template_versions method definition

await def list_message_template_versions(
    self,
    *,
    knowledgeBaseId: str,
    messageTemplateId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMessageTemplateVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMessageTemplateVersionsResponseTypeDef](./type_defs.md#listmessagetemplateversionsresponsetypedef) 


```python
# list_message_template_versions method usage example with argument unpacking

kwargs: ListMessageTemplateVersionsRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
}

parent.list_message_template_versions(**kwargs)
```

1. See [:material-code-braces: ListMessageTemplateVersionsRequestRequestTypeDef](./type_defs.md#listmessagetemplateversionsrequestrequesttypedef) 

### list\_message\_templates

Lists all the available Amazon Q in Connect message templates for the specified
knowledge base.

Type annotations and code completion for `#!python session.create_client("qconnect").list_message_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_message_templates.html)

```python
# list_message_templates method definition

await def list_message_templates(
    self,
    *,
    knowledgeBaseId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMessageTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMessageTemplatesResponseTypeDef](./type_defs.md#listmessagetemplatesresponsetypedef) 


```python
# list_message_templates method usage example with argument unpacking

kwargs: ListMessageTemplatesRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.list_message_templates(**kwargs)
```

1. See [:material-code-braces: ListMessageTemplatesRequestRequestTypeDef](./type_defs.md#listmessagetemplatesrequestrequesttypedef) 

### list\_messages

Lists messages on an Amazon Q in Connect session.

Type annotations and code completion for `#!python session.create_client("qconnect").list_messages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_messages.html)

```python
# list_messages method definition

await def list_messages(
    self,
    *,
    assistantId: str,
    sessionId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMessagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMessagesResponseTypeDef](./type_defs.md#listmessagesresponsetypedef) 


```python
# list_messages method usage example with argument unpacking

kwargs: ListMessagesRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "sessionId": ...,
}

parent.list_messages(**kwargs)
```

1. See [:material-code-braces: ListMessagesRequestRequestTypeDef](./type_defs.md#listmessagesrequestrequesttypedef) 

### list\_quick\_responses

Lists information about quick response.

Type annotations and code completion for `#!python session.create_client("qconnect").list_quick_responses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_quick_responses.html)

```python
# list_quick_responses method definition

await def list_quick_responses(
    self,
    *,
    knowledgeBaseId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListQuickResponsesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListQuickResponsesResponseTypeDef](./type_defs.md#listquickresponsesresponsetypedef) 


```python
# list_quick_responses method usage example with argument unpacking

kwargs: ListQuickResponsesRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.list_quick_responses(**kwargs)
```

1. See [:material-code-braces: ListQuickResponsesRequestRequestTypeDef](./type_defs.md#listquickresponsesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("qconnect").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/list_tags_for_resource.html)

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

### notify\_recommendations\_received

Removes the specified recommendations from the specified assistant's queue of
newly available recommendations.

Type annotations and code completion for `#!python session.create_client("qconnect").notify_recommendations_received` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/notify_recommendations_received.html)

```python
# notify_recommendations_received method definition

await def notify_recommendations_received(
    self,
    *,
    assistantId: str,
    recommendationIds: Sequence[str],
    sessionId: str,
) -> NotifyRecommendationsReceivedResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: NotifyRecommendationsReceivedResponseTypeDef](./type_defs.md#notifyrecommendationsreceivedresponsetypedef) 


```python
# notify_recommendations_received method usage example with argument unpacking

kwargs: NotifyRecommendationsReceivedRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "recommendationIds": ...,
    "sessionId": ...,
}

parent.notify_recommendations_received(**kwargs)
```

1. See [:material-code-braces: NotifyRecommendationsReceivedRequestRequestTypeDef](./type_defs.md#notifyrecommendationsreceivedrequestrequesttypedef) 

### put\_feedback

Provides feedback against the specified assistant for the specified target.

Type annotations and code completion for `#!python session.create_client("qconnect").put_feedback` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/put_feedback.html)

```python
# put_feedback method definition

await def put_feedback(
    self,
    *,
    assistantId: str,
    contentFeedback: ContentFeedbackDataTypeDef,  # (1)
    targetId: str,
    targetType: TargetTypeType,  # (2)
) -> PutFeedbackResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ContentFeedbackDataTypeDef](./type_defs.md#contentfeedbackdatatypedef) 
2. See [:material-code-brackets: TargetTypeType](./literals.md#targettypetype) 
3. See [:material-code-braces: PutFeedbackResponseTypeDef](./type_defs.md#putfeedbackresponsetypedef) 


```python
# put_feedback method usage example with argument unpacking

kwargs: PutFeedbackRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "contentFeedback": ...,
    "targetId": ...,
    "targetType": ...,
}

parent.put_feedback(**kwargs)
```

1. See [:material-code-braces: PutFeedbackRequestRequestTypeDef](./type_defs.md#putfeedbackrequestrequesttypedef) 

### query\_assistant

This API will be discontinued starting June 1, 2024.

Type annotations and code completion for `#!python session.create_client("qconnect").query_assistant` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/query_assistant.html)

```python
# query_assistant method definition

await def query_assistant(
    self,
    *,
    assistantId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    overrideKnowledgeBaseSearchType: KnowledgeBaseSearchTypeType = ...,  # (1)
    queryCondition: Sequence[QueryConditionTypeDef] = ...,  # (2)
    queryInputData: QueryInputDataTypeDef = ...,  # (3)
    queryText: str = ...,
    sessionId: str = ...,
) -> QueryAssistantResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: KnowledgeBaseSearchTypeType](./literals.md#knowledgebasesearchtypetype) 
2. See [:material-code-braces: QueryConditionTypeDef](./type_defs.md#queryconditiontypedef) 
3. See [:material-code-braces: QueryInputDataTypeDef](./type_defs.md#queryinputdatatypedef) 
4. See [:material-code-braces: QueryAssistantResponseTypeDef](./type_defs.md#queryassistantresponsetypedef) 


```python
# query_assistant method usage example with argument unpacking

kwargs: QueryAssistantRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
}

parent.query_assistant(**kwargs)
```

1. See [:material-code-braces: QueryAssistantRequestRequestTypeDef](./type_defs.md#queryassistantrequestrequesttypedef) 

### remove\_assistant\_ai\_agent

Removes the AI Agent that is set for use by defafult on an Amazon Q in Connect
Assistant.

Type annotations and code completion for `#!python session.create_client("qconnect").remove_assistant_ai_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/remove_assistant_ai_agent.html)

```python
# remove_assistant_ai_agent method definition

await def remove_assistant_ai_agent(
    self,
    *,
    aiAgentType: AIAgentTypeType,  # (1)
    assistantId: str,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) 


```python
# remove_assistant_ai_agent method usage example with argument unpacking

kwargs: RemoveAssistantAIAgentRequestRequestTypeDef = {  # (1)
    "aiAgentType": ...,
    "assistantId": ...,
}

parent.remove_assistant_ai_agent(**kwargs)
```

1. See [:material-code-braces: RemoveAssistantAIAgentRequestRequestTypeDef](./type_defs.md#removeassistantaiagentrequestrequesttypedef) 

### remove\_knowledge\_base\_template\_uri

Removes a URI template from a knowledge base.

Type annotations and code completion for `#!python session.create_client("qconnect").remove_knowledge_base_template_uri` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/remove_knowledge_base_template_uri.html)

```python
# remove_knowledge_base_template_uri method definition

await def remove_knowledge_base_template_uri(
    self,
    *,
    knowledgeBaseId: str,
) -> Dict[str, Any]:
    ...
```



```python
# remove_knowledge_base_template_uri method usage example with argument unpacking

kwargs: RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.remove_knowledge_base_template_uri(**kwargs)
```

1. See [:material-code-braces: RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef](./type_defs.md#removeknowledgebasetemplateurirequestrequesttypedef) 

### render\_message\_template

Renders the Amazon Q in Connect message template based on the attribute values
provided and generates the message content.

Type annotations and code completion for `#!python session.create_client("qconnect").render_message_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/render_message_template.html)

```python
# render_message_template method definition

await def render_message_template(
    self,
    *,
    attributes: MessageTemplateAttributesTypeDef,  # (1)
    knowledgeBaseId: str,
    messageTemplateId: str,
) -> RenderMessageTemplateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MessageTemplateAttributesTypeDef](./type_defs.md#messagetemplateattributestypedef) 
2. See [:material-code-braces: RenderMessageTemplateResponseTypeDef](./type_defs.md#rendermessagetemplateresponsetypedef) 


```python
# render_message_template method usage example with argument unpacking

kwargs: RenderMessageTemplateRequestRequestTypeDef = {  # (1)
    "attributes": ...,
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
}

parent.render_message_template(**kwargs)
```

1. See [:material-code-braces: RenderMessageTemplateRequestRequestTypeDef](./type_defs.md#rendermessagetemplaterequestrequesttypedef) 

### search\_content

Searches for content in a specified knowledge base.

Type annotations and code completion for `#!python session.create_client("qconnect").search_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/search_content.html)

```python
# search_content method definition

await def search_content(
    self,
    *,
    knowledgeBaseId: str,
    searchExpression: SearchExpressionTypeDef,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchContentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
2. See [:material-code-braces: SearchContentResponseTypeDef](./type_defs.md#searchcontentresponsetypedef) 


```python
# search_content method usage example with argument unpacking

kwargs: SearchContentRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "searchExpression": ...,
}

parent.search_content(**kwargs)
```

1. See [:material-code-braces: SearchContentRequestRequestTypeDef](./type_defs.md#searchcontentrequestrequesttypedef) 

### search\_message\_templates

Searches for Amazon Q in Connect message templates in the specified knowledge
base.

Type annotations and code completion for `#!python session.create_client("qconnect").search_message_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/search_message_templates.html)

```python
# search_message_templates method definition

await def search_message_templates(
    self,
    *,
    knowledgeBaseId: str,
    searchExpression: MessageTemplateSearchExpressionTypeDef,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchMessageTemplatesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MessageTemplateSearchExpressionTypeDef](./type_defs.md#messagetemplatesearchexpressiontypedef) 
2. See [:material-code-braces: SearchMessageTemplatesResponseTypeDef](./type_defs.md#searchmessagetemplatesresponsetypedef) 


```python
# search_message_templates method usage example with argument unpacking

kwargs: SearchMessageTemplatesRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "searchExpression": ...,
}

parent.search_message_templates(**kwargs)
```

1. See [:material-code-braces: SearchMessageTemplatesRequestRequestTypeDef](./type_defs.md#searchmessagetemplatesrequestrequesttypedef) 

### search\_quick\_responses

Searches existing Amazon Q in Connect quick responses in an Amazon Q in Connect
knowledge base.

Type annotations and code completion for `#!python session.create_client("qconnect").search_quick_responses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/search_quick_responses.html)

```python
# search_quick_responses method definition

await def search_quick_responses(
    self,
    *,
    knowledgeBaseId: str,
    searchExpression: QuickResponseSearchExpressionTypeDef,  # (1)
    attributes: Mapping[str, str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchQuickResponsesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: QuickResponseSearchExpressionTypeDef](./type_defs.md#quickresponsesearchexpressiontypedef) 
2. See [:material-code-braces: SearchQuickResponsesResponseTypeDef](./type_defs.md#searchquickresponsesresponsetypedef) 


```python
# search_quick_responses method usage example with argument unpacking

kwargs: SearchQuickResponsesRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "searchExpression": ...,
}

parent.search_quick_responses(**kwargs)
```

1. See [:material-code-braces: SearchQuickResponsesRequestRequestTypeDef](./type_defs.md#searchquickresponsesrequestrequesttypedef) 

### search\_sessions

Searches for sessions.

Type annotations and code completion for `#!python session.create_client("qconnect").search_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/search_sessions.html)

```python
# search_sessions method definition

await def search_sessions(
    self,
    *,
    assistantId: str,
    searchExpression: SearchExpressionTypeDef,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> SearchSessionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
2. See [:material-code-braces: SearchSessionsResponseTypeDef](./type_defs.md#searchsessionsresponsetypedef) 


```python
# search_sessions method usage example with argument unpacking

kwargs: SearchSessionsRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "searchExpression": ...,
}

parent.search_sessions(**kwargs)
```

1. See [:material-code-braces: SearchSessionsRequestRequestTypeDef](./type_defs.md#searchsessionsrequestrequesttypedef) 

### send\_message

Submits a message to the Amazon Q in Connect session.

Type annotations and code completion for `#!python session.create_client("qconnect").send_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/send_message.html)

```python
# send_message method definition

await def send_message(
    self,
    *,
    assistantId: str,
    message: MessageInputTypeDef,  # (1)
    sessionId: str,
    type: MessageTypeType,  # (2)
    clientToken: str = ...,
    conversationContext: ConversationContextTypeDef = ...,  # (3)
) -> SendMessageResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: MessageInputTypeDef](./type_defs.md#messageinputtypedef) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-braces: ConversationContextTypeDef](./type_defs.md#conversationcontexttypedef) 
4. See [:material-code-braces: SendMessageResponseTypeDef](./type_defs.md#sendmessageresponsetypedef) 


```python
# send_message method usage example with argument unpacking

kwargs: SendMessageRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "message": ...,
    "sessionId": ...,
    "type": ...,
}

parent.send_message(**kwargs)
```

1. See [:material-code-braces: SendMessageRequestRequestTypeDef](./type_defs.md#sendmessagerequestrequesttypedef) 

### start\_content\_upload

Get a URL to upload content to a knowledge base.

Type annotations and code completion for `#!python session.create_client("qconnect").start_content_upload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/start_content_upload.html)

```python
# start_content_upload method definition

await def start_content_upload(
    self,
    *,
    contentType: str,
    knowledgeBaseId: str,
    presignedUrlTimeToLive: int = ...,
) -> StartContentUploadResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartContentUploadResponseTypeDef](./type_defs.md#startcontentuploadresponsetypedef) 


```python
# start_content_upload method usage example with argument unpacking

kwargs: StartContentUploadRequestRequestTypeDef = {  # (1)
    "contentType": ...,
    "knowledgeBaseId": ...,
}

parent.start_content_upload(**kwargs)
```

1. See [:material-code-braces: StartContentUploadRequestRequestTypeDef](./type_defs.md#startcontentuploadrequestrequesttypedef) 

### start\_import\_job

Start an asynchronous job to import Amazon Q in Connect resources from an
uploaded source file.

Type annotations and code completion for `#!python session.create_client("qconnect").start_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/start_import_job.html)

```python
# start_import_job method definition

await def start_import_job(
    self,
    *,
    importJobType: ImportJobTypeType,  # (1)
    knowledgeBaseId: str,
    uploadId: str,
    clientToken: str = ...,
    externalSourceConfiguration: ExternalSourceConfigurationTypeDef = ...,  # (2)
    metadata: Mapping[str, str] = ...,
) -> StartImportJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ImportJobTypeType](./literals.md#importjobtypetype) 
2. See [:material-code-braces: ExternalSourceConfigurationTypeDef](./type_defs.md#externalsourceconfigurationtypedef) 
3. See [:material-code-braces: StartImportJobResponseTypeDef](./type_defs.md#startimportjobresponsetypedef) 


```python
# start_import_job method usage example with argument unpacking

kwargs: StartImportJobRequestRequestTypeDef = {  # (1)
    "importJobType": ...,
    "knowledgeBaseId": ...,
    "uploadId": ...,
}

parent.start_import_job(**kwargs)
```

1. See [:material-code-braces: StartImportJobRequestRequestTypeDef](./type_defs.md#startimportjobrequestrequesttypedef) 

### tag\_resource

Adds the specified tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("qconnect").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/tag_resource.html)

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

Removes the specified tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("qconnect").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/untag_resource.html)

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

### update\_ai\_agent

Updates an AI Agent.

Type annotations and code completion for `#!python session.create_client("qconnect").update_ai_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_ai_agent.html)

```python
# update_ai_agent method definition

await def update_ai_agent(
    self,
    *,
    aiAgentId: str,
    assistantId: str,
    visibilityStatus: VisibilityStatusType,  # (1)
    clientToken: str = ...,
    configuration: AIAgentConfigurationTypeDef = ...,  # (2)
    description: str = ...,
) -> UpdateAIAgentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
2. See [:material-code-braces: AIAgentConfigurationTypeDef](./type_defs.md#aiagentconfigurationtypedef) 
3. See [:material-code-braces: UpdateAIAgentResponseTypeDef](./type_defs.md#updateaiagentresponsetypedef) 


```python
# update_ai_agent method usage example with argument unpacking

kwargs: UpdateAIAgentRequestRequestTypeDef = {  # (1)
    "aiAgentId": ...,
    "assistantId": ...,
    "visibilityStatus": ...,
}

parent.update_ai_agent(**kwargs)
```

1. See [:material-code-braces: UpdateAIAgentRequestRequestTypeDef](./type_defs.md#updateaiagentrequestrequesttypedef) 

### update\_ai\_guardrail

Updates an AI Guardrail.

Type annotations and code completion for `#!python session.create_client("qconnect").update_ai_guardrail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_ai_guardrail.html)

```python
# update_ai_guardrail method definition

await def update_ai_guardrail(
    self,
    *,
    aiGuardrailId: str,
    assistantId: str,
    blockedInputMessaging: str,
    blockedOutputsMessaging: str,
    visibilityStatus: VisibilityStatusType,  # (1)
    clientToken: str = ...,
    contentPolicyConfig: AIGuardrailContentPolicyConfigTypeDef = ...,  # (2)
    contextualGroundingPolicyConfig: AIGuardrailContextualGroundingPolicyConfigTypeDef = ...,  # (3)
    description: str = ...,
    sensitiveInformationPolicyConfig: AIGuardrailSensitiveInformationPolicyConfigTypeDef = ...,  # (4)
    topicPolicyConfig: AIGuardrailTopicPolicyConfigTypeDef = ...,  # (5)
    wordPolicyConfig: AIGuardrailWordPolicyConfigTypeDef = ...,  # (6)
) -> UpdateAIGuardrailResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
2. See [:material-code-braces: AIGuardrailContentPolicyConfigTypeDef](./type_defs.md#aiguardrailcontentpolicyconfigtypedef) 
3. See [:material-code-braces: AIGuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#aiguardrailcontextualgroundingpolicyconfigtypedef) 
4. See [:material-code-braces: AIGuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#aiguardrailsensitiveinformationpolicyconfigtypedef) 
5. See [:material-code-braces: AIGuardrailTopicPolicyConfigTypeDef](./type_defs.md#aiguardrailtopicpolicyconfigtypedef) 
6. See [:material-code-braces: AIGuardrailWordPolicyConfigTypeDef](./type_defs.md#aiguardrailwordpolicyconfigtypedef) 
7. See [:material-code-braces: UpdateAIGuardrailResponseTypeDef](./type_defs.md#updateaiguardrailresponsetypedef) 


```python
# update_ai_guardrail method usage example with argument unpacking

kwargs: UpdateAIGuardrailRequestRequestTypeDef = {  # (1)
    "aiGuardrailId": ...,
    "assistantId": ...,
    "blockedInputMessaging": ...,
    "blockedOutputsMessaging": ...,
    "visibilityStatus": ...,
}

parent.update_ai_guardrail(**kwargs)
```

1. See [:material-code-braces: UpdateAIGuardrailRequestRequestTypeDef](./type_defs.md#updateaiguardrailrequestrequesttypedef) 

### update\_ai\_prompt

Updates an AI Prompt.

Type annotations and code completion for `#!python session.create_client("qconnect").update_ai_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_ai_prompt.html)

```python
# update_ai_prompt method definition

await def update_ai_prompt(
    self,
    *,
    aiPromptId: str,
    assistantId: str,
    visibilityStatus: VisibilityStatusType,  # (1)
    clientToken: str = ...,
    description: str = ...,
    templateConfiguration: AIPromptTemplateConfigurationTypeDef = ...,  # (2)
) -> UpdateAIPromptResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: VisibilityStatusType](./literals.md#visibilitystatustype) 
2. See [:material-code-braces: AIPromptTemplateConfigurationTypeDef](./type_defs.md#aiprompttemplateconfigurationtypedef) 
3. See [:material-code-braces: UpdateAIPromptResponseTypeDef](./type_defs.md#updateaipromptresponsetypedef) 


```python
# update_ai_prompt method usage example with argument unpacking

kwargs: UpdateAIPromptRequestRequestTypeDef = {  # (1)
    "aiPromptId": ...,
    "assistantId": ...,
    "visibilityStatus": ...,
}

parent.update_ai_prompt(**kwargs)
```

1. See [:material-code-braces: UpdateAIPromptRequestRequestTypeDef](./type_defs.md#updateaipromptrequestrequesttypedef) 

### update\_assistant\_ai\_agent

Updates the AI Agent that is set for use by defafult on an Amazon Q in Connect
Assistant.

Type annotations and code completion for `#!python session.create_client("qconnect").update_assistant_ai_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_assistant_ai_agent.html)

```python
# update_assistant_ai_agent method definition

await def update_assistant_ai_agent(
    self,
    *,
    aiAgentType: AIAgentTypeType,  # (1)
    assistantId: str,
    configuration: AIAgentConfigurationDataTypeDef,  # (2)
) -> UpdateAssistantAIAgentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) 
2. See [:material-code-braces: AIAgentConfigurationDataTypeDef](./type_defs.md#aiagentconfigurationdatatypedef) 
3. See [:material-code-braces: UpdateAssistantAIAgentResponseTypeDef](./type_defs.md#updateassistantaiagentresponsetypedef) 


```python
# update_assistant_ai_agent method usage example with argument unpacking

kwargs: UpdateAssistantAIAgentRequestRequestTypeDef = {  # (1)
    "aiAgentType": ...,
    "assistantId": ...,
    "configuration": ...,
}

parent.update_assistant_ai_agent(**kwargs)
```

1. See [:material-code-braces: UpdateAssistantAIAgentRequestRequestTypeDef](./type_defs.md#updateassistantaiagentrequestrequesttypedef) 

### update\_content

Updates information about the content.

Type annotations and code completion for `#!python session.create_client("qconnect").update_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_content.html)

```python
# update_content method definition

await def update_content(
    self,
    *,
    contentId: str,
    knowledgeBaseId: str,
    metadata: Mapping[str, str] = ...,
    overrideLinkOutUri: str = ...,
    removeOverrideLinkOutUri: bool = ...,
    revisionId: str = ...,
    title: str = ...,
    uploadId: str = ...,
) -> UpdateContentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateContentResponseTypeDef](./type_defs.md#updatecontentresponsetypedef) 


```python
# update_content method usage example with argument unpacking

kwargs: UpdateContentRequestRequestTypeDef = {  # (1)
    "contentId": ...,
    "knowledgeBaseId": ...,
}

parent.update_content(**kwargs)
```

1. See [:material-code-braces: UpdateContentRequestRequestTypeDef](./type_defs.md#updatecontentrequestrequesttypedef) 

### update\_knowledge\_base\_template\_uri

Updates the template URI of a knowledge base.

Type annotations and code completion for `#!python session.create_client("qconnect").update_knowledge_base_template_uri` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_knowledge_base_template_uri.html)

```python
# update_knowledge_base_template_uri method definition

await def update_knowledge_base_template_uri(
    self,
    *,
    knowledgeBaseId: str,
    templateUri: str,
) -> UpdateKnowledgeBaseTemplateUriResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateKnowledgeBaseTemplateUriResponseTypeDef](./type_defs.md#updateknowledgebasetemplateuriresponsetypedef) 


```python
# update_knowledge_base_template_uri method usage example with argument unpacking

kwargs: UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "templateUri": ...,
}

parent.update_knowledge_base_template_uri(**kwargs)
```

1. See [:material-code-braces: UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef](./type_defs.md#updateknowledgebasetemplateurirequestrequesttypedef) 

### update\_message\_template

Updates the Amazon Q in Connect message template.

Type annotations and code completion for `#!python session.create_client("qconnect").update_message_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_message_template.html)

```python
# update_message_template method definition

await def update_message_template(
    self,
    *,
    knowledgeBaseId: str,
    messageTemplateId: str,
    content: MessageTemplateContentProviderTypeDef = ...,  # (1)
    defaultAttributes: MessageTemplateAttributesTypeDef = ...,  # (2)
    language: str = ...,
) -> UpdateMessageTemplateResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MessageTemplateContentProviderTypeDef](./type_defs.md#messagetemplatecontentprovidertypedef) 
2. See [:material-code-braces: MessageTemplateAttributesTypeDef](./type_defs.md#messagetemplateattributestypedef) 
3. See [:material-code-braces: UpdateMessageTemplateResponseTypeDef](./type_defs.md#updatemessagetemplateresponsetypedef) 


```python
# update_message_template method usage example with argument unpacking

kwargs: UpdateMessageTemplateRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
}

parent.update_message_template(**kwargs)
```

1. See [:material-code-braces: UpdateMessageTemplateRequestRequestTypeDef](./type_defs.md#updatemessagetemplaterequestrequesttypedef) 

### update\_message\_template\_metadata

Updates the Amazon Q in Connect message template metadata.

Type annotations and code completion for `#!python session.create_client("qconnect").update_message_template_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_message_template_metadata.html)

```python
# update_message_template_metadata method definition

await def update_message_template_metadata(
    self,
    *,
    knowledgeBaseId: str,
    messageTemplateId: str,
    description: str = ...,
    groupingConfiguration: GroupingConfigurationTypeDef = ...,  # (1)
    name: str = ...,
) -> UpdateMessageTemplateMetadataResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef) 
2. See [:material-code-braces: UpdateMessageTemplateMetadataResponseTypeDef](./type_defs.md#updatemessagetemplatemetadataresponsetypedef) 


```python
# update_message_template_metadata method usage example with argument unpacking

kwargs: UpdateMessageTemplateMetadataRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
}

parent.update_message_template_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateMessageTemplateMetadataRequestRequestTypeDef](./type_defs.md#updatemessagetemplatemetadatarequestrequesttypedef) 

### update\_quick\_response

Updates an existing Amazon Q in Connect quick response.

Type annotations and code completion for `#!python session.create_client("qconnect").update_quick_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_quick_response.html)

```python
# update_quick_response method definition

await def update_quick_response(
    self,
    *,
    knowledgeBaseId: str,
    quickResponseId: str,
    channels: Sequence[str] = ...,
    content: QuickResponseDataProviderTypeDef = ...,  # (1)
    contentType: str = ...,
    description: str = ...,
    groupingConfiguration: GroupingConfigurationTypeDef = ...,  # (2)
    isActive: bool = ...,
    language: str = ...,
    name: str = ...,
    removeDescription: bool = ...,
    removeGroupingConfiguration: bool = ...,
    removeShortcutKey: bool = ...,
    shortcutKey: str = ...,
) -> UpdateQuickResponseResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: QuickResponseDataProviderTypeDef](./type_defs.md#quickresponsedataprovidertypedef) 
2. See [:material-code-braces: GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef) 
3. See [:material-code-braces: UpdateQuickResponseResponseTypeDef](./type_defs.md#updatequickresponseresponsetypedef) 


```python
# update_quick_response method usage example with argument unpacking

kwargs: UpdateQuickResponseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "quickResponseId": ...,
}

parent.update_quick_response(**kwargs)
```

1. See [:material-code-braces: UpdateQuickResponseRequestRequestTypeDef](./type_defs.md#updatequickresponserequestrequesttypedef) 

### update\_session

Updates a session.

Type annotations and code completion for `#!python session.create_client("qconnect").update_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_session.html)

```python
# update_session method definition

await def update_session(
    self,
    *,
    assistantId: str,
    sessionId: str,
    aiAgentConfiguration: Mapping[AIAgentTypeType, AIAgentConfigurationDataTypeDef] = ...,  # (1)
    description: str = ...,
    tagFilter: TagFilterTypeDef = ...,  # (2)
) -> UpdateSessionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AIAgentTypeType](./literals.md#aiagenttypetype) [:material-code-braces: AIAgentConfigurationDataTypeDef](./type_defs.md#aiagentconfigurationdatatypedef) 
2. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
3. See [:material-code-braces: UpdateSessionResponseTypeDef](./type_defs.md#updatesessionresponsetypedef) 


```python
# update_session method usage example with argument unpacking

kwargs: UpdateSessionRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "sessionId": ...,
}

parent.update_session(**kwargs)
```

1. See [:material-code-braces: UpdateSessionRequestRequestTypeDef](./type_defs.md#updatesessionrequestrequesttypedef) 

### update\_session\_data

Updates the data stored on an Amazon Q in Connect Session.

Type annotations and code completion for `#!python session.create_client("qconnect").update_session_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/client/update_session_data.html)

```python
# update_session_data method definition

await def update_session_data(
    self,
    *,
    assistantId: str,
    data: Sequence[RuntimeSessionDataTypeDef],  # (1)
    sessionId: str,
    namespace: SessionDataNamespaceType = ...,  # (2)
) -> UpdateSessionDataResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RuntimeSessionDataTypeDef](./type_defs.md#runtimesessiondatatypedef) 
2. See [:material-code-brackets: SessionDataNamespaceType](./literals.md#sessiondatanamespacetype) 
3. See [:material-code-braces: UpdateSessionDataResponseTypeDef](./type_defs.md#updatesessiondataresponsetypedef) 


```python
# update_session_data method usage example with argument unpacking

kwargs: UpdateSessionDataRequestRequestTypeDef = {  # (1)
    "assistantId": ...,
    "data": ...,
    "sessionId": ...,
}

parent.update_session_data(**kwargs)
```

1. See [:material-code-braces: UpdateSessionDataRequestRequestTypeDef](./type_defs.md#updatesessiondatarequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("qconnect").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("qconnect").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client)

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

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator` method with overloads.

- `client.get_paginator("list_ai_agent_versions")` -> [ListAIAgentVersionsPaginator](./paginators.md#listaiagentversionspaginator)
- `client.get_paginator("list_ai_agents")` -> [ListAIAgentsPaginator](./paginators.md#listaiagentspaginator)
- `client.get_paginator("list_ai_guardrail_versions")` -> [ListAIGuardrailVersionsPaginator](./paginators.md#listaiguardrailversionspaginator)
- `client.get_paginator("list_ai_guardrails")` -> [ListAIGuardrailsPaginator](./paginators.md#listaiguardrailspaginator)
- `client.get_paginator("list_ai_prompt_versions")` -> [ListAIPromptVersionsPaginator](./paginators.md#listaipromptversionspaginator)
- `client.get_paginator("list_ai_prompts")` -> [ListAIPromptsPaginator](./paginators.md#listaipromptspaginator)
- `client.get_paginator("list_assistant_associations")` -> [ListAssistantAssociationsPaginator](./paginators.md#listassistantassociationspaginator)
- `client.get_paginator("list_assistants")` -> [ListAssistantsPaginator](./paginators.md#listassistantspaginator)
- `client.get_paginator("list_content_associations")` -> [ListContentAssociationsPaginator](./paginators.md#listcontentassociationspaginator)
- `client.get_paginator("list_contents")` -> [ListContentsPaginator](./paginators.md#listcontentspaginator)
- `client.get_paginator("list_import_jobs")` -> [ListImportJobsPaginator](./paginators.md#listimportjobspaginator)
- `client.get_paginator("list_knowledge_bases")` -> [ListKnowledgeBasesPaginator](./paginators.md#listknowledgebasespaginator)
- `client.get_paginator("list_message_template_versions")` -> [ListMessageTemplateVersionsPaginator](./paginators.md#listmessagetemplateversionspaginator)
- `client.get_paginator("list_message_templates")` -> [ListMessageTemplatesPaginator](./paginators.md#listmessagetemplatespaginator)
- `client.get_paginator("list_messages")` -> [ListMessagesPaginator](./paginators.md#listmessagespaginator)
- `client.get_paginator("list_quick_responses")` -> [ListQuickResponsesPaginator](./paginators.md#listquickresponsespaginator)
- `client.get_paginator("query_assistant")` -> [QueryAssistantPaginator](./paginators.md#queryassistantpaginator)
- `client.get_paginator("search_content")` -> [SearchContentPaginator](./paginators.md#searchcontentpaginator)
- `client.get_paginator("search_message_templates")` -> [SearchMessageTemplatesPaginator](./paginators.md#searchmessagetemplatespaginator)
- `client.get_paginator("search_quick_responses")` -> [SearchQuickResponsesPaginator](./paginators.md#searchquickresponsespaginator)
- `client.get_paginator("search_sessions")` -> [SearchSessionsPaginator](./paginators.md#searchsessionspaginator)



