# Type definitions

> [Index](../README.md) > [RoboMaker](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RoboMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/robomaker.html#RoboMaker)
    type annotations stubs module [types-aiobotocore-robomaker](https://pypi.org/project/types-aiobotocore-robomaker/).

## DataSourceConfigUnionTypeDef

```python
# DataSourceConfigUnionTypeDef definition

DataSourceConfigUnionTypeDef = Union[
    DataSourceConfigTypeDef,  # (1)
    DataSourceConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataSourceConfigTypeDef](./type_defs.md#datasourceconfigtypedef) 
2. See [:material-code-braces: DataSourceConfigOutputTypeDef](./type_defs.md#datasourceconfigoutputtypedef) 

## DeploymentLaunchConfigUnionTypeDef

```python
# DeploymentLaunchConfigUnionTypeDef definition

DeploymentLaunchConfigUnionTypeDef = Union[
    DeploymentLaunchConfigTypeDef,  # (1)
    DeploymentLaunchConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeploymentLaunchConfigTypeDef](./type_defs.md#deploymentlaunchconfigtypedef) 
2. See [:material-code-braces: DeploymentLaunchConfigOutputTypeDef](./type_defs.md#deploymentlaunchconfigoutputtypedef) 

## VPCConfigUnionTypeDef

```python
# VPCConfigUnionTypeDef definition

VPCConfigUnionTypeDef = Union[
    VPCConfigTypeDef,  # (1)
    VPCConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VPCConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
2. See [:material-code-braces: VPCConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 

## PortForwardingConfigUnionTypeDef

```python
# PortForwardingConfigUnionTypeDef definition

PortForwardingConfigUnionTypeDef = Union[
    PortForwardingConfigTypeDef,  # (1)
    PortForwardingConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PortForwardingConfigTypeDef](./type_defs.md#portforwardingconfigtypedef) 
2. See [:material-code-braces: PortForwardingConfigOutputTypeDef](./type_defs.md#portforwardingconfigoutputtypedef) 

## DeploymentApplicationConfigUnionTypeDef

```python
# DeploymentApplicationConfigUnionTypeDef definition

DeploymentApplicationConfigUnionTypeDef = Union[
    DeploymentApplicationConfigTypeDef,  # (1)
    DeploymentApplicationConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeploymentApplicationConfigTypeDef](./type_defs.md#deploymentapplicationconfigtypedef) 
2. See [:material-code-braces: DeploymentApplicationConfigOutputTypeDef](./type_defs.md#deploymentapplicationconfigoutputtypedef) 

## LaunchConfigUnionTypeDef

```python
# LaunchConfigUnionTypeDef definition

LaunchConfigUnionTypeDef = Union[
    LaunchConfigTypeDef,  # (1)
    LaunchConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LaunchConfigTypeDef](./type_defs.md#launchconfigtypedef) 
2. See [:material-code-braces: LaunchConfigOutputTypeDef](./type_defs.md#launchconfigoutputtypedef) 

## RobotApplicationConfigUnionTypeDef

```python
# RobotApplicationConfigUnionTypeDef definition

RobotApplicationConfigUnionTypeDef = Union[
    RobotApplicationConfigTypeDef,  # (1)
    RobotApplicationConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RobotApplicationConfigTypeDef](./type_defs.md#robotapplicationconfigtypedef) 
2. See [:material-code-braces: RobotApplicationConfigOutputTypeDef](./type_defs.md#robotapplicationconfigoutputtypedef) 

## SimulationApplicationConfigUnionTypeDef

```python
# SimulationApplicationConfigUnionTypeDef definition

SimulationApplicationConfigUnionTypeDef = Union[
    SimulationApplicationConfigTypeDef,  # (1)
    SimulationApplicationConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SimulationApplicationConfigTypeDef](./type_defs.md#simulationapplicationconfigtypedef) 
2. See [:material-code-braces: SimulationApplicationConfigOutputTypeDef](./type_defs.md#simulationapplicationconfigoutputtypedef) 

## SimulationJobRequestUnionTypeDef

```python
# SimulationJobRequestUnionTypeDef definition

SimulationJobRequestUnionTypeDef = Union[
    SimulationJobRequestTypeDef,  # (1)
    SimulationJobRequestOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SimulationJobRequestTypeDef](./type_defs.md#simulationjobrequesttypedef) 
2. See [:material-code-braces: SimulationJobRequestOutputTypeDef](./type_defs.md#simulationjobrequestoutputtypedef) 



## BatchDeleteWorldsRequestRequestTypeDef

```python
# BatchDeleteWorldsRequestRequestTypeDef definition

class BatchDeleteWorldsRequestRequestTypeDef(TypedDict):
    worlds: Sequence[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## BatchDescribeSimulationJobRequestRequestTypeDef

```python
# BatchDescribeSimulationJobRequestRequestTypeDef definition

class BatchDescribeSimulationJobRequestRequestTypeDef(TypedDict):
    jobs: Sequence[str],
```

## BatchPolicyTypeDef

```python
# BatchPolicyTypeDef definition

class BatchPolicyTypeDef(TypedDict):
    timeoutInSeconds: NotRequired[int],
    maxConcurrency: NotRequired[int],
```

## CancelDeploymentJobRequestRequestTypeDef

```python
# CancelDeploymentJobRequestRequestTypeDef definition

class CancelDeploymentJobRequestRequestTypeDef(TypedDict):
    job: str,
```

## CancelSimulationJobBatchRequestRequestTypeDef

```python
# CancelSimulationJobBatchRequestRequestTypeDef definition

class CancelSimulationJobBatchRequestRequestTypeDef(TypedDict):
    batch: str,
```

## CancelSimulationJobRequestRequestTypeDef

```python
# CancelSimulationJobRequestRequestTypeDef definition

class CancelSimulationJobRequestRequestTypeDef(TypedDict):
    job: str,
```

## CancelWorldExportJobRequestRequestTypeDef

```python
# CancelWorldExportJobRequestRequestTypeDef definition

class CancelWorldExportJobRequestRequestTypeDef(TypedDict):
    job: str,
```

## CancelWorldGenerationJobRequestRequestTypeDef

```python
# CancelWorldGenerationJobRequestRequestTypeDef definition

class CancelWorldGenerationJobRequestRequestTypeDef(TypedDict):
    job: str,
```

## ComputeResponseTypeDef

```python
# ComputeResponseTypeDef definition

class ComputeResponseTypeDef(TypedDict):
    simulationUnitLimit: NotRequired[int],
    computeType: NotRequired[ComputeTypeType],  # (1)
    gpuUnitLimit: NotRequired[int],
```

1. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
## ComputeTypeDef

```python
# ComputeTypeDef definition

class ComputeTypeDef(TypedDict):
    simulationUnitLimit: NotRequired[int],
    computeType: NotRequired[ComputeTypeType],  # (1)
    gpuUnitLimit: NotRequired[int],
```

1. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
## CreateFleetRequestRequestTypeDef

```python
# CreateFleetRequestRequestTypeDef definition

class CreateFleetRequestRequestTypeDef(TypedDict):
    name: str,
    tags: NotRequired[Mapping[str, str]],
```

## EnvironmentTypeDef

```python
# EnvironmentTypeDef definition

class EnvironmentTypeDef(TypedDict):
    uri: NotRequired[str],
```

## RobotSoftwareSuiteTypeDef

```python
# RobotSoftwareSuiteTypeDef definition

class RobotSoftwareSuiteTypeDef(TypedDict):
    name: NotRequired[RobotSoftwareSuiteTypeType],  # (1)
    version: NotRequired[RobotSoftwareSuiteVersionTypeType],  # (2)
```

1. See [:material-code-brackets: RobotSoftwareSuiteTypeType](./literals.md#robotsoftwaresuitetypetype) 
2. See [:material-code-brackets: RobotSoftwareSuiteVersionTypeType](./literals.md#robotsoftwaresuiteversiontypetype) 
## SourceConfigTypeDef

```python
# SourceConfigTypeDef definition

class SourceConfigTypeDef(TypedDict):
    s3Bucket: NotRequired[str],
    s3Key: NotRequired[str],
    architecture: NotRequired[ArchitectureType],  # (1)
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## SourceTypeDef

```python
# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    s3Bucket: NotRequired[str],
    s3Key: NotRequired[str],
    etag: NotRequired[str],
    architecture: NotRequired[ArchitectureType],  # (1)
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## CreateRobotApplicationVersionRequestRequestTypeDef

```python
# CreateRobotApplicationVersionRequestRequestTypeDef definition

class CreateRobotApplicationVersionRequestRequestTypeDef(TypedDict):
    application: str,
    currentRevisionId: NotRequired[str],
    s3Etags: NotRequired[Sequence[str]],
    imageDigest: NotRequired[str],
```

## CreateRobotRequestRequestTypeDef

```python
# CreateRobotRequestRequestTypeDef definition

class CreateRobotRequestRequestTypeDef(TypedDict):
    name: str,
    architecture: ArchitectureType,  # (1)
    greengrassGroupId: str,
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## RenderingEngineTypeDef

```python
# RenderingEngineTypeDef definition

class RenderingEngineTypeDef(TypedDict):
    name: NotRequired[RenderingEngineTypeType],  # (1)
    version: NotRequired[str],
```

1. See [:material-code-brackets: RenderingEngineTypeType](./literals.md#renderingenginetypetype) 
## SimulationSoftwareSuiteTypeDef

```python
# SimulationSoftwareSuiteTypeDef definition

class SimulationSoftwareSuiteTypeDef(TypedDict):
    name: NotRequired[SimulationSoftwareSuiteTypeType],  # (1)
    version: NotRequired[str],
```

1. See [:material-code-brackets: SimulationSoftwareSuiteTypeType](./literals.md#simulationsoftwaresuitetypetype) 
## CreateSimulationApplicationVersionRequestRequestTypeDef

```python
# CreateSimulationApplicationVersionRequestRequestTypeDef definition

class CreateSimulationApplicationVersionRequestRequestTypeDef(TypedDict):
    application: str,
    currentRevisionId: NotRequired[str],
    s3Etags: NotRequired[Sequence[str]],
    imageDigest: NotRequired[str],
```

## LoggingConfigTypeDef

```python
# LoggingConfigTypeDef definition

class LoggingConfigTypeDef(TypedDict):
    recordAllRosTopics: NotRequired[bool],
```

## OutputLocationTypeDef

```python
# OutputLocationTypeDef definition

class OutputLocationTypeDef(TypedDict):
    s3Bucket: NotRequired[str],
    s3Prefix: NotRequired[str],
```

## VPCConfigTypeDef

```python
# VPCConfigTypeDef definition

class VPCConfigTypeDef(TypedDict):
    subnets: Sequence[str],
    securityGroups: NotRequired[Sequence[str]],
    assignPublicIp: NotRequired[bool],
```

## VPCConfigResponseTypeDef

```python
# VPCConfigResponseTypeDef definition

class VPCConfigResponseTypeDef(TypedDict):
    subnets: NotRequired[List[str]],
    securityGroups: NotRequired[List[str]],
    vpcId: NotRequired[str],
    assignPublicIp: NotRequired[bool],
```

## WorldCountTypeDef

```python
# WorldCountTypeDef definition

class WorldCountTypeDef(TypedDict):
    floorplanCount: NotRequired[int],
    interiorCountPerFloorplan: NotRequired[int],
```

## TemplateLocationTypeDef

```python
# TemplateLocationTypeDef definition

class TemplateLocationTypeDef(TypedDict):
    s3Bucket: str,
    s3Key: str,
```

## DataSourceConfigOutputTypeDef

```python
# DataSourceConfigOutputTypeDef definition

class DataSourceConfigOutputTypeDef(TypedDict):
    name: str,
    s3Bucket: str,
    s3Keys: List[str],
    type: NotRequired[DataSourceTypeType],  # (1)
    destination: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
## DataSourceConfigTypeDef

```python
# DataSourceConfigTypeDef definition

class DataSourceConfigTypeDef(TypedDict):
    name: str,
    s3Bucket: str,
    s3Keys: Sequence[str],
    type: NotRequired[DataSourceTypeType],  # (1)
    destination: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
## S3KeyOutputTypeDef

```python
# S3KeyOutputTypeDef definition

class S3KeyOutputTypeDef(TypedDict):
    s3Key: NotRequired[str],
    etag: NotRequired[str],
```

## DeleteFleetRequestRequestTypeDef

```python
# DeleteFleetRequestRequestTypeDef definition

class DeleteFleetRequestRequestTypeDef(TypedDict):
    fleet: str,
```

## DeleteRobotApplicationRequestRequestTypeDef

```python
# DeleteRobotApplicationRequestRequestTypeDef definition

class DeleteRobotApplicationRequestRequestTypeDef(TypedDict):
    application: str,
    applicationVersion: NotRequired[str],
```

## DeleteRobotRequestRequestTypeDef

```python
# DeleteRobotRequestRequestTypeDef definition

class DeleteRobotRequestRequestTypeDef(TypedDict):
    robot: str,
```

## DeleteSimulationApplicationRequestRequestTypeDef

```python
# DeleteSimulationApplicationRequestRequestTypeDef definition

class DeleteSimulationApplicationRequestRequestTypeDef(TypedDict):
    application: str,
    applicationVersion: NotRequired[str],
```

## DeleteWorldTemplateRequestRequestTypeDef

```python
# DeleteWorldTemplateRequestRequestTypeDef definition

class DeleteWorldTemplateRequestRequestTypeDef(TypedDict):
    template: str,
```

## DeploymentLaunchConfigOutputTypeDef

```python
# DeploymentLaunchConfigOutputTypeDef definition

class DeploymentLaunchConfigOutputTypeDef(TypedDict):
    packageName: str,
    launchFile: str,
    preLaunchFile: NotRequired[str],
    postLaunchFile: NotRequired[str],
    environmentVariables: NotRequired[Dict[str, str]],
```

## S3ObjectTypeDef

```python
# S3ObjectTypeDef definition

class S3ObjectTypeDef(TypedDict):
    bucket: str,
    key: str,
    etag: NotRequired[str],
```

## DeploymentLaunchConfigTypeDef

```python
# DeploymentLaunchConfigTypeDef definition

class DeploymentLaunchConfigTypeDef(TypedDict):
    packageName: str,
    launchFile: str,
    preLaunchFile: NotRequired[str],
    postLaunchFile: NotRequired[str],
    environmentVariables: NotRequired[Mapping[str, str]],
```

## DeregisterRobotRequestRequestTypeDef

```python
# DeregisterRobotRequestRequestTypeDef definition

class DeregisterRobotRequestRequestTypeDef(TypedDict):
    fleet: str,
    robot: str,
```

## DescribeDeploymentJobRequestRequestTypeDef

```python
# DescribeDeploymentJobRequestRequestTypeDef definition

class DescribeDeploymentJobRequestRequestTypeDef(TypedDict):
    job: str,
```

## DescribeFleetRequestRequestTypeDef

```python
# DescribeFleetRequestRequestTypeDef definition

class DescribeFleetRequestRequestTypeDef(TypedDict):
    fleet: str,
```

## RobotTypeDef

```python
# RobotTypeDef definition

class RobotTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    fleetArn: NotRequired[str],
    status: NotRequired[RobotStatusType],  # (1)
    greenGrassGroupId: NotRequired[str],
    createdAt: NotRequired[datetime],
    architecture: NotRequired[ArchitectureType],  # (2)
    lastDeploymentJob: NotRequired[str],
    lastDeploymentTime: NotRequired[datetime],
```

1. See [:material-code-brackets: RobotStatusType](./literals.md#robotstatustype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## DescribeRobotApplicationRequestRequestTypeDef

```python
# DescribeRobotApplicationRequestRequestTypeDef definition

class DescribeRobotApplicationRequestRequestTypeDef(TypedDict):
    application: str,
    applicationVersion: NotRequired[str],
```

## DescribeRobotRequestRequestTypeDef

```python
# DescribeRobotRequestRequestTypeDef definition

class DescribeRobotRequestRequestTypeDef(TypedDict):
    robot: str,
```

## DescribeSimulationApplicationRequestRequestTypeDef

```python
# DescribeSimulationApplicationRequestRequestTypeDef definition

class DescribeSimulationApplicationRequestRequestTypeDef(TypedDict):
    application: str,
    applicationVersion: NotRequired[str],
```

## DescribeSimulationJobBatchRequestRequestTypeDef

```python
# DescribeSimulationJobBatchRequestRequestTypeDef definition

class DescribeSimulationJobBatchRequestRequestTypeDef(TypedDict):
    batch: str,
```

## SimulationJobSummaryTypeDef

```python
# SimulationJobSummaryTypeDef definition

class SimulationJobSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    name: NotRequired[str],
    status: NotRequired[SimulationJobStatusType],  # (1)
    simulationApplicationNames: NotRequired[List[str]],
    robotApplicationNames: NotRequired[List[str]],
    dataSourceNames: NotRequired[List[str]],
    computeType: NotRequired[ComputeTypeType],  # (2)
```

1. See [:material-code-brackets: SimulationJobStatusType](./literals.md#simulationjobstatustype) 
2. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
## DescribeSimulationJobRequestRequestTypeDef

```python
# DescribeSimulationJobRequestRequestTypeDef definition

class DescribeSimulationJobRequestRequestTypeDef(TypedDict):
    job: str,
```

## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    networkInterfaceId: NotRequired[str],
    privateIpAddress: NotRequired[str],
    publicIpAddress: NotRequired[str],
```

## DescribeWorldExportJobRequestRequestTypeDef

```python
# DescribeWorldExportJobRequestRequestTypeDef definition

class DescribeWorldExportJobRequestRequestTypeDef(TypedDict):
    job: str,
```

## DescribeWorldGenerationJobRequestRequestTypeDef

```python
# DescribeWorldGenerationJobRequestRequestTypeDef definition

class DescribeWorldGenerationJobRequestRequestTypeDef(TypedDict):
    job: str,
```

## DescribeWorldRequestRequestTypeDef

```python
# DescribeWorldRequestRequestTypeDef definition

class DescribeWorldRequestRequestTypeDef(TypedDict):
    world: str,
```

## DescribeWorldTemplateRequestRequestTypeDef

```python
# DescribeWorldTemplateRequestRequestTypeDef definition

class DescribeWorldTemplateRequestRequestTypeDef(TypedDict):
    template: str,
```

## WorldFailureTypeDef

```python
# WorldFailureTypeDef definition

class WorldFailureTypeDef(TypedDict):
    failureCode: NotRequired[WorldGenerationJobErrorCodeType],  # (1)
    sampleFailureReason: NotRequired[str],
    failureCount: NotRequired[int],
```

1. See [:material-code-brackets: WorldGenerationJobErrorCodeType](./literals.md#worldgenerationjoberrorcodetype) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    name: NotRequired[str],
    values: NotRequired[Sequence[str]],
```

## FleetTypeDef

```python
# FleetTypeDef definition

class FleetTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    lastDeploymentStatus: NotRequired[DeploymentStatusType],  # (1)
    lastDeploymentJob: NotRequired[str],
    lastDeploymentTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## GetWorldTemplateBodyRequestRequestTypeDef

```python
# GetWorldTemplateBodyRequestRequestTypeDef definition

class GetWorldTemplateBodyRequestRequestTypeDef(TypedDict):
    template: NotRequired[str],
    generationJob: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## SimulationJobBatchSummaryTypeDef

```python
# SimulationJobBatchSummaryTypeDef definition

class SimulationJobBatchSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    createdAt: NotRequired[datetime],
    status: NotRequired[SimulationJobBatchStatusType],  # (1)
    failedRequestCount: NotRequired[int],
    pendingRequestCount: NotRequired[int],
    createdRequestCount: NotRequired[int],
```

1. See [:material-code-brackets: SimulationJobBatchStatusType](./literals.md#simulationjobbatchstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListWorldTemplatesRequestRequestTypeDef

```python
# ListWorldTemplatesRequestRequestTypeDef definition

class ListWorldTemplatesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TemplateSummaryTypeDef

```python
# TemplateSummaryTypeDef definition

class TemplateSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    name: NotRequired[str],
    version: NotRequired[str],
```

## WorldSummaryTypeDef

```python
# WorldSummaryTypeDef definition

class WorldSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    generationJob: NotRequired[str],
    template: NotRequired[str],
```

## PortMappingTypeDef

```python
# PortMappingTypeDef definition

class PortMappingTypeDef(TypedDict):
    jobPort: int,
    applicationPort: int,
    enableOnPublicIp: NotRequired[bool],
```

## ProgressDetailTypeDef

```python
# ProgressDetailTypeDef definition

class ProgressDetailTypeDef(TypedDict):
    currentProgress: NotRequired[RobotDeploymentStepType],  # (1)
    percentDone: NotRequired[float],
    estimatedTimeRemainingSeconds: NotRequired[int],
    targetResource: NotRequired[str],
```

1. See [:material-code-brackets: RobotDeploymentStepType](./literals.md#robotdeploymentsteptype) 
## RegisterRobotRequestRequestTypeDef

```python
# RegisterRobotRequestRequestTypeDef definition

class RegisterRobotRequestRequestTypeDef(TypedDict):
    fleet: str,
    robot: str,
```

## RestartSimulationJobRequestRequestTypeDef

```python
# RestartSimulationJobRequestRequestTypeDef definition

class RestartSimulationJobRequestRequestTypeDef(TypedDict):
    job: str,
```

## ToolTypeDef

```python
# ToolTypeDef definition

class ToolTypeDef(TypedDict):
    name: str,
    command: str,
    streamUI: NotRequired[bool],
    streamOutputToCloudWatch: NotRequired[bool],
    exitBehavior: NotRequired[ExitBehaviorType],  # (1)
```

1. See [:material-code-brackets: ExitBehaviorType](./literals.md#exitbehaviortype) 
## UploadConfigurationTypeDef

```python
# UploadConfigurationTypeDef definition

class UploadConfigurationTypeDef(TypedDict):
    name: str,
    path: str,
    uploadBehavior: UploadBehaviorType,  # (1)
```

1. See [:material-code-brackets: UploadBehaviorType](./literals.md#uploadbehaviortype) 
## WorldConfigTypeDef

```python
# WorldConfigTypeDef definition

class WorldConfigTypeDef(TypedDict):
    world: NotRequired[str],
```

## VPCConfigOutputTypeDef

```python
# VPCConfigOutputTypeDef definition

class VPCConfigOutputTypeDef(TypedDict):
    subnets: List[str],
    securityGroups: NotRequired[List[str]],
    assignPublicIp: NotRequired[bool],
```

## SyncDeploymentJobRequestRequestTypeDef

```python
# SyncDeploymentJobRequestRequestTypeDef definition

class SyncDeploymentJobRequestRequestTypeDef(TypedDict):
    clientRequestToken: str,
    fleet: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## BatchDeleteWorldsResponseTypeDef

```python
# BatchDeleteWorldsResponseTypeDef definition

class BatchDeleteWorldsResponseTypeDef(TypedDict):
    unprocessedWorlds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetResponseTypeDef

```python
# CreateFleetResponseTypeDef definition

class CreateFleetResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    createdAt: datetime,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRobotResponseTypeDef

```python
# CreateRobotResponseTypeDef definition

class CreateRobotResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    createdAt: datetime,
    greengrassGroupId: str,
    architecture: ArchitectureType,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorldTemplateResponseTypeDef

```python
# CreateWorldTemplateResponseTypeDef definition

class CreateWorldTemplateResponseTypeDef(TypedDict):
    arn: str,
    clientRequestToken: str,
    createdAt: datetime,
    name: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterRobotResponseTypeDef

```python
# DeregisterRobotResponseTypeDef definition

class DeregisterRobotResponseTypeDef(TypedDict):
    fleet: str,
    robot: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRobotResponseTypeDef

```python
# DescribeRobotResponseTypeDef definition

class DescribeRobotResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    fleetArn: str,
    status: RobotStatusType,  # (1)
    greengrassGroupId: str,
    createdAt: datetime,
    architecture: ArchitectureType,  # (2)
    lastDeploymentJob: str,
    lastDeploymentTime: datetime,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: RobotStatusType](./literals.md#robotstatustype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorldResponseTypeDef

```python
# DescribeWorldResponseTypeDef definition

class DescribeWorldResponseTypeDef(TypedDict):
    arn: str,
    generationJob: str,
    template: str,
    createdAt: datetime,
    tags: Dict[str, str],
    worldDescriptionBody: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorldTemplateResponseTypeDef

```python
# DescribeWorldTemplateResponseTypeDef definition

class DescribeWorldTemplateResponseTypeDef(TypedDict):
    arn: str,
    clientRequestToken: str,
    name: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    tags: Dict[str, str],
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorldTemplateBodyResponseTypeDef

```python
# GetWorldTemplateBodyResponseTypeDef definition

class GetWorldTemplateBodyResponseTypeDef(TypedDict):
    templateBody: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterRobotResponseTypeDef

```python
# RegisterRobotResponseTypeDef definition

class RegisterRobotResponseTypeDef(TypedDict):
    fleet: str,
    robot: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorldTemplateResponseTypeDef

```python
# UpdateWorldTemplateResponseTypeDef definition

class UpdateWorldTemplateResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RobotApplicationSummaryTypeDef

```python
# RobotApplicationSummaryTypeDef definition

class RobotApplicationSummaryTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    version: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    robotSoftwareSuite: NotRequired[RobotSoftwareSuiteTypeDef],  # (1)
```

1. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
## CreateRobotApplicationRequestRequestTypeDef

```python
# CreateRobotApplicationRequestRequestTypeDef definition

class CreateRobotApplicationRequestRequestTypeDef(TypedDict):
    name: str,
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (1)
    sources: NotRequired[Sequence[SourceConfigTypeDef]],  # (2)
    tags: NotRequired[Mapping[str, str]],
    environment: NotRequired[EnvironmentTypeDef],  # (3)
```

1. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
2. See [:material-code-braces: SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef) 
3. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
## UpdateRobotApplicationRequestRequestTypeDef

```python
# UpdateRobotApplicationRequestRequestTypeDef definition

class UpdateRobotApplicationRequestRequestTypeDef(TypedDict):
    application: str,
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (1)
    sources: NotRequired[Sequence[SourceConfigTypeDef]],  # (2)
    currentRevisionId: NotRequired[str],
    environment: NotRequired[EnvironmentTypeDef],  # (3)
```

1. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
2. See [:material-code-braces: SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef) 
3. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
## CreateRobotApplicationResponseTypeDef

```python
# CreateRobotApplicationResponseTypeDef definition

class CreateRobotApplicationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    version: str,
    sources: List[SourceTypeDef],  # (1)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (2)
    lastUpdatedAt: datetime,
    revisionId: str,
    tags: Dict[str, str],
    environment: EnvironmentTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
3. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRobotApplicationVersionResponseTypeDef

```python
# CreateRobotApplicationVersionResponseTypeDef definition

class CreateRobotApplicationVersionResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    version: str,
    sources: List[SourceTypeDef],  # (1)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (2)
    lastUpdatedAt: datetime,
    revisionId: str,
    environment: EnvironmentTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
3. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRobotApplicationResponseTypeDef

```python
# DescribeRobotApplicationResponseTypeDef definition

class DescribeRobotApplicationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    version: str,
    sources: List[SourceTypeDef],  # (1)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (2)
    revisionId: str,
    lastUpdatedAt: datetime,
    tags: Dict[str, str],
    environment: EnvironmentTypeDef,  # (3)
    imageDigest: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
3. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRobotApplicationResponseTypeDef

```python
# UpdateRobotApplicationResponseTypeDef definition

class UpdateRobotApplicationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    version: str,
    sources: List[SourceTypeDef],  # (1)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (2)
    lastUpdatedAt: datetime,
    revisionId: str,
    environment: EnvironmentTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
3. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSimulationApplicationRequestRequestTypeDef

```python
# CreateSimulationApplicationRequestRequestTypeDef definition

class CreateSimulationApplicationRequestRequestTypeDef(TypedDict):
    name: str,
    simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,  # (1)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (2)
    sources: NotRequired[Sequence[SourceConfigTypeDef]],  # (3)
    renderingEngine: NotRequired[RenderingEngineTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
    environment: NotRequired[EnvironmentTypeDef],  # (5)
```

1. See [:material-code-braces: SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef) 
2. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
3. See [:material-code-braces: SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef) 
4. See [:material-code-braces: RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef) 
5. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
## CreateSimulationApplicationResponseTypeDef

```python
# CreateSimulationApplicationResponseTypeDef definition

class CreateSimulationApplicationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    version: str,
    sources: List[SourceTypeDef],  # (1)
    simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,  # (2)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (3)
    renderingEngine: RenderingEngineTypeDef,  # (4)
    lastUpdatedAt: datetime,
    revisionId: str,
    tags: Dict[str, str],
    environment: EnvironmentTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef) 
3. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
4. See [:material-code-braces: RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef) 
5. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSimulationApplicationVersionResponseTypeDef

```python
# CreateSimulationApplicationVersionResponseTypeDef definition

class CreateSimulationApplicationVersionResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    version: str,
    sources: List[SourceTypeDef],  # (1)
    simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,  # (2)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (3)
    renderingEngine: RenderingEngineTypeDef,  # (4)
    lastUpdatedAt: datetime,
    revisionId: str,
    environment: EnvironmentTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef) 
3. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
4. See [:material-code-braces: RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef) 
5. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSimulationApplicationResponseTypeDef

```python
# DescribeSimulationApplicationResponseTypeDef definition

class DescribeSimulationApplicationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    version: str,
    sources: List[SourceTypeDef],  # (1)
    simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,  # (2)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (3)
    renderingEngine: RenderingEngineTypeDef,  # (4)
    revisionId: str,
    lastUpdatedAt: datetime,
    tags: Dict[str, str],
    environment: EnvironmentTypeDef,  # (5)
    imageDigest: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef) 
3. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
4. See [:material-code-braces: RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef) 
5. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SimulationApplicationSummaryTypeDef

```python
# SimulationApplicationSummaryTypeDef definition

class SimulationApplicationSummaryTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    version: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    robotSoftwareSuite: NotRequired[RobotSoftwareSuiteTypeDef],  # (1)
    simulationSoftwareSuite: NotRequired[SimulationSoftwareSuiteTypeDef],  # (2)
```

1. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
2. See [:material-code-braces: SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef) 
## UpdateSimulationApplicationRequestRequestTypeDef

```python
# UpdateSimulationApplicationRequestRequestTypeDef definition

class UpdateSimulationApplicationRequestRequestTypeDef(TypedDict):
    application: str,
    simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,  # (1)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (2)
    sources: NotRequired[Sequence[SourceConfigTypeDef]],  # (3)
    renderingEngine: NotRequired[RenderingEngineTypeDef],  # (4)
    currentRevisionId: NotRequired[str],
    environment: NotRequired[EnvironmentTypeDef],  # (5)
```

1. See [:material-code-braces: SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef) 
2. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
3. See [:material-code-braces: SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef) 
4. See [:material-code-braces: RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef) 
5. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
## UpdateSimulationApplicationResponseTypeDef

```python
# UpdateSimulationApplicationResponseTypeDef definition

class UpdateSimulationApplicationResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    version: str,
    sources: List[SourceTypeDef],  # (1)
    simulationSoftwareSuite: SimulationSoftwareSuiteTypeDef,  # (2)
    robotSoftwareSuite: RobotSoftwareSuiteTypeDef,  # (3)
    renderingEngine: RenderingEngineTypeDef,  # (4)
    lastUpdatedAt: datetime,
    revisionId: str,
    environment: EnvironmentTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-braces: SimulationSoftwareSuiteTypeDef](./type_defs.md#simulationsoftwaresuitetypedef) 
3. See [:material-code-braces: RobotSoftwareSuiteTypeDef](./type_defs.md#robotsoftwaresuitetypedef) 
4. See [:material-code-braces: RenderingEngineTypeDef](./type_defs.md#renderingenginetypedef) 
5. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorldExportJobRequestRequestTypeDef

```python
# CreateWorldExportJobRequestRequestTypeDef definition

class CreateWorldExportJobRequestRequestTypeDef(TypedDict):
    worlds: Sequence[str],
    outputLocation: OutputLocationTypeDef,  # (1)
    iamRole: str,
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
## CreateWorldExportJobResponseTypeDef

```python
# CreateWorldExportJobResponseTypeDef definition

class CreateWorldExportJobResponseTypeDef(TypedDict):
    arn: str,
    status: WorldExportJobStatusType,  # (1)
    createdAt: datetime,
    failureCode: WorldExportJobErrorCodeType,  # (2)
    clientRequestToken: str,
    outputLocation: OutputLocationTypeDef,  # (3)
    iamRole: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: WorldExportJobStatusType](./literals.md#worldexportjobstatustype) 
2. See [:material-code-brackets: WorldExportJobErrorCodeType](./literals.md#worldexportjoberrorcodetype) 
3. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorldExportJobResponseTypeDef

```python
# DescribeWorldExportJobResponseTypeDef definition

class DescribeWorldExportJobResponseTypeDef(TypedDict):
    arn: str,
    status: WorldExportJobStatusType,  # (1)
    createdAt: datetime,
    failureCode: WorldExportJobErrorCodeType,  # (2)
    failureReason: str,
    clientRequestToken: str,
    worlds: List[str],
    outputLocation: OutputLocationTypeDef,  # (3)
    iamRole: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: WorldExportJobStatusType](./literals.md#worldexportjobstatustype) 
2. See [:material-code-brackets: WorldExportJobErrorCodeType](./literals.md#worldexportjoberrorcodetype) 
3. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorldExportJobSummaryTypeDef

```python
# WorldExportJobSummaryTypeDef definition

class WorldExportJobSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    status: NotRequired[WorldExportJobStatusType],  # (1)
    createdAt: NotRequired[datetime],
    worlds: NotRequired[List[str]],
    outputLocation: NotRequired[OutputLocationTypeDef],  # (2)
```

1. See [:material-code-brackets: WorldExportJobStatusType](./literals.md#worldexportjobstatustype) 
2. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
## CreateWorldGenerationJobRequestRequestTypeDef

```python
# CreateWorldGenerationJobRequestRequestTypeDef definition

class CreateWorldGenerationJobRequestRequestTypeDef(TypedDict):
    template: str,
    worldCount: WorldCountTypeDef,  # (1)
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    worldTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: WorldCountTypeDef](./type_defs.md#worldcounttypedef) 
## CreateWorldGenerationJobResponseTypeDef

```python
# CreateWorldGenerationJobResponseTypeDef definition

class CreateWorldGenerationJobResponseTypeDef(TypedDict):
    arn: str,
    status: WorldGenerationJobStatusType,  # (1)
    createdAt: datetime,
    failureCode: WorldGenerationJobErrorCodeType,  # (2)
    clientRequestToken: str,
    template: str,
    worldCount: WorldCountTypeDef,  # (3)
    tags: Dict[str, str],
    worldTags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: WorldGenerationJobStatusType](./literals.md#worldgenerationjobstatustype) 
2. See [:material-code-brackets: WorldGenerationJobErrorCodeType](./literals.md#worldgenerationjoberrorcodetype) 
3. See [:material-code-braces: WorldCountTypeDef](./type_defs.md#worldcounttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorldGenerationJobSummaryTypeDef

```python
# WorldGenerationJobSummaryTypeDef definition

class WorldGenerationJobSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    template: NotRequired[str],
    createdAt: NotRequired[datetime],
    status: NotRequired[WorldGenerationJobStatusType],  # (1)
    worldCount: NotRequired[WorldCountTypeDef],  # (2)
    succeededWorldCount: NotRequired[int],
    failedWorldCount: NotRequired[int],
```

1. See [:material-code-brackets: WorldGenerationJobStatusType](./literals.md#worldgenerationjobstatustype) 
2. See [:material-code-braces: WorldCountTypeDef](./type_defs.md#worldcounttypedef) 
## CreateWorldTemplateRequestRequestTypeDef

```python
# CreateWorldTemplateRequestRequestTypeDef definition

class CreateWorldTemplateRequestRequestTypeDef(TypedDict):
    clientRequestToken: NotRequired[str],
    name: NotRequired[str],
    templateBody: NotRequired[str],
    templateLocation: NotRequired[TemplateLocationTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TemplateLocationTypeDef](./type_defs.md#templatelocationtypedef) 
## UpdateWorldTemplateRequestRequestTypeDef

```python
# UpdateWorldTemplateRequestRequestTypeDef definition

class UpdateWorldTemplateRequestRequestTypeDef(TypedDict):
    template: str,
    name: NotRequired[str],
    templateBody: NotRequired[str],
    templateLocation: NotRequired[TemplateLocationTypeDef],  # (1)
```

1. See [:material-code-braces: TemplateLocationTypeDef](./type_defs.md#templatelocationtypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    name: NotRequired[str],
    s3Bucket: NotRequired[str],
    s3Keys: NotRequired[List[S3KeyOutputTypeDef]],  # (1)
    type: NotRequired[DataSourceTypeType],  # (2)
    destination: NotRequired[str],
```

1. See [:material-code-braces: S3KeyOutputTypeDef](./type_defs.md#s3keyoutputtypedef) 
2. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
## DeploymentApplicationConfigOutputTypeDef

```python
# DeploymentApplicationConfigOutputTypeDef definition

class DeploymentApplicationConfigOutputTypeDef(TypedDict):
    application: str,
    applicationVersion: str,
    launchConfig: DeploymentLaunchConfigOutputTypeDef,  # (1)
```

1. See [:material-code-braces: DeploymentLaunchConfigOutputTypeDef](./type_defs.md#deploymentlaunchconfigoutputtypedef) 
## DeploymentConfigTypeDef

```python
# DeploymentConfigTypeDef definition

class DeploymentConfigTypeDef(TypedDict):
    concurrentDeploymentPercentage: NotRequired[int],
    failureThresholdPercentage: NotRequired[int],
    robotDeploymentTimeoutInSeconds: NotRequired[int],
    downloadConditionFile: NotRequired[S3ObjectTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
## DescribeFleetResponseTypeDef

```python
# DescribeFleetResponseTypeDef definition

class DescribeFleetResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    robots: List[RobotTypeDef],  # (1)
    createdAt: datetime,
    lastDeploymentStatus: DeploymentStatusType,  # (2)
    lastDeploymentJob: str,
    lastDeploymentTime: datetime,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RobotTypeDef](./type_defs.md#robottypedef) 
2. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRobotsResponseTypeDef

```python
# ListRobotsResponseTypeDef definition

class ListRobotsResponseTypeDef(TypedDict):
    robots: List[RobotTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RobotTypeDef](./type_defs.md#robottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSimulationJobsResponseTypeDef

```python
# ListSimulationJobsResponseTypeDef definition

class ListSimulationJobsResponseTypeDef(TypedDict):
    simulationJobSummaries: List[SimulationJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SimulationJobSummaryTypeDef](./type_defs.md#simulationjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailureSummaryTypeDef

```python
# FailureSummaryTypeDef definition

class FailureSummaryTypeDef(TypedDict):
    totalFailureCount: NotRequired[int],
    failures: NotRequired[List[WorldFailureTypeDef]],  # (1)
```

1. See [:material-code-braces: WorldFailureTypeDef](./type_defs.md#worldfailuretypedef) 
## ListDeploymentJobsRequestRequestTypeDef

```python
# ListDeploymentJobsRequestRequestTypeDef definition

class ListDeploymentJobsRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListFleetsRequestRequestTypeDef

```python
# ListFleetsRequestRequestTypeDef definition

class ListFleetsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListRobotApplicationsRequestRequestTypeDef

```python
# ListRobotApplicationsRequestRequestTypeDef definition

class ListRobotApplicationsRequestRequestTypeDef(TypedDict):
    versionQualifier: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListRobotsRequestRequestTypeDef

```python
# ListRobotsRequestRequestTypeDef definition

class ListRobotsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListSimulationApplicationsRequestRequestTypeDef

```python
# ListSimulationApplicationsRequestRequestTypeDef definition

class ListSimulationApplicationsRequestRequestTypeDef(TypedDict):
    versionQualifier: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListSimulationJobBatchesRequestRequestTypeDef

```python
# ListSimulationJobBatchesRequestRequestTypeDef definition

class ListSimulationJobBatchesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListSimulationJobsRequestRequestTypeDef

```python
# ListSimulationJobsRequestRequestTypeDef definition

class ListSimulationJobsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListWorldExportJobsRequestRequestTypeDef

```python
# ListWorldExportJobsRequestRequestTypeDef definition

class ListWorldExportJobsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListWorldGenerationJobsRequestRequestTypeDef

```python
# ListWorldGenerationJobsRequestRequestTypeDef definition

class ListWorldGenerationJobsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListWorldsRequestRequestTypeDef

```python
# ListWorldsRequestRequestTypeDef definition

class ListWorldsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListFleetsResponseTypeDef

```python
# ListFleetsResponseTypeDef definition

class ListFleetsResponseTypeDef(TypedDict):
    fleetDetails: List[FleetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetTypeDef](./type_defs.md#fleettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef

```python
# ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef definition

class ListDeploymentJobsRequestListDeploymentJobsPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFleetsRequestListFleetsPaginateTypeDef

```python
# ListFleetsRequestListFleetsPaginateTypeDef definition

class ListFleetsRequestListFleetsPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef

```python
# ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef definition

class ListRobotApplicationsRequestListRobotApplicationsPaginateTypeDef(TypedDict):
    versionQualifier: NotRequired[str],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRobotsRequestListRobotsPaginateTypeDef

```python
# ListRobotsRequestListRobotsPaginateTypeDef definition

class ListRobotsRequestListRobotsPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef

```python
# ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef definition

class ListSimulationApplicationsRequestListSimulationApplicationsPaginateTypeDef(TypedDict):
    versionQualifier: NotRequired[str],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef

```python
# ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef definition

class ListSimulationJobBatchesRequestListSimulationJobBatchesPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSimulationJobsRequestListSimulationJobsPaginateTypeDef

```python
# ListSimulationJobsRequestListSimulationJobsPaginateTypeDef definition

class ListSimulationJobsRequestListSimulationJobsPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef

```python
# ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef definition

class ListWorldExportJobsRequestListWorldExportJobsPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef

```python
# ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef definition

class ListWorldGenerationJobsRequestListWorldGenerationJobsPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef

```python
# ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef definition

class ListWorldTemplatesRequestListWorldTemplatesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorldsRequestListWorldsPaginateTypeDef

```python
# ListWorldsRequestListWorldsPaginateTypeDef definition

class ListWorldsRequestListWorldsPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSimulationJobBatchesResponseTypeDef

```python
# ListSimulationJobBatchesResponseTypeDef definition

class ListSimulationJobBatchesResponseTypeDef(TypedDict):
    simulationJobBatchSummaries: List[SimulationJobBatchSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SimulationJobBatchSummaryTypeDef](./type_defs.md#simulationjobbatchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorldTemplatesResponseTypeDef

```python
# ListWorldTemplatesResponseTypeDef definition

class ListWorldTemplatesResponseTypeDef(TypedDict):
    templateSummaries: List[TemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorldsResponseTypeDef

```python
# ListWorldsResponseTypeDef definition

class ListWorldsResponseTypeDef(TypedDict):
    worldSummaries: List[WorldSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorldSummaryTypeDef](./type_defs.md#worldsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PortForwardingConfigOutputTypeDef

```python
# PortForwardingConfigOutputTypeDef definition

class PortForwardingConfigOutputTypeDef(TypedDict):
    portMappings: NotRequired[List[PortMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: PortMappingTypeDef](./type_defs.md#portmappingtypedef) 
## PortForwardingConfigTypeDef

```python
# PortForwardingConfigTypeDef definition

class PortForwardingConfigTypeDef(TypedDict):
    portMappings: NotRequired[Sequence[PortMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: PortMappingTypeDef](./type_defs.md#portmappingtypedef) 
## RobotDeploymentTypeDef

```python
# RobotDeploymentTypeDef definition

class RobotDeploymentTypeDef(TypedDict):
    arn: NotRequired[str],
    deploymentStartTime: NotRequired[datetime],
    deploymentFinishTime: NotRequired[datetime],
    status: NotRequired[RobotStatusType],  # (1)
    progressDetail: NotRequired[ProgressDetailTypeDef],  # (2)
    failureReason: NotRequired[str],
    failureCode: NotRequired[DeploymentJobErrorCodeType],  # (3)
```

1. See [:material-code-brackets: RobotStatusType](./literals.md#robotstatustype) 
2. See [:material-code-braces: ProgressDetailTypeDef](./type_defs.md#progressdetailtypedef) 
3. See [:material-code-brackets: DeploymentJobErrorCodeType](./literals.md#deploymentjoberrorcodetype) 
## ListRobotApplicationsResponseTypeDef

```python
# ListRobotApplicationsResponseTypeDef definition

class ListRobotApplicationsResponseTypeDef(TypedDict):
    robotApplicationSummaries: List[RobotApplicationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RobotApplicationSummaryTypeDef](./type_defs.md#robotapplicationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSimulationApplicationsResponseTypeDef

```python
# ListSimulationApplicationsResponseTypeDef definition

class ListSimulationApplicationsResponseTypeDef(TypedDict):
    simulationApplicationSummaries: List[SimulationApplicationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SimulationApplicationSummaryTypeDef](./type_defs.md#simulationapplicationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorldExportJobsResponseTypeDef

```python
# ListWorldExportJobsResponseTypeDef definition

class ListWorldExportJobsResponseTypeDef(TypedDict):
    worldExportJobSummaries: List[WorldExportJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorldExportJobSummaryTypeDef](./type_defs.md#worldexportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorldGenerationJobsResponseTypeDef

```python
# ListWorldGenerationJobsResponseTypeDef definition

class ListWorldGenerationJobsResponseTypeDef(TypedDict):
    worldGenerationJobSummaries: List[WorldGenerationJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorldGenerationJobSummaryTypeDef](./type_defs.md#worldgenerationjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentJobResponseTypeDef

```python
# CreateDeploymentJobResponseTypeDef definition

class CreateDeploymentJobResponseTypeDef(TypedDict):
    arn: str,
    fleet: str,
    status: DeploymentStatusType,  # (1)
    deploymentApplicationConfigs: List[DeploymentApplicationConfigOutputTypeDef],  # (2)
    failureReason: str,
    failureCode: DeploymentJobErrorCodeType,  # (3)
    createdAt: datetime,
    deploymentConfig: DeploymentConfigTypeDef,  # (4)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: DeploymentApplicationConfigOutputTypeDef](./type_defs.md#deploymentapplicationconfigoutputtypedef) 
3. See [:material-code-brackets: DeploymentJobErrorCodeType](./literals.md#deploymentjoberrorcodetype) 
4. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentJobTypeDef

```python
# DeploymentJobTypeDef definition

class DeploymentJobTypeDef(TypedDict):
    arn: NotRequired[str],
    fleet: NotRequired[str],
    status: NotRequired[DeploymentStatusType],  # (1)
    deploymentApplicationConfigs: NotRequired[List[DeploymentApplicationConfigOutputTypeDef]],  # (2)
    deploymentConfig: NotRequired[DeploymentConfigTypeDef],  # (3)
    failureReason: NotRequired[str],
    failureCode: NotRequired[DeploymentJobErrorCodeType],  # (4)
    createdAt: NotRequired[datetime],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: DeploymentApplicationConfigOutputTypeDef](./type_defs.md#deploymentapplicationconfigoutputtypedef) 
3. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) 
4. See [:material-code-brackets: DeploymentJobErrorCodeType](./literals.md#deploymentjoberrorcodetype) 
## SyncDeploymentJobResponseTypeDef

```python
# SyncDeploymentJobResponseTypeDef definition

class SyncDeploymentJobResponseTypeDef(TypedDict):
    arn: str,
    fleet: str,
    status: DeploymentStatusType,  # (1)
    deploymentConfig: DeploymentConfigTypeDef,  # (2)
    deploymentApplicationConfigs: List[DeploymentApplicationConfigOutputTypeDef],  # (3)
    failureReason: str,
    failureCode: DeploymentJobErrorCodeType,  # (4)
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) 
3. See [:material-code-braces: DeploymentApplicationConfigOutputTypeDef](./type_defs.md#deploymentapplicationconfigoutputtypedef) 
4. See [:material-code-brackets: DeploymentJobErrorCodeType](./literals.md#deploymentjoberrorcodetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentApplicationConfigTypeDef

```python
# DeploymentApplicationConfigTypeDef definition

class DeploymentApplicationConfigTypeDef(TypedDict):
    application: str,
    applicationVersion: str,
    launchConfig: DeploymentLaunchConfigUnionTypeDef,  # (1)
```

1. See [:material-code-braces: DeploymentLaunchConfigTypeDef](./type_defs.md#deploymentlaunchconfigtypedef) [:material-code-braces: DeploymentLaunchConfigOutputTypeDef](./type_defs.md#deploymentlaunchconfigoutputtypedef) 
## FinishedWorldsSummaryTypeDef

```python
# FinishedWorldsSummaryTypeDef definition

class FinishedWorldsSummaryTypeDef(TypedDict):
    finishedCount: NotRequired[int],
    succeededWorlds: NotRequired[List[str]],
    failureSummary: NotRequired[FailureSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: FailureSummaryTypeDef](./type_defs.md#failuresummarytypedef) 
## LaunchConfigOutputTypeDef

```python
# LaunchConfigOutputTypeDef definition

class LaunchConfigOutputTypeDef(TypedDict):
    packageName: NotRequired[str],
    launchFile: NotRequired[str],
    environmentVariables: NotRequired[Dict[str, str]],
    portForwardingConfig: NotRequired[PortForwardingConfigOutputTypeDef],  # (1)
    streamUI: NotRequired[bool],
    command: NotRequired[List[str]],
```

1. See [:material-code-braces: PortForwardingConfigOutputTypeDef](./type_defs.md#portforwardingconfigoutputtypedef) 
## DescribeDeploymentJobResponseTypeDef

```python
# DescribeDeploymentJobResponseTypeDef definition

class DescribeDeploymentJobResponseTypeDef(TypedDict):
    arn: str,
    fleet: str,
    status: DeploymentStatusType,  # (1)
    deploymentConfig: DeploymentConfigTypeDef,  # (2)
    deploymentApplicationConfigs: List[DeploymentApplicationConfigOutputTypeDef],  # (3)
    failureReason: str,
    failureCode: DeploymentJobErrorCodeType,  # (4)
    createdAt: datetime,
    robotDeploymentSummary: List[RobotDeploymentTypeDef],  # (5)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) 
3. See [:material-code-braces: DeploymentApplicationConfigOutputTypeDef](./type_defs.md#deploymentapplicationconfigoutputtypedef) 
4. See [:material-code-brackets: DeploymentJobErrorCodeType](./literals.md#deploymentjoberrorcodetype) 
5. See [:material-code-braces: RobotDeploymentTypeDef](./type_defs.md#robotdeploymenttypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentJobsResponseTypeDef

```python
# ListDeploymentJobsResponseTypeDef definition

class ListDeploymentJobsResponseTypeDef(TypedDict):
    deploymentJobs: List[DeploymentJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentJobTypeDef](./type_defs.md#deploymentjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWorldGenerationJobResponseTypeDef

```python
# DescribeWorldGenerationJobResponseTypeDef definition

class DescribeWorldGenerationJobResponseTypeDef(TypedDict):
    arn: str,
    status: WorldGenerationJobStatusType,  # (1)
    createdAt: datetime,
    failureCode: WorldGenerationJobErrorCodeType,  # (2)
    failureReason: str,
    clientRequestToken: str,
    template: str,
    worldCount: WorldCountTypeDef,  # (3)
    finishedWorldsSummary: FinishedWorldsSummaryTypeDef,  # (4)
    tags: Dict[str, str],
    worldTags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: WorldGenerationJobStatusType](./literals.md#worldgenerationjobstatustype) 
2. See [:material-code-brackets: WorldGenerationJobErrorCodeType](./literals.md#worldgenerationjoberrorcodetype) 
3. See [:material-code-braces: WorldCountTypeDef](./type_defs.md#worldcounttypedef) 
4. See [:material-code-braces: FinishedWorldsSummaryTypeDef](./type_defs.md#finishedworldssummarytypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RobotApplicationConfigOutputTypeDef

```python
# RobotApplicationConfigOutputTypeDef definition

class RobotApplicationConfigOutputTypeDef(TypedDict):
    application: str,
    launchConfig: LaunchConfigOutputTypeDef,  # (1)
    applicationVersion: NotRequired[str],
    uploadConfigurations: NotRequired[List[UploadConfigurationTypeDef]],  # (2)
    useDefaultUploadConfigurations: NotRequired[bool],
    tools: NotRequired[List[ToolTypeDef]],  # (3)
    useDefaultTools: NotRequired[bool],
```

1. See [:material-code-braces: LaunchConfigOutputTypeDef](./type_defs.md#launchconfigoutputtypedef) 
2. See [:material-code-braces: UploadConfigurationTypeDef](./type_defs.md#uploadconfigurationtypedef) 
3. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
## SimulationApplicationConfigOutputTypeDef

```python
# SimulationApplicationConfigOutputTypeDef definition

class SimulationApplicationConfigOutputTypeDef(TypedDict):
    application: str,
    launchConfig: LaunchConfigOutputTypeDef,  # (1)
    applicationVersion: NotRequired[str],
    uploadConfigurations: NotRequired[List[UploadConfigurationTypeDef]],  # (2)
    worldConfigs: NotRequired[List[WorldConfigTypeDef]],  # (3)
    useDefaultUploadConfigurations: NotRequired[bool],
    tools: NotRequired[List[ToolTypeDef]],  # (4)
    useDefaultTools: NotRequired[bool],
```

1. See [:material-code-braces: LaunchConfigOutputTypeDef](./type_defs.md#launchconfigoutputtypedef) 
2. See [:material-code-braces: UploadConfigurationTypeDef](./type_defs.md#uploadconfigurationtypedef) 
3. See [:material-code-braces: WorldConfigTypeDef](./type_defs.md#worldconfigtypedef) 
4. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
## LaunchConfigTypeDef

```python
# LaunchConfigTypeDef definition

class LaunchConfigTypeDef(TypedDict):
    packageName: NotRequired[str],
    launchFile: NotRequired[str],
    environmentVariables: NotRequired[Mapping[str, str]],
    portForwardingConfig: NotRequired[PortForwardingConfigUnionTypeDef],  # (1)
    streamUI: NotRequired[bool],
    command: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: PortForwardingConfigTypeDef](./type_defs.md#portforwardingconfigtypedef) [:material-code-braces: PortForwardingConfigOutputTypeDef](./type_defs.md#portforwardingconfigoutputtypedef) 
## CreateDeploymentJobRequestRequestTypeDef

```python
# CreateDeploymentJobRequestRequestTypeDef definition

class CreateDeploymentJobRequestRequestTypeDef(TypedDict):
    clientRequestToken: str,
    fleet: str,
    deploymentApplicationConfigs: Sequence[DeploymentApplicationConfigUnionTypeDef],  # (1)
    deploymentConfig: NotRequired[DeploymentConfigTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DeploymentApplicationConfigTypeDef](./type_defs.md#deploymentapplicationconfigtypedef) [:material-code-braces: DeploymentApplicationConfigOutputTypeDef](./type_defs.md#deploymentapplicationconfigoutputtypedef) 
2. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) 
## CreateSimulationJobResponseTypeDef

```python
# CreateSimulationJobResponseTypeDef definition

class CreateSimulationJobResponseTypeDef(TypedDict):
    arn: str,
    status: SimulationJobStatusType,  # (1)
    lastStartedAt: datetime,
    lastUpdatedAt: datetime,
    failureBehavior: FailureBehaviorType,  # (2)
    failureCode: SimulationJobErrorCodeType,  # (3)
    clientRequestToken: str,
    outputLocation: OutputLocationTypeDef,  # (4)
    loggingConfig: LoggingConfigTypeDef,  # (5)
    maxJobDurationInSeconds: int,
    simulationTimeMillis: int,
    iamRole: str,
    robotApplications: List[RobotApplicationConfigOutputTypeDef],  # (6)
    simulationApplications: List[SimulationApplicationConfigOutputTypeDef],  # (7)
    dataSources: List[DataSourceTypeDef],  # (8)
    tags: Dict[str, str],
    vpcConfig: VPCConfigResponseTypeDef,  # (9)
    compute: ComputeResponseTypeDef,  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-brackets: SimulationJobStatusType](./literals.md#simulationjobstatustype) 
2. See [:material-code-brackets: FailureBehaviorType](./literals.md#failurebehaviortype) 
3. See [:material-code-brackets: SimulationJobErrorCodeType](./literals.md#simulationjoberrorcodetype) 
4. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
5. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
6. See [:material-code-braces: RobotApplicationConfigOutputTypeDef](./type_defs.md#robotapplicationconfigoutputtypedef) 
7. See [:material-code-braces: SimulationApplicationConfigOutputTypeDef](./type_defs.md#simulationapplicationconfigoutputtypedef) 
8. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
9. See [:material-code-braces: VPCConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef) 
10. See [:material-code-braces: ComputeResponseTypeDef](./type_defs.md#computeresponsetypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSimulationJobResponseTypeDef

```python
# DescribeSimulationJobResponseTypeDef definition

class DescribeSimulationJobResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    status: SimulationJobStatusType,  # (1)
    lastStartedAt: datetime,
    lastUpdatedAt: datetime,
    failureBehavior: FailureBehaviorType,  # (2)
    failureCode: SimulationJobErrorCodeType,  # (3)
    failureReason: str,
    clientRequestToken: str,
    outputLocation: OutputLocationTypeDef,  # (4)
    loggingConfig: LoggingConfigTypeDef,  # (5)
    maxJobDurationInSeconds: int,
    simulationTimeMillis: int,
    iamRole: str,
    robotApplications: List[RobotApplicationConfigOutputTypeDef],  # (6)
    simulationApplications: List[SimulationApplicationConfigOutputTypeDef],  # (7)
    dataSources: List[DataSourceTypeDef],  # (8)
    tags: Dict[str, str],
    vpcConfig: VPCConfigResponseTypeDef,  # (9)
    networkInterface: NetworkInterfaceTypeDef,  # (10)
    compute: ComputeResponseTypeDef,  # (11)
    ResponseMetadata: ResponseMetadataTypeDef,  # (12)
```

1. See [:material-code-brackets: SimulationJobStatusType](./literals.md#simulationjobstatustype) 
2. See [:material-code-brackets: FailureBehaviorType](./literals.md#failurebehaviortype) 
3. See [:material-code-brackets: SimulationJobErrorCodeType](./literals.md#simulationjoberrorcodetype) 
4. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
5. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
6. See [:material-code-braces: RobotApplicationConfigOutputTypeDef](./type_defs.md#robotapplicationconfigoutputtypedef) 
7. See [:material-code-braces: SimulationApplicationConfigOutputTypeDef](./type_defs.md#simulationapplicationconfigoutputtypedef) 
8. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
9. See [:material-code-braces: VPCConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef) 
10. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
11. See [:material-code-braces: ComputeResponseTypeDef](./type_defs.md#computeresponsetypedef) 
12. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SimulationJobRequestOutputTypeDef

```python
# SimulationJobRequestOutputTypeDef definition

class SimulationJobRequestOutputTypeDef(TypedDict):
    maxJobDurationInSeconds: int,
    outputLocation: NotRequired[OutputLocationTypeDef],  # (1)
    loggingConfig: NotRequired[LoggingConfigTypeDef],  # (2)
    iamRole: NotRequired[str],
    failureBehavior: NotRequired[FailureBehaviorType],  # (3)
    useDefaultApplications: NotRequired[bool],
    robotApplications: NotRequired[List[RobotApplicationConfigOutputTypeDef]],  # (4)
    simulationApplications: NotRequired[List[SimulationApplicationConfigOutputTypeDef]],  # (5)
    dataSources: NotRequired[List[DataSourceConfigOutputTypeDef]],  # (6)
    vpcConfig: NotRequired[VPCConfigOutputTypeDef],  # (7)
    compute: NotRequired[ComputeTypeDef],  # (8)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
2. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
3. See [:material-code-brackets: FailureBehaviorType](./literals.md#failurebehaviortype) 
4. See [:material-code-braces: RobotApplicationConfigOutputTypeDef](./type_defs.md#robotapplicationconfigoutputtypedef) 
5. See [:material-code-braces: SimulationApplicationConfigOutputTypeDef](./type_defs.md#simulationapplicationconfigoutputtypedef) 
6. See [:material-code-braces: DataSourceConfigOutputTypeDef](./type_defs.md#datasourceconfigoutputtypedef) 
7. See [:material-code-braces: VPCConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
8. See [:material-code-braces: ComputeTypeDef](./type_defs.md#computetypedef) 
## SimulationJobTypeDef

```python
# SimulationJobTypeDef definition

class SimulationJobTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[SimulationJobStatusType],  # (1)
    lastStartedAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    failureBehavior: NotRequired[FailureBehaviorType],  # (2)
    failureCode: NotRequired[SimulationJobErrorCodeType],  # (3)
    failureReason: NotRequired[str],
    clientRequestToken: NotRequired[str],
    outputLocation: NotRequired[OutputLocationTypeDef],  # (4)
    loggingConfig: NotRequired[LoggingConfigTypeDef],  # (5)
    maxJobDurationInSeconds: NotRequired[int],
    simulationTimeMillis: NotRequired[int],
    iamRole: NotRequired[str],
    robotApplications: NotRequired[List[RobotApplicationConfigOutputTypeDef]],  # (6)
    simulationApplications: NotRequired[List[SimulationApplicationConfigOutputTypeDef]],  # (7)
    dataSources: NotRequired[List[DataSourceTypeDef]],  # (8)
    tags: NotRequired[Dict[str, str]],
    vpcConfig: NotRequired[VPCConfigResponseTypeDef],  # (9)
    networkInterface: NotRequired[NetworkInterfaceTypeDef],  # (10)
    compute: NotRequired[ComputeResponseTypeDef],  # (11)
```

1. See [:material-code-brackets: SimulationJobStatusType](./literals.md#simulationjobstatustype) 
2. See [:material-code-brackets: FailureBehaviorType](./literals.md#failurebehaviortype) 
3. See [:material-code-brackets: SimulationJobErrorCodeType](./literals.md#simulationjoberrorcodetype) 
4. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
5. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
6. See [:material-code-braces: RobotApplicationConfigOutputTypeDef](./type_defs.md#robotapplicationconfigoutputtypedef) 
7. See [:material-code-braces: SimulationApplicationConfigOutputTypeDef](./type_defs.md#simulationapplicationconfigoutputtypedef) 
8. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
9. See [:material-code-braces: VPCConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef) 
10. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
11. See [:material-code-braces: ComputeResponseTypeDef](./type_defs.md#computeresponsetypedef) 
## FailedCreateSimulationJobRequestTypeDef

```python
# FailedCreateSimulationJobRequestTypeDef definition

class FailedCreateSimulationJobRequestTypeDef(TypedDict):
    request: NotRequired[SimulationJobRequestOutputTypeDef],  # (1)
    failureReason: NotRequired[str],
    failureCode: NotRequired[SimulationJobErrorCodeType],  # (2)
    failedAt: NotRequired[datetime],
```

1. See [:material-code-braces: SimulationJobRequestOutputTypeDef](./type_defs.md#simulationjobrequestoutputtypedef) 
2. See [:material-code-brackets: SimulationJobErrorCodeType](./literals.md#simulationjoberrorcodetype) 
## BatchDescribeSimulationJobResponseTypeDef

```python
# BatchDescribeSimulationJobResponseTypeDef definition

class BatchDescribeSimulationJobResponseTypeDef(TypedDict):
    jobs: List[SimulationJobTypeDef],  # (1)
    unprocessedJobs: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SimulationJobTypeDef](./type_defs.md#simulationjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RobotApplicationConfigTypeDef

```python
# RobotApplicationConfigTypeDef definition

class RobotApplicationConfigTypeDef(TypedDict):
    application: str,
    launchConfig: LaunchConfigUnionTypeDef,  # (1)
    applicationVersion: NotRequired[str],
    uploadConfigurations: NotRequired[Sequence[UploadConfigurationTypeDef]],  # (2)
    useDefaultUploadConfigurations: NotRequired[bool],
    tools: NotRequired[Sequence[ToolTypeDef]],  # (3)
    useDefaultTools: NotRequired[bool],
```

1. See [:material-code-braces: LaunchConfigTypeDef](./type_defs.md#launchconfigtypedef) [:material-code-braces: LaunchConfigOutputTypeDef](./type_defs.md#launchconfigoutputtypedef) 
2. See [:material-code-braces: UploadConfigurationTypeDef](./type_defs.md#uploadconfigurationtypedef) 
3. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
## SimulationApplicationConfigTypeDef

```python
# SimulationApplicationConfigTypeDef definition

class SimulationApplicationConfigTypeDef(TypedDict):
    application: str,
    launchConfig: LaunchConfigUnionTypeDef,  # (1)
    applicationVersion: NotRequired[str],
    uploadConfigurations: NotRequired[Sequence[UploadConfigurationTypeDef]],  # (2)
    worldConfigs: NotRequired[Sequence[WorldConfigTypeDef]],  # (3)
    useDefaultUploadConfigurations: NotRequired[bool],
    tools: NotRequired[Sequence[ToolTypeDef]],  # (4)
    useDefaultTools: NotRequired[bool],
```

1. See [:material-code-braces: LaunchConfigTypeDef](./type_defs.md#launchconfigtypedef) [:material-code-braces: LaunchConfigOutputTypeDef](./type_defs.md#launchconfigoutputtypedef) 
2. See [:material-code-braces: UploadConfigurationTypeDef](./type_defs.md#uploadconfigurationtypedef) 
3. See [:material-code-braces: WorldConfigTypeDef](./type_defs.md#worldconfigtypedef) 
4. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
## DescribeSimulationJobBatchResponseTypeDef

```python
# DescribeSimulationJobBatchResponseTypeDef definition

class DescribeSimulationJobBatchResponseTypeDef(TypedDict):
    arn: str,
    status: SimulationJobBatchStatusType,  # (1)
    lastUpdatedAt: datetime,
    createdAt: datetime,
    clientRequestToken: str,
    batchPolicy: BatchPolicyTypeDef,  # (2)
    failureCode: SimulationJobBatchErrorCodeType,  # (3)
    failureReason: str,
    failedRequests: List[FailedCreateSimulationJobRequestTypeDef],  # (4)
    pendingRequests: List[SimulationJobRequestOutputTypeDef],  # (5)
    createdRequests: List[SimulationJobSummaryTypeDef],  # (6)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: SimulationJobBatchStatusType](./literals.md#simulationjobbatchstatustype) 
2. See [:material-code-braces: BatchPolicyTypeDef](./type_defs.md#batchpolicytypedef) 
3. See [:material-code-brackets: SimulationJobBatchErrorCodeType](./literals.md#simulationjobbatcherrorcodetype) 
4. See [:material-code-braces: FailedCreateSimulationJobRequestTypeDef](./type_defs.md#failedcreatesimulationjobrequesttypedef) 
5. See [:material-code-braces: SimulationJobRequestOutputTypeDef](./type_defs.md#simulationjobrequestoutputtypedef) 
6. See [:material-code-braces: SimulationJobSummaryTypeDef](./type_defs.md#simulationjobsummarytypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSimulationJobBatchResponseTypeDef

```python
# StartSimulationJobBatchResponseTypeDef definition

class StartSimulationJobBatchResponseTypeDef(TypedDict):
    arn: str,
    status: SimulationJobBatchStatusType,  # (1)
    createdAt: datetime,
    clientRequestToken: str,
    batchPolicy: BatchPolicyTypeDef,  # (2)
    failureCode: SimulationJobBatchErrorCodeType,  # (3)
    failureReason: str,
    failedRequests: List[FailedCreateSimulationJobRequestTypeDef],  # (4)
    pendingRequests: List[SimulationJobRequestOutputTypeDef],  # (5)
    createdRequests: List[SimulationJobSummaryTypeDef],  # (6)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: SimulationJobBatchStatusType](./literals.md#simulationjobbatchstatustype) 
2. See [:material-code-braces: BatchPolicyTypeDef](./type_defs.md#batchpolicytypedef) 
3. See [:material-code-brackets: SimulationJobBatchErrorCodeType](./literals.md#simulationjobbatcherrorcodetype) 
4. See [:material-code-braces: FailedCreateSimulationJobRequestTypeDef](./type_defs.md#failedcreatesimulationjobrequesttypedef) 
5. See [:material-code-braces: SimulationJobRequestOutputTypeDef](./type_defs.md#simulationjobrequestoutputtypedef) 
6. See [:material-code-braces: SimulationJobSummaryTypeDef](./type_defs.md#simulationjobsummarytypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSimulationJobRequestRequestTypeDef

```python
# CreateSimulationJobRequestRequestTypeDef definition

class CreateSimulationJobRequestRequestTypeDef(TypedDict):
    maxJobDurationInSeconds: int,
    iamRole: str,
    clientRequestToken: NotRequired[str],
    outputLocation: NotRequired[OutputLocationTypeDef],  # (1)
    loggingConfig: NotRequired[LoggingConfigTypeDef],  # (2)
    failureBehavior: NotRequired[FailureBehaviorType],  # (3)
    robotApplications: NotRequired[Sequence[RobotApplicationConfigUnionTypeDef]],  # (4)
    simulationApplications: NotRequired[Sequence[SimulationApplicationConfigUnionTypeDef]],  # (5)
    dataSources: NotRequired[Sequence[DataSourceConfigUnionTypeDef]],  # (6)
    tags: NotRequired[Mapping[str, str]],
    vpcConfig: NotRequired[VPCConfigTypeDef],  # (7)
    compute: NotRequired[ComputeTypeDef],  # (8)
```

1. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
2. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
3. See [:material-code-brackets: FailureBehaviorType](./literals.md#failurebehaviortype) 
4. See [:material-code-braces: RobotApplicationConfigTypeDef](./type_defs.md#robotapplicationconfigtypedef) [:material-code-braces: RobotApplicationConfigOutputTypeDef](./type_defs.md#robotapplicationconfigoutputtypedef) 
5. See [:material-code-braces: SimulationApplicationConfigTypeDef](./type_defs.md#simulationapplicationconfigtypedef) [:material-code-braces: SimulationApplicationConfigOutputTypeDef](./type_defs.md#simulationapplicationconfigoutputtypedef) 
6. See [:material-code-braces: DataSourceConfigTypeDef](./type_defs.md#datasourceconfigtypedef) [:material-code-braces: DataSourceConfigOutputTypeDef](./type_defs.md#datasourceconfigoutputtypedef) 
7. See [:material-code-braces: VPCConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
8. See [:material-code-braces: ComputeTypeDef](./type_defs.md#computetypedef) 
## SimulationJobRequestTypeDef

```python
# SimulationJobRequestTypeDef definition

class SimulationJobRequestTypeDef(TypedDict):
    maxJobDurationInSeconds: int,
    outputLocation: NotRequired[OutputLocationTypeDef],  # (1)
    loggingConfig: NotRequired[LoggingConfigTypeDef],  # (2)
    iamRole: NotRequired[str],
    failureBehavior: NotRequired[FailureBehaviorType],  # (3)
    useDefaultApplications: NotRequired[bool],
    robotApplications: NotRequired[Sequence[RobotApplicationConfigUnionTypeDef]],  # (4)
    simulationApplications: NotRequired[Sequence[SimulationApplicationConfigUnionTypeDef]],  # (5)
    dataSources: NotRequired[Sequence[DataSourceConfigUnionTypeDef]],  # (6)
    vpcConfig: NotRequired[VPCConfigUnionTypeDef],  # (7)
    compute: NotRequired[ComputeTypeDef],  # (8)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: OutputLocationTypeDef](./type_defs.md#outputlocationtypedef) 
2. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
3. See [:material-code-brackets: FailureBehaviorType](./literals.md#failurebehaviortype) 
4. See [:material-code-braces: RobotApplicationConfigTypeDef](./type_defs.md#robotapplicationconfigtypedef) [:material-code-braces: RobotApplicationConfigOutputTypeDef](./type_defs.md#robotapplicationconfigoutputtypedef) 
5. See [:material-code-braces: SimulationApplicationConfigTypeDef](./type_defs.md#simulationapplicationconfigtypedef) [:material-code-braces: SimulationApplicationConfigOutputTypeDef](./type_defs.md#simulationapplicationconfigoutputtypedef) 
6. See [:material-code-braces: DataSourceConfigTypeDef](./type_defs.md#datasourceconfigtypedef) [:material-code-braces: DataSourceConfigOutputTypeDef](./type_defs.md#datasourceconfigoutputtypedef) 
7. See [:material-code-braces: VPCConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VPCConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
8. See [:material-code-braces: ComputeTypeDef](./type_defs.md#computetypedef) 
## StartSimulationJobBatchRequestRequestTypeDef

```python
# StartSimulationJobBatchRequestRequestTypeDef definition

class StartSimulationJobBatchRequestRequestTypeDef(TypedDict):
    createSimulationJobRequests: Sequence[SimulationJobRequestUnionTypeDef],  # (1)
    clientRequestToken: NotRequired[str],
    batchPolicy: NotRequired[BatchPolicyTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SimulationJobRequestTypeDef](./type_defs.md#simulationjobrequesttypedef) [:material-code-braces: SimulationJobRequestOutputTypeDef](./type_defs.md#simulationjobrequestoutputtypedef) 
2. See [:material-code-braces: BatchPolicyTypeDef](./type_defs.md#batchpolicytypedef) 
