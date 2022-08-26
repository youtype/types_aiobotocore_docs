# Paginators

> [Index](../README.md) > [Comprehend](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Comprehend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
    type annotations stubs module [types-aiobotocore-comprehend](https://pypi.org/project/types-aiobotocore-comprehend/).

## ListDocumentClassificationJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_document_classification_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListDocumentClassificationJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:  # (1)
    paginator: ListDocumentClassificationJobsPaginator = client.get_paginator("list_document_classification_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDocumentClassificationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListDocumentClassificationJobsPaginator](./paginators.md#listdocumentclassificationjobspaginator)
3. item: [:material-code-braces: ListDocumentClassificationJobsResponseTypeDef](./type_defs.md#listdocumentclassificationjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDocumentClassificationJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: DocumentClassificationJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDocumentClassificationJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DocumentClassificationJobFilterTypeDef](./type_defs.md#documentclassificationjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDocumentClassificationJobsResponseTypeDef](./type_defs.md#listdocumentclassificationjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDocumentClassificationJobsRequestListDocumentClassificationJobsPaginateTypeDef](./type_defs.md#listdocumentclassificationjobsrequestlistdocumentclassificationjobspaginatetypedef) 
## ListDocumentClassifiersPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_document_classifiers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListDocumentClassifiersPaginator

session = get_session()
async with session.create_client("comprehend") as client:  # (1)
    paginator: ListDocumentClassifiersPaginator = client.get_paginator("list_document_classifiers")  # (2)
    async for item in paginator.paginate(...):
        item: ListDocumentClassifiersResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListDocumentClassifiersPaginator](./paginators.md#listdocumentclassifierspaginator)
3. item: [:material-code-braces: ListDocumentClassifiersResponseTypeDef](./type_defs.md#listdocumentclassifiersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDocumentClassifiersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: DocumentClassifierFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDocumentClassifiersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DocumentClassifierFilterTypeDef](./type_defs.md#documentclassifierfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDocumentClassifiersResponseTypeDef](./type_defs.md#listdocumentclassifiersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDocumentClassifiersRequestListDocumentClassifiersPaginateTypeDef](./type_defs.md#listdocumentclassifiersrequestlistdocumentclassifierspaginatetypedef) 
## ListDominantLanguageDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_dominant_language_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListDominantLanguageDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:  # (1)
    paginator: ListDominantLanguageDetectionJobsPaginator = client.get_paginator("list_dominant_language_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDominantLanguageDetectionJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListDominantLanguageDetectionJobsPaginator](./paginators.md#listdominantlanguagedetectionjobspaginator)
3. item: [:material-code-braces: ListDominantLanguageDetectionJobsResponseTypeDef](./type_defs.md#listdominantlanguagedetectionjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDominantLanguageDetectionJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: DominantLanguageDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDominantLanguageDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DominantLanguageDetectionJobFilterTypeDef](./type_defs.md#dominantlanguagedetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDominantLanguageDetectionJobsResponseTypeDef](./type_defs.md#listdominantlanguagedetectionjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDominantLanguageDetectionJobsRequestListDominantLanguageDetectionJobsPaginateTypeDef](./type_defs.md#listdominantlanguagedetectionjobsrequestlistdominantlanguagedetectionjobspaginatetypedef) 
## ListEntitiesDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_entities_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListEntitiesDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:  # (1)
    paginator: ListEntitiesDetectionJobsPaginator = client.get_paginator("list_entities_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntitiesDetectionJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListEntitiesDetectionJobsPaginator](./paginators.md#listentitiesdetectionjobspaginator)
3. item: [:material-code-braces: ListEntitiesDetectionJobsResponseTypeDef](./type_defs.md#listentitiesdetectionjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEntitiesDetectionJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: EntitiesDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEntitiesDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EntitiesDetectionJobFilterTypeDef](./type_defs.md#entitiesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEntitiesDetectionJobsResponseTypeDef](./type_defs.md#listentitiesdetectionjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitiesDetectionJobsRequestListEntitiesDetectionJobsPaginateTypeDef](./type_defs.md#listentitiesdetectionjobsrequestlistentitiesdetectionjobspaginatetypedef) 
## ListEntityRecognizersPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_entity_recognizers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListEntityRecognizersPaginator

session = get_session()
async with session.create_client("comprehend") as client:  # (1)
    paginator: ListEntityRecognizersPaginator = client.get_paginator("list_entity_recognizers")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntityRecognizersResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListEntityRecognizersPaginator](./paginators.md#listentityrecognizerspaginator)
3. item: [:material-code-braces: ListEntityRecognizersResponseTypeDef](./type_defs.md#listentityrecognizersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEntityRecognizersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: EntityRecognizerFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListEntityRecognizersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EntityRecognizerFilterTypeDef](./type_defs.md#entityrecognizerfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEntityRecognizersResponseTypeDef](./type_defs.md#listentityrecognizersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntityRecognizersRequestListEntityRecognizersPaginateTypeDef](./type_defs.md#listentityrecognizersrequestlistentityrecognizerspaginatetypedef) 
## ListKeyPhrasesDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_key_phrases_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListKeyPhrasesDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:  # (1)
    paginator: ListKeyPhrasesDetectionJobsPaginator = client.get_paginator("list_key_phrases_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListKeyPhrasesDetectionJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListKeyPhrasesDetectionJobsPaginator](./paginators.md#listkeyphrasesdetectionjobspaginator)
3. item: [:material-code-braces: ListKeyPhrasesDetectionJobsResponseTypeDef](./type_defs.md#listkeyphrasesdetectionjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListKeyPhrasesDetectionJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListKeyPhrasesDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: KeyPhrasesDetectionJobFilterTypeDef](./type_defs.md#keyphrasesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListKeyPhrasesDetectionJobsResponseTypeDef](./type_defs.md#listkeyphrasesdetectionjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeyPhrasesDetectionJobsRequestListKeyPhrasesDetectionJobsPaginateTypeDef](./type_defs.md#listkeyphrasesdetectionjobsrequestlistkeyphrasesdetectionjobspaginatetypedef) 
## ListSentimentDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_sentiment_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListSentimentDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:  # (1)
    paginator: ListSentimentDetectionJobsPaginator = client.get_paginator("list_sentiment_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListSentimentDetectionJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListSentimentDetectionJobsPaginator](./paginators.md#listsentimentdetectionjobspaginator)
3. item: [:material-code-braces: ListSentimentDetectionJobsResponseTypeDef](./type_defs.md#listsentimentdetectionjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSentimentDetectionJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: SentimentDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSentimentDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SentimentDetectionJobFilterTypeDef](./type_defs.md#sentimentdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSentimentDetectionJobsResponseTypeDef](./type_defs.md#listsentimentdetectionjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSentimentDetectionJobsRequestListSentimentDetectionJobsPaginateTypeDef](./type_defs.md#listsentimentdetectionjobsrequestlistsentimentdetectionjobspaginatetypedef) 
## ListTopicsDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_topics_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListTopicsDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:  # (1)
    paginator: ListTopicsDetectionJobsPaginator = client.get_paginator("list_topics_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListTopicsDetectionJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListTopicsDetectionJobsPaginator](./paginators.md#listtopicsdetectionjobspaginator)
3. item: [:material-code-braces: ListTopicsDetectionJobsResponseTypeDef](./type_defs.md#listtopicsdetectionjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTopicsDetectionJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: TopicsDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListTopicsDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TopicsDetectionJobFilterTypeDef](./type_defs.md#topicsdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTopicsDetectionJobsResponseTypeDef](./type_defs.md#listtopicsdetectionjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTopicsDetectionJobsRequestListTopicsDetectionJobsPaginateTypeDef](./type_defs.md#listtopicsdetectionjobsrequestlisttopicsdetectionjobspaginatetypedef) 
