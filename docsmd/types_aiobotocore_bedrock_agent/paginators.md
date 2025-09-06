# Paginators

> [Index](../README.md) > [AgentsforBedrock](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#agentsforbedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).

## ListAgentActionGroupsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_agent_action_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListAgentActionGroups.html#AgentsforBedrock.Paginator.ListAgentActionGroups)

```python
# ListAgentActionGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListAgentActionGroupsPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListAgentActionGroupsPaginator = client.get_paginator("list_agent_action_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentActionGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListAgentActionGroupsPaginator](./paginators.md#listagentactiongroupspaginator)
3. item: `AioPageIterator[ListAgentActionGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAgentActionGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentId: str,
    agentVersion: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAgentActionGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAgentActionGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAgentActionGroupsRequestPaginateTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgentActionGroupsRequestPaginateTypeDef](./type_defs.md#listagentactiongroupsrequestpaginatetypedef)
## ListAgentAliasesPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_agent_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListAgentAliases.html#AgentsforBedrock.Paginator.ListAgentAliases)

```python
# ListAgentAliasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListAgentAliasesPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListAgentAliasesPaginator = client.get_paginator("list_agent_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListAgentAliasesPaginator](./paginators.md#listagentaliasespaginator)
3. item: `AioPageIterator[ListAgentAliasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAgentAliasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAgentAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAgentAliasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAgentAliasesRequestPaginateTypeDef = {  # (1)
    "agentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgentAliasesRequestPaginateTypeDef](./type_defs.md#listagentaliasesrequestpaginatetypedef)
## ListAgentCollaboratorsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_agent_collaborators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListAgentCollaborators.html#AgentsforBedrock.Paginator.ListAgentCollaborators)

```python
# ListAgentCollaboratorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListAgentCollaboratorsPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListAgentCollaboratorsPaginator = client.get_paginator("list_agent_collaborators")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentCollaboratorsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListAgentCollaboratorsPaginator](./paginators.md#listagentcollaboratorspaginator)
3. item: `AioPageIterator[ListAgentCollaboratorsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAgentCollaboratorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentId: str,
    agentVersion: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAgentCollaboratorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAgentCollaboratorsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAgentCollaboratorsRequestPaginateTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgentCollaboratorsRequestPaginateTypeDef](./type_defs.md#listagentcollaboratorsrequestpaginatetypedef)
## ListAgentKnowledgeBasesPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_agent_knowledge_bases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListAgentKnowledgeBases.html#AgentsforBedrock.Paginator.ListAgentKnowledgeBases)

```python
# ListAgentKnowledgeBasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListAgentKnowledgeBasesPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListAgentKnowledgeBasesPaginator = client.get_paginator("list_agent_knowledge_bases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentKnowledgeBasesResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListAgentKnowledgeBasesPaginator](./paginators.md#listagentknowledgebasespaginator)
3. item: `AioPageIterator[ListAgentKnowledgeBasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAgentKnowledgeBasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentId: str,
    agentVersion: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAgentKnowledgeBasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAgentKnowledgeBasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAgentKnowledgeBasesRequestPaginateTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgentKnowledgeBasesRequestPaginateTypeDef](./type_defs.md#listagentknowledgebasesrequestpaginatetypedef)
## ListAgentVersionsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_agent_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListAgentVersions.html#AgentsforBedrock.Paginator.ListAgentVersions)

```python
# ListAgentVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListAgentVersionsPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListAgentVersionsPaginator = client.get_paginator("list_agent_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListAgentVersionsPaginator](./paginators.md#listagentversionspaginator)
3. item: `AioPageIterator[ListAgentVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAgentVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAgentVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAgentVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAgentVersionsRequestPaginateTypeDef = {  # (1)
    "agentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgentVersionsRequestPaginateTypeDef](./type_defs.md#listagentversionsrequestpaginatetypedef)
## ListAgentsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_agents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListAgents.html#AgentsforBedrock.Paginator.ListAgents)

```python
# ListAgentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListAgentsPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListAgentsPaginator = client.get_paginator("list_agents")  # (2)
    async for item in paginator.paginate(...):
        item: ListAgentsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListAgentsPaginator](./paginators.md#listagentspaginator)
3. item: `AioPageIterator[ListAgentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAgentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAgentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAgentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAgentsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAgentsRequestPaginateTypeDef](./type_defs.md#listagentsrequestpaginatetypedef)
## ListDataSourcesPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_data_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListDataSources.html#AgentsforBedrock.Paginator.ListDataSources)

```python
# ListDataSourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListDataSourcesPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListDataSourcesPaginator = client.get_paginator("list_data_sources")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataSourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
3. item: `AioPageIterator[ListDataSourcesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataSourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataSourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataSourcesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataSourcesRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestPaginateTypeDef](./type_defs.md#listdatasourcesrequestpaginatetypedef)
## ListFlowAliasesPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_flow_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListFlowAliases.html#AgentsforBedrock.Paginator.ListFlowAliases)

```python
# ListFlowAliasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListFlowAliasesPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListFlowAliasesPaginator = client.get_paginator("list_flow_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListFlowAliasesPaginator](./paginators.md#listflowaliasespaginator)
3. item: `AioPageIterator[ListFlowAliasesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowAliasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    flowIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFlowAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFlowAliasesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowAliasesRequestPaginateTypeDef = {  # (1)
    "flowIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowAliasesRequestPaginateTypeDef](./type_defs.md#listflowaliasesrequestpaginatetypedef)
## ListFlowVersionsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_flow_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListFlowVersions.html#AgentsforBedrock.Paginator.ListFlowVersions)

```python
# ListFlowVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListFlowVersionsPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListFlowVersionsPaginator = client.get_paginator("list_flow_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListFlowVersionsPaginator](./paginators.md#listflowversionspaginator)
3. item: `AioPageIterator[ListFlowVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    flowIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFlowVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFlowVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowVersionsRequestPaginateTypeDef = {  # (1)
    "flowIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowVersionsRequestPaginateTypeDef](./type_defs.md#listflowversionsrequestpaginatetypedef)
## ListFlowsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_flows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListFlows.html#AgentsforBedrock.Paginator.ListFlows)

```python
# ListFlowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListFlowsPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListFlowsPaginator = client.get_paginator("list_flows")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListFlowsPaginator](./paginators.md#listflowspaginator)
3. item: `AioPageIterator[ListFlowsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFlowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFlowsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowsRequestPaginateTypeDef](./type_defs.md#listflowsrequestpaginatetypedef)
## ListIngestionJobsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_ingestion_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListIngestionJobs.html#AgentsforBedrock.Paginator.ListIngestionJobs)

```python
# ListIngestionJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListIngestionJobsPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListIngestionJobsPaginator = client.get_paginator("list_ingestion_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListIngestionJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListIngestionJobsPaginator](./paginators.md#listingestionjobspaginator)
3. item: `AioPageIterator[ListIngestionJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIngestionJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    dataSourceId: str,
    filters: Sequence[IngestionJobFilterTypeDef] = ...,  # (1)
    sortBy: IngestionJobSortByTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListIngestionJobsResponseTypeDef]:  # (4)
    ...
```

1. See `Sequence[IngestionJobFilterTypeDef]`
2. See [:material-code-braces: IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListIngestionJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIngestionJobsRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "dataSourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIngestionJobsRequestPaginateTypeDef](./type_defs.md#listingestionjobsrequestpaginatetypedef)
## ListKnowledgeBaseDocumentsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_knowledge_base_documents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListKnowledgeBaseDocuments.html#AgentsforBedrock.Paginator.ListKnowledgeBaseDocuments)

```python
# ListKnowledgeBaseDocumentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListKnowledgeBaseDocumentsPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListKnowledgeBaseDocumentsPaginator = client.get_paginator("list_knowledge_base_documents")  # (2)
    async for item in paginator.paginate(...):
        item: ListKnowledgeBaseDocumentsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListKnowledgeBaseDocumentsPaginator](./paginators.md#listknowledgebasedocumentspaginator)
3. item: `AioPageIterator[ListKnowledgeBaseDocumentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListKnowledgeBaseDocumentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    dataSourceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListKnowledgeBaseDocumentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListKnowledgeBaseDocumentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListKnowledgeBaseDocumentsRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "dataSourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKnowledgeBaseDocumentsRequestPaginateTypeDef](./type_defs.md#listknowledgebasedocumentsrequestpaginatetypedef)
## ListKnowledgeBasesPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_knowledge_bases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListKnowledgeBases.html#AgentsforBedrock.Paginator.ListKnowledgeBases)

```python
# ListKnowledgeBasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListKnowledgeBasesPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListKnowledgeBasesPaginator = client.get_paginator("list_knowledge_bases")  # (2)
    async for item in paginator.paginate(...):
        item: ListKnowledgeBasesResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
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
## ListPromptsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator("list_prompts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent/paginator/ListPrompts.html#AgentsforBedrock.Paginator.ListPrompts)

```python
# ListPromptsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.paginator import ListPromptsPaginator

session = get_session()
async with session.create_client("bedrock-agent") as client:  # (1)
    paginator: ListPromptsPaginator = client.get_paginator("list_prompts")  # (2)
    async for item in paginator.paginate(...):
        item: ListPromptsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListPromptsPaginator](./paginators.md#listpromptspaginator)
3. item: `AioPageIterator[ListPromptsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPromptsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    promptIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPromptsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPromptsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPromptsRequestPaginateTypeDef = {  # (1)
    "promptIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPromptsRequestPaginateTypeDef](./type_defs.md#listpromptsrequestpaginatetypedef)
