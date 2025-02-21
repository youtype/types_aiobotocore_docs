# Examples

> [Index](../README.md) > [Pinpoint](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Pinpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#pinpoint)
    type annotations stubs module [types-aiobotocore-pinpoint](https://pypi.org/project/types-aiobotocore-pinpoint/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[pinpoint]` package installed.

Write your `Pinpoint` code as usual,
type checking and code completion should work out of the box.



```python
# PinpointClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pinpoint") as client:  # (1)
    result = await client.create_app()  # (2)
```

1. client: [PinpointClient](./client.md)
2. result: [:material-code-braces: CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[pinpoint]`
or a standalone `types_aiobotocore_pinpoint` package, you have to explicitly specify
`client: PinpointClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PinpointClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint.client import PinpointClient
from types_aiobotocore_pinpoint.type_defs import CreateAppResponseTypeDef
from types_aiobotocore_pinpoint.type_defs import CreateAppRequestTypeDef


session = get_session()

async with session.create_client("pinpoint") as client:
    client: PinpointClient
    kwargs: CreateAppRequestTypeDef = {...}
    result: CreateAppResponseTypeDef = await client.create_app(**kwargs)
```




