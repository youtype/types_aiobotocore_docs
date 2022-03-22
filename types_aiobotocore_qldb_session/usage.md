<a id="examples-for-aiobotocore-qldbsession-module"></a>

# Examples for aiobotocore QLDBSession module

> [Index](../README.md) > [QLDBSession](./README.md) > Examples

- [Examples for aiobotocore QLDBSession module](#examples-for-aiobotocore-qldbsession-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[qldb-session]` package installed.

Write your `QLDBSession` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type QLDBSessionClient
# and provides type checking and code completion
async with session.create_client("qldb-session") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[qldb-session]` or a standalone
`types_aiobotocore_qldb_session` package, you have to explicitly specify
`client: QLDBSessionClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_qldb_session.client import QLDBSessionClient
from types_aiobotocore_qldb_session.type_defs import bool






session = get_session()

async with session.create_client("qldb-session") as client:
    client: QLDBSessionClient

    
    result: bool = client.can_paginate()
    

    

    
```
