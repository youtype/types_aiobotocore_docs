# OpsWorks module

> [Index](../README.md) > OpsWorks


!!! note ""

    Auto-generated documentation for [OpsWorks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#opsworks)
    type annotations stubs module [types-aiobotocore-opsworks](https://pypi.org/project/types-aiobotocore-opsworks/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `OpsWorks` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `OpsWorks` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[opsworks]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[opsworks]'

# standalone installation
python -m pip install types-aiobotocore-opsworks
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-opsworks
```

## Usage

Code samples can be found in [Examples](./usage.md).

## OpsWorksClient

Type annotations and code completion for  `#!python session.create_client("opsworks")` as [OpsWorksClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks.html#OpsWorks.Client)

```python
# OpsWorksClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_opsworks.client import OpsWorksClient


session = get_session()
async with session.create_client("opsworks") as client:
    client: OpsWorksClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("opsworks").get_paginator("...")`.

```python
# DescribeEcsClustersPaginator usage example

from types_aiobotocore_opsworks.paginator import DescribeEcsClustersPaginator

def get_describe_ecs_clusters_paginator() -> DescribeEcsClustersPaginator:
    return client.get_paginator("describe_ecs_clusters"))
```

- [DescribeEcsClustersPaginator](./paginators.md#describeecsclusterspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("opsworks").get_waiter("...")`.

```python
# AppExistsWaiter usage example

from types_aiobotocore_opsworks.waiter import AppExistsWaiter

def get_app_exists_waiter() -> AppExistsWaiter:
    return Session().client("opsworks").get_waiter("app_exists")
```

- [AppExistsWaiter](./waiters.md#appexistswaiter)
- [DeploymentSuccessfulWaiter](./waiters.md#deploymentsuccessfulwaiter)
- [InstanceOnlineWaiter](./waiters.md#instanceonlinewaiter)
- [InstanceRegisteredWaiter](./waiters.md#instanceregisteredwaiter)
- [InstanceStoppedWaiter](./waiters.md#instancestoppedwaiter)
- [InstanceTerminatedWaiter](./waiters.md#instanceterminatedwaiter)




## OpsWorksServiceResource

Type annotations and code completion for `#!python session.resource("opsworks")` as
[OpsWorksServiceResource](./service_resource.md#opsworksserviceresource)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworks/service-resource/index.html)

```python
# OpsWorksServiceResource usage example

from types_aiobotocore_opsworks.service_resource import OpsWorksServiceResource
```


### Collections

Type annotations and code completion for collections
from `#!python session.resource("opsworks").*`.

```python
# ServiceResourceStacksCollection usage example

from types_aiobotocore_opsworks.service_resource import ServiceResourceStacksCollection

def get_collection() -> ServiceResourceStacksCollection:
    return resource.stacks
```

- [ServiceResourceStacksCollection](./service_resource.md#serviceresourcestackscollection)





### Resources

Type annotations and code completion for additional resources
from `#!python session.resource("opsworks").*`.

```python
# Layer usage example

from types_aiobotocore_opsworks.service_resource import Layer

def get_resource() -> Layer:
    return resource.Layer(...)
```

- [Layer](./service_resource.md#layer)
- [Stack](./service_resource.md#stack)
- [StackSummary](./service_resource.md#stacksummary)





## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AppAttributesKeysType usage example

from types_aiobotocore_opsworks.literals import AppAttributesKeysType

def get_value() -> AppAttributesKeysType:
    return "AutoBundleOnDeploy"
```

- [AppAttributesKeysType](./literals.md#appattributeskeystype)
- [AppExistsWaiterName](./literals.md#appexistswaitername)
- [AppTypeType](./literals.md#apptypetype)
- [ArchitectureType](./literals.md#architecturetype)
- [AutoScalingTypeType](./literals.md#autoscalingtypetype)
- [CloudWatchLogsEncodingType](./literals.md#cloudwatchlogsencodingtype)
- [CloudWatchLogsInitialPositionType](./literals.md#cloudwatchlogsinitialpositiontype)
- [CloudWatchLogsTimeZoneType](./literals.md#cloudwatchlogstimezonetype)
- [DeploymentCommandNameType](./literals.md#deploymentcommandnametype)
- [DeploymentSuccessfulWaiterName](./literals.md#deploymentsuccessfulwaitername)
- [DescribeEcsClustersPaginatorName](./literals.md#describeecsclusterspaginatorname)
- [InstanceOnlineWaiterName](./literals.md#instanceonlinewaitername)
- [InstanceRegisteredWaiterName](./literals.md#instanceregisteredwaitername)
- [InstanceStoppedWaiterName](./literals.md#instancestoppedwaitername)
- [InstanceTerminatedWaiterName](./literals.md#instanceterminatedwaitername)
- [LayerAttributesKeysType](./literals.md#layerattributeskeystype)
- [LayerTypeType](./literals.md#layertypetype)
- [RootDeviceTypeType](./literals.md#rootdevicetypetype)
- [SourceTypeType](./literals.md#sourcetypetype)
- [StackAttributesKeysType](./literals.md#stackattributeskeystype)
- [VirtualizationTypeType](./literals.md#virtualizationtypetype)
- [VolumeTypeType](./literals.md#volumetypetype)
- [OpsWorksServiceName](./literals.md#opsworksservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [StackConfigurationManagerTypeDef](./type_defs.md#stackconfigurationmanagertypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [SslConfigurationTypeDef](./type_defs.md#sslconfigurationtypedef)
- [AssignInstanceRequestTypeDef](./type_defs.md#assigninstancerequesttypedef)
- [AssignVolumeRequestTypeDef](./type_defs.md#assignvolumerequesttypedef)
- [AssociateElasticIpRequestTypeDef](./type_defs.md#associateelasticiprequesttypedef)
- [AttachElasticLoadBalancerRequestTypeDef](./type_defs.md#attachelasticloadbalancerrequesttypedef)
- [AutoScalingThresholdsOutputTypeDef](./type_defs.md#autoscalingthresholdsoutputtypedef)
- [AutoScalingThresholdsTypeDef](./type_defs.md#autoscalingthresholdstypedef)
- [EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef)
- [ChefConfigurationTypeDef](./type_defs.md#chefconfigurationtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CloudWatchLogsLogStreamTypeDef](./type_defs.md#cloudwatchlogslogstreamtypedef)
- [CommandTypeDef](./type_defs.md#commandtypedef)
- [VolumeConfigurationTypeDef](./type_defs.md#volumeconfigurationtypedef)
- [CreateUserProfileRequestTypeDef](./type_defs.md#createuserprofilerequesttypedef)
- [DeleteAppRequestTypeDef](./type_defs.md#deleteapprequesttypedef)
- [DeleteInstanceRequestTypeDef](./type_defs.md#deleteinstancerequesttypedef)
- [DeleteLayerRequestTypeDef](./type_defs.md#deletelayerrequesttypedef)
- [DeleteStackRequestTypeDef](./type_defs.md#deletestackrequesttypedef)
- [DeleteUserProfileRequestTypeDef](./type_defs.md#deleteuserprofilerequesttypedef)
- [DeploymentCommandOutputTypeDef](./type_defs.md#deploymentcommandoutputtypedef)
- [DeploymentCommandTypeDef](./type_defs.md#deploymentcommandtypedef)
- [DeregisterEcsClusterRequestTypeDef](./type_defs.md#deregisterecsclusterrequesttypedef)
- [DeregisterElasticIpRequestTypeDef](./type_defs.md#deregisterelasticiprequesttypedef)
- [DeregisterInstanceRequestTypeDef](./type_defs.md#deregisterinstancerequesttypedef)
- [DeregisterRdsDbInstanceRequestTypeDef](./type_defs.md#deregisterrdsdbinstancerequesttypedef)
- [DeregisterVolumeRequestTypeDef](./type_defs.md#deregistervolumerequesttypedef)
- [DescribeAppsRequestTypeDef](./type_defs.md#describeappsrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeCommandsRequestTypeDef](./type_defs.md#describecommandsrequesttypedef)
- [DescribeDeploymentsRequestTypeDef](./type_defs.md#describedeploymentsrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeEcsClustersRequestTypeDef](./type_defs.md#describeecsclustersrequesttypedef)
- [EcsClusterTypeDef](./type_defs.md#ecsclustertypedef)
- [DescribeElasticIpsRequestTypeDef](./type_defs.md#describeelasticipsrequesttypedef)
- [ElasticIpTypeDef](./type_defs.md#elasticiptypedef)
- [DescribeElasticLoadBalancersRequestTypeDef](./type_defs.md#describeelasticloadbalancersrequesttypedef)
- [ElasticLoadBalancerTypeDef](./type_defs.md#elasticloadbalancertypedef)
- [DescribeInstancesRequestTypeDef](./type_defs.md#describeinstancesrequesttypedef)
- [DescribeLayersRequestTypeDef](./type_defs.md#describelayersrequesttypedef)
- [DescribeLoadBasedAutoScalingRequestTypeDef](./type_defs.md#describeloadbasedautoscalingrequesttypedef)
- [SelfUserProfileTypeDef](./type_defs.md#selfuserprofiletypedef)
- [DescribePermissionsRequestTypeDef](./type_defs.md#describepermissionsrequesttypedef)
- [PermissionTypeDef](./type_defs.md#permissiontypedef)
- [DescribeRaidArraysRequestTypeDef](./type_defs.md#describeraidarraysrequesttypedef)
- [RaidArrayTypeDef](./type_defs.md#raidarraytypedef)
- [DescribeRdsDbInstancesRequestTypeDef](./type_defs.md#describerdsdbinstancesrequesttypedef)
- [RdsDbInstanceTypeDef](./type_defs.md#rdsdbinstancetypedef)
- [DescribeServiceErrorsRequestTypeDef](./type_defs.md#describeserviceerrorsrequesttypedef)
- [ServiceErrorTypeDef](./type_defs.md#serviceerrortypedef)
- [DescribeStackProvisioningParametersRequestTypeDef](./type_defs.md#describestackprovisioningparametersrequesttypedef)
- [DescribeStackSummaryRequestTypeDef](./type_defs.md#describestacksummaryrequesttypedef)
- [DescribeStacksRequestTypeDef](./type_defs.md#describestacksrequesttypedef)
- [DescribeTimeBasedAutoScalingRequestTypeDef](./type_defs.md#describetimebasedautoscalingrequesttypedef)
- [DescribeUserProfilesRequestTypeDef](./type_defs.md#describeuserprofilesrequesttypedef)
- [UserProfileTypeDef](./type_defs.md#userprofiletypedef)
- [DescribeVolumesRequestTypeDef](./type_defs.md#describevolumesrequesttypedef)
- [VolumeTypeDef](./type_defs.md#volumetypedef)
- [DetachElasticLoadBalancerRequestTypeDef](./type_defs.md#detachelasticloadbalancerrequesttypedef)
- [DisassociateElasticIpRequestTypeDef](./type_defs.md#disassociateelasticiprequesttypedef)
- [GetHostnameSuggestionRequestTypeDef](./type_defs.md#gethostnamesuggestionrequesttypedef)
- [GrantAccessRequestTypeDef](./type_defs.md#grantaccessrequesttypedef)
- [TemporaryCredentialTypeDef](./type_defs.md#temporarycredentialtypedef)
- [InstanceIdentityTypeDef](./type_defs.md#instanceidentitytypedef)
- [ReportedOsTypeDef](./type_defs.md#reportedostypedef)
- [InstancesCountTypeDef](./type_defs.md#instancescounttypedef)
- [RecipesOutputTypeDef](./type_defs.md#recipesoutputtypedef)
- [ShutdownEventConfigurationTypeDef](./type_defs.md#shutdowneventconfigurationtypedef)
- [ListTagsRequestTypeDef](./type_defs.md#listtagsrequesttypedef)
- [OperatingSystemConfigurationManagerTypeDef](./type_defs.md#operatingsystemconfigurationmanagertypedef)
- [RebootInstanceRequestTypeDef](./type_defs.md#rebootinstancerequesttypedef)
- [RecipesTypeDef](./type_defs.md#recipestypedef)
- [RegisterEcsClusterRequestTypeDef](./type_defs.md#registerecsclusterrequesttypedef)
- [RegisterElasticIpRequestTypeDef](./type_defs.md#registerelasticiprequesttypedef)
- [RegisterRdsDbInstanceRequestTypeDef](./type_defs.md#registerrdsdbinstancerequesttypedef)
- [RegisterVolumeRequestTypeDef](./type_defs.md#registervolumerequesttypedef)
- [SetPermissionRequestTypeDef](./type_defs.md#setpermissionrequesttypedef)
- [StartInstanceRequestTypeDef](./type_defs.md#startinstancerequesttypedef)
- [StartStackRequestTypeDef](./type_defs.md#startstackrequesttypedef)
- [StopInstanceRequestTypeDef](./type_defs.md#stopinstancerequesttypedef)
- [StopStackRequestTypeDef](./type_defs.md#stopstackrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [WeeklyAutoScalingScheduleOutputTypeDef](./type_defs.md#weeklyautoscalingscheduleoutputtypedef)
- [UnassignInstanceRequestTypeDef](./type_defs.md#unassigninstancerequesttypedef)
- [UnassignVolumeRequestTypeDef](./type_defs.md#unassignvolumerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateElasticIpRequestTypeDef](./type_defs.md#updateelasticiprequesttypedef)
- [UpdateInstanceRequestTypeDef](./type_defs.md#updateinstancerequesttypedef)
- [UpdateMyUserProfileRequestTypeDef](./type_defs.md#updatemyuserprofilerequesttypedef)
- [UpdateRdsDbInstanceRequestTypeDef](./type_defs.md#updaterdsdbinstancerequesttypedef)
- [UpdateUserProfileRequestTypeDef](./type_defs.md#updateuserprofilerequesttypedef)
- [UpdateVolumeRequestTypeDef](./type_defs.md#updatevolumerequesttypedef)
- [WeeklyAutoScalingScheduleTypeDef](./type_defs.md#weeklyautoscalingscheduletypedef)
- [AgentVersionTypeDef](./type_defs.md#agentversiontypedef)
- [DescribeAgentVersionsRequestTypeDef](./type_defs.md#describeagentversionsrequesttypedef)
- [AppTypeDef](./type_defs.md#apptypedef)
- [CreateAppRequestTypeDef](./type_defs.md#createapprequesttypedef)
- [UpdateAppRequestTypeDef](./type_defs.md#updateapprequesttypedef)
- [LoadBasedAutoScalingConfigurationTypeDef](./type_defs.md#loadbasedautoscalingconfigurationtypedef)
- [AutoScalingThresholdsUnionTypeDef](./type_defs.md#autoscalingthresholdsuniontypedef)
- [BlockDeviceMappingTypeDef](./type_defs.md#blockdevicemappingtypedef)
- [CloneStackRequestTypeDef](./type_defs.md#clonestackrequesttypedef)
- [CreateStackRequestServiceResourceCreateStackTypeDef](./type_defs.md#createstackrequestserviceresourcecreatestacktypedef)
- [CreateStackRequestTypeDef](./type_defs.md#createstackrequesttypedef)
- [StackTypeDef](./type_defs.md#stacktypedef)
- [UpdateStackRequestTypeDef](./type_defs.md#updatestackrequesttypedef)
- [CloneStackResultTypeDef](./type_defs.md#clonestackresulttypedef)
- [CreateAppResultTypeDef](./type_defs.md#createappresulttypedef)
- [CreateDeploymentResultTypeDef](./type_defs.md#createdeploymentresulttypedef)
- [CreateInstanceResultTypeDef](./type_defs.md#createinstanceresulttypedef)
- [CreateLayerResultTypeDef](./type_defs.md#createlayerresulttypedef)
- [CreateStackResultTypeDef](./type_defs.md#createstackresulttypedef)
- [CreateUserProfileResultTypeDef](./type_defs.md#createuserprofileresulttypedef)
- [DescribeStackProvisioningParametersResultTypeDef](./type_defs.md#describestackprovisioningparametersresulttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetHostnameSuggestionResultTypeDef](./type_defs.md#gethostnamesuggestionresulttypedef)
- [ListTagsResultTypeDef](./type_defs.md#listtagsresulttypedef)
- [RegisterEcsClusterResultTypeDef](./type_defs.md#registerecsclusterresulttypedef)
- [RegisterElasticIpResultTypeDef](./type_defs.md#registerelasticipresulttypedef)
- [RegisterInstanceResultTypeDef](./type_defs.md#registerinstanceresulttypedef)
- [RegisterVolumeResultTypeDef](./type_defs.md#registervolumeresulttypedef)
- [CloudWatchLogsConfigurationOutputTypeDef](./type_defs.md#cloudwatchlogsconfigurationoutputtypedef)
- [CloudWatchLogsConfigurationTypeDef](./type_defs.md#cloudwatchlogsconfigurationtypedef)
- [DescribeCommandsResultTypeDef](./type_defs.md#describecommandsresulttypedef)
- [DeploymentTypeDef](./type_defs.md#deploymenttypedef)
- [DeploymentCommandUnionTypeDef](./type_defs.md#deploymentcommanduniontypedef)
- [DescribeAppsRequestWaitTypeDef](./type_defs.md#describeappsrequestwaittypedef)
- [DescribeDeploymentsRequestWaitTypeDef](./type_defs.md#describedeploymentsrequestwaittypedef)
- [DescribeInstancesRequestWaitExtraExtraExtraTypeDef](./type_defs.md#describeinstancesrequestwaitextraextraextratypedef)
- [DescribeInstancesRequestWaitExtraExtraTypeDef](./type_defs.md#describeinstancesrequestwaitextraextratypedef)
- [DescribeInstancesRequestWaitExtraTypeDef](./type_defs.md#describeinstancesrequestwaitextratypedef)
- [DescribeInstancesRequestWaitTypeDef](./type_defs.md#describeinstancesrequestwaittypedef)
- [DescribeEcsClustersRequestPaginateTypeDef](./type_defs.md#describeecsclustersrequestpaginatetypedef)
- [DescribeEcsClustersResultTypeDef](./type_defs.md#describeecsclustersresulttypedef)
- [DescribeElasticIpsResultTypeDef](./type_defs.md#describeelasticipsresulttypedef)
- [DescribeElasticLoadBalancersResultTypeDef](./type_defs.md#describeelasticloadbalancersresulttypedef)
- [DescribeMyUserProfileResultTypeDef](./type_defs.md#describemyuserprofileresulttypedef)
- [DescribePermissionsResultTypeDef](./type_defs.md#describepermissionsresulttypedef)
- [DescribeRaidArraysResultTypeDef](./type_defs.md#describeraidarraysresulttypedef)
- [DescribeRdsDbInstancesResultTypeDef](./type_defs.md#describerdsdbinstancesresulttypedef)
- [DescribeServiceErrorsResultTypeDef](./type_defs.md#describeserviceerrorsresulttypedef)
- [DescribeUserProfilesResultTypeDef](./type_defs.md#describeuserprofilesresulttypedef)
- [DescribeVolumesResultTypeDef](./type_defs.md#describevolumesresulttypedef)
- [GrantAccessResultTypeDef](./type_defs.md#grantaccessresulttypedef)
- [RegisterInstanceRequestTypeDef](./type_defs.md#registerinstancerequesttypedef)
- [StackSummaryTypeDef](./type_defs.md#stacksummarytypedef)
- [LifecycleEventConfigurationTypeDef](./type_defs.md#lifecycleeventconfigurationtypedef)
- [OperatingSystemTypeDef](./type_defs.md#operatingsystemtypedef)
- [RecipesUnionTypeDef](./type_defs.md#recipesuniontypedef)
- [TimeBasedAutoScalingConfigurationTypeDef](./type_defs.md#timebasedautoscalingconfigurationtypedef)
- [WeeklyAutoScalingScheduleUnionTypeDef](./type_defs.md#weeklyautoscalingscheduleuniontypedef)
- [DescribeAgentVersionsResultTypeDef](./type_defs.md#describeagentversionsresulttypedef)
- [DescribeAppsResultTypeDef](./type_defs.md#describeappsresulttypedef)
- [DescribeLoadBasedAutoScalingResultTypeDef](./type_defs.md#describeloadbasedautoscalingresulttypedef)
- [SetLoadBasedAutoScalingRequestTypeDef](./type_defs.md#setloadbasedautoscalingrequesttypedef)
- [CreateInstanceRequestTypeDef](./type_defs.md#createinstancerequesttypedef)
- [InstanceTypeDef](./type_defs.md#instancetypedef)
- [DescribeStacksResultTypeDef](./type_defs.md#describestacksresulttypedef)
- [CloudWatchLogsConfigurationUnionTypeDef](./type_defs.md#cloudwatchlogsconfigurationuniontypedef)
- [DescribeDeploymentsResultTypeDef](./type_defs.md#describedeploymentsresulttypedef)
- [CreateDeploymentRequestTypeDef](./type_defs.md#createdeploymentrequesttypedef)
- [DescribeStackSummaryResultTypeDef](./type_defs.md#describestacksummaryresulttypedef)
- [LayerTypeDef](./type_defs.md#layertypedef)
- [DescribeOperatingSystemsResponseTypeDef](./type_defs.md#describeoperatingsystemsresponsetypedef)
- [DescribeTimeBasedAutoScalingResultTypeDef](./type_defs.md#describetimebasedautoscalingresulttypedef)
- [SetTimeBasedAutoScalingRequestTypeDef](./type_defs.md#settimebasedautoscalingrequesttypedef)
- [DescribeInstancesResultTypeDef](./type_defs.md#describeinstancesresulttypedef)
- [CreateLayerRequestStackCreateLayerTypeDef](./type_defs.md#createlayerrequeststackcreatelayertypedef)
- [CreateLayerRequestTypeDef](./type_defs.md#createlayerrequesttypedef)
- [UpdateLayerRequestTypeDef](./type_defs.md#updatelayerrequesttypedef)
- [DescribeLayersResultTypeDef](./type_defs.md#describelayersresulttypedef)

