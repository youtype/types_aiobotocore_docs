# Paginators

> [Index](../README.md) > [ACMPCA](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ACMPCA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#acmpca)
    type annotations stubs module [types-aiobotocore-acm-pca](https://pypi.org/project/types-aiobotocore-acm-pca/).

## ListCertificateAuthoritiesPaginator

Type annotations and code completion for `#!python session.create_client("acm-pca").get_paginator("list_certificate_authorities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca/paginator/ListCertificateAuthorities.html#ACMPCA.Paginator.ListCertificateAuthorities)

```python
# ListCertificateAuthoritiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_acm_pca.paginator import ListCertificateAuthoritiesPaginator

session = get_session()
async with session.create_client("acm-pca") as client:  # (1)
    paginator: ListCertificateAuthoritiesPaginator = client.get_paginator("list_certificate_authorities")  # (2)
    async for item in paginator.paginate(...):
        item: ListCertificateAuthoritiesResponseTypeDef
        print(item)  # (3)
```

1. client: [ACMPCAClient](./client.md)
2. paginator: [ListCertificateAuthoritiesPaginator](./paginators.md#listcertificateauthoritiespaginator)
3. item: [:material-code-braces: ListCertificateAuthoritiesResponseTypeDef](./type_defs.md#listcertificateauthoritiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCertificateAuthoritiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceOwner: ResourceOwnerType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListCertificateAuthoritiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCertificateAuthoritiesResponseTypeDef](./type_defs.md#listcertificateauthoritiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCertificateAuthoritiesRequestPaginateTypeDef = {  # (1)
    "ResourceOwner": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCertificateAuthoritiesRequestPaginateTypeDef](./type_defs.md#listcertificateauthoritiesrequestpaginatetypedef) 
## ListPermissionsPaginator

Type annotations and code completion for `#!python session.create_client("acm-pca").get_paginator("list_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca/paginator/ListPermissions.html#ACMPCA.Paginator.ListPermissions)

```python
# ListPermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_acm_pca.paginator import ListPermissionsPaginator

session = get_session()
async with session.create_client("acm-pca") as client:  # (1)
    paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ACMPCAClient](./client.md)
2. paginator: [ListPermissionsPaginator](./paginators.md#listpermissionspaginator)
3. item: [:material-code-braces: ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CertificateAuthorityArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPermissionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPermissionsRequestPaginateTypeDef = {  # (1)
    "CertificateAuthorityArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionsRequestPaginateTypeDef](./type_defs.md#listpermissionsrequestpaginatetypedef) 
## ListTagsPaginator

Type annotations and code completion for `#!python session.create_client("acm-pca").get_paginator("list_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca/paginator/ListTags.html#ACMPCA.Paginator.ListTags)

```python
# ListTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_acm_pca.paginator import ListTagsPaginator

session = get_session()
async with session.create_client("acm-pca") as client:  # (1)
    paginator: ListTagsPaginator = client.get_paginator("list_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [ACMPCAClient](./client.md)
2. paginator: [ListTagsPaginator](./paginators.md#listtagspaginator)
3. item: [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CertificateAuthorityArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsRequestPaginateTypeDef = {  # (1)
    "CertificateAuthorityArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestPaginateTypeDef](./type_defs.md#listtagsrequestpaginatetypedef) 
