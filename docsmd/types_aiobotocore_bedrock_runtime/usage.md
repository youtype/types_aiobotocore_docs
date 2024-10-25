# Examples

> [Index](../README.md) > [BedrockRuntime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#BedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-runtime](https://pypi.org/project/types-aiobotocore-bedrock-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bedrock-runtime]` package installed.

Write your `BedrockRuntime` code as usual,
type checking and code completion should work out of the box.



```python
# BedrockRuntimeClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-runtime") as client:  # (1)
    result = await client.apply_guardrail()  # (2)
```

1. client: [BedrockRuntimeClient](./client.md)
2. result: [:material-code-braces: ApplyGuardrailResponseTypeDef](./type_defs.md#applyguardrailresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[bedrock-runtime]`
or a standalone `types_aiobotocore_bedrock_runtime` package, you have to explicitly specify
`client: BedrockRuntimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# BedrockRuntimeClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_runtime.client import BedrockRuntimeClient
from types_aiobotocore_bedrock_runtime.type_defs import ApplyGuardrailResponseTypeDef
from types_aiobotocore_bedrock_runtime.type_defs import ApplyGuardrailRequestRequestTypeDef


session = get_session()

async with session.create_client("bedrock-runtime") as client:
    client: BedrockRuntimeClient
    kwargs: ApplyGuardrailRequestRequestTypeDef = {...}
    result: ApplyGuardrailResponseTypeDef = await client.apply_guardrail(**kwargs)
```




