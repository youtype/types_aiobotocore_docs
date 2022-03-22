<a id="examples-for-aiobotocore-waf-module"></a>

# Examples for aiobotocore WAF module

> [Index](../README.md) > [WAF](./README.md) > Examples

- [Examples for aiobotocore WAF module](#examples-for-aiobotocore-waf-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[waf]` package installed.

Write your `WAF` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type WAFClient
# and provides type checking and code completion
async with session.create_client("waf") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetRateBasedRuleManagedKeysPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_rate_based_rule_managed_keys")
    async for item in paginator.paginate(...):
        # item has type GetRateBasedRuleManagedKeysResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[waf]` or a standalone `types_aiobotocore_waf`
package, you have to explicitly specify `client: WAFClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_waf.client import WAFClient
from types_aiobotocore_waf.type_defs import bool
from types_aiobotocore_waf.paginator import GetRateBasedRuleManagedKeysPaginator

from types_aiobotocore_waf.literals import PaginatorName



session = get_session()

async with session.create_client("waf") as client:
    client: WAFClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_rate_based_rule_managed_keys"
    paginator: GetRateBasedRuleManagedKeysPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetRateBasedRuleManagedKeysResponseTypeDef
        print(item)
    

    
```
