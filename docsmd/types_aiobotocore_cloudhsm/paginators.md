# Paginators

> [Index](../README.md) > [CloudHSM](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudHSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#cloudhsm)
    type annotations stubs module [types-aiobotocore-cloudhsm](https://pypi.org/project/types-aiobotocore-cloudhsm/).

## ListHapgsPaginator

Type annotations and code completion for `#!python session.create_client("cloudhsm").get_paginator("list_hapgs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm/paginator/ListHapgs.html#CloudHSM.Paginator.ListHapgs)

```python
# ListHapgsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudhsm.paginator import ListHapgsPaginator

session = get_session()
async with session.create_client("cloudhsm") as client:  # (1)
    paginator: ListHapgsPaginator = client.get_paginator("list_hapgs")  # (2)
    async for item in paginator.paginate(...):
        item: ListHapgsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudHSMClient](./client.md)
2. paginator: [ListHapgsPaginator](./paginators.md#listhapgspaginator)
3. item: [:material-code-braces: ListHapgsResponseTypeDef](./type_defs.md#listhapgsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHapgsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListHapgsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHapgsResponseTypeDef](./type_defs.md#listhapgsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHapgsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHapgsRequestPaginateTypeDef](./type_defs.md#listhapgsrequestpaginatetypedef) 
## ListHsmsPaginator

Type annotations and code completion for `#!python session.create_client("cloudhsm").get_paginator("list_hsms")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm/paginator/ListHsms.html#CloudHSM.Paginator.ListHsms)

```python
# ListHsmsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudhsm.paginator import ListHsmsPaginator

session = get_session()
async with session.create_client("cloudhsm") as client:  # (1)
    paginator: ListHsmsPaginator = client.get_paginator("list_hsms")  # (2)
    async for item in paginator.paginate(...):
        item: ListHsmsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudHSMClient](./client.md)
2. paginator: [ListHsmsPaginator](./paginators.md#listhsmspaginator)
3. item: [:material-code-braces: ListHsmsResponseTypeDef](./type_defs.md#listhsmsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHsmsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListHsmsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHsmsResponseTypeDef](./type_defs.md#listhsmsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHsmsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHsmsRequestPaginateTypeDef](./type_defs.md#listhsmsrequestpaginatetypedef) 
## ListLunaClientsPaginator

Type annotations and code completion for `#!python session.create_client("cloudhsm").get_paginator("list_luna_clients")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm/paginator/ListLunaClients.html#CloudHSM.Paginator.ListLunaClients)

```python
# ListLunaClientsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudhsm.paginator import ListLunaClientsPaginator

session = get_session()
async with session.create_client("cloudhsm") as client:  # (1)
    paginator: ListLunaClientsPaginator = client.get_paginator("list_luna_clients")  # (2)
    async for item in paginator.paginate(...):
        item: ListLunaClientsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudHSMClient](./client.md)
2. paginator: [ListLunaClientsPaginator](./paginators.md#listlunaclientspaginator)
3. item: [:material-code-braces: ListLunaClientsResponseTypeDef](./type_defs.md#listlunaclientsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLunaClientsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListLunaClientsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLunaClientsResponseTypeDef](./type_defs.md#listlunaclientsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLunaClientsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLunaClientsRequestPaginateTypeDef](./type_defs.md#listlunaclientsrequestpaginatetypedef) 
