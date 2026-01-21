# Paginators

> [Index](../README.md) > [BedrockAgentCore](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [BedrockAgentCore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#bedrockagentcore)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore](https://pypi.org/project/types-aiobotocore-bedrock-agentcore/).

## ListActorsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("list_actors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/ListActors.html#BedrockAgentCore.Paginator.ListActors)

```python
# ListActorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import ListActorsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: ListActorsPaginator = client.get_paginator("list_actors")  # (2)
    async for item in paginator.paginate(...):
        item: ListActorsOutputTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListActorsPaginator](./paginators.md#listactorspaginator)
3. item: `AioPageIterator[ListActorsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListActorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    memoryId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListActorsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListActorsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListActorsInputPaginateTypeDef = {  # (1)
    "memoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActorsInputPaginateTypeDef](./type_defs.md#listactorsinputpaginatetypedef)
## ListEventsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("list_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/ListEvents.html#BedrockAgentCore.Paginator.ListEvents)

```python
# ListEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import ListEventsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: ListEventsPaginator = client.get_paginator("list_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListEventsPaginator](./paginators.md#listeventspaginator)
3. item: `AioPageIterator[ListEventsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    memoryId: str,
    sessionId: str,
    actorId: str,
    includePayloads: bool = ...,
    filter: FilterInputTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListEventsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterInputTypeDef](./type_defs.md#filterinputtypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListEventsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEventsInputPaginateTypeDef = {  # (1)
    "memoryId": ...,
    "sessionId": ...,
    "actorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventsInputPaginateTypeDef](./type_defs.md#listeventsinputpaginatetypedef)
## ListMemoryExtractionJobsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("list_memory_extraction_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/ListMemoryExtractionJobs.html#BedrockAgentCore.Paginator.ListMemoryExtractionJobs)

```python
# ListMemoryExtractionJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import ListMemoryExtractionJobsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: ListMemoryExtractionJobsPaginator = client.get_paginator("list_memory_extraction_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListMemoryExtractionJobsOutputTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListMemoryExtractionJobsPaginator](./paginators.md#listmemoryextractionjobspaginator)
3. item: `AioPageIterator[ListMemoryExtractionJobsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMemoryExtractionJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    memoryId: str,
    filter: ExtractionJobFilterInputTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListMemoryExtractionJobsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ExtractionJobFilterInputTypeDef](./type_defs.md#extractionjobfilterinputtypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListMemoryExtractionJobsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMemoryExtractionJobsInputPaginateTypeDef = {  # (1)
    "memoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMemoryExtractionJobsInputPaginateTypeDef](./type_defs.md#listmemoryextractionjobsinputpaginatetypedef)
## ListMemoryRecordsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("list_memory_records")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/ListMemoryRecords.html#BedrockAgentCore.Paginator.ListMemoryRecords)

```python
# ListMemoryRecordsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import ListMemoryRecordsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: ListMemoryRecordsPaginator = client.get_paginator("list_memory_records")  # (2)
    async for item in paginator.paginate(...):
        item: ListMemoryRecordsOutputTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListMemoryRecordsPaginator](./paginators.md#listmemoryrecordspaginator)
3. item: `AioPageIterator[ListMemoryRecordsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMemoryRecordsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    memoryId: str,
    namespace: str,
    memoryStrategyId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListMemoryRecordsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListMemoryRecordsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMemoryRecordsInputPaginateTypeDef = {  # (1)
    "memoryId": ...,
    "namespace": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMemoryRecordsInputPaginateTypeDef](./type_defs.md#listmemoryrecordsinputpaginatetypedef)
## ListSessionsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("list_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/ListSessions.html#BedrockAgentCore.Paginator.ListSessions)

```python
# ListSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import ListSessionsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: ListSessionsPaginator = client.get_paginator("list_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSessionsOutputTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListSessionsPaginator](./paginators.md#listsessionspaginator)
3. item: `AioPageIterator[ListSessionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    memoryId: str,
    actorId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSessionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSessionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSessionsInputPaginateTypeDef = {  # (1)
    "memoryId": ...,
    "actorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSessionsInputPaginateTypeDef](./type_defs.md#listsessionsinputpaginatetypedef)
## RetrieveMemoryRecordsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("retrieve_memory_records")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/RetrieveMemoryRecords.html#BedrockAgentCore.Paginator.RetrieveMemoryRecords)

```python
# RetrieveMemoryRecordsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import RetrieveMemoryRecordsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: RetrieveMemoryRecordsPaginator = client.get_paginator("retrieve_memory_records")  # (2)
    async for item in paginator.paginate(...):
        item: RetrieveMemoryRecordsOutputTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [RetrieveMemoryRecordsPaginator](./paginators.md#retrievememoryrecordspaginator)
3. item: `AioPageIterator[RetrieveMemoryRecordsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python RetrieveMemoryRecordsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    memoryId: str,
    namespace: str,
    searchCriteria: SearchCriteriaTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[RetrieveMemoryRecordsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[RetrieveMemoryRecordsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: RetrieveMemoryRecordsInputPaginateTypeDef = {  # (1)
    "memoryId": ...,
    "namespace": ...,
    "searchCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: RetrieveMemoryRecordsInputPaginateTypeDef](./type_defs.md#retrievememoryrecordsinputpaginatetypedef)
