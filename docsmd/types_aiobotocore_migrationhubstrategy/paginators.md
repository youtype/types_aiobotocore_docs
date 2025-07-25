# Paginators

> [Index](../README.md) > [MigrationHubStrategyRecommendations](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MigrationHubStrategyRecommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#migrationhubstrategyrecommendations)
    type annotations stubs module [types-aiobotocore-migrationhubstrategy](https://pypi.org/project/types-aiobotocore-migrationhubstrategy/).

## GetServerDetailsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("get_server_details")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy/paginator/GetServerDetails.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails)

```python
# GetServerDetailsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import GetServerDetailsPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:  # (1)
    paginator: GetServerDetailsPaginator = client.get_paginator("get_server_details")  # (2)
    async for item in paginator.paginate(...):
        item: GetServerDetailsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
2. paginator: [GetServerDetailsPaginator](./paginators.md#getserverdetailspaginator)
3. item: `AioPageIterator[GetServerDetailsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetServerDetailsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    serverId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetServerDetailsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetServerDetailsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetServerDetailsRequestPaginateTypeDef = {  # (1)
    "serverId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetServerDetailsRequestPaginateTypeDef](./type_defs.md#getserverdetailsrequestpaginatetypedef)
## ListAnalyzableServersPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("list_analyzable_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy/paginator/ListAnalyzableServers.html#MigrationHubStrategyRecommendations.Paginator.ListAnalyzableServers)

```python
# ListAnalyzableServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListAnalyzableServersPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:  # (1)
    paginator: ListAnalyzableServersPaginator = client.get_paginator("list_analyzable_servers")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnalyzableServersResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
2. paginator: [ListAnalyzableServersPaginator](./paginators.md#listanalyzableserverspaginator)
3. item: `AioPageIterator[ListAnalyzableServersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAnalyzableServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sort: SortOrderType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAnalyzableServersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAnalyzableServersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAnalyzableServersRequestPaginateTypeDef = {  # (1)
    "sort": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAnalyzableServersRequestPaginateTypeDef](./type_defs.md#listanalyzableserversrequestpaginatetypedef)
## ListApplicationComponentsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("list_application_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy/paginator/ListApplicationComponents.html#MigrationHubStrategyRecommendations.Paginator.ListApplicationComponents)

```python
# ListApplicationComponentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListApplicationComponentsPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:  # (1)
    paginator: ListApplicationComponentsPaginator = client.get_paginator("list_application_components")  # (2)
    async for item in paginator.paginate(...):
        item: ListApplicationComponentsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
2. paginator: [ListApplicationComponentsPaginator](./paginators.md#listapplicationcomponentspaginator)
3. item: `AioPageIterator[ListApplicationComponentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListApplicationComponentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    applicationComponentCriteria: ApplicationComponentCriteriaType = ...,  # (1)
    filterValue: str = ...,
    groupIdFilter: Sequence[GroupTypeDef] = ...,  # (2)
    sort: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListApplicationComponentsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ApplicationComponentCriteriaType](./literals.md#applicationcomponentcriteriatype)
2. See `Sequence[GroupTypeDef]`
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListApplicationComponentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListApplicationComponentsRequestPaginateTypeDef = {  # (1)
    "applicationComponentCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListApplicationComponentsRequestPaginateTypeDef](./type_defs.md#listapplicationcomponentsrequestpaginatetypedef)
## ListCollectorsPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("list_collectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy/paginator/ListCollectors.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors)

```python
# ListCollectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListCollectorsPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:  # (1)
    paginator: ListCollectorsPaginator = client.get_paginator("list_collectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListCollectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
2. paginator: [ListCollectorsPaginator](./paginators.md#listcollectorspaginator)
3. item: `AioPageIterator[ListCollectorsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCollectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCollectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCollectorsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCollectorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollectorsRequestPaginateTypeDef](./type_defs.md#listcollectorsrequestpaginatetypedef)
## ListImportFileTaskPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("list_import_file_task")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy/paginator/ListImportFileTask.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask)

```python
# ListImportFileTaskPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListImportFileTaskPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:  # (1)
    paginator: ListImportFileTaskPaginator = client.get_paginator("list_import_file_task")  # (2)
    async for item in paginator.paginate(...):
        item: ListImportFileTaskResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
2. paginator: [ListImportFileTaskPaginator](./paginators.md#listimportfiletaskpaginator)
3. item: `AioPageIterator[ListImportFileTaskResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListImportFileTaskPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListImportFileTaskResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListImportFileTaskResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListImportFileTaskRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImportFileTaskRequestPaginateTypeDef](./type_defs.md#listimportfiletaskrequestpaginatetypedef)
## ListServersPaginator

Type annotations and code completion for `#!python session.create_client("migrationhubstrategy").get_paginator("list_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy/paginator/ListServers.html#MigrationHubStrategyRecommendations.Paginator.ListServers)

```python
# ListServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_migrationhubstrategy.paginator import ListServersPaginator

session = get_session()
async with session.create_client("migrationhubstrategy") as client:  # (1)
    paginator: ListServersPaginator = client.get_paginator("list_servers")  # (2)
    async for item in paginator.paginate(...):
        item: ListServersResponseTypeDef
        print(item)  # (3)
```

1. client: [MigrationHubStrategyRecommendationsClient](./client.md)
2. paginator: [ListServersPaginator](./paginators.md#listserverspaginator)
3. item: `AioPageIterator[ListServersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterValue: str = ...,
    groupIdFilter: Sequence[GroupTypeDef] = ...,  # (1)
    serverCriteria: ServerCriteriaType = ...,  # (2)
    sort: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListServersResponseTypeDef]:  # (5)
    ...
```

1. See `Sequence[GroupTypeDef]`
2. See [:material-code-brackets: ServerCriteriaType](./literals.md#servercriteriatype)
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListServersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListServersRequestPaginateTypeDef = {  # (1)
    "filterValue": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServersRequestPaginateTypeDef](./type_defs.md#listserversrequestpaginatetypedef)
