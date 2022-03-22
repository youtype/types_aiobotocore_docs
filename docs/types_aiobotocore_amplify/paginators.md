<a id="paginators-for-aiobotocore-amplify-module"></a>

# Paginators for aiobotocore Amplify module

> [Index](../README.md) > [Amplify](./README.md) > Paginators

Auto-generated documentation for
[Amplify](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
type annotations stubs module
[types-aiobotocore-amplify](https://pypi.org/project/types-aiobotocore-amplify/).

- [Paginators for aiobotocore Amplify module](#paginators-for-aiobotocore-amplify-module)
  - [ListAppsPaginator](#listappspaginator)
  - [ListBranchesPaginator](#listbranchespaginator)
  - [ListDomainAssociationsPaginator](#listdomainassociationspaginator)
  - [ListJobsPaginator](#listjobspaginator)

<a id="listappspaginator"></a>

## ListAppsPaginator

Type annotations for
`session.create_client("amplify").get_paginator("list_apps")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplify.paginator import ListAppsPaginator

session = get_session()
async with session.create_client("amplify") as client:
    client: AmplifyClient
    paginator: ListAppsPaginator = client.get_paginator("list_apps")
```

Boto3 documentation:
[Amplify.Paginator.ListApps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListApps)

Arguments for `ListAppsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAppsPaginator.paginate` returns
`AsyncIterator`\[[ListAppsResultTypeDef](./type_defs.md#listappsresulttypedef)\].

<a id="listbranchespaginator"></a>

## ListBranchesPaginator

Type annotations for
`session.create_client("amplify").get_paginator("list_branches")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplify.paginator import ListBranchesPaginator

session = get_session()
async with session.create_client("amplify") as client:
    client: AmplifyClient
    paginator: ListBranchesPaginator = client.get_paginator("list_branches")
```

Boto3 documentation:
[Amplify.Paginator.ListBranches](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListBranches)

Arguments for `ListBranchesPaginator.paginate` method:

- `appId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListBranchesPaginator.paginate` returns
`AsyncIterator`\[[ListBranchesResultTypeDef](./type_defs.md#listbranchesresulttypedef)\].

<a id="listdomainassociationspaginator"></a>

## ListDomainAssociationsPaginator

Type annotations for
`session.create_client("amplify").get_paginator("list_domain_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplify.paginator import ListDomainAssociationsPaginator

session = get_session()
async with session.create_client("amplify") as client:
    client: AmplifyClient
    paginator: ListDomainAssociationsPaginator = client.get_paginator("list_domain_associations")
```

Boto3 documentation:
[Amplify.Paginator.ListDomainAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListDomainAssociations)

Arguments for `ListDomainAssociationsPaginator.paginate` method:

- `appId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDomainAssociationsPaginator.paginate` returns
`AsyncIterator`\[[ListDomainAssociationsResultTypeDef](./type_defs.md#listdomainassociationsresulttypedef)\].

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for
`session.create_client("amplify").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplify.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("amplify") as client:
    client: AmplifyClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```

Boto3 documentation:
[Amplify.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `appId`: `str` *(required)*
- `branchName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`AsyncIterator`\[[ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef)\].
