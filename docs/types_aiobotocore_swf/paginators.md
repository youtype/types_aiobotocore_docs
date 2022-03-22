<a id="paginators-for-aiobotocore-swf-module"></a>

# Paginators for aiobotocore SWF module

> [Index](../README.md) > [SWF](./README.md) > Paginators

Auto-generated documentation for
[SWF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
type annotations stubs module
[types-aiobotocore-swf](https://pypi.org/project/types-aiobotocore-swf/).

- [Paginators for aiobotocore SWF module](#paginators-for-aiobotocore-swf-module)
  - [GetWorkflowExecutionHistoryPaginator](#getworkflowexecutionhistorypaginator)
  - [ListActivityTypesPaginator](#listactivitytypespaginator)
  - [ListClosedWorkflowExecutionsPaginator](#listclosedworkflowexecutionspaginator)
  - [ListDomainsPaginator](#listdomainspaginator)
  - [ListOpenWorkflowExecutionsPaginator](#listopenworkflowexecutionspaginator)
  - [ListWorkflowTypesPaginator](#listworkflowtypespaginator)
  - [PollForDecisionTaskPaginator](#pollfordecisiontaskpaginator)

<a id="getworkflowexecutionhistorypaginator"></a>

## GetWorkflowExecutionHistoryPaginator

Type annotations for
`session.create_client("swf").get_paginator("get_workflow_execution_history")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import GetWorkflowExecutionHistoryPaginator

session = get_session()
async with session.create_client("swf") as client:
    client: SWFClient
    paginator: GetWorkflowExecutionHistoryPaginator = client.get_paginator("get_workflow_execution_history")
```

Boto3 documentation:
[SWF.Paginator.GetWorkflowExecutionHistory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.GetWorkflowExecutionHistory)

Arguments for `GetWorkflowExecutionHistoryPaginator.paginate` method:

- `domain`: `str` *(required)*
- `execution`:
  [WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef)
  *(required)*
- `reverseOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetWorkflowExecutionHistoryPaginator.paginate` returns
`AsyncIterator`\[[HistoryTypeDef](./type_defs.md#historytypedef)\].

<a id="listactivitytypespaginator"></a>

## ListActivityTypesPaginator

Type annotations for
`session.create_client("swf").get_paginator("list_activity_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import ListActivityTypesPaginator

session = get_session()
async with session.create_client("swf") as client:
    client: SWFClient
    paginator: ListActivityTypesPaginator = client.get_paginator("list_activity_types")
```

Boto3 documentation:
[SWF.Paginator.ListActivityTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListActivityTypes)

Arguments for `ListActivityTypesPaginator.paginate` method:

- `domain`: `str` *(required)*
- `registrationStatus`:
  [RegistrationStatusType](./literals.md#registrationstatustype) *(required)*
- `name`: `str`
- `reverseOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListActivityTypesPaginator.paginate` returns
`AsyncIterator`\[[ActivityTypeInfosTypeDef](./type_defs.md#activitytypeinfostypedef)\].

<a id="listclosedworkflowexecutionspaginator"></a>

## ListClosedWorkflowExecutionsPaginator

Type annotations for
`session.create_client("swf").get_paginator("list_closed_workflow_executions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import ListClosedWorkflowExecutionsPaginator

session = get_session()
async with session.create_client("swf") as client:
    client: SWFClient
    paginator: ListClosedWorkflowExecutionsPaginator = client.get_paginator("list_closed_workflow_executions")
```

Boto3 documentation:
[SWF.Paginator.ListClosedWorkflowExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListClosedWorkflowExecutions)

Arguments for `ListClosedWorkflowExecutionsPaginator.paginate` method:

- `domain`: `str` *(required)*
- `startTimeFilter`:
  [ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef)
- `closeTimeFilter`:
  [ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef)
- `executionFilter`:
  [WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef)
- `closeStatusFilter`:
  [CloseStatusFilterTypeDef](./type_defs.md#closestatusfiltertypedef)
- `typeFilter`:
  [WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef)
- `tagFilter`: [TagFilterTypeDef](./type_defs.md#tagfiltertypedef)
- `reverseOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListClosedWorkflowExecutionsPaginator.paginate` returns
`AsyncIterator`\[[WorkflowExecutionInfosTypeDef](./type_defs.md#workflowexecutioninfostypedef)\].

<a id="listdomainspaginator"></a>

## ListDomainsPaginator

Type annotations for
`session.create_client("swf").get_paginator("list_domains")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import ListDomainsPaginator

session = get_session()
async with session.create_client("swf") as client:
    client: SWFClient
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")
```

Boto3 documentation:
[SWF.Paginator.ListDomains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListDomains)

Arguments for `ListDomainsPaginator.paginate` method:

- `registrationStatus`:
  [RegistrationStatusType](./literals.md#registrationstatustype) *(required)*
- `reverseOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDomainsPaginator.paginate` returns
`AsyncIterator`\[[DomainInfosTypeDef](./type_defs.md#domaininfostypedef)\].

<a id="listopenworkflowexecutionspaginator"></a>

## ListOpenWorkflowExecutionsPaginator

Type annotations for
`session.create_client("swf").get_paginator("list_open_workflow_executions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import ListOpenWorkflowExecutionsPaginator

session = get_session()
async with session.create_client("swf") as client:
    client: SWFClient
    paginator: ListOpenWorkflowExecutionsPaginator = client.get_paginator("list_open_workflow_executions")
```

Boto3 documentation:
[SWF.Paginator.ListOpenWorkflowExecutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListOpenWorkflowExecutions)

Arguments for `ListOpenWorkflowExecutionsPaginator.paginate` method:

- `domain`: `str` *(required)*
- `startTimeFilter`:
  [ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef)
  *(required)*
- `typeFilter`:
  [WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef)
- `tagFilter`: [TagFilterTypeDef](./type_defs.md#tagfiltertypedef)
- `reverseOrder`: `bool`
- `executionFilter`:
  [WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOpenWorkflowExecutionsPaginator.paginate` returns
`AsyncIterator`\[[WorkflowExecutionInfosTypeDef](./type_defs.md#workflowexecutioninfostypedef)\].

<a id="listworkflowtypespaginator"></a>

## ListWorkflowTypesPaginator

Type annotations for
`session.create_client("swf").get_paginator("list_workflow_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import ListWorkflowTypesPaginator

session = get_session()
async with session.create_client("swf") as client:
    client: SWFClient
    paginator: ListWorkflowTypesPaginator = client.get_paginator("list_workflow_types")
```

Boto3 documentation:
[SWF.Paginator.ListWorkflowTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListWorkflowTypes)

Arguments for `ListWorkflowTypesPaginator.paginate` method:

- `domain`: `str` *(required)*
- `registrationStatus`:
  [RegistrationStatusType](./literals.md#registrationstatustype) *(required)*
- `name`: `str`
- `reverseOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListWorkflowTypesPaginator.paginate` returns
`AsyncIterator`\[[WorkflowTypeInfosTypeDef](./type_defs.md#workflowtypeinfostypedef)\].

<a id="pollfordecisiontaskpaginator"></a>

## PollForDecisionTaskPaginator

Type annotations for
`session.create_client("swf").get_paginator("poll_for_decision_task")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import PollForDecisionTaskPaginator

session = get_session()
async with session.create_client("swf") as client:
    client: SWFClient
    paginator: PollForDecisionTaskPaginator = client.get_paginator("poll_for_decision_task")
```

Boto3 documentation:
[SWF.Paginator.PollForDecisionTask](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.PollForDecisionTask)

Arguments for `PollForDecisionTaskPaginator.paginate` method:

- `domain`: `str` *(required)*
- `taskList`: [TaskListTypeDef](./type_defs.md#tasklisttypedef) *(required)*
- `identity`: `str`
- `reverseOrder`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`PollForDecisionTaskPaginator.paginate` returns
`AsyncIterator`\[[DecisionTaskTypeDef](./type_defs.md#decisiontasktypedef)\].
