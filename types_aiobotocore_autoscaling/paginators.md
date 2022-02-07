<a id="paginators-for-aiobotocore-autoscaling-module"></a>

# Paginators for aiobotocore AutoScaling module

> [Index](..) > [AutoScaling](.) > Paginators

Auto-generated documentation for
[AutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling)
type annotations stubs module
[types-aiobotocore-autoscaling](https://pypi.org/project/types-aiobotocore-autoscaling/).

- [Paginators for aiobotocore AutoScaling module](#paginators-for-aiobotocore-autoscaling-module)
  - [DescribeAutoScalingGroupsPaginator](#describeautoscalinggroupspaginator)
  - [DescribeAutoScalingInstancesPaginator](#describeautoscalinginstancespaginator)
  - [DescribeLaunchConfigurationsPaginator](#describelaunchconfigurationspaginator)
  - [DescribeLoadBalancerTargetGroupsPaginator](#describeloadbalancertargetgroupspaginator)
  - [DescribeLoadBalancersPaginator](#describeloadbalancerspaginator)
  - [DescribeNotificationConfigurationsPaginator](#describenotificationconfigurationspaginator)
  - [DescribePoliciesPaginator](#describepoliciespaginator)
  - [DescribeScalingActivitiesPaginator](#describescalingactivitiespaginator)
  - [DescribeScheduledActionsPaginator](#describescheduledactionspaginator)
  - [DescribeTagsPaginator](#describetagspaginator)

<a id="describeautoscalinggroupspaginator"></a>

## DescribeAutoScalingGroupsPaginator

Type annotations for
`session.create_client("autoscaling").get_paginator("describe_auto_scaling_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeAutoScalingGroupsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:
    client: AutoScalingClient
    paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator("describe_auto_scaling_groups")
```

Boto3 documentation:
[AutoScaling.Paginator.DescribeAutoScalingGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingGroups)

Arguments for `DescribeAutoScalingGroupsPaginator.paginate` method:

- `AutoScalingGroupNames`: `Sequence`\[`str`\]
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAutoScalingGroupsPaginator.paginate` returns
`_PageIterator`\[[AutoScalingGroupsTypeTypeDef](./type_defs.md#autoscalinggroupstypetypedef)\].

<a id="describeautoscalinginstancespaginator"></a>

## DescribeAutoScalingInstancesPaginator

Type annotations for
`session.create_client("autoscaling").get_paginator("describe_auto_scaling_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeAutoScalingInstancesPaginator

session = get_session()
async with session.create_client("autoscaling") as client:
    client: AutoScalingClient
    paginator: DescribeAutoScalingInstancesPaginator = client.get_paginator("describe_auto_scaling_instances")
```

Boto3 documentation:
[AutoScaling.Paginator.DescribeAutoScalingInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeAutoScalingInstances)

Arguments for `DescribeAutoScalingInstancesPaginator.paginate` method:

- `InstanceIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAutoScalingInstancesPaginator.paginate` returns
`_PageIterator`\[[AutoScalingInstancesTypeTypeDef](./type_defs.md#autoscalinginstancestypetypedef)\].

<a id="describelaunchconfigurationspaginator"></a>

## DescribeLaunchConfigurationsPaginator

Type annotations for
`session.create_client("autoscaling").get_paginator("describe_launch_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeLaunchConfigurationsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:
    client: AutoScalingClient
    paginator: DescribeLaunchConfigurationsPaginator = client.get_paginator("describe_launch_configurations")
```

Boto3 documentation:
[AutoScaling.Paginator.DescribeLaunchConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLaunchConfigurations)

Arguments for `DescribeLaunchConfigurationsPaginator.paginate` method:

- `LaunchConfigurationNames`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeLaunchConfigurationsPaginator.paginate` returns
`_PageIterator`\[[LaunchConfigurationsTypeTypeDef](./type_defs.md#launchconfigurationstypetypedef)\].

<a id="describeloadbalancertargetgroupspaginator"></a>

## DescribeLoadBalancerTargetGroupsPaginator

Type annotations for
`session.create_client("autoscaling").get_paginator("describe_load_balancer_target_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeLoadBalancerTargetGroupsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:
    client: AutoScalingClient
    paginator: DescribeLoadBalancerTargetGroupsPaginator = client.get_paginator("describe_load_balancer_target_groups")
```

Boto3 documentation:
[AutoScaling.Paginator.DescribeLoadBalancerTargetGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups)

Arguments for `DescribeLoadBalancerTargetGroupsPaginator.paginate` method:

- `AutoScalingGroupName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeLoadBalancerTargetGroupsPaginator.paginate` returns
`_PageIterator`\[[DescribeLoadBalancerTargetGroupsResponseTypeDef](./type_defs.md#describeloadbalancertargetgroupsresponsetypedef)\].

<a id="describeloadbalancerspaginator"></a>

## DescribeLoadBalancersPaginator

Type annotations for
`session.create_client("autoscaling").get_paginator("describe_load_balancers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeLoadBalancersPaginator

session = get_session()
async with session.create_client("autoscaling") as client:
    client: AutoScalingClient
    paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")
```

Boto3 documentation:
[AutoScaling.Paginator.DescribeLoadBalancers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeLoadBalancers)

Arguments for `DescribeLoadBalancersPaginator.paginate` method:

- `AutoScalingGroupName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeLoadBalancersPaginator.paginate` returns
`_PageIterator`\[[DescribeLoadBalancersResponseTypeDef](./type_defs.md#describeloadbalancersresponsetypedef)\].

<a id="describenotificationconfigurationspaginator"></a>

## DescribeNotificationConfigurationsPaginator

Type annotations for
`session.create_client("autoscaling").get_paginator("describe_notification_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeNotificationConfigurationsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:
    client: AutoScalingClient
    paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")
```

Boto3 documentation:
[AutoScaling.Paginator.DescribeNotificationConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeNotificationConfigurations)

Arguments for `DescribeNotificationConfigurationsPaginator.paginate` method:

- `AutoScalingGroupNames`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeNotificationConfigurationsPaginator.paginate` returns
`_PageIterator`\[[DescribeNotificationConfigurationsAnswerTypeDef](./type_defs.md#describenotificationconfigurationsanswertypedef)\].

<a id="describepoliciespaginator"></a>

## DescribePoliciesPaginator

Type annotations for
`session.create_client("autoscaling").get_paginator("describe_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribePoliciesPaginator

session = get_session()
async with session.create_client("autoscaling") as client:
    client: AutoScalingClient
    paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")
```

Boto3 documentation:
[AutoScaling.Paginator.DescribePolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribePolicies)

Arguments for `DescribePoliciesPaginator.paginate` method:

- `AutoScalingGroupName`: `str`
- `PolicyNames`: `Sequence`\[`str`\]
- `PolicyTypes`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribePoliciesPaginator.paginate` returns
`_PageIterator`\[[PoliciesTypeTypeDef](./type_defs.md#policiestypetypedef)\].

<a id="describescalingactivitiespaginator"></a>

## DescribeScalingActivitiesPaginator

Type annotations for
`session.create_client("autoscaling").get_paginator("describe_scaling_activities")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeScalingActivitiesPaginator

session = get_session()
async with session.create_client("autoscaling") as client:
    client: AutoScalingClient
    paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")
```

Boto3 documentation:
[AutoScaling.Paginator.DescribeScalingActivities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScalingActivities)

Arguments for `DescribeScalingActivitiesPaginator.paginate` method:

- `ActivityIds`: `Sequence`\[`str`\]
- `AutoScalingGroupName`: `str`
- `IncludeDeletedGroups`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeScalingActivitiesPaginator.paginate` returns
`_PageIterator`\[[ActivitiesTypeTypeDef](./type_defs.md#activitiestypetypedef)\].

<a id="describescheduledactionspaginator"></a>

## DescribeScheduledActionsPaginator

Type annotations for
`session.create_client("autoscaling").get_paginator("describe_scheduled_actions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeScheduledActionsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:
    client: AutoScalingClient
    paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")
```

Boto3 documentation:
[AutoScaling.Paginator.DescribeScheduledActions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeScheduledActions)

Arguments for `DescribeScheduledActionsPaginator.paginate` method:

- `AutoScalingGroupName`: `str`
- `ScheduledActionNames`: `Sequence`\[`str`\]
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeScheduledActionsPaginator.paginate` returns
`_PageIterator`\[[ScheduledActionsTypeTypeDef](./type_defs.md#scheduledactionstypetypedef)\].

<a id="describetagspaginator"></a>

## DescribeTagsPaginator

Type annotations for
`session.create_client("autoscaling").get_paginator("describe_tags")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeTagsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:
    client: AutoScalingClient
    paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")
```

Boto3 documentation:
[AutoScaling.Paginator.DescribeTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#AutoScaling.Paginator.DescribeTags)

Arguments for `DescribeTagsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeTagsPaginator.paginate` returns
`_PageIterator`\[[TagsTypeTypeDef](./type_defs.md#tagstypetypedef)\].
