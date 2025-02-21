# Examples

> [Index](../README.md) > [CodeStarconnections](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeStarconnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#codestarconnections)
    type annotations stubs module [types-aiobotocore-codestar-connections](https://pypi.org/project/types-aiobotocore-codestar-connections/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[codestar-connections]` package installed.

Write your `CodeStarconnections` code as usual,
type checking and code completion should work out of the box.



```python
# CodeStarconnectionsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codestar-connections") as client:  # (1)
    result = await client.create_connection()  # (2)
```

1. client: [CodeStarconnectionsClient](./client.md)
2. result: [:material-code-braces: CreateConnectionOutputTypeDef](./type_defs.md#createconnectionoutputtypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[codestar-connections]`
or a standalone `types_aiobotocore_codestar_connections` package, you have to explicitly specify
`client: CodeStarconnectionsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CodeStarconnectionsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codestar_connections.client import CodeStarconnectionsClient
from types_aiobotocore_codestar_connections.type_defs import CreateConnectionOutputTypeDef
from types_aiobotocore_codestar_connections.type_defs import CreateConnectionInputTypeDef


session = get_session()

async with session.create_client("codestar-connections") as client:
    client: CodeStarconnectionsClient
    kwargs: CreateConnectionInputTypeDef = {...}
    result: CreateConnectionOutputTypeDef = await client.create_connection(**kwargs)
```




