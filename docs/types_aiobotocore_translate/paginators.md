<a id="paginators-for-aiobotocore-translate-module"></a>

# Paginators for aiobotocore Translate module

> [Index](../README.md) > [Translate](./README.md) > Paginators

Auto-generated documentation for
[Translate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
type annotations stubs module
[types-aiobotocore-translate](https://pypi.org/project/types-aiobotocore-translate/).

- [Paginators for aiobotocore Translate module](#paginators-for-aiobotocore-translate-module)
  - [ListTerminologiesPaginator](#listterminologiespaginator)

<a id="listterminologiespaginator"></a>

## ListTerminologiesPaginator

Type annotations for
`session.create_client("translate").get_paginator("list_terminologies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_translate.paginator import ListTerminologiesPaginator

session = get_session()
async with session.create_client("translate") as client:
    client: TranslateClient
    paginator: ListTerminologiesPaginator = client.get_paginator("list_terminologies")
```

Boto3 documentation:
[Translate.Paginator.ListTerminologies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)

Arguments for `ListTerminologiesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTerminologiesPaginator.paginate` returns
`AsyncIterator`\[[ListTerminologiesResponseTypeDef](./type_defs.md#listterminologiesresponsetypedef)\].