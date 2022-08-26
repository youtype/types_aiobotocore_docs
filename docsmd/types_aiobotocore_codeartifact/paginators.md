# Paginators

> [Index](../README.md) > [CodeArtifact](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CodeArtifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact)
    type annotations stubs module [types-aiobotocore-codeartifact](https://pypi.org/project/types-aiobotocore-codeartifact/).

## ListDomainsPaginator

Type annotations and code completion for `#!python session.create_client("codeartifact").get_paginator("list_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListDomains)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListDomainsPaginator

session = get_session()
async with session.create_client("codeartifact") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsResultTypeDef
        print(item)  # (3)
```

1. client: [CodeArtifactClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDomainsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListDomainsRequestListDomainsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainsRequestListDomainsPaginateTypeDef](./type_defs.md#listdomainsrequestlistdomainspaginatetypedef) 
## ListPackageVersionAssetsPaginator

Type annotations and code completion for `#!python session.create_client("codeartifact").get_paginator("list_package_version_assets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersionAssets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListPackageVersionAssetsPaginator

session = get_session()
async with session.create_client("codeartifact") as client:  # (1)
    paginator: ListPackageVersionAssetsPaginator = client.get_paginator("list_package_version_assets")  # (2)
    async for item in paginator.paginate(...):
        item: ListPackageVersionAssetsResultTypeDef
        print(item)  # (3)
```

1. client: [CodeArtifactClient](./client.md)
2. paginator: [ListPackageVersionAssetsPaginator](./paginators.md#listpackageversionassetspaginator)
3. item: [:material-code-braces: ListPackageVersionAssetsResultTypeDef](./type_defs.md#listpackageversionassetsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListPackageVersionAssetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    packageVersion: str,
    domainOwner: str = ...,
    namespace: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPackageVersionAssetsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPackageVersionAssetsResultTypeDef](./type_defs.md#listpackageversionassetsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef = {  # (1)
    "domain": ...,
    "repository": ...,
    "format": ...,
    "package": ...,
    "packageVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPackageVersionAssetsRequestListPackageVersionAssetsPaginateTypeDef](./type_defs.md#listpackageversionassetsrequestlistpackageversionassetspaginatetypedef) 
## ListPackageVersionsPaginator

Type annotations and code completion for `#!python session.create_client("codeartifact").get_paginator("list_package_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackageVersions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListPackageVersionsPaginator

session = get_session()
async with session.create_client("codeartifact") as client:  # (1)
    paginator: ListPackageVersionsPaginator = client.get_paginator("list_package_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPackageVersionsResultTypeDef
        print(item)  # (3)
```

1. client: [CodeArtifactClient](./client.md)
2. paginator: [ListPackageVersionsPaginator](./paginators.md#listpackageversionspaginator)
3. item: [:material-code-braces: ListPackageVersionsResultTypeDef](./type_defs.md#listpackageversionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListPackageVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    domain: str,
    repository: str,
    format: PackageFormatType,  # (1)
    package: str,
    domainOwner: str = ...,
    namespace: str = ...,
    status: PackageVersionStatusType = ...,  # (2)
    sortBy: PackageVersionSortTypeType = ...,  # (3)
    originType: PackageVersionOriginTypeType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AsyncIterator[ListPackageVersionsResultTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: PackageVersionStatusType](./literals.md#packageversionstatustype) 
3. See [:material-code-brackets: PackageVersionSortTypeType](./literals.md#packageversionsorttypetype) 
4. See [:material-code-brackets: PackageVersionOriginTypeType](./literals.md#packageversionorigintypetype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ListPackageVersionsResultTypeDef](./type_defs.md#listpackageversionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListPackageVersionsRequestListPackageVersionsPaginateTypeDef = {  # (1)
    "domain": ...,
    "repository": ...,
    "format": ...,
    "package": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPackageVersionsRequestListPackageVersionsPaginateTypeDef](./type_defs.md#listpackageversionsrequestlistpackageversionspaginatetypedef) 
## ListPackagesPaginator

Type annotations and code completion for `#!python session.create_client("codeartifact").get_paginator("list_packages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListPackages)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListPackagesPaginator

session = get_session()
async with session.create_client("codeartifact") as client:  # (1)
    paginator: ListPackagesPaginator = client.get_paginator("list_packages")  # (2)
    async for item in paginator.paginate(...):
        item: ListPackagesResultTypeDef
        print(item)  # (3)
```

1. client: [CodeArtifactClient](./client.md)
2. paginator: [ListPackagesPaginator](./paginators.md#listpackagespaginator)
3. item: [:material-code-braces: ListPackagesResultTypeDef](./type_defs.md#listpackagesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListPackagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    domain: str,
    repository: str,
    domainOwner: str = ...,
    format: PackageFormatType = ...,  # (1)
    namespace: str = ...,
    packagePrefix: str = ...,
    publish: AllowPublishType = ...,  # (2)
    upstream: AllowUpstreamType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[ListPackagesResultTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: PackageFormatType](./literals.md#packageformattype) 
2. See [:material-code-brackets: AllowPublishType](./literals.md#allowpublishtype) 
3. See [:material-code-brackets: AllowUpstreamType](./literals.md#allowupstreamtype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListPackagesResultTypeDef](./type_defs.md#listpackagesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListPackagesRequestListPackagesPaginateTypeDef = {  # (1)
    "domain": ...,
    "repository": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPackagesRequestListPackagesPaginateTypeDef](./type_defs.md#listpackagesrequestlistpackagespaginatetypedef) 
## ListRepositoriesPaginator

Type annotations and code completion for `#!python session.create_client("codeartifact").get_paginator("list_repositories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositories)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListRepositoriesPaginator

session = get_session()
async with session.create_client("codeartifact") as client:  # (1)
    paginator: ListRepositoriesPaginator = client.get_paginator("list_repositories")  # (2)
    async for item in paginator.paginate(...):
        item: ListRepositoriesResultTypeDef
        print(item)  # (3)
```

1. client: [CodeArtifactClient](./client.md)
2. paginator: [ListRepositoriesPaginator](./paginators.md#listrepositoriespaginator)
3. item: [:material-code-braces: ListRepositoriesResultTypeDef](./type_defs.md#listrepositoriesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListRepositoriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    repositoryPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRepositoriesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRepositoriesResultTypeDef](./type_defs.md#listrepositoriesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListRepositoriesRequestListRepositoriesPaginateTypeDef = {  # (1)
    "repositoryPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRepositoriesRequestListRepositoriesPaginateTypeDef](./type_defs.md#listrepositoriesrequestlistrepositoriespaginatetypedef) 
## ListRepositoriesInDomainPaginator

Type annotations and code completion for `#!python session.create_client("codeartifact").get_paginator("list_repositories_in_domain")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#CodeArtifact.Paginator.ListRepositoriesInDomain)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_codeartifact.paginator import ListRepositoriesInDomainPaginator

session = get_session()
async with session.create_client("codeartifact") as client:  # (1)
    paginator: ListRepositoriesInDomainPaginator = client.get_paginator("list_repositories_in_domain")  # (2)
    async for item in paginator.paginate(...):
        item: ListRepositoriesInDomainResultTypeDef
        print(item)  # (3)
```

1. client: [CodeArtifactClient](./client.md)
2. paginator: [ListRepositoriesInDomainPaginator](./paginators.md#listrepositoriesindomainpaginator)
3. item: [:material-code-braces: ListRepositoriesInDomainResultTypeDef](./type_defs.md#listrepositoriesindomainresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListRepositoriesInDomainPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    domain: str,
    domainOwner: str = ...,
    administratorAccount: str = ...,
    repositoryPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRepositoriesInDomainResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRepositoriesInDomainResultTypeDef](./type_defs.md#listrepositoriesindomainresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef = {  # (1)
    "domain": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRepositoriesInDomainRequestListRepositoriesInDomainPaginateTypeDef](./type_defs.md#listrepositoriesindomainrequestlistrepositoriesindomainpaginatetypedef) 
