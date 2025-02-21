# Paginators

> [Index](../README.md) > [Schemas](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#schemas)
    type annotations stubs module [types-aiobotocore-schemas](https://pypi.org/project/types-aiobotocore-schemas/).

## ListDiscoverersPaginator

Type annotations and code completion for `#!python session.create_client("schemas").get_paginator("list_discoverers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas/paginator/ListDiscoverers.html#Schemas.Paginator.ListDiscoverers)

```python
# ListDiscoverersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_schemas.paginator import ListDiscoverersPaginator

session = get_session()
async with session.create_client("schemas") as client:  # (1)
    paginator: ListDiscoverersPaginator = client.get_paginator("list_discoverers")  # (2)
    async for item in paginator.paginate(...):
        item: ListDiscoverersResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListDiscoverersPaginator](./paginators.md#listdiscovererspaginator)
3. item: [:material-code-braces: ListDiscoverersResponseTypeDef](./type_defs.md#listdiscoverersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDiscoverersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DiscovererIdPrefix: str = ...,
    SourceArnPrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDiscoverersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDiscoverersResponseTypeDef](./type_defs.md#listdiscoverersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDiscoverersRequestPaginateTypeDef = {  # (1)
    "DiscovererIdPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDiscoverersRequestPaginateTypeDef](./type_defs.md#listdiscoverersrequestpaginatetypedef) 
## ListRegistriesPaginator

Type annotations and code completion for `#!python session.create_client("schemas").get_paginator("list_registries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas/paginator/ListRegistries.html#Schemas.Paginator.ListRegistries)

```python
# ListRegistriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_schemas.paginator import ListRegistriesPaginator

session = get_session()
async with session.create_client("schemas") as client:  # (1)
    paginator: ListRegistriesPaginator = client.get_paginator("list_registries")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegistriesResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListRegistriesPaginator](./paginators.md#listregistriespaginator)
3. item: [:material-code-braces: ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRegistriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistryNamePrefix: str = ...,
    Scope: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRegistriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRegistriesRequestPaginateTypeDef = {  # (1)
    "RegistryNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegistriesRequestPaginateTypeDef](./type_defs.md#listregistriesrequestpaginatetypedef) 
## ListSchemaVersionsPaginator

Type annotations and code completion for `#!python session.create_client("schemas").get_paginator("list_schema_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas/paginator/ListSchemaVersions.html#Schemas.Paginator.ListSchemaVersions)

```python
# ListSchemaVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_schemas.paginator import ListSchemaVersionsPaginator

session = get_session()
async with session.create_client("schemas") as client:  # (1)
    paginator: ListSchemaVersionsPaginator = client.get_paginator("list_schema_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemaVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListSchemaVersionsPaginator](./paginators.md#listschemaversionspaginator)
3. item: [:material-code-braces: ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemaVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistryName: str,
    SchemaName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSchemaVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemaVersionsRequestPaginateTypeDef = {  # (1)
    "RegistryName": ...,
    "SchemaName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemaVersionsRequestPaginateTypeDef](./type_defs.md#listschemaversionsrequestpaginatetypedef) 
## ListSchemasPaginator

Type annotations and code completion for `#!python session.create_client("schemas").get_paginator("list_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas/paginator/ListSchemas.html#Schemas.Paginator.ListSchemas)

```python
# ListSchemasPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_schemas.paginator import ListSchemasPaginator

session = get_session()
async with session.create_client("schemas") as client:  # (1)
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemasResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [ListSchemasPaginator](./paginators.md#listschemaspaginator)
3. item: [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemasPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistryName: str,
    SchemaNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemasRequestPaginateTypeDef = {  # (1)
    "RegistryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemasRequestPaginateTypeDef](./type_defs.md#listschemasrequestpaginatetypedef) 
## SearchSchemasPaginator

Type annotations and code completion for `#!python session.create_client("schemas").get_paginator("search_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas/paginator/SearchSchemas.html#Schemas.Paginator.SearchSchemas)

```python
# SearchSchemasPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_schemas.paginator import SearchSchemasPaginator

session = get_session()
async with session.create_client("schemas") as client:  # (1)
    paginator: SearchSchemasPaginator = client.get_paginator("search_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: SearchSchemasResponseTypeDef
        print(item)  # (3)
```

1. client: [SchemasClient](./client.md)
2. paginator: [SearchSchemasPaginator](./paginators.md#searchschemaspaginator)
3. item: [:material-code-braces: SearchSchemasResponseTypeDef](./type_defs.md#searchschemasresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchSchemasPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Keywords: str,
    RegistryName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[SearchSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SearchSchemasResponseTypeDef](./type_defs.md#searchschemasresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchSchemasRequestPaginateTypeDef = {  # (1)
    "Keywords": ...,
    "RegistryName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSchemasRequestPaginateTypeDef](./type_defs.md#searchschemasrequestpaginatetypedef) 
