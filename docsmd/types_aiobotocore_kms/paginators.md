# Paginators

> [Index](../README.md) > [KMS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [KMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
    type annotations stubs module [types-aiobotocore-kms](https://pypi.org/project/types-aiobotocore-kms/).

## DescribeCustomKeyStoresPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("describe_custom_key_stores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import DescribeCustomKeyStoresPaginator

session = get_session()
async with session.create_client("kms") as client:  # (1)
    paginator: DescribeCustomKeyStoresPaginator = client.get_paginator("describe_custom_key_stores")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCustomKeyStoresResponseTypeDef
        print(item)  # (3)
```

1. client: [KMSClient](./client.md)
2. paginator: [DescribeCustomKeyStoresPaginator](./paginators.md#describecustomkeystorespaginator)
3. item: [:material-code-braces: DescribeCustomKeyStoresResponseTypeDef](./type_defs.md#describecustomkeystoresresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCustomKeyStoresPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CustomKeyStoreId: str = ...,
    CustomKeyStoreName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeCustomKeyStoresResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeCustomKeyStoresResponseTypeDef](./type_defs.md#describecustomkeystoresresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef = {  # (1)
    "CustomKeyStoreId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef](./type_defs.md#describecustomkeystoresrequestdescribecustomkeystorespaginatetypedef) 
## ListAliasesPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListAliasesPaginator

session = get_session()
async with session.create_client("kms") as client:  # (1)
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAliasesResponseTypeDef
        print(item)  # (3)
```

1. client: [KMSClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


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
async with session.create_client("kms") as client:  # (1)
    paginator: ListGrantsPaginator = client.get_paginator("list_grants")  # (2)
    async for item in paginator.paginate(...):
        item: ListGrantsResponseTypeDef
        print(item)  # (3)
```

1. client: [KMSClient](./client.md)
2. paginator: [ListGrantsPaginator](./paginators.md#listgrantspaginator)
3. item: [:material-code-braces: ListGrantsResponseTypeDef](./type_defs.md#listgrantsresponsetypedef) 


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
async with session.create_client("kms") as client:  # (1)
    paginator: ListKeyPoliciesPaginator = client.get_paginator("list_key_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListKeyPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [KMSClient](./client.md)
2. paginator: [ListKeyPoliciesPaginator](./paginators.md#listkeypoliciespaginator)
3. item: [:material-code-braces: ListKeyPoliciesResponseTypeDef](./type_defs.md#listkeypoliciesresponsetypedef) 


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
async with session.create_client("kms") as client:  # (1)
    paginator: ListKeysPaginator = client.get_paginator("list_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [KMSClient](./client.md)
2. paginator: [ListKeysPaginator](./paginators.md#listkeyspaginator)
3. item: [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


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
## ListResourceTagsPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_resource_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListResourceTagsPaginator

session = get_session()
async with session.create_client("kms") as client:  # (1)
    paginator: ListResourceTagsPaginator = client.get_paginator("list_resource_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [KMSClient](./client.md)
2. paginator: [ListResourceTagsPaginator](./paginators.md#listresourcetagspaginator)
3. item: [:material-code-braces: ListResourceTagsResponseTypeDef](./type_defs.md#listresourcetagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    KeyId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourceTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceTagsResponseTypeDef](./type_defs.md#listresourcetagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListResourceTagsRequestListResourceTagsPaginateTypeDef = {  # (1)
    "KeyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceTagsRequestListResourceTagsPaginateTypeDef](./type_defs.md#listresourcetagsrequestlistresourcetagspaginatetypedef) 
## ListRetirableGrantsPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_retirable_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListRetirableGrantsPaginator

session = get_session()
async with session.create_client("kms") as client:  # (1)
    paginator: ListRetirableGrantsPaginator = client.get_paginator("list_retirable_grants")  # (2)
    async for item in paginator.paginate(...):
        item: ListGrantsResponseTypeDef
        print(item)  # (3)
```

1. client: [KMSClient](./client.md)
2. paginator: [ListRetirableGrantsPaginator](./paginators.md#listretirablegrantspaginator)
3. item: [:material-code-braces: ListGrantsResponseTypeDef](./type_defs.md#listgrantsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRetirableGrantsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RetiringPrincipal: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGrantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGrantsResponseTypeDef](./type_defs.md#listgrantsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef = {  # (1)
    "RetiringPrincipal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef](./type_defs.md#listretirablegrantsrequestlistretirablegrantspaginatetypedef) 
