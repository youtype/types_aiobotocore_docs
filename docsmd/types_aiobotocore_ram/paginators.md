# Paginators

> [Index](../README.md) > [RAM](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [RAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#ram)
    type annotations stubs module [types-aiobotocore-ram](https://pypi.org/project/types-aiobotocore-ram/).

## GetResourcePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("ram").get_paginator("get_resource_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram/paginator/GetResourcePolicies.html#RAM.Paginator.GetResourcePolicies)

```python
# GetResourcePoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ram.paginator import GetResourcePoliciesPaginator

session = get_session()
async with session.create_client("ram") as client:  # (1)
    paginator: GetResourcePoliciesPaginator = client.get_paginator("get_resource_policies")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourcePoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [RAMClient](./client.md)
2. paginator: [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
3. item: [:material-code-braces: GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetResourcePoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArns: Sequence[str],
    principal: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetResourcePoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetResourcePoliciesResponseTypeDef](./type_defs.md#getresourcepoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetResourcePoliciesRequestPaginateTypeDef = {  # (1)
    "resourceArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourcePoliciesRequestPaginateTypeDef](./type_defs.md#getresourcepoliciesrequestpaginatetypedef) 
## GetResourceShareAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ram").get_paginator("get_resource_share_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram/paginator/GetResourceShareAssociations.html#RAM.Paginator.GetResourceShareAssociations)

```python
# GetResourceShareAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ram.paginator import GetResourceShareAssociationsPaginator

session = get_session()
async with session.create_client("ram") as client:  # (1)
    paginator: GetResourceShareAssociationsPaginator = client.get_paginator("get_resource_share_associations")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourceShareAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [RAMClient](./client.md)
2. paginator: [GetResourceShareAssociationsPaginator](./paginators.md#getresourceshareassociationspaginator)
3. item: [:material-code-braces: GetResourceShareAssociationsResponseTypeDef](./type_defs.md#getresourceshareassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetResourceShareAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    associationType: ResourceShareAssociationTypeType,  # (1)
    resourceShareArns: Sequence[str] = ...,
    resourceArn: str = ...,
    principal: str = ...,
    associationStatus: ResourceShareAssociationStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[GetResourceShareAssociationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceShareAssociationTypeType](./literals.md#resourceshareassociationtypetype) 
2. See [:material-code-brackets: ResourceShareAssociationStatusType](./literals.md#resourceshareassociationstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetResourceShareAssociationsResponseTypeDef](./type_defs.md#getresourceshareassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetResourceShareAssociationsRequestPaginateTypeDef = {  # (1)
    "associationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourceShareAssociationsRequestPaginateTypeDef](./type_defs.md#getresourceshareassociationsrequestpaginatetypedef) 
## GetResourceShareInvitationsPaginator

Type annotations and code completion for `#!python session.create_client("ram").get_paginator("get_resource_share_invitations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram/paginator/GetResourceShareInvitations.html#RAM.Paginator.GetResourceShareInvitations)

```python
# GetResourceShareInvitationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ram.paginator import GetResourceShareInvitationsPaginator

session = get_session()
async with session.create_client("ram") as client:  # (1)
    paginator: GetResourceShareInvitationsPaginator = client.get_paginator("get_resource_share_invitations")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourceShareInvitationsResponseTypeDef
        print(item)  # (3)
```

1. client: [RAMClient](./client.md)
2. paginator: [GetResourceShareInvitationsPaginator](./paginators.md#getresourceshareinvitationspaginator)
3. item: [:material-code-braces: GetResourceShareInvitationsResponseTypeDef](./type_defs.md#getresourceshareinvitationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetResourceShareInvitationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceShareInvitationArns: Sequence[str] = ...,
    resourceShareArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetResourceShareInvitationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetResourceShareInvitationsResponseTypeDef](./type_defs.md#getresourceshareinvitationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetResourceShareInvitationsRequestPaginateTypeDef = {  # (1)
    "resourceShareInvitationArns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourceShareInvitationsRequestPaginateTypeDef](./type_defs.md#getresourceshareinvitationsrequestpaginatetypedef) 
## GetResourceSharesPaginator

Type annotations and code completion for `#!python session.create_client("ram").get_paginator("get_resource_shares")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram/paginator/GetResourceShares.html#RAM.Paginator.GetResourceShares)

```python
# GetResourceSharesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ram.paginator import GetResourceSharesPaginator

session = get_session()
async with session.create_client("ram") as client:  # (1)
    paginator: GetResourceSharesPaginator = client.get_paginator("get_resource_shares")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourceSharesResponseTypeDef
        print(item)  # (3)
```

1. client: [RAMClient](./client.md)
2. paginator: [GetResourceSharesPaginator](./paginators.md#getresourcesharespaginator)
3. item: [:material-code-braces: GetResourceSharesResponseTypeDef](./type_defs.md#getresourcesharesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetResourceSharesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceOwner: ResourceOwnerType,  # (1)
    resourceShareArns: Sequence[str] = ...,
    resourceShareStatus: ResourceShareStatusType = ...,  # (2)
    name: str = ...,
    tagFilters: Sequence[TagFilterTypeDef] = ...,  # (3)
    permissionArn: str = ...,
    permissionVersion: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[GetResourceSharesResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-brackets: ResourceShareStatusType](./literals.md#resourcesharestatustype) 
3. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: GetResourceSharesResponseTypeDef](./type_defs.md#getresourcesharesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetResourceSharesRequestPaginateTypeDef = {  # (1)
    "resourceOwner": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourceSharesRequestPaginateTypeDef](./type_defs.md#getresourcesharesrequestpaginatetypedef) 
## ListPrincipalsPaginator

Type annotations and code completion for `#!python session.create_client("ram").get_paginator("list_principals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram/paginator/ListPrincipals.html#RAM.Paginator.ListPrincipals)

```python
# ListPrincipalsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ram.paginator import ListPrincipalsPaginator

session = get_session()
async with session.create_client("ram") as client:  # (1)
    paginator: ListPrincipalsPaginator = client.get_paginator("list_principals")  # (2)
    async for item in paginator.paginate(...):
        item: ListPrincipalsResponseTypeDef
        print(item)  # (3)
```

1. client: [RAMClient](./client.md)
2. paginator: [ListPrincipalsPaginator](./paginators.md#listprincipalspaginator)
3. item: [:material-code-braces: ListPrincipalsResponseTypeDef](./type_defs.md#listprincipalsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPrincipalsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceOwner: ResourceOwnerType,  # (1)
    resourceArn: str = ...,
    principals: Sequence[str] = ...,
    resourceType: str = ...,
    resourceShareArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListPrincipalsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPrincipalsResponseTypeDef](./type_defs.md#listprincipalsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPrincipalsRequestPaginateTypeDef = {  # (1)
    "resourceOwner": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPrincipalsRequestPaginateTypeDef](./type_defs.md#listprincipalsrequestpaginatetypedef) 
## ListResourcesPaginator

Type annotations and code completion for `#!python session.create_client("ram").get_paginator("list_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram/paginator/ListResources.html#RAM.Paginator.ListResources)

```python
# ListResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ram.paginator import ListResourcesPaginator

session = get_session()
async with session.create_client("ram") as client:  # (1)
    paginator: ListResourcesPaginator = client.get_paginator("list_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [RAMClient](./client.md)
2. paginator: [ListResourcesPaginator](./paginators.md#listresourcespaginator)
3. item: [:material-code-braces: ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceOwner: ResourceOwnerType,  # (1)
    principal: str = ...,
    resourceType: str = ...,
    resourceArns: Sequence[str] = ...,
    resourceShareArns: Sequence[str] = ...,
    resourceRegionScope: ResourceRegionScopeFilterType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListResourcesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-brackets: ResourceRegionScopeFilterType](./literals.md#resourceregionscopefiltertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListResourcesResponseTypeDef](./type_defs.md#listresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourcesRequestPaginateTypeDef = {  # (1)
    "resourceOwner": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourcesRequestPaginateTypeDef](./type_defs.md#listresourcesrequestpaginatetypedef) 
