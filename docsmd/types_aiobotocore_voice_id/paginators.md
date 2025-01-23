# Paginators

> [Index](../README.md) > [VoiceID](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [VoiceID](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#voiceid)
    type annotations stubs module [types-aiobotocore-voice-id](https://pypi.org/project/types-aiobotocore-voice-id/).

## ListDomainsPaginator

Type annotations and code completion for `#!python session.create_client("voice-id").get_paginator("list_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id/paginator/ListDomains.html#VoiceID.Paginator.ListDomains)

```python
# ListDomainsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_voice_id.paginator import ListDomainsPaginator

session = get_session()
async with session.create_client("voice-id") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsResponseTypeDef
        print(item)  # (3)
```

1. client: [VoiceIDClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDomainsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainsRequestPaginateTypeDef](./type_defs.md#listdomainsrequestpaginatetypedef) 
## ListFraudsterRegistrationJobsPaginator

Type annotations and code completion for `#!python session.create_client("voice-id").get_paginator("list_fraudster_registration_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id/paginator/ListFraudsterRegistrationJobs.html#VoiceID.Paginator.ListFraudsterRegistrationJobs)

```python
# ListFraudsterRegistrationJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_voice_id.paginator import ListFraudsterRegistrationJobsPaginator

session = get_session()
async with session.create_client("voice-id") as client:  # (1)
    paginator: ListFraudsterRegistrationJobsPaginator = client.get_paginator("list_fraudster_registration_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListFraudsterRegistrationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [VoiceIDClient](./client.md)
2. paginator: [ListFraudsterRegistrationJobsPaginator](./paginators.md#listfraudsterregistrationjobspaginator)
3. item: [:material-code-braces: ListFraudsterRegistrationJobsResponseTypeDef](./type_defs.md#listfraudsterregistrationjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFraudsterRegistrationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainId: str,
    JobStatus: FraudsterRegistrationJobStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListFraudsterRegistrationJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: FraudsterRegistrationJobStatusType](./literals.md#fraudsterregistrationjobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFraudsterRegistrationJobsResponseTypeDef](./type_defs.md#listfraudsterregistrationjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFraudsterRegistrationJobsRequestPaginateTypeDef = {  # (1)
    "DomainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFraudsterRegistrationJobsRequestPaginateTypeDef](./type_defs.md#listfraudsterregistrationjobsrequestpaginatetypedef) 
## ListFraudstersPaginator

Type annotations and code completion for `#!python session.create_client("voice-id").get_paginator("list_fraudsters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id/paginator/ListFraudsters.html#VoiceID.Paginator.ListFraudsters)

```python
# ListFraudstersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_voice_id.paginator import ListFraudstersPaginator

session = get_session()
async with session.create_client("voice-id") as client:  # (1)
    paginator: ListFraudstersPaginator = client.get_paginator("list_fraudsters")  # (2)
    async for item in paginator.paginate(...):
        item: ListFraudstersResponseTypeDef
        print(item)  # (3)
```

1. client: [VoiceIDClient](./client.md)
2. paginator: [ListFraudstersPaginator](./paginators.md#listfraudsterspaginator)
3. item: [:material-code-braces: ListFraudstersResponseTypeDef](./type_defs.md#listfraudstersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFraudstersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainId: str,
    WatchlistId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFraudstersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFraudstersResponseTypeDef](./type_defs.md#listfraudstersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFraudstersRequestPaginateTypeDef = {  # (1)
    "DomainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFraudstersRequestPaginateTypeDef](./type_defs.md#listfraudstersrequestpaginatetypedef) 
## ListSpeakerEnrollmentJobsPaginator

Type annotations and code completion for `#!python session.create_client("voice-id").get_paginator("list_speaker_enrollment_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id/paginator/ListSpeakerEnrollmentJobs.html#VoiceID.Paginator.ListSpeakerEnrollmentJobs)

```python
# ListSpeakerEnrollmentJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_voice_id.paginator import ListSpeakerEnrollmentJobsPaginator

session = get_session()
async with session.create_client("voice-id") as client:  # (1)
    paginator: ListSpeakerEnrollmentJobsPaginator = client.get_paginator("list_speaker_enrollment_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListSpeakerEnrollmentJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [VoiceIDClient](./client.md)
2. paginator: [ListSpeakerEnrollmentJobsPaginator](./paginators.md#listspeakerenrollmentjobspaginator)
3. item: [:material-code-braces: ListSpeakerEnrollmentJobsResponseTypeDef](./type_defs.md#listspeakerenrollmentjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSpeakerEnrollmentJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainId: str,
    JobStatus: SpeakerEnrollmentJobStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSpeakerEnrollmentJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SpeakerEnrollmentJobStatusType](./literals.md#speakerenrollmentjobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSpeakerEnrollmentJobsResponseTypeDef](./type_defs.md#listspeakerenrollmentjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSpeakerEnrollmentJobsRequestPaginateTypeDef = {  # (1)
    "DomainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSpeakerEnrollmentJobsRequestPaginateTypeDef](./type_defs.md#listspeakerenrollmentjobsrequestpaginatetypedef) 
## ListSpeakersPaginator

Type annotations and code completion for `#!python session.create_client("voice-id").get_paginator("list_speakers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id/paginator/ListSpeakers.html#VoiceID.Paginator.ListSpeakers)

```python
# ListSpeakersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_voice_id.paginator import ListSpeakersPaginator

session = get_session()
async with session.create_client("voice-id") as client:  # (1)
    paginator: ListSpeakersPaginator = client.get_paginator("list_speakers")  # (2)
    async for item in paginator.paginate(...):
        item: ListSpeakersResponseTypeDef
        print(item)  # (3)
```

1. client: [VoiceIDClient](./client.md)
2. paginator: [ListSpeakersPaginator](./paginators.md#listspeakerspaginator)
3. item: [:material-code-braces: ListSpeakersResponseTypeDef](./type_defs.md#listspeakersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSpeakersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSpeakersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSpeakersResponseTypeDef](./type_defs.md#listspeakersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSpeakersRequestPaginateTypeDef = {  # (1)
    "DomainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSpeakersRequestPaginateTypeDef](./type_defs.md#listspeakersrequestpaginatetypedef) 
## ListWatchlistsPaginator

Type annotations and code completion for `#!python session.create_client("voice-id").get_paginator("list_watchlists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id/paginator/ListWatchlists.html#VoiceID.Paginator.ListWatchlists)

```python
# ListWatchlistsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_voice_id.paginator import ListWatchlistsPaginator

session = get_session()
async with session.create_client("voice-id") as client:  # (1)
    paginator: ListWatchlistsPaginator = client.get_paginator("list_watchlists")  # (2)
    async for item in paginator.paginate(...):
        item: ListWatchlistsResponseTypeDef
        print(item)  # (3)
```

1. client: [VoiceIDClient](./client.md)
2. paginator: [ListWatchlistsPaginator](./paginators.md#listwatchlistspaginator)
3. item: [:material-code-braces: ListWatchlistsResponseTypeDef](./type_defs.md#listwatchlistsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWatchlistsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListWatchlistsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWatchlistsResponseTypeDef](./type_defs.md#listwatchlistsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWatchlistsRequestPaginateTypeDef = {  # (1)
    "DomainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWatchlistsRequestPaginateTypeDef](./type_defs.md#listwatchlistsrequestpaginatetypedef) 
