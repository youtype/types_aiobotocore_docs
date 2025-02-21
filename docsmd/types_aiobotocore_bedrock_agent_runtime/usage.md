# Examples

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#agentsforbedrockruntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bedrock-agent-runtime]` package installed.

Write your `AgentsforBedrockRuntime` code as usual,
type checking and code completion should work out of the box.



```python
# AgentsforBedrockRuntimeClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-agent-runtime") as client:  # (1)
    result = await client.generate_query()  # (2)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. result: [:material-code-braces: GenerateQueryResponseTypeDef](./type_defs.md#generatequeryresponsetypedef) 



```python
# GetAgentMemoryPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-agent-runtime") as client:  # (1)
    paginator = client.get_paginator("get_agent_memory")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AgentsforBedrockRuntimeClient](./client.md)
2. paginator: [GetAgentMemoryPaginator](./paginators.md#getagentmemorypaginator)
3. item: [:material-code-braces: GetAgentMemoryResponseTypeDef](./type_defs.md#getagentmemoryresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[bedrock-agent-runtime]`
or a standalone `types_aiobotocore_bedrock_agent_runtime` package, you have to explicitly specify
`client: AgentsforBedrockRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AgentsforBedrockRuntimeClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient
from types_aiobotocore_bedrock_agent_runtime.type_defs import GenerateQueryResponseTypeDef
from types_aiobotocore_bedrock_agent_runtime.type_defs import GenerateQueryRequestTypeDef


session = get_session()

async with session.create_client("bedrock-agent-runtime") as client:
    client: AgentsforBedrockRuntimeClient
    kwargs: GenerateQueryRequestTypeDef = {...}
    result: GenerateQueryResponseTypeDef = await client.generate_query(**kwargs)
```



```python
# GetAgentMemoryPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient
from types_aiobotocore_bedrock_agent_runtime.paginator import GetAgentMemoryPaginator
from types_aiobotocore_bedrock_agent_runtime.type_defs import GetAgentMemoryResponseTypeDef


session = get_session()

async with session.create_client("bedrock-agent-runtime") as client:
    client: AgentsforBedrockRuntimeClient
    paginator: GetAgentMemoryPaginator = client.get_paginator("get_agent_memory")
    async for item in paginator.paginate(...):
        item: GetAgentMemoryResponseTypeDef
        print(item)
```


