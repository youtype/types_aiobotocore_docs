# Paginators

> [Index](../README.md) > [signer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
    type annotations stubs module [types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

## ListSigningJobsPaginator

Type annotations and code completion for `#!python session.create_client("signer").get_paginator("list_signing_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_signer.paginator import ListSigningJobsPaginator

session = get_session()
async with session.create_client("signer") as client:  # (1)
    paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListSigningJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [signerClient](./client.md)
2. paginator: [ListSigningJobsPaginator](./paginators.md#listsigningjobspaginator)
3. item: [:material-code-braces: ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSigningJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    status: SigningStatusType = ...,  # (1)
    platformId: str = ...,
    requestedBy: str = ...,
    isRevoked: bool = ...,
    signatureExpiresBefore: Union[datetime, str] = ...,
    signatureExpiresAfter: Union[datetime, str] = ...,
    jobInvoker: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSigningJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SigningStatusType](./literals.md#signingstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSigningJobsRequestListSigningJobsPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSigningJobsRequestListSigningJobsPaginateTypeDef](./type_defs.md#listsigningjobsrequestlistsigningjobspaginatetypedef) 
## ListSigningPlatformsPaginator

Type annotations and code completion for `#!python session.create_client("signer").get_paginator("list_signing_platforms")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_signer.paginator import ListSigningPlatformsPaginator

session = get_session()
async with session.create_client("signer") as client:  # (1)
    paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")  # (2)
    async for item in paginator.paginate(...):
        item: ListSigningPlatformsResponseTypeDef
        print(item)  # (3)
```

1. client: [signerClient](./client.md)
2. paginator: [ListSigningPlatformsPaginator](./paginators.md#listsigningplatformspaginator)
3. item: [:material-code-braces: ListSigningPlatformsResponseTypeDef](./type_defs.md#listsigningplatformsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSigningPlatformsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    category: str = ...,
    partner: str = ...,
    target: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSigningPlatformsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSigningPlatformsResponseTypeDef](./type_defs.md#listsigningplatformsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = {  # (1)
    "category": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef](./type_defs.md#listsigningplatformsrequestlistsigningplatformspaginatetypedef) 
## ListSigningProfilesPaginator

Type annotations and code completion for `#!python session.create_client("signer").get_paginator("list_signing_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_signer.paginator import ListSigningProfilesPaginator

session = get_session()
async with session.create_client("signer") as client:  # (1)
    paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListSigningProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [signerClient](./client.md)
2. paginator: [ListSigningProfilesPaginator](./paginators.md#listsigningprofilespaginator)
3. item: [:material-code-braces: ListSigningProfilesResponseTypeDef](./type_defs.md#listsigningprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSigningProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    includeCanceled: bool = ...,
    platformId: str = ...,
    statuses: Sequence[SigningProfileStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSigningProfilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SigningProfileStatusType](./literals.md#signingprofilestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSigningProfilesResponseTypeDef](./type_defs.md#listsigningprofilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = {  # (1)
    "includeCanceled": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSigningProfilesRequestListSigningProfilesPaginateTypeDef](./type_defs.md#listsigningprofilesrequestlistsigningprofilespaginatetypedef) 
