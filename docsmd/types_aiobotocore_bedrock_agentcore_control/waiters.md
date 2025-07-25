# Waiters

> [Index](../README.md) > [BedrockAgentCoreControlPlaneFrontingLayer](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [BedrockAgentCoreControlPlaneFrontingLayer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#bedrockagentcorecontrolplanefrontinglayer)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore-control](https://pypi.org/project/types-aiobotocore-bedrock-agentcore-control/).

## MemoryCreatedWaiter

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_waiter("memory_created")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/waiter/MemoryCreated.html#BedrockAgentCoreControlPlaneFrontingLayer.Waiter.MemoryCreated)

```python
# MemoryCreatedWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_bedrock_agentcore_control.waiter import MemoryCreatedWaiter

session = get_session()
async with session.create_client("bedrock-agentcore-control") as client:  # (1)
    waiter: MemoryCreatedWaiter = client.get_waiter("memory_created")  # (2)
    await waiter.wait(...)
```

1. client: [BedrockAgentCoreControlPlaneFrontingLayerClient](./client.md)
2. waiter: [MemoryCreatedWaiter](./waiters.md#memorycreatedwaiter)


### wait

Type annotations and code completion for `#!python MemoryCreatedWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    memoryId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)


```python
# wait method usage example with argument unpacking

kwargs: GetMemoryInputWaitTypeDef = {  # (1)
    "memoryId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetMemoryInputWaitTypeDef](./type_defs.md#getmemoryinputwaittypedef)
