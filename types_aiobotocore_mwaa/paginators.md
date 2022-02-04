<a id="paginators-for-aiobotocore-mwaa-module"></a>

# Paginators for aiobotocore MWAA module

> [Index](..) > [MWAA](.) > Paginators

Auto-generated documentation for
[MWAA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
type annotations stubs module
[types-aiobotocore-mwaa](https://pypi.org/project/types-aiobotocore-mwaa/).

- [Paginators for aiobotocore MWAA module](#paginators-for-aiobotocore-mwaa-module)
  - [ListEnvironmentsPaginator](#listenvironmentspaginator)

<a id="listenvironmentspaginator"></a>

## ListEnvironmentsPaginator

Type annotations for
`aiobotocore.create_client("mwaa").get_paginator("list_environments")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_mwaa.paginator import ListEnvironmentsPaginator

def get_list_environments_paginator() -> ListEnvironmentsPaginator:
    return Session().create_client("mwaa").get_paginator("list_environments")
```

Boto3 documentation:
[MWAA.Paginator.ListEnvironments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)

Arguments for `ListEnvironmentsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEnvironmentsPaginator.paginate` returns
`_PageIterator`\[[ListEnvironmentsOutputTypeDef](./type_defs.md#listenvironmentsoutputtypedef)\].
