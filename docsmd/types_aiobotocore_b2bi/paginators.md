# Paginators

> [Index](../README.md) > [B2BI](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [B2BI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#b2bi)
    type annotations stubs module [types-aiobotocore-b2bi](https://pypi.org/project/types-aiobotocore-b2bi/).

## ListCapabilitiesPaginator

Type annotations and code completion for `#!python session.create_client("b2bi").get_paginator("list_capabilities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi/paginator/ListCapabilities.html#B2BI.Paginator.ListCapabilities)

```python
# ListCapabilitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_b2bi.paginator import ListCapabilitiesPaginator

session = get_session()
async with session.create_client("b2bi") as client:  # (1)
    paginator: ListCapabilitiesPaginator = client.get_paginator("list_capabilities")  # (2)
    async for item in paginator.paginate(...):
        item: ListCapabilitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [B2BIClient](./client.md)
2. paginator: [ListCapabilitiesPaginator](./paginators.md#listcapabilitiespaginator)
3. item: [:material-code-braces: ListCapabilitiesResponseTypeDef](./type_defs.md#listcapabilitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCapabilitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCapabilitiesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCapabilitiesResponseTypeDef](./type_defs.md#listcapabilitiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCapabilitiesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCapabilitiesRequestPaginateTypeDef](./type_defs.md#listcapabilitiesrequestpaginatetypedef) 
## ListPartnershipsPaginator

Type annotations and code completion for `#!python session.create_client("b2bi").get_paginator("list_partnerships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi/paginator/ListPartnerships.html#B2BI.Paginator.ListPartnerships)

```python
# ListPartnershipsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_b2bi.paginator import ListPartnershipsPaginator

session = get_session()
async with session.create_client("b2bi") as client:  # (1)
    paginator: ListPartnershipsPaginator = client.get_paginator("list_partnerships")  # (2)
    async for item in paginator.paginate(...):
        item: ListPartnershipsResponseTypeDef
        print(item)  # (3)
```

1. client: [B2BIClient](./client.md)
2. paginator: [ListPartnershipsPaginator](./paginators.md#listpartnershipspaginator)
3. item: [:material-code-braces: ListPartnershipsResponseTypeDef](./type_defs.md#listpartnershipsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPartnershipsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    profileId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPartnershipsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPartnershipsResponseTypeDef](./type_defs.md#listpartnershipsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPartnershipsRequestPaginateTypeDef = {  # (1)
    "profileId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPartnershipsRequestPaginateTypeDef](./type_defs.md#listpartnershipsrequestpaginatetypedef) 
## ListProfilesPaginator

Type annotations and code completion for `#!python session.create_client("b2bi").get_paginator("list_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi/paginator/ListProfiles.html#B2BI.Paginator.ListProfiles)

```python
# ListProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_b2bi.paginator import ListProfilesPaginator

session = get_session()
async with session.create_client("b2bi") as client:  # (1)
    paginator: ListProfilesPaginator = client.get_paginator("list_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [B2BIClient](./client.md)
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
## ListTransformersPaginator

Type annotations and code completion for `#!python session.create_client("b2bi").get_paginator("list_transformers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi/paginator/ListTransformers.html#B2BI.Paginator.ListTransformers)

```python
# ListTransformersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_b2bi.paginator import ListTransformersPaginator

session = get_session()
async with session.create_client("b2bi") as client:  # (1)
    paginator: ListTransformersPaginator = client.get_paginator("list_transformers")  # (2)
    async for item in paginator.paginate(...):
        item: ListTransformersResponseTypeDef
        print(item)  # (3)
```

1. client: [B2BIClient](./client.md)
2. paginator: [ListTransformersPaginator](./paginators.md#listtransformerspaginator)
3. item: [:material-code-braces: ListTransformersResponseTypeDef](./type_defs.md#listtransformersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTransformersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTransformersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTransformersResponseTypeDef](./type_defs.md#listtransformersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTransformersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTransformersRequestPaginateTypeDef](./type_defs.md#listtransformersrequestpaginatetypedef) 
