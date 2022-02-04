<a id="paginators-for-aiobotocore-sfn-module"></a>

# Paginators for aiobotocore SFN module

> [Index](..) > [SFN](.) > Paginators

Auto-generated documentation for
[SFN](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
type annotations stubs module
[types-aiobotocore-stepfunctions](https://pypi.org/project/types-aiobotocore-stepfunctions/).

- [Paginators for aiobotocore SFN module](#paginators-for-aiobotocore-sfn-module)
  - [GetExecutionHistoryPaginator](#getexecutionhistorypaginator)
  - [ListActivitiesPaginator](#listactivitiespaginator)
  - [ListExecutionsPaginator](#listexecutionspaginator)
  - [ListStateMachinesPaginator](#liststatemachinespaginator)

<a id="getexecutionhistorypaginator"></a>

## GetExecutionHistoryPaginator

Type annotations for
`aiobotocore.create_client("stepfunctions").get_paginator("get_execution_history")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_stepfunctions.paginator import GetExecutionHistoryPaginator

def get_get_execution_history_paginator() -> GetExecutionHistoryPaginator:
    return Session().create_client("stepfunctions").get_paginator("get_execution_history")
```

Boto3 documentation:
[SFN.Paginator.GetExecutionHistory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory)

Arguments for `GetExecutionHistoryPaginator.paginate` method:

- `executionArn`: `str` *(required)*
- `reverseOrder`: `bool`
- `includeExecutionData`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetExecutionHistoryPaginator.paginate` returns
`_PageIterator`\[[GetExecutionHistoryOutputTypeDef](./type_defs.md#getexecutionhistoryoutputtypedef)\].

<a id="listactivitiespaginator"></a>

## ListActivitiesPaginator

Type annotations for
`aiobotocore.create_client("stepfunctions").get_paginator("list_activities")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_stepfunctions.paginator import ListActivitiesPaginator

def get_list_activities_paginator() -> ListActivitiesPaginator:
    return Session().create_client("stepfunctions").get_paginator("list_activities")
```

Boto3 documentation:
[SFN.Paginator.ListActivities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListActivities)

Arguments for `ListActivitiesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListActivitiesPaginator.paginate` returns
`_PageIterator`\[[ListActivitiesOutputTypeDef](./type_defs.md#listactivitiesoutputtypedef)\].

<a id="listexecutionspaginator"></a>

## ListExecutionsPaginator

Type annotations for
`aiobotocore.create_client("stepfunctions").get_paginator("list_executions")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_stepfunctions.paginator import ListExecutionsPaginator

def get_list_executions_paginator() -> ListExecutionsPaginator:
    return Session().create_client("stepfunctions").get_paginator("list_executions")
```

Boto3 documentation:
[SFN.Paginator.ListExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions)

Arguments for `ListExecutionsPaginator.paginate` method:

- `stateMachineArn`: `str` *(required)*
- `statusFilter`: [ExecutionStatusType](./literals.md#executionstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListExecutionsPaginator.paginate` returns
`_PageIterator`\[[ListExecutionsOutputTypeDef](./type_defs.md#listexecutionsoutputtypedef)\].

<a id="liststatemachinespaginator"></a>

## ListStateMachinesPaginator

Type annotations for
`aiobotocore.create_client("stepfunctions").get_paginator("list_state_machines")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_stepfunctions.paginator import ListStateMachinesPaginator

def get_list_state_machines_paginator() -> ListStateMachinesPaginator:
    return Session().create_client("stepfunctions").get_paginator("list_state_machines")
```

Boto3 documentation:
[SFN.Paginator.ListStateMachines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListStateMachines)

Arguments for `ListStateMachinesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListStateMachinesPaginator.paginate` returns
`_PageIterator`\[[ListStateMachinesOutputTypeDef](./type_defs.md#liststatemachinesoutputtypedef)\].
