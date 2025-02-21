# Paginators

> [Index](../README.md) > [PaymentCryptographyControlPlane](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PaymentCryptographyControlPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#paymentcryptographycontrolplane)
    type annotations stubs module [types-aiobotocore-payment-cryptography](https://pypi.org/project/types-aiobotocore-payment-cryptography/).

## ListAliasesPaginator

Type annotations and code completion for `#!python session.create_client("payment-cryptography").get_paginator("list_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/paginator/ListAliases.html#PaymentCryptographyControlPlane.Paginator.ListAliases)

```python
# ListAliasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_payment_cryptography.paginator import ListAliasesPaginator

session = get_session()
async with session.create_client("payment-cryptography") as client:  # (1)
    paginator: ListAliasesPaginator = client.get_paginator("list_aliases")  # (2)
    async for item in paginator.paginate(...):
        item: ListAliasesOutputTypeDef
        print(item)  # (3)
```

1. client: [PaymentCryptographyControlPlaneClient](./client.md)
2. paginator: [ListAliasesPaginator](./paginators.md#listaliasespaginator)
3. item: [:material-code-braces: ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListAliasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    KeyArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAliasesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAliasesOutputTypeDef](./type_defs.md#listaliasesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAliasesInputPaginateTypeDef = {  # (1)
    "KeyArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAliasesInputPaginateTypeDef](./type_defs.md#listaliasesinputpaginatetypedef) 
## ListKeysPaginator

Type annotations and code completion for `#!python session.create_client("payment-cryptography").get_paginator("list_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/paginator/ListKeys.html#PaymentCryptographyControlPlane.Paginator.ListKeys)

```python
# ListKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_payment_cryptography.paginator import ListKeysPaginator

session = get_session()
async with session.create_client("payment-cryptography") as client:  # (1)
    paginator: ListKeysPaginator = client.get_paginator("list_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListKeysOutputTypeDef
        print(item)  # (3)
```

1. client: [PaymentCryptographyControlPlaneClient](./client.md)
2. paginator: [ListKeysPaginator](./paginators.md#listkeyspaginator)
3. item: [:material-code-braces: ListKeysOutputTypeDef](./type_defs.md#listkeysoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    KeyState: KeyStateType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListKeysOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: KeyStateType](./literals.md#keystatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListKeysOutputTypeDef](./type_defs.md#listkeysoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKeysInputPaginateTypeDef = {  # (1)
    "KeyState": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeysInputPaginateTypeDef](./type_defs.md#listkeysinputpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("payment-cryptography").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography/paginator/ListTagsForResource.html#PaymentCryptographyControlPlane.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_payment_cryptography.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("payment-cryptography") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceOutputTypeDef
        print(item)  # (3)
```

1. client: [PaymentCryptographyControlPlaneClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsForResourceOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceInputPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputPaginateTypeDef](./type_defs.md#listtagsforresourceinputpaginatetypedef) 
