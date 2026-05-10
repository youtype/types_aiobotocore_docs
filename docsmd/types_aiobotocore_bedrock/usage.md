# Examples

> [Index](../README.md) > [Bedrock](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bedrock]` package installed.

Write your `Bedrock` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# BedrockClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock") as client:  # (1)
    result = await client.batch_delete_evaluation_job()  # (2)
```

1. client: [BedrockClient](./client.md)
2. result: [:material-code-braces: BatchDeleteEvaluationJobResponseTypeDef](./type_defs.md#batchdeleteevaluationjobresponsetypedef)



#### Paginator usage example

```python
# ListAutomatedReasoningPoliciesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock") as client:  # (1)
    paginator = client.get_paginator("list_automated_reasoning_policies")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BedrockClient](./client.md)
2. paginator: [ListAutomatedReasoningPoliciesPaginator](./paginators.md#listautomatedreasoningpoliciespaginator)
3. item: [:material-code-braces: ListAutomatedReasoningPoliciesResponseTypeDef](./type_defs.md#listautomatedreasoningpoliciesresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[bedrock]`
or a standalone `types_aiobotocore_bedrock` package, you have to explicitly specify
`client: BedrockClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# BedrockClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.client import BedrockClient
from types_aiobotocore_bedrock.type_defs import BatchDeleteEvaluationJobResponseTypeDef
from types_aiobotocore_bedrock.type_defs import BatchDeleteEvaluationJobRequestTypeDef


session = get_session()

async with session.create_client("bedrock") as client:
    client: BedrockClient
    kwargs: BatchDeleteEvaluationJobRequestTypeDef = {...}
    result: BatchDeleteEvaluationJobResponseTypeDef = await client.batch_delete_evaluation_job(**kwargs)
```



#### Paginator usage example

```python
# ListAutomatedReasoningPoliciesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock.client import BedrockClient
from types_aiobotocore_bedrock.paginator import ListAutomatedReasoningPoliciesPaginator
from types_aiobotocore_bedrock.type_defs import ListAutomatedReasoningPoliciesResponseTypeDef


session = get_session()

async with session.create_client("bedrock") as client:
    client: BedrockClient
    paginator: ListAutomatedReasoningPoliciesPaginator = client.get_paginator("list_automated_reasoning_policies")
    async for item in paginator.paginate(...):
        item: ListAutomatedReasoningPoliciesResponseTypeDef
        print(item)
```


