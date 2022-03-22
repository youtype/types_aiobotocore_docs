<a id="examples-for-aiobotocore-applicationautoscaling-module"></a>

# Examples for aiobotocore ApplicationAutoScaling module

> [Index](../README.md) > [ApplicationAutoScaling](./README.md) > Examples

- [Examples for aiobotocore ApplicationAutoScaling module](#examples-for-aiobotocore-applicationautoscaling-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[application-autoscaling]` package
installed.

Write your `ApplicationAutoScaling` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ApplicationAutoScalingClient
# and provides type checking and code completion
async with session.create_client("application-autoscaling") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeScalableTargetsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_scalable_targets")
    async for item in paginator.paginate(...):
        # item has type DescribeScalableTargetsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[application-autoscaling]` or a standalone
`types_aiobotocore_application_autoscaling` package, you have to explicitly
specify `client: ApplicationAutoScalingClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_application_autoscaling.client import ApplicationAutoScalingClient
from types_aiobotocore_application_autoscaling.type_defs import bool
from types_aiobotocore_application_autoscaling.paginator import DescribeScalableTargetsPaginator

from types_aiobotocore_application_autoscaling.literals import PaginatorName



session = get_session()

async with session.create_client("application-autoscaling") as client:
    client: ApplicationAutoScalingClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_scalable_targets"
    paginator: DescribeScalableTargetsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeScalableTargetsResponseTypeDef
        print(item)
    

    
```
