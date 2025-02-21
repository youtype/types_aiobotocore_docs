# Paginators

> [Index](../README.md) > [AutoScaling](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#autoscaling)
    type annotations stubs module [types-aiobotocore-autoscaling](https://pypi.org/project/types-aiobotocore-autoscaling/).

## DescribeAutoScalingGroupsPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_auto_scaling_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribeAutoScalingGroups.html#AutoScaling.Paginator.DescribeAutoScalingGroups)

```python
# DescribeAutoScalingGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeAutoScalingGroupsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribeAutoScalingGroupsPaginator = client.get_paginator("describe_auto_scaling_groups")  # (2)
    async for item in paginator.paginate(...):
        item: AutoScalingGroupsTypeTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeAutoScalingGroupsPaginator](./paginators.md#describeautoscalinggroupspaginator)
3. item: [:material-code-braces: AutoScalingGroupsTypeTypeDef](./type_defs.md#autoscalinggroupstypetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAutoScalingGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AutoScalingGroupNames: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[AutoScalingGroupsTypeTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: AutoScalingGroupsTypeTypeDef](./type_defs.md#autoscalinggroupstypetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: AutoScalingGroupNamesTypePaginateTypeDef = {  # (1)
    "AutoScalingGroupNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: AutoScalingGroupNamesTypePaginateTypeDef](./type_defs.md#autoscalinggroupnamestypepaginatetypedef) 
## DescribeAutoScalingInstancesPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_auto_scaling_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribeAutoScalingInstances.html#AutoScaling.Paginator.DescribeAutoScalingInstances)

```python
# DescribeAutoScalingInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeAutoScalingInstancesPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribeAutoScalingInstancesPaginator = client.get_paginator("describe_auto_scaling_instances")  # (2)
    async for item in paginator.paginate(...):
        item: AutoScalingInstancesTypeTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeAutoScalingInstancesPaginator](./paginators.md#describeautoscalinginstancespaginator)
3. item: [:material-code-braces: AutoScalingInstancesTypeTypeDef](./type_defs.md#autoscalinginstancestypetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAutoScalingInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[AutoScalingInstancesTypeTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: AutoScalingInstancesTypeTypeDef](./type_defs.md#autoscalinginstancestypetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAutoScalingInstancesTypePaginateTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAutoScalingInstancesTypePaginateTypeDef](./type_defs.md#describeautoscalinginstancestypepaginatetypedef) 
## DescribeLaunchConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_launch_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribeLaunchConfigurations.html#AutoScaling.Paginator.DescribeLaunchConfigurations)

```python
# DescribeLaunchConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeLaunchConfigurationsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribeLaunchConfigurationsPaginator = client.get_paginator("describe_launch_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: LaunchConfigurationsTypeTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeLaunchConfigurationsPaginator](./paginators.md#describelaunchconfigurationspaginator)
3. item: [:material-code-braces: LaunchConfigurationsTypeTypeDef](./type_defs.md#launchconfigurationstypetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLaunchConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LaunchConfigurationNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[LaunchConfigurationsTypeTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: LaunchConfigurationsTypeTypeDef](./type_defs.md#launchconfigurationstypetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: LaunchConfigurationNamesTypePaginateTypeDef = {  # (1)
    "LaunchConfigurationNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: LaunchConfigurationNamesTypePaginateTypeDef](./type_defs.md#launchconfigurationnamestypepaginatetypedef) 
## DescribeLoadBalancerTargetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_load_balancer_target_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribeLoadBalancerTargetGroups.html#AutoScaling.Paginator.DescribeLoadBalancerTargetGroups)

```python
# DescribeLoadBalancerTargetGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeLoadBalancerTargetGroupsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribeLoadBalancerTargetGroupsPaginator = client.get_paginator("describe_load_balancer_target_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLoadBalancerTargetGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeLoadBalancerTargetGroupsPaginator](./paginators.md#describeloadbalancertargetgroupspaginator)
3. item: [:material-code-braces: DescribeLoadBalancerTargetGroupsResponseTypeDef](./type_defs.md#describeloadbalancertargetgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLoadBalancerTargetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AutoScalingGroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeLoadBalancerTargetGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeLoadBalancerTargetGroupsResponseTypeDef](./type_defs.md#describeloadbalancertargetgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLoadBalancerTargetGroupsRequestPaginateTypeDef = {  # (1)
    "AutoScalingGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBalancerTargetGroupsRequestPaginateTypeDef](./type_defs.md#describeloadbalancertargetgroupsrequestpaginatetypedef) 
## DescribeLoadBalancersPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_load_balancers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribeLoadBalancers.html#AutoScaling.Paginator.DescribeLoadBalancers)

```python
# DescribeLoadBalancersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeLoadBalancersPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribeLoadBalancersPaginator = client.get_paginator("describe_load_balancers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLoadBalancersResponseTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeLoadBalancersPaginator](./paginators.md#describeloadbalancerspaginator)
3. item: [:material-code-braces: DescribeLoadBalancersResponseTypeDef](./type_defs.md#describeloadbalancersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLoadBalancersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AutoScalingGroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeLoadBalancersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeLoadBalancersResponseTypeDef](./type_defs.md#describeloadbalancersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLoadBalancersRequestPaginateTypeDef = {  # (1)
    "AutoScalingGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLoadBalancersRequestPaginateTypeDef](./type_defs.md#describeloadbalancersrequestpaginatetypedef) 
## DescribeNotificationConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_notification_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribeNotificationConfigurations.html#AutoScaling.Paginator.DescribeNotificationConfigurations)

```python
# DescribeNotificationConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeNotificationConfigurationsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribeNotificationConfigurationsPaginator = client.get_paginator("describe_notification_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNotificationConfigurationsAnswerTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeNotificationConfigurationsPaginator](./paginators.md#describenotificationconfigurationspaginator)
3. item: [:material-code-braces: DescribeNotificationConfigurationsAnswerTypeDef](./type_defs.md#describenotificationconfigurationsanswertypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNotificationConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AutoScalingGroupNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeNotificationConfigurationsAnswerTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeNotificationConfigurationsAnswerTypeDef](./type_defs.md#describenotificationconfigurationsanswertypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNotificationConfigurationsTypePaginateTypeDef = {  # (1)
    "AutoScalingGroupNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNotificationConfigurationsTypePaginateTypeDef](./type_defs.md#describenotificationconfigurationstypepaginatetypedef) 
## DescribePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribePolicies.html#AutoScaling.Paginator.DescribePolicies)

```python
# DescribePoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribePoliciesPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribePoliciesPaginator = client.get_paginator("describe_policies")  # (2)
    async for item in paginator.paginate(...):
        item: PoliciesTypeTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribePoliciesPaginator](./paginators.md#describepoliciespaginator)
3. item: [:material-code-braces: PoliciesTypeTypeDef](./type_defs.md#policiestypetypedef) 


### paginate

Type annotations and code completion for `#!python DescribePoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AutoScalingGroupName: str = ...,
    PolicyNames: Sequence[str] = ...,
    PolicyTypes: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[PoliciesTypeTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: PoliciesTypeTypeDef](./type_defs.md#policiestypetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribePoliciesTypePaginateTypeDef = {  # (1)
    "AutoScalingGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePoliciesTypePaginateTypeDef](./type_defs.md#describepoliciestypepaginatetypedef) 
## DescribeScalingActivitiesPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_scaling_activities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribeScalingActivities.html#AutoScaling.Paginator.DescribeScalingActivities)

```python
# DescribeScalingActivitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeScalingActivitiesPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribeScalingActivitiesPaginator = client.get_paginator("describe_scaling_activities")  # (2)
    async for item in paginator.paginate(...):
        item: ActivitiesTypeTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeScalingActivitiesPaginator](./paginators.md#describescalingactivitiespaginator)
3. item: [:material-code-braces: ActivitiesTypeTypeDef](./type_defs.md#activitiestypetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeScalingActivitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ActivityIds: Sequence[str] = ...,
    AutoScalingGroupName: str = ...,
    IncludeDeletedGroups: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ActivitiesTypeTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ActivitiesTypeTypeDef](./type_defs.md#activitiestypetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScalingActivitiesTypePaginateTypeDef = {  # (1)
    "ActivityIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScalingActivitiesTypePaginateTypeDef](./type_defs.md#describescalingactivitiestypepaginatetypedef) 
## DescribeScheduledActionsPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_scheduled_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribeScheduledActions.html#AutoScaling.Paginator.DescribeScheduledActions)

```python
# DescribeScheduledActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeScheduledActionsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribeScheduledActionsPaginator = client.get_paginator("describe_scheduled_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ScheduledActionsTypeTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeScheduledActionsPaginator](./paginators.md#describescheduledactionspaginator)
3. item: [:material-code-braces: ScheduledActionsTypeTypeDef](./type_defs.md#scheduledactionstypetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeScheduledActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AutoScalingGroupName: str = ...,
    ScheduledActionNames: Sequence[str] = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ScheduledActionsTypeTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ScheduledActionsTypeTypeDef](./type_defs.md#scheduledactionstypetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScheduledActionsTypePaginateTypeDef = {  # (1)
    "AutoScalingGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledActionsTypePaginateTypeDef](./type_defs.md#describescheduledactionstypepaginatetypedef) 
## DescribeTagsPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribeTags.html#AutoScaling.Paginator.DescribeTags)

```python
# DescribeTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeTagsPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")  # (2)
    async for item in paginator.paginate(...):
        item: TagsTypeTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeTagsPaginator](./paginators.md#describetagspaginator)
3. item: [:material-code-braces: TagsTypeTypeDef](./type_defs.md#tagstypetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[TagsTypeTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: TagsTypeTypeDef](./type_defs.md#tagstypetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTagsTypePaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTagsTypePaginateTypeDef](./type_defs.md#describetagstypepaginatetypedef) 
## DescribeWarmPoolPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling").get_paginator("describe_warm_pool")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling/paginator/DescribeWarmPool.html#AutoScaling.Paginator.DescribeWarmPool)

```python
# DescribeWarmPoolPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling.paginator import DescribeWarmPoolPaginator

session = get_session()
async with session.create_client("autoscaling") as client:  # (1)
    paginator: DescribeWarmPoolPaginator = client.get_paginator("describe_warm_pool")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeWarmPoolAnswerTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingClient](./client.md)
2. paginator: [DescribeWarmPoolPaginator](./paginators.md#describewarmpoolpaginator)
3. item: [:material-code-braces: DescribeWarmPoolAnswerTypeDef](./type_defs.md#describewarmpoolanswertypedef) 


### paginate

Type annotations and code completion for `#!python DescribeWarmPoolPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AutoScalingGroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeWarmPoolAnswerTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeWarmPoolAnswerTypeDef](./type_defs.md#describewarmpoolanswertypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeWarmPoolTypePaginateTypeDef = {  # (1)
    "AutoScalingGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeWarmPoolTypePaginateTypeDef](./type_defs.md#describewarmpooltypepaginatetypedef) 
