<a id="paginators-for-aiobotocore-signer-module"></a>

# Paginators for aiobotocore signer module

> [Index](../README.md) > [signer](./README.md) > Paginators

Auto-generated documentation for
[signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
type annotations stubs module
[types-aiobotocore-signer](https://pypi.org/project/types-aiobotocore-signer/).

- [Paginators for aiobotocore signer module](#paginators-for-aiobotocore-signer-module)
  - [ListSigningJobsPaginator](#listsigningjobspaginator)
  - [ListSigningPlatformsPaginator](#listsigningplatformspaginator)
  - [ListSigningProfilesPaginator](#listsigningprofilespaginator)

<a id="listsigningjobspaginator"></a>

## ListSigningJobsPaginator

Type annotations for
`session.create_client("signer").get_paginator("list_signing_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_signer.paginator import ListSigningJobsPaginator

session = get_session()
async with session.create_client("signer") as client:
    client: signerClient
    paginator: ListSigningJobsPaginator = client.get_paginator("list_signing_jobs")
```

Boto3 documentation:
[signer.Paginator.ListSigningJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs)

Arguments for `ListSigningJobsPaginator.paginate` method:

- `status`: [SigningStatusType](./literals.md#signingstatustype)
- `platformId`: `str`
- `requestedBy`: `str`
- `isRevoked`: `bool`
- `signatureExpiresBefore`: `Union`\[`datetime`, `str`\]
- `signatureExpiresAfter`: `Union`\[`datetime`, `str`\]
- `jobInvoker`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSigningJobsPaginator.paginate` returns
`AsyncIterator`\[[ListSigningJobsResponseTypeDef](./type_defs.md#listsigningjobsresponsetypedef)\].

<a id="listsigningplatformspaginator"></a>

## ListSigningPlatformsPaginator

Type annotations for
`session.create_client("signer").get_paginator("list_signing_platforms")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_signer.paginator import ListSigningPlatformsPaginator

session = get_session()
async with session.create_client("signer") as client:
    client: signerClient
    paginator: ListSigningPlatformsPaginator = client.get_paginator("list_signing_platforms")
```

Boto3 documentation:
[signer.Paginator.ListSigningPlatforms](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms)

Arguments for `ListSigningPlatformsPaginator.paginate` method:

- `category`: `str`
- `partner`: `str`
- `target`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSigningPlatformsPaginator.paginate` returns
`AsyncIterator`\[[ListSigningPlatformsResponseTypeDef](./type_defs.md#listsigningplatformsresponsetypedef)\].

<a id="listsigningprofilespaginator"></a>

## ListSigningProfilesPaginator

Type annotations for
`session.create_client("signer").get_paginator("list_signing_profiles")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_signer.paginator import ListSigningProfilesPaginator

session = get_session()
async with session.create_client("signer") as client:
    client: signerClient
    paginator: ListSigningProfilesPaginator = client.get_paginator("list_signing_profiles")
```

Boto3 documentation:
[signer.Paginator.ListSigningProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles)

Arguments for `ListSigningProfilesPaginator.paginate` method:

- `includeCanceled`: `bool`
- `platformId`: `str`
- `statuses`:
  `Sequence`\[[SigningProfileStatusType](./literals.md#signingprofilestatustype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSigningProfilesPaginator.paginate` returns
`AsyncIterator`\[[ListSigningProfilesResponseTypeDef](./type_defs.md#listsigningprofilesresponsetypedef)\].
