# Paginators

> [Index](../README.md) > [KMS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [KMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#kms)
    type annotations stubs module [types-aiobotocore-kms](https://pypi.org/project/types-aiobotocore-kms/).

## DescribeCustomKeyStoresPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("describe_custom_key_stores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms/paginator/DescribeCustomKeyStores.html#KMS.Paginator.DescribeCustomKeyStores)

```python
# DescribeCustomKeyStoresPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    CustomKeyStoreId: str = ...,
    CustomKeyStoreName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeCustomKeyStoresResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeCustomKeyStoresResponseTypeDef](./type_defs.md#describecustomkeystoresresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCustomKeyStoresRequestPaginateTypeDef = {  # (1)
    "CustomKeyStoreId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCustomKeyStoresRequestPaginateTypeDef](./type_defs.md#describecustomkeystoresrequestpaginatetypedef) 
## ListAliasesPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms/paginator/ListAliases.html#KMS.Paginator.ListAliases)

```python
# ListAliasesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    KeyId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAliasesRequestPaginateTypeDef = {  # (1)
    "KeyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAliasesRequestPaginateTypeDef](./type_defs.md#listaliasesrequestpaginatetypedef) 
## ListGrantsPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms/paginator/ListGrants.html#KMS.Paginator.ListGrants)

```python
# ListGrantsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    KeyId: str,
    GrantId: str = ...,
    GranteePrincipal: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGrantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGrantsResponseTypeDef](./type_defs.md#listgrantsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGrantsRequestPaginateTypeDef = {  # (1)
    "KeyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGrantsRequestPaginateTypeDef](./type_defs.md#listgrantsrequestpaginatetypedef) 
## ListKeyPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_key_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms/paginator/ListKeyPolicies.html#KMS.Paginator.ListKeyPolicies)

```python
# ListKeyPoliciesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    KeyId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListKeyPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKeyPoliciesResponseTypeDef](./type_defs.md#listkeypoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKeyPoliciesRequestPaginateTypeDef = {  # (1)
    "KeyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeyPoliciesRequestPaginateTypeDef](./type_defs.md#listkeypoliciesrequestpaginatetypedef) 
## ListKeyRotationsPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_key_rotations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms/paginator/ListKeyRotations.html#KMS.Paginator.ListKeyRotations)

```python
# ListKeyRotationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_kms.paginator import ListKeyRotationsPaginator

session = get_session()
async with session.create_client("kms") as client:  # (1)
    paginator: ListKeyRotationsPaginator = client.get_paginator("list_key_rotations")  # (2)
    async for item in paginator.paginate(...):
        item: ListKeyRotationsResponseTypeDef
        print(item)  # (3)
```

1. client: [KMSClient](./client.md)
2. paginator: [ListKeyRotationsPaginator](./paginators.md#listkeyrotationspaginator)
3. item: [:material-code-braces: ListKeyRotationsResponseTypeDef](./type_defs.md#listkeyrotationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListKeyRotationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    KeyId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListKeyRotationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKeyRotationsResponseTypeDef](./type_defs.md#listkeyrotationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKeyRotationsRequestPaginateTypeDef = {  # (1)
    "KeyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeyRotationsRequestPaginateTypeDef](./type_defs.md#listkeyrotationsrequestpaginatetypedef) 
## ListKeysPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms/paginator/ListKeys.html#KMS.Paginator.ListKeys)

```python
# ListKeysPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKeysRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeysRequestPaginateTypeDef](./type_defs.md#listkeysrequestpaginatetypedef) 
## ListResourceTagsPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_resource_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms/paginator/ListResourceTags.html#KMS.Paginator.ListResourceTags)

```python
# ListResourceTagsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    KeyId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResourceTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceTagsResponseTypeDef](./type_defs.md#listresourcetagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceTagsRequestPaginateTypeDef = {  # (1)
    "KeyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceTagsRequestPaginateTypeDef](./type_defs.md#listresourcetagsrequestpaginatetypedef) 
## ListRetirableGrantsPaginator

Type annotations and code completion for `#!python session.create_client("kms").get_paginator("list_retirable_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms/paginator/ListRetirableGrants.html#KMS.Paginator.ListRetirableGrants)

```python
# ListRetirableGrantsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    RetiringPrincipal: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGrantsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGrantsResponseTypeDef](./type_defs.md#listgrantsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRetirableGrantsRequestPaginateTypeDef = {  # (1)
    "RetiringPrincipal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRetirableGrantsRequestPaginateTypeDef](./type_defs.md#listretirablegrantsrequestpaginatetypedef) 
