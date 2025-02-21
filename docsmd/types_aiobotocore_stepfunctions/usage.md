# Examples

> [Index](../README.md) > [SFN](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SFN](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#sfn)
    type annotations stubs module [types-aiobotocore-stepfunctions](https://pypi.org/project/types-aiobotocore-stepfunctions/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[stepfunctions]` package installed.

Write your `SFN` code as usual,
type checking and code completion should work out of the box.



```python
# SFNClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("stepfunctions") as client:  # (1)
    result = await client.create_activity()  # (2)
```

1. client: [SFNClient](./client.md)
2. result: [:material-code-braces: CreateActivityOutputTypeDef](./type_defs.md#createactivityoutputtypedef) 



```python
# GetExecutionHistoryPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("stepfunctions") as client:  # (1)
    paginator = client.get_paginator("get_execution_history")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SFNClient](./client.md)
2. paginator: [GetExecutionHistoryPaginator](./paginators.md#getexecutionhistorypaginator)
3. item: [:material-code-braces: GetExecutionHistoryOutputTypeDef](./type_defs.md#getexecutionhistoryoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[stepfunctions]`
or a standalone `types_aiobotocore_stepfunctions` package, you have to explicitly specify
`client: SFNClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SFNClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_stepfunctions.client import SFNClient
from types_aiobotocore_stepfunctions.type_defs import CreateActivityOutputTypeDef
from types_aiobotocore_stepfunctions.type_defs import CreateActivityInputTypeDef


session = get_session()

async with session.create_client("stepfunctions") as client:
    client: SFNClient
    kwargs: CreateActivityInputTypeDef = {...}
    result: CreateActivityOutputTypeDef = await client.create_activity(**kwargs)
```



```python
# GetExecutionHistoryPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_stepfunctions.client import SFNClient
from types_aiobotocore_stepfunctions.paginator import GetExecutionHistoryPaginator
from types_aiobotocore_stepfunctions.type_defs import GetExecutionHistoryOutputTypeDef


session = get_session()

async with session.create_client("stepfunctions") as client:
    client: SFNClient
    paginator: GetExecutionHistoryPaginator = client.get_paginator("get_execution_history")
    async for item in paginator.paginate(...):
        item: GetExecutionHistoryOutputTypeDef
        print(item)
```


