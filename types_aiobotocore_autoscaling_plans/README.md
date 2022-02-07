<a id="type-annotations-for-aiobotocore-autoscalingplans-module"></a>

# Type annotations for aiobotocore AutoScalingPlans module

> [Index](..) > AutoScalingPlans

Auto-generated documentation for
[AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans)
type annotations stubs module
[types-aiobotocore-autoscaling-plans](https://pypi.org/project/types-aiobotocore-autoscaling-plans/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[autoscaling-plans]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[autoscaling-plans]'

# standalone installation
pip install types-aiobotocore-autoscaling-plans
```

- [Type annotations for aiobotocore AutoScalingPlans module](#type-annotations-for-aiobotocore-autoscalingplans-module)
  - [AutoScalingPlansClient](#autoscalingplansclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Paginators](#paginators)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="autoscalingplansclient"></a>

## AutoScalingPlansClient

Type annotations for `session.create_client("autoscaling-plans")` as
[AutoScalingPlansClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_autoscaling_plans.client import AutoScalingPlansClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [create_scaling_plan](./client.md#create_scaling_plan)
- [delete_scaling_plan](./client.md#delete_scaling_plan)
- [describe_scaling_plan_resources](./client.md#describe_scaling_plan_resources)
- [describe_scaling_plans](./client.md#describe_scaling_plans)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_paginator](./client.md#get_paginator)
- [get_scaling_plan_resource_forecast_data](./client.md#get_scaling_plan_resource_forecast_data)
- [update_scaling_plan](./client.md#update_scaling_plan)

<a id="exceptions"></a>

### Exceptions

AutoScalingPlansClient [exceptions](./client.md#exceptions)

- ClientError
- ConcurrentUpdateException
- InternalServiceException
- InvalidNextTokenException
- LimitExceededException
- ObjectNotFoundException
- ValidationException

<a id="paginators"></a>

## Paginators

Type annotations for [paginators](./paginators.md) from
`boto3.client("autoscaling-plans").get_paginator("...")`.

Can be used directly:

```python
from types_aiobotocore_autoscaling_plans.paginator import DescribeScalingPlanResourcesPaginator, ...
```

- [DescribeScalingPlanResourcesPaginator](./paginators.md#describescalingplanresourcespaginator)
- [DescribeScalingPlansPaginator](./paginators.md#describescalingplanspaginator)

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_autoscaling_plans.literals import DescribeScalingPlanResourcesPaginatorName, ...
```

- [DescribeScalingPlanResourcesPaginatorName](./literals.md#describescalingplanresourcespaginatorname)
- [DescribeScalingPlansPaginatorName](./literals.md#describescalingplanspaginatorname)
- [ForecastDataTypeType](./literals.md#forecastdatatypetype)
- [LoadMetricTypeType](./literals.md#loadmetrictypetype)
- [MetricStatisticType](./literals.md#metricstatistictype)
- [PolicyTypeType](./literals.md#policytypetype)
- [PredictiveScalingMaxCapacityBehaviorType](./literals.md#predictivescalingmaxcapacitybehaviortype)
- [PredictiveScalingModeType](./literals.md#predictivescalingmodetype)
- [ScalableDimensionType](./literals.md#scalabledimensiontype)
- [ScalingMetricTypeType](./literals.md#scalingmetrictypetype)
- [ScalingPlanStatusCodeType](./literals.md#scalingplanstatuscodetype)
- [ScalingPolicyUpdateBehaviorType](./literals.md#scalingpolicyupdatebehaviortype)
- [ScalingStatusCodeType](./literals.md#scalingstatuscodetype)
- [ServiceNamespaceType](./literals.md#servicenamespacetype)
- [ServiceName](./literals.md#servicename)
- [PaginatorName](./literals.md#paginatorname)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_autoscaling_plans.type_defs import ApplicationSourceTypeDef, ...
```

- [ApplicationSourceTypeDef](./type_defs.md#applicationsourcetypedef)
- [CreateScalingPlanRequestRequestTypeDef](./type_defs.md#createscalingplanrequestrequesttypedef)
- [CreateScalingPlanResponseTypeDef](./type_defs.md#createscalingplanresponsetypedef)
- [CustomizedLoadMetricSpecificationTypeDef](./type_defs.md#customizedloadmetricspecificationtypedef)
- [CustomizedScalingMetricSpecificationTypeDef](./type_defs.md#customizedscalingmetricspecificationtypedef)
- [DatapointTypeDef](./type_defs.md#datapointtypedef)
- [DeleteScalingPlanRequestRequestTypeDef](./type_defs.md#deletescalingplanrequestrequesttypedef)
- [DescribeScalingPlanResourcesRequestRequestTypeDef](./type_defs.md#describescalingplanresourcesrequestrequesttypedef)
- [DescribeScalingPlanResourcesResponseTypeDef](./type_defs.md#describescalingplanresourcesresponsetypedef)
- [DescribeScalingPlansRequestRequestTypeDef](./type_defs.md#describescalingplansrequestrequesttypedef)
- [DescribeScalingPlansResponseTypeDef](./type_defs.md#describescalingplansresponsetypedef)
- [GetScalingPlanResourceForecastDataRequestRequestTypeDef](./type_defs.md#getscalingplanresourceforecastdatarequestrequesttypedef)
- [GetScalingPlanResourceForecastDataResponseTypeDef](./type_defs.md#getscalingplanresourceforecastdataresponsetypedef)
- [MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [PredefinedLoadMetricSpecificationTypeDef](./type_defs.md#predefinedloadmetricspecificationtypedef)
- [PredefinedScalingMetricSpecificationTypeDef](./type_defs.md#predefinedscalingmetricspecificationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ScalingInstructionTypeDef](./type_defs.md#scalinginstructiontypedef)
- [ScalingPlanResourceTypeDef](./type_defs.md#scalingplanresourcetypedef)
- [ScalingPlanTypeDef](./type_defs.md#scalingplantypedef)
- [ScalingPolicyTypeDef](./type_defs.md#scalingpolicytypedef)
- [TagFilterTypeDef](./type_defs.md#tagfiltertypedef)
- [TargetTrackingConfigurationTypeDef](./type_defs.md#targettrackingconfigurationtypedef)
- [UpdateScalingPlanRequestRequestTypeDef](./type_defs.md#updatescalingplanrequestrequesttypedef)
