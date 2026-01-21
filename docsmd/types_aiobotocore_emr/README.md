# EMR module

> [Index](../README.md) > EMR


!!! note ""

    Auto-generated documentation for [EMR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#emr)
    type annotations stubs module [types-aiobotocore-emr](https://pypi.org/project/types-aiobotocore-emr/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `EMR` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `EMR` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[emr]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[emr]'

# standalone installation
python -m pip install types-aiobotocore-emr
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-emr
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EMRClient

Type annotations and code completion for  `#!python session.create_client("emr")` as [EMRClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Client)

```python
# EMRClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_emr.client import EMRClient


session = get_session()
async with session.create_client("emr") as client:
    client: EMRClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("emr").get_paginator("...")`.

```python
# ListBootstrapActionsPaginator usage example

from types_aiobotocore_emr.paginator import ListBootstrapActionsPaginator

def get_list_bootstrap_actions_paginator() -> ListBootstrapActionsPaginator:
    return client.get_paginator("list_bootstrap_actions"))
```

- [ListBootstrapActionsPaginator](./paginators.md#listbootstrapactionspaginator)
- [ListClustersPaginator](./paginators.md#listclusterspaginator)
- [ListInstanceFleetsPaginator](./paginators.md#listinstancefleetspaginator)
- [ListInstanceGroupsPaginator](./paginators.md#listinstancegroupspaginator)
- [ListInstancesPaginator](./paginators.md#listinstancespaginator)
- [ListNotebookExecutionsPaginator](./paginators.md#listnotebookexecutionspaginator)
- [ListSecurityConfigurationsPaginator](./paginators.md#listsecurityconfigurationspaginator)
- [ListStepsPaginator](./paginators.md#liststepspaginator)
- [ListStudioSessionMappingsPaginator](./paginators.md#liststudiosessionmappingspaginator)
- [ListStudiosPaginator](./paginators.md#liststudiospaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("emr").get_waiter("...")`.

```python
# ClusterRunningWaiter usage example

from types_aiobotocore_emr.waiter import ClusterRunningWaiter

def get_cluster_running_waiter() -> ClusterRunningWaiter:
    return Session().client("emr").get_waiter("cluster_running")
```

- [ClusterRunningWaiter](./waiters.md#clusterrunningwaiter)
- [ClusterTerminatedWaiter](./waiters.md#clusterterminatedwaiter)
- [StepCompleteWaiter](./waiters.md#stepcompletewaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionOnFailureType usage example

from types_aiobotocore_emr.literals import ActionOnFailureType

def get_value() -> ActionOnFailureType:
    return "CANCEL_AND_WAIT"
```

- [ActionOnFailureType](./literals.md#actiononfailuretype)
- [AdjustmentTypeType](./literals.md#adjustmenttypetype)
- [AuthModeType](./literals.md#authmodetype)
- [AutoScalingPolicyStateChangeReasonCodeType](./literals.md#autoscalingpolicystatechangereasoncodetype)
- [AutoScalingPolicyStateType](./literals.md#autoscalingpolicystatetype)
- [CancelStepsRequestStatusType](./literals.md#cancelstepsrequeststatustype)
- [ClusterRunningWaiterName](./literals.md#clusterrunningwaitername)
- [ClusterStateChangeReasonCodeType](./literals.md#clusterstatechangereasoncodetype)
- [ClusterStateType](./literals.md#clusterstatetype)
- [ClusterTerminatedWaiterName](./literals.md#clusterterminatedwaitername)
- [ComparisonOperatorType](./literals.md#comparisonoperatortype)
- [ComputeLimitsUnitTypeType](./literals.md#computelimitsunittypetype)
- [ExecutionEngineTypeType](./literals.md#executionenginetypetype)
- [IdcUserAssignmentType](./literals.md#idcuserassignmenttype)
- [IdentityTypeType](./literals.md#identitytypetype)
- [InstanceCollectionTypeType](./literals.md#instancecollectiontypetype)
- [InstanceFleetStateChangeReasonCodeType](./literals.md#instancefleetstatechangereasoncodetype)
- [InstanceFleetStateType](./literals.md#instancefleetstatetype)
- [InstanceFleetTypeType](./literals.md#instancefleettypetype)
- [InstanceGroupStateChangeReasonCodeType](./literals.md#instancegroupstatechangereasoncodetype)
- [InstanceGroupStateType](./literals.md#instancegroupstatetype)
- [InstanceGroupTypeType](./literals.md#instancegrouptypetype)
- [InstanceRoleTypeType](./literals.md#instanceroletypetype)
- [InstanceStateChangeReasonCodeType](./literals.md#instancestatechangereasoncodetype)
- [InstanceStateType](./literals.md#instancestatetype)
- [JobFlowExecutionStateType](./literals.md#jobflowexecutionstatetype)
- [ListBootstrapActionsPaginatorName](./literals.md#listbootstrapactionspaginatorname)
- [ListClustersPaginatorName](./literals.md#listclusterspaginatorname)
- [ListInstanceFleetsPaginatorName](./literals.md#listinstancefleetspaginatorname)
- [ListInstanceGroupsPaginatorName](./literals.md#listinstancegroupspaginatorname)
- [ListInstancesPaginatorName](./literals.md#listinstancespaginatorname)
- [ListNotebookExecutionsPaginatorName](./literals.md#listnotebookexecutionspaginatorname)
- [ListSecurityConfigurationsPaginatorName](./literals.md#listsecurityconfigurationspaginatorname)
- [ListStepsPaginatorName](./literals.md#liststepspaginatorname)
- [ListStudioSessionMappingsPaginatorName](./literals.md#liststudiosessionmappingspaginatorname)
- [ListStudiosPaginatorName](./literals.md#liststudiospaginatorname)
- [MarketTypeType](./literals.md#markettypetype)
- [NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype)
- [OnClusterAppUITypeType](./literals.md#onclusterappuitypetype)
- [OnDemandCapacityReservationPreferenceType](./literals.md#ondemandcapacityreservationpreferencetype)
- [OnDemandCapacityReservationUsageStrategyType](./literals.md#ondemandcapacityreservationusagestrategytype)
- [OnDemandProvisioningAllocationStrategyType](./literals.md#ondemandprovisioningallocationstrategytype)
- [OutputNotebookFormatType](./literals.md#outputnotebookformattype)
- [PersistentAppUITypeType](./literals.md#persistentappuitypetype)
- [PlacementGroupStrategyType](./literals.md#placementgroupstrategytype)
- [ProfilerTypeType](./literals.md#profilertypetype)
- [ReconfigurationTypeType](./literals.md#reconfigurationtypetype)
- [RepoUpgradeOnBootType](./literals.md#repoupgradeonboottype)
- [ScaleDownBehaviorType](./literals.md#scaledownbehaviortype)
- [ScalingStrategyType](./literals.md#scalingstrategytype)
- [SpotProvisioningAllocationStrategyType](./literals.md#spotprovisioningallocationstrategytype)
- [SpotProvisioningTimeoutActionType](./literals.md#spotprovisioningtimeoutactiontype)
- [StatisticType](./literals.md#statistictype)
- [StepCancellationOptionType](./literals.md#stepcancellationoptiontype)
- [StepCompleteWaiterName](./literals.md#stepcompletewaitername)
- [StepExecutionStateType](./literals.md#stepexecutionstatetype)
- [StepStateChangeReasonCodeType](./literals.md#stepstatechangereasoncodetype)
- [StepStateType](./literals.md#stepstatetype)
- [UnitType](./literals.md#unittype)
- [EMRServiceName](./literals.md#emrservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef)
- [ApplicationTypeDef](./type_defs.md#applicationtypedef)
- [ScalingConstraintsTypeDef](./type_defs.md#scalingconstraintstypedef)
- [AutoScalingPolicyStateChangeReasonTypeDef](./type_defs.md#autoscalingpolicystatechangereasontypedef)
- [AutoTerminationPolicyTypeDef](./type_defs.md#autoterminationpolicytypedef)
- [BlockPublicAccessConfigurationMetadataTypeDef](./type_defs.md#blockpublicaccessconfigurationmetadatatypedef)
- [PortRangeTypeDef](./type_defs.md#portrangetypedef)
- [ScriptBootstrapActionConfigOutputTypeDef](./type_defs.md#scriptbootstrapactionconfigoutputtypedef)
- [CancelStepsInfoTypeDef](./type_defs.md#cancelstepsinfotypedef)
- [CancelStepsInputTypeDef](./type_defs.md#cancelstepsinputtypedef)
- [MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef)
- [CloudWatchLogConfigurationOutputTypeDef](./type_defs.md#cloudwatchlogconfigurationoutputtypedef)
- [CloudWatchLogConfigurationTypeDef](./type_defs.md#cloudwatchlogconfigurationtypedef)
- [ClusterStateChangeReasonTypeDef](./type_defs.md#clusterstatechangereasontypedef)
- [ClusterTimelineTypeDef](./type_defs.md#clustertimelinetypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef)
- [Ec2InstanceAttributesTypeDef](./type_defs.md#ec2instanceattributestypedef)
- [KerberosAttributesTypeDef](./type_defs.md#kerberosattributestypedef)
- [PlacementGroupConfigTypeDef](./type_defs.md#placementgroupconfigtypedef)
- [CommandTypeDef](./type_defs.md#commandtypedef)
- [ComputeLimitsTypeDef](./type_defs.md#computelimitstypedef)
- [ConfigurationPaginatorTypeDef](./type_defs.md#configurationpaginatortypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [EMRContainersConfigTypeDef](./type_defs.md#emrcontainersconfigtypedef)
- [CreateSecurityConfigurationInputTypeDef](./type_defs.md#createsecurityconfigurationinputtypedef)
- [CreateStudioSessionMappingInputTypeDef](./type_defs.md#createstudiosessionmappinginputtypedef)
- [UsernamePasswordTypeDef](./type_defs.md#usernamepasswordtypedef)
- [DeleteSecurityConfigurationInputTypeDef](./type_defs.md#deletesecurityconfigurationinputtypedef)
- [DeleteStudioInputTypeDef](./type_defs.md#deletestudioinputtypedef)
- [DeleteStudioSessionMappingInputTypeDef](./type_defs.md#deletestudiosessionmappinginputtypedef)
- [DescribeClusterInputTypeDef](./type_defs.md#describeclusterinputtypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DescribeNotebookExecutionInputTypeDef](./type_defs.md#describenotebookexecutioninputtypedef)
- [DescribePersistentAppUIInputTypeDef](./type_defs.md#describepersistentappuiinputtypedef)
- [DescribeReleaseLabelInputTypeDef](./type_defs.md#describereleaselabelinputtypedef)
- [OSReleaseTypeDef](./type_defs.md#osreleasetypedef)
- [SimplifiedApplicationTypeDef](./type_defs.md#simplifiedapplicationtypedef)
- [DescribeSecurityConfigurationInputTypeDef](./type_defs.md#describesecurityconfigurationinputtypedef)
- [DescribeStepInputTypeDef](./type_defs.md#describestepinputtypedef)
- [DescribeStudioInputTypeDef](./type_defs.md#describestudioinputtypedef)
- [VolumeSpecificationTypeDef](./type_defs.md#volumespecificationtypedef)
- [EbsVolumeTypeDef](./type_defs.md#ebsvolumetypedef)
- [ExecutionEngineConfigTypeDef](./type_defs.md#executionengineconfigtypedef)
- [FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef)
- [GetAutoTerminationPolicyInputTypeDef](./type_defs.md#getautoterminationpolicyinputtypedef)
- [GetClusterSessionCredentialsInputTypeDef](./type_defs.md#getclustersessioncredentialsinputtypedef)
- [GetManagedScalingPolicyInputTypeDef](./type_defs.md#getmanagedscalingpolicyinputtypedef)
- [GetOnClusterAppUIPresignedURLInputTypeDef](./type_defs.md#getonclusterappuipresignedurlinputtypedef)
- [GetPersistentAppUIPresignedURLInputTypeDef](./type_defs.md#getpersistentappuipresignedurlinputtypedef)
- [GetStudioSessionMappingInputTypeDef](./type_defs.md#getstudiosessionmappinginputtypedef)
- [SessionMappingDetailTypeDef](./type_defs.md#sessionmappingdetailtypedef)
- [KeyValueTypeDef](./type_defs.md#keyvaluetypedef)
- [HadoopStepConfigTypeDef](./type_defs.md#hadoopstepconfigtypedef)
- [SpotProvisioningSpecificationTypeDef](./type_defs.md#spotprovisioningspecificationtypedef)
- [SpotResizingSpecificationTypeDef](./type_defs.md#spotresizingspecificationtypedef)
- [InstanceFleetStateChangeReasonTypeDef](./type_defs.md#instancefleetstatechangereasontypedef)
- [InstanceFleetTimelineTypeDef](./type_defs.md#instancefleettimelinetypedef)
- [InstanceGroupDetailTypeDef](./type_defs.md#instancegroupdetailtypedef)
- [InstanceGroupStateChangeReasonTypeDef](./type_defs.md#instancegroupstatechangereasontypedef)
- [InstanceGroupTimelineTypeDef](./type_defs.md#instancegrouptimelinetypedef)
- [InstanceResizePolicyOutputTypeDef](./type_defs.md#instanceresizepolicyoutputtypedef)
- [InstanceResizePolicyTypeDef](./type_defs.md#instanceresizepolicytypedef)
- [InstanceStateChangeReasonTypeDef](./type_defs.md#instancestatechangereasontypedef)
- [InstanceTimelineTypeDef](./type_defs.md#instancetimelinetypedef)
- [JobFlowExecutionStatusDetailTypeDef](./type_defs.md#jobflowexecutionstatusdetailtypedef)
- [PlacementTypeOutputTypeDef](./type_defs.md#placementtypeoutputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBootstrapActionsInputTypeDef](./type_defs.md#listbootstrapactionsinputtypedef)
- [ListInstanceFleetsInputTypeDef](./type_defs.md#listinstancefleetsinputtypedef)
- [ListInstanceGroupsInputTypeDef](./type_defs.md#listinstancegroupsinputtypedef)
- [ListInstancesInputTypeDef](./type_defs.md#listinstancesinputtypedef)
- [ReleaseLabelFilterTypeDef](./type_defs.md#releaselabelfiltertypedef)
- [ListSecurityConfigurationsInputTypeDef](./type_defs.md#listsecurityconfigurationsinputtypedef)
- [SecurityConfigurationSummaryTypeDef](./type_defs.md#securityconfigurationsummarytypedef)
- [ListStepsInputTypeDef](./type_defs.md#liststepsinputtypedef)
- [ListStudioSessionMappingsInputTypeDef](./type_defs.md#liststudiosessionmappingsinputtypedef)
- [SessionMappingSummaryTypeDef](./type_defs.md#sessionmappingsummarytypedef)
- [ListStudiosInputTypeDef](./type_defs.md#liststudiosinputtypedef)
- [StudioSummaryTypeDef](./type_defs.md#studiosummarytypedef)
- [ListSupportedInstanceTypesInputTypeDef](./type_defs.md#listsupportedinstancetypesinputtypedef)
- [SupportedInstanceTypeTypeDef](./type_defs.md#supportedinstancetypetypedef)
- [ModifyClusterInputTypeDef](./type_defs.md#modifyclusterinputtypedef)
- [NotebookS3LocationForOutputTypeDef](./type_defs.md#notebooks3locationforoutputtypedef)
- [OutputNotebookS3LocationForOutputTypeDef](./type_defs.md#outputnotebooks3locationforoutputtypedef)
- [NotebookS3LocationFromInputTypeDef](./type_defs.md#notebooks3locationfrominputtypedef)
- [OnDemandCapacityReservationOptionsTypeDef](./type_defs.md#ondemandcapacityreservationoptionstypedef)
- [OutputNotebookS3LocationFromInputTypeDef](./type_defs.md#outputnotebooks3locationfrominputtypedef)
- [PlacementTypeTypeDef](./type_defs.md#placementtypetypedef)
- [RemoveAutoScalingPolicyInputTypeDef](./type_defs.md#removeautoscalingpolicyinputtypedef)
- [RemoveAutoTerminationPolicyInputTypeDef](./type_defs.md#removeautoterminationpolicyinputtypedef)
- [RemoveManagedScalingPolicyInputTypeDef](./type_defs.md#removemanagedscalingpolicyinputtypedef)
- [RemoveTagsInputTypeDef](./type_defs.md#removetagsinputtypedef)
- [SupportedProductConfigTypeDef](./type_defs.md#supportedproductconfigtypedef)
- [S3MonitoringConfigurationTypeDef](./type_defs.md#s3monitoringconfigurationtypedef)
- [SimpleScalingPolicyConfigurationTypeDef](./type_defs.md#simplescalingpolicyconfigurationtypedef)
- [ScriptBootstrapActionConfigTypeDef](./type_defs.md#scriptbootstrapactionconfigtypedef)
- [SetKeepJobFlowAliveWhenNoStepsInputTypeDef](./type_defs.md#setkeepjobflowalivewhennostepsinputtypedef)
- [SetTerminationProtectionInputTypeDef](./type_defs.md#setterminationprotectioninputtypedef)
- [SetUnhealthyNodeReplacementInputTypeDef](./type_defs.md#setunhealthynodereplacementinputtypedef)
- [SetVisibleToAllUsersInputTypeDef](./type_defs.md#setvisibletoallusersinputtypedef)
- [StepExecutionStatusDetailTypeDef](./type_defs.md#stepexecutionstatusdetailtypedef)
- [StepStateChangeReasonTypeDef](./type_defs.md#stepstatechangereasontypedef)
- [StepTimelineTypeDef](./type_defs.md#steptimelinetypedef)
- [StopNotebookExecutionInputTypeDef](./type_defs.md#stopnotebookexecutioninputtypedef)
- [TerminateJobFlowsInputTypeDef](./type_defs.md#terminatejobflowsinputtypedef)
- [UpdateStudioInputTypeDef](./type_defs.md#updatestudioinputtypedef)
- [UpdateStudioSessionMappingInputTypeDef](./type_defs.md#updatestudiosessionmappinginputtypedef)
- [AddInstanceFleetOutputTypeDef](./type_defs.md#addinstancefleetoutputtypedef)
- [AddInstanceGroupsOutputTypeDef](./type_defs.md#addinstancegroupsoutputtypedef)
- [AddJobFlowStepsOutputTypeDef](./type_defs.md#addjobflowstepsoutputtypedef)
- [CreatePersistentAppUIOutputTypeDef](./type_defs.md#createpersistentappuioutputtypedef)
- [CreateSecurityConfigurationOutputTypeDef](./type_defs.md#createsecurityconfigurationoutputtypedef)
- [CreateStudioOutputTypeDef](./type_defs.md#createstudiooutputtypedef)
- [DescribeSecurityConfigurationOutputTypeDef](./type_defs.md#describesecurityconfigurationoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetOnClusterAppUIPresignedURLOutputTypeDef](./type_defs.md#getonclusterappuipresignedurloutputtypedef)
- [GetPersistentAppUIPresignedURLOutputTypeDef](./type_defs.md#getpersistentappuipresignedurloutputtypedef)
- [ListReleaseLabelsOutputTypeDef](./type_defs.md#listreleaselabelsoutputtypedef)
- [ModifyClusterOutputTypeDef](./type_defs.md#modifyclusteroutputtypedef)
- [RunJobFlowOutputTypeDef](./type_defs.md#runjobflowoutputtypedef)
- [StartNotebookExecutionOutputTypeDef](./type_defs.md#startnotebookexecutionoutputtypedef)
- [AddTagsInputTypeDef](./type_defs.md#addtagsinputtypedef)
- [CreateStudioInputTypeDef](./type_defs.md#createstudioinputtypedef)
- [PersistentAppUITypeDef](./type_defs.md#persistentappuitypedef)
- [StudioTypeDef](./type_defs.md#studiotypedef)
- [ApplicationUnionTypeDef](./type_defs.md#applicationuniontypedef)
- [AutoScalingPolicyStatusTypeDef](./type_defs.md#autoscalingpolicystatustypedef)
- [GetAutoTerminationPolicyOutputTypeDef](./type_defs.md#getautoterminationpolicyoutputtypedef)
- [PutAutoTerminationPolicyInputTypeDef](./type_defs.md#putautoterminationpolicyinputtypedef)
- [BlockPublicAccessConfigurationOutputTypeDef](./type_defs.md#blockpublicaccessconfigurationoutputtypedef)
- [BlockPublicAccessConfigurationTypeDef](./type_defs.md#blockpublicaccessconfigurationtypedef)
- [BootstrapActionConfigOutputTypeDef](./type_defs.md#bootstrapactionconfigoutputtypedef)
- [CancelStepsOutputTypeDef](./type_defs.md#cancelstepsoutputtypedef)
- [CloudWatchAlarmDefinitionOutputTypeDef](./type_defs.md#cloudwatchalarmdefinitionoutputtypedef)
- [CloudWatchAlarmDefinitionTypeDef](./type_defs.md#cloudwatchalarmdefinitiontypedef)
- [MonitoringConfigurationOutputTypeDef](./type_defs.md#monitoringconfigurationoutputtypedef)
- [MonitoringConfigurationTypeDef](./type_defs.md#monitoringconfigurationtypedef)
- [ClusterStatusTypeDef](./type_defs.md#clusterstatustypedef)
- [ListBootstrapActionsOutputTypeDef](./type_defs.md#listbootstrapactionsoutputtypedef)
- [ManagedScalingPolicyTypeDef](./type_defs.md#managedscalingpolicytypedef)
- [ConfigurationUnionTypeDef](./type_defs.md#configurationuniontypedef)
- [CreatePersistentAppUIInputTypeDef](./type_defs.md#createpersistentappuiinputtypedef)
- [CredentialsTypeDef](./type_defs.md#credentialstypedef)
- [DescribeClusterInputWaitExtraTypeDef](./type_defs.md#describeclusterinputwaitextratypedef)
- [DescribeClusterInputWaitTypeDef](./type_defs.md#describeclusterinputwaittypedef)
- [DescribeStepInputWaitTypeDef](./type_defs.md#describestepinputwaittypedef)
- [DescribeJobFlowsInputTypeDef](./type_defs.md#describejobflowsinputtypedef)
- [ListClustersInputTypeDef](./type_defs.md#listclustersinputtypedef)
- [ListNotebookExecutionsInputTypeDef](./type_defs.md#listnotebookexecutionsinputtypedef)
- [DescribeReleaseLabelOutputTypeDef](./type_defs.md#describereleaselabeloutputtypedef)
- [EbsBlockDeviceConfigTypeDef](./type_defs.md#ebsblockdeviceconfigtypedef)
- [EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef)
- [GetStudioSessionMappingOutputTypeDef](./type_defs.md#getstudiosessionmappingoutputtypedef)
- [HadoopJarStepConfigOutputTypeDef](./type_defs.md#hadoopjarstepconfigoutputtypedef)
- [HadoopJarStepConfigTypeDef](./type_defs.md#hadoopjarstepconfigtypedef)
- [InstanceFleetStatusTypeDef](./type_defs.md#instancefleetstatustypedef)
- [InstanceGroupStatusTypeDef](./type_defs.md#instancegroupstatustypedef)
- [ShrinkPolicyOutputTypeDef](./type_defs.md#shrinkpolicyoutputtypedef)
- [InstanceResizePolicyUnionTypeDef](./type_defs.md#instanceresizepolicyuniontypedef)
- [InstanceStatusTypeDef](./type_defs.md#instancestatustypedef)
- [JobFlowInstancesDetailTypeDef](./type_defs.md#jobflowinstancesdetailtypedef)
- [ListBootstrapActionsInputPaginateTypeDef](./type_defs.md#listbootstrapactionsinputpaginatetypedef)
- [ListClustersInputPaginateTypeDef](./type_defs.md#listclustersinputpaginatetypedef)
- [ListInstanceFleetsInputPaginateTypeDef](./type_defs.md#listinstancefleetsinputpaginatetypedef)
- [ListInstanceGroupsInputPaginateTypeDef](./type_defs.md#listinstancegroupsinputpaginatetypedef)
- [ListInstancesInputPaginateTypeDef](./type_defs.md#listinstancesinputpaginatetypedef)
- [ListNotebookExecutionsInputPaginateTypeDef](./type_defs.md#listnotebookexecutionsinputpaginatetypedef)
- [ListSecurityConfigurationsInputPaginateTypeDef](./type_defs.md#listsecurityconfigurationsinputpaginatetypedef)
- [ListStepsInputPaginateTypeDef](./type_defs.md#liststepsinputpaginatetypedef)
- [ListStudioSessionMappingsInputPaginateTypeDef](./type_defs.md#liststudiosessionmappingsinputpaginatetypedef)
- [ListStudiosInputPaginateTypeDef](./type_defs.md#liststudiosinputpaginatetypedef)
- [ListReleaseLabelsInputTypeDef](./type_defs.md#listreleaselabelsinputtypedef)
- [ListSecurityConfigurationsOutputTypeDef](./type_defs.md#listsecurityconfigurationsoutputtypedef)
- [ListStudioSessionMappingsOutputTypeDef](./type_defs.md#liststudiosessionmappingsoutputtypedef)
- [ListStudiosOutputTypeDef](./type_defs.md#liststudiosoutputtypedef)
- [ListSupportedInstanceTypesOutputTypeDef](./type_defs.md#listsupportedinstancetypesoutputtypedef)
- [NotebookExecutionSummaryTypeDef](./type_defs.md#notebookexecutionsummarytypedef)
- [NotebookExecutionTypeDef](./type_defs.md#notebookexecutiontypedef)
- [OnDemandProvisioningSpecificationTypeDef](./type_defs.md#ondemandprovisioningspecificationtypedef)
- [OnDemandResizingSpecificationTypeDef](./type_defs.md#ondemandresizingspecificationtypedef)
- [StartNotebookExecutionInputTypeDef](./type_defs.md#startnotebookexecutioninputtypedef)
- [PlacementTypeUnionTypeDef](./type_defs.md#placementtypeuniontypedef)
- [StepMonitoringConfigurationTypeDef](./type_defs.md#stepmonitoringconfigurationtypedef)
- [ScalingActionTypeDef](./type_defs.md#scalingactiontypedef)
- [ScriptBootstrapActionConfigUnionTypeDef](./type_defs.md#scriptbootstrapactionconfiguniontypedef)
- [StepStatusTypeDef](./type_defs.md#stepstatustypedef)
- [DescribePersistentAppUIOutputTypeDef](./type_defs.md#describepersistentappuioutputtypedef)
- [DescribeStudioOutputTypeDef](./type_defs.md#describestudiooutputtypedef)
- [GetBlockPublicAccessConfigurationOutputTypeDef](./type_defs.md#getblockpublicaccessconfigurationoutputtypedef)
- [BlockPublicAccessConfigurationUnionTypeDef](./type_defs.md#blockpublicaccessconfigurationuniontypedef)
- [BootstrapActionDetailTypeDef](./type_defs.md#bootstrapactiondetailtypedef)
- [ScalingTriggerOutputTypeDef](./type_defs.md#scalingtriggeroutputtypedef)
- [CloudWatchAlarmDefinitionUnionTypeDef](./type_defs.md#cloudwatchalarmdefinitionuniontypedef)
- [MonitoringConfigurationUnionTypeDef](./type_defs.md#monitoringconfigurationuniontypedef)
- [ClusterSummaryTypeDef](./type_defs.md#clustersummarytypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [GetManagedScalingPolicyOutputTypeDef](./type_defs.md#getmanagedscalingpolicyoutputtypedef)
- [PutManagedScalingPolicyInputTypeDef](./type_defs.md#putmanagedscalingpolicyinputtypedef)
- [GetClusterSessionCredentialsOutputTypeDef](./type_defs.md#getclustersessioncredentialsoutputtypedef)
- [EbsConfigurationTypeDef](./type_defs.md#ebsconfigurationtypedef)
- [InstanceTypeSpecificationPaginatorTypeDef](./type_defs.md#instancetypespecificationpaginatortypedef)
- [InstanceTypeSpecificationTypeDef](./type_defs.md#instancetypespecificationtypedef)
- [HadoopJarStepConfigUnionTypeDef](./type_defs.md#hadoopjarstepconfiguniontypedef)
- [ShrinkPolicyTypeDef](./type_defs.md#shrinkpolicytypedef)
- [InstanceTypeDef](./type_defs.md#instancetypedef)
- [ListNotebookExecutionsOutputTypeDef](./type_defs.md#listnotebookexecutionsoutputtypedef)
- [DescribeNotebookExecutionOutputTypeDef](./type_defs.md#describenotebookexecutionoutputtypedef)
- [InstanceFleetProvisioningSpecificationsTypeDef](./type_defs.md#instancefleetprovisioningspecificationstypedef)
- [InstanceFleetResizingSpecificationsTypeDef](./type_defs.md#instancefleetresizingspecificationstypedef)
- [StepConfigOutputTypeDef](./type_defs.md#stepconfigoutputtypedef)
- [BootstrapActionConfigTypeDef](./type_defs.md#bootstrapactionconfigtypedef)
- [StepSummaryTypeDef](./type_defs.md#stepsummarytypedef)
- [StepTypeDef](./type_defs.md#steptypedef)
- [PutBlockPublicAccessConfigurationInputTypeDef](./type_defs.md#putblockpublicaccessconfigurationinputtypedef)
- [ScalingRuleOutputTypeDef](./type_defs.md#scalingruleoutputtypedef)
- [ScalingTriggerTypeDef](./type_defs.md#scalingtriggertypedef)
- [ListClustersOutputTypeDef](./type_defs.md#listclustersoutputtypedef)
- [DescribeClusterOutputTypeDef](./type_defs.md#describeclusteroutputtypedef)
- [InstanceTypeConfigTypeDef](./type_defs.md#instancetypeconfigtypedef)
- [StepConfigTypeDef](./type_defs.md#stepconfigtypedef)
- [ShrinkPolicyUnionTypeDef](./type_defs.md#shrinkpolicyuniontypedef)
- [ListInstancesOutputTypeDef](./type_defs.md#listinstancesoutputtypedef)
- [InstanceFleetPaginatorTypeDef](./type_defs.md#instancefleetpaginatortypedef)
- [InstanceFleetTypeDef](./type_defs.md#instancefleettypedef)
- [StepDetailTypeDef](./type_defs.md#stepdetailtypedef)
- [BootstrapActionConfigUnionTypeDef](./type_defs.md#bootstrapactionconfiguniontypedef)
- [ListStepsOutputTypeDef](./type_defs.md#liststepsoutputtypedef)
- [DescribeStepOutputTypeDef](./type_defs.md#describestepoutputtypedef)
- [AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef)
- [ScalingTriggerUnionTypeDef](./type_defs.md#scalingtriggeruniontypedef)
- [InstanceFleetConfigTypeDef](./type_defs.md#instancefleetconfigtypedef)
- [InstanceFleetModifyConfigTypeDef](./type_defs.md#instancefleetmodifyconfigtypedef)
- [StepConfigUnionTypeDef](./type_defs.md#stepconfiguniontypedef)
- [InstanceGroupModifyConfigTypeDef](./type_defs.md#instancegroupmodifyconfigtypedef)
- [ListInstanceFleetsOutputPaginatorTypeDef](./type_defs.md#listinstancefleetsoutputpaginatortypedef)
- [ListInstanceFleetsOutputTypeDef](./type_defs.md#listinstancefleetsoutputtypedef)
- [JobFlowDetailTypeDef](./type_defs.md#jobflowdetailtypedef)
- [InstanceGroupPaginatorTypeDef](./type_defs.md#instancegrouppaginatortypedef)
- [InstanceGroupTypeDef](./type_defs.md#instancegrouptypedef)
- [PutAutoScalingPolicyOutputTypeDef](./type_defs.md#putautoscalingpolicyoutputtypedef)
- [ScalingRuleTypeDef](./type_defs.md#scalingruletypedef)
- [AddInstanceFleetInputTypeDef](./type_defs.md#addinstancefleetinputtypedef)
- [ModifyInstanceFleetInputTypeDef](./type_defs.md#modifyinstancefleetinputtypedef)
- [AddJobFlowStepsInputTypeDef](./type_defs.md#addjobflowstepsinputtypedef)
- [ModifyInstanceGroupsInputTypeDef](./type_defs.md#modifyinstancegroupsinputtypedef)
- [DescribeJobFlowsOutputTypeDef](./type_defs.md#describejobflowsoutputtypedef)
- [ListInstanceGroupsOutputPaginatorTypeDef](./type_defs.md#listinstancegroupsoutputpaginatortypedef)
- [ListInstanceGroupsOutputTypeDef](./type_defs.md#listinstancegroupsoutputtypedef)
- [ScalingRuleUnionTypeDef](./type_defs.md#scalingruleuniontypedef)
- [AutoScalingPolicyTypeDef](./type_defs.md#autoscalingpolicytypedef)
- [InstanceGroupConfigTypeDef](./type_defs.md#instancegroupconfigtypedef)
- [PutAutoScalingPolicyInputTypeDef](./type_defs.md#putautoscalingpolicyinputtypedef)
- [AddInstanceGroupsInputTypeDef](./type_defs.md#addinstancegroupsinputtypedef)
- [JobFlowInstancesConfigTypeDef](./type_defs.md#jobflowinstancesconfigtypedef)
- [RunJobFlowInputTypeDef](./type_defs.md#runjobflowinputtypedef)

