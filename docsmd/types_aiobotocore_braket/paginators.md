# Paginators

> [Index](../README.md) > [Braket](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Braket](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#braket)
    type annotations stubs module [types-aiobotocore-braket](https://pypi.org/project/types-aiobotocore-braket/).

## SearchDevicesPaginator

Type annotations and code completion for `#!python session.create_client("braket").get_paginator("search_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket/paginator/SearchDevices.html#Braket.Paginator.SearchDevices)

```python
# SearchDevicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_braket.paginator import SearchDevicesPaginator

session = get_session()
async with session.create_client("braket") as client:  # (1)
    paginator: SearchDevicesPaginator = client.get_paginator("search_devices")  # (2)
    async for item in paginator.paginate(...):
        item: SearchDevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [BraketClient](./client.md)
2. paginator: [SearchDevicesPaginator](./paginators.md#searchdevicespaginator)
3. item: [:material-code-braces: SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchDevicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[SearchDevicesFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[SearchDevicesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchDevicesFilterTypeDef](./type_defs.md#searchdevicesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchDevicesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchDevicesRequestPaginateTypeDef](./type_defs.md#searchdevicesrequestpaginatetypedef) 
## SearchJobsPaginator

Type annotations and code completion for `#!python session.create_client("braket").get_paginator("search_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket/paginator/SearchJobs.html#Braket.Paginator.SearchJobs)

```python
# SearchJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_braket.paginator import SearchJobsPaginator

session = get_session()
async with session.create_client("braket") as client:  # (1)
    paginator: SearchJobsPaginator = client.get_paginator("search_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: SearchJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [BraketClient](./client.md)
2. paginator: [SearchJobsPaginator](./paginators.md#searchjobspaginator)
3. item: [:material-code-braces: SearchJobsResponseTypeDef](./type_defs.md#searchjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[SearchJobsFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[SearchJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchJobsFilterTypeDef](./type_defs.md#searchjobsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchJobsResponseTypeDef](./type_defs.md#searchjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchJobsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchJobsRequestPaginateTypeDef](./type_defs.md#searchjobsrequestpaginatetypedef) 
## SearchQuantumTasksPaginator

Type annotations and code completion for `#!python session.create_client("braket").get_paginator("search_quantum_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket/paginator/SearchQuantumTasks.html#Braket.Paginator.SearchQuantumTasks)

```python
# SearchQuantumTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_braket.paginator import SearchQuantumTasksPaginator

session = get_session()
async with session.create_client("braket") as client:  # (1)
    paginator: SearchQuantumTasksPaginator = client.get_paginator("search_quantum_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: SearchQuantumTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [BraketClient](./client.md)
2. paginator: [SearchQuantumTasksPaginator](./paginators.md#searchquantumtaskspaginator)
3. item: [:material-code-braces: SearchQuantumTasksResponseTypeDef](./type_defs.md#searchquantumtasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchQuantumTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[SearchQuantumTasksFilterTypeDef],  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[SearchQuantumTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchQuantumTasksFilterTypeDef](./type_defs.md#searchquantumtasksfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchQuantumTasksResponseTypeDef](./type_defs.md#searchquantumtasksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchQuantumTasksRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchQuantumTasksRequestPaginateTypeDef](./type_defs.md#searchquantumtasksrequestpaginatetypedef) 
