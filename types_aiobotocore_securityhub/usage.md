<a id="examples-for-aiobotocore-securityhub-module"></a>

# Examples for aiobotocore SecurityHub module

> [Index](../README.md) > [SecurityHub](./README.md) > Examples

- [Examples for aiobotocore SecurityHub module](#examples-for-aiobotocore-securityhub-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[securityhub]` package installed.

Write your `SecurityHub` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SecurityHubClient
# and provides type checking and code completion
async with session.create_client("securityhub") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_administrator_invitation()
    

    
    # paginator has type DescribeActionTargetsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_action_targets")
    async for item in paginator.paginate(...):
        # item has type DescribeActionTargetsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[securityhub]` or a standalone
`types_aiobotocore_securityhub` package, you have to explicitly specify
`client: SecurityHubClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.client import SecurityHubClient
from types_aiobotocore_securityhub.type_defs import Dict[str, Any]
from types_aiobotocore_securityhub.paginator import DescribeActionTargetsPaginator

from types_aiobotocore_securityhub.literals import PaginatorName



session = get_session()

async with session.create_client("securityhub") as client:
    client: SecurityHubClient

    
    result: Dict[str, Any] = client.accept_administrator_invitation()
    

    
    paginator_name: PaginatorName = "describe_action_targets"
    paginator: DescribeActionTargetsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeActionTargetsResponseTypeDef
        print(item)
    

    
```
