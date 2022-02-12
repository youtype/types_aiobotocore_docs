<a id="paginators-for-aiobotocore-recyclebin-module"></a>

# Paginators for aiobotocore RecycleBin module

> [Index](..) > [RecycleBin](.) > Paginators

Auto-generated documentation for
[RecycleBin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
type annotations stubs module
[types-aiobotocore-rbin](https://pypi.org/project/types-aiobotocore-rbin/).

- [Paginators for aiobotocore RecycleBin module](#paginators-for-aiobotocore-recyclebin-module)
  - [ListRulesPaginator](#listrulespaginator)

<a id="listrulespaginator"></a>

## ListRulesPaginator

Type annotations for
`session.create_client("rbin").get_paginator("list_rules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_rbin.paginator import ListRulesPaginator

session = get_session()
async with session.create_client("rbin") as client:
    client: RecycleBinClient
    paginator: ListRulesPaginator = client.get_paginator("list_rules")
```

Boto3 documentation:
[RecycleBin.Paginator.ListRules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Paginator.ListRules)

Arguments for `ListRulesPaginator.paginate` method:

- `ResourceType`: `Literal['EBS_SNAPSHOT']` (see
  [ResourceTypeType](./literals.md#resourcetypetype)) *(required)*
- `ResourceTags`:
  `Sequence`\[[ResourceTagTypeDef](./type_defs.md#resourcetagtypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRulesPaginator.paginate` returns
`AsyncIterable`\[[ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef)\].
