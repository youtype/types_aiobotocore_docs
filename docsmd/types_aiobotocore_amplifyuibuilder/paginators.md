# Paginators

> [Index](../README.md) > [AmplifyUIBuilder](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#amplifyuibuilder)
    type annotations stubs module [types-aiobotocore-amplifyuibuilder](https://pypi.org/project/types-aiobotocore-amplifyuibuilder/).

## ExportComponentsPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("export_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder/paginator/ExportComponents.html#AmplifyUIBuilder.Paginator.ExportComponents)

```python
# ExportComponentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ExportComponentsPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:  # (1)
    paginator: ExportComponentsPaginator = client.get_paginator("export_components")  # (2)
    async for item in paginator.paginate(...):
        item: ExportComponentsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ExportComponentsPaginator](./paginators.md#exportcomponentspaginator)
3. item: [:material-code-braces: ExportComponentsResponsePaginatorTypeDef](./type_defs.md#exportcomponentsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ExportComponentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ExportComponentsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ExportComponentsResponsePaginatorTypeDef](./type_defs.md#exportcomponentsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ExportComponentsRequestPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ExportComponentsRequestPaginateTypeDef](./type_defs.md#exportcomponentsrequestpaginatetypedef) 
## ExportFormsPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("export_forms")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder/paginator/ExportForms.html#AmplifyUIBuilder.Paginator.ExportForms)

```python
# ExportFormsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ExportFormsPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:  # (1)
    paginator: ExportFormsPaginator = client.get_paginator("export_forms")  # (2)
    async for item in paginator.paginate(...):
        item: ExportFormsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ExportFormsPaginator](./paginators.md#exportformspaginator)
3. item: [:material-code-braces: ExportFormsResponsePaginatorTypeDef](./type_defs.md#exportformsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ExportFormsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ExportFormsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ExportFormsResponsePaginatorTypeDef](./type_defs.md#exportformsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ExportFormsRequestPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ExportFormsRequestPaginateTypeDef](./type_defs.md#exportformsrequestpaginatetypedef) 
## ExportThemesPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("export_themes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder/paginator/ExportThemes.html#AmplifyUIBuilder.Paginator.ExportThemes)

```python
# ExportThemesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ExportThemesPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:  # (1)
    paginator: ExportThemesPaginator = client.get_paginator("export_themes")  # (2)
    async for item in paginator.paginate(...):
        item: ExportThemesResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ExportThemesPaginator](./paginators.md#exportthemespaginator)
3. item: [:material-code-braces: ExportThemesResponsePaginatorTypeDef](./type_defs.md#exportthemesresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ExportThemesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ExportThemesResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ExportThemesResponsePaginatorTypeDef](./type_defs.md#exportthemesresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ExportThemesRequestPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ExportThemesRequestPaginateTypeDef](./type_defs.md#exportthemesrequestpaginatetypedef) 
## ListCodegenJobsPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("list_codegen_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder/paginator/ListCodegenJobs.html#AmplifyUIBuilder.Paginator.ListCodegenJobs)

```python
# ListCodegenJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ListCodegenJobsPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:  # (1)
    paginator: ListCodegenJobsPaginator = client.get_paginator("list_codegen_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListCodegenJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ListCodegenJobsPaginator](./paginators.md#listcodegenjobspaginator)
3. item: [:material-code-braces: ListCodegenJobsResponseTypeDef](./type_defs.md#listcodegenjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCodegenJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCodegenJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCodegenJobsResponseTypeDef](./type_defs.md#listcodegenjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCodegenJobsRequestPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCodegenJobsRequestPaginateTypeDef](./type_defs.md#listcodegenjobsrequestpaginatetypedef) 
## ListComponentsPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("list_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder/paginator/ListComponents.html#AmplifyUIBuilder.Paginator.ListComponents)

```python
# ListComponentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ListComponentsPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:  # (1)
    paginator: ListComponentsPaginator = client.get_paginator("list_components")  # (2)
    async for item in paginator.paginate(...):
        item: ListComponentsResponseTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
3. item: [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListComponentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListComponentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListComponentsRequestPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComponentsRequestPaginateTypeDef](./type_defs.md#listcomponentsrequestpaginatetypedef) 
## ListFormsPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("list_forms")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder/paginator/ListForms.html#AmplifyUIBuilder.Paginator.ListForms)

```python
# ListFormsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ListFormsPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:  # (1)
    paginator: ListFormsPaginator = client.get_paginator("list_forms")  # (2)
    async for item in paginator.paginate(...):
        item: ListFormsResponseTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ListFormsPaginator](./paginators.md#listformspaginator)
3. item: [:material-code-braces: ListFormsResponseTypeDef](./type_defs.md#listformsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFormsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFormsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFormsResponseTypeDef](./type_defs.md#listformsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFormsRequestPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFormsRequestPaginateTypeDef](./type_defs.md#listformsrequestpaginatetypedef) 
## ListThemesPaginator

Type annotations and code completion for `#!python session.create_client("amplifyuibuilder").get_paginator("list_themes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder/paginator/ListThemes.html#AmplifyUIBuilder.Paginator.ListThemes)

```python
# ListThemesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_amplifyuibuilder.paginator import ListThemesPaginator

session = get_session()
async with session.create_client("amplifyuibuilder") as client:  # (1)
    paginator: ListThemesPaginator = client.get_paginator("list_themes")  # (2)
    async for item in paginator.paginate(...):
        item: ListThemesResponseTypeDef
        print(item)  # (3)
```

1. client: [AmplifyUIBuilderClient](./client.md)
2. paginator: [ListThemesPaginator](./paginators.md#listthemespaginator)
3. item: [:material-code-braces: ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThemesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    appId: str,
    environmentName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListThemesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListThemesResponseTypeDef](./type_defs.md#listthemesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListThemesRequestPaginateTypeDef = {  # (1)
    "appId": ...,
    "environmentName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThemesRequestPaginateTypeDef](./type_defs.md#listthemesrequestpaginatetypedef) 
