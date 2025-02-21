# Examples

> [Index](../README.md) > [KendraRanking](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KendraRanking](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#kendraranking)
    type annotations stubs module [types-aiobotocore-kendra-ranking](https://pypi.org/project/types-aiobotocore-kendra-ranking/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kendra-ranking]` package installed.

Write your `KendraRanking` code as usual,
type checking and code completion should work out of the box.



```python
# KendraRankingClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kendra-ranking") as client:  # (1)
    result = await client.create_rescore_execution_plan()  # (2)
```

1. client: [KendraRankingClient](./client.md)
2. result: [:material-code-braces: CreateRescoreExecutionPlanResponseTypeDef](./type_defs.md#createrescoreexecutionplanresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[kendra-ranking]`
or a standalone `types_aiobotocore_kendra_ranking` package, you have to explicitly specify
`client: KendraRankingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KendraRankingClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kendra_ranking.client import KendraRankingClient
from types_aiobotocore_kendra_ranking.type_defs import CreateRescoreExecutionPlanResponseTypeDef
from types_aiobotocore_kendra_ranking.type_defs import CreateRescoreExecutionPlanRequestTypeDef


session = get_session()

async with session.create_client("kendra-ranking") as client:
    client: KendraRankingClient
    kwargs: CreateRescoreExecutionPlanRequestTypeDef = {...}
    result: CreateRescoreExecutionPlanResponseTypeDef = await client.create_rescore_execution_plan(**kwargs)
```




