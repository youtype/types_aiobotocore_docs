<a id="paginators-for-aiobotocore-transfer-module"></a>

# Paginators for aiobotocore Transfer module

> [Index](..) > [Transfer](.) > Paginators

Auto-generated documentation for
[Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
type annotations stubs module
[types-aiobotocore-transfer](https://pypi.org/project/types-aiobotocore-transfer/).

- [Paginators for aiobotocore Transfer module](#paginators-for-aiobotocore-transfer-module)
  - [ListServersPaginator](#listserverspaginator)

<a id="listserverspaginator"></a>

## ListServersPaginator

Type annotations for
`session.create_client("transfer").get_paginator("list_servers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_transfer.paginator import ListServersPaginator

session = get_session()
async with session.create_client("transfer") as client:
    client: TransferClient
    paginator: ListServersPaginator = client.get_paginator("list_servers")
```

Boto3 documentation:
[Transfer.Paginator.ListServers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Paginator.ListServers)

Arguments for `ListServersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListServersPaginator.paginate` returns
`AsyncIterable`\[[ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef)\].
