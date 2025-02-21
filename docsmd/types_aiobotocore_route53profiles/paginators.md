# Paginators

> [Index](../README.md) > [Route53Profiles](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Route53Profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#route53profiles)
    type annotations stubs module [types-aiobotocore-route53profiles](https://pypi.org/project/types-aiobotocore-route53profiles/).

## ListProfileAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("route53profiles").get_paginator("list_profile_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles/paginator/ListProfileAssociations.html#Route53Profiles.Paginator.ListProfileAssociations)

```python
# ListProfileAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53profiles.paginator import ListProfileAssociationsPaginator

session = get_session()
async with session.create_client("route53profiles") as client:  # (1)
    paginator: ListProfileAssociationsPaginator = client.get_paginator("list_profile_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListProfileAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ProfilesClient](./client.md)
2. paginator: [ListProfileAssociationsPaginator](./paginators.md#listprofileassociationspaginator)
3. item: [:material-code-braces: ListProfileAssociationsResponseTypeDef](./type_defs.md#listprofileassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProfileAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProfileId: str = ...,
    ResourceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListProfileAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProfileAssociationsResponseTypeDef](./type_defs.md#listprofileassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProfileAssociationsRequestPaginateTypeDef = {  # (1)
    "ProfileId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProfileAssociationsRequestPaginateTypeDef](./type_defs.md#listprofileassociationsrequestpaginatetypedef) 
## ListProfileResourceAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("route53profiles").get_paginator("list_profile_resource_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles/paginator/ListProfileResourceAssociations.html#Route53Profiles.Paginator.ListProfileResourceAssociations)

```python
# ListProfileResourceAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53profiles.paginator import ListProfileResourceAssociationsPaginator

session = get_session()
async with session.create_client("route53profiles") as client:  # (1)
    paginator: ListProfileResourceAssociationsPaginator = client.get_paginator("list_profile_resource_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListProfileResourceAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ProfilesClient](./client.md)
2. paginator: [ListProfileResourceAssociationsPaginator](./paginators.md#listprofileresourceassociationspaginator)
3. item: [:material-code-braces: ListProfileResourceAssociationsResponseTypeDef](./type_defs.md#listprofileresourceassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProfileResourceAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProfileId: str,
    ResourceType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListProfileResourceAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProfileResourceAssociationsResponseTypeDef](./type_defs.md#listprofileresourceassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProfileResourceAssociationsRequestPaginateTypeDef = {  # (1)
    "ProfileId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProfileResourceAssociationsRequestPaginateTypeDef](./type_defs.md#listprofileresourceassociationsrequestpaginatetypedef) 
## ListProfilesPaginator

Type annotations and code completion for `#!python session.create_client("route53profiles").get_paginator("list_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles/paginator/ListProfiles.html#Route53Profiles.Paginator.ListProfiles)

```python
# ListProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53profiles.paginator import ListProfilesPaginator

session = get_session()
async with session.create_client("route53profiles") as client:  # (1)
    paginator: ListProfilesPaginator = client.get_paginator("list_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ProfilesClient](./client.md)
2. paginator: [ListProfilesPaginator](./paginators.md#listprofilespaginator)
3. item: [:material-code-braces: ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProfilesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProfilesRequestPaginateTypeDef](./type_defs.md#listprofilesrequestpaginatetypedef) 
