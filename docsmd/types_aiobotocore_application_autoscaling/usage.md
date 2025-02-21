# Examples

> [Index](../README.md) > [ApplicationAutoScaling](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ApplicationAutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#applicationautoscaling)
    type annotations stubs module [types-aiobotocore-application-autoscaling](https://pypi.org/project/types-aiobotocore-application-autoscaling/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[application-autoscaling]` package installed.

Write your `ApplicationAutoScaling` code as usual,
type checking and code completion should work out of the box.



```python
# ApplicationAutoScalingClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("application-autoscaling") as client:  # (1)
    result = await client.describe_scalable_targets()  # (2)
```

1. client: [ApplicationAutoScalingClient](./client.md)
2. result: [:material-code-braces: DescribeScalableTargetsResponseTypeDef](./type_defs.md#describescalabletargetsresponsetypedef) 



```python
# DescribeScalableTargetsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("application-autoscaling") as client:  # (1)
    paginator = client.get_paginator("describe_scalable_targets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ApplicationAutoScalingClient](./client.md)
2. paginator: [DescribeScalableTargetsPaginator](./paginators.md#describescalabletargetspaginator)
3. item: [:material-code-braces: DescribeScalableTargetsResponseTypeDef](./type_defs.md#describescalabletargetsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[application-autoscaling]`
or a standalone `types_aiobotocore_application_autoscaling` package, you have to explicitly specify
`client: ApplicationAutoScalingClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ApplicationAutoScalingClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_application_autoscaling.client import ApplicationAutoScalingClient
from types_aiobotocore_application_autoscaling.type_defs import DescribeScalableTargetsResponseTypeDef
from types_aiobotocore_application_autoscaling.type_defs import DescribeScalableTargetsRequestTypeDef


session = get_session()

async with session.create_client("application-autoscaling") as client:
    client: ApplicationAutoScalingClient
    kwargs: DescribeScalableTargetsRequestTypeDef = {...}
    result: DescribeScalableTargetsResponseTypeDef = await client.describe_scalable_targets(**kwargs)
```



```python
# DescribeScalableTargetsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_application_autoscaling.client import ApplicationAutoScalingClient
from types_aiobotocore_application_autoscaling.paginator import DescribeScalableTargetsPaginator
from types_aiobotocore_application_autoscaling.type_defs import DescribeScalableTargetsResponseTypeDef


session = get_session()

async with session.create_client("application-autoscaling") as client:
    client: ApplicationAutoScalingClient
    paginator: DescribeScalableTargetsPaginator = client.get_paginator("describe_scalable_targets")
    async for item in paginator.paginate(...):
        item: DescribeScalableTargetsResponseTypeDef
        print(item)
```


