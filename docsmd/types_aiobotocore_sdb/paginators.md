# Paginators

> [Index](../README.md) > [SimpleDB](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SimpleDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#simpledb)
    type annotations stubs module [types-aiobotocore-sdb](https://pypi.org/project/types-aiobotocore-sdb/).

## ListDomainsPaginator

Type annotations and code completion for `#!python session.create_client("sdb").get_paginator("list_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/paginator/ListDomains.html#SimpleDB.Paginator.ListDomains)

```python
# ListDomainsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sdb.paginator import ListDomainsPaginator

session = get_session()
async with session.create_client("sdb") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainsResultTypeDef
        print(item)  # (3)
```

1. client: [SimpleDBClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDomainsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainsRequestPaginateTypeDef](./type_defs.md#listdomainsrequestpaginatetypedef) 
## SelectPaginator

Type annotations and code completion for `#!python session.create_client("sdb").get_paginator("select")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/paginator/Select.html#SimpleDB.Paginator.Select)

```python
# SelectPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sdb.paginator import SelectPaginator

session = get_session()
async with session.create_client("sdb") as client:  # (1)
    paginator: SelectPaginator = client.get_paginator("select")  # (2)
    async for item in paginator.paginate(...):
        item: SelectResultTypeDef
        print(item)  # (3)
```

1. client: [SimpleDBClient](./client.md)
2. paginator: [SelectPaginator](./paginators.md#selectpaginator)
3. item: [:material-code-braces: SelectResultTypeDef](./type_defs.md#selectresulttypedef) 


### paginate

Type annotations and code completion for `#!python SelectPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SelectExpression: str,
    ConsistentRead: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[SelectResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SelectResultTypeDef](./type_defs.md#selectresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SelectRequestPaginateTypeDef = {  # (1)
    "SelectExpression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SelectRequestPaginateTypeDef](./type_defs.md#selectrequestpaginatetypedef) 
