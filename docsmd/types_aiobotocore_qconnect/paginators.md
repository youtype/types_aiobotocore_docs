# Paginators

> [Index](../README.md) > [QConnect](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
    type annotations stubs module [types-aiobotocore-qconnect](https://pypi.org/project/types-aiobotocore-qconnect/).

## ListAIAgentVersionsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_ai_agent_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListAIAgentVersions)

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
3. item: [:material-code-braces: ListAIAgentVersionsResponseTypeDef](./type_defs.md#listaiagentversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAIAgentVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    aiAgentId: str,
    assistantId: str,
    origin: OriginType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAIAgentVersionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAIAgentVersionsResponseTypeDef](./type_defs.md#listaiagentversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAIAgentVersionsRequestListAIAgentVersionsPaginateTypeDef = {  # (1)
    "aiAgentId": ...,
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAIAgentVersionsRequestListAIAgentVersionsPaginateTypeDef](./type_defs.md#listaiagentversionsrequestlistaiagentversionspaginatetypedef) 
## ListAIAgentsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_ai_agents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListAIAgents)

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
3. item: [:material-code-braces: ListAIAgentsResponseTypeDef](./type_defs.md#listaiagentsresponsetypedef) 


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
) -> AsyncIterator[ListAIAgentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAIAgentsResponseTypeDef](./type_defs.md#listaiagentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAIAgentsRequestListAIAgentsPaginateTypeDef = {  # (1)
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAIAgentsRequestListAIAgentsPaginateTypeDef](./type_defs.md#listaiagentsrequestlistaiagentspaginatetypedef) 
## ListAIPromptVersionsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_ai_prompt_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListAIPromptVersions)

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
3. item: [:material-code-braces: ListAIPromptVersionsResponseTypeDef](./type_defs.md#listaipromptversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAIPromptVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    aiPromptId: str,
    assistantId: str,
    origin: OriginType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAIPromptVersionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAIPromptVersionsResponseTypeDef](./type_defs.md#listaipromptversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAIPromptVersionsRequestListAIPromptVersionsPaginateTypeDef = {  # (1)
    "aiPromptId": ...,
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAIPromptVersionsRequestListAIPromptVersionsPaginateTypeDef](./type_defs.md#listaipromptversionsrequestlistaipromptversionspaginatetypedef) 
## ListAIPromptsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_ai_prompts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListAIPrompts)

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
3. item: [:material-code-braces: ListAIPromptsResponseTypeDef](./type_defs.md#listaipromptsresponsetypedef) 


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
) -> AsyncIterator[ListAIPromptsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OriginType](./literals.md#origintype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAIPromptsResponseTypeDef](./type_defs.md#listaipromptsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAIPromptsRequestListAIPromptsPaginateTypeDef = {  # (1)
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAIPromptsRequestListAIPromptsPaginateTypeDef](./type_defs.md#listaipromptsrequestlistaipromptspaginatetypedef) 
## ListAssistantAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_assistant_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListAssistantAssociations)

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
3. item: [:material-code-braces: ListAssistantAssociationsResponseTypeDef](./type_defs.md#listassistantassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssistantAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAssistantAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssistantAssociationsResponseTypeDef](./type_defs.md#listassistantassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = {  # (1)
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef](./type_defs.md#listassistantassociationsrequestlistassistantassociationspaginatetypedef) 
## ListAssistantsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_assistants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListAssistants)

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
3. item: [:material-code-braces: ListAssistantsResponseTypeDef](./type_defs.md#listassistantsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssistantsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAssistantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssistantsResponseTypeDef](./type_defs.md#listassistantsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssistantsRequestListAssistantsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssistantsRequestListAssistantsPaginateTypeDef](./type_defs.md#listassistantsrequestlistassistantspaginatetypedef) 
## ListContentAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_content_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListContentAssociations)

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
3. item: [:material-code-braces: ListContentAssociationsResponseTypeDef](./type_defs.md#listcontentassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListContentAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    contentId: str,
    knowledgeBaseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListContentAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListContentAssociationsResponseTypeDef](./type_defs.md#listcontentassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListContentAssociationsRequestListContentAssociationsPaginateTypeDef = {  # (1)
    "contentId": ...,
    "knowledgeBaseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContentAssociationsRequestListContentAssociationsPaginateTypeDef](./type_defs.md#listcontentassociationsrequestlistcontentassociationspaginatetypedef) 
## ListContentsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_contents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListContents)

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
3. item: [:material-code-braces: ListContentsResponseTypeDef](./type_defs.md#listcontentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListContentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListContentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListContentsResponseTypeDef](./type_defs.md#listcontentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListContentsRequestListContentsPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContentsRequestListContentsPaginateTypeDef](./type_defs.md#listcontentsrequestlistcontentspaginatetypedef) 
## ListImportJobsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListImportJobs)

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
3. item: [:material-code-braces: ListImportJobsResponseTypeDef](./type_defs.md#listimportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListImportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListImportJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListImportJobsResponseTypeDef](./type_defs.md#listimportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListImportJobsRequestListImportJobsPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportJobsRequestListImportJobsPaginateTypeDef](./type_defs.md#listimportjobsrequestlistimportjobspaginatetypedef) 
## ListKnowledgeBasesPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_knowledge_bases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListKnowledgeBases)

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
3. item: [:material-code-braces: ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListKnowledgeBasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListKnowledgeBasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef](./type_defs.md#listknowledgebasesrequestlistknowledgebasespaginatetypedef) 
## ListQuickResponsesPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("list_quick_responses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.ListQuickResponses)

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
3. item: [:material-code-braces: ListQuickResponsesResponseTypeDef](./type_defs.md#listquickresponsesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListQuickResponsesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListQuickResponsesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListQuickResponsesResponseTypeDef](./type_defs.md#listquickresponsesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListQuickResponsesRequestListQuickResponsesPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQuickResponsesRequestListQuickResponsesPaginateTypeDef](./type_defs.md#listquickresponsesrequestlistquickresponsespaginatetypedef) 
## QueryAssistantPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("query_assistant")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.QueryAssistant)

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
3. item: [:material-code-braces: QueryAssistantResponsePaginatorTypeDef](./type_defs.md#queryassistantresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python QueryAssistantPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assistantId: str,
    overrideKnowledgeBaseSearchType: KnowledgeBaseSearchTypeType = ...,  # (1)
    queryCondition: Sequence[QueryConditionTypeDef] = ...,  # (2)
    queryInputData: QueryInputDataTypeDef = ...,  # (3)
    queryText: str = ...,
    sessionId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[QueryAssistantResponsePaginatorTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: KnowledgeBaseSearchTypeType](./literals.md#knowledgebasesearchtypetype) 
2. See [:material-code-braces: QueryConditionTypeDef](./type_defs.md#queryconditiontypedef) 
3. See [:material-code-braces: QueryInputDataTypeDef](./type_defs.md#queryinputdatatypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: QueryAssistantResponsePaginatorTypeDef](./type_defs.md#queryassistantresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: QueryAssistantRequestQueryAssistantPaginateTypeDef = {  # (1)
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: QueryAssistantRequestQueryAssistantPaginateTypeDef](./type_defs.md#queryassistantrequestqueryassistantpaginatetypedef) 
## SearchContentPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("search_content")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.SearchContent)

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
3. item: [:material-code-braces: SearchContentResponseTypeDef](./type_defs.md#searchcontentresponsetypedef) 


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
) -> AsyncIterator[SearchContentResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchContentResponseTypeDef](./type_defs.md#searchcontentresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchContentRequestSearchContentPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "searchExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchContentRequestSearchContentPaginateTypeDef](./type_defs.md#searchcontentrequestsearchcontentpaginatetypedef) 
## SearchQuickResponsesPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("search_quick_responses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.SearchQuickResponses)

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
3. item: [:material-code-braces: SearchQuickResponsesResponseTypeDef](./type_defs.md#searchquickresponsesresponsetypedef) 


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
) -> AsyncIterator[SearchQuickResponsesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: QuickResponseSearchExpressionTypeDef](./type_defs.md#quickresponsesearchexpressiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchQuickResponsesResponseTypeDef](./type_defs.md#searchquickresponsesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchQuickResponsesRequestSearchQuickResponsesPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "searchExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchQuickResponsesRequestSearchQuickResponsesPaginateTypeDef](./type_defs.md#searchquickresponsesrequestsearchquickresponsespaginatetypedef) 
## SearchSessionsPaginator

Type annotations and code completion for `#!python session.create_client("qconnect").get_paginator("search_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Paginator.SearchSessions)

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
3. item: [:material-code-braces: SearchSessionsResponseTypeDef](./type_defs.md#searchsessionsresponsetypedef) 


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
) -> AsyncIterator[SearchSessionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchSessionsResponseTypeDef](./type_defs.md#searchsessionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchSessionsRequestSearchSessionsPaginateTypeDef = {  # (1)
    "assistantId": ...,
    "searchExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSessionsRequestSearchSessionsPaginateTypeDef](./type_defs.md#searchsessionsrequestsearchsessionspaginatetypedef) 
