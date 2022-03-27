# Paginators

> [Index](../README.md) > [ConnectWisdomService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ConnectWisdomService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
    type annotations stubs module [types-aiobotocore-wisdom](https://pypi.org/project/types-aiobotocore-wisdom/).

## ListAssistantAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("wisdom").get_paginator("list_assistant_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import ListAssistantAssociationsPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: ListAssistantAssociationsPaginator = client.get_paginator("list_assistant_associations")
```


### paginate

Type annotations and code completion for `#!python ListAssistantAssociationsPaginator.paginate` method.

```python title="Method definition"
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


```python title="Usage example with kwargs"
kwargs: ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef = {  # (1)
    "assistantId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef](./type_defs.md#listassistantassociationsrequestlistassistantassociationspaginatetypedef) 
## ListAssistantsPaginator

Type annotations and code completion for `#!python session.create_client("wisdom").get_paginator("list_assistants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import ListAssistantsPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: ListAssistantsPaginator = client.get_paginator("list_assistants")
```


### paginate

Type annotations and code completion for `#!python ListAssistantsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAssistantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssistantsResponseTypeDef](./type_defs.md#listassistantsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssistantsRequestListAssistantsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssistantsRequestListAssistantsPaginateTypeDef](./type_defs.md#listassistantsrequestlistassistantspaginatetypedef) 
## ListContentsPaginator

Type annotations and code completion for `#!python session.create_client("wisdom").get_paginator("list_contents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import ListContentsPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: ListContentsPaginator = client.get_paginator("list_contents")
```


### paginate

Type annotations and code completion for `#!python ListContentsPaginator.paginate` method.

```python title="Method definition"
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


```python title="Usage example with kwargs"
kwargs: ListContentsRequestListContentsPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContentsRequestListContentsPaginateTypeDef](./type_defs.md#listcontentsrequestlistcontentspaginatetypedef) 
## ListKnowledgeBasesPaginator

Type annotations and code completion for `#!python session.create_client("wisdom").get_paginator("list_knowledge_bases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import ListKnowledgeBasesPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: ListKnowledgeBasesPaginator = client.get_paginator("list_knowledge_bases")
```


### paginate

Type annotations and code completion for `#!python ListKnowledgeBasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListKnowledgeBasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef](./type_defs.md#listknowledgebasesrequestlistknowledgebasespaginatetypedef) 
## QueryAssistantPaginator

Type annotations and code completion for `#!python session.create_client("wisdom").get_paginator("query_assistant")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import QueryAssistantPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: QueryAssistantPaginator = client.get_paginator("query_assistant")
```


### paginate

Type annotations and code completion for `#!python QueryAssistantPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    assistantId: str,
    queryText: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[QueryAssistantResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: QueryAssistantResponseTypeDef](./type_defs.md#queryassistantresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: QueryAssistantRequestQueryAssistantPaginateTypeDef = {  # (1)
    "assistantId": ...,
    "queryText": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: QueryAssistantRequestQueryAssistantPaginateTypeDef](./type_defs.md#queryassistantrequestqueryassistantpaginatetypedef) 
## SearchContentPaginator

Type annotations and code completion for `#!python session.create_client("wisdom").get_paginator("search_content")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import SearchContentPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: SearchContentPaginator = client.get_paginator("search_content")
```


### paginate

Type annotations and code completion for `#!python SearchContentPaginator.paginate` method.

```python title="Method definition"
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


```python title="Usage example with kwargs"
kwargs: SearchContentRequestSearchContentPaginateTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "searchExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchContentRequestSearchContentPaginateTypeDef](./type_defs.md#searchcontentrequestsearchcontentpaginatetypedef) 
## SearchSessionsPaginator

Type annotations and code completion for `#!python session.create_client("wisdom").get_paginator("search_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import SearchSessionsPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: SearchSessionsPaginator = client.get_paginator("search_sessions")
```


### paginate

Type annotations and code completion for `#!python SearchSessionsPaginator.paginate` method.

```python title="Method definition"
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


```python title="Usage example with kwargs"
kwargs: SearchSessionsRequestSearchSessionsPaginateTypeDef = {  # (1)
    "assistantId": ...,
    "searchExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSessionsRequestSearchSessionsPaginateTypeDef](./type_defs.md#searchsessionsrequestsearchsessionspaginatetypedef) 
