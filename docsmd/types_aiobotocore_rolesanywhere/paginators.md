# Paginators

> [Index](../README.md) > [IAMRolesAnywhere](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IAMRolesAnywhere](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere)
    type annotations stubs module [types-aiobotocore-rolesanywhere](https://pypi.org/project/types-aiobotocore-rolesanywhere/).

## ListCrlsPaginator

Type annotations and code completion for `#!python session.create_client("rolesanywhere").get_paginator("list_crls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListCrls)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    pageSize: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCrlsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCrlsResponseTypeDef](./type_defs.md#listcrlsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRequestListCrlsPaginateTypeDef = {  # (1)
    "pageSize": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRequestListCrlsPaginateTypeDef](./type_defs.md#listrequestlistcrlspaginatetypedef) 
## ListProfilesPaginator

Type annotations and code completion for `#!python session.create_client("rolesanywhere").get_paginator("list_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListProfiles)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    pageSize: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProfilesResponseTypeDef](./type_defs.md#listprofilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRequestListProfilesPaginateTypeDef = {  # (1)
    "pageSize": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRequestListProfilesPaginateTypeDef](./type_defs.md#listrequestlistprofilespaginatetypedef) 
## ListSubjectsPaginator

Type annotations and code completion for `#!python session.create_client("rolesanywhere").get_paginator("list_subjects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListSubjects)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    pageSize: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSubjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSubjectsResponseTypeDef](./type_defs.md#listsubjectsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRequestListSubjectsPaginateTypeDef = {  # (1)
    "pageSize": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRequestListSubjectsPaginateTypeDef](./type_defs.md#listrequestlistsubjectspaginatetypedef) 
## ListTrustAnchorsPaginator

Type annotations and code completion for `#!python session.create_client("rolesanywhere").get_paginator("list_trust_anchors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere.Paginator.ListTrustAnchors)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    pageSize: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTrustAnchorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTrustAnchorsResponseTypeDef](./type_defs.md#listtrustanchorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRequestListTrustAnchorsPaginateTypeDef = {  # (1)
    "pageSize": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRequestListTrustAnchorsPaginateTypeDef](./type_defs.md#listrequestlisttrustanchorspaginatetypedef) 
