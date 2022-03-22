<a id="paginators-for-aiobotocore-codeartifact-module"></a>

# Paginators for aiobotocore CodeArtifact module

> [Index](../README.md) > [CodeArtifact](./README.md) > Paginators

Auto-generated documentation for
[CodeArtifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
type annotations stubs module
[types-aiobotocore-codeartifact](https://pypi.org/project/types-aiobotocore-codeartifact/).

- [Paginators for aiobotocore CodeArtifact module](#paginators-for-aiobotocore-codeartifact-module)
  - [ListDomainsPaginator](#listdomainspaginator)
  - [ListPackageVersionAssetsPaginator](#listpackageversionassetspaginator)
  - [ListPackageVersionsPaginator](#listpackageversionspaginator)
  - [ListPackagesPaginator](#listpackagespaginator)
  - [ListRepositoriesPaginator](#listrepositoriespaginator)
  - [ListRepositoriesInDomainPaginator](#listrepositoriesindomainpaginator)

<a id="listdomainspaginator"></a>

## ListDomainsPaginator

Type annotations for
`session.create_client("codeartifact").get_paginator("list_domains")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListDomainsPaginator

session = get_session()
async with session.create_client("codeartifact") as client:
    client: CodeArtifactClient
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")
```

Boto3 documentation:
[CodeArtifact.Paginator.ListDomains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains)

Arguments for `ListDomainsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDomainsPaginator.paginate` returns
`AsyncIterator`\[[ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef)\].

<a id="listpackageversionassetspaginator"></a>

## ListPackageVersionAssetsPaginator

Type annotations for
`session.create_client("codeartifact").get_paginator("list_package_version_assets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListPackageVersionAssetsPaginator

session = get_session()
async with session.create_client("codeartifact") as client:
    client: CodeArtifactClient
    paginator: ListPackageVersionAssetsPaginator = client.get_paginator("list_package_version_assets")
```

Boto3 documentation:
[CodeArtifact.Paginator.ListPackageVersionAssets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets)

Arguments for `ListPackageVersionAssetsPaginator.paginate` method:

- `domain`: `str` *(required)*
- `repository`: `str` *(required)*
- `format`: [PackageFormatType](./literals.md#packageformattype) *(required)*
- `package`: `str` *(required)*
- `packageVersion`: `str` *(required)*
- `domainOwner`: `str`
- `namespace`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPackageVersionAssetsPaginator.paginate` returns
`AsyncIterator`\[[ListPackageVersionAssetsResultTypeDef](./type_defs.md#listpackageversionassetsresulttypedef)\].

<a id="listpackageversionspaginator"></a>

## ListPackageVersionsPaginator

Type annotations for
`session.create_client("codeartifact").get_paginator("list_package_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListPackageVersionsPaginator

session = get_session()
async with session.create_client("codeartifact") as client:
    client: CodeArtifactClient
    paginator: ListPackageVersionsPaginator = client.get_paginator("list_package_versions")
```

Boto3 documentation:
[CodeArtifact.Paginator.ListPackageVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions)

Arguments for `ListPackageVersionsPaginator.paginate` method:

- `domain`: `str` *(required)*
- `repository`: `str` *(required)*
- `format`: [PackageFormatType](./literals.md#packageformattype) *(required)*
- `package`: `str` *(required)*
- `domainOwner`: `str`
- `namespace`: `str`
- `status`: [PackageVersionStatusType](./literals.md#packageversionstatustype)
- `sortBy`: `Literal['PUBLISHED_TIME']` (see
  [PackageVersionSortTypeType](./literals.md#packageversionsorttypetype))
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPackageVersionsPaginator.paginate` returns
`AsyncIterator`\[[ListPackageVersionsResultTypeDef](./type_defs.md#listpackageversionsresulttypedef)\].

<a id="listpackagespaginator"></a>

## ListPackagesPaginator

Type annotations for
`session.create_client("codeartifact").get_paginator("list_packages")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListPackagesPaginator

session = get_session()
async with session.create_client("codeartifact") as client:
    client: CodeArtifactClient
    paginator: ListPackagesPaginator = client.get_paginator("list_packages")
```

Boto3 documentation:
[CodeArtifact.Paginator.ListPackages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages)

Arguments for `ListPackagesPaginator.paginate` method:

- `domain`: `str` *(required)*
- `repository`: `str` *(required)*
- `domainOwner`: `str`
- `format`: [PackageFormatType](./literals.md#packageformattype)
- `namespace`: `str`
- `packagePrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPackagesPaginator.paginate` returns
`AsyncIterator`\[[ListPackagesResultTypeDef](./type_defs.md#listpackagesresulttypedef)\].

<a id="listrepositoriespaginator"></a>

## ListRepositoriesPaginator

Type annotations for
`session.create_client("codeartifact").get_paginator("list_repositories")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListRepositoriesPaginator

session = get_session()
async with session.create_client("codeartifact") as client:
    client: CodeArtifactClient
    paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")
```

Boto3 documentation:
[CodeArtifact.Paginator.ListRepositories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories)

Arguments for `ListRepositoriesPaginator.paginate` method:

- `repositoryPrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRepositoriesPaginator.paginate` returns
`AsyncIterator`\[[ListRepositoriesResultTypeDef](./type_defs.md#listrepositoriesresulttypedef)\].

<a id="listrepositoriesindomainpaginator"></a>

## ListRepositoriesInDomainPaginator

Type annotations for
`session.create_client("codeartifact").get_paginator("list_repositories_in_domain")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListRepositoriesInDomainPaginator

session = get_session()
async with session.create_client("codeartifact") as client:
    client: CodeArtifactClient
    paginator: ListRepositoriesInDomainPaginator = client.get_paginator("list_repositories_in_domain")
```

Boto3 documentation:
[CodeArtifact.Paginator.ListRepositoriesInDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain)

Arguments for `ListRepositoriesInDomainPaginator.paginate` method:

- `domain`: `str` *(required)*
- `domainOwner`: `str`
- `administratorAccount`: `str`
- `repositoryPrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRepositoriesInDomainPaginator.paginate` returns
`AsyncIterator`\[[ListRepositoriesInDomainResultTypeDef](./type_defs.md#listrepositoriesindomainresulttypedef)\].
