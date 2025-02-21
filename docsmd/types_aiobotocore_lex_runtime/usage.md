# Examples

> [Index](../README.md) > [LexRuntimeService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LexRuntimeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#lexruntimeservice)
    type annotations stubs module [types-aiobotocore-lex-runtime](https://pypi.org/project/types-aiobotocore-lex-runtime/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[lex-runtime]` package installed.

Write your `LexRuntimeService` code as usual,
type checking and code completion should work out of the box.



```python
# LexRuntimeServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("lex-runtime") as client:  # (1)
    result = await client.delete_session()  # (2)
```

1. client: [LexRuntimeServiceClient](./client.md)
2. result: [:material-code-braces: DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[lex-runtime]`
or a standalone `types_aiobotocore_lex_runtime` package, you have to explicitly specify
`client: LexRuntimeServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LexRuntimeServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_lex_runtime.client import LexRuntimeServiceClient
from types_aiobotocore_lex_runtime.type_defs import DeleteSessionResponseTypeDef
from types_aiobotocore_lex_runtime.type_defs import DeleteSessionRequestTypeDef


session = get_session()

async with session.create_client("lex-runtime") as client:
    client: LexRuntimeServiceClient
    kwargs: DeleteSessionRequestTypeDef = {...}
    result: DeleteSessionResponseTypeDef = await client.delete_session(**kwargs)
```




