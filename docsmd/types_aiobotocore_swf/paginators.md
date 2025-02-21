# Paginators

> [Index](../README.md) > [SWF](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SWF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#swf)
    type annotations stubs module [types-aiobotocore-swf](https://pypi.org/project/types-aiobotocore-swf/).

## GetWorkflowExecutionHistoryPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("get_workflow_execution_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf/paginator/GetWorkflowExecutionHistory.html#SWF.Paginator.GetWorkflowExecutionHistory)

```python
# GetWorkflowExecutionHistoryPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    domain: str,
    execution: WorkflowExecutionTypeDef,  # (1)
    reverseOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[HistoryTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: WorkflowExecutionTypeDef](./type_defs.md#workflowexecutiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: HistoryTypeDef](./type_defs.md#historytypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetWorkflowExecutionHistoryInputPaginateTypeDef = {  # (1)
    "domain": ...,
    "execution": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetWorkflowExecutionHistoryInputPaginateTypeDef](./type_defs.md#getworkflowexecutionhistoryinputpaginatetypedef) 
## ListActivityTypesPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("list_activity_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf/paginator/ListActivityTypes.html#SWF.Paginator.ListActivityTypes)

```python
# ListActivityTypesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    domain: str,
    registrationStatus: RegistrationStatusType,  # (1)
    name: str = ...,
    reverseOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ActivityTypeInfosTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ActivityTypeInfosTypeDef](./type_defs.md#activitytypeinfostypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListActivityTypesInputPaginateTypeDef = {  # (1)
    "domain": ...,
    "registrationStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActivityTypesInputPaginateTypeDef](./type_defs.md#listactivitytypesinputpaginatetypedef) 
## ListClosedWorkflowExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("list_closed_workflow_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf/paginator/ListClosedWorkflowExecutions.html#SWF.Paginator.ListClosedWorkflowExecutions)

```python
# ListClosedWorkflowExecutionsPaginator usage example

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

```python
# paginate method definition

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
) -> AioPageIterator[WorkflowExecutionInfosTypeDef]:  # (8)
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


```python
# paginate method usage example with argument unpacking

kwargs: ListClosedWorkflowExecutionsInputPaginateTypeDef = {  # (1)
    "domain": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClosedWorkflowExecutionsInputPaginateTypeDef](./type_defs.md#listclosedworkflowexecutionsinputpaginatetypedef) 
## ListDomainsPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("list_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf/paginator/ListDomains.html#SWF.Paginator.ListDomains)

```python
# ListDomainsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    registrationStatus: RegistrationStatusType,  # (1)
    reverseOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DomainInfosTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DomainInfosTypeDef](./type_defs.md#domaininfostypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainsInputPaginateTypeDef = {  # (1)
    "registrationStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainsInputPaginateTypeDef](./type_defs.md#listdomainsinputpaginatetypedef) 
## ListOpenWorkflowExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("list_open_workflow_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf/paginator/ListOpenWorkflowExecutions.html#SWF.Paginator.ListOpenWorkflowExecutions)

```python
# ListOpenWorkflowExecutionsPaginator usage example

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

```python
# paginate method definition

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
) -> AioPageIterator[WorkflowExecutionInfosTypeDef]:  # (6)
    ...
```

1. See [:material-code-braces: ExecutionTimeFilterTypeDef](./type_defs.md#executiontimefiltertypedef) 
2. See [:material-code-braces: WorkflowTypeFilterTypeDef](./type_defs.md#workflowtypefiltertypedef) 
3. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
4. See [:material-code-braces: WorkflowExecutionFilterTypeDef](./type_defs.md#workflowexecutionfiltertypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: WorkflowExecutionInfosTypeDef](./type_defs.md#workflowexecutioninfostypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOpenWorkflowExecutionsInputPaginateTypeDef = {  # (1)
    "domain": ...,
    "startTimeFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOpenWorkflowExecutionsInputPaginateTypeDef](./type_defs.md#listopenworkflowexecutionsinputpaginatetypedef) 
## ListWorkflowTypesPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("list_workflow_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf/paginator/ListWorkflowTypes.html#SWF.Paginator.ListWorkflowTypes)

```python
# ListWorkflowTypesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    domain: str,
    registrationStatus: RegistrationStatusType,  # (1)
    name: str = ...,
    reverseOrder: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[WorkflowTypeInfosTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: WorkflowTypeInfosTypeDef](./type_defs.md#workflowtypeinfostypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkflowTypesInputPaginateTypeDef = {  # (1)
    "domain": ...,
    "registrationStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkflowTypesInputPaginateTypeDef](./type_defs.md#listworkflowtypesinputpaginatetypedef) 
## PollForDecisionTaskPaginator

Type annotations and code completion for `#!python session.create_client("swf").get_paginator("poll_for_decision_task")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf/paginator/PollForDecisionTask.html#SWF.Paginator.PollForDecisionTask)

```python
# PollForDecisionTaskPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    domain: str,
    taskList: TaskListTypeDef,  # (1)
    identity: str = ...,
    reverseOrder: bool = ...,
    startAtPreviousStartedEvent: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DecisionTaskTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: TaskListTypeDef](./type_defs.md#tasklisttypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DecisionTaskTypeDef](./type_defs.md#decisiontasktypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: PollForDecisionTaskInputPaginateTypeDef = {  # (1)
    "domain": ...,
    "taskList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: PollForDecisionTaskInputPaginateTypeDef](./type_defs.md#pollfordecisiontaskinputpaginatetypedef) 
