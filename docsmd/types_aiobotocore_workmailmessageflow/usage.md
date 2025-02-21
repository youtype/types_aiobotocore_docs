# Examples

> [Index](../README.md) > [WorkMailMessageFlow](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkMailMessageFlow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#workmailmessageflow)
    type annotations stubs module [types-aiobotocore-workmailmessageflow](https://pypi.org/project/types-aiobotocore-workmailmessageflow/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[workmailmessageflow]` package installed.

Write your `WorkMailMessageFlow` code as usual,
type checking and code completion should work out of the box.



```python
# WorkMailMessageFlowClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("workmailmessageflow") as client:  # (1)
    result = await client.get_raw_message_content()  # (2)
```

1. client: [WorkMailMessageFlowClient](./client.md)
2. result: [:material-code-braces: GetRawMessageContentResponseTypeDef](./type_defs.md#getrawmessagecontentresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[workmailmessageflow]`
or a standalone `types_aiobotocore_workmailmessageflow` package, you have to explicitly specify
`client: WorkMailMessageFlowClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# WorkMailMessageFlowClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_workmailmessageflow.client import WorkMailMessageFlowClient
from types_aiobotocore_workmailmessageflow.type_defs import GetRawMessageContentResponseTypeDef
from types_aiobotocore_workmailmessageflow.type_defs import GetRawMessageContentRequestTypeDef


session = get_session()

async with session.create_client("workmailmessageflow") as client:
    client: WorkMailMessageFlowClient
    kwargs: GetRawMessageContentRequestTypeDef = {...}
    result: GetRawMessageContentResponseTypeDef = await client.get_raw_message_content(**kwargs)
```




