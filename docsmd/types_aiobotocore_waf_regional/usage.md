# Examples

> [Index](../README.md) > [WAFRegional](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WAFRegional](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#wafregional)
    type annotations stubs module [types-aiobotocore-waf-regional](https://pypi.org/project/types-aiobotocore-waf-regional/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[waf-regional]` package installed.

Write your `WAFRegional` code as usual,
type checking and code completion should work out of the box.



```python
# WAFRegionalClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("waf-regional") as client:  # (1)
    result = await client.create_byte_match_set()  # (2)
```

1. client: [WAFRegionalClient](./client.md)
2. result: [:material-code-braces: CreateByteMatchSetResponseTypeDef](./type_defs.md#createbytematchsetresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[waf-regional]`
or a standalone `types_aiobotocore_waf_regional` package, you have to explicitly specify
`client: WAFRegionalClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# WAFRegionalClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_waf_regional.client import WAFRegionalClient
from types_aiobotocore_waf_regional.type_defs import CreateByteMatchSetResponseTypeDef
from types_aiobotocore_waf_regional.type_defs import CreateByteMatchSetRequestTypeDef


session = get_session()

async with session.create_client("waf-regional") as client:
    client: WAFRegionalClient
    kwargs: CreateByteMatchSetRequestTypeDef = {...}
    result: CreateByteMatchSetResponseTypeDef = await client.create_byte_match_set(**kwargs)
```




