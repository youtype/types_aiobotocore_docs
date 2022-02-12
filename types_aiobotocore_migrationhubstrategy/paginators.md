<a id="paginators-for-aiobotocore-migrationhubstrategyrecommendations-module"></a>

# Paginators for aiobotocore MigrationHubStrategyRecommendations module

> [Index](..) > [MigrationHubStrategyRecommendations](.) > Paginators

Auto-generated documentation for
[MigrationHubStrategyRecommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
type annotations stubs module
[types-aiobotocore-migrationhubstrategy](https://pypi.org/project/types-aiobotocore-migrationhubstrategy/).

- [Paginators for aiobotocore MigrationHubStrategyRecommendations module](#paginators-for-aiobotocore-migrationhubstrategyrecommendations-module)
  - [GetServerDetailsPaginator](#getserverdetailspaginator)
  - [ListApplicationComponentsPaginator](#listapplicationcomponentspaginator)
  - [ListCollectorsPaginator](#listcollectorspaginator)
  - [ListImportFileTaskPaginator](#listimportfiletaskpaginator)
  - [ListServersPaginator](#listserverspaginator)

<a id="getserverdetailspaginator"></a>

## GetServerDetailsPaginator

Type annotations for
`session.create_client("migrationhubstrategy").get_paginator("get_server_details")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import GetServerDetailsPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: GetServerDetailsPaginator = client.get_paginator("get_server_details")
```

Boto3 documentation:
[MigrationHubStrategyRecommendations.Paginator.GetServerDetails](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails)

Arguments for `GetServerDetailsPaginator.paginate` method:

- `serverId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetServerDetailsPaginator.paginate` returns
`AsyncIterable`\[[GetServerDetailsResponseTypeDef](./type_defs.md#getserverdetailsresponsetypedef)\].

<a id="listapplicationcomponentspaginator"></a>

## ListApplicationComponentsPaginator

Type annotations for
`session.create_client("migrationhubstrategy").get_paginator("list_application_components")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListApplicationComponentsPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: ListApplicationComponentsPaginator = client.get_paginator("list_application_components")
```

Boto3 documentation:
[MigrationHubStrategyRecommendations.Paginator.ListApplicationComponents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListApplicationComponents)

Arguments for `ListApplicationComponentsPaginator.paginate` method:

- `applicationComponentCriteria`:
  [ApplicationComponentCriteriaType](./literals.md#applicationcomponentcriteriatype)
- `filterValue`: `str`
- `groupIdFilter`: `Sequence`\[[GroupTypeDef](./type_defs.md#grouptypedef)\]
- `sort`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListApplicationComponentsPaginator.paginate` returns
`AsyncIterable`\[[ListApplicationComponentsResponseTypeDef](./type_defs.md#listapplicationcomponentsresponsetypedef)\].

<a id="listcollectorspaginator"></a>

## ListCollectorsPaginator

Type annotations for
`session.create_client("migrationhubstrategy").get_paginator("list_collectors")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListCollectorsPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: ListCollectorsPaginator = client.get_paginator("list_collectors")
```

Boto3 documentation:
[MigrationHubStrategyRecommendations.Paginator.ListCollectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors)

Arguments for `ListCollectorsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCollectorsPaginator.paginate` returns
`AsyncIterable`\[[ListCollectorsResponseTypeDef](./type_defs.md#listcollectorsresponsetypedef)\].

<a id="listimportfiletaskpaginator"></a>

## ListImportFileTaskPaginator

Type annotations for
`session.create_client("migrationhubstrategy").get_paginator("list_import_file_task")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListImportFileTaskPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: ListImportFileTaskPaginator = client.get_paginator("list_import_file_task")
```

Boto3 documentation:
[MigrationHubStrategyRecommendations.Paginator.ListImportFileTask](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask)

Arguments for `ListImportFileTaskPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListImportFileTaskPaginator.paginate` returns
`AsyncIterable`\[[ListImportFileTaskResponseTypeDef](./type_defs.md#listimportfiletaskresponsetypedef)\].

<a id="listserverspaginator"></a>

## ListServersPaginator

Type annotations for
`session.create_client("migrationhubstrategy").get_paginator("list_servers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListServersPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: ListServersPaginator = client.get_paginator("list_servers")
```

Boto3 documentation:
[MigrationHubStrategyRecommendations.Paginator.ListServers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListServers)

Arguments for `ListServersPaginator.paginate` method:

- `filterValue`: `str`
- `groupIdFilter`: `Sequence`\[[GroupTypeDef](./type_defs.md#grouptypedef)\]
- `serverCriteria`: [ServerCriteriaType](./literals.md#servercriteriatype)
- `sort`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListServersPaginator.paginate` returns
`AsyncIterable`\[[ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef)\].
