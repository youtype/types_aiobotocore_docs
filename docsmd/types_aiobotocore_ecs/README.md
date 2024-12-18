# ECS module

> [Index](../README.md) > ECS


!!! note ""

    Auto-generated documentation for [ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ecs)
    type annotations stubs module [types-aiobotocore-ecs](https://pypi.org/project/types-aiobotocore-ecs/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ECS` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ECS` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ecs]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ecs]'

# standalone installation
python -m pip install types-aiobotocore-ecs
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ecs
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ECSClient

Type annotations and code completion for  `#!python session.create_client("ecs")` as [ECSClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ECS.Client)

```python
# ECSClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecs.client import ECSClient


session = get_session()
async with session.create_client("ecs") as client:
    client: ECSClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("ecs").get_paginator("...")`.

```python
# ListAccountSettingsPaginator usage example

from types_aiobotocore_ecs.paginator import ListAccountSettingsPaginator

def get_list_account_settings_paginator() -> ListAccountSettingsPaginator:
    return client.get_paginator("list_account_settings"))
```

- [ListAccountSettingsPaginator](./paginators.md#listaccountsettingspaginator)
- [ListAttributesPaginator](./paginators.md#listattributespaginator)
- [ListClustersPaginator](./paginators.md#listclusterspaginator)
- [ListContainerInstancesPaginator](./paginators.md#listcontainerinstancespaginator)
- [ListServicesByNamespacePaginator](./paginators.md#listservicesbynamespacepaginator)
- [ListServicesPaginator](./paginators.md#listservicespaginator)
- [ListTaskDefinitionFamiliesPaginator](./paginators.md#listtaskdefinitionfamiliespaginator)
- [ListTaskDefinitionsPaginator](./paginators.md#listtaskdefinitionspaginator)
- [ListTasksPaginator](./paginators.md#listtaskspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("ecs").get_waiter("...")`.

```python
# ServicesInactiveWaiter usage example

from types_aiobotocore_ecs.waiter import ServicesInactiveWaiter

def get_services_inactive_waiter() -> ServicesInactiveWaiter:
    return Session().client("ecs").get_waiter("services_inactive")
```

- [ServicesInactiveWaiter](./waiters.md#servicesinactivewaiter)
- [ServicesStableWaiter](./waiters.md#servicesstablewaiter)
- [TasksRunningWaiter](./waiters.md#tasksrunningwaiter)
- [TasksStoppedWaiter](./waiters.md#tasksstoppedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AgentUpdateStatusType usage example

from types_aiobotocore_ecs.literals import AgentUpdateStatusType

def get_value() -> AgentUpdateStatusType:
    return "FAILED"
```

- [AgentUpdateStatusType](./literals.md#agentupdatestatustype)
- [ApplicationProtocolType](./literals.md#applicationprotocoltype)
- [AssignPublicIpType](./literals.md#assignpubliciptype)
- [AvailabilityZoneRebalancingType](./literals.md#availabilityzonerebalancingtype)
- [CPUArchitectureType](./literals.md#cpuarchitecturetype)
- [CapacityProviderFieldType](./literals.md#capacityproviderfieldtype)
- [CapacityProviderStatusType](./literals.md#capacityproviderstatustype)
- [CapacityProviderUpdateStatusType](./literals.md#capacityproviderupdatestatustype)
- [ClusterFieldType](./literals.md#clusterfieldtype)
- [ClusterSettingNameType](./literals.md#clustersettingnametype)
- [CompatibilityType](./literals.md#compatibilitytype)
- [ConnectivityType](./literals.md#connectivitytype)
- [ContainerConditionType](./literals.md#containerconditiontype)
- [ContainerInstanceFieldType](./literals.md#containerinstancefieldtype)
- [ContainerInstanceStatusType](./literals.md#containerinstancestatustype)
- [DeploymentControllerTypeType](./literals.md#deploymentcontrollertypetype)
- [DeploymentRolloutStateType](./literals.md#deploymentrolloutstatetype)
- [DesiredStatusType](./literals.md#desiredstatustype)
- [DeviceCgroupPermissionType](./literals.md#devicecgrouppermissiontype)
- [EBSResourceTypeType](./literals.md#ebsresourcetypetype)
- [EFSAuthorizationConfigIAMType](./literals.md#efsauthorizationconfigiamtype)
- [EFSTransitEncryptionType](./literals.md#efstransitencryptiontype)
- [EnvironmentFileTypeType](./literals.md#environmentfiletypetype)
- [ExecuteCommandLoggingType](./literals.md#executecommandloggingtype)
- [FirelensConfigurationTypeType](./literals.md#firelensconfigurationtypetype)
- [HealthStatusType](./literals.md#healthstatustype)
- [InstanceHealthCheckStateType](./literals.md#instancehealthcheckstatetype)
- [InstanceHealthCheckTypeType](./literals.md#instancehealthchecktypetype)
- [IpcModeType](./literals.md#ipcmodetype)
- [LaunchTypeType](./literals.md#launchtypetype)
- [ListAccountSettingsPaginatorName](./literals.md#listaccountsettingspaginatorname)
- [ListAttributesPaginatorName](./literals.md#listattributespaginatorname)
- [ListClustersPaginatorName](./literals.md#listclusterspaginatorname)
- [ListContainerInstancesPaginatorName](./literals.md#listcontainerinstancespaginatorname)
- [ListServicesByNamespacePaginatorName](./literals.md#listservicesbynamespacepaginatorname)
- [ListServicesPaginatorName](./literals.md#listservicespaginatorname)
- [ListTaskDefinitionFamiliesPaginatorName](./literals.md#listtaskdefinitionfamiliespaginatorname)
- [ListTaskDefinitionsPaginatorName](./literals.md#listtaskdefinitionspaginatorname)
- [ListTasksPaginatorName](./literals.md#listtaskspaginatorname)
- [LogDriverType](./literals.md#logdrivertype)
- [ManagedAgentNameType](./literals.md#managedagentnametype)
- [ManagedDrainingType](./literals.md#manageddrainingtype)
- [ManagedScalingStatusType](./literals.md#managedscalingstatustype)
- [ManagedTerminationProtectionType](./literals.md#managedterminationprotectiontype)
- [NetworkModeType](./literals.md#networkmodetype)
- [OSFamilyType](./literals.md#osfamilytype)
- [PidModeType](./literals.md#pidmodetype)
- [PlacementConstraintTypeType](./literals.md#placementconstrainttypetype)
- [PlacementStrategyTypeType](./literals.md#placementstrategytypetype)
- [PlatformDeviceTypeType](./literals.md#platformdevicetypetype)
- [PropagateTagsType](./literals.md#propagatetagstype)
- [ProxyConfigurationTypeType](./literals.md#proxyconfigurationtypetype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [ScaleUnitType](./literals.md#scaleunittype)
- [SchedulingStrategyType](./literals.md#schedulingstrategytype)
- [ScopeType](./literals.md#scopetype)
- [ServiceDeploymentRollbackMonitorsStatusType](./literals.md#servicedeploymentrollbackmonitorsstatustype)
- [ServiceDeploymentStatusType](./literals.md#servicedeploymentstatustype)
- [ServiceFieldType](./literals.md#servicefieldtype)
- [ServicesInactiveWaiterName](./literals.md#servicesinactivewaitername)
- [ServicesStableWaiterName](./literals.md#servicesstablewaitername)
- [SettingNameType](./literals.md#settingnametype)
- [SettingTypeType](./literals.md#settingtypetype)
- [SortOrderType](./literals.md#sortordertype)
- [StabilityStatusType](./literals.md#stabilitystatustype)
- [TargetTypeType](./literals.md#targettypetype)
- [TaskDefinitionFamilyStatusType](./literals.md#taskdefinitionfamilystatustype)
- [TaskDefinitionFieldType](./literals.md#taskdefinitionfieldtype)
- [TaskDefinitionPlacementConstraintTypeType](./literals.md#taskdefinitionplacementconstrainttypetype)
- [TaskDefinitionStatusType](./literals.md#taskdefinitionstatustype)
- [TaskFieldType](./literals.md#taskfieldtype)
- [TaskFilesystemTypeType](./literals.md#taskfilesystemtypetype)
- [TaskSetFieldType](./literals.md#tasksetfieldtype)
- [TaskStopCodeType](./literals.md#taskstopcodetype)
- [TasksRunningWaiterName](./literals.md#tasksrunningwaitername)
- [TasksStoppedWaiterName](./literals.md#tasksstoppedwaitername)
- [TransportProtocolType](./literals.md#transportprotocoltype)
- [UlimitNameType](./literals.md#ulimitnametype)
- [VersionConsistencyType](./literals.md#versionconsistencytype)
- [ECSServiceName](./literals.md#ecsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AttachmentStateChangeTypeDef](./type_defs.md#attachmentstatechangetypedef)
- [KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef)
- [AttributeTypeDef](./type_defs.md#attributetypedef)
- [ManagedScalingTypeDef](./type_defs.md#managedscalingtypedef)
- [AwsVpcConfigurationOutputTypeDef](./type_defs.md#awsvpcconfigurationoutputtypedef)
- [AwsVpcConfigurationTypeDef](./type_defs.md#awsvpcconfigurationtypedef)
- [CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ManagedStorageConfigurationTypeDef](./type_defs.md#managedstorageconfigurationtypedef)
- [ClusterServiceConnectDefaultsRequestTypeDef](./type_defs.md#clusterserviceconnectdefaultsrequesttypedef)
- [ClusterServiceConnectDefaultsTypeDef](./type_defs.md#clusterserviceconnectdefaultstypedef)
- [ClusterSettingTypeDef](./type_defs.md#clustersettingtypedef)
- [ContainerDependencyTypeDef](./type_defs.md#containerdependencytypedef)
- [ContainerRestartPolicyOutputTypeDef](./type_defs.md#containerrestartpolicyoutputtypedef)
- [EnvironmentFileTypeDef](./type_defs.md#environmentfiletypedef)
- [FirelensConfigurationOutputTypeDef](./type_defs.md#firelensconfigurationoutputtypedef)
- [HealthCheckOutputTypeDef](./type_defs.md#healthcheckoutputtypedef)
- [HostEntryTypeDef](./type_defs.md#hostentrytypedef)
- [MountPointTypeDef](./type_defs.md#mountpointtypedef)
- [PortMappingTypeDef](./type_defs.md#portmappingtypedef)
- [RepositoryCredentialsTypeDef](./type_defs.md#repositorycredentialstypedef)
- [ResourceRequirementTypeDef](./type_defs.md#resourcerequirementtypedef)
- [SecretTypeDef](./type_defs.md#secrettypedef)
- [SystemControlTypeDef](./type_defs.md#systemcontroltypedef)
- [UlimitTypeDef](./type_defs.md#ulimittypedef)
- [VolumeFromTypeDef](./type_defs.md#volumefromtypedef)
- [ContainerImageTypeDef](./type_defs.md#containerimagetypedef)
- [InstanceHealthCheckResultTypeDef](./type_defs.md#instancehealthcheckresulttypedef)
- [ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef)
- [VersionInfoTypeDef](./type_defs.md#versioninfotypedef)
- [ContainerRestartPolicyTypeDef](./type_defs.md#containerrestartpolicytypedef)
- [NetworkBindingTypeDef](./type_defs.md#networkbindingtypedef)
- [ManagedAgentTypeDef](./type_defs.md#managedagenttypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeploymentControllerTypeDef](./type_defs.md#deploymentcontrollertypedef)
- [LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef)
- [PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef)
- [PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef)
- [ServiceRegistryTypeDef](./type_defs.md#serviceregistrytypedef)
- [VpcLatticeConfigurationTypeDef](./type_defs.md#vpclatticeconfigurationtypedef)
- [ScaleTypeDef](./type_defs.md#scaletypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DeleteAccountSettingRequestRequestTypeDef](./type_defs.md#deleteaccountsettingrequestrequesttypedef)
- [SettingTypeDef](./type_defs.md#settingtypedef)
- [DeleteCapacityProviderRequestRequestTypeDef](./type_defs.md#deletecapacityproviderrequestrequesttypedef)
- [DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef)
- [DeleteServiceRequestRequestTypeDef](./type_defs.md#deleteservicerequestrequesttypedef)
- [DeleteTaskDefinitionsRequestRequestTypeDef](./type_defs.md#deletetaskdefinitionsrequestrequesttypedef)
- [FailureTypeDef](./type_defs.md#failuretypedef)
- [DeleteTaskSetRequestRequestTypeDef](./type_defs.md#deletetasksetrequestrequesttypedef)
- [DeploymentAlarmsOutputTypeDef](./type_defs.md#deploymentalarmsoutputtypedef)
- [DeploymentAlarmsTypeDef](./type_defs.md#deploymentalarmstypedef)
- [DeploymentCircuitBreakerTypeDef](./type_defs.md#deploymentcircuitbreakertypedef)
- [DeploymentEphemeralStorageTypeDef](./type_defs.md#deploymentephemeralstoragetypedef)
- [ServiceConnectServiceResourceTypeDef](./type_defs.md#serviceconnectserviceresourcetypedef)
- [DeregisterContainerInstanceRequestRequestTypeDef](./type_defs.md#deregistercontainerinstancerequestrequesttypedef)
- [DeregisterTaskDefinitionRequestRequestTypeDef](./type_defs.md#deregistertaskdefinitionrequestrequesttypedef)
- [DescribeCapacityProvidersRequestRequestTypeDef](./type_defs.md#describecapacityprovidersrequestrequesttypedef)
- [DescribeClustersRequestRequestTypeDef](./type_defs.md#describeclustersrequestrequesttypedef)
- [DescribeContainerInstancesRequestRequestTypeDef](./type_defs.md#describecontainerinstancesrequestrequesttypedef)
- [DescribeServiceDeploymentsRequestRequestTypeDef](./type_defs.md#describeservicedeploymentsrequestrequesttypedef)
- [DescribeServiceRevisionsRequestRequestTypeDef](./type_defs.md#describeservicerevisionsrequestrequesttypedef)
- [DescribeServicesRequestRequestTypeDef](./type_defs.md#describeservicesrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeTaskDefinitionRequestRequestTypeDef](./type_defs.md#describetaskdefinitionrequestrequesttypedef)
- [DescribeTaskSetsRequestRequestTypeDef](./type_defs.md#describetasksetsrequestrequesttypedef)
- [DescribeTasksRequestRequestTypeDef](./type_defs.md#describetasksrequestrequesttypedef)
- [DeviceOutputTypeDef](./type_defs.md#deviceoutputtypedef)
- [DeviceTypeDef](./type_defs.md#devicetypedef)
- [DiscoverPollEndpointRequestRequestTypeDef](./type_defs.md#discoverpollendpointrequestrequesttypedef)
- [DockerVolumeConfigurationOutputTypeDef](./type_defs.md#dockervolumeconfigurationoutputtypedef)
- [DockerVolumeConfigurationTypeDef](./type_defs.md#dockervolumeconfigurationtypedef)
- [EFSAuthorizationConfigTypeDef](./type_defs.md#efsauthorizationconfigtypedef)
- [EphemeralStorageTypeDef](./type_defs.md#ephemeralstoragetypedef)
- [ExecuteCommandLogConfigurationTypeDef](./type_defs.md#executecommandlogconfigurationtypedef)
- [ExecuteCommandRequestRequestTypeDef](./type_defs.md#executecommandrequestrequesttypedef)
- [SessionTypeDef](./type_defs.md#sessiontypedef)
- [FSxWindowsFileServerAuthorizationConfigTypeDef](./type_defs.md#fsxwindowsfileserverauthorizationconfigtypedef)
- [FirelensConfigurationTypeDef](./type_defs.md#firelensconfigurationtypedef)
- [GetTaskProtectionRequestRequestTypeDef](./type_defs.md#gettaskprotectionrequestrequesttypedef)
- [ProtectedTaskTypeDef](./type_defs.md#protectedtasktypedef)
- [HealthCheckTypeDef](./type_defs.md#healthchecktypedef)
- [HostVolumePropertiesTypeDef](./type_defs.md#hostvolumepropertiestypedef)
- [InferenceAcceleratorOverrideTypeDef](./type_defs.md#inferenceacceleratoroverridetypedef)
- [InferenceAcceleratorTypeDef](./type_defs.md#inferenceacceleratortypedef)
- [KernelCapabilitiesOutputTypeDef](./type_defs.md#kernelcapabilitiesoutputtypedef)
- [KernelCapabilitiesTypeDef](./type_defs.md#kernelcapabilitiestypedef)
- [TmpfsOutputTypeDef](./type_defs.md#tmpfsoutputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAccountSettingsRequestRequestTypeDef](./type_defs.md#listaccountsettingsrequestrequesttypedef)
- [ListAttributesRequestRequestTypeDef](./type_defs.md#listattributesrequestrequesttypedef)
- [ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef)
- [ListContainerInstancesRequestRequestTypeDef](./type_defs.md#listcontainerinstancesrequestrequesttypedef)
- [ServiceDeploymentBriefTypeDef](./type_defs.md#servicedeploymentbrieftypedef)
- [ListServicesByNamespaceRequestRequestTypeDef](./type_defs.md#listservicesbynamespacerequestrequesttypedef)
- [ListServicesRequestRequestTypeDef](./type_defs.md#listservicesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTaskDefinitionFamiliesRequestRequestTypeDef](./type_defs.md#listtaskdefinitionfamiliesrequestrequesttypedef)
- [ListTaskDefinitionsRequestRequestTypeDef](./type_defs.md#listtaskdefinitionsrequestrequesttypedef)
- [ListTasksRequestRequestTypeDef](./type_defs.md#listtasksrequestrequesttypedef)
- [ManagedAgentStateChangeTypeDef](./type_defs.md#managedagentstatechangetypedef)
- [PlatformDeviceTypeDef](./type_defs.md#platformdevicetypedef)
- [PutAccountSettingDefaultRequestRequestTypeDef](./type_defs.md#putaccountsettingdefaultrequestrequesttypedef)
- [PutAccountSettingRequestRequestTypeDef](./type_defs.md#putaccountsettingrequestrequesttypedef)
- [RuntimePlatformTypeDef](./type_defs.md#runtimeplatformtypedef)
- [TaskDefinitionPlacementConstraintTypeDef](./type_defs.md#taskdefinitionplacementconstrainttypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [RollbackTypeDef](./type_defs.md#rollbacktypedef)
- [ServiceConnectClientAliasTypeDef](./type_defs.md#serviceconnectclientaliastypedef)
- [TimeoutConfigurationTypeDef](./type_defs.md#timeoutconfigurationtypedef)
- [ServiceConnectTlsCertificateAuthorityTypeDef](./type_defs.md#serviceconnecttlscertificateauthoritytypedef)
- [ServiceDeploymentAlarmsTypeDef](./type_defs.md#servicedeploymentalarmstypedef)
- [ServiceDeploymentCircuitBreakerTypeDef](./type_defs.md#servicedeploymentcircuitbreakertypedef)
- [ServiceRevisionSummaryTypeDef](./type_defs.md#servicerevisionsummarytypedef)
- [ServiceEventTypeDef](./type_defs.md#serviceeventtypedef)
- [StopTaskRequestRequestTypeDef](./type_defs.md#stoptaskrequestrequesttypedef)
- [TaskEphemeralStorageTypeDef](./type_defs.md#taskephemeralstoragetypedef)
- [TaskManagedEBSVolumeTerminationPolicyTypeDef](./type_defs.md#taskmanagedebsvolumeterminationpolicytypedef)
- [TmpfsTypeDef](./type_defs.md#tmpfstypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateContainerAgentRequestRequestTypeDef](./type_defs.md#updatecontaineragentrequestrequesttypedef)
- [UpdateContainerInstancesStateRequestRequestTypeDef](./type_defs.md#updatecontainerinstancesstaterequestrequesttypedef)
- [UpdateServicePrimaryTaskSetRequestRequestTypeDef](./type_defs.md#updateserviceprimarytasksetrequestrequesttypedef)
- [UpdateTaskProtectionRequestRequestTypeDef](./type_defs.md#updatetaskprotectionrequestrequesttypedef)
- [SubmitAttachmentStateChangesRequestRequestTypeDef](./type_defs.md#submitattachmentstatechangesrequestrequesttypedef)
- [AttachmentTypeDef](./type_defs.md#attachmenttypedef)
- [ProxyConfigurationOutputTypeDef](./type_defs.md#proxyconfigurationoutputtypedef)
- [ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef)
- [DeleteAttributesRequestRequestTypeDef](./type_defs.md#deleteattributesrequestrequesttypedef)
- [PutAttributesRequestRequestTypeDef](./type_defs.md#putattributesrequestrequesttypedef)
- [AutoScalingGroupProviderTypeDef](./type_defs.md#autoscalinggroupprovidertypedef)
- [AutoScalingGroupProviderUpdateTypeDef](./type_defs.md#autoscalinggroupproviderupdatetypedef)
- [NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef)
- [AwsVpcConfigurationUnionTypeDef](./type_defs.md#awsvpcconfigurationuniontypedef)
- [PutClusterCapacityProvidersRequestRequestTypeDef](./type_defs.md#putclustercapacityprovidersrequestrequesttypedef)
- [EBSTagSpecificationOutputTypeDef](./type_defs.md#ebstagspecificationoutputtypedef)
- [EBSTagSpecificationTypeDef](./type_defs.md#ebstagspecificationtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UpdateClusterSettingsRequestRequestTypeDef](./type_defs.md#updateclustersettingsrequestrequesttypedef)
- [ContainerOverrideOutputTypeDef](./type_defs.md#containeroverrideoutputtypedef)
- [ContainerOverrideTypeDef](./type_defs.md#containeroverridetypedef)
- [LogConfigurationOutputTypeDef](./type_defs.md#logconfigurationoutputtypedef)
- [LogConfigurationTypeDef](./type_defs.md#logconfigurationtypedef)
- [ContainerInstanceHealthStatusTypeDef](./type_defs.md#containerinstancehealthstatustypedef)
- [ContainerRestartPolicyUnionTypeDef](./type_defs.md#containerrestartpolicyuniontypedef)
- [ContainerStateChangeTypeDef](./type_defs.md#containerstatechangetypedef)
- [SubmitContainerStateChangeRequestRequestTypeDef](./type_defs.md#submitcontainerstatechangerequestrequesttypedef)
- [ContainerTypeDef](./type_defs.md#containertypedef)
- [DeleteAttributesResponseTypeDef](./type_defs.md#deleteattributesresponsetypedef)
- [DiscoverPollEndpointResponseTypeDef](./type_defs.md#discoverpollendpointresponsetypedef)
- [ListAttributesResponseTypeDef](./type_defs.md#listattributesresponsetypedef)
- [ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef)
- [ListContainerInstancesResponseTypeDef](./type_defs.md#listcontainerinstancesresponsetypedef)
- [ListServicesByNamespaceResponseTypeDef](./type_defs.md#listservicesbynamespaceresponsetypedef)
- [ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListTaskDefinitionFamiliesResponseTypeDef](./type_defs.md#listtaskdefinitionfamiliesresponsetypedef)
- [ListTaskDefinitionsResponseTypeDef](./type_defs.md#listtaskdefinitionsresponsetypedef)
- [ListTasksResponseTypeDef](./type_defs.md#listtasksresponsetypedef)
- [PutAttributesResponseTypeDef](./type_defs.md#putattributesresponsetypedef)
- [SubmitAttachmentStateChangesResponseTypeDef](./type_defs.md#submitattachmentstatechangesresponsetypedef)
- [SubmitContainerStateChangeResponseTypeDef](./type_defs.md#submitcontainerstatechangeresponsetypedef)
- [SubmitTaskStateChangeResponseTypeDef](./type_defs.md#submittaskstatechangeresponsetypedef)
- [UpdateTaskSetRequestRequestTypeDef](./type_defs.md#updatetasksetrequestrequesttypedef)
- [CreatedAtTypeDef](./type_defs.md#createdattypedef)
- [DeleteAccountSettingResponseTypeDef](./type_defs.md#deleteaccountsettingresponsetypedef)
- [ListAccountSettingsResponseTypeDef](./type_defs.md#listaccountsettingsresponsetypedef)
- [PutAccountSettingDefaultResponseTypeDef](./type_defs.md#putaccountsettingdefaultresponsetypedef)
- [PutAccountSettingResponseTypeDef](./type_defs.md#putaccountsettingresponsetypedef)
- [DeploymentAlarmsUnionTypeDef](./type_defs.md#deploymentalarmsuniontypedef)
- [DeploymentConfigurationOutputTypeDef](./type_defs.md#deploymentconfigurationoutputtypedef)
- [DescribeServicesRequestServicesInactiveWaitTypeDef](./type_defs.md#describeservicesrequestservicesinactivewaittypedef)
- [DescribeServicesRequestServicesStableWaitTypeDef](./type_defs.md#describeservicesrequestservicesstablewaittypedef)
- [DescribeTasksRequestTasksRunningWaitTypeDef](./type_defs.md#describetasksrequesttasksrunningwaittypedef)
- [DescribeTasksRequestTasksStoppedWaitTypeDef](./type_defs.md#describetasksrequesttasksstoppedwaittypedef)
- [DeviceUnionTypeDef](./type_defs.md#deviceuniontypedef)
- [DockerVolumeConfigurationUnionTypeDef](./type_defs.md#dockervolumeconfigurationuniontypedef)
- [EFSVolumeConfigurationTypeDef](./type_defs.md#efsvolumeconfigurationtypedef)
- [ExecuteCommandConfigurationTypeDef](./type_defs.md#executecommandconfigurationtypedef)
- [ExecuteCommandResponseTypeDef](./type_defs.md#executecommandresponsetypedef)
- [FSxWindowsFileServerVolumeConfigurationTypeDef](./type_defs.md#fsxwindowsfileservervolumeconfigurationtypedef)
- [FirelensConfigurationUnionTypeDef](./type_defs.md#firelensconfigurationuniontypedef)
- [GetTaskProtectionResponseTypeDef](./type_defs.md#gettaskprotectionresponsetypedef)
- [UpdateTaskProtectionResponseTypeDef](./type_defs.md#updatetaskprotectionresponsetypedef)
- [HealthCheckUnionTypeDef](./type_defs.md#healthcheckuniontypedef)
- [KernelCapabilitiesUnionTypeDef](./type_defs.md#kernelcapabilitiesuniontypedef)
- [LinuxParametersOutputTypeDef](./type_defs.md#linuxparametersoutputtypedef)
- [ListAccountSettingsRequestListAccountSettingsPaginateTypeDef](./type_defs.md#listaccountsettingsrequestlistaccountsettingspaginatetypedef)
- [ListAttributesRequestListAttributesPaginateTypeDef](./type_defs.md#listattributesrequestlistattributespaginatetypedef)
- [ListClustersRequestListClustersPaginateTypeDef](./type_defs.md#listclustersrequestlistclusterspaginatetypedef)
- [ListContainerInstancesRequestListContainerInstancesPaginateTypeDef](./type_defs.md#listcontainerinstancesrequestlistcontainerinstancespaginatetypedef)
- [ListServicesByNamespaceRequestListServicesByNamespacePaginateTypeDef](./type_defs.md#listservicesbynamespacerequestlistservicesbynamespacepaginatetypedef)
- [ListServicesRequestListServicesPaginateTypeDef](./type_defs.md#listservicesrequestlistservicespaginatetypedef)
- [ListTaskDefinitionFamiliesRequestListTaskDefinitionFamiliesPaginateTypeDef](./type_defs.md#listtaskdefinitionfamiliesrequestlisttaskdefinitionfamiliespaginatetypedef)
- [ListTaskDefinitionsRequestListTaskDefinitionsPaginateTypeDef](./type_defs.md#listtaskdefinitionsrequestlisttaskdefinitionspaginatetypedef)
- [ListTasksRequestListTasksPaginateTypeDef](./type_defs.md#listtasksrequestlisttaskspaginatetypedef)
- [ListServiceDeploymentsResponseTypeDef](./type_defs.md#listservicedeploymentsresponsetypedef)
- [ResourceUnionTypeDef](./type_defs.md#resourceuniontypedef)
- [ServiceConnectTlsConfigurationTypeDef](./type_defs.md#serviceconnecttlsconfigurationtypedef)
- [TmpfsUnionTypeDef](./type_defs.md#tmpfsuniontypedef)
- [CapacityProviderTypeDef](./type_defs.md#capacityprovidertypedef)
- [CreateCapacityProviderRequestRequestTypeDef](./type_defs.md#createcapacityproviderrequestrequesttypedef)
- [UpdateCapacityProviderRequestRequestTypeDef](./type_defs.md#updatecapacityproviderrequestrequesttypedef)
- [TaskSetTypeDef](./type_defs.md#tasksettypedef)
- [NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef)
- [ServiceManagedEBSVolumeConfigurationOutputTypeDef](./type_defs.md#servicemanagedebsvolumeconfigurationoutputtypedef)
- [EBSTagSpecificationUnionTypeDef](./type_defs.md#ebstagspecificationuniontypedef)
- [TaskOverrideOutputTypeDef](./type_defs.md#taskoverrideoutputtypedef)
- [ContainerOverrideUnionTypeDef](./type_defs.md#containeroverrideuniontypedef)
- [LogConfigurationUnionTypeDef](./type_defs.md#logconfigurationuniontypedef)
- [ContainerInstanceTypeDef](./type_defs.md#containerinstancetypedef)
- [SubmitTaskStateChangeRequestRequestTypeDef](./type_defs.md#submittaskstatechangerequestrequesttypedef)
- [ListServiceDeploymentsRequestRequestTypeDef](./type_defs.md#listservicedeploymentsrequestrequesttypedef)
- [DeploymentConfigurationTypeDef](./type_defs.md#deploymentconfigurationtypedef)
- [ServiceDeploymentTypeDef](./type_defs.md#servicedeploymenttypedef)
- [ClusterConfigurationTypeDef](./type_defs.md#clusterconfigurationtypedef)
- [VolumeOutputTypeDef](./type_defs.md#volumeoutputtypedef)
- [VolumeTypeDef](./type_defs.md#volumetypedef)
- [ContainerDefinitionOutputTypeDef](./type_defs.md#containerdefinitionoutputtypedef)
- [RegisterContainerInstanceRequestRequestTypeDef](./type_defs.md#registercontainerinstancerequestrequesttypedef)
- [ServiceConnectServiceOutputTypeDef](./type_defs.md#serviceconnectserviceoutputtypedef)
- [ServiceConnectServiceTypeDef](./type_defs.md#serviceconnectservicetypedef)
- [LinuxParametersTypeDef](./type_defs.md#linuxparameterstypedef)
- [CreateCapacityProviderResponseTypeDef](./type_defs.md#createcapacityproviderresponsetypedef)
- [DeleteCapacityProviderResponseTypeDef](./type_defs.md#deletecapacityproviderresponsetypedef)
- [DescribeCapacityProvidersResponseTypeDef](./type_defs.md#describecapacityprovidersresponsetypedef)
- [UpdateCapacityProviderResponseTypeDef](./type_defs.md#updatecapacityproviderresponsetypedef)
- [CreateTaskSetResponseTypeDef](./type_defs.md#createtasksetresponsetypedef)
- [DeleteTaskSetResponseTypeDef](./type_defs.md#deletetasksetresponsetypedef)
- [DescribeTaskSetsResponseTypeDef](./type_defs.md#describetasksetsresponsetypedef)
- [UpdateServicePrimaryTaskSetResponseTypeDef](./type_defs.md#updateserviceprimarytasksetresponsetypedef)
- [UpdateTaskSetResponseTypeDef](./type_defs.md#updatetasksetresponsetypedef)
- [CreateTaskSetRequestRequestTypeDef](./type_defs.md#createtasksetrequestrequesttypedef)
- [ServiceVolumeConfigurationOutputTypeDef](./type_defs.md#servicevolumeconfigurationoutputtypedef)
- [ServiceManagedEBSVolumeConfigurationTypeDef](./type_defs.md#servicemanagedebsvolumeconfigurationtypedef)
- [TaskManagedEBSVolumeConfigurationTypeDef](./type_defs.md#taskmanagedebsvolumeconfigurationtypedef)
- [TaskTypeDef](./type_defs.md#tasktypedef)
- [TaskOverrideTypeDef](./type_defs.md#taskoverridetypedef)
- [DeregisterContainerInstanceResponseTypeDef](./type_defs.md#deregistercontainerinstanceresponsetypedef)
- [DescribeContainerInstancesResponseTypeDef](./type_defs.md#describecontainerinstancesresponsetypedef)
- [RegisterContainerInstanceResponseTypeDef](./type_defs.md#registercontainerinstanceresponsetypedef)
- [UpdateContainerAgentResponseTypeDef](./type_defs.md#updatecontaineragentresponsetypedef)
- [UpdateContainerInstancesStateResponseTypeDef](./type_defs.md#updatecontainerinstancesstateresponsetypedef)
- [DescribeServiceDeploymentsResponseTypeDef](./type_defs.md#describeservicedeploymentsresponsetypedef)
- [ClusterTypeDef](./type_defs.md#clustertypedef)
- [CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef)
- [UpdateClusterRequestRequestTypeDef](./type_defs.md#updateclusterrequestrequesttypedef)
- [VolumeUnionTypeDef](./type_defs.md#volumeuniontypedef)
- [TaskDefinitionTypeDef](./type_defs.md#taskdefinitiontypedef)
- [ServiceConnectConfigurationOutputTypeDef](./type_defs.md#serviceconnectconfigurationoutputtypedef)
- [ServiceConnectServiceUnionTypeDef](./type_defs.md#serviceconnectserviceuniontypedef)
- [LinuxParametersUnionTypeDef](./type_defs.md#linuxparametersuniontypedef)
- [ServiceManagedEBSVolumeConfigurationUnionTypeDef](./type_defs.md#servicemanagedebsvolumeconfigurationuniontypedef)
- [TaskVolumeConfigurationTypeDef](./type_defs.md#taskvolumeconfigurationtypedef)
- [DescribeTasksResponseTypeDef](./type_defs.md#describetasksresponsetypedef)
- [RunTaskResponseTypeDef](./type_defs.md#runtaskresponsetypedef)
- [StartTaskResponseTypeDef](./type_defs.md#starttaskresponsetypedef)
- [StopTaskResponseTypeDef](./type_defs.md#stoptaskresponsetypedef)
- [CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef)
- [DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef)
- [DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef)
- [PutClusterCapacityProvidersResponseTypeDef](./type_defs.md#putclustercapacityprovidersresponsetypedef)
- [UpdateClusterResponseTypeDef](./type_defs.md#updateclusterresponsetypedef)
- [UpdateClusterSettingsResponseTypeDef](./type_defs.md#updateclustersettingsresponsetypedef)
- [DeleteTaskDefinitionsResponseTypeDef](./type_defs.md#deletetaskdefinitionsresponsetypedef)
- [DeregisterTaskDefinitionResponseTypeDef](./type_defs.md#deregistertaskdefinitionresponsetypedef)
- [DescribeTaskDefinitionResponseTypeDef](./type_defs.md#describetaskdefinitionresponsetypedef)
- [RegisterTaskDefinitionResponseTypeDef](./type_defs.md#registertaskdefinitionresponsetypedef)
- [DeploymentTypeDef](./type_defs.md#deploymenttypedef)
- [ServiceRevisionTypeDef](./type_defs.md#servicerevisiontypedef)
- [ServiceConnectConfigurationTypeDef](./type_defs.md#serviceconnectconfigurationtypedef)
- [ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef)
- [ServiceVolumeConfigurationTypeDef](./type_defs.md#servicevolumeconfigurationtypedef)
- [RunTaskRequestRequestTypeDef](./type_defs.md#runtaskrequestrequesttypedef)
- [StartTaskRequestRequestTypeDef](./type_defs.md#starttaskrequestrequesttypedef)
- [ServiceTypeDef](./type_defs.md#servicetypedef)
- [DescribeServiceRevisionsResponseTypeDef](./type_defs.md#describeservicerevisionsresponsetypedef)
- [ContainerDefinitionUnionTypeDef](./type_defs.md#containerdefinitionuniontypedef)
- [ServiceVolumeConfigurationUnionTypeDef](./type_defs.md#servicevolumeconfigurationuniontypedef)
- [UpdateServiceRequestRequestTypeDef](./type_defs.md#updateservicerequestrequesttypedef)
- [CreateServiceResponseTypeDef](./type_defs.md#createserviceresponsetypedef)
- [DeleteServiceResponseTypeDef](./type_defs.md#deleteserviceresponsetypedef)
- [DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef)
- [UpdateServiceResponseTypeDef](./type_defs.md#updateserviceresponsetypedef)
- [RegisterTaskDefinitionRequestRequestTypeDef](./type_defs.md#registertaskdefinitionrequestrequesttypedef)
- [CreateServiceRequestRequestTypeDef](./type_defs.md#createservicerequestrequesttypedef)

