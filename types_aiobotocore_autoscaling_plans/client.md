<a id="autoscalingplansclient-for-aiobotocore-autoscalingplans-module"></a>

# AutoScalingPlansClient for aiobotocore AutoScalingPlans module

> [Index](..) > [AutoScalingPlans](.) > AutoScalingPlansClient

Auto-generated documentation for
[AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
type annotations stubs module
[types-aiobotocore-autoscaling-plans](https://pypi.org/project/types-aiobotocore-autoscaling-plans/).

- [AutoScalingPlansClient for aiobotocore AutoScalingPlans module](#autoscalingplansclient-for-aiobotocore-autoscalingplans-module)
  - [AutoScalingPlansClient](#autoscalingplansclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_scaling_plan](#create_scaling_plan)
    - [delete_scaling_plan](#delete_scaling_plan)
    - [describe_scaling_plan_resources](#describe_scaling_plan_resources)
    - [describe_scaling_plans](#describe_scaling_plans)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_scaling_plan_resource_forecast_data](#get_scaling_plan_resource_forecast_data)
    - [update_scaling_plan](#update_scaling_plan)
    - [get_paginator](#get_paginator)

<a id="autoscalingplansclient"></a>

## AutoScalingPlansClient

Type annotations for `aiobotocore.create_client("autoscaling-plans")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_autoscaling_plans.client import AutoScalingPlansClient

def get_autoscaling-plans_client() -> AutoScalingPlansClient:
    return Session().client("autoscaling-plans")
```

Boto3 documentation:
[AutoScalingPlans.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_autoscaling_plans.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConcurrentUpdateException`
- `Exceptions.InternalServiceException`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.LimitExceededException`
- `Exceptions.ObjectNotFoundException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

AutoScalingPlansClient exceptions.

Type annotations for
`aiobotocore.create_client("autoscaling-plans").exceptions` method.

Boto3 documentation:
[AutoScalingPlans.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`aiobotocore.create_client("autoscaling-plans").can_paginate` method.

Boto3 documentation:
[AutoScalingPlans.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_scaling_plan"></a>

### create_scaling_plan

Creates a scaling plan.

Type annotations for
`aiobotocore.create_client("autoscaling-plans").create_scaling_plan` method.

Boto3 documentation:
[AutoScalingPlans.Client.create_scaling_plan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)

Asynchronous method. Use `await create_scaling_plan(...)` for a synchronous
call.

Arguments mapping described in
[CreateScalingPlanRequestRequestTypeDef](./type_defs.md#createscalingplanrequestrequesttypedef).

Keyword-only arguments:

- `ScalingPlanName`: `str` *(required)*
- `ApplicationSource`:
  [ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef)
  *(required)*
- `ScalingInstructions`:
  `Sequence`\[[ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef)\]
  *(required)*

Returns a `Coroutine` for
[CreateScalingPlanResponseTypeDef](./type_defs.md#createscalingplanresponsetypedef).

<a id="delete_scaling_plan"></a>

### delete_scaling_plan

Deletes the specified scaling plan.

Type annotations for
`aiobotocore.create_client("autoscaling-plans").delete_scaling_plan` method.

Boto3 documentation:
[AutoScalingPlans.Client.delete_scaling_plan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.delete_scaling_plan)

Asynchronous method. Use `await delete_scaling_plan(...)` for a synchronous
call.

Arguments mapping described in
[DeleteScalingPlanRequestRequestTypeDef](./type_defs.md#deletescalingplanrequestrequesttypedef).

Keyword-only arguments:

- `ScalingPlanName`: `str` *(required)*
- `ScalingPlanVersion`: `int` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_scaling_plan_resources"></a>

### describe_scaling_plan_resources

Describes the scalable resources in the specified scaling plan.

Type annotations for
`aiobotocore.create_client("autoscaling-plans").describe_scaling_plan_resources`
method.

Boto3 documentation:
[AutoScalingPlans.Client.describe_scaling_plan_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plan_resources)

Asynchronous method. Use `await describe_scaling_plan_resources(...)` for a
synchronous call.

Arguments mapping described in
[DescribeScalingPlanResourcesRequestRequestTypeDef](./type_defs.md#describescalingplanresourcesrequestrequesttypedef).

Keyword-only arguments:

- `ScalingPlanName`: `str` *(required)*
- `ScalingPlanVersion`: `int` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeScalingPlanResourcesResponseTypeDef](./type_defs.md#describescalingplanresourcesresponsetypedef).

<a id="describe_scaling_plans"></a>

### describe_scaling_plans

Describes one or more of your scaling plans.

Type annotations for
`aiobotocore.create_client("autoscaling-plans").describe_scaling_plans` method.

Boto3 documentation:
[AutoScalingPlans.Client.describe_scaling_plans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)

Asynchronous method. Use `await describe_scaling_plans(...)` for a synchronous
call.

Arguments mapping described in
[DescribeScalingPlansRequestRequestTypeDef](./type_defs.md#describescalingplansrequestrequesttypedef).

Keyword-only arguments:

- `ScalingPlanNames`: `Sequence`\[`str`\]
- `ScalingPlanVersion`: `int`
- `ApplicationSources`:
  `Sequence`\[[ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef)\]
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeScalingPlansResponseTypeDef](./type_defs.md#describescalingplansresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("autoscaling-plans").generate_presigned_url` method.

Boto3 documentation:
[AutoScalingPlans.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_scaling_plan_resource_forecast_data"></a>

### get_scaling_plan_resource_forecast_data

Retrieves the forecast data for a scalable resource.

Type annotations for
`aiobotocore.create_client("autoscaling-plans").get_scaling_plan_resource_forecast_data`
method.

Boto3 documentation:
[AutoScalingPlans.Client.get_scaling_plan_resource_forecast_data](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.get_scaling_plan_resource_forecast_data)

Asynchronous method. Use `await get_scaling_plan_resource_forecast_data(...)`
for a synchronous call.

Arguments mapping described in
[GetScalingPlanResourceForecastDataRequestRequestTypeDef](./type_defs.md#getscalingplanresourceforecastdatarequestrequesttypedef).

Keyword-only arguments:

- `ScalingPlanName`: `str` *(required)*
- `ScalingPlanVersion`: `int` *(required)*
- `ServiceNamespace`:
  [ServiceNamespaceType](./literals.md#servicenamespacetype) *(required)*
- `ResourceId`: `str` *(required)*
- `ScalableDimension`:
  [ScalableDimensionType](./literals.md#scalabledimensiontype) *(required)*
- `ForecastDataType`:
  [ForecastDataTypeType](./literals.md#forecastdatatypetype) *(required)*
- `StartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\] *(required)*

Returns a `Coroutine` for
[GetScalingPlanResourceForecastDataResponseTypeDef](./type_defs.md#getscalingplanresourceforecastdataresponsetypedef).

<a id="update_scaling_plan"></a>

### update_scaling_plan

Updates the specified scaling plan.

Type annotations for
`aiobotocore.create_client("autoscaling-plans").update_scaling_plan` method.

Boto3 documentation:
[AutoScalingPlans.Client.update_scaling_plan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)

Asynchronous method. Use `await update_scaling_plan(...)` for a synchronous
call.

Arguments mapping described in
[UpdateScalingPlanRequestRequestTypeDef](./type_defs.md#updatescalingplanrequestrequesttypedef).

Keyword-only arguments:

- `ScalingPlanName`: `str` *(required)*
- `ScalingPlanVersion`: `int` *(required)*
- `ApplicationSource`:
  [ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef)
- `ScalingInstructions`:
  `Sequence`\[[ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef)\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="get_paginator"></a>

### get_paginator

Type annotations for
`aiobotocore.create_client("autoscaling-plans").get_paginator` method with
overloads.

- `client.get_paginator("describe_scaling_plan_resources")` ->
  [DescribeScalingPlanResourcesPaginator](./paginators.md#describescalingplanresourcespaginator)
- `client.get_paginator("describe_scaling_plans")` ->
  [DescribeScalingPlansPaginator](./paginators.md#describescalingplanspaginator)
