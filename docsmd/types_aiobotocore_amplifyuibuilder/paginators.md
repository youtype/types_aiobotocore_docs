# Paginators

> [Index](../README.md) > [AmplifyUIBuilder](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
    type annotations stubs module [types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).

## ExportComponentsPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("export_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportComponents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ExportComponentsPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
    paginator: ExportComponentsPaginator = client.get_paginator("export_components")
```


### paginate

Type annotations and code completion for `#!python ExportComponentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ExportComponentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ExportComponentsResponseTypeDef](./type_defs.md#exportcomponentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ExportComponentsRequestExportComponentsPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ExportComponentsRequestExportComponentsPaginateTypeDef](./type_defs.md#exportcomponentsrequestexportcomponentspaginatetypedef) 
## ExportThemesPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("export_themes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ExportThemes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ExportThemesPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
    paginator: ExportThemesPaginator = client.get_paginator("export_themes")
```


### paginate

Type annotations and code completion for `#!python ExportThemesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ExportThemesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ExportThemesResponseTypeDef](./type_defs.md#exportthemesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ExportThemesRequestExportThemesPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ExportThemesRequestExportThemesPaginateTypeDef](./type_defs.md#exportthemesrequestexportthemespaginatetypedef) 
## ListComponentsPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("list_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListComponents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ListComponentsPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
    paginator: ListComponentsPaginator = client.get_paginator("list_components")
```


### paginate

Type annotations and code completion for `#!python ListComponentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListComponentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListComponentsRequestListComponentsPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComponentsRequestListComponentsPaginateTypeDef](./type_defs.md#listcomponentsrequestlistcomponentspaginatetypedef) 
## ListThemesPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("list_themes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Paginator.ListThemes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ListThemesPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:
    client: AmplifyUIBuilderClient
    paginator: ListThemesPaginator = client.get_paginator("list_themes")
```


### paginate

Type annotations and code completion for `#!python ListThemesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListThemesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThemesRequestListThemesPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThemesRequestListThemesPaginateTypeDef](./type_defs.md#listthemesrequestlistthemespaginatetypedef) 
