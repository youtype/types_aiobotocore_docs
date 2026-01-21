# Paginators

> [Index](../README.md) > [Amplify](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Amplify](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#amplify)
    type annotations stubs module [types-aiobotocore-amplify](https://pypi.org/project/types-aiobotocore-amplify/).

## ListAppsPaginator

Type annotations and code completion for `#!python session.create_client("amplify").get_paginator("list_apps")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify/paginator/ListApps.html#Amplify.Paginator.ListApps)

```python
# ListAppsPaginator usage example

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
3. item: `AioPageIterator[ListAppsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAppsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAppsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAppsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAppsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppsRequestPaginateTypeDef](./type_defs.md#listappsrequestpaginatetypedef)
## ListBranchesPaginator

Type annotations and code completion for `#!python session.create_client("amplify").get_paginator("list_branches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify/paginator/ListBranches.html#Amplify.Paginator.ListBranches)

```python
# ListBranchesPaginator usage example

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
3. item: `AioPageIterator[ListBranchesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBranchesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBranchesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBranchesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBranchesRequestPaginateTypeDef = {  # (1)
    "appId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBranchesRequestPaginateTypeDef](./type_defs.md#listbranchesrequestpaginatetypedef)
## ListDomainAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("amplify").get_paginator("list_domain_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify/paginator/ListDomainAssociations.html#Amplify.Paginator.ListDomainAssociations)

```python
# ListDomainAssociationsPaginator usage example

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
3. item: `AioPageIterator[ListDomainAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDomainAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDomainAssociationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDomainAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainAssociationsRequestPaginateTypeDef = {  # (1)
    "appId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainAssociationsRequestPaginateTypeDef](./type_defs.md#listdomainassociationsrequestpaginatetypedef)
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("amplify").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify/paginator/ListJobs.html#Amplify.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

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
3. item: `AioPageIterator[ListJobsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appId: str,
    branchName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListJobsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListJobsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsRequestPaginateTypeDef = {  # (1)
    "appId": ...,
    "branchName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestPaginateTypeDef](./type_defs.md#listjobsrequestpaginatetypedef)
