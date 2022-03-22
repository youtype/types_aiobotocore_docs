<a id="examples-for-aiobotocore-costexplorer-module"></a>

# Examples for aiobotocore CostExplorer module

> [Index](../README.md) > [CostExplorer](./README.md) > Examples

- [Examples for aiobotocore CostExplorer module](#examples-for-aiobotocore-costexplorer-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ce]` package installed.

Write your `CostExplorer` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CostExplorerClient
# and provides type checking and code completion
async with session.create_client("ce") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ce]` or a standalone `types_aiobotocore_ce`
package, you have to explicitly specify `client: CostExplorerClient` type
annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ce.client import CostExplorerClient
from types_aiobotocore_ce.type_defs import bool






session = get_session()

async with session.create_client("ce") as client:
    client: CostExplorerClient

    
    result: bool = client.can_paginate()
    

    

    
```
