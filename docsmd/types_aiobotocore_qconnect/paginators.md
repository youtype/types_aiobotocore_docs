# Paginators

> [Index](../README.md) > [QConnect](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#qconnect)
    type annotations stubs module [types-aiobotocore-qconnect](https://pypi.org/project/types-aiobotocore-qconnect/).

## ListAIAgentVersionsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_ai_agent_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListAIAgentVersions.html#QConnect.Paginator.ListAIAgentVersions)

```python
# ListAIAgentVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListAIAgentVersionsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListAIAgentVersionsPaginator = client.get_paginator("list_ai_agent_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAIAgentVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAIAgentVersionsPaginator](./paginators.md#listaiagentversionspaginator)
3. item: `AioPageIterator[ListAIAgentVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAIAgentVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    aiAgentId: str,
    origin: OriginType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAIAgentVersionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAIAgentVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAIAgentVersionsRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
    "aiAgentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAIAgentVersionsRequestPaginateTypeDef](./type_defs.md#listaiagentversionsrequestpaginatetypedef)
## ListAIAgentsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_ai_agents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListAIAgents.html#QConnect.Paginator.ListAIAgents)

```python
# ListAIAgentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListAIAgentsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListAIAgentsPaginator = client.get_paginator("list_ai_agents")  # (2)
    async for item in paginator.paginate(...):
        item: ListAIAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAIAgentsPaginator](./paginators.md#listaiagentspaginator)
3. item: `AioPageIterator[ListAIAgentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAIAgentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    origin: OriginType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAIAgentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAIAgentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAIAgentsRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAIAgentsRequestPaginateTypeDef](./type_defs.md#listaiagentsrequestpaginatetypedef)
## ListAIGuardrailVersionsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_ai_guardrail_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListAIGuardrailVersions.html#QConnect.Paginator.ListAIGuardrailVersions)

```python
# ListAIGuardrailVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListAIGuardrailVersionsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListAIGuardrailVersionsPaginator = client.get_paginator("list_ai_guardrail_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAIGuardrailVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAIGuardrailVersionsPaginator](./paginators.md#listaiguardrailversionspaginator)
3. item: `AioPageIterator[ListAIGuardrailVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAIGuardrailVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    aiGuardrailId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAIGuardrailVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAIGuardrailVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAIGuardrailVersionsRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
    "aiGuardrailId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAIGuardrailVersionsRequestPaginateTypeDef](./type_defs.md#listaiguardrailversionsrequestpaginatetypedef)
## ListAIGuardrailsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_ai_guardrails")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListAIGuardrails.html#QConnect.Paginator.ListAIGuardrails)

```python
# ListAIGuardrailsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListAIGuardrailsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListAIGuardrailsPaginator = client.get_paginator("list_ai_guardrails")  # (2)
    async for item in paginator.paginate(...):
        item: ListAIGuardrailsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAIGuardrailsPaginator](./paginators.md#listaiguardrailspaginator)
3. item: `AioPageIterator[ListAIGuardrailsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAIGuardrailsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAIGuardrailsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAIGuardrailsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAIGuardrailsRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAIGuardrailsRequestPaginateTypeDef](./type_defs.md#listaiguardrailsrequestpaginatetypedef)
## ListAIPromptVersionsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_ai_prompt_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListAIPromptVersions.html#QConnect.Paginator.ListAIPromptVersions)

```python
# ListAIPromptVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListAIPromptVersionsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListAIPromptVersionsPaginator = client.get_paginator("list_ai_prompt_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAIPromptVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAIPromptVersionsPaginator](./paginators.md#listaipromptversionspaginator)
3. item: `AioPageIterator[ListAIPromptVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAIPromptVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    aiPromptId: str,
    origin: OriginType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAIPromptVersionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAIPromptVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAIPromptVersionsRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
    "aiPromptId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAIPromptVersionsRequestPaginateTypeDef](./type_defs.md#listaipromptversionsrequestpaginatetypedef)
## ListAIPromptsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_ai_prompts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListAIPrompts.html#QConnect.Paginator.ListAIPrompts)

```python
# ListAIPromptsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListAIPromptsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListAIPromptsPaginator = client.get_paginator("list_ai_prompts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAIPromptsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAIPromptsPaginator](./paginators.md#listaipromptspaginator)
3. item: `AioPageIterator[ListAIPromptsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAIPromptsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    origin: OriginType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAIPromptsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAIPromptsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAIPromptsRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAIPromptsRequestPaginateTypeDef](./type_defs.md#listaipromptsrequestpaginatetypedef)
## ListAssistantAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_assistant_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListAssistantAssociations.html#QConnect.Paginator.ListAssistantAssociations)

```python
# ListAssistantAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListAssistantAssociationsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListAssistantAssociationsPaginator = client.get_paginator("list_assistant_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssistantAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAssistantAssociationsPaginator](./paginators.md#listassistantassociationspaginator)
3. item: `AioPageIterator[ListAssistantAssociationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAssistantAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAssistantAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAssistantAssociationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAssistantAssociationsRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssistantAssociationsRequestPaginateTypeDef](./type_defs.md#listassistantassociationsrequestpaginatetypedef)
## ListAssistantsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_assistants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListAssistants.html#QConnect.Paginator.ListAssistants)

```python
# ListAssistantsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListAssistantsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListAssistantsPaginator = client.get_paginator("list_assistants")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssistantsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAssistantsPaginator](./paginators.md#listassistantspaginator)
3. item: `AioPageIterator[ListAssistantsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAssistantsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAssistantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAssistantsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAssistantsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssistantsRequestPaginateTypeDef](./type_defs.md#listassistantsrequestpaginatetypedef)
## ListContentAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_content_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListContentAssociations.html#QConnect.Paginator.ListContentAssociations)

```python
# ListContentAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListContentAssociationsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListContentAssociationsPaginator = client.get_paginator("list_content_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListContentAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListContentAssociationsPaginator](./paginators.md#listcontentassociationspaginator)
3. item: `AioPageIterator[ListContentAssociationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContentAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    contentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListContentAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListContentAssociationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContentAssociationsRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "contentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContentAssociationsRequestPaginateTypeDef](./type_defs.md#listcontentassociationsrequestpaginatetypedef)
## ListContentsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_contents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListContents.html#QConnect.Paginator.ListContents)

```python
# ListContentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListContentsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListContentsPaginator = client.get_paginator("list_contents")  # (2)
    async for item in paginator.paginate(...):
        item: ListContentsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListContentsPaginator](./paginators.md#listcontentspaginator)
3. item: `AioPageIterator[ListContentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListContentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListContentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContentsRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContentsRequestPaginateTypeDef](./type_defs.md#listcontentsrequestpaginatetypedef)
## ListImportJobsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListImportJobs.html#QConnect.Paginator.ListImportJobs)

```python
# ListImportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListImportJobsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListImportJobsPaginator = client.get_paginator("list_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListImportJobsPaginator](./paginators.md#listimportjobspaginator)
3. item: `AioPageIterator[ListImportJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListImportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListImportJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListImportJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListImportJobsRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportJobsRequestPaginateTypeDef](./type_defs.md#listimportjobsrequestpaginatetypedef)
## ListKnowledgeBasesPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_knowledge_bases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListKnowledgeBases.html#QConnect.Paginator.ListKnowledgeBases)

```python
# ListKnowledgeBasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListKnowledgeBasesPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListKnowledgeBasesPaginator = client.get_paginator("list_knowledge_bases")  # (2)
    async for item in paginator.paginate(...):
        item: ListKnowledgeBasesResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListKnowledgeBasesPaginator](./paginators.md#listknowledgebasespaginator)
3. item: `AioPageIterator[ListKnowledgeBasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListKnowledgeBasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListKnowledgeBasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListKnowledgeBasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListKnowledgeBasesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKnowledgeBasesRequestPaginateTypeDef](./type_defs.md#listknowledgebasesrequestpaginatetypedef)
## ListMessageTemplateVersionsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_message_template_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListMessageTemplateVersions.html#QConnect.Paginator.ListMessageTemplateVersions)

```python
# ListMessageTemplateVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListMessageTemplateVersionsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListMessageTemplateVersionsPaginator = client.get_paginator("list_message_template_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListMessageTemplateVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListMessageTemplateVersionsPaginator](./paginators.md#listmessagetemplateversionspaginator)
3. item: `AioPageIterator[ListMessageTemplateVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMessageTemplateVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    messageTemplateId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListMessageTemplateVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListMessageTemplateVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMessageTemplateVersionsRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "messageTemplateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMessageTemplateVersionsRequestPaginateTypeDef](./type_defs.md#listmessagetemplateversionsrequestpaginatetypedef)
## ListMessageTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_message_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListMessageTemplates.html#QConnect.Paginator.ListMessageTemplates)

```python
# ListMessageTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListMessageTemplatesPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListMessageTemplatesPaginator = client.get_paginator("list_message_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListMessageTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListMessageTemplatesPaginator](./paginators.md#listmessagetemplatespaginator)
3. item: `AioPageIterator[ListMessageTemplatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMessageTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListMessageTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListMessageTemplatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMessageTemplatesRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMessageTemplatesRequestPaginateTypeDef](./type_defs.md#listmessagetemplatesrequestpaginatetypedef)
## ListMessagesPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_messages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListMessages.html#QConnect.Paginator.ListMessages)

```python
# ListMessagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListMessagesPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListMessagesPaginator = client.get_paginator("list_messages")  # (2)
    async for item in paginator.paginate(...):
        item: ListMessagesResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListMessagesPaginator](./paginators.md#listmessagespaginator)
3. item: `AioPageIterator[ListMessagesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMessagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    sessionId: str,
    filter: MessageFilterTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListMessagesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MessageFilterTypeType](./literals.md#messagefiltertypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListMessagesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMessagesRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
    "sessionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMessagesRequestPaginateTypeDef](./type_defs.md#listmessagesrequestpaginatetypedef)
## ListQuickResponsesPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_quick_responses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListQuickResponses.html#QConnect.Paginator.ListQuickResponses)

```python
# ListQuickResponsesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListQuickResponsesPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListQuickResponsesPaginator = client.get_paginator("list_quick_responses")  # (2)
    async for item in paginator.paginate(...):
        item: ListQuickResponsesResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListQuickResponsesPaginator](./paginators.md#listquickresponsespaginator)
3. item: `AioPageIterator[ListQuickResponsesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListQuickResponsesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListQuickResponsesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListQuickResponsesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListQuickResponsesRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQuickResponsesRequestPaginateTypeDef](./type_defs.md#listquickresponsesrequestpaginatetypedef)
## ListSpansPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_spans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/ListSpans.html#QConnect.Paginator.ListSpans)

```python
# ListSpansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import ListSpansPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: ListSpansPaginator = client.get_paginator("list_spans")  # (2)
    async for item in paginator.paginate(...):
        item: ListSpansResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListSpansPaginator](./paginators.md#listspanspaginator)
3. item: `AioPageIterator[ListSpansResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSpansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    sessionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSpansResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSpansResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSpansRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
    "sessionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSpansRequestPaginateTypeDef](./type_defs.md#listspansrequestpaginatetypedef)
## QueryAssistantPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("query_assistant")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/QueryAssistant.html#QConnect.Paginator.QueryAssistant)

```python
# QueryAssistantPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import QueryAssistantPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: QueryAssistantPaginator = client.get_paginator("query_assistant")  # (2)
    async for item in paginator.paginate(...):
        item: QueryAssistantResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [QueryAssistantPaginator](./paginators.md#queryassistantpaginator)
3. item: `AioPageIterator[QueryAssistantResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python QueryAssistantPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    queryText: str = ...,
    sessionId: str = ...,
    queryCondition: Sequence[QueryConditionTypeDef] = ...,  # (1)
    queryInputData: QueryInputDataTypeDef = ...,  # (2)
    overrideKnowledgeBaseSearchType: KnowledgeBaseSearchTypeType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[QueryAssistantResponsePaginatorTypeDef]:  # (5)
    ...
```

1. See `Sequence[QueryConditionTypeDef]`
2. See [:material-code-braces: QueryInputDataTypeDef](./type_defs.md#queryinputdatatypedef)
3. See [:material-code-brackets: KnowledgeBaseSearchTypeType](./literals.md#knowledgebasesearchtypetype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[QueryAssistantResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: QueryAssistantRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: QueryAssistantRequestPaginateTypeDef](./type_defs.md#queryassistantrequestpaginatetypedef)
## SearchContentPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("search_content")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/SearchContent.html#QConnect.Paginator.SearchContent)

```python
# SearchContentPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import SearchContentPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: SearchContentPaginator = client.get_paginator("search_content")  # (2)
    async for item in paginator.paginate(...):
        item: SearchContentResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [SearchContentPaginator](./paginators.md#searchcontentpaginator)
3. item: `AioPageIterator[SearchContentResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchContentPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    searchExpression: SearchExpressionTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchContentResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchContentResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchContentRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "searchExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchContentRequestPaginateTypeDef](./type_defs.md#searchcontentrequestpaginatetypedef)
## SearchMessageTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("search_message_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/SearchMessageTemplates.html#QConnect.Paginator.SearchMessageTemplates)

```python
# SearchMessageTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import SearchMessageTemplatesPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: SearchMessageTemplatesPaginator = client.get_paginator("search_message_templates")  # (2)
    async for item in paginator.paginate(...):
        item: SearchMessageTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [SearchMessageTemplatesPaginator](./paginators.md#searchmessagetemplatespaginator)
3. item: `AioPageIterator[SearchMessageTemplatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchMessageTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    searchExpression: MessageTemplateSearchExpressionTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchMessageTemplatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: MessageTemplateSearchExpressionTypeDef](./type_defs.md#messagetemplatesearchexpressiontypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchMessageTemplatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchMessageTemplatesRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "searchExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchMessageTemplatesRequestPaginateTypeDef](./type_defs.md#searchmessagetemplatesrequestpaginatetypedef)
## SearchQuickResponsesPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("search_quick_responses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/SearchQuickResponses.html#QConnect.Paginator.SearchQuickResponses)

```python
# SearchQuickResponsesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import SearchQuickResponsesPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: SearchQuickResponsesPaginator = client.get_paginator("search_quick_responses")  # (2)
    async for item in paginator.paginate(...):
        item: SearchQuickResponsesResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [SearchQuickResponsesPaginator](./paginators.md#searchquickresponsespaginator)
3. item: `AioPageIterator[SearchQuickResponsesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchQuickResponsesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    searchExpression: QuickResponseSearchExpressionTypeDef,  # (1)
    attributes: Mapping[str, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchQuickResponsesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: QuickResponseSearchExpressionTypeDef](./type_defs.md#quickresponsesearchexpressiontypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchQuickResponsesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchQuickResponsesRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "searchExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchQuickResponsesRequestPaginateTypeDef](./type_defs.md#searchquickresponsesrequestpaginatetypedef)
## SearchSessionsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("search_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect/paginator/SearchSessions.html#QConnect.Paginator.SearchSessions)

```python
# SearchSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.paginator import SearchSessionsPaginator

session = get_session()
async with session.create_client("qconnect") as client:  # (1)
    paginator: SearchSessionsPaginator = client.get_paginator("search_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: SearchSessionsResponseTypeDef
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [SearchSessionsPaginator](./paginators.md#searchsessionspaginator)
3. item: `AioPageIterator[SearchSessionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    searchExpression: SearchExpressionTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchSessionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchSessionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchSessionsRequestPaginateTypeDef = {  # (1)
    "assistantId": ...,
    "searchExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSessionsRequestPaginateTypeDef](./type_defs.md#searchsessionsrequestpaginatetypedef)
