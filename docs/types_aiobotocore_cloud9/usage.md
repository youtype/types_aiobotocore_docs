<a id="examples-for-aiobotocore-cloud9-module"></a>

# Examples for aiobotocore Cloud9 module

> [Index](../README.md) > [Cloud9](./README.md) > Examples

- [Examples for aiobotocore Cloud9 module](#examples-for-aiobotocore-cloud9-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cloud9]` package installed.

Write your `Cloud9` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type Cloud9Client
# and provides type checking and code completion
async with session.create_client("cloud9") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeEnvironmentMembershipsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_environment_memberships")
    async for item in paginator.paginate(...):
        # item has type DescribeEnvironmentMembershipsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cloud9]` or a standalone
`types_aiobotocore_cloud9` package, you have to explicitly specify
`client: Cloud9Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloud9.client import Cloud9Client
from types_aiobotocore_cloud9.type_defs import bool
from types_aiobotocore_cloud9.paginator import DescribeEnvironmentMembershipsPaginator

from types_aiobotocore_cloud9.literals import PaginatorName



session = get_session()

async with session.create_client("cloud9") as client:
    client: Cloud9Client

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_environment_memberships"
    paginator: DescribeEnvironmentMembershipsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeEnvironmentMembershipsResultTypeDef
        print(item)
    

    
```
