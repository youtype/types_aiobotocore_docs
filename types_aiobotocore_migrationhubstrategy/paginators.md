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
`aiobotocore.create_client("migrationhubstrategy").get_paginator("get_server_details")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_migrationhubstrategy.paginator import GetServerDetailsPaginator

def get_get_server_details_paginator() -> GetServerDetailsPaginator:
    return Session().create_client("migrationhubstrategy").get_paginator("get_server_details")
```

Boto3 documentation:
[MigrationHubStrategyRecommendations.Paginator.GetServerDetails](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails)

Arguments for `GetServerDetailsPaginator.paginate` method:

- `serverId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetServerDetailsPaginator.paginate` returns
`_PageIterator`\[[GetServerDetailsResponseTypeDef](./type_defs.md#getserverdetailsresponsetypedef)\].

<a id="listapplicationcomponentspaginator"></a>

## ListApplicationComponentsPaginator

Type annotations for
`aiobotocore.create_client("migrationhubstrategy").get_paginator("list_application_components")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_migrationhubstrategy.paginator import ListApplicationComponentsPaginator

def get_list_application_components_paginator() -> ListApplicationComponentsPaginator:
    return Session().create_client("migrationhubstrategy").get_paginator("list_application_components")
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
`_PageIterator`\[[ListApplicationComponentsResponseTypeDef](./type_defs.md#listapplicationcomponentsresponsetypedef)\].

<a id="listcollectorspaginator"></a>

## ListCollectorsPaginator

Type annotations for
`aiobotocore.create_client("migrationhubstrategy").get_paginator("list_collectors")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_migrationhubstrategy.paginator import ListCollectorsPaginator

def get_list_collectors_paginator() -> ListCollectorsPaginator:
    return Session().create_client("migrationhubstrategy").get_paginator("list_collectors")
```

Boto3 documentation:
[MigrationHubStrategyRecommendations.Paginator.ListCollectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors)

Arguments for `ListCollectorsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCollectorsPaginator.paginate` returns
`_PageIterator`\[[ListCollectorsResponseTypeDef](./type_defs.md#listcollectorsresponsetypedef)\].

<a id="listimportfiletaskpaginator"></a>

## ListImportFileTaskPaginator

Type annotations for
`aiobotocore.create_client("migrationhubstrategy").get_paginator("list_import_file_task")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_migrationhubstrategy.paginator import ListImportFileTaskPaginator

def get_list_import_file_task_paginator() -> ListImportFileTaskPaginator:
    return Session().create_client("migrationhubstrategy").get_paginator("list_import_file_task")
```

Boto3 documentation:
[MigrationHubStrategyRecommendations.Paginator.ListImportFileTask](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask)

Arguments for `ListImportFileTaskPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListImportFileTaskPaginator.paginate` returns
`_PageIterator`\[[ListImportFileTaskResponseTypeDef](./type_defs.md#listimportfiletaskresponsetypedef)\].

<a id="listserverspaginator"></a>

## ListServersPaginator

Type annotations for
`aiobotocore.create_client("migrationhubstrategy").get_paginator("list_servers")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_migrationhubstrategy.paginator import ListServersPaginator

def get_list_servers_paginator() -> ListServersPaginator:
    return Session().create_client("migrationhubstrategy").get_paginator("list_servers")
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
`_PageIterator`\[[ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef)\].
