# Paginators

> [Index](../README.md) > [BedrockAgentCore](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [BedrockAgentCore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#bedrockagentcore)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore](https://pypi.org/project/types-aiobotocore-bedrock-agentcore/).

## ListABTestsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("list_ab_tests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/ListABTests.html#BedrockAgentCore.Paginator.ListABTests)

```python
# ListABTestsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import ListABTestsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: ListABTestsPaginator = client.get_paginator("list_ab_tests")  # (2)
    async for item in paginator.paginate(...):
        item: ListABTestsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListABTestsPaginator](./paginators.md#listabtestspaginator)
3. item: `AioPageIterator[ListABTestsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListABTestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListABTestsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListABTestsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListABTestsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListABTestsRequestPaginateTypeDef](./type_defs.md#listabtestsrequestpaginatetypedef)
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
## ListBatchEvaluationsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("list_batch_evaluations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/ListBatchEvaluations.html#BedrockAgentCore.Paginator.ListBatchEvaluations)

```python
# ListBatchEvaluationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import ListBatchEvaluationsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: ListBatchEvaluationsPaginator = client.get_paginator("list_batch_evaluations")  # (2)
    async for item in paginator.paginate(...):
        item: ListBatchEvaluationsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListBatchEvaluationsPaginator](./paginators.md#listbatchevaluationspaginator)
3. item: `AioPageIterator[ListBatchEvaluationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBatchEvaluationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBatchEvaluationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBatchEvaluationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBatchEvaluationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBatchEvaluationsRequestPaginateTypeDef](./type_defs.md#listbatchevaluationsrequestpaginatetypedef)
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
    namespace: str = ...,
    namespacePath: str = ...,
    memoryStrategyId: str = ...,
    metadataFilters: Sequence[MemoryMetadataFilterExpressionTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListMemoryRecordsOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[MemoryMetadataFilterExpressionTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListMemoryRecordsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMemoryRecordsInputPaginateTypeDef = {  # (1)
    "memoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMemoryRecordsInputPaginateTypeDef](./type_defs.md#listmemoryrecordsinputpaginatetypedef)
## ListPaymentInstrumentsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("list_payment_instruments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/ListPaymentInstruments.html#BedrockAgentCore.Paginator.ListPaymentInstruments)

```python
# ListPaymentInstrumentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import ListPaymentInstrumentsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: ListPaymentInstrumentsPaginator = client.get_paginator("list_payment_instruments")  # (2)
    async for item in paginator.paginate(...):
        item: ListPaymentInstrumentsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListPaymentInstrumentsPaginator](./paginators.md#listpaymentinstrumentspaginator)
3. item: `AioPageIterator[ListPaymentInstrumentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPaymentInstrumentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    paymentManagerArn: str,
    userId: str = ...,
    agentName: str = ...,
    paymentConnectorId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPaymentInstrumentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPaymentInstrumentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPaymentInstrumentsRequestPaginateTypeDef = {  # (1)
    "paymentManagerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPaymentInstrumentsRequestPaginateTypeDef](./type_defs.md#listpaymentinstrumentsrequestpaginatetypedef)
## ListPaymentSessionsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("list_payment_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/ListPaymentSessions.html#BedrockAgentCore.Paginator.ListPaymentSessions)

```python
# ListPaymentSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import ListPaymentSessionsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: ListPaymentSessionsPaginator = client.get_paginator("list_payment_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPaymentSessionsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListPaymentSessionsPaginator](./paginators.md#listpaymentsessionspaginator)
3. item: `AioPageIterator[ListPaymentSessionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPaymentSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    paymentManagerArn: str,
    userId: str = ...,
    agentName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPaymentSessionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPaymentSessionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPaymentSessionsRequestPaginateTypeDef = {  # (1)
    "paymentManagerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPaymentSessionsRequestPaginateTypeDef](./type_defs.md#listpaymentsessionsrequestpaginatetypedef)
## ListRecommendationsPaginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator("list_recommendations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/paginator/ListRecommendations.html#BedrockAgentCore.Paginator.ListRecommendations)

```python
# ListRecommendationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.paginator import ListRecommendationsPaginator

session = get_session()
async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator: ListRecommendationsPaginator = client.get_paginator("list_recommendations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendationsResponseTypeDef
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)
3. item: `AioPageIterator[ListRecommendationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecommendationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    statusFilter: RecommendationStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRecommendationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRecommendationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendationsRequestPaginateTypeDef = {  # (1)
    "statusFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestPaginateTypeDef](./type_defs.md#listrecommendationsrequestpaginatetypedef)
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
    filter: SessionFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListSessionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SessionFilterTypeDef](./type_defs.md#sessionfiltertypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSessionsOutputTypeDef]`


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
    searchCriteria: SearchCriteriaTypeDef,  # (1)
    namespace: str = ...,
    namespacePath: str = ...,
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
    "searchCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: RetrieveMemoryRecordsInputPaginateTypeDef](./type_defs.md#retrievememoryrecordsinputpaginatetypedef)
