# Paginators

> [Index](../README.md) > [SFN](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SFN](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
    type annotations stubs module [types-aiobotocore-stepfunctions](https://pypi.org/project/types-aiobotocore-stepfunctions/).

## GetExecutionHistoryPaginator

Type annotations and code completion for `#!python session.create_client("stepfunctions").get_paginator("get_execution_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory)

```python
# GetExecutionHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_stepfunctions.paginator import GetExecutionHistoryPaginator

session = get_session()
async with session.create_client("stepfunctions") as client:  # (1)
    paginator: GetExecutionHistoryPaginator = client.get_paginator("get_execution_history")  # (2)
    async for item in paginator.paginate(...):
        item: GetExecutionHistoryOutputTypeDef
        print(item)  # (3)
```

1. client: [SFNClient](./client.md)
2. paginator: [GetExecutionHistoryPaginator](./paginators.md#getexecutionhistorypaginator)
3. item: [:material-code-braces: GetExecutionHistoryOutputTypeDef](./type_defs.md#getexecutionhistoryoutputtypedef) 


### paginate

Type annotations and code completion for `#!python GetExecutionHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    executionArn: str,
    reverseOrder: bool = ...,
    includeExecutionData: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetExecutionHistoryOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetExecutionHistoryOutputTypeDef](./type_defs.md#getexecutionhistoryoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef = {  # (1)
    "executionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef](./type_defs.md#getexecutionhistoryinputgetexecutionhistorypaginatetypedef) 
## ListActivitiesPaginator

Type annotations and code completion for `#!python session.create_client("stepfunctions").get_paginator("list_activities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities)

```python
# ListActivitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_stepfunctions.paginator import ListActivitiesPaginator

session = get_session()
async with session.create_client("stepfunctions") as client:  # (1)
    paginator: ListActivitiesPaginator = client.get_paginator("list_activities")  # (2)
    async for item in paginator.paginate(...):
        item: ListActivitiesOutputTypeDef
        print(item)  # (3)
```

1. client: [SFNClient](./client.md)
2. paginator: [ListActivitiesPaginator](./paginators.md#listactivitiespaginator)
3. item: [:material-code-braces: ListActivitiesOutputTypeDef](./type_defs.md#listactivitiesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListActivitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListActivitiesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListActivitiesOutputTypeDef](./type_defs.md#listactivitiesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListActivitiesInputListActivitiesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActivitiesInputListActivitiesPaginateTypeDef](./type_defs.md#listactivitiesinputlistactivitiespaginatetypedef) 
## ListExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("stepfunctions").get_paginator("list_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions)

```python
# ListExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_stepfunctions.paginator import ListExecutionsPaginator

session = get_session()
async with session.create_client("stepfunctions") as client:  # (1)
    paginator: ListExecutionsPaginator = client.get_paginator("list_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListExecutionsOutputTypeDef
        print(item)  # (3)
```

1. client: [SFNClient](./client.md)
2. paginator: [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
3. item: [:material-code-braces: ListExecutionsOutputTypeDef](./type_defs.md#listexecutionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    stateMachineArn: str = ...,
    statusFilter: ExecutionStatusType = ...,  # (1)
    mapRunArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListExecutionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListExecutionsOutputTypeDef](./type_defs.md#listexecutionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExecutionsInputListExecutionsPaginateTypeDef = {  # (1)
    "stateMachineArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExecutionsInputListExecutionsPaginateTypeDef](./type_defs.md#listexecutionsinputlistexecutionspaginatetypedef) 
## ListMapRunsPaginator

Type annotations and code completion for `#!python session.create_client("stepfunctions").get_paginator("list_map_runs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListMapRuns)

```python
# ListMapRunsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_stepfunctions.paginator import ListMapRunsPaginator

session = get_session()
async with session.create_client("stepfunctions") as client:  # (1)
    paginator: ListMapRunsPaginator = client.get_paginator("list_map_runs")  # (2)
    async for item in paginator.paginate(...):
        item: ListMapRunsOutputTypeDef
        print(item)  # (3)
```

1. client: [SFNClient](./client.md)
2. paginator: [ListMapRunsPaginator](./paginators.md#listmaprunspaginator)
3. item: [:material-code-braces: ListMapRunsOutputTypeDef](./type_defs.md#listmaprunsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListMapRunsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    executionArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMapRunsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMapRunsOutputTypeDef](./type_defs.md#listmaprunsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMapRunsInputListMapRunsPaginateTypeDef = {  # (1)
    "executionArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMapRunsInputListMapRunsPaginateTypeDef](./type_defs.md#listmaprunsinputlistmaprunspaginatetypedef) 
## ListStateMachinesPaginator

Type annotations and code completion for `#!python session.create_client("stepfunctions").get_paginator("list_state_machines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines)

```python
# ListStateMachinesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_stepfunctions.paginator import ListStateMachinesPaginator

session = get_session()
async with session.create_client("stepfunctions") as client:  # (1)
    paginator: ListStateMachinesPaginator = client.get_paginator("list_state_machines")  # (2)
    async for item in paginator.paginate(...):
        item: ListStateMachinesOutputTypeDef
        print(item)  # (3)
```

1. client: [SFNClient](./client.md)
2. paginator: [ListStateMachinesPaginator](./paginators.md#liststatemachinespaginator)
3. item: [:material-code-braces: ListStateMachinesOutputTypeDef](./type_defs.md#liststatemachinesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListStateMachinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStateMachinesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStateMachinesOutputTypeDef](./type_defs.md#liststatemachinesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListStateMachinesInputListStateMachinesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStateMachinesInputListStateMachinesPaginateTypeDef](./type_defs.md#liststatemachinesinputliststatemachinespaginatetypedef) 
