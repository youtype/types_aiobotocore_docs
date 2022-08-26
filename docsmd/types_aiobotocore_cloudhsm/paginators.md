# Paginators

> [Index](../README.md) > [CloudHSM](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudHSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
    type annotations stubs module [types-aiobotocore-cloudhsm](https://pypi.org/project/types-aiobotocore-cloudhsm/).

## ListHapgsPaginator

Type annotations and code completion for `#!python session.create_client("cloudhsm").get_paginator("list_hapgs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListHapgsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHapgsResponseTypeDef](./type_defs.md#listhapgsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHapgsRequestListHapgsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHapgsRequestListHapgsPaginateTypeDef](./type_defs.md#listhapgsrequestlisthapgspaginatetypedef) 
## ListHsmsPaginator

Type annotations and code completion for `#!python session.create_client("cloudhsm").get_paginator("list_hsms")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListHsmsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHsmsResponseTypeDef](./type_defs.md#listhsmsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHsmsRequestListHsmsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHsmsRequestListHsmsPaginateTypeDef](./type_defs.md#listhsmsrequestlisthsmspaginatetypedef) 
## ListLunaClientsPaginator

Type annotations and code completion for `#!python session.create_client("cloudhsm").get_paginator("list_luna_clients")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLunaClientsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLunaClientsResponseTypeDef](./type_defs.md#listlunaclientsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListLunaClientsRequestListLunaClientsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLunaClientsRequestListLunaClientsPaginateTypeDef](./type_defs.md#listlunaclientsrequestlistlunaclientspaginatetypedef) 
