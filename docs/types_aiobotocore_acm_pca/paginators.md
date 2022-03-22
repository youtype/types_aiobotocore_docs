<a id="paginators-for-aiobotocore-acmpca-module"></a>

# Paginators for aiobotocore ACMPCA module

> [Index](../README.md) > [ACMPCA](./README.md) > Paginators

Auto-generated documentation for
[ACMPCA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
type annotations stubs module
[types-aiobotocore-acm-pca](https://pypi.org/project/types-aiobotocore-acm-pca/).

- [Paginators for aiobotocore ACMPCA module](#paginators-for-aiobotocore-acmpca-module)
  - [ListCertificateAuthoritiesPaginator](#listcertificateauthoritiespaginator)
  - [ListPermissionsPaginator](#listpermissionspaginator)
  - [ListTagsPaginator](#listtagspaginator)

<a id="listcertificateauthoritiespaginator"></a>

## ListCertificateAuthoritiesPaginator

Type annotations for
`session.create_client("acm-pca").get_paginator("list_certificate_authorities")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_acm_pca.paginator import ListCertificateAuthoritiesPaginator

session = get_session()
async with session.create_client("acm-pca") as client:
    client: ACMPCAClient
    paginator: ListCertificateAuthoritiesPaginator = client.get_paginator("list_certificate_authorities")
```

Boto3 documentation:
[ACMPCA.Paginator.ListCertificateAuthorities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListCertificateAuthorities)

Arguments for `ListCertificateAuthoritiesPaginator.paginate` method:

- `ResourceOwner`: [ResourceOwnerType](./literals.md#resourceownertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCertificateAuthoritiesPaginator.paginate` returns
`AsyncIterator`\[[ListCertificateAuthoritiesResponseTypeDef](./type_defs.md#listcertificateauthoritiesresponsetypedef)\].

<a id="listpermissionspaginator"></a>

## ListPermissionsPaginator

Type annotations for
`session.create_client("acm-pca").get_paginator("list_permissions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_acm_pca.paginator import ListPermissionsPaginator

session = get_session()
async with session.create_client("acm-pca") as client:
    client: ACMPCAClient
    paginator: ListPermissionsPaginator = client.get_paginator("list_permissions")
```

Boto3 documentation:
[ACMPCA.Paginator.ListPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListPermissions)

Arguments for `ListPermissionsPaginator.paginate` method:

- `CertificateAuthorityArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPermissionsPaginator.paginate` returns
`AsyncIterator`\[[ListPermissionsResponseTypeDef](./type_defs.md#listpermissionsresponsetypedef)\].

<a id="listtagspaginator"></a>

## ListTagsPaginator

Type annotations for
`session.create_client("acm-pca").get_paginator("list_tags")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_acm_pca.paginator import ListTagsPaginator

session = get_session()
async with session.create_client("acm-pca") as client:
    client: ACMPCAClient
    paginator: ListTagsPaginator = client.get_paginator("list_tags")
```

Boto3 documentation:
[ACMPCA.Paginator.ListTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListTags)

Arguments for `ListTagsPaginator.paginate` method:

- `CertificateAuthorityArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsPaginator.paginate` returns
`AsyncIterator`\[[ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)\].
