# SageMakerClient

> [Index](../README.md) > [SageMaker](./README.md) > SageMakerClient

!!! note ""

    Auto-generated documentation for [SageMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#sagemaker)
    type annotations stubs module [types-aiobotocore-sagemaker](https://pypi.org/project/types-aiobotocore-sagemaker/).

## SageMakerClient

Type annotations and code completion for `#!python session.create_client("sagemaker")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client)

```python
# SageMakerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_sagemaker.client import SageMakerClient

session = get_session()
async with session.create_client("sagemaker") as client:
    client: SageMakerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sagemaker").exceptions` structure.

```python
# SageMakerClient.exceptions usage example

async with session.create_client("sagemaker") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConflictException,
        client.ResourceInUse,
        client.ResourceLimitExceeded,
        client.ResourceNotFound,
    ) as e:
        print(e)
```

```python
# SageMakerClient usage type checking example

from types_aiobotocore_sagemaker.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("sagemaker").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("sagemaker").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/generate_presigned_url.html)

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


### add\_association

Creates an <i>association</i> between the source and the destination.

Type annotations and code completion for `#!python session.create_client("sagemaker").add_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/add_association.html)

```python
# add_association method definition

await def add_association(
    self,
    *,
    SourceArn: str,
    DestinationArn: str,
    AssociationType: AssociationEdgeTypeType = ...,  # (1)
) -> AddAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssociationEdgeTypeType](./literals.md#associationedgetypetype) 
2. See [:material-code-braces: AddAssociationResponseTypeDef](./type_defs.md#addassociationresponsetypedef) 


```python
# add_association method usage example with argument unpacking

kwargs: AddAssociationRequestTypeDef = {  # (1)
    "SourceArn": ...,
    "DestinationArn": ...,
}

parent.add_association(**kwargs)
```

1. See [:material-code-braces: AddAssociationRequestTypeDef](./type_defs.md#addassociationrequesttypedef) 

### add\_tags

Adds or overwrites one or more tags for the specified SageMaker resource.

Type annotations and code completion for `#!python session.create_client("sagemaker").add_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/add_tags.html)

```python
# add_tags method definition

await def add_tags(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> AddTagsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: AddTagsOutputTypeDef](./type_defs.md#addtagsoutputtypedef) 


```python
# add_tags method usage example with argument unpacking

kwargs: AddTagsInputTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.add_tags(**kwargs)
```

1. See [:material-code-braces: AddTagsInputTypeDef](./type_defs.md#addtagsinputtypedef) 

### associate\_trial\_component

Associates a trial component with a trial.

Type annotations and code completion for `#!python session.create_client("sagemaker").associate_trial_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/associate_trial_component.html)

```python
# associate_trial_component method definition

await def associate_trial_component(
    self,
    *,
    TrialComponentName: str,
    TrialName: str,
) -> AssociateTrialComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateTrialComponentResponseTypeDef](./type_defs.md#associatetrialcomponentresponsetypedef) 


```python
# associate_trial_component method usage example with argument unpacking

kwargs: AssociateTrialComponentRequestTypeDef = {  # (1)
    "TrialComponentName": ...,
    "TrialName": ...,
}

parent.associate_trial_component(**kwargs)
```

1. See [:material-code-braces: AssociateTrialComponentRequestTypeDef](./type_defs.md#associatetrialcomponentrequesttypedef) 

### batch\_delete\_cluster\_nodes

Deletes specific nodes within a SageMaker HyperPod cluster.

Type annotations and code completion for `#!python session.create_client("sagemaker").batch_delete_cluster_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/batch_delete_cluster_nodes.html)

```python
# batch_delete_cluster_nodes method definition

await def batch_delete_cluster_nodes(
    self,
    *,
    ClusterName: str,
    NodeIds: Sequence[str],
) -> BatchDeleteClusterNodesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteClusterNodesResponseTypeDef](./type_defs.md#batchdeleteclusternodesresponsetypedef) 


```python
# batch_delete_cluster_nodes method usage example with argument unpacking

kwargs: BatchDeleteClusterNodesRequestTypeDef = {  # (1)
    "ClusterName": ...,
    "NodeIds": ...,
}

parent.batch_delete_cluster_nodes(**kwargs)
```

1. See [:material-code-braces: BatchDeleteClusterNodesRequestTypeDef](./type_defs.md#batchdeleteclusternodesrequesttypedef) 

### batch\_describe\_model\_package

This action batch describes a list of versioned model packages.

Type annotations and code completion for `#!python session.create_client("sagemaker").batch_describe_model_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/batch_describe_model_package.html)

```python
# batch_describe_model_package method definition

await def batch_describe_model_package(
    self,
    *,
    ModelPackageArnList: Sequence[str],
) -> BatchDescribeModelPackageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDescribeModelPackageOutputTypeDef](./type_defs.md#batchdescribemodelpackageoutputtypedef) 


```python
# batch_describe_model_package method usage example with argument unpacking

kwargs: BatchDescribeModelPackageInputTypeDef = {  # (1)
    "ModelPackageArnList": ...,
}

parent.batch_describe_model_package(**kwargs)
```

1. See [:material-code-braces: BatchDescribeModelPackageInputTypeDef](./type_defs.md#batchdescribemodelpackageinputtypedef) 

### create\_action

Creates an <i>action</i>.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_action.html)

```python
# create_action method definition

await def create_action(
    self,
    *,
    ActionName: str,
    Source: ActionSourceTypeDef,  # (1)
    ActionType: str,
    Description: str = ...,
    Status: ActionStatusType = ...,  # (2)
    Properties: Mapping[str, str] = ...,
    MetadataProperties: MetadataPropertiesTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateActionResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ActionSourceTypeDef](./type_defs.md#actionsourcetypedef) 
2. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
3. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateActionResponseTypeDef](./type_defs.md#createactionresponsetypedef) 


```python
# create_action method usage example with argument unpacking

kwargs: CreateActionRequestTypeDef = {  # (1)
    "ActionName": ...,
    "Source": ...,
    "ActionType": ...,
}

parent.create_action(**kwargs)
```

1. See [:material-code-braces: CreateActionRequestTypeDef](./type_defs.md#createactionrequesttypedef) 

### create\_algorithm

Create a machine learning algorithm that you can use in SageMaker and list in
the Amazon Web Services Marketplace.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_algorithm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_algorithm.html)

```python
# create_algorithm method definition

await def create_algorithm(
    self,
    *,
    AlgorithmName: str,
    TrainingSpecification: TrainingSpecificationUnionTypeDef,  # (1)
    AlgorithmDescription: str = ...,
    InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,  # (2)
    ValidationSpecification: AlgorithmValidationSpecificationUnionTypeDef = ...,  # (3)
    CertifyForMarketplace: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateAlgorithmOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: TrainingSpecificationTypeDef](./type_defs.md#trainingspecificationtypedef) [:material-code-braces: TrainingSpecificationOutputTypeDef](./type_defs.md#trainingspecificationoutputtypedef) 
2. See [:material-code-braces: InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef) [:material-code-braces: InferenceSpecificationOutputTypeDef](./type_defs.md#inferencespecificationoutputtypedef) 
3. See [:material-code-braces: AlgorithmValidationSpecificationTypeDef](./type_defs.md#algorithmvalidationspecificationtypedef) [:material-code-braces: AlgorithmValidationSpecificationOutputTypeDef](./type_defs.md#algorithmvalidationspecificationoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateAlgorithmOutputTypeDef](./type_defs.md#createalgorithmoutputtypedef) 


```python
# create_algorithm method usage example with argument unpacking

kwargs: CreateAlgorithmInputTypeDef = {  # (1)
    "AlgorithmName": ...,
    "TrainingSpecification": ...,
}

parent.create_algorithm(**kwargs)
```

1. See [:material-code-braces: CreateAlgorithmInputTypeDef](./type_defs.md#createalgorithminputtypedef) 

### create\_app

Creates a running app for the specified UserProfile.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_app.html)

```python
# create_app method definition

await def create_app(
    self,
    *,
    DomainId: str,
    AppType: AppTypeType,  # (1)
    AppName: str,
    UserProfileName: str = ...,
    SpaceName: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    ResourceSpec: ResourceSpecTypeDef = ...,  # (3)
) -> CreateAppResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResourceSpecTypeDef](./type_defs.md#resourcespectypedef) 
4. See [:material-code-braces: CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef) 


```python
# create_app method usage example with argument unpacking

kwargs: CreateAppRequestTypeDef = {  # (1)
    "DomainId": ...,
    "AppType": ...,
    "AppName": ...,
}

parent.create_app(**kwargs)
```

1. See [:material-code-braces: CreateAppRequestTypeDef](./type_defs.md#createapprequesttypedef) 

### create\_app\_image\_config

Creates a configuration for running a SageMaker AI image as a KernelGateway app.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_app_image_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_app_image_config.html)

```python
# create_app_image_config method definition

await def create_app_image_config(
    self,
    *,
    AppImageConfigName: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    KernelGatewayImageConfig: KernelGatewayImageConfigUnionTypeDef = ...,  # (2)
    JupyterLabAppImageConfig: JupyterLabAppImageConfigUnionTypeDef = ...,  # (3)
    CodeEditorAppImageConfig: CodeEditorAppImageConfigUnionTypeDef = ...,  # (4)
) -> CreateAppImageConfigResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: KernelGatewayImageConfigTypeDef](./type_defs.md#kernelgatewayimageconfigtypedef) [:material-code-braces: KernelGatewayImageConfigOutputTypeDef](./type_defs.md#kernelgatewayimageconfigoutputtypedef) 
3. See [:material-code-braces: JupyterLabAppImageConfigTypeDef](./type_defs.md#jupyterlabappimageconfigtypedef) [:material-code-braces: JupyterLabAppImageConfigOutputTypeDef](./type_defs.md#jupyterlabappimageconfigoutputtypedef) 
4. See [:material-code-braces: CodeEditorAppImageConfigTypeDef](./type_defs.md#codeeditorappimageconfigtypedef) [:material-code-braces: CodeEditorAppImageConfigOutputTypeDef](./type_defs.md#codeeditorappimageconfigoutputtypedef) 
5. See [:material-code-braces: CreateAppImageConfigResponseTypeDef](./type_defs.md#createappimageconfigresponsetypedef) 


```python
# create_app_image_config method usage example with argument unpacking

kwargs: CreateAppImageConfigRequestTypeDef = {  # (1)
    "AppImageConfigName": ...,
}

parent.create_app_image_config(**kwargs)
```

1. See [:material-code-braces: CreateAppImageConfigRequestTypeDef](./type_defs.md#createappimageconfigrequesttypedef) 

### create\_artifact

Creates an <i>artifact</i>.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_artifact.html)

```python
# create_artifact method definition

await def create_artifact(
    self,
    *,
    Source: ArtifactSourceUnionTypeDef,  # (1)
    ArtifactType: str,
    ArtifactName: str = ...,
    Properties: Mapping[str, str] = ...,
    MetadataProperties: MetadataPropertiesTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateArtifactResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ArtifactSourceTypeDef](./type_defs.md#artifactsourcetypedef) [:material-code-braces: ArtifactSourceOutputTypeDef](./type_defs.md#artifactsourceoutputtypedef) 
2. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateArtifactResponseTypeDef](./type_defs.md#createartifactresponsetypedef) 


```python
# create_artifact method usage example with argument unpacking

kwargs: CreateArtifactRequestTypeDef = {  # (1)
    "Source": ...,
    "ArtifactType": ...,
}

parent.create_artifact(**kwargs)
```

1. See [:material-code-braces: CreateArtifactRequestTypeDef](./type_defs.md#createartifactrequesttypedef) 

### create\_auto\_ml\_job

Creates an Autopilot job also referred to as Autopilot experiment or AutoML job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_auto_ml_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_auto_ml_job.html)

```python
# create_auto_ml_job method definition

await def create_auto_ml_job(
    self,
    *,
    AutoMLJobName: str,
    InputDataConfig: Sequence[AutoMLChannelTypeDef],  # (1)
    OutputDataConfig: AutoMLOutputDataConfigTypeDef,  # (2)
    RoleArn: str,
    ProblemType: ProblemTypeType = ...,  # (3)
    AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,  # (4)
    AutoMLJobConfig: AutoMLJobConfigUnionTypeDef = ...,  # (5)
    GenerateCandidateDefinitionsOnly: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (6)
    ModelDeployConfig: ModelDeployConfigTypeDef = ...,  # (7)
) -> CreateAutoMLJobResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: AutoMLChannelTypeDef](./type_defs.md#automlchanneltypedef) 
2. See [:material-code-braces: AutoMLOutputDataConfigTypeDef](./type_defs.md#automloutputdataconfigtypedef) 
3. See [:material-code-brackets: ProblemTypeType](./literals.md#problemtypetype) 
4. See [:material-code-braces: AutoMLJobObjectiveTypeDef](./type_defs.md#automljobobjectivetypedef) 
5. See [:material-code-braces: AutoMLJobConfigTypeDef](./type_defs.md#automljobconfigtypedef) [:material-code-braces: AutoMLJobConfigOutputTypeDef](./type_defs.md#automljobconfigoutputtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: ModelDeployConfigTypeDef](./type_defs.md#modeldeployconfigtypedef) 
8. See [:material-code-braces: CreateAutoMLJobResponseTypeDef](./type_defs.md#createautomljobresponsetypedef) 


```python
# create_auto_ml_job method usage example with argument unpacking

kwargs: CreateAutoMLJobRequestTypeDef = {  # (1)
    "AutoMLJobName": ...,
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "RoleArn": ...,
}

parent.create_auto_ml_job(**kwargs)
```

1. See [:material-code-braces: CreateAutoMLJobRequestTypeDef](./type_defs.md#createautomljobrequesttypedef) 

### create\_auto\_ml\_job\_v2

Creates an Autopilot job also referred to as Autopilot experiment or AutoML job
V2.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_auto_ml_job_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_auto_ml_job_v2.html)

```python
# create_auto_ml_job_v2 method definition

await def create_auto_ml_job_v2(
    self,
    *,
    AutoMLJobName: str,
    AutoMLJobInputDataConfig: Sequence[AutoMLJobChannelTypeDef],  # (1)
    OutputDataConfig: AutoMLOutputDataConfigTypeDef,  # (2)
    AutoMLProblemTypeConfig: AutoMLProblemTypeConfigUnionTypeDef,  # (3)
    RoleArn: str,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    SecurityConfig: AutoMLSecurityConfigUnionTypeDef = ...,  # (5)
    AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,  # (6)
    ModelDeployConfig: ModelDeployConfigTypeDef = ...,  # (7)
    DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...,  # (8)
    AutoMLComputeConfig: AutoMLComputeConfigTypeDef = ...,  # (9)
) -> CreateAutoMLJobV2ResponseTypeDef:  # (10)
    ...
```

1. See [:material-code-braces: AutoMLJobChannelTypeDef](./type_defs.md#automljobchanneltypedef) 
2. See [:material-code-braces: AutoMLOutputDataConfigTypeDef](./type_defs.md#automloutputdataconfigtypedef) 
3. See [:material-code-braces: AutoMLProblemTypeConfigTypeDef](./type_defs.md#automlproblemtypeconfigtypedef) [:material-code-braces: AutoMLProblemTypeConfigOutputTypeDef](./type_defs.md#automlproblemtypeconfigoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: AutoMLSecurityConfigTypeDef](./type_defs.md#automlsecurityconfigtypedef) [:material-code-braces: AutoMLSecurityConfigOutputTypeDef](./type_defs.md#automlsecurityconfigoutputtypedef) 
6. See [:material-code-braces: AutoMLJobObjectiveTypeDef](./type_defs.md#automljobobjectivetypedef) 
7. See [:material-code-braces: ModelDeployConfigTypeDef](./type_defs.md#modeldeployconfigtypedef) 
8. See [:material-code-braces: AutoMLDataSplitConfigTypeDef](./type_defs.md#automldatasplitconfigtypedef) 
9. See [:material-code-braces: AutoMLComputeConfigTypeDef](./type_defs.md#automlcomputeconfigtypedef) 
10. See [:material-code-braces: CreateAutoMLJobV2ResponseTypeDef](./type_defs.md#createautomljobv2responsetypedef) 


```python
# create_auto_ml_job_v2 method usage example with argument unpacking

kwargs: CreateAutoMLJobV2RequestTypeDef = {  # (1)
    "AutoMLJobName": ...,
    "AutoMLJobInputDataConfig": ...,
    "OutputDataConfig": ...,
    "AutoMLProblemTypeConfig": ...,
    "RoleArn": ...,
}

parent.create_auto_ml_job_v2(**kwargs)
```

1. See [:material-code-braces: CreateAutoMLJobV2RequestTypeDef](./type_defs.md#createautomljobv2requesttypedef) 

### create\_cluster

Creates a SageMaker HyperPod cluster.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_cluster.html)

```python
# create_cluster method definition

await def create_cluster(
    self,
    *,
    ClusterName: str,
    InstanceGroups: Sequence[ClusterInstanceGroupSpecificationTypeDef],  # (1)
    VpcConfig: VpcConfigUnionTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    Orchestrator: ClusterOrchestratorTypeDef = ...,  # (4)
    NodeRecovery: ClusterNodeRecoveryType = ...,  # (5)
) -> CreateClusterResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ClusterInstanceGroupSpecificationTypeDef](./type_defs.md#clusterinstancegroupspecificationtypedef) 
2. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ClusterOrchestratorTypeDef](./type_defs.md#clusterorchestratortypedef) 
5. See [:material-code-brackets: ClusterNodeRecoveryType](./literals.md#clusternoderecoverytype) 
6. See [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef) 


```python
# create_cluster method usage example with argument unpacking

kwargs: CreateClusterRequestTypeDef = {  # (1)
    "ClusterName": ...,
    "InstanceGroups": ...,
}

parent.create_cluster(**kwargs)
```

1. See [:material-code-braces: CreateClusterRequestTypeDef](./type_defs.md#createclusterrequesttypedef) 

### create\_cluster\_scheduler\_config

Create cluster policy configuration.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_cluster_scheduler_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_cluster_scheduler_config.html)

```python
# create_cluster_scheduler_config method definition

await def create_cluster_scheduler_config(
    self,
    *,
    Name: str,
    ClusterArn: str,
    SchedulerConfig: SchedulerConfigUnionTypeDef,  # (1)
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateClusterSchedulerConfigResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SchedulerConfigTypeDef](./type_defs.md#schedulerconfigtypedef) [:material-code-braces: SchedulerConfigOutputTypeDef](./type_defs.md#schedulerconfigoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateClusterSchedulerConfigResponseTypeDef](./type_defs.md#createclusterschedulerconfigresponsetypedef) 


```python
# create_cluster_scheduler_config method usage example with argument unpacking

kwargs: CreateClusterSchedulerConfigRequestTypeDef = {  # (1)
    "Name": ...,
    "ClusterArn": ...,
    "SchedulerConfig": ...,
}

parent.create_cluster_scheduler_config(**kwargs)
```

1. See [:material-code-braces: CreateClusterSchedulerConfigRequestTypeDef](./type_defs.md#createclusterschedulerconfigrequesttypedef) 

### create\_code\_repository

Creates a Git repository as a resource in your SageMaker AI account.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_code_repository` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_code_repository.html)

```python
# create_code_repository method definition

await def create_code_repository(
    self,
    *,
    CodeRepositoryName: str,
    GitConfig: GitConfigTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateCodeRepositoryOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: GitConfigTypeDef](./type_defs.md#gitconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateCodeRepositoryOutputTypeDef](./type_defs.md#createcoderepositoryoutputtypedef) 


```python
# create_code_repository method usage example with argument unpacking

kwargs: CreateCodeRepositoryInputTypeDef = {  # (1)
    "CodeRepositoryName": ...,
    "GitConfig": ...,
}

parent.create_code_repository(**kwargs)
```

1. See [:material-code-braces: CreateCodeRepositoryInputTypeDef](./type_defs.md#createcoderepositoryinputtypedef) 

### create\_compilation\_job

Starts a model compilation job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_compilation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_compilation_job.html)

```python
# create_compilation_job method definition

await def create_compilation_job(
    self,
    *,
    CompilationJobName: str,
    RoleArn: str,
    OutputConfig: OutputConfigTypeDef,  # (1)
    StoppingCondition: StoppingConditionTypeDef,  # (2)
    ModelPackageVersionArn: str = ...,
    InputConfig: InputConfigTypeDef = ...,  # (3)
    VpcConfig: NeoVpcConfigUnionTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreateCompilationJobResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
2. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
3. See [:material-code-braces: InputConfigTypeDef](./type_defs.md#inputconfigtypedef) 
4. See [:material-code-braces: NeoVpcConfigTypeDef](./type_defs.md#neovpcconfigtypedef) [:material-code-braces: NeoVpcConfigOutputTypeDef](./type_defs.md#neovpcconfigoutputtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateCompilationJobResponseTypeDef](./type_defs.md#createcompilationjobresponsetypedef) 


```python
# create_compilation_job method usage example with argument unpacking

kwargs: CreateCompilationJobRequestTypeDef = {  # (1)
    "CompilationJobName": ...,
    "RoleArn": ...,
    "OutputConfig": ...,
    "StoppingCondition": ...,
}

parent.create_compilation_job(**kwargs)
```

1. See [:material-code-braces: CreateCompilationJobRequestTypeDef](./type_defs.md#createcompilationjobrequesttypedef) 

### create\_compute\_quota

Create compute allocation definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_compute_quota` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_compute_quota.html)

```python
# create_compute_quota method definition

await def create_compute_quota(
    self,
    *,
    Name: str,
    ClusterArn: str,
    ComputeQuotaConfig: ComputeQuotaConfigUnionTypeDef,  # (1)
    ComputeQuotaTarget: ComputeQuotaTargetTypeDef,  # (2)
    Description: str = ...,
    ActivationState: ActivationStateType = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateComputeQuotaResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ComputeQuotaConfigTypeDef](./type_defs.md#computequotaconfigtypedef) [:material-code-braces: ComputeQuotaConfigOutputTypeDef](./type_defs.md#computequotaconfigoutputtypedef) 
2. See [:material-code-braces: ComputeQuotaTargetTypeDef](./type_defs.md#computequotatargettypedef) 
3. See [:material-code-brackets: ActivationStateType](./literals.md#activationstatetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateComputeQuotaResponseTypeDef](./type_defs.md#createcomputequotaresponsetypedef) 


```python
# create_compute_quota method usage example with argument unpacking

kwargs: CreateComputeQuotaRequestTypeDef = {  # (1)
    "Name": ...,
    "ClusterArn": ...,
    "ComputeQuotaConfig": ...,
    "ComputeQuotaTarget": ...,
}

parent.create_compute_quota(**kwargs)
```

1. See [:material-code-braces: CreateComputeQuotaRequestTypeDef](./type_defs.md#createcomputequotarequesttypedef) 

### create\_context

Creates a <i>context</i>.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_context` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_context.html)

```python
# create_context method definition

await def create_context(
    self,
    *,
    ContextName: str,
    Source: ContextSourceTypeDef,  # (1)
    ContextType: str,
    Description: str = ...,
    Properties: Mapping[str, str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateContextResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ContextSourceTypeDef](./type_defs.md#contextsourcetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateContextResponseTypeDef](./type_defs.md#createcontextresponsetypedef) 


```python
# create_context method usage example with argument unpacking

kwargs: CreateContextRequestTypeDef = {  # (1)
    "ContextName": ...,
    "Source": ...,
    "ContextType": ...,
}

parent.create_context(**kwargs)
```

1. See [:material-code-braces: CreateContextRequestTypeDef](./type_defs.md#createcontextrequesttypedef) 

### create\_data\_quality\_job\_definition

Creates a definition for a job that monitors data quality and drift.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_data_quality_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_data_quality_job_definition.html)

```python
# create_data_quality_job_definition method definition

await def create_data_quality_job_definition(
    self,
    *,
    JobDefinitionName: str,
    DataQualityAppSpecification: DataQualityAppSpecificationUnionTypeDef,  # (1)
    DataQualityJobInput: DataQualityJobInputUnionTypeDef,  # (2)
    DataQualityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,  # (3)
    JobResources: MonitoringResourcesTypeDef,  # (4)
    RoleArn: str,
    DataQualityBaselineConfig: DataQualityBaselineConfigTypeDef = ...,  # (5)
    NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,  # (6)
    StoppingCondition: MonitoringStoppingConditionTypeDef = ...,  # (7)
    Tags: Sequence[TagTypeDef] = ...,  # (8)
) -> CreateDataQualityJobDefinitionResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: DataQualityAppSpecificationTypeDef](./type_defs.md#dataqualityappspecificationtypedef) [:material-code-braces: DataQualityAppSpecificationOutputTypeDef](./type_defs.md#dataqualityappspecificationoutputtypedef) 
2. See [:material-code-braces: DataQualityJobInputTypeDef](./type_defs.md#dataqualityjobinputtypedef) [:material-code-braces: DataQualityJobInputOutputTypeDef](./type_defs.md#dataqualityjobinputoutputtypedef) 
3. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) [:material-code-braces: MonitoringOutputConfigOutputTypeDef](./type_defs.md#monitoringoutputconfigoutputtypedef) 
4. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
5. See [:material-code-braces: DataQualityBaselineConfigTypeDef](./type_defs.md#dataqualitybaselineconfigtypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) [:material-code-braces: MonitoringNetworkConfigOutputTypeDef](./type_defs.md#monitoringnetworkconfigoutputtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: CreateDataQualityJobDefinitionResponseTypeDef](./type_defs.md#createdataqualityjobdefinitionresponsetypedef) 


```python
# create_data_quality_job_definition method usage example with argument unpacking

kwargs: CreateDataQualityJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
    "DataQualityAppSpecification": ...,
    "DataQualityJobInput": ...,
    "DataQualityJobOutputConfig": ...,
    "JobResources": ...,
    "RoleArn": ...,
}

parent.create_data_quality_job_definition(**kwargs)
```

1. See [:material-code-braces: CreateDataQualityJobDefinitionRequestTypeDef](./type_defs.md#createdataqualityjobdefinitionrequesttypedef) 

### create\_device\_fleet

Creates a device fleet.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_device_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_device_fleet.html)

```python
# create_device_fleet method definition

await def create_device_fleet(
    self,
    *,
    DeviceFleetName: str,
    OutputConfig: EdgeOutputConfigTypeDef,  # (1)
    RoleArn: str = ...,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    EnableIotRoleAlias: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_device_fleet method usage example with argument unpacking

kwargs: CreateDeviceFleetRequestTypeDef = {  # (1)
    "DeviceFleetName": ...,
    "OutputConfig": ...,
}

parent.create_device_fleet(**kwargs)
```

1. See [:material-code-braces: CreateDeviceFleetRequestTypeDef](./type_defs.md#createdevicefleetrequesttypedef) 

### create\_domain

Creates a <code>Domain</code>.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_domain.html)

```python
# create_domain method definition

await def create_domain(
    self,
    *,
    DomainName: str,
    AuthMode: AuthModeType,  # (1)
    DefaultUserSettings: UserSettingsUnionTypeDef,  # (2)
    SubnetIds: Sequence[str],
    VpcId: str,
    DomainSettings: DomainSettingsUnionTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    AppNetworkAccessType: AppNetworkAccessTypeType = ...,  # (5)
    HomeEfsFileSystemKmsKeyId: str = ...,
    KmsKeyId: str = ...,
    AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,  # (6)
    TagPropagation: TagPropagationType = ...,  # (7)
    DefaultSpaceSettings: DefaultSpaceSettingsUnionTypeDef = ...,  # (8)
) -> CreateDomainResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
2. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) [:material-code-braces: UserSettingsOutputTypeDef](./type_defs.md#usersettingsoutputtypedef) 
3. See [:material-code-braces: DomainSettingsTypeDef](./type_defs.md#domainsettingstypedef) [:material-code-braces: DomainSettingsOutputTypeDef](./type_defs.md#domainsettingsoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-brackets: AppNetworkAccessTypeType](./literals.md#appnetworkaccesstypetype) 
6. See [:material-code-brackets: AppSecurityGroupManagementType](./literals.md#appsecuritygroupmanagementtype) 
7. See [:material-code-brackets: TagPropagationType](./literals.md#tagpropagationtype) 
8. See [:material-code-braces: DefaultSpaceSettingsTypeDef](./type_defs.md#defaultspacesettingstypedef) [:material-code-braces: DefaultSpaceSettingsOutputTypeDef](./type_defs.md#defaultspacesettingsoutputtypedef) 
9. See [:material-code-braces: CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef) 


```python
# create_domain method usage example with argument unpacking

kwargs: CreateDomainRequestTypeDef = {  # (1)
    "DomainName": ...,
    "AuthMode": ...,
    "DefaultUserSettings": ...,
    "SubnetIds": ...,
    "VpcId": ...,
}

parent.create_domain(**kwargs)
```

1. See [:material-code-braces: CreateDomainRequestTypeDef](./type_defs.md#createdomainrequesttypedef) 

### create\_edge\_deployment\_plan

Creates an edge deployment plan, consisting of multiple stages.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_edge_deployment_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_edge_deployment_plan.html)

```python
# create_edge_deployment_plan method definition

await def create_edge_deployment_plan(
    self,
    *,
    EdgeDeploymentPlanName: str,
    ModelConfigs: Sequence[EdgeDeploymentModelConfigTypeDef],  # (1)
    DeviceFleetName: str,
    Stages: Sequence[DeploymentStageTypeDef] = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateEdgeDeploymentPlanResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: EdgeDeploymentModelConfigTypeDef](./type_defs.md#edgedeploymentmodelconfigtypedef) 
2. See [:material-code-braces: DeploymentStageTypeDef](./type_defs.md#deploymentstagetypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateEdgeDeploymentPlanResponseTypeDef](./type_defs.md#createedgedeploymentplanresponsetypedef) 


```python
# create_edge_deployment_plan method usage example with argument unpacking

kwargs: CreateEdgeDeploymentPlanRequestTypeDef = {  # (1)
    "EdgeDeploymentPlanName": ...,
    "ModelConfigs": ...,
    "DeviceFleetName": ...,
}

parent.create_edge_deployment_plan(**kwargs)
```

1. See [:material-code-braces: CreateEdgeDeploymentPlanRequestTypeDef](./type_defs.md#createedgedeploymentplanrequesttypedef) 

### create\_edge\_deployment\_stage

Creates a new stage in an existing edge deployment plan.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_edge_deployment_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_edge_deployment_stage.html)

```python
# create_edge_deployment_stage method definition

await def create_edge_deployment_stage(
    self,
    *,
    EdgeDeploymentPlanName: str,
    Stages: Sequence[DeploymentStageTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeploymentStageTypeDef](./type_defs.md#deploymentstagetypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_edge_deployment_stage method usage example with argument unpacking

kwargs: CreateEdgeDeploymentStageRequestTypeDef = {  # (1)
    "EdgeDeploymentPlanName": ...,
    "Stages": ...,
}

parent.create_edge_deployment_stage(**kwargs)
```

1. See [:material-code-braces: CreateEdgeDeploymentStageRequestTypeDef](./type_defs.md#createedgedeploymentstagerequesttypedef) 

### create\_edge\_packaging\_job

Starts a SageMaker Edge Manager model packaging job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_edge_packaging_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_edge_packaging_job.html)

```python
# create_edge_packaging_job method definition

await def create_edge_packaging_job(
    self,
    *,
    EdgePackagingJobName: str,
    CompilationJobName: str,
    ModelName: str,
    ModelVersion: str,
    RoleArn: str,
    OutputConfig: EdgeOutputConfigTypeDef,  # (1)
    ResourceKey: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_edge_packaging_job method usage example with argument unpacking

kwargs: CreateEdgePackagingJobRequestTypeDef = {  # (1)
    "EdgePackagingJobName": ...,
    "CompilationJobName": ...,
    "ModelName": ...,
    "ModelVersion": ...,
    "RoleArn": ...,
    "OutputConfig": ...,
}

parent.create_edge_packaging_job(**kwargs)
```

1. See [:material-code-braces: CreateEdgePackagingJobRequestTypeDef](./type_defs.md#createedgepackagingjobrequesttypedef) 

### create\_endpoint

Creates an endpoint using the endpoint configuration specified in the request.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_endpoint.html)

```python
# create_endpoint method definition

await def create_endpoint(
    self,
    *,
    EndpointName: str,
    EndpointConfigName: str,
    DeploymentConfig: DeploymentConfigUnionTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateEndpointOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) [:material-code-braces: DeploymentConfigOutputTypeDef](./type_defs.md#deploymentconfigoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateEndpointOutputTypeDef](./type_defs.md#createendpointoutputtypedef) 


```python
# create_endpoint method usage example with argument unpacking

kwargs: CreateEndpointInputTypeDef = {  # (1)
    "EndpointName": ...,
    "EndpointConfigName": ...,
}

parent.create_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateEndpointInputTypeDef](./type_defs.md#createendpointinputtypedef) 

### create\_endpoint\_config

Creates an endpoint configuration that SageMaker hosting services uses to
deploy models.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_endpoint_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_endpoint_config.html)

```python
# create_endpoint_config method definition

await def create_endpoint_config(
    self,
    *,
    EndpointConfigName: str,
    ProductionVariants: Sequence[ProductionVariantTypeDef],  # (1)
    DataCaptureConfig: DataCaptureConfigUnionTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    KmsKeyId: str = ...,
    AsyncInferenceConfig: AsyncInferenceConfigUnionTypeDef = ...,  # (4)
    ExplainerConfig: ExplainerConfigUnionTypeDef = ...,  # (5)
    ShadowProductionVariants: Sequence[ProductionVariantTypeDef] = ...,  # (1)
    ExecutionRoleArn: str = ...,
    VpcConfig: VpcConfigUnionTypeDef = ...,  # (7)
    EnableNetworkIsolation: bool = ...,
) -> CreateEndpointConfigOutputTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: ProductionVariantTypeDef](./type_defs.md#productionvarianttypedef) 
2. See [:material-code-braces: DataCaptureConfigTypeDef](./type_defs.md#datacaptureconfigtypedef) [:material-code-braces: DataCaptureConfigOutputTypeDef](./type_defs.md#datacaptureconfigoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: AsyncInferenceConfigTypeDef](./type_defs.md#asyncinferenceconfigtypedef) [:material-code-braces: AsyncInferenceConfigOutputTypeDef](./type_defs.md#asyncinferenceconfigoutputtypedef) 
5. See [:material-code-braces: ExplainerConfigTypeDef](./type_defs.md#explainerconfigtypedef) [:material-code-braces: ExplainerConfigOutputTypeDef](./type_defs.md#explainerconfigoutputtypedef) 
6. See [:material-code-braces: ProductionVariantTypeDef](./type_defs.md#productionvarianttypedef) 
7. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
8. See [:material-code-braces: CreateEndpointConfigOutputTypeDef](./type_defs.md#createendpointconfigoutputtypedef) 


```python
# create_endpoint_config method usage example with argument unpacking

kwargs: CreateEndpointConfigInputTypeDef = {  # (1)
    "EndpointConfigName": ...,
    "ProductionVariants": ...,
}

parent.create_endpoint_config(**kwargs)
```

1. See [:material-code-braces: CreateEndpointConfigInputTypeDef](./type_defs.md#createendpointconfiginputtypedef) 

### create\_experiment

Creates a SageMaker <i>experiment</i>.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_experiment.html)

```python
# create_experiment method definition

await def create_experiment(
    self,
    *,
    ExperimentName: str,
    DisplayName: str = ...,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateExperimentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateExperimentResponseTypeDef](./type_defs.md#createexperimentresponsetypedef) 


```python
# create_experiment method usage example with argument unpacking

kwargs: CreateExperimentRequestTypeDef = {  # (1)
    "ExperimentName": ...,
}

parent.create_experiment(**kwargs)
```

1. See [:material-code-braces: CreateExperimentRequestTypeDef](./type_defs.md#createexperimentrequesttypedef) 

### create\_feature\_group

Create a new <code>FeatureGroup</code>.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_feature_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_feature_group.html)

```python
# create_feature_group method definition

await def create_feature_group(
    self,
    *,
    FeatureGroupName: str,
    RecordIdentifierFeatureName: str,
    EventTimeFeatureName: str,
    FeatureDefinitions: Sequence[FeatureDefinitionTypeDef],  # (1)
    OnlineStoreConfig: OnlineStoreConfigTypeDef = ...,  # (2)
    OfflineStoreConfig: OfflineStoreConfigTypeDef = ...,  # (3)
    ThroughputConfig: ThroughputConfigTypeDef = ...,  # (4)
    RoleArn: str = ...,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreateFeatureGroupResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: FeatureDefinitionTypeDef](./type_defs.md#featuredefinitiontypedef) 
2. See [:material-code-braces: OnlineStoreConfigTypeDef](./type_defs.md#onlinestoreconfigtypedef) 
3. See [:material-code-braces: OfflineStoreConfigTypeDef](./type_defs.md#offlinestoreconfigtypedef) 
4. See [:material-code-braces: ThroughputConfigTypeDef](./type_defs.md#throughputconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateFeatureGroupResponseTypeDef](./type_defs.md#createfeaturegroupresponsetypedef) 


```python
# create_feature_group method usage example with argument unpacking

kwargs: CreateFeatureGroupRequestTypeDef = {  # (1)
    "FeatureGroupName": ...,
    "RecordIdentifierFeatureName": ...,
    "EventTimeFeatureName": ...,
    "FeatureDefinitions": ...,
}

parent.create_feature_group(**kwargs)
```

1. See [:material-code-braces: CreateFeatureGroupRequestTypeDef](./type_defs.md#createfeaturegrouprequesttypedef) 

### create\_flow\_definition

Creates a flow definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_flow_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_flow_definition.html)

```python
# create_flow_definition method definition

await def create_flow_definition(
    self,
    *,
    FlowDefinitionName: str,
    OutputConfig: FlowDefinitionOutputConfigTypeDef,  # (1)
    RoleArn: str,
    HumanLoopRequestSource: HumanLoopRequestSourceTypeDef = ...,  # (2)
    HumanLoopActivationConfig: HumanLoopActivationConfigTypeDef = ...,  # (3)
    HumanLoopConfig: HumanLoopConfigUnionTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreateFlowDefinitionResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: FlowDefinitionOutputConfigTypeDef](./type_defs.md#flowdefinitionoutputconfigtypedef) 
2. See [:material-code-braces: HumanLoopRequestSourceTypeDef](./type_defs.md#humanlooprequestsourcetypedef) 
3. See [:material-code-braces: HumanLoopActivationConfigTypeDef](./type_defs.md#humanloopactivationconfigtypedef) 
4. See [:material-code-braces: HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef) [:material-code-braces: HumanLoopConfigOutputTypeDef](./type_defs.md#humanloopconfigoutputtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateFlowDefinitionResponseTypeDef](./type_defs.md#createflowdefinitionresponsetypedef) 


```python
# create_flow_definition method usage example with argument unpacking

kwargs: CreateFlowDefinitionRequestTypeDef = {  # (1)
    "FlowDefinitionName": ...,
    "OutputConfig": ...,
    "RoleArn": ...,
}

parent.create_flow_definition(**kwargs)
```

1. See [:material-code-braces: CreateFlowDefinitionRequestTypeDef](./type_defs.md#createflowdefinitionrequesttypedef) 

### create\_hub

Create a hub.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_hub` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_hub.html)

```python
# create_hub method definition

await def create_hub(
    self,
    *,
    HubName: str,
    HubDescription: str,
    HubDisplayName: str = ...,
    HubSearchKeywords: Sequence[str] = ...,
    S3StorageConfig: HubS3StorageConfigTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateHubResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: HubS3StorageConfigTypeDef](./type_defs.md#hubs3storageconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateHubResponseTypeDef](./type_defs.md#createhubresponsetypedef) 


```python
# create_hub method usage example with argument unpacking

kwargs: CreateHubRequestTypeDef = {  # (1)
    "HubName": ...,
    "HubDescription": ...,
}

parent.create_hub(**kwargs)
```

1. See [:material-code-braces: CreateHubRequestTypeDef](./type_defs.md#createhubrequesttypedef) 

### create\_hub\_content\_reference

Create a hub content reference in order to add a model in the JumpStart public
hub to a private hub.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_hub_content_reference` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_hub_content_reference.html)

```python
# create_hub_content_reference method definition

await def create_hub_content_reference(
    self,
    *,
    HubName: str,
    SageMakerPublicHubContentArn: str,
    HubContentName: str = ...,
    MinVersion: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateHubContentReferenceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateHubContentReferenceResponseTypeDef](./type_defs.md#createhubcontentreferenceresponsetypedef) 


```python
# create_hub_content_reference method usage example with argument unpacking

kwargs: CreateHubContentReferenceRequestTypeDef = {  # (1)
    "HubName": ...,
    "SageMakerPublicHubContentArn": ...,
}

parent.create_hub_content_reference(**kwargs)
```

1. See [:material-code-braces: CreateHubContentReferenceRequestTypeDef](./type_defs.md#createhubcontentreferencerequesttypedef) 

### create\_human\_task\_ui

Defines the settings you will use for the human review workflow user interface.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_human_task_ui` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_human_task_ui.html)

```python
# create_human_task_ui method definition

await def create_human_task_ui(
    self,
    *,
    HumanTaskUiName: str,
    UiTemplate: UiTemplateTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateHumanTaskUiResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UiTemplateTypeDef](./type_defs.md#uitemplatetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateHumanTaskUiResponseTypeDef](./type_defs.md#createhumantaskuiresponsetypedef) 


```python
# create_human_task_ui method usage example with argument unpacking

kwargs: CreateHumanTaskUiRequestTypeDef = {  # (1)
    "HumanTaskUiName": ...,
    "UiTemplate": ...,
}

parent.create_human_task_ui(**kwargs)
```

1. See [:material-code-braces: CreateHumanTaskUiRequestTypeDef](./type_defs.md#createhumantaskuirequesttypedef) 

### create\_hyper\_parameter\_tuning\_job

Starts a hyperparameter tuning job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_hyper_parameter_tuning_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_hyper_parameter_tuning_job.html)

```python
# create_hyper_parameter_tuning_job method definition

await def create_hyper_parameter_tuning_job(
    self,
    *,
    HyperParameterTuningJobName: str,
    HyperParameterTuningJobConfig: HyperParameterTuningJobConfigUnionTypeDef,  # (1)
    TrainingJobDefinition: HyperParameterTrainingJobDefinitionUnionTypeDef = ...,  # (2)
    TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionUnionTypeDef] = ...,  # (3)
    WarmStartConfig: HyperParameterTuningJobWarmStartConfigUnionTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
    Autotune: AutotuneTypeDef = ...,  # (6)
) -> CreateHyperParameterTuningJobResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: HyperParameterTuningJobConfigTypeDef](./type_defs.md#hyperparametertuningjobconfigtypedef) [:material-code-braces: HyperParameterTuningJobConfigOutputTypeDef](./type_defs.md#hyperparametertuningjobconfigoutputtypedef) 
2. See [:material-code-braces: HyperParameterTrainingJobDefinitionTypeDef](./type_defs.md#hyperparametertrainingjobdefinitiontypedef) [:material-code-braces: HyperParameterTrainingJobDefinitionOutputTypeDef](./type_defs.md#hyperparametertrainingjobdefinitionoutputtypedef) 
3. See [:material-code-braces: HyperParameterTrainingJobDefinitionTypeDef](./type_defs.md#hyperparametertrainingjobdefinitiontypedef) [:material-code-braces: HyperParameterTrainingJobDefinitionOutputTypeDef](./type_defs.md#hyperparametertrainingjobdefinitionoutputtypedef) 
4. See [:material-code-braces: HyperParameterTuningJobWarmStartConfigTypeDef](./type_defs.md#hyperparametertuningjobwarmstartconfigtypedef) [:material-code-braces: HyperParameterTuningJobWarmStartConfigOutputTypeDef](./type_defs.md#hyperparametertuningjobwarmstartconfigoutputtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: AutotuneTypeDef](./type_defs.md#autotunetypedef) 
7. See [:material-code-braces: CreateHyperParameterTuningJobResponseTypeDef](./type_defs.md#createhyperparametertuningjobresponsetypedef) 


```python
# create_hyper_parameter_tuning_job method usage example with argument unpacking

kwargs: CreateHyperParameterTuningJobRequestTypeDef = {  # (1)
    "HyperParameterTuningJobName": ...,
    "HyperParameterTuningJobConfig": ...,
}

parent.create_hyper_parameter_tuning_job(**kwargs)
```

1. See [:material-code-braces: CreateHyperParameterTuningJobRequestTypeDef](./type_defs.md#createhyperparametertuningjobrequesttypedef) 

### create\_image

Creates a custom SageMaker AI image.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_image.html)

```python
# create_image method definition

await def create_image(
    self,
    *,
    ImageName: str,
    RoleArn: str,
    Description: str = ...,
    DisplayName: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateImageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateImageResponseTypeDef](./type_defs.md#createimageresponsetypedef) 


```python
# create_image method usage example with argument unpacking

kwargs: CreateImageRequestTypeDef = {  # (1)
    "ImageName": ...,
    "RoleArn": ...,
}

parent.create_image(**kwargs)
```

1. See [:material-code-braces: CreateImageRequestTypeDef](./type_defs.md#createimagerequesttypedef) 

### create\_image\_version

Creates a version of the SageMaker AI image specified by <code>ImageName</code>.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_image_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_image_version.html)

```python
# create_image_version method definition

await def create_image_version(
    self,
    *,
    BaseImage: str,
    ClientToken: str,
    ImageName: str,
    Aliases: Sequence[str] = ...,
    VendorGuidance: VendorGuidanceType = ...,  # (1)
    JobType: JobTypeType = ...,  # (2)
    MLFramework: str = ...,
    ProgrammingLang: str = ...,
    Processor: ProcessorType = ...,  # (3)
    Horovod: bool = ...,
    ReleaseNotes: str = ...,
) -> CreateImageVersionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: VendorGuidanceType](./literals.md#vendorguidancetype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: ProcessorType](./literals.md#processortype) 
4. See [:material-code-braces: CreateImageVersionResponseTypeDef](./type_defs.md#createimageversionresponsetypedef) 


```python
# create_image_version method usage example with argument unpacking

kwargs: CreateImageVersionRequestTypeDef = {  # (1)
    "BaseImage": ...,
    "ClientToken": ...,
    "ImageName": ...,
}

parent.create_image_version(**kwargs)
```

1. See [:material-code-braces: CreateImageVersionRequestTypeDef](./type_defs.md#createimageversionrequesttypedef) 

### create\_inference\_component

Creates an inference component, which is a SageMaker AI hosting object that you
can use to deploy a model to an endpoint.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_inference_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_inference_component.html)

```python
# create_inference_component method definition

await def create_inference_component(
    self,
    *,
    InferenceComponentName: str,
    EndpointName: str,
    Specification: InferenceComponentSpecificationTypeDef,  # (1)
    VariantName: str = ...,
    RuntimeConfig: InferenceComponentRuntimeConfigTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateInferenceComponentOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: InferenceComponentSpecificationTypeDef](./type_defs.md#inferencecomponentspecificationtypedef) 
2. See [:material-code-braces: InferenceComponentRuntimeConfigTypeDef](./type_defs.md#inferencecomponentruntimeconfigtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateInferenceComponentOutputTypeDef](./type_defs.md#createinferencecomponentoutputtypedef) 


```python
# create_inference_component method usage example with argument unpacking

kwargs: CreateInferenceComponentInputTypeDef = {  # (1)
    "InferenceComponentName": ...,
    "EndpointName": ...,
    "Specification": ...,
}

parent.create_inference_component(**kwargs)
```

1. See [:material-code-braces: CreateInferenceComponentInputTypeDef](./type_defs.md#createinferencecomponentinputtypedef) 

### create\_inference\_experiment

Creates an inference experiment using the configurations specified in the
request.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_inference_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_inference_experiment.html)

```python
# create_inference_experiment method definition

await def create_inference_experiment(
    self,
    *,
    Name: str,
    Type: InferenceExperimentTypeType,  # (1)
    RoleArn: str,
    EndpointName: str,
    ModelVariants: Sequence[ModelVariantConfigTypeDef],  # (2)
    ShadowModeConfig: ShadowModeConfigUnionTypeDef,  # (3)
    Schedule: InferenceExperimentScheduleUnionTypeDef = ...,  # (4)
    Description: str = ...,
    DataStorageConfig: InferenceExperimentDataStorageConfigUnionTypeDef = ...,  # (5)
    KmsKey: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (6)
) -> CreateInferenceExperimentResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: InferenceExperimentTypeType](./literals.md#inferenceexperimenttypetype) 
2. See [:material-code-braces: ModelVariantConfigTypeDef](./type_defs.md#modelvariantconfigtypedef) 
3. See [:material-code-braces: ShadowModeConfigTypeDef](./type_defs.md#shadowmodeconfigtypedef) [:material-code-braces: ShadowModeConfigOutputTypeDef](./type_defs.md#shadowmodeconfigoutputtypedef) 
4. See [:material-code-braces: InferenceExperimentScheduleTypeDef](./type_defs.md#inferenceexperimentscheduletypedef) [:material-code-braces: InferenceExperimentScheduleOutputTypeDef](./type_defs.md#inferenceexperimentscheduleoutputtypedef) 
5. See [:material-code-braces: InferenceExperimentDataStorageConfigTypeDef](./type_defs.md#inferenceexperimentdatastorageconfigtypedef) [:material-code-braces: InferenceExperimentDataStorageConfigOutputTypeDef](./type_defs.md#inferenceexperimentdatastorageconfigoutputtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: CreateInferenceExperimentResponseTypeDef](./type_defs.md#createinferenceexperimentresponsetypedef) 


```python
# create_inference_experiment method usage example with argument unpacking

kwargs: CreateInferenceExperimentRequestTypeDef = {  # (1)
    "Name": ...,
    "Type": ...,
    "RoleArn": ...,
    "EndpointName": ...,
    "ModelVariants": ...,
    "ShadowModeConfig": ...,
}

parent.create_inference_experiment(**kwargs)
```

1. See [:material-code-braces: CreateInferenceExperimentRequestTypeDef](./type_defs.md#createinferenceexperimentrequesttypedef) 

### create\_inference\_recommendations\_job

Starts a recommendation job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_inference_recommendations_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_inference_recommendations_job.html)

```python
# create_inference_recommendations_job method definition

await def create_inference_recommendations_job(
    self,
    *,
    JobName: str,
    JobType: RecommendationJobTypeType,  # (1)
    RoleArn: str,
    InputConfig: RecommendationJobInputConfigUnionTypeDef,  # (2)
    JobDescription: str = ...,
    StoppingConditions: RecommendationJobStoppingConditionsUnionTypeDef = ...,  # (3)
    OutputConfig: RecommendationJobOutputConfigTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreateInferenceRecommendationsJobResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: RecommendationJobTypeType](./literals.md#recommendationjobtypetype) 
2. See [:material-code-braces: RecommendationJobInputConfigTypeDef](./type_defs.md#recommendationjobinputconfigtypedef) [:material-code-braces: RecommendationJobInputConfigOutputTypeDef](./type_defs.md#recommendationjobinputconfigoutputtypedef) 
3. See [:material-code-braces: RecommendationJobStoppingConditionsTypeDef](./type_defs.md#recommendationjobstoppingconditionstypedef) [:material-code-braces: RecommendationJobStoppingConditionsOutputTypeDef](./type_defs.md#recommendationjobstoppingconditionsoutputtypedef) 
4. See [:material-code-braces: RecommendationJobOutputConfigTypeDef](./type_defs.md#recommendationjoboutputconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreateInferenceRecommendationsJobResponseTypeDef](./type_defs.md#createinferencerecommendationsjobresponsetypedef) 


```python
# create_inference_recommendations_job method usage example with argument unpacking

kwargs: CreateInferenceRecommendationsJobRequestTypeDef = {  # (1)
    "JobName": ...,
    "JobType": ...,
    "RoleArn": ...,
    "InputConfig": ...,
}

parent.create_inference_recommendations_job(**kwargs)
```

1. See [:material-code-braces: CreateInferenceRecommendationsJobRequestTypeDef](./type_defs.md#createinferencerecommendationsjobrequesttypedef) 

### create\_labeling\_job

Creates a job that uses workers to label the data objects in your input dataset.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_labeling_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_labeling_job.html)

```python
# create_labeling_job method definition

await def create_labeling_job(
    self,
    *,
    LabelingJobName: str,
    LabelAttributeName: str,
    InputConfig: LabelingJobInputConfigUnionTypeDef,  # (1)
    OutputConfig: LabelingJobOutputConfigTypeDef,  # (2)
    RoleArn: str,
    HumanTaskConfig: HumanTaskConfigUnionTypeDef,  # (3)
    LabelCategoryConfigS3Uri: str = ...,
    StoppingConditions: LabelingJobStoppingConditionsTypeDef = ...,  # (4)
    LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigUnionTypeDef = ...,  # (5)
    Tags: Sequence[TagTypeDef] = ...,  # (6)
) -> CreateLabelingJobResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: LabelingJobInputConfigTypeDef](./type_defs.md#labelingjobinputconfigtypedef) [:material-code-braces: LabelingJobInputConfigOutputTypeDef](./type_defs.md#labelingjobinputconfigoutputtypedef) 
2. See [:material-code-braces: LabelingJobOutputConfigTypeDef](./type_defs.md#labelingjoboutputconfigtypedef) 
3. See [:material-code-braces: HumanTaskConfigTypeDef](./type_defs.md#humantaskconfigtypedef) [:material-code-braces: HumanTaskConfigOutputTypeDef](./type_defs.md#humantaskconfigoutputtypedef) 
4. See [:material-code-braces: LabelingJobStoppingConditionsTypeDef](./type_defs.md#labelingjobstoppingconditionstypedef) 
5. See [:material-code-braces: LabelingJobAlgorithmsConfigTypeDef](./type_defs.md#labelingjobalgorithmsconfigtypedef) [:material-code-braces: LabelingJobAlgorithmsConfigOutputTypeDef](./type_defs.md#labelingjobalgorithmsconfigoutputtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: CreateLabelingJobResponseTypeDef](./type_defs.md#createlabelingjobresponsetypedef) 


```python
# create_labeling_job method usage example with argument unpacking

kwargs: CreateLabelingJobRequestTypeDef = {  # (1)
    "LabelingJobName": ...,
    "LabelAttributeName": ...,
    "InputConfig": ...,
    "OutputConfig": ...,
    "RoleArn": ...,
    "HumanTaskConfig": ...,
}

parent.create_labeling_job(**kwargs)
```

1. See [:material-code-braces: CreateLabelingJobRequestTypeDef](./type_defs.md#createlabelingjobrequesttypedef) 

### create\_mlflow\_tracking\_server

Creates an MLflow Tracking Server using a general purpose Amazon S3 bucket as
the artifact store.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_mlflow_tracking_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_mlflow_tracking_server.html)

```python
# create_mlflow_tracking_server method definition

await def create_mlflow_tracking_server(
    self,
    *,
    TrackingServerName: str,
    ArtifactStoreUri: str,
    RoleArn: str,
    TrackingServerSize: TrackingServerSizeType = ...,  # (1)
    MlflowVersion: str = ...,
    AutomaticModelRegistration: bool = ...,
    WeeklyMaintenanceWindowStart: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateMlflowTrackingServerResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TrackingServerSizeType](./literals.md#trackingserversizetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateMlflowTrackingServerResponseTypeDef](./type_defs.md#createmlflowtrackingserverresponsetypedef) 


```python
# create_mlflow_tracking_server method usage example with argument unpacking

kwargs: CreateMlflowTrackingServerRequestTypeDef = {  # (1)
    "TrackingServerName": ...,
    "ArtifactStoreUri": ...,
    "RoleArn": ...,
}

parent.create_mlflow_tracking_server(**kwargs)
```

1. See [:material-code-braces: CreateMlflowTrackingServerRequestTypeDef](./type_defs.md#createmlflowtrackingserverrequesttypedef) 

### create\_model

Creates a model in SageMaker.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_model.html)

```python
# create_model method definition

await def create_model(
    self,
    *,
    ModelName: str,
    PrimaryContainer: ContainerDefinitionUnionTypeDef = ...,  # (1)
    Containers: Sequence[ContainerDefinitionUnionTypeDef] = ...,  # (2)
    InferenceExecutionConfig: InferenceExecutionConfigTypeDef = ...,  # (3)
    ExecutionRoleArn: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    VpcConfig: VpcConfigUnionTypeDef = ...,  # (5)
    EnableNetworkIsolation: bool = ...,
) -> CreateModelOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) [:material-code-braces: ContainerDefinitionOutputTypeDef](./type_defs.md#containerdefinitionoutputtypedef) 
2. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) [:material-code-braces: ContainerDefinitionOutputTypeDef](./type_defs.md#containerdefinitionoutputtypedef) 
3. See [:material-code-braces: InferenceExecutionConfigTypeDef](./type_defs.md#inferenceexecutionconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
6. See [:material-code-braces: CreateModelOutputTypeDef](./type_defs.md#createmodeloutputtypedef) 


```python
# create_model method usage example with argument unpacking

kwargs: CreateModelInputTypeDef = {  # (1)
    "ModelName": ...,
}

parent.create_model(**kwargs)
```

1. See [:material-code-braces: CreateModelInputTypeDef](./type_defs.md#createmodelinputtypedef) 

### create\_model\_bias\_job\_definition

Creates the definition for a model bias job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_model_bias_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_model_bias_job_definition.html)

```python
# create_model_bias_job_definition method definition

await def create_model_bias_job_definition(
    self,
    *,
    JobDefinitionName: str,
    ModelBiasAppSpecification: ModelBiasAppSpecificationUnionTypeDef,  # (1)
    ModelBiasJobInput: ModelBiasJobInputUnionTypeDef,  # (2)
    ModelBiasJobOutputConfig: MonitoringOutputConfigUnionTypeDef,  # (3)
    JobResources: MonitoringResourcesTypeDef,  # (4)
    RoleArn: str,
    ModelBiasBaselineConfig: ModelBiasBaselineConfigTypeDef = ...,  # (5)
    NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,  # (6)
    StoppingCondition: MonitoringStoppingConditionTypeDef = ...,  # (7)
    Tags: Sequence[TagTypeDef] = ...,  # (8)
) -> CreateModelBiasJobDefinitionResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: ModelBiasAppSpecificationTypeDef](./type_defs.md#modelbiasappspecificationtypedef) [:material-code-braces: ModelBiasAppSpecificationOutputTypeDef](./type_defs.md#modelbiasappspecificationoutputtypedef) 
2. See [:material-code-braces: ModelBiasJobInputTypeDef](./type_defs.md#modelbiasjobinputtypedef) [:material-code-braces: ModelBiasJobInputOutputTypeDef](./type_defs.md#modelbiasjobinputoutputtypedef) 
3. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) [:material-code-braces: MonitoringOutputConfigOutputTypeDef](./type_defs.md#monitoringoutputconfigoutputtypedef) 
4. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
5. See [:material-code-braces: ModelBiasBaselineConfigTypeDef](./type_defs.md#modelbiasbaselineconfigtypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) [:material-code-braces: MonitoringNetworkConfigOutputTypeDef](./type_defs.md#monitoringnetworkconfigoutputtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: CreateModelBiasJobDefinitionResponseTypeDef](./type_defs.md#createmodelbiasjobdefinitionresponsetypedef) 


```python
# create_model_bias_job_definition method usage example with argument unpacking

kwargs: CreateModelBiasJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
    "ModelBiasAppSpecification": ...,
    "ModelBiasJobInput": ...,
    "ModelBiasJobOutputConfig": ...,
    "JobResources": ...,
    "RoleArn": ...,
}

parent.create_model_bias_job_definition(**kwargs)
```

1. See [:material-code-braces: CreateModelBiasJobDefinitionRequestTypeDef](./type_defs.md#createmodelbiasjobdefinitionrequesttypedef) 

### create\_model\_card

Creates an Amazon SageMaker Model Card.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_model_card` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_model_card.html)

```python
# create_model_card method definition

await def create_model_card(
    self,
    *,
    ModelCardName: str,
    Content: str,
    ModelCardStatus: ModelCardStatusType,  # (1)
    SecurityConfig: ModelCardSecurityConfigTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateModelCardResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-braces: ModelCardSecurityConfigTypeDef](./type_defs.md#modelcardsecurityconfigtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateModelCardResponseTypeDef](./type_defs.md#createmodelcardresponsetypedef) 


```python
# create_model_card method usage example with argument unpacking

kwargs: CreateModelCardRequestTypeDef = {  # (1)
    "ModelCardName": ...,
    "Content": ...,
    "ModelCardStatus": ...,
}

parent.create_model_card(**kwargs)
```

1. See [:material-code-braces: CreateModelCardRequestTypeDef](./type_defs.md#createmodelcardrequesttypedef) 

### create\_model\_card\_export\_job

Creates an Amazon SageMaker Model Card export job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_model_card_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_model_card_export_job.html)

```python
# create_model_card_export_job method definition

await def create_model_card_export_job(
    self,
    *,
    ModelCardName: str,
    ModelCardExportJobName: str,
    OutputConfig: ModelCardExportOutputConfigTypeDef,  # (1)
    ModelCardVersion: int = ...,
) -> CreateModelCardExportJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ModelCardExportOutputConfigTypeDef](./type_defs.md#modelcardexportoutputconfigtypedef) 
2. See [:material-code-braces: CreateModelCardExportJobResponseTypeDef](./type_defs.md#createmodelcardexportjobresponsetypedef) 


```python
# create_model_card_export_job method usage example with argument unpacking

kwargs: CreateModelCardExportJobRequestTypeDef = {  # (1)
    "ModelCardName": ...,
    "ModelCardExportJobName": ...,
    "OutputConfig": ...,
}

parent.create_model_card_export_job(**kwargs)
```

1. See [:material-code-braces: CreateModelCardExportJobRequestTypeDef](./type_defs.md#createmodelcardexportjobrequesttypedef) 

### create\_model\_explainability\_job\_definition

Creates the definition for a model explainability job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_model_explainability_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_model_explainability_job_definition.html)

```python
# create_model_explainability_job_definition method definition

await def create_model_explainability_job_definition(
    self,
    *,
    JobDefinitionName: str,
    ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationUnionTypeDef,  # (1)
    ModelExplainabilityJobInput: ModelExplainabilityJobInputUnionTypeDef,  # (2)
    ModelExplainabilityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,  # (3)
    JobResources: MonitoringResourcesTypeDef,  # (4)
    RoleArn: str,
    ModelExplainabilityBaselineConfig: ModelExplainabilityBaselineConfigTypeDef = ...,  # (5)
    NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,  # (6)
    StoppingCondition: MonitoringStoppingConditionTypeDef = ...,  # (7)
    Tags: Sequence[TagTypeDef] = ...,  # (8)
) -> CreateModelExplainabilityJobDefinitionResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: ModelExplainabilityAppSpecificationTypeDef](./type_defs.md#modelexplainabilityappspecificationtypedef) [:material-code-braces: ModelExplainabilityAppSpecificationOutputTypeDef](./type_defs.md#modelexplainabilityappspecificationoutputtypedef) 
2. See [:material-code-braces: ModelExplainabilityJobInputTypeDef](./type_defs.md#modelexplainabilityjobinputtypedef) [:material-code-braces: ModelExplainabilityJobInputOutputTypeDef](./type_defs.md#modelexplainabilityjobinputoutputtypedef) 
3. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) [:material-code-braces: MonitoringOutputConfigOutputTypeDef](./type_defs.md#monitoringoutputconfigoutputtypedef) 
4. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
5. See [:material-code-braces: ModelExplainabilityBaselineConfigTypeDef](./type_defs.md#modelexplainabilitybaselineconfigtypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) [:material-code-braces: MonitoringNetworkConfigOutputTypeDef](./type_defs.md#monitoringnetworkconfigoutputtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: CreateModelExplainabilityJobDefinitionResponseTypeDef](./type_defs.md#createmodelexplainabilityjobdefinitionresponsetypedef) 


```python
# create_model_explainability_job_definition method usage example with argument unpacking

kwargs: CreateModelExplainabilityJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
    "ModelExplainabilityAppSpecification": ...,
    "ModelExplainabilityJobInput": ...,
    "ModelExplainabilityJobOutputConfig": ...,
    "JobResources": ...,
    "RoleArn": ...,
}

parent.create_model_explainability_job_definition(**kwargs)
```

1. See [:material-code-braces: CreateModelExplainabilityJobDefinitionRequestTypeDef](./type_defs.md#createmodelexplainabilityjobdefinitionrequesttypedef) 

### create\_model\_package

Creates a model package that you can use to create SageMaker models or list on
Amazon Web Services Marketplace, or a versioned model that is part of a model
group.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_model_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_model_package.html)

```python
# create_model_package method definition

await def create_model_package(
    self,
    *,
    ModelPackageName: str = ...,
    ModelPackageGroupName: str = ...,
    ModelPackageDescription: str = ...,
    InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,  # (1)
    ValidationSpecification: ModelPackageValidationSpecificationUnionTypeDef = ...,  # (2)
    SourceAlgorithmSpecification: SourceAlgorithmSpecificationUnionTypeDef = ...,  # (3)
    CertifyForMarketplace: bool = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    ModelApprovalStatus: ModelApprovalStatusType = ...,  # (5)
    MetadataProperties: MetadataPropertiesTypeDef = ...,  # (6)
    ModelMetrics: ModelMetricsTypeDef = ...,  # (7)
    ClientToken: str = ...,
    Domain: str = ...,
    Task: str = ...,
    SamplePayloadUrl: str = ...,
    CustomerMetadataProperties: Mapping[str, str] = ...,
    DriftCheckBaselines: DriftCheckBaselinesTypeDef = ...,  # (8)
    AdditionalInferenceSpecifications: Sequence[AdditionalInferenceSpecificationDefinitionUnionTypeDef] = ...,  # (9)
    SkipModelValidation: SkipModelValidationType = ...,  # (10)
    SourceUri: str = ...,
    SecurityConfig: ModelPackageSecurityConfigTypeDef = ...,  # (11)
    ModelCard: ModelPackageModelCardTypeDef = ...,  # (12)
    ModelLifeCycle: ModelLifeCycleTypeDef = ...,  # (13)
) -> CreateModelPackageOutputTypeDef:  # (14)
    ...
```

1. See [:material-code-braces: InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef) [:material-code-braces: InferenceSpecificationOutputTypeDef](./type_defs.md#inferencespecificationoutputtypedef) 
2. See [:material-code-braces: ModelPackageValidationSpecificationTypeDef](./type_defs.md#modelpackagevalidationspecificationtypedef) [:material-code-braces: ModelPackageValidationSpecificationOutputTypeDef](./type_defs.md#modelpackagevalidationspecificationoutputtypedef) 
3. See [:material-code-braces: SourceAlgorithmSpecificationTypeDef](./type_defs.md#sourcealgorithmspecificationtypedef) [:material-code-braces: SourceAlgorithmSpecificationOutputTypeDef](./type_defs.md#sourcealgorithmspecificationoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
6. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
7. See [:material-code-braces: ModelMetricsTypeDef](./type_defs.md#modelmetricstypedef) 
8. See [:material-code-braces: DriftCheckBaselinesTypeDef](./type_defs.md#driftcheckbaselinestypedef) 
9. See [:material-code-braces: AdditionalInferenceSpecificationDefinitionTypeDef](./type_defs.md#additionalinferencespecificationdefinitiontypedef) [:material-code-braces: AdditionalInferenceSpecificationDefinitionOutputTypeDef](./type_defs.md#additionalinferencespecificationdefinitionoutputtypedef) 
10. See [:material-code-brackets: SkipModelValidationType](./literals.md#skipmodelvalidationtype) 
11. See [:material-code-braces: ModelPackageSecurityConfigTypeDef](./type_defs.md#modelpackagesecurityconfigtypedef) 
12. See [:material-code-braces: ModelPackageModelCardTypeDef](./type_defs.md#modelpackagemodelcardtypedef) 
13. See [:material-code-braces: ModelLifeCycleTypeDef](./type_defs.md#modellifecycletypedef) 
14. See [:material-code-braces: CreateModelPackageOutputTypeDef](./type_defs.md#createmodelpackageoutputtypedef) 


```python
# create_model_package method usage example with argument unpacking

kwargs: CreateModelPackageInputTypeDef = {  # (1)
    "ModelPackageName": ...,
}

parent.create_model_package(**kwargs)
```

1. See [:material-code-braces: CreateModelPackageInputTypeDef](./type_defs.md#createmodelpackageinputtypedef) 

### create\_model\_package\_group

Creates a model group.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_model_package_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_model_package_group.html)

```python
# create_model_package_group method definition

await def create_model_package_group(
    self,
    *,
    ModelPackageGroupName: str,
    ModelPackageGroupDescription: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateModelPackageGroupOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateModelPackageGroupOutputTypeDef](./type_defs.md#createmodelpackagegroupoutputtypedef) 


```python
# create_model_package_group method usage example with argument unpacking

kwargs: CreateModelPackageGroupInputTypeDef = {  # (1)
    "ModelPackageGroupName": ...,
}

parent.create_model_package_group(**kwargs)
```

1. See [:material-code-braces: CreateModelPackageGroupInputTypeDef](./type_defs.md#createmodelpackagegroupinputtypedef) 

### create\_model\_quality\_job\_definition

Creates a definition for a job that monitors model quality and drift.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_model_quality_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_model_quality_job_definition.html)

```python
# create_model_quality_job_definition method definition

await def create_model_quality_job_definition(
    self,
    *,
    JobDefinitionName: str,
    ModelQualityAppSpecification: ModelQualityAppSpecificationUnionTypeDef,  # (1)
    ModelQualityJobInput: ModelQualityJobInputUnionTypeDef,  # (2)
    ModelQualityJobOutputConfig: MonitoringOutputConfigUnionTypeDef,  # (3)
    JobResources: MonitoringResourcesTypeDef,  # (4)
    RoleArn: str,
    ModelQualityBaselineConfig: ModelQualityBaselineConfigTypeDef = ...,  # (5)
    NetworkConfig: MonitoringNetworkConfigUnionTypeDef = ...,  # (6)
    StoppingCondition: MonitoringStoppingConditionTypeDef = ...,  # (7)
    Tags: Sequence[TagTypeDef] = ...,  # (8)
) -> CreateModelQualityJobDefinitionResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: ModelQualityAppSpecificationTypeDef](./type_defs.md#modelqualityappspecificationtypedef) [:material-code-braces: ModelQualityAppSpecificationOutputTypeDef](./type_defs.md#modelqualityappspecificationoutputtypedef) 
2. See [:material-code-braces: ModelQualityJobInputTypeDef](./type_defs.md#modelqualityjobinputtypedef) [:material-code-braces: ModelQualityJobInputOutputTypeDef](./type_defs.md#modelqualityjobinputoutputtypedef) 
3. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) [:material-code-braces: MonitoringOutputConfigOutputTypeDef](./type_defs.md#monitoringoutputconfigoutputtypedef) 
4. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
5. See [:material-code-braces: ModelQualityBaselineConfigTypeDef](./type_defs.md#modelqualitybaselineconfigtypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) [:material-code-braces: MonitoringNetworkConfigOutputTypeDef](./type_defs.md#monitoringnetworkconfigoutputtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: CreateModelQualityJobDefinitionResponseTypeDef](./type_defs.md#createmodelqualityjobdefinitionresponsetypedef) 


```python
# create_model_quality_job_definition method usage example with argument unpacking

kwargs: CreateModelQualityJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
    "ModelQualityAppSpecification": ...,
    "ModelQualityJobInput": ...,
    "ModelQualityJobOutputConfig": ...,
    "JobResources": ...,
    "RoleArn": ...,
}

parent.create_model_quality_job_definition(**kwargs)
```

1. See [:material-code-braces: CreateModelQualityJobDefinitionRequestTypeDef](./type_defs.md#createmodelqualityjobdefinitionrequesttypedef) 

### create\_monitoring\_schedule

Creates a schedule that regularly starts Amazon SageMaker AI Processing Jobs to
monitor the data captured for an Amazon SageMaker AI Endpoint.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_monitoring_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_monitoring_schedule.html)

```python
# create_monitoring_schedule method definition

await def create_monitoring_schedule(
    self,
    *,
    MonitoringScheduleName: str,
    MonitoringScheduleConfig: MonitoringScheduleConfigUnionTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateMonitoringScheduleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MonitoringScheduleConfigTypeDef](./type_defs.md#monitoringscheduleconfigtypedef) [:material-code-braces: MonitoringScheduleConfigOutputTypeDef](./type_defs.md#monitoringscheduleconfigoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateMonitoringScheduleResponseTypeDef](./type_defs.md#createmonitoringscheduleresponsetypedef) 


```python
# create_monitoring_schedule method usage example with argument unpacking

kwargs: CreateMonitoringScheduleRequestTypeDef = {  # (1)
    "MonitoringScheduleName": ...,
    "MonitoringScheduleConfig": ...,
}

parent.create_monitoring_schedule(**kwargs)
```

1. See [:material-code-braces: CreateMonitoringScheduleRequestTypeDef](./type_defs.md#createmonitoringschedulerequesttypedef) 

### create\_notebook\_instance

Creates an SageMaker AI notebook instance.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_notebook_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_notebook_instance.html)

```python
# create_notebook_instance method definition

await def create_notebook_instance(
    self,
    *,
    NotebookInstanceName: str,
    InstanceType: InstanceTypeType,  # (1)
    RoleArn: str,
    SubnetId: str = ...,
    SecurityGroupIds: Sequence[str] = ...,
    KmsKeyId: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    LifecycleConfigName: str = ...,
    DirectInternetAccess: DirectInternetAccessType = ...,  # (3)
    VolumeSizeInGB: int = ...,
    AcceleratorTypes: Sequence[NotebookInstanceAcceleratorTypeType] = ...,  # (4)
    DefaultCodeRepository: str = ...,
    AdditionalCodeRepositories: Sequence[str] = ...,
    RootAccess: RootAccessType = ...,  # (5)
    PlatformIdentifier: str = ...,
    InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef = ...,  # (6)
) -> CreateNotebookInstanceOutputTypeDef:  # (7)
    ...
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: DirectInternetAccessType](./literals.md#directinternetaccesstype) 
4. See [:material-code-brackets: NotebookInstanceAcceleratorTypeType](./literals.md#notebookinstanceacceleratortypetype) 
5. See [:material-code-brackets: RootAccessType](./literals.md#rootaccesstype) 
6. See [:material-code-braces: InstanceMetadataServiceConfigurationTypeDef](./type_defs.md#instancemetadataserviceconfigurationtypedef) 
7. See [:material-code-braces: CreateNotebookInstanceOutputTypeDef](./type_defs.md#createnotebookinstanceoutputtypedef) 


```python
# create_notebook_instance method usage example with argument unpacking

kwargs: CreateNotebookInstanceInputTypeDef = {  # (1)
    "NotebookInstanceName": ...,
    "InstanceType": ...,
    "RoleArn": ...,
}

parent.create_notebook_instance(**kwargs)
```

1. See [:material-code-braces: CreateNotebookInstanceInputTypeDef](./type_defs.md#createnotebookinstanceinputtypedef) 

### create\_notebook\_instance\_lifecycle\_config

Creates a lifecycle configuration that you can associate with a notebook
instance.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_notebook_instance_lifecycle_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_notebook_instance_lifecycle_config.html)

```python
# create_notebook_instance_lifecycle_config method definition

await def create_notebook_instance_lifecycle_config(
    self,
    *,
    NotebookInstanceLifecycleConfigName: str,
    OnCreate: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,  # (1)
    OnStart: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,  # (1)
) -> CreateNotebookInstanceLifecycleConfigOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef) 
2. See [:material-code-braces: NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef) 
3. See [:material-code-braces: CreateNotebookInstanceLifecycleConfigOutputTypeDef](./type_defs.md#createnotebookinstancelifecycleconfigoutputtypedef) 


```python
# create_notebook_instance_lifecycle_config method usage example with argument unpacking

kwargs: CreateNotebookInstanceLifecycleConfigInputTypeDef = {  # (1)
    "NotebookInstanceLifecycleConfigName": ...,
}

parent.create_notebook_instance_lifecycle_config(**kwargs)
```

1. See [:material-code-braces: CreateNotebookInstanceLifecycleConfigInputTypeDef](./type_defs.md#createnotebookinstancelifecycleconfiginputtypedef) 

### create\_optimization\_job

Creates a job that optimizes a model for inference performance.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_optimization_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_optimization_job.html)

```python
# create_optimization_job method definition

await def create_optimization_job(
    self,
    *,
    OptimizationJobName: str,
    RoleArn: str,
    ModelSource: OptimizationJobModelSourceTypeDef,  # (1)
    DeploymentInstanceType: OptimizationJobDeploymentInstanceTypeType,  # (2)
    OptimizationConfigs: Sequence[OptimizationConfigUnionTypeDef],  # (3)
    OutputConfig: OptimizationJobOutputConfigTypeDef,  # (4)
    StoppingCondition: StoppingConditionTypeDef,  # (5)
    OptimizationEnvironment: Mapping[str, str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (6)
    VpcConfig: OptimizationVpcConfigUnionTypeDef = ...,  # (7)
) -> CreateOptimizationJobResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: OptimizationJobModelSourceTypeDef](./type_defs.md#optimizationjobmodelsourcetypedef) 
2. See [:material-code-brackets: OptimizationJobDeploymentInstanceTypeType](./literals.md#optimizationjobdeploymentinstancetypetype) 
3. See [:material-code-braces: OptimizationConfigTypeDef](./type_defs.md#optimizationconfigtypedef) [:material-code-braces: OptimizationConfigOutputTypeDef](./type_defs.md#optimizationconfigoutputtypedef) 
4. See [:material-code-braces: OptimizationJobOutputConfigTypeDef](./type_defs.md#optimizationjoboutputconfigtypedef) 
5. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: OptimizationVpcConfigTypeDef](./type_defs.md#optimizationvpcconfigtypedef) [:material-code-braces: OptimizationVpcConfigOutputTypeDef](./type_defs.md#optimizationvpcconfigoutputtypedef) 
8. See [:material-code-braces: CreateOptimizationJobResponseTypeDef](./type_defs.md#createoptimizationjobresponsetypedef) 


```python
# create_optimization_job method usage example with argument unpacking

kwargs: CreateOptimizationJobRequestTypeDef = {  # (1)
    "OptimizationJobName": ...,
    "RoleArn": ...,
    "ModelSource": ...,
    "DeploymentInstanceType": ...,
    "OptimizationConfigs": ...,
    "OutputConfig": ...,
    "StoppingCondition": ...,
}

parent.create_optimization_job(**kwargs)
```

1. See [:material-code-braces: CreateOptimizationJobRequestTypeDef](./type_defs.md#createoptimizationjobrequesttypedef) 

### create\_partner\_app

Creates an Amazon SageMaker Partner AI App.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_partner_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_partner_app.html)

```python
# create_partner_app method definition

await def create_partner_app(
    self,
    *,
    Name: str,
    Type: PartnerAppTypeType,  # (1)
    ExecutionRoleArn: str,
    Tier: str,
    AuthType: PartnerAppAuthTypeType,  # (2)
    MaintenanceConfig: PartnerAppMaintenanceConfigTypeDef = ...,  # (3)
    ApplicationConfig: PartnerAppConfigUnionTypeDef = ...,  # (4)
    EnableIamSessionBasedIdentity: bool = ...,
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> CreatePartnerAppResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: PartnerAppTypeType](./literals.md#partnerapptypetype) 
2. See [:material-code-brackets: PartnerAppAuthTypeType](./literals.md#partnerappauthtypetype) 
3. See [:material-code-braces: PartnerAppMaintenanceConfigTypeDef](./type_defs.md#partnerappmaintenanceconfigtypedef) 
4. See [:material-code-braces: PartnerAppConfigTypeDef](./type_defs.md#partnerappconfigtypedef) [:material-code-braces: PartnerAppConfigOutputTypeDef](./type_defs.md#partnerappconfigoutputtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: CreatePartnerAppResponseTypeDef](./type_defs.md#createpartnerappresponsetypedef) 


```python
# create_partner_app method usage example with argument unpacking

kwargs: CreatePartnerAppRequestTypeDef = {  # (1)
    "Name": ...,
    "Type": ...,
    "ExecutionRoleArn": ...,
    "Tier": ...,
    "AuthType": ...,
}

parent.create_partner_app(**kwargs)
```

1. See [:material-code-braces: CreatePartnerAppRequestTypeDef](./type_defs.md#createpartnerapprequesttypedef) 

### create\_partner\_app\_presigned\_url

Creates a presigned URL to access an Amazon SageMaker Partner AI App.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_partner_app_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_partner_app_presigned_url.html)

```python
# create_partner_app_presigned_url method definition

await def create_partner_app_presigned_url(
    self,
    *,
    Arn: str,
    ExpiresInSeconds: int = ...,
    SessionExpirationDurationInSeconds: int = ...,
) -> CreatePartnerAppPresignedUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePartnerAppPresignedUrlResponseTypeDef](./type_defs.md#createpartnerapppresignedurlresponsetypedef) 


```python
# create_partner_app_presigned_url method usage example with argument unpacking

kwargs: CreatePartnerAppPresignedUrlRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.create_partner_app_presigned_url(**kwargs)
```

1. See [:material-code-braces: CreatePartnerAppPresignedUrlRequestTypeDef](./type_defs.md#createpartnerapppresignedurlrequesttypedef) 

### create\_pipeline

Creates a pipeline using a JSON pipeline definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_pipeline.html)

```python
# create_pipeline method definition

await def create_pipeline(
    self,
    *,
    PipelineName: str,
    ClientRequestToken: str,
    RoleArn: str,
    PipelineDisplayName: str = ...,
    PipelineDefinition: str = ...,
    PipelineDefinitionS3Location: PipelineDefinitionS3LocationTypeDef = ...,  # (1)
    PipelineDescription: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,  # (3)
) -> CreatePipelineResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: PipelineDefinitionS3LocationTypeDef](./type_defs.md#pipelinedefinitions3locationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
4. See [:material-code-braces: CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef) 


```python
# create_pipeline method usage example with argument unpacking

kwargs: CreatePipelineRequestTypeDef = {  # (1)
    "PipelineName": ...,
    "ClientRequestToken": ...,
    "RoleArn": ...,
}

parent.create_pipeline(**kwargs)
```

1. See [:material-code-braces: CreatePipelineRequestTypeDef](./type_defs.md#createpipelinerequesttypedef) 

### create\_presigned\_domain\_url

Creates a URL for a specified UserProfile in a Domain.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_presigned_domain_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_presigned_domain_url.html)

```python
# create_presigned_domain_url method definition

await def create_presigned_domain_url(
    self,
    *,
    DomainId: str,
    UserProfileName: str,
    SessionExpirationDurationInSeconds: int = ...,
    ExpiresInSeconds: int = ...,
    SpaceName: str = ...,
    LandingUri: str = ...,
) -> CreatePresignedDomainUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePresignedDomainUrlResponseTypeDef](./type_defs.md#createpresigneddomainurlresponsetypedef) 


```python
# create_presigned_domain_url method usage example with argument unpacking

kwargs: CreatePresignedDomainUrlRequestTypeDef = {  # (1)
    "DomainId": ...,
    "UserProfileName": ...,
}

parent.create_presigned_domain_url(**kwargs)
```

1. See [:material-code-braces: CreatePresignedDomainUrlRequestTypeDef](./type_defs.md#createpresigneddomainurlrequesttypedef) 

### create\_presigned\_mlflow\_tracking\_server\_url

Returns a presigned URL that you can use to connect to the MLflow UI attached
to your tracking server.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_presigned_mlflow_tracking_server_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_presigned_mlflow_tracking_server_url.html)

```python
# create_presigned_mlflow_tracking_server_url method definition

await def create_presigned_mlflow_tracking_server_url(
    self,
    *,
    TrackingServerName: str,
    ExpiresInSeconds: int = ...,
    SessionExpirationDurationInSeconds: int = ...,
) -> CreatePresignedMlflowTrackingServerUrlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePresignedMlflowTrackingServerUrlResponseTypeDef](./type_defs.md#createpresignedmlflowtrackingserverurlresponsetypedef) 


```python
# create_presigned_mlflow_tracking_server_url method usage example with argument unpacking

kwargs: CreatePresignedMlflowTrackingServerUrlRequestTypeDef = {  # (1)
    "TrackingServerName": ...,
}

parent.create_presigned_mlflow_tracking_server_url(**kwargs)
```

1. See [:material-code-braces: CreatePresignedMlflowTrackingServerUrlRequestTypeDef](./type_defs.md#createpresignedmlflowtrackingserverurlrequesttypedef) 

### create\_presigned\_notebook\_instance\_url

Returns a URL that you can use to connect to the Jupyter server from a notebook
instance.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_presigned_notebook_instance_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_presigned_notebook_instance_url.html)

```python
# create_presigned_notebook_instance_url method definition

await def create_presigned_notebook_instance_url(
    self,
    *,
    NotebookInstanceName: str,
    SessionExpirationDurationInSeconds: int = ...,
) -> CreatePresignedNotebookInstanceUrlOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePresignedNotebookInstanceUrlOutputTypeDef](./type_defs.md#createpresignednotebookinstanceurloutputtypedef) 


```python
# create_presigned_notebook_instance_url method usage example with argument unpacking

kwargs: CreatePresignedNotebookInstanceUrlInputTypeDef = {  # (1)
    "NotebookInstanceName": ...,
}

parent.create_presigned_notebook_instance_url(**kwargs)
```

1. See [:material-code-braces: CreatePresignedNotebookInstanceUrlInputTypeDef](./type_defs.md#createpresignednotebookinstanceurlinputtypedef) 

### create\_processing\_job

Creates a processing job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_processing_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_processing_job.html)

```python
# create_processing_job method definition

await def create_processing_job(
    self,
    *,
    ProcessingJobName: str,
    ProcessingResources: ProcessingResourcesTypeDef,  # (1)
    AppSpecification: AppSpecificationUnionTypeDef,  # (2)
    RoleArn: str,
    ProcessingInputs: Sequence[ProcessingInputTypeDef] = ...,  # (3)
    ProcessingOutputConfig: ProcessingOutputConfigUnionTypeDef = ...,  # (4)
    StoppingCondition: ProcessingStoppingConditionTypeDef = ...,  # (5)
    Environment: Mapping[str, str] = ...,
    NetworkConfig: NetworkConfigUnionTypeDef = ...,  # (6)
    Tags: Sequence[TagTypeDef] = ...,  # (7)
    ExperimentConfig: ExperimentConfigTypeDef = ...,  # (8)
) -> CreateProcessingJobResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: ProcessingResourcesTypeDef](./type_defs.md#processingresourcestypedef) 
2. See [:material-code-braces: AppSpecificationTypeDef](./type_defs.md#appspecificationtypedef) [:material-code-braces: AppSpecificationOutputTypeDef](./type_defs.md#appspecificationoutputtypedef) 
3. See [:material-code-braces: ProcessingInputTypeDef](./type_defs.md#processinginputtypedef) 
4. See [:material-code-braces: ProcessingOutputConfigTypeDef](./type_defs.md#processingoutputconfigtypedef) [:material-code-braces: ProcessingOutputConfigOutputTypeDef](./type_defs.md#processingoutputconfigoutputtypedef) 
5. See [:material-code-braces: ProcessingStoppingConditionTypeDef](./type_defs.md#processingstoppingconditiontypedef) 
6. See [:material-code-braces: NetworkConfigTypeDef](./type_defs.md#networkconfigtypedef) [:material-code-braces: NetworkConfigOutputTypeDef](./type_defs.md#networkconfigoutputtypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
9. See [:material-code-braces: CreateProcessingJobResponseTypeDef](./type_defs.md#createprocessingjobresponsetypedef) 


```python
# create_processing_job method usage example with argument unpacking

kwargs: CreateProcessingJobRequestTypeDef = {  # (1)
    "ProcessingJobName": ...,
    "ProcessingResources": ...,
    "AppSpecification": ...,
    "RoleArn": ...,
}

parent.create_processing_job(**kwargs)
```

1. See [:material-code-braces: CreateProcessingJobRequestTypeDef](./type_defs.md#createprocessingjobrequesttypedef) 

### create\_project

Creates a machine learning (ML) project that can contain one or more templates
that set up an ML pipeline from training to deploying an approved model.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_project.html)

```python
# create_project method definition

await def create_project(
    self,
    *,
    ProjectName: str,
    ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsUnionTypeDef,  # (1)
    ProjectDescription: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateProjectOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ServiceCatalogProvisioningDetailsTypeDef](./type_defs.md#servicecatalogprovisioningdetailstypedef) [:material-code-braces: ServiceCatalogProvisioningDetailsOutputTypeDef](./type_defs.md#servicecatalogprovisioningdetailsoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateProjectOutputTypeDef](./type_defs.md#createprojectoutputtypedef) 


```python
# create_project method usage example with argument unpacking

kwargs: CreateProjectInputTypeDef = {  # (1)
    "ProjectName": ...,
    "ServiceCatalogProvisioningDetails": ...,
}

parent.create_project(**kwargs)
```

1. See [:material-code-braces: CreateProjectInputTypeDef](./type_defs.md#createprojectinputtypedef) 

### create\_space

Creates a private space or a space used for real time collaboration in a domain.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_space.html)

```python
# create_space method definition

await def create_space(
    self,
    *,
    DomainId: str,
    SpaceName: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    SpaceSettings: SpaceSettingsUnionTypeDef = ...,  # (2)
    OwnershipSettings: OwnershipSettingsTypeDef = ...,  # (3)
    SpaceSharingSettings: SpaceSharingSettingsTypeDef = ...,  # (4)
    SpaceDisplayName: str = ...,
) -> CreateSpaceResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: SpaceSettingsTypeDef](./type_defs.md#spacesettingstypedef) [:material-code-braces: SpaceSettingsOutputTypeDef](./type_defs.md#spacesettingsoutputtypedef) 
3. See [:material-code-braces: OwnershipSettingsTypeDef](./type_defs.md#ownershipsettingstypedef) 
4. See [:material-code-braces: SpaceSharingSettingsTypeDef](./type_defs.md#spacesharingsettingstypedef) 
5. See [:material-code-braces: CreateSpaceResponseTypeDef](./type_defs.md#createspaceresponsetypedef) 


```python
# create_space method usage example with argument unpacking

kwargs: CreateSpaceRequestTypeDef = {  # (1)
    "DomainId": ...,
    "SpaceName": ...,
}

parent.create_space(**kwargs)
```

1. See [:material-code-braces: CreateSpaceRequestTypeDef](./type_defs.md#createspacerequesttypedef) 

### create\_studio\_lifecycle\_config

Creates a new Amazon SageMaker AI Studio Lifecycle Configuration.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_studio_lifecycle_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_studio_lifecycle_config.html)

```python
# create_studio_lifecycle_config method definition

await def create_studio_lifecycle_config(
    self,
    *,
    StudioLifecycleConfigName: str,
    StudioLifecycleConfigContent: str,
    StudioLifecycleConfigAppType: StudioLifecycleConfigAppTypeType,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateStudioLifecycleConfigResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: StudioLifecycleConfigAppTypeType](./literals.md#studiolifecycleconfigapptypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateStudioLifecycleConfigResponseTypeDef](./type_defs.md#createstudiolifecycleconfigresponsetypedef) 


```python
# create_studio_lifecycle_config method usage example with argument unpacking

kwargs: CreateStudioLifecycleConfigRequestTypeDef = {  # (1)
    "StudioLifecycleConfigName": ...,
    "StudioLifecycleConfigContent": ...,
    "StudioLifecycleConfigAppType": ...,
}

parent.create_studio_lifecycle_config(**kwargs)
```

1. See [:material-code-braces: CreateStudioLifecycleConfigRequestTypeDef](./type_defs.md#createstudiolifecycleconfigrequesttypedef) 

### create\_training\_job

Starts a model training job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_training_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_training_job.html)

```python
# create_training_job method definition

await def create_training_job(
    self,
    *,
    TrainingJobName: str,
    AlgorithmSpecification: AlgorithmSpecificationUnionTypeDef,  # (1)
    RoleArn: str,
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    ResourceConfig: ResourceConfigUnionTypeDef,  # (3)
    StoppingCondition: StoppingConditionTypeDef,  # (4)
    HyperParameters: Mapping[str, str] = ...,
    InputDataConfig: Sequence[ChannelUnionTypeDef] = ...,  # (5)
    VpcConfig: VpcConfigUnionTypeDef = ...,  # (6)
    Tags: Sequence[TagTypeDef] = ...,  # (7)
    EnableNetworkIsolation: bool = ...,
    EnableInterContainerTrafficEncryption: bool = ...,
    EnableManagedSpotTraining: bool = ...,
    CheckpointConfig: CheckpointConfigTypeDef = ...,  # (8)
    DebugHookConfig: DebugHookConfigUnionTypeDef = ...,  # (9)
    DebugRuleConfigurations: Sequence[DebugRuleConfigurationUnionTypeDef] = ...,  # (10)
    TensorBoardOutputConfig: TensorBoardOutputConfigTypeDef = ...,  # (11)
    ExperimentConfig: ExperimentConfigTypeDef = ...,  # (12)
    ProfilerConfig: ProfilerConfigUnionTypeDef = ...,  # (13)
    ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationUnionTypeDef] = ...,  # (14)
    Environment: Mapping[str, str] = ...,
    RetryStrategy: RetryStrategyTypeDef = ...,  # (15)
    RemoteDebugConfig: RemoteDebugConfigTypeDef = ...,  # (16)
    InfraCheckConfig: InfraCheckConfigTypeDef = ...,  # (17)
    SessionChainingConfig: SessionChainingConfigTypeDef = ...,  # (18)
) -> CreateTrainingJobResponseTypeDef:  # (19)
    ...
```

1. See [:material-code-braces: AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef) [:material-code-braces: AlgorithmSpecificationOutputTypeDef](./type_defs.md#algorithmspecificationoutputtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) [:material-code-braces: ResourceConfigOutputTypeDef](./type_defs.md#resourceconfigoutputtypedef) 
4. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
5. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) [:material-code-braces: ChannelOutputTypeDef](./type_defs.md#channeloutputtypedef) 
6. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: CheckpointConfigTypeDef](./type_defs.md#checkpointconfigtypedef) 
9. See [:material-code-braces: DebugHookConfigTypeDef](./type_defs.md#debughookconfigtypedef) [:material-code-braces: DebugHookConfigOutputTypeDef](./type_defs.md#debughookconfigoutputtypedef) 
10. See [:material-code-braces: DebugRuleConfigurationTypeDef](./type_defs.md#debugruleconfigurationtypedef) [:material-code-braces: DebugRuleConfigurationOutputTypeDef](./type_defs.md#debugruleconfigurationoutputtypedef) 
11. See [:material-code-braces: TensorBoardOutputConfigTypeDef](./type_defs.md#tensorboardoutputconfigtypedef) 
12. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
13. See [:material-code-braces: ProfilerConfigTypeDef](./type_defs.md#profilerconfigtypedef) [:material-code-braces: ProfilerConfigOutputTypeDef](./type_defs.md#profilerconfigoutputtypedef) 
14. See [:material-code-braces: ProfilerRuleConfigurationTypeDef](./type_defs.md#profilerruleconfigurationtypedef) [:material-code-braces: ProfilerRuleConfigurationOutputTypeDef](./type_defs.md#profilerruleconfigurationoutputtypedef) 
15. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
16. See [:material-code-braces: RemoteDebugConfigTypeDef](./type_defs.md#remotedebugconfigtypedef) 
17. See [:material-code-braces: InfraCheckConfigTypeDef](./type_defs.md#infracheckconfigtypedef) 
18. See [:material-code-braces: SessionChainingConfigTypeDef](./type_defs.md#sessionchainingconfigtypedef) 
19. See [:material-code-braces: CreateTrainingJobResponseTypeDef](./type_defs.md#createtrainingjobresponsetypedef) 


```python
# create_training_job method usage example with argument unpacking

kwargs: CreateTrainingJobRequestTypeDef = {  # (1)
    "TrainingJobName": ...,
    "AlgorithmSpecification": ...,
    "RoleArn": ...,
    "OutputDataConfig": ...,
    "ResourceConfig": ...,
    "StoppingCondition": ...,
}

parent.create_training_job(**kwargs)
```

1. See [:material-code-braces: CreateTrainingJobRequestTypeDef](./type_defs.md#createtrainingjobrequesttypedef) 

### create\_training\_plan

Creates a new training plan in SageMaker to reserve compute capacity.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_training_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_training_plan.html)

```python
# create_training_plan method definition

await def create_training_plan(
    self,
    *,
    TrainingPlanName: str,
    TrainingPlanOfferingId: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateTrainingPlanResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateTrainingPlanResponseTypeDef](./type_defs.md#createtrainingplanresponsetypedef) 


```python
# create_training_plan method usage example with argument unpacking

kwargs: CreateTrainingPlanRequestTypeDef = {  # (1)
    "TrainingPlanName": ...,
    "TrainingPlanOfferingId": ...,
}

parent.create_training_plan(**kwargs)
```

1. See [:material-code-braces: CreateTrainingPlanRequestTypeDef](./type_defs.md#createtrainingplanrequesttypedef) 

### create\_transform\_job

Starts a transform job.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_transform_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_transform_job.html)

```python
# create_transform_job method definition

await def create_transform_job(
    self,
    *,
    TransformJobName: str,
    ModelName: str,
    TransformInput: TransformInputTypeDef,  # (1)
    TransformOutput: TransformOutputTypeDef,  # (2)
    TransformResources: TransformResourcesTypeDef,  # (3)
    MaxConcurrentTransforms: int = ...,
    ModelClientConfig: ModelClientConfigTypeDef = ...,  # (4)
    MaxPayloadInMB: int = ...,
    BatchStrategy: BatchStrategyType = ...,  # (5)
    Environment: Mapping[str, str] = ...,
    DataCaptureConfig: BatchDataCaptureConfigTypeDef = ...,  # (6)
    DataProcessing: DataProcessingTypeDef = ...,  # (7)
    Tags: Sequence[TagTypeDef] = ...,  # (8)
    ExperimentConfig: ExperimentConfigTypeDef = ...,  # (9)
) -> CreateTransformJobResponseTypeDef:  # (10)
    ...
```

1. See [:material-code-braces: TransformInputTypeDef](./type_defs.md#transforminputtypedef) 
2. See [:material-code-braces: TransformOutputTypeDef](./type_defs.md#transformoutputtypedef) 
3. See [:material-code-braces: TransformResourcesTypeDef](./type_defs.md#transformresourcestypedef) 
4. See [:material-code-braces: ModelClientConfigTypeDef](./type_defs.md#modelclientconfigtypedef) 
5. See [:material-code-brackets: BatchStrategyType](./literals.md#batchstrategytype) 
6. See [:material-code-braces: BatchDataCaptureConfigTypeDef](./type_defs.md#batchdatacaptureconfigtypedef) 
7. See [:material-code-braces: DataProcessingTypeDef](./type_defs.md#dataprocessingtypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
10. See [:material-code-braces: CreateTransformJobResponseTypeDef](./type_defs.md#createtransformjobresponsetypedef) 


```python
# create_transform_job method usage example with argument unpacking

kwargs: CreateTransformJobRequestTypeDef = {  # (1)
    "TransformJobName": ...,
    "ModelName": ...,
    "TransformInput": ...,
    "TransformOutput": ...,
    "TransformResources": ...,
}

parent.create_transform_job(**kwargs)
```

1. See [:material-code-braces: CreateTransformJobRequestTypeDef](./type_defs.md#createtransformjobrequesttypedef) 

### create\_trial

Creates an SageMaker <i>trial</i>.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_trial` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_trial.html)

```python
# create_trial method definition

await def create_trial(
    self,
    *,
    TrialName: str,
    ExperimentName: str,
    DisplayName: str = ...,
    MetadataProperties: MetadataPropertiesTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateTrialResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateTrialResponseTypeDef](./type_defs.md#createtrialresponsetypedef) 


```python
# create_trial method usage example with argument unpacking

kwargs: CreateTrialRequestTypeDef = {  # (1)
    "TrialName": ...,
    "ExperimentName": ...,
}

parent.create_trial(**kwargs)
```

1. See [:material-code-braces: CreateTrialRequestTypeDef](./type_defs.md#createtrialrequesttypedef) 

### create\_trial\_component

Creates a <i>trial component</i>, which is a stage of a machine learning
<i>trial</i>.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_trial_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_trial_component.html)

```python
# create_trial_component method definition

await def create_trial_component(
    self,
    *,
    TrialComponentName: str,
    DisplayName: str = ...,
    Status: TrialComponentStatusTypeDef = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Parameters: Mapping[str, TrialComponentParameterValueTypeDef] = ...,  # (2)
    InputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,  # (3)
    OutputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,  # (3)
    MetadataProperties: MetadataPropertiesTypeDef = ...,  # (5)
    Tags: Sequence[TagTypeDef] = ...,  # (6)
) -> CreateTrialComponentResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: TrialComponentStatusTypeDef](./type_defs.md#trialcomponentstatustypedef) 
2. See [:material-code-braces: TrialComponentParameterValueTypeDef](./type_defs.md#trialcomponentparametervaluetypedef) 
3. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
4. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
5. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: CreateTrialComponentResponseTypeDef](./type_defs.md#createtrialcomponentresponsetypedef) 


```python
# create_trial_component method usage example with argument unpacking

kwargs: CreateTrialComponentRequestTypeDef = {  # (1)
    "TrialComponentName": ...,
}

parent.create_trial_component(**kwargs)
```

1. See [:material-code-braces: CreateTrialComponentRequestTypeDef](./type_defs.md#createtrialcomponentrequesttypedef) 

### create\_user\_profile

Creates a user profile.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_user_profile.html)

```python
# create_user_profile method definition

await def create_user_profile(
    self,
    *,
    DomainId: str,
    UserProfileName: str,
    SingleSignOnUserIdentifier: str = ...,
    SingleSignOnUserValue: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    UserSettings: UserSettingsUnionTypeDef = ...,  # (2)
) -> CreateUserProfileResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) [:material-code-braces: UserSettingsOutputTypeDef](./type_defs.md#usersettingsoutputtypedef) 
3. See [:material-code-braces: CreateUserProfileResponseTypeDef](./type_defs.md#createuserprofileresponsetypedef) 


```python
# create_user_profile method usage example with argument unpacking

kwargs: CreateUserProfileRequestTypeDef = {  # (1)
    "DomainId": ...,
    "UserProfileName": ...,
}

parent.create_user_profile(**kwargs)
```

1. See [:material-code-braces: CreateUserProfileRequestTypeDef](./type_defs.md#createuserprofilerequesttypedef) 

### create\_workforce

Use this operation to create a workforce.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_workforce` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_workforce.html)

```python
# create_workforce method definition

await def create_workforce(
    self,
    *,
    WorkforceName: str,
    CognitoConfig: CognitoConfigTypeDef = ...,  # (1)
    OidcConfig: OidcConfigTypeDef = ...,  # (2)
    SourceIpConfig: SourceIpConfigUnionTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...,  # (5)
) -> CreateWorkforceResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: CognitoConfigTypeDef](./type_defs.md#cognitoconfigtypedef) 
2. See [:material-code-braces: OidcConfigTypeDef](./type_defs.md#oidcconfigtypedef) 
3. See [:material-code-braces: SourceIpConfigTypeDef](./type_defs.md#sourceipconfigtypedef) [:material-code-braces: SourceIpConfigOutputTypeDef](./type_defs.md#sourceipconfigoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: WorkforceVpcConfigRequestTypeDef](./type_defs.md#workforcevpcconfigrequesttypedef) 
6. See [:material-code-braces: CreateWorkforceResponseTypeDef](./type_defs.md#createworkforceresponsetypedef) 


```python
# create_workforce method usage example with argument unpacking

kwargs: CreateWorkforceRequestTypeDef = {  # (1)
    "WorkforceName": ...,
}

parent.create_workforce(**kwargs)
```

1. See [:material-code-braces: CreateWorkforceRequestTypeDef](./type_defs.md#createworkforcerequesttypedef) 

### create\_workteam

Creates a new work team for labeling your data.

Type annotations and code completion for `#!python session.create_client("sagemaker").create_workteam` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/create_workteam.html)

```python
# create_workteam method definition

await def create_workteam(
    self,
    *,
    WorkteamName: str,
    MemberDefinitions: Sequence[MemberDefinitionUnionTypeDef],  # (1)
    Description: str,
    WorkforceName: str = ...,
    NotificationConfiguration: NotificationConfigurationTypeDef = ...,  # (2)
    WorkerAccessConfiguration: WorkerAccessConfigurationTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateWorkteamResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: MemberDefinitionTypeDef](./type_defs.md#memberdefinitiontypedef) [:material-code-braces: MemberDefinitionOutputTypeDef](./type_defs.md#memberdefinitionoutputtypedef) 
2. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
3. See [:material-code-braces: WorkerAccessConfigurationTypeDef](./type_defs.md#workeraccessconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateWorkteamResponseTypeDef](./type_defs.md#createworkteamresponsetypedef) 


```python
# create_workteam method usage example with argument unpacking

kwargs: CreateWorkteamRequestTypeDef = {  # (1)
    "WorkteamName": ...,
    "MemberDefinitions": ...,
    "Description": ...,
}

parent.create_workteam(**kwargs)
```

1. See [:material-code-braces: CreateWorkteamRequestTypeDef](./type_defs.md#createworkteamrequesttypedef) 

### delete\_action

Deletes an action.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_action.html)

```python
# delete_action method definition

await def delete_action(
    self,
    *,
    ActionName: str,
) -> DeleteActionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteActionResponseTypeDef](./type_defs.md#deleteactionresponsetypedef) 


```python
# delete_action method usage example with argument unpacking

kwargs: DeleteActionRequestTypeDef = {  # (1)
    "ActionName": ...,
}

parent.delete_action(**kwargs)
```

1. See [:material-code-braces: DeleteActionRequestTypeDef](./type_defs.md#deleteactionrequesttypedef) 

### delete\_algorithm

Removes the specified algorithm from your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_algorithm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_algorithm.html)

```python
# delete_algorithm method definition

await def delete_algorithm(
    self,
    *,
    AlgorithmName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_algorithm method usage example with argument unpacking

kwargs: DeleteAlgorithmInputTypeDef = {  # (1)
    "AlgorithmName": ...,
}

parent.delete_algorithm(**kwargs)
```

1. See [:material-code-braces: DeleteAlgorithmInputTypeDef](./type_defs.md#deletealgorithminputtypedef) 

### delete\_app

Used to stop and delete an app.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_app.html)

```python
# delete_app method definition

await def delete_app(
    self,
    *,
    DomainId: str,
    AppType: AppTypeType,  # (1)
    AppName: str,
    UserProfileName: str = ...,
    SpaceName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_app method usage example with argument unpacking

kwargs: DeleteAppRequestTypeDef = {  # (1)
    "DomainId": ...,
    "AppType": ...,
    "AppName": ...,
}

parent.delete_app(**kwargs)
```

1. See [:material-code-braces: DeleteAppRequestTypeDef](./type_defs.md#deleteapprequesttypedef) 

### delete\_app\_image\_config

Deletes an AppImageConfig.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_app_image_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_app_image_config.html)

```python
# delete_app_image_config method definition

await def delete_app_image_config(
    self,
    *,
    AppImageConfigName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_app_image_config method usage example with argument unpacking

kwargs: DeleteAppImageConfigRequestTypeDef = {  # (1)
    "AppImageConfigName": ...,
}

parent.delete_app_image_config(**kwargs)
```

1. See [:material-code-braces: DeleteAppImageConfigRequestTypeDef](./type_defs.md#deleteappimageconfigrequesttypedef) 

### delete\_artifact

Deletes an artifact.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_artifact.html)

```python
# delete_artifact method definition

await def delete_artifact(
    self,
    *,
    ArtifactArn: str = ...,
    Source: ArtifactSourceUnionTypeDef = ...,  # (1)
) -> DeleteArtifactResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ArtifactSourceTypeDef](./type_defs.md#artifactsourcetypedef) [:material-code-braces: ArtifactSourceOutputTypeDef](./type_defs.md#artifactsourceoutputtypedef) 
2. See [:material-code-braces: DeleteArtifactResponseTypeDef](./type_defs.md#deleteartifactresponsetypedef) 


```python
# delete_artifact method usage example with argument unpacking

kwargs: DeleteArtifactRequestTypeDef = {  # (1)
    "ArtifactArn": ...,
}

parent.delete_artifact(**kwargs)
```

1. See [:material-code-braces: DeleteArtifactRequestTypeDef](./type_defs.md#deleteartifactrequesttypedef) 

### delete\_association

Deletes an association.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_association.html)

```python
# delete_association method definition

await def delete_association(
    self,
    *,
    SourceArn: str,
    DestinationArn: str,
) -> DeleteAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAssociationResponseTypeDef](./type_defs.md#deleteassociationresponsetypedef) 


```python
# delete_association method usage example with argument unpacking

kwargs: DeleteAssociationRequestTypeDef = {  # (1)
    "SourceArn": ...,
    "DestinationArn": ...,
}

parent.delete_association(**kwargs)
```

1. See [:material-code-braces: DeleteAssociationRequestTypeDef](./type_defs.md#deleteassociationrequesttypedef) 

### delete\_cluster

Delete a SageMaker HyperPod cluster.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_cluster.html)

```python
# delete_cluster method definition

await def delete_cluster(
    self,
    *,
    ClusterName: str,
) -> DeleteClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef) 


```python
# delete_cluster method usage example with argument unpacking

kwargs: DeleteClusterRequestTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.delete_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteClusterRequestTypeDef](./type_defs.md#deleteclusterrequesttypedef) 

### delete\_cluster\_scheduler\_config

Deletes the cluster policy of the cluster.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_cluster_scheduler_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_cluster_scheduler_config.html)

```python
# delete_cluster_scheduler_config method definition

await def delete_cluster_scheduler_config(
    self,
    *,
    ClusterSchedulerConfigId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_cluster_scheduler_config method usage example with argument unpacking

kwargs: DeleteClusterSchedulerConfigRequestTypeDef = {  # (1)
    "ClusterSchedulerConfigId": ...,
}

parent.delete_cluster_scheduler_config(**kwargs)
```

1. See [:material-code-braces: DeleteClusterSchedulerConfigRequestTypeDef](./type_defs.md#deleteclusterschedulerconfigrequesttypedef) 

### delete\_code\_repository

Deletes the specified Git repository from your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_code_repository` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_code_repository.html)

```python
# delete_code_repository method definition

await def delete_code_repository(
    self,
    *,
    CodeRepositoryName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_code_repository method usage example with argument unpacking

kwargs: DeleteCodeRepositoryInputTypeDef = {  # (1)
    "CodeRepositoryName": ...,
}

parent.delete_code_repository(**kwargs)
```

1. See [:material-code-braces: DeleteCodeRepositoryInputTypeDef](./type_defs.md#deletecoderepositoryinputtypedef) 

### delete\_compilation\_job

Deletes the specified compilation job.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_compilation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_compilation_job.html)

```python
# delete_compilation_job method definition

await def delete_compilation_job(
    self,
    *,
    CompilationJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_compilation_job method usage example with argument unpacking

kwargs: DeleteCompilationJobRequestTypeDef = {  # (1)
    "CompilationJobName": ...,
}

parent.delete_compilation_job(**kwargs)
```

1. See [:material-code-braces: DeleteCompilationJobRequestTypeDef](./type_defs.md#deletecompilationjobrequesttypedef) 

### delete\_compute\_quota

Deletes the compute allocation from the cluster.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_compute_quota` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_compute_quota.html)

```python
# delete_compute_quota method definition

await def delete_compute_quota(
    self,
    *,
    ComputeQuotaId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_compute_quota method usage example with argument unpacking

kwargs: DeleteComputeQuotaRequestTypeDef = {  # (1)
    "ComputeQuotaId": ...,
}

parent.delete_compute_quota(**kwargs)
```

1. See [:material-code-braces: DeleteComputeQuotaRequestTypeDef](./type_defs.md#deletecomputequotarequesttypedef) 

### delete\_context

Deletes an context.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_context` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_context.html)

```python
# delete_context method definition

await def delete_context(
    self,
    *,
    ContextName: str,
) -> DeleteContextResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteContextResponseTypeDef](./type_defs.md#deletecontextresponsetypedef) 


```python
# delete_context method usage example with argument unpacking

kwargs: DeleteContextRequestTypeDef = {  # (1)
    "ContextName": ...,
}

parent.delete_context(**kwargs)
```

1. See [:material-code-braces: DeleteContextRequestTypeDef](./type_defs.md#deletecontextrequesttypedef) 

### delete\_data\_quality\_job\_definition

Deletes a data quality monitoring job definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_data_quality_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_data_quality_job_definition.html)

```python
# delete_data_quality_job_definition method definition

await def delete_data_quality_job_definition(
    self,
    *,
    JobDefinitionName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_data_quality_job_definition method usage example with argument unpacking

kwargs: DeleteDataQualityJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
}

parent.delete_data_quality_job_definition(**kwargs)
```

1. See [:material-code-braces: DeleteDataQualityJobDefinitionRequestTypeDef](./type_defs.md#deletedataqualityjobdefinitionrequesttypedef) 

### delete\_device\_fleet

Deletes a fleet.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_device_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_device_fleet.html)

```python
# delete_device_fleet method definition

await def delete_device_fleet(
    self,
    *,
    DeviceFleetName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_device_fleet method usage example with argument unpacking

kwargs: DeleteDeviceFleetRequestTypeDef = {  # (1)
    "DeviceFleetName": ...,
}

parent.delete_device_fleet(**kwargs)
```

1. See [:material-code-braces: DeleteDeviceFleetRequestTypeDef](./type_defs.md#deletedevicefleetrequesttypedef) 

### delete\_domain

Used to delete a domain.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_domain.html)

```python
# delete_domain method definition

await def delete_domain(
    self,
    *,
    DomainId: str,
    RetentionPolicy: RetentionPolicyTypeDef = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RetentionPolicyTypeDef](./type_defs.md#retentionpolicytypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_domain method usage example with argument unpacking

kwargs: DeleteDomainRequestTypeDef = {  # (1)
    "DomainId": ...,
}

parent.delete_domain(**kwargs)
```

1. See [:material-code-braces: DeleteDomainRequestTypeDef](./type_defs.md#deletedomainrequesttypedef) 

### delete\_edge\_deployment\_plan

Deletes an edge deployment plan if (and only if) all the stages in the plan are
inactive or there are no stages in the plan.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_edge_deployment_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_edge_deployment_plan.html)

```python
# delete_edge_deployment_plan method definition

await def delete_edge_deployment_plan(
    self,
    *,
    EdgeDeploymentPlanName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_edge_deployment_plan method usage example with argument unpacking

kwargs: DeleteEdgeDeploymentPlanRequestTypeDef = {  # (1)
    "EdgeDeploymentPlanName": ...,
}

parent.delete_edge_deployment_plan(**kwargs)
```

1. See [:material-code-braces: DeleteEdgeDeploymentPlanRequestTypeDef](./type_defs.md#deleteedgedeploymentplanrequesttypedef) 

### delete\_edge\_deployment\_stage

Delete a stage in an edge deployment plan if (and only if) the stage is
inactive.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_edge_deployment_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_edge_deployment_stage.html)

```python
# delete_edge_deployment_stage method definition

await def delete_edge_deployment_stage(
    self,
    *,
    EdgeDeploymentPlanName: str,
    StageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_edge_deployment_stage method usage example with argument unpacking

kwargs: DeleteEdgeDeploymentStageRequestTypeDef = {  # (1)
    "EdgeDeploymentPlanName": ...,
    "StageName": ...,
}

parent.delete_edge_deployment_stage(**kwargs)
```

1. See [:material-code-braces: DeleteEdgeDeploymentStageRequestTypeDef](./type_defs.md#deleteedgedeploymentstagerequesttypedef) 

### delete\_endpoint

Deletes an endpoint.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_endpoint.html)

```python
# delete_endpoint method definition

await def delete_endpoint(
    self,
    *,
    EndpointName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_endpoint method usage example with argument unpacking

kwargs: DeleteEndpointInputTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.delete_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteEndpointInputTypeDef](./type_defs.md#deleteendpointinputtypedef) 

### delete\_endpoint\_config

Deletes an endpoint configuration.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_endpoint_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_endpoint_config.html)

```python
# delete_endpoint_config method definition

await def delete_endpoint_config(
    self,
    *,
    EndpointConfigName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_endpoint_config method usage example with argument unpacking

kwargs: DeleteEndpointConfigInputTypeDef = {  # (1)
    "EndpointConfigName": ...,
}

parent.delete_endpoint_config(**kwargs)
```

1. See [:material-code-braces: DeleteEndpointConfigInputTypeDef](./type_defs.md#deleteendpointconfiginputtypedef) 

### delete\_experiment

Deletes an SageMaker experiment.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_experiment.html)

```python
# delete_experiment method definition

await def delete_experiment(
    self,
    *,
    ExperimentName: str,
) -> DeleteExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteExperimentResponseTypeDef](./type_defs.md#deleteexperimentresponsetypedef) 


```python
# delete_experiment method usage example with argument unpacking

kwargs: DeleteExperimentRequestTypeDef = {  # (1)
    "ExperimentName": ...,
}

parent.delete_experiment(**kwargs)
```

1. See [:material-code-braces: DeleteExperimentRequestTypeDef](./type_defs.md#deleteexperimentrequesttypedef) 

### delete\_feature\_group

Delete the <code>FeatureGroup</code> and any data that was written to the
<code>OnlineStore</code> of the <code>FeatureGroup</code>.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_feature_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_feature_group.html)

```python
# delete_feature_group method definition

await def delete_feature_group(
    self,
    *,
    FeatureGroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_feature_group method usage example with argument unpacking

kwargs: DeleteFeatureGroupRequestTypeDef = {  # (1)
    "FeatureGroupName": ...,
}

parent.delete_feature_group(**kwargs)
```

1. See [:material-code-braces: DeleteFeatureGroupRequestTypeDef](./type_defs.md#deletefeaturegrouprequesttypedef) 

### delete\_flow\_definition

Deletes the specified flow definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_flow_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_flow_definition.html)

```python
# delete_flow_definition method definition

await def delete_flow_definition(
    self,
    *,
    FlowDefinitionName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_flow_definition method usage example with argument unpacking

kwargs: DeleteFlowDefinitionRequestTypeDef = {  # (1)
    "FlowDefinitionName": ...,
}

parent.delete_flow_definition(**kwargs)
```

1. See [:material-code-braces: DeleteFlowDefinitionRequestTypeDef](./type_defs.md#deleteflowdefinitionrequesttypedef) 

### delete\_hub

Delete a hub.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_hub` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_hub.html)

```python
# delete_hub method definition

await def delete_hub(
    self,
    *,
    HubName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_hub method usage example with argument unpacking

kwargs: DeleteHubRequestTypeDef = {  # (1)
    "HubName": ...,
}

parent.delete_hub(**kwargs)
```

1. See [:material-code-braces: DeleteHubRequestTypeDef](./type_defs.md#deletehubrequesttypedef) 

### delete\_hub\_content

Delete the contents of a hub.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_hub_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_hub_content.html)

```python
# delete_hub_content method definition

await def delete_hub_content(
    self,
    *,
    HubName: str,
    HubContentType: HubContentTypeType,  # (1)
    HubContentName: str,
    HubContentVersion: str,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_hub_content method usage example with argument unpacking

kwargs: DeleteHubContentRequestTypeDef = {  # (1)
    "HubName": ...,
    "HubContentType": ...,
    "HubContentName": ...,
    "HubContentVersion": ...,
}

parent.delete_hub_content(**kwargs)
```

1. See [:material-code-braces: DeleteHubContentRequestTypeDef](./type_defs.md#deletehubcontentrequesttypedef) 

### delete\_hub\_content\_reference

Delete a hub content reference in order to remove a model from a private hub.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_hub_content_reference` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_hub_content_reference.html)

```python
# delete_hub_content_reference method definition

await def delete_hub_content_reference(
    self,
    *,
    HubName: str,
    HubContentType: HubContentTypeType,  # (1)
    HubContentName: str,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_hub_content_reference method usage example with argument unpacking

kwargs: DeleteHubContentReferenceRequestTypeDef = {  # (1)
    "HubName": ...,
    "HubContentType": ...,
    "HubContentName": ...,
}

parent.delete_hub_content_reference(**kwargs)
```

1. See [:material-code-braces: DeleteHubContentReferenceRequestTypeDef](./type_defs.md#deletehubcontentreferencerequesttypedef) 

### delete\_human\_task\_ui

Use this operation to delete a human task user interface (worker task template).

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_human_task_ui` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_human_task_ui.html)

```python
# delete_human_task_ui method definition

await def delete_human_task_ui(
    self,
    *,
    HumanTaskUiName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_human_task_ui method usage example with argument unpacking

kwargs: DeleteHumanTaskUiRequestTypeDef = {  # (1)
    "HumanTaskUiName": ...,
}

parent.delete_human_task_ui(**kwargs)
```

1. See [:material-code-braces: DeleteHumanTaskUiRequestTypeDef](./type_defs.md#deletehumantaskuirequesttypedef) 

### delete\_hyper\_parameter\_tuning\_job

Deletes a hyperparameter tuning job.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_hyper_parameter_tuning_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_hyper_parameter_tuning_job.html)

```python
# delete_hyper_parameter_tuning_job method definition

await def delete_hyper_parameter_tuning_job(
    self,
    *,
    HyperParameterTuningJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_hyper_parameter_tuning_job method usage example with argument unpacking

kwargs: DeleteHyperParameterTuningJobRequestTypeDef = {  # (1)
    "HyperParameterTuningJobName": ...,
}

parent.delete_hyper_parameter_tuning_job(**kwargs)
```

1. See [:material-code-braces: DeleteHyperParameterTuningJobRequestTypeDef](./type_defs.md#deletehyperparametertuningjobrequesttypedef) 

### delete\_image

Deletes a SageMaker AI image and all versions of the image.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_image.html)

```python
# delete_image method definition

await def delete_image(
    self,
    *,
    ImageName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_image method usage example with argument unpacking

kwargs: DeleteImageRequestTypeDef = {  # (1)
    "ImageName": ...,
}

parent.delete_image(**kwargs)
```

1. See [:material-code-braces: DeleteImageRequestTypeDef](./type_defs.md#deleteimagerequesttypedef) 

### delete\_image\_version

Deletes a version of a SageMaker AI image.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_image_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_image_version.html)

```python
# delete_image_version method definition

await def delete_image_version(
    self,
    *,
    ImageName: str,
    Version: int = ...,
    Alias: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_image_version method usage example with argument unpacking

kwargs: DeleteImageVersionRequestTypeDef = {  # (1)
    "ImageName": ...,
}

parent.delete_image_version(**kwargs)
```

1. See [:material-code-braces: DeleteImageVersionRequestTypeDef](./type_defs.md#deleteimageversionrequesttypedef) 

### delete\_inference\_component

Deletes an inference component.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_inference_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_inference_component.html)

```python
# delete_inference_component method definition

await def delete_inference_component(
    self,
    *,
    InferenceComponentName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_inference_component method usage example with argument unpacking

kwargs: DeleteInferenceComponentInputTypeDef = {  # (1)
    "InferenceComponentName": ...,
}

parent.delete_inference_component(**kwargs)
```

1. See [:material-code-braces: DeleteInferenceComponentInputTypeDef](./type_defs.md#deleteinferencecomponentinputtypedef) 

### delete\_inference\_experiment

Deletes an inference experiment.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_inference_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_inference_experiment.html)

```python
# delete_inference_experiment method definition

await def delete_inference_experiment(
    self,
    *,
    Name: str,
) -> DeleteInferenceExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteInferenceExperimentResponseTypeDef](./type_defs.md#deleteinferenceexperimentresponsetypedef) 


```python
# delete_inference_experiment method usage example with argument unpacking

kwargs: DeleteInferenceExperimentRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_inference_experiment(**kwargs)
```

1. See [:material-code-braces: DeleteInferenceExperimentRequestTypeDef](./type_defs.md#deleteinferenceexperimentrequesttypedef) 

### delete\_mlflow\_tracking\_server

Deletes an MLflow Tracking Server.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_mlflow_tracking_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_mlflow_tracking_server.html)

```python
# delete_mlflow_tracking_server method definition

await def delete_mlflow_tracking_server(
    self,
    *,
    TrackingServerName: str,
) -> DeleteMlflowTrackingServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMlflowTrackingServerResponseTypeDef](./type_defs.md#deletemlflowtrackingserverresponsetypedef) 


```python
# delete_mlflow_tracking_server method usage example with argument unpacking

kwargs: DeleteMlflowTrackingServerRequestTypeDef = {  # (1)
    "TrackingServerName": ...,
}

parent.delete_mlflow_tracking_server(**kwargs)
```

1. See [:material-code-braces: DeleteMlflowTrackingServerRequestTypeDef](./type_defs.md#deletemlflowtrackingserverrequesttypedef) 

### delete\_model

Deletes a model.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_model.html)

```python
# delete_model method definition

await def delete_model(
    self,
    *,
    ModelName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_model method usage example with argument unpacking

kwargs: DeleteModelInputTypeDef = {  # (1)
    "ModelName": ...,
}

parent.delete_model(**kwargs)
```

1. See [:material-code-braces: DeleteModelInputTypeDef](./type_defs.md#deletemodelinputtypedef) 

### delete\_model\_bias\_job\_definition

Deletes an Amazon SageMaker AI model bias job definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_model_bias_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_model_bias_job_definition.html)

```python
# delete_model_bias_job_definition method definition

await def delete_model_bias_job_definition(
    self,
    *,
    JobDefinitionName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_model_bias_job_definition method usage example with argument unpacking

kwargs: DeleteModelBiasJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
}

parent.delete_model_bias_job_definition(**kwargs)
```

1. See [:material-code-braces: DeleteModelBiasJobDefinitionRequestTypeDef](./type_defs.md#deletemodelbiasjobdefinitionrequesttypedef) 

### delete\_model\_card

Deletes an Amazon SageMaker Model Card.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_model_card` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_model_card.html)

```python
# delete_model_card method definition

await def delete_model_card(
    self,
    *,
    ModelCardName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_model_card method usage example with argument unpacking

kwargs: DeleteModelCardRequestTypeDef = {  # (1)
    "ModelCardName": ...,
}

parent.delete_model_card(**kwargs)
```

1. See [:material-code-braces: DeleteModelCardRequestTypeDef](./type_defs.md#deletemodelcardrequesttypedef) 

### delete\_model\_explainability\_job\_definition

Deletes an Amazon SageMaker AI model explainability job definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_model_explainability_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_model_explainability_job_definition.html)

```python
# delete_model_explainability_job_definition method definition

await def delete_model_explainability_job_definition(
    self,
    *,
    JobDefinitionName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_model_explainability_job_definition method usage example with argument unpacking

kwargs: DeleteModelExplainabilityJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
}

parent.delete_model_explainability_job_definition(**kwargs)
```

1. See [:material-code-braces: DeleteModelExplainabilityJobDefinitionRequestTypeDef](./type_defs.md#deletemodelexplainabilityjobdefinitionrequesttypedef) 

### delete\_model\_package

Deletes a model package.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_model_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_model_package.html)

```python
# delete_model_package method definition

await def delete_model_package(
    self,
    *,
    ModelPackageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_model_package method usage example with argument unpacking

kwargs: DeleteModelPackageInputTypeDef = {  # (1)
    "ModelPackageName": ...,
}

parent.delete_model_package(**kwargs)
```

1. See [:material-code-braces: DeleteModelPackageInputTypeDef](./type_defs.md#deletemodelpackageinputtypedef) 

### delete\_model\_package\_group

Deletes the specified model group.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_model_package_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_model_package_group.html)

```python
# delete_model_package_group method definition

await def delete_model_package_group(
    self,
    *,
    ModelPackageGroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_model_package_group method usage example with argument unpacking

kwargs: DeleteModelPackageGroupInputTypeDef = {  # (1)
    "ModelPackageGroupName": ...,
}

parent.delete_model_package_group(**kwargs)
```

1. See [:material-code-braces: DeleteModelPackageGroupInputTypeDef](./type_defs.md#deletemodelpackagegroupinputtypedef) 

### delete\_model\_package\_group\_policy

Deletes a model group resource policy.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_model_package_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_model_package_group_policy.html)

```python
# delete_model_package_group_policy method definition

await def delete_model_package_group_policy(
    self,
    *,
    ModelPackageGroupName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_model_package_group_policy method usage example with argument unpacking

kwargs: DeleteModelPackageGroupPolicyInputTypeDef = {  # (1)
    "ModelPackageGroupName": ...,
}

parent.delete_model_package_group_policy(**kwargs)
```

1. See [:material-code-braces: DeleteModelPackageGroupPolicyInputTypeDef](./type_defs.md#deletemodelpackagegrouppolicyinputtypedef) 

### delete\_model\_quality\_job\_definition

Deletes the secified model quality monitoring job definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_model_quality_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_model_quality_job_definition.html)

```python
# delete_model_quality_job_definition method definition

await def delete_model_quality_job_definition(
    self,
    *,
    JobDefinitionName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_model_quality_job_definition method usage example with argument unpacking

kwargs: DeleteModelQualityJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
}

parent.delete_model_quality_job_definition(**kwargs)
```

1. See [:material-code-braces: DeleteModelQualityJobDefinitionRequestTypeDef](./type_defs.md#deletemodelqualityjobdefinitionrequesttypedef) 

### delete\_monitoring\_schedule

Deletes a monitoring schedule.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_monitoring_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_monitoring_schedule.html)

```python
# delete_monitoring_schedule method definition

await def delete_monitoring_schedule(
    self,
    *,
    MonitoringScheduleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_monitoring_schedule method usage example with argument unpacking

kwargs: DeleteMonitoringScheduleRequestTypeDef = {  # (1)
    "MonitoringScheduleName": ...,
}

parent.delete_monitoring_schedule(**kwargs)
```

1. See [:material-code-braces: DeleteMonitoringScheduleRequestTypeDef](./type_defs.md#deletemonitoringschedulerequesttypedef) 

### delete\_notebook\_instance

Deletes an SageMaker AI notebook instance.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_notebook_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_notebook_instance.html)

```python
# delete_notebook_instance method definition

await def delete_notebook_instance(
    self,
    *,
    NotebookInstanceName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_notebook_instance method usage example with argument unpacking

kwargs: DeleteNotebookInstanceInputTypeDef = {  # (1)
    "NotebookInstanceName": ...,
}

parent.delete_notebook_instance(**kwargs)
```

1. See [:material-code-braces: DeleteNotebookInstanceInputTypeDef](./type_defs.md#deletenotebookinstanceinputtypedef) 

### delete\_notebook\_instance\_lifecycle\_config

Deletes a notebook instance lifecycle configuration.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_notebook_instance_lifecycle_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_notebook_instance_lifecycle_config.html)

```python
# delete_notebook_instance_lifecycle_config method definition

await def delete_notebook_instance_lifecycle_config(
    self,
    *,
    NotebookInstanceLifecycleConfigName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_notebook_instance_lifecycle_config method usage example with argument unpacking

kwargs: DeleteNotebookInstanceLifecycleConfigInputTypeDef = {  # (1)
    "NotebookInstanceLifecycleConfigName": ...,
}

parent.delete_notebook_instance_lifecycle_config(**kwargs)
```

1. See [:material-code-braces: DeleteNotebookInstanceLifecycleConfigInputTypeDef](./type_defs.md#deletenotebookinstancelifecycleconfiginputtypedef) 

### delete\_optimization\_job

Deletes an optimization job.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_optimization_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_optimization_job.html)

```python
# delete_optimization_job method definition

await def delete_optimization_job(
    self,
    *,
    OptimizationJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_optimization_job method usage example with argument unpacking

kwargs: DeleteOptimizationJobRequestTypeDef = {  # (1)
    "OptimizationJobName": ...,
}

parent.delete_optimization_job(**kwargs)
```

1. See [:material-code-braces: DeleteOptimizationJobRequestTypeDef](./type_defs.md#deleteoptimizationjobrequesttypedef) 

### delete\_partner\_app

Deletes a SageMaker Partner AI App.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_partner_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_partner_app.html)

```python
# delete_partner_app method definition

await def delete_partner_app(
    self,
    *,
    Arn: str,
    ClientToken: str = ...,
) -> DeletePartnerAppResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePartnerAppResponseTypeDef](./type_defs.md#deletepartnerappresponsetypedef) 


```python
# delete_partner_app method usage example with argument unpacking

kwargs: DeletePartnerAppRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.delete_partner_app(**kwargs)
```

1. See [:material-code-braces: DeletePartnerAppRequestTypeDef](./type_defs.md#deletepartnerapprequesttypedef) 

### delete\_pipeline

Deletes a pipeline if there are no running instances of the pipeline.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_pipeline.html)

```python
# delete_pipeline method definition

await def delete_pipeline(
    self,
    *,
    PipelineName: str,
    ClientRequestToken: str,
) -> DeletePipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePipelineResponseTypeDef](./type_defs.md#deletepipelineresponsetypedef) 


```python
# delete_pipeline method usage example with argument unpacking

kwargs: DeletePipelineRequestTypeDef = {  # (1)
    "PipelineName": ...,
    "ClientRequestToken": ...,
}

parent.delete_pipeline(**kwargs)
```

1. See [:material-code-braces: DeletePipelineRequestTypeDef](./type_defs.md#deletepipelinerequesttypedef) 

### delete\_project

Delete the specified project.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_project.html)

```python
# delete_project method definition

await def delete_project(
    self,
    *,
    ProjectName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_project method usage example with argument unpacking

kwargs: DeleteProjectInputTypeDef = {  # (1)
    "ProjectName": ...,
}

parent.delete_project(**kwargs)
```

1. See [:material-code-braces: DeleteProjectInputTypeDef](./type_defs.md#deleteprojectinputtypedef) 

### delete\_space

Used to delete a space.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_space.html)

```python
# delete_space method definition

await def delete_space(
    self,
    *,
    DomainId: str,
    SpaceName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_space method usage example with argument unpacking

kwargs: DeleteSpaceRequestTypeDef = {  # (1)
    "DomainId": ...,
    "SpaceName": ...,
}

parent.delete_space(**kwargs)
```

1. See [:material-code-braces: DeleteSpaceRequestTypeDef](./type_defs.md#deletespacerequesttypedef) 

### delete\_studio\_lifecycle\_config

Deletes the Amazon SageMaker AI Studio Lifecycle Configuration.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_studio_lifecycle_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_studio_lifecycle_config.html)

```python
# delete_studio_lifecycle_config method definition

await def delete_studio_lifecycle_config(
    self,
    *,
    StudioLifecycleConfigName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_studio_lifecycle_config method usage example with argument unpacking

kwargs: DeleteStudioLifecycleConfigRequestTypeDef = {  # (1)
    "StudioLifecycleConfigName": ...,
}

parent.delete_studio_lifecycle_config(**kwargs)
```

1. See [:material-code-braces: DeleteStudioLifecycleConfigRequestTypeDef](./type_defs.md#deletestudiolifecycleconfigrequesttypedef) 

### delete\_tags

Deletes the specified tags from an SageMaker resource.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_tags.html)

```python
# delete_tags method definition

await def delete_tags(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# delete_tags method usage example with argument unpacking

kwargs: DeleteTagsInputTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.delete_tags(**kwargs)
```

1. See [:material-code-braces: DeleteTagsInputTypeDef](./type_defs.md#deletetagsinputtypedef) 

### delete\_trial

Deletes the specified trial.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_trial` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_trial.html)

```python
# delete_trial method definition

await def delete_trial(
    self,
    *,
    TrialName: str,
) -> DeleteTrialResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTrialResponseTypeDef](./type_defs.md#deletetrialresponsetypedef) 


```python
# delete_trial method usage example with argument unpacking

kwargs: DeleteTrialRequestTypeDef = {  # (1)
    "TrialName": ...,
}

parent.delete_trial(**kwargs)
```

1. See [:material-code-braces: DeleteTrialRequestTypeDef](./type_defs.md#deletetrialrequesttypedef) 

### delete\_trial\_component

Deletes the specified trial component.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_trial_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_trial_component.html)

```python
# delete_trial_component method definition

await def delete_trial_component(
    self,
    *,
    TrialComponentName: str,
) -> DeleteTrialComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTrialComponentResponseTypeDef](./type_defs.md#deletetrialcomponentresponsetypedef) 


```python
# delete_trial_component method usage example with argument unpacking

kwargs: DeleteTrialComponentRequestTypeDef = {  # (1)
    "TrialComponentName": ...,
}

parent.delete_trial_component(**kwargs)
```

1. See [:material-code-braces: DeleteTrialComponentRequestTypeDef](./type_defs.md#deletetrialcomponentrequesttypedef) 

### delete\_user\_profile

Deletes a user profile.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_user_profile.html)

```python
# delete_user_profile method definition

await def delete_user_profile(
    self,
    *,
    DomainId: str,
    UserProfileName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_user_profile method usage example with argument unpacking

kwargs: DeleteUserProfileRequestTypeDef = {  # (1)
    "DomainId": ...,
    "UserProfileName": ...,
}

parent.delete_user_profile(**kwargs)
```

1. See [:material-code-braces: DeleteUserProfileRequestTypeDef](./type_defs.md#deleteuserprofilerequesttypedef) 

### delete\_workforce

Use this operation to delete a workforce.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_workforce` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_workforce.html)

```python
# delete_workforce method definition

await def delete_workforce(
    self,
    *,
    WorkforceName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_workforce method usage example with argument unpacking

kwargs: DeleteWorkforceRequestTypeDef = {  # (1)
    "WorkforceName": ...,
}

parent.delete_workforce(**kwargs)
```

1. See [:material-code-braces: DeleteWorkforceRequestTypeDef](./type_defs.md#deleteworkforcerequesttypedef) 

### delete\_workteam

Deletes an existing work team.

Type annotations and code completion for `#!python session.create_client("sagemaker").delete_workteam` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/delete_workteam.html)

```python
# delete_workteam method definition

await def delete_workteam(
    self,
    *,
    WorkteamName: str,
) -> DeleteWorkteamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteWorkteamResponseTypeDef](./type_defs.md#deleteworkteamresponsetypedef) 


```python
# delete_workteam method usage example with argument unpacking

kwargs: DeleteWorkteamRequestTypeDef = {  # (1)
    "WorkteamName": ...,
}

parent.delete_workteam(**kwargs)
```

1. See [:material-code-braces: DeleteWorkteamRequestTypeDef](./type_defs.md#deleteworkteamrequesttypedef) 

### deregister\_devices

Deregisters the specified devices.

Type annotations and code completion for `#!python session.create_client("sagemaker").deregister_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/deregister_devices.html)

```python
# deregister_devices method definition

await def deregister_devices(
    self,
    *,
    DeviceFleetName: str,
    DeviceNames: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deregister_devices method usage example with argument unpacking

kwargs: DeregisterDevicesRequestTypeDef = {  # (1)
    "DeviceFleetName": ...,
    "DeviceNames": ...,
}

parent.deregister_devices(**kwargs)
```

1. See [:material-code-braces: DeregisterDevicesRequestTypeDef](./type_defs.md#deregisterdevicesrequesttypedef) 

### describe\_action

Describes an action.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_action.html)

```python
# describe_action method definition

await def describe_action(
    self,
    *,
    ActionName: str,
) -> DescribeActionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeActionResponseTypeDef](./type_defs.md#describeactionresponsetypedef) 


```python
# describe_action method usage example with argument unpacking

kwargs: DescribeActionRequestTypeDef = {  # (1)
    "ActionName": ...,
}

parent.describe_action(**kwargs)
```

1. See [:material-code-braces: DescribeActionRequestTypeDef](./type_defs.md#describeactionrequesttypedef) 

### describe\_algorithm

Returns a description of the specified algorithm that is in your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_algorithm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_algorithm.html)

```python
# describe_algorithm method definition

await def describe_algorithm(
    self,
    *,
    AlgorithmName: str,
) -> DescribeAlgorithmOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAlgorithmOutputTypeDef](./type_defs.md#describealgorithmoutputtypedef) 


```python
# describe_algorithm method usage example with argument unpacking

kwargs: DescribeAlgorithmInputTypeDef = {  # (1)
    "AlgorithmName": ...,
}

parent.describe_algorithm(**kwargs)
```

1. See [:material-code-braces: DescribeAlgorithmInputTypeDef](./type_defs.md#describealgorithminputtypedef) 

### describe\_app

Describes the app.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_app.html)

```python
# describe_app method definition

await def describe_app(
    self,
    *,
    DomainId: str,
    AppType: AppTypeType,  # (1)
    AppName: str,
    UserProfileName: str = ...,
    SpaceName: str = ...,
) -> DescribeAppResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
2. See [:material-code-braces: DescribeAppResponseTypeDef](./type_defs.md#describeappresponsetypedef) 


```python
# describe_app method usage example with argument unpacking

kwargs: DescribeAppRequestTypeDef = {  # (1)
    "DomainId": ...,
    "AppType": ...,
    "AppName": ...,
}

parent.describe_app(**kwargs)
```

1. See [:material-code-braces: DescribeAppRequestTypeDef](./type_defs.md#describeapprequesttypedef) 

### describe\_app\_image\_config

Describes an AppImageConfig.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_app_image_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_app_image_config.html)

```python
# describe_app_image_config method definition

await def describe_app_image_config(
    self,
    *,
    AppImageConfigName: str,
) -> DescribeAppImageConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAppImageConfigResponseTypeDef](./type_defs.md#describeappimageconfigresponsetypedef) 


```python
# describe_app_image_config method usage example with argument unpacking

kwargs: DescribeAppImageConfigRequestTypeDef = {  # (1)
    "AppImageConfigName": ...,
}

parent.describe_app_image_config(**kwargs)
```

1. See [:material-code-braces: DescribeAppImageConfigRequestTypeDef](./type_defs.md#describeappimageconfigrequesttypedef) 

### describe\_artifact

Describes an artifact.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_artifact.html)

```python
# describe_artifact method definition

await def describe_artifact(
    self,
    *,
    ArtifactArn: str,
) -> DescribeArtifactResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeArtifactResponseTypeDef](./type_defs.md#describeartifactresponsetypedef) 


```python
# describe_artifact method usage example with argument unpacking

kwargs: DescribeArtifactRequestTypeDef = {  # (1)
    "ArtifactArn": ...,
}

parent.describe_artifact(**kwargs)
```

1. See [:material-code-braces: DescribeArtifactRequestTypeDef](./type_defs.md#describeartifactrequesttypedef) 

### describe\_auto\_ml\_job

Returns information about an AutoML job created by calling <a
href="https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJob.html">CreateAutoMLJob</a>.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_auto_ml_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_auto_ml_job.html)

```python
# describe_auto_ml_job method definition

await def describe_auto_ml_job(
    self,
    *,
    AutoMLJobName: str,
) -> DescribeAutoMLJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAutoMLJobResponseTypeDef](./type_defs.md#describeautomljobresponsetypedef) 


```python
# describe_auto_ml_job method usage example with argument unpacking

kwargs: DescribeAutoMLJobRequestTypeDef = {  # (1)
    "AutoMLJobName": ...,
}

parent.describe_auto_ml_job(**kwargs)
```

1. See [:material-code-braces: DescribeAutoMLJobRequestTypeDef](./type_defs.md#describeautomljobrequesttypedef) 

### describe\_auto\_ml\_job\_v2

Returns information about an AutoML job created by calling <a
href="https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJobV2.html">CreateAutoMLJobV2</a>
or <a
href="https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateAutoMLJob.html">CreateAutoMLJob</a>.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_auto_ml_job_v2` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_auto_ml_job_v2.html)

```python
# describe_auto_ml_job_v2 method definition

await def describe_auto_ml_job_v2(
    self,
    *,
    AutoMLJobName: str,
) -> DescribeAutoMLJobV2ResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAutoMLJobV2ResponseTypeDef](./type_defs.md#describeautomljobv2responsetypedef) 


```python
# describe_auto_ml_job_v2 method usage example with argument unpacking

kwargs: DescribeAutoMLJobV2RequestTypeDef = {  # (1)
    "AutoMLJobName": ...,
}

parent.describe_auto_ml_job_v2(**kwargs)
```

1. See [:material-code-braces: DescribeAutoMLJobV2RequestTypeDef](./type_defs.md#describeautomljobv2requesttypedef) 

### describe\_cluster

Retrieves information of a SageMaker HyperPod cluster.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_cluster.html)

```python
# describe_cluster method definition

await def describe_cluster(
    self,
    *,
    ClusterName: str,
) -> DescribeClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClusterResponseTypeDef](./type_defs.md#describeclusterresponsetypedef) 


```python
# describe_cluster method usage example with argument unpacking

kwargs: DescribeClusterRequestTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.describe_cluster(**kwargs)
```

1. See [:material-code-braces: DescribeClusterRequestTypeDef](./type_defs.md#describeclusterrequesttypedef) 

### describe\_cluster\_node

Retrieves information of a node (also called a <i>instance</i> interchangeably)
of a SageMaker HyperPod cluster.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_cluster_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_cluster_node.html)

```python
# describe_cluster_node method definition

await def describe_cluster_node(
    self,
    *,
    ClusterName: str,
    NodeId: str,
) -> DescribeClusterNodeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClusterNodeResponseTypeDef](./type_defs.md#describeclusternoderesponsetypedef) 


```python
# describe_cluster_node method usage example with argument unpacking

kwargs: DescribeClusterNodeRequestTypeDef = {  # (1)
    "ClusterName": ...,
    "NodeId": ...,
}

parent.describe_cluster_node(**kwargs)
```

1. See [:material-code-braces: DescribeClusterNodeRequestTypeDef](./type_defs.md#describeclusternoderequesttypedef) 

### describe\_cluster\_scheduler\_config

Description of the cluster policy.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_cluster_scheduler_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_cluster_scheduler_config.html)

```python
# describe_cluster_scheduler_config method definition

await def describe_cluster_scheduler_config(
    self,
    *,
    ClusterSchedulerConfigId: str,
    ClusterSchedulerConfigVersion: int = ...,
) -> DescribeClusterSchedulerConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClusterSchedulerConfigResponseTypeDef](./type_defs.md#describeclusterschedulerconfigresponsetypedef) 


```python
# describe_cluster_scheduler_config method usage example with argument unpacking

kwargs: DescribeClusterSchedulerConfigRequestTypeDef = {  # (1)
    "ClusterSchedulerConfigId": ...,
}

parent.describe_cluster_scheduler_config(**kwargs)
```

1. See [:material-code-braces: DescribeClusterSchedulerConfigRequestTypeDef](./type_defs.md#describeclusterschedulerconfigrequesttypedef) 

### describe\_code\_repository

Gets details about the specified Git repository.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_code_repository` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_code_repository.html)

```python
# describe_code_repository method definition

await def describe_code_repository(
    self,
    *,
    CodeRepositoryName: str,
) -> DescribeCodeRepositoryOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCodeRepositoryOutputTypeDef](./type_defs.md#describecoderepositoryoutputtypedef) 


```python
# describe_code_repository method usage example with argument unpacking

kwargs: DescribeCodeRepositoryInputTypeDef = {  # (1)
    "CodeRepositoryName": ...,
}

parent.describe_code_repository(**kwargs)
```

1. See [:material-code-braces: DescribeCodeRepositoryInputTypeDef](./type_defs.md#describecoderepositoryinputtypedef) 

### describe\_compilation\_job

Returns information about a model compilation job.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_compilation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_compilation_job.html)

```python
# describe_compilation_job method definition

await def describe_compilation_job(
    self,
    *,
    CompilationJobName: str,
) -> DescribeCompilationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCompilationJobResponseTypeDef](./type_defs.md#describecompilationjobresponsetypedef) 


```python
# describe_compilation_job method usage example with argument unpacking

kwargs: DescribeCompilationJobRequestTypeDef = {  # (1)
    "CompilationJobName": ...,
}

parent.describe_compilation_job(**kwargs)
```

1. See [:material-code-braces: DescribeCompilationJobRequestTypeDef](./type_defs.md#describecompilationjobrequesttypedef) 

### describe\_compute\_quota

Description of the compute allocation definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_compute_quota` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_compute_quota.html)

```python
# describe_compute_quota method definition

await def describe_compute_quota(
    self,
    *,
    ComputeQuotaId: str,
    ComputeQuotaVersion: int = ...,
) -> DescribeComputeQuotaResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeComputeQuotaResponseTypeDef](./type_defs.md#describecomputequotaresponsetypedef) 


```python
# describe_compute_quota method usage example with argument unpacking

kwargs: DescribeComputeQuotaRequestTypeDef = {  # (1)
    "ComputeQuotaId": ...,
}

parent.describe_compute_quota(**kwargs)
```

1. See [:material-code-braces: DescribeComputeQuotaRequestTypeDef](./type_defs.md#describecomputequotarequesttypedef) 

### describe\_context

Describes a context.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_context` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_context.html)

```python
# describe_context method definition

await def describe_context(
    self,
    *,
    ContextName: str,
) -> DescribeContextResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeContextResponseTypeDef](./type_defs.md#describecontextresponsetypedef) 


```python
# describe_context method usage example with argument unpacking

kwargs: DescribeContextRequestTypeDef = {  # (1)
    "ContextName": ...,
}

parent.describe_context(**kwargs)
```

1. See [:material-code-braces: DescribeContextRequestTypeDef](./type_defs.md#describecontextrequesttypedef) 

### describe\_data\_quality\_job\_definition

Gets the details of a data quality monitoring job definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_data_quality_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_data_quality_job_definition.html)

```python
# describe_data_quality_job_definition method definition

await def describe_data_quality_job_definition(
    self,
    *,
    JobDefinitionName: str,
) -> DescribeDataQualityJobDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDataQualityJobDefinitionResponseTypeDef](./type_defs.md#describedataqualityjobdefinitionresponsetypedef) 


```python
# describe_data_quality_job_definition method usage example with argument unpacking

kwargs: DescribeDataQualityJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
}

parent.describe_data_quality_job_definition(**kwargs)
```

1. See [:material-code-braces: DescribeDataQualityJobDefinitionRequestTypeDef](./type_defs.md#describedataqualityjobdefinitionrequesttypedef) 

### describe\_device

Describes the device.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_device.html)

```python
# describe_device method definition

await def describe_device(
    self,
    *,
    DeviceName: str,
    DeviceFleetName: str,
    NextToken: str = ...,
) -> DescribeDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeviceResponseTypeDef](./type_defs.md#describedeviceresponsetypedef) 


```python
# describe_device method usage example with argument unpacking

kwargs: DescribeDeviceRequestTypeDef = {  # (1)
    "DeviceName": ...,
    "DeviceFleetName": ...,
}

parent.describe_device(**kwargs)
```

1. See [:material-code-braces: DescribeDeviceRequestTypeDef](./type_defs.md#describedevicerequesttypedef) 

### describe\_device\_fleet

A description of the fleet the device belongs to.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_device_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_device_fleet.html)

```python
# describe_device_fleet method definition

await def describe_device_fleet(
    self,
    *,
    DeviceFleetName: str,
) -> DescribeDeviceFleetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDeviceFleetResponseTypeDef](./type_defs.md#describedevicefleetresponsetypedef) 


```python
# describe_device_fleet method usage example with argument unpacking

kwargs: DescribeDeviceFleetRequestTypeDef = {  # (1)
    "DeviceFleetName": ...,
}

parent.describe_device_fleet(**kwargs)
```

1. See [:material-code-braces: DescribeDeviceFleetRequestTypeDef](./type_defs.md#describedevicefleetrequesttypedef) 

### describe\_domain

The description of the domain.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_domain.html)

```python
# describe_domain method definition

await def describe_domain(
    self,
    *,
    DomainId: str,
) -> DescribeDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainResponseTypeDef](./type_defs.md#describedomainresponsetypedef) 


```python
# describe_domain method usage example with argument unpacking

kwargs: DescribeDomainRequestTypeDef = {  # (1)
    "DomainId": ...,
}

parent.describe_domain(**kwargs)
```

1. See [:material-code-braces: DescribeDomainRequestTypeDef](./type_defs.md#describedomainrequesttypedef) 

### describe\_edge\_deployment\_plan

Describes an edge deployment plan with deployment status per stage.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_edge_deployment_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_edge_deployment_plan.html)

```python
# describe_edge_deployment_plan method definition

await def describe_edge_deployment_plan(
    self,
    *,
    EdgeDeploymentPlanName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeEdgeDeploymentPlanResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEdgeDeploymentPlanResponseTypeDef](./type_defs.md#describeedgedeploymentplanresponsetypedef) 


```python
# describe_edge_deployment_plan method usage example with argument unpacking

kwargs: DescribeEdgeDeploymentPlanRequestTypeDef = {  # (1)
    "EdgeDeploymentPlanName": ...,
}

parent.describe_edge_deployment_plan(**kwargs)
```

1. See [:material-code-braces: DescribeEdgeDeploymentPlanRequestTypeDef](./type_defs.md#describeedgedeploymentplanrequesttypedef) 

### describe\_edge\_packaging\_job

A description of edge packaging jobs.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_edge_packaging_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_edge_packaging_job.html)

```python
# describe_edge_packaging_job method definition

await def describe_edge_packaging_job(
    self,
    *,
    EdgePackagingJobName: str,
) -> DescribeEdgePackagingJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEdgePackagingJobResponseTypeDef](./type_defs.md#describeedgepackagingjobresponsetypedef) 


```python
# describe_edge_packaging_job method usage example with argument unpacking

kwargs: DescribeEdgePackagingJobRequestTypeDef = {  # (1)
    "EdgePackagingJobName": ...,
}

parent.describe_edge_packaging_job(**kwargs)
```

1. See [:material-code-braces: DescribeEdgePackagingJobRequestTypeDef](./type_defs.md#describeedgepackagingjobrequesttypedef) 

### describe\_endpoint

Returns the description of an endpoint.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_endpoint.html)

```python
# describe_endpoint method definition

await def describe_endpoint(
    self,
    *,
    EndpointName: str,
) -> DescribeEndpointOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEndpointOutputTypeDef](./type_defs.md#describeendpointoutputtypedef) 


```python
# describe_endpoint method usage example with argument unpacking

kwargs: DescribeEndpointInputTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.describe_endpoint(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointInputTypeDef](./type_defs.md#describeendpointinputtypedef) 

### describe\_endpoint\_config

Returns the description of an endpoint configuration created using the
<code>CreateEndpointConfig</code> API.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_endpoint_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_endpoint_config.html)

```python
# describe_endpoint_config method definition

await def describe_endpoint_config(
    self,
    *,
    EndpointConfigName: str,
) -> DescribeEndpointConfigOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEndpointConfigOutputTypeDef](./type_defs.md#describeendpointconfigoutputtypedef) 


```python
# describe_endpoint_config method usage example with argument unpacking

kwargs: DescribeEndpointConfigInputTypeDef = {  # (1)
    "EndpointConfigName": ...,
}

parent.describe_endpoint_config(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointConfigInputTypeDef](./type_defs.md#describeendpointconfiginputtypedef) 

### describe\_experiment

Provides a list of an experiment's properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_experiment.html)

```python
# describe_experiment method definition

await def describe_experiment(
    self,
    *,
    ExperimentName: str,
) -> DescribeExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeExperimentResponseTypeDef](./type_defs.md#describeexperimentresponsetypedef) 


```python
# describe_experiment method usage example with argument unpacking

kwargs: DescribeExperimentRequestTypeDef = {  # (1)
    "ExperimentName": ...,
}

parent.describe_experiment(**kwargs)
```

1. See [:material-code-braces: DescribeExperimentRequestTypeDef](./type_defs.md#describeexperimentrequesttypedef) 

### describe\_feature\_group

Use this operation to describe a <code>FeatureGroup</code>.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_feature_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_feature_group.html)

```python
# describe_feature_group method definition

await def describe_feature_group(
    self,
    *,
    FeatureGroupName: str,
    NextToken: str = ...,
) -> DescribeFeatureGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFeatureGroupResponseTypeDef](./type_defs.md#describefeaturegroupresponsetypedef) 


```python
# describe_feature_group method usage example with argument unpacking

kwargs: DescribeFeatureGroupRequestTypeDef = {  # (1)
    "FeatureGroupName": ...,
}

parent.describe_feature_group(**kwargs)
```

1. See [:material-code-braces: DescribeFeatureGroupRequestTypeDef](./type_defs.md#describefeaturegrouprequesttypedef) 

### describe\_feature\_metadata

Shows the metadata for a feature within a feature group.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_feature_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_feature_metadata.html)

```python
# describe_feature_metadata method definition

await def describe_feature_metadata(
    self,
    *,
    FeatureGroupName: str,
    FeatureName: str,
) -> DescribeFeatureMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFeatureMetadataResponseTypeDef](./type_defs.md#describefeaturemetadataresponsetypedef) 


```python
# describe_feature_metadata method usage example with argument unpacking

kwargs: DescribeFeatureMetadataRequestTypeDef = {  # (1)
    "FeatureGroupName": ...,
    "FeatureName": ...,
}

parent.describe_feature_metadata(**kwargs)
```

1. See [:material-code-braces: DescribeFeatureMetadataRequestTypeDef](./type_defs.md#describefeaturemetadatarequesttypedef) 

### describe\_flow\_definition

Returns information about the specified flow definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_flow_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_flow_definition.html)

```python
# describe_flow_definition method definition

await def describe_flow_definition(
    self,
    *,
    FlowDefinitionName: str,
) -> DescribeFlowDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFlowDefinitionResponseTypeDef](./type_defs.md#describeflowdefinitionresponsetypedef) 


```python
# describe_flow_definition method usage example with argument unpacking

kwargs: DescribeFlowDefinitionRequestTypeDef = {  # (1)
    "FlowDefinitionName": ...,
}

parent.describe_flow_definition(**kwargs)
```

1. See [:material-code-braces: DescribeFlowDefinitionRequestTypeDef](./type_defs.md#describeflowdefinitionrequesttypedef) 

### describe\_hub

Describes a hub.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_hub` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_hub.html)

```python
# describe_hub method definition

await def describe_hub(
    self,
    *,
    HubName: str,
) -> DescribeHubResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHubResponseTypeDef](./type_defs.md#describehubresponsetypedef) 


```python
# describe_hub method usage example with argument unpacking

kwargs: DescribeHubRequestTypeDef = {  # (1)
    "HubName": ...,
}

parent.describe_hub(**kwargs)
```

1. See [:material-code-braces: DescribeHubRequestTypeDef](./type_defs.md#describehubrequesttypedef) 

### describe\_hub\_content

Describe the content of a hub.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_hub_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_hub_content.html)

```python
# describe_hub_content method definition

await def describe_hub_content(
    self,
    *,
    HubName: str,
    HubContentType: HubContentTypeType,  # (1)
    HubContentName: str,
    HubContentVersion: str = ...,
) -> DescribeHubContentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-braces: DescribeHubContentResponseTypeDef](./type_defs.md#describehubcontentresponsetypedef) 


```python
# describe_hub_content method usage example with argument unpacking

kwargs: DescribeHubContentRequestTypeDef = {  # (1)
    "HubName": ...,
    "HubContentType": ...,
    "HubContentName": ...,
}

parent.describe_hub_content(**kwargs)
```

1. See [:material-code-braces: DescribeHubContentRequestTypeDef](./type_defs.md#describehubcontentrequesttypedef) 

### describe\_human\_task\_ui

Returns information about the requested human task user interface (worker task
template).

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_human_task_ui` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_human_task_ui.html)

```python
# describe_human_task_ui method definition

await def describe_human_task_ui(
    self,
    *,
    HumanTaskUiName: str,
) -> DescribeHumanTaskUiResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHumanTaskUiResponseTypeDef](./type_defs.md#describehumantaskuiresponsetypedef) 


```python
# describe_human_task_ui method usage example with argument unpacking

kwargs: DescribeHumanTaskUiRequestTypeDef = {  # (1)
    "HumanTaskUiName": ...,
}

parent.describe_human_task_ui(**kwargs)
```

1. See [:material-code-braces: DescribeHumanTaskUiRequestTypeDef](./type_defs.md#describehumantaskuirequesttypedef) 

### describe\_hyper\_parameter\_tuning\_job

Returns a description of a hyperparameter tuning job, depending on the fields
selected.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_hyper_parameter_tuning_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_hyper_parameter_tuning_job.html)

```python
# describe_hyper_parameter_tuning_job method definition

await def describe_hyper_parameter_tuning_job(
    self,
    *,
    HyperParameterTuningJobName: str,
) -> DescribeHyperParameterTuningJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHyperParameterTuningJobResponseTypeDef](./type_defs.md#describehyperparametertuningjobresponsetypedef) 


```python
# describe_hyper_parameter_tuning_job method usage example with argument unpacking

kwargs: DescribeHyperParameterTuningJobRequestTypeDef = {  # (1)
    "HyperParameterTuningJobName": ...,
}

parent.describe_hyper_parameter_tuning_job(**kwargs)
```

1. See [:material-code-braces: DescribeHyperParameterTuningJobRequestTypeDef](./type_defs.md#describehyperparametertuningjobrequesttypedef) 

### describe\_image

Describes a SageMaker AI image.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_image.html)

```python
# describe_image method definition

await def describe_image(
    self,
    *,
    ImageName: str,
) -> DescribeImageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeImageResponseTypeDef](./type_defs.md#describeimageresponsetypedef) 


```python
# describe_image method usage example with argument unpacking

kwargs: DescribeImageRequestTypeDef = {  # (1)
    "ImageName": ...,
}

parent.describe_image(**kwargs)
```

1. See [:material-code-braces: DescribeImageRequestTypeDef](./type_defs.md#describeimagerequesttypedef) 

### describe\_image\_version

Describes a version of a SageMaker AI image.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_image_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_image_version.html)

```python
# describe_image_version method definition

await def describe_image_version(
    self,
    *,
    ImageName: str,
    Version: int = ...,
    Alias: str = ...,
) -> DescribeImageVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeImageVersionResponseTypeDef](./type_defs.md#describeimageversionresponsetypedef) 


```python
# describe_image_version method usage example with argument unpacking

kwargs: DescribeImageVersionRequestTypeDef = {  # (1)
    "ImageName": ...,
}

parent.describe_image_version(**kwargs)
```

1. See [:material-code-braces: DescribeImageVersionRequestTypeDef](./type_defs.md#describeimageversionrequesttypedef) 

### describe\_inference\_component

Returns information about an inference component.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_inference_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_inference_component.html)

```python
# describe_inference_component method definition

await def describe_inference_component(
    self,
    *,
    InferenceComponentName: str,
) -> DescribeInferenceComponentOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInferenceComponentOutputTypeDef](./type_defs.md#describeinferencecomponentoutputtypedef) 


```python
# describe_inference_component method usage example with argument unpacking

kwargs: DescribeInferenceComponentInputTypeDef = {  # (1)
    "InferenceComponentName": ...,
}

parent.describe_inference_component(**kwargs)
```

1. See [:material-code-braces: DescribeInferenceComponentInputTypeDef](./type_defs.md#describeinferencecomponentinputtypedef) 

### describe\_inference\_experiment

Returns details about an inference experiment.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_inference_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_inference_experiment.html)

```python
# describe_inference_experiment method definition

await def describe_inference_experiment(
    self,
    *,
    Name: str,
) -> DescribeInferenceExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInferenceExperimentResponseTypeDef](./type_defs.md#describeinferenceexperimentresponsetypedef) 


```python
# describe_inference_experiment method usage example with argument unpacking

kwargs: DescribeInferenceExperimentRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_inference_experiment(**kwargs)
```

1. See [:material-code-braces: DescribeInferenceExperimentRequestTypeDef](./type_defs.md#describeinferenceexperimentrequesttypedef) 

### describe\_inference\_recommendations\_job

Provides the results of the Inference Recommender job.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_inference_recommendations_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_inference_recommendations_job.html)

```python
# describe_inference_recommendations_job method definition

await def describe_inference_recommendations_job(
    self,
    *,
    JobName: str,
) -> DescribeInferenceRecommendationsJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInferenceRecommendationsJobResponseTypeDef](./type_defs.md#describeinferencerecommendationsjobresponsetypedef) 


```python
# describe_inference_recommendations_job method usage example with argument unpacking

kwargs: DescribeInferenceRecommendationsJobRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.describe_inference_recommendations_job(**kwargs)
```

1. See [:material-code-braces: DescribeInferenceRecommendationsJobRequestTypeDef](./type_defs.md#describeinferencerecommendationsjobrequesttypedef) 

### describe\_labeling\_job

Gets information about a labeling job.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_labeling_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_labeling_job.html)

```python
# describe_labeling_job method definition

await def describe_labeling_job(
    self,
    *,
    LabelingJobName: str,
) -> DescribeLabelingJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLabelingJobResponseTypeDef](./type_defs.md#describelabelingjobresponsetypedef) 


```python
# describe_labeling_job method usage example with argument unpacking

kwargs: DescribeLabelingJobRequestTypeDef = {  # (1)
    "LabelingJobName": ...,
}

parent.describe_labeling_job(**kwargs)
```

1. See [:material-code-braces: DescribeLabelingJobRequestTypeDef](./type_defs.md#describelabelingjobrequesttypedef) 

### describe\_lineage\_group

Provides a list of properties for the requested lineage group.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_lineage_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_lineage_group.html)

```python
# describe_lineage_group method definition

await def describe_lineage_group(
    self,
    *,
    LineageGroupName: str,
) -> DescribeLineageGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLineageGroupResponseTypeDef](./type_defs.md#describelineagegroupresponsetypedef) 


```python
# describe_lineage_group method usage example with argument unpacking

kwargs: DescribeLineageGroupRequestTypeDef = {  # (1)
    "LineageGroupName": ...,
}

parent.describe_lineage_group(**kwargs)
```

1. See [:material-code-braces: DescribeLineageGroupRequestTypeDef](./type_defs.md#describelineagegrouprequesttypedef) 

### describe\_mlflow\_tracking\_server

Returns information about an MLflow Tracking Server.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_mlflow_tracking_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_mlflow_tracking_server.html)

```python
# describe_mlflow_tracking_server method definition

await def describe_mlflow_tracking_server(
    self,
    *,
    TrackingServerName: str,
) -> DescribeMlflowTrackingServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMlflowTrackingServerResponseTypeDef](./type_defs.md#describemlflowtrackingserverresponsetypedef) 


```python
# describe_mlflow_tracking_server method usage example with argument unpacking

kwargs: DescribeMlflowTrackingServerRequestTypeDef = {  # (1)
    "TrackingServerName": ...,
}

parent.describe_mlflow_tracking_server(**kwargs)
```

1. See [:material-code-braces: DescribeMlflowTrackingServerRequestTypeDef](./type_defs.md#describemlflowtrackingserverrequesttypedef) 

### describe\_model

Describes a model that you created using the <code>CreateModel</code> API.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_model.html)

```python
# describe_model method definition

await def describe_model(
    self,
    *,
    ModelName: str,
) -> DescribeModelOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelOutputTypeDef](./type_defs.md#describemodeloutputtypedef) 


```python
# describe_model method usage example with argument unpacking

kwargs: DescribeModelInputTypeDef = {  # (1)
    "ModelName": ...,
}

parent.describe_model(**kwargs)
```

1. See [:material-code-braces: DescribeModelInputTypeDef](./type_defs.md#describemodelinputtypedef) 

### describe\_model\_bias\_job\_definition

Returns a description of a model bias job definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_model_bias_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_model_bias_job_definition.html)

```python
# describe_model_bias_job_definition method definition

await def describe_model_bias_job_definition(
    self,
    *,
    JobDefinitionName: str,
) -> DescribeModelBiasJobDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelBiasJobDefinitionResponseTypeDef](./type_defs.md#describemodelbiasjobdefinitionresponsetypedef) 


```python
# describe_model_bias_job_definition method usage example with argument unpacking

kwargs: DescribeModelBiasJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
}

parent.describe_model_bias_job_definition(**kwargs)
```

1. See [:material-code-braces: DescribeModelBiasJobDefinitionRequestTypeDef](./type_defs.md#describemodelbiasjobdefinitionrequesttypedef) 

### describe\_model\_card

Describes the content, creation time, and security configuration of an Amazon
SageMaker Model Card.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_model_card` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_model_card.html)

```python
# describe_model_card method definition

await def describe_model_card(
    self,
    *,
    ModelCardName: str,
    ModelCardVersion: int = ...,
) -> DescribeModelCardResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelCardResponseTypeDef](./type_defs.md#describemodelcardresponsetypedef) 


```python
# describe_model_card method usage example with argument unpacking

kwargs: DescribeModelCardRequestTypeDef = {  # (1)
    "ModelCardName": ...,
}

parent.describe_model_card(**kwargs)
```

1. See [:material-code-braces: DescribeModelCardRequestTypeDef](./type_defs.md#describemodelcardrequesttypedef) 

### describe\_model\_card\_export\_job

Describes an Amazon SageMaker Model Card export job.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_model_card_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_model_card_export_job.html)

```python
# describe_model_card_export_job method definition

await def describe_model_card_export_job(
    self,
    *,
    ModelCardExportJobArn: str,
) -> DescribeModelCardExportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelCardExportJobResponseTypeDef](./type_defs.md#describemodelcardexportjobresponsetypedef) 


```python
# describe_model_card_export_job method usage example with argument unpacking

kwargs: DescribeModelCardExportJobRequestTypeDef = {  # (1)
    "ModelCardExportJobArn": ...,
}

parent.describe_model_card_export_job(**kwargs)
```

1. See [:material-code-braces: DescribeModelCardExportJobRequestTypeDef](./type_defs.md#describemodelcardexportjobrequesttypedef) 

### describe\_model\_explainability\_job\_definition

Returns a description of a model explainability job definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_model_explainability_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_model_explainability_job_definition.html)

```python
# describe_model_explainability_job_definition method definition

await def describe_model_explainability_job_definition(
    self,
    *,
    JobDefinitionName: str,
) -> DescribeModelExplainabilityJobDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelExplainabilityJobDefinitionResponseTypeDef](./type_defs.md#describemodelexplainabilityjobdefinitionresponsetypedef) 


```python
# describe_model_explainability_job_definition method usage example with argument unpacking

kwargs: DescribeModelExplainabilityJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
}

parent.describe_model_explainability_job_definition(**kwargs)
```

1. See [:material-code-braces: DescribeModelExplainabilityJobDefinitionRequestTypeDef](./type_defs.md#describemodelexplainabilityjobdefinitionrequesttypedef) 

### describe\_model\_package

Returns a description of the specified model package, which is used to create
SageMaker models or list them on Amazon Web Services Marketplace.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_model_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_model_package.html)

```python
# describe_model_package method definition

await def describe_model_package(
    self,
    *,
    ModelPackageName: str,
) -> DescribeModelPackageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelPackageOutputTypeDef](./type_defs.md#describemodelpackageoutputtypedef) 


```python
# describe_model_package method usage example with argument unpacking

kwargs: DescribeModelPackageInputTypeDef = {  # (1)
    "ModelPackageName": ...,
}

parent.describe_model_package(**kwargs)
```

1. See [:material-code-braces: DescribeModelPackageInputTypeDef](./type_defs.md#describemodelpackageinputtypedef) 

### describe\_model\_package\_group

Gets a description for the specified model group.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_model_package_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_model_package_group.html)

```python
# describe_model_package_group method definition

await def describe_model_package_group(
    self,
    *,
    ModelPackageGroupName: str,
) -> DescribeModelPackageGroupOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelPackageGroupOutputTypeDef](./type_defs.md#describemodelpackagegroupoutputtypedef) 


```python
# describe_model_package_group method usage example with argument unpacking

kwargs: DescribeModelPackageGroupInputTypeDef = {  # (1)
    "ModelPackageGroupName": ...,
}

parent.describe_model_package_group(**kwargs)
```

1. See [:material-code-braces: DescribeModelPackageGroupInputTypeDef](./type_defs.md#describemodelpackagegroupinputtypedef) 

### describe\_model\_quality\_job\_definition

Returns a description of a model quality job definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_model_quality_job_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_model_quality_job_definition.html)

```python
# describe_model_quality_job_definition method definition

await def describe_model_quality_job_definition(
    self,
    *,
    JobDefinitionName: str,
) -> DescribeModelQualityJobDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeModelQualityJobDefinitionResponseTypeDef](./type_defs.md#describemodelqualityjobdefinitionresponsetypedef) 


```python
# describe_model_quality_job_definition method usage example with argument unpacking

kwargs: DescribeModelQualityJobDefinitionRequestTypeDef = {  # (1)
    "JobDefinitionName": ...,
}

parent.describe_model_quality_job_definition(**kwargs)
```

1. See [:material-code-braces: DescribeModelQualityJobDefinitionRequestTypeDef](./type_defs.md#describemodelqualityjobdefinitionrequesttypedef) 

### describe\_monitoring\_schedule

Describes the schedule for a monitoring job.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_monitoring_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_monitoring_schedule.html)

```python
# describe_monitoring_schedule method definition

await def describe_monitoring_schedule(
    self,
    *,
    MonitoringScheduleName: str,
) -> DescribeMonitoringScheduleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMonitoringScheduleResponseTypeDef](./type_defs.md#describemonitoringscheduleresponsetypedef) 


```python
# describe_monitoring_schedule method usage example with argument unpacking

kwargs: DescribeMonitoringScheduleRequestTypeDef = {  # (1)
    "MonitoringScheduleName": ...,
}

parent.describe_monitoring_schedule(**kwargs)
```

1. See [:material-code-braces: DescribeMonitoringScheduleRequestTypeDef](./type_defs.md#describemonitoringschedulerequesttypedef) 

### describe\_notebook\_instance

Returns information about a notebook instance.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_notebook_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_notebook_instance.html)

```python
# describe_notebook_instance method definition

await def describe_notebook_instance(
    self,
    *,
    NotebookInstanceName: str,
) -> DescribeNotebookInstanceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeNotebookInstanceOutputTypeDef](./type_defs.md#describenotebookinstanceoutputtypedef) 


```python
# describe_notebook_instance method usage example with argument unpacking

kwargs: DescribeNotebookInstanceInputTypeDef = {  # (1)
    "NotebookInstanceName": ...,
}

parent.describe_notebook_instance(**kwargs)
```

1. See [:material-code-braces: DescribeNotebookInstanceInputTypeDef](./type_defs.md#describenotebookinstanceinputtypedef) 

### describe\_notebook\_instance\_lifecycle\_config

Returns a description of a notebook instance lifecycle configuration.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_notebook_instance_lifecycle_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_notebook_instance_lifecycle_config.html)

```python
# describe_notebook_instance_lifecycle_config method definition

await def describe_notebook_instance_lifecycle_config(
    self,
    *,
    NotebookInstanceLifecycleConfigName: str,
) -> DescribeNotebookInstanceLifecycleConfigOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeNotebookInstanceLifecycleConfigOutputTypeDef](./type_defs.md#describenotebookinstancelifecycleconfigoutputtypedef) 


```python
# describe_notebook_instance_lifecycle_config method usage example with argument unpacking

kwargs: DescribeNotebookInstanceLifecycleConfigInputTypeDef = {  # (1)
    "NotebookInstanceLifecycleConfigName": ...,
}

parent.describe_notebook_instance_lifecycle_config(**kwargs)
```

1. See [:material-code-braces: DescribeNotebookInstanceLifecycleConfigInputTypeDef](./type_defs.md#describenotebookinstancelifecycleconfiginputtypedef) 

### describe\_optimization\_job

Provides the properties of the specified optimization job.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_optimization_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_optimization_job.html)

```python
# describe_optimization_job method definition

await def describe_optimization_job(
    self,
    *,
    OptimizationJobName: str,
) -> DescribeOptimizationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOptimizationJobResponseTypeDef](./type_defs.md#describeoptimizationjobresponsetypedef) 


```python
# describe_optimization_job method usage example with argument unpacking

kwargs: DescribeOptimizationJobRequestTypeDef = {  # (1)
    "OptimizationJobName": ...,
}

parent.describe_optimization_job(**kwargs)
```

1. See [:material-code-braces: DescribeOptimizationJobRequestTypeDef](./type_defs.md#describeoptimizationjobrequesttypedef) 

### describe\_partner\_app

Gets information about a SageMaker Partner AI App.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_partner_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_partner_app.html)

```python
# describe_partner_app method definition

await def describe_partner_app(
    self,
    *,
    Arn: str,
) -> DescribePartnerAppResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePartnerAppResponseTypeDef](./type_defs.md#describepartnerappresponsetypedef) 


```python
# describe_partner_app method usage example with argument unpacking

kwargs: DescribePartnerAppRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.describe_partner_app(**kwargs)
```

1. See [:material-code-braces: DescribePartnerAppRequestTypeDef](./type_defs.md#describepartnerapprequesttypedef) 

### describe\_pipeline

Describes the details of a pipeline.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_pipeline.html)

```python
# describe_pipeline method definition

await def describe_pipeline(
    self,
    *,
    PipelineName: str,
) -> DescribePipelineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePipelineResponseTypeDef](./type_defs.md#describepipelineresponsetypedef) 


```python
# describe_pipeline method usage example with argument unpacking

kwargs: DescribePipelineRequestTypeDef = {  # (1)
    "PipelineName": ...,
}

parent.describe_pipeline(**kwargs)
```

1. See [:material-code-braces: DescribePipelineRequestTypeDef](./type_defs.md#describepipelinerequesttypedef) 

### describe\_pipeline\_definition\_for\_execution

Describes the details of an execution's pipeline definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_pipeline_definition_for_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_pipeline_definition_for_execution.html)

```python
# describe_pipeline_definition_for_execution method definition

await def describe_pipeline_definition_for_execution(
    self,
    *,
    PipelineExecutionArn: str,
) -> DescribePipelineDefinitionForExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePipelineDefinitionForExecutionResponseTypeDef](./type_defs.md#describepipelinedefinitionforexecutionresponsetypedef) 


```python
# describe_pipeline_definition_for_execution method usage example with argument unpacking

kwargs: DescribePipelineDefinitionForExecutionRequestTypeDef = {  # (1)
    "PipelineExecutionArn": ...,
}

parent.describe_pipeline_definition_for_execution(**kwargs)
```

1. See [:material-code-braces: DescribePipelineDefinitionForExecutionRequestTypeDef](./type_defs.md#describepipelinedefinitionforexecutionrequesttypedef) 

### describe\_pipeline\_execution

Describes the details of a pipeline execution.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_pipeline_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_pipeline_execution.html)

```python
# describe_pipeline_execution method definition

await def describe_pipeline_execution(
    self,
    *,
    PipelineExecutionArn: str,
) -> DescribePipelineExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePipelineExecutionResponseTypeDef](./type_defs.md#describepipelineexecutionresponsetypedef) 


```python
# describe_pipeline_execution method usage example with argument unpacking

kwargs: DescribePipelineExecutionRequestTypeDef = {  # (1)
    "PipelineExecutionArn": ...,
}

parent.describe_pipeline_execution(**kwargs)
```

1. See [:material-code-braces: DescribePipelineExecutionRequestTypeDef](./type_defs.md#describepipelineexecutionrequesttypedef) 

### describe\_processing\_job

Returns a description of a processing job.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_processing_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_processing_job.html)

```python
# describe_processing_job method definition

await def describe_processing_job(
    self,
    *,
    ProcessingJobName: str,
) -> DescribeProcessingJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProcessingJobResponseTypeDef](./type_defs.md#describeprocessingjobresponsetypedef) 


```python
# describe_processing_job method usage example with argument unpacking

kwargs: DescribeProcessingJobRequestTypeDef = {  # (1)
    "ProcessingJobName": ...,
}

parent.describe_processing_job(**kwargs)
```

1. See [:material-code-braces: DescribeProcessingJobRequestTypeDef](./type_defs.md#describeprocessingjobrequesttypedef) 

### describe\_project

Describes the details of a project.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_project.html)

```python
# describe_project method definition

await def describe_project(
    self,
    *,
    ProjectName: str,
) -> DescribeProjectOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeProjectOutputTypeDef](./type_defs.md#describeprojectoutputtypedef) 


```python
# describe_project method usage example with argument unpacking

kwargs: DescribeProjectInputTypeDef = {  # (1)
    "ProjectName": ...,
}

parent.describe_project(**kwargs)
```

1. See [:material-code-braces: DescribeProjectInputTypeDef](./type_defs.md#describeprojectinputtypedef) 

### describe\_space

Describes the space.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_space.html)

```python
# describe_space method definition

await def describe_space(
    self,
    *,
    DomainId: str,
    SpaceName: str,
) -> DescribeSpaceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSpaceResponseTypeDef](./type_defs.md#describespaceresponsetypedef) 


```python
# describe_space method usage example with argument unpacking

kwargs: DescribeSpaceRequestTypeDef = {  # (1)
    "DomainId": ...,
    "SpaceName": ...,
}

parent.describe_space(**kwargs)
```

1. See [:material-code-braces: DescribeSpaceRequestTypeDef](./type_defs.md#describespacerequesttypedef) 

### describe\_studio\_lifecycle\_config

Describes the Amazon SageMaker AI Studio Lifecycle Configuration.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_studio_lifecycle_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_studio_lifecycle_config.html)

```python
# describe_studio_lifecycle_config method definition

await def describe_studio_lifecycle_config(
    self,
    *,
    StudioLifecycleConfigName: str,
) -> DescribeStudioLifecycleConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeStudioLifecycleConfigResponseTypeDef](./type_defs.md#describestudiolifecycleconfigresponsetypedef) 


```python
# describe_studio_lifecycle_config method usage example with argument unpacking

kwargs: DescribeStudioLifecycleConfigRequestTypeDef = {  # (1)
    "StudioLifecycleConfigName": ...,
}

parent.describe_studio_lifecycle_config(**kwargs)
```

1. See [:material-code-braces: DescribeStudioLifecycleConfigRequestTypeDef](./type_defs.md#describestudiolifecycleconfigrequesttypedef) 

### describe\_subscribed\_workteam

Gets information about a work team provided by a vendor.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_subscribed_workteam` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_subscribed_workteam.html)

```python
# describe_subscribed_workteam method definition

await def describe_subscribed_workteam(
    self,
    *,
    WorkteamArn: str,
) -> DescribeSubscribedWorkteamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSubscribedWorkteamResponseTypeDef](./type_defs.md#describesubscribedworkteamresponsetypedef) 


```python
# describe_subscribed_workteam method usage example with argument unpacking

kwargs: DescribeSubscribedWorkteamRequestTypeDef = {  # (1)
    "WorkteamArn": ...,
}

parent.describe_subscribed_workteam(**kwargs)
```

1. See [:material-code-braces: DescribeSubscribedWorkteamRequestTypeDef](./type_defs.md#describesubscribedworkteamrequesttypedef) 

### describe\_training\_job

Returns information about a training job.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_training_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_training_job.html)

```python
# describe_training_job method definition

await def describe_training_job(
    self,
    *,
    TrainingJobName: str,
) -> DescribeTrainingJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrainingJobResponseTypeDef](./type_defs.md#describetrainingjobresponsetypedef) 


```python
# describe_training_job method usage example with argument unpacking

kwargs: DescribeTrainingJobRequestTypeDef = {  # (1)
    "TrainingJobName": ...,
}

parent.describe_training_job(**kwargs)
```

1. See [:material-code-braces: DescribeTrainingJobRequestTypeDef](./type_defs.md#describetrainingjobrequesttypedef) 

### describe\_training\_plan

Retrieves detailed information about a specific training plan.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_training_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_training_plan.html)

```python
# describe_training_plan method definition

await def describe_training_plan(
    self,
    *,
    TrainingPlanName: str,
) -> DescribeTrainingPlanResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrainingPlanResponseTypeDef](./type_defs.md#describetrainingplanresponsetypedef) 


```python
# describe_training_plan method usage example with argument unpacking

kwargs: DescribeTrainingPlanRequestTypeDef = {  # (1)
    "TrainingPlanName": ...,
}

parent.describe_training_plan(**kwargs)
```

1. See [:material-code-braces: DescribeTrainingPlanRequestTypeDef](./type_defs.md#describetrainingplanrequesttypedef) 

### describe\_transform\_job

Returns information about a transform job.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_transform_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_transform_job.html)

```python
# describe_transform_job method definition

await def describe_transform_job(
    self,
    *,
    TransformJobName: str,
) -> DescribeTransformJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTransformJobResponseTypeDef](./type_defs.md#describetransformjobresponsetypedef) 


```python
# describe_transform_job method usage example with argument unpacking

kwargs: DescribeTransformJobRequestTypeDef = {  # (1)
    "TransformJobName": ...,
}

parent.describe_transform_job(**kwargs)
```

1. See [:material-code-braces: DescribeTransformJobRequestTypeDef](./type_defs.md#describetransformjobrequesttypedef) 

### describe\_trial

Provides a list of a trial's properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_trial` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_trial.html)

```python
# describe_trial method definition

await def describe_trial(
    self,
    *,
    TrialName: str,
) -> DescribeTrialResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrialResponseTypeDef](./type_defs.md#describetrialresponsetypedef) 


```python
# describe_trial method usage example with argument unpacking

kwargs: DescribeTrialRequestTypeDef = {  # (1)
    "TrialName": ...,
}

parent.describe_trial(**kwargs)
```

1. See [:material-code-braces: DescribeTrialRequestTypeDef](./type_defs.md#describetrialrequesttypedef) 

### describe\_trial\_component

Provides a list of a trials component's properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_trial_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_trial_component.html)

```python
# describe_trial_component method definition

await def describe_trial_component(
    self,
    *,
    TrialComponentName: str,
) -> DescribeTrialComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrialComponentResponseTypeDef](./type_defs.md#describetrialcomponentresponsetypedef) 


```python
# describe_trial_component method usage example with argument unpacking

kwargs: DescribeTrialComponentRequestTypeDef = {  # (1)
    "TrialComponentName": ...,
}

parent.describe_trial_component(**kwargs)
```

1. See [:material-code-braces: DescribeTrialComponentRequestTypeDef](./type_defs.md#describetrialcomponentrequesttypedef) 

### describe\_user\_profile

Describes a user profile.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_user_profile.html)

```python
# describe_user_profile method definition

await def describe_user_profile(
    self,
    *,
    DomainId: str,
    UserProfileName: str,
) -> DescribeUserProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeUserProfileResponseTypeDef](./type_defs.md#describeuserprofileresponsetypedef) 


```python
# describe_user_profile method usage example with argument unpacking

kwargs: DescribeUserProfileRequestTypeDef = {  # (1)
    "DomainId": ...,
    "UserProfileName": ...,
}

parent.describe_user_profile(**kwargs)
```

1. See [:material-code-braces: DescribeUserProfileRequestTypeDef](./type_defs.md#describeuserprofilerequesttypedef) 

### describe\_workforce

Lists private workforce information, including workforce name, Amazon Resource
Name (ARN), and, if applicable, allowed IP address ranges (<a
href="https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html">CIDRs</a>).

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_workforce` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_workforce.html)

```python
# describe_workforce method definition

await def describe_workforce(
    self,
    *,
    WorkforceName: str,
) -> DescribeWorkforceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkforceResponseTypeDef](./type_defs.md#describeworkforceresponsetypedef) 


```python
# describe_workforce method usage example with argument unpacking

kwargs: DescribeWorkforceRequestTypeDef = {  # (1)
    "WorkforceName": ...,
}

parent.describe_workforce(**kwargs)
```

1. See [:material-code-braces: DescribeWorkforceRequestTypeDef](./type_defs.md#describeworkforcerequesttypedef) 

### describe\_workteam

Gets information about a specific work team.

Type annotations and code completion for `#!python session.create_client("sagemaker").describe_workteam` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/describe_workteam.html)

```python
# describe_workteam method definition

await def describe_workteam(
    self,
    *,
    WorkteamName: str,
) -> DescribeWorkteamResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeWorkteamResponseTypeDef](./type_defs.md#describeworkteamresponsetypedef) 


```python
# describe_workteam method usage example with argument unpacking

kwargs: DescribeWorkteamRequestTypeDef = {  # (1)
    "WorkteamName": ...,
}

parent.describe_workteam(**kwargs)
```

1. See [:material-code-braces: DescribeWorkteamRequestTypeDef](./type_defs.md#describeworkteamrequesttypedef) 

### disable\_sagemaker\_servicecatalog\_portfolio

Disables using Service Catalog in SageMaker.

Type annotations and code completion for `#!python session.create_client("sagemaker").disable_sagemaker_servicecatalog_portfolio` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/disable_sagemaker_servicecatalog_portfolio.html)

```python
# disable_sagemaker_servicecatalog_portfolio method definition

await def disable_sagemaker_servicecatalog_portfolio(
    self,
) -> Dict[str, Any]:
    ...
```


### disassociate\_trial\_component

Disassociates a trial component from a trial.

Type annotations and code completion for `#!python session.create_client("sagemaker").disassociate_trial_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/disassociate_trial_component.html)

```python
# disassociate_trial_component method definition

await def disassociate_trial_component(
    self,
    *,
    TrialComponentName: str,
    TrialName: str,
) -> DisassociateTrialComponentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateTrialComponentResponseTypeDef](./type_defs.md#disassociatetrialcomponentresponsetypedef) 


```python
# disassociate_trial_component method usage example with argument unpacking

kwargs: DisassociateTrialComponentRequestTypeDef = {  # (1)
    "TrialComponentName": ...,
    "TrialName": ...,
}

parent.disassociate_trial_component(**kwargs)
```

1. See [:material-code-braces: DisassociateTrialComponentRequestTypeDef](./type_defs.md#disassociatetrialcomponentrequesttypedef) 

### enable\_sagemaker\_servicecatalog\_portfolio

Enables using Service Catalog in SageMaker.

Type annotations and code completion for `#!python session.create_client("sagemaker").enable_sagemaker_servicecatalog_portfolio` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/enable_sagemaker_servicecatalog_portfolio.html)

```python
# enable_sagemaker_servicecatalog_portfolio method definition

await def enable_sagemaker_servicecatalog_portfolio(
    self,
) -> Dict[str, Any]:
    ...
```


### get\_device\_fleet\_report

Describes a fleet.

Type annotations and code completion for `#!python session.create_client("sagemaker").get_device_fleet_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/get_device_fleet_report.html)

```python
# get_device_fleet_report method definition

await def get_device_fleet_report(
    self,
    *,
    DeviceFleetName: str,
) -> GetDeviceFleetReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceFleetReportResponseTypeDef](./type_defs.md#getdevicefleetreportresponsetypedef) 


```python
# get_device_fleet_report method usage example with argument unpacking

kwargs: GetDeviceFleetReportRequestTypeDef = {  # (1)
    "DeviceFleetName": ...,
}

parent.get_device_fleet_report(**kwargs)
```

1. See [:material-code-braces: GetDeviceFleetReportRequestTypeDef](./type_defs.md#getdevicefleetreportrequesttypedef) 

### get\_lineage\_group\_policy

The resource policy for the lineage group.

Type annotations and code completion for `#!python session.create_client("sagemaker").get_lineage_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/get_lineage_group_policy.html)

```python
# get_lineage_group_policy method definition

await def get_lineage_group_policy(
    self,
    *,
    LineageGroupName: str,
) -> GetLineageGroupPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLineageGroupPolicyResponseTypeDef](./type_defs.md#getlineagegrouppolicyresponsetypedef) 


```python
# get_lineage_group_policy method usage example with argument unpacking

kwargs: GetLineageGroupPolicyRequestTypeDef = {  # (1)
    "LineageGroupName": ...,
}

parent.get_lineage_group_policy(**kwargs)
```

1. See [:material-code-braces: GetLineageGroupPolicyRequestTypeDef](./type_defs.md#getlineagegrouppolicyrequesttypedef) 

### get\_model\_package\_group\_policy

Gets a resource policy that manages access for a model group.

Type annotations and code completion for `#!python session.create_client("sagemaker").get_model_package_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/get_model_package_group_policy.html)

```python
# get_model_package_group_policy method definition

await def get_model_package_group_policy(
    self,
    *,
    ModelPackageGroupName: str,
) -> GetModelPackageGroupPolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelPackageGroupPolicyOutputTypeDef](./type_defs.md#getmodelpackagegrouppolicyoutputtypedef) 


```python
# get_model_package_group_policy method usage example with argument unpacking

kwargs: GetModelPackageGroupPolicyInputTypeDef = {  # (1)
    "ModelPackageGroupName": ...,
}

parent.get_model_package_group_policy(**kwargs)
```

1. See [:material-code-braces: GetModelPackageGroupPolicyInputTypeDef](./type_defs.md#getmodelpackagegrouppolicyinputtypedef) 

### get\_sagemaker\_servicecatalog\_portfolio\_status

Gets the status of Service Catalog in SageMaker.

Type annotations and code completion for `#!python session.create_client("sagemaker").get_sagemaker_servicecatalog_portfolio_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/get_sagemaker_servicecatalog_portfolio_status.html)

```python
# get_sagemaker_servicecatalog_portfolio_status method definition

await def get_sagemaker_servicecatalog_portfolio_status(
    self,
) -> GetSagemakerServicecatalogPortfolioStatusOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSagemakerServicecatalogPortfolioStatusOutputTypeDef](./type_defs.md#getsagemakerservicecatalogportfoliostatusoutputtypedef) 

### get\_scaling\_configuration\_recommendation

Starts an Amazon SageMaker Inference Recommender autoscaling recommendation job.

Type annotations and code completion for `#!python session.create_client("sagemaker").get_scaling_configuration_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/get_scaling_configuration_recommendation.html)

```python
# get_scaling_configuration_recommendation method definition

await def get_scaling_configuration_recommendation(
    self,
    *,
    InferenceRecommendationsJobName: str,
    RecommendationId: str = ...,
    EndpointName: str = ...,
    TargetCpuUtilizationPerCore: int = ...,
    ScalingPolicyObjective: ScalingPolicyObjectiveTypeDef = ...,  # (1)
) -> GetScalingConfigurationRecommendationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ScalingPolicyObjectiveTypeDef](./type_defs.md#scalingpolicyobjectivetypedef) 
2. See [:material-code-braces: GetScalingConfigurationRecommendationResponseTypeDef](./type_defs.md#getscalingconfigurationrecommendationresponsetypedef) 


```python
# get_scaling_configuration_recommendation method usage example with argument unpacking

kwargs: GetScalingConfigurationRecommendationRequestTypeDef = {  # (1)
    "InferenceRecommendationsJobName": ...,
}

parent.get_scaling_configuration_recommendation(**kwargs)
```

1. See [:material-code-braces: GetScalingConfigurationRecommendationRequestTypeDef](./type_defs.md#getscalingconfigurationrecommendationrequesttypedef) 

### get\_search\_suggestions

An auto-complete API for the search functionality in the SageMaker console.

Type annotations and code completion for `#!python session.create_client("sagemaker").get_search_suggestions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/get_search_suggestions.html)

```python
# get_search_suggestions method definition

await def get_search_suggestions(
    self,
    *,
    Resource: ResourceTypeType,  # (1)
    SuggestionQuery: SuggestionQueryTypeDef = ...,  # (2)
) -> GetSearchSuggestionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: SuggestionQueryTypeDef](./type_defs.md#suggestionquerytypedef) 
3. See [:material-code-braces: GetSearchSuggestionsResponseTypeDef](./type_defs.md#getsearchsuggestionsresponsetypedef) 


```python
# get_search_suggestions method usage example with argument unpacking

kwargs: GetSearchSuggestionsRequestTypeDef = {  # (1)
    "Resource": ...,
}

parent.get_search_suggestions(**kwargs)
```

1. See [:material-code-braces: GetSearchSuggestionsRequestTypeDef](./type_defs.md#getsearchsuggestionsrequesttypedef) 

### import\_hub\_content

Import hub content.

Type annotations and code completion for `#!python session.create_client("sagemaker").import_hub_content` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/import_hub_content.html)

```python
# import_hub_content method definition

await def import_hub_content(
    self,
    *,
    HubContentName: str,
    HubContentType: HubContentTypeType,  # (1)
    DocumentSchemaVersion: str,
    HubName: str,
    HubContentDocument: str,
    HubContentVersion: str = ...,
    HubContentDisplayName: str = ...,
    HubContentDescription: str = ...,
    HubContentMarkdown: str = ...,
    HubContentSearchKeywords: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> ImportHubContentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ImportHubContentResponseTypeDef](./type_defs.md#importhubcontentresponsetypedef) 


```python
# import_hub_content method usage example with argument unpacking

kwargs: ImportHubContentRequestTypeDef = {  # (1)
    "HubContentName": ...,
    "HubContentType": ...,
    "DocumentSchemaVersion": ...,
    "HubName": ...,
    "HubContentDocument": ...,
}

parent.import_hub_content(**kwargs)
```

1. See [:material-code-braces: ImportHubContentRequestTypeDef](./type_defs.md#importhubcontentrequesttypedef) 

### list\_actions

Lists the actions in your account and their properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_actions.html)

```python
# list_actions method definition

await def list_actions(
    self,
    *,
    SourceUri: str = ...,
    ActionType: str = ...,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    SortBy: SortActionsByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListActionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortActionsByType](./literals.md#sortactionsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef) 


```python
# list_actions method usage example with argument unpacking

kwargs: ListActionsRequestTypeDef = {  # (1)
    "SourceUri": ...,
}

parent.list_actions(**kwargs)
```

1. See [:material-code-braces: ListActionsRequestTypeDef](./type_defs.md#listactionsrequesttypedef) 

### list\_algorithms

Lists the machine learning algorithms that have been created.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_algorithms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_algorithms.html)

```python
# list_algorithms method definition

await def list_algorithms(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    NextToken: str = ...,
    SortBy: AlgorithmSortByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
) -> ListAlgorithmsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AlgorithmSortByType](./literals.md#algorithmsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListAlgorithmsOutputTypeDef](./type_defs.md#listalgorithmsoutputtypedef) 


```python
# list_algorithms method usage example with argument unpacking

kwargs: ListAlgorithmsInputTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_algorithms(**kwargs)
```

1. See [:material-code-braces: ListAlgorithmsInputTypeDef](./type_defs.md#listalgorithmsinputtypedef) 

### list\_aliases

Lists the aliases of a specified image or image version.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_aliases.html)

```python
# list_aliases method definition

await def list_aliases(
    self,
    *,
    ImageName: str,
    Alias: str = ...,
    Version: int = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAliasesResponseTypeDef](./type_defs.md#listaliasesresponsetypedef) 


```python
# list_aliases method usage example with argument unpacking

kwargs: ListAliasesRequestTypeDef = {  # (1)
    "ImageName": ...,
}

parent.list_aliases(**kwargs)
```

1. See [:material-code-braces: ListAliasesRequestTypeDef](./type_defs.md#listaliasesrequesttypedef) 

### list\_app\_image\_configs

Lists the AppImageConfigs in your account and their properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_app_image_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_app_image_configs.html)

```python
# list_app_image_configs method definition

await def list_app_image_configs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    ModifiedTimeBefore: TimestampTypeDef = ...,
    ModifiedTimeAfter: TimestampTypeDef = ...,
    SortBy: AppImageConfigSortKeyType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
) -> ListAppImageConfigsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AppImageConfigSortKeyType](./literals.md#appimageconfigsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListAppImageConfigsResponseTypeDef](./type_defs.md#listappimageconfigsresponsetypedef) 


```python
# list_app_image_configs method usage example with argument unpacking

kwargs: ListAppImageConfigsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_app_image_configs(**kwargs)
```

1. See [:material-code-braces: ListAppImageConfigsRequestTypeDef](./type_defs.md#listappimageconfigsrequesttypedef) 

### list\_apps

Lists apps.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_apps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_apps.html)

```python
# list_apps method definition

await def list_apps(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    SortOrder: SortOrderType = ...,  # (1)
    SortBy: AppSortKeyType = ...,  # (2)
    DomainIdEquals: str = ...,
    UserProfileNameEquals: str = ...,
    SpaceNameEquals: str = ...,
) -> ListAppsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: AppSortKeyType](./literals.md#appsortkeytype) 
3. See [:material-code-braces: ListAppsResponseTypeDef](./type_defs.md#listappsresponsetypedef) 


```python
# list_apps method usage example with argument unpacking

kwargs: ListAppsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_apps(**kwargs)
```

1. See [:material-code-braces: ListAppsRequestTypeDef](./type_defs.md#listappsrequesttypedef) 

### list\_artifacts

Lists the artifacts in your account and their properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_artifacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_artifacts.html)

```python
# list_artifacts method definition

await def list_artifacts(
    self,
    *,
    SourceUri: str = ...,
    ArtifactType: str = ...,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    SortBy: SortArtifactsByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListArtifactsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortArtifactsByType](./literals.md#sortartifactsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListArtifactsResponseTypeDef](./type_defs.md#listartifactsresponsetypedef) 


```python
# list_artifacts method usage example with argument unpacking

kwargs: ListArtifactsRequestTypeDef = {  # (1)
    "SourceUri": ...,
}

parent.list_artifacts(**kwargs)
```

1. See [:material-code-braces: ListArtifactsRequestTypeDef](./type_defs.md#listartifactsrequesttypedef) 

### list\_associations

Lists the associations in your account and their properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_associations.html)

```python
# list_associations method definition

await def list_associations(
    self,
    *,
    SourceArn: str = ...,
    DestinationArn: str = ...,
    SourceType: str = ...,
    DestinationType: str = ...,
    AssociationType: AssociationEdgeTypeType = ...,  # (1)
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    SortBy: SortAssociationsByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListAssociationsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AssociationEdgeTypeType](./literals.md#associationedgetypetype) 
2. See [:material-code-brackets: SortAssociationsByType](./literals.md#sortassociationsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListAssociationsResponseTypeDef](./type_defs.md#listassociationsresponsetypedef) 


```python
# list_associations method usage example with argument unpacking

kwargs: ListAssociationsRequestTypeDef = {  # (1)
    "SourceArn": ...,
}

parent.list_associations(**kwargs)
```

1. See [:material-code-braces: ListAssociationsRequestTypeDef](./type_defs.md#listassociationsrequesttypedef) 

### list\_auto\_ml\_jobs

Request a list of jobs.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_auto_ml_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_auto_ml_jobs.html)

```python
# list_auto_ml_jobs method definition

await def list_auto_ml_jobs(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    StatusEquals: AutoMLJobStatusType = ...,  # (1)
    SortOrder: AutoMLSortOrderType = ...,  # (2)
    SortBy: AutoMLSortByType = ...,  # (3)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListAutoMLJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AutoMLJobStatusType](./literals.md#automljobstatustype) 
2. See [:material-code-brackets: AutoMLSortOrderType](./literals.md#automlsortordertype) 
3. See [:material-code-brackets: AutoMLSortByType](./literals.md#automlsortbytype) 
4. See [:material-code-braces: ListAutoMLJobsResponseTypeDef](./type_defs.md#listautomljobsresponsetypedef) 


```python
# list_auto_ml_jobs method usage example with argument unpacking

kwargs: ListAutoMLJobsRequestTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_auto_ml_jobs(**kwargs)
```

1. See [:material-code-braces: ListAutoMLJobsRequestTypeDef](./type_defs.md#listautomljobsrequesttypedef) 

### list\_candidates\_for\_auto\_ml\_job

List the candidates created for the job.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_candidates_for_auto_ml_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_candidates_for_auto_ml_job.html)

```python
# list_candidates_for_auto_ml_job method definition

await def list_candidates_for_auto_ml_job(
    self,
    *,
    AutoMLJobName: str,
    StatusEquals: CandidateStatusType = ...,  # (1)
    CandidateNameEquals: str = ...,
    SortOrder: AutoMLSortOrderType = ...,  # (2)
    SortBy: CandidateSortByType = ...,  # (3)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListCandidatesForAutoMLJobResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: CandidateStatusType](./literals.md#candidatestatustype) 
2. See [:material-code-brackets: AutoMLSortOrderType](./literals.md#automlsortordertype) 
3. See [:material-code-brackets: CandidateSortByType](./literals.md#candidatesortbytype) 
4. See [:material-code-braces: ListCandidatesForAutoMLJobResponseTypeDef](./type_defs.md#listcandidatesforautomljobresponsetypedef) 


```python
# list_candidates_for_auto_ml_job method usage example with argument unpacking

kwargs: ListCandidatesForAutoMLJobRequestTypeDef = {  # (1)
    "AutoMLJobName": ...,
}

parent.list_candidates_for_auto_ml_job(**kwargs)
```

1. See [:material-code-braces: ListCandidatesForAutoMLJobRequestTypeDef](./type_defs.md#listcandidatesforautomljobrequesttypedef) 

### list\_cluster\_nodes

Retrieves the list of instances (also called <i>nodes</i> interchangeably) in a
SageMaker HyperPod cluster.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_cluster_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_cluster_nodes.html)

```python
# list_cluster_nodes method definition

await def list_cluster_nodes(
    self,
    *,
    ClusterName: str,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    InstanceGroupNameContains: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    SortBy: ClusterSortByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
) -> ListClusterNodesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ClusterSortByType](./literals.md#clustersortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListClusterNodesResponseTypeDef](./type_defs.md#listclusternodesresponsetypedef) 


```python
# list_cluster_nodes method usage example with argument unpacking

kwargs: ListClusterNodesRequestTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.list_cluster_nodes(**kwargs)
```

1. See [:material-code-braces: ListClusterNodesRequestTypeDef](./type_defs.md#listclusternodesrequesttypedef) 

### list\_cluster\_scheduler\_configs

List the cluster policy configurations.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_cluster_scheduler_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_cluster_scheduler_configs.html)

```python
# list_cluster_scheduler_configs method definition

await def list_cluster_scheduler_configs(
    self,
    *,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    ClusterArn: str = ...,
    Status: SchedulerResourceStatusType = ...,  # (1)
    SortBy: SortClusterSchedulerConfigByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListClusterSchedulerConfigsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: SchedulerResourceStatusType](./literals.md#schedulerresourcestatustype) 
2. See [:material-code-brackets: SortClusterSchedulerConfigByType](./literals.md#sortclusterschedulerconfigbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListClusterSchedulerConfigsResponseTypeDef](./type_defs.md#listclusterschedulerconfigsresponsetypedef) 


```python
# list_cluster_scheduler_configs method usage example with argument unpacking

kwargs: ListClusterSchedulerConfigsRequestTypeDef = {  # (1)
    "CreatedAfter": ...,
}

parent.list_cluster_scheduler_configs(**kwargs)
```

1. See [:material-code-braces: ListClusterSchedulerConfigsRequestTypeDef](./type_defs.md#listclusterschedulerconfigsrequesttypedef) 

### list\_clusters

Retrieves the list of SageMaker HyperPod clusters.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_clusters.html)

```python
# list_clusters method definition

await def list_clusters(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    NextToken: str = ...,
    SortBy: ClusterSortByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    TrainingPlanArn: str = ...,
) -> ListClustersResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ClusterSortByType](./literals.md#clustersortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


```python
# list_clusters method usage example with argument unpacking

kwargs: ListClustersRequestTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_clusters(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestTypeDef](./type_defs.md#listclustersrequesttypedef) 

### list\_code\_repositories

Gets a list of the Git repositories in your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_code_repositories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_code_repositories.html)

```python
# list_code_repositories method definition

await def list_code_repositories(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    NextToken: str = ...,
    SortBy: CodeRepositorySortByType = ...,  # (1)
    SortOrder: CodeRepositorySortOrderType = ...,  # (2)
) -> ListCodeRepositoriesOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CodeRepositorySortByType](./literals.md#coderepositorysortbytype) 
2. See [:material-code-brackets: CodeRepositorySortOrderType](./literals.md#coderepositorysortordertype) 
3. See [:material-code-braces: ListCodeRepositoriesOutputTypeDef](./type_defs.md#listcoderepositoriesoutputtypedef) 


```python
# list_code_repositories method usage example with argument unpacking

kwargs: ListCodeRepositoriesInputTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_code_repositories(**kwargs)
```

1. See [:material-code-braces: ListCodeRepositoriesInputTypeDef](./type_defs.md#listcoderepositoriesinputtypedef) 

### list\_compilation\_jobs

Lists model compilation jobs that satisfy various filters.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_compilation_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_compilation_jobs.html)

```python
# list_compilation_jobs method definition

await def list_compilation_jobs(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    StatusEquals: CompilationJobStatusType = ...,  # (1)
    SortBy: ListCompilationJobsSortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
) -> ListCompilationJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: CompilationJobStatusType](./literals.md#compilationjobstatustype) 
2. See [:material-code-brackets: ListCompilationJobsSortByType](./literals.md#listcompilationjobssortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListCompilationJobsResponseTypeDef](./type_defs.md#listcompilationjobsresponsetypedef) 


```python
# list_compilation_jobs method usage example with argument unpacking

kwargs: ListCompilationJobsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_compilation_jobs(**kwargs)
```

1. See [:material-code-braces: ListCompilationJobsRequestTypeDef](./type_defs.md#listcompilationjobsrequesttypedef) 

### list\_compute\_quotas

List the resource allocation definitions.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_compute_quotas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_compute_quotas.html)

```python
# list_compute_quotas method definition

await def list_compute_quotas(
    self,
    *,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    Status: SchedulerResourceStatusType = ...,  # (1)
    ClusterArn: str = ...,
    SortBy: SortQuotaByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListComputeQuotasResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: SchedulerResourceStatusType](./literals.md#schedulerresourcestatustype) 
2. See [:material-code-brackets: SortQuotaByType](./literals.md#sortquotabytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListComputeQuotasResponseTypeDef](./type_defs.md#listcomputequotasresponsetypedef) 


```python
# list_compute_quotas method usage example with argument unpacking

kwargs: ListComputeQuotasRequestTypeDef = {  # (1)
    "CreatedAfter": ...,
}

parent.list_compute_quotas(**kwargs)
```

1. See [:material-code-braces: ListComputeQuotasRequestTypeDef](./type_defs.md#listcomputequotasrequesttypedef) 

### list\_contexts

Lists the contexts in your account and their properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_contexts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_contexts.html)

```python
# list_contexts method definition

await def list_contexts(
    self,
    *,
    SourceUri: str = ...,
    ContextType: str = ...,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    SortBy: SortContextsByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListContextsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortContextsByType](./literals.md#sortcontextsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListContextsResponseTypeDef](./type_defs.md#listcontextsresponsetypedef) 


```python
# list_contexts method usage example with argument unpacking

kwargs: ListContextsRequestTypeDef = {  # (1)
    "SourceUri": ...,
}

parent.list_contexts(**kwargs)
```

1. See [:material-code-braces: ListContextsRequestTypeDef](./type_defs.md#listcontextsrequesttypedef) 

### list\_data\_quality\_job\_definitions

Lists the data quality job definitions in your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_data_quality_job_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_data_quality_job_definitions.html)

```python
# list_data_quality_job_definitions method definition

await def list_data_quality_job_definitions(
    self,
    *,
    EndpointName: str = ...,
    SortBy: MonitoringJobDefinitionSortKeyType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
) -> ListDataQualityJobDefinitionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListDataQualityJobDefinitionsResponseTypeDef](./type_defs.md#listdataqualityjobdefinitionsresponsetypedef) 


```python
# list_data_quality_job_definitions method usage example with argument unpacking

kwargs: ListDataQualityJobDefinitionsRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.list_data_quality_job_definitions(**kwargs)
```

1. See [:material-code-braces: ListDataQualityJobDefinitionsRequestTypeDef](./type_defs.md#listdataqualityjobdefinitionsrequesttypedef) 

### list\_device\_fleets

Returns a list of devices in the fleet.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_device_fleets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_device_fleets.html)

```python
# list_device_fleets method definition

await def list_device_fleets(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    SortBy: ListDeviceFleetsSortByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
) -> ListDeviceFleetsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ListDeviceFleetsSortByType](./literals.md#listdevicefleetssortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListDeviceFleetsResponseTypeDef](./type_defs.md#listdevicefleetsresponsetypedef) 


```python
# list_device_fleets method usage example with argument unpacking

kwargs: ListDeviceFleetsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_device_fleets(**kwargs)
```

1. See [:material-code-braces: ListDeviceFleetsRequestTypeDef](./type_defs.md#listdevicefleetsrequesttypedef) 

### list\_devices

A list of devices.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_devices.html)

```python
# list_devices method definition

await def list_devices(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    LatestHeartbeatAfter: TimestampTypeDef = ...,
    ModelName: str = ...,
    DeviceFleetName: str = ...,
) -> ListDevicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 


```python
# list_devices method usage example with argument unpacking

kwargs: ListDevicesRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_devices(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestTypeDef](./type_defs.md#listdevicesrequesttypedef) 

### list\_domains

Lists the domains.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_domains.html)

```python
# list_domains method definition

await def list_domains(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDomainsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 


```python
# list_domains method usage example with argument unpacking

kwargs: ListDomainsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_domains(**kwargs)
```

1. See [:material-code-braces: ListDomainsRequestTypeDef](./type_defs.md#listdomainsrequesttypedef) 

### list\_edge\_deployment\_plans

Lists all edge deployment plans.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_edge_deployment_plans` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_edge_deployment_plans.html)

```python
# list_edge_deployment_plans method definition

await def list_edge_deployment_plans(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    DeviceFleetNameContains: str = ...,
    SortBy: ListEdgeDeploymentPlansSortByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
) -> ListEdgeDeploymentPlansResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ListEdgeDeploymentPlansSortByType](./literals.md#listedgedeploymentplanssortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListEdgeDeploymentPlansResponseTypeDef](./type_defs.md#listedgedeploymentplansresponsetypedef) 


```python
# list_edge_deployment_plans method usage example with argument unpacking

kwargs: ListEdgeDeploymentPlansRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_edge_deployment_plans(**kwargs)
```

1. See [:material-code-braces: ListEdgeDeploymentPlansRequestTypeDef](./type_defs.md#listedgedeploymentplansrequesttypedef) 

### list\_edge\_packaging\_jobs

Returns a list of edge packaging jobs.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_edge_packaging_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_edge_packaging_jobs.html)

```python
# list_edge_packaging_jobs method definition

await def list_edge_packaging_jobs(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    ModelNameContains: str = ...,
    StatusEquals: EdgePackagingJobStatusType = ...,  # (1)
    SortBy: ListEdgePackagingJobsSortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
) -> ListEdgePackagingJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: EdgePackagingJobStatusType](./literals.md#edgepackagingjobstatustype) 
2. See [:material-code-brackets: ListEdgePackagingJobsSortByType](./literals.md#listedgepackagingjobssortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListEdgePackagingJobsResponseTypeDef](./type_defs.md#listedgepackagingjobsresponsetypedef) 


```python
# list_edge_packaging_jobs method usage example with argument unpacking

kwargs: ListEdgePackagingJobsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_edge_packaging_jobs(**kwargs)
```

1. See [:material-code-braces: ListEdgePackagingJobsRequestTypeDef](./type_defs.md#listedgepackagingjobsrequesttypedef) 

### list\_endpoint\_configs

Lists endpoint configurations.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_endpoint_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_endpoint_configs.html)

```python
# list_endpoint_configs method definition

await def list_endpoint_configs(
    self,
    *,
    SortBy: EndpointConfigSortKeyType = ...,  # (1)
    SortOrder: OrderKeyType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
) -> ListEndpointConfigsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EndpointConfigSortKeyType](./literals.md#endpointconfigsortkeytype) 
2. See [:material-code-brackets: OrderKeyType](./literals.md#orderkeytype) 
3. See [:material-code-braces: ListEndpointConfigsOutputTypeDef](./type_defs.md#listendpointconfigsoutputtypedef) 


```python
# list_endpoint_configs method usage example with argument unpacking

kwargs: ListEndpointConfigsInputTypeDef = {  # (1)
    "SortBy": ...,
}

parent.list_endpoint_configs(**kwargs)
```

1. See [:material-code-braces: ListEndpointConfigsInputTypeDef](./type_defs.md#listendpointconfigsinputtypedef) 

### list\_endpoints

Lists endpoints.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_endpoints.html)

```python
# list_endpoints method definition

await def list_endpoints(
    self,
    *,
    SortBy: EndpointSortKeyType = ...,  # (1)
    SortOrder: OrderKeyType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    StatusEquals: EndpointStatusType = ...,  # (3)
) -> ListEndpointsOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: EndpointSortKeyType](./literals.md#endpointsortkeytype) 
2. See [:material-code-brackets: OrderKeyType](./literals.md#orderkeytype) 
3. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
4. See [:material-code-braces: ListEndpointsOutputTypeDef](./type_defs.md#listendpointsoutputtypedef) 


```python
# list_endpoints method usage example with argument unpacking

kwargs: ListEndpointsInputTypeDef = {  # (1)
    "SortBy": ...,
}

parent.list_endpoints(**kwargs)
```

1. See [:material-code-braces: ListEndpointsInputTypeDef](./type_defs.md#listendpointsinputtypedef) 

### list\_experiments

Lists all the experiments in your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_experiments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_experiments.html)

```python
# list_experiments method definition

await def list_experiments(
    self,
    *,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    SortBy: SortExperimentsByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListExperimentsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortExperimentsByType](./literals.md#sortexperimentsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef) 


```python
# list_experiments method usage example with argument unpacking

kwargs: ListExperimentsRequestTypeDef = {  # (1)
    "CreatedAfter": ...,
}

parent.list_experiments(**kwargs)
```

1. See [:material-code-braces: ListExperimentsRequestTypeDef](./type_defs.md#listexperimentsrequesttypedef) 

### list\_feature\_groups

List <code>FeatureGroup</code>s based on given filter and order.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_feature_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_feature_groups.html)

```python
# list_feature_groups method definition

await def list_feature_groups(
    self,
    *,
    NameContains: str = ...,
    FeatureGroupStatusEquals: FeatureGroupStatusType = ...,  # (1)
    OfflineStoreStatusEquals: OfflineStoreStatusValueType = ...,  # (2)
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    SortOrder: FeatureGroupSortOrderType = ...,  # (3)
    SortBy: FeatureGroupSortByType = ...,  # (4)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListFeatureGroupsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: FeatureGroupStatusType](./literals.md#featuregroupstatustype) 
2. See [:material-code-brackets: OfflineStoreStatusValueType](./literals.md#offlinestorestatusvaluetype) 
3. See [:material-code-brackets: FeatureGroupSortOrderType](./literals.md#featuregroupsortordertype) 
4. See [:material-code-brackets: FeatureGroupSortByType](./literals.md#featuregroupsortbytype) 
5. See [:material-code-braces: ListFeatureGroupsResponseTypeDef](./type_defs.md#listfeaturegroupsresponsetypedef) 


```python
# list_feature_groups method usage example with argument unpacking

kwargs: ListFeatureGroupsRequestTypeDef = {  # (1)
    "NameContains": ...,
}

parent.list_feature_groups(**kwargs)
```

1. See [:material-code-braces: ListFeatureGroupsRequestTypeDef](./type_defs.md#listfeaturegroupsrequesttypedef) 

### list\_flow\_definitions

Returns information about the flow definitions in your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_flow_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_flow_definitions.html)

```python
# list_flow_definitions method definition

await def list_flow_definitions(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    SortOrder: SortOrderType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListFlowDefinitionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: ListFlowDefinitionsResponseTypeDef](./type_defs.md#listflowdefinitionsresponsetypedef) 


```python
# list_flow_definitions method usage example with argument unpacking

kwargs: ListFlowDefinitionsRequestTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_flow_definitions(**kwargs)
```

1. See [:material-code-braces: ListFlowDefinitionsRequestTypeDef](./type_defs.md#listflowdefinitionsrequesttypedef) 

### list\_hub\_content\_versions

List hub content versions.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_hub_content_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_hub_content_versions.html)

```python
# list_hub_content_versions method definition

await def list_hub_content_versions(
    self,
    *,
    HubName: str,
    HubContentType: HubContentTypeType,  # (1)
    HubContentName: str,
    MinVersion: str = ...,
    MaxSchemaVersion: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    SortBy: HubContentSortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListHubContentVersionsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-brackets: HubContentSortByType](./literals.md#hubcontentsortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListHubContentVersionsResponseTypeDef](./type_defs.md#listhubcontentversionsresponsetypedef) 


```python
# list_hub_content_versions method usage example with argument unpacking

kwargs: ListHubContentVersionsRequestTypeDef = {  # (1)
    "HubName": ...,
    "HubContentType": ...,
    "HubContentName": ...,
}

parent.list_hub_content_versions(**kwargs)
```

1. See [:material-code-braces: ListHubContentVersionsRequestTypeDef](./type_defs.md#listhubcontentversionsrequesttypedef) 

### list\_hub\_contents

List the contents of a hub.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_hub_contents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_hub_contents.html)

```python
# list_hub_contents method definition

await def list_hub_contents(
    self,
    *,
    HubName: str,
    HubContentType: HubContentTypeType,  # (1)
    NameContains: str = ...,
    MaxSchemaVersion: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    SortBy: HubContentSortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListHubContentsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-brackets: HubContentSortByType](./literals.md#hubcontentsortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListHubContentsResponseTypeDef](./type_defs.md#listhubcontentsresponsetypedef) 


```python
# list_hub_contents method usage example with argument unpacking

kwargs: ListHubContentsRequestTypeDef = {  # (1)
    "HubName": ...,
    "HubContentType": ...,
}

parent.list_hub_contents(**kwargs)
```

1. See [:material-code-braces: ListHubContentsRequestTypeDef](./type_defs.md#listhubcontentsrequesttypedef) 

### list\_hubs

List all existing hubs.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_hubs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_hubs.html)

```python
# list_hubs method definition

await def list_hubs(
    self,
    *,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    SortBy: HubSortByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListHubsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: HubSortByType](./literals.md#hubsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListHubsResponseTypeDef](./type_defs.md#listhubsresponsetypedef) 


```python
# list_hubs method usage example with argument unpacking

kwargs: ListHubsRequestTypeDef = {  # (1)
    "NameContains": ...,
}

parent.list_hubs(**kwargs)
```

1. See [:material-code-braces: ListHubsRequestTypeDef](./type_defs.md#listhubsrequesttypedef) 

### list\_human\_task\_uis

Returns information about the human task user interfaces in your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_human_task_uis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_human_task_uis.html)

```python
# list_human_task_uis method definition

await def list_human_task_uis(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    SortOrder: SortOrderType = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListHumanTaskUisResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: ListHumanTaskUisResponseTypeDef](./type_defs.md#listhumantaskuisresponsetypedef) 


```python
# list_human_task_uis method usage example with argument unpacking

kwargs: ListHumanTaskUisRequestTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_human_task_uis(**kwargs)
```

1. See [:material-code-braces: ListHumanTaskUisRequestTypeDef](./type_defs.md#listhumantaskuisrequesttypedef) 

### list\_hyper\_parameter\_tuning\_jobs

Gets a list of <a
href="https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobSummary.html">HyperParameterTuningJobSummary</a>
objects that describe the hyperparameter tuning jobs launched in your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_hyper_parameter_tuning_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_hyper_parameter_tuning_jobs.html)

```python
# list_hyper_parameter_tuning_jobs method definition

await def list_hyper_parameter_tuning_jobs(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    SortBy: HyperParameterTuningJobSortByOptionsType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NameContains: str = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    StatusEquals: HyperParameterTuningJobStatusType = ...,  # (3)
) -> ListHyperParameterTuningJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: HyperParameterTuningJobSortByOptionsType](./literals.md#hyperparametertuningjobsortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: HyperParameterTuningJobStatusType](./literals.md#hyperparametertuningjobstatustype) 
4. See [:material-code-braces: ListHyperParameterTuningJobsResponseTypeDef](./type_defs.md#listhyperparametertuningjobsresponsetypedef) 


```python
# list_hyper_parameter_tuning_jobs method usage example with argument unpacking

kwargs: ListHyperParameterTuningJobsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_hyper_parameter_tuning_jobs(**kwargs)
```

1. See [:material-code-braces: ListHyperParameterTuningJobsRequestTypeDef](./type_defs.md#listhyperparametertuningjobsrequesttypedef) 

### list\_image\_versions

Lists the versions of a specified image and their properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_image_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_image_versions.html)

```python
# list_image_versions method definition

await def list_image_versions(
    self,
    *,
    ImageName: str,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    SortBy: ImageVersionSortByType = ...,  # (1)
    SortOrder: ImageVersionSortOrderType = ...,  # (2)
) -> ListImageVersionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ImageVersionSortByType](./literals.md#imageversionsortbytype) 
2. See [:material-code-brackets: ImageVersionSortOrderType](./literals.md#imageversionsortordertype) 
3. See [:material-code-braces: ListImageVersionsResponseTypeDef](./type_defs.md#listimageversionsresponsetypedef) 


```python
# list_image_versions method usage example with argument unpacking

kwargs: ListImageVersionsRequestTypeDef = {  # (1)
    "ImageName": ...,
}

parent.list_image_versions(**kwargs)
```

1. See [:material-code-braces: ListImageVersionsRequestTypeDef](./type_defs.md#listimageversionsrequesttypedef) 

### list\_images

Lists the images in your account and their properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_images` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_images.html)

```python
# list_images method definition

await def list_images(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    NextToken: str = ...,
    SortBy: ImageSortByType = ...,  # (1)
    SortOrder: ImageSortOrderType = ...,  # (2)
) -> ListImagesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ImageSortByType](./literals.md#imagesortbytype) 
2. See [:material-code-brackets: ImageSortOrderType](./literals.md#imagesortordertype) 
3. See [:material-code-braces: ListImagesResponseTypeDef](./type_defs.md#listimagesresponsetypedef) 


```python
# list_images method usage example with argument unpacking

kwargs: ListImagesRequestTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_images(**kwargs)
```

1. See [:material-code-braces: ListImagesRequestTypeDef](./type_defs.md#listimagesrequesttypedef) 

### list\_inference\_components

Lists the inference components in your account and their properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_inference_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_inference_components.html)

```python
# list_inference_components method definition

await def list_inference_components(
    self,
    *,
    SortBy: InferenceComponentSortKeyType = ...,  # (1)
    SortOrder: OrderKeyType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    StatusEquals: InferenceComponentStatusType = ...,  # (3)
    EndpointNameEquals: str = ...,
    VariantNameEquals: str = ...,
) -> ListInferenceComponentsOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: InferenceComponentSortKeyType](./literals.md#inferencecomponentsortkeytype) 
2. See [:material-code-brackets: OrderKeyType](./literals.md#orderkeytype) 
3. See [:material-code-brackets: InferenceComponentStatusType](./literals.md#inferencecomponentstatustype) 
4. See [:material-code-braces: ListInferenceComponentsOutputTypeDef](./type_defs.md#listinferencecomponentsoutputtypedef) 


```python
# list_inference_components method usage example with argument unpacking

kwargs: ListInferenceComponentsInputTypeDef = {  # (1)
    "SortBy": ...,
}

parent.list_inference_components(**kwargs)
```

1. See [:material-code-braces: ListInferenceComponentsInputTypeDef](./type_defs.md#listinferencecomponentsinputtypedef) 

### list\_inference\_experiments

Returns the list of all inference experiments.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_inference_experiments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_inference_experiments.html)

```python
# list_inference_experiments method definition

await def list_inference_experiments(
    self,
    *,
    NameContains: str = ...,
    Type: InferenceExperimentTypeType = ...,  # (1)
    StatusEquals: InferenceExperimentStatusType = ...,  # (2)
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    SortBy: SortInferenceExperimentsByType = ...,  # (3)
    SortOrder: SortOrderType = ...,  # (4)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListInferenceExperimentsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: InferenceExperimentTypeType](./literals.md#inferenceexperimenttypetype) 
2. See [:material-code-brackets: InferenceExperimentStatusType](./literals.md#inferenceexperimentstatustype) 
3. See [:material-code-brackets: SortInferenceExperimentsByType](./literals.md#sortinferenceexperimentsbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: ListInferenceExperimentsResponseTypeDef](./type_defs.md#listinferenceexperimentsresponsetypedef) 


```python
# list_inference_experiments method usage example with argument unpacking

kwargs: ListInferenceExperimentsRequestTypeDef = {  # (1)
    "NameContains": ...,
}

parent.list_inference_experiments(**kwargs)
```

1. See [:material-code-braces: ListInferenceExperimentsRequestTypeDef](./type_defs.md#listinferenceexperimentsrequesttypedef) 

### list\_inference\_recommendations\_job\_steps

Returns a list of the subtasks for an Inference Recommender job.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_inference_recommendations_job_steps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_inference_recommendations_job_steps.html)

```python
# list_inference_recommendations_job_steps method definition

await def list_inference_recommendations_job_steps(
    self,
    *,
    JobName: str,
    Status: RecommendationJobStatusType = ...,  # (1)
    StepType: RecommendationStepTypeType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListInferenceRecommendationsJobStepsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RecommendationJobStatusType](./literals.md#recommendationjobstatustype) 
2. See [:material-code-brackets: RecommendationStepTypeType](./literals.md#recommendationsteptypetype) 
3. See [:material-code-braces: ListInferenceRecommendationsJobStepsResponseTypeDef](./type_defs.md#listinferencerecommendationsjobstepsresponsetypedef) 


```python
# list_inference_recommendations_job_steps method usage example with argument unpacking

kwargs: ListInferenceRecommendationsJobStepsRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.list_inference_recommendations_job_steps(**kwargs)
```

1. See [:material-code-braces: ListInferenceRecommendationsJobStepsRequestTypeDef](./type_defs.md#listinferencerecommendationsjobstepsrequesttypedef) 

### list\_inference\_recommendations\_jobs

Lists recommendation jobs that satisfy various filters.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_inference_recommendations_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_inference_recommendations_jobs.html)

```python
# list_inference_recommendations_jobs method definition

await def list_inference_recommendations_jobs(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    StatusEquals: RecommendationJobStatusType = ...,  # (1)
    SortBy: ListInferenceRecommendationsJobsSortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
    ModelNameEquals: str = ...,
    ModelPackageVersionArnEquals: str = ...,
) -> ListInferenceRecommendationsJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: RecommendationJobStatusType](./literals.md#recommendationjobstatustype) 
2. See [:material-code-brackets: ListInferenceRecommendationsJobsSortByType](./literals.md#listinferencerecommendationsjobssortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListInferenceRecommendationsJobsResponseTypeDef](./type_defs.md#listinferencerecommendationsjobsresponsetypedef) 


```python
# list_inference_recommendations_jobs method usage example with argument unpacking

kwargs: ListInferenceRecommendationsJobsRequestTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_inference_recommendations_jobs(**kwargs)
```

1. See [:material-code-braces: ListInferenceRecommendationsJobsRequestTypeDef](./type_defs.md#listinferencerecommendationsjobsrequesttypedef) 

### list\_labeling\_jobs

Gets a list of labeling jobs.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_labeling_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_labeling_jobs.html)

```python
# list_labeling_jobs method definition

await def list_labeling_jobs(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    NameContains: str = ...,
    SortBy: SortByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    StatusEquals: LabelingJobStatusType = ...,  # (3)
) -> ListLabelingJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: LabelingJobStatusType](./literals.md#labelingjobstatustype) 
4. See [:material-code-braces: ListLabelingJobsResponseTypeDef](./type_defs.md#listlabelingjobsresponsetypedef) 


```python
# list_labeling_jobs method usage example with argument unpacking

kwargs: ListLabelingJobsRequestTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_labeling_jobs(**kwargs)
```

1. See [:material-code-braces: ListLabelingJobsRequestTypeDef](./type_defs.md#listlabelingjobsrequesttypedef) 

### list\_labeling\_jobs\_for\_workteam

Gets a list of labeling jobs assigned to a specified work team.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_labeling_jobs_for_workteam` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_labeling_jobs_for_workteam.html)

```python
# list_labeling_jobs_for_workteam method definition

await def list_labeling_jobs_for_workteam(
    self,
    *,
    WorkteamArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    JobReferenceCodeContains: str = ...,
    SortBy: ListLabelingJobsForWorkteamSortByOptionsType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
) -> ListLabelingJobsForWorkteamResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ListLabelingJobsForWorkteamSortByOptionsType](./literals.md#listlabelingjobsforworkteamsortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListLabelingJobsForWorkteamResponseTypeDef](./type_defs.md#listlabelingjobsforworkteamresponsetypedef) 


```python
# list_labeling_jobs_for_workteam method usage example with argument unpacking

kwargs: ListLabelingJobsForWorkteamRequestTypeDef = {  # (1)
    "WorkteamArn": ...,
}

parent.list_labeling_jobs_for_workteam(**kwargs)
```

1. See [:material-code-braces: ListLabelingJobsForWorkteamRequestTypeDef](./type_defs.md#listlabelingjobsforworkteamrequesttypedef) 

### list\_lineage\_groups

A list of lineage groups shared with your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_lineage_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_lineage_groups.html)

```python
# list_lineage_groups method definition

await def list_lineage_groups(
    self,
    *,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    SortBy: SortLineageGroupsByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListLineageGroupsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortLineageGroupsByType](./literals.md#sortlineagegroupsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListLineageGroupsResponseTypeDef](./type_defs.md#listlineagegroupsresponsetypedef) 


```python
# list_lineage_groups method usage example with argument unpacking

kwargs: ListLineageGroupsRequestTypeDef = {  # (1)
    "CreatedAfter": ...,
}

parent.list_lineage_groups(**kwargs)
```

1. See [:material-code-braces: ListLineageGroupsRequestTypeDef](./type_defs.md#listlineagegroupsrequesttypedef) 

### list\_mlflow\_tracking\_servers

Lists all MLflow Tracking Servers.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_mlflow_tracking_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_mlflow_tracking_servers.html)

```python
# list_mlflow_tracking_servers method definition

await def list_mlflow_tracking_servers(
    self,
    *,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    TrackingServerStatus: TrackingServerStatusType = ...,  # (1)
    MlflowVersion: str = ...,
    SortBy: SortTrackingServerByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMlflowTrackingServersResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: TrackingServerStatusType](./literals.md#trackingserverstatustype) 
2. See [:material-code-brackets: SortTrackingServerByType](./literals.md#sorttrackingserverbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListMlflowTrackingServersResponseTypeDef](./type_defs.md#listmlflowtrackingserversresponsetypedef) 


```python
# list_mlflow_tracking_servers method usage example with argument unpacking

kwargs: ListMlflowTrackingServersRequestTypeDef = {  # (1)
    "CreatedAfter": ...,
}

parent.list_mlflow_tracking_servers(**kwargs)
```

1. See [:material-code-braces: ListMlflowTrackingServersRequestTypeDef](./type_defs.md#listmlflowtrackingserversrequesttypedef) 

### list\_model\_bias\_job\_definitions

Lists model bias jobs definitions that satisfy various filters.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_model_bias_job_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_model_bias_job_definitions.html)

```python
# list_model_bias_job_definitions method definition

await def list_model_bias_job_definitions(
    self,
    *,
    EndpointName: str = ...,
    SortBy: MonitoringJobDefinitionSortKeyType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
) -> ListModelBiasJobDefinitionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListModelBiasJobDefinitionsResponseTypeDef](./type_defs.md#listmodelbiasjobdefinitionsresponsetypedef) 


```python
# list_model_bias_job_definitions method usage example with argument unpacking

kwargs: ListModelBiasJobDefinitionsRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.list_model_bias_job_definitions(**kwargs)
```

1. See [:material-code-braces: ListModelBiasJobDefinitionsRequestTypeDef](./type_defs.md#listmodelbiasjobdefinitionsrequesttypedef) 

### list\_model\_card\_export\_jobs

List the export jobs for the Amazon SageMaker Model Card.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_model_card_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_model_card_export_jobs.html)

```python
# list_model_card_export_jobs method definition

await def list_model_card_export_jobs(
    self,
    *,
    ModelCardName: str,
    ModelCardVersion: int = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    ModelCardExportJobNameContains: str = ...,
    StatusEquals: ModelCardExportJobStatusType = ...,  # (1)
    SortBy: ModelCardExportJobSortByType = ...,  # (2)
    SortOrder: ModelCardExportJobSortOrderType = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListModelCardExportJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelCardExportJobStatusType](./literals.md#modelcardexportjobstatustype) 
2. See [:material-code-brackets: ModelCardExportJobSortByType](./literals.md#modelcardexportjobsortbytype) 
3. See [:material-code-brackets: ModelCardExportJobSortOrderType](./literals.md#modelcardexportjobsortordertype) 
4. See [:material-code-braces: ListModelCardExportJobsResponseTypeDef](./type_defs.md#listmodelcardexportjobsresponsetypedef) 


```python
# list_model_card_export_jobs method usage example with argument unpacking

kwargs: ListModelCardExportJobsRequestTypeDef = {  # (1)
    "ModelCardName": ...,
}

parent.list_model_card_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListModelCardExportJobsRequestTypeDef](./type_defs.md#listmodelcardexportjobsrequesttypedef) 

### list\_model\_card\_versions

List existing versions of an Amazon SageMaker Model Card.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_model_card_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_model_card_versions.html)

```python
# list_model_card_versions method definition

await def list_model_card_versions(
    self,
    *,
    ModelCardName: str,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    ModelCardStatus: ModelCardStatusType = ...,  # (1)
    NextToken: str = ...,
    SortBy: ModelCardVersionSortByType = ...,  # (2)
    SortOrder: ModelCardSortOrderType = ...,  # (3)
) -> ListModelCardVersionsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-brackets: ModelCardVersionSortByType](./literals.md#modelcardversionsortbytype) 
3. See [:material-code-brackets: ModelCardSortOrderType](./literals.md#modelcardsortordertype) 
4. See [:material-code-braces: ListModelCardVersionsResponseTypeDef](./type_defs.md#listmodelcardversionsresponsetypedef) 


```python
# list_model_card_versions method usage example with argument unpacking

kwargs: ListModelCardVersionsRequestTypeDef = {  # (1)
    "ModelCardName": ...,
}

parent.list_model_card_versions(**kwargs)
```

1. See [:material-code-braces: ListModelCardVersionsRequestTypeDef](./type_defs.md#listmodelcardversionsrequesttypedef) 

### list\_model\_cards

List existing model cards.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_model_cards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_model_cards.html)

```python
# list_model_cards method definition

await def list_model_cards(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    ModelCardStatus: ModelCardStatusType = ...,  # (1)
    NextToken: str = ...,
    SortBy: ModelCardSortByType = ...,  # (2)
    SortOrder: ModelCardSortOrderType = ...,  # (3)
) -> ListModelCardsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-brackets: ModelCardSortByType](./literals.md#modelcardsortbytype) 
3. See [:material-code-brackets: ModelCardSortOrderType](./literals.md#modelcardsortordertype) 
4. See [:material-code-braces: ListModelCardsResponseTypeDef](./type_defs.md#listmodelcardsresponsetypedef) 


```python
# list_model_cards method usage example with argument unpacking

kwargs: ListModelCardsRequestTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_model_cards(**kwargs)
```

1. See [:material-code-braces: ListModelCardsRequestTypeDef](./type_defs.md#listmodelcardsrequesttypedef) 

### list\_model\_explainability\_job\_definitions

Lists model explainability job definitions that satisfy various filters.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_model_explainability_job_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_model_explainability_job_definitions.html)

```python
# list_model_explainability_job_definitions method definition

await def list_model_explainability_job_definitions(
    self,
    *,
    EndpointName: str = ...,
    SortBy: MonitoringJobDefinitionSortKeyType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
) -> ListModelExplainabilityJobDefinitionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListModelExplainabilityJobDefinitionsResponseTypeDef](./type_defs.md#listmodelexplainabilityjobdefinitionsresponsetypedef) 


```python
# list_model_explainability_job_definitions method usage example with argument unpacking

kwargs: ListModelExplainabilityJobDefinitionsRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.list_model_explainability_job_definitions(**kwargs)
```

1. See [:material-code-braces: ListModelExplainabilityJobDefinitionsRequestTypeDef](./type_defs.md#listmodelexplainabilityjobdefinitionsrequesttypedef) 

### list\_model\_metadata

Lists the domain, framework, task, and model name of standard machine learning
models found in common model zoos.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_model_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_model_metadata.html)

```python
# list_model_metadata method definition

await def list_model_metadata(
    self,
    *,
    SearchExpression: ModelMetadataSearchExpressionTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListModelMetadataResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ModelMetadataSearchExpressionTypeDef](./type_defs.md#modelmetadatasearchexpressiontypedef) 
2. See [:material-code-braces: ListModelMetadataResponseTypeDef](./type_defs.md#listmodelmetadataresponsetypedef) 


```python
# list_model_metadata method usage example with argument unpacking

kwargs: ListModelMetadataRequestTypeDef = {  # (1)
    "SearchExpression": ...,
}

parent.list_model_metadata(**kwargs)
```

1. See [:material-code-braces: ListModelMetadataRequestTypeDef](./type_defs.md#listmodelmetadatarequesttypedef) 

### list\_model\_package\_groups

Gets a list of the model groups in your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_model_package_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_model_package_groups.html)

```python
# list_model_package_groups method definition

await def list_model_package_groups(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    NextToken: str = ...,
    SortBy: ModelPackageGroupSortByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    CrossAccountFilterOption: CrossAccountFilterOptionType = ...,  # (3)
) -> ListModelPackageGroupsOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelPackageGroupSortByType](./literals.md#modelpackagegroupsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: CrossAccountFilterOptionType](./literals.md#crossaccountfilteroptiontype) 
4. See [:material-code-braces: ListModelPackageGroupsOutputTypeDef](./type_defs.md#listmodelpackagegroupsoutputtypedef) 


```python
# list_model_package_groups method usage example with argument unpacking

kwargs: ListModelPackageGroupsInputTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_model_package_groups(**kwargs)
```

1. See [:material-code-braces: ListModelPackageGroupsInputTypeDef](./type_defs.md#listmodelpackagegroupsinputtypedef) 

### list\_model\_packages

Lists the model packages that have been created.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_model_packages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_model_packages.html)

```python
# list_model_packages method definition

await def list_model_packages(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    ModelApprovalStatus: ModelApprovalStatusType = ...,  # (1)
    ModelPackageGroupName: str = ...,
    ModelPackageType: ModelPackageTypeType = ...,  # (2)
    NextToken: str = ...,
    SortBy: ModelPackageSortByType = ...,  # (3)
    SortOrder: SortOrderType = ...,  # (4)
) -> ListModelPackagesOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
2. See [:material-code-brackets: ModelPackageTypeType](./literals.md#modelpackagetypetype) 
3. See [:material-code-brackets: ModelPackageSortByType](./literals.md#modelpackagesortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: ListModelPackagesOutputTypeDef](./type_defs.md#listmodelpackagesoutputtypedef) 


```python
# list_model_packages method usage example with argument unpacking

kwargs: ListModelPackagesInputTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_model_packages(**kwargs)
```

1. See [:material-code-braces: ListModelPackagesInputTypeDef](./type_defs.md#listmodelpackagesinputtypedef) 

### list\_model\_quality\_job\_definitions

Gets a list of model quality monitoring job definitions in your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_model_quality_job_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_model_quality_job_definitions.html)

```python
# list_model_quality_job_definitions method definition

await def list_model_quality_job_definitions(
    self,
    *,
    EndpointName: str = ...,
    SortBy: MonitoringJobDefinitionSortKeyType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
) -> ListModelQualityJobDefinitionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListModelQualityJobDefinitionsResponseTypeDef](./type_defs.md#listmodelqualityjobdefinitionsresponsetypedef) 


```python
# list_model_quality_job_definitions method usage example with argument unpacking

kwargs: ListModelQualityJobDefinitionsRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.list_model_quality_job_definitions(**kwargs)
```

1. See [:material-code-braces: ListModelQualityJobDefinitionsRequestTypeDef](./type_defs.md#listmodelqualityjobdefinitionsrequesttypedef) 

### list\_models

Lists models created with the <code>CreateModel</code> API.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_models.html)

```python
# list_models method definition

await def list_models(
    self,
    *,
    SortBy: ModelSortKeyType = ...,  # (1)
    SortOrder: OrderKeyType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
) -> ListModelsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ModelSortKeyType](./literals.md#modelsortkeytype) 
2. See [:material-code-brackets: OrderKeyType](./literals.md#orderkeytype) 
3. See [:material-code-braces: ListModelsOutputTypeDef](./type_defs.md#listmodelsoutputtypedef) 


```python
# list_models method usage example with argument unpacking

kwargs: ListModelsInputTypeDef = {  # (1)
    "SortBy": ...,
}

parent.list_models(**kwargs)
```

1. See [:material-code-braces: ListModelsInputTypeDef](./type_defs.md#listmodelsinputtypedef) 

### list\_monitoring\_alert\_history

Gets a list of past alerts in a model monitoring schedule.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_monitoring_alert_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_monitoring_alert_history.html)

```python
# list_monitoring_alert_history method definition

await def list_monitoring_alert_history(
    self,
    *,
    MonitoringScheduleName: str = ...,
    MonitoringAlertName: str = ...,
    SortBy: MonitoringAlertHistorySortKeyType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    StatusEquals: MonitoringAlertStatusType = ...,  # (3)
) -> ListMonitoringAlertHistoryResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: MonitoringAlertHistorySortKeyType](./literals.md#monitoringalerthistorysortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: MonitoringAlertStatusType](./literals.md#monitoringalertstatustype) 
4. See [:material-code-braces: ListMonitoringAlertHistoryResponseTypeDef](./type_defs.md#listmonitoringalerthistoryresponsetypedef) 


```python
# list_monitoring_alert_history method usage example with argument unpacking

kwargs: ListMonitoringAlertHistoryRequestTypeDef = {  # (1)
    "MonitoringScheduleName": ...,
}

parent.list_monitoring_alert_history(**kwargs)
```

1. See [:material-code-braces: ListMonitoringAlertHistoryRequestTypeDef](./type_defs.md#listmonitoringalerthistoryrequesttypedef) 

### list\_monitoring\_alerts

Gets the alerts for a single monitoring schedule.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_monitoring_alerts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_monitoring_alerts.html)

```python
# list_monitoring_alerts method definition

await def list_monitoring_alerts(
    self,
    *,
    MonitoringScheduleName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMonitoringAlertsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMonitoringAlertsResponseTypeDef](./type_defs.md#listmonitoringalertsresponsetypedef) 


```python
# list_monitoring_alerts method usage example with argument unpacking

kwargs: ListMonitoringAlertsRequestTypeDef = {  # (1)
    "MonitoringScheduleName": ...,
}

parent.list_monitoring_alerts(**kwargs)
```

1. See [:material-code-braces: ListMonitoringAlertsRequestTypeDef](./type_defs.md#listmonitoringalertsrequesttypedef) 

### list\_monitoring\_executions

Returns list of all monitoring job executions.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_monitoring_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_monitoring_executions.html)

```python
# list_monitoring_executions method definition

await def list_monitoring_executions(
    self,
    *,
    MonitoringScheduleName: str = ...,
    EndpointName: str = ...,
    SortBy: MonitoringExecutionSortKeyType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    ScheduledTimeBefore: TimestampTypeDef = ...,
    ScheduledTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    StatusEquals: ExecutionStatusType = ...,  # (3)
    MonitoringJobDefinitionName: str = ...,
    MonitoringTypeEquals: MonitoringTypeType = ...,  # (4)
) -> ListMonitoringExecutionsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: MonitoringExecutionSortKeyType](./literals.md#monitoringexecutionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
4. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
5. See [:material-code-braces: ListMonitoringExecutionsResponseTypeDef](./type_defs.md#listmonitoringexecutionsresponsetypedef) 


```python
# list_monitoring_executions method usage example with argument unpacking

kwargs: ListMonitoringExecutionsRequestTypeDef = {  # (1)
    "MonitoringScheduleName": ...,
}

parent.list_monitoring_executions(**kwargs)
```

1. See [:material-code-braces: ListMonitoringExecutionsRequestTypeDef](./type_defs.md#listmonitoringexecutionsrequesttypedef) 

### list\_monitoring\_schedules

Returns list of all monitoring schedules.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_monitoring_schedules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_monitoring_schedules.html)

```python
# list_monitoring_schedules method definition

await def list_monitoring_schedules(
    self,
    *,
    EndpointName: str = ...,
    SortBy: MonitoringScheduleSortKeyType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    StatusEquals: ScheduleStatusType = ...,  # (3)
    MonitoringJobDefinitionName: str = ...,
    MonitoringTypeEquals: MonitoringTypeType = ...,  # (4)
) -> ListMonitoringSchedulesResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: MonitoringScheduleSortKeyType](./literals.md#monitoringschedulesortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ScheduleStatusType](./literals.md#schedulestatustype) 
4. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
5. See [:material-code-braces: ListMonitoringSchedulesResponseTypeDef](./type_defs.md#listmonitoringschedulesresponsetypedef) 


```python
# list_monitoring_schedules method usage example with argument unpacking

kwargs: ListMonitoringSchedulesRequestTypeDef = {  # (1)
    "EndpointName": ...,
}

parent.list_monitoring_schedules(**kwargs)
```

1. See [:material-code-braces: ListMonitoringSchedulesRequestTypeDef](./type_defs.md#listmonitoringschedulesrequesttypedef) 

### list\_notebook\_instance\_lifecycle\_configs

Lists notebook instance lifestyle configurations created with the <a
href="https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateNotebookInstanceLifecycleConfig.html">CreateNotebookInstanceLifecycleConfig</a>
API.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_notebook_instance_lifecycle_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_notebook_instance_lifecycle_configs.html)

```python
# list_notebook_instance_lifecycle_configs method definition

await def list_notebook_instance_lifecycle_configs(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    SortBy: NotebookInstanceLifecycleConfigSortKeyType = ...,  # (1)
    SortOrder: NotebookInstanceLifecycleConfigSortOrderType = ...,  # (2)
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
) -> ListNotebookInstanceLifecycleConfigsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: NotebookInstanceLifecycleConfigSortKeyType](./literals.md#notebookinstancelifecycleconfigsortkeytype) 
2. See [:material-code-brackets: NotebookInstanceLifecycleConfigSortOrderType](./literals.md#notebookinstancelifecycleconfigsortordertype) 
3. See [:material-code-braces: ListNotebookInstanceLifecycleConfigsOutputTypeDef](./type_defs.md#listnotebookinstancelifecycleconfigsoutputtypedef) 


```python
# list_notebook_instance_lifecycle_configs method usage example with argument unpacking

kwargs: ListNotebookInstanceLifecycleConfigsInputTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_notebook_instance_lifecycle_configs(**kwargs)
```

1. See [:material-code-braces: ListNotebookInstanceLifecycleConfigsInputTypeDef](./type_defs.md#listnotebookinstancelifecycleconfigsinputtypedef) 

### list\_notebook\_instances

Returns a list of the SageMaker AI notebook instances in the requester's
account in an Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_notebook_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_notebook_instances.html)

```python
# list_notebook_instances method definition

await def list_notebook_instances(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    SortBy: NotebookInstanceSortKeyType = ...,  # (1)
    SortOrder: NotebookInstanceSortOrderType = ...,  # (2)
    NameContains: str = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    StatusEquals: NotebookInstanceStatusType = ...,  # (3)
    NotebookInstanceLifecycleConfigNameContains: str = ...,
    DefaultCodeRepositoryContains: str = ...,
    AdditionalCodeRepositoryEquals: str = ...,
) -> ListNotebookInstancesOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: NotebookInstanceSortKeyType](./literals.md#notebookinstancesortkeytype) 
2. See [:material-code-brackets: NotebookInstanceSortOrderType](./literals.md#notebookinstancesortordertype) 
3. See [:material-code-brackets: NotebookInstanceStatusType](./literals.md#notebookinstancestatustype) 
4. See [:material-code-braces: ListNotebookInstancesOutputTypeDef](./type_defs.md#listnotebookinstancesoutputtypedef) 


```python
# list_notebook_instances method usage example with argument unpacking

kwargs: ListNotebookInstancesInputTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_notebook_instances(**kwargs)
```

1. See [:material-code-braces: ListNotebookInstancesInputTypeDef](./type_defs.md#listnotebookinstancesinputtypedef) 

### list\_optimization\_jobs

Lists the optimization jobs in your account and their properties.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_optimization_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_optimization_jobs.html)

```python
# list_optimization_jobs method definition

await def list_optimization_jobs(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    OptimizationContains: str = ...,
    NameContains: str = ...,
    StatusEquals: OptimizationJobStatusType = ...,  # (1)
    SortBy: ListOptimizationJobsSortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
) -> ListOptimizationJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: OptimizationJobStatusType](./literals.md#optimizationjobstatustype) 
2. See [:material-code-brackets: ListOptimizationJobsSortByType](./literals.md#listoptimizationjobssortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListOptimizationJobsResponseTypeDef](./type_defs.md#listoptimizationjobsresponsetypedef) 


```python
# list_optimization_jobs method usage example with argument unpacking

kwargs: ListOptimizationJobsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_optimization_jobs(**kwargs)
```

1. See [:material-code-braces: ListOptimizationJobsRequestTypeDef](./type_defs.md#listoptimizationjobsrequesttypedef) 

### list\_partner\_apps

Lists all of the SageMaker Partner AI Apps in an account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_partner_apps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_partner_apps.html)

```python
# list_partner_apps method definition

await def list_partner_apps(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPartnerAppsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPartnerAppsResponseTypeDef](./type_defs.md#listpartnerappsresponsetypedef) 


```python
# list_partner_apps method usage example with argument unpacking

kwargs: ListPartnerAppsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_partner_apps(**kwargs)
```

1. See [:material-code-braces: ListPartnerAppsRequestTypeDef](./type_defs.md#listpartnerappsrequesttypedef) 

### list\_pipeline\_execution\_steps

Gets a list of <code>PipeLineExecutionStep</code> objects.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_pipeline_execution_steps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_pipeline_execution_steps.html)

```python
# list_pipeline_execution_steps method definition

await def list_pipeline_execution_steps(
    self,
    *,
    PipelineExecutionArn: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    SortOrder: SortOrderType = ...,  # (1)
) -> ListPipelineExecutionStepsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: ListPipelineExecutionStepsResponseTypeDef](./type_defs.md#listpipelineexecutionstepsresponsetypedef) 


```python
# list_pipeline_execution_steps method usage example with argument unpacking

kwargs: ListPipelineExecutionStepsRequestTypeDef = {  # (1)
    "PipelineExecutionArn": ...,
}

parent.list_pipeline_execution_steps(**kwargs)
```

1. See [:material-code-braces: ListPipelineExecutionStepsRequestTypeDef](./type_defs.md#listpipelineexecutionstepsrequesttypedef) 

### list\_pipeline\_executions

Gets a list of the pipeline executions.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_pipeline_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_pipeline_executions.html)

```python
# list_pipeline_executions method definition

await def list_pipeline_executions(
    self,
    *,
    PipelineName: str,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    SortBy: SortPipelineExecutionsByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPipelineExecutionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortPipelineExecutionsByType](./literals.md#sortpipelineexecutionsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListPipelineExecutionsResponseTypeDef](./type_defs.md#listpipelineexecutionsresponsetypedef) 


```python
# list_pipeline_executions method usage example with argument unpacking

kwargs: ListPipelineExecutionsRequestTypeDef = {  # (1)
    "PipelineName": ...,
}

parent.list_pipeline_executions(**kwargs)
```

1. See [:material-code-braces: ListPipelineExecutionsRequestTypeDef](./type_defs.md#listpipelineexecutionsrequesttypedef) 

### list\_pipeline\_parameters\_for\_execution

Gets a list of parameters for a pipeline execution.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_pipeline_parameters_for_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_pipeline_parameters_for_execution.html)

```python
# list_pipeline_parameters_for_execution method definition

await def list_pipeline_parameters_for_execution(
    self,
    *,
    PipelineExecutionArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPipelineParametersForExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPipelineParametersForExecutionResponseTypeDef](./type_defs.md#listpipelineparametersforexecutionresponsetypedef) 


```python
# list_pipeline_parameters_for_execution method usage example with argument unpacking

kwargs: ListPipelineParametersForExecutionRequestTypeDef = {  # (1)
    "PipelineExecutionArn": ...,
}

parent.list_pipeline_parameters_for_execution(**kwargs)
```

1. See [:material-code-braces: ListPipelineParametersForExecutionRequestTypeDef](./type_defs.md#listpipelineparametersforexecutionrequesttypedef) 

### list\_pipelines

Gets a list of pipelines.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_pipelines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_pipelines.html)

```python
# list_pipelines method definition

await def list_pipelines(
    self,
    *,
    PipelineNamePrefix: str = ...,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    SortBy: SortPipelinesByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPipelinesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortPipelinesByType](./literals.md#sortpipelinesbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef) 


```python
# list_pipelines method usage example with argument unpacking

kwargs: ListPipelinesRequestTypeDef = {  # (1)
    "PipelineNamePrefix": ...,
}

parent.list_pipelines(**kwargs)
```

1. See [:material-code-braces: ListPipelinesRequestTypeDef](./type_defs.md#listpipelinesrequesttypedef) 

### list\_processing\_jobs

Lists processing jobs that satisfy various filters.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_processing_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_processing_jobs.html)

```python
# list_processing_jobs method definition

await def list_processing_jobs(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    StatusEquals: ProcessingJobStatusType = ...,  # (1)
    SortBy: SortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListProcessingJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ProcessingJobStatusType](./literals.md#processingjobstatustype) 
2. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListProcessingJobsResponseTypeDef](./type_defs.md#listprocessingjobsresponsetypedef) 


```python
# list_processing_jobs method usage example with argument unpacking

kwargs: ListProcessingJobsRequestTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_processing_jobs(**kwargs)
```

1. See [:material-code-braces: ListProcessingJobsRequestTypeDef](./type_defs.md#listprocessingjobsrequesttypedef) 

### list\_projects

Gets a list of the projects in an Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_projects` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_projects.html)

```python
# list_projects method definition

await def list_projects(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    MaxResults: int = ...,
    NameContains: str = ...,
    NextToken: str = ...,
    SortBy: ProjectSortByType = ...,  # (1)
    SortOrder: ProjectSortOrderType = ...,  # (2)
) -> ListProjectsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ProjectSortByType](./literals.md#projectsortbytype) 
2. See [:material-code-brackets: ProjectSortOrderType](./literals.md#projectsortordertype) 
3. See [:material-code-braces: ListProjectsOutputTypeDef](./type_defs.md#listprojectsoutputtypedef) 


```python
# list_projects method usage example with argument unpacking

kwargs: ListProjectsInputTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_projects(**kwargs)
```

1. See [:material-code-braces: ListProjectsInputTypeDef](./type_defs.md#listprojectsinputtypedef) 

### list\_resource\_catalogs

Lists Amazon SageMaker Catalogs based on given filters and orders.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_resource_catalogs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_resource_catalogs.html)

```python
# list_resource_catalogs method definition

await def list_resource_catalogs(
    self,
    *,
    NameContains: str = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    SortOrder: ResourceCatalogSortOrderType = ...,  # (1)
    SortBy: ResourceCatalogSortByType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListResourceCatalogsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceCatalogSortOrderType](./literals.md#resourcecatalogsortordertype) 
2. See [:material-code-brackets: ResourceCatalogSortByType](./literals.md#resourcecatalogsortbytype) 
3. See [:material-code-braces: ListResourceCatalogsResponseTypeDef](./type_defs.md#listresourcecatalogsresponsetypedef) 


```python
# list_resource_catalogs method usage example with argument unpacking

kwargs: ListResourceCatalogsRequestTypeDef = {  # (1)
    "NameContains": ...,
}

parent.list_resource_catalogs(**kwargs)
```

1. See [:material-code-braces: ListResourceCatalogsRequestTypeDef](./type_defs.md#listresourcecatalogsrequesttypedef) 

### list\_spaces

Lists spaces.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_spaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_spaces.html)

```python
# list_spaces method definition

await def list_spaces(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    SortOrder: SortOrderType = ...,  # (1)
    SortBy: SpaceSortKeyType = ...,  # (2)
    DomainIdEquals: str = ...,
    SpaceNameContains: str = ...,
) -> ListSpacesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: SpaceSortKeyType](./literals.md#spacesortkeytype) 
3. See [:material-code-braces: ListSpacesResponseTypeDef](./type_defs.md#listspacesresponsetypedef) 


```python
# list_spaces method usage example with argument unpacking

kwargs: ListSpacesRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_spaces(**kwargs)
```

1. See [:material-code-braces: ListSpacesRequestTypeDef](./type_defs.md#listspacesrequesttypedef) 

### list\_stage\_devices

Lists devices allocated to the stage, containing detailed device information
and deployment status.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_stage_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_stage_devices.html)

```python
# list_stage_devices method definition

await def list_stage_devices(
    self,
    *,
    EdgeDeploymentPlanName: str,
    StageName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    ExcludeDevicesDeployedInOtherStage: bool = ...,
) -> ListStageDevicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListStageDevicesResponseTypeDef](./type_defs.md#liststagedevicesresponsetypedef) 


```python
# list_stage_devices method usage example with argument unpacking

kwargs: ListStageDevicesRequestTypeDef = {  # (1)
    "EdgeDeploymentPlanName": ...,
    "StageName": ...,
}

parent.list_stage_devices(**kwargs)
```

1. See [:material-code-braces: ListStageDevicesRequestTypeDef](./type_defs.md#liststagedevicesrequesttypedef) 

### list\_studio\_lifecycle\_configs

Lists the Amazon SageMaker AI Studio Lifecycle Configurations in your Amazon
Web Services Account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_studio_lifecycle_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_studio_lifecycle_configs.html)

```python
# list_studio_lifecycle_configs method definition

await def list_studio_lifecycle_configs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    NameContains: str = ...,
    AppTypeEquals: StudioLifecycleConfigAppTypeType = ...,  # (1)
    CreationTimeBefore: TimestampTypeDef = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    ModifiedTimeBefore: TimestampTypeDef = ...,
    ModifiedTimeAfter: TimestampTypeDef = ...,
    SortBy: StudioLifecycleConfigSortKeyType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
) -> ListStudioLifecycleConfigsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: StudioLifecycleConfigAppTypeType](./literals.md#studiolifecycleconfigapptypetype) 
2. See [:material-code-brackets: StudioLifecycleConfigSortKeyType](./literals.md#studiolifecycleconfigsortkeytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListStudioLifecycleConfigsResponseTypeDef](./type_defs.md#liststudiolifecycleconfigsresponsetypedef) 


```python
# list_studio_lifecycle_configs method usage example with argument unpacking

kwargs: ListStudioLifecycleConfigsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_studio_lifecycle_configs(**kwargs)
```

1. See [:material-code-braces: ListStudioLifecycleConfigsRequestTypeDef](./type_defs.md#liststudiolifecycleconfigsrequesttypedef) 

### list\_subscribed\_workteams

Gets a list of the work teams that you are subscribed to in the Amazon Web
Services Marketplace.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_subscribed_workteams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_subscribed_workteams.html)

```python
# list_subscribed_workteams method definition

await def list_subscribed_workteams(
    self,
    *,
    NameContains: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSubscribedWorkteamsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSubscribedWorkteamsResponseTypeDef](./type_defs.md#listsubscribedworkteamsresponsetypedef) 


```python
# list_subscribed_workteams method usage example with argument unpacking

kwargs: ListSubscribedWorkteamsRequestTypeDef = {  # (1)
    "NameContains": ...,
}

parent.list_subscribed_workteams(**kwargs)
```

1. See [:material-code-braces: ListSubscribedWorkteamsRequestTypeDef](./type_defs.md#listsubscribedworkteamsrequesttypedef) 

### list\_tags

Returns the tags for the specified SageMaker resource.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_tags.html)

```python
# list_tags method definition

await def list_tags(
    self,
    *,
    ResourceArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTagsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsOutputTypeDef](./type_defs.md#listtagsoutputtypedef) 


```python
# list_tags method usage example with argument unpacking

kwargs: ListTagsInputTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags(**kwargs)
```

1. See [:material-code-braces: ListTagsInputTypeDef](./type_defs.md#listtagsinputtypedef) 

### list\_training\_jobs

Lists training jobs.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_training_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_training_jobs.html)

```python
# list_training_jobs method definition

await def list_training_jobs(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    StatusEquals: TrainingJobStatusType = ...,  # (1)
    SortBy: SortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    WarmPoolStatusEquals: WarmPoolResourceStatusType = ...,  # (4)
    TrainingPlanArnEquals: str = ...,
) -> ListTrainingJobsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: TrainingJobStatusType](./literals.md#trainingjobstatustype) 
2. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-brackets: WarmPoolResourceStatusType](./literals.md#warmpoolresourcestatustype) 
5. See [:material-code-braces: ListTrainingJobsResponseTypeDef](./type_defs.md#listtrainingjobsresponsetypedef) 


```python
# list_training_jobs method usage example with argument unpacking

kwargs: ListTrainingJobsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_training_jobs(**kwargs)
```

1. See [:material-code-braces: ListTrainingJobsRequestTypeDef](./type_defs.md#listtrainingjobsrequesttypedef) 

### list\_training\_jobs\_for\_hyper\_parameter\_tuning\_job

Gets a list of <a
href="https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TrainingJobSummary.html">TrainingJobSummary</a>
objects that describe the training jobs that a hyperparameter tuning job
launched.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_training_jobs_for_hyper_parameter_tuning_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_training_jobs_for_hyper_parameter_tuning_job.html)

```python
# list_training_jobs_for_hyper_parameter_tuning_job method definition

await def list_training_jobs_for_hyper_parameter_tuning_job(
    self,
    *,
    HyperParameterTuningJobName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    StatusEquals: TrainingJobStatusType = ...,  # (1)
    SortBy: TrainingJobSortByOptionsType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
) -> ListTrainingJobsForHyperParameterTuningJobResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: TrainingJobStatusType](./literals.md#trainingjobstatustype) 
2. See [:material-code-brackets: TrainingJobSortByOptionsType](./literals.md#trainingjobsortbyoptionstype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListTrainingJobsForHyperParameterTuningJobResponseTypeDef](./type_defs.md#listtrainingjobsforhyperparametertuningjobresponsetypedef) 


```python
# list_training_jobs_for_hyper_parameter_tuning_job method usage example with argument unpacking

kwargs: ListTrainingJobsForHyperParameterTuningJobRequestTypeDef = {  # (1)
    "HyperParameterTuningJobName": ...,
}

parent.list_training_jobs_for_hyper_parameter_tuning_job(**kwargs)
```

1. See [:material-code-braces: ListTrainingJobsForHyperParameterTuningJobRequestTypeDef](./type_defs.md#listtrainingjobsforhyperparametertuningjobrequesttypedef) 

### list\_training\_plans

Retrieves a list of training plans for the current account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_training_plans` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_training_plans.html)

```python
# list_training_plans method definition

await def list_training_plans(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    StartTimeAfter: TimestampTypeDef = ...,
    StartTimeBefore: TimestampTypeDef = ...,
    SortBy: TrainingPlanSortByType = ...,  # (1)
    SortOrder: TrainingPlanSortOrderType = ...,  # (2)
    Filters: Sequence[TrainingPlanFilterTypeDef] = ...,  # (3)
) -> ListTrainingPlansResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: TrainingPlanSortByType](./literals.md#trainingplansortbytype) 
2. See [:material-code-brackets: TrainingPlanSortOrderType](./literals.md#trainingplansortordertype) 
3. See [:material-code-braces: TrainingPlanFilterTypeDef](./type_defs.md#trainingplanfiltertypedef) 
4. See [:material-code-braces: ListTrainingPlansResponseTypeDef](./type_defs.md#listtrainingplansresponsetypedef) 


```python
# list_training_plans method usage example with argument unpacking

kwargs: ListTrainingPlansRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_training_plans(**kwargs)
```

1. See [:material-code-braces: ListTrainingPlansRequestTypeDef](./type_defs.md#listtrainingplansrequesttypedef) 

### list\_transform\_jobs

Lists transform jobs.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_transform_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_transform_jobs.html)

```python
# list_transform_jobs method definition

await def list_transform_jobs(
    self,
    *,
    CreationTimeAfter: TimestampTypeDef = ...,
    CreationTimeBefore: TimestampTypeDef = ...,
    LastModifiedTimeAfter: TimestampTypeDef = ...,
    LastModifiedTimeBefore: TimestampTypeDef = ...,
    NameContains: str = ...,
    StatusEquals: TransformJobStatusType = ...,  # (1)
    SortBy: SortByType = ...,  # (2)
    SortOrder: SortOrderType = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTransformJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: TransformJobStatusType](./literals.md#transformjobstatustype) 
2. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListTransformJobsResponseTypeDef](./type_defs.md#listtransformjobsresponsetypedef) 


```python
# list_transform_jobs method usage example with argument unpacking

kwargs: ListTransformJobsRequestTypeDef = {  # (1)
    "CreationTimeAfter": ...,
}

parent.list_transform_jobs(**kwargs)
```

1. See [:material-code-braces: ListTransformJobsRequestTypeDef](./type_defs.md#listtransformjobsrequesttypedef) 

### list\_trial\_components

Lists the trial components in your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_trial_components` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_trial_components.html)

```python
# list_trial_components method definition

await def list_trial_components(
    self,
    *,
    ExperimentName: str = ...,
    TrialName: str = ...,
    SourceArn: str = ...,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    SortBy: SortTrialComponentsByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTrialComponentsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortTrialComponentsByType](./literals.md#sorttrialcomponentsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListTrialComponentsResponseTypeDef](./type_defs.md#listtrialcomponentsresponsetypedef) 


```python
# list_trial_components method usage example with argument unpacking

kwargs: ListTrialComponentsRequestTypeDef = {  # (1)
    "ExperimentName": ...,
}

parent.list_trial_components(**kwargs)
```

1. See [:material-code-braces: ListTrialComponentsRequestTypeDef](./type_defs.md#listtrialcomponentsrequesttypedef) 

### list\_trials

Lists the trials in your account.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_trials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_trials.html)

```python
# list_trials method definition

await def list_trials(
    self,
    *,
    ExperimentName: str = ...,
    TrialComponentName: str = ...,
    CreatedAfter: TimestampTypeDef = ...,
    CreatedBefore: TimestampTypeDef = ...,
    SortBy: SortTrialsByType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTrialsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortTrialsByType](./literals.md#sorttrialsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListTrialsResponseTypeDef](./type_defs.md#listtrialsresponsetypedef) 


```python
# list_trials method usage example with argument unpacking

kwargs: ListTrialsRequestTypeDef = {  # (1)
    "ExperimentName": ...,
}

parent.list_trials(**kwargs)
```

1. See [:material-code-braces: ListTrialsRequestTypeDef](./type_defs.md#listtrialsrequesttypedef) 

### list\_user\_profiles

Lists user profiles.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_user_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_user_profiles.html)

```python
# list_user_profiles method definition

await def list_user_profiles(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    SortOrder: SortOrderType = ...,  # (1)
    SortBy: UserProfileSortKeyType = ...,  # (2)
    DomainIdEquals: str = ...,
    UserProfileNameContains: str = ...,
) -> ListUserProfilesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: UserProfileSortKeyType](./literals.md#userprofilesortkeytype) 
3. See [:material-code-braces: ListUserProfilesResponseTypeDef](./type_defs.md#listuserprofilesresponsetypedef) 


```python
# list_user_profiles method usage example with argument unpacking

kwargs: ListUserProfilesRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_user_profiles(**kwargs)
```

1. See [:material-code-braces: ListUserProfilesRequestTypeDef](./type_defs.md#listuserprofilesrequesttypedef) 

### list\_workforces

Use this operation to list all private and vendor workforces in an Amazon Web
Services Region.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_workforces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_workforces.html)

```python
# list_workforces method definition

await def list_workforces(
    self,
    *,
    SortBy: ListWorkforcesSortByOptionsType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NameContains: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListWorkforcesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ListWorkforcesSortByOptionsType](./literals.md#listworkforcessortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListWorkforcesResponseTypeDef](./type_defs.md#listworkforcesresponsetypedef) 


```python
# list_workforces method usage example with argument unpacking

kwargs: ListWorkforcesRequestTypeDef = {  # (1)
    "SortBy": ...,
}

parent.list_workforces(**kwargs)
```

1. See [:material-code-braces: ListWorkforcesRequestTypeDef](./type_defs.md#listworkforcesrequesttypedef) 

### list\_workteams

Gets a list of private work teams that you have defined in a region.

Type annotations and code completion for `#!python session.create_client("sagemaker").list_workteams` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/list_workteams.html)

```python
# list_workteams method definition

await def list_workteams(
    self,
    *,
    SortBy: ListWorkteamsSortByOptionsType = ...,  # (1)
    SortOrder: SortOrderType = ...,  # (2)
    NameContains: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListWorkteamsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ListWorkteamsSortByOptionsType](./literals.md#listworkteamssortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListWorkteamsResponseTypeDef](./type_defs.md#listworkteamsresponsetypedef) 


```python
# list_workteams method usage example with argument unpacking

kwargs: ListWorkteamsRequestTypeDef = {  # (1)
    "SortBy": ...,
}

parent.list_workteams(**kwargs)
```

1. See [:material-code-braces: ListWorkteamsRequestTypeDef](./type_defs.md#listworkteamsrequesttypedef) 

### put\_model\_package\_group\_policy

Adds a resouce policy to control access to a model group.

Type annotations and code completion for `#!python session.create_client("sagemaker").put_model_package_group_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/put_model_package_group_policy.html)

```python
# put_model_package_group_policy method definition

await def put_model_package_group_policy(
    self,
    *,
    ModelPackageGroupName: str,
    ResourcePolicy: str,
) -> PutModelPackageGroupPolicyOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutModelPackageGroupPolicyOutputTypeDef](./type_defs.md#putmodelpackagegrouppolicyoutputtypedef) 


```python
# put_model_package_group_policy method usage example with argument unpacking

kwargs: PutModelPackageGroupPolicyInputTypeDef = {  # (1)
    "ModelPackageGroupName": ...,
    "ResourcePolicy": ...,
}

parent.put_model_package_group_policy(**kwargs)
```

1. See [:material-code-braces: PutModelPackageGroupPolicyInputTypeDef](./type_defs.md#putmodelpackagegrouppolicyinputtypedef) 

### query\_lineage

Use this action to inspect your lineage and discover relationships between
entities.

Type annotations and code completion for `#!python session.create_client("sagemaker").query_lineage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/query_lineage.html)

```python
# query_lineage method definition

await def query_lineage(
    self,
    *,
    StartArns: Sequence[str] = ...,
    Direction: DirectionType = ...,  # (1)
    IncludeEdges: bool = ...,
    Filters: QueryFiltersTypeDef = ...,  # (2)
    MaxDepth: int = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> QueryLineageResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DirectionType](./literals.md#directiontype) 
2. See [:material-code-braces: QueryFiltersTypeDef](./type_defs.md#queryfilterstypedef) 
3. See [:material-code-braces: QueryLineageResponseTypeDef](./type_defs.md#querylineageresponsetypedef) 


```python
# query_lineage method usage example with argument unpacking

kwargs: QueryLineageRequestTypeDef = {  # (1)
    "StartArns": ...,
}

parent.query_lineage(**kwargs)
```

1. See [:material-code-braces: QueryLineageRequestTypeDef](./type_defs.md#querylineagerequesttypedef) 

### register\_devices

Register devices.

Type annotations and code completion for `#!python session.create_client("sagemaker").register_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/register_devices.html)

```python
# register_devices method definition

await def register_devices(
    self,
    *,
    DeviceFleetName: str,
    Devices: Sequence[DeviceTypeDef],  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# register_devices method usage example with argument unpacking

kwargs: RegisterDevicesRequestTypeDef = {  # (1)
    "DeviceFleetName": ...,
    "Devices": ...,
}

parent.register_devices(**kwargs)
```

1. See [:material-code-braces: RegisterDevicesRequestTypeDef](./type_defs.md#registerdevicesrequesttypedef) 

### render\_ui\_template

Renders the UI template so that you can preview the worker's experience.

Type annotations and code completion for `#!python session.create_client("sagemaker").render_ui_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/render_ui_template.html)

```python
# render_ui_template method definition

await def render_ui_template(
    self,
    *,
    Task: RenderableTaskTypeDef,  # (1)
    RoleArn: str,
    UiTemplate: UiTemplateTypeDef = ...,  # (2)
    HumanTaskUiArn: str = ...,
) -> RenderUiTemplateResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RenderableTaskTypeDef](./type_defs.md#renderabletasktypedef) 
2. See [:material-code-braces: UiTemplateTypeDef](./type_defs.md#uitemplatetypedef) 
3. See [:material-code-braces: RenderUiTemplateResponseTypeDef](./type_defs.md#renderuitemplateresponsetypedef) 


```python
# render_ui_template method usage example with argument unpacking

kwargs: RenderUiTemplateRequestTypeDef = {  # (1)
    "Task": ...,
    "RoleArn": ...,
}

parent.render_ui_template(**kwargs)
```

1. See [:material-code-braces: RenderUiTemplateRequestTypeDef](./type_defs.md#renderuitemplaterequesttypedef) 

### retry\_pipeline\_execution

Retry the execution of the pipeline.

Type annotations and code completion for `#!python session.create_client("sagemaker").retry_pipeline_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/retry_pipeline_execution.html)

```python
# retry_pipeline_execution method definition

await def retry_pipeline_execution(
    self,
    *,
    PipelineExecutionArn: str,
    ClientRequestToken: str,
    ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,  # (1)
) -> RetryPipelineExecutionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
2. See [:material-code-braces: RetryPipelineExecutionResponseTypeDef](./type_defs.md#retrypipelineexecutionresponsetypedef) 


```python
# retry_pipeline_execution method usage example with argument unpacking

kwargs: RetryPipelineExecutionRequestTypeDef = {  # (1)
    "PipelineExecutionArn": ...,
    "ClientRequestToken": ...,
}

parent.retry_pipeline_execution(**kwargs)
```

1. See [:material-code-braces: RetryPipelineExecutionRequestTypeDef](./type_defs.md#retrypipelineexecutionrequesttypedef) 

### search

Finds SageMaker resources that match a search query.

Type annotations and code completion for `#!python session.create_client("sagemaker").search` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/search.html)

```python
# search method definition

await def search(
    self,
    *,
    Resource: ResourceTypeType,  # (1)
    SearchExpression: SearchExpressionTypeDef = ...,  # (2)
    SortBy: str = ...,
    SortOrder: SearchSortOrderType = ...,  # (3)
    NextToken: str = ...,
    MaxResults: int = ...,
    CrossAccountFilterOption: CrossAccountFilterOptionType = ...,  # (4)
    VisibilityConditions: Sequence[VisibilityConditionsTypeDef] = ...,  # (5)
) -> SearchResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
3. See [:material-code-brackets: SearchSortOrderType](./literals.md#searchsortordertype) 
4. See [:material-code-brackets: CrossAccountFilterOptionType](./literals.md#crossaccountfilteroptiontype) 
5. See [:material-code-braces: VisibilityConditionsTypeDef](./type_defs.md#visibilityconditionstypedef) 
6. See [:material-code-braces: SearchResponseTypeDef](./type_defs.md#searchresponsetypedef) 


```python
# search method usage example with argument unpacking

kwargs: SearchRequestTypeDef = {  # (1)
    "Resource": ...,
}

parent.search(**kwargs)
```

1. See [:material-code-braces: SearchRequestTypeDef](./type_defs.md#searchrequesttypedef) 

### search\_training\_plan\_offerings

Searches for available training plan offerings based on specified criteria.

Type annotations and code completion for `#!python session.create_client("sagemaker").search_training_plan_offerings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/search_training_plan_offerings.html)

```python
# search_training_plan_offerings method definition

await def search_training_plan_offerings(
    self,
    *,
    InstanceType: ReservedCapacityInstanceTypeType,  # (1)
    InstanceCount: int,
    TargetResources: Sequence[SageMakerResourceNameType],  # (2)
    StartTimeAfter: TimestampTypeDef = ...,
    EndTimeBefore: TimestampTypeDef = ...,
    DurationHours: int = ...,
) -> SearchTrainingPlanOfferingsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ReservedCapacityInstanceTypeType](./literals.md#reservedcapacityinstancetypetype) 
2. See [:material-code-brackets: SageMakerResourceNameType](./literals.md#sagemakerresourcenametype) 
3. See [:material-code-braces: SearchTrainingPlanOfferingsResponseTypeDef](./type_defs.md#searchtrainingplanofferingsresponsetypedef) 


```python
# search_training_plan_offerings method usage example with argument unpacking

kwargs: SearchTrainingPlanOfferingsRequestTypeDef = {  # (1)
    "InstanceType": ...,
    "InstanceCount": ...,
    "TargetResources": ...,
}

parent.search_training_plan_offerings(**kwargs)
```

1. See [:material-code-braces: SearchTrainingPlanOfferingsRequestTypeDef](./type_defs.md#searchtrainingplanofferingsrequesttypedef) 

### send\_pipeline\_execution\_step\_failure

Notifies the pipeline that the execution of a callback step failed, along with
a message describing why.

Type annotations and code completion for `#!python session.create_client("sagemaker").send_pipeline_execution_step_failure` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/send_pipeline_execution_step_failure.html)

```python
# send_pipeline_execution_step_failure method definition

await def send_pipeline_execution_step_failure(
    self,
    *,
    CallbackToken: str,
    FailureReason: str = ...,
    ClientRequestToken: str = ...,
) -> SendPipelineExecutionStepFailureResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SendPipelineExecutionStepFailureResponseTypeDef](./type_defs.md#sendpipelineexecutionstepfailureresponsetypedef) 


```python
# send_pipeline_execution_step_failure method usage example with argument unpacking

kwargs: SendPipelineExecutionStepFailureRequestTypeDef = {  # (1)
    "CallbackToken": ...,
}

parent.send_pipeline_execution_step_failure(**kwargs)
```

1. See [:material-code-braces: SendPipelineExecutionStepFailureRequestTypeDef](./type_defs.md#sendpipelineexecutionstepfailurerequesttypedef) 

### send\_pipeline\_execution\_step\_success

Notifies the pipeline that the execution of a callback step succeeded and
provides a list of the step's output parameters.

Type annotations and code completion for `#!python session.create_client("sagemaker").send_pipeline_execution_step_success` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/send_pipeline_execution_step_success.html)

```python
# send_pipeline_execution_step_success method definition

await def send_pipeline_execution_step_success(
    self,
    *,
    CallbackToken: str,
    OutputParameters: Sequence[OutputParameterTypeDef] = ...,  # (1)
    ClientRequestToken: str = ...,
) -> SendPipelineExecutionStepSuccessResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OutputParameterTypeDef](./type_defs.md#outputparametertypedef) 
2. See [:material-code-braces: SendPipelineExecutionStepSuccessResponseTypeDef](./type_defs.md#sendpipelineexecutionstepsuccessresponsetypedef) 


```python
# send_pipeline_execution_step_success method usage example with argument unpacking

kwargs: SendPipelineExecutionStepSuccessRequestTypeDef = {  # (1)
    "CallbackToken": ...,
}

parent.send_pipeline_execution_step_success(**kwargs)
```

1. See [:material-code-braces: SendPipelineExecutionStepSuccessRequestTypeDef](./type_defs.md#sendpipelineexecutionstepsuccessrequesttypedef) 

### start\_edge\_deployment\_stage

Starts a stage in an edge deployment plan.

Type annotations and code completion for `#!python session.create_client("sagemaker").start_edge_deployment_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/start_edge_deployment_stage.html)

```python
# start_edge_deployment_stage method definition

await def start_edge_deployment_stage(
    self,
    *,
    EdgeDeploymentPlanName: str,
    StageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_edge_deployment_stage method usage example with argument unpacking

kwargs: StartEdgeDeploymentStageRequestTypeDef = {  # (1)
    "EdgeDeploymentPlanName": ...,
    "StageName": ...,
}

parent.start_edge_deployment_stage(**kwargs)
```

1. See [:material-code-braces: StartEdgeDeploymentStageRequestTypeDef](./type_defs.md#startedgedeploymentstagerequesttypedef) 

### start\_inference\_experiment

Starts an inference experiment.

Type annotations and code completion for `#!python session.create_client("sagemaker").start_inference_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/start_inference_experiment.html)

```python
# start_inference_experiment method definition

await def start_inference_experiment(
    self,
    *,
    Name: str,
) -> StartInferenceExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartInferenceExperimentResponseTypeDef](./type_defs.md#startinferenceexperimentresponsetypedef) 


```python
# start_inference_experiment method usage example with argument unpacking

kwargs: StartInferenceExperimentRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.start_inference_experiment(**kwargs)
```

1. See [:material-code-braces: StartInferenceExperimentRequestTypeDef](./type_defs.md#startinferenceexperimentrequesttypedef) 

### start\_mlflow\_tracking\_server

Programmatically start an MLflow Tracking Server.

Type annotations and code completion for `#!python session.create_client("sagemaker").start_mlflow_tracking_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/start_mlflow_tracking_server.html)

```python
# start_mlflow_tracking_server method definition

await def start_mlflow_tracking_server(
    self,
    *,
    TrackingServerName: str,
) -> StartMlflowTrackingServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMlflowTrackingServerResponseTypeDef](./type_defs.md#startmlflowtrackingserverresponsetypedef) 


```python
# start_mlflow_tracking_server method usage example with argument unpacking

kwargs: StartMlflowTrackingServerRequestTypeDef = {  # (1)
    "TrackingServerName": ...,
}

parent.start_mlflow_tracking_server(**kwargs)
```

1. See [:material-code-braces: StartMlflowTrackingServerRequestTypeDef](./type_defs.md#startmlflowtrackingserverrequesttypedef) 

### start\_monitoring\_schedule

Starts a previously stopped monitoring schedule.

Type annotations and code completion for `#!python session.create_client("sagemaker").start_monitoring_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/start_monitoring_schedule.html)

```python
# start_monitoring_schedule method definition

await def start_monitoring_schedule(
    self,
    *,
    MonitoringScheduleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_monitoring_schedule method usage example with argument unpacking

kwargs: StartMonitoringScheduleRequestTypeDef = {  # (1)
    "MonitoringScheduleName": ...,
}

parent.start_monitoring_schedule(**kwargs)
```

1. See [:material-code-braces: StartMonitoringScheduleRequestTypeDef](./type_defs.md#startmonitoringschedulerequesttypedef) 

### start\_notebook\_instance

Launches an ML compute instance with the latest version of the libraries and
attaches your ML storage volume.

Type annotations and code completion for `#!python session.create_client("sagemaker").start_notebook_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/start_notebook_instance.html)

```python
# start_notebook_instance method definition

await def start_notebook_instance(
    self,
    *,
    NotebookInstanceName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_notebook_instance method usage example with argument unpacking

kwargs: StartNotebookInstanceInputTypeDef = {  # (1)
    "NotebookInstanceName": ...,
}

parent.start_notebook_instance(**kwargs)
```

1. See [:material-code-braces: StartNotebookInstanceInputTypeDef](./type_defs.md#startnotebookinstanceinputtypedef) 

### start\_pipeline\_execution

Starts a pipeline execution.

Type annotations and code completion for `#!python session.create_client("sagemaker").start_pipeline_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/start_pipeline_execution.html)

```python
# start_pipeline_execution method definition

await def start_pipeline_execution(
    self,
    *,
    PipelineName: str,
    ClientRequestToken: str,
    PipelineExecutionDisplayName: str = ...,
    PipelineParameters: Sequence[ParameterTypeDef] = ...,  # (1)
    PipelineExecutionDescription: str = ...,
    ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,  # (2)
    SelectiveExecutionConfig: SelectiveExecutionConfigUnionTypeDef = ...,  # (3)
) -> StartPipelineExecutionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
3. See [:material-code-braces: SelectiveExecutionConfigTypeDef](./type_defs.md#selectiveexecutionconfigtypedef) [:material-code-braces: SelectiveExecutionConfigOutputTypeDef](./type_defs.md#selectiveexecutionconfigoutputtypedef) 
4. See [:material-code-braces: StartPipelineExecutionResponseTypeDef](./type_defs.md#startpipelineexecutionresponsetypedef) 


```python
# start_pipeline_execution method usage example with argument unpacking

kwargs: StartPipelineExecutionRequestTypeDef = {  # (1)
    "PipelineName": ...,
    "ClientRequestToken": ...,
}

parent.start_pipeline_execution(**kwargs)
```

1. See [:material-code-braces: StartPipelineExecutionRequestTypeDef](./type_defs.md#startpipelineexecutionrequesttypedef) 

### stop\_auto\_ml\_job

A method for forcing a running job to shut down.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_auto_ml_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_auto_ml_job.html)

```python
# stop_auto_ml_job method definition

await def stop_auto_ml_job(
    self,
    *,
    AutoMLJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_auto_ml_job method usage example with argument unpacking

kwargs: StopAutoMLJobRequestTypeDef = {  # (1)
    "AutoMLJobName": ...,
}

parent.stop_auto_ml_job(**kwargs)
```

1. See [:material-code-braces: StopAutoMLJobRequestTypeDef](./type_defs.md#stopautomljobrequesttypedef) 

### stop\_compilation\_job

Stops a model compilation job.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_compilation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_compilation_job.html)

```python
# stop_compilation_job method definition

await def stop_compilation_job(
    self,
    *,
    CompilationJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_compilation_job method usage example with argument unpacking

kwargs: StopCompilationJobRequestTypeDef = {  # (1)
    "CompilationJobName": ...,
}

parent.stop_compilation_job(**kwargs)
```

1. See [:material-code-braces: StopCompilationJobRequestTypeDef](./type_defs.md#stopcompilationjobrequesttypedef) 

### stop\_edge\_deployment\_stage

Stops a stage in an edge deployment plan.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_edge_deployment_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_edge_deployment_stage.html)

```python
# stop_edge_deployment_stage method definition

await def stop_edge_deployment_stage(
    self,
    *,
    EdgeDeploymentPlanName: str,
    StageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_edge_deployment_stage method usage example with argument unpacking

kwargs: StopEdgeDeploymentStageRequestTypeDef = {  # (1)
    "EdgeDeploymentPlanName": ...,
    "StageName": ...,
}

parent.stop_edge_deployment_stage(**kwargs)
```

1. See [:material-code-braces: StopEdgeDeploymentStageRequestTypeDef](./type_defs.md#stopedgedeploymentstagerequesttypedef) 

### stop\_edge\_packaging\_job

Request to stop an edge packaging job.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_edge_packaging_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_edge_packaging_job.html)

```python
# stop_edge_packaging_job method definition

await def stop_edge_packaging_job(
    self,
    *,
    EdgePackagingJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_edge_packaging_job method usage example with argument unpacking

kwargs: StopEdgePackagingJobRequestTypeDef = {  # (1)
    "EdgePackagingJobName": ...,
}

parent.stop_edge_packaging_job(**kwargs)
```

1. See [:material-code-braces: StopEdgePackagingJobRequestTypeDef](./type_defs.md#stopedgepackagingjobrequesttypedef) 

### stop\_hyper\_parameter\_tuning\_job

Stops a running hyperparameter tuning job and all running training jobs that
the tuning job launched.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_hyper_parameter_tuning_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_hyper_parameter_tuning_job.html)

```python
# stop_hyper_parameter_tuning_job method definition

await def stop_hyper_parameter_tuning_job(
    self,
    *,
    HyperParameterTuningJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_hyper_parameter_tuning_job method usage example with argument unpacking

kwargs: StopHyperParameterTuningJobRequestTypeDef = {  # (1)
    "HyperParameterTuningJobName": ...,
}

parent.stop_hyper_parameter_tuning_job(**kwargs)
```

1. See [:material-code-braces: StopHyperParameterTuningJobRequestTypeDef](./type_defs.md#stophyperparametertuningjobrequesttypedef) 

### stop\_inference\_experiment

Stops an inference experiment.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_inference_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_inference_experiment.html)

```python
# stop_inference_experiment method definition

await def stop_inference_experiment(
    self,
    *,
    Name: str,
    ModelVariantActions: Mapping[str, ModelVariantActionType],  # (1)
    DesiredModelVariants: Sequence[ModelVariantConfigTypeDef] = ...,  # (2)
    DesiredState: InferenceExperimentStopDesiredStateType = ...,  # (3)
    Reason: str = ...,
) -> StopInferenceExperimentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelVariantActionType](./literals.md#modelvariantactiontype) 
2. See [:material-code-braces: ModelVariantConfigTypeDef](./type_defs.md#modelvariantconfigtypedef) 
3. See [:material-code-brackets: InferenceExperimentStopDesiredStateType](./literals.md#inferenceexperimentstopdesiredstatetype) 
4. See [:material-code-braces: StopInferenceExperimentResponseTypeDef](./type_defs.md#stopinferenceexperimentresponsetypedef) 


```python
# stop_inference_experiment method usage example with argument unpacking

kwargs: StopInferenceExperimentRequestTypeDef = {  # (1)
    "Name": ...,
    "ModelVariantActions": ...,
}

parent.stop_inference_experiment(**kwargs)
```

1. See [:material-code-braces: StopInferenceExperimentRequestTypeDef](./type_defs.md#stopinferenceexperimentrequesttypedef) 

### stop\_inference\_recommendations\_job

Stops an Inference Recommender job.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_inference_recommendations_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_inference_recommendations_job.html)

```python
# stop_inference_recommendations_job method definition

await def stop_inference_recommendations_job(
    self,
    *,
    JobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_inference_recommendations_job method usage example with argument unpacking

kwargs: StopInferenceRecommendationsJobRequestTypeDef = {  # (1)
    "JobName": ...,
}

parent.stop_inference_recommendations_job(**kwargs)
```

1. See [:material-code-braces: StopInferenceRecommendationsJobRequestTypeDef](./type_defs.md#stopinferencerecommendationsjobrequesttypedef) 

### stop\_labeling\_job

Stops a running labeling job.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_labeling_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_labeling_job.html)

```python
# stop_labeling_job method definition

await def stop_labeling_job(
    self,
    *,
    LabelingJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_labeling_job method usage example with argument unpacking

kwargs: StopLabelingJobRequestTypeDef = {  # (1)
    "LabelingJobName": ...,
}

parent.stop_labeling_job(**kwargs)
```

1. See [:material-code-braces: StopLabelingJobRequestTypeDef](./type_defs.md#stoplabelingjobrequesttypedef) 

### stop\_mlflow\_tracking\_server

Programmatically stop an MLflow Tracking Server.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_mlflow_tracking_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_mlflow_tracking_server.html)

```python
# stop_mlflow_tracking_server method definition

await def stop_mlflow_tracking_server(
    self,
    *,
    TrackingServerName: str,
) -> StopMlflowTrackingServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopMlflowTrackingServerResponseTypeDef](./type_defs.md#stopmlflowtrackingserverresponsetypedef) 


```python
# stop_mlflow_tracking_server method usage example with argument unpacking

kwargs: StopMlflowTrackingServerRequestTypeDef = {  # (1)
    "TrackingServerName": ...,
}

parent.stop_mlflow_tracking_server(**kwargs)
```

1. See [:material-code-braces: StopMlflowTrackingServerRequestTypeDef](./type_defs.md#stopmlflowtrackingserverrequesttypedef) 

### stop\_monitoring\_schedule

Stops a previously started monitoring schedule.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_monitoring_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_monitoring_schedule.html)

```python
# stop_monitoring_schedule method definition

await def stop_monitoring_schedule(
    self,
    *,
    MonitoringScheduleName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_monitoring_schedule method usage example with argument unpacking

kwargs: StopMonitoringScheduleRequestTypeDef = {  # (1)
    "MonitoringScheduleName": ...,
}

parent.stop_monitoring_schedule(**kwargs)
```

1. See [:material-code-braces: StopMonitoringScheduleRequestTypeDef](./type_defs.md#stopmonitoringschedulerequesttypedef) 

### stop\_notebook\_instance

Terminates the ML compute instance.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_notebook_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_notebook_instance.html)

```python
# stop_notebook_instance method definition

await def stop_notebook_instance(
    self,
    *,
    NotebookInstanceName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_notebook_instance method usage example with argument unpacking

kwargs: StopNotebookInstanceInputTypeDef = {  # (1)
    "NotebookInstanceName": ...,
}

parent.stop_notebook_instance(**kwargs)
```

1. See [:material-code-braces: StopNotebookInstanceInputTypeDef](./type_defs.md#stopnotebookinstanceinputtypedef) 

### stop\_optimization\_job

Ends a running inference optimization job.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_optimization_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_optimization_job.html)

```python
# stop_optimization_job method definition

await def stop_optimization_job(
    self,
    *,
    OptimizationJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_optimization_job method usage example with argument unpacking

kwargs: StopOptimizationJobRequestTypeDef = {  # (1)
    "OptimizationJobName": ...,
}

parent.stop_optimization_job(**kwargs)
```

1. See [:material-code-braces: StopOptimizationJobRequestTypeDef](./type_defs.md#stopoptimizationjobrequesttypedef) 

### stop\_pipeline\_execution

Stops a pipeline execution.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_pipeline_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_pipeline_execution.html)

```python
# stop_pipeline_execution method definition

await def stop_pipeline_execution(
    self,
    *,
    PipelineExecutionArn: str,
    ClientRequestToken: str,
) -> StopPipelineExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopPipelineExecutionResponseTypeDef](./type_defs.md#stoppipelineexecutionresponsetypedef) 


```python
# stop_pipeline_execution method usage example with argument unpacking

kwargs: StopPipelineExecutionRequestTypeDef = {  # (1)
    "PipelineExecutionArn": ...,
    "ClientRequestToken": ...,
}

parent.stop_pipeline_execution(**kwargs)
```

1. See [:material-code-braces: StopPipelineExecutionRequestTypeDef](./type_defs.md#stoppipelineexecutionrequesttypedef) 

### stop\_processing\_job

Stops a processing job.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_processing_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_processing_job.html)

```python
# stop_processing_job method definition

await def stop_processing_job(
    self,
    *,
    ProcessingJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_processing_job method usage example with argument unpacking

kwargs: StopProcessingJobRequestTypeDef = {  # (1)
    "ProcessingJobName": ...,
}

parent.stop_processing_job(**kwargs)
```

1. See [:material-code-braces: StopProcessingJobRequestTypeDef](./type_defs.md#stopprocessingjobrequesttypedef) 

### stop\_training\_job

Stops a training job.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_training_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_training_job.html)

```python
# stop_training_job method definition

await def stop_training_job(
    self,
    *,
    TrainingJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_training_job method usage example with argument unpacking

kwargs: StopTrainingJobRequestTypeDef = {  # (1)
    "TrainingJobName": ...,
}

parent.stop_training_job(**kwargs)
```

1. See [:material-code-braces: StopTrainingJobRequestTypeDef](./type_defs.md#stoptrainingjobrequesttypedef) 

### stop\_transform\_job

Stops a batch transform job.

Type annotations and code completion for `#!python session.create_client("sagemaker").stop_transform_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/stop_transform_job.html)

```python
# stop_transform_job method definition

await def stop_transform_job(
    self,
    *,
    TransformJobName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_transform_job method usage example with argument unpacking

kwargs: StopTransformJobRequestTypeDef = {  # (1)
    "TransformJobName": ...,
}

parent.stop_transform_job(**kwargs)
```

1. See [:material-code-braces: StopTransformJobRequestTypeDef](./type_defs.md#stoptransformjobrequesttypedef) 

### update\_action

Updates an action.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_action.html)

```python
# update_action method definition

await def update_action(
    self,
    *,
    ActionName: str,
    Description: str = ...,
    Status: ActionStatusType = ...,  # (1)
    Properties: Mapping[str, str] = ...,
    PropertiesToRemove: Sequence[str] = ...,
) -> UpdateActionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
2. See [:material-code-braces: UpdateActionResponseTypeDef](./type_defs.md#updateactionresponsetypedef) 


```python
# update_action method usage example with argument unpacking

kwargs: UpdateActionRequestTypeDef = {  # (1)
    "ActionName": ...,
}

parent.update_action(**kwargs)
```

1. See [:material-code-braces: UpdateActionRequestTypeDef](./type_defs.md#updateactionrequesttypedef) 

### update\_app\_image\_config

Updates the properties of an AppImageConfig.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_app_image_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_app_image_config.html)

```python
# update_app_image_config method definition

await def update_app_image_config(
    self,
    *,
    AppImageConfigName: str,
    KernelGatewayImageConfig: KernelGatewayImageConfigUnionTypeDef = ...,  # (1)
    JupyterLabAppImageConfig: JupyterLabAppImageConfigUnionTypeDef = ...,  # (2)
    CodeEditorAppImageConfig: CodeEditorAppImageConfigUnionTypeDef = ...,  # (3)
) -> UpdateAppImageConfigResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: KernelGatewayImageConfigTypeDef](./type_defs.md#kernelgatewayimageconfigtypedef) [:material-code-braces: KernelGatewayImageConfigOutputTypeDef](./type_defs.md#kernelgatewayimageconfigoutputtypedef) 
2. See [:material-code-braces: JupyterLabAppImageConfigTypeDef](./type_defs.md#jupyterlabappimageconfigtypedef) [:material-code-braces: JupyterLabAppImageConfigOutputTypeDef](./type_defs.md#jupyterlabappimageconfigoutputtypedef) 
3. See [:material-code-braces: CodeEditorAppImageConfigTypeDef](./type_defs.md#codeeditorappimageconfigtypedef) [:material-code-braces: CodeEditorAppImageConfigOutputTypeDef](./type_defs.md#codeeditorappimageconfigoutputtypedef) 
4. See [:material-code-braces: UpdateAppImageConfigResponseTypeDef](./type_defs.md#updateappimageconfigresponsetypedef) 


```python
# update_app_image_config method usage example with argument unpacking

kwargs: UpdateAppImageConfigRequestTypeDef = {  # (1)
    "AppImageConfigName": ...,
}

parent.update_app_image_config(**kwargs)
```

1. See [:material-code-braces: UpdateAppImageConfigRequestTypeDef](./type_defs.md#updateappimageconfigrequesttypedef) 

### update\_artifact

Updates an artifact.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_artifact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_artifact.html)

```python
# update_artifact method definition

await def update_artifact(
    self,
    *,
    ArtifactArn: str,
    ArtifactName: str = ...,
    Properties: Mapping[str, str] = ...,
    PropertiesToRemove: Sequence[str] = ...,
) -> UpdateArtifactResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateArtifactResponseTypeDef](./type_defs.md#updateartifactresponsetypedef) 


```python
# update_artifact method usage example with argument unpacking

kwargs: UpdateArtifactRequestTypeDef = {  # (1)
    "ArtifactArn": ...,
}

parent.update_artifact(**kwargs)
```

1. See [:material-code-braces: UpdateArtifactRequestTypeDef](./type_defs.md#updateartifactrequesttypedef) 

### update\_cluster

Updates a SageMaker HyperPod cluster.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_cluster.html)

```python
# update_cluster method definition

await def update_cluster(
    self,
    *,
    ClusterName: str,
    InstanceGroups: Sequence[ClusterInstanceGroupSpecificationTypeDef],  # (1)
    NodeRecovery: ClusterNodeRecoveryType = ...,  # (2)
    InstanceGroupsToDelete: Sequence[str] = ...,
) -> UpdateClusterResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ClusterInstanceGroupSpecificationTypeDef](./type_defs.md#clusterinstancegroupspecificationtypedef) 
2. See [:material-code-brackets: ClusterNodeRecoveryType](./literals.md#clusternoderecoverytype) 
3. See [:material-code-braces: UpdateClusterResponseTypeDef](./type_defs.md#updateclusterresponsetypedef) 


```python
# update_cluster method usage example with argument unpacking

kwargs: UpdateClusterRequestTypeDef = {  # (1)
    "ClusterName": ...,
    "InstanceGroups": ...,
}

parent.update_cluster(**kwargs)
```

1. See [:material-code-braces: UpdateClusterRequestTypeDef](./type_defs.md#updateclusterrequesttypedef) 

### update\_cluster\_scheduler\_config

Update the cluster policy configuration.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_cluster_scheduler_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_cluster_scheduler_config.html)

```python
# update_cluster_scheduler_config method definition

await def update_cluster_scheduler_config(
    self,
    *,
    ClusterSchedulerConfigId: str,
    TargetVersion: int,
    SchedulerConfig: SchedulerConfigUnionTypeDef = ...,  # (1)
    Description: str = ...,
) -> UpdateClusterSchedulerConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SchedulerConfigTypeDef](./type_defs.md#schedulerconfigtypedef) [:material-code-braces: SchedulerConfigOutputTypeDef](./type_defs.md#schedulerconfigoutputtypedef) 
2. See [:material-code-braces: UpdateClusterSchedulerConfigResponseTypeDef](./type_defs.md#updateclusterschedulerconfigresponsetypedef) 


```python
# update_cluster_scheduler_config method usage example with argument unpacking

kwargs: UpdateClusterSchedulerConfigRequestTypeDef = {  # (1)
    "ClusterSchedulerConfigId": ...,
    "TargetVersion": ...,
}

parent.update_cluster_scheduler_config(**kwargs)
```

1. See [:material-code-braces: UpdateClusterSchedulerConfigRequestTypeDef](./type_defs.md#updateclusterschedulerconfigrequesttypedef) 

### update\_cluster\_software

Updates the platform software of a SageMaker HyperPod cluster for security
patching.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_cluster_software` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_cluster_software.html)

```python
# update_cluster_software method definition

await def update_cluster_software(
    self,
    *,
    ClusterName: str,
) -> UpdateClusterSoftwareResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateClusterSoftwareResponseTypeDef](./type_defs.md#updateclustersoftwareresponsetypedef) 


```python
# update_cluster_software method usage example with argument unpacking

kwargs: UpdateClusterSoftwareRequestTypeDef = {  # (1)
    "ClusterName": ...,
}

parent.update_cluster_software(**kwargs)
```

1. See [:material-code-braces: UpdateClusterSoftwareRequestTypeDef](./type_defs.md#updateclustersoftwarerequesttypedef) 

### update\_code\_repository

Updates the specified Git repository with the specified values.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_code_repository` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_code_repository.html)

```python
# update_code_repository method definition

await def update_code_repository(
    self,
    *,
    CodeRepositoryName: str,
    GitConfig: GitConfigForUpdateTypeDef = ...,  # (1)
) -> UpdateCodeRepositoryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GitConfigForUpdateTypeDef](./type_defs.md#gitconfigforupdatetypedef) 
2. See [:material-code-braces: UpdateCodeRepositoryOutputTypeDef](./type_defs.md#updatecoderepositoryoutputtypedef) 


```python
# update_code_repository method usage example with argument unpacking

kwargs: UpdateCodeRepositoryInputTypeDef = {  # (1)
    "CodeRepositoryName": ...,
}

parent.update_code_repository(**kwargs)
```

1. See [:material-code-braces: UpdateCodeRepositoryInputTypeDef](./type_defs.md#updatecoderepositoryinputtypedef) 

### update\_compute\_quota

Update the compute allocation definition.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_compute_quota` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_compute_quota.html)

```python
# update_compute_quota method definition

await def update_compute_quota(
    self,
    *,
    ComputeQuotaId: str,
    TargetVersion: int,
    ComputeQuotaConfig: ComputeQuotaConfigUnionTypeDef = ...,  # (1)
    ComputeQuotaTarget: ComputeQuotaTargetTypeDef = ...,  # (2)
    ActivationState: ActivationStateType = ...,  # (3)
    Description: str = ...,
) -> UpdateComputeQuotaResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ComputeQuotaConfigTypeDef](./type_defs.md#computequotaconfigtypedef) [:material-code-braces: ComputeQuotaConfigOutputTypeDef](./type_defs.md#computequotaconfigoutputtypedef) 
2. See [:material-code-braces: ComputeQuotaTargetTypeDef](./type_defs.md#computequotatargettypedef) 
3. See [:material-code-brackets: ActivationStateType](./literals.md#activationstatetype) 
4. See [:material-code-braces: UpdateComputeQuotaResponseTypeDef](./type_defs.md#updatecomputequotaresponsetypedef) 


```python
# update_compute_quota method usage example with argument unpacking

kwargs: UpdateComputeQuotaRequestTypeDef = {  # (1)
    "ComputeQuotaId": ...,
    "TargetVersion": ...,
}

parent.update_compute_quota(**kwargs)
```

1. See [:material-code-braces: UpdateComputeQuotaRequestTypeDef](./type_defs.md#updatecomputequotarequesttypedef) 

### update\_context

Updates a context.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_context` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_context.html)

```python
# update_context method definition

await def update_context(
    self,
    *,
    ContextName: str,
    Description: str = ...,
    Properties: Mapping[str, str] = ...,
    PropertiesToRemove: Sequence[str] = ...,
) -> UpdateContextResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateContextResponseTypeDef](./type_defs.md#updatecontextresponsetypedef) 


```python
# update_context method usage example with argument unpacking

kwargs: UpdateContextRequestTypeDef = {  # (1)
    "ContextName": ...,
}

parent.update_context(**kwargs)
```

1. See [:material-code-braces: UpdateContextRequestTypeDef](./type_defs.md#updatecontextrequesttypedef) 

### update\_device\_fleet

Updates a fleet of devices.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_device_fleet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_device_fleet.html)

```python
# update_device_fleet method definition

await def update_device_fleet(
    self,
    *,
    DeviceFleetName: str,
    OutputConfig: EdgeOutputConfigTypeDef,  # (1)
    RoleArn: str = ...,
    Description: str = ...,
    EnableIotRoleAlias: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_device_fleet method usage example with argument unpacking

kwargs: UpdateDeviceFleetRequestTypeDef = {  # (1)
    "DeviceFleetName": ...,
    "OutputConfig": ...,
}

parent.update_device_fleet(**kwargs)
```

1. See [:material-code-braces: UpdateDeviceFleetRequestTypeDef](./type_defs.md#updatedevicefleetrequesttypedef) 

### update\_devices

Updates one or more devices in a fleet.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_devices.html)

```python
# update_devices method definition

await def update_devices(
    self,
    *,
    DeviceFleetName: str,
    Devices: Sequence[DeviceTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_devices method usage example with argument unpacking

kwargs: UpdateDevicesRequestTypeDef = {  # (1)
    "DeviceFleetName": ...,
    "Devices": ...,
}

parent.update_devices(**kwargs)
```

1. See [:material-code-braces: UpdateDevicesRequestTypeDef](./type_defs.md#updatedevicesrequesttypedef) 

### update\_domain

Updates the default settings for new user profiles in the domain.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_domain.html)

```python
# update_domain method definition

await def update_domain(
    self,
    *,
    DomainId: str,
    DefaultUserSettings: UserSettingsUnionTypeDef = ...,  # (1)
    DomainSettingsForUpdate: DomainSettingsForUpdateTypeDef = ...,  # (2)
    AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,  # (3)
    DefaultSpaceSettings: DefaultSpaceSettingsUnionTypeDef = ...,  # (4)
    SubnetIds: Sequence[str] = ...,
    AppNetworkAccessType: AppNetworkAccessTypeType = ...,  # (5)
    TagPropagation: TagPropagationType = ...,  # (6)
) -> UpdateDomainResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) [:material-code-braces: UserSettingsOutputTypeDef](./type_defs.md#usersettingsoutputtypedef) 
2. See [:material-code-braces: DomainSettingsForUpdateTypeDef](./type_defs.md#domainsettingsforupdatetypedef) 
3. See [:material-code-brackets: AppSecurityGroupManagementType](./literals.md#appsecuritygroupmanagementtype) 
4. See [:material-code-braces: DefaultSpaceSettingsTypeDef](./type_defs.md#defaultspacesettingstypedef) [:material-code-braces: DefaultSpaceSettingsOutputTypeDef](./type_defs.md#defaultspacesettingsoutputtypedef) 
5. See [:material-code-brackets: AppNetworkAccessTypeType](./literals.md#appnetworkaccesstypetype) 
6. See [:material-code-brackets: TagPropagationType](./literals.md#tagpropagationtype) 
7. See [:material-code-braces: UpdateDomainResponseTypeDef](./type_defs.md#updatedomainresponsetypedef) 


```python
# update_domain method usage example with argument unpacking

kwargs: UpdateDomainRequestTypeDef = {  # (1)
    "DomainId": ...,
}

parent.update_domain(**kwargs)
```

1. See [:material-code-braces: UpdateDomainRequestTypeDef](./type_defs.md#updatedomainrequesttypedef) 

### update\_endpoint

Deploys the <code>EndpointConfig</code> specified in the request to a new fleet
of instances.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_endpoint.html)

```python
# update_endpoint method definition

await def update_endpoint(
    self,
    *,
    EndpointName: str,
    EndpointConfigName: str,
    RetainAllVariantProperties: bool = ...,
    ExcludeRetainedVariantProperties: Sequence[VariantPropertyTypeDef] = ...,  # (1)
    DeploymentConfig: DeploymentConfigUnionTypeDef = ...,  # (2)
    RetainDeploymentConfig: bool = ...,
) -> UpdateEndpointOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VariantPropertyTypeDef](./type_defs.md#variantpropertytypedef) 
2. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) [:material-code-braces: DeploymentConfigOutputTypeDef](./type_defs.md#deploymentconfigoutputtypedef) 
3. See [:material-code-braces: UpdateEndpointOutputTypeDef](./type_defs.md#updateendpointoutputtypedef) 


```python
# update_endpoint method usage example with argument unpacking

kwargs: UpdateEndpointInputTypeDef = {  # (1)
    "EndpointName": ...,
    "EndpointConfigName": ...,
}

parent.update_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateEndpointInputTypeDef](./type_defs.md#updateendpointinputtypedef) 

### update\_endpoint\_weights\_and\_capacities

Updates variant weight of one or more variants associated with an existing
endpoint, or capacity of one variant associated with an existing endpoint.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_endpoint_weights_and_capacities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_endpoint_weights_and_capacities.html)

```python
# update_endpoint_weights_and_capacities method definition

await def update_endpoint_weights_and_capacities(
    self,
    *,
    EndpointName: str,
    DesiredWeightsAndCapacities: Sequence[DesiredWeightAndCapacityTypeDef],  # (1)
) -> UpdateEndpointWeightsAndCapacitiesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DesiredWeightAndCapacityTypeDef](./type_defs.md#desiredweightandcapacitytypedef) 
2. See [:material-code-braces: UpdateEndpointWeightsAndCapacitiesOutputTypeDef](./type_defs.md#updateendpointweightsandcapacitiesoutputtypedef) 


```python
# update_endpoint_weights_and_capacities method usage example with argument unpacking

kwargs: UpdateEndpointWeightsAndCapacitiesInputTypeDef = {  # (1)
    "EndpointName": ...,
    "DesiredWeightsAndCapacities": ...,
}

parent.update_endpoint_weights_and_capacities(**kwargs)
```

1. See [:material-code-braces: UpdateEndpointWeightsAndCapacitiesInputTypeDef](./type_defs.md#updateendpointweightsandcapacitiesinputtypedef) 

### update\_experiment

Adds, updates, or removes the description of an experiment.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_experiment.html)

```python
# update_experiment method definition

await def update_experiment(
    self,
    *,
    ExperimentName: str,
    DisplayName: str = ...,
    Description: str = ...,
) -> UpdateExperimentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateExperimentResponseTypeDef](./type_defs.md#updateexperimentresponsetypedef) 


```python
# update_experiment method usage example with argument unpacking

kwargs: UpdateExperimentRequestTypeDef = {  # (1)
    "ExperimentName": ...,
}

parent.update_experiment(**kwargs)
```

1. See [:material-code-braces: UpdateExperimentRequestTypeDef](./type_defs.md#updateexperimentrequesttypedef) 

### update\_feature\_group

Updates the feature group by either adding features or updating the online
store configuration.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_feature_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_feature_group.html)

```python
# update_feature_group method definition

await def update_feature_group(
    self,
    *,
    FeatureGroupName: str,
    FeatureAdditions: Sequence[FeatureDefinitionTypeDef] = ...,  # (1)
    OnlineStoreConfig: OnlineStoreConfigUpdateTypeDef = ...,  # (2)
    ThroughputConfig: ThroughputConfigUpdateTypeDef = ...,  # (3)
) -> UpdateFeatureGroupResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: FeatureDefinitionTypeDef](./type_defs.md#featuredefinitiontypedef) 
2. See [:material-code-braces: OnlineStoreConfigUpdateTypeDef](./type_defs.md#onlinestoreconfigupdatetypedef) 
3. See [:material-code-braces: ThroughputConfigUpdateTypeDef](./type_defs.md#throughputconfigupdatetypedef) 
4. See [:material-code-braces: UpdateFeatureGroupResponseTypeDef](./type_defs.md#updatefeaturegroupresponsetypedef) 


```python
# update_feature_group method usage example with argument unpacking

kwargs: UpdateFeatureGroupRequestTypeDef = {  # (1)
    "FeatureGroupName": ...,
}

parent.update_feature_group(**kwargs)
```

1. See [:material-code-braces: UpdateFeatureGroupRequestTypeDef](./type_defs.md#updatefeaturegrouprequesttypedef) 

### update\_feature\_metadata

Updates the description and parameters of the feature group.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_feature_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_feature_metadata.html)

```python
# update_feature_metadata method definition

await def update_feature_metadata(
    self,
    *,
    FeatureGroupName: str,
    FeatureName: str,
    Description: str = ...,
    ParameterAdditions: Sequence[FeatureParameterTypeDef] = ...,  # (1)
    ParameterRemovals: Sequence[str] = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FeatureParameterTypeDef](./type_defs.md#featureparametertypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# update_feature_metadata method usage example with argument unpacking

kwargs: UpdateFeatureMetadataRequestTypeDef = {  # (1)
    "FeatureGroupName": ...,
    "FeatureName": ...,
}

parent.update_feature_metadata(**kwargs)
```

1. See [:material-code-braces: UpdateFeatureMetadataRequestTypeDef](./type_defs.md#updatefeaturemetadatarequesttypedef) 

### update\_hub

Update a hub.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_hub` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_hub.html)

```python
# update_hub method definition

await def update_hub(
    self,
    *,
    HubName: str,
    HubDescription: str = ...,
    HubDisplayName: str = ...,
    HubSearchKeywords: Sequence[str] = ...,
) -> UpdateHubResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateHubResponseTypeDef](./type_defs.md#updatehubresponsetypedef) 


```python
# update_hub method usage example with argument unpacking

kwargs: UpdateHubRequestTypeDef = {  # (1)
    "HubName": ...,
}

parent.update_hub(**kwargs)
```

1. See [:material-code-braces: UpdateHubRequestTypeDef](./type_defs.md#updatehubrequesttypedef) 

### update\_image

Updates the properties of a SageMaker AI image.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_image` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_image.html)

```python
# update_image method definition

await def update_image(
    self,
    *,
    ImageName: str,
    DeleteProperties: Sequence[str] = ...,
    Description: str = ...,
    DisplayName: str = ...,
    RoleArn: str = ...,
) -> UpdateImageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateImageResponseTypeDef](./type_defs.md#updateimageresponsetypedef) 


```python
# update_image method usage example with argument unpacking

kwargs: UpdateImageRequestTypeDef = {  # (1)
    "ImageName": ...,
}

parent.update_image(**kwargs)
```

1. See [:material-code-braces: UpdateImageRequestTypeDef](./type_defs.md#updateimagerequesttypedef) 

### update\_image\_version

Updates the properties of a SageMaker AI image version.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_image_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_image_version.html)

```python
# update_image_version method definition

await def update_image_version(
    self,
    *,
    ImageName: str,
    Alias: str = ...,
    Version: int = ...,
    AliasesToAdd: Sequence[str] = ...,
    AliasesToDelete: Sequence[str] = ...,
    VendorGuidance: VendorGuidanceType = ...,  # (1)
    JobType: JobTypeType = ...,  # (2)
    MLFramework: str = ...,
    ProgrammingLang: str = ...,
    Processor: ProcessorType = ...,  # (3)
    Horovod: bool = ...,
    ReleaseNotes: str = ...,
) -> UpdateImageVersionResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: VendorGuidanceType](./literals.md#vendorguidancetype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: ProcessorType](./literals.md#processortype) 
4. See [:material-code-braces: UpdateImageVersionResponseTypeDef](./type_defs.md#updateimageversionresponsetypedef) 


```python
# update_image_version method usage example with argument unpacking

kwargs: UpdateImageVersionRequestTypeDef = {  # (1)
    "ImageName": ...,
}

parent.update_image_version(**kwargs)
```

1. See [:material-code-braces: UpdateImageVersionRequestTypeDef](./type_defs.md#updateimageversionrequesttypedef) 

### update\_inference\_component

Updates an inference component.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_inference_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_inference_component.html)

```python
# update_inference_component method definition

await def update_inference_component(
    self,
    *,
    InferenceComponentName: str,
    Specification: InferenceComponentSpecificationTypeDef = ...,  # (1)
    RuntimeConfig: InferenceComponentRuntimeConfigTypeDef = ...,  # (2)
) -> UpdateInferenceComponentOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InferenceComponentSpecificationTypeDef](./type_defs.md#inferencecomponentspecificationtypedef) 
2. See [:material-code-braces: InferenceComponentRuntimeConfigTypeDef](./type_defs.md#inferencecomponentruntimeconfigtypedef) 
3. See [:material-code-braces: UpdateInferenceComponentOutputTypeDef](./type_defs.md#updateinferencecomponentoutputtypedef) 


```python
# update_inference_component method usage example with argument unpacking

kwargs: UpdateInferenceComponentInputTypeDef = {  # (1)
    "InferenceComponentName": ...,
}

parent.update_inference_component(**kwargs)
```

1. See [:material-code-braces: UpdateInferenceComponentInputTypeDef](./type_defs.md#updateinferencecomponentinputtypedef) 

### update\_inference\_component\_runtime\_config

Runtime settings for a model that is deployed with an inference component.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_inference_component_runtime_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_inference_component_runtime_config.html)

```python
# update_inference_component_runtime_config method definition

await def update_inference_component_runtime_config(
    self,
    *,
    InferenceComponentName: str,
    DesiredRuntimeConfig: InferenceComponentRuntimeConfigTypeDef,  # (1)
) -> UpdateInferenceComponentRuntimeConfigOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InferenceComponentRuntimeConfigTypeDef](./type_defs.md#inferencecomponentruntimeconfigtypedef) 
2. See [:material-code-braces: UpdateInferenceComponentRuntimeConfigOutputTypeDef](./type_defs.md#updateinferencecomponentruntimeconfigoutputtypedef) 


```python
# update_inference_component_runtime_config method usage example with argument unpacking

kwargs: UpdateInferenceComponentRuntimeConfigInputTypeDef = {  # (1)
    "InferenceComponentName": ...,
    "DesiredRuntimeConfig": ...,
}

parent.update_inference_component_runtime_config(**kwargs)
```

1. See [:material-code-braces: UpdateInferenceComponentRuntimeConfigInputTypeDef](./type_defs.md#updateinferencecomponentruntimeconfiginputtypedef) 

### update\_inference\_experiment

Updates an inference experiment that you created.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_inference_experiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_inference_experiment.html)

```python
# update_inference_experiment method definition

await def update_inference_experiment(
    self,
    *,
    Name: str,
    Schedule: InferenceExperimentScheduleUnionTypeDef = ...,  # (1)
    Description: str = ...,
    ModelVariants: Sequence[ModelVariantConfigTypeDef] = ...,  # (2)
    DataStorageConfig: InferenceExperimentDataStorageConfigUnionTypeDef = ...,  # (3)
    ShadowModeConfig: ShadowModeConfigUnionTypeDef = ...,  # (4)
) -> UpdateInferenceExperimentResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: InferenceExperimentScheduleTypeDef](./type_defs.md#inferenceexperimentscheduletypedef) [:material-code-braces: InferenceExperimentScheduleOutputTypeDef](./type_defs.md#inferenceexperimentscheduleoutputtypedef) 
2. See [:material-code-braces: ModelVariantConfigTypeDef](./type_defs.md#modelvariantconfigtypedef) 
3. See [:material-code-braces: InferenceExperimentDataStorageConfigTypeDef](./type_defs.md#inferenceexperimentdatastorageconfigtypedef) [:material-code-braces: InferenceExperimentDataStorageConfigOutputTypeDef](./type_defs.md#inferenceexperimentdatastorageconfigoutputtypedef) 
4. See [:material-code-braces: ShadowModeConfigTypeDef](./type_defs.md#shadowmodeconfigtypedef) [:material-code-braces: ShadowModeConfigOutputTypeDef](./type_defs.md#shadowmodeconfigoutputtypedef) 
5. See [:material-code-braces: UpdateInferenceExperimentResponseTypeDef](./type_defs.md#updateinferenceexperimentresponsetypedef) 


```python
# update_inference_experiment method usage example with argument unpacking

kwargs: UpdateInferenceExperimentRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_inference_experiment(**kwargs)
```

1. See [:material-code-braces: UpdateInferenceExperimentRequestTypeDef](./type_defs.md#updateinferenceexperimentrequesttypedef) 

### update\_mlflow\_tracking\_server

Updates properties of an existing MLflow Tracking Server.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_mlflow_tracking_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_mlflow_tracking_server.html)

```python
# update_mlflow_tracking_server method definition

await def update_mlflow_tracking_server(
    self,
    *,
    TrackingServerName: str,
    ArtifactStoreUri: str = ...,
    TrackingServerSize: TrackingServerSizeType = ...,  # (1)
    AutomaticModelRegistration: bool = ...,
    WeeklyMaintenanceWindowStart: str = ...,
) -> UpdateMlflowTrackingServerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TrackingServerSizeType](./literals.md#trackingserversizetype) 
2. See [:material-code-braces: UpdateMlflowTrackingServerResponseTypeDef](./type_defs.md#updatemlflowtrackingserverresponsetypedef) 


```python
# update_mlflow_tracking_server method usage example with argument unpacking

kwargs: UpdateMlflowTrackingServerRequestTypeDef = {  # (1)
    "TrackingServerName": ...,
}

parent.update_mlflow_tracking_server(**kwargs)
```

1. See [:material-code-braces: UpdateMlflowTrackingServerRequestTypeDef](./type_defs.md#updatemlflowtrackingserverrequesttypedef) 

### update\_model\_card

Update an Amazon SageMaker Model Card.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_model_card` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_model_card.html)

```python
# update_model_card method definition

await def update_model_card(
    self,
    *,
    ModelCardName: str,
    Content: str = ...,
    ModelCardStatus: ModelCardStatusType = ...,  # (1)
) -> UpdateModelCardResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-braces: UpdateModelCardResponseTypeDef](./type_defs.md#updatemodelcardresponsetypedef) 


```python
# update_model_card method usage example with argument unpacking

kwargs: UpdateModelCardRequestTypeDef = {  # (1)
    "ModelCardName": ...,
}

parent.update_model_card(**kwargs)
```

1. See [:material-code-braces: UpdateModelCardRequestTypeDef](./type_defs.md#updatemodelcardrequesttypedef) 

### update\_model\_package

Updates a versioned model.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_model_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_model_package.html)

```python
# update_model_package method definition

await def update_model_package(
    self,
    *,
    ModelPackageArn: str,
    ModelApprovalStatus: ModelApprovalStatusType = ...,  # (1)
    ApprovalDescription: str = ...,
    CustomerMetadataProperties: Mapping[str, str] = ...,
    CustomerMetadataPropertiesToRemove: Sequence[str] = ...,
    AdditionalInferenceSpecificationsToAdd: Sequence[AdditionalInferenceSpecificationDefinitionUnionTypeDef] = ...,  # (2)
    InferenceSpecification: InferenceSpecificationUnionTypeDef = ...,  # (3)
    SourceUri: str = ...,
    ModelCard: ModelPackageModelCardTypeDef = ...,  # (4)
    ModelLifeCycle: ModelLifeCycleTypeDef = ...,  # (5)
    ClientToken: str = ...,
) -> UpdateModelPackageOutputTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
2. See [:material-code-braces: AdditionalInferenceSpecificationDefinitionTypeDef](./type_defs.md#additionalinferencespecificationdefinitiontypedef) [:material-code-braces: AdditionalInferenceSpecificationDefinitionOutputTypeDef](./type_defs.md#additionalinferencespecificationdefinitionoutputtypedef) 
3. See [:material-code-braces: InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef) [:material-code-braces: InferenceSpecificationOutputTypeDef](./type_defs.md#inferencespecificationoutputtypedef) 
4. See [:material-code-braces: ModelPackageModelCardTypeDef](./type_defs.md#modelpackagemodelcardtypedef) 
5. See [:material-code-braces: ModelLifeCycleTypeDef](./type_defs.md#modellifecycletypedef) 
6. See [:material-code-braces: UpdateModelPackageOutputTypeDef](./type_defs.md#updatemodelpackageoutputtypedef) 


```python
# update_model_package method usage example with argument unpacking

kwargs: UpdateModelPackageInputTypeDef = {  # (1)
    "ModelPackageArn": ...,
}

parent.update_model_package(**kwargs)
```

1. See [:material-code-braces: UpdateModelPackageInputTypeDef](./type_defs.md#updatemodelpackageinputtypedef) 

### update\_monitoring\_alert

Update the parameters of a model monitor alert.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_monitoring_alert` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_monitoring_alert.html)

```python
# update_monitoring_alert method definition

await def update_monitoring_alert(
    self,
    *,
    MonitoringScheduleName: str,
    MonitoringAlertName: str,
    DatapointsToAlert: int,
    EvaluationPeriod: int,
) -> UpdateMonitoringAlertResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateMonitoringAlertResponseTypeDef](./type_defs.md#updatemonitoringalertresponsetypedef) 


```python
# update_monitoring_alert method usage example with argument unpacking

kwargs: UpdateMonitoringAlertRequestTypeDef = {  # (1)
    "MonitoringScheduleName": ...,
    "MonitoringAlertName": ...,
    "DatapointsToAlert": ...,
    "EvaluationPeriod": ...,
}

parent.update_monitoring_alert(**kwargs)
```

1. See [:material-code-braces: UpdateMonitoringAlertRequestTypeDef](./type_defs.md#updatemonitoringalertrequesttypedef) 

### update\_monitoring\_schedule

Updates a previously created schedule.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_monitoring_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_monitoring_schedule.html)

```python
# update_monitoring_schedule method definition

await def update_monitoring_schedule(
    self,
    *,
    MonitoringScheduleName: str,
    MonitoringScheduleConfig: MonitoringScheduleConfigUnionTypeDef,  # (1)
) -> UpdateMonitoringScheduleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MonitoringScheduleConfigTypeDef](./type_defs.md#monitoringscheduleconfigtypedef) [:material-code-braces: MonitoringScheduleConfigOutputTypeDef](./type_defs.md#monitoringscheduleconfigoutputtypedef) 
2. See [:material-code-braces: UpdateMonitoringScheduleResponseTypeDef](./type_defs.md#updatemonitoringscheduleresponsetypedef) 


```python
# update_monitoring_schedule method usage example with argument unpacking

kwargs: UpdateMonitoringScheduleRequestTypeDef = {  # (1)
    "MonitoringScheduleName": ...,
    "MonitoringScheduleConfig": ...,
}

parent.update_monitoring_schedule(**kwargs)
```

1. See [:material-code-braces: UpdateMonitoringScheduleRequestTypeDef](./type_defs.md#updatemonitoringschedulerequesttypedef) 

### update\_notebook\_instance

Updates a notebook instance.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_notebook_instance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_notebook_instance.html)

```python
# update_notebook_instance method definition

await def update_notebook_instance(
    self,
    *,
    NotebookInstanceName: str,
    InstanceType: InstanceTypeType = ...,  # (1)
    RoleArn: str = ...,
    LifecycleConfigName: str = ...,
    DisassociateLifecycleConfig: bool = ...,
    VolumeSizeInGB: int = ...,
    DefaultCodeRepository: str = ...,
    AdditionalCodeRepositories: Sequence[str] = ...,
    AcceleratorTypes: Sequence[NotebookInstanceAcceleratorTypeType] = ...,  # (2)
    DisassociateAcceleratorTypes: bool = ...,
    DisassociateDefaultCodeRepository: bool = ...,
    DisassociateAdditionalCodeRepositories: bool = ...,
    RootAccess: RootAccessType = ...,  # (3)
    InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef = ...,  # (4)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
2. See [:material-code-brackets: NotebookInstanceAcceleratorTypeType](./literals.md#notebookinstanceacceleratortypetype) 
3. See [:material-code-brackets: RootAccessType](./literals.md#rootaccesstype) 
4. See [:material-code-braces: InstanceMetadataServiceConfigurationTypeDef](./type_defs.md#instancemetadataserviceconfigurationtypedef) 


```python
# update_notebook_instance method usage example with argument unpacking

kwargs: UpdateNotebookInstanceInputTypeDef = {  # (1)
    "NotebookInstanceName": ...,
}

parent.update_notebook_instance(**kwargs)
```

1. See [:material-code-braces: UpdateNotebookInstanceInputTypeDef](./type_defs.md#updatenotebookinstanceinputtypedef) 

### update\_notebook\_instance\_lifecycle\_config

Updates a notebook instance lifecycle configuration created with the <a
href="https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateNotebookInstanceLifecycleConfig.html">CreateNotebookInstanceLifecycleConfig</a>
API.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_notebook_instance_lifecycle_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_notebook_instance_lifecycle_config.html)

```python
# update_notebook_instance_lifecycle_config method definition

await def update_notebook_instance_lifecycle_config(
    self,
    *,
    NotebookInstanceLifecycleConfigName: str,
    OnCreate: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,  # (1)
    OnStart: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef) 
2. See [:material-code-braces: NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef) 


```python
# update_notebook_instance_lifecycle_config method usage example with argument unpacking

kwargs: UpdateNotebookInstanceLifecycleConfigInputTypeDef = {  # (1)
    "NotebookInstanceLifecycleConfigName": ...,
}

parent.update_notebook_instance_lifecycle_config(**kwargs)
```

1. See [:material-code-braces: UpdateNotebookInstanceLifecycleConfigInputTypeDef](./type_defs.md#updatenotebookinstancelifecycleconfiginputtypedef) 

### update\_partner\_app

Updates all of the SageMaker Partner AI Apps in an account.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_partner_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_partner_app.html)

```python
# update_partner_app method definition

await def update_partner_app(
    self,
    *,
    Arn: str,
    MaintenanceConfig: PartnerAppMaintenanceConfigTypeDef = ...,  # (1)
    Tier: str = ...,
    ApplicationConfig: PartnerAppConfigUnionTypeDef = ...,  # (2)
    EnableIamSessionBasedIdentity: bool = ...,
    ClientToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> UpdatePartnerAppResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: PartnerAppMaintenanceConfigTypeDef](./type_defs.md#partnerappmaintenanceconfigtypedef) 
2. See [:material-code-braces: PartnerAppConfigTypeDef](./type_defs.md#partnerappconfigtypedef) [:material-code-braces: PartnerAppConfigOutputTypeDef](./type_defs.md#partnerappconfigoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: UpdatePartnerAppResponseTypeDef](./type_defs.md#updatepartnerappresponsetypedef) 


```python
# update_partner_app method usage example with argument unpacking

kwargs: UpdatePartnerAppRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.update_partner_app(**kwargs)
```

1. See [:material-code-braces: UpdatePartnerAppRequestTypeDef](./type_defs.md#updatepartnerapprequesttypedef) 

### update\_pipeline

Updates a pipeline.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_pipeline` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_pipeline.html)

```python
# update_pipeline method definition

await def update_pipeline(
    self,
    *,
    PipelineName: str,
    PipelineDisplayName: str = ...,
    PipelineDefinition: str = ...,
    PipelineDefinitionS3Location: PipelineDefinitionS3LocationTypeDef = ...,  # (1)
    PipelineDescription: str = ...,
    RoleArn: str = ...,
    ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,  # (2)
) -> UpdatePipelineResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PipelineDefinitionS3LocationTypeDef](./type_defs.md#pipelinedefinitions3locationtypedef) 
2. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
3. See [:material-code-braces: UpdatePipelineResponseTypeDef](./type_defs.md#updatepipelineresponsetypedef) 


```python
# update_pipeline method usage example with argument unpacking

kwargs: UpdatePipelineRequestTypeDef = {  # (1)
    "PipelineName": ...,
}

parent.update_pipeline(**kwargs)
```

1. See [:material-code-braces: UpdatePipelineRequestTypeDef](./type_defs.md#updatepipelinerequesttypedef) 

### update\_pipeline\_execution

Updates a pipeline execution.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_pipeline_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_pipeline_execution.html)

```python
# update_pipeline_execution method definition

await def update_pipeline_execution(
    self,
    *,
    PipelineExecutionArn: str,
    PipelineExecutionDescription: str = ...,
    PipelineExecutionDisplayName: str = ...,
    ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,  # (1)
) -> UpdatePipelineExecutionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
2. See [:material-code-braces: UpdatePipelineExecutionResponseTypeDef](./type_defs.md#updatepipelineexecutionresponsetypedef) 


```python
# update_pipeline_execution method usage example with argument unpacking

kwargs: UpdatePipelineExecutionRequestTypeDef = {  # (1)
    "PipelineExecutionArn": ...,
}

parent.update_pipeline_execution(**kwargs)
```

1. See [:material-code-braces: UpdatePipelineExecutionRequestTypeDef](./type_defs.md#updatepipelineexecutionrequesttypedef) 

### update\_project

Updates a machine learning (ML) project that is created from a template that
sets up an ML pipeline from training to deploying an approved model.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_project` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_project.html)

```python
# update_project method definition

await def update_project(
    self,
    *,
    ProjectName: str,
    ProjectDescription: str = ...,
    ServiceCatalogProvisioningUpdateDetails: ServiceCatalogProvisioningUpdateDetailsTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> UpdateProjectOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ServiceCatalogProvisioningUpdateDetailsTypeDef](./type_defs.md#servicecatalogprovisioningupdatedetailstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: UpdateProjectOutputTypeDef](./type_defs.md#updateprojectoutputtypedef) 


```python
# update_project method usage example with argument unpacking

kwargs: UpdateProjectInputTypeDef = {  # (1)
    "ProjectName": ...,
}

parent.update_project(**kwargs)
```

1. See [:material-code-braces: UpdateProjectInputTypeDef](./type_defs.md#updateprojectinputtypedef) 

### update\_space

Updates the settings of a space.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_space.html)

```python
# update_space method definition

await def update_space(
    self,
    *,
    DomainId: str,
    SpaceName: str,
    SpaceSettings: SpaceSettingsUnionTypeDef = ...,  # (1)
    SpaceDisplayName: str = ...,
) -> UpdateSpaceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SpaceSettingsTypeDef](./type_defs.md#spacesettingstypedef) [:material-code-braces: SpaceSettingsOutputTypeDef](./type_defs.md#spacesettingsoutputtypedef) 
2. See [:material-code-braces: UpdateSpaceResponseTypeDef](./type_defs.md#updatespaceresponsetypedef) 


```python
# update_space method usage example with argument unpacking

kwargs: UpdateSpaceRequestTypeDef = {  # (1)
    "DomainId": ...,
    "SpaceName": ...,
}

parent.update_space(**kwargs)
```

1. See [:material-code-braces: UpdateSpaceRequestTypeDef](./type_defs.md#updatespacerequesttypedef) 

### update\_training\_job

Update a model training job to request a new Debugger profiling configuration
or to change warm pool retention length.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_training_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_training_job.html)

```python
# update_training_job method definition

await def update_training_job(
    self,
    *,
    TrainingJobName: str,
    ProfilerConfig: ProfilerConfigForUpdateTypeDef = ...,  # (1)
    ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationUnionTypeDef] = ...,  # (2)
    ResourceConfig: ResourceConfigForUpdateTypeDef = ...,  # (3)
    RemoteDebugConfig: RemoteDebugConfigForUpdateTypeDef = ...,  # (4)
) -> UpdateTrainingJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ProfilerConfigForUpdateTypeDef](./type_defs.md#profilerconfigforupdatetypedef) 
2. See [:material-code-braces: ProfilerRuleConfigurationTypeDef](./type_defs.md#profilerruleconfigurationtypedef) [:material-code-braces: ProfilerRuleConfigurationOutputTypeDef](./type_defs.md#profilerruleconfigurationoutputtypedef) 
3. See [:material-code-braces: ResourceConfigForUpdateTypeDef](./type_defs.md#resourceconfigforupdatetypedef) 
4. See [:material-code-braces: RemoteDebugConfigForUpdateTypeDef](./type_defs.md#remotedebugconfigforupdatetypedef) 
5. See [:material-code-braces: UpdateTrainingJobResponseTypeDef](./type_defs.md#updatetrainingjobresponsetypedef) 


```python
# update_training_job method usage example with argument unpacking

kwargs: UpdateTrainingJobRequestTypeDef = {  # (1)
    "TrainingJobName": ...,
}

parent.update_training_job(**kwargs)
```

1. See [:material-code-braces: UpdateTrainingJobRequestTypeDef](./type_defs.md#updatetrainingjobrequesttypedef) 

### update\_trial

Updates the display name of a trial.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_trial` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_trial.html)

```python
# update_trial method definition

await def update_trial(
    self,
    *,
    TrialName: str,
    DisplayName: str = ...,
) -> UpdateTrialResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateTrialResponseTypeDef](./type_defs.md#updatetrialresponsetypedef) 


```python
# update_trial method usage example with argument unpacking

kwargs: UpdateTrialRequestTypeDef = {  # (1)
    "TrialName": ...,
}

parent.update_trial(**kwargs)
```

1. See [:material-code-braces: UpdateTrialRequestTypeDef](./type_defs.md#updatetrialrequesttypedef) 

### update\_trial\_component

Updates one or more properties of a trial component.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_trial_component` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_trial_component.html)

```python
# update_trial_component method definition

await def update_trial_component(
    self,
    *,
    TrialComponentName: str,
    DisplayName: str = ...,
    Status: TrialComponentStatusTypeDef = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    Parameters: Mapping[str, TrialComponentParameterValueTypeDef] = ...,  # (2)
    ParametersToRemove: Sequence[str] = ...,
    InputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,  # (3)
    InputArtifactsToRemove: Sequence[str] = ...,
    OutputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,  # (3)
    OutputArtifactsToRemove: Sequence[str] = ...,
) -> UpdateTrialComponentResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: TrialComponentStatusTypeDef](./type_defs.md#trialcomponentstatustypedef) 
2. See [:material-code-braces: TrialComponentParameterValueTypeDef](./type_defs.md#trialcomponentparametervaluetypedef) 
3. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
4. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
5. See [:material-code-braces: UpdateTrialComponentResponseTypeDef](./type_defs.md#updatetrialcomponentresponsetypedef) 


```python
# update_trial_component method usage example with argument unpacking

kwargs: UpdateTrialComponentRequestTypeDef = {  # (1)
    "TrialComponentName": ...,
}

parent.update_trial_component(**kwargs)
```

1. See [:material-code-braces: UpdateTrialComponentRequestTypeDef](./type_defs.md#updatetrialcomponentrequesttypedef) 

### update\_user\_profile

Updates a user profile.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_user_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_user_profile.html)

```python
# update_user_profile method definition

await def update_user_profile(
    self,
    *,
    DomainId: str,
    UserProfileName: str,
    UserSettings: UserSettingsUnionTypeDef = ...,  # (1)
) -> UpdateUserProfileResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) [:material-code-braces: UserSettingsOutputTypeDef](./type_defs.md#usersettingsoutputtypedef) 
2. See [:material-code-braces: UpdateUserProfileResponseTypeDef](./type_defs.md#updateuserprofileresponsetypedef) 


```python
# update_user_profile method usage example with argument unpacking

kwargs: UpdateUserProfileRequestTypeDef = {  # (1)
    "DomainId": ...,
    "UserProfileName": ...,
}

parent.update_user_profile(**kwargs)
```

1. See [:material-code-braces: UpdateUserProfileRequestTypeDef](./type_defs.md#updateuserprofilerequesttypedef) 

### update\_workforce

Use this operation to update your workforce.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_workforce` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_workforce.html)

```python
# update_workforce method definition

await def update_workforce(
    self,
    *,
    WorkforceName: str,
    SourceIpConfig: SourceIpConfigUnionTypeDef = ...,  # (1)
    OidcConfig: OidcConfigTypeDef = ...,  # (2)
    WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...,  # (3)
) -> UpdateWorkforceResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: SourceIpConfigTypeDef](./type_defs.md#sourceipconfigtypedef) [:material-code-braces: SourceIpConfigOutputTypeDef](./type_defs.md#sourceipconfigoutputtypedef) 
2. See [:material-code-braces: OidcConfigTypeDef](./type_defs.md#oidcconfigtypedef) 
3. See [:material-code-braces: WorkforceVpcConfigRequestTypeDef](./type_defs.md#workforcevpcconfigrequesttypedef) 
4. See [:material-code-braces: UpdateWorkforceResponseTypeDef](./type_defs.md#updateworkforceresponsetypedef) 


```python
# update_workforce method usage example with argument unpacking

kwargs: UpdateWorkforceRequestTypeDef = {  # (1)
    "WorkforceName": ...,
}

parent.update_workforce(**kwargs)
```

1. See [:material-code-braces: UpdateWorkforceRequestTypeDef](./type_defs.md#updateworkforcerequesttypedef) 

### update\_workteam

Updates an existing work team with new member definitions or description.

Type annotations and code completion for `#!python session.create_client("sagemaker").update_workteam` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker/client/update_workteam.html)

```python
# update_workteam method definition

await def update_workteam(
    self,
    *,
    WorkteamName: str,
    MemberDefinitions: Sequence[MemberDefinitionUnionTypeDef] = ...,  # (1)
    Description: str = ...,
    NotificationConfiguration: NotificationConfigurationTypeDef = ...,  # (2)
    WorkerAccessConfiguration: WorkerAccessConfigurationTypeDef = ...,  # (3)
) -> UpdateWorkteamResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: MemberDefinitionTypeDef](./type_defs.md#memberdefinitiontypedef) [:material-code-braces: MemberDefinitionOutputTypeDef](./type_defs.md#memberdefinitionoutputtypedef) 
2. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
3. See [:material-code-braces: WorkerAccessConfigurationTypeDef](./type_defs.md#workeraccessconfigurationtypedef) 
4. See [:material-code-braces: UpdateWorkteamResponseTypeDef](./type_defs.md#updateworkteamresponsetypedef) 


```python
# update_workteam method usage example with argument unpacking

kwargs: UpdateWorkteamRequestTypeDef = {  # (1)
    "WorkteamName": ...,
}

parent.update_workteam(**kwargs)
```

1. See [:material-code-braces: UpdateWorkteamRequestTypeDef](./type_defs.md#updateworkteamrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sagemaker").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sagemaker").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("sagemaker").get_paginator` method with overloads.

- `client.get_paginator("list_actions")` -> [ListActionsPaginator](./paginators.md#listactionspaginator)
- `client.get_paginator("list_algorithms")` -> [ListAlgorithmsPaginator](./paginators.md#listalgorithmspaginator)
- `client.get_paginator("list_aliases")` -> [ListAliasesPaginator](./paginators.md#listaliasespaginator)
- `client.get_paginator("list_app_image_configs")` -> [ListAppImageConfigsPaginator](./paginators.md#listappimageconfigspaginator)
- `client.get_paginator("list_apps")` -> [ListAppsPaginator](./paginators.md#listappspaginator)
- `client.get_paginator("list_artifacts")` -> [ListArtifactsPaginator](./paginators.md#listartifactspaginator)
- `client.get_paginator("list_associations")` -> [ListAssociationsPaginator](./paginators.md#listassociationspaginator)
- `client.get_paginator("list_auto_ml_jobs")` -> [ListAutoMLJobsPaginator](./paginators.md#listautomljobspaginator)
- `client.get_paginator("list_candidates_for_auto_ml_job")` -> [ListCandidatesForAutoMLJobPaginator](./paginators.md#listcandidatesforautomljobpaginator)
- `client.get_paginator("list_cluster_nodes")` -> [ListClusterNodesPaginator](./paginators.md#listclusternodespaginator)
- `client.get_paginator("list_cluster_scheduler_configs")` -> [ListClusterSchedulerConfigsPaginator](./paginators.md#listclusterschedulerconfigspaginator)
- `client.get_paginator("list_clusters")` -> [ListClustersPaginator](./paginators.md#listclusterspaginator)
- `client.get_paginator("list_code_repositories")` -> [ListCodeRepositoriesPaginator](./paginators.md#listcoderepositoriespaginator)
- `client.get_paginator("list_compilation_jobs")` -> [ListCompilationJobsPaginator](./paginators.md#listcompilationjobspaginator)
- `client.get_paginator("list_compute_quotas")` -> [ListComputeQuotasPaginator](./paginators.md#listcomputequotaspaginator)
- `client.get_paginator("list_contexts")` -> [ListContextsPaginator](./paginators.md#listcontextspaginator)
- `client.get_paginator("list_data_quality_job_definitions")` -> [ListDataQualityJobDefinitionsPaginator](./paginators.md#listdataqualityjobdefinitionspaginator)
- `client.get_paginator("list_device_fleets")` -> [ListDeviceFleetsPaginator](./paginators.md#listdevicefleetspaginator)
- `client.get_paginator("list_devices")` -> [ListDevicesPaginator](./paginators.md#listdevicespaginator)
- `client.get_paginator("list_domains")` -> [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- `client.get_paginator("list_edge_deployment_plans")` -> [ListEdgeDeploymentPlansPaginator](./paginators.md#listedgedeploymentplanspaginator)
- `client.get_paginator("list_edge_packaging_jobs")` -> [ListEdgePackagingJobsPaginator](./paginators.md#listedgepackagingjobspaginator)
- `client.get_paginator("list_endpoint_configs")` -> [ListEndpointConfigsPaginator](./paginators.md#listendpointconfigspaginator)
- `client.get_paginator("list_endpoints")` -> [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
- `client.get_paginator("list_experiments")` -> [ListExperimentsPaginator](./paginators.md#listexperimentspaginator)
- `client.get_paginator("list_feature_groups")` -> [ListFeatureGroupsPaginator](./paginators.md#listfeaturegroupspaginator)
- `client.get_paginator("list_flow_definitions")` -> [ListFlowDefinitionsPaginator](./paginators.md#listflowdefinitionspaginator)
- `client.get_paginator("list_human_task_uis")` -> [ListHumanTaskUisPaginator](./paginators.md#listhumantaskuispaginator)
- `client.get_paginator("list_hyper_parameter_tuning_jobs")` -> [ListHyperParameterTuningJobsPaginator](./paginators.md#listhyperparametertuningjobspaginator)
- `client.get_paginator("list_image_versions")` -> [ListImageVersionsPaginator](./paginators.md#listimageversionspaginator)
- `client.get_paginator("list_images")` -> [ListImagesPaginator](./paginators.md#listimagespaginator)
- `client.get_paginator("list_inference_components")` -> [ListInferenceComponentsPaginator](./paginators.md#listinferencecomponentspaginator)
- `client.get_paginator("list_inference_experiments")` -> [ListInferenceExperimentsPaginator](./paginators.md#listinferenceexperimentspaginator)
- `client.get_paginator("list_inference_recommendations_job_steps")` -> [ListInferenceRecommendationsJobStepsPaginator](./paginators.md#listinferencerecommendationsjobstepspaginator)
- `client.get_paginator("list_inference_recommendations_jobs")` -> [ListInferenceRecommendationsJobsPaginator](./paginators.md#listinferencerecommendationsjobspaginator)
- `client.get_paginator("list_labeling_jobs_for_workteam")` -> [ListLabelingJobsForWorkteamPaginator](./paginators.md#listlabelingjobsforworkteampaginator)
- `client.get_paginator("list_labeling_jobs")` -> [ListLabelingJobsPaginator](./paginators.md#listlabelingjobspaginator)
- `client.get_paginator("list_lineage_groups")` -> [ListLineageGroupsPaginator](./paginators.md#listlineagegroupspaginator)
- `client.get_paginator("list_mlflow_tracking_servers")` -> [ListMlflowTrackingServersPaginator](./paginators.md#listmlflowtrackingserverspaginator)
- `client.get_paginator("list_model_bias_job_definitions")` -> [ListModelBiasJobDefinitionsPaginator](./paginators.md#listmodelbiasjobdefinitionspaginator)
- `client.get_paginator("list_model_card_export_jobs")` -> [ListModelCardExportJobsPaginator](./paginators.md#listmodelcardexportjobspaginator)
- `client.get_paginator("list_model_card_versions")` -> [ListModelCardVersionsPaginator](./paginators.md#listmodelcardversionspaginator)
- `client.get_paginator("list_model_cards")` -> [ListModelCardsPaginator](./paginators.md#listmodelcardspaginator)
- `client.get_paginator("list_model_explainability_job_definitions")` -> [ListModelExplainabilityJobDefinitionsPaginator](./paginators.md#listmodelexplainabilityjobdefinitionspaginator)
- `client.get_paginator("list_model_metadata")` -> [ListModelMetadataPaginator](./paginators.md#listmodelmetadatapaginator)
- `client.get_paginator("list_model_package_groups")` -> [ListModelPackageGroupsPaginator](./paginators.md#listmodelpackagegroupspaginator)
- `client.get_paginator("list_model_packages")` -> [ListModelPackagesPaginator](./paginators.md#listmodelpackagespaginator)
- `client.get_paginator("list_model_quality_job_definitions")` -> [ListModelQualityJobDefinitionsPaginator](./paginators.md#listmodelqualityjobdefinitionspaginator)
- `client.get_paginator("list_models")` -> [ListModelsPaginator](./paginators.md#listmodelspaginator)
- `client.get_paginator("list_monitoring_alert_history")` -> [ListMonitoringAlertHistoryPaginator](./paginators.md#listmonitoringalerthistorypaginator)
- `client.get_paginator("list_monitoring_alerts")` -> [ListMonitoringAlertsPaginator](./paginators.md#listmonitoringalertspaginator)
- `client.get_paginator("list_monitoring_executions")` -> [ListMonitoringExecutionsPaginator](./paginators.md#listmonitoringexecutionspaginator)
- `client.get_paginator("list_monitoring_schedules")` -> [ListMonitoringSchedulesPaginator](./paginators.md#listmonitoringschedulespaginator)
- `client.get_paginator("list_notebook_instance_lifecycle_configs")` -> [ListNotebookInstanceLifecycleConfigsPaginator](./paginators.md#listnotebookinstancelifecycleconfigspaginator)
- `client.get_paginator("list_notebook_instances")` -> [ListNotebookInstancesPaginator](./paginators.md#listnotebookinstancespaginator)
- `client.get_paginator("list_optimization_jobs")` -> [ListOptimizationJobsPaginator](./paginators.md#listoptimizationjobspaginator)
- `client.get_paginator("list_partner_apps")` -> [ListPartnerAppsPaginator](./paginators.md#listpartnerappspaginator)
- `client.get_paginator("list_pipeline_execution_steps")` -> [ListPipelineExecutionStepsPaginator](./paginators.md#listpipelineexecutionstepspaginator)
- `client.get_paginator("list_pipeline_executions")` -> [ListPipelineExecutionsPaginator](./paginators.md#listpipelineexecutionspaginator)
- `client.get_paginator("list_pipeline_parameters_for_execution")` -> [ListPipelineParametersForExecutionPaginator](./paginators.md#listpipelineparametersforexecutionpaginator)
- `client.get_paginator("list_pipelines")` -> [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
- `client.get_paginator("list_processing_jobs")` -> [ListProcessingJobsPaginator](./paginators.md#listprocessingjobspaginator)
- `client.get_paginator("list_resource_catalogs")` -> [ListResourceCatalogsPaginator](./paginators.md#listresourcecatalogspaginator)
- `client.get_paginator("list_spaces")` -> [ListSpacesPaginator](./paginators.md#listspacespaginator)
- `client.get_paginator("list_stage_devices")` -> [ListStageDevicesPaginator](./paginators.md#liststagedevicespaginator)
- `client.get_paginator("list_studio_lifecycle_configs")` -> [ListStudioLifecycleConfigsPaginator](./paginators.md#liststudiolifecycleconfigspaginator)
- `client.get_paginator("list_subscribed_workteams")` -> [ListSubscribedWorkteamsPaginator](./paginators.md#listsubscribedworkteamspaginator)
- `client.get_paginator("list_tags")` -> [ListTagsPaginator](./paginators.md#listtagspaginator)
- `client.get_paginator("list_training_jobs_for_hyper_parameter_tuning_job")` -> [ListTrainingJobsForHyperParameterTuningJobPaginator](./paginators.md#listtrainingjobsforhyperparametertuningjobpaginator)
- `client.get_paginator("list_training_jobs")` -> [ListTrainingJobsPaginator](./paginators.md#listtrainingjobspaginator)
- `client.get_paginator("list_training_plans")` -> [ListTrainingPlansPaginator](./paginators.md#listtrainingplanspaginator)
- `client.get_paginator("list_transform_jobs")` -> [ListTransformJobsPaginator](./paginators.md#listtransformjobspaginator)
- `client.get_paginator("list_trial_components")` -> [ListTrialComponentsPaginator](./paginators.md#listtrialcomponentspaginator)
- `client.get_paginator("list_trials")` -> [ListTrialsPaginator](./paginators.md#listtrialspaginator)
- `client.get_paginator("list_user_profiles")` -> [ListUserProfilesPaginator](./paginators.md#listuserprofilespaginator)
- `client.get_paginator("list_workforces")` -> [ListWorkforcesPaginator](./paginators.md#listworkforcespaginator)
- `client.get_paginator("list_workteams")` -> [ListWorkteamsPaginator](./paginators.md#listworkteamspaginator)
- `client.get_paginator("search")` -> [SearchPaginator](./paginators.md#searchpaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("sagemaker").get_waiter` method with overloads.

- `client.get_waiter("endpoint_deleted")` -> [EndpointDeletedWaiter](./waiters.md#endpointdeletedwaiter)
- `client.get_waiter("endpoint_in_service")` -> [EndpointInServiceWaiter](./waiters.md#endpointinservicewaiter)
- `client.get_waiter("image_created")` -> [ImageCreatedWaiter](./waiters.md#imagecreatedwaiter)
- `client.get_waiter("image_deleted")` -> [ImageDeletedWaiter](./waiters.md#imagedeletedwaiter)
- `client.get_waiter("image_updated")` -> [ImageUpdatedWaiter](./waiters.md#imageupdatedwaiter)
- `client.get_waiter("image_version_created")` -> [ImageVersionCreatedWaiter](./waiters.md#imageversioncreatedwaiter)
- `client.get_waiter("image_version_deleted")` -> [ImageVersionDeletedWaiter](./waiters.md#imageversiondeletedwaiter)
- `client.get_waiter("notebook_instance_deleted")` -> [NotebookInstanceDeletedWaiter](./waiters.md#notebookinstancedeletedwaiter)
- `client.get_waiter("notebook_instance_in_service")` -> [NotebookInstanceInServiceWaiter](./waiters.md#notebookinstanceinservicewaiter)
- `client.get_waiter("notebook_instance_stopped")` -> [NotebookInstanceStoppedWaiter](./waiters.md#notebookinstancestoppedwaiter)
- `client.get_waiter("processing_job_completed_or_stopped")` -> [ProcessingJobCompletedOrStoppedWaiter](./waiters.md#processingjobcompletedorstoppedwaiter)
- `client.get_waiter("training_job_completed_or_stopped")` -> [TrainingJobCompletedOrStoppedWaiter](./waiters.md#trainingjobcompletedorstoppedwaiter)
- `client.get_waiter("transform_job_completed_or_stopped")` -> [TransformJobCompletedOrStoppedWaiter](./waiters.md#transformjobcompletedorstoppedwaiter)

