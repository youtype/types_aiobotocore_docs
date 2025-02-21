# Paginators

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#agentsforbedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

## GetAgentMemoryPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").get_paginator("get_agent_memory")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/GetAgentMemory.html#AgentsforBedrockRuntime.Paginator.GetAgentMemory)

```python
# GetAgentMemoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.paginator import GetAgentMemoryPaginator

session = get_session()
async with session.create_client("bedrock-agent-runtime") as client:  # (1)
    paginator: GetAgentMemoryPaginator = client.get_paginator("get_agent_memory")  # (2)
    async for item in paginator.paginate(...):
        item: GetAgentMemoryResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [GetAgentMemoryPaginator](./paginators.md#getagentmemorypaginator)
3. item: [:material-code-braces: GetAgentMemoryResponseTypeDef](./type_defs.md#getagentmemoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetAgentMemoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    agentAliasId: str,
    agentId: str,
    memoryId: str,
    memoryType: MemoryTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetAgentMemoryResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MemoryTypeType](./literals.md#memorytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetAgentMemoryResponseTypeDef](./type_defs.md#getagentmemoryresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetAgentMemoryRequestPaginateTypeDef = {  # (1)
    "agentAliasId": ...,
    "agentId": ...,
    "memoryId": ...,
    "memoryType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAgentMemoryRequestPaginateTypeDef](./type_defs.md#getagentmemoryrequestpaginatetypedef) 
## RerankPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").get_paginator("rerank")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/Rerank.html#AgentsforBedrockRuntime.Paginator.Rerank)

```python
# RerankPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.paginator import RerankPaginator

session = get_session()
async with session.create_client("bedrock-agent-runtime") as client:  # (1)
    paginator: RerankPaginator = client.get_paginator("rerank")  # (2)
    async for item in paginator.paginate(...):
        item: RerankResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [RerankPaginator](./paginators.md#rerankpaginator)
3. item: [:material-code-braces: RerankResponseTypeDef](./type_defs.md#rerankresponsetypedef) 


### paginate

Type annotations and code completion for `#!python RerankPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    queries: Sequence[RerankQueryTypeDef],  # (1)
    rerankingConfiguration: RerankingConfigurationTypeDef,  # (2)
    sources: Sequence[RerankSourceTypeDef],  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[RerankResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: RerankQueryTypeDef](./type_defs.md#rerankquerytypedef) 
2. See [:material-code-braces: RerankingConfigurationTypeDef](./type_defs.md#rerankingconfigurationtypedef) 
3. See [:material-code-braces: RerankSourceTypeDef](./type_defs.md#reranksourcetypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: RerankResponseTypeDef](./type_defs.md#rerankresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: RerankRequestPaginateTypeDef = {  # (1)
    "queries": ...,
    "rerankingConfiguration": ...,
    "sources": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: RerankRequestPaginateTypeDef](./type_defs.md#rerankrequestpaginatetypedef) 
## RetrievePaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").get_paginator("retrieve")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/Retrieve.html#AgentsforBedrockRuntime.Paginator.Retrieve)

```python
# RetrievePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.paginator import RetrievePaginator

session = get_session()
async with session.create_client("bedrock-agent-runtime") as client:  # (1)
    paginator: RetrievePaginator = client.get_paginator("retrieve")  # (2)
    async for item in paginator.paginate(...):
        item: RetrieveResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [RetrievePaginator](./paginators.md#retrievepaginator)
3. item: [:material-code-braces: RetrieveResponseTypeDef](./type_defs.md#retrieveresponsetypedef) 


### paginate

Type annotations and code completion for `#!python RetrievePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    knowledgeBaseId: str,
    retrievalQuery: KnowledgeBaseQueryTypeDef,  # (1)
    guardrailConfiguration: GuardrailConfigurationTypeDef = ...,  # (2)
    retrievalConfiguration: KnowledgeBaseRetrievalConfigurationPaginatorTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[RetrieveResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef) 
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
3. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationPaginatorTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationpaginatortypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: RetrieveResponseTypeDef](./type_defs.md#retrieveresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: RetrieveRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "retrievalQuery": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: RetrieveRequestPaginateTypeDef](./type_defs.md#retrieverequestpaginatetypedef) 
