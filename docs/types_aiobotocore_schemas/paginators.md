<a id="paginators-for-aiobotocore-schemas-module"></a>

# Paginators for aiobotocore Schemas module

> [Index](../README.md) > [Schemas](./README.md) > Paginators

Auto-generated documentation for
[Schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
type annotations stubs module
[types-aiobotocore-schemas](https://pypi.org/project/types-aiobotocore-schemas/).

- [Paginators for aiobotocore Schemas module](#paginators-for-aiobotocore-schemas-module)
  - [ListDiscoverersPaginator](#listdiscovererspaginator)
  - [ListRegistriesPaginator](#listregistriespaginator)
  - [ListSchemaVersionsPaginator](#listschemaversionspaginator)
  - [ListSchemasPaginator](#listschemaspaginator)
  - [SearchSchemasPaginator](#searchschemaspaginator)

<a id="listdiscovererspaginator"></a>

## ListDiscoverersPaginator

Type annotations for
`session.create_client("schemas").get_paginator("list_discoverers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_schemas.paginator import ListDiscoverersPaginator

session = get_session()
async with session.create_client("schemas") as client:
    client: SchemasClient
    paginator: ListDiscoverersPaginator = client.get_paginator("list_discoverers")
```

Boto3 documentation:
[Schemas.Paginator.ListDiscoverers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers)

Arguments for `ListDiscoverersPaginator.paginate` method:

- `DiscovererIdPrefix`: `str`
- `SourceArnPrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDiscoverersPaginator.paginate` returns
`AsyncIterator`\[[ListDiscoverersResponseTypeDef](./type_defs.md#listdiscoverersresponsetypedef)\].

<a id="listregistriespaginator"></a>

## ListRegistriesPaginator

Type annotations for
`session.create_client("schemas").get_paginator("list_registries")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_schemas.paginator import ListRegistriesPaginator

session = get_session()
async with session.create_client("schemas") as client:
    client: SchemasClient
    paginator: ListRegistriesPaginator = client.get_paginator("list_registries")
```

Boto3 documentation:
[Schemas.Paginator.ListRegistries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries)

Arguments for `ListRegistriesPaginator.paginate` method:

- `RegistryNamePrefix`: `str`
- `Scope`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRegistriesPaginator.paginate` returns
`AsyncIterator`\[[ListRegistriesResponseTypeDef](./type_defs.md#listregistriesresponsetypedef)\].

<a id="listschemaversionspaginator"></a>

## ListSchemaVersionsPaginator

Type annotations for
`session.create_client("schemas").get_paginator("list_schema_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_schemas.paginator import ListSchemaVersionsPaginator

session = get_session()
async with session.create_client("schemas") as client:
    client: SchemasClient
    paginator: ListSchemaVersionsPaginator = client.get_paginator("list_schema_versions")
```

Boto3 documentation:
[Schemas.Paginator.ListSchemaVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions)

Arguments for `ListSchemaVersionsPaginator.paginate` method:

- `RegistryName`: `str` *(required)*
- `SchemaName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSchemaVersionsPaginator.paginate` returns
`AsyncIterator`\[[ListSchemaVersionsResponseTypeDef](./type_defs.md#listschemaversionsresponsetypedef)\].

<a id="listschemaspaginator"></a>

## ListSchemasPaginator

Type annotations for
`session.create_client("schemas").get_paginator("list_schemas")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_schemas.paginator import ListSchemasPaginator

session = get_session()
async with session.create_client("schemas") as client:
    client: SchemasClient
    paginator: ListSchemasPaginator = client.get_paginator("list_schemas")
```

Boto3 documentation:
[Schemas.Paginator.ListSchemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas)

Arguments for `ListSchemasPaginator.paginate` method:

- `RegistryName`: `str` *(required)*
- `SchemaNamePrefix`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSchemasPaginator.paginate` returns
`AsyncIterator`\[[ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef)\].

<a id="searchschemaspaginator"></a>

## SearchSchemasPaginator

Type annotations for
`session.create_client("schemas").get_paginator("search_schemas")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_schemas.paginator import SearchSchemasPaginator

session = get_session()
async with session.create_client("schemas") as client:
    client: SchemasClient
    paginator: SearchSchemasPaginator = client.get_paginator("search_schemas")
```

Boto3 documentation:
[Schemas.Paginator.SearchSchemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas)

Arguments for `SearchSchemasPaginator.paginate` method:

- `Keywords`: `str` *(required)*
- `RegistryName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`SearchSchemasPaginator.paginate` returns
`AsyncIterator`\[[SearchSchemasResponseTypeDef](./type_defs.md#searchschemasresponsetypedef)\].
