# ImagebuilderClient

> [Index](../README.md) > [Imagebuilder](./README.md) > ImagebuilderClient

!!! note ""

    Auto-generated documentation for [Imagebuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder)
    type annotations stubs module [types-aiobotocore-imagebuilder](https://pypi.org/project/types-aiobotocore-imagebuilder/).

## ImagebuilderClient

Type annotations and code completion for `#!python session.create_client("imagebuilder")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#Imagebuilder.Client)

```python
# ImagebuilderClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_imagebuilder.client import ImagebuilderClient

session = get_session()
async with session.create_client("imagebuilder") as client:
    client: ImagebuilderClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("imagebuilder").exceptions` structure.

```python
# ImagebuilderClient.exceptions usage example

async with session.create_client("imagebuilder") as client:
    try:
        do_something(client)
    except (
            client.CallRateLimitExceededException,
        client.ClientError,
        client.ClientException,
        client.ForbiddenException,
        client.IdempotentParameterMismatchException,
        client.InvalidPaginationTokenException,
        client.InvalidParameterCombinationException,
        client.InvalidParameterException,
        client.InvalidParameterValueException,
        client.InvalidRequestException,
        client.InvalidVersionNumberException,
        client.ResourceAlreadyExistsException,
        client.ResourceDependencyException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.ServiceException,
        client.ServiceQuotaExceededException,
        client.ServiceUnavailableException,
    ) as e:
        print(e)
```

```python
# ImagebuilderClient usage type checking example

from types_aiobotocore_imagebuilder.client import Exceptions

def handle_error(exc: Exceptions.CallRateLimitExceededException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("imagebuilder").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("imagebuilder").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### close



Type annotations and code completion for `#!python session.create_client("imagebuilder").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### cancel\_image\_creation

CancelImageCreation cancels the creation of Image.

Type annotations and code completion for `#!python session.create_client("imagebuilder").cancel_image_creation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/cancel_image_creation.html)

```python
# cancel_image_creation method definition

await def cancel_image_creation(
    self,
    *,
    imageBuildVersionArn: str,
    clientToken: str,
) -> CancelImageCreationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelImageCreationResponseTypeDef](./type_defs.md#cancelimagecreationresponsetypedef) 


```python
# cancel_image_creation method usage example with argument unpacking

kwargs: CancelImageCreationRequestRequestTypeDef = {  # (1)
    "imageBuildVersionArn": ...,
    "clientToken": ...,
}

parent.cancel_image_creation(**kwargs)
```

1. See [:material-code-braces: CancelImageCreationRequestRequestTypeDef](./type_defs.md#cancelimagecreationrequestrequesttypedef) 

### cancel\_lifecycle\_execution

Cancel a specific image lifecycle policy runtime instance.

Type annotations and code completion for `#!python session.create_client("imagebuilder").cancel_lifecycle_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/cancel_lifecycle_execution.html)

```python
# cancel_lifecycle_execution method definition

await def cancel_lifecycle_execution(
    self,
    *,
    lifecycleExecutionId: str,
    clientToken: str,
) -> CancelLifecycleExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelLifecycleExecutionResponseTypeDef](./type_defs.md#cancellifecycleexecutionresponsetypedef) 


```python
# cancel_lifecycle_execution method usage example with argument unpacking

kwargs: CancelLifecycleExecutionRequestRequestTypeDef = {  # (1)
    "lifecycleExecutionId": ...,
    "clientToken": ...,
}

parent.cancel_lifecycle_execution(**kwargs)
```

1. See [:material-code-braces: CancelLifecycleExecutionRequestRequestTypeDef](./type_defs.md#cancellifecycleexecutionrequestrequesttypedef) 

### create\_component

Creates a new component that can be used to build, validate, test, and assess
your image.

Type annotations and code completion for `#!python session.create_client("imagebuilder").create_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/create_component.html)

```python
# create_component method definition

await def create_component(
    self,
    *,
    name: str,
    semanticVersion: str,
    platform: PlatformType,  # (1)
    clientToken: str,
    description: str = ...,
    changeDescription: str = ...,
    supportedOsVersions: Sequence[str] = ...,
    data: str = ...,
    uri: str = ...,
    kmsKeyId: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateComponentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: CreateComponentResponseTypeDef](./type_defs.md#createcomponentresponsetypedef) 


```python
# create_component method usage example with argument unpacking

kwargs: CreateComponentRequestRequestTypeDef = {  # (1)
    "name": ...,
    "semanticVersion": ...,
    "platform": ...,
    "clientToken": ...,
}

parent.create_component(**kwargs)
```

1. See [:material-code-braces: CreateComponentRequestRequestTypeDef](./type_defs.md#createcomponentrequestrequesttypedef) 

### create\_container\_recipe

Creates a new container recipe.

Type annotations and code completion for `#!python session.create_client("imagebuilder").create_container_recipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/create_container_recipe.html)

```python
# create_container_recipe method definition

await def create_container_recipe(
    self,
    *,
    containerType: ContainerTypeType,  # (1)
    name: str,
    semanticVersion: str,
    components: Sequence[ComponentConfigurationUnionTypeDef],  # (2)
    parentImage: str,
    targetRepository: TargetContainerRepositoryTypeDef,  # (3)
    clientToken: str,
    description: str = ...,
    instanceConfiguration: InstanceConfigurationTypeDef = ...,  # (4)
    dockerfileTemplateData: str = ...,
    dockerfileTemplateUri: str = ...,
    platformOverride: PlatformType = ...,  # (5)
    imageOsVersionOverride: str = ...,
    tags: Mapping[str, str] = ...,
    workingDirectory: str = ...,
    kmsKeyId: str = ...,
) -> CreateContainerRecipeResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ContainerTypeType](./literals.md#containertypetype) 
2. See [:material-code-braces: ComponentConfigurationTypeDef](./type_defs.md#componentconfigurationtypedef) [:material-code-braces: ComponentConfigurationOutputTypeDef](./type_defs.md#componentconfigurationoutputtypedef) 
3. See [:material-code-braces: TargetContainerRepositoryTypeDef](./type_defs.md#targetcontainerrepositorytypedef) 
4. See [:material-code-braces: InstanceConfigurationTypeDef](./type_defs.md#instanceconfigurationtypedef) 
5. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
6. See [:material-code-braces: CreateContainerRecipeResponseTypeDef](./type_defs.md#createcontainerreciperesponsetypedef) 


```python
# create_container_recipe method usage example with argument unpacking

kwargs: CreateContainerRecipeRequestRequestTypeDef = {  # (1)
    "containerType": ...,
    "name": ...,
    "semanticVersion": ...,
    "components": ...,
    "parentImage": ...,
    "targetRepository": ...,
    "clientToken": ...,
}

parent.create_container_recipe(**kwargs)
```

1. See [:material-code-braces: CreateContainerRecipeRequestRequestTypeDef](./type_defs.md#createcontainerreciperequestrequesttypedef) 

### create\_distribution\_configuration

Creates a new distribution configuration.

Type annotations and code completion for `#!python session.create_client("imagebuilder").create_distribution_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/create_distribution_configuration.html)

```python
# create_distribution_configuration method definition

await def create_distribution_configuration(
    self,
    *,
    name: str,
    distributions: Sequence[DistributionUnionTypeDef],  # (1)
    clientToken: str,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateDistributionConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) [:material-code-braces: DistributionOutputTypeDef](./type_defs.md#distributionoutputtypedef) 
2. See [:material-code-braces: CreateDistributionConfigurationResponseTypeDef](./type_defs.md#createdistributionconfigurationresponsetypedef) 


```python
# create_distribution_configuration method usage example with argument unpacking

kwargs: CreateDistributionConfigurationRequestRequestTypeDef = {  # (1)
    "name": ...,
    "distributions": ...,
    "clientToken": ...,
}

parent.create_distribution_configuration(**kwargs)
```

1. See [:material-code-braces: CreateDistributionConfigurationRequestRequestTypeDef](./type_defs.md#createdistributionconfigurationrequestrequesttypedef) 

### create\_image

Creates a new image.

Type annotations and code completion for `#!python session.create_client("imagebuilder").create_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/create_image.html)

```python
# create_image method definition

await def create_image(
    self,
    *,
    infrastructureConfigurationArn: str,
    clientToken: str,
    imageRecipeArn: str = ...,
    containerRecipeArn: str = ...,
    distributionConfigurationArn: str = ...,
    imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,  # (1)
    enhancedImageMetadataEnabled: bool = ...,
    tags: Mapping[str, str] = ...,
    imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,  # (2)
    workflows: Sequence[WorkflowConfigurationUnionTypeDef] = ...,  # (3)
    executionRole: str = ...,
) -> CreateImageResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ImageTestsConfigurationTypeDef](./type_defs.md#imagetestsconfigurationtypedef) 
2. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
3. See [:material-code-braces: WorkflowConfigurationTypeDef](./type_defs.md#workflowconfigurationtypedef) [:material-code-braces: WorkflowConfigurationOutputTypeDef](./type_defs.md#workflowconfigurationoutputtypedef) 
4. See [:material-code-braces: CreateImageResponseTypeDef](./type_defs.md#createimageresponsetypedef) 


```python
# create_image method usage example with argument unpacking

kwargs: CreateImageRequestRequestTypeDef = {  # (1)
    "infrastructureConfigurationArn": ...,
    "clientToken": ...,
}

parent.create_image(**kwargs)
```

1. See [:material-code-braces: CreateImageRequestRequestTypeDef](./type_defs.md#createimagerequestrequesttypedef) 

### create\_image\_pipeline

Creates a new image pipeline.

Type annotations and code completion for `#!python session.create_client("imagebuilder").create_image_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/create_image_pipeline.html)

```python
# create_image_pipeline method definition

await def create_image_pipeline(
    self,
    *,
    name: str,
    infrastructureConfigurationArn: str,
    clientToken: str,
    description: str = ...,
    imageRecipeArn: str = ...,
    containerRecipeArn: str = ...,
    distributionConfigurationArn: str = ...,
    imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,  # (1)
    enhancedImageMetadataEnabled: bool = ...,
    schedule: ScheduleTypeDef = ...,  # (2)
    status: PipelineStatusType = ...,  # (3)
    tags: Mapping[str, str] = ...,
    imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,  # (4)
    workflows: Sequence[WorkflowConfigurationTypeDef] = ...,  # (5)
    executionRole: str = ...,
) -> CreateImagePipelineResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ImageTestsConfigurationTypeDef](./type_defs.md#imagetestsconfigurationtypedef) 
2. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
3. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
4. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
5. See [:material-code-braces: WorkflowConfigurationTypeDef](./type_defs.md#workflowconfigurationtypedef) 
6. See [:material-code-braces: CreateImagePipelineResponseTypeDef](./type_defs.md#createimagepipelineresponsetypedef) 


```python
# create_image_pipeline method usage example with argument unpacking

kwargs: CreateImagePipelineRequestRequestTypeDef = {  # (1)
    "name": ...,
    "infrastructureConfigurationArn": ...,
    "clientToken": ...,
}

parent.create_image_pipeline(**kwargs)
```

1. See [:material-code-braces: CreateImagePipelineRequestRequestTypeDef](./type_defs.md#createimagepipelinerequestrequesttypedef) 

### create\_image\_recipe

Creates a new image recipe.

Type annotations and code completion for `#!python session.create_client("imagebuilder").create_image_recipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/create_image_recipe.html)

```python
# create_image_recipe method definition

await def create_image_recipe(
    self,
    *,
    name: str,
    semanticVersion: str,
    components: Sequence[ComponentConfigurationTypeDef],  # (1)
    parentImage: str,
    clientToken: str,
    description: str = ...,
    blockDeviceMappings: Sequence[InstanceBlockDeviceMappingTypeDef] = ...,  # (2)
    tags: Mapping[str, str] = ...,
    workingDirectory: str = ...,
    additionalInstanceConfiguration: AdditionalInstanceConfigurationTypeDef = ...,  # (3)
) -> CreateImageRecipeResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ComponentConfigurationTypeDef](./type_defs.md#componentconfigurationtypedef) 
2. See [:material-code-braces: InstanceBlockDeviceMappingTypeDef](./type_defs.md#instanceblockdevicemappingtypedef) 
3. See [:material-code-braces: AdditionalInstanceConfigurationTypeDef](./type_defs.md#additionalinstanceconfigurationtypedef) 
4. See [:material-code-braces: CreateImageRecipeResponseTypeDef](./type_defs.md#createimagereciperesponsetypedef) 


```python
# create_image_recipe method usage example with argument unpacking

kwargs: CreateImageRecipeRequestRequestTypeDef = {  # (1)
    "name": ...,
    "semanticVersion": ...,
    "components": ...,
    "parentImage": ...,
    "clientToken": ...,
}

parent.create_image_recipe(**kwargs)
```

1. See [:material-code-braces: CreateImageRecipeRequestRequestTypeDef](./type_defs.md#createimagereciperequestrequesttypedef) 

### create\_infrastructure\_configuration

Creates a new infrastructure configuration.

Type annotations and code completion for `#!python session.create_client("imagebuilder").create_infrastructure_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/create_infrastructure_configuration.html)

```python
# create_infrastructure_configuration method definition

await def create_infrastructure_configuration(
    self,
    *,
    name: str,
    instanceProfileName: str,
    clientToken: str,
    description: str = ...,
    instanceTypes: Sequence[str] = ...,
    securityGroupIds: Sequence[str] = ...,
    subnetId: str = ...,
    logging: LoggingTypeDef = ...,  # (1)
    keyPair: str = ...,
    terminateInstanceOnFailure: bool = ...,
    snsTopicArn: str = ...,
    resourceTags: Mapping[str, str] = ...,
    instanceMetadataOptions: InstanceMetadataOptionsTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
    placement: PlacementTypeDef = ...,  # (3)
) -> CreateInfrastructureConfigurationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
2. See [:material-code-braces: InstanceMetadataOptionsTypeDef](./type_defs.md#instancemetadataoptionstypedef) 
3. See [:material-code-braces: PlacementTypeDef](./type_defs.md#placementtypedef) 
4. See [:material-code-braces: CreateInfrastructureConfigurationResponseTypeDef](./type_defs.md#createinfrastructureconfigurationresponsetypedef) 


```python
# create_infrastructure_configuration method usage example with argument unpacking

kwargs: CreateInfrastructureConfigurationRequestRequestTypeDef = {  # (1)
    "name": ...,
    "instanceProfileName": ...,
    "clientToken": ...,
}

parent.create_infrastructure_configuration(**kwargs)
```

1. See [:material-code-braces: CreateInfrastructureConfigurationRequestRequestTypeDef](./type_defs.md#createinfrastructureconfigurationrequestrequesttypedef) 

### create\_lifecycle\_policy

Create a lifecycle policy resource.

Type annotations and code completion for `#!python session.create_client("imagebuilder").create_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/create_lifecycle_policy.html)

```python
# create_lifecycle_policy method definition

await def create_lifecycle_policy(
    self,
    *,
    name: str,
    executionRole: str,
    resourceType: LifecyclePolicyResourceTypeType,  # (1)
    policyDetails: Sequence[LifecyclePolicyDetailUnionTypeDef],  # (2)
    resourceSelection: LifecyclePolicyResourceSelectionTypeDef,  # (3)
    clientToken: str,
    description: str = ...,
    status: LifecyclePolicyStatusType = ...,  # (4)
    tags: Mapping[str, str] = ...,
) -> CreateLifecyclePolicyResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: LifecyclePolicyResourceTypeType](./literals.md#lifecyclepolicyresourcetypetype) 
2. See [:material-code-braces: LifecyclePolicyDetailTypeDef](./type_defs.md#lifecyclepolicydetailtypedef) [:material-code-braces: LifecyclePolicyDetailOutputTypeDef](./type_defs.md#lifecyclepolicydetailoutputtypedef) 
3. See [:material-code-braces: LifecyclePolicyResourceSelectionTypeDef](./type_defs.md#lifecyclepolicyresourceselectiontypedef) 
4. See [:material-code-brackets: LifecyclePolicyStatusType](./literals.md#lifecyclepolicystatustype) 
5. See [:material-code-braces: CreateLifecyclePolicyResponseTypeDef](./type_defs.md#createlifecyclepolicyresponsetypedef) 


```python
# create_lifecycle_policy method usage example with argument unpacking

kwargs: CreateLifecyclePolicyRequestRequestTypeDef = {  # (1)
    "name": ...,
    "executionRole": ...,
    "resourceType": ...,
    "policyDetails": ...,
    "resourceSelection": ...,
    "clientToken": ...,
}

parent.create_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: CreateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#createlifecyclepolicyrequestrequesttypedef) 

### create\_workflow

Create a new workflow or a new version of an existing workflow.

Type annotations and code completion for `#!python session.create_client("imagebuilder").create_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/create_workflow.html)

```python
# create_workflow method definition

await def create_workflow(
    self,
    *,
    name: str,
    semanticVersion: str,
    clientToken: str,
    type: WorkflowTypeType,  # (1)
    description: str = ...,
    changeDescription: str = ...,
    data: str = ...,
    uri: str = ...,
    kmsKeyId: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateWorkflowResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WorkflowTypeType](./literals.md#workflowtypetype) 
2. See [:material-code-braces: CreateWorkflowResponseTypeDef](./type_defs.md#createworkflowresponsetypedef) 


```python
# create_workflow method usage example with argument unpacking

kwargs: CreateWorkflowRequestRequestTypeDef = {  # (1)
    "name": ...,
    "semanticVersion": ...,
    "clientToken": ...,
    "type": ...,
}

parent.create_workflow(**kwargs)
```

1. See [:material-code-braces: CreateWorkflowRequestRequestTypeDef](./type_defs.md#createworkflowrequestrequesttypedef) 

### delete\_component

Deletes a component build version.

Type annotations and code completion for `#!python session.create_client("imagebuilder").delete_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/delete_component.html)

```python
# delete_component method definition

await def delete_component(
    self,
    *,
    componentBuildVersionArn: str,
) -> DeleteComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteComponentResponseTypeDef](./type_defs.md#deletecomponentresponsetypedef) 


```python
# delete_component method usage example with argument unpacking

kwargs: DeleteComponentRequestRequestTypeDef = {  # (1)
    "componentBuildVersionArn": ...,
}

parent.delete_component(**kwargs)
```

1. See [:material-code-braces: DeleteComponentRequestRequestTypeDef](./type_defs.md#deletecomponentrequestrequesttypedef) 

### delete\_container\_recipe

Deletes a container recipe.

Type annotations and code completion for `#!python session.create_client("imagebuilder").delete_container_recipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/delete_container_recipe.html)

```python
# delete_container_recipe method definition

await def delete_container_recipe(
    self,
    *,
    containerRecipeArn: str,
) -> DeleteContainerRecipeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteContainerRecipeResponseTypeDef](./type_defs.md#deletecontainerreciperesponsetypedef) 


```python
# delete_container_recipe method usage example with argument unpacking

kwargs: DeleteContainerRecipeRequestRequestTypeDef = {  # (1)
    "containerRecipeArn": ...,
}

parent.delete_container_recipe(**kwargs)
```

1. See [:material-code-braces: DeleteContainerRecipeRequestRequestTypeDef](./type_defs.md#deletecontainerreciperequestrequesttypedef) 

### delete\_distribution\_configuration

Deletes a distribution configuration.

Type annotations and code completion for `#!python session.create_client("imagebuilder").delete_distribution_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/delete_distribution_configuration.html)

```python
# delete_distribution_configuration method definition

await def delete_distribution_configuration(
    self,
    *,
    distributionConfigurationArn: str,
) -> DeleteDistributionConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDistributionConfigurationResponseTypeDef](./type_defs.md#deletedistributionconfigurationresponsetypedef) 


```python
# delete_distribution_configuration method usage example with argument unpacking

kwargs: DeleteDistributionConfigurationRequestRequestTypeDef = {  # (1)
    "distributionConfigurationArn": ...,
}

parent.delete_distribution_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteDistributionConfigurationRequestRequestTypeDef](./type_defs.md#deletedistributionconfigurationrequestrequesttypedef) 

### delete\_image

Deletes an Image Builder image resource.

Type annotations and code completion for `#!python session.create_client("imagebuilder").delete_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/delete_image.html)

```python
# delete_image method definition

await def delete_image(
    self,
    *,
    imageBuildVersionArn: str,
) -> DeleteImageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteImageResponseTypeDef](./type_defs.md#deleteimageresponsetypedef) 


```python
# delete_image method usage example with argument unpacking

kwargs: DeleteImageRequestRequestTypeDef = {  # (1)
    "imageBuildVersionArn": ...,
}

parent.delete_image(**kwargs)
```

1. See [:material-code-braces: DeleteImageRequestRequestTypeDef](./type_defs.md#deleteimagerequestrequesttypedef) 

### delete\_image\_pipeline

Deletes an image pipeline.

Type annotations and code completion for `#!python session.create_client("imagebuilder").delete_image_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/delete_image_pipeline.html)

```python
# delete_image_pipeline method definition

await def delete_image_pipeline(
    self,
    *,
    imagePipelineArn: str,
) -> DeleteImagePipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteImagePipelineResponseTypeDef](./type_defs.md#deleteimagepipelineresponsetypedef) 


```python
# delete_image_pipeline method usage example with argument unpacking

kwargs: DeleteImagePipelineRequestRequestTypeDef = {  # (1)
    "imagePipelineArn": ...,
}

parent.delete_image_pipeline(**kwargs)
```

1. See [:material-code-braces: DeleteImagePipelineRequestRequestTypeDef](./type_defs.md#deleteimagepipelinerequestrequesttypedef) 

### delete\_image\_recipe

Deletes an image recipe.

Type annotations and code completion for `#!python session.create_client("imagebuilder").delete_image_recipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/delete_image_recipe.html)

```python
# delete_image_recipe method definition

await def delete_image_recipe(
    self,
    *,
    imageRecipeArn: str,
) -> DeleteImageRecipeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteImageRecipeResponseTypeDef](./type_defs.md#deleteimagereciperesponsetypedef) 


```python
# delete_image_recipe method usage example with argument unpacking

kwargs: DeleteImageRecipeRequestRequestTypeDef = {  # (1)
    "imageRecipeArn": ...,
}

parent.delete_image_recipe(**kwargs)
```

1. See [:material-code-braces: DeleteImageRecipeRequestRequestTypeDef](./type_defs.md#deleteimagereciperequestrequesttypedef) 

### delete\_infrastructure\_configuration

Deletes an infrastructure configuration.

Type annotations and code completion for `#!python session.create_client("imagebuilder").delete_infrastructure_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/delete_infrastructure_configuration.html)

```python
# delete_infrastructure_configuration method definition

await def delete_infrastructure_configuration(
    self,
    *,
    infrastructureConfigurationArn: str,
) -> DeleteInfrastructureConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteInfrastructureConfigurationResponseTypeDef](./type_defs.md#deleteinfrastructureconfigurationresponsetypedef) 


```python
# delete_infrastructure_configuration method usage example with argument unpacking

kwargs: DeleteInfrastructureConfigurationRequestRequestTypeDef = {  # (1)
    "infrastructureConfigurationArn": ...,
}

parent.delete_infrastructure_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteInfrastructureConfigurationRequestRequestTypeDef](./type_defs.md#deleteinfrastructureconfigurationrequestrequesttypedef) 

### delete\_lifecycle\_policy

Delete the specified lifecycle policy resource.

Type annotations and code completion for `#!python session.create_client("imagebuilder").delete_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/delete_lifecycle_policy.html)

```python
# delete_lifecycle_policy method definition

await def delete_lifecycle_policy(
    self,
    *,
    lifecyclePolicyArn: str,
) -> DeleteLifecyclePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteLifecyclePolicyResponseTypeDef](./type_defs.md#deletelifecyclepolicyresponsetypedef) 


```python
# delete_lifecycle_policy method usage example with argument unpacking

kwargs: DeleteLifecyclePolicyRequestRequestTypeDef = {  # (1)
    "lifecyclePolicyArn": ...,
}

parent.delete_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: DeleteLifecyclePolicyRequestRequestTypeDef](./type_defs.md#deletelifecyclepolicyrequestrequesttypedef) 

### delete\_workflow

Deletes a specific workflow resource.

Type annotations and code completion for `#!python session.create_client("imagebuilder").delete_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/delete_workflow.html)

```python
# delete_workflow method definition

await def delete_workflow(
    self,
    *,
    workflowBuildVersionArn: str,
) -> DeleteWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWorkflowResponseTypeDef](./type_defs.md#deleteworkflowresponsetypedef) 


```python
# delete_workflow method usage example with argument unpacking

kwargs: DeleteWorkflowRequestRequestTypeDef = {  # (1)
    "workflowBuildVersionArn": ...,
}

parent.delete_workflow(**kwargs)
```

1. See [:material-code-braces: DeleteWorkflowRequestRequestTypeDef](./type_defs.md#deleteworkflowrequestrequesttypedef) 

### get\_component

Gets a component object.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_component.html)

```python
# get_component method definition

await def get_component(
    self,
    *,
    componentBuildVersionArn: str,
) -> GetComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComponentResponseTypeDef](./type_defs.md#getcomponentresponsetypedef) 


```python
# get_component method usage example with argument unpacking

kwargs: GetComponentRequestRequestTypeDef = {  # (1)
    "componentBuildVersionArn": ...,
}

parent.get_component(**kwargs)
```

1. See [:material-code-braces: GetComponentRequestRequestTypeDef](./type_defs.md#getcomponentrequestrequesttypedef) 

### get\_component\_policy

Gets a component policy.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_component_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_component_policy.html)

```python
# get_component_policy method definition

await def get_component_policy(
    self,
    *,
    componentArn: str,
) -> GetComponentPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetComponentPolicyResponseTypeDef](./type_defs.md#getcomponentpolicyresponsetypedef) 


```python
# get_component_policy method usage example with argument unpacking

kwargs: GetComponentPolicyRequestRequestTypeDef = {  # (1)
    "componentArn": ...,
}

parent.get_component_policy(**kwargs)
```

1. See [:material-code-braces: GetComponentPolicyRequestRequestTypeDef](./type_defs.md#getcomponentpolicyrequestrequesttypedef) 

### get\_container\_recipe

Retrieves a container recipe.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_container_recipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_container_recipe.html)

```python
# get_container_recipe method definition

await def get_container_recipe(
    self,
    *,
    containerRecipeArn: str,
) -> GetContainerRecipeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContainerRecipeResponseTypeDef](./type_defs.md#getcontainerreciperesponsetypedef) 


```python
# get_container_recipe method usage example with argument unpacking

kwargs: GetContainerRecipeRequestRequestTypeDef = {  # (1)
    "containerRecipeArn": ...,
}

parent.get_container_recipe(**kwargs)
```

1. See [:material-code-braces: GetContainerRecipeRequestRequestTypeDef](./type_defs.md#getcontainerreciperequestrequesttypedef) 

### get\_container\_recipe\_policy

Retrieves the policy for a container recipe.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_container_recipe_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_container_recipe_policy.html)

```python
# get_container_recipe_policy method definition

await def get_container_recipe_policy(
    self,
    *,
    containerRecipeArn: str,
) -> GetContainerRecipePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetContainerRecipePolicyResponseTypeDef](./type_defs.md#getcontainerrecipepolicyresponsetypedef) 


```python
# get_container_recipe_policy method usage example with argument unpacking

kwargs: GetContainerRecipePolicyRequestRequestTypeDef = {  # (1)
    "containerRecipeArn": ...,
}

parent.get_container_recipe_policy(**kwargs)
```

1. See [:material-code-braces: GetContainerRecipePolicyRequestRequestTypeDef](./type_defs.md#getcontainerrecipepolicyrequestrequesttypedef) 

### get\_distribution\_configuration

Gets a distribution configuration.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_distribution_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_distribution_configuration.html)

```python
# get_distribution_configuration method definition

await def get_distribution_configuration(
    self,
    *,
    distributionConfigurationArn: str,
) -> GetDistributionConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDistributionConfigurationResponseTypeDef](./type_defs.md#getdistributionconfigurationresponsetypedef) 


```python
# get_distribution_configuration method usage example with argument unpacking

kwargs: GetDistributionConfigurationRequestRequestTypeDef = {  # (1)
    "distributionConfigurationArn": ...,
}

parent.get_distribution_configuration(**kwargs)
```

1. See [:material-code-braces: GetDistributionConfigurationRequestRequestTypeDef](./type_defs.md#getdistributionconfigurationrequestrequesttypedef) 

### get\_image

Gets an image.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_image.html)

```python
# get_image method definition

await def get_image(
    self,
    *,
    imageBuildVersionArn: str,
) -> GetImageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImageResponseTypeDef](./type_defs.md#getimageresponsetypedef) 


```python
# get_image method usage example with argument unpacking

kwargs: GetImageRequestRequestTypeDef = {  # (1)
    "imageBuildVersionArn": ...,
}

parent.get_image(**kwargs)
```

1. See [:material-code-braces: GetImageRequestRequestTypeDef](./type_defs.md#getimagerequestrequesttypedef) 

### get\_image\_pipeline

Gets an image pipeline.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_image_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_image_pipeline.html)

```python
# get_image_pipeline method definition

await def get_image_pipeline(
    self,
    *,
    imagePipelineArn: str,
) -> GetImagePipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImagePipelineResponseTypeDef](./type_defs.md#getimagepipelineresponsetypedef) 


```python
# get_image_pipeline method usage example with argument unpacking

kwargs: GetImagePipelineRequestRequestTypeDef = {  # (1)
    "imagePipelineArn": ...,
}

parent.get_image_pipeline(**kwargs)
```

1. See [:material-code-braces: GetImagePipelineRequestRequestTypeDef](./type_defs.md#getimagepipelinerequestrequesttypedef) 

### get\_image\_policy

Gets an image policy.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_image_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_image_policy.html)

```python
# get_image_policy method definition

await def get_image_policy(
    self,
    *,
    imageArn: str,
) -> GetImagePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImagePolicyResponseTypeDef](./type_defs.md#getimagepolicyresponsetypedef) 


```python
# get_image_policy method usage example with argument unpacking

kwargs: GetImagePolicyRequestRequestTypeDef = {  # (1)
    "imageArn": ...,
}

parent.get_image_policy(**kwargs)
```

1. See [:material-code-braces: GetImagePolicyRequestRequestTypeDef](./type_defs.md#getimagepolicyrequestrequesttypedef) 

### get\_image\_recipe

Gets an image recipe.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_image_recipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_image_recipe.html)

```python
# get_image_recipe method definition

await def get_image_recipe(
    self,
    *,
    imageRecipeArn: str,
) -> GetImageRecipeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImageRecipeResponseTypeDef](./type_defs.md#getimagereciperesponsetypedef) 


```python
# get_image_recipe method usage example with argument unpacking

kwargs: GetImageRecipeRequestRequestTypeDef = {  # (1)
    "imageRecipeArn": ...,
}

parent.get_image_recipe(**kwargs)
```

1. See [:material-code-braces: GetImageRecipeRequestRequestTypeDef](./type_defs.md#getimagereciperequestrequesttypedef) 

### get\_image\_recipe\_policy

Gets an image recipe policy.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_image_recipe_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_image_recipe_policy.html)

```python
# get_image_recipe_policy method definition

await def get_image_recipe_policy(
    self,
    *,
    imageRecipeArn: str,
) -> GetImageRecipePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImageRecipePolicyResponseTypeDef](./type_defs.md#getimagerecipepolicyresponsetypedef) 


```python
# get_image_recipe_policy method usage example with argument unpacking

kwargs: GetImageRecipePolicyRequestRequestTypeDef = {  # (1)
    "imageRecipeArn": ...,
}

parent.get_image_recipe_policy(**kwargs)
```

1. See [:material-code-braces: GetImageRecipePolicyRequestRequestTypeDef](./type_defs.md#getimagerecipepolicyrequestrequesttypedef) 

### get\_infrastructure\_configuration

Gets an infrastructure configuration.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_infrastructure_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_infrastructure_configuration.html)

```python
# get_infrastructure_configuration method definition

await def get_infrastructure_configuration(
    self,
    *,
    infrastructureConfigurationArn: str,
) -> GetInfrastructureConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInfrastructureConfigurationResponseTypeDef](./type_defs.md#getinfrastructureconfigurationresponsetypedef) 


```python
# get_infrastructure_configuration method usage example with argument unpacking

kwargs: GetInfrastructureConfigurationRequestRequestTypeDef = {  # (1)
    "infrastructureConfigurationArn": ...,
}

parent.get_infrastructure_configuration(**kwargs)
```

1. See [:material-code-braces: GetInfrastructureConfigurationRequestRequestTypeDef](./type_defs.md#getinfrastructureconfigurationrequestrequesttypedef) 

### get\_lifecycle\_execution

Get the runtime information that was logged for a specific runtime instance of
the lifecycle policy.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_lifecycle_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_lifecycle_execution.html)

```python
# get_lifecycle_execution method definition

await def get_lifecycle_execution(
    self,
    *,
    lifecycleExecutionId: str,
) -> GetLifecycleExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLifecycleExecutionResponseTypeDef](./type_defs.md#getlifecycleexecutionresponsetypedef) 


```python
# get_lifecycle_execution method usage example with argument unpacking

kwargs: GetLifecycleExecutionRequestRequestTypeDef = {  # (1)
    "lifecycleExecutionId": ...,
}

parent.get_lifecycle_execution(**kwargs)
```

1. See [:material-code-braces: GetLifecycleExecutionRequestRequestTypeDef](./type_defs.md#getlifecycleexecutionrequestrequesttypedef) 

### get\_lifecycle\_policy

Get details for the specified image lifecycle policy.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_lifecycle_policy.html)

```python
# get_lifecycle_policy method definition

await def get_lifecycle_policy(
    self,
    *,
    lifecyclePolicyArn: str,
) -> GetLifecyclePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLifecyclePolicyResponseTypeDef](./type_defs.md#getlifecyclepolicyresponsetypedef) 


```python
# get_lifecycle_policy method usage example with argument unpacking

kwargs: GetLifecyclePolicyRequestRequestTypeDef = {  # (1)
    "lifecyclePolicyArn": ...,
}

parent.get_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: GetLifecyclePolicyRequestRequestTypeDef](./type_defs.md#getlifecyclepolicyrequestrequesttypedef) 

### get\_marketplace\_resource

Verify the subscription and perform resource dependency checks on the requested
Amazon Web Services Marketplace resource.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_marketplace_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_marketplace_resource.html)

```python
# get_marketplace_resource method definition

await def get_marketplace_resource(
    self,
    *,
    resourceType: MarketplaceResourceTypeType,  # (1)
    resourceArn: str,
    resourceLocation: str = ...,
) -> GetMarketplaceResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MarketplaceResourceTypeType](./literals.md#marketplaceresourcetypetype) 
2. See [:material-code-braces: GetMarketplaceResourceResponseTypeDef](./type_defs.md#getmarketplaceresourceresponsetypedef) 


```python
# get_marketplace_resource method usage example with argument unpacking

kwargs: GetMarketplaceResourceRequestRequestTypeDef = {  # (1)
    "resourceType": ...,
    "resourceArn": ...,
}

parent.get_marketplace_resource(**kwargs)
```

1. See [:material-code-braces: GetMarketplaceResourceRequestRequestTypeDef](./type_defs.md#getmarketplaceresourcerequestrequesttypedef) 

### get\_workflow

Get a workflow resource object.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_workflow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_workflow.html)

```python
# get_workflow method definition

await def get_workflow(
    self,
    *,
    workflowBuildVersionArn: str,
) -> GetWorkflowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowResponseTypeDef](./type_defs.md#getworkflowresponsetypedef) 


```python
# get_workflow method usage example with argument unpacking

kwargs: GetWorkflowRequestRequestTypeDef = {  # (1)
    "workflowBuildVersionArn": ...,
}

parent.get_workflow(**kwargs)
```

1. See [:material-code-braces: GetWorkflowRequestRequestTypeDef](./type_defs.md#getworkflowrequestrequesttypedef) 

### get\_workflow\_execution

Get the runtime information that was logged for a specific runtime instance of
the workflow.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_workflow_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_workflow_execution.html)

```python
# get_workflow_execution method definition

await def get_workflow_execution(
    self,
    *,
    workflowExecutionId: str,
) -> GetWorkflowExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowExecutionResponseTypeDef](./type_defs.md#getworkflowexecutionresponsetypedef) 


```python
# get_workflow_execution method usage example with argument unpacking

kwargs: GetWorkflowExecutionRequestRequestTypeDef = {  # (1)
    "workflowExecutionId": ...,
}

parent.get_workflow_execution(**kwargs)
```

1. See [:material-code-braces: GetWorkflowExecutionRequestRequestTypeDef](./type_defs.md#getworkflowexecutionrequestrequesttypedef) 

### get\_workflow\_step\_execution

Get the runtime information that was logged for a specific runtime instance of
the workflow step.

Type annotations and code completion for `#!python session.create_client("imagebuilder").get_workflow_step_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/get_workflow_step_execution.html)

```python
# get_workflow_step_execution method definition

await def get_workflow_step_execution(
    self,
    *,
    stepExecutionId: str,
) -> GetWorkflowStepExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkflowStepExecutionResponseTypeDef](./type_defs.md#getworkflowstepexecutionresponsetypedef) 


```python
# get_workflow_step_execution method usage example with argument unpacking

kwargs: GetWorkflowStepExecutionRequestRequestTypeDef = {  # (1)
    "stepExecutionId": ...,
}

parent.get_workflow_step_execution(**kwargs)
```

1. See [:material-code-braces: GetWorkflowStepExecutionRequestRequestTypeDef](./type_defs.md#getworkflowstepexecutionrequestrequesttypedef) 

### import\_component

Imports a component and transforms its data into a component document.

Type annotations and code completion for `#!python session.create_client("imagebuilder").import_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/import_component.html)

```python
# import_component method definition

await def import_component(
    self,
    *,
    name: str,
    semanticVersion: str,
    type: ComponentTypeType,  # (1)
    format: ComponentFormatType,  # (2)
    platform: PlatformType,  # (3)
    clientToken: str,
    description: str = ...,
    changeDescription: str = ...,
    data: str = ...,
    uri: str = ...,
    kmsKeyId: str = ...,
    tags: Mapping[str, str] = ...,
) -> ImportComponentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ComponentTypeType](./literals.md#componenttypetype) 
2. See [:material-code-brackets: ComponentFormatType](./literals.md#componentformattype) 
3. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
4. See [:material-code-braces: ImportComponentResponseTypeDef](./type_defs.md#importcomponentresponsetypedef) 


```python
# import_component method usage example with argument unpacking

kwargs: ImportComponentRequestRequestTypeDef = {  # (1)
    "name": ...,
    "semanticVersion": ...,
    "type": ...,
    "format": ...,
    "platform": ...,
    "clientToken": ...,
}

parent.import_component(**kwargs)
```

1. See [:material-code-braces: ImportComponentRequestRequestTypeDef](./type_defs.md#importcomponentrequestrequesttypedef) 

### import\_vm\_image

When you export your virtual machine (VM) from its virtualization environment,
that process creates a set of one or more disk container files that act as
snapshots of your VM's environment, settings, and data.

Type annotations and code completion for `#!python session.create_client("imagebuilder").import_vm_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/import_vm_image.html)

```python
# import_vm_image method definition

await def import_vm_image(
    self,
    *,
    name: str,
    semanticVersion: str,
    platform: PlatformType,  # (1)
    vmImportTaskId: str,
    clientToken: str,
    description: str = ...,
    osVersion: str = ...,
    tags: Mapping[str, str] = ...,
) -> ImportVmImageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: ImportVmImageResponseTypeDef](./type_defs.md#importvmimageresponsetypedef) 


```python
# import_vm_image method usage example with argument unpacking

kwargs: ImportVmImageRequestRequestTypeDef = {  # (1)
    "name": ...,
    "semanticVersion": ...,
    "platform": ...,
    "vmImportTaskId": ...,
    "clientToken": ...,
}

parent.import_vm_image(**kwargs)
```

1. See [:material-code-braces: ImportVmImageRequestRequestTypeDef](./type_defs.md#importvmimagerequestrequesttypedef) 

### list\_component\_build\_versions

Returns the list of component build versions for the specified component
version Amazon Resource Name (ARN).

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_component_build_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_component_build_versions.html)

```python
# list_component_build_versions method definition

await def list_component_build_versions(
    self,
    *,
    componentVersionArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListComponentBuildVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListComponentBuildVersionsResponseTypeDef](./type_defs.md#listcomponentbuildversionsresponsetypedef) 


```python
# list_component_build_versions method usage example with argument unpacking

kwargs: ListComponentBuildVersionsRequestRequestTypeDef = {  # (1)
    "componentVersionArn": ...,
}

parent.list_component_build_versions(**kwargs)
```

1. See [:material-code-braces: ListComponentBuildVersionsRequestRequestTypeDef](./type_defs.md#listcomponentbuildversionsrequestrequesttypedef) 

### list\_components

Returns the list of components that can be filtered by name, or by using the
listed <code>filters</code> to streamline results.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_components.html)

```python
# list_components method definition

await def list_components(
    self,
    *,
    owner: OwnershipType = ...,  # (1)
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    byName: bool = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListComponentsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


```python
# list_components method usage example with argument unpacking

kwargs: ListComponentsRequestRequestTypeDef = {  # (1)
    "owner": ...,
}

parent.list_components(**kwargs)
```

1. See [:material-code-braces: ListComponentsRequestRequestTypeDef](./type_defs.md#listcomponentsrequestrequesttypedef) 

### list\_container\_recipes

Returns a list of container recipes.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_container_recipes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_container_recipes.html)

```python
# list_container_recipes method definition

await def list_container_recipes(
    self,
    *,
    owner: OwnershipType = ...,  # (1)
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListContainerRecipesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: ListContainerRecipesResponseTypeDef](./type_defs.md#listcontainerrecipesresponsetypedef) 


```python
# list_container_recipes method usage example with argument unpacking

kwargs: ListContainerRecipesRequestRequestTypeDef = {  # (1)
    "owner": ...,
}

parent.list_container_recipes(**kwargs)
```

1. See [:material-code-braces: ListContainerRecipesRequestRequestTypeDef](./type_defs.md#listcontainerrecipesrequestrequesttypedef) 

### list\_distribution\_configurations

Returns a list of distribution configurations.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_distribution_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_distribution_configurations.html)

```python
# list_distribution_configurations method definition

await def list_distribution_configurations(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDistributionConfigurationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListDistributionConfigurationsResponseTypeDef](./type_defs.md#listdistributionconfigurationsresponsetypedef) 


```python
# list_distribution_configurations method usage example with argument unpacking

kwargs: ListDistributionConfigurationsRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_distribution_configurations(**kwargs)
```

1. See [:material-code-braces: ListDistributionConfigurationsRequestRequestTypeDef](./type_defs.md#listdistributionconfigurationsrequestrequesttypedef) 

### list\_image\_build\_versions

Returns a list of image build versions.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_image_build_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_image_build_versions.html)

```python
# list_image_build_versions method definition

await def list_image_build_versions(
    self,
    *,
    imageVersionArn: str,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListImageBuildVersionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListImageBuildVersionsResponseTypeDef](./type_defs.md#listimagebuildversionsresponsetypedef) 


```python
# list_image_build_versions method usage example with argument unpacking

kwargs: ListImageBuildVersionsRequestRequestTypeDef = {  # (1)
    "imageVersionArn": ...,
}

parent.list_image_build_versions(**kwargs)
```

1. See [:material-code-braces: ListImageBuildVersionsRequestRequestTypeDef](./type_defs.md#listimagebuildversionsrequestrequesttypedef) 

### list\_image\_packages

List the Packages that are associated with an Image Build Version, as
determined by Amazon Web Services Systems Manager Inventory at build time.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_image_packages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_image_packages.html)

```python
# list_image_packages method definition

await def list_image_packages(
    self,
    *,
    imageBuildVersionArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListImagePackagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListImagePackagesResponseTypeDef](./type_defs.md#listimagepackagesresponsetypedef) 


```python
# list_image_packages method usage example with argument unpacking

kwargs: ListImagePackagesRequestRequestTypeDef = {  # (1)
    "imageBuildVersionArn": ...,
}

parent.list_image_packages(**kwargs)
```

1. See [:material-code-braces: ListImagePackagesRequestRequestTypeDef](./type_defs.md#listimagepackagesrequestrequesttypedef) 

### list\_image\_pipeline\_images

Returns a list of images created by the specified pipeline.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_image_pipeline_images` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_image_pipeline_images.html)

```python
# list_image_pipeline_images method definition

await def list_image_pipeline_images(
    self,
    *,
    imagePipelineArn: str,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListImagePipelineImagesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListImagePipelineImagesResponseTypeDef](./type_defs.md#listimagepipelineimagesresponsetypedef) 


```python
# list_image_pipeline_images method usage example with argument unpacking

kwargs: ListImagePipelineImagesRequestRequestTypeDef = {  # (1)
    "imagePipelineArn": ...,
}

parent.list_image_pipeline_images(**kwargs)
```

1. See [:material-code-braces: ListImagePipelineImagesRequestRequestTypeDef](./type_defs.md#listimagepipelineimagesrequestrequesttypedef) 

### list\_image\_pipelines

Returns a list of image pipelines.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_image_pipelines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_image_pipelines.html)

```python
# list_image_pipelines method definition

await def list_image_pipelines(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListImagePipelinesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListImagePipelinesResponseTypeDef](./type_defs.md#listimagepipelinesresponsetypedef) 


```python
# list_image_pipelines method usage example with argument unpacking

kwargs: ListImagePipelinesRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_image_pipelines(**kwargs)
```

1. See [:material-code-braces: ListImagePipelinesRequestRequestTypeDef](./type_defs.md#listimagepipelinesrequestrequesttypedef) 

### list\_image\_recipes

Returns a list of image recipes.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_image_recipes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_image_recipes.html)

```python
# list_image_recipes method definition

await def list_image_recipes(
    self,
    *,
    owner: OwnershipType = ...,  # (1)
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListImageRecipesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: ListImageRecipesResponseTypeDef](./type_defs.md#listimagerecipesresponsetypedef) 


```python
# list_image_recipes method usage example with argument unpacking

kwargs: ListImageRecipesRequestRequestTypeDef = {  # (1)
    "owner": ...,
}

parent.list_image_recipes(**kwargs)
```

1. See [:material-code-braces: ListImageRecipesRequestRequestTypeDef](./type_defs.md#listimagerecipesrequestrequesttypedef) 

### list\_image\_scan\_finding\_aggregations

Returns a list of image scan aggregations for your account.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_image_scan_finding_aggregations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_image_scan_finding_aggregations.html)

```python
# list_image_scan_finding_aggregations method definition

await def list_image_scan_finding_aggregations(
    self,
    *,
    filter: FilterTypeDef = ...,  # (1)
    nextToken: str = ...,
) -> ListImageScanFindingAggregationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListImageScanFindingAggregationsResponseTypeDef](./type_defs.md#listimagescanfindingaggregationsresponsetypedef) 


```python
# list_image_scan_finding_aggregations method usage example with argument unpacking

kwargs: ListImageScanFindingAggregationsRequestRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.list_image_scan_finding_aggregations(**kwargs)
```

1. See [:material-code-braces: ListImageScanFindingAggregationsRequestRequestTypeDef](./type_defs.md#listimagescanfindingaggregationsrequestrequesttypedef) 

### list\_image\_scan\_findings

Returns a list of image scan findings for your account.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_image_scan_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_image_scan_findings.html)

```python
# list_image_scan_findings method definition

await def list_image_scan_findings(
    self,
    *,
    filters: Sequence[ImageScanFindingsFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListImageScanFindingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ImageScanFindingsFilterTypeDef](./type_defs.md#imagescanfindingsfiltertypedef) 
2. See [:material-code-braces: ListImageScanFindingsResponseTypeDef](./type_defs.md#listimagescanfindingsresponsetypedef) 


```python
# list_image_scan_findings method usage example with argument unpacking

kwargs: ListImageScanFindingsRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_image_scan_findings(**kwargs)
```

1. See [:material-code-braces: ListImageScanFindingsRequestRequestTypeDef](./type_defs.md#listimagescanfindingsrequestrequesttypedef) 

### list\_images

Returns the list of images that you have access to.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_images` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_images.html)

```python
# list_images method definition

await def list_images(
    self,
    *,
    owner: OwnershipType = ...,  # (1)
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    byName: bool = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    includeDeprecated: bool = ...,
) -> ListImagesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: ListImagesResponseTypeDef](./type_defs.md#listimagesresponsetypedef) 


```python
# list_images method usage example with argument unpacking

kwargs: ListImagesRequestRequestTypeDef = {  # (1)
    "owner": ...,
}

parent.list_images(**kwargs)
```

1. See [:material-code-braces: ListImagesRequestRequestTypeDef](./type_defs.md#listimagesrequestrequesttypedef) 

### list\_infrastructure\_configurations

Returns a list of infrastructure configurations.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_infrastructure_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_infrastructure_configurations.html)

```python
# list_infrastructure_configurations method definition

await def list_infrastructure_configurations(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListInfrastructureConfigurationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListInfrastructureConfigurationsResponseTypeDef](./type_defs.md#listinfrastructureconfigurationsresponsetypedef) 


```python
# list_infrastructure_configurations method usage example with argument unpacking

kwargs: ListInfrastructureConfigurationsRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_infrastructure_configurations(**kwargs)
```

1. See [:material-code-braces: ListInfrastructureConfigurationsRequestRequestTypeDef](./type_defs.md#listinfrastructureconfigurationsrequestrequesttypedef) 

### list\_lifecycle\_execution\_resources

List resources that the runtime instance of the image lifecycle identified for
lifecycle actions.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_lifecycle_execution_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_lifecycle_execution_resources.html)

```python
# list_lifecycle_execution_resources method definition

await def list_lifecycle_execution_resources(
    self,
    *,
    lifecycleExecutionId: str,
    parentResourceId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListLifecycleExecutionResourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLifecycleExecutionResourcesResponseTypeDef](./type_defs.md#listlifecycleexecutionresourcesresponsetypedef) 


```python
# list_lifecycle_execution_resources method usage example with argument unpacking

kwargs: ListLifecycleExecutionResourcesRequestRequestTypeDef = {  # (1)
    "lifecycleExecutionId": ...,
}

parent.list_lifecycle_execution_resources(**kwargs)
```

1. See [:material-code-braces: ListLifecycleExecutionResourcesRequestRequestTypeDef](./type_defs.md#listlifecycleexecutionresourcesrequestrequesttypedef) 

### list\_lifecycle\_executions

Get the lifecycle runtime history for the specified resource.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_lifecycle_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_lifecycle_executions.html)

```python
# list_lifecycle_executions method definition

await def list_lifecycle_executions(
    self,
    *,
    resourceArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListLifecycleExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLifecycleExecutionsResponseTypeDef](./type_defs.md#listlifecycleexecutionsresponsetypedef) 


```python
# list_lifecycle_executions method usage example with argument unpacking

kwargs: ListLifecycleExecutionsRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_lifecycle_executions(**kwargs)
```

1. See [:material-code-braces: ListLifecycleExecutionsRequestRequestTypeDef](./type_defs.md#listlifecycleexecutionsrequestrequesttypedef) 

### list\_lifecycle\_policies

Get a list of lifecycle policies in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_lifecycle_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_lifecycle_policies.html)

```python
# list_lifecycle_policies method definition

await def list_lifecycle_policies(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListLifecyclePoliciesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListLifecyclePoliciesResponseTypeDef](./type_defs.md#listlifecyclepoliciesresponsetypedef) 


```python
# list_lifecycle_policies method usage example with argument unpacking

kwargs: ListLifecyclePoliciesRequestRequestTypeDef = {  # (1)
    "filters": ...,
}

parent.list_lifecycle_policies(**kwargs)
```

1. See [:material-code-braces: ListLifecyclePoliciesRequestRequestTypeDef](./type_defs.md#listlifecyclepoliciesrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns the list of tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_waiting\_workflow\_steps

Get a list of workflow steps that are waiting for action for workflows in your
Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_waiting_workflow_steps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_waiting_workflow_steps.html)

```python
# list_waiting_workflow_steps method definition

await def list_waiting_workflow_steps(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWaitingWorkflowStepsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWaitingWorkflowStepsResponseTypeDef](./type_defs.md#listwaitingworkflowstepsresponsetypedef) 


```python
# list_waiting_workflow_steps method usage example with argument unpacking

kwargs: ListWaitingWorkflowStepsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_waiting_workflow_steps(**kwargs)
```

1. See [:material-code-braces: ListWaitingWorkflowStepsRequestRequestTypeDef](./type_defs.md#listwaitingworkflowstepsrequestrequesttypedef) 

### list\_workflow\_build\_versions

Returns a list of build versions for a specific workflow resource.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_workflow_build_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_workflow_build_versions.html)

```python
# list_workflow_build_versions method definition

await def list_workflow_build_versions(
    self,
    *,
    workflowVersionArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkflowBuildVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkflowBuildVersionsResponseTypeDef](./type_defs.md#listworkflowbuildversionsresponsetypedef) 


```python
# list_workflow_build_versions method usage example with argument unpacking

kwargs: ListWorkflowBuildVersionsRequestRequestTypeDef = {  # (1)
    "workflowVersionArn": ...,
}

parent.list_workflow_build_versions(**kwargs)
```

1. See [:material-code-braces: ListWorkflowBuildVersionsRequestRequestTypeDef](./type_defs.md#listworkflowbuildversionsrequestrequesttypedef) 

### list\_workflow\_executions

Returns a list of workflow runtime instance metadata objects for a specific
image build version.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_workflow_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_workflow_executions.html)

```python
# list_workflow_executions method definition

await def list_workflow_executions(
    self,
    *,
    imageBuildVersionArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkflowExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkflowExecutionsResponseTypeDef](./type_defs.md#listworkflowexecutionsresponsetypedef) 


```python
# list_workflow_executions method usage example with argument unpacking

kwargs: ListWorkflowExecutionsRequestRequestTypeDef = {  # (1)
    "imageBuildVersionArn": ...,
}

parent.list_workflow_executions(**kwargs)
```

1. See [:material-code-braces: ListWorkflowExecutionsRequestRequestTypeDef](./type_defs.md#listworkflowexecutionsrequestrequesttypedef) 

### list\_workflow\_step\_executions

Returns runtime data for each step in a runtime instance of the workflow that
you specify in the request.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_workflow_step_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_workflow_step_executions.html)

```python
# list_workflow_step_executions method definition

await def list_workflow_step_executions(
    self,
    *,
    workflowExecutionId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkflowStepExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkflowStepExecutionsResponseTypeDef](./type_defs.md#listworkflowstepexecutionsresponsetypedef) 


```python
# list_workflow_step_executions method usage example with argument unpacking

kwargs: ListWorkflowStepExecutionsRequestRequestTypeDef = {  # (1)
    "workflowExecutionId": ...,
}

parent.list_workflow_step_executions(**kwargs)
```

1. See [:material-code-braces: ListWorkflowStepExecutionsRequestRequestTypeDef](./type_defs.md#listworkflowstepexecutionsrequestrequesttypedef) 

### list\_workflows

Lists workflow build versions based on filtering parameters.

Type annotations and code completion for `#!python session.create_client("imagebuilder").list_workflows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/list_workflows.html)

```python
# list_workflows method definition

await def list_workflows(
    self,
    *,
    owner: OwnershipType = ...,  # (1)
    filters: Sequence[FilterTypeDef] = ...,  # (2)
    byName: bool = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListWorkflowsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: ListWorkflowsResponseTypeDef](./type_defs.md#listworkflowsresponsetypedef) 


```python
# list_workflows method usage example with argument unpacking

kwargs: ListWorkflowsRequestRequestTypeDef = {  # (1)
    "owner": ...,
}

parent.list_workflows(**kwargs)
```

1. See [:material-code-braces: ListWorkflowsRequestRequestTypeDef](./type_defs.md#listworkflowsrequestrequesttypedef) 

### put\_component\_policy

Applies a policy to a component.

Type annotations and code completion for `#!python session.create_client("imagebuilder").put_component_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/put_component_policy.html)

```python
# put_component_policy method definition

await def put_component_policy(
    self,
    *,
    componentArn: str,
    policy: str,
) -> PutComponentPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutComponentPolicyResponseTypeDef](./type_defs.md#putcomponentpolicyresponsetypedef) 


```python
# put_component_policy method usage example with argument unpacking

kwargs: PutComponentPolicyRequestRequestTypeDef = {  # (1)
    "componentArn": ...,
    "policy": ...,
}

parent.put_component_policy(**kwargs)
```

1. See [:material-code-braces: PutComponentPolicyRequestRequestTypeDef](./type_defs.md#putcomponentpolicyrequestrequesttypedef) 

### put\_container\_recipe\_policy

Applies a policy to a container image.

Type annotations and code completion for `#!python session.create_client("imagebuilder").put_container_recipe_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/put_container_recipe_policy.html)

```python
# put_container_recipe_policy method definition

await def put_container_recipe_policy(
    self,
    *,
    containerRecipeArn: str,
    policy: str,
) -> PutContainerRecipePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutContainerRecipePolicyResponseTypeDef](./type_defs.md#putcontainerrecipepolicyresponsetypedef) 


```python
# put_container_recipe_policy method usage example with argument unpacking

kwargs: PutContainerRecipePolicyRequestRequestTypeDef = {  # (1)
    "containerRecipeArn": ...,
    "policy": ...,
}

parent.put_container_recipe_policy(**kwargs)
```

1. See [:material-code-braces: PutContainerRecipePolicyRequestRequestTypeDef](./type_defs.md#putcontainerrecipepolicyrequestrequesttypedef) 

### put\_image\_policy

Applies a policy to an image.

Type annotations and code completion for `#!python session.create_client("imagebuilder").put_image_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/put_image_policy.html)

```python
# put_image_policy method definition

await def put_image_policy(
    self,
    *,
    imageArn: str,
    policy: str,
) -> PutImagePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutImagePolicyResponseTypeDef](./type_defs.md#putimagepolicyresponsetypedef) 


```python
# put_image_policy method usage example with argument unpacking

kwargs: PutImagePolicyRequestRequestTypeDef = {  # (1)
    "imageArn": ...,
    "policy": ...,
}

parent.put_image_policy(**kwargs)
```

1. See [:material-code-braces: PutImagePolicyRequestRequestTypeDef](./type_defs.md#putimagepolicyrequestrequesttypedef) 

### put\_image\_recipe\_policy

Applies a policy to an image recipe.

Type annotations and code completion for `#!python session.create_client("imagebuilder").put_image_recipe_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/put_image_recipe_policy.html)

```python
# put_image_recipe_policy method definition

await def put_image_recipe_policy(
    self,
    *,
    imageRecipeArn: str,
    policy: str,
) -> PutImageRecipePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutImageRecipePolicyResponseTypeDef](./type_defs.md#putimagerecipepolicyresponsetypedef) 


```python
# put_image_recipe_policy method usage example with argument unpacking

kwargs: PutImageRecipePolicyRequestRequestTypeDef = {  # (1)
    "imageRecipeArn": ...,
    "policy": ...,
}

parent.put_image_recipe_policy(**kwargs)
```

1. See [:material-code-braces: PutImageRecipePolicyRequestRequestTypeDef](./type_defs.md#putimagerecipepolicyrequestrequesttypedef) 

### send\_workflow\_step\_action

Pauses or resumes image creation when the associated workflow runs a
<code>WaitForAction</code> step.

Type annotations and code completion for `#!python session.create_client("imagebuilder").send_workflow_step_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/send_workflow_step_action.html)

```python
# send_workflow_step_action method definition

await def send_workflow_step_action(
    self,
    *,
    stepExecutionId: str,
    imageBuildVersionArn: str,
    action: WorkflowStepActionTypeType,  # (1)
    clientToken: str,
    reason: str = ...,
) -> SendWorkflowStepActionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WorkflowStepActionTypeType](./literals.md#workflowstepactiontypetype) 
2. See [:material-code-braces: SendWorkflowStepActionResponseTypeDef](./type_defs.md#sendworkflowstepactionresponsetypedef) 


```python
# send_workflow_step_action method usage example with argument unpacking

kwargs: SendWorkflowStepActionRequestRequestTypeDef = {  # (1)
    "stepExecutionId": ...,
    "imageBuildVersionArn": ...,
    "action": ...,
    "clientToken": ...,
}

parent.send_workflow_step_action(**kwargs)
```

1. See [:material-code-braces: SendWorkflowStepActionRequestRequestTypeDef](./type_defs.md#sendworkflowstepactionrequestrequesttypedef) 

### start\_image\_pipeline\_execution

Manually triggers a pipeline to create an image.

Type annotations and code completion for `#!python session.create_client("imagebuilder").start_image_pipeline_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/start_image_pipeline_execution.html)

```python
# start_image_pipeline_execution method definition

await def start_image_pipeline_execution(
    self,
    *,
    imagePipelineArn: str,
    clientToken: str,
) -> StartImagePipelineExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartImagePipelineExecutionResponseTypeDef](./type_defs.md#startimagepipelineexecutionresponsetypedef) 


```python
# start_image_pipeline_execution method usage example with argument unpacking

kwargs: StartImagePipelineExecutionRequestRequestTypeDef = {  # (1)
    "imagePipelineArn": ...,
    "clientToken": ...,
}

parent.start_image_pipeline_execution(**kwargs)
```

1. See [:material-code-braces: StartImagePipelineExecutionRequestRequestTypeDef](./type_defs.md#startimagepipelineexecutionrequestrequesttypedef) 

### start\_resource\_state\_update

Begin asynchronous resource state update for lifecycle changes to the specified
image resources.

Type annotations and code completion for `#!python session.create_client("imagebuilder").start_resource_state_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/start_resource_state_update.html)

```python
# start_resource_state_update method definition

await def start_resource_state_update(
    self,
    *,
    resourceArn: str,
    state: ResourceStateTypeDef,  # (1)
    clientToken: str,
    executionRole: str = ...,
    includeResources: ResourceStateUpdateIncludeResourcesTypeDef = ...,  # (2)
    exclusionRules: ResourceStateUpdateExclusionRulesTypeDef = ...,  # (3)
    updateAt: TimestampTypeDef = ...,
) -> StartResourceStateUpdateResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ResourceStateTypeDef](./type_defs.md#resourcestatetypedef) 
2. See [:material-code-braces: ResourceStateUpdateIncludeResourcesTypeDef](./type_defs.md#resourcestateupdateincluderesourcestypedef) 
3. See [:material-code-braces: ResourceStateUpdateExclusionRulesTypeDef](./type_defs.md#resourcestateupdateexclusionrulestypedef) 
4. See [:material-code-braces: StartResourceStateUpdateResponseTypeDef](./type_defs.md#startresourcestateupdateresponsetypedef) 


```python
# start_resource_state_update method usage example with argument unpacking

kwargs: StartResourceStateUpdateRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "state": ...,
    "clientToken": ...,
}

parent.start_resource_state_update(**kwargs)
```

1. See [:material-code-braces: StartResourceStateUpdateRequestRequestTypeDef](./type_defs.md#startresourcestateupdaterequestrequesttypedef) 

### tag\_resource

Adds a tag to a resource.

Type annotations and code completion for `#!python session.create_client("imagebuilder").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a tag from a resource.

Type annotations and code completion for `#!python session.create_client("imagebuilder").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_distribution\_configuration

Updates a new distribution configuration.

Type annotations and code completion for `#!python session.create_client("imagebuilder").update_distribution_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/update_distribution_configuration.html)

```python
# update_distribution_configuration method definition

await def update_distribution_configuration(
    self,
    *,
    distributionConfigurationArn: str,
    distributions: Sequence[DistributionTypeDef],  # (1)
    clientToken: str,
    description: str = ...,
) -> UpdateDistributionConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DistributionTypeDef](./type_defs.md#distributiontypedef) 
2. See [:material-code-braces: UpdateDistributionConfigurationResponseTypeDef](./type_defs.md#updatedistributionconfigurationresponsetypedef) 


```python
# update_distribution_configuration method usage example with argument unpacking

kwargs: UpdateDistributionConfigurationRequestRequestTypeDef = {  # (1)
    "distributionConfigurationArn": ...,
    "distributions": ...,
    "clientToken": ...,
}

parent.update_distribution_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateDistributionConfigurationRequestRequestTypeDef](./type_defs.md#updatedistributionconfigurationrequestrequesttypedef) 

### update\_image\_pipeline

Updates an image pipeline.

Type annotations and code completion for `#!python session.create_client("imagebuilder").update_image_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/update_image_pipeline.html)

```python
# update_image_pipeline method definition

await def update_image_pipeline(
    self,
    *,
    imagePipelineArn: str,
    infrastructureConfigurationArn: str,
    clientToken: str,
    description: str = ...,
    imageRecipeArn: str = ...,
    containerRecipeArn: str = ...,
    distributionConfigurationArn: str = ...,
    imageTestsConfiguration: ImageTestsConfigurationTypeDef = ...,  # (1)
    enhancedImageMetadataEnabled: bool = ...,
    schedule: ScheduleTypeDef = ...,  # (2)
    status: PipelineStatusType = ...,  # (3)
    imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,  # (4)
    workflows: Sequence[WorkflowConfigurationTypeDef] = ...,  # (5)
    executionRole: str = ...,
) -> UpdateImagePipelineResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ImageTestsConfigurationTypeDef](./type_defs.md#imagetestsconfigurationtypedef) 
2. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
3. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
4. See [:material-code-braces: ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef) 
5. See [:material-code-braces: WorkflowConfigurationTypeDef](./type_defs.md#workflowconfigurationtypedef) 
6. See [:material-code-braces: UpdateImagePipelineResponseTypeDef](./type_defs.md#updateimagepipelineresponsetypedef) 


```python
# update_image_pipeline method usage example with argument unpacking

kwargs: UpdateImagePipelineRequestRequestTypeDef = {  # (1)
    "imagePipelineArn": ...,
    "infrastructureConfigurationArn": ...,
    "clientToken": ...,
}

parent.update_image_pipeline(**kwargs)
```

1. See [:material-code-braces: UpdateImagePipelineRequestRequestTypeDef](./type_defs.md#updateimagepipelinerequestrequesttypedef) 

### update\_infrastructure\_configuration

Updates a new infrastructure configuration.

Type annotations and code completion for `#!python session.create_client("imagebuilder").update_infrastructure_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/update_infrastructure_configuration.html)

```python
# update_infrastructure_configuration method definition

await def update_infrastructure_configuration(
    self,
    *,
    infrastructureConfigurationArn: str,
    instanceProfileName: str,
    clientToken: str,
    description: str = ...,
    instanceTypes: Sequence[str] = ...,
    securityGroupIds: Sequence[str] = ...,
    subnetId: str = ...,
    logging: LoggingTypeDef = ...,  # (1)
    keyPair: str = ...,
    terminateInstanceOnFailure: bool = ...,
    snsTopicArn: str = ...,
    resourceTags: Mapping[str, str] = ...,
    instanceMetadataOptions: InstanceMetadataOptionsTypeDef = ...,  # (2)
    placement: PlacementTypeDef = ...,  # (3)
) -> UpdateInfrastructureConfigurationResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
2. See [:material-code-braces: InstanceMetadataOptionsTypeDef](./type_defs.md#instancemetadataoptionstypedef) 
3. See [:material-code-braces: PlacementTypeDef](./type_defs.md#placementtypedef) 
4. See [:material-code-braces: UpdateInfrastructureConfigurationResponseTypeDef](./type_defs.md#updateinfrastructureconfigurationresponsetypedef) 


```python
# update_infrastructure_configuration method usage example with argument unpacking

kwargs: UpdateInfrastructureConfigurationRequestRequestTypeDef = {  # (1)
    "infrastructureConfigurationArn": ...,
    "instanceProfileName": ...,
    "clientToken": ...,
}

parent.update_infrastructure_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateInfrastructureConfigurationRequestRequestTypeDef](./type_defs.md#updateinfrastructureconfigurationrequestrequesttypedef) 

### update\_lifecycle\_policy

Update the specified lifecycle policy.

Type annotations and code completion for `#!python session.create_client("imagebuilder").update_lifecycle_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder/client/update_lifecycle_policy.html)

```python
# update_lifecycle_policy method definition

await def update_lifecycle_policy(
    self,
    *,
    lifecyclePolicyArn: str,
    executionRole: str,
    resourceType: LifecyclePolicyResourceTypeType,  # (1)
    policyDetails: Sequence[LifecyclePolicyDetailTypeDef],  # (2)
    resourceSelection: LifecyclePolicyResourceSelectionTypeDef,  # (3)
    clientToken: str,
    description: str = ...,
    status: LifecyclePolicyStatusType = ...,  # (4)
) -> UpdateLifecyclePolicyResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: LifecyclePolicyResourceTypeType](./literals.md#lifecyclepolicyresourcetypetype) 
2. See [:material-code-braces: LifecyclePolicyDetailTypeDef](./type_defs.md#lifecyclepolicydetailtypedef) 
3. See [:material-code-braces: LifecyclePolicyResourceSelectionTypeDef](./type_defs.md#lifecyclepolicyresourceselectiontypedef) 
4. See [:material-code-brackets: LifecyclePolicyStatusType](./literals.md#lifecyclepolicystatustype) 
5. See [:material-code-braces: UpdateLifecyclePolicyResponseTypeDef](./type_defs.md#updatelifecyclepolicyresponsetypedef) 


```python
# update_lifecycle_policy method usage example with argument unpacking

kwargs: UpdateLifecyclePolicyRequestRequestTypeDef = {  # (1)
    "lifecyclePolicyArn": ...,
    "executionRole": ...,
    "resourceType": ...,
    "policyDetails": ...,
    "resourceSelection": ...,
    "clientToken": ...,
}

parent.update_lifecycle_policy(**kwargs)
```

1. See [:material-code-braces: UpdateLifecyclePolicyRequestRequestTypeDef](./type_defs.md#updatelifecyclepolicyrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("imagebuilder").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#Imagebuilder.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ImagebuilderClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("imagebuilder").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#Imagebuilder.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





