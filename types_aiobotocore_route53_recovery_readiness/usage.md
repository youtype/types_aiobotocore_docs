<a id="examples-for-aiobotocore-route53recoveryreadiness-module"></a>

# Examples for aiobotocore Route53RecoveryReadiness module

> [Index](../README.md) > [Route53RecoveryReadiness](./README.md) > Examples

- [Examples for aiobotocore Route53RecoveryReadiness module](#examples-for-aiobotocore-route53recoveryreadiness-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[route53-recovery-readiness]` package
installed.

Write your `Route53RecoveryReadiness` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type Route53RecoveryReadinessClient
# and provides type checking and code completion
async with session.create_client("route53-recovery-readiness") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetCellReadinessSummaryPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_cell_readiness_summary")
    async for item in paginator.paginate(...):
        # item has type GetCellReadinessSummaryResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[route53-recovery-readiness]` or a standalone
`types_aiobotocore_route53_recovery_readiness` package, you have to explicitly
specify `client: Route53RecoveryReadinessClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_readiness.client import Route53RecoveryReadinessClient
from types_aiobotocore_route53_recovery_readiness.type_defs import bool
from types_aiobotocore_route53_recovery_readiness.paginator import GetCellReadinessSummaryPaginator

from types_aiobotocore_route53_recovery_readiness.literals import PaginatorName



session = get_session()

async with session.create_client("route53-recovery-readiness") as client:
    client: Route53RecoveryReadinessClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_cell_readiness_summary"
    paginator: GetCellReadinessSummaryPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetCellReadinessSummaryResponseTypeDef
        print(item)
    

    
```
