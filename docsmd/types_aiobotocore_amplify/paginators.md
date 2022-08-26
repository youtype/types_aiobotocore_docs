# Paginators

> [Index](../README.md) > [Amplify](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Amplify](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify)
    type annotations stubs module [types-aiobotocore-amplify](https://pypi.org/project/types-aiobotocore-amplify/).

## ListAppsPaginator

Type annotations and code completion for `#!python session.create_client("amplify").get_paginator("list_apps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListApps)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_amplify.paginator import ListAppsPaginator

session = get_session()
async with session.create_client("amplify") as client:  # (1)
    paginator: ListAppsPaginator = client.get_paginator("list_apps")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppsResultTypeDef
        print(item)  # (3)
```

1. client: [AmplifyClient](./client.md)
2. paginator: [ListAppsPaginator](./paginators.md#listappspaginator)
3. item: [:material-code-braces: ListAppsResultTypeDef](./type_defs.md#listappsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListAppsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAppsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppsResultTypeDef](./type_defs.md#listappsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListAppsRequestListAppsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppsRequestListAppsPaginateTypeDef](./type_defs.md#listappsrequestlistappspaginatetypedef) 
## ListBranchesPaginator

Type annotations and code completion for `#!python session.create_client("amplify").get_paginator("list_branches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListBranches)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_amplify.paginator import ListBranchesPaginator

session = get_session()
async with session.create_client("amplify") as client:  # (1)
    paginator: ListBranchesPaginator = client.get_paginator("list_branches")  # (2)
    async for item in paginator.paginate(...):
        item: ListBranchesResultTypeDef
        print(item)  # (3)
```

1. client: [AmplifyClient](./client.md)
2. paginator: [ListBranchesPaginator](./paginators.md#listbranchespaginator)
3. item: [:material-code-braces: ListBranchesResultTypeDef](./type_defs.md#listbranchesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListBranchesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBranchesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBranchesResultTypeDef](./type_defs.md#listbranchesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListBranchesRequestListBranchesPaginateTypeDef = {  # (1)
    "appId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBranchesRequestListBranchesPaginateTypeDef](./type_defs.md#listbranchesrequestlistbranchespaginatetypedef) 
## ListDomainAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("amplify").get_paginator("list_domain_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListDomainAssociations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_amplify.paginator import ListDomainAssociationsPaginator

session = get_session()
async with session.create_client("amplify") as client:  # (1)
    paginator: ListDomainAssociationsPaginator = client.get_paginator("list_domain_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [AmplifyClient](./client.md)
2. paginator: [ListDomainAssociationsPaginator](./paginators.md#listdomainassociationspaginator)
3. item: [:material-code-braces: ListDomainAssociationsResultTypeDef](./type_defs.md#listdomainassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDomainAssociationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDomainAssociationsResultTypeDef](./type_defs.md#listdomainassociationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef = {  # (1)
    "appId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainAssociationsRequestListDomainAssociationsPaginateTypeDef](./type_defs.md#listdomainassociationsrequestlistdomainassociationspaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("amplify").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Paginator.ListJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_amplify.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("amplify") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResultTypeDef
        print(item)  # (3)
```

1. client: [AmplifyClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    branchName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsRequestListJobsPaginateTypeDef = {  # (1)
    "appId": ...,
    "branchName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef) 
