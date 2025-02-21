# Examples

> [Index](../README.md) > [QLDBSession](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QLDBSession](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#qldbsession)
    type annotations stubs module [types-aiobotocore-qldb-session](https://pypi.org/project/types-aiobotocore-qldb-session/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[qldb-session]` package installed.

Write your `QLDBSession` code as usual,
type checking and code completion should work out of the box.



```python
# QLDBSessionClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("qldb-session") as client:  # (1)
    result = await client.send_command()  # (2)
```

1. client: [QLDBSessionClient](./client.md)
2. result: [:material-code-braces: SendCommandResultTypeDef](./type_defs.md#sendcommandresulttypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[qldb-session]`
or a standalone `types_aiobotocore_qldb_session` package, you have to explicitly specify
`client: QLDBSessionClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# QLDBSessionClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_qldb_session.client import QLDBSessionClient
from types_aiobotocore_qldb_session.type_defs import SendCommandResultTypeDef
from types_aiobotocore_qldb_session.type_defs import SendCommandRequestTypeDef


session = get_session()

async with session.create_client("qldb-session") as client:
    client: QLDBSessionClient
    kwargs: SendCommandRequestTypeDef = {...}
    result: SendCommandResultTypeDef = await client.send_command(**kwargs)
```




