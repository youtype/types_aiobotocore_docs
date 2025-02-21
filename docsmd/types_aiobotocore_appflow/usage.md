# Examples

> [Index](../README.md) > [Appflow](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Appflow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#appflow)
    type annotations stubs module [types-aiobotocore-appflow](https://pypi.org/project/types-aiobotocore-appflow/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[appflow]` package installed.

Write your `Appflow` code as usual,
type checking and code completion should work out of the box.



```python
# AppflowClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appflow") as client:  # (1)
    result = await client.cancel_flow_executions()  # (2)
```

1. client: [AppflowClient](./client.md)
2. result: [:material-code-braces: CancelFlowExecutionsResponseTypeDef](./type_defs.md#cancelflowexecutionsresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[appflow]`
or a standalone `types_aiobotocore_appflow` package, you have to explicitly specify
`client: AppflowClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AppflowClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appflow.client import AppflowClient
from types_aiobotocore_appflow.type_defs import CancelFlowExecutionsResponseTypeDef
from types_aiobotocore_appflow.type_defs import CancelFlowExecutionsRequestTypeDef


session = get_session()

async with session.create_client("appflow") as client:
    client: AppflowClient
    kwargs: CancelFlowExecutionsRequestTypeDef = {...}
    result: CancelFlowExecutionsResponseTypeDef = await client.cancel_flow_executions(**kwargs)
```




