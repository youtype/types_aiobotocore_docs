# Paginators

> [Index](../README.md) > [Signer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
    type annotations stubs module [types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

## ListSigningJobsPaginator

Type annotations and code completion for `#!python session.create_client("signer").get_paginator("list_signing_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/paginator/ListSigningJobs.html#Signer.Paginator.ListSigningJobs)

```python
# ListSigningJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_signer.paginator import ListSigningJobsPaginator

session = get_session()
async with session.create_client("signer") as client:  # (1)
    paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListSigningJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [SignerClient](./client.md)
2. paginator: [ListSigningJobsPaginator](./paginators.md#listsigningjobspaginator)
3. item: [:material-code-braces: ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSigningJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    status: SigningStatusType = ...,  # (1)
    platformId: str = ...,
    requestedBy: str = ...,
    isRevoked: bool = ...,
    signatureExpiresBefore: TimestampTypeDef = ...,
    signatureExpiresAfter: TimestampTypeDef = ...,
    jobInvoker: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSigningJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SigningStatusType](./literals.md#signingstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSigningJobsRequestPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSigningJobsRequestPaginateTypeDef](./type_defs.md#listsigningjobsrequestpaginatetypedef) 
## ListSigningPlatformsPaginator

Type annotations and code completion for `#!python session.create_client("signer").get_paginator("list_signing_platforms")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/paginator/ListSigningPlatforms.html#Signer.Paginator.ListSigningPlatforms)

```python
# ListSigningPlatformsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_signer.paginator import ListSigningPlatformsPaginator

session = get_session()
async with session.create_client("signer") as client:  # (1)
    paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")  # (2)
    async for item in paginator.paginate(...):
        item: ListSigningPlatformsResponseTypeDef
        print(item)  # (3)
```

1. client: [SignerClient](./client.md)
2. paginator: [ListSigningPlatformsPaginator](./paginators.md#listsigningplatformspaginator)
3. item: [:material-code-braces: ListSigningPlatformsResponseTypeDef](./type_defs.md#listsigningplatformsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSigningPlatformsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    category: str = ...,
    partner: str = ...,
    target: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSigningPlatformsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSigningPlatformsResponseTypeDef](./type_defs.md#listsigningplatformsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSigningPlatformsRequestPaginateTypeDef = {  # (1)
    "category": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSigningPlatformsRequestPaginateTypeDef](./type_defs.md#listsigningplatformsrequestpaginatetypedef) 
## ListSigningProfilesPaginator

Type annotations and code completion for `#!python session.create_client("signer").get_paginator("list_signing_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer/paginator/ListSigningProfiles.html#Signer.Paginator.ListSigningProfiles)

```python
# ListSigningProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_signer.paginator import ListSigningProfilesPaginator

session = get_session()
async with session.create_client("signer") as client:  # (1)
    paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListSigningProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [SignerClient](./client.md)
2. paginator: [ListSigningProfilesPaginator](./paginators.md#listsigningprofilespaginator)
3. item: [:material-code-braces: ListSigningProfilesResponseTypeDef](./type_defs.md#listsigningprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSigningProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    includeCanceled: bool = ...,
    platformId: str = ...,
    statuses: Sequence[SigningProfileStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSigningProfilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SigningProfileStatusType](./literals.md#signingprofilestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSigningProfilesResponseTypeDef](./type_defs.md#listsigningprofilesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSigningProfilesRequestPaginateTypeDef = {  # (1)
    "includeCanceled": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSigningProfilesRequestPaginateTypeDef](./type_defs.md#listsigningprofilesrequestpaginatetypedef) 
