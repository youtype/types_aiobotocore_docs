# Paginators

> [Index](../README.md) > [KMS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [KMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
    type annotations stubs module [types-aiobotocore-kms](https://pypi.org/project/types-aiobotocore-kms/).

## ListAliasesPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListAliasesPaginator

session = get_session()
async with session.create_client("kms") as client:
    client: KMSClient
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
```


### paginate

Type annotations and code completion for `#!python ListAliasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    KeyId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAliasesRequestListAliasesPaginateTypeDef = {  # (1)
    "KeyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAliasesRequestListAliasesPaginateTypeDef](./type_defs.md#listaliasesrequestlistaliasespaginatetypedef) 
## ListGrantsPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListGrantsPaginator

session = get_session()
async with session.create_client("kms") as client:
    client: KMSClient
    paginator: ListGrantsPaginator = client.get_paginator("list_grants")
```


### paginate

Type annotations and code completion for `#!python ListGrantsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    KeyId: str,
    GrantId: str = ...,
    GranteePrincipal: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGrantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGrantsResponseTypeDef](./type_defs.md#listgrantsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGrantsRequestListGrantsPaginateTypeDef = {  # (1)
    "KeyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGrantsRequestListGrantsPaginateTypeDef](./type_defs.md#listgrantsrequestlistgrantspaginatetypedef) 
## ListKeyPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_key_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListKeyPoliciesPaginator

session = get_session()
async with session.create_client("kms") as client:
    client: KMSClient
    paginator: ListKeyPoliciesPaginator = client.get_paginator("list_key_policies")
```


### paginate

Type annotations and code completion for `#!python ListKeyPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    KeyId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListKeyPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKeyPoliciesResponseTypeDef](./type_defs.md#listkeypoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = {  # (1)
    "KeyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef](./type_defs.md#listkeypoliciesrequestlistkeypoliciespaginatetypedef) 
## ListKeysPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListKeysPaginator

session = get_session()
async with session.create_client("kms") as client:
    client: KMSClient
    paginator: ListKeysPaginator = client.get_paginator("list_keys")
```


### paginate

Type annotations and code completion for `#!python ListKeysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListKeysRequestListKeysPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeysRequestListKeysPaginateTypeDef](./type_defs.md#listkeysrequestlistkeyspaginatetypedef) 
