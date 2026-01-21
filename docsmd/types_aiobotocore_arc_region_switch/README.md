# ARCRegionswitch module

> [Index](../README.md) > ARCRegionswitch


!!! note ""

    Auto-generated documentation for [ARCRegionswitch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-region-switch.html#arcregionswitch)
    type annotations stubs module [types-aiobotocore-arc-region-switch](https://pypi.org/project/types-aiobotocore-arc-region-switch/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ARCRegionswitch` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ARCRegionswitch` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[arc-region-switch]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[arc-region-switch]'

# standalone installation
python -m pip install types-aiobotocore-arc-region-switch
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-arc-region-switch
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ARCRegionswitchClient

Type annotations and code completion for  `#!python session.create_client("arc-region-switch")` as [ARCRegionswitchClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-region-switch.html#ARCRegionswitch.Client)

```python
# ARCRegionswitchClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_arc_region_switch.client import ARCRegionswitchClient


session = get_session()
async with session.create_client("arc-region-switch") as client:
    client: ARCRegionswitchClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("arc-region-switch").get_paginator("...")`.

```python
# GetPlanEvaluationStatusPaginator usage example

from types_aiobotocore_arc_region_switch.paginator import GetPlanEvaluationStatusPaginator

def get_get_plan_evaluation_status_paginator() -> GetPlanEvaluationStatusPaginator:
    return client.get_paginator("get_plan_evaluation_status"))
```

- [GetPlanEvaluationStatusPaginator](./paginators.md#getplanevaluationstatuspaginator)
- [GetPlanExecutionPaginator](./paginators.md#getplanexecutionpaginator)
- [ListPlanExecutionEventsPaginator](./paginators.md#listplanexecutioneventspaginator)
- [ListPlanExecutionsPaginator](./paginators.md#listplanexecutionspaginator)
- [ListPlansInRegionPaginator](./paginators.md#listplansinregionpaginator)
- [ListPlansPaginator](./paginators.md#listplanspaginator)
- [ListRoute53HealthChecksInRegionPaginator](./paginators.md#listroute53healthchecksinregionpaginator)
- [ListRoute53HealthChecksPaginator](./paginators.md#listroute53healthcheckspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("arc-region-switch").get_waiter("...")`.

```python
# PlanEvaluationStatusPassedWaiter usage example

from types_aiobotocore_arc_region_switch.waiter import PlanEvaluationStatusPassedWaiter

def get_plan_evaluation_status_passed_waiter() -> PlanEvaluationStatusPassedWaiter:
    return Session().client("arc-region-switch").get_waiter("plan_evaluation_status_passed")
```

- [PlanEvaluationStatusPassedWaiter](./waiters.md#planevaluationstatuspassedwaiter)
- [PlanExecutionCompletedWaiter](./waiters.md#planexecutioncompletedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AlarmConditionType usage example

from types_aiobotocore_arc_region_switch.literals import AlarmConditionType

def get_value() -> AlarmConditionType:
    return "green"
```

- [AlarmConditionType](./literals.md#alarmconditiontype)
- [AlarmTypeType](./literals.md#alarmtypetype)
- [ApprovalType](./literals.md#approvaltype)
- [DocumentDbDefaultBehaviorType](./literals.md#documentdbdefaultbehaviortype)
- [DocumentDbUngracefulBehaviorType](./literals.md#documentdbungracefulbehaviortype)
- [Ec2AsgCapacityMonitoringApproachType](./literals.md#ec2asgcapacitymonitoringapproachtype)
- [EcsCapacityMonitoringApproachType](./literals.md#ecscapacitymonitoringapproachtype)
- [EksCapacityMonitoringApproachType](./literals.md#ekscapacitymonitoringapproachtype)
- [EvaluationStatusType](./literals.md#evaluationstatustype)
- [ExecutionActionType](./literals.md#executionactiontype)
- [ExecutionBlockTypeType](./literals.md#executionblocktypetype)
- [ExecutionEventTypeType](./literals.md#executioneventtypetype)
- [ExecutionModeType](./literals.md#executionmodetype)
- [ExecutionStateType](./literals.md#executionstatetype)
- [FailedReportErrorCodeType](./literals.md#failedreporterrorcodetype)
- [GetPlanEvaluationStatusPaginatorName](./literals.md#getplanevaluationstatuspaginatorname)
- [GetPlanExecutionPaginatorName](./literals.md#getplanexecutionpaginatorname)
- [GlobalAuroraDefaultBehaviorType](./literals.md#globalauroradefaultbehaviortype)
- [GlobalAuroraUngracefulBehaviorType](./literals.md#globalauroraungracefulbehaviortype)
- [LambdaUngracefulBehaviorType](./literals.md#lambdaungracefulbehaviortype)
- [ListPlanExecutionEventsPaginatorName](./literals.md#listplanexecutioneventspaginatorname)
- [ListPlanExecutionsPaginatorName](./literals.md#listplanexecutionspaginatorname)
- [ListPlansInRegionPaginatorName](./literals.md#listplansinregionpaginatorname)
- [ListPlansPaginatorName](./literals.md#listplanspaginatorname)
- [ListRoute53HealthChecksInRegionPaginatorName](./literals.md#listroute53healthchecksinregionpaginatorname)
- [ListRoute53HealthChecksPaginatorName](./literals.md#listroute53healthcheckspaginatorname)
- [PlanEvaluationStatusPassedWaiterName](./literals.md#planevaluationstatuspassedwaitername)
- [PlanExecutionCompletedWaiterName](./literals.md#planexecutioncompletedwaitername)
- [RecoveryApproachType](./literals.md#recoveryapproachtype)
- [RegionToRunInType](./literals.md#regiontorunintype)
- [ResourceWarningStatusType](./literals.md#resourcewarningstatustype)
- [Route53HealthCheckStatusType](./literals.md#route53healthcheckstatustype)
- [RoutingControlStateChangeType](./literals.md#routingcontrolstatechangetype)
- [StepStatusType](./literals.md#stepstatustype)
- [UpdatePlanExecutionActionType](./literals.md#updateplanexecutionactiontype)
- [UpdatePlanExecutionStepActionType](./literals.md#updateplanexecutionstepactiontype)
- [WorkflowTargetActionType](./literals.md#workflowtargetactiontype)
- [ARCRegionswitchServiceName](./literals.md#arcregionswitchservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AbbreviatedExecutionTypeDef](./type_defs.md#abbreviatedexecutiontypedef)
- [AbbreviatedPlanTypeDef](./type_defs.md#abbreviatedplantypedef)
- [ApprovePlanExecutionStepRequestTypeDef](./type_defs.md#approveplanexecutionsteprequesttypedef)
- [ArcRoutingControlStateTypeDef](./type_defs.md#arcroutingcontrolstatetypedef)
- [AsgTypeDef](./type_defs.md#asgtypedef)
- [AssociatedAlarmTypeDef](./type_defs.md#associatedalarmtypedef)
- [CancelPlanExecutionRequestTypeDef](./type_defs.md#cancelplanexecutionrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [LambdaUngracefulTypeDef](./type_defs.md#lambdaungracefultypedef)
- [LambdasTypeDef](./type_defs.md#lambdastypedef)
- [DeletePlanRequestTypeDef](./type_defs.md#deleteplanrequesttypedef)
- [DocumentDbUngracefulTypeDef](./type_defs.md#documentdbungracefultypedef)
- [Ec2UngracefulTypeDef](./type_defs.md#ec2ungracefultypedef)
- [EcsUngracefulTypeDef](./type_defs.md#ecsungracefultypedef)
- [ServiceTypeDef](./type_defs.md#servicetypedef)
- [EksClusterTypeDef](./type_defs.md#eksclustertypedef)
- [EksResourceScalingUngracefulTypeDef](./type_defs.md#eksresourcescalingungracefultypedef)
- [KubernetesResourceTypeTypeDef](./type_defs.md#kubernetesresourcetypetypedef)
- [KubernetesScalingResourceTypeDef](./type_defs.md#kubernetesscalingresourcetypedef)
- [ExecutionApprovalConfigurationTypeDef](./type_defs.md#executionapprovalconfigurationtypedef)
- [ParallelExecutionBlockConfigurationOutputTypeDef](./type_defs.md#parallelexecutionblockconfigurationoutputtypedef)
- [RegionSwitchPlanConfigurationTypeDef](./type_defs.md#regionswitchplanconfigurationtypedef)
- [ParallelExecutionBlockConfigurationPaginatorTypeDef](./type_defs.md#parallelexecutionblockconfigurationpaginatortypedef)
- [ExecutionEventTypeDef](./type_defs.md#executioneventtypedef)
- [FailedReportOutputTypeDef](./type_defs.md#failedreportoutputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetPlanEvaluationStatusRequestTypeDef](./type_defs.md#getplanevaluationstatusrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetPlanExecutionRequestTypeDef](./type_defs.md#getplanexecutionrequesttypedef)
- [StepStateTypeDef](./type_defs.md#stepstatetypedef)
- [GetPlanInRegionRequestTypeDef](./type_defs.md#getplaninregionrequesttypedef)
- [GetPlanRequestTypeDef](./type_defs.md#getplanrequesttypedef)
- [GlobalAuroraUngracefulTypeDef](./type_defs.md#globalauroraungracefultypedef)
- [ListPlanExecutionEventsRequestTypeDef](./type_defs.md#listplanexecutioneventsrequesttypedef)
- [ListPlanExecutionsRequestTypeDef](./type_defs.md#listplanexecutionsrequesttypedef)
- [ListPlansInRegionRequestTypeDef](./type_defs.md#listplansinregionrequesttypedef)
- [ListPlansRequestTypeDef](./type_defs.md#listplansrequesttypedef)
- [ListRoute53HealthChecksInRegionRequestTypeDef](./type_defs.md#listroute53healthchecksinregionrequesttypedef)
- [Route53HealthCheckTypeDef](./type_defs.md#route53healthchecktypedef)
- [ListRoute53HealthChecksRequestTypeDef](./type_defs.md#listroute53healthchecksrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [MinimalWorkflowTypeDef](./type_defs.md#minimalworkflowtypedef)
- [ParallelExecutionBlockConfigurationTypeDef](./type_defs.md#parallelexecutionblockconfigurationtypedef)
- [S3ReportOutputConfigurationTypeDef](./type_defs.md#s3reportoutputconfigurationtypedef)
- [S3ReportOutputTypeDef](./type_defs.md#s3reportoutputtypedef)
- [Route53ResourceRecordSetTypeDef](./type_defs.md#route53resourcerecordsettypedef)
- [StartPlanExecutionRequestTypeDef](./type_defs.md#startplanexecutionrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [TriggerConditionTypeDef](./type_defs.md#triggerconditiontypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdatePlanExecutionRequestTypeDef](./type_defs.md#updateplanexecutionrequesttypedef)
- [UpdatePlanExecutionStepRequestTypeDef](./type_defs.md#updateplanexecutionsteprequesttypedef)
- [ArcRoutingControlConfigurationOutputTypeDef](./type_defs.md#arcroutingcontrolconfigurationoutputtypedef)
- [ArcRoutingControlConfigurationTypeDef](./type_defs.md#arcroutingcontrolconfigurationtypedef)
- [ListPlanExecutionsResponseTypeDef](./type_defs.md#listplanexecutionsresponsetypedef)
- [ListPlansInRegionResponseTypeDef](./type_defs.md#listplansinregionresponsetypedef)
- [ListPlansResponseTypeDef](./type_defs.md#listplansresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartPlanExecutionResponseTypeDef](./type_defs.md#startplanexecutionresponsetypedef)
- [CustomActionLambdaConfigurationOutputTypeDef](./type_defs.md#customactionlambdaconfigurationoutputtypedef)
- [CustomActionLambdaConfigurationTypeDef](./type_defs.md#customactionlambdaconfigurationtypedef)
- [DocumentDbConfigurationOutputTypeDef](./type_defs.md#documentdbconfigurationoutputtypedef)
- [DocumentDbConfigurationTypeDef](./type_defs.md#documentdbconfigurationtypedef)
- [Ec2AsgCapacityIncreaseConfigurationOutputTypeDef](./type_defs.md#ec2asgcapacityincreaseconfigurationoutputtypedef)
- [Ec2AsgCapacityIncreaseConfigurationTypeDef](./type_defs.md#ec2asgcapacityincreaseconfigurationtypedef)
- [EcsCapacityIncreaseConfigurationOutputTypeDef](./type_defs.md#ecscapacityincreaseconfigurationoutputtypedef)
- [EcsCapacityIncreaseConfigurationTypeDef](./type_defs.md#ecscapacityincreaseconfigurationtypedef)
- [EksResourceScalingConfigurationOutputTypeDef](./type_defs.md#eksresourcescalingconfigurationoutputtypedef)
- [EksResourceScalingConfigurationTypeDef](./type_defs.md#eksresourcescalingconfigurationtypedef)
- [ListPlanExecutionEventsResponseTypeDef](./type_defs.md#listplanexecutioneventsresponsetypedef)
- [GetPlanEvaluationStatusRequestPaginateTypeDef](./type_defs.md#getplanevaluationstatusrequestpaginatetypedef)
- [GetPlanExecutionRequestPaginateTypeDef](./type_defs.md#getplanexecutionrequestpaginatetypedef)
- [ListPlanExecutionEventsRequestPaginateTypeDef](./type_defs.md#listplanexecutioneventsrequestpaginatetypedef)
- [ListPlanExecutionsRequestPaginateTypeDef](./type_defs.md#listplanexecutionsrequestpaginatetypedef)
- [ListPlansInRegionRequestPaginateTypeDef](./type_defs.md#listplansinregionrequestpaginatetypedef)
- [ListPlansRequestPaginateTypeDef](./type_defs.md#listplansrequestpaginatetypedef)
- [ListRoute53HealthChecksInRegionRequestPaginateTypeDef](./type_defs.md#listroute53healthchecksinregionrequestpaginatetypedef)
- [ListRoute53HealthChecksRequestPaginateTypeDef](./type_defs.md#listroute53healthchecksrequestpaginatetypedef)
- [GetPlanEvaluationStatusRequestWaitTypeDef](./type_defs.md#getplanevaluationstatusrequestwaittypedef)
- [GetPlanExecutionRequestWaitTypeDef](./type_defs.md#getplanexecutionrequestwaittypedef)
- [GlobalAuroraConfigurationOutputTypeDef](./type_defs.md#globalauroraconfigurationoutputtypedef)
- [GlobalAuroraConfigurationTypeDef](./type_defs.md#globalauroraconfigurationtypedef)
- [ListRoute53HealthChecksInRegionResponseTypeDef](./type_defs.md#listroute53healthchecksinregionresponsetypedef)
- [ListRoute53HealthChecksResponseTypeDef](./type_defs.md#listroute53healthchecksresponsetypedef)
- [ResourceWarningTypeDef](./type_defs.md#resourcewarningtypedef)
- [ParallelExecutionBlockConfigurationUnionTypeDef](./type_defs.md#parallelexecutionblockconfigurationuniontypedef)
- [ReportOutputConfigurationTypeDef](./type_defs.md#reportoutputconfigurationtypedef)
- [ReportOutputTypeDef](./type_defs.md#reportoutputtypedef)
- [Route53HealthCheckConfigurationOutputTypeDef](./type_defs.md#route53healthcheckconfigurationoutputtypedef)
- [Route53HealthCheckConfigurationTypeDef](./type_defs.md#route53healthcheckconfigurationtypedef)
- [TriggerOutputTypeDef](./type_defs.md#triggeroutputtypedef)
- [TriggerTypeDef](./type_defs.md#triggertypedef)
- [ArcRoutingControlConfigurationUnionTypeDef](./type_defs.md#arcroutingcontrolconfigurationuniontypedef)
- [CustomActionLambdaConfigurationUnionTypeDef](./type_defs.md#customactionlambdaconfigurationuniontypedef)
- [DocumentDbConfigurationUnionTypeDef](./type_defs.md#documentdbconfigurationuniontypedef)
- [Ec2AsgCapacityIncreaseConfigurationUnionTypeDef](./type_defs.md#ec2asgcapacityincreaseconfigurationuniontypedef)
- [EcsCapacityIncreaseConfigurationUnionTypeDef](./type_defs.md#ecscapacityincreaseconfigurationuniontypedef)
- [EksResourceScalingConfigurationUnionTypeDef](./type_defs.md#eksresourcescalingconfigurationuniontypedef)
- [GlobalAuroraConfigurationUnionTypeDef](./type_defs.md#globalauroraconfigurationuniontypedef)
- [GetPlanEvaluationStatusResponseTypeDef](./type_defs.md#getplanevaluationstatusresponsetypedef)
- [ReportConfigurationOutputTypeDef](./type_defs.md#reportconfigurationoutputtypedef)
- [ReportConfigurationTypeDef](./type_defs.md#reportconfigurationtypedef)
- [GeneratedReportTypeDef](./type_defs.md#generatedreporttypedef)
- [ExecutionBlockConfigurationOutputTypeDef](./type_defs.md#executionblockconfigurationoutputtypedef)
- [ExecutionBlockConfigurationPaginatorTypeDef](./type_defs.md#executionblockconfigurationpaginatortypedef)
- [Route53HealthCheckConfigurationUnionTypeDef](./type_defs.md#route53healthcheckconfigurationuniontypedef)
- [TriggerUnionTypeDef](./type_defs.md#triggeruniontypedef)
- [ReportConfigurationUnionTypeDef](./type_defs.md#reportconfigurationuniontypedef)
- [StepOutputTypeDef](./type_defs.md#stepoutputtypedef)
- [StepPaginatorTypeDef](./type_defs.md#steppaginatortypedef)
- [ExecutionBlockConfigurationTypeDef](./type_defs.md#executionblockconfigurationtypedef)
- [WorkflowOutputTypeDef](./type_defs.md#workflowoutputtypedef)
- [WorkflowPaginatorTypeDef](./type_defs.md#workflowpaginatortypedef)
- [ExecutionBlockConfigurationUnionTypeDef](./type_defs.md#executionblockconfigurationuniontypedef)
- [PlanTypeDef](./type_defs.md#plantypedef)
- [PlanPaginatorTypeDef](./type_defs.md#planpaginatortypedef)
- [StepTypeDef](./type_defs.md#steptypedef)
- [CreatePlanResponseTypeDef](./type_defs.md#createplanresponsetypedef)
- [GetPlanExecutionResponseTypeDef](./type_defs.md#getplanexecutionresponsetypedef)
- [GetPlanInRegionResponseTypeDef](./type_defs.md#getplaninregionresponsetypedef)
- [GetPlanResponseTypeDef](./type_defs.md#getplanresponsetypedef)
- [UpdatePlanResponseTypeDef](./type_defs.md#updateplanresponsetypedef)
- [GetPlanExecutionResponsePaginatorTypeDef](./type_defs.md#getplanexecutionresponsepaginatortypedef)
- [StepUnionTypeDef](./type_defs.md#stepuniontypedef)
- [WorkflowTypeDef](./type_defs.md#workflowtypedef)
- [WorkflowUnionTypeDef](./type_defs.md#workflowuniontypedef)
- [CreatePlanRequestTypeDef](./type_defs.md#createplanrequesttypedef)
- [UpdatePlanRequestTypeDef](./type_defs.md#updateplanrequesttypedef)

