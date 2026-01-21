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
3. item: `AioPageIterator[GetAgentMemoryResponseTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[GetAgentMemoryResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MemoryTypeType](./literals.md#memorytypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetAgentMemoryResponseTypeDef]`


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
## ListFlowExecutionEventsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").get_paginator("list_flow_execution_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/ListFlowExecutionEvents.html#AgentsforBedrockRuntime.Paginator.ListFlowExecutionEvents)

```python
# ListFlowExecutionEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.paginator import ListFlowExecutionEventsPaginator

session = get_session()
async with session.create_client("bedrock-agent-runtime") as client:  # (1)
    paginator: ListFlowExecutionEventsPaginator = client.get_paginator("list_flow_execution_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowExecutionEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [ListFlowExecutionEventsPaginator](./paginators.md#listflowexecutioneventspaginator)
3. item: `AioPageIterator[ListFlowExecutionEventsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowExecutionEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    eventType: FlowExecutionEventTypeType,  # (1)
    executionIdentifier: str,
    flowAliasIdentifier: str,
    flowIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListFlowExecutionEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: FlowExecutionEventTypeType](./literals.md#flowexecutioneventtypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListFlowExecutionEventsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowExecutionEventsRequestPaginateTypeDef = {  # (1)
    "eventType": ...,
    "executionIdentifier": ...,
    "flowAliasIdentifier": ...,
    "flowIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowExecutionEventsRequestPaginateTypeDef](./type_defs.md#listflowexecutioneventsrequestpaginatetypedef)
## ListFlowExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").get_paginator("list_flow_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/ListFlowExecutions.html#AgentsforBedrockRuntime.Paginator.ListFlowExecutions)

```python
# ListFlowExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.paginator import ListFlowExecutionsPaginator

session = get_session()
async with session.create_client("bedrock-agent-runtime") as client:  # (1)
    paginator: ListFlowExecutionsPaginator = client.get_paginator("list_flow_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [ListFlowExecutionsPaginator](./paginators.md#listflowexecutionspaginator)
3. item: `AioPageIterator[ListFlowExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    flowIdentifier: str,
    flowAliasIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFlowExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFlowExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowExecutionsRequestPaginateTypeDef = {  # (1)
    "flowIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowExecutionsRequestPaginateTypeDef](./type_defs.md#listflowexecutionsrequestpaginatetypedef)
## ListInvocationStepsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").get_paginator("list_invocation_steps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/ListInvocationSteps.html#AgentsforBedrockRuntime.Paginator.ListInvocationSteps)

```python
# ListInvocationStepsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.paginator import ListInvocationStepsPaginator

session = get_session()
async with session.create_client("bedrock-agent-runtime") as client:  # (1)
    paginator: ListInvocationStepsPaginator = client.get_paginator("list_invocation_steps")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvocationStepsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [ListInvocationStepsPaginator](./paginators.md#listinvocationstepspaginator)
3. item: `AioPageIterator[ListInvocationStepsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInvocationStepsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sessionIdentifier: str,
    invocationIdentifier: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListInvocationStepsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListInvocationStepsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInvocationStepsRequestPaginateTypeDef = {  # (1)
    "sessionIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvocationStepsRequestPaginateTypeDef](./type_defs.md#listinvocationstepsrequestpaginatetypedef)
## ListInvocationsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").get_paginator("list_invocations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/ListInvocations.html#AgentsforBedrockRuntime.Paginator.ListInvocations)

```python
# ListInvocationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.paginator import ListInvocationsPaginator

session = get_session()
async with session.create_client("bedrock-agent-runtime") as client:  # (1)
    paginator: ListInvocationsPaginator = client.get_paginator("list_invocations")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvocationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [ListInvocationsPaginator](./paginators.md#listinvocationspaginator)
3. item: `AioPageIterator[ListInvocationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInvocationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sessionIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListInvocationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListInvocationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInvocationsRequestPaginateTypeDef = {  # (1)
    "sessionIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvocationsRequestPaginateTypeDef](./type_defs.md#listinvocationsrequestpaginatetypedef)
## ListSessionsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").get_paginator("list_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime/paginator/ListSessions.html#AgentsforBedrockRuntime.Paginator.ListSessions)

```python
# ListSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.paginator import ListSessionsPaginator

session = get_session()
async with session.create_client("bedrock-agent-runtime") as client:  # (1)
    paginator: ListSessionsPaginator = client.get_paginator("list_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSessionsResponseTypeDef
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [ListSessionsPaginator](./paginators.md#listsessionspaginator)
3. item: `AioPageIterator[ListSessionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSessionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSessionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSessionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSessionsRequestPaginateTypeDef](./type_defs.md#listsessionsrequestpaginatetypedef)
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
3. item: `AioPageIterator[RerankResponseTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[RerankResponseTypeDef]:  # (5)
    ...
```

1. See `Sequence[RerankQueryTypeDef]`
2. See [:material-code-braces: RerankingConfigurationTypeDef](./type_defs.md#rerankingconfigurationtypedef)
3. See `Sequence[RerankSourceTypeDef]`
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[RerankResponseTypeDef]`


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
3. item: `AioPageIterator[RetrieveResponseTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[RetrieveResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef)
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
3. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationPaginatorTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationpaginatortypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[RetrieveResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: RetrieveRequestPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "retrievalQuery": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: RetrieveRequestPaginateTypeDef](./type_defs.md#retrieverequestpaginatetypedef)
