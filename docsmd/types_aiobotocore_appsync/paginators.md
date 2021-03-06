# Paginators

> [Index](../README.md) > [AppSync](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AppSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
    type annotations stubs module [types-aiobotocore-appsync](https://pypi.org/project/types-aiobotocore-appsync/).

## ListApiKeysPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_api_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListApiKeys)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListApiKeysPaginator

session = get_session()
async with session.create_client("appsync") as client:
    client: AppSyncClient
    paginator: ListApiKeysPaginator = client.get_paginator("list_api_keys")
```


### paginate

Type annotations and code completion for `#!python ListApiKeysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    apiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListApiKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListApiKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListApiKeysRequestListApiKeysPaginateTypeDef = {  # (1)
    "apiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApiKeysRequestListApiKeysPaginateTypeDef](./type_defs.md#listapikeysrequestlistapikeyspaginatetypedef) 
## ListDataSourcesPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_data_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListDataSources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListDataSourcesPaginator

session = get_session()
async with session.create_client("appsync") as client:
    client: AppSyncClient
    paginator: ListDataSourcesPaginator = client.get_paginator("list_data_sources")
```


### paginate

Type annotations and code completion for `#!python ListDataSourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    apiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDataSourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDataSourcesRequestListDataSourcesPaginateTypeDef = {  # (1)
    "apiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestListDataSourcesPaginateTypeDef](./type_defs.md#listdatasourcesrequestlistdatasourcespaginatetypedef) 
## ListFunctionsPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_functions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListFunctions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListFunctionsPaginator

session = get_session()
async with session.create_client("appsync") as client:
    client: AppSyncClient
    paginator: ListFunctionsPaginator = client.get_paginator("list_functions")
```


### paginate

Type annotations and code completion for `#!python ListFunctionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    apiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFunctionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFunctionsResponseTypeDef](./type_defs.md#listfunctionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFunctionsRequestListFunctionsPaginateTypeDef = {  # (1)
    "apiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFunctionsRequestListFunctionsPaginateTypeDef](./type_defs.md#listfunctionsrequestlistfunctionspaginatetypedef) 
## ListGraphqlApisPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_graphql_apis")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListGraphqlApis)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListGraphqlApisPaginator

session = get_session()
async with session.create_client("appsync") as client:
    client: AppSyncClient
    paginator: ListGraphqlApisPaginator = client.get_paginator("list_graphql_apis")
```


### paginate

Type annotations and code completion for `#!python ListGraphqlApisPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGraphqlApisResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGraphqlApisResponseTypeDef](./type_defs.md#listgraphqlapisresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListGraphqlApisRequestListGraphqlApisPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGraphqlApisRequestListGraphqlApisPaginateTypeDef](./type_defs.md#listgraphqlapisrequestlistgraphqlapispaginatetypedef) 
## ListResolversPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_resolvers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListResolversPaginator

session = get_session()
async with session.create_client("appsync") as client:
    client: AppSyncClient
    paginator: ListResolversPaginator = client.get_paginator("list_resolvers")
```


### paginate

Type annotations and code completion for `#!python ListResolversPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    apiId: str,
    typeName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResolversResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResolversResponseTypeDef](./type_defs.md#listresolversresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListResolversRequestListResolversPaginateTypeDef = {  # (1)
    "apiId": ...,
    "typeName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolversRequestListResolversPaginateTypeDef](./type_defs.md#listresolversrequestlistresolverspaginatetypedef) 
## ListResolversByFunctionPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_resolvers_by_function")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListResolversByFunctionPaginator

session = get_session()
async with session.create_client("appsync") as client:
    client: AppSyncClient
    paginator: ListResolversByFunctionPaginator = client.get_paginator("list_resolvers_by_function")
```


### paginate

Type annotations and code completion for `#!python ListResolversByFunctionPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    apiId: str,
    functionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResolversByFunctionResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResolversByFunctionResponseTypeDef](./type_defs.md#listresolversbyfunctionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = {  # (1)
    "apiId": ...,
    "functionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef](./type_defs.md#listresolversbyfunctionrequestlistresolversbyfunctionpaginatetypedef) 
## ListTypesPaginator

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator("list_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListTypes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appsync.paginator import ListTypesPaginator

session = get_session()
async with session.create_client("appsync") as client:
    client: AppSyncClient
    paginator: ListTypesPaginator = client.get_paginator("list_types")
```


### paginate

Type annotations and code completion for `#!python ListTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    apiId: str,
    format: TypeDefinitionFormatType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListTypesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TypeDefinitionFormatType](./literals.md#typedefinitionformattype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTypesResponseTypeDef](./type_defs.md#listtypesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTypesRequestListTypesPaginateTypeDef = {  # (1)
    "apiId": ...,
    "format": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTypesRequestListTypesPaginateTypeDef](./type_defs.md#listtypesrequestlisttypespaginatetypedef) 
