<a id="paginators-for-aiobotocore-shield-module"></a>

# Paginators for aiobotocore Shield module

> [Index](..) > [Shield](.) > Paginators

Auto-generated documentation for
[Shield](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
type annotations stubs module
[types-aiobotocore-shield](https://pypi.org/project/types-aiobotocore-shield/).

- [Paginators for aiobotocore Shield module](#paginators-for-aiobotocore-shield-module)
  - [ListAttacksPaginator](#listattackspaginator)
  - [ListProtectionsPaginator](#listprotectionspaginator)

<a id="listattackspaginator"></a>

## ListAttacksPaginator

Type annotations for
`session.create_client("shield").get_paginator("list_attacks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_shield.paginator import ListAttacksPaginator

session = get_session()
async with session.create_client("shield") as client:
    client: ShieldClient
    paginator: ListAttacksPaginator = client.get_paginator("list_attacks")
```

Boto3 documentation:
[Shield.Paginator.ListAttacks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks)

Arguments for `ListAttacksPaginator.paginate` method:

- `ResourceArns`: `Sequence`\[`str`\]
- `StartTime`: [TimeRangeTypeDef](./type_defs.md#timerangetypedef)
- `EndTime`: [TimeRangeTypeDef](./type_defs.md#timerangetypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAttacksPaginator.paginate` returns
`_PageIterator`\[[ListAttacksResponseTypeDef](./type_defs.md#listattacksresponsetypedef)\].

<a id="listprotectionspaginator"></a>

## ListProtectionsPaginator

Type annotations for
`session.create_client("shield").get_paginator("list_protections")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_shield.paginator import ListProtectionsPaginator

session = get_session()
async with session.create_client("shield") as client:
    client: ShieldClient
    paginator: ListProtectionsPaginator = client.get_paginator("list_protections")
```

Boto3 documentation:
[Shield.Paginator.ListProtections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections)

Arguments for `ListProtectionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListProtectionsPaginator.paginate` returns
`_PageIterator`\[[ListProtectionsResponseTypeDef](./type_defs.md#listprotectionsresponsetypedef)\].
