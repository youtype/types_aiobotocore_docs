<a id="examples-for-aiobotocore-codepipeline-module"></a>

# Examples for aiobotocore CodePipeline module

> [Index](../README.md) > [CodePipeline](./README.md) > Examples

- [Examples for aiobotocore CodePipeline module](#examples-for-aiobotocore-codepipeline-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[codepipeline]` package installed.

Write your `CodePipeline` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CodePipelineClient
# and provides type checking and code completion
async with session.create_client("codepipeline") as client:
    
    # result has type AcknowledgeJobOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.acknowledge_job()
    

    
    # paginator has type ListActionExecutionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_action_executions")
    async for item in paginator.paginate(...):
        # item has type ListActionExecutionsOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[codepipeline]` or a standalone
`types_aiobotocore_codepipeline` package, you have to explicitly specify
`client: CodePipelineClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_codepipeline.client import CodePipelineClient
from types_aiobotocore_codepipeline.type_defs import AcknowledgeJobOutputTypeDef
from types_aiobotocore_codepipeline.paginator import ListActionExecutionsPaginator

from types_aiobotocore_codepipeline.literals import PaginatorName



session = get_session()

async with session.create_client("codepipeline") as client:
    client: CodePipelineClient

    
    result: AcknowledgeJobOutputTypeDef = client.acknowledge_job()
    

    
    paginator_name: PaginatorName = "list_action_executions"
    paginator: ListActionExecutionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListActionExecutionsOutputTypeDef
        print(item)
    

    
```
