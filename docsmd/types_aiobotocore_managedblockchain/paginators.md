# Paginators

> [Index](../README.md) > [ManagedBlockchain](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ManagedBlockchain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#managedblockchain)
    type annotations stubs module [types-aiobotocore-managedblockchain](https://pypi.org/project/types-aiobotocore-managedblockchain/).

## ListAccessorsPaginator

Type annotations and code completion for `#!python session.create_client("managedblockchain").get_paginator("list_accessors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain/paginator/ListAccessors.html#ManagedBlockchain.Paginator.ListAccessors)

```python
# ListAccessorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_managedblockchain.paginator import ListAccessorsPaginator

session = get_session()
async with session.create_client("managedblockchain") as client:  # (1)
    paginator: ListAccessorsPaginator = client.get_paginator("list_accessors")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessorsOutputTypeDef
        print(item)  # (3)
```

1. client: [ManagedBlockchainClient](./client.md)
2. paginator: [ListAccessorsPaginator](./paginators.md#listaccessorspaginator)
3. item: [:material-code-braces: ListAccessorsOutputTypeDef](./type_defs.md#listaccessorsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListAccessorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    NetworkType: AccessorNetworkTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAccessorsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AccessorNetworkTypeType](./literals.md#accessornetworktypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAccessorsOutputTypeDef](./type_defs.md#listaccessorsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessorsInputPaginateTypeDef = {  # (1)
    "NetworkType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessorsInputPaginateTypeDef](./type_defs.md#listaccessorsinputpaginatetypedef) 
