# Paginators

> [Index](../README.md) > [Macie](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Macie](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
    type annotations stubs module [types-aiobotocore-macie](https://pypi.org/project/types-aiobotocore-macie/).

## ListMemberAccountsPaginator

Type annotations and code completion for `#!python session.create_client("macie").get_paginator("list_member_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_macie.paginator import ListMemberAccountsPaginator

session = get_session()
async with session.create_client("macie") as client:
    client: MacieClient
    paginator: ListMemberAccountsPaginator = client.get_paginator("list_member_accounts")
```


### paginate

Type annotations and code completion for `#!python ListMemberAccountsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMemberAccountsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMemberAccountsResultTypeDef](./type_defs.md#listmemberaccountsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMemberAccountsRequestListMemberAccountsPaginateTypeDef](./type_defs.md#listmemberaccountsrequestlistmemberaccountspaginatetypedef) 
## ListS3ResourcesPaginator

Type annotations and code completion for `#!python session.create_client("macie").get_paginator("list_s3_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_macie.paginator import ListS3ResourcesPaginator

session = get_session()
async with session.create_client("macie") as client:
    client: MacieClient
    paginator: ListS3ResourcesPaginator = client.get_paginator("list_s3_resources")
```


### paginate

Type annotations and code completion for `#!python ListS3ResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    memberAccountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListS3ResourcesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListS3ResourcesResultTypeDef](./type_defs.md#lists3resourcesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = {  # (1)
    "memberAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListS3ResourcesRequestListS3ResourcesPaginateTypeDef](./type_defs.md#lists3resourcesrequestlists3resourcespaginatetypedef) 
