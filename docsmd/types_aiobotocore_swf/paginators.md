# Paginators

> [Index](../README.md) > [SWF](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SWF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF)
    type annotations stubs module [types-aiobotocore-swf](https://pypi.org/project/types-aiobotocore-swf/).

## GetWorkflowExecutionHistoryPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("get_workflow_execution_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.GetWorkflowExecutionHistory)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import GetWorkflowExecutionHistoryPaginator

session = get_session()
async with session.create_client("swf") as client:  # (1)
    paginator: GetWorkflowExecutionHistoryPaginator = client.get_paginator("get_workflow_execution_history")  # (2)
    async for item in paginator.paginate(...):
        item: HistoryTypeDef
        print(item)  # (3)
```

1. client: [SWFClient](./client.md)
2. paginator: [GetWorkflowExecutionHistoryPaginator](./paginators.md#getworkflowexecutionhistorypaginator)
3. item: [:material-code-braces: HistoryTypeDef](./type_defs.md#historytypedef) 


### paginate

Type annotations and code completion for `#!python GetWorkflowExecutionHistoryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    domain: str,
    execution: WorkflowExecutionTypeDef,  # (1)
    reverseOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[HistoryTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: HistoryTypeDef](./type_defs.md#historytypedef) 


```python title="Usage example with kwargs"
kwargs: GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef = {  # (1)
    "domain": ...,
    "execution": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetWorkflowExecutionHistoryInputGetWorkflowExecutionHistoryPaginateTypeDef](./type_defs.md#getworkflowexecutionhistoryinputgetworkflowexecutionhistorypaginatetypedef) 
## ListActivityTypesPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("list_activity_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListActivityTypes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import ListActivityTypesPaginator

session = get_session()
async with session.create_client("swf") as client:  # (1)
    paginator: ListActivityTypesPaginator = client.get_paginator("list_activity_types")  # (2)
    async for item in paginator.paginate(...):
        item: ActivityTypeInfosTypeDef
        print(item)  # (3)
```

1. client: [SWFClient](./client.md)
2. paginator: [ListActivityTypesPaginator](./paginators.md#listactivitytypespaginator)
3. item: [:material-code-braces: ActivityTypeInfosTypeDef](./type_defs.md#activitytypeinfostypedef) 


### paginate

Type annotations and code completion for `#!python ListActivityTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    domain: str,
    registrationStatus: RegistrationStatusType,  # (1)
    name: str = ...,
    reverseOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ActivityTypeInfosTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ActivityTypeInfosTypeDef](./type_defs.md#activitytypeinfostypedef) 


```python title="Usage example with kwargs"
kwargs: ListActivityTypesInputListActivityTypesPaginateTypeDef = {  # (1)
    "domain": ...,
    "registrationStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActivityTypesInputListActivityTypesPaginateTypeDef](./type_defs.md#listactivitytypesinputlistactivitytypespaginatetypedef) 
## ListClosedWorkflowExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("list_closed_workflow_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListClosedWorkflowExecutions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import ListClosedWorkflowExecutionsPaginator

session = get_session()
async with session.create_client("swf") as client:  # (1)
    paginator: ListClosedWorkflowExecutionsPaginator = client.get_paginator("list_closed_workflow_executions")  # (2)
    async for item in paginator.paginate(...):
        item: WorkflowExecutionInfosTypeDef
        print(item)  # (3)
```

1. client: [SWFClient](./client.md)
2. paginator: [ListClosedWorkflowExecutionsPaginator](./paginators.md#listclosedworkflowexecutionspaginator)
3. item: [:material-code-braces: WorkflowExecutionInfosTypeDef](./type_defs.md#workflowexecutioninfostypedef) 


### paginate

Type annotations and code completion for `#!python ListClosedWorkflowExecutionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    domain: str,
    startTimeFilter: ExecutionTimeFilterTypeDef = ...,  # (1)
    closeTimeFilter: ExecutionTimeFilterTypeDef = ...,  # (1)
    executionFilter: WorkflowExecutionFilterTypeDef = ...,  # (3)
    closeStatusFilter: CloseStatusFilterTypeDef = ...,  # (4)
    typeFilter: WorkflowTypeFilterTypeDef = ...,  # (5)
    tagFilter: TagFilterTypeDef = ...,  # (6)
    reverseOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (7)
) -> AsyncIterator[WorkflowExecutionInfosTypeDef]:  # (8)
    ...
```

1. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
2. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
3. See [:material-code-braces: WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef) 
4. See [:material-code-braces: CloseStatusFilterTypeDef](./type_defs.md#closestatusfiltertypedef) 
5. See [:material-code-braces: WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef) 
6. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
7. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
8. See [:material-code-braces: WorkflowExecutionInfosTypeDef](./type_defs.md#workflowexecutioninfostypedef) 


```python title="Usage example with kwargs"
kwargs: ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef = {  # (1)
    "domain": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClosedWorkflowExecutionsInputListClosedWorkflowExecutionsPaginateTypeDef](./type_defs.md#listclosedworkflowexecutionsinputlistclosedworkflowexecutionspaginatetypedef) 
## ListDomainsPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("list_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListDomains)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import ListDomainsPaginator

session = get_session()
async with session.create_client("swf") as client:  # (1)
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        item: DomainInfosTypeDef
        print(item)  # (3)
```

1. client: [SWFClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: DomainInfosTypeDef](./type_defs.md#domaininfostypedef) 


### paginate

Type annotations and code completion for `#!python ListDomainsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    registrationStatus: RegistrationStatusType,  # (1)
    reverseOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DomainInfosTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DomainInfosTypeDef](./type_defs.md#domaininfostypedef) 


```python title="Usage example with kwargs"
kwargs: ListDomainsInputListDomainsPaginateTypeDef = {  # (1)
    "registrationStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainsInputListDomainsPaginateTypeDef](./type_defs.md#listdomainsinputlistdomainspaginatetypedef) 
## ListOpenWorkflowExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("list_open_workflow_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListOpenWorkflowExecutions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import ListOpenWorkflowExecutionsPaginator

session = get_session()
async with session.create_client("swf") as client:  # (1)
    paginator: ListOpenWorkflowExecutionsPaginator = client.get_paginator("list_open_workflow_executions")  # (2)
    async for item in paginator.paginate(...):
        item: WorkflowExecutionInfosTypeDef
        print(item)  # (3)
```

1. client: [SWFClient](./client.md)
2. paginator: [ListOpenWorkflowExecutionsPaginator](./paginators.md#listopenworkflowexecutionspaginator)
3. item: [:material-code-braces: WorkflowExecutionInfosTypeDef](./type_defs.md#workflowexecutioninfostypedef) 


### paginate

Type annotations and code completion for `#!python ListOpenWorkflowExecutionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    domain: str,
    startTimeFilter: ExecutionTimeFilterTypeDef,  # (1)
    typeFilter: WorkflowTypeFilterTypeDef = ...,  # (2)
    tagFilter: TagFilterTypeDef = ...,  # (3)
    reverseOrder: bool = ...,
    executionFilter: WorkflowExecutionFilterTypeDef = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AsyncIterator[WorkflowExecutionInfosTypeDef]:  # (6)
    ...
```

1. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
2. See [:material-code-braces: WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef) 
3. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
4. See [:material-code-braces: WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: WorkflowExecutionInfosTypeDef](./type_defs.md#workflowexecutioninfostypedef) 


```python title="Usage example with kwargs"
kwargs: ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef = {  # (1)
    "domain": ...,
    "startTimeFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOpenWorkflowExecutionsInputListOpenWorkflowExecutionsPaginateTypeDef](./type_defs.md#listopenworkflowexecutionsinputlistopenworkflowexecutionspaginatetypedef) 
## ListWorkflowTypesPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("list_workflow_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.ListWorkflowTypes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import ListWorkflowTypesPaginator

session = get_session()
async with session.create_client("swf") as client:  # (1)
    paginator: ListWorkflowTypesPaginator = client.get_paginator("list_workflow_types")  # (2)
    async for item in paginator.paginate(...):
        item: WorkflowTypeInfosTypeDef
        print(item)  # (3)
```

1. client: [SWFClient](./client.md)
2. paginator: [ListWorkflowTypesPaginator](./paginators.md#listworkflowtypespaginator)
3. item: [:material-code-braces: WorkflowTypeInfosTypeDef](./type_defs.md#workflowtypeinfostypedef) 


### paginate

Type annotations and code completion for `#!python ListWorkflowTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    domain: str,
    registrationStatus: RegistrationStatusType,  # (1)
    name: str = ...,
    reverseOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[WorkflowTypeInfosTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: WorkflowTypeInfosTypeDef](./type_defs.md#workflowtypeinfostypedef) 


```python title="Usage example with kwargs"
kwargs: ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef = {  # (1)
    "domain": ...,
    "registrationStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowTypesInputListWorkflowTypesPaginateTypeDef](./type_defs.md#listworkflowtypesinputlistworkflowtypespaginatetypedef) 
## PollForDecisionTaskPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("poll_for_decision_task")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#SWF.Paginator.PollForDecisionTask)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_swf.paginator import PollForDecisionTaskPaginator

session = get_session()
async with session.create_client("swf") as client:  # (1)
    paginator: PollForDecisionTaskPaginator = client.get_paginator("poll_for_decision_task")  # (2)
    async for item in paginator.paginate(...):
        item: DecisionTaskTypeDef
        print(item)  # (3)
```

1. client: [SWFClient](./client.md)
2. paginator: [PollForDecisionTaskPaginator](./paginators.md#pollfordecisiontaskpaginator)
3. item: [:material-code-braces: DecisionTaskTypeDef](./type_defs.md#decisiontasktypedef) 


### paginate

Type annotations and code completion for `#!python PollForDecisionTaskPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    domain: str,
    taskList: TaskListTypeDef,  # (1)
    identity: str = ...,
    reverseOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DecisionTaskTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DecisionTaskTypeDef](./type_defs.md#decisiontasktypedef) 


```python title="Usage example with kwargs"
kwargs: PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef = {  # (1)
    "domain": ...,
    "taskList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: PollForDecisionTaskInputPollForDecisionTaskPaginateTypeDef](./type_defs.md#pollfordecisiontaskinputpollfordecisiontaskpaginatetypedef) 
