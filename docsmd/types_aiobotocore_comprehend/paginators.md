# Paginators

> [Index](../README.md) > [Comprehend](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Comprehend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#comprehend)
    type annotations stubs module [types-aiobotocore-comprehend](https://pypi.org/project/types-aiobotocore-comprehend/).

## ListDocumentClassificationJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_document_classification_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend/paginator/ListDocumentClassificationJobs.html#Comprehend.Paginator.ListDocumentClassificationJobs)

```python
# ListDocumentClassificationJobsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: DocumentClassificationJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDocumentClassificationJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DocumentClassificationJobFilterTypeDef](./type_defs.md#documentclassificationjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDocumentClassificationJobsResponseTypeDef](./type_defs.md#listdocumentclassificationjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDocumentClassificationJobsRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDocumentClassificationJobsRequestPaginateTypeDef](./type_defs.md#listdocumentclassificationjobsrequestpaginatetypedef) 
## ListDocumentClassifiersPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_document_classifiers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend/paginator/ListDocumentClassifiers.html#Comprehend.Paginator.ListDocumentClassifiers)

```python
# ListDocumentClassifiersPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: DocumentClassifierFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDocumentClassifiersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DocumentClassifierFilterTypeDef](./type_defs.md#documentclassifierfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDocumentClassifiersResponseTypeDef](./type_defs.md#listdocumentclassifiersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDocumentClassifiersRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDocumentClassifiersRequestPaginateTypeDef](./type_defs.md#listdocumentclassifiersrequestpaginatetypedef) 
## ListDominantLanguageDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_dominant_language_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend/paginator/ListDominantLanguageDetectionJobs.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs)

```python
# ListDominantLanguageDetectionJobsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: DominantLanguageDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDominantLanguageDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DominantLanguageDetectionJobFilterTypeDef](./type_defs.md#dominantlanguagedetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDominantLanguageDetectionJobsResponseTypeDef](./type_defs.md#listdominantlanguagedetectionjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDominantLanguageDetectionJobsRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDominantLanguageDetectionJobsRequestPaginateTypeDef](./type_defs.md#listdominantlanguagedetectionjobsrequestpaginatetypedef) 
## ListEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend/paginator/ListEndpoints.html#Comprehend.Paginator.ListEndpoints)

```python
# ListEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListEndpointsPaginator

session = get_session()
async with session.create_client("comprehend") as client:  # (1)
    paginator: ListEndpointsPaginator = client.get_paginator("list_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
3. item: [:material-code-braces: ListEndpointsResponseTypeDef](./type_defs.md#listendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: EndpointFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListEndpointsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EndpointFilterTypeDef](./type_defs.md#endpointfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEndpointsResponseTypeDef](./type_defs.md#listendpointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEndpointsRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEndpointsRequestPaginateTypeDef](./type_defs.md#listendpointsrequestpaginatetypedef) 
## ListEntitiesDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_entities_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend/paginator/ListEntitiesDetectionJobs.html#Comprehend.Paginator.ListEntitiesDetectionJobs)

```python
# ListEntitiesDetectionJobsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: EntitiesDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListEntitiesDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EntitiesDetectionJobFilterTypeDef](./type_defs.md#entitiesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEntitiesDetectionJobsResponseTypeDef](./type_defs.md#listentitiesdetectionjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEntitiesDetectionJobsRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitiesDetectionJobsRequestPaginateTypeDef](./type_defs.md#listentitiesdetectionjobsrequestpaginatetypedef) 
## ListEntityRecognizersPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_entity_recognizers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend/paginator/ListEntityRecognizers.html#Comprehend.Paginator.ListEntityRecognizers)

```python
# ListEntityRecognizersPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: EntityRecognizerFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListEntityRecognizersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: EntityRecognizerFilterTypeDef](./type_defs.md#entityrecognizerfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListEntityRecognizersResponseTypeDef](./type_defs.md#listentityrecognizersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEntityRecognizersRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntityRecognizersRequestPaginateTypeDef](./type_defs.md#listentityrecognizersrequestpaginatetypedef) 
## ListKeyPhrasesDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_key_phrases_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend/paginator/ListKeyPhrasesDetectionJobs.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs)

```python
# ListKeyPhrasesDetectionJobsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListKeyPhrasesDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: KeyPhrasesDetectionJobFilterTypeDef](./type_defs.md#keyphrasesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListKeyPhrasesDetectionJobsResponseTypeDef](./type_defs.md#listkeyphrasesdetectionjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKeyPhrasesDetectionJobsRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeyPhrasesDetectionJobsRequestPaginateTypeDef](./type_defs.md#listkeyphrasesdetectionjobsrequestpaginatetypedef) 
## ListPiiEntitiesDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_pii_entities_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend/paginator/ListPiiEntitiesDetectionJobs.html#Comprehend.Paginator.ListPiiEntitiesDetectionJobs)

```python
# ListPiiEntitiesDetectionJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_comprehend.paginator import ListPiiEntitiesDetectionJobsPaginator

session = get_session()
async with session.create_client("comprehend") as client:  # (1)
    paginator: ListPiiEntitiesDetectionJobsPaginator = client.get_paginator("list_pii_entities_detection_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListPiiEntitiesDetectionJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ComprehendClient](./client.md)
2. paginator: [ListPiiEntitiesDetectionJobsPaginator](./paginators.md#listpiientitiesdetectionjobspaginator)
3. item: [:material-code-braces: ListPiiEntitiesDetectionJobsResponseTypeDef](./type_defs.md#listpiientitiesdetectionjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPiiEntitiesDetectionJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListPiiEntitiesDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: PiiEntitiesDetectionJobFilterTypeDef](./type_defs.md#piientitiesdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPiiEntitiesDetectionJobsResponseTypeDef](./type_defs.md#listpiientitiesdetectionjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPiiEntitiesDetectionJobsRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPiiEntitiesDetectionJobsRequestPaginateTypeDef](./type_defs.md#listpiientitiesdetectionjobsrequestpaginatetypedef) 
## ListSentimentDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_sentiment_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend/paginator/ListSentimentDetectionJobs.html#Comprehend.Paginator.ListSentimentDetectionJobs)

```python
# ListSentimentDetectionJobsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: SentimentDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSentimentDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SentimentDetectionJobFilterTypeDef](./type_defs.md#sentimentdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSentimentDetectionJobsResponseTypeDef](./type_defs.md#listsentimentdetectionjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSentimentDetectionJobsRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSentimentDetectionJobsRequestPaginateTypeDef](./type_defs.md#listsentimentdetectionjobsrequestpaginatetypedef) 
## ListTopicsDetectionJobsPaginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator("list_topics_detection_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend/paginator/ListTopicsDetectionJobs.html#Comprehend.Paginator.ListTopicsDetectionJobs)

```python
# ListTopicsDetectionJobsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    Filter: TopicsDetectionJobFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListTopicsDetectionJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TopicsDetectionJobFilterTypeDef](./type_defs.md#topicsdetectionjobfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTopicsDetectionJobsResponseTypeDef](./type_defs.md#listtopicsdetectionjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTopicsDetectionJobsRequestPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTopicsDetectionJobsRequestPaginateTypeDef](./type_defs.md#listtopicsdetectionjobsrequestpaginatetypedef) 
