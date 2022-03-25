<a id="paginators-for-aiobotocore-mwaa-module"></a>

# Paginators for aiobotocore MWAA module

> [Index](../README.md) > [MWAA](./README.md) > Paginators

Auto-generated documentation for
[MWAA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
type annotations stubs module
[types-aiobotocore-mwaa](https://pypi.org/project/types-aiobotocore-mwaa/).

- [Paginators for aiobotocore MWAA module](#paginators-for-aiobotocore-mwaa-module)
  - [ListEnvironmentsPaginator](#listenvironmentspaginator)

<a id="listenvironmentspaginator"></a>

## ListEnvironmentsPaginator

Type annotations for
`session.create_client("mwaa").get_paginator("list_environments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mwaa.paginator import ListEnvironmentsPaginator

session = get_session()
async with session.create_client("mwaa") as client:
    client: MWAAClient
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
```

Boto3 documentation:
[MWAA.Paginator.ListEnvironments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)

Arguments for `ListEnvironmentsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEnvironmentsPaginator.paginate` returns
`AsyncIterator`\[[ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef)\].