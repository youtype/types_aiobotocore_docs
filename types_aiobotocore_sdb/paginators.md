<a id="paginators-for-aiobotocore-simpledb-module"></a>

# Paginators for aiobotocore SimpleDB module

> [Index](..) > [SimpleDB](.) > Paginators

Auto-generated documentation for
[SimpleDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
type annotations stubs module
[types-aiobotocore-sdb](https://pypi.org/project/types-aiobotocore-sdb/).

- [Paginators for aiobotocore SimpleDB module](#paginators-for-aiobotocore-simpledb-module)
  - [ListDomainsPaginator](#listdomainspaginator)
  - [SelectPaginator](#selectpaginator)

<a id="listdomainspaginator"></a>

## ListDomainsPaginator

Type annotations for
`session.create_client("sdb").get_paginator("list_domains")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sdb.paginator import ListDomainsPaginator

session = get_session()
async with session.create_client("sdb") as client:
    client: SimpleDBClient
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")
```

Boto3 documentation:
[SimpleDB.Paginator.ListDomains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains)

Arguments for `ListDomainsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDomainsPaginator.paginate` returns
`_PageIterator`\[[ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef)\].

<a id="selectpaginator"></a>

## SelectPaginator

Type annotations for `session.create_client("sdb").get_paginator("select")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_sdb.paginator import SelectPaginator

session = get_session()
async with session.create_client("sdb") as client:
    client: SimpleDBClient
    paginator: SelectPaginator = client.get_paginator("select")
```

Boto3 documentation:
[SimpleDB.Paginator.Select](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.Select)

Arguments for `SelectPaginator.paginate` method:

- `SelectExpression`: `str` *(required)*
- `ConsistentRead`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SelectPaginator.paginate` returns
`_PageIterator`\[[SelectResultTypeDef](./type_defs.md#selectresulttypedef)\].
