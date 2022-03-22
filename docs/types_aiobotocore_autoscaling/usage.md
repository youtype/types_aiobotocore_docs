<a id="examples-for-aiobotocore-autoscaling-module"></a>

# Examples for aiobotocore AutoScaling module

> [Index](../README.md) > [AutoScaling](./README.md) > Examples

- [Examples for aiobotocore AutoScaling module](#examples-for-aiobotocore-autoscaling-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[autoscaling]` package installed.

Write your `AutoScaling` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AutoScalingClient
# and provides type checking and code completion
async with session.create_client("autoscaling") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.attach_instances()
    

    
    # paginator has type DescribeAutoScalingGroupsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_auto_scaling_groups")
    async for item in paginator.paginate(...):
        # item has type AutoScalingGroupsTypeTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[autoscaling]` or a standalone
`types_aiobotocore_autoscaling` package, you have to explicitly specify
`client: AutoScalingClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.client import AutoScalingClient
from types_aiobotocore_autoscaling.type_defs import None
from types_aiobotocore_autoscaling.paginator import DescribeAutoScalingGroupsPaginator

from types_aiobotocore_autoscaling.literals import PaginatorName



session = get_session()

async with session.create_client("autoscaling") as client:
    client: AutoScalingClient

    
    result: None = client.attach_instances()
    

    
    paginator_name: PaginatorName = "describe_auto_scaling_groups"
    paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: AutoScalingGroupsTypeTypeDef
        print(item)
    

    
```
