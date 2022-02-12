<a id="paginators-for-aiobotocore-connectwisdomservice-module"></a>

# Paginators for aiobotocore ConnectWisdomService module

> [Index](..) > [ConnectWisdomService](.) > Paginators

Auto-generated documentation for
[ConnectWisdomService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
type annotations stubs module
[types-aiobotocore-wisdom](https://pypi.org/project/types-aiobotocore-wisdom/).

- [Paginators for aiobotocore ConnectWisdomService module](#paginators-for-aiobotocore-connectwisdomservice-module)
  - [ListAssistantAssociationsPaginator](#listassistantassociationspaginator)
  - [ListAssistantsPaginator](#listassistantspaginator)
  - [ListContentsPaginator](#listcontentspaginator)
  - [ListKnowledgeBasesPaginator](#listknowledgebasespaginator)
  - [QueryAssistantPaginator](#queryassistantpaginator)
  - [SearchContentPaginator](#searchcontentpaginator)
  - [SearchSessionsPaginator](#searchsessionspaginator)

<a id="listassistantassociationspaginator"></a>

## ListAssistantAssociationsPaginator

Type annotations for
`session.create_client("wisdom").get_paginator("list_assistant_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import ListAssistantAssociationsPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: ListAssistantAssociationsPaginator = client.get_paginator("list_assistant_associations")
```

Boto3 documentation:
[ConnectWisdomService.Paginator.ListAssistantAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistantAssociations)

Arguments for `ListAssistantAssociationsPaginator.paginate` method:

- `assistantId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssistantAssociationsPaginator.paginate` returns
`AsyncIterable`\[[ListAssistantAssociationsResponseTypeDef](./type_defs.md#listassistantassociationsresponsetypedef)\].

<a id="listassistantspaginator"></a>

## ListAssistantsPaginator

Type annotations for
`session.create_client("wisdom").get_paginator("list_assistants")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import ListAssistantsPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: ListAssistantsPaginator = client.get_paginator("list_assistants")
```

Boto3 documentation:
[ConnectWisdomService.Paginator.ListAssistants](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListAssistants)

Arguments for `ListAssistantsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssistantsPaginator.paginate` returns
`AsyncIterable`\[[ListAssistantsResponseTypeDef](./type_defs.md#listassistantsresponsetypedef)\].

<a id="listcontentspaginator"></a>

## ListContentsPaginator

Type annotations for
`session.create_client("wisdom").get_paginator("list_contents")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import ListContentsPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: ListContentsPaginator = client.get_paginator("list_contents")
```

Boto3 documentation:
[ConnectWisdomService.Paginator.ListContents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListContents)

Arguments for `ListContentsPaginator.paginate` method:

- `knowledgeBaseId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListContentsPaginator.paginate` returns
`AsyncIterable`\[[ListContentsResponseTypeDef](./type_defs.md#listcontentsresponsetypedef)\].

<a id="listknowledgebasespaginator"></a>

## ListKnowledgeBasesPaginator

Type annotations for
`session.create_client("wisdom").get_paginator("list_knowledge_bases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import ListKnowledgeBasesPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: ListKnowledgeBasesPaginator = client.get_paginator("list_knowledge_bases")
```

Boto3 documentation:
[ConnectWisdomService.Paginator.ListKnowledgeBases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.ListKnowledgeBases)

Arguments for `ListKnowledgeBasesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListKnowledgeBasesPaginator.paginate` returns
`AsyncIterable`\[[ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef)\].

<a id="queryassistantpaginator"></a>

## QueryAssistantPaginator

Type annotations for
`session.create_client("wisdom").get_paginator("query_assistant")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import QueryAssistantPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: QueryAssistantPaginator = client.get_paginator("query_assistant")
```

Boto3 documentation:
[ConnectWisdomService.Paginator.QueryAssistant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.QueryAssistant)

Arguments for `QueryAssistantPaginator.paginate` method:

- `assistantId`: `str` *(required)*
- `queryText`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`QueryAssistantPaginator.paginate` returns
`AsyncIterable`\[[QueryAssistantResponseTypeDef](./type_defs.md#queryassistantresponsetypedef)\].

<a id="searchcontentpaginator"></a>

## SearchContentPaginator

Type annotations for
`session.create_client("wisdom").get_paginator("search_content")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import SearchContentPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: SearchContentPaginator = client.get_paginator("search_content")
```

Boto3 documentation:
[ConnectWisdomService.Paginator.SearchContent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent)

Arguments for `SearchContentPaginator.paginate` method:

- `knowledgeBaseId`: `str` *(required)*
- `searchExpression`:
  [SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchContentPaginator.paginate` returns
`AsyncIterable`\[[SearchContentResponseTypeDef](./type_defs.md#searchcontentresponsetypedef)\].

<a id="searchsessionspaginator"></a>

## SearchSessionsPaginator

Type annotations for
`session.create_client("wisdom").get_paginator("search_sessions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_wisdom.paginator import SearchSessionsPaginator

session = get_session()
async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: SearchSessionsPaginator = client.get_paginator("search_sessions")
```

Boto3 documentation:
[ConnectWisdomService.Paginator.SearchSessions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions)

Arguments for `SearchSessionsPaginator.paginate` method:

- `assistantId`: `str` *(required)*
- `searchExpression`:
  [SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef)
  *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchSessionsPaginator.paginate` returns
`AsyncIterable`\[[SearchSessionsResponseTypeDef](./type_defs.md#searchsessionsresponsetypedef)\].
