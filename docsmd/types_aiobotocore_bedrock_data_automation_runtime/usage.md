# Examples

> [Index](../README.md) > [RuntimeforBedrockDataAutomation](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RuntimeforBedrockDataAutomation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation-runtime.html#runtimeforbedrockdataautomation)
    type annotations stubs module [types-aiobotocore-bedrock-data-automation-runtime](https://pypi.org/project/types-aiobotocore-bedrock-data-automation-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bedrock-data-automation-runtime]` package installed.

Write your `RuntimeforBedrockDataAutomation` code as usual,
type checking and code completion should work out of the box.



```python
# RuntimeforBedrockDataAutomationClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-data-automation-runtime") as client:  # (1)
    result = await client.get_data_automation_status()  # (2)
```

1. client: [RuntimeforBedrockDataAutomationClient](./client.md)
2. result: [:material-code-braces: GetDataAutomationStatusResponseTypeDef](./type_defs.md#getdataautomationstatusresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[bedrock-data-automation-runtime]`
or a standalone `types_aiobotocore_bedrock_data_automation_runtime` package, you have to explicitly specify
`client: RuntimeforBedrockDataAutomationClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# RuntimeforBedrockDataAutomationClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_data_automation_runtime.client import RuntimeforBedrockDataAutomationClient
from types_aiobotocore_bedrock_data_automation_runtime.type_defs import GetDataAutomationStatusResponseTypeDef
from types_aiobotocore_bedrock_data_automation_runtime.type_defs import GetDataAutomationStatusRequestTypeDef


session = get_session()

async with session.create_client("bedrock-data-automation-runtime") as client:
    client: RuntimeforBedrockDataAutomationClient
    kwargs: GetDataAutomationStatusRequestTypeDef = {...}
    result: GetDataAutomationStatusResponseTypeDef = await client.get_data_automation_status(**kwargs)
```




