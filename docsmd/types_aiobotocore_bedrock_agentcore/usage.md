# Examples

> [Index](../README.md) > [BedrockAgentCore](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BedrockAgentCore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#bedrockagentcore)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore](https://pypi.org/project/types-aiobotocore-bedrock-agentcore/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bedrock-agentcore]` package installed.

Write your `BedrockAgentCore` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# BedrockAgentCoreClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-agentcore") as client:  # (1)
    result = await client.batch_create_memory_records()  # (2)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. result: [:material-code-braces: BatchCreateMemoryRecordsOutputTypeDef](./type_defs.md#batchcreatememoryrecordsoutputtypedef)



#### Paginator usage example

```python
# ListABTestsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-agentcore") as client:  # (1)
    paginator = client.get_paginator("list_ab_tests")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BedrockAgentCoreClient](./client.md)
2. paginator: [ListABTestsPaginator](./paginators.md#listabtestspaginator)
3. item: [:material-code-braces: ListABTestsResponseTypeDef](./type_defs.md#listabtestsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[bedrock-agentcore]`
or a standalone `types_aiobotocore_bedrock_agentcore` package, you have to explicitly specify
`client: BedrockAgentCoreClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# BedrockAgentCoreClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.client import BedrockAgentCoreClient
from types_aiobotocore_bedrock_agentcore.type_defs import BatchCreateMemoryRecordsOutputTypeDef
from types_aiobotocore_bedrock_agentcore.type_defs import BatchCreateMemoryRecordsInputTypeDef


session = get_session()

async with session.create_client("bedrock-agentcore") as client:
    client: BedrockAgentCoreClient
    kwargs: BatchCreateMemoryRecordsInputTypeDef = {...}
    result: BatchCreateMemoryRecordsOutputTypeDef = await client.batch_create_memory_records(**kwargs)
```



#### Paginator usage example

```python
# ListABTestsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore.client import BedrockAgentCoreClient
from types_aiobotocore_bedrock_agentcore.paginator import ListABTestsPaginator
from types_aiobotocore_bedrock_agentcore.type_defs import ListABTestsResponseTypeDef


session = get_session()

async with session.create_client("bedrock-agentcore") as client:
    client: BedrockAgentCoreClient
    paginator: ListABTestsPaginator = client.get_paginator("list_ab_tests")
    async for item in paginator.paginate(...):
        item: ListABTestsResponseTypeDef
        print(item)
```


