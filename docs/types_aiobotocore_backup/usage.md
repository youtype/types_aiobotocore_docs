<a id="examples-for-aiobotocore-backup-module"></a>

# Examples for aiobotocore Backup module

> [Index](../README.md) > [Backup](./README.md) > Examples

- [Examples for aiobotocore Backup module](#examples-for-aiobotocore-backup-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[backup]` package installed.

Write your `Backup` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type BackupClient
# and provides type checking and code completion
async with session.create_client("backup") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[backup]` or a standalone
`types_aiobotocore_backup` package, you have to explicitly specify
`client: BackupClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_backup.client import BackupClient
from types_aiobotocore_backup.type_defs import bool






session = get_session()

async with session.create_client("backup") as client:
    client: BackupClient

    
    result: bool = client.can_paginate()
    

    

    
```
