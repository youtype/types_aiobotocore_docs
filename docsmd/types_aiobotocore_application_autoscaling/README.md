# ApplicationAutoScaling module

> [Index](../README.md) > ApplicationAutoScaling


!!! note ""

    Auto-generated documentation for [ApplicationAutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#applicationautoscaling)
    type annotations stubs module [types-aiobotocore-application-autoscaling](https://pypi.org/project/types-aiobotocore-application-autoscaling/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ApplicationAutoScaling` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ApplicationAutoScaling` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[application-autoscaling]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[application-autoscaling]'

# standalone installation
python -m pip install types-aiobotocore-application-autoscaling
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-application-autoscaling
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ApplicationAutoScalingClient

Type annotations and code completion for  `#!python session.create_client("application-autoscaling")` as [ApplicationAutoScalingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client)

```python
# ApplicationAutoScalingClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_application_autoscaling.client import ApplicationAutoScalingClient


session = get_session()
async with session.create_client("application-autoscaling") as client:
    client: ApplicationAutoScalingClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("application-autoscaling").get_paginator("...")`.

```python
# DescribeScalableTargetsPaginator usage example

from types_aiobotocore_application_autoscaling.paginator import DescribeScalableTargetsPaginator

def get_describe_scalable_targets_paginator() -> DescribeScalableTargetsPaginator:
    return client.get_paginator("describe_scalable_targets"))
```

- [DescribeScalableTargetsPaginator](./paginators.md#describescalabletargetspaginator)
- [DescribeScalingActivitiesPaginator](./paginators.md#describescalingactivitiespaginator)
- [DescribeScalingPoliciesPaginator](./paginators.md#describescalingpoliciespaginator)
- [DescribeScheduledActionsPaginator](./paginators.md#describescheduledactionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AdjustmentTypeType usage example

from types_aiobotocore_application_autoscaling.literals import AdjustmentTypeType

def get_value() -> AdjustmentTypeType:
    return "ChangeInCapacity"
```

- [AdjustmentTypeType](./literals.md#adjustmenttypetype)
- [DescribeScalableTargetsPaginatorName](./literals.md#describescalabletargetspaginatorname)
- [DescribeScalingActivitiesPaginatorName](./literals.md#describescalingactivitiespaginatorname)
- [DescribeScalingPoliciesPaginatorName](./literals.md#describescalingpoliciespaginatorname)
- [DescribeScheduledActionsPaginatorName](./literals.md#describescheduledactionspaginatorname)
- [MetricAggregationTypeType](./literals.md#metricaggregationtypetype)
- [MetricStatisticType](./literals.md#metricstatistictype)
- [MetricTypeType](./literals.md#metrictypetype)
- [PolicyTypeType](./literals.md#policytypetype)
- [PredictiveScalingMaxCapacityBreachBehaviorType](./literals.md#predictivescalingmaxcapacitybreachbehaviortype)
- [PredictiveScalingModeType](./literals.md#predictivescalingmodetype)
- [ScalableDimensionType](./literals.md#scalabledimensiontype)
- [ScalingActivityStatusCodeType](./literals.md#scalingactivitystatuscodetype)
- [ServiceNamespaceType](./literals.md#servicenamespacetype)
- [ApplicationAutoScalingServiceName](./literals.md#applicationautoscalingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AlarmTypeDef](./type_defs.md#alarmtypedef)
- [CapacityForecastTypeDef](./type_defs.md#capacityforecasttypedef)
- [MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef)
- [DeleteScalingPolicyRequestRequestTypeDef](./type_defs.md#deletescalingpolicyrequestrequesttypedef)
- [DeleteScheduledActionRequestRequestTypeDef](./type_defs.md#deletescheduledactionrequestrequesttypedef)
- [DeregisterScalableTargetRequestRequestTypeDef](./type_defs.md#deregisterscalabletargetrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeScalableTargetsRequestRequestTypeDef](./type_defs.md#describescalabletargetsrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DescribeScalingActivitiesRequestRequestTypeDef](./type_defs.md#describescalingactivitiesrequestrequesttypedef)
- [DescribeScalingPoliciesRequestRequestTypeDef](./type_defs.md#describescalingpoliciesrequestrequesttypedef)
- [DescribeScheduledActionsRequestRequestTypeDef](./type_defs.md#describescheduledactionsrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [NotScaledReasonTypeDef](./type_defs.md#notscaledreasontypedef)
- [PredefinedMetricSpecificationTypeDef](./type_defs.md#predefinedmetricspecificationtypedef)
- [PredictiveScalingMetricDimensionTypeDef](./type_defs.md#predictivescalingmetricdimensiontypedef)
- [PredictiveScalingPredefinedLoadMetricSpecificationTypeDef](./type_defs.md#predictivescalingpredefinedloadmetricspecificationtypedef)
- [PredictiveScalingPredefinedMetricPairSpecificationTypeDef](./type_defs.md#predictivescalingpredefinedmetricpairspecificationtypedef)
- [PredictiveScalingPredefinedScalingMetricSpecificationTypeDef](./type_defs.md#predictivescalingpredefinedscalingmetricspecificationtypedef)
- [ScalableTargetActionTypeDef](./type_defs.md#scalabletargetactiontypedef)
- [SuspendedStateTypeDef](./type_defs.md#suspendedstatetypedef)
- [StepAdjustmentTypeDef](./type_defs.md#stepadjustmenttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TargetTrackingMetricDimensionTypeDef](./type_defs.md#targettrackingmetricdimensiontypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef](./type_defs.md#describescalabletargetsrequestdescribescalabletargetspaginatetypedef)
- [DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef](./type_defs.md#describescalingactivitiesrequestdescribescalingactivitiespaginatetypedef)
- [DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef](./type_defs.md#describescalingpoliciesrequestdescribescalingpoliciespaginatetypedef)
- [DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef](./type_defs.md#describescheduledactionsrequestdescribescheduledactionspaginatetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutScalingPolicyResponseTypeDef](./type_defs.md#putscalingpolicyresponsetypedef)
- [RegisterScalableTargetResponseTypeDef](./type_defs.md#registerscalabletargetresponsetypedef)
- [GetPredictiveScalingForecastRequestRequestTypeDef](./type_defs.md#getpredictivescalingforecastrequestrequesttypedef)
- [ScalingActivityTypeDef](./type_defs.md#scalingactivitytypedef)
- [PredictiveScalingMetricOutputTypeDef](./type_defs.md#predictivescalingmetricoutputtypedef)
- [PredictiveScalingMetricTypeDef](./type_defs.md#predictivescalingmetrictypedef)
- [PutScheduledActionRequestRequestTypeDef](./type_defs.md#putscheduledactionrequestrequesttypedef)
- [ScheduledActionTypeDef](./type_defs.md#scheduledactiontypedef)
- [RegisterScalableTargetRequestRequestTypeDef](./type_defs.md#registerscalabletargetrequestrequesttypedef)
- [ScalableTargetTypeDef](./type_defs.md#scalabletargettypedef)
- [StepScalingPolicyConfigurationOutputTypeDef](./type_defs.md#stepscalingpolicyconfigurationoutputtypedef)
- [StepScalingPolicyConfigurationTypeDef](./type_defs.md#stepscalingpolicyconfigurationtypedef)
- [TargetTrackingMetricOutputTypeDef](./type_defs.md#targettrackingmetricoutputtypedef)
- [TargetTrackingMetricTypeDef](./type_defs.md#targettrackingmetrictypedef)
- [DescribeScalingActivitiesResponseTypeDef](./type_defs.md#describescalingactivitiesresponsetypedef)
- [PredictiveScalingMetricStatOutputTypeDef](./type_defs.md#predictivescalingmetricstatoutputtypedef)
- [PredictiveScalingMetricUnionTypeDef](./type_defs.md#predictivescalingmetricuniontypedef)
- [DescribeScheduledActionsResponseTypeDef](./type_defs.md#describescheduledactionsresponsetypedef)
- [DescribeScalableTargetsResponseTypeDef](./type_defs.md#describescalabletargetsresponsetypedef)
- [TargetTrackingMetricStatOutputTypeDef](./type_defs.md#targettrackingmetricstatoutputtypedef)
- [TargetTrackingMetricUnionTypeDef](./type_defs.md#targettrackingmetricuniontypedef)
- [PredictiveScalingMetricDataQueryOutputTypeDef](./type_defs.md#predictivescalingmetricdataqueryoutputtypedef)
- [PredictiveScalingMetricStatTypeDef](./type_defs.md#predictivescalingmetricstattypedef)
- [TargetTrackingMetricDataQueryOutputTypeDef](./type_defs.md#targettrackingmetricdataqueryoutputtypedef)
- [TargetTrackingMetricStatTypeDef](./type_defs.md#targettrackingmetricstattypedef)
- [PredictiveScalingCustomizedMetricSpecificationOutputTypeDef](./type_defs.md#predictivescalingcustomizedmetricspecificationoutputtypedef)
- [PredictiveScalingMetricStatUnionTypeDef](./type_defs.md#predictivescalingmetricstatuniontypedef)
- [CustomizedMetricSpecificationOutputTypeDef](./type_defs.md#customizedmetricspecificationoutputtypedef)
- [TargetTrackingMetricStatUnionTypeDef](./type_defs.md#targettrackingmetricstatuniontypedef)
- [PredictiveScalingMetricSpecificationOutputTypeDef](./type_defs.md#predictivescalingmetricspecificationoutputtypedef)
- [PredictiveScalingMetricDataQueryTypeDef](./type_defs.md#predictivescalingmetricdataquerytypedef)
- [TargetTrackingScalingPolicyConfigurationOutputTypeDef](./type_defs.md#targettrackingscalingpolicyconfigurationoutputtypedef)
- [TargetTrackingMetricDataQueryTypeDef](./type_defs.md#targettrackingmetricdataquerytypedef)
- [LoadForecastTypeDef](./type_defs.md#loadforecasttypedef)
- [PredictiveScalingPolicyConfigurationOutputTypeDef](./type_defs.md#predictivescalingpolicyconfigurationoutputtypedef)
- [PredictiveScalingMetricDataQueryUnionTypeDef](./type_defs.md#predictivescalingmetricdataqueryuniontypedef)
- [TargetTrackingMetricDataQueryUnionTypeDef](./type_defs.md#targettrackingmetricdataqueryuniontypedef)
- [GetPredictiveScalingForecastResponseTypeDef](./type_defs.md#getpredictivescalingforecastresponsetypedef)
- [ScalingPolicyTypeDef](./type_defs.md#scalingpolicytypedef)
- [PredictiveScalingCustomizedMetricSpecificationTypeDef](./type_defs.md#predictivescalingcustomizedmetricspecificationtypedef)
- [CustomizedMetricSpecificationTypeDef](./type_defs.md#customizedmetricspecificationtypedef)
- [DescribeScalingPoliciesResponseTypeDef](./type_defs.md#describescalingpoliciesresponsetypedef)
- [PredictiveScalingCustomizedMetricSpecificationUnionTypeDef](./type_defs.md#predictivescalingcustomizedmetricspecificationuniontypedef)
- [CustomizedMetricSpecificationUnionTypeDef](./type_defs.md#customizedmetricspecificationuniontypedef)
- [PredictiveScalingMetricSpecificationTypeDef](./type_defs.md#predictivescalingmetricspecificationtypedef)
- [TargetTrackingScalingPolicyConfigurationTypeDef](./type_defs.md#targettrackingscalingpolicyconfigurationtypedef)
- [PredictiveScalingMetricSpecificationUnionTypeDef](./type_defs.md#predictivescalingmetricspecificationuniontypedef)
- [PredictiveScalingPolicyConfigurationTypeDef](./type_defs.md#predictivescalingpolicyconfigurationtypedef)
- [PutScalingPolicyRequestRequestTypeDef](./type_defs.md#putscalingpolicyrequestrequesttypedef)

