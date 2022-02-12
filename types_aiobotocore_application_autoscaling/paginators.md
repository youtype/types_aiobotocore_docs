<a id="paginators-for-aiobotocore-applicationautoscaling-module"></a>

# Paginators for aiobotocore ApplicationAutoScaling module

> [Index](..) > [ApplicationAutoScaling](.) > Paginators

Auto-generated documentation for
[ApplicationAutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling)
type annotations stubs module
[types-aiobotocore-application-autoscaling](https://pypi.org/project/types-aiobotocore-application-autoscaling/).

- [Paginators for aiobotocore ApplicationAutoScaling module](#paginators-for-aiobotocore-applicationautoscaling-module)
  - [DescribeScalableTargetsPaginator](#describescalabletargetspaginator)
  - [DescribeScalingActivitiesPaginator](#describescalingactivitiespaginator)
  - [DescribeScalingPoliciesPaginator](#describescalingpoliciespaginator)
  - [DescribeScheduledActionsPaginator](#describescheduledactionspaginator)

<a id="describescalabletargetspaginator"></a>

## DescribeScalableTargetsPaginator

Type annotations for
`session.create_client("application-autoscaling").get_paginator("describe_scalable_targets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_application_autoscaling.paginator import DescribeScalableTargetsPaginator

session = get_session()
async with session.create_client("application-autoscaling") as client:
    client: ApplicationAutoScalingClient
    paginator: DescribeScalableTargetsPaginator = client.get_paginator("describe_scalable_targets")
```

Boto3 documentation:
[ApplicationAutoScaling.Paginator.DescribeScalableTargets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalableTargets)

Arguments for `DescribeScalableTargetsPaginator.paginate` method:

- `ServiceNamespace`:
  [ServiceNamespaceType](./literals.md#servicenamespacetype) *(required)*
- `ResourceIds`: `Sequence`\[`str`\]
- `ScalableDimension`:
  [ScalableDimensionType](./literals.md#scalabledimensiontype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeScalableTargetsPaginator.paginate` returns
`AsyncIterable`\[[DescribeScalableTargetsResponseTypeDef](./type_defs.md#describescalabletargetsresponsetypedef)\].

<a id="describescalingactivitiespaginator"></a>

## DescribeScalingActivitiesPaginator

Type annotations for
`session.create_client("application-autoscaling").get_paginator("describe_scaling_activities")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_application_autoscaling.paginator import DescribeScalingActivitiesPaginator

session = get_session()
async with session.create_client("application-autoscaling") as client:
    client: ApplicationAutoScalingClient
    paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
```

Boto3 documentation:
[ApplicationAutoScaling.Paginator.DescribeScalingActivities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingActivities)

Arguments for `DescribeScalingActivitiesPaginator.paginate` method:

- `ServiceNamespace`:
  [ServiceNamespaceType](./literals.md#servicenamespacetype) *(required)*
- `ResourceId`: `str`
- `ScalableDimension`:
  [ScalableDimensionType](./literals.md#scalabledimensiontype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeScalingActivitiesPaginator.paginate` returns
`AsyncIterable`\[[DescribeScalingActivitiesResponseTypeDef](./type_defs.md#describescalingactivitiesresponsetypedef)\].

<a id="describescalingpoliciespaginator"></a>

## DescribeScalingPoliciesPaginator

Type annotations for
`session.create_client("application-autoscaling").get_paginator("describe_scaling_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_application_autoscaling.paginator import DescribeScalingPoliciesPaginator

session = get_session()
async with session.create_client("application-autoscaling") as client:
    client: ApplicationAutoScalingClient
    paginator: DescribeScalingPoliciesPaginator = client.get_paginator("describe_scaling_policies")
```

Boto3 documentation:
[ApplicationAutoScaling.Paginator.DescribeScalingPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScalingPolicies)

Arguments for `DescribeScalingPoliciesPaginator.paginate` method:

- `ServiceNamespace`:
  [ServiceNamespaceType](./literals.md#servicenamespacetype) *(required)*
- `PolicyNames`: `Sequence`\[`str`\]
- `ResourceId`: `str`
- `ScalableDimension`:
  [ScalableDimensionType](./literals.md#scalabledimensiontype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeScalingPoliciesPaginator.paginate` returns
`AsyncIterable`\[[DescribeScalingPoliciesResponseTypeDef](./type_defs.md#describescalingpoliciesresponsetypedef)\].

<a id="describescheduledactionspaginator"></a>

## DescribeScheduledActionsPaginator

Type annotations for
`session.create_client("application-autoscaling").get_paginator("describe_scheduled_actions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_application_autoscaling.paginator import DescribeScheduledActionsPaginator

session = get_session()
async with session.create_client("application-autoscaling") as client:
    client: ApplicationAutoScalingClient
    paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
```

Boto3 documentation:
[ApplicationAutoScaling.Paginator.DescribeScheduledActions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Paginator.DescribeScheduledActions)

Arguments for `DescribeScheduledActionsPaginator.paginate` method:

- `ServiceNamespace`:
  [ServiceNamespaceType](./literals.md#servicenamespacetype) *(required)*
- `ScheduledActionNames`: `Sequence`\[`str`\]
- `ResourceId`: `str`
- `ScalableDimension`:
  [ScalableDimensionType](./literals.md#scalabledimensiontype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeScheduledActionsPaginator.paginate` returns
`AsyncIterable`\[[DescribeScheduledActionsResponseTypeDef](./type_defs.md#describescheduledactionsresponsetypedef)\].
