# Paginators

> [Index](../README.md) > [IAMRolesAnywhere](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IAMRolesAnywhere](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#iamrolesanywhere)
    type annotations stubs module [types-aiobotocore-rolesanywhere](https://pypi.org/project/types-aiobotocore-rolesanywhere/).

## ListCrlsPaginator

Type annotations and code completion for `#!python session.create_client("rolesanywhere").get_paginator("list_crls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere/paginator/ListCrls.html#IAMRolesAnywhere.Paginator.ListCrls)

```python
# ListCrlsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rolesanywhere.paginator import ListCrlsPaginator

session = get_session()
async with session.create_client("rolesanywhere") as client:  # (1)
    paginator: ListCrlsPaginator = client.get_paginator("list_crls")  # (2)
    async for item in paginator.paginate(...):
        item: ListCrlsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMRolesAnywhereClient](./client.md)
2. paginator: [ListCrlsPaginator](./paginators.md#listcrlspaginator)
3. item: [:material-code-braces: ListCrlsResponseTypeDef](./type_defs.md#listcrlsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCrlsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    pageSize: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCrlsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCrlsResponseTypeDef](./type_defs.md#listcrlsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRequestPaginateTypeDef = {  # (1)
    "pageSize": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRequestPaginateTypeDef](./type_defs.md#listrequestpaginatetypedef) 
## ListProfilesPaginator

Type annotations and code completion for `#!python session.create_client("rolesanywhere").get_paginator("list_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere/paginator/ListProfiles.html#IAMRolesAnywhere.Paginator.ListProfiles)

```python
# ListProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rolesanywhere.paginator import ListProfilesPaginator

session = get_session()
async with session.create_client("rolesanywhere") as client:  # (1)
    paginator: ListProfilesPaginator = client.get_paginator("list_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMRolesAnywhereClient](./client.md)
2. paginator: [ListProfilesPaginator](./paginators.md#listprofilespaginator)
3. item: [:material-code-braces: ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    pageSize: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRequestPaginateExtraTypeDef = {  # (1)
    "pageSize": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRequestPaginateExtraTypeDef](./type_defs.md#listrequestpaginateextratypedef) 
## ListSubjectsPaginator

Type annotations and code completion for `#!python session.create_client("rolesanywhere").get_paginator("list_subjects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere/paginator/ListSubjects.html#IAMRolesAnywhere.Paginator.ListSubjects)

```python
# ListSubjectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rolesanywhere.paginator import ListSubjectsPaginator

session = get_session()
async with session.create_client("rolesanywhere") as client:  # (1)
    paginator: ListSubjectsPaginator = client.get_paginator("list_subjects")  # (2)
    async for item in paginator.paginate(...):
        item: ListSubjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMRolesAnywhereClient](./client.md)
2. paginator: [ListSubjectsPaginator](./paginators.md#listsubjectspaginator)
3. item: [:material-code-braces: ListSubjectsResponseTypeDef](./type_defs.md#listsubjectsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSubjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    pageSize: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSubjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubjectsResponseTypeDef](./type_defs.md#listsubjectsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRequestPaginateExtraExtraTypeDef = {  # (1)
    "pageSize": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRequestPaginateExtraExtraTypeDef](./type_defs.md#listrequestpaginateextraextratypedef) 
## ListTrustAnchorsPaginator

Type annotations and code completion for `#!python session.create_client("rolesanywhere").get_paginator("list_trust_anchors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere/paginator/ListTrustAnchors.html#IAMRolesAnywhere.Paginator.ListTrustAnchors)

```python
# ListTrustAnchorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rolesanywhere.paginator import ListTrustAnchorsPaginator

session = get_session()
async with session.create_client("rolesanywhere") as client:  # (1)
    paginator: ListTrustAnchorsPaginator = client.get_paginator("list_trust_anchors")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrustAnchorsResponseTypeDef
        print(item)  # (3)
```

1. client: [IAMRolesAnywhereClient](./client.md)
2. paginator: [ListTrustAnchorsPaginator](./paginators.md#listtrustanchorspaginator)
3. item: [:material-code-braces: ListTrustAnchorsResponseTypeDef](./type_defs.md#listtrustanchorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTrustAnchorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    pageSize: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTrustAnchorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrustAnchorsResponseTypeDef](./type_defs.md#listtrustanchorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRequestPaginateExtraExtraExtraTypeDef = {  # (1)
    "pageSize": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRequestPaginateExtraExtraExtraTypeDef](./type_defs.md#listrequestpaginateextraextraextratypedef) 
