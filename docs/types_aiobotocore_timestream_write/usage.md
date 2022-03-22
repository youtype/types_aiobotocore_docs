<a id="examples-for-aiobotocore-timestreamwrite-module"></a>

# Examples for aiobotocore TimestreamWrite module

> [Index](../README.md) > [TimestreamWrite](./README.md) > Examples

- [Examples for aiobotocore TimestreamWrite module](#examples-for-aiobotocore-timestreamwrite-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[timestream-write]` package installed.

Write your `TimestreamWrite` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type TimestreamWriteClient
# and provides type checking and code completion
async with session.create_client("timestream-write") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[timestream-write]` or a standalone
`types_aiobotocore_timestream_write` package, you have to explicitly specify
`client: TimestreamWriteClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_timestream_write.client import TimestreamWriteClient
from types_aiobotocore_timestream_write.type_defs import bool






session = get_session()

async with session.create_client("timestream-write") as client:
    client: TimestreamWriteClient

    
    result: bool = client.can_paginate()
    

    

    
```
