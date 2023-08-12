# Type definitions

> [Index](../README.md) > [imagebuilder](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [imagebuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
    type annotations stubs module [types-aiobotocore-imagebuilder](https://pypi.org/project/types-aiobotocore-imagebuilder/).



## SeverityCountsTypeDef

```python
# SeverityCountsTypeDef definition

class SeverityCountsTypeDef(TypedDict):
    all: NotRequired[int],
    critical: NotRequired[int],
    high: NotRequired[int],
    medium: NotRequired[int],
```

## SystemsManagerAgentTypeDef

```python
# SystemsManagerAgentTypeDef definition

class SystemsManagerAgentTypeDef(TypedDict):
    uninstallAfterBuild: NotRequired[bool],
```

## LaunchPermissionConfigurationTypeDef

```python
# LaunchPermissionConfigurationTypeDef definition

class LaunchPermissionConfigurationTypeDef(TypedDict):
    userIds: NotRequired[Sequence[str]],
    userGroups: NotRequired[Sequence[str]],
    organizationArns: NotRequired[Sequence[str]],
    organizationalUnitArns: NotRequired[Sequence[str]],
```

## ImageStateTypeDef

```python
# ImageStateTypeDef definition

class ImageStateTypeDef(TypedDict):
    status: NotRequired[ImageStatusType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: ImageStatusType](./literals.md#imagestatustype) 
## CancelImageCreationRequestRequestTypeDef

```python
# CancelImageCreationRequestRequestTypeDef definition

class CancelImageCreationRequestRequestTypeDef(TypedDict):
    imageBuildVersionArn: str,
    clientToken: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## ComponentParameterTypeDef

```python
# ComponentParameterTypeDef definition

class ComponentParameterTypeDef(TypedDict):
    name: str,
    value: Sequence[str],
```

## ComponentParameterDetailTypeDef

```python
# ComponentParameterDetailTypeDef definition

class ComponentParameterDetailTypeDef(TypedDict):
    name: str,
    type: str,
    defaultValue: NotRequired[List[str]],
    description: NotRequired[str],
```

## ComponentStateTypeDef

```python
# ComponentStateTypeDef definition

class ComponentStateTypeDef(TypedDict):
    status: NotRequired[ComponentStatusType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: ComponentStatusType](./literals.md#componentstatustype) 
## ComponentVersionTypeDef

```python
# ComponentVersionTypeDef definition

class ComponentVersionTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    version: NotRequired[str],
    description: NotRequired[str],
    platform: NotRequired[PlatformType],  # (1)
    supportedOsVersions: NotRequired[List[str]],
    type: NotRequired[ComponentTypeType],  # (2)
    owner: NotRequired[str],
    dateCreated: NotRequired[str],
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-brackets: ComponentTypeType](./literals.md#componenttypetype) 
## TargetContainerRepositoryTypeDef

```python
# TargetContainerRepositoryTypeDef definition

class TargetContainerRepositoryTypeDef(TypedDict):
    service: ContainerRepositoryServiceType,  # (1)
    repositoryName: str,
```

1. See [:material-code-brackets: ContainerRepositoryServiceType](./literals.md#containerrepositoryservicetype) 
## ContainerRecipeSummaryTypeDef

```python
# ContainerRecipeSummaryTypeDef definition

class ContainerRecipeSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    containerType: NotRequired[ContainerTypeType],  # (1)
    name: NotRequired[str],
    platform: NotRequired[PlatformType],  # (2)
    owner: NotRequired[str],
    parentImage: NotRequired[str],
    dateCreated: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## ContainerTypeDef

```python
# ContainerTypeDef definition

class ContainerTypeDef(TypedDict):
    region: NotRequired[str],
    imageUris: NotRequired[List[str]],
```

## CreateComponentRequestRequestTypeDef

```python
# CreateComponentRequestRequestTypeDef definition

class CreateComponentRequestRequestTypeDef(TypedDict):
    name: str,
    semanticVersion: str,
    platform: PlatformType,  # (1)
    clientToken: str,
    description: NotRequired[str],
    changeDescription: NotRequired[str],
    supportedOsVersions: NotRequired[Sequence[str]],
    data: NotRequired[str],
    uri: NotRequired[str],
    kmsKeyId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## ImageTestsConfigurationTypeDef

```python
# ImageTestsConfigurationTypeDef definition

class ImageTestsConfigurationTypeDef(TypedDict):
    imageTestsEnabled: NotRequired[bool],
    timeoutMinutes: NotRequired[int],
```

## ScheduleTypeDef

```python
# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    scheduleExpression: NotRequired[str],
    timezone: NotRequired[str],
    pipelineExecutionStartCondition: NotRequired[PipelineExecutionStartConditionType],  # (1)
```

1. See [:material-code-brackets: PipelineExecutionStartConditionType](./literals.md#pipelineexecutionstartconditiontype) 
## InstanceMetadataOptionsTypeDef

```python
# InstanceMetadataOptionsTypeDef definition

class InstanceMetadataOptionsTypeDef(TypedDict):
    httpTokens: NotRequired[str],
    httpPutResponseHopLimit: NotRequired[int],
```

## CvssScoreAdjustmentTypeDef

```python
# CvssScoreAdjustmentTypeDef definition

class CvssScoreAdjustmentTypeDef(TypedDict):
    metric: NotRequired[str],
    reason: NotRequired[str],
```

## CvssScoreTypeDef

```python
# CvssScoreTypeDef definition

class CvssScoreTypeDef(TypedDict):
    baseScore: NotRequired[float],
    scoringVector: NotRequired[str],
    version: NotRequired[str],
    source: NotRequired[str],
```

## DeleteComponentRequestRequestTypeDef

```python
# DeleteComponentRequestRequestTypeDef definition

class DeleteComponentRequestRequestTypeDef(TypedDict):
    componentBuildVersionArn: str,
```

## DeleteContainerRecipeRequestRequestTypeDef

```python
# DeleteContainerRecipeRequestRequestTypeDef definition

class DeleteContainerRecipeRequestRequestTypeDef(TypedDict):
    containerRecipeArn: str,
```

## DeleteDistributionConfigurationRequestRequestTypeDef

```python
# DeleteDistributionConfigurationRequestRequestTypeDef definition

class DeleteDistributionConfigurationRequestRequestTypeDef(TypedDict):
    distributionConfigurationArn: str,
```

## DeleteImagePipelineRequestRequestTypeDef

```python
# DeleteImagePipelineRequestRequestTypeDef definition

class DeleteImagePipelineRequestRequestTypeDef(TypedDict):
    imagePipelineArn: str,
```

## DeleteImageRecipeRequestRequestTypeDef

```python
# DeleteImageRecipeRequestRequestTypeDef definition

class DeleteImageRecipeRequestRequestTypeDef(TypedDict):
    imageRecipeArn: str,
```

## DeleteImageRequestRequestTypeDef

```python
# DeleteImageRequestRequestTypeDef definition

class DeleteImageRequestRequestTypeDef(TypedDict):
    imageBuildVersionArn: str,
```

## DeleteInfrastructureConfigurationRequestRequestTypeDef

```python
# DeleteInfrastructureConfigurationRequestRequestTypeDef definition

class DeleteInfrastructureConfigurationRequestRequestTypeDef(TypedDict):
    infrastructureConfigurationArn: str,
```

## DistributionConfigurationSummaryTypeDef

```python
# DistributionConfigurationSummaryTypeDef definition

class DistributionConfigurationSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    dateCreated: NotRequired[str],
    dateUpdated: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    regions: NotRequired[List[str]],
```

## LaunchTemplateConfigurationTypeDef

```python
# LaunchTemplateConfigurationTypeDef definition

class LaunchTemplateConfigurationTypeDef(TypedDict):
    launchTemplateId: str,
    accountId: NotRequired[str],
    setDefaultVersion: NotRequired[bool],
```

## S3ExportConfigurationTypeDef

```python
# S3ExportConfigurationTypeDef definition

class S3ExportConfigurationTypeDef(TypedDict):
    roleName: str,
    diskImageFormat: DiskImageFormatType,  # (1)
    s3Bucket: str,
    s3Prefix: NotRequired[str],
```

1. See [:material-code-brackets: DiskImageFormatType](./literals.md#diskimageformattype) 
## EbsInstanceBlockDeviceSpecificationTypeDef

```python
# EbsInstanceBlockDeviceSpecificationTypeDef definition

class EbsInstanceBlockDeviceSpecificationTypeDef(TypedDict):
    encrypted: NotRequired[bool],
    deleteOnTermination: NotRequired[bool],
    iops: NotRequired[int],
    kmsKeyId: NotRequired[str],
    snapshotId: NotRequired[str],
    volumeSize: NotRequired[int],
    volumeType: NotRequired[EbsVolumeTypeType],  # (1)
    throughput: NotRequired[int],
```

1. See [:material-code-brackets: EbsVolumeTypeType](./literals.md#ebsvolumetypetype) 
## EcrConfigurationTypeDef

```python
# EcrConfigurationTypeDef definition

class EcrConfigurationTypeDef(TypedDict):
    repositoryName: NotRequired[str],
    containerTags: NotRequired[Sequence[str]],
```

## FastLaunchLaunchTemplateSpecificationTypeDef

```python
# FastLaunchLaunchTemplateSpecificationTypeDef definition

class FastLaunchLaunchTemplateSpecificationTypeDef(TypedDict):
    launchTemplateId: NotRequired[str],
    launchTemplateName: NotRequired[str],
    launchTemplateVersion: NotRequired[str],
```

## FastLaunchSnapshotConfigurationTypeDef

```python
# FastLaunchSnapshotConfigurationTypeDef definition

class FastLaunchSnapshotConfigurationTypeDef(TypedDict):
    targetResourceCount: NotRequired[int],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    name: NotRequired[str],
    values: NotRequired[Sequence[str]],
```

## GetComponentPolicyRequestRequestTypeDef

```python
# GetComponentPolicyRequestRequestTypeDef definition

class GetComponentPolicyRequestRequestTypeDef(TypedDict):
    componentArn: str,
```

## GetComponentRequestRequestTypeDef

```python
# GetComponentRequestRequestTypeDef definition

class GetComponentRequestRequestTypeDef(TypedDict):
    componentBuildVersionArn: str,
```

## GetContainerRecipePolicyRequestRequestTypeDef

```python
# GetContainerRecipePolicyRequestRequestTypeDef definition

class GetContainerRecipePolicyRequestRequestTypeDef(TypedDict):
    containerRecipeArn: str,
```

## GetContainerRecipeRequestRequestTypeDef

```python
# GetContainerRecipeRequestRequestTypeDef definition

class GetContainerRecipeRequestRequestTypeDef(TypedDict):
    containerRecipeArn: str,
```

## GetDistributionConfigurationRequestRequestTypeDef

```python
# GetDistributionConfigurationRequestRequestTypeDef definition

class GetDistributionConfigurationRequestRequestTypeDef(TypedDict):
    distributionConfigurationArn: str,
```

## GetImagePipelineRequestRequestTypeDef

```python
# GetImagePipelineRequestRequestTypeDef definition

class GetImagePipelineRequestRequestTypeDef(TypedDict):
    imagePipelineArn: str,
```

## GetImagePolicyRequestRequestTypeDef

```python
# GetImagePolicyRequestRequestTypeDef definition

class GetImagePolicyRequestRequestTypeDef(TypedDict):
    imageArn: str,
```

## GetImageRecipePolicyRequestRequestTypeDef

```python
# GetImageRecipePolicyRequestRequestTypeDef definition

class GetImageRecipePolicyRequestRequestTypeDef(TypedDict):
    imageRecipeArn: str,
```

## GetImageRecipeRequestRequestTypeDef

```python
# GetImageRecipeRequestRequestTypeDef definition

class GetImageRecipeRequestRequestTypeDef(TypedDict):
    imageRecipeArn: str,
```

## GetImageRequestRequestTypeDef

```python
# GetImageRequestRequestTypeDef definition

class GetImageRequestRequestTypeDef(TypedDict):
    imageBuildVersionArn: str,
```

## GetInfrastructureConfigurationRequestRequestTypeDef

```python
# GetInfrastructureConfigurationRequestRequestTypeDef definition

class GetInfrastructureConfigurationRequestRequestTypeDef(TypedDict):
    infrastructureConfigurationArn: str,
```

## GetWorkflowExecutionRequestRequestTypeDef

```python
# GetWorkflowExecutionRequestRequestTypeDef definition

class GetWorkflowExecutionRequestRequestTypeDef(TypedDict):
    workflowExecutionId: str,
```

## GetWorkflowStepExecutionRequestRequestTypeDef

```python
# GetWorkflowStepExecutionRequestRequestTypeDef definition

class GetWorkflowStepExecutionRequestRequestTypeDef(TypedDict):
    stepExecutionId: str,
```

## ImagePackageTypeDef

```python
# ImagePackageTypeDef definition

class ImagePackageTypeDef(TypedDict):
    packageName: NotRequired[str],
    packageVersion: NotRequired[str],
```

## ImageRecipeSummaryTypeDef

```python
# ImageRecipeSummaryTypeDef definition

class ImageRecipeSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    platform: NotRequired[PlatformType],  # (1)
    owner: NotRequired[str],
    parentImage: NotRequired[str],
    dateCreated: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## ImageScanFindingsFilterTypeDef

```python
# ImageScanFindingsFilterTypeDef definition

class ImageScanFindingsFilterTypeDef(TypedDict):
    name: NotRequired[str],
    values: NotRequired[Sequence[str]],
```

## ImageScanStateTypeDef

```python
# ImageScanStateTypeDef definition

class ImageScanStateTypeDef(TypedDict):
    status: NotRequired[ImageScanStatusType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: ImageScanStatusType](./literals.md#imagescanstatustype) 
## ImageVersionTypeDef

```python
# ImageVersionTypeDef definition

class ImageVersionTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[ImageTypeType],  # (1)
    version: NotRequired[str],
    platform: NotRequired[PlatformType],  # (2)
    osVersion: NotRequired[str],
    owner: NotRequired[str],
    dateCreated: NotRequired[str],
    buildType: NotRequired[BuildTypeType],  # (3)
    imageSource: NotRequired[ImageSourceType],  # (4)
```

1. See [:material-code-brackets: ImageTypeType](./literals.md#imagetypetype) 
2. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
3. See [:material-code-brackets: BuildTypeType](./literals.md#buildtypetype) 
4. See [:material-code-brackets: ImageSourceType](./literals.md#imagesourcetype) 
## ImportComponentRequestRequestTypeDef

```python
# ImportComponentRequestRequestTypeDef definition

class ImportComponentRequestRequestTypeDef(TypedDict):
    name: str,
    semanticVersion: str,
    type: ComponentTypeType,  # (1)
    format: ComponentFormatType,  # (2)
    platform: PlatformType,  # (3)
    clientToken: str,
    description: NotRequired[str],
    changeDescription: NotRequired[str],
    data: NotRequired[str],
    uri: NotRequired[str],
    kmsKeyId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ComponentTypeType](./literals.md#componenttypetype) 
2. See [:material-code-brackets: ComponentFormatType](./literals.md#componentformattype) 
3. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## ImportVmImageRequestRequestTypeDef

```python
# ImportVmImageRequestRequestTypeDef definition

class ImportVmImageRequestRequestTypeDef(TypedDict):
    name: str,
    semanticVersion: str,
    platform: PlatformType,  # (1)
    vmImportTaskId: str,
    clientToken: str,
    description: NotRequired[str],
    osVersion: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## InfrastructureConfigurationSummaryTypeDef

```python
# InfrastructureConfigurationSummaryTypeDef definition

class InfrastructureConfigurationSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    dateCreated: NotRequired[str],
    dateUpdated: NotRequired[str],
    resourceTags: NotRequired[Dict[str, str]],
    tags: NotRequired[Dict[str, str]],
    instanceTypes: NotRequired[List[str]],
    instanceProfileName: NotRequired[str],
```

## ListComponentBuildVersionsRequestRequestTypeDef

```python
# ListComponentBuildVersionsRequestRequestTypeDef definition

class ListComponentBuildVersionsRequestRequestTypeDef(TypedDict):
    componentVersionArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListImagePackagesRequestRequestTypeDef

```python
# ListImagePackagesRequestRequestTypeDef definition

class ListImagePackagesRequestRequestTypeDef(TypedDict):
    imageBuildVersionArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListWorkflowExecutionsRequestRequestTypeDef

```python
# ListWorkflowExecutionsRequestRequestTypeDef definition

class ListWorkflowExecutionsRequestRequestTypeDef(TypedDict):
    imageBuildVersionArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## WorkflowExecutionMetadataTypeDef

```python
# WorkflowExecutionMetadataTypeDef definition

class WorkflowExecutionMetadataTypeDef(TypedDict):
    workflowBuildVersionArn: NotRequired[str],
    workflowExecutionId: NotRequired[str],
    type: NotRequired[WorkflowTypeType],  # (1)
    status: NotRequired[WorkflowExecutionStatusType],  # (2)
    message: NotRequired[str],
    totalStepCount: NotRequired[int],
    totalStepsSucceeded: NotRequired[int],
    totalStepsFailed: NotRequired[int],
    totalStepsSkipped: NotRequired[int],
    startTime: NotRequired[str],
    endTime: NotRequired[str],
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: WorkflowExecutionStatusType](./literals.md#workflowexecutionstatustype) 
## ListWorkflowStepExecutionsRequestRequestTypeDef

```python
# ListWorkflowStepExecutionsRequestRequestTypeDef definition

class ListWorkflowStepExecutionsRequestRequestTypeDef(TypedDict):
    workflowExecutionId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## WorkflowStepMetadataTypeDef

```python
# WorkflowStepMetadataTypeDef definition

class WorkflowStepMetadataTypeDef(TypedDict):
    stepExecutionId: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    action: NotRequired[str],
    status: NotRequired[WorkflowStepExecutionStatusType],  # (1)
    rollbackStatus: NotRequired[WorkflowStepExecutionRollbackStatusType],  # (2)
    message: NotRequired[str],
    inputs: NotRequired[str],
    outputs: NotRequired[str],
    startTime: NotRequired[str],
    endTime: NotRequired[str],
```

1. See [:material-code-brackets: WorkflowStepExecutionStatusType](./literals.md#workflowstepexecutionstatustype) 
2. See [:material-code-brackets: WorkflowStepExecutionRollbackStatusType](./literals.md#workflowstepexecutionrollbackstatustype) 
## S3LogsTypeDef

```python
# S3LogsTypeDef definition

class S3LogsTypeDef(TypedDict):
    s3BucketName: NotRequired[str],
    s3KeyPrefix: NotRequired[str],
```

## VulnerablePackageTypeDef

```python
# VulnerablePackageTypeDef definition

class VulnerablePackageTypeDef(TypedDict):
    name: NotRequired[str],
    version: NotRequired[str],
    sourceLayerHash: NotRequired[str],
    epoch: NotRequired[int],
    release: NotRequired[str],
    arch: NotRequired[str],
    packageManager: NotRequired[str],
    filePath: NotRequired[str],
    fixedInVersion: NotRequired[str],
    remediation: NotRequired[str],
```

## PutComponentPolicyRequestRequestTypeDef

```python
# PutComponentPolicyRequestRequestTypeDef definition

class PutComponentPolicyRequestRequestTypeDef(TypedDict):
    componentArn: str,
    policy: str,
```

## PutContainerRecipePolicyRequestRequestTypeDef

```python
# PutContainerRecipePolicyRequestRequestTypeDef definition

class PutContainerRecipePolicyRequestRequestTypeDef(TypedDict):
    containerRecipeArn: str,
    policy: str,
```

## PutImagePolicyRequestRequestTypeDef

```python
# PutImagePolicyRequestRequestTypeDef definition

class PutImagePolicyRequestRequestTypeDef(TypedDict):
    imageArn: str,
    policy: str,
```

## PutImageRecipePolicyRequestRequestTypeDef

```python
# PutImageRecipePolicyRequestRequestTypeDef definition

class PutImageRecipePolicyRequestRequestTypeDef(TypedDict):
    imageRecipeArn: str,
    policy: str,
```

## RemediationRecommendationTypeDef

```python
# RemediationRecommendationTypeDef definition

class RemediationRecommendationTypeDef(TypedDict):
    text: NotRequired[str],
    url: NotRequired[str],
```

## StartImagePipelineExecutionRequestRequestTypeDef

```python
# StartImagePipelineExecutionRequestRequestTypeDef definition

class StartImagePipelineExecutionRequestRequestTypeDef(TypedDict):
    imagePipelineArn: str,
    clientToken: str,
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

## AccountAggregationTypeDef

```python
# AccountAggregationTypeDef definition

class AccountAggregationTypeDef(TypedDict):
    accountId: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## ImageAggregationTypeDef

```python
# ImageAggregationTypeDef definition

class ImageAggregationTypeDef(TypedDict):
    imageBuildVersionArn: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## ImagePipelineAggregationTypeDef

```python
# ImagePipelineAggregationTypeDef definition

class ImagePipelineAggregationTypeDef(TypedDict):
    imagePipelineArn: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## VulnerabilityIdAggregationTypeDef

```python
# VulnerabilityIdAggregationTypeDef definition

class VulnerabilityIdAggregationTypeDef(TypedDict):
    vulnerabilityId: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## AdditionalInstanceConfigurationTypeDef

```python
# AdditionalInstanceConfigurationTypeDef definition

class AdditionalInstanceConfigurationTypeDef(TypedDict):
    systemsManagerAgent: NotRequired[SystemsManagerAgentTypeDef],  # (1)
    userDataOverride: NotRequired[str],
```

1. See [:material-code-braces: SystemsManagerAgentTypeDef](./type_defs.md#systemsmanageragenttypedef) 
## AmiDistributionConfigurationTypeDef

```python
# AmiDistributionConfigurationTypeDef definition

class AmiDistributionConfigurationTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    targetAccountIds: NotRequired[Sequence[str]],
    amiTags: NotRequired[Mapping[str, str]],
    kmsKeyId: NotRequired[str],
    launchPermission: NotRequired[LaunchPermissionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: LaunchPermissionConfigurationTypeDef](./type_defs.md#launchpermissionconfigurationtypedef) 
## AmiTypeDef

```python
# AmiTypeDef definition

class AmiTypeDef(TypedDict):
    region: NotRequired[str],
    image: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    state: NotRequired[ImageStateTypeDef],  # (1)
    accountId: NotRequired[str],
```

1. See [:material-code-braces: ImageStateTypeDef](./type_defs.md#imagestatetypedef) 
## CancelImageCreationResponseTypeDef

```python
# CancelImageCreationResponseTypeDef definition

class CancelImageCreationResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    imageBuildVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateComponentResponseTypeDef

```python
# CreateComponentResponseTypeDef definition

class CreateComponentResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    componentBuildVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContainerRecipeResponseTypeDef

```python
# CreateContainerRecipeResponseTypeDef definition

class CreateContainerRecipeResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    containerRecipeArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDistributionConfigurationResponseTypeDef

```python
# CreateDistributionConfigurationResponseTypeDef definition

class CreateDistributionConfigurationResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    distributionConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateImagePipelineResponseTypeDef

```python
# CreateImagePipelineResponseTypeDef definition

class CreateImagePipelineResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    imagePipelineArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateImageRecipeResponseTypeDef

```python
# CreateImageRecipeResponseTypeDef definition

class CreateImageRecipeResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    imageRecipeArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateImageResponseTypeDef

```python
# CreateImageResponseTypeDef definition

class CreateImageResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    imageBuildVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInfrastructureConfigurationResponseTypeDef

```python
# CreateInfrastructureConfigurationResponseTypeDef definition

class CreateInfrastructureConfigurationResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    infrastructureConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteComponentResponseTypeDef

```python
# DeleteComponentResponseTypeDef definition

class DeleteComponentResponseTypeDef(TypedDict):
    requestId: str,
    componentBuildVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteContainerRecipeResponseTypeDef

```python
# DeleteContainerRecipeResponseTypeDef definition

class DeleteContainerRecipeResponseTypeDef(TypedDict):
    requestId: str,
    containerRecipeArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDistributionConfigurationResponseTypeDef

```python
# DeleteDistributionConfigurationResponseTypeDef definition

class DeleteDistributionConfigurationResponseTypeDef(TypedDict):
    requestId: str,
    distributionConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteImagePipelineResponseTypeDef

```python
# DeleteImagePipelineResponseTypeDef definition

class DeleteImagePipelineResponseTypeDef(TypedDict):
    requestId: str,
    imagePipelineArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteImageRecipeResponseTypeDef

```python
# DeleteImageRecipeResponseTypeDef definition

class DeleteImageRecipeResponseTypeDef(TypedDict):
    requestId: str,
    imageRecipeArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteImageResponseTypeDef

```python
# DeleteImageResponseTypeDef definition

class DeleteImageResponseTypeDef(TypedDict):
    requestId: str,
    imageBuildVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInfrastructureConfigurationResponseTypeDef

```python
# DeleteInfrastructureConfigurationResponseTypeDef definition

class DeleteInfrastructureConfigurationResponseTypeDef(TypedDict):
    requestId: str,
    infrastructureConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComponentPolicyResponseTypeDef

```python
# GetComponentPolicyResponseTypeDef definition

class GetComponentPolicyResponseTypeDef(TypedDict):
    requestId: str,
    policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContainerRecipePolicyResponseTypeDef

```python
# GetContainerRecipePolicyResponseTypeDef definition

class GetContainerRecipePolicyResponseTypeDef(TypedDict):
    requestId: str,
    policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImagePolicyResponseTypeDef

```python
# GetImagePolicyResponseTypeDef definition

class GetImagePolicyResponseTypeDef(TypedDict):
    requestId: str,
    policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImageRecipePolicyResponseTypeDef

```python
# GetImageRecipePolicyResponseTypeDef definition

class GetImageRecipePolicyResponseTypeDef(TypedDict):
    requestId: str,
    policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowExecutionResponseTypeDef

```python
# GetWorkflowExecutionResponseTypeDef definition

class GetWorkflowExecutionResponseTypeDef(TypedDict):
    requestId: str,
    workflowBuildVersionArn: str,
    workflowExecutionId: str,
    imageBuildVersionArn: str,
    type: WorkflowTypeType,  # (1)
    status: WorkflowExecutionStatusType,  # (2)
    message: str,
    totalStepCount: int,
    totalStepsSucceeded: int,
    totalStepsFailed: int,
    totalStepsSkipped: int,
    startTime: str,
    endTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-brackets: WorkflowExecutionStatusType](./literals.md#workflowexecutionstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowStepExecutionResponseTypeDef

```python
# GetWorkflowStepExecutionResponseTypeDef definition

class GetWorkflowStepExecutionResponseTypeDef(TypedDict):
    requestId: str,
    stepExecutionId: str,
    workflowBuildVersionArn: str,
    workflowExecutionId: str,
    imageBuildVersionArn: str,
    name: str,
    description: str,
    action: str,
    status: WorkflowStepExecutionStatusType,  # (1)
    rollbackStatus: WorkflowStepExecutionRollbackStatusType,  # (2)
    message: str,
    inputs: str,
    outputs: str,
    startTime: str,
    endTime: str,
    onFailure: str,
    timeoutSeconds: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: WorkflowStepExecutionStatusType](./literals.md#workflowstepexecutionstatustype) 
2. See [:material-code-brackets: WorkflowStepExecutionRollbackStatusType](./literals.md#workflowstepexecutionrollbackstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportComponentResponseTypeDef

```python
# ImportComponentResponseTypeDef definition

class ImportComponentResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    componentBuildVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportVmImageResponseTypeDef

```python
# ImportVmImageResponseTypeDef definition

class ImportVmImageResponseTypeDef(TypedDict):
    requestId: str,
    imageArn: str,
    clientToken: str,
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
## PutComponentPolicyResponseTypeDef

```python
# PutComponentPolicyResponseTypeDef definition

class PutComponentPolicyResponseTypeDef(TypedDict):
    requestId: str,
    componentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutContainerRecipePolicyResponseTypeDef

```python
# PutContainerRecipePolicyResponseTypeDef definition

class PutContainerRecipePolicyResponseTypeDef(TypedDict):
    requestId: str,
    containerRecipeArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutImagePolicyResponseTypeDef

```python
# PutImagePolicyResponseTypeDef definition

class PutImagePolicyResponseTypeDef(TypedDict):
    requestId: str,
    imageArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutImageRecipePolicyResponseTypeDef

```python
# PutImageRecipePolicyResponseTypeDef definition

class PutImageRecipePolicyResponseTypeDef(TypedDict):
    requestId: str,
    imageRecipeArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImagePipelineExecutionResponseTypeDef

```python
# StartImagePipelineExecutionResponseTypeDef definition

class StartImagePipelineExecutionResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    imageBuildVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDistributionConfigurationResponseTypeDef

```python
# UpdateDistributionConfigurationResponseTypeDef definition

class UpdateDistributionConfigurationResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    distributionConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateImagePipelineResponseTypeDef

```python
# UpdateImagePipelineResponseTypeDef definition

class UpdateImagePipelineResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    imagePipelineArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInfrastructureConfigurationResponseTypeDef

```python
# UpdateInfrastructureConfigurationResponseTypeDef definition

class UpdateInfrastructureConfigurationResponseTypeDef(TypedDict):
    requestId: str,
    clientToken: str,
    infrastructureConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ComponentConfigurationTypeDef

```python
# ComponentConfigurationTypeDef definition

class ComponentConfigurationTypeDef(TypedDict):
    componentArn: str,
    parameters: NotRequired[Sequence[ComponentParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ComponentParameterTypeDef](./type_defs.md#componentparametertypedef) 
## ComponentSummaryTypeDef

```python
# ComponentSummaryTypeDef definition

class ComponentSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    version: NotRequired[str],
    platform: NotRequired[PlatformType],  # (1)
    supportedOsVersions: NotRequired[List[str]],
    state: NotRequired[ComponentStateTypeDef],  # (2)
    type: NotRequired[ComponentTypeType],  # (3)
    owner: NotRequired[str],
    description: NotRequired[str],
    changeDescription: NotRequired[str],
    dateCreated: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    publisher: NotRequired[str],
    obfuscate: NotRequired[bool],
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: ComponentStateTypeDef](./type_defs.md#componentstatetypedef) 
3. See [:material-code-brackets: ComponentTypeType](./literals.md#componenttypetype) 
## ComponentTypeDef

```python
# ComponentTypeDef definition

class ComponentTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    version: NotRequired[str],
    description: NotRequired[str],
    changeDescription: NotRequired[str],
    type: NotRequired[ComponentTypeType],  # (1)
    platform: NotRequired[PlatformType],  # (2)
    supportedOsVersions: NotRequired[List[str]],
    state: NotRequired[ComponentStateTypeDef],  # (3)
    parameters: NotRequired[List[ComponentParameterDetailTypeDef]],  # (4)
    owner: NotRequired[str],
    data: NotRequired[str],
    kmsKeyId: NotRequired[str],
    encrypted: NotRequired[bool],
    dateCreated: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    publisher: NotRequired[str],
    obfuscate: NotRequired[bool],
```

1. See [:material-code-brackets: ComponentTypeType](./literals.md#componenttypetype) 
2. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
3. See [:material-code-braces: ComponentStateTypeDef](./type_defs.md#componentstatetypedef) 
4. See [:material-code-braces: ComponentParameterDetailTypeDef](./type_defs.md#componentparameterdetailtypedef) 
## ListComponentsResponseTypeDef

```python
# ListComponentsResponseTypeDef definition

class ListComponentsResponseTypeDef(TypedDict):
    requestId: str,
    componentVersionList: List[ComponentVersionTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentVersionTypeDef](./type_defs.md#componentversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContainerDistributionConfigurationTypeDef

```python
# ContainerDistributionConfigurationTypeDef definition

class ContainerDistributionConfigurationTypeDef(TypedDict):
    targetRepository: TargetContainerRepositoryTypeDef,  # (1)
    description: NotRequired[str],
    containerTags: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TargetContainerRepositoryTypeDef](./type_defs.md#targetcontainerrepositorytypedef) 
## ListContainerRecipesResponseTypeDef

```python
# ListContainerRecipesResponseTypeDef definition

class ListContainerRecipesResponseTypeDef(TypedDict):
    requestId: str,
    containerRecipeSummaryList: List[ContainerRecipeSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerRecipeSummaryTypeDef](./type_defs.md#containerrecipesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CvssScoreDetailsTypeDef

```python
# CvssScoreDetailsTypeDef definition

class CvssScoreDetailsTypeDef(TypedDict):
    scoreSource: NotRequired[str],
    cvssSource: NotRequired[str],
    version: NotRequired[str],
    score: NotRequired[float],
    scoringVector: NotRequired[str],
    adjustments: NotRequired[List[CvssScoreAdjustmentTypeDef]],  # (1)
```

1. See [:material-code-braces: CvssScoreAdjustmentTypeDef](./type_defs.md#cvssscoreadjustmenttypedef) 
## ListDistributionConfigurationsResponseTypeDef

```python
# ListDistributionConfigurationsResponseTypeDef definition

class ListDistributionConfigurationsResponseTypeDef(TypedDict):
    requestId: str,
    distributionConfigurationSummaryList: List[DistributionConfigurationSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionConfigurationSummaryTypeDef](./type_defs.md#distributionconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceBlockDeviceMappingTypeDef

```python
# InstanceBlockDeviceMappingTypeDef definition

class InstanceBlockDeviceMappingTypeDef(TypedDict):
    deviceName: NotRequired[str],
    ebs: NotRequired[EbsInstanceBlockDeviceSpecificationTypeDef],  # (1)
    virtualName: NotRequired[str],
    noDevice: NotRequired[str],
```

1. See [:material-code-braces: EbsInstanceBlockDeviceSpecificationTypeDef](./type_defs.md#ebsinstanceblockdevicespecificationtypedef) 
## ImageScanningConfigurationTypeDef

```python
# ImageScanningConfigurationTypeDef definition

class ImageScanningConfigurationTypeDef(TypedDict):
    imageScanningEnabled: NotRequired[bool],
    ecrConfiguration: NotRequired[EcrConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EcrConfigurationTypeDef](./type_defs.md#ecrconfigurationtypedef) 
## FastLaunchConfigurationTypeDef

```python
# FastLaunchConfigurationTypeDef definition

class FastLaunchConfigurationTypeDef(TypedDict):
    enabled: bool,
    snapshotConfiguration: NotRequired[FastLaunchSnapshotConfigurationTypeDef],  # (1)
    maxParallelLaunches: NotRequired[int],
    launchTemplate: NotRequired[FastLaunchLaunchTemplateSpecificationTypeDef],  # (2)
    accountId: NotRequired[str],
```

1. See [:material-code-braces: FastLaunchSnapshotConfigurationTypeDef](./type_defs.md#fastlaunchsnapshotconfigurationtypedef) 
2. See [:material-code-braces: FastLaunchLaunchTemplateSpecificationTypeDef](./type_defs.md#fastlaunchlaunchtemplatespecificationtypedef) 
## ListComponentsRequestRequestTypeDef

```python
# ListComponentsRequestRequestTypeDef definition

class ListComponentsRequestRequestTypeDef(TypedDict):
    owner: NotRequired[OwnershipType],  # (1)
    filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    byName: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListContainerRecipesRequestRequestTypeDef

```python
# ListContainerRecipesRequestRequestTypeDef definition

class ListContainerRecipesRequestRequestTypeDef(TypedDict):
    owner: NotRequired[OwnershipType],  # (1)
    filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListDistributionConfigurationsRequestRequestTypeDef

```python
# ListDistributionConfigurationsRequestRequestTypeDef definition

class ListDistributionConfigurationsRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListImageBuildVersionsRequestRequestTypeDef

```python
# ListImageBuildVersionsRequestRequestTypeDef definition

class ListImageBuildVersionsRequestRequestTypeDef(TypedDict):
    imageVersionArn: str,
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListImagePipelineImagesRequestRequestTypeDef

```python
# ListImagePipelineImagesRequestRequestTypeDef definition

class ListImagePipelineImagesRequestRequestTypeDef(TypedDict):
    imagePipelineArn: str,
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListImagePipelinesRequestRequestTypeDef

```python
# ListImagePipelinesRequestRequestTypeDef definition

class ListImagePipelinesRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListImageRecipesRequestRequestTypeDef

```python
# ListImageRecipesRequestRequestTypeDef definition

class ListImageRecipesRequestRequestTypeDef(TypedDict):
    owner: NotRequired[OwnershipType],  # (1)
    filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListImageScanFindingAggregationsRequestRequestTypeDef

```python
# ListImageScanFindingAggregationsRequestRequestTypeDef definition

class ListImageScanFindingAggregationsRequestRequestTypeDef(TypedDict):
    filter: NotRequired[FilterTypeDef],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListImagesRequestRequestTypeDef

```python
# ListImagesRequestRequestTypeDef definition

class ListImagesRequestRequestTypeDef(TypedDict):
    owner: NotRequired[OwnershipType],  # (1)
    filters: NotRequired[Sequence[FilterTypeDef]],  # (2)
    byName: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    includeDeprecated: NotRequired[bool],
```

1. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListInfrastructureConfigurationsRequestRequestTypeDef

```python
# ListInfrastructureConfigurationsRequestRequestTypeDef definition

class ListInfrastructureConfigurationsRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListImagePackagesResponseTypeDef

```python
# ListImagePackagesResponseTypeDef definition

class ListImagePackagesResponseTypeDef(TypedDict):
    requestId: str,
    imagePackageList: List[ImagePackageTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImagePackageTypeDef](./type_defs.md#imagepackagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImageRecipesResponseTypeDef

```python
# ListImageRecipesResponseTypeDef definition

class ListImageRecipesResponseTypeDef(TypedDict):
    requestId: str,
    imageRecipeSummaryList: List[ImageRecipeSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageRecipeSummaryTypeDef](./type_defs.md#imagerecipesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImageScanFindingsRequestRequestTypeDef

```python
# ListImageScanFindingsRequestRequestTypeDef definition

class ListImageScanFindingsRequestRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[ImageScanFindingsFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImageScanFindingsFilterTypeDef](./type_defs.md#imagescanfindingsfiltertypedef) 
## ListImagesResponseTypeDef

```python
# ListImagesResponseTypeDef definition

class ListImagesResponseTypeDef(TypedDict):
    requestId: str,
    imageVersionList: List[ImageVersionTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageVersionTypeDef](./type_defs.md#imageversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInfrastructureConfigurationsResponseTypeDef

```python
# ListInfrastructureConfigurationsResponseTypeDef definition

class ListInfrastructureConfigurationsResponseTypeDef(TypedDict):
    requestId: str,
    infrastructureConfigurationSummaryList: List[InfrastructureConfigurationSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InfrastructureConfigurationSummaryTypeDef](./type_defs.md#infrastructureconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkflowExecutionsResponseTypeDef

```python
# ListWorkflowExecutionsResponseTypeDef definition

class ListWorkflowExecutionsResponseTypeDef(TypedDict):
    requestId: str,
    workflowExecutions: List[WorkflowExecutionMetadataTypeDef],  # (1)
    imageBuildVersionArn: str,
    message: str,
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowExecutionMetadataTypeDef](./type_defs.md#workflowexecutionmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkflowStepExecutionsResponseTypeDef

```python
# ListWorkflowStepExecutionsResponseTypeDef definition

class ListWorkflowStepExecutionsResponseTypeDef(TypedDict):
    requestId: str,
    steps: List[WorkflowStepMetadataTypeDef],  # (1)
    workflowBuildVersionArn: str,
    workflowExecutionId: str,
    imageBuildVersionArn: str,
    message: str,
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowStepMetadataTypeDef](./type_defs.md#workflowstepmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingTypeDef

```python
# LoggingTypeDef definition

class LoggingTypeDef(TypedDict):
    s3Logs: NotRequired[S3LogsTypeDef],  # (1)
```

1. See [:material-code-braces: S3LogsTypeDef](./type_defs.md#s3logstypedef) 
## PackageVulnerabilityDetailsTypeDef

```python
# PackageVulnerabilityDetailsTypeDef definition

class PackageVulnerabilityDetailsTypeDef(TypedDict):
    vulnerabilityId: str,
    vulnerablePackages: NotRequired[List[VulnerablePackageTypeDef]],  # (1)
    source: NotRequired[str],
    cvss: NotRequired[List[CvssScoreTypeDef]],  # (2)
    relatedVulnerabilities: NotRequired[List[str]],
    sourceUrl: NotRequired[str],
    vendorSeverity: NotRequired[str],
    vendorCreatedAt: NotRequired[datetime],
    vendorUpdatedAt: NotRequired[datetime],
    referenceUrls: NotRequired[List[str]],
```

1. See [:material-code-braces: VulnerablePackageTypeDef](./type_defs.md#vulnerablepackagetypedef) 
2. See [:material-code-braces: CvssScoreTypeDef](./type_defs.md#cvssscoretypedef) 
## RemediationTypeDef

```python
# RemediationTypeDef definition

class RemediationTypeDef(TypedDict):
    recommendation: NotRequired[RemediationRecommendationTypeDef],  # (1)
```

1. See [:material-code-braces: RemediationRecommendationTypeDef](./type_defs.md#remediationrecommendationtypedef) 
## ImageScanFindingAggregationTypeDef

```python
# ImageScanFindingAggregationTypeDef definition

class ImageScanFindingAggregationTypeDef(TypedDict):
    accountAggregation: NotRequired[AccountAggregationTypeDef],  # (1)
    imageAggregation: NotRequired[ImageAggregationTypeDef],  # (2)
    imagePipelineAggregation: NotRequired[ImagePipelineAggregationTypeDef],  # (3)
    vulnerabilityIdAggregation: NotRequired[VulnerabilityIdAggregationTypeDef],  # (4)
```

1. See [:material-code-braces: AccountAggregationTypeDef](./type_defs.md#accountaggregationtypedef) 
2. See [:material-code-braces: ImageAggregationTypeDef](./type_defs.md#imageaggregationtypedef) 
3. See [:material-code-braces: ImagePipelineAggregationTypeDef](./type_defs.md#imagepipelineaggregationtypedef) 
4. See [:material-code-braces: VulnerabilityIdAggregationTypeDef](./type_defs.md#vulnerabilityidaggregationtypedef) 
## OutputResourcesTypeDef

```python
# OutputResourcesTypeDef definition

class OutputResourcesTypeDef(TypedDict):
    amis: NotRequired[List[AmiTypeDef]],  # (1)
    containers: NotRequired[List[ContainerTypeDef]],  # (2)
```

1. See [:material-code-braces: AmiTypeDef](./type_defs.md#amitypedef) 
2. See [:material-code-braces: ContainerTypeDef](./type_defs.md#containertypedef) 
## ListComponentBuildVersionsResponseTypeDef

```python
# ListComponentBuildVersionsResponseTypeDef definition

class ListComponentBuildVersionsResponseTypeDef(TypedDict):
    requestId: str,
    componentSummaryList: List[ComponentSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComponentResponseTypeDef

```python
# GetComponentResponseTypeDef definition

class GetComponentResponseTypeDef(TypedDict):
    requestId: str,
    component: ComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InspectorScoreDetailsTypeDef

```python
# InspectorScoreDetailsTypeDef definition

class InspectorScoreDetailsTypeDef(TypedDict):
    adjustedCvss: NotRequired[CvssScoreDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: CvssScoreDetailsTypeDef](./type_defs.md#cvssscoredetailstypedef) 
## CreateImageRecipeRequestRequestTypeDef

```python
# CreateImageRecipeRequestRequestTypeDef definition

class CreateImageRecipeRequestRequestTypeDef(TypedDict):
    name: str,
    semanticVersion: str,
    components: Sequence[ComponentConfigurationTypeDef],  # (1)
    parentImage: str,
    clientToken: str,
    description: NotRequired[str],
    blockDeviceMappings: NotRequired[Sequence[InstanceBlockDeviceMappingTypeDef]],  # (2)
    tags: NotRequired[Mapping[str, str]],
    workingDirectory: NotRequired[str],
    additionalInstanceConfiguration: NotRequired[AdditionalInstanceConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ComponentConfigurationTypeDef](./type_defs.md#componentconfigurationtypedef) 
2. See [:material-code-braces: InstanceBlockDeviceMappingTypeDef](./type_defs.md#instanceblockdevicemappingtypedef) 
3. See [:material-code-braces: AdditionalInstanceConfigurationTypeDef](./type_defs.md#additionalinstanceconfigurationtypedef) 
## ImageRecipeTypeDef

```python
# ImageRecipeTypeDef definition

class ImageRecipeTypeDef(TypedDict):
    arn: NotRequired[str],
    type: NotRequired[ImageTypeType],  # (1)
    name: NotRequired[str],
    description: NotRequired[str],
    platform: NotRequired[PlatformType],  # (2)
    owner: NotRequired[str],
    version: NotRequired[str],
    components: NotRequired[List[ComponentConfigurationTypeDef]],  # (3)
    parentImage: NotRequired[str],
    blockDeviceMappings: NotRequired[List[InstanceBlockDeviceMappingTypeDef]],  # (4)
    dateCreated: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    workingDirectory: NotRequired[str],
    additionalInstanceConfiguration: NotRequired[AdditionalInstanceConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: ImageTypeType](./literals.md#imagetypetype) 
2. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
3. See [:material-code-braces: ComponentConfigurationTypeDef](./type_defs.md#componentconfigurationtypedef) 
4. See [:material-code-braces: InstanceBlockDeviceMappingTypeDef](./type_defs.md#instanceblockdevicemappingtypedef) 
5. See [:material-code-braces: AdditionalInstanceConfigurationTypeDef](./type_defs.md#additionalinstanceconfigurationtypedef) 
## InstanceConfigurationTypeDef

```python
# InstanceConfigurationTypeDef definition

class InstanceConfigurationTypeDef(TypedDict):
    image: NotRequired[str],
    blockDeviceMappings: NotRequired[Sequence[InstanceBlockDeviceMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: InstanceBlockDeviceMappingTypeDef](./type_defs.md#instanceblockdevicemappingtypedef) 
## CreateImagePipelineRequestRequestTypeDef

```python
# CreateImagePipelineRequestRequestTypeDef definition

class CreateImagePipelineRequestRequestTypeDef(TypedDict):
    name: str,
    infrastructureConfigurationArn: str,
    clientToken: str,
    description: NotRequired[str],
    imageRecipeArn: NotRequired[str],
    containerRecipeArn: NotRequired[str],
    distributionConfigurationArn: NotRequired[str],
    imageTestsConfiguration: NotRequired[ImageTestsConfigurationTypeDef],  # (1)
    enhancedImageMetadataEnabled: NotRequired[bool],
    schedule: NotRequired[ScheduleTypeDef],  # (2)
    status: NotRequired[PipelineStatusType],  # (3)
    tags: NotRequired[Mapping[str, str]],
    imageScanningConfiguration: NotRequired[ImageScanningConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: ImageTestsConfigurationTypeDef](./type_defs.md#imagetestsconfigurationtypedef) 
2. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
3. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
4. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
## CreateImageRequestRequestTypeDef

```python
# CreateImageRequestRequestTypeDef definition

class CreateImageRequestRequestTypeDef(TypedDict):
    infrastructureConfigurationArn: str,
    clientToken: str,
    imageRecipeArn: NotRequired[str],
    containerRecipeArn: NotRequired[str],
    distributionConfigurationArn: NotRequired[str],
    imageTestsConfiguration: NotRequired[ImageTestsConfigurationTypeDef],  # (1)
    enhancedImageMetadataEnabled: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
    imageScanningConfiguration: NotRequired[ImageScanningConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ImageTestsConfigurationTypeDef](./type_defs.md#imagetestsconfigurationtypedef) 
2. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
## ImagePipelineTypeDef

```python
# ImagePipelineTypeDef definition

class ImagePipelineTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    platform: NotRequired[PlatformType],  # (1)
    enhancedImageMetadataEnabled: NotRequired[bool],
    imageRecipeArn: NotRequired[str],
    containerRecipeArn: NotRequired[str],
    infrastructureConfigurationArn: NotRequired[str],
    distributionConfigurationArn: NotRequired[str],
    imageTestsConfiguration: NotRequired[ImageTestsConfigurationTypeDef],  # (2)
    schedule: NotRequired[ScheduleTypeDef],  # (3)
    status: NotRequired[PipelineStatusType],  # (4)
    dateCreated: NotRequired[str],
    dateUpdated: NotRequired[str],
    dateLastRun: NotRequired[str],
    dateNextRun: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    imageScanningConfiguration: NotRequired[ImageScanningConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: ImageTestsConfigurationTypeDef](./type_defs.md#imagetestsconfigurationtypedef) 
3. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
4. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
5. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
## UpdateImagePipelineRequestRequestTypeDef

```python
# UpdateImagePipelineRequestRequestTypeDef definition

class UpdateImagePipelineRequestRequestTypeDef(TypedDict):
    imagePipelineArn: str,
    infrastructureConfigurationArn: str,
    clientToken: str,
    description: NotRequired[str],
    imageRecipeArn: NotRequired[str],
    containerRecipeArn: NotRequired[str],
    distributionConfigurationArn: NotRequired[str],
    imageTestsConfiguration: NotRequired[ImageTestsConfigurationTypeDef],  # (1)
    enhancedImageMetadataEnabled: NotRequired[bool],
    schedule: NotRequired[ScheduleTypeDef],  # (2)
    status: NotRequired[PipelineStatusType],  # (3)
    imageScanningConfiguration: NotRequired[ImageScanningConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: ImageTestsConfigurationTypeDef](./type_defs.md#imagetestsconfigurationtypedef) 
2. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
3. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
4. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
## DistributionTypeDef

```python
# DistributionTypeDef definition

class DistributionTypeDef(TypedDict):
    region: str,
    amiDistributionConfiguration: NotRequired[AmiDistributionConfigurationTypeDef],  # (1)
    containerDistributionConfiguration: NotRequired[ContainerDistributionConfigurationTypeDef],  # (2)
    licenseConfigurationArns: NotRequired[Sequence[str]],
    launchTemplateConfigurations: NotRequired[Sequence[LaunchTemplateConfigurationTypeDef]],  # (3)
    s3ExportConfiguration: NotRequired[S3ExportConfigurationTypeDef],  # (4)
    fastLaunchConfigurations: NotRequired[Sequence[FastLaunchConfigurationTypeDef]],  # (5)
```

1. See [:material-code-braces: AmiDistributionConfigurationTypeDef](./type_defs.md#amidistributionconfigurationtypedef) 
2. See [:material-code-braces: ContainerDistributionConfigurationTypeDef](./type_defs.md#containerdistributionconfigurationtypedef) 
3. See [:material-code-braces: LaunchTemplateConfigurationTypeDef](./type_defs.md#launchtemplateconfigurationtypedef) 
4. See [:material-code-braces: S3ExportConfigurationTypeDef](./type_defs.md#s3exportconfigurationtypedef) 
5. See [:material-code-braces: FastLaunchConfigurationTypeDef](./type_defs.md#fastlaunchconfigurationtypedef) 
## CreateInfrastructureConfigurationRequestRequestTypeDef

```python
# CreateInfrastructureConfigurationRequestRequestTypeDef definition

class CreateInfrastructureConfigurationRequestRequestTypeDef(TypedDict):
    name: str,
    instanceProfileName: str,
    clientToken: str,
    description: NotRequired[str],
    instanceTypes: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
    subnetId: NotRequired[str],
    logging: NotRequired[LoggingTypeDef],  # (1)
    keyPair: NotRequired[str],
    terminateInstanceOnFailure: NotRequired[bool],
    snsTopicArn: NotRequired[str],
    resourceTags: NotRequired[Mapping[str, str]],
    instanceMetadataOptions: NotRequired[InstanceMetadataOptionsTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
2. See [:material-code-braces: InstanceMetadataOptionsTypeDef](./type_defs.md#instancemetadataoptionstypedef) 
## InfrastructureConfigurationTypeDef

```python
# InfrastructureConfigurationTypeDef definition

class InfrastructureConfigurationTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    instanceTypes: NotRequired[List[str]],
    instanceProfileName: NotRequired[str],
    securityGroupIds: NotRequired[List[str]],
    subnetId: NotRequired[str],
    logging: NotRequired[LoggingTypeDef],  # (1)
    keyPair: NotRequired[str],
    terminateInstanceOnFailure: NotRequired[bool],
    snsTopicArn: NotRequired[str],
    dateCreated: NotRequired[str],
    dateUpdated: NotRequired[str],
    resourceTags: NotRequired[Dict[str, str]],
    instanceMetadataOptions: NotRequired[InstanceMetadataOptionsTypeDef],  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
2. See [:material-code-braces: InstanceMetadataOptionsTypeDef](./type_defs.md#instancemetadataoptionstypedef) 
## UpdateInfrastructureConfigurationRequestRequestTypeDef

```python
# UpdateInfrastructureConfigurationRequestRequestTypeDef definition

class UpdateInfrastructureConfigurationRequestRequestTypeDef(TypedDict):
    infrastructureConfigurationArn: str,
    instanceProfileName: str,
    clientToken: str,
    description: NotRequired[str],
    instanceTypes: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
    subnetId: NotRequired[str],
    logging: NotRequired[LoggingTypeDef],  # (1)
    keyPair: NotRequired[str],
    terminateInstanceOnFailure: NotRequired[bool],
    snsTopicArn: NotRequired[str],
    resourceTags: NotRequired[Mapping[str, str]],
    instanceMetadataOptions: NotRequired[InstanceMetadataOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
2. See [:material-code-braces: InstanceMetadataOptionsTypeDef](./type_defs.md#instancemetadataoptionstypedef) 
## ListImageScanFindingAggregationsResponseTypeDef

```python
# ListImageScanFindingAggregationsResponseTypeDef definition

class ListImageScanFindingAggregationsResponseTypeDef(TypedDict):
    requestId: str,
    aggregationType: str,
    responses: List[ImageScanFindingAggregationTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageScanFindingAggregationTypeDef](./type_defs.md#imagescanfindingaggregationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImageSummaryTypeDef

```python
# ImageSummaryTypeDef definition

class ImageSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[ImageTypeType],  # (1)
    version: NotRequired[str],
    platform: NotRequired[PlatformType],  # (2)
    osVersion: NotRequired[str],
    state: NotRequired[ImageStateTypeDef],  # (3)
    owner: NotRequired[str],
    dateCreated: NotRequired[str],
    outputResources: NotRequired[OutputResourcesTypeDef],  # (4)
    tags: NotRequired[Dict[str, str]],
    buildType: NotRequired[BuildTypeType],  # (5)
    imageSource: NotRequired[ImageSourceType],  # (6)
```

1. See [:material-code-brackets: ImageTypeType](./literals.md#imagetypetype) 
2. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
3. See [:material-code-braces: ImageStateTypeDef](./type_defs.md#imagestatetypedef) 
4. See [:material-code-braces: OutputResourcesTypeDef](./type_defs.md#outputresourcestypedef) 
5. See [:material-code-brackets: BuildTypeType](./literals.md#buildtypetype) 
6. See [:material-code-brackets: ImageSourceType](./literals.md#imagesourcetype) 
## ImageScanFindingTypeDef

```python
# ImageScanFindingTypeDef definition

class ImageScanFindingTypeDef(TypedDict):
    awsAccountId: NotRequired[str],
    imageBuildVersionArn: NotRequired[str],
    imagePipelineArn: NotRequired[str],
    type: NotRequired[str],
    description: NotRequired[str],
    title: NotRequired[str],
    remediation: NotRequired[RemediationTypeDef],  # (1)
    severity: NotRequired[str],
    firstObservedAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
    inspectorScore: NotRequired[float],
    inspectorScoreDetails: NotRequired[InspectorScoreDetailsTypeDef],  # (2)
    packageVulnerabilityDetails: NotRequired[PackageVulnerabilityDetailsTypeDef],  # (3)
    fixAvailable: NotRequired[str],
```

1. See [:material-code-braces: RemediationTypeDef](./type_defs.md#remediationtypedef) 
2. See [:material-code-braces: InspectorScoreDetailsTypeDef](./type_defs.md#inspectorscoredetailstypedef) 
3. See [:material-code-braces: PackageVulnerabilityDetailsTypeDef](./type_defs.md#packagevulnerabilitydetailstypedef) 
## GetImageRecipeResponseTypeDef

```python
# GetImageRecipeResponseTypeDef definition

class GetImageRecipeResponseTypeDef(TypedDict):
    requestId: str,
    imageRecipe: ImageRecipeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageRecipeTypeDef](./type_defs.md#imagerecipetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContainerRecipeTypeDef

```python
# ContainerRecipeTypeDef definition

class ContainerRecipeTypeDef(TypedDict):
    arn: NotRequired[str],
    containerType: NotRequired[ContainerTypeType],  # (1)
    name: NotRequired[str],
    description: NotRequired[str],
    platform: NotRequired[PlatformType],  # (2)
    owner: NotRequired[str],
    version: NotRequired[str],
    components: NotRequired[List[ComponentConfigurationTypeDef]],  # (3)
    instanceConfiguration: NotRequired[InstanceConfigurationTypeDef],  # (4)
    dockerfileTemplateData: NotRequired[str],
    kmsKeyId: NotRequired[str],
    encrypted: NotRequired[bool],
    parentImage: NotRequired[str],
    dateCreated: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    workingDirectory: NotRequired[str],
    targetRepository: NotRequired[TargetContainerRepositoryTypeDef],  # (5)
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
3. See [:material-code-braces: ComponentConfigurationTypeDef](./type_defs.md#componentconfigurationtypedef) 
4. See [:material-code-braces: InstanceConfigurationTypeDef](./type_defs.md#instanceconfigurationtypedef) 
5. See [:material-code-braces: TargetContainerRepositoryTypeDef](./type_defs.md#targetcontainerrepositorytypedef) 
## CreateContainerRecipeRequestRequestTypeDef

```python
# CreateContainerRecipeRequestRequestTypeDef definition

class CreateContainerRecipeRequestRequestTypeDef(TypedDict):
    containerType: ContainerTypeType,  # (1)
    name: str,
    semanticVersion: str,
    components: Sequence[ComponentConfigurationTypeDef],  # (2)
    parentImage: str,
    targetRepository: TargetContainerRepositoryTypeDef,  # (3)
    clientToken: str,
    description: NotRequired[str],
    instanceConfiguration: NotRequired[InstanceConfigurationTypeDef],  # (4)
    dockerfileTemplateData: NotRequired[str],
    dockerfileTemplateUri: NotRequired[str],
    platformOverride: NotRequired[PlatformType],  # (5)
    imageOsVersionOverride: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    workingDirectory: NotRequired[str],
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: ComponentConfigurationTypeDef](./type_defs.md#componentconfigurationtypedef) 
3. See [:material-code-braces: TargetContainerRepositoryTypeDef](./type_defs.md#targetcontainerrepositorytypedef) 
4. See [:material-code-braces: InstanceConfigurationTypeDef](./type_defs.md#instanceconfigurationtypedef) 
5. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
## GetImagePipelineResponseTypeDef

```python
# GetImagePipelineResponseTypeDef definition

class GetImagePipelineResponseTypeDef(TypedDict):
    requestId: str,
    imagePipeline: ImagePipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImagePipelineTypeDef](./type_defs.md#imagepipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImagePipelinesResponseTypeDef

```python
# ListImagePipelinesResponseTypeDef definition

class ListImagePipelinesResponseTypeDef(TypedDict):
    requestId: str,
    imagePipelineList: List[ImagePipelineTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImagePipelineTypeDef](./type_defs.md#imagepipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDistributionConfigurationRequestRequestTypeDef

```python
# CreateDistributionConfigurationRequestRequestTypeDef definition

class CreateDistributionConfigurationRequestRequestTypeDef(TypedDict):
    name: str,
    distributions: Sequence[DistributionTypeDef],  # (1)
    clientToken: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
## DistributionConfigurationTypeDef

```python
# DistributionConfigurationTypeDef definition

class DistributionConfigurationTypeDef(TypedDict):
    timeoutMinutes: int,
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    distributions: NotRequired[List[DistributionTypeDef]],  # (1)
    dateCreated: NotRequired[str],
    dateUpdated: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
## UpdateDistributionConfigurationRequestRequestTypeDef

```python
# UpdateDistributionConfigurationRequestRequestTypeDef definition

class UpdateDistributionConfigurationRequestRequestTypeDef(TypedDict):
    distributionConfigurationArn: str,
    distributions: Sequence[DistributionTypeDef],  # (1)
    clientToken: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
## GetInfrastructureConfigurationResponseTypeDef

```python
# GetInfrastructureConfigurationResponseTypeDef definition

class GetInfrastructureConfigurationResponseTypeDef(TypedDict):
    requestId: str,
    infrastructureConfiguration: InfrastructureConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InfrastructureConfigurationTypeDef](./type_defs.md#infrastructureconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImageBuildVersionsResponseTypeDef

```python
# ListImageBuildVersionsResponseTypeDef definition

class ListImageBuildVersionsResponseTypeDef(TypedDict):
    requestId: str,
    imageSummaryList: List[ImageSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageSummaryTypeDef](./type_defs.md#imagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImagePipelineImagesResponseTypeDef

```python
# ListImagePipelineImagesResponseTypeDef definition

class ListImagePipelineImagesResponseTypeDef(TypedDict):
    requestId: str,
    imageSummaryList: List[ImageSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageSummaryTypeDef](./type_defs.md#imagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImageScanFindingsResponseTypeDef

```python
# ListImageScanFindingsResponseTypeDef definition

class ListImageScanFindingsResponseTypeDef(TypedDict):
    requestId: str,
    findings: List[ImageScanFindingTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageScanFindingTypeDef](./type_defs.md#imagescanfindingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContainerRecipeResponseTypeDef

```python
# GetContainerRecipeResponseTypeDef definition

class GetContainerRecipeResponseTypeDef(TypedDict):
    requestId: str,
    containerRecipe: ContainerRecipeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContainerRecipeTypeDef](./type_defs.md#containerrecipetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDistributionConfigurationResponseTypeDef

```python
# GetDistributionConfigurationResponseTypeDef definition

class GetDistributionConfigurationResponseTypeDef(TypedDict):
    requestId: str,
    distributionConfiguration: DistributionConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DistributionConfigurationTypeDef](./type_defs.md#distributionconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImageTypeDef

```python
# ImageTypeDef definition

class ImageTypeDef(TypedDict):
    arn: NotRequired[str],
    type: NotRequired[ImageTypeType],  # (1)
    name: NotRequired[str],
    version: NotRequired[str],
    platform: NotRequired[PlatformType],  # (2)
    enhancedImageMetadataEnabled: NotRequired[bool],
    osVersion: NotRequired[str],
    state: NotRequired[ImageStateTypeDef],  # (3)
    imageRecipe: NotRequired[ImageRecipeTypeDef],  # (4)
    containerRecipe: NotRequired[ContainerRecipeTypeDef],  # (5)
    sourcePipelineName: NotRequired[str],
    sourcePipelineArn: NotRequired[str],
    infrastructureConfiguration: NotRequired[InfrastructureConfigurationTypeDef],  # (6)
    distributionConfiguration: NotRequired[DistributionConfigurationTypeDef],  # (7)
    imageTestsConfiguration: NotRequired[ImageTestsConfigurationTypeDef],  # (8)
    dateCreated: NotRequired[str],
    outputResources: NotRequired[OutputResourcesTypeDef],  # (9)
    tags: NotRequired[Dict[str, str]],
    buildType: NotRequired[BuildTypeType],  # (10)
    imageSource: NotRequired[ImageSourceType],  # (11)
    scanState: NotRequired[ImageScanStateTypeDef],  # (12)
    imageScanningConfiguration: NotRequired[ImageScanningConfigurationTypeDef],  # (13)
```

1. See [:material-code-brackets: ImageTypeType](./literals.md#imagetypetype) 
2. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
3. See [:material-code-braces: ImageStateTypeDef](./type_defs.md#imagestatetypedef) 
4. See [:material-code-braces: ImageRecipeTypeDef](./type_defs.md#imagerecipetypedef) 
5. See [:material-code-braces: ContainerRecipeTypeDef](./type_defs.md#containerrecipetypedef) 
6. See [:material-code-braces: InfrastructureConfigurationTypeDef](./type_defs.md#infrastructureconfigurationtypedef) 
7. See [:material-code-braces: DistributionConfigurationTypeDef](./type_defs.md#distributionconfigurationtypedef) 
8. See [:material-code-braces: ImageTestsConfigurationTypeDef](./type_defs.md#imagetestsconfigurationtypedef) 
9. See [:material-code-braces: OutputResourcesTypeDef](./type_defs.md#outputresourcestypedef) 
10. See [:material-code-brackets: BuildTypeType](./literals.md#buildtypetype) 
11. See [:material-code-brackets: ImageSourceType](./literals.md#imagesourcetype) 
12. See [:material-code-braces: ImageScanStateTypeDef](./type_defs.md#imagescanstatetypedef) 
13. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
## GetImageResponseTypeDef

```python
# GetImageResponseTypeDef definition

class GetImageResponseTypeDef(TypedDict):
    requestId: str,
    image: ImageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
