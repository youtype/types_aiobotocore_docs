<a id="paginators-for-aiobotocore-amplifyuibuilder-module"></a>

# Paginators for aiobotocore AmplifyUIBuilder module

> [Index](..) > [AmplifyUIBuilder](.) > Paginators

Auto-generated documentation for
[AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
type annotations stubs module
[types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).

- [Paginators for aiobotocore AmplifyUIBuilder module](#paginators-for-aiobotocore-amplifyuibuilder-module)
  - [ListComponentsPaginator](#listcomponentspaginator)
  - [ListThemesPaginator](#listthemespaginator)

<a id="listcomponentspaginator"></a>

## ListComponentsPaginator

Type annotations for
`session.create_client("amplifyuibuilder").get_paginator("list_components")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ListComponentsPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
    paginator: ListComponentsPaginator = client.get_paginator("list_components")
```

Boto3 documentation:
[AmplifyUIBuilder.Paginator.ListComponents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents)

Arguments for `ListComponentsPaginator.paginate` method:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListComponentsPaginator.paginate` returns
`AsyncIterable`\[[ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef)\].

<a id="listthemespaginator"></a>

## ListThemesPaginator

Type annotations for
`session.create_client("amplifyuibuilder").get_paginator("list_themes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ListThemesPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
    paginator: ListThemesPaginator = client.get_paginator("list_themes")
```

Boto3 documentation:
[AmplifyUIBuilder.Paginator.ListThemes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes)

Arguments for `ListThemesPaginator.paginate` method:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThemesPaginator.paginate` returns
`AsyncIterable`\[[ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef)\].
