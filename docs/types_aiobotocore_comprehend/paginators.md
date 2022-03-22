<a id="paginators-for-aiobotocore-comprehend-module"></a>

# Paginators for aiobotocore Comprehend module

> [Index](../README.md) > [Comprehend](./README.md) > Paginators

Auto-generated documentation for
[Comprehend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
type annotations stubs module
[types-aiobotocore-comprehend](https://pypi.org/project/types-aiobotocore-comprehend/).

- [Paginators for aiobotocore Comprehend module](#paginators-for-aiobotocore-comprehend-module)
  - [ListDocumentClassificationJobsPaginator](#listdocumentclassificationjobspaginator)
  - [ListDocumentClassifiersPaginator](#listdocumentclassifierspaginator)
  - [ListDominantLanguageDetectionJobsPaginator](#listdominantlanguagedetectionjobspaginator)
  - [ListEntitiesDetectionJobsPaginator](#listentitiesdetectionjobspaginator)
  - [ListEntityRecognizersPaginator](#listentityrecognizerspaginator)
  - [ListKeyPhrasesDetectionJobsPaginator](#listkeyphrasesdetectionjobspaginator)
  - [ListSentimentDetectionJobsPaginator](#listsentimentdetectionjobspaginator)
  - [ListTopicsDetectionJobsPaginator](#listtopicsdetectionjobspaginator)

<a id="listdocumentclassificationjobspaginator"></a>

## ListDocumentClassificationJobsPaginator

Type annotations for
`session.create_client("comprehend").get_paginator("list_document_classification_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListDocumentClassificationJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:
    client: ComprehendClient
    paginator: ListDocumentClassificationJobsPaginator = client.get_paginator("list_document_classification_jobs")
```

Boto3 documentation:
[Comprehend.Paginator.ListDocumentClassificationJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs)

Arguments for `ListDocumentClassificationJobsPaginator.paginate` method:

- `Filter`:
  [DocumentClassificationJobFilterTypeDef](./type_defs.md#documentclassificationjobfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDocumentClassificationJobsPaginator.paginate` returns
`AsyncIterator`\[[ListDocumentClassificationJobsResponseTypeDef](./type_defs.md#listdocumentclassificationjobsresponsetypedef)\].

<a id="listdocumentclassifierspaginator"></a>

## ListDocumentClassifiersPaginator

Type annotations for
`session.create_client("comprehend").get_paginator("list_document_classifiers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListDocumentClassifiersPaginator

session = get_session()
async with session.create_client("comprehend") as client:
    client: ComprehendClient
    paginator: ListDocumentClassifiersPaginator = client.get_paginator("list_document_classifiers")
```

Boto3 documentation:
[Comprehend.Paginator.ListDocumentClassifiers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers)

Arguments for `ListDocumentClassifiersPaginator.paginate` method:

- `Filter`:
  [DocumentClassifierFilterTypeDef](./type_defs.md#documentclassifierfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDocumentClassifiersPaginator.paginate` returns
`AsyncIterator`\[[ListDocumentClassifiersResponseTypeDef](./type_defs.md#listdocumentclassifiersresponsetypedef)\].

<a id="listdominantlanguagedetectionjobspaginator"></a>

## ListDominantLanguageDetectionJobsPaginator

Type annotations for
`session.create_client("comprehend").get_paginator("list_dominant_language_detection_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListDominantLanguageDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:
    client: ComprehendClient
    paginator: ListDominantLanguageDetectionJobsPaginator = client.get_paginator("list_dominant_language_detection_jobs")
```

Boto3 documentation:
[Comprehend.Paginator.ListDominantLanguageDetectionJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs)

Arguments for `ListDominantLanguageDetectionJobsPaginator.paginate` method:

- `Filter`:
  [DominantLanguageDetectionJobFilterTypeDef](./type_defs.md#dominantlanguagedetectionjobfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDominantLanguageDetectionJobsPaginator.paginate` returns
`AsyncIterator`\[[ListDominantLanguageDetectionJobsResponseTypeDef](./type_defs.md#listdominantlanguagedetectionjobsresponsetypedef)\].

<a id="listentitiesdetectionjobspaginator"></a>

## ListEntitiesDetectionJobsPaginator

Type annotations for
`session.create_client("comprehend").get_paginator("list_entities_detection_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListEntitiesDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:
    client: ComprehendClient
    paginator: ListEntitiesDetectionJobsPaginator = client.get_paginator("list_entities_detection_jobs")
```

Boto3 documentation:
[Comprehend.Paginator.ListEntitiesDetectionJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs)

Arguments for `ListEntitiesDetectionJobsPaginator.paginate` method:

- `Filter`:
  [EntitiesDetectionJobFilterTypeDef](./type_defs.md#entitiesdetectionjobfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEntitiesDetectionJobsPaginator.paginate` returns
`AsyncIterator`\[[ListEntitiesDetectionJobsResponseTypeDef](./type_defs.md#listentitiesdetectionjobsresponsetypedef)\].

<a id="listentityrecognizerspaginator"></a>

## ListEntityRecognizersPaginator

Type annotations for
`session.create_client("comprehend").get_paginator("list_entity_recognizers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListEntityRecognizersPaginator

session = get_session()
async with session.create_client("comprehend") as client:
    client: ComprehendClient
    paginator: ListEntityRecognizersPaginator = client.get_paginator("list_entity_recognizers")
```

Boto3 documentation:
[Comprehend.Paginator.ListEntityRecognizers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers)

Arguments for `ListEntityRecognizersPaginator.paginate` method:

- `Filter`:
  [EntityRecognizerFilterTypeDef](./type_defs.md#entityrecognizerfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEntityRecognizersPaginator.paginate` returns
`AsyncIterator`\[[ListEntityRecognizersResponseTypeDef](./type_defs.md#listentityrecognizersresponsetypedef)\].

<a id="listkeyphrasesdetectionjobspaginator"></a>

## ListKeyPhrasesDetectionJobsPaginator

Type annotations for
`session.create_client("comprehend").get_paginator("list_key_phrases_detection_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListKeyPhrasesDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:
    client: ComprehendClient
    paginator: ListKeyPhrasesDetectionJobsPaginator = client.get_paginator("list_key_phrases_detection_jobs")
```

Boto3 documentation:
[Comprehend.Paginator.ListKeyPhrasesDetectionJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs)

Arguments for `ListKeyPhrasesDetectionJobsPaginator.paginate` method:

- `Filter`:
  [KeyPhrasesDetectionJobFilterTypeDef](./type_defs.md#keyphrasesdetectionjobfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListKeyPhrasesDetectionJobsPaginator.paginate` returns
`AsyncIterator`\[[ListKeyPhrasesDetectionJobsResponseTypeDef](./type_defs.md#listkeyphrasesdetectionjobsresponsetypedef)\].

<a id="listsentimentdetectionjobspaginator"></a>

## ListSentimentDetectionJobsPaginator

Type annotations for
`session.create_client("comprehend").get_paginator("list_sentiment_detection_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListSentimentDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:
    client: ComprehendClient
    paginator: ListSentimentDetectionJobsPaginator = client.get_paginator("list_sentiment_detection_jobs")
```

Boto3 documentation:
[Comprehend.Paginator.ListSentimentDetectionJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs)

Arguments for `ListSentimentDetectionJobsPaginator.paginate` method:

- `Filter`:
  [SentimentDetectionJobFilterTypeDef](./type_defs.md#sentimentdetectionjobfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSentimentDetectionJobsPaginator.paginate` returns
`AsyncIterator`\[[ListSentimentDetectionJobsResponseTypeDef](./type_defs.md#listsentimentdetectionjobsresponsetypedef)\].

<a id="listtopicsdetectionjobspaginator"></a>

## ListTopicsDetectionJobsPaginator

Type annotations for
`session.create_client("comprehend").get_paginator("list_topics_detection_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListTopicsDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:
    client: ComprehendClient
    paginator: ListTopicsDetectionJobsPaginator = client.get_paginator("list_topics_detection_jobs")
```

Boto3 documentation:
[Comprehend.Paginator.ListTopicsDetectionJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs)

Arguments for `ListTopicsDetectionJobsPaginator.paginate` method:

- `Filter`:
  [TopicsDetectionJobFilterTypeDef](./type_defs.md#topicsdetectionjobfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTopicsDetectionJobsPaginator.paginate` returns
`AsyncIterator`\[[ListTopicsDetectionJobsResponseTypeDef](./type_defs.md#listtopicsdetectionjobsresponsetypedef)\].
