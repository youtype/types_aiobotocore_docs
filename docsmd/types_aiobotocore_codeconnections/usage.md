# Examples

> [Index](../README.md) > [CodeConnections](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeConnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections.html#codeconnections)
    type annotations stubs module [types-aiobotocore-codeconnections](https://pypi.org/project/types-aiobotocore-codeconnections/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[codeconnections]` package installed.

Write your `CodeConnections` code as usual,
type checking and code completion should work out of the box.



```python
# CodeConnectionsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codeconnections") as client:  # (1)
    result = await client.create_connection()  # (2)
```

1. client: [CodeConnectionsClient](./client.md)
2. result: [:material-code-braces: CreateConnectionOutputTypeDef](./type_defs.md#createconnectionoutputtypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[codeconnections]`
or a standalone `types_aiobotocore_codeconnections` package, you have to explicitly specify
`client: CodeConnectionsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CodeConnectionsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codeconnections.client import CodeConnectionsClient
from types_aiobotocore_codeconnections.type_defs import CreateConnectionOutputTypeDef
from types_aiobotocore_codeconnections.type_defs import CreateConnectionInputTypeDef


session = get_session()

async with session.create_client("codeconnections") as client:
    client: CodeConnectionsClient
    kwargs: CreateConnectionInputTypeDef = {...}
    result: CreateConnectionOutputTypeDef = await client.create_connection(**kwargs)
```




