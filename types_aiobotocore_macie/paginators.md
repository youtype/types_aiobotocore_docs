<a id="paginators-for-aiobotocore-macie-module"></a>

# Paginators for aiobotocore Macie module

> [Index](..) > [Macie](.) > Paginators

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
`aiobotocore.create_client("macie").get_paginator("list_member_accounts")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_macie.paginator import ListMemberAccountsPaginator

def get_list_member_accounts_paginator() -> ListMemberAccountsPaginator:
    return Session().create_client("macie").get_paginator("list_member_accounts")
```

Boto3 documentation:
[Macie.Paginator.ListMemberAccounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts)

Arguments for `ListMemberAccountsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMemberAccountsPaginator.paginate` returns
`_PageIterator`\[[ListMemberAccountsResultTypeDef](./type_defs.md#listmemberaccountsresulttypedef)\].

<a id="lists3resourcespaginator"></a>

## ListS3ResourcesPaginator

Type annotations for
`aiobotocore.create_client("macie").get_paginator("list_s3_resources")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_macie.paginator import ListS3ResourcesPaginator

def get_list_s3_resources_paginator() -> ListS3ResourcesPaginator:
    return Session().create_client("macie").get_paginator("list_s3_resources")
```

Boto3 documentation:
[Macie.Paginator.ListS3Resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources)

Arguments for `ListS3ResourcesPaginator.paginate` method:

- `memberAccountId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListS3ResourcesPaginator.paginate` returns
`_PageIterator`\[[ListS3ResourcesResultTypeDef](./type_defs.md#lists3resourcesresulttypedef)\].
