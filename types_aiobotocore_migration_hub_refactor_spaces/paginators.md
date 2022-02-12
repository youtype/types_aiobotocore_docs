<a id="paginators-for-aiobotocore-migrationhubrefactorspaces-module"></a>

# Paginators for aiobotocore MigrationHubRefactorSpaces module

> [Index](..) > [MigrationHubRefactorSpaces](.) > Paginators

Auto-generated documentation for
[MigrationHubRefactorSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
type annotations stubs module
[types-aiobotocore-migration-hub-refactor-spaces](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces/).

- [Paginators for aiobotocore MigrationHubRefactorSpaces module](#paginators-for-aiobotocore-migrationhubrefactorspaces-module)
  - [ListApplicationsPaginator](#listapplicationspaginator)
  - [ListEnvironmentVpcsPaginator](#listenvironmentvpcspaginator)
  - [ListEnvironmentsPaginator](#listenvironmentspaginator)
  - [ListRoutesPaginator](#listroutespaginator)
  - [ListServicesPaginator](#listservicespaginator)

<a id="listapplicationspaginator"></a>

## ListApplicationsPaginator

Type annotations for
`session.create_client("migration-hub-refactor-spaces").get_paginator("list_applications")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListApplicationsPaginator

session = get_session()
async with session.create_client("migration-hub-refactor-spaces") as client:
    client: MigrationHubRefactorSpacesClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
```

Boto3 documentation:
[MigrationHubRefactorSpaces.Paginator.ListApplications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListApplications)

Arguments for `ListApplicationsPaginator.paginate` method:

- `EnvironmentIdentifier`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationsPaginator.paginate` returns
`AsyncIterable`\[[ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef)\].

<a id="listenvironmentvpcspaginator"></a>

## ListEnvironmentVpcsPaginator

Type annotations for
`session.create_client("migration-hub-refactor-spaces").get_paginator("list_environment_vpcs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListEnvironmentVpcsPaginator

session = get_session()
async with session.create_client("migration-hub-refactor-spaces") as client:
    client: MigrationHubRefactorSpacesClient
    paginator: ListEnvironmentVpcsPaginator = client.get_paginator("list_environment_vpcs")
```

Boto3 documentation:
[MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs)

Arguments for `ListEnvironmentVpcsPaginator.paginate` method:

- `EnvironmentIdentifier`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEnvironmentVpcsPaginator.paginate` returns
`AsyncIterable`\[[ListEnvironmentVpcsResponseTypeDef](./type_defs.md#listenvironmentvpcsresponsetypedef)\].

<a id="listenvironmentspaginator"></a>

## ListEnvironmentsPaginator

Type annotations for
`session.create_client("migration-hub-refactor-spaces").get_paginator("list_environments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListEnvironmentsPaginator

session = get_session()
async with session.create_client("migration-hub-refactor-spaces") as client:
    client: MigrationHubRefactorSpacesClient
    paginator: ListEnvironmentsPaginator = client.get_paginator("list_environments")
```

Boto3 documentation:
[MigrationHubRefactorSpaces.Paginator.ListEnvironments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments)

Arguments for `ListEnvironmentsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEnvironmentsPaginator.paginate` returns
`AsyncIterable`\[[ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef)\].

<a id="listroutespaginator"></a>

## ListRoutesPaginator

Type annotations for
`session.create_client("migration-hub-refactor-spaces").get_paginator("list_routes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListRoutesPaginator

session = get_session()
async with session.create_client("migration-hub-refactor-spaces") as client:
    client: MigrationHubRefactorSpacesClient
    paginator: ListRoutesPaginator = client.get_paginator("list_routes")
```

Boto3 documentation:
[MigrationHubRefactorSpaces.Paginator.ListRoutes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListRoutes)

Arguments for `ListRoutesPaginator.paginate` method:

- `ApplicationIdentifier`: `str` *(required)*
- `EnvironmentIdentifier`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRoutesPaginator.paginate` returns
`AsyncIterable`\[[ListRoutesResponseTypeDef](./type_defs.md#listroutesresponsetypedef)\].

<a id="listservicespaginator"></a>

## ListServicesPaginator

Type annotations for
`session.create_client("migration-hub-refactor-spaces").get_paginator("list_services")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListServicesPaginator

session = get_session()
async with session.create_client("migration-hub-refactor-spaces") as client:
    client: MigrationHubRefactorSpacesClient
    paginator: ListServicesPaginator = client.get_paginator("list_services")
```

Boto3 documentation:
[MigrationHubRefactorSpaces.Paginator.ListServices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListServices)

Arguments for `ListServicesPaginator.paginate` method:

- `ApplicationIdentifier`: `str` *(required)*
- `EnvironmentIdentifier`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListServicesPaginator.paginate` returns
`AsyncIterable`\[[ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef)\].
