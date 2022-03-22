<a id="examples-for-aiobotocore-autoscalingplans-module"></a>

# Examples for aiobotocore AutoScalingPlans module

> [Index](../README.md) > [AutoScalingPlans](./README.md) > Examples

- [Examples for aiobotocore AutoScalingPlans module](#examples-for-aiobotocore-autoscalingplans-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[autoscaling-plans]` package installed.

Write your `AutoScalingPlans` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AutoScalingPlansClient
# and provides type checking and code completion
async with session.create_client("autoscaling-plans") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeScalingPlanResourcesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_scaling_plan_resources")
    async for item in paginator.paginate(...):
        # item has type DescribeScalingPlanResourcesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[autoscaling-plans]` or a standalone
`types_aiobotocore_autoscaling_plans` package, you have to explicitly specify
`client: AutoScalingPlansClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling_plans.client import AutoScalingPlansClient
from types_aiobotocore_autoscaling_plans.type_defs import bool
from types_aiobotocore_autoscaling_plans.paginator import DescribeScalingPlanResourcesPaginator

from types_aiobotocore_autoscaling_plans.literals import PaginatorName



session = get_session()

async with session.create_client("autoscaling-plans") as client:
    client: AutoScalingPlansClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_scaling_plan_resources"
    paginator: DescribeScalingPlanResourcesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeScalingPlanResourcesResponseTypeDef
        print(item)
    

    
```
