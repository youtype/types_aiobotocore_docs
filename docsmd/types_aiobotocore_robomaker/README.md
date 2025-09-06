# RoboMaker module

> [Index](../README.md) > RoboMaker


!!! note ""

    Auto-generated documentation for [RoboMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#robomaker)
    type annotations stubs module [types-aiobotocore-robomaker](https://pypi.org/project/types-aiobotocore-robomaker/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `RoboMaker` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `RoboMaker` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[robomaker]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[robomaker]'

# standalone installation
python -m pip install types-aiobotocore-robomaker
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-robomaker
```

## Usage

Code samples can be found in [Examples](./usage.md).

## RoboMakerClient

Type annotations and code completion for  `#!python session.create_client("robomaker")` as [RoboMakerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker.Client)

```python
# RoboMakerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_robomaker.client import RoboMakerClient


session = get_session()
async with session.create_client("robomaker") as client:
    client: RoboMakerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("robomaker").get_paginator("...")`.

```python
# ListDeploymentJobsPaginator usage example

from types_aiobotocore_robomaker.paginator import ListDeploymentJobsPaginator

def get_list_deployment_jobs_paginator() -> ListDeploymentJobsPaginator:
    return client.get_paginator("list_deployment_jobs"))
```

- [ListDeploymentJobsPaginator](./paginators.md#listdeploymentjobspaginator)
- [ListFleetsPaginator](./paginators.md#listfleetspaginator)
- [ListRobotApplicationsPaginator](./paginators.md#listrobotapplicationspaginator)
- [ListRobotsPaginator](./paginators.md#listrobotspaginator)
- [ListSimulationApplicationsPaginator](./paginators.md#listsimulationapplicationspaginator)
- [ListSimulationJobBatchesPaginator](./paginators.md#listsimulationjobbatchespaginator)
- [ListSimulationJobsPaginator](./paginators.md#listsimulationjobspaginator)
- [ListWorldExportJobsPaginator](./paginators.md#listworldexportjobspaginator)
- [ListWorldGenerationJobsPaginator](./paginators.md#listworldgenerationjobspaginator)
- [ListWorldTemplatesPaginator](./paginators.md#listworldtemplatespaginator)
- [ListWorldsPaginator](./paginators.md#listworldspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ArchitectureType usage example

from types_aiobotocore_robomaker.literals import ArchitectureType

def get_value() -> ArchitectureType:
    return "ARM64"
```

- [ArchitectureType](./literals.md#architecturetype)
- [ComputeTypeType](./literals.md#computetypetype)
- [DataSourceTypeType](./literals.md#datasourcetypetype)
- [DeploymentJobErrorCodeType](./literals.md#deploymentjoberrorcodetype)
- [DeploymentStatusType](./literals.md#deploymentstatustype)
- [ExitBehaviorType](./literals.md#exitbehaviortype)
- [FailureBehaviorType](./literals.md#failurebehaviortype)
- [ListDeploymentJobsPaginatorName](./literals.md#listdeploymentjobspaginatorname)
- [ListFleetsPaginatorName](./literals.md#listfleetspaginatorname)
- [ListRobotApplicationsPaginatorName](./literals.md#listrobotapplicationspaginatorname)
- [ListRobotsPaginatorName](./literals.md#listrobotspaginatorname)
- [ListSimulationApplicationsPaginatorName](./literals.md#listsimulationapplicationspaginatorname)
- [ListSimulationJobBatchesPaginatorName](./literals.md#listsimulationjobbatchespaginatorname)
- [ListSimulationJobsPaginatorName](./literals.md#listsimulationjobspaginatorname)
- [ListWorldExportJobsPaginatorName](./literals.md#listworldexportjobspaginatorname)
- [ListWorldGenerationJobsPaginatorName](./literals.md#listworldgenerationjobspaginatorname)
- [ListWorldTemplatesPaginatorName](./literals.md#listworldtemplatespaginatorname)
- [ListWorldsPaginatorName](./literals.md#listworldspaginatorname)
- [RenderingEngineTypeType](./literals.md#renderingenginetypetype)
- [RobotDeploymentStepType](./literals.md#robotdeploymentsteptype)
- [RobotSoftwareSuiteTypeType](./literals.md#robotsoftwaresuitetypetype)
- [RobotSoftwareSuiteVersionTypeType](./literals.md#robotsoftwaresuiteversiontypetype)
- [RobotStatusType](./literals.md#robotstatustype)
- [SimulationJobBatchErrorCodeType](./literals.md#simulationjobbatcherrorcodetype)
- [SimulationJobBatchStatusType](./literals.md#simulationjobbatchstatustype)
- [SimulationJobErrorCodeType](./literals.md#simulationjoberrorcodetype)
- [SimulationJobStatusType](./literals.md#simulationjobstatustype)
- [SimulationSoftwareSuiteTypeType](./literals.md#simulationsoftwaresuitetypetype)
- [UploadBehaviorType](./literals.md#uploadbehaviortype)
- [WorldExportJobErrorCodeType](./literals.md#worldexportjoberrorcodetype)
- [WorldExportJobStatusType](./literals.md#worldexportjobstatustype)
- [WorldGenerationJobErrorCodeType](./literals.md#worldgenerationjoberrorcodetype)
- [WorldGenerationJobStatusType](./literals.md#worldgenerationjobstatustype)
- [RoboMakerServiceName](./literals.md#robomakerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BatchDeleteWorldsRequestTypeDef](./type_defs.md#batchdeleteworldsrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchDescribeSimulationJobRequestTypeDef](./type_defs.md#batchdescribesimulationjobrequesttypedef)
- [BatchPolicyTypeDef](./type_defs.md#batchpolicytypedef)
- [CancelDeploymentJobRequestTypeDef](./type_defs.md#canceldeploymentjobrequesttypedef)
- [CancelSimulationJobBatchRequestTypeDef](./type_defs.md#cancelsimulationjobbatchrequesttypedef)
- [CancelSimulationJobRequestTypeDef](./type_defs.md#cancelsimulationjobrequesttypedef)
- [CancelWorldExportJobRequestTypeDef](./type_defs.md#cancelworldexportjobrequesttypedef)
- [CancelWorldGenerationJobRequestTypeDef](./type_defs.md#cancelworldgenerationjobrequesttypedef)
- [ComputeResponseTypeDef](./type_defs.md#computeresponsetypedef)
- [ComputeTypeDef](./type_defs.md#computetypedef)
- [CreateFleetRequestTypeDef](./type_defs.md#createfleetrequesttypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef)
- [SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef)
- [SourceTypeDef](./type_defs.md#sourcetypedef)
- [CreateRobotApplicationVersionRequestTypeDef](./type_defs.md#createrobotapplicationversionrequesttypedef)
- [CreateRobotRequestTypeDef](./type_defs.md#createrobotrequesttypedef)
- [RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef)
- [SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef)
- [CreateSimulationApplicationVersionRequestTypeDef](./type_defs.md#createsimulationapplicationversionrequesttypedef)
- [LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef)
- [OutputLocationTypeDef](./type_defs.md#outputlocationtypedef)
- [VPCConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef)
- [WorldCountTypeDef](./type_defs.md#worldcounttypedef)
- [TemplateLocationTypeDef](./type_defs.md#templatelocationtypedef)
- [DataSourceConfigOutputTypeDef](./type_defs.md#datasourceconfigoutputtypedef)
- [DataSourceConfigTypeDef](./type_defs.md#datasourceconfigtypedef)
- [S3KeyOutputTypeDef](./type_defs.md#s3keyoutputtypedef)
- [DeleteFleetRequestTypeDef](./type_defs.md#deletefleetrequesttypedef)
- [DeleteRobotApplicationRequestTypeDef](./type_defs.md#deleterobotapplicationrequesttypedef)
- [DeleteRobotRequestTypeDef](./type_defs.md#deleterobotrequesttypedef)
- [DeleteSimulationApplicationRequestTypeDef](./type_defs.md#deletesimulationapplicationrequesttypedef)
- [DeleteWorldTemplateRequestTypeDef](./type_defs.md#deleteworldtemplaterequesttypedef)
- [DeploymentLaunchConfigOutputTypeDef](./type_defs.md#deploymentlaunchconfigoutputtypedef)
- [S3ObjectTypeDef](./type_defs.md#s3objecttypedef)
- [DeploymentLaunchConfigTypeDef](./type_defs.md#deploymentlaunchconfigtypedef)
- [DeregisterRobotRequestTypeDef](./type_defs.md#deregisterrobotrequesttypedef)
- [DescribeDeploymentJobRequestTypeDef](./type_defs.md#describedeploymentjobrequesttypedef)
- [DescribeFleetRequestTypeDef](./type_defs.md#describefleetrequesttypedef)
- [RobotTypeDef](./type_defs.md#robottypedef)
- [DescribeRobotApplicationRequestTypeDef](./type_defs.md#describerobotapplicationrequesttypedef)
- [DescribeRobotRequestTypeDef](./type_defs.md#describerobotrequesttypedef)
- [DescribeSimulationApplicationRequestTypeDef](./type_defs.md#describesimulationapplicationrequesttypedef)
- [DescribeSimulationJobBatchRequestTypeDef](./type_defs.md#describesimulationjobbatchrequesttypedef)
- [SimulationJobSummaryTypeDef](./type_defs.md#simulationjobsummarytypedef)
- [DescribeSimulationJobRequestTypeDef](./type_defs.md#describesimulationjobrequesttypedef)
- [NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef)
- [DescribeWorldExportJobRequestTypeDef](./type_defs.md#describeworldexportjobrequesttypedef)
- [DescribeWorldGenerationJobRequestTypeDef](./type_defs.md#describeworldgenerationjobrequesttypedef)
- [DescribeWorldRequestTypeDef](./type_defs.md#describeworldrequesttypedef)
- [DescribeWorldTemplateRequestTypeDef](./type_defs.md#describeworldtemplaterequesttypedef)
- [WorldFailureTypeDef](./type_defs.md#worldfailuretypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [FleetTypeDef](./type_defs.md#fleettypedef)
- [GetWorldTemplateBodyRequestTypeDef](./type_defs.md#getworldtemplatebodyrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [SimulationJobBatchSummaryTypeDef](./type_defs.md#simulationjobbatchsummarytypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListWorldTemplatesRequestTypeDef](./type_defs.md#listworldtemplatesrequesttypedef)
- [TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef)
- [WorldSummaryTypeDef](./type_defs.md#worldsummarytypedef)
- [PortMappingTypeDef](./type_defs.md#portmappingtypedef)
- [ProgressDetailTypeDef](./type_defs.md#progressdetailtypedef)
- [RegisterRobotRequestTypeDef](./type_defs.md#registerrobotrequesttypedef)
- [RestartSimulationJobRequestTypeDef](./type_defs.md#restartsimulationjobrequesttypedef)
- [ToolTypeDef](./type_defs.md#tooltypedef)
- [UploadConfigurationTypeDef](./type_defs.md#uploadconfigurationtypedef)
- [WorldConfigTypeDef](./type_defs.md#worldconfigtypedef)
- [VPCConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef)
- [SyncDeploymentJobRequestTypeDef](./type_defs.md#syncdeploymentjobrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [VPCConfigTypeDef](./type_defs.md#vpcconfigtypedef)
- [BatchDeleteWorldsResponseTypeDef](./type_defs.md#batchdeleteworldsresponsetypedef)
- [CreateFleetResponseTypeDef](./type_defs.md#createfleetresponsetypedef)
- [CreateRobotResponseTypeDef](./type_defs.md#createrobotresponsetypedef)
- [CreateWorldTemplateResponseTypeDef](./type_defs.md#createworldtemplateresponsetypedef)
- [DeregisterRobotResponseTypeDef](./type_defs.md#deregisterrobotresponsetypedef)
- [DescribeRobotResponseTypeDef](./type_defs.md#describerobotresponsetypedef)
- [DescribeWorldResponseTypeDef](./type_defs.md#describeworldresponsetypedef)
- [DescribeWorldTemplateResponseTypeDef](./type_defs.md#describeworldtemplateresponsetypedef)
- [GetWorldTemplateBodyResponseTypeDef](./type_defs.md#getworldtemplatebodyresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [RegisterRobotResponseTypeDef](./type_defs.md#registerrobotresponsetypedef)
- [UpdateWorldTemplateResponseTypeDef](./type_defs.md#updateworldtemplateresponsetypedef)
- [RobotApplicationSummaryTypeDef](./type_defs.md#robotapplicationsummarytypedef)
- [CreateRobotApplicationRequestTypeDef](./type_defs.md#createrobotapplicationrequesttypedef)
- [UpdateRobotApplicationRequestTypeDef](./type_defs.md#updaterobotapplicationrequesttypedef)
- [CreateRobotApplicationResponseTypeDef](./type_defs.md#createrobotapplicationresponsetypedef)
- [CreateRobotApplicationVersionResponseTypeDef](./type_defs.md#createrobotapplicationversionresponsetypedef)
- [DescribeRobotApplicationResponseTypeDef](./type_defs.md#describerobotapplicationresponsetypedef)
- [UpdateRobotApplicationResponseTypeDef](./type_defs.md#updaterobotapplicationresponsetypedef)
- [CreateSimulationApplicationRequestTypeDef](./type_defs.md#createsimulationapplicationrequesttypedef)
- [CreateSimulationApplicationResponseTypeDef](./type_defs.md#createsimulationapplicationresponsetypedef)
- [CreateSimulationApplicationVersionResponseTypeDef](./type_defs.md#createsimulationapplicationversionresponsetypedef)
- [DescribeSimulationApplicationResponseTypeDef](./type_defs.md#describesimulationapplicationresponsetypedef)
- [SimulationApplicationSummaryTypeDef](./type_defs.md#simulationapplicationsummarytypedef)
- [UpdateSimulationApplicationRequestTypeDef](./type_defs.md#updatesimulationapplicationrequesttypedef)
- [UpdateSimulationApplicationResponseTypeDef](./type_defs.md#updatesimulationapplicationresponsetypedef)
- [CreateWorldExportJobRequestTypeDef](./type_defs.md#createworldexportjobrequesttypedef)
- [CreateWorldExportJobResponseTypeDef](./type_defs.md#createworldexportjobresponsetypedef)
- [DescribeWorldExportJobResponseTypeDef](./type_defs.md#describeworldexportjobresponsetypedef)
- [WorldExportJobSummaryTypeDef](./type_defs.md#worldexportjobsummarytypedef)
- [CreateWorldGenerationJobRequestTypeDef](./type_defs.md#createworldgenerationjobrequesttypedef)
- [CreateWorldGenerationJobResponseTypeDef](./type_defs.md#createworldgenerationjobresponsetypedef)
- [WorldGenerationJobSummaryTypeDef](./type_defs.md#worldgenerationjobsummarytypedef)
- [CreateWorldTemplateRequestTypeDef](./type_defs.md#createworldtemplaterequesttypedef)
- [UpdateWorldTemplateRequestTypeDef](./type_defs.md#updateworldtemplaterequesttypedef)
- [DataSourceConfigUnionTypeDef](./type_defs.md#datasourceconfiguniontypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [DeploymentApplicationConfigOutputTypeDef](./type_defs.md#deploymentapplicationconfigoutputtypedef)
- [DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef)
- [DeploymentLaunchConfigUnionTypeDef](./type_defs.md#deploymentlaunchconfiguniontypedef)
- [DescribeFleetResponseTypeDef](./type_defs.md#describefleetresponsetypedef)
- [ListRobotsResponseTypeDef](./type_defs.md#listrobotsresponsetypedef)
- [ListSimulationJobsResponseTypeDef](./type_defs.md#listsimulationjobsresponsetypedef)
- [FailureSummaryTypeDef](./type_defs.md#failuresummarytypedef)
- [ListDeploymentJobsRequestTypeDef](./type_defs.md#listdeploymentjobsrequesttypedef)
- [ListFleetsRequestTypeDef](./type_defs.md#listfleetsrequesttypedef)
- [ListRobotApplicationsRequestTypeDef](./type_defs.md#listrobotapplicationsrequesttypedef)
- [ListRobotsRequestTypeDef](./type_defs.md#listrobotsrequesttypedef)
- [ListSimulationApplicationsRequestTypeDef](./type_defs.md#listsimulationapplicationsrequesttypedef)
- [ListSimulationJobBatchesRequestTypeDef](./type_defs.md#listsimulationjobbatchesrequesttypedef)
- [ListSimulationJobsRequestTypeDef](./type_defs.md#listsimulationjobsrequesttypedef)
- [ListWorldExportJobsRequestTypeDef](./type_defs.md#listworldexportjobsrequesttypedef)
- [ListWorldGenerationJobsRequestTypeDef](./type_defs.md#listworldgenerationjobsrequesttypedef)
- [ListWorldsRequestTypeDef](./type_defs.md#listworldsrequesttypedef)
- [ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef)
- [ListDeploymentJobsRequestPaginateTypeDef](./type_defs.md#listdeploymentjobsrequestpaginatetypedef)
- [ListFleetsRequestPaginateTypeDef](./type_defs.md#listfleetsrequestpaginatetypedef)
- [ListRobotApplicationsRequestPaginateTypeDef](./type_defs.md#listrobotapplicationsrequestpaginatetypedef)
- [ListRobotsRequestPaginateTypeDef](./type_defs.md#listrobotsrequestpaginatetypedef)
- [ListSimulationApplicationsRequestPaginateTypeDef](./type_defs.md#listsimulationapplicationsrequestpaginatetypedef)
- [ListSimulationJobBatchesRequestPaginateTypeDef](./type_defs.md#listsimulationjobbatchesrequestpaginatetypedef)
- [ListSimulationJobsRequestPaginateTypeDef](./type_defs.md#listsimulationjobsrequestpaginatetypedef)
- [ListWorldExportJobsRequestPaginateTypeDef](./type_defs.md#listworldexportjobsrequestpaginatetypedef)
- [ListWorldGenerationJobsRequestPaginateTypeDef](./type_defs.md#listworldgenerationjobsrequestpaginatetypedef)
- [ListWorldTemplatesRequestPaginateTypeDef](./type_defs.md#listworldtemplatesrequestpaginatetypedef)
- [ListWorldsRequestPaginateTypeDef](./type_defs.md#listworldsrequestpaginatetypedef)
- [ListSimulationJobBatchesResponseTypeDef](./type_defs.md#listsimulationjobbatchesresponsetypedef)
- [ListWorldTemplatesResponseTypeDef](./type_defs.md#listworldtemplatesresponsetypedef)
- [ListWorldsResponseTypeDef](./type_defs.md#listworldsresponsetypedef)
- [PortForwardingConfigOutputTypeDef](./type_defs.md#portforwardingconfigoutputtypedef)
- [PortForwardingConfigTypeDef](./type_defs.md#portforwardingconfigtypedef)
- [RobotDeploymentTypeDef](./type_defs.md#robotdeploymenttypedef)
- [VPCConfigUnionTypeDef](./type_defs.md#vpcconfiguniontypedef)
- [ListRobotApplicationsResponseTypeDef](./type_defs.md#listrobotapplicationsresponsetypedef)
- [ListSimulationApplicationsResponseTypeDef](./type_defs.md#listsimulationapplicationsresponsetypedef)
- [ListWorldExportJobsResponseTypeDef](./type_defs.md#listworldexportjobsresponsetypedef)
- [ListWorldGenerationJobsResponseTypeDef](./type_defs.md#listworldgenerationjobsresponsetypedef)
- [CreateDeploymentJobResponseTypeDef](./type_defs.md#createdeploymentjobresponsetypedef)
- [DeploymentJobTypeDef](./type_defs.md#deploymentjobtypedef)
- [SyncDeploymentJobResponseTypeDef](./type_defs.md#syncdeploymentjobresponsetypedef)
- [DeploymentApplicationConfigTypeDef](./type_defs.md#deploymentapplicationconfigtypedef)
- [FinishedWorldsSummaryTypeDef](./type_defs.md#finishedworldssummarytypedef)
- [LaunchConfigOutputTypeDef](./type_defs.md#launchconfigoutputtypedef)
- [PortForwardingConfigUnionTypeDef](./type_defs.md#portforwardingconfiguniontypedef)
- [DescribeDeploymentJobResponseTypeDef](./type_defs.md#describedeploymentjobresponsetypedef)
- [ListDeploymentJobsResponseTypeDef](./type_defs.md#listdeploymentjobsresponsetypedef)
- [DeploymentApplicationConfigUnionTypeDef](./type_defs.md#deploymentapplicationconfiguniontypedef)
- [DescribeWorldGenerationJobResponseTypeDef](./type_defs.md#describeworldgenerationjobresponsetypedef)
- [RobotApplicationConfigOutputTypeDef](./type_defs.md#robotapplicationconfigoutputtypedef)
- [SimulationApplicationConfigOutputTypeDef](./type_defs.md#simulationapplicationconfigoutputtypedef)
- [LaunchConfigTypeDef](./type_defs.md#launchconfigtypedef)
- [CreateDeploymentJobRequestTypeDef](./type_defs.md#createdeploymentjobrequesttypedef)
- [CreateSimulationJobResponseTypeDef](./type_defs.md#createsimulationjobresponsetypedef)
- [DescribeSimulationJobResponseTypeDef](./type_defs.md#describesimulationjobresponsetypedef)
- [SimulationJobRequestOutputTypeDef](./type_defs.md#simulationjobrequestoutputtypedef)
- [SimulationJobTypeDef](./type_defs.md#simulationjobtypedef)
- [LaunchConfigUnionTypeDef](./type_defs.md#launchconfiguniontypedef)
- [FailedCreateSimulationJobRequestTypeDef](./type_defs.md#failedcreatesimulationjobrequesttypedef)
- [BatchDescribeSimulationJobResponseTypeDef](./type_defs.md#batchdescribesimulationjobresponsetypedef)
- [RobotApplicationConfigTypeDef](./type_defs.md#robotapplicationconfigtypedef)
- [SimulationApplicationConfigTypeDef](./type_defs.md#simulationapplicationconfigtypedef)
- [DescribeSimulationJobBatchResponseTypeDef](./type_defs.md#describesimulationjobbatchresponsetypedef)
- [StartSimulationJobBatchResponseTypeDef](./type_defs.md#startsimulationjobbatchresponsetypedef)
- [RobotApplicationConfigUnionTypeDef](./type_defs.md#robotapplicationconfiguniontypedef)
- [SimulationApplicationConfigUnionTypeDef](./type_defs.md#simulationapplicationconfiguniontypedef)
- [CreateSimulationJobRequestTypeDef](./type_defs.md#createsimulationjobrequesttypedef)
- [SimulationJobRequestTypeDef](./type_defs.md#simulationjobrequesttypedef)
- [SimulationJobRequestUnionTypeDef](./type_defs.md#simulationjobrequestuniontypedef)
- [StartSimulationJobBatchRequestTypeDef](./type_defs.md#startsimulationjobbatchrequesttypedef)

