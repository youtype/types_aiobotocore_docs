# Paginators

> [Index](../README.md) > [MigrationHubStrategyRecommendations](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MigrationHubStrategyRecommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
    type annotations stubs module [types-aiobotocore-migrationhubstrategy](https://pypi.org/project/types-aiobotocore-migrationhubstrategy/).

## GetServerDetailsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("get_server_details")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import GetServerDetailsPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: GetServerDetailsPaginator = client.get_paginator("get_server_details")
```


### paginate

Type annotations and code completion for `#!python GetServerDetailsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    serverId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetServerDetailsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetServerDetailsResponseTypeDef](./type_defs.md#getserverdetailsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetServerDetailsRequestGetServerDetailsPaginateTypeDef = {  # (1)
    "serverId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetServerDetailsRequestGetServerDetailsPaginateTypeDef](./type_defs.md#getserverdetailsrequestgetserverdetailspaginatetypedef) 
## ListApplicationComponentsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("list_application_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListApplicationComponents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListApplicationComponentsPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: ListApplicationComponentsPaginator = client.get_paginator("list_application_components")
```


### paginate

Type annotations and code completion for `#!python ListApplicationComponentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    applicationComponentCriteria: ApplicationComponentCriteriaType = ...,  # (1)
    filterValue: str = ...,
    groupIdFilter: Sequence[GroupTypeDef] = ...,  # (2)
    sort: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[ListApplicationComponentsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ApplicationComponentCriteriaType](./literals.md#applicationcomponentcriteriatype) 
2. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListApplicationComponentsResponseTypeDef](./type_defs.md#listapplicationcomponentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef = {  # (1)
    "applicationComponentCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef](./type_defs.md#listapplicationcomponentsrequestlistapplicationcomponentspaginatetypedef) 
## ListCollectorsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("list_collectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListCollectorsPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: ListCollectorsPaginator = client.get_paginator("list_collectors")
```


### paginate

Type annotations and code completion for `#!python ListCollectorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCollectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCollectorsResponseTypeDef](./type_defs.md#listcollectorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCollectorsRequestListCollectorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollectorsRequestListCollectorsPaginateTypeDef](./type_defs.md#listcollectorsrequestlistcollectorspaginatetypedef) 
## ListImportFileTaskPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("list_import_file_task")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListImportFileTaskPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: ListImportFileTaskPaginator = client.get_paginator("list_import_file_task")
```


### paginate

Type annotations and code completion for `#!python ListImportFileTaskPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListImportFileTaskResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListImportFileTaskResponseTypeDef](./type_defs.md#listimportfiletaskresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListImportFileTaskRequestListImportFileTaskPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportFileTaskRequestListImportFileTaskPaginateTypeDef](./type_defs.md#listimportfiletaskrequestlistimportfiletaskpaginatetypedef) 
## ListServersPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("list_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListServers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListServersPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:
    client: MigrationHubStrategyRecommendationsClient
    paginator: ListServersPaginator = client.get_paginator("list_servers")
```


### paginate

Type annotations and code completion for `#!python ListServersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filterValue: str = ...,
    groupIdFilter: Sequence[GroupTypeDef] = ...,  # (1)
    serverCriteria: ServerCriteriaType = ...,  # (2)
    sort: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[ListServersResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-brackets: ServerCriteriaType](./literals.md#servercriteriatype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListServersResponseTypeDef](./type_defs.md#listserversresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListServersRequestListServersPaginateTypeDef = {  # (1)
    "filterValue": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServersRequestListServersPaginateTypeDef](./type_defs.md#listserversrequestlistserverspaginatetypedef) 
