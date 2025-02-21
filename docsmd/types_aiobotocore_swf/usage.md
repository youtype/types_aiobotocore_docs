# Examples

> [Index](../README.md) > [SWF](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SWF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#swf)
    type annotations stubs module [types-aiobotocore-swf](https://pypi.org/project/types-aiobotocore-swf/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[swf]` package installed.

Write your `SWF` code as usual,
type checking and code completion should work out of the box.



```python
# SWFClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("swf") as client:  # (1)
    result = await client.count_closed_workflow_executions()  # (2)
```

1. client: [SWFClient](./client.md)
2. result: [:material-code-braces: WorkflowExecutionCountTypeDef](./type_defs.md#workflowexecutioncounttypedef) 



```python
# GetWorkflowExecutionHistoryPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("swf") as client:  # (1)
    paginator = client.get_paginator("get_workflow_execution_history")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SWFClient](./client.md)
2. paginator: [GetWorkflowExecutionHistoryPaginator](./paginators.md#getworkflowexecutionhistorypaginator)
3. item: [:material-code-braces: HistoryTypeDef](./type_defs.md#historytypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[swf]`
or a standalone `types_aiobotocore_swf` package, you have to explicitly specify
`client: SWFClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SWFClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_swf.client import SWFClient
from types_aiobotocore_swf.type_defs import WorkflowExecutionCountTypeDef
from types_aiobotocore_swf.type_defs import CountClosedWorkflowExecutionsInputTypeDef


session = get_session()

async with session.create_client("swf") as client:
    client: SWFClient
    kwargs: CountClosedWorkflowExecutionsInputTypeDef = {...}
    result: WorkflowExecutionCountTypeDef = await client.count_closed_workflow_executions(**kwargs)
```



```python
# GetWorkflowExecutionHistoryPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_swf.client import SWFClient
from types_aiobotocore_swf.paginator import GetWorkflowExecutionHistoryPaginator
from types_aiobotocore_swf.type_defs import HistoryTypeDef


session = get_session()

async with session.create_client("swf") as client:
    client: SWFClient
    paginator: GetWorkflowExecutionHistoryPaginator = client.get_paginator("get_workflow_execution_history")
    async for item in paginator.paginate(...):
        item: HistoryTypeDef
        print(item)
```


