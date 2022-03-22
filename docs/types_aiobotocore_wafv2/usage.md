<a id="examples-for-aiobotocore-wafv2-module"></a>

# Examples for aiobotocore WAFV2 module

> [Index](../README.md) > [WAFV2](./README.md) > Examples

- [Examples for aiobotocore WAFV2 module](#examples-for-aiobotocore-wafv2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[wafv2]` package installed.

Write your `WAFV2` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type WAFV2Client
# and provides type checking and code completion
async with session.create_client("wafv2") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_web_acl()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[wafv2]` or a standalone `types_aiobotocore_wafv2`
package, you have to explicitly specify `client: WAFV2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_wafv2.client import WAFV2Client
from types_aiobotocore_wafv2.type_defs import Dict[str, Any]






session = get_session()

async with session.create_client("wafv2") as client:
    client: WAFV2Client

    
    result: Dict[str, Any] = client.associate_web_acl()
    

    

    
```
