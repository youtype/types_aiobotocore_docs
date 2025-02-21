# Examples

> [Index](../README.md) > [CodePipeline](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodePipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#codepipeline)
    type annotations stubs module [types-aiobotocore-codepipeline](https://pypi.org/project/types-aiobotocore-codepipeline/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[codepipeline]` package installed.

Write your `CodePipeline` code as usual,
type checking and code completion should work out of the box.



```python
# CodePipelineClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codepipeline") as client:  # (1)
    result = await client.acknowledge_job()  # (2)
```

1. client: [CodePipelineClient](./client.md)
2. result: [:material-code-braces: AcknowledgeJobOutputTypeDef](./type_defs.md#acknowledgejoboutputtypedef) 



```python
# ListActionExecutionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codepipeline") as client:  # (1)
    paginator = client.get_paginator("list_action_executions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodePipelineClient](./client.md)
2. paginator: [ListActionExecutionsPaginator](./paginators.md#listactionexecutionspaginator)
3. item: [:material-code-braces: ListActionExecutionsOutputTypeDef](./type_defs.md#listactionexecutionsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[codepipeline]`
or a standalone `types_aiobotocore_codepipeline` package, you have to explicitly specify
`client: CodePipelineClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CodePipelineClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.client import CodePipelineClient
from types_aiobotocore_codepipeline.type_defs import AcknowledgeJobOutputTypeDef
from types_aiobotocore_codepipeline.type_defs import AcknowledgeJobInputTypeDef


session = get_session()

async with session.create_client("codepipeline") as client:
    client: CodePipelineClient
    kwargs: AcknowledgeJobInputTypeDef = {...}
    result: AcknowledgeJobOutputTypeDef = await client.acknowledge_job(**kwargs)
```



```python
# ListActionExecutionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.client import CodePipelineClient
from types_aiobotocore_codepipeline.paginator import ListActionExecutionsPaginator
from types_aiobotocore_codepipeline.type_defs import ListActionExecutionsOutputTypeDef


session = get_session()

async with session.create_client("codepipeline") as client:
    client: CodePipelineClient
    paginator: ListActionExecutionsPaginator = client.get_paginator("list_action_executions")
    async for item in paginator.paginate(...):
        item: ListActionExecutionsOutputTypeDef
        print(item)
```


