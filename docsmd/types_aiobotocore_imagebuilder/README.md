# Imagebuilder module

> [Index](../README.md) > Imagebuilder


!!! note ""

    Auto-generated documentation for [Imagebuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
    type annotations stubs module [types-aiobotocore-imagebuilder](https://pypi.org/project/types-aiobotocore-imagebuilder/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Imagebuilder` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Imagebuilder` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[imagebuilder]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[imagebuilder]'

# standalone installation
python -m pip install types-aiobotocore-imagebuilder
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-imagebuilder
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ImagebuilderClient

Type annotations and code completion for  `#!python session.create_client("imagebuilder")` as [ImagebuilderClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#Imagebuilder.Client)

```python
# ImagebuilderClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_imagebuilder.client import ImagebuilderClient


session = get_session()
async with session.create_client("imagebuilder") as client:
    client: ImagebuilderClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BuildTypeType usage example

from types_aiobotocore_imagebuilder.literals import BuildTypeType

def get_value() -> BuildTypeType:
    return "IMPORT"
```

- [BuildTypeType](./literals.md#buildtypetype)
- [ComponentFormatType](./literals.md#componentformattype)
- [ComponentStatusType](./literals.md#componentstatustype)
- [ComponentTypeType](./literals.md#componenttypetype)
- [ContainerRepositoryServiceType](./literals.md#containerrepositoryservicetype)
- [ContainerTypeType](./literals.md#containertypetype)
- [DiskImageFormatType](./literals.md#diskimageformattype)
- [EbsVolumeTypeType](./literals.md#ebsvolumetypetype)
- [ImageScanStatusType](./literals.md#imagescanstatustype)
- [ImageSourceType](./literals.md#imagesourcetype)
- [ImageStatusType](./literals.md#imagestatustype)
- [ImageTypeType](./literals.md#imagetypetype)
- [LifecycleExecutionResourceActionNameType](./literals.md#lifecycleexecutionresourceactionnametype)
- [LifecycleExecutionResourceStatusType](./literals.md#lifecycleexecutionresourcestatustype)
- [LifecycleExecutionStatusType](./literals.md#lifecycleexecutionstatustype)
- [LifecyclePolicyDetailActionTypeType](./literals.md#lifecyclepolicydetailactiontypetype)
- [LifecyclePolicyDetailFilterTypeType](./literals.md#lifecyclepolicydetailfiltertypetype)
- [LifecyclePolicyResourceTypeType](./literals.md#lifecyclepolicyresourcetypetype)
- [LifecyclePolicyStatusType](./literals.md#lifecyclepolicystatustype)
- [LifecyclePolicyTimeUnitType](./literals.md#lifecyclepolicytimeunittype)
- [MarketplaceResourceTypeType](./literals.md#marketplaceresourcetypetype)
- [OnWorkflowFailureType](./literals.md#onworkflowfailuretype)
- [OwnershipType](./literals.md#ownershiptype)
- [PipelineExecutionStartConditionType](./literals.md#pipelineexecutionstartconditiontype)
- [PipelineStatusType](./literals.md#pipelinestatustype)
- [PlatformType](./literals.md#platformtype)
- [ProductCodeTypeType](./literals.md#productcodetypetype)
- [ResourceStatusType](./literals.md#resourcestatustype)
- [TenancyTypeType](./literals.md#tenancytypetype)
- [WorkflowExecutionStatusType](./literals.md#workflowexecutionstatustype)
- [WorkflowStatusType](./literals.md#workflowstatustype)
- [WorkflowStepActionTypeType](./literals.md#workflowstepactiontypetype)
- [WorkflowStepExecutionRollbackStatusType](./literals.md#workflowstepexecutionrollbackstatustype)
- [WorkflowStepExecutionStatusType](./literals.md#workflowstepexecutionstatustype)
- [WorkflowTypeType](./literals.md#workflowtypetype)
- [ImagebuilderServiceName](./literals.md#imagebuilderservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [SeverityCountsTypeDef](./type_defs.md#severitycountstypedef)
- [SystemsManagerAgentTypeDef](./type_defs.md#systemsmanageragenttypedef)
- [LaunchPermissionConfigurationOutputTypeDef](./type_defs.md#launchpermissionconfigurationoutputtypedef)
- [ImageStateTypeDef](./type_defs.md#imagestatetypedef)
- [CancelImageCreationRequestRequestTypeDef](./type_defs.md#cancelimagecreationrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CancelLifecycleExecutionRequestRequestTypeDef](./type_defs.md#cancellifecycleexecutionrequestrequesttypedef)
- [ComponentParameterOutputTypeDef](./type_defs.md#componentparameteroutputtypedef)
- [ComponentParameterDetailTypeDef](./type_defs.md#componentparameterdetailtypedef)
- [ComponentParameterTypeDef](./type_defs.md#componentparametertypedef)
- [ComponentStateTypeDef](./type_defs.md#componentstatetypedef)
- [ProductCodeListItemTypeDef](./type_defs.md#productcodelistitemtypedef)
- [TargetContainerRepositoryTypeDef](./type_defs.md#targetcontainerrepositorytypedef)
- [ContainerRecipeSummaryTypeDef](./type_defs.md#containerrecipesummarytypedef)
- [ContainerTypeDef](./type_defs.md#containertypedef)
- [CreateComponentRequestRequestTypeDef](./type_defs.md#createcomponentrequestrequesttypedef)
- [ImageTestsConfigurationTypeDef](./type_defs.md#imagetestsconfigurationtypedef)
- [ScheduleTypeDef](./type_defs.md#scheduletypedef)
- [InstanceMetadataOptionsTypeDef](./type_defs.md#instancemetadataoptionstypedef)
- [PlacementTypeDef](./type_defs.md#placementtypedef)
- [CreateWorkflowRequestRequestTypeDef](./type_defs.md#createworkflowrequestrequesttypedef)
- [CvssScoreAdjustmentTypeDef](./type_defs.md#cvssscoreadjustmenttypedef)
- [CvssScoreTypeDef](./type_defs.md#cvssscoretypedef)
- [DeleteComponentRequestRequestTypeDef](./type_defs.md#deletecomponentrequestrequesttypedef)
- [DeleteContainerRecipeRequestRequestTypeDef](./type_defs.md#deletecontainerreciperequestrequesttypedef)
- [DeleteDistributionConfigurationRequestRequestTypeDef](./type_defs.md#deletedistributionconfigurationrequestrequesttypedef)
- [DeleteImagePipelineRequestRequestTypeDef](./type_defs.md#deleteimagepipelinerequestrequesttypedef)
- [DeleteImageRecipeRequestRequestTypeDef](./type_defs.md#deleteimagereciperequestrequesttypedef)
- [DeleteImageRequestRequestTypeDef](./type_defs.md#deleteimagerequestrequesttypedef)
- [DeleteInfrastructureConfigurationRequestRequestTypeDef](./type_defs.md#deleteinfrastructureconfigurationrequestrequesttypedef)
- [DeleteLifecyclePolicyRequestRequestTypeDef](./type_defs.md#deletelifecyclepolicyrequestrequesttypedef)
- [DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef)
- [DistributionConfigurationSummaryTypeDef](./type_defs.md#distributionconfigurationsummarytypedef)
- [LaunchTemplateConfigurationTypeDef](./type_defs.md#launchtemplateconfigurationtypedef)
- [S3ExportConfigurationTypeDef](./type_defs.md#s3exportconfigurationtypedef)
- [EbsInstanceBlockDeviceSpecificationTypeDef](./type_defs.md#ebsinstanceblockdevicespecificationtypedef)
- [EcrConfigurationOutputTypeDef](./type_defs.md#ecrconfigurationoutputtypedef)
- [EcrConfigurationTypeDef](./type_defs.md#ecrconfigurationtypedef)
- [FastLaunchLaunchTemplateSpecificationTypeDef](./type_defs.md#fastlaunchlaunchtemplatespecificationtypedef)
- [FastLaunchSnapshotConfigurationTypeDef](./type_defs.md#fastlaunchsnapshotconfigurationtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetComponentPolicyRequestRequestTypeDef](./type_defs.md#getcomponentpolicyrequestrequesttypedef)
- [GetComponentRequestRequestTypeDef](./type_defs.md#getcomponentrequestrequesttypedef)
- [GetContainerRecipePolicyRequestRequestTypeDef](./type_defs.md#getcontainerrecipepolicyrequestrequesttypedef)
- [GetContainerRecipeRequestRequestTypeDef](./type_defs.md#getcontainerreciperequestrequesttypedef)
- [GetDistributionConfigurationRequestRequestTypeDef](./type_defs.md#getdistributionconfigurationrequestrequesttypedef)
- [GetImagePipelineRequestRequestTypeDef](./type_defs.md#getimagepipelinerequestrequesttypedef)
- [GetImagePolicyRequestRequestTypeDef](./type_defs.md#getimagepolicyrequestrequesttypedef)
- [GetImageRecipePolicyRequestRequestTypeDef](./type_defs.md#getimagerecipepolicyrequestrequesttypedef)
- [GetImageRecipeRequestRequestTypeDef](./type_defs.md#getimagereciperequestrequesttypedef)
- [GetImageRequestRequestTypeDef](./type_defs.md#getimagerequestrequesttypedef)
- [GetInfrastructureConfigurationRequestRequestTypeDef](./type_defs.md#getinfrastructureconfigurationrequestrequesttypedef)
- [GetLifecycleExecutionRequestRequestTypeDef](./type_defs.md#getlifecycleexecutionrequestrequesttypedef)
- [GetLifecyclePolicyRequestRequestTypeDef](./type_defs.md#getlifecyclepolicyrequestrequesttypedef)
- [GetMarketplaceResourceRequestRequestTypeDef](./type_defs.md#getmarketplaceresourcerequestrequesttypedef)
- [GetWorkflowExecutionRequestRequestTypeDef](./type_defs.md#getworkflowexecutionrequestrequesttypedef)
- [GetWorkflowRequestRequestTypeDef](./type_defs.md#getworkflowrequestrequesttypedef)
- [GetWorkflowStepExecutionRequestRequestTypeDef](./type_defs.md#getworkflowstepexecutionrequestrequesttypedef)
- [ImagePackageTypeDef](./type_defs.md#imagepackagetypedef)
- [ImageRecipeSummaryTypeDef](./type_defs.md#imagerecipesummarytypedef)
- [ImageScanFindingsFilterTypeDef](./type_defs.md#imagescanfindingsfiltertypedef)
- [ImageScanStateTypeDef](./type_defs.md#imagescanstatetypedef)
- [ImageVersionTypeDef](./type_defs.md#imageversiontypedef)
- [ImportComponentRequestRequestTypeDef](./type_defs.md#importcomponentrequestrequesttypedef)
- [ImportVmImageRequestRequestTypeDef](./type_defs.md#importvmimagerequestrequesttypedef)
- [LaunchPermissionConfigurationTypeDef](./type_defs.md#launchpermissionconfigurationtypedef)
- [LifecycleExecutionResourceActionTypeDef](./type_defs.md#lifecycleexecutionresourceactiontypedef)
- [LifecycleExecutionResourceStateTypeDef](./type_defs.md#lifecycleexecutionresourcestatetypedef)
- [LifecycleExecutionResourcesImpactedSummaryTypeDef](./type_defs.md#lifecycleexecutionresourcesimpactedsummarytypedef)
- [LifecycleExecutionStateTypeDef](./type_defs.md#lifecycleexecutionstatetypedef)
- [LifecyclePolicyDetailActionIncludeResourcesTypeDef](./type_defs.md#lifecyclepolicydetailactionincluderesourcestypedef)
- [LifecyclePolicyDetailExclusionRulesAmisLastLaunchedTypeDef](./type_defs.md#lifecyclepolicydetailexclusionrulesamislastlaunchedtypedef)
- [LifecyclePolicyDetailFilterTypeDef](./type_defs.md#lifecyclepolicydetailfiltertypedef)
- [LifecyclePolicyResourceSelectionRecipeTypeDef](./type_defs.md#lifecyclepolicyresourceselectionrecipetypedef)
- [LifecyclePolicySummaryTypeDef](./type_defs.md#lifecyclepolicysummarytypedef)
- [ListComponentBuildVersionsRequestRequestTypeDef](./type_defs.md#listcomponentbuildversionsrequestrequesttypedef)
- [ListImagePackagesRequestRequestTypeDef](./type_defs.md#listimagepackagesrequestrequesttypedef)
- [ListLifecycleExecutionResourcesRequestRequestTypeDef](./type_defs.md#listlifecycleexecutionresourcesrequestrequesttypedef)
- [ListLifecycleExecutionsRequestRequestTypeDef](./type_defs.md#listlifecycleexecutionsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWaitingWorkflowStepsRequestRequestTypeDef](./type_defs.md#listwaitingworkflowstepsrequestrequesttypedef)
- [WorkflowStepExecutionTypeDef](./type_defs.md#workflowstepexecutiontypedef)
- [ListWorkflowBuildVersionsRequestRequestTypeDef](./type_defs.md#listworkflowbuildversionsrequestrequesttypedef)
- [ListWorkflowExecutionsRequestRequestTypeDef](./type_defs.md#listworkflowexecutionsrequestrequesttypedef)
- [WorkflowExecutionMetadataTypeDef](./type_defs.md#workflowexecutionmetadatatypedef)
- [ListWorkflowStepExecutionsRequestRequestTypeDef](./type_defs.md#listworkflowstepexecutionsrequestrequesttypedef)
- [WorkflowStepMetadataTypeDef](./type_defs.md#workflowstepmetadatatypedef)
- [WorkflowVersionTypeDef](./type_defs.md#workflowversiontypedef)
- [S3LogsTypeDef](./type_defs.md#s3logstypedef)
- [VulnerablePackageTypeDef](./type_defs.md#vulnerablepackagetypedef)
- [PutComponentPolicyRequestRequestTypeDef](./type_defs.md#putcomponentpolicyrequestrequesttypedef)
- [PutContainerRecipePolicyRequestRequestTypeDef](./type_defs.md#putcontainerrecipepolicyrequestrequesttypedef)
- [PutImagePolicyRequestRequestTypeDef](./type_defs.md#putimagepolicyrequestrequesttypedef)
- [PutImageRecipePolicyRequestRequestTypeDef](./type_defs.md#putimagerecipepolicyrequestrequesttypedef)
- [RemediationRecommendationTypeDef](./type_defs.md#remediationrecommendationtypedef)
- [ResourceStateTypeDef](./type_defs.md#resourcestatetypedef)
- [ResourceStateUpdateIncludeResourcesTypeDef](./type_defs.md#resourcestateupdateincluderesourcestypedef)
- [SendWorkflowStepActionRequestRequestTypeDef](./type_defs.md#sendworkflowstepactionrequestrequesttypedef)
- [StartImagePipelineExecutionRequestRequestTypeDef](./type_defs.md#startimagepipelineexecutionrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [WorkflowParameterOutputTypeDef](./type_defs.md#workflowparameteroutputtypedef)
- [WorkflowParameterDetailTypeDef](./type_defs.md#workflowparameterdetailtypedef)
- [WorkflowParameterTypeDef](./type_defs.md#workflowparametertypedef)
- [WorkflowStateTypeDef](./type_defs.md#workflowstatetypedef)
- [AccountAggregationTypeDef](./type_defs.md#accountaggregationtypedef)
- [ImageAggregationTypeDef](./type_defs.md#imageaggregationtypedef)
- [ImagePipelineAggregationTypeDef](./type_defs.md#imagepipelineaggregationtypedef)
- [VulnerabilityIdAggregationTypeDef](./type_defs.md#vulnerabilityidaggregationtypedef)
- [AdditionalInstanceConfigurationTypeDef](./type_defs.md#additionalinstanceconfigurationtypedef)
- [AmiDistributionConfigurationOutputTypeDef](./type_defs.md#amidistributionconfigurationoutputtypedef)
- [AmiTypeDef](./type_defs.md#amitypedef)
- [CancelImageCreationResponseTypeDef](./type_defs.md#cancelimagecreationresponsetypedef)
- [CancelLifecycleExecutionResponseTypeDef](./type_defs.md#cancellifecycleexecutionresponsetypedef)
- [CreateComponentResponseTypeDef](./type_defs.md#createcomponentresponsetypedef)
- [CreateContainerRecipeResponseTypeDef](./type_defs.md#createcontainerreciperesponsetypedef)
- [CreateDistributionConfigurationResponseTypeDef](./type_defs.md#createdistributionconfigurationresponsetypedef)
- [CreateImagePipelineResponseTypeDef](./type_defs.md#createimagepipelineresponsetypedef)
- [CreateImageRecipeResponseTypeDef](./type_defs.md#createimagereciperesponsetypedef)
- [CreateImageResponseTypeDef](./type_defs.md#createimageresponsetypedef)
- [CreateInfrastructureConfigurationResponseTypeDef](./type_defs.md#createinfrastructureconfigurationresponsetypedef)
- [CreateLifecyclePolicyResponseTypeDef](./type_defs.md#createlifecyclepolicyresponsetypedef)
- [CreateWorkflowResponseTypeDef](./type_defs.md#createworkflowresponsetypedef)
- [DeleteComponentResponseTypeDef](./type_defs.md#deletecomponentresponsetypedef)
- [DeleteContainerRecipeResponseTypeDef](./type_defs.md#deletecontainerreciperesponsetypedef)
- [DeleteDistributionConfigurationResponseTypeDef](./type_defs.md#deletedistributionconfigurationresponsetypedef)
- [DeleteImagePipelineResponseTypeDef](./type_defs.md#deleteimagepipelineresponsetypedef)
- [DeleteImageRecipeResponseTypeDef](./type_defs.md#deleteimagereciperesponsetypedef)
- [DeleteImageResponseTypeDef](./type_defs.md#deleteimageresponsetypedef)
- [DeleteInfrastructureConfigurationResponseTypeDef](./type_defs.md#deleteinfrastructureconfigurationresponsetypedef)
- [DeleteLifecyclePolicyResponseTypeDef](./type_defs.md#deletelifecyclepolicyresponsetypedef)
- [DeleteWorkflowResponseTypeDef](./type_defs.md#deleteworkflowresponsetypedef)
- [GetComponentPolicyResponseTypeDef](./type_defs.md#getcomponentpolicyresponsetypedef)
- [GetContainerRecipePolicyResponseTypeDef](./type_defs.md#getcontainerrecipepolicyresponsetypedef)
- [GetImagePolicyResponseTypeDef](./type_defs.md#getimagepolicyresponsetypedef)
- [GetImageRecipePolicyResponseTypeDef](./type_defs.md#getimagerecipepolicyresponsetypedef)
- [GetMarketplaceResourceResponseTypeDef](./type_defs.md#getmarketplaceresourceresponsetypedef)
- [GetWorkflowExecutionResponseTypeDef](./type_defs.md#getworkflowexecutionresponsetypedef)
- [GetWorkflowStepExecutionResponseTypeDef](./type_defs.md#getworkflowstepexecutionresponsetypedef)
- [ImportComponentResponseTypeDef](./type_defs.md#importcomponentresponsetypedef)
- [ImportVmImageResponseTypeDef](./type_defs.md#importvmimageresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutComponentPolicyResponseTypeDef](./type_defs.md#putcomponentpolicyresponsetypedef)
- [PutContainerRecipePolicyResponseTypeDef](./type_defs.md#putcontainerrecipepolicyresponsetypedef)
- [PutImagePolicyResponseTypeDef](./type_defs.md#putimagepolicyresponsetypedef)
- [PutImageRecipePolicyResponseTypeDef](./type_defs.md#putimagerecipepolicyresponsetypedef)
- [SendWorkflowStepActionResponseTypeDef](./type_defs.md#sendworkflowstepactionresponsetypedef)
- [StartImagePipelineExecutionResponseTypeDef](./type_defs.md#startimagepipelineexecutionresponsetypedef)
- [StartResourceStateUpdateResponseTypeDef](./type_defs.md#startresourcestateupdateresponsetypedef)
- [UpdateDistributionConfigurationResponseTypeDef](./type_defs.md#updatedistributionconfigurationresponsetypedef)
- [UpdateImagePipelineResponseTypeDef](./type_defs.md#updateimagepipelineresponsetypedef)
- [UpdateInfrastructureConfigurationResponseTypeDef](./type_defs.md#updateinfrastructureconfigurationresponsetypedef)
- [UpdateLifecyclePolicyResponseTypeDef](./type_defs.md#updatelifecyclepolicyresponsetypedef)
- [ComponentConfigurationOutputTypeDef](./type_defs.md#componentconfigurationoutputtypedef)
- [ComponentParameterUnionTypeDef](./type_defs.md#componentparameteruniontypedef)
- [ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef)
- [ComponentTypeDef](./type_defs.md#componenttypedef)
- [ComponentVersionTypeDef](./type_defs.md#componentversiontypedef)
- [ContainerDistributionConfigurationOutputTypeDef](./type_defs.md#containerdistributionconfigurationoutputtypedef)
- [ContainerDistributionConfigurationTypeDef](./type_defs.md#containerdistributionconfigurationtypedef)
- [ListContainerRecipesResponseTypeDef](./type_defs.md#listcontainerrecipesresponsetypedef)
- [InfrastructureConfigurationSummaryTypeDef](./type_defs.md#infrastructureconfigurationsummarytypedef)
- [CvssScoreDetailsTypeDef](./type_defs.md#cvssscoredetailstypedef)
- [ListDistributionConfigurationsResponseTypeDef](./type_defs.md#listdistributionconfigurationsresponsetypedef)
- [InstanceBlockDeviceMappingTypeDef](./type_defs.md#instanceblockdevicemappingtypedef)
- [ImageScanningConfigurationOutputTypeDef](./type_defs.md#imagescanningconfigurationoutputtypedef)
- [EcrConfigurationUnionTypeDef](./type_defs.md#ecrconfigurationuniontypedef)
- [FastLaunchConfigurationTypeDef](./type_defs.md#fastlaunchconfigurationtypedef)
- [ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef)
- [ListContainerRecipesRequestRequestTypeDef](./type_defs.md#listcontainerrecipesrequestrequesttypedef)
- [ListDistributionConfigurationsRequestRequestTypeDef](./type_defs.md#listdistributionconfigurationsrequestrequesttypedef)
- [ListImageBuildVersionsRequestRequestTypeDef](./type_defs.md#listimagebuildversionsrequestrequesttypedef)
- [ListImagePipelineImagesRequestRequestTypeDef](./type_defs.md#listimagepipelineimagesrequestrequesttypedef)
- [ListImagePipelinesRequestRequestTypeDef](./type_defs.md#listimagepipelinesrequestrequesttypedef)
- [ListImageRecipesRequestRequestTypeDef](./type_defs.md#listimagerecipesrequestrequesttypedef)
- [ListImageScanFindingAggregationsRequestRequestTypeDef](./type_defs.md#listimagescanfindingaggregationsrequestrequesttypedef)
- [ListImagesRequestRequestTypeDef](./type_defs.md#listimagesrequestrequesttypedef)
- [ListInfrastructureConfigurationsRequestRequestTypeDef](./type_defs.md#listinfrastructureconfigurationsrequestrequesttypedef)
- [ListLifecyclePoliciesRequestRequestTypeDef](./type_defs.md#listlifecyclepoliciesrequestrequesttypedef)
- [ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef)
- [ListImagePackagesResponseTypeDef](./type_defs.md#listimagepackagesresponsetypedef)
- [ListImageRecipesResponseTypeDef](./type_defs.md#listimagerecipesresponsetypedef)
- [ListImageScanFindingsRequestRequestTypeDef](./type_defs.md#listimagescanfindingsrequestrequesttypedef)
- [ListImagesResponseTypeDef](./type_defs.md#listimagesresponsetypedef)
- [LaunchPermissionConfigurationUnionTypeDef](./type_defs.md#launchpermissionconfigurationuniontypedef)
- [LifecycleExecutionSnapshotResourceTypeDef](./type_defs.md#lifecycleexecutionsnapshotresourcetypedef)
- [LifecycleExecutionTypeDef](./type_defs.md#lifecycleexecutiontypedef)
- [LifecyclePolicyDetailActionTypeDef](./type_defs.md#lifecyclepolicydetailactiontypedef)
- [LifecyclePolicyDetailExclusionRulesAmisOutputTypeDef](./type_defs.md#lifecyclepolicydetailexclusionrulesamisoutputtypedef)
- [LifecyclePolicyDetailExclusionRulesAmisTypeDef](./type_defs.md#lifecyclepolicydetailexclusionrulesamistypedef)
- [LifecyclePolicyResourceSelectionOutputTypeDef](./type_defs.md#lifecyclepolicyresourceselectionoutputtypedef)
- [LifecyclePolicyResourceSelectionTypeDef](./type_defs.md#lifecyclepolicyresourceselectiontypedef)
- [ListLifecyclePoliciesResponseTypeDef](./type_defs.md#listlifecyclepoliciesresponsetypedef)
- [ListWaitingWorkflowStepsResponseTypeDef](./type_defs.md#listwaitingworkflowstepsresponsetypedef)
- [ListWorkflowExecutionsResponseTypeDef](./type_defs.md#listworkflowexecutionsresponsetypedef)
- [ListWorkflowStepExecutionsResponseTypeDef](./type_defs.md#listworkflowstepexecutionsresponsetypedef)
- [ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef)
- [LoggingTypeDef](./type_defs.md#loggingtypedef)
- [PackageVulnerabilityDetailsTypeDef](./type_defs.md#packagevulnerabilitydetailstypedef)
- [RemediationTypeDef](./type_defs.md#remediationtypedef)
- [WorkflowConfigurationOutputTypeDef](./type_defs.md#workflowconfigurationoutputtypedef)
- [WorkflowParameterUnionTypeDef](./type_defs.md#workflowparameteruniontypedef)
- [WorkflowSummaryTypeDef](./type_defs.md#workflowsummarytypedef)
- [WorkflowTypeDef](./type_defs.md#workflowtypedef)
- [ImageScanFindingAggregationTypeDef](./type_defs.md#imagescanfindingaggregationtypedef)
- [OutputResourcesTypeDef](./type_defs.md#outputresourcestypedef)
- [ComponentConfigurationTypeDef](./type_defs.md#componentconfigurationtypedef)
- [ListComponentBuildVersionsResponseTypeDef](./type_defs.md#listcomponentbuildversionsresponsetypedef)
- [GetComponentResponseTypeDef](./type_defs.md#getcomponentresponsetypedef)
- [ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef)
- [ContainerDistributionConfigurationUnionTypeDef](./type_defs.md#containerdistributionconfigurationuniontypedef)
- [ListInfrastructureConfigurationsResponseTypeDef](./type_defs.md#listinfrastructureconfigurationsresponsetypedef)
- [InspectorScoreDetailsTypeDef](./type_defs.md#inspectorscoredetailstypedef)
- [ImageRecipeTypeDef](./type_defs.md#imagerecipetypedef)
- [InstanceConfigurationOutputTypeDef](./type_defs.md#instanceconfigurationoutputtypedef)
- [InstanceConfigurationTypeDef](./type_defs.md#instanceconfigurationtypedef)
- [ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef)
- [DistributionOutputTypeDef](./type_defs.md#distributionoutputtypedef)
- [AmiDistributionConfigurationTypeDef](./type_defs.md#amidistributionconfigurationtypedef)
- [LifecycleExecutionResourceTypeDef](./type_defs.md#lifecycleexecutionresourcetypedef)
- [GetLifecycleExecutionResponseTypeDef](./type_defs.md#getlifecycleexecutionresponsetypedef)
- [ListLifecycleExecutionsResponseTypeDef](./type_defs.md#listlifecycleexecutionsresponsetypedef)
- [LifecyclePolicyDetailExclusionRulesOutputTypeDef](./type_defs.md#lifecyclepolicydetailexclusionrulesoutputtypedef)
- [LifecyclePolicyDetailExclusionRulesAmisUnionTypeDef](./type_defs.md#lifecyclepolicydetailexclusionrulesamisuniontypedef)
- [CreateInfrastructureConfigurationRequestRequestTypeDef](./type_defs.md#createinfrastructureconfigurationrequestrequesttypedef)
- [InfrastructureConfigurationTypeDef](./type_defs.md#infrastructureconfigurationtypedef)
- [UpdateInfrastructureConfigurationRequestRequestTypeDef](./type_defs.md#updateinfrastructureconfigurationrequestrequesttypedef)
- [ImagePipelineTypeDef](./type_defs.md#imagepipelinetypedef)
- [WorkflowConfigurationTypeDef](./type_defs.md#workflowconfigurationtypedef)
- [ListWorkflowBuildVersionsResponseTypeDef](./type_defs.md#listworkflowbuildversionsresponsetypedef)
- [GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef)
- [ListImageScanFindingAggregationsResponseTypeDef](./type_defs.md#listimagescanfindingaggregationsresponsetypedef)
- [ImageSummaryTypeDef](./type_defs.md#imagesummarytypedef)
- [ComponentConfigurationUnionTypeDef](./type_defs.md#componentconfigurationuniontypedef)
- [CreateImageRecipeRequestRequestTypeDef](./type_defs.md#createimagereciperequestrequesttypedef)
- [ImageScanFindingTypeDef](./type_defs.md#imagescanfindingtypedef)
- [GetImageRecipeResponseTypeDef](./type_defs.md#getimagereciperesponsetypedef)
- [ContainerRecipeTypeDef](./type_defs.md#containerrecipetypedef)
- [DistributionConfigurationTypeDef](./type_defs.md#distributionconfigurationtypedef)
- [AmiDistributionConfigurationUnionTypeDef](./type_defs.md#amidistributionconfigurationuniontypedef)
- [ListLifecycleExecutionResourcesResponseTypeDef](./type_defs.md#listlifecycleexecutionresourcesresponsetypedef)
- [LifecyclePolicyDetailOutputTypeDef](./type_defs.md#lifecyclepolicydetailoutputtypedef)
- [LifecyclePolicyDetailExclusionRulesTypeDef](./type_defs.md#lifecyclepolicydetailexclusionrulestypedef)
- [ResourceStateUpdateExclusionRulesTypeDef](./type_defs.md#resourcestateupdateexclusionrulestypedef)
- [GetInfrastructureConfigurationResponseTypeDef](./type_defs.md#getinfrastructureconfigurationresponsetypedef)
- [GetImagePipelineResponseTypeDef](./type_defs.md#getimagepipelineresponsetypedef)
- [ListImagePipelinesResponseTypeDef](./type_defs.md#listimagepipelinesresponsetypedef)
- [CreateImagePipelineRequestRequestTypeDef](./type_defs.md#createimagepipelinerequestrequesttypedef)
- [UpdateImagePipelineRequestRequestTypeDef](./type_defs.md#updateimagepipelinerequestrequesttypedef)
- [WorkflowConfigurationUnionTypeDef](./type_defs.md#workflowconfigurationuniontypedef)
- [ListImageBuildVersionsResponseTypeDef](./type_defs.md#listimagebuildversionsresponsetypedef)
- [ListImagePipelineImagesResponseTypeDef](./type_defs.md#listimagepipelineimagesresponsetypedef)
- [CreateContainerRecipeRequestRequestTypeDef](./type_defs.md#createcontainerreciperequestrequesttypedef)
- [ListImageScanFindingsResponseTypeDef](./type_defs.md#listimagescanfindingsresponsetypedef)
- [GetContainerRecipeResponseTypeDef](./type_defs.md#getcontainerreciperesponsetypedef)
- [GetDistributionConfigurationResponseTypeDef](./type_defs.md#getdistributionconfigurationresponsetypedef)
- [ImageTypeDef](./type_defs.md#imagetypedef)
- [DistributionTypeDef](./type_defs.md#distributiontypedef)
- [LifecyclePolicyTypeDef](./type_defs.md#lifecyclepolicytypedef)
- [LifecyclePolicyDetailExclusionRulesUnionTypeDef](./type_defs.md#lifecyclepolicydetailexclusionrulesuniontypedef)
- [StartResourceStateUpdateRequestRequestTypeDef](./type_defs.md#startresourcestateupdaterequestrequesttypedef)
- [CreateImageRequestRequestTypeDef](./type_defs.md#createimagerequestrequesttypedef)
- [GetImageResponseTypeDef](./type_defs.md#getimageresponsetypedef)
- [DistributionUnionTypeDef](./type_defs.md#distributionuniontypedef)
- [UpdateDistributionConfigurationRequestRequestTypeDef](./type_defs.md#updatedistributionconfigurationrequestrequesttypedef)
- [GetLifecyclePolicyResponseTypeDef](./type_defs.md#getlifecyclepolicyresponsetypedef)
- [LifecyclePolicyDetailTypeDef](./type_defs.md#lifecyclepolicydetailtypedef)
- [CreateDistributionConfigurationRequestRequestTypeDef](./type_defs.md#createdistributionconfigurationrequestrequesttypedef)
- [LifecyclePolicyDetailUnionTypeDef](./type_defs.md#lifecyclepolicydetailuniontypedef)
- [UpdateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#updatelifecyclepolicyrequestrequesttypedef)
- [CreateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#createlifecyclepolicyrequestrequesttypedef)

