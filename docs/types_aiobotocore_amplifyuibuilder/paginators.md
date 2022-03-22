<a id="paginators-for-aiobotocore-amplifyuibuilder-module"></a>

# Paginators for aiobotocore AmplifyUIBuilder module

> [Index](../README.md) > [AmplifyUIBuilder](./README.md) > Paginators

Auto-generated documentation for
[AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
type annotations stubs module
[types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).

- [Paginators for aiobotocore AmplifyUIBuilder module](#paginators-for-aiobotocore-amplifyuibuilder-module)
  - [ExportComponentsPaginator](#exportcomponentspaginator)
  - [ExportThemesPaginator](#exportthemespaginator)
  - [ListComponentsPaginator](#listcomponentspaginator)
  - [ListThemesPaginator](#listthemespaginator)

<a id="exportcomponentspaginator"></a>

## ExportComponentsPaginator

Type annotations for
`session.create_client("amplifyuibuilder").get_paginator("export_components")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ExportComponentsPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
    paginator: ExportComponentsPaginator = client.get_paginator("export_components")
```

Boto3 documentation:
[AmplifyUIBuilder.Paginator.ExportComponents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents)

Arguments for `ExportComponentsPaginator.paginate` method:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ExportComponentsPaginator.paginate` returns
`AsyncIterator`\[[ExportComponentsResponseTypeDef](./type_defs.md#exportcomponentsresponsetypedef)\].

<a id="exportthemespaginator"></a>

## ExportThemesPaginator

Type annotations for
`session.create_client("amplifyuibuilder").get_paginator("export_themes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ExportThemesPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
    paginator: ExportThemesPaginator = client.get_paginator("export_themes")
```

Boto3 documentation:
[AmplifyUIBuilder.Paginator.ExportThemes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes)

Arguments for `ExportThemesPaginator.paginate` method:

- `appId`: `str` *(required)*
- `environmentName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ExportThemesPaginator.paginate` returns
`AsyncIterator`\[[ExportThemesResponseTypeDef](./type_defs.md#exportthemesresponsetypedef)\].

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
`AsyncIterator`\[[ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef)\].

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
`AsyncIterator`\[[ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef)\].
