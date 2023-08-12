# Paginators

> [Index](../README.md) > [IoTRoboRunner](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTRoboRunner](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
    type annotations stubs module [types-aiobotocore-iot-roborunner](https://pypi.org/project/types-aiobotocore-iot-roborunner/).

## ListDestinationsPaginator

Type annotations and code completion for `#!python session.create_client("iot-roborunner").get_paginator("list_destinations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListDestinations)

```python
# ListDestinationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_roborunner.paginator import ListDestinationsPaginator

session = get_session()
async with session.create_client("iot-roborunner") as client:  # (1)
    paginator: ListDestinationsPaginator = client.get_paginator("list_destinations")  # (2)
    async for item in paginator.paginate(...):
        item: ListDestinationsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTRoboRunnerClient](./client.md)
2. paginator: [ListDestinationsPaginator](./paginators.md#listdestinationspaginator)
3. item: [:material-code-braces: ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDestinationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    site: str,
    state: DestinationStateType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDestinationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DestinationStateType](./literals.md#destinationstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDestinationsRequestListDestinationsPaginateTypeDef = {  # (1)
    "site": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDestinationsRequestListDestinationsPaginateTypeDef](./type_defs.md#listdestinationsrequestlistdestinationspaginatetypedef) 
## ListSitesPaginator

Type annotations and code completion for `#!python session.create_client("iot-roborunner").get_paginator("list_sites")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListSites)

```python
# ListSitesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_roborunner.paginator import ListSitesPaginator

session = get_session()
async with session.create_client("iot-roborunner") as client:  # (1)
    paginator: ListSitesPaginator = client.get_paginator("list_sites")  # (2)
    async for item in paginator.paginate(...):
        item: ListSitesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTRoboRunnerClient](./client.md)
2. paginator: [ListSitesPaginator](./paginators.md#listsitespaginator)
3. item: [:material-code-braces: ListSitesResponseTypeDef](./type_defs.md#listsitesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSitesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSitesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSitesResponseTypeDef](./type_defs.md#listsitesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSitesRequestListSitesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSitesRequestListSitesPaginateTypeDef](./type_defs.md#listsitesrequestlistsitespaginatetypedef) 
## ListWorkerFleetsPaginator

Type annotations and code completion for `#!python session.create_client("iot-roborunner").get_paginator("list_worker_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkerFleets)

```python
# ListWorkerFleetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_roborunner.paginator import ListWorkerFleetsPaginator

session = get_session()
async with session.create_client("iot-roborunner") as client:  # (1)
    paginator: ListWorkerFleetsPaginator = client.get_paginator("list_worker_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkerFleetsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTRoboRunnerClient](./client.md)
2. paginator: [ListWorkerFleetsPaginator](./paginators.md#listworkerfleetspaginator)
3. item: [:material-code-braces: ListWorkerFleetsResponseTypeDef](./type_defs.md#listworkerfleetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkerFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    site: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListWorkerFleetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkerFleetsResponseTypeDef](./type_defs.md#listworkerfleetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef = {  # (1)
    "site": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef](./type_defs.md#listworkerfleetsrequestlistworkerfleetspaginatetypedef) 
## ListWorkersPaginator

Type annotations and code completion for `#!python session.create_client("iot-roborunner").get_paginator("list_workers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Paginator.ListWorkers)

```python
# ListWorkersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_roborunner.paginator import ListWorkersPaginator

session = get_session()
async with session.create_client("iot-roborunner") as client:  # (1)
    paginator: ListWorkersPaginator = client.get_paginator("list_workers")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkersResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTRoboRunnerClient](./client.md)
2. paginator: [ListWorkersPaginator](./paginators.md#listworkerspaginator)
3. item: [:material-code-braces: ListWorkersResponseTypeDef](./type_defs.md#listworkersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    site: str,
    fleet: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListWorkersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListWorkersResponseTypeDef](./type_defs.md#listworkersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkersRequestListWorkersPaginateTypeDef = {  # (1)
    "site": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkersRequestListWorkersPaginateTypeDef](./type_defs.md#listworkersrequestlistworkerspaginatetypedef) 
