# Examples

> [Index](../README.md) > [WAF](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WAF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#waf)
    type annotations stubs module [types-aiobotocore-waf](https://pypi.org/project/types-aiobotocore-waf/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[waf]` package installed.

Write your `WAF` code as usual,
type checking and code completion should work out of the box.



```python
# WAFClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("waf") as client:  # (1)
    result = await client.create_byte_match_set()  # (2)
```

1. client: [WAFClient](./client.md)
2. result: [:material-code-braces: CreateByteMatchSetResponseTypeDef](./type_defs.md#createbytematchsetresponsetypedef) 



```python
# GetRateBasedRuleManagedKeysPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("waf") as client:  # (1)
    paginator = client.get_paginator("get_rate_based_rule_managed_keys")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WAFClient](./client.md)
2. paginator: [GetRateBasedRuleManagedKeysPaginator](./paginators.md#getratebasedrulemanagedkeyspaginator)
3. item: [:material-code-braces: GetRateBasedRuleManagedKeysResponseTypeDef](./type_defs.md#getratebasedrulemanagedkeysresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[waf]`
or a standalone `types_aiobotocore_waf` package, you have to explicitly specify
`client: WAFClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# WAFClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_waf.client import WAFClient
from types_aiobotocore_waf.type_defs import CreateByteMatchSetResponseTypeDef
from types_aiobotocore_waf.type_defs import CreateByteMatchSetRequestTypeDef


session = get_session()

async with session.create_client("waf") as client:
    client: WAFClient
    kwargs: CreateByteMatchSetRequestTypeDef = {...}
    result: CreateByteMatchSetResponseTypeDef = await client.create_byte_match_set(**kwargs)
```



```python
# GetRateBasedRuleManagedKeysPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_waf.client import WAFClient
from types_aiobotocore_waf.paginator import GetRateBasedRuleManagedKeysPaginator
from types_aiobotocore_waf.type_defs import GetRateBasedRuleManagedKeysResponseTypeDef


session = get_session()

async with session.create_client("waf") as client:
    client: WAFClient
    paginator: GetRateBasedRuleManagedKeysPaginator = client.get_paginator("get_rate_based_rule_managed_keys")
    async for item in paginator.paginate(...):
        item: GetRateBasedRuleManagedKeysResponseTypeDef
        print(item)
```


