<a id="examples-for-aiobotocore-memorydb-module"></a>

# Examples for aiobotocore MemoryDB module

> [Index](../README.md) > [MemoryDB](./README.md) > Examples

- [Examples for aiobotocore MemoryDB module](#examples-for-aiobotocore-memorydb-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[memorydb]` package installed.

Write your `MemoryDB` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MemoryDBClient
# and provides type checking and code completion
async with session.create_client("memorydb") as client:
    
    # result has type BatchUpdateClusterResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_update_cluster()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[memorydb]` or a standalone
`types_aiobotocore_memorydb` package, you have to explicitly specify
`client: MemoryDBClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_memorydb.client import MemoryDBClient
from types_aiobotocore_memorydb.type_defs import BatchUpdateClusterResponseTypeDef






session = get_session()

async with session.create_client("memorydb") as client:
    client: MemoryDBClient

    
    result: BatchUpdateClusterResponseTypeDef = client.batch_update_cluster()
    

    

    
```
