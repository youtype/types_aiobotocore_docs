# Examples

> [Index](../README.md) > [NeptuneData](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NeptuneData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#neptunedata)
    type annotations stubs module [types-aiobotocore-neptunedata](https://pypi.org/project/types-aiobotocore-neptunedata/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[neptunedata]` package installed.

Write your `NeptuneData` code as usual,
type checking and code completion should work out of the box.



```python
# NeptuneDataClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("neptunedata") as client:  # (1)
    result = await client.cancel_gremlin_query()  # (2)
```

1. client: [NeptuneDataClient](./client.md)
2. result: [:material-code-braces: CancelGremlinQueryOutputTypeDef](./type_defs.md#cancelgremlinqueryoutputtypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[neptunedata]`
or a standalone `types_aiobotocore_neptunedata` package, you have to explicitly specify
`client: NeptuneDataClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# NeptuneDataClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_neptunedata.client import NeptuneDataClient
from types_aiobotocore_neptunedata.type_defs import CancelGremlinQueryOutputTypeDef
from types_aiobotocore_neptunedata.type_defs import CancelGremlinQueryInputTypeDef


session = get_session()

async with session.create_client("neptunedata") as client:
    client: NeptuneDataClient
    kwargs: CancelGremlinQueryInputTypeDef = {...}
    result: CancelGremlinQueryOutputTypeDef = await client.cancel_gremlin_query(**kwargs)
```




