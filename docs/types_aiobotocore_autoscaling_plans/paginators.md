<a id="paginators-for-aiobotocore-autoscalingplans-module"></a>

# Paginators for aiobotocore AutoScalingPlans module

> [Index](../README.md) > [AutoScalingPlans](./README.md) > Paginators

Auto-generated documentation for
[AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
type annotations stubs module
[types-aiobotocore-autoscaling-plans](https://pypi.org/project/types-aiobotocore-autoscaling-plans/).

- [Paginators for aiobotocore AutoScalingPlans module](#paginators-for-aiobotocore-autoscalingplans-module)
  - [DescribeScalingPlanResourcesPaginator](#describescalingplanresourcespaginator)
  - [DescribeScalingPlansPaginator](#describescalingplanspaginator)

<a id="describescalingplanresourcespaginator"></a>

## DescribeScalingPlanResourcesPaginator

Type annotations for
`session.create_client("autoscaling-plans").get_paginator("describe_scaling_plan_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling_plans.paginator import DescribeScalingPlanResourcesPaginator

session = get_session()
async with session.create_client("autoscaling-plans") as client:
    client: AutoScalingPlansClient
    paginator: DescribeScalingPlanResourcesPaginator = client.get_paginator("describe_scaling_plan_resources")
```

Boto3 documentation:
[AutoScalingPlans.Paginator.DescribeScalingPlanResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources)

Arguments for `DescribeScalingPlanResourcesPaginator.paginate` method:

- `ScalingPlanName`: `str` *(required)*
- `ScalingPlanVersion`: `int` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeScalingPlanResourcesPaginator.paginate` returns
`AsyncIterator`\[[DescribeScalingPlanResourcesResponseTypeDef](./type_defs.md#describescalingplanresourcesresponsetypedef)\].

<a id="describescalingplanspaginator"></a>

## DescribeScalingPlansPaginator

Type annotations for
`session.create_client("autoscaling-plans").get_paginator("describe_scaling_plans")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling_plans.paginator import DescribeScalingPlansPaginator

session = get_session()
async with session.create_client("autoscaling-plans") as client:
    client: AutoScalingPlansClient
    paginator: DescribeScalingPlansPaginator = client.get_paginator("describe_scaling_plans")
```

Boto3 documentation:
[AutoScalingPlans.Paginator.DescribeScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans)

Arguments for `DescribeScalingPlansPaginator.paginate` method:

- `ScalingPlanNames`: `Sequence`\[`str`\]
- `ScalingPlanVersion`: `int`
- `ApplicationSources`:
  `Sequence`\[[ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeScalingPlansPaginator.paginate` returns
`AsyncIterator`\[[DescribeScalingPlansResponseTypeDef](./type_defs.md#describescalingplansresponsetypedef)\].
