# CleanRoomsMLClient

> [Index](../README.md) > [CleanRoomsML](./README.md) > CleanRoomsMLClient

!!! note ""

    Auto-generated documentation for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#cleanroomsml)
    type annotations stubs module [types-aiobotocore-cleanroomsml](https://pypi.org/project/types-aiobotocore-cleanroomsml/).

## CleanRoomsMLClient

Type annotations and code completion for `#!python session.create_client("cleanroomsml")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client)

```python
# CleanRoomsMLClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cleanroomsml.client import CleanRoomsMLClient

session = get_session()
async with session.create_client("cleanroomsml") as client:
    client: CleanRoomsMLClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cleanroomsml").exceptions` structure.

```python
# CleanRoomsMLClient.exceptions usage example

async with session.create_client("cleanroomsml") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# CleanRoomsMLClient usage type checking example

from types_aiobotocore_cleanroomsml.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("cleanroomsml").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("cleanroomsml").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/generate_presigned_url.html)

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


### cancel\_trained\_model

Submits a request to cancel the trained model job.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").cancel_trained_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/cancel_trained_model.html)

```python
# cancel_trained_model method definition

await def cancel_trained_model(
    self,
    *,
    membershipIdentifier: str,
    trainedModelArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_trained_model method usage example with argument unpacking

kwargs: CancelTrainedModelRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "trainedModelArn": ...,
}

parent.cancel_trained_model(**kwargs)
```

1. See [:material-code-braces: CancelTrainedModelRequestRequestTypeDef](./type_defs.md#canceltrainedmodelrequestrequesttypedef) 

### cancel\_trained\_model\_inference\_job

Submits a request to cancel a trained model inference job.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").cancel_trained_model_inference_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/cancel_trained_model_inference_job.html)

```python
# cancel_trained_model_inference_job method definition

await def cancel_trained_model_inference_job(
    self,
    *,
    membershipIdentifier: str,
    trainedModelInferenceJobArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# cancel_trained_model_inference_job method usage example with argument unpacking

kwargs: CancelTrainedModelInferenceJobRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "trainedModelInferenceJobArn": ...,
}

parent.cancel_trained_model_inference_job(**kwargs)
```

1. See [:material-code-braces: CancelTrainedModelInferenceJobRequestRequestTypeDef](./type_defs.md#canceltrainedmodelinferencejobrequestrequesttypedef) 

### create\_audience\_model

Defines the information necessary to create an audience model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").create_audience_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/create_audience_model.html)

```python
# create_audience_model method definition

await def create_audience_model(
    self,
    *,
    name: str,
    trainingDatasetArn: str,
    trainingDataStartTime: TimestampTypeDef = ...,
    trainingDataEndTime: TimestampTypeDef = ...,
    kmsKeyArn: str = ...,
    tags: Mapping[str, str] = ...,
    description: str = ...,
) -> CreateAudienceModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAudienceModelResponseTypeDef](./type_defs.md#createaudiencemodelresponsetypedef) 


```python
# create_audience_model method usage example with argument unpacking

kwargs: CreateAudienceModelRequestRequestTypeDef = {  # (1)
    "name": ...,
    "trainingDatasetArn": ...,
}

parent.create_audience_model(**kwargs)
```

1. See [:material-code-braces: CreateAudienceModelRequestRequestTypeDef](./type_defs.md#createaudiencemodelrequestrequesttypedef) 

### create\_configured\_audience\_model

Defines the information necessary to create a configured audience model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").create_configured_audience_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/create_configured_audience_model.html)

```python
# create_configured_audience_model method definition

await def create_configured_audience_model(
    self,
    *,
    name: str,
    audienceModelArn: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,  # (1)
    sharedAudienceMetrics: Sequence[SharedAudienceMetricsType],  # (2)
    description: str = ...,
    minMatchingSeedSize: int = ...,
    audienceSizeConfig: AudienceSizeConfigTypeDef = ...,  # (3)
    tags: Mapping[str, str] = ...,
    childResourceTagOnCreatePolicy: TagOnCreatePolicyType = ...,  # (4)
) -> CreateConfiguredAudienceModelResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
3. See [:material-code-braces: AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef) 
4. See [:material-code-brackets: TagOnCreatePolicyType](./literals.md#tagoncreatepolicytype) 
5. See [:material-code-braces: CreateConfiguredAudienceModelResponseTypeDef](./type_defs.md#createconfiguredaudiencemodelresponsetypedef) 


```python
# create_configured_audience_model method usage example with argument unpacking

kwargs: CreateConfiguredAudienceModelRequestRequestTypeDef = {  # (1)
    "name": ...,
    "audienceModelArn": ...,
    "outputConfig": ...,
    "sharedAudienceMetrics": ...,
}

parent.create_configured_audience_model(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#createconfiguredaudiencemodelrequestrequesttypedef) 

### create\_configured\_model\_algorithm

Creates a configured model algorithm using a container image stored in an ECR
repository.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").create_configured_model_algorithm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/create_configured_model_algorithm.html)

```python
# create_configured_model_algorithm method definition

await def create_configured_model_algorithm(
    self,
    *,
    name: str,
    roleArn: str,
    description: str = ...,
    trainingContainerConfig: ContainerConfigTypeDef = ...,  # (1)
    inferenceContainerConfig: InferenceContainerConfigTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
    kmsKeyArn: str = ...,
) -> CreateConfiguredModelAlgorithmResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ContainerConfigTypeDef](./type_defs.md#containerconfigtypedef) 
2. See [:material-code-braces: InferenceContainerConfigTypeDef](./type_defs.md#inferencecontainerconfigtypedef) 
3. See [:material-code-braces: CreateConfiguredModelAlgorithmResponseTypeDef](./type_defs.md#createconfiguredmodelalgorithmresponsetypedef) 


```python
# create_configured_model_algorithm method usage example with argument unpacking

kwargs: CreateConfiguredModelAlgorithmRequestRequestTypeDef = {  # (1)
    "name": ...,
    "roleArn": ...,
}

parent.create_configured_model_algorithm(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredModelAlgorithmRequestRequestTypeDef](./type_defs.md#createconfiguredmodelalgorithmrequestrequesttypedef) 

### create\_configured\_model\_algorithm\_association

Associates a configured model algorithm to a collaboration for use by any
member of the collaboration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").create_configured_model_algorithm_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/create_configured_model_algorithm_association.html)

```python
# create_configured_model_algorithm_association method definition

await def create_configured_model_algorithm_association(
    self,
    *,
    membershipIdentifier: str,
    configuredModelAlgorithmArn: str,
    name: str,
    description: str = ...,
    privacyConfiguration: PrivacyConfigurationTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateConfiguredModelAlgorithmAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PrivacyConfigurationTypeDef](./type_defs.md#privacyconfigurationtypedef) 
2. See [:material-code-braces: CreateConfiguredModelAlgorithmAssociationResponseTypeDef](./type_defs.md#createconfiguredmodelalgorithmassociationresponsetypedef) 


```python
# create_configured_model_algorithm_association method usage example with argument unpacking

kwargs: CreateConfiguredModelAlgorithmAssociationRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "configuredModelAlgorithmArn": ...,
    "name": ...,
}

parent.create_configured_model_algorithm_association(**kwargs)
```

1. See [:material-code-braces: CreateConfiguredModelAlgorithmAssociationRequestRequestTypeDef](./type_defs.md#createconfiguredmodelalgorithmassociationrequestrequesttypedef) 

### create\_ml\_input\_channel

Provides the information to create an ML input channel.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").create_ml_input_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/create_ml_input_channel.html)

```python
# create_ml_input_channel method definition

await def create_ml_input_channel(
    self,
    *,
    membershipIdentifier: str,
    configuredModelAlgorithmAssociations: Sequence[str],
    inputChannel: InputChannelTypeDef,  # (1)
    name: str,
    retentionInDays: int,
    description: str = ...,
    kmsKeyArn: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateMLInputChannelResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InputChannelTypeDef](./type_defs.md#inputchanneltypedef) 
2. See [:material-code-braces: CreateMLInputChannelResponseTypeDef](./type_defs.md#createmlinputchannelresponsetypedef) 


```python
# create_ml_input_channel method usage example with argument unpacking

kwargs: CreateMLInputChannelRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "configuredModelAlgorithmAssociations": ...,
    "inputChannel": ...,
    "name": ...,
    "retentionInDays": ...,
}

parent.create_ml_input_channel(**kwargs)
```

1. See [:material-code-braces: CreateMLInputChannelRequestRequestTypeDef](./type_defs.md#createmlinputchannelrequestrequesttypedef) 

### create\_trained\_model

Creates a trained model from an associated configured model algorithm using
data from any member of the collaboration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").create_trained_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/create_trained_model.html)

```python
# create_trained_model method definition

await def create_trained_model(
    self,
    *,
    membershipIdentifier: str,
    name: str,
    configuredModelAlgorithmAssociationArn: str,
    resourceConfig: ResourceConfigTypeDef,  # (1)
    dataChannels: Sequence[ModelTrainingDataChannelTypeDef],  # (2)
    hyperparameters: Mapping[str, str] = ...,
    environment: Mapping[str, str] = ...,
    stoppingCondition: StoppingConditionTypeDef = ...,  # (3)
    description: str = ...,
    kmsKeyArn: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateTrainedModelResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) 
2. See [:material-code-braces: ModelTrainingDataChannelTypeDef](./type_defs.md#modeltrainingdatachanneltypedef) 
3. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
4. See [:material-code-braces: CreateTrainedModelResponseTypeDef](./type_defs.md#createtrainedmodelresponsetypedef) 


```python
# create_trained_model method usage example with argument unpacking

kwargs: CreateTrainedModelRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "name": ...,
    "configuredModelAlgorithmAssociationArn": ...,
    "resourceConfig": ...,
    "dataChannels": ...,
}

parent.create_trained_model(**kwargs)
```

1. See [:material-code-braces: CreateTrainedModelRequestRequestTypeDef](./type_defs.md#createtrainedmodelrequestrequesttypedef) 

### create\_training\_dataset

Defines the information necessary to create a training dataset.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").create_training_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/create_training_dataset.html)

```python
# create_training_dataset method definition

await def create_training_dataset(
    self,
    *,
    name: str,
    roleArn: str,
    trainingData: Sequence[DatasetUnionTypeDef],  # (1)
    tags: Mapping[str, str] = ...,
    description: str = ...,
) -> CreateTrainingDatasetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) [:material-code-braces: DatasetOutputTypeDef](./type_defs.md#datasetoutputtypedef) 
2. See [:material-code-braces: CreateTrainingDatasetResponseTypeDef](./type_defs.md#createtrainingdatasetresponsetypedef) 


```python
# create_training_dataset method usage example with argument unpacking

kwargs: CreateTrainingDatasetRequestRequestTypeDef = {  # (1)
    "name": ...,
    "roleArn": ...,
    "trainingData": ...,
}

parent.create_training_dataset(**kwargs)
```

1. See [:material-code-braces: CreateTrainingDatasetRequestRequestTypeDef](./type_defs.md#createtrainingdatasetrequestrequesttypedef) 

### delete\_audience\_generation\_job

Deletes the specified audience generation job, and removes all data associated
with the job.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_audience_generation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/delete_audience_generation_job.html)

```python
# delete_audience_generation_job method definition

await def delete_audience_generation_job(
    self,
    *,
    audienceGenerationJobArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_audience_generation_job method usage example with argument unpacking

kwargs: DeleteAudienceGenerationJobRequestRequestTypeDef = {  # (1)
    "audienceGenerationJobArn": ...,
}

parent.delete_audience_generation_job(**kwargs)
```

1. See [:material-code-braces: DeleteAudienceGenerationJobRequestRequestTypeDef](./type_defs.md#deleteaudiencegenerationjobrequestrequesttypedef) 

### delete\_audience\_model

Specifies an audience model that you want to delete.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_audience_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/delete_audience_model.html)

```python
# delete_audience_model method definition

await def delete_audience_model(
    self,
    *,
    audienceModelArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_audience_model method usage example with argument unpacking

kwargs: DeleteAudienceModelRequestRequestTypeDef = {  # (1)
    "audienceModelArn": ...,
}

parent.delete_audience_model(**kwargs)
```

1. See [:material-code-braces: DeleteAudienceModelRequestRequestTypeDef](./type_defs.md#deleteaudiencemodelrequestrequesttypedef) 

### delete\_configured\_audience\_model

Deletes the specified configured audience model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_configured_audience_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/delete_configured_audience_model.html)

```python
# delete_configured_audience_model method definition

await def delete_configured_audience_model(
    self,
    *,
    configuredAudienceModelArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_configured_audience_model method usage example with argument unpacking

kwargs: DeleteConfiguredAudienceModelRequestRequestTypeDef = {  # (1)
    "configuredAudienceModelArn": ...,
}

parent.delete_configured_audience_model(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#deleteconfiguredaudiencemodelrequestrequesttypedef) 

### delete\_configured\_audience\_model\_policy

Deletes the specified configured audience model policy.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_configured_audience_model_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/delete_configured_audience_model_policy.html)

```python
# delete_configured_audience_model_policy method definition

await def delete_configured_audience_model_policy(
    self,
    *,
    configuredAudienceModelArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_configured_audience_model_policy method usage example with argument unpacking

kwargs: DeleteConfiguredAudienceModelPolicyRequestRequestTypeDef = {  # (1)
    "configuredAudienceModelArn": ...,
}

parent.delete_configured_audience_model_policy(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredAudienceModelPolicyRequestRequestTypeDef](./type_defs.md#deleteconfiguredaudiencemodelpolicyrequestrequesttypedef) 

### delete\_configured\_model\_algorithm

Deletes a configured model algorithm.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_configured_model_algorithm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/delete_configured_model_algorithm.html)

```python
# delete_configured_model_algorithm method definition

await def delete_configured_model_algorithm(
    self,
    *,
    configuredModelAlgorithmArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_configured_model_algorithm method usage example with argument unpacking

kwargs: DeleteConfiguredModelAlgorithmRequestRequestTypeDef = {  # (1)
    "configuredModelAlgorithmArn": ...,
}

parent.delete_configured_model_algorithm(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredModelAlgorithmRequestRequestTypeDef](./type_defs.md#deleteconfiguredmodelalgorithmrequestrequesttypedef) 

### delete\_configured\_model\_algorithm\_association

Deletes a configured model algorithm association.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_configured_model_algorithm_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/delete_configured_model_algorithm_association.html)

```python
# delete_configured_model_algorithm_association method definition

await def delete_configured_model_algorithm_association(
    self,
    *,
    configuredModelAlgorithmAssociationArn: str,
    membershipIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_configured_model_algorithm_association method usage example with argument unpacking

kwargs: DeleteConfiguredModelAlgorithmAssociationRequestRequestTypeDef = {  # (1)
    "configuredModelAlgorithmAssociationArn": ...,
    "membershipIdentifier": ...,
}

parent.delete_configured_model_algorithm_association(**kwargs)
```

1. See [:material-code-braces: DeleteConfiguredModelAlgorithmAssociationRequestRequestTypeDef](./type_defs.md#deleteconfiguredmodelalgorithmassociationrequestrequesttypedef) 

### delete\_ml\_configuration

Deletes a ML modeling configuration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_ml_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/delete_ml_configuration.html)

```python
# delete_ml_configuration method definition

await def delete_ml_configuration(
    self,
    *,
    membershipIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_ml_configuration method usage example with argument unpacking

kwargs: DeleteMLConfigurationRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.delete_ml_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteMLConfigurationRequestRequestTypeDef](./type_defs.md#deletemlconfigurationrequestrequesttypedef) 

### delete\_ml\_input\_channel\_data

Provides the information necessary to delete an ML input channel.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_ml_input_channel_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/delete_ml_input_channel_data.html)

```python
# delete_ml_input_channel_data method definition

await def delete_ml_input_channel_data(
    self,
    *,
    mlInputChannelArn: str,
    membershipIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_ml_input_channel_data method usage example with argument unpacking

kwargs: DeleteMLInputChannelDataRequestRequestTypeDef = {  # (1)
    "mlInputChannelArn": ...,
    "membershipIdentifier": ...,
}

parent.delete_ml_input_channel_data(**kwargs)
```

1. See [:material-code-braces: DeleteMLInputChannelDataRequestRequestTypeDef](./type_defs.md#deletemlinputchanneldatarequestrequesttypedef) 

### delete\_trained\_model\_output

Deletes the output of a trained model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_trained_model_output` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/delete_trained_model_output.html)

```python
# delete_trained_model_output method definition

await def delete_trained_model_output(
    self,
    *,
    trainedModelArn: str,
    membershipIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_trained_model_output method usage example with argument unpacking

kwargs: DeleteTrainedModelOutputRequestRequestTypeDef = {  # (1)
    "trainedModelArn": ...,
    "membershipIdentifier": ...,
}

parent.delete_trained_model_output(**kwargs)
```

1. See [:material-code-braces: DeleteTrainedModelOutputRequestRequestTypeDef](./type_defs.md#deletetrainedmodeloutputrequestrequesttypedef) 

### delete\_training\_dataset

Specifies a training dataset that you want to delete.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_training_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/delete_training_dataset.html)

```python
# delete_training_dataset method definition

await def delete_training_dataset(
    self,
    *,
    trainingDatasetArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_training_dataset method usage example with argument unpacking

kwargs: DeleteTrainingDatasetRequestRequestTypeDef = {  # (1)
    "trainingDatasetArn": ...,
}

parent.delete_training_dataset(**kwargs)
```

1. See [:material-code-braces: DeleteTrainingDatasetRequestRequestTypeDef](./type_defs.md#deletetrainingdatasetrequestrequesttypedef) 

### get\_audience\_generation\_job

Returns information about an audience generation job.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_audience_generation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_audience_generation_job.html)

```python
# get_audience_generation_job method definition

await def get_audience_generation_job(
    self,
    *,
    audienceGenerationJobArn: str,
) -> GetAudienceGenerationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAudienceGenerationJobResponseTypeDef](./type_defs.md#getaudiencegenerationjobresponsetypedef) 


```python
# get_audience_generation_job method usage example with argument unpacking

kwargs: GetAudienceGenerationJobRequestRequestTypeDef = {  # (1)
    "audienceGenerationJobArn": ...,
}

parent.get_audience_generation_job(**kwargs)
```

1. See [:material-code-braces: GetAudienceGenerationJobRequestRequestTypeDef](./type_defs.md#getaudiencegenerationjobrequestrequesttypedef) 

### get\_audience\_model

Returns information about an audience model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_audience_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_audience_model.html)

```python
# get_audience_model method definition

await def get_audience_model(
    self,
    *,
    audienceModelArn: str,
) -> GetAudienceModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAudienceModelResponseTypeDef](./type_defs.md#getaudiencemodelresponsetypedef) 


```python
# get_audience_model method usage example with argument unpacking

kwargs: GetAudienceModelRequestRequestTypeDef = {  # (1)
    "audienceModelArn": ...,
}

parent.get_audience_model(**kwargs)
```

1. See [:material-code-braces: GetAudienceModelRequestRequestTypeDef](./type_defs.md#getaudiencemodelrequestrequesttypedef) 

### get\_collaboration\_configured\_model\_algorithm\_association

Returns information about the configured model algorithm association in a
collaboration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_collaboration_configured_model_algorithm_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_collaboration_configured_model_algorithm_association.html)

```python
# get_collaboration_configured_model_algorithm_association method definition

await def get_collaboration_configured_model_algorithm_association(
    self,
    *,
    configuredModelAlgorithmAssociationArn: str,
    collaborationIdentifier: str,
) -> GetCollaborationConfiguredModelAlgorithmAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCollaborationConfiguredModelAlgorithmAssociationResponseTypeDef](./type_defs.md#getcollaborationconfiguredmodelalgorithmassociationresponsetypedef) 


```python
# get_collaboration_configured_model_algorithm_association method usage example with argument unpacking

kwargs: GetCollaborationConfiguredModelAlgorithmAssociationRequestRequestTypeDef = {  # (1)
    "configuredModelAlgorithmAssociationArn": ...,
    "collaborationIdentifier": ...,
}

parent.get_collaboration_configured_model_algorithm_association(**kwargs)
```

1. See [:material-code-braces: GetCollaborationConfiguredModelAlgorithmAssociationRequestRequestTypeDef](./type_defs.md#getcollaborationconfiguredmodelalgorithmassociationrequestrequesttypedef) 

### get\_collaboration\_ml\_input\_channel

Returns information about a specific ML input channel in a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_collaboration_ml_input_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_collaboration_ml_input_channel.html)

```python
# get_collaboration_ml_input_channel method definition

await def get_collaboration_ml_input_channel(
    self,
    *,
    mlInputChannelArn: str,
    collaborationIdentifier: str,
) -> GetCollaborationMLInputChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCollaborationMLInputChannelResponseTypeDef](./type_defs.md#getcollaborationmlinputchannelresponsetypedef) 


```python
# get_collaboration_ml_input_channel method usage example with argument unpacking

kwargs: GetCollaborationMLInputChannelRequestRequestTypeDef = {  # (1)
    "mlInputChannelArn": ...,
    "collaborationIdentifier": ...,
}

parent.get_collaboration_ml_input_channel(**kwargs)
```

1. See [:material-code-braces: GetCollaborationMLInputChannelRequestRequestTypeDef](./type_defs.md#getcollaborationmlinputchannelrequestrequesttypedef) 

### get\_collaboration\_trained\_model

Returns information about a trained model in a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_collaboration_trained_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_collaboration_trained_model.html)

```python
# get_collaboration_trained_model method definition

await def get_collaboration_trained_model(
    self,
    *,
    trainedModelArn: str,
    collaborationIdentifier: str,
) -> GetCollaborationTrainedModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCollaborationTrainedModelResponseTypeDef](./type_defs.md#getcollaborationtrainedmodelresponsetypedef) 


```python
# get_collaboration_trained_model method usage example with argument unpacking

kwargs: GetCollaborationTrainedModelRequestRequestTypeDef = {  # (1)
    "trainedModelArn": ...,
    "collaborationIdentifier": ...,
}

parent.get_collaboration_trained_model(**kwargs)
```

1. See [:material-code-braces: GetCollaborationTrainedModelRequestRequestTypeDef](./type_defs.md#getcollaborationtrainedmodelrequestrequesttypedef) 

### get\_configured\_audience\_model

Returns information about a specified configured audience model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_configured_audience_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_configured_audience_model.html)

```python
# get_configured_audience_model method definition

await def get_configured_audience_model(
    self,
    *,
    configuredAudienceModelArn: str,
) -> GetConfiguredAudienceModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfiguredAudienceModelResponseTypeDef](./type_defs.md#getconfiguredaudiencemodelresponsetypedef) 


```python
# get_configured_audience_model method usage example with argument unpacking

kwargs: GetConfiguredAudienceModelRequestRequestTypeDef = {  # (1)
    "configuredAudienceModelArn": ...,
}

parent.get_configured_audience_model(**kwargs)
```

1. See [:material-code-braces: GetConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#getconfiguredaudiencemodelrequestrequesttypedef) 

### get\_configured\_audience\_model\_policy

Returns information about a configured audience model policy.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_configured_audience_model_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_configured_audience_model_policy.html)

```python
# get_configured_audience_model_policy method definition

await def get_configured_audience_model_policy(
    self,
    *,
    configuredAudienceModelArn: str,
) -> GetConfiguredAudienceModelPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfiguredAudienceModelPolicyResponseTypeDef](./type_defs.md#getconfiguredaudiencemodelpolicyresponsetypedef) 


```python
# get_configured_audience_model_policy method usage example with argument unpacking

kwargs: GetConfiguredAudienceModelPolicyRequestRequestTypeDef = {  # (1)
    "configuredAudienceModelArn": ...,
}

parent.get_configured_audience_model_policy(**kwargs)
```

1. See [:material-code-braces: GetConfiguredAudienceModelPolicyRequestRequestTypeDef](./type_defs.md#getconfiguredaudiencemodelpolicyrequestrequesttypedef) 

### get\_configured\_model\_algorithm

Returns information about a configured model algorithm.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_configured_model_algorithm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_configured_model_algorithm.html)

```python
# get_configured_model_algorithm method definition

await def get_configured_model_algorithm(
    self,
    *,
    configuredModelAlgorithmArn: str,
) -> GetConfiguredModelAlgorithmResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfiguredModelAlgorithmResponseTypeDef](./type_defs.md#getconfiguredmodelalgorithmresponsetypedef) 


```python
# get_configured_model_algorithm method usage example with argument unpacking

kwargs: GetConfiguredModelAlgorithmRequestRequestTypeDef = {  # (1)
    "configuredModelAlgorithmArn": ...,
}

parent.get_configured_model_algorithm(**kwargs)
```

1. See [:material-code-braces: GetConfiguredModelAlgorithmRequestRequestTypeDef](./type_defs.md#getconfiguredmodelalgorithmrequestrequesttypedef) 

### get\_configured\_model\_algorithm\_association

Returns information about a configured model algorithm association.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_configured_model_algorithm_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_configured_model_algorithm_association.html)

```python
# get_configured_model_algorithm_association method definition

await def get_configured_model_algorithm_association(
    self,
    *,
    configuredModelAlgorithmAssociationArn: str,
    membershipIdentifier: str,
) -> GetConfiguredModelAlgorithmAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfiguredModelAlgorithmAssociationResponseTypeDef](./type_defs.md#getconfiguredmodelalgorithmassociationresponsetypedef) 


```python
# get_configured_model_algorithm_association method usage example with argument unpacking

kwargs: GetConfiguredModelAlgorithmAssociationRequestRequestTypeDef = {  # (1)
    "configuredModelAlgorithmAssociationArn": ...,
    "membershipIdentifier": ...,
}

parent.get_configured_model_algorithm_association(**kwargs)
```

1. See [:material-code-braces: GetConfiguredModelAlgorithmAssociationRequestRequestTypeDef](./type_defs.md#getconfiguredmodelalgorithmassociationrequestrequesttypedef) 

### get\_ml\_configuration

Returns information about a specific ML configuration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_ml_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_ml_configuration.html)

```python
# get_ml_configuration method definition

await def get_ml_configuration(
    self,
    *,
    membershipIdentifier: str,
) -> GetMLConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMLConfigurationResponseTypeDef](./type_defs.md#getmlconfigurationresponsetypedef) 


```python
# get_ml_configuration method usage example with argument unpacking

kwargs: GetMLConfigurationRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.get_ml_configuration(**kwargs)
```

1. See [:material-code-braces: GetMLConfigurationRequestRequestTypeDef](./type_defs.md#getmlconfigurationrequestrequesttypedef) 

### get\_ml\_input\_channel

Returns information about an ML input channel.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_ml_input_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_ml_input_channel.html)

```python
# get_ml_input_channel method definition

await def get_ml_input_channel(
    self,
    *,
    mlInputChannelArn: str,
    membershipIdentifier: str,
) -> GetMLInputChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMLInputChannelResponseTypeDef](./type_defs.md#getmlinputchannelresponsetypedef) 


```python
# get_ml_input_channel method usage example with argument unpacking

kwargs: GetMLInputChannelRequestRequestTypeDef = {  # (1)
    "mlInputChannelArn": ...,
    "membershipIdentifier": ...,
}

parent.get_ml_input_channel(**kwargs)
```

1. See [:material-code-braces: GetMLInputChannelRequestRequestTypeDef](./type_defs.md#getmlinputchannelrequestrequesttypedef) 

### get\_trained\_model

Returns information about a trained model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_trained_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_trained_model.html)

```python
# get_trained_model method definition

await def get_trained_model(
    self,
    *,
    trainedModelArn: str,
    membershipIdentifier: str,
) -> GetTrainedModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrainedModelResponseTypeDef](./type_defs.md#gettrainedmodelresponsetypedef) 


```python
# get_trained_model method usage example with argument unpacking

kwargs: GetTrainedModelRequestRequestTypeDef = {  # (1)
    "trainedModelArn": ...,
    "membershipIdentifier": ...,
}

parent.get_trained_model(**kwargs)
```

1. See [:material-code-braces: GetTrainedModelRequestRequestTypeDef](./type_defs.md#gettrainedmodelrequestrequesttypedef) 

### get\_trained\_model\_inference\_job

Returns information about a trained model inference job.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_trained_model_inference_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_trained_model_inference_job.html)

```python
# get_trained_model_inference_job method definition

await def get_trained_model_inference_job(
    self,
    *,
    membershipIdentifier: str,
    trainedModelInferenceJobArn: str,
) -> GetTrainedModelInferenceJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrainedModelInferenceJobResponseTypeDef](./type_defs.md#gettrainedmodelinferencejobresponsetypedef) 


```python
# get_trained_model_inference_job method usage example with argument unpacking

kwargs: GetTrainedModelInferenceJobRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "trainedModelInferenceJobArn": ...,
}

parent.get_trained_model_inference_job(**kwargs)
```

1. See [:material-code-braces: GetTrainedModelInferenceJobRequestRequestTypeDef](./type_defs.md#gettrainedmodelinferencejobrequestrequesttypedef) 

### get\_training\_dataset

Returns information about a training dataset.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_training_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/get_training_dataset.html)

```python
# get_training_dataset method definition

await def get_training_dataset(
    self,
    *,
    trainingDatasetArn: str,
) -> GetTrainingDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTrainingDatasetResponseTypeDef](./type_defs.md#gettrainingdatasetresponsetypedef) 


```python
# get_training_dataset method usage example with argument unpacking

kwargs: GetTrainingDatasetRequestRequestTypeDef = {  # (1)
    "trainingDatasetArn": ...,
}

parent.get_training_dataset(**kwargs)
```

1. See [:material-code-braces: GetTrainingDatasetRequestRequestTypeDef](./type_defs.md#gettrainingdatasetrequestrequesttypedef) 

### list\_audience\_export\_jobs

Returns a list of the audience export jobs.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_audience_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_audience_export_jobs.html)

```python
# list_audience_export_jobs method definition

await def list_audience_export_jobs(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    audienceGenerationJobArn: str = ...,
) -> ListAudienceExportJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAudienceExportJobsResponseTypeDef](./type_defs.md#listaudienceexportjobsresponsetypedef) 


```python
# list_audience_export_jobs method usage example with argument unpacking

kwargs: ListAudienceExportJobsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_audience_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListAudienceExportJobsRequestRequestTypeDef](./type_defs.md#listaudienceexportjobsrequestrequesttypedef) 

### list\_audience\_generation\_jobs

Returns a list of audience generation jobs.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_audience_generation_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_audience_generation_jobs.html)

```python
# list_audience_generation_jobs method definition

await def list_audience_generation_jobs(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    configuredAudienceModelArn: str = ...,
    collaborationId: str = ...,
) -> ListAudienceGenerationJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAudienceGenerationJobsResponseTypeDef](./type_defs.md#listaudiencegenerationjobsresponsetypedef) 


```python
# list_audience_generation_jobs method usage example with argument unpacking

kwargs: ListAudienceGenerationJobsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_audience_generation_jobs(**kwargs)
```

1. See [:material-code-braces: ListAudienceGenerationJobsRequestRequestTypeDef](./type_defs.md#listaudiencegenerationjobsrequestrequesttypedef) 

### list\_audience\_models

Returns a list of audience models.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_audience_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_audience_models.html)

```python
# list_audience_models method definition

await def list_audience_models(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAudienceModelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAudienceModelsResponseTypeDef](./type_defs.md#listaudiencemodelsresponsetypedef) 


```python
# list_audience_models method usage example with argument unpacking

kwargs: ListAudienceModelsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_audience_models(**kwargs)
```

1. See [:material-code-braces: ListAudienceModelsRequestRequestTypeDef](./type_defs.md#listaudiencemodelsrequestrequesttypedef) 

### list\_collaboration\_configured\_model\_algorithm\_associations

Returns a list of the configured model algorithm associations in a
collaboration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_collaboration_configured_model_algorithm_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_collaboration_configured_model_algorithm_associations.html)

```python
# list_collaboration_configured_model_algorithm_associations method definition

await def list_collaboration_configured_model_algorithm_associations(
    self,
    *,
    collaborationIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCollaborationConfiguredModelAlgorithmAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCollaborationConfiguredModelAlgorithmAssociationsResponseTypeDef](./type_defs.md#listcollaborationconfiguredmodelalgorithmassociationsresponsetypedef) 


```python
# list_collaboration_configured_model_algorithm_associations method usage example with argument unpacking

kwargs: ListCollaborationConfiguredModelAlgorithmAssociationsRequestRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_collaboration_configured_model_algorithm_associations(**kwargs)
```

1. See [:material-code-braces: ListCollaborationConfiguredModelAlgorithmAssociationsRequestRequestTypeDef](./type_defs.md#listcollaborationconfiguredmodelalgorithmassociationsrequestrequesttypedef) 

### list\_collaboration\_ml\_input\_channels

Returns a list of the ML input channels in a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_collaboration_ml_input_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_collaboration_ml_input_channels.html)

```python
# list_collaboration_ml_input_channels method definition

await def list_collaboration_ml_input_channels(
    self,
    *,
    collaborationIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCollaborationMLInputChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCollaborationMLInputChannelsResponseTypeDef](./type_defs.md#listcollaborationmlinputchannelsresponsetypedef) 


```python
# list_collaboration_ml_input_channels method usage example with argument unpacking

kwargs: ListCollaborationMLInputChannelsRequestRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_collaboration_ml_input_channels(**kwargs)
```

1. See [:material-code-braces: ListCollaborationMLInputChannelsRequestRequestTypeDef](./type_defs.md#listcollaborationmlinputchannelsrequestrequesttypedef) 

### list\_collaboration\_trained\_model\_export\_jobs

Returns a list of the export jobs for a trained model in a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_collaboration_trained_model_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_collaboration_trained_model_export_jobs.html)

```python
# list_collaboration_trained_model_export_jobs method definition

await def list_collaboration_trained_model_export_jobs(
    self,
    *,
    collaborationIdentifier: str,
    trainedModelArn: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCollaborationTrainedModelExportJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCollaborationTrainedModelExportJobsResponseTypeDef](./type_defs.md#listcollaborationtrainedmodelexportjobsresponsetypedef) 


```python
# list_collaboration_trained_model_export_jobs method usage example with argument unpacking

kwargs: ListCollaborationTrainedModelExportJobsRequestRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
    "trainedModelArn": ...,
}

parent.list_collaboration_trained_model_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListCollaborationTrainedModelExportJobsRequestRequestTypeDef](./type_defs.md#listcollaborationtrainedmodelexportjobsrequestrequesttypedef) 

### list\_collaboration\_trained\_model\_inference\_jobs

Returns a list of trained model inference jobs in a specified collaboration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_collaboration_trained_model_inference_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_collaboration_trained_model_inference_jobs.html)

```python
# list_collaboration_trained_model_inference_jobs method definition

await def list_collaboration_trained_model_inference_jobs(
    self,
    *,
    collaborationIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
    trainedModelArn: str = ...,
) -> ListCollaborationTrainedModelInferenceJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCollaborationTrainedModelInferenceJobsResponseTypeDef](./type_defs.md#listcollaborationtrainedmodelinferencejobsresponsetypedef) 


```python
# list_collaboration_trained_model_inference_jobs method usage example with argument unpacking

kwargs: ListCollaborationTrainedModelInferenceJobsRequestRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_collaboration_trained_model_inference_jobs(**kwargs)
```

1. See [:material-code-braces: ListCollaborationTrainedModelInferenceJobsRequestRequestTypeDef](./type_defs.md#listcollaborationtrainedmodelinferencejobsrequestrequesttypedef) 

### list\_collaboration\_trained\_models

Returns a list of the trained models in a collaboration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_collaboration_trained_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_collaboration_trained_models.html)

```python
# list_collaboration_trained_models method definition

await def list_collaboration_trained_models(
    self,
    *,
    collaborationIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCollaborationTrainedModelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCollaborationTrainedModelsResponseTypeDef](./type_defs.md#listcollaborationtrainedmodelsresponsetypedef) 


```python
# list_collaboration_trained_models method usage example with argument unpacking

kwargs: ListCollaborationTrainedModelsRequestRequestTypeDef = {  # (1)
    "collaborationIdentifier": ...,
}

parent.list_collaboration_trained_models(**kwargs)
```

1. See [:material-code-braces: ListCollaborationTrainedModelsRequestRequestTypeDef](./type_defs.md#listcollaborationtrainedmodelsrequestrequesttypedef) 

### list\_configured\_audience\_models

Returns a list of the configured audience models.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_configured_audience_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_configured_audience_models.html)

```python
# list_configured_audience_models method definition

await def list_configured_audience_models(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListConfiguredAudienceModelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfiguredAudienceModelsResponseTypeDef](./type_defs.md#listconfiguredaudiencemodelsresponsetypedef) 


```python
# list_configured_audience_models method usage example with argument unpacking

kwargs: ListConfiguredAudienceModelsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_configured_audience_models(**kwargs)
```

1. See [:material-code-braces: ListConfiguredAudienceModelsRequestRequestTypeDef](./type_defs.md#listconfiguredaudiencemodelsrequestrequesttypedef) 

### list\_configured\_model\_algorithm\_associations

Returns a list of configured model algorithm associations.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_configured_model_algorithm_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_configured_model_algorithm_associations.html)

```python
# list_configured_model_algorithm_associations method definition

await def list_configured_model_algorithm_associations(
    self,
    *,
    membershipIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListConfiguredModelAlgorithmAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfiguredModelAlgorithmAssociationsResponseTypeDef](./type_defs.md#listconfiguredmodelalgorithmassociationsresponsetypedef) 


```python
# list_configured_model_algorithm_associations method usage example with argument unpacking

kwargs: ListConfiguredModelAlgorithmAssociationsRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_configured_model_algorithm_associations(**kwargs)
```

1. See [:material-code-braces: ListConfiguredModelAlgorithmAssociationsRequestRequestTypeDef](./type_defs.md#listconfiguredmodelalgorithmassociationsrequestrequesttypedef) 

### list\_configured\_model\_algorithms

Returns a list of configured model algorithms.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_configured_model_algorithms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_configured_model_algorithms.html)

```python
# list_configured_model_algorithms method definition

await def list_configured_model_algorithms(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListConfiguredModelAlgorithmsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfiguredModelAlgorithmsResponseTypeDef](./type_defs.md#listconfiguredmodelalgorithmsresponsetypedef) 


```python
# list_configured_model_algorithms method usage example with argument unpacking

kwargs: ListConfiguredModelAlgorithmsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_configured_model_algorithms(**kwargs)
```

1. See [:material-code-braces: ListConfiguredModelAlgorithmsRequestRequestTypeDef](./type_defs.md#listconfiguredmodelalgorithmsrequestrequesttypedef) 

### list\_ml\_input\_channels

Returns a list of ML input channels.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_ml_input_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_ml_input_channels.html)

```python
# list_ml_input_channels method definition

await def list_ml_input_channels(
    self,
    *,
    membershipIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListMLInputChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMLInputChannelsResponseTypeDef](./type_defs.md#listmlinputchannelsresponsetypedef) 


```python
# list_ml_input_channels method usage example with argument unpacking

kwargs: ListMLInputChannelsRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_ml_input_channels(**kwargs)
```

1. See [:material-code-braces: ListMLInputChannelsRequestRequestTypeDef](./type_defs.md#listmlinputchannelsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags for a provided resource.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_tags_for_resource.html)

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

### list\_trained\_model\_inference\_jobs

Returns a list of trained model inference jobs that match the request
parameters.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_trained_model_inference_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_trained_model_inference_jobs.html)

```python
# list_trained_model_inference_jobs method definition

await def list_trained_model_inference_jobs(
    self,
    *,
    membershipIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
    trainedModelArn: str = ...,
) -> ListTrainedModelInferenceJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrainedModelInferenceJobsResponseTypeDef](./type_defs.md#listtrainedmodelinferencejobsresponsetypedef) 


```python
# list_trained_model_inference_jobs method usage example with argument unpacking

kwargs: ListTrainedModelInferenceJobsRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_trained_model_inference_jobs(**kwargs)
```

1. See [:material-code-braces: ListTrainedModelInferenceJobsRequestRequestTypeDef](./type_defs.md#listtrainedmodelinferencejobsrequestrequesttypedef) 

### list\_trained\_models

Returns a list of trained models.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_trained_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_trained_models.html)

```python
# list_trained_models method definition

await def list_trained_models(
    self,
    *,
    membershipIdentifier: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTrainedModelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrainedModelsResponseTypeDef](./type_defs.md#listtrainedmodelsresponsetypedef) 


```python
# list_trained_models method usage example with argument unpacking

kwargs: ListTrainedModelsRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
}

parent.list_trained_models(**kwargs)
```

1. See [:material-code-braces: ListTrainedModelsRequestRequestTypeDef](./type_defs.md#listtrainedmodelsrequestrequesttypedef) 

### list\_training\_datasets

Returns a list of training datasets.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_training_datasets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/list_training_datasets.html)

```python
# list_training_datasets method definition

await def list_training_datasets(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTrainingDatasetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTrainingDatasetsResponseTypeDef](./type_defs.md#listtrainingdatasetsresponsetypedef) 


```python
# list_training_datasets method usage example with argument unpacking

kwargs: ListTrainingDatasetsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_training_datasets(**kwargs)
```

1. See [:material-code-braces: ListTrainingDatasetsRequestRequestTypeDef](./type_defs.md#listtrainingdatasetsrequestrequesttypedef) 

### put\_configured\_audience\_model\_policy

Create or update the resource policy for a configured audience model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").put_configured_audience_model_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/put_configured_audience_model_policy.html)

```python
# put_configured_audience_model_policy method definition

await def put_configured_audience_model_policy(
    self,
    *,
    configuredAudienceModelArn: str,
    configuredAudienceModelPolicy: str,
    previousPolicyHash: str = ...,
    policyExistenceCondition: PolicyExistenceConditionType = ...,  # (1)
) -> PutConfiguredAudienceModelPolicyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PolicyExistenceConditionType](./literals.md#policyexistenceconditiontype) 
2. See [:material-code-braces: PutConfiguredAudienceModelPolicyResponseTypeDef](./type_defs.md#putconfiguredaudiencemodelpolicyresponsetypedef) 


```python
# put_configured_audience_model_policy method usage example with argument unpacking

kwargs: PutConfiguredAudienceModelPolicyRequestRequestTypeDef = {  # (1)
    "configuredAudienceModelArn": ...,
    "configuredAudienceModelPolicy": ...,
}

parent.put_configured_audience_model_policy(**kwargs)
```

1. See [:material-code-braces: PutConfiguredAudienceModelPolicyRequestRequestTypeDef](./type_defs.md#putconfiguredaudiencemodelpolicyrequestrequesttypedef) 

### put\_ml\_configuration

Assigns information about an ML configuration.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").put_ml_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/put_ml_configuration.html)

```python
# put_ml_configuration method definition

await def put_ml_configuration(
    self,
    *,
    membershipIdentifier: str,
    defaultOutputLocation: MLOutputConfigurationTypeDef,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MLOutputConfigurationTypeDef](./type_defs.md#mloutputconfigurationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_ml_configuration method usage example with argument unpacking

kwargs: PutMLConfigurationRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "defaultOutputLocation": ...,
}

parent.put_ml_configuration(**kwargs)
```

1. See [:material-code-braces: PutMLConfigurationRequestRequestTypeDef](./type_defs.md#putmlconfigurationrequestrequesttypedef) 

### start\_audience\_export\_job

Export an audience of a specified size after you have generated an audience.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").start_audience_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/start_audience_export_job.html)

```python
# start_audience_export_job method definition

await def start_audience_export_job(
    self,
    *,
    name: str,
    audienceGenerationJobArn: str,
    audienceSize: AudienceSizeTypeDef,  # (1)
    description: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_audience_export_job method usage example with argument unpacking

kwargs: StartAudienceExportJobRequestRequestTypeDef = {  # (1)
    "name": ...,
    "audienceGenerationJobArn": ...,
    "audienceSize": ...,
}

parent.start_audience_export_job(**kwargs)
```

1. See [:material-code-braces: StartAudienceExportJobRequestRequestTypeDef](./type_defs.md#startaudienceexportjobrequestrequesttypedef) 

### start\_audience\_generation\_job

Information necessary to start the audience generation job.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").start_audience_generation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/start_audience_generation_job.html)

```python
# start_audience_generation_job method definition

await def start_audience_generation_job(
    self,
    *,
    name: str,
    configuredAudienceModelArn: str,
    seedAudience: AudienceGenerationJobDataSourceTypeDef,  # (1)
    includeSeedInOutput: bool = ...,
    collaborationId: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> StartAudienceGenerationJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AudienceGenerationJobDataSourceTypeDef](./type_defs.md#audiencegenerationjobdatasourcetypedef) 
2. See [:material-code-braces: StartAudienceGenerationJobResponseTypeDef](./type_defs.md#startaudiencegenerationjobresponsetypedef) 


```python
# start_audience_generation_job method usage example with argument unpacking

kwargs: StartAudienceGenerationJobRequestRequestTypeDef = {  # (1)
    "name": ...,
    "configuredAudienceModelArn": ...,
    "seedAudience": ...,
}

parent.start_audience_generation_job(**kwargs)
```

1. See [:material-code-braces: StartAudienceGenerationJobRequestRequestTypeDef](./type_defs.md#startaudiencegenerationjobrequestrequesttypedef) 

### start\_trained\_model\_export\_job

Provides the information necessary to start a trained model export job.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").start_trained_model_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/start_trained_model_export_job.html)

```python
# start_trained_model_export_job method definition

await def start_trained_model_export_job(
    self,
    *,
    name: str,
    trainedModelArn: str,
    membershipIdentifier: str,
    outputConfiguration: TrainedModelExportOutputConfigurationTypeDef,  # (1)
    description: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TrainedModelExportOutputConfigurationTypeDef](./type_defs.md#trainedmodelexportoutputconfigurationtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_trained_model_export_job method usage example with argument unpacking

kwargs: StartTrainedModelExportJobRequestRequestTypeDef = {  # (1)
    "name": ...,
    "trainedModelArn": ...,
    "membershipIdentifier": ...,
    "outputConfiguration": ...,
}

parent.start_trained_model_export_job(**kwargs)
```

1. See [:material-code-braces: StartTrainedModelExportJobRequestRequestTypeDef](./type_defs.md#starttrainedmodelexportjobrequestrequesttypedef) 

### start\_trained\_model\_inference\_job

Defines the information necessary to begin a trained model inference job.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").start_trained_model_inference_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/start_trained_model_inference_job.html)

```python
# start_trained_model_inference_job method definition

await def start_trained_model_inference_job(
    self,
    *,
    membershipIdentifier: str,
    name: str,
    trainedModelArn: str,
    resourceConfig: InferenceResourceConfigTypeDef,  # (1)
    outputConfiguration: InferenceOutputConfigurationTypeDef,  # (2)
    dataSource: ModelInferenceDataSourceTypeDef,  # (3)
    configuredModelAlgorithmAssociationArn: str = ...,
    description: str = ...,
    containerExecutionParameters: InferenceContainerExecutionParametersTypeDef = ...,  # (4)
    environment: Mapping[str, str] = ...,
    kmsKeyArn: str = ...,
    tags: Mapping[str, str] = ...,
) -> StartTrainedModelInferenceJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: InferenceResourceConfigTypeDef](./type_defs.md#inferenceresourceconfigtypedef) 
2. See [:material-code-braces: InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef) 
3. See [:material-code-braces: ModelInferenceDataSourceTypeDef](./type_defs.md#modelinferencedatasourcetypedef) 
4. See [:material-code-braces: InferenceContainerExecutionParametersTypeDef](./type_defs.md#inferencecontainerexecutionparameterstypedef) 
5. See [:material-code-braces: StartTrainedModelInferenceJobResponseTypeDef](./type_defs.md#starttrainedmodelinferencejobresponsetypedef) 


```python
# start_trained_model_inference_job method usage example with argument unpacking

kwargs: StartTrainedModelInferenceJobRequestRequestTypeDef = {  # (1)
    "membershipIdentifier": ...,
    "name": ...,
    "trainedModelArn": ...,
    "resourceConfig": ...,
    "outputConfiguration": ...,
    "dataSource": ...,
}

parent.start_trained_model_inference_job(**kwargs)
```

1. See [:material-code-braces: StartTrainedModelInferenceJobRequestRequestTypeDef](./type_defs.md#starttrainedmodelinferencejobrequestrequesttypedef) 

### tag\_resource

Adds metadata tags to a specified resource.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/tag_resource.html)

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

Removes metadata tags from a specified resource.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/untag_resource.html)

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

### update\_configured\_audience\_model

Provides the information necessary to update a configured audience model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").update_configured_audience_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml/client/update_configured_audience_model.html)

```python
# update_configured_audience_model method definition

await def update_configured_audience_model(
    self,
    *,
    configuredAudienceModelArn: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef = ...,  # (1)
    audienceModelArn: str = ...,
    sharedAudienceMetrics: Sequence[SharedAudienceMetricsType] = ...,  # (2)
    minMatchingSeedSize: int = ...,
    audienceSizeConfig: AudienceSizeConfigTypeDef = ...,  # (3)
    description: str = ...,
) -> UpdateConfiguredAudienceModelResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
3. See [:material-code-braces: AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef) 
4. See [:material-code-braces: UpdateConfiguredAudienceModelResponseTypeDef](./type_defs.md#updateconfiguredaudiencemodelresponsetypedef) 


```python
# update_configured_audience_model method usage example with argument unpacking

kwargs: UpdateConfiguredAudienceModelRequestRequestTypeDef = {  # (1)
    "configuredAudienceModelArn": ...,
}

parent.update_configured_audience_model(**kwargs)
```

1. See [:material-code-braces: UpdateConfiguredAudienceModelRequestRequestTypeDef](./type_defs.md#updateconfiguredaudiencemodelrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cleanroomsml").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cleanroomsml").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client)

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

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_paginator` method with overloads.

- `client.get_paginator("list_audience_export_jobs")` -> [ListAudienceExportJobsPaginator](./paginators.md#listaudienceexportjobspaginator)
- `client.get_paginator("list_audience_generation_jobs")` -> [ListAudienceGenerationJobsPaginator](./paginators.md#listaudiencegenerationjobspaginator)
- `client.get_paginator("list_audience_models")` -> [ListAudienceModelsPaginator](./paginators.md#listaudiencemodelspaginator)
- `client.get_paginator("list_collaboration_configured_model_algorithm_associations")` -> [ListCollaborationConfiguredModelAlgorithmAssociationsPaginator](./paginators.md#listcollaborationconfiguredmodelalgorithmassociationspaginator)
- `client.get_paginator("list_collaboration_ml_input_channels")` -> [ListCollaborationMLInputChannelsPaginator](./paginators.md#listcollaborationmlinputchannelspaginator)
- `client.get_paginator("list_collaboration_trained_model_export_jobs")` -> [ListCollaborationTrainedModelExportJobsPaginator](./paginators.md#listcollaborationtrainedmodelexportjobspaginator)
- `client.get_paginator("list_collaboration_trained_model_inference_jobs")` -> [ListCollaborationTrainedModelInferenceJobsPaginator](./paginators.md#listcollaborationtrainedmodelinferencejobspaginator)
- `client.get_paginator("list_collaboration_trained_models")` -> [ListCollaborationTrainedModelsPaginator](./paginators.md#listcollaborationtrainedmodelspaginator)
- `client.get_paginator("list_configured_audience_models")` -> [ListConfiguredAudienceModelsPaginator](./paginators.md#listconfiguredaudiencemodelspaginator)
- `client.get_paginator("list_configured_model_algorithm_associations")` -> [ListConfiguredModelAlgorithmAssociationsPaginator](./paginators.md#listconfiguredmodelalgorithmassociationspaginator)
- `client.get_paginator("list_configured_model_algorithms")` -> [ListConfiguredModelAlgorithmsPaginator](./paginators.md#listconfiguredmodelalgorithmspaginator)
- `client.get_paginator("list_ml_input_channels")` -> [ListMLInputChannelsPaginator](./paginators.md#listmlinputchannelspaginator)
- `client.get_paginator("list_trained_model_inference_jobs")` -> [ListTrainedModelInferenceJobsPaginator](./paginators.md#listtrainedmodelinferencejobspaginator)
- `client.get_paginator("list_trained_models")` -> [ListTrainedModelsPaginator](./paginators.md#listtrainedmodelspaginator)
- `client.get_paginator("list_training_datasets")` -> [ListTrainingDatasetsPaginator](./paginators.md#listtrainingdatasetspaginator)



