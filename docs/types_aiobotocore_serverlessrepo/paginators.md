<a id="paginators-for-aiobotocore-serverlessapplicationrepository-module"></a>

# Paginators for aiobotocore ServerlessApplicationRepository module

> [Index](../README.md) > [ServerlessApplicationRepository](./README.md) >
> Paginators

Auto-generated documentation for
[ServerlessApplicationRepository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository)
type annotations stubs module
[types-aiobotocore-serverlessrepo](https://pypi.org/project/types-aiobotocore-serverlessrepo/).

- [Paginators for aiobotocore ServerlessApplicationRepository module](#paginators-for-aiobotocore-serverlessapplicationrepository-module)
  - [ListApplicationDependenciesPaginator](#listapplicationdependenciespaginator)
  - [ListApplicationVersionsPaginator](#listapplicationversionspaginator)
  - [ListApplicationsPaginator](#listapplicationspaginator)

<a id="listapplicationdependenciespaginator"></a>

## ListApplicationDependenciesPaginator

Type annotations for
`session.create_client("serverlessrepo").get_paginator("list_application_dependencies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_serverlessrepo.paginator import ListApplicationDependenciesPaginator

session = get_session()
async with session.create_client("serverlessrepo") as client:
    client: ServerlessApplicationRepositoryClient
    paginator: ListApplicationDependenciesPaginator = client.get_paginator("list_application_dependencies")
```

Boto3 documentation:
[ServerlessApplicationRepository.Paginator.ListApplicationDependencies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationDependencies)

Arguments for `ListApplicationDependenciesPaginator.paginate` method:

- `ApplicationId`: `str` *(required)*
- `SemanticVersion`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationDependenciesPaginator.paginate` returns
`AsyncIterator`\[[ListApplicationDependenciesResponseTypeDef](./type_defs.md#listapplicationdependenciesresponsetypedef)\].

<a id="listapplicationversionspaginator"></a>

## ListApplicationVersionsPaginator

Type annotations for
`session.create_client("serverlessrepo").get_paginator("list_application_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_serverlessrepo.paginator import ListApplicationVersionsPaginator

session = get_session()
async with session.create_client("serverlessrepo") as client:
    client: ServerlessApplicationRepositoryClient
    paginator: ListApplicationVersionsPaginator = client.get_paginator("list_application_versions")
```

Boto3 documentation:
[ServerlessApplicationRepository.Paginator.ListApplicationVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplicationVersions)

Arguments for `ListApplicationVersionsPaginator.paginate` method:

- `ApplicationId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationVersionsPaginator.paginate` returns
`AsyncIterator`\[[ListApplicationVersionsResponseTypeDef](./type_defs.md#listapplicationversionsresponsetypedef)\].

<a id="listapplicationspaginator"></a>

## ListApplicationsPaginator

Type annotations for
`session.create_client("serverlessrepo").get_paginator("list_applications")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_serverlessrepo.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("serverlessrepo") as client:
    client: ServerlessApplicationRepositoryClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
```

Boto3 documentation:
[ServerlessApplicationRepository.Paginator.ListApplications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Paginator.ListApplications)

Arguments for `ListApplicationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationsPaginator.paginate` returns
`AsyncIterator`\[[ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)\].
