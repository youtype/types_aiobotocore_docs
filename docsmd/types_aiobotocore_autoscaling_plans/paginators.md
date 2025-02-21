# Paginators

> [Index](../README.md) > [AutoScalingPlans](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#autoscalingplans)
    type annotations stubs module [types-aiobotocore-autoscaling-plans](https://pypi.org/project/types-aiobotocore-autoscaling-plans/).

## DescribeScalingPlanResourcesPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling-plans").get_paginator("describe_scaling_plan_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans/paginator/DescribeScalingPlanResources.html#AutoScalingPlans.Paginator.DescribeScalingPlanResources)

```python
# DescribeScalingPlanResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling_plans.paginator import DescribeScalingPlanResourcesPaginator

session = get_session()
async with session.create_client("autoscaling-plans") as client:  # (1)
    paginator: DescribeScalingPlanResourcesPaginator = client.get_paginator("describe_scaling_plan_resources")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeScalingPlanResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingPlansClient](./client.md)
2. paginator: [DescribeScalingPlanResourcesPaginator](./paginators.md#describescalingplanresourcespaginator)
3. item: [:material-code-braces: DescribeScalingPlanResourcesResponseTypeDef](./type_defs.md#describescalingplanresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeScalingPlanResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ScalingPlanName: str,
    ScalingPlanVersion: int,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeScalingPlanResourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeScalingPlanResourcesResponseTypeDef](./type_defs.md#describescalingplanresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScalingPlanResourcesRequestPaginateTypeDef = {  # (1)
    "ScalingPlanName": ...,
    "ScalingPlanVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScalingPlanResourcesRequestPaginateTypeDef](./type_defs.md#describescalingplanresourcesrequestpaginatetypedef) 
## DescribeScalingPlansPaginator

Type annotations and code completion for `#!python session.create_client("autoscaling-plans").get_paginator("describe_scaling_plans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans/paginator/DescribeScalingPlans.html#AutoScalingPlans.Paginator.DescribeScalingPlans)

```python
# DescribeScalingPlansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_autoscaling_plans.paginator import DescribeScalingPlansPaginator

session = get_session()
async with session.create_client("autoscaling-plans") as client:  # (1)
    paginator: DescribeScalingPlansPaginator = client.get_paginator("describe_scaling_plans")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeScalingPlansResponseTypeDef
        print(item)  # (3)
```

1. client: [AutoScalingPlansClient](./client.md)
2. paginator: [DescribeScalingPlansPaginator](./paginators.md#describescalingplanspaginator)
3. item: [:material-code-braces: DescribeScalingPlansResponseTypeDef](./type_defs.md#describescalingplansresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeScalingPlansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ScalingPlanNames: Sequence[str] = ...,
    ScalingPlanVersion: int = ...,
    ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeScalingPlansResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef) [:material-code-braces: ApplicationSourceOutputTypeDef](./type_defs.md#applicationsourceoutputtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeScalingPlansResponseTypeDef](./type_defs.md#describescalingplansresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScalingPlansRequestPaginateTypeDef = {  # (1)
    "ScalingPlanNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScalingPlansRequestPaginateTypeDef](./type_defs.md#describescalingplansrequestpaginatetypedef) 
