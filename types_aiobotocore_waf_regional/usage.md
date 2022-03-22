<a id="examples-for-aiobotocore-wafregional-module"></a>

# Examples for aiobotocore WAFRegional module

> [Index](../README.md) > [WAFRegional](./README.md) > Examples

- [Examples for aiobotocore WAFRegional module](#examples-for-aiobotocore-wafregional-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[waf-regional]` package installed.

Write your `WAFRegional` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type WAFRegionalClient
# and provides type checking and code completion
async with session.create_client("waf-regional") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_web_acl()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[waf-regional]` or a standalone
`types_aiobotocore_waf_regional` package, you have to explicitly specify
`client: WAFRegionalClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_waf_regional.client import WAFRegionalClient
from types_aiobotocore_waf_regional.type_defs import Dict[str, Any]






session = get_session()

async with session.create_client("waf-regional") as client:
    client: WAFRegionalClient

    
    result: Dict[str, Any] = client.associate_web_acl()
    

    

    
```
