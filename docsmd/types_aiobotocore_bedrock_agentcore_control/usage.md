# Examples

> [Index](../README.md) > [BedrockAgentCoreControl](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BedrockAgentCoreControl](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#bedrockagentcorecontrol)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore-control](https://pypi.org/project/types-aiobotocore-bedrock-agentcore-control/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bedrock-agentcore-control]` package installed.

Write your `BedrockAgentCoreControl` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# BedrockAgentCoreControlClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-agentcore-control") as client:  # (1)
    result = await client.create_agent_runtime()  # (2)
```

1. client: [BedrockAgentCoreControlClient](./client.md)
2. result: [:material-code-braces: CreateAgentRuntimeResponseTypeDef](./type_defs.md#createagentruntimeresponsetypedef)



#### Paginator usage example

```python
# ListAgentRuntimeEndpointsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-agentcore-control") as client:  # (1)
    paginator = client.get_paginator("list_agent_runtime_endpoints")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BedrockAgentCoreControlClient](./client.md)
2. paginator: [ListAgentRuntimeEndpointsPaginator](./paginators.md#listagentruntimeendpointspaginator)
3. item: [:material-code-braces: ListAgentRuntimeEndpointsResponseTypeDef](./type_defs.md#listagentruntimeendpointsresponsetypedef)



#### Waiter usage example

```python
# MemoryCreatedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-agentcore-control") as client:  # (1)
    waiter = client.get_waiter("memory_created")  # (2)
    await waiter.wait(...)
```

1. client: [BedrockAgentCoreControlClient](./client.md)
2. waiter: [MemoryCreatedWaiter](./waiters.md#memorycreatedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[bedrock-agentcore-control]`
or a standalone `types_aiobotocore_bedrock_agentcore_control` package, you have to explicitly specify
`client: BedrockAgentCoreControlClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# BedrockAgentCoreControlClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore_control.client import BedrockAgentCoreControlClient
from types_aiobotocore_bedrock_agentcore_control.type_defs import CreateAgentRuntimeResponseTypeDef
from types_aiobotocore_bedrock_agentcore_control.type_defs import CreateAgentRuntimeRequestTypeDef


session = get_session()

async with session.create_client("bedrock-agentcore-control") as client:
    client: BedrockAgentCoreControlClient
    kwargs: CreateAgentRuntimeRequestTypeDef = {...}
    result: CreateAgentRuntimeResponseTypeDef = await client.create_agent_runtime(**kwargs)
```



#### Paginator usage example

```python
# ListAgentRuntimeEndpointsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore_control.client import BedrockAgentCoreControlClient
from types_aiobotocore_bedrock_agentcore_control.paginator import ListAgentRuntimeEndpointsPaginator
from types_aiobotocore_bedrock_agentcore_control.type_defs import ListAgentRuntimeEndpointsResponseTypeDef


session = get_session()

async with session.create_client("bedrock-agentcore-control") as client:
    client: BedrockAgentCoreControlClient
    paginator: ListAgentRuntimeEndpointsPaginator = client.get_paginator("list_agent_runtime_endpoints")
    async for item in paginator.paginate(...):
        item: ListAgentRuntimeEndpointsResponseTypeDef
        print(item)
```



#### Waiter usage example

```python
# MemoryCreatedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agentcore_control.client import BedrockAgentCoreControlClient
from types_aiobotocore_bedrock_agentcore_control.waiter import MemoryCreatedWaiter


session = get_session()

async with session.create_client("bedrock-agentcore-control") as client:
    client: BedrockAgentCoreControlClient
    waiter: MemoryCreatedWaiter = client.get_waiter("memory_created")
    await waiter.wait(...)
```
