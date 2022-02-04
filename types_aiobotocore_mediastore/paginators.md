<a id="paginators-for-aiobotocore-mediastore-module"></a>

# Paginators for aiobotocore MediaStore module

> [Index](..) > [MediaStore](.) > Paginators

Auto-generated documentation for
[MediaStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
type annotations stubs module
[types-aiobotocore-mediastore](https://pypi.org/project/types-aiobotocore-mediastore/).

- [Paginators for aiobotocore MediaStore module](#paginators-for-aiobotocore-mediastore-module)
  - [ListContainersPaginator](#listcontainerspaginator)

<a id="listcontainerspaginator"></a>

## ListContainersPaginator

Type annotations for
`aiobotocore.create_client("mediastore").get_paginator("list_containers")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_mediastore.paginator import ListContainersPaginator

def get_list_containers_paginator() -> ListContainersPaginator:
    return Session().create_client("mediastore").get_paginator("list_containers")
```

Boto3 documentation:
[MediaStore.Paginator.ListContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Paginator.ListContainers)

Arguments for `ListContainersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListContainersPaginator.paginate` returns
`_PageIterator`\[[ListContainersOutputTypeDef](./type_defs.md#listcontainersoutputtypedef)\].
