# Examples

> [Index](../README.md) > [MWAAServerless](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MWAAServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa-serverless.html#mwaaserverless)
    type annotations stubs module [types-aiobotocore-mwaa-serverless](https://pypi.org/project/types-aiobotocore-mwaa-serverless/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[mwaa-serverless]` package installed.

Write your `MWAAServerless` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# MWAAServerlessClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mwaa-serverless") as client:  # (1)
    result = await client.create_workflow()  # (2)
```

1. client: [MWAAServerlessClient](./client.md)
2. result: [:material-code-braces: CreateWorkflowResponseTypeDef](./type_defs.md#createworkflowresponsetypedef)



#### Paginator usage example

```python
# ListTaskInstancesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("mwaa-serverless") as client:  # (1)
    paginator = client.get_paginator("list_task_instances")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MWAAServerlessClient](./client.md)
2. paginator: [ListTaskInstancesPaginator](./paginators.md#listtaskinstancespaginator)
3. item: [:material-code-braces: ListTaskInstancesResponseTypeDef](./type_defs.md#listtaskinstancesresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[mwaa-serverless]`
or a standalone `types_aiobotocore_mwaa_serverless` package, you have to explicitly specify
`client: MWAAServerlessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# MWAAServerlessClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mwaa_serverless.client import MWAAServerlessClient
from types_aiobotocore_mwaa_serverless.type_defs import CreateWorkflowResponseTypeDef
from types_aiobotocore_mwaa_serverless.type_defs import CreateWorkflowRequestTypeDef


session = get_session()

async with session.create_client("mwaa-serverless") as client:
    client: MWAAServerlessClient
    kwargs: CreateWorkflowRequestTypeDef = {...}
    result: CreateWorkflowResponseTypeDef = await client.create_workflow(**kwargs)
```



#### Paginator usage example

```python
# ListTaskInstancesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_mwaa_serverless.client import MWAAServerlessClient
from types_aiobotocore_mwaa_serverless.paginator import ListTaskInstancesPaginator
from types_aiobotocore_mwaa_serverless.type_defs import ListTaskInstancesResponseTypeDef


session = get_session()

async with session.create_client("mwaa-serverless") as client:
    client: MWAAServerlessClient
    paginator: ListTaskInstancesPaginator = client.get_paginator("list_task_instances")
    async for item in paginator.paginate(...):
        item: ListTaskInstancesResponseTypeDef
        print(item)
```


