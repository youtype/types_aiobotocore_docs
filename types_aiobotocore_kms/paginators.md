<a id="paginators-for-aiobotocore-kms-module"></a>

# Paginators for aiobotocore KMS module

> [Index](..) > [KMS](.) > Paginators

Auto-generated documentation for
[KMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
type annotations stubs module
[types-aiobotocore-kms](https://pypi.org/project/types-aiobotocore-kms/).

- [Paginators for aiobotocore KMS module](#paginators-for-aiobotocore-kms-module)
  - [ListAliasesPaginator](#listaliasespaginator)
  - [ListGrantsPaginator](#listgrantspaginator)
  - [ListKeyPoliciesPaginator](#listkeypoliciespaginator)
  - [ListKeysPaginator](#listkeyspaginator)

<a id="listaliasespaginator"></a>

## ListAliasesPaginator

Type annotations for
`session.create_client("kms").get_paginator("list_aliases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListAliasesPaginator

session = get_session()
async with session.create_client("kms") as client:
    client: KMSClient
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
```

Boto3 documentation:
[KMS.Paginator.ListAliases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases)

Arguments for `ListAliasesPaginator.paginate` method:

- `KeyId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAliasesPaginator.paginate` returns
`_PageIterator`\[[ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef)\].

<a id="listgrantspaginator"></a>

## ListGrantsPaginator

Type annotations for
`session.create_client("kms").get_paginator("list_grants")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListGrantsPaginator

session = get_session()
async with session.create_client("kms") as client:
    client: KMSClient
    paginator: ListGrantsPaginator = client.get_paginator("list_grants")
```

Boto3 documentation:
[KMS.Paginator.ListGrants](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants)

Arguments for `ListGrantsPaginator.paginate` method:

- `KeyId`: `str` *(required)*
- `GrantId`: `str`
- `GranteePrincipal`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGrantsPaginator.paginate` returns
`_PageIterator`\[[ListGrantsResponseTypeDef](./type_defs.md#listgrantsresponsetypedef)\].

<a id="listkeypoliciespaginator"></a>

## ListKeyPoliciesPaginator

Type annotations for
`session.create_client("kms").get_paginator("list_key_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListKeyPoliciesPaginator

session = get_session()
async with session.create_client("kms") as client:
    client: KMSClient
    paginator: ListKeyPoliciesPaginator = client.get_paginator("list_key_policies")
```

Boto3 documentation:
[KMS.Paginator.ListKeyPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies)

Arguments for `ListKeyPoliciesPaginator.paginate` method:

- `KeyId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListKeyPoliciesPaginator.paginate` returns
`_PageIterator`\[[ListKeyPoliciesResponseTypeDef](./type_defs.md#listkeypoliciesresponsetypedef)\].

<a id="listkeyspaginator"></a>

## ListKeysPaginator

Type annotations for `session.create_client("kms").get_paginator("list_keys")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListKeysPaginator

session = get_session()
async with session.create_client("kms") as client:
    client: KMSClient
    paginator: ListKeysPaginator = client.get_paginator("list_keys")
```

Boto3 documentation:
[KMS.Paginator.ListKeys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys)

Arguments for `ListKeysPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListKeysPaginator.paginate` returns
`_PageIterator`\[[ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef)\].
