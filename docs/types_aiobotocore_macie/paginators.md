<a id="paginators-for-aiobotocore-macie-module"></a>

# Paginators for aiobotocore Macie module

> [Index](../README.md) > [Macie](./README.md) > Paginators

Auto-generated documentation for
[Macie](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
type annotations stubs module
[types-aiobotocore-macie](https://pypi.org/project/types-aiobotocore-macie/).

- [Paginators for aiobotocore Macie module](#paginators-for-aiobotocore-macie-module)
  - [ListMemberAccountsPaginator](#listmemberaccountspaginator)
  - [ListS3ResourcesPaginator](#lists3resourcespaginator)

<a id="listmemberaccountspaginator"></a>

## ListMemberAccountsPaginator

Type annotations for
`session.create_client("macie").get_paginator("list_member_accounts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_macie.paginator import ListMemberAccountsPaginator

session = get_session()
async with session.create_client("macie") as client:
    client: MacieClient
    paginator: ListMemberAccountsPaginator = client.get_paginator("list_member_accounts")
```

Boto3 documentation:
[Macie.Paginator.ListMemberAccounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts)

Arguments for `ListMemberAccountsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMemberAccountsPaginator.paginate` returns
`AsyncIterator`\[[ListMemberAccountsResultTypeDef](./type_defs.md#listmemberaccountsresulttypedef)\].

<a id="lists3resourcespaginator"></a>

## ListS3ResourcesPaginator

Type annotations for
`session.create_client("macie").get_paginator("list_s3_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_macie.paginator import ListS3ResourcesPaginator

session = get_session()
async with session.create_client("macie") as client:
    client: MacieClient
    paginator: ListS3ResourcesPaginator = client.get_paginator("list_s3_resources")
```

Boto3 documentation:
[Macie.Paginator.ListS3Resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources)

Arguments for `ListS3ResourcesPaginator.paginate` method:

- `memberAccountId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListS3ResourcesPaginator.paginate` returns
`AsyncIterator`\[[ListS3ResourcesResultTypeDef](./type_defs.md#lists3resourcesresulttypedef)\].
