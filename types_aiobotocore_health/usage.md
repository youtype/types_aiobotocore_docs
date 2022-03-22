<a id="examples-for-aiobotocore-health-module"></a>

# Examples for aiobotocore Health module

> [Index](../README.md) > [Health](./README.md) > Examples

- [Examples for aiobotocore Health module](#examples-for-aiobotocore-health-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[health]` package installed.

Write your `Health` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type HealthClient
# and provides type checking and code completion
async with session.create_client("health") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeAffectedAccountsForOrganizationPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_affected_accounts_for_organization")
    async for item in paginator.paginate(...):
        # item has type DescribeAffectedAccountsForOrganizationResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[health]` or a standalone
`types_aiobotocore_health` package, you have to explicitly specify
`client: HealthClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_health.client import HealthClient
from types_aiobotocore_health.type_defs import bool
from types_aiobotocore_health.paginator import DescribeAffectedAccountsForOrganizationPaginator

from types_aiobotocore_health.literals import PaginatorName



session = get_session()

async with session.create_client("health") as client:
    client: HealthClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_affected_accounts_for_organization"
    paginator: DescribeAffectedAccountsForOrganizationPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAffectedAccountsForOrganizationResponseTypeDef
        print(item)
    

    
```
