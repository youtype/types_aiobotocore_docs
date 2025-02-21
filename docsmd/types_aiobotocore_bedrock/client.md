# BedrockClient

> [Index](../README.md) > [Bedrock](./README.md) > BedrockClient

!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## BedrockClient

Type annotations and code completion for `#!python session.create_client("bedrock")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client)

```python
# BedrockClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_bedrock.client import BedrockClient

session = get_session()
async with session.create_client("bedrock") as client:
    client: BedrockClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("bedrock").exceptions` structure.

```python
# BedrockClient.exceptions usage example

async with session.create_client("bedrock") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
        client.TooManyTagsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# BedrockClient usage type checking example

from types_aiobotocore_bedrock.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("bedrock").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("bedrock").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/generate_presigned_url.html)

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


### batch\_delete\_evaluation\_job

Deletes a batch of evaluation jobs.

Type annotations and code completion for `#!python session.create_client("bedrock").batch_delete_evaluation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/batch_delete_evaluation_job.html)

```python
# batch_delete_evaluation_job method definition

await def batch_delete_evaluation_job(
    self,
    *,
    jobIdentifiers: Sequence[str],
) -> BatchDeleteEvaluationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteEvaluationJobResponseTypeDef](./type_defs.md#batchdeleteevaluationjobresponsetypedef) 


```python
# batch_delete_evaluation_job method usage example with argument unpacking

kwargs: BatchDeleteEvaluationJobRequestTypeDef = {  # (1)
    "jobIdentifiers": ...,
}

parent.batch_delete_evaluation_job(**kwargs)
```

1. See [:material-code-braces: BatchDeleteEvaluationJobRequestTypeDef](./type_defs.md#batchdeleteevaluationjobrequesttypedef) 

### create\_evaluation\_job

Creates an evaluation job.

Type annotations and code completion for `#!python session.create_client("bedrock").create_evaluation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/create_evaluation_job.html)

```python
# create_evaluation_job method definition

await def create_evaluation_job(
    self,
    *,
    jobName: str,
    roleArn: str,
    evaluationConfig: EvaluationConfigUnionTypeDef,  # (1)
    inferenceConfig: EvaluationInferenceConfigUnionTypeDef,  # (2)
    outputDataConfig: EvaluationOutputDataConfigTypeDef,  # (3)
    jobDescription: str = ...,
    clientRequestToken: str = ...,
    customerEncryptionKeyId: str = ...,
    jobTags: Sequence[TagTypeDef] = ...,  # (4)
    applicationType: ApplicationTypeType = ...,  # (5)
) -> CreateEvaluationJobResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: EvaluationConfigTypeDef](./type_defs.md#evaluationconfigtypedef) [:material-code-braces: EvaluationConfigOutputTypeDef](./type_defs.md#evaluationconfigoutputtypedef) 
2. See [:material-code-braces: EvaluationInferenceConfigTypeDef](./type_defs.md#evaluationinferenceconfigtypedef) [:material-code-braces: EvaluationInferenceConfigOutputTypeDef](./type_defs.md#evaluationinferenceconfigoutputtypedef) 
3. See [:material-code-braces: EvaluationOutputDataConfigTypeDef](./type_defs.md#evaluationoutputdataconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
6. See [:material-code-braces: CreateEvaluationJobResponseTypeDef](./type_defs.md#createevaluationjobresponsetypedef) 


```python
# create_evaluation_job method usage example with argument unpacking

kwargs: CreateEvaluationJobRequestTypeDef = {  # (1)
    "jobName": ...,
    "roleArn": ...,
    "evaluationConfig": ...,
    "inferenceConfig": ...,
    "outputDataConfig": ...,
}

parent.create_evaluation_job(**kwargs)
```

1. See [:material-code-braces: CreateEvaluationJobRequestTypeDef](./type_defs.md#createevaluationjobrequesttypedef) 

### create\_guardrail

Creates a guardrail to block topics and to implement safeguards for your
generative AI applications.

Type annotations and code completion for `#!python session.create_client("bedrock").create_guardrail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/create_guardrail.html)

```python
# create_guardrail method definition

await def create_guardrail(
    self,
    *,
    name: str,
    blockedInputMessaging: str,
    blockedOutputsMessaging: str,
    description: str = ...,
    topicPolicyConfig: GuardrailTopicPolicyConfigTypeDef = ...,  # (1)
    contentPolicyConfig: GuardrailContentPolicyConfigTypeDef = ...,  # (2)
    wordPolicyConfig: GuardrailWordPolicyConfigTypeDef = ...,  # (3)
    sensitiveInformationPolicyConfig: GuardrailSensitiveInformationPolicyConfigTypeDef = ...,  # (4)
    contextualGroundingPolicyConfig: GuardrailContextualGroundingPolicyConfigTypeDef = ...,  # (5)
    kmsKeyId: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (6)
    clientRequestToken: str = ...,
) -> CreateGuardrailResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: GuardrailTopicPolicyConfigTypeDef](./type_defs.md#guardrailtopicpolicyconfigtypedef) 
2. See [:material-code-braces: GuardrailContentPolicyConfigTypeDef](./type_defs.md#guardrailcontentpolicyconfigtypedef) 
3. See [:material-code-braces: GuardrailWordPolicyConfigTypeDef](./type_defs.md#guardrailwordpolicyconfigtypedef) 
4. See [:material-code-braces: GuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyconfigtypedef) 
5. See [:material-code-braces: GuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#guardrailcontextualgroundingpolicyconfigtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: CreateGuardrailResponseTypeDef](./type_defs.md#createguardrailresponsetypedef) 


```python
# create_guardrail method usage example with argument unpacking

kwargs: CreateGuardrailRequestTypeDef = {  # (1)
    "name": ...,
    "blockedInputMessaging": ...,
    "blockedOutputsMessaging": ...,
}

parent.create_guardrail(**kwargs)
```

1. See [:material-code-braces: CreateGuardrailRequestTypeDef](./type_defs.md#createguardrailrequesttypedef) 

### create\_guardrail\_version

Creates a version of the guardrail.

Type annotations and code completion for `#!python session.create_client("bedrock").create_guardrail_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/create_guardrail_version.html)

```python
# create_guardrail_version method definition

await def create_guardrail_version(
    self,
    *,
    guardrailIdentifier: str,
    description: str = ...,
    clientRequestToken: str = ...,
) -> CreateGuardrailVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateGuardrailVersionResponseTypeDef](./type_defs.md#createguardrailversionresponsetypedef) 


```python
# create_guardrail_version method usage example with argument unpacking

kwargs: CreateGuardrailVersionRequestTypeDef = {  # (1)
    "guardrailIdentifier": ...,
}

parent.create_guardrail_version(**kwargs)
```

1. See [:material-code-braces: CreateGuardrailVersionRequestTypeDef](./type_defs.md#createguardrailversionrequesttypedef) 

### create\_inference\_profile

Creates an application inference profile to track metrics and costs when
invoking a model.

Type annotations and code completion for `#!python session.create_client("bedrock").create_inference_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/create_inference_profile.html)

```python
# create_inference_profile method definition

await def create_inference_profile(
    self,
    *,
    inferenceProfileName: str,
    modelSource: InferenceProfileModelSourceTypeDef,  # (1)
    description: str = ...,
    clientRequestToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateInferenceProfileResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InferenceProfileModelSourceTypeDef](./type_defs.md#inferenceprofilemodelsourcetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateInferenceProfileResponseTypeDef](./type_defs.md#createinferenceprofileresponsetypedef) 


```python
# create_inference_profile method usage example with argument unpacking

kwargs: CreateInferenceProfileRequestTypeDef = {  # (1)
    "inferenceProfileName": ...,
    "modelSource": ...,
}

parent.create_inference_profile(**kwargs)
```

1. See [:material-code-braces: CreateInferenceProfileRequestTypeDef](./type_defs.md#createinferenceprofilerequesttypedef) 

### create\_marketplace\_model\_endpoint

Creates an endpoint for a model from Amazon Bedrock Marketplace.

Type annotations and code completion for `#!python session.create_client("bedrock").create_marketplace_model_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/create_marketplace_model_endpoint.html)

```python
# create_marketplace_model_endpoint method definition

await def create_marketplace_model_endpoint(
    self,
    *,
    modelSourceIdentifier: str,
    endpointConfig: EndpointConfigUnionTypeDef,  # (1)
    endpointName: str,
    acceptEula: bool = ...,
    clientRequestToken: str = ...,
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateMarketplaceModelEndpointResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EndpointConfigTypeDef](./type_defs.md#endpointconfigtypedef) [:material-code-braces: EndpointConfigOutputTypeDef](./type_defs.md#endpointconfigoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateMarketplaceModelEndpointResponseTypeDef](./type_defs.md#createmarketplacemodelendpointresponsetypedef) 


```python
# create_marketplace_model_endpoint method usage example with argument unpacking

kwargs: CreateMarketplaceModelEndpointRequestTypeDef = {  # (1)
    "modelSourceIdentifier": ...,
    "endpointConfig": ...,
    "endpointName": ...,
}

parent.create_marketplace_model_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateMarketplaceModelEndpointRequestTypeDef](./type_defs.md#createmarketplacemodelendpointrequesttypedef) 

### create\_model\_copy\_job

Copies a model to another region so that it can be used there.

Type annotations and code completion for `#!python session.create_client("bedrock").create_model_copy_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/create_model_copy_job.html)

```python
# create_model_copy_job method definition

await def create_model_copy_job(
    self,
    *,
    sourceModelArn: str,
    targetModelName: str,
    modelKmsKeyId: str = ...,
    targetModelTags: Sequence[TagTypeDef] = ...,  # (1)
    clientRequestToken: str = ...,
) -> CreateModelCopyJobResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateModelCopyJobResponseTypeDef](./type_defs.md#createmodelcopyjobresponsetypedef) 


```python
# create_model_copy_job method usage example with argument unpacking

kwargs: CreateModelCopyJobRequestTypeDef = {  # (1)
    "sourceModelArn": ...,
    "targetModelName": ...,
}

parent.create_model_copy_job(**kwargs)
```

1. See [:material-code-braces: CreateModelCopyJobRequestTypeDef](./type_defs.md#createmodelcopyjobrequesttypedef) 

### create\_model\_customization\_job

Creates a fine-tuning job to customize a base model.

Type annotations and code completion for `#!python session.create_client("bedrock").create_model_customization_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/create_model_customization_job.html)

```python
# create_model_customization_job method definition

await def create_model_customization_job(
    self,
    *,
    jobName: str,
    customModelName: str,
    roleArn: str,
    baseModelIdentifier: str,
    trainingDataConfig: TrainingDataConfigUnionTypeDef,  # (1)
    outputDataConfig: OutputDataConfigTypeDef,  # (2)
    clientRequestToken: str = ...,
    customizationType: CustomizationTypeType = ...,  # (3)
    customModelKmsKeyId: str = ...,
    jobTags: Sequence[TagTypeDef] = ...,  # (4)
    customModelTags: Sequence[TagTypeDef] = ...,  # (4)
    validationDataConfig: ValidationDataConfigUnionTypeDef = ...,  # (6)
    hyperParameters: Mapping[str, str] = ...,
    vpcConfig: VpcConfigUnionTypeDef = ...,  # (7)
    customizationConfig: CustomizationConfigTypeDef = ...,  # (8)
) -> CreateModelCustomizationJobResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: TrainingDataConfigTypeDef](./type_defs.md#trainingdataconfigtypedef) [:material-code-braces: TrainingDataConfigOutputTypeDef](./type_defs.md#trainingdataconfigoutputtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: CustomizationTypeType](./literals.md#customizationtypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: ValidationDataConfigTypeDef](./type_defs.md#validationdataconfigtypedef) [:material-code-braces: ValidationDataConfigOutputTypeDef](./type_defs.md#validationdataconfigoutputtypedef) 
7. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
8. See [:material-code-braces: CustomizationConfigTypeDef](./type_defs.md#customizationconfigtypedef) 
9. See [:material-code-braces: CreateModelCustomizationJobResponseTypeDef](./type_defs.md#createmodelcustomizationjobresponsetypedef) 


```python
# create_model_customization_job method usage example with argument unpacking

kwargs: CreateModelCustomizationJobRequestTypeDef = {  # (1)
    "jobName": ...,
    "customModelName": ...,
    "roleArn": ...,
    "baseModelIdentifier": ...,
    "trainingDataConfig": ...,
    "outputDataConfig": ...,
}

parent.create_model_customization_job(**kwargs)
```

1. See [:material-code-braces: CreateModelCustomizationJobRequestTypeDef](./type_defs.md#createmodelcustomizationjobrequesttypedef) 

### create\_model\_import\_job

Creates a model import job to import model that you have customized in other
environments, such as Amazon SageMaker.

Type annotations and code completion for `#!python session.create_client("bedrock").create_model_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/create_model_import_job.html)

```python
# create_model_import_job method definition

await def create_model_import_job(
    self,
    *,
    jobName: str,
    importedModelName: str,
    roleArn: str,
    modelDataSource: ModelDataSourceTypeDef,  # (1)
    jobTags: Sequence[TagTypeDef] = ...,  # (2)
    importedModelTags: Sequence[TagTypeDef] = ...,  # (2)
    clientRequestToken: str = ...,
    vpcConfig: VpcConfigUnionTypeDef = ...,  # (4)
    importedModelKmsKeyId: str = ...,
) -> CreateModelImportJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ModelDataSourceTypeDef](./type_defs.md#modeldatasourcetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
5. See [:material-code-braces: CreateModelImportJobResponseTypeDef](./type_defs.md#createmodelimportjobresponsetypedef) 


```python
# create_model_import_job method usage example with argument unpacking

kwargs: CreateModelImportJobRequestTypeDef = {  # (1)
    "jobName": ...,
    "importedModelName": ...,
    "roleArn": ...,
    "modelDataSource": ...,
}

parent.create_model_import_job(**kwargs)
```

1. See [:material-code-braces: CreateModelImportJobRequestTypeDef](./type_defs.md#createmodelimportjobrequesttypedef) 

### create\_model\_invocation\_job

Creates a batch inference job to invoke a model on multiple prompts.

Type annotations and code completion for `#!python session.create_client("bedrock").create_model_invocation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/create_model_invocation_job.html)

```python
# create_model_invocation_job method definition

await def create_model_invocation_job(
    self,
    *,
    jobName: str,
    roleArn: str,
    modelId: str,
    inputDataConfig: ModelInvocationJobInputDataConfigTypeDef,  # (1)
    outputDataConfig: ModelInvocationJobOutputDataConfigTypeDef,  # (2)
    clientRequestToken: str = ...,
    vpcConfig: VpcConfigUnionTypeDef = ...,  # (3)
    timeoutDurationInHours: int = ...,
    tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateModelInvocationJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: ModelInvocationJobInputDataConfigTypeDef](./type_defs.md#modelinvocationjobinputdataconfigtypedef) 
2. See [:material-code-braces: ModelInvocationJobOutputDataConfigTypeDef](./type_defs.md#modelinvocationjoboutputdataconfigtypedef) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateModelInvocationJobResponseTypeDef](./type_defs.md#createmodelinvocationjobresponsetypedef) 


```python
# create_model_invocation_job method usage example with argument unpacking

kwargs: CreateModelInvocationJobRequestTypeDef = {  # (1)
    "jobName": ...,
    "roleArn": ...,
    "modelId": ...,
    "inputDataConfig": ...,
    "outputDataConfig": ...,
}

parent.create_model_invocation_job(**kwargs)
```

1. See [:material-code-braces: CreateModelInvocationJobRequestTypeDef](./type_defs.md#createmodelinvocationjobrequesttypedef) 

### create\_provisioned\_model\_throughput

Creates dedicated throughput for a base or custom model with the model units
and for the duration that you specify.

Type annotations and code completion for `#!python session.create_client("bedrock").create_provisioned_model_throughput` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/create_provisioned_model_throughput.html)

```python
# create_provisioned_model_throughput method definition

await def create_provisioned_model_throughput(
    self,
    *,
    modelUnits: int,
    provisionedModelName: str,
    modelId: str,
    clientRequestToken: str = ...,
    commitmentDuration: CommitmentDurationType = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateProvisionedModelThroughputResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CommitmentDurationType](./literals.md#commitmentdurationtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateProvisionedModelThroughputResponseTypeDef](./type_defs.md#createprovisionedmodelthroughputresponsetypedef) 


```python
# create_provisioned_model_throughput method usage example with argument unpacking

kwargs: CreateProvisionedModelThroughputRequestTypeDef = {  # (1)
    "modelUnits": ...,
    "provisionedModelName": ...,
    "modelId": ...,
}

parent.create_provisioned_model_throughput(**kwargs)
```

1. See [:material-code-braces: CreateProvisionedModelThroughputRequestTypeDef](./type_defs.md#createprovisionedmodelthroughputrequesttypedef) 

### delete\_custom\_model

Deletes a custom model that you created earlier.

Type annotations and code completion for `#!python session.create_client("bedrock").delete_custom_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/delete_custom_model.html)

```python
# delete_custom_model method definition

await def delete_custom_model(
    self,
    *,
    modelIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_custom_model method usage example with argument unpacking

kwargs: DeleteCustomModelRequestTypeDef = {  # (1)
    "modelIdentifier": ...,
}

parent.delete_custom_model(**kwargs)
```

1. See [:material-code-braces: DeleteCustomModelRequestTypeDef](./type_defs.md#deletecustommodelrequesttypedef) 

### delete\_guardrail

Deletes a guardrail.

Type annotations and code completion for `#!python session.create_client("bedrock").delete_guardrail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/delete_guardrail.html)

```python
# delete_guardrail method definition

await def delete_guardrail(
    self,
    *,
    guardrailIdentifier: str,
    guardrailVersion: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_guardrail method usage example with argument unpacking

kwargs: DeleteGuardrailRequestTypeDef = {  # (1)
    "guardrailIdentifier": ...,
}

parent.delete_guardrail(**kwargs)
```

1. See [:material-code-braces: DeleteGuardrailRequestTypeDef](./type_defs.md#deleteguardrailrequesttypedef) 

### delete\_imported\_model

Deletes a custom model that you imported earlier.

Type annotations and code completion for `#!python session.create_client("bedrock").delete_imported_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/delete_imported_model.html)

```python
# delete_imported_model method definition

await def delete_imported_model(
    self,
    *,
    modelIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_imported_model method usage example with argument unpacking

kwargs: DeleteImportedModelRequestTypeDef = {  # (1)
    "modelIdentifier": ...,
}

parent.delete_imported_model(**kwargs)
```

1. See [:material-code-braces: DeleteImportedModelRequestTypeDef](./type_defs.md#deleteimportedmodelrequesttypedef) 

### delete\_inference\_profile

Deletes an application inference profile.

Type annotations and code completion for `#!python session.create_client("bedrock").delete_inference_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/delete_inference_profile.html)

```python
# delete_inference_profile method definition

await def delete_inference_profile(
    self,
    *,
    inferenceProfileIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_inference_profile method usage example with argument unpacking

kwargs: DeleteInferenceProfileRequestTypeDef = {  # (1)
    "inferenceProfileIdentifier": ...,
}

parent.delete_inference_profile(**kwargs)
```

1. See [:material-code-braces: DeleteInferenceProfileRequestTypeDef](./type_defs.md#deleteinferenceprofilerequesttypedef) 

### delete\_marketplace\_model\_endpoint

Deletes an endpoint for a model from Amazon Bedrock Marketplace.

Type annotations and code completion for `#!python session.create_client("bedrock").delete_marketplace_model_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/delete_marketplace_model_endpoint.html)

```python
# delete_marketplace_model_endpoint method definition

await def delete_marketplace_model_endpoint(
    self,
    *,
    endpointArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_marketplace_model_endpoint method usage example with argument unpacking

kwargs: DeleteMarketplaceModelEndpointRequestTypeDef = {  # (1)
    "endpointArn": ...,
}

parent.delete_marketplace_model_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteMarketplaceModelEndpointRequestTypeDef](./type_defs.md#deletemarketplacemodelendpointrequesttypedef) 

### delete\_model\_invocation\_logging\_configuration

Delete the invocation logging.

Type annotations and code completion for `#!python session.create_client("bedrock").delete_model_invocation_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/delete_model_invocation_logging_configuration.html)

```python
# delete_model_invocation_logging_configuration method definition

await def delete_model_invocation_logging_configuration(
    self,
) -> Dict[str, Any]:
    ...
```


### delete\_provisioned\_model\_throughput

Deletes a Provisioned Throughput.

Type annotations and code completion for `#!python session.create_client("bedrock").delete_provisioned_model_throughput` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/delete_provisioned_model_throughput.html)

```python
# delete_provisioned_model_throughput method definition

await def delete_provisioned_model_throughput(
    self,
    *,
    provisionedModelId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_provisioned_model_throughput method usage example with argument unpacking

kwargs: DeleteProvisionedModelThroughputRequestTypeDef = {  # (1)
    "provisionedModelId": ...,
}

parent.delete_provisioned_model_throughput(**kwargs)
```

1. See [:material-code-braces: DeleteProvisionedModelThroughputRequestTypeDef](./type_defs.md#deleteprovisionedmodelthroughputrequesttypedef) 

### deregister\_marketplace\_model\_endpoint

Deregisters an endpoint for a model from Amazon Bedrock Marketplace.

Type annotations and code completion for `#!python session.create_client("bedrock").deregister_marketplace_model_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/deregister_marketplace_model_endpoint.html)

```python
# deregister_marketplace_model_endpoint method definition

await def deregister_marketplace_model_endpoint(
    self,
    *,
    endpointArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# deregister_marketplace_model_endpoint method usage example with argument unpacking

kwargs: DeregisterMarketplaceModelEndpointRequestTypeDef = {  # (1)
    "endpointArn": ...,
}

parent.deregister_marketplace_model_endpoint(**kwargs)
```

1. See [:material-code-braces: DeregisterMarketplaceModelEndpointRequestTypeDef](./type_defs.md#deregistermarketplacemodelendpointrequesttypedef) 

### get\_custom\_model

Get the properties associated with a Amazon Bedrock custom model that you have
created.For more information, see <a
href="https://docs.aws.amazon.com/bedrock/latest/userguide/custom-models.html">Custom
models</a> in the <a
href="https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-service...

Type annotations and code completion for `#!python session.create_client("bedrock").get_custom_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_custom_model.html)

```python
# get_custom_model method definition

await def get_custom_model(
    self,
    *,
    modelIdentifier: str,
) -> GetCustomModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCustomModelResponseTypeDef](./type_defs.md#getcustommodelresponsetypedef) 


```python
# get_custom_model method usage example with argument unpacking

kwargs: GetCustomModelRequestTypeDef = {  # (1)
    "modelIdentifier": ...,
}

parent.get_custom_model(**kwargs)
```

1. See [:material-code-braces: GetCustomModelRequestTypeDef](./type_defs.md#getcustommodelrequesttypedef) 

### get\_evaluation\_job

Gets information about an evaluation job, such as the status of the job.

Type annotations and code completion for `#!python session.create_client("bedrock").get_evaluation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_evaluation_job.html)

```python
# get_evaluation_job method definition

await def get_evaluation_job(
    self,
    *,
    jobIdentifier: str,
) -> GetEvaluationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEvaluationJobResponseTypeDef](./type_defs.md#getevaluationjobresponsetypedef) 


```python
# get_evaluation_job method usage example with argument unpacking

kwargs: GetEvaluationJobRequestTypeDef = {  # (1)
    "jobIdentifier": ...,
}

parent.get_evaluation_job(**kwargs)
```

1. See [:material-code-braces: GetEvaluationJobRequestTypeDef](./type_defs.md#getevaluationjobrequesttypedef) 

### get\_foundation\_model

Get details about a Amazon Bedrock foundation model.

Type annotations and code completion for `#!python session.create_client("bedrock").get_foundation_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_foundation_model.html)

```python
# get_foundation_model method definition

await def get_foundation_model(
    self,
    *,
    modelIdentifier: str,
) -> GetFoundationModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFoundationModelResponseTypeDef](./type_defs.md#getfoundationmodelresponsetypedef) 


```python
# get_foundation_model method usage example with argument unpacking

kwargs: GetFoundationModelRequestTypeDef = {  # (1)
    "modelIdentifier": ...,
}

parent.get_foundation_model(**kwargs)
```

1. See [:material-code-braces: GetFoundationModelRequestTypeDef](./type_defs.md#getfoundationmodelrequesttypedef) 

### get\_guardrail

Gets details about a guardrail.

Type annotations and code completion for `#!python session.create_client("bedrock").get_guardrail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_guardrail.html)

```python
# get_guardrail method definition

await def get_guardrail(
    self,
    *,
    guardrailIdentifier: str,
    guardrailVersion: str = ...,
) -> GetGuardrailResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGuardrailResponseTypeDef](./type_defs.md#getguardrailresponsetypedef) 


```python
# get_guardrail method usage example with argument unpacking

kwargs: GetGuardrailRequestTypeDef = {  # (1)
    "guardrailIdentifier": ...,
}

parent.get_guardrail(**kwargs)
```

1. See [:material-code-braces: GetGuardrailRequestTypeDef](./type_defs.md#getguardrailrequesttypedef) 

### get\_imported\_model

Gets properties associated with a customized model you imported.

Type annotations and code completion for `#!python session.create_client("bedrock").get_imported_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_imported_model.html)

```python
# get_imported_model method definition

await def get_imported_model(
    self,
    *,
    modelIdentifier: str,
) -> GetImportedModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetImportedModelResponseTypeDef](./type_defs.md#getimportedmodelresponsetypedef) 


```python
# get_imported_model method usage example with argument unpacking

kwargs: GetImportedModelRequestTypeDef = {  # (1)
    "modelIdentifier": ...,
}

parent.get_imported_model(**kwargs)
```

1. See [:material-code-braces: GetImportedModelRequestTypeDef](./type_defs.md#getimportedmodelrequesttypedef) 

### get\_inference\_profile

Gets information about an inference profile.

Type annotations and code completion for `#!python session.create_client("bedrock").get_inference_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_inference_profile.html)

```python
# get_inference_profile method definition

await def get_inference_profile(
    self,
    *,
    inferenceProfileIdentifier: str,
) -> GetInferenceProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInferenceProfileResponseTypeDef](./type_defs.md#getinferenceprofileresponsetypedef) 


```python
# get_inference_profile method usage example with argument unpacking

kwargs: GetInferenceProfileRequestTypeDef = {  # (1)
    "inferenceProfileIdentifier": ...,
}

parent.get_inference_profile(**kwargs)
```

1. See [:material-code-braces: GetInferenceProfileRequestTypeDef](./type_defs.md#getinferenceprofilerequesttypedef) 

### get\_marketplace\_model\_endpoint

Retrieves details about a specific endpoint for a model from Amazon Bedrock
Marketplace.

Type annotations and code completion for `#!python session.create_client("bedrock").get_marketplace_model_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_marketplace_model_endpoint.html)

```python
# get_marketplace_model_endpoint method definition

await def get_marketplace_model_endpoint(
    self,
    *,
    endpointArn: str,
) -> GetMarketplaceModelEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMarketplaceModelEndpointResponseTypeDef](./type_defs.md#getmarketplacemodelendpointresponsetypedef) 


```python
# get_marketplace_model_endpoint method usage example with argument unpacking

kwargs: GetMarketplaceModelEndpointRequestTypeDef = {  # (1)
    "endpointArn": ...,
}

parent.get_marketplace_model_endpoint(**kwargs)
```

1. See [:material-code-braces: GetMarketplaceModelEndpointRequestTypeDef](./type_defs.md#getmarketplacemodelendpointrequesttypedef) 

### get\_model\_copy\_job

Retrieves information about a model copy job.

Type annotations and code completion for `#!python session.create_client("bedrock").get_model_copy_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_model_copy_job.html)

```python
# get_model_copy_job method definition

await def get_model_copy_job(
    self,
    *,
    jobArn: str,
) -> GetModelCopyJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelCopyJobResponseTypeDef](./type_defs.md#getmodelcopyjobresponsetypedef) 


```python
# get_model_copy_job method usage example with argument unpacking

kwargs: GetModelCopyJobRequestTypeDef = {  # (1)
    "jobArn": ...,
}

parent.get_model_copy_job(**kwargs)
```

1. See [:material-code-braces: GetModelCopyJobRequestTypeDef](./type_defs.md#getmodelcopyjobrequesttypedef) 

### get\_model\_customization\_job

Retrieves the properties associated with a model-customization job, including
the status of the job.

Type annotations and code completion for `#!python session.create_client("bedrock").get_model_customization_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_model_customization_job.html)

```python
# get_model_customization_job method definition

await def get_model_customization_job(
    self,
    *,
    jobIdentifier: str,
) -> GetModelCustomizationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelCustomizationJobResponseTypeDef](./type_defs.md#getmodelcustomizationjobresponsetypedef) 


```python
# get_model_customization_job method usage example with argument unpacking

kwargs: GetModelCustomizationJobRequestTypeDef = {  # (1)
    "jobIdentifier": ...,
}

parent.get_model_customization_job(**kwargs)
```

1. See [:material-code-braces: GetModelCustomizationJobRequestTypeDef](./type_defs.md#getmodelcustomizationjobrequesttypedef) 

### get\_model\_import\_job

Retrieves the properties associated with import model job, including the status
of the job.

Type annotations and code completion for `#!python session.create_client("bedrock").get_model_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_model_import_job.html)

```python
# get_model_import_job method definition

await def get_model_import_job(
    self,
    *,
    jobIdentifier: str,
) -> GetModelImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelImportJobResponseTypeDef](./type_defs.md#getmodelimportjobresponsetypedef) 


```python
# get_model_import_job method usage example with argument unpacking

kwargs: GetModelImportJobRequestTypeDef = {  # (1)
    "jobIdentifier": ...,
}

parent.get_model_import_job(**kwargs)
```

1. See [:material-code-braces: GetModelImportJobRequestTypeDef](./type_defs.md#getmodelimportjobrequesttypedef) 

### get\_model\_invocation\_job

Gets details about a batch inference job.

Type annotations and code completion for `#!python session.create_client("bedrock").get_model_invocation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_model_invocation_job.html)

```python
# get_model_invocation_job method definition

await def get_model_invocation_job(
    self,
    *,
    jobIdentifier: str,
) -> GetModelInvocationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelInvocationJobResponseTypeDef](./type_defs.md#getmodelinvocationjobresponsetypedef) 


```python
# get_model_invocation_job method usage example with argument unpacking

kwargs: GetModelInvocationJobRequestTypeDef = {  # (1)
    "jobIdentifier": ...,
}

parent.get_model_invocation_job(**kwargs)
```

1. See [:material-code-braces: GetModelInvocationJobRequestTypeDef](./type_defs.md#getmodelinvocationjobrequesttypedef) 

### get\_model\_invocation\_logging\_configuration

Get the current configuration values for model invocation logging.

Type annotations and code completion for `#!python session.create_client("bedrock").get_model_invocation_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_model_invocation_logging_configuration.html)

```python
# get_model_invocation_logging_configuration method definition

await def get_model_invocation_logging_configuration(
    self,
) -> GetModelInvocationLoggingConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetModelInvocationLoggingConfigurationResponseTypeDef](./type_defs.md#getmodelinvocationloggingconfigurationresponsetypedef) 

### get\_prompt\_router

Retrieves details about a prompt router.

Type annotations and code completion for `#!python session.create_client("bedrock").get_prompt_router` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_prompt_router.html)

```python
# get_prompt_router method definition

await def get_prompt_router(
    self,
    *,
    promptRouterArn: str,
) -> GetPromptRouterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPromptRouterResponseTypeDef](./type_defs.md#getpromptrouterresponsetypedef) 


```python
# get_prompt_router method usage example with argument unpacking

kwargs: GetPromptRouterRequestTypeDef = {  # (1)
    "promptRouterArn": ...,
}

parent.get_prompt_router(**kwargs)
```

1. See [:material-code-braces: GetPromptRouterRequestTypeDef](./type_defs.md#getpromptrouterrequesttypedef) 

### get\_provisioned\_model\_throughput

Returns details for a Provisioned Throughput.

Type annotations and code completion for `#!python session.create_client("bedrock").get_provisioned_model_throughput` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/get_provisioned_model_throughput.html)

```python
# get_provisioned_model_throughput method definition

await def get_provisioned_model_throughput(
    self,
    *,
    provisionedModelId: str,
) -> GetProvisionedModelThroughputResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetProvisionedModelThroughputResponseTypeDef](./type_defs.md#getprovisionedmodelthroughputresponsetypedef) 


```python
# get_provisioned_model_throughput method usage example with argument unpacking

kwargs: GetProvisionedModelThroughputRequestTypeDef = {  # (1)
    "provisionedModelId": ...,
}

parent.get_provisioned_model_throughput(**kwargs)
```

1. See [:material-code-braces: GetProvisionedModelThroughputRequestTypeDef](./type_defs.md#getprovisionedmodelthroughputrequesttypedef) 

### list\_custom\_models

Returns a list of the custom models that you have created with the
<code>CreateModelCustomizationJob</code> operation.

Type annotations and code completion for `#!python session.create_client("bedrock").list_custom_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_custom_models.html)

```python
# list_custom_models method definition

await def list_custom_models(
    self,
    *,
    creationTimeBefore: TimestampTypeDef = ...,
    creationTimeAfter: TimestampTypeDef = ...,
    nameContains: str = ...,
    baseModelArnEquals: str = ...,
    foundationModelArnEquals: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortModelsByType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
    isOwned: bool = ...,
) -> ListCustomModelsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortModelsByType](./literals.md#sortmodelsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListCustomModelsResponseTypeDef](./type_defs.md#listcustommodelsresponsetypedef) 


```python
# list_custom_models method usage example with argument unpacking

kwargs: ListCustomModelsRequestTypeDef = {  # (1)
    "creationTimeBefore": ...,
}

parent.list_custom_models(**kwargs)
```

1. See [:material-code-braces: ListCustomModelsRequestTypeDef](./type_defs.md#listcustommodelsrequesttypedef) 

### list\_evaluation\_jobs

Lists all existing evaluation jobs.

Type annotations and code completion for `#!python session.create_client("bedrock").list_evaluation_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_evaluation_jobs.html)

```python
# list_evaluation_jobs method definition

await def list_evaluation_jobs(
    self,
    *,
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    statusEquals: EvaluationJobStatusType = ...,  # (1)
    applicationTypeEquals: ApplicationTypeType = ...,  # (2)
    nameContains: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortJobsByType = ...,  # (3)
    sortOrder: SortOrderType = ...,  # (4)
) -> ListEvaluationJobsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: EvaluationJobStatusType](./literals.md#evaluationjobstatustype) 
2. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
3. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: ListEvaluationJobsResponseTypeDef](./type_defs.md#listevaluationjobsresponsetypedef) 


```python
# list_evaluation_jobs method usage example with argument unpacking

kwargs: ListEvaluationJobsRequestTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.list_evaluation_jobs(**kwargs)
```

1. See [:material-code-braces: ListEvaluationJobsRequestTypeDef](./type_defs.md#listevaluationjobsrequesttypedef) 

### list\_foundation\_models

Lists Amazon Bedrock foundation models that you can use.

Type annotations and code completion for `#!python session.create_client("bedrock").list_foundation_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_foundation_models.html)

```python
# list_foundation_models method definition

await def list_foundation_models(
    self,
    *,
    byProvider: str = ...,
    byCustomizationType: ModelCustomizationType = ...,  # (1)
    byOutputModality: ModelModalityType = ...,  # (2)
    byInferenceType: InferenceTypeType = ...,  # (3)
) -> ListFoundationModelsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelCustomizationType](./literals.md#modelcustomizationtype) 
2. See [:material-code-brackets: ModelModalityType](./literals.md#modelmodalitytype) 
3. See [:material-code-brackets: InferenceTypeType](./literals.md#inferencetypetype) 
4. See [:material-code-braces: ListFoundationModelsResponseTypeDef](./type_defs.md#listfoundationmodelsresponsetypedef) 


```python
# list_foundation_models method usage example with argument unpacking

kwargs: ListFoundationModelsRequestTypeDef = {  # (1)
    "byProvider": ...,
}

parent.list_foundation_models(**kwargs)
```

1. See [:material-code-braces: ListFoundationModelsRequestTypeDef](./type_defs.md#listfoundationmodelsrequesttypedef) 

### list\_guardrails

Lists details about all the guardrails in an account.

Type annotations and code completion for `#!python session.create_client("bedrock").list_guardrails` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_guardrails.html)

```python
# list_guardrails method definition

await def list_guardrails(
    self,
    *,
    guardrailIdentifier: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListGuardrailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGuardrailsResponseTypeDef](./type_defs.md#listguardrailsresponsetypedef) 


```python
# list_guardrails method usage example with argument unpacking

kwargs: ListGuardrailsRequestTypeDef = {  # (1)
    "guardrailIdentifier": ...,
}

parent.list_guardrails(**kwargs)
```

1. See [:material-code-braces: ListGuardrailsRequestTypeDef](./type_defs.md#listguardrailsrequesttypedef) 

### list\_imported\_models

Returns a list of models you've imported.

Type annotations and code completion for `#!python session.create_client("bedrock").list_imported_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_imported_models.html)

```python
# list_imported_models method definition

await def list_imported_models(
    self,
    *,
    creationTimeBefore: TimestampTypeDef = ...,
    creationTimeAfter: TimestampTypeDef = ...,
    nameContains: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortModelsByType = ...,  # (1)
    sortOrder: SortOrderType = ...,  # (2)
) -> ListImportedModelsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortModelsByType](./literals.md#sortmodelsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: ListImportedModelsResponseTypeDef](./type_defs.md#listimportedmodelsresponsetypedef) 


```python
# list_imported_models method usage example with argument unpacking

kwargs: ListImportedModelsRequestTypeDef = {  # (1)
    "creationTimeBefore": ...,
}

parent.list_imported_models(**kwargs)
```

1. See [:material-code-braces: ListImportedModelsRequestTypeDef](./type_defs.md#listimportedmodelsrequesttypedef) 

### list\_inference\_profiles

Returns a list of inference profiles that you can use.

Type annotations and code completion for `#!python session.create_client("bedrock").list_inference_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_inference_profiles.html)

```python
# list_inference_profiles method definition

await def list_inference_profiles(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    typeEquals: InferenceProfileTypeType = ...,  # (1)
) -> ListInferenceProfilesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: InferenceProfileTypeType](./literals.md#inferenceprofiletypetype) 
2. See [:material-code-braces: ListInferenceProfilesResponseTypeDef](./type_defs.md#listinferenceprofilesresponsetypedef) 


```python
# list_inference_profiles method usage example with argument unpacking

kwargs: ListInferenceProfilesRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_inference_profiles(**kwargs)
```

1. See [:material-code-braces: ListInferenceProfilesRequestTypeDef](./type_defs.md#listinferenceprofilesrequesttypedef) 

### list\_marketplace\_model\_endpoints

Lists the endpoints for models from Amazon Bedrock Marketplace in your Amazon
Web Services account.

Type annotations and code completion for `#!python session.create_client("bedrock").list_marketplace_model_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_marketplace_model_endpoints.html)

```python
# list_marketplace_model_endpoints method definition

await def list_marketplace_model_endpoints(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    modelSourceEquals: str = ...,
) -> ListMarketplaceModelEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMarketplaceModelEndpointsResponseTypeDef](./type_defs.md#listmarketplacemodelendpointsresponsetypedef) 


```python
# list_marketplace_model_endpoints method usage example with argument unpacking

kwargs: ListMarketplaceModelEndpointsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_marketplace_model_endpoints(**kwargs)
```

1. See [:material-code-braces: ListMarketplaceModelEndpointsRequestTypeDef](./type_defs.md#listmarketplacemodelendpointsrequesttypedef) 

### list\_model\_copy\_jobs

Returns a list of model copy jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("bedrock").list_model_copy_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_model_copy_jobs.html)

```python
# list_model_copy_jobs method definition

await def list_model_copy_jobs(
    self,
    *,
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    statusEquals: ModelCopyJobStatusType = ...,  # (1)
    sourceAccountEquals: str = ...,
    sourceModelArnEquals: str = ...,
    targetModelNameContains: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortJobsByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
) -> ListModelCopyJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelCopyJobStatusType](./literals.md#modelcopyjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListModelCopyJobsResponseTypeDef](./type_defs.md#listmodelcopyjobsresponsetypedef) 


```python
# list_model_copy_jobs method usage example with argument unpacking

kwargs: ListModelCopyJobsRequestTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.list_model_copy_jobs(**kwargs)
```

1. See [:material-code-braces: ListModelCopyJobsRequestTypeDef](./type_defs.md#listmodelcopyjobsrequesttypedef) 

### list\_model\_customization\_jobs

Returns a list of model customization jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("bedrock").list_model_customization_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_model_customization_jobs.html)

```python
# list_model_customization_jobs method definition

await def list_model_customization_jobs(
    self,
    *,
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    statusEquals: FineTuningJobStatusType = ...,  # (1)
    nameContains: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortJobsByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
) -> ListModelCustomizationJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: FineTuningJobStatusType](./literals.md#finetuningjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListModelCustomizationJobsResponseTypeDef](./type_defs.md#listmodelcustomizationjobsresponsetypedef) 


```python
# list_model_customization_jobs method usage example with argument unpacking

kwargs: ListModelCustomizationJobsRequestTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.list_model_customization_jobs(**kwargs)
```

1. See [:material-code-braces: ListModelCustomizationJobsRequestTypeDef](./type_defs.md#listmodelcustomizationjobsrequesttypedef) 

### list\_model\_import\_jobs

Returns a list of import jobs you've submitted.

Type annotations and code completion for `#!python session.create_client("bedrock").list_model_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_model_import_jobs.html)

```python
# list_model_import_jobs method definition

await def list_model_import_jobs(
    self,
    *,
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    statusEquals: ModelImportJobStatusType = ...,  # (1)
    nameContains: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortJobsByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
) -> ListModelImportJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelImportJobStatusType](./literals.md#modelimportjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListModelImportJobsResponseTypeDef](./type_defs.md#listmodelimportjobsresponsetypedef) 


```python
# list_model_import_jobs method usage example with argument unpacking

kwargs: ListModelImportJobsRequestTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.list_model_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListModelImportJobsRequestTypeDef](./type_defs.md#listmodelimportjobsrequesttypedef) 

### list\_model\_invocation\_jobs

Lists all batch inference jobs in the account.

Type annotations and code completion for `#!python session.create_client("bedrock").list_model_invocation_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_model_invocation_jobs.html)

```python
# list_model_invocation_jobs method definition

await def list_model_invocation_jobs(
    self,
    *,
    submitTimeAfter: TimestampTypeDef = ...,
    submitTimeBefore: TimestampTypeDef = ...,
    statusEquals: ModelInvocationJobStatusType = ...,  # (1)
    nameContains: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortJobsByType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
) -> ListModelInvocationJobsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ModelInvocationJobStatusType](./literals.md#modelinvocationjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListModelInvocationJobsResponseTypeDef](./type_defs.md#listmodelinvocationjobsresponsetypedef) 


```python
# list_model_invocation_jobs method usage example with argument unpacking

kwargs: ListModelInvocationJobsRequestTypeDef = {  # (1)
    "submitTimeAfter": ...,
}

parent.list_model_invocation_jobs(**kwargs)
```

1. See [:material-code-braces: ListModelInvocationJobsRequestTypeDef](./type_defs.md#listmodelinvocationjobsrequesttypedef) 

### list\_prompt\_routers

Retrieves a list of prompt routers.

Type annotations and code completion for `#!python session.create_client("bedrock").list_prompt_routers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_prompt_routers.html)

```python
# list_prompt_routers method definition

await def list_prompt_routers(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListPromptRoutersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPromptRoutersResponseTypeDef](./type_defs.md#listpromptroutersresponsetypedef) 


```python
# list_prompt_routers method usage example with argument unpacking

kwargs: ListPromptRoutersRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_prompt_routers(**kwargs)
```

1. See [:material-code-braces: ListPromptRoutersRequestTypeDef](./type_defs.md#listpromptroutersrequesttypedef) 

### list\_provisioned\_model\_throughputs

Lists the Provisioned Throughputs in the account.

Type annotations and code completion for `#!python session.create_client("bedrock").list_provisioned_model_throughputs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_provisioned_model_throughputs.html)

```python
# list_provisioned_model_throughputs method definition

await def list_provisioned_model_throughputs(
    self,
    *,
    creationTimeAfter: TimestampTypeDef = ...,
    creationTimeBefore: TimestampTypeDef = ...,
    statusEquals: ProvisionedModelStatusType = ...,  # (1)
    modelArnEquals: str = ...,
    nameContains: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: SortByProvisionedModelsType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
) -> ListProvisionedModelThroughputsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype) 
2. See [:material-code-brackets: SortByProvisionedModelsType](./literals.md#sortbyprovisionedmodelstype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: ListProvisionedModelThroughputsResponseTypeDef](./type_defs.md#listprovisionedmodelthroughputsresponsetypedef) 


```python
# list_provisioned_model_throughputs method usage example with argument unpacking

kwargs: ListProvisionedModelThroughputsRequestTypeDef = {  # (1)
    "creationTimeAfter": ...,
}

parent.list_provisioned_model_throughputs(**kwargs)
```

1. See [:material-code-braces: ListProvisionedModelThroughputsRequestTypeDef](./type_defs.md#listprovisionedmodelthroughputsrequesttypedef) 

### list\_tags\_for\_resource

List the tags associated with the specified resource.

Type annotations and code completion for `#!python session.create_client("bedrock").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### put\_model\_invocation\_logging\_configuration

Set the configuration values for model invocation logging.

Type annotations and code completion for `#!python session.create_client("bedrock").put_model_invocation_logging_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/put_model_invocation_logging_configuration.html)

```python
# put_model_invocation_logging_configuration method definition

await def put_model_invocation_logging_configuration(
    self,
    *,
    loggingConfig: LoggingConfigTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 


```python
# put_model_invocation_logging_configuration method usage example with argument unpacking

kwargs: PutModelInvocationLoggingConfigurationRequestTypeDef = {  # (1)
    "loggingConfig": ...,
}

parent.put_model_invocation_logging_configuration(**kwargs)
```

1. See [:material-code-braces: PutModelInvocationLoggingConfigurationRequestTypeDef](./type_defs.md#putmodelinvocationloggingconfigurationrequesttypedef) 

### register\_marketplace\_model\_endpoint

Registers an existing Amazon SageMaker endpoint with Amazon Bedrock
Marketplace, allowing it to be used with Amazon Bedrock APIs.

Type annotations and code completion for `#!python session.create_client("bedrock").register_marketplace_model_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/register_marketplace_model_endpoint.html)

```python
# register_marketplace_model_endpoint method definition

await def register_marketplace_model_endpoint(
    self,
    *,
    endpointIdentifier: str,
    modelSourceIdentifier: str,
) -> RegisterMarketplaceModelEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterMarketplaceModelEndpointResponseTypeDef](./type_defs.md#registermarketplacemodelendpointresponsetypedef) 


```python
# register_marketplace_model_endpoint method usage example with argument unpacking

kwargs: RegisterMarketplaceModelEndpointRequestTypeDef = {  # (1)
    "endpointIdentifier": ...,
    "modelSourceIdentifier": ...,
}

parent.register_marketplace_model_endpoint(**kwargs)
```

1. See [:material-code-braces: RegisterMarketplaceModelEndpointRequestTypeDef](./type_defs.md#registermarketplacemodelendpointrequesttypedef) 

### stop\_evaluation\_job

Stops an evaluation job that is current being created or running.

Type annotations and code completion for `#!python session.create_client("bedrock").stop_evaluation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/stop_evaluation_job.html)

```python
# stop_evaluation_job method definition

await def stop_evaluation_job(
    self,
    *,
    jobIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_evaluation_job method usage example with argument unpacking

kwargs: StopEvaluationJobRequestTypeDef = {  # (1)
    "jobIdentifier": ...,
}

parent.stop_evaluation_job(**kwargs)
```

1. See [:material-code-braces: StopEvaluationJobRequestTypeDef](./type_defs.md#stopevaluationjobrequesttypedef) 

### stop\_model\_customization\_job

Stops an active model customization job.

Type annotations and code completion for `#!python session.create_client("bedrock").stop_model_customization_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/stop_model_customization_job.html)

```python
# stop_model_customization_job method definition

await def stop_model_customization_job(
    self,
    *,
    jobIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_model_customization_job method usage example with argument unpacking

kwargs: StopModelCustomizationJobRequestTypeDef = {  # (1)
    "jobIdentifier": ...,
}

parent.stop_model_customization_job(**kwargs)
```

1. See [:material-code-braces: StopModelCustomizationJobRequestTypeDef](./type_defs.md#stopmodelcustomizationjobrequesttypedef) 

### stop\_model\_invocation\_job

Stops a batch inference job.

Type annotations and code completion for `#!python session.create_client("bedrock").stop_model_invocation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/stop_model_invocation_job.html)

```python
# stop_model_invocation_job method definition

await def stop_model_invocation_job(
    self,
    *,
    jobIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_model_invocation_job method usage example with argument unpacking

kwargs: StopModelInvocationJobRequestTypeDef = {  # (1)
    "jobIdentifier": ...,
}

parent.stop_model_invocation_job(**kwargs)
```

1. See [:material-code-braces: StopModelInvocationJobRequestTypeDef](./type_defs.md#stopmodelinvocationjobrequesttypedef) 

### tag\_resource

Associate tags with a resource.

Type annotations and code completion for `#!python session.create_client("bedrock").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceARN: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Remove one or more tags from a resource.

Type annotations and code completion for `#!python session.create_client("bedrock").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceARN: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceARN": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_guardrail

Updates a guardrail with the values you specify.

Type annotations and code completion for `#!python session.create_client("bedrock").update_guardrail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/update_guardrail.html)

```python
# update_guardrail method definition

await def update_guardrail(
    self,
    *,
    guardrailIdentifier: str,
    name: str,
    blockedInputMessaging: str,
    blockedOutputsMessaging: str,
    description: str = ...,
    topicPolicyConfig: GuardrailTopicPolicyConfigTypeDef = ...,  # (1)
    contentPolicyConfig: GuardrailContentPolicyConfigTypeDef = ...,  # (2)
    wordPolicyConfig: GuardrailWordPolicyConfigTypeDef = ...,  # (3)
    sensitiveInformationPolicyConfig: GuardrailSensitiveInformationPolicyConfigTypeDef = ...,  # (4)
    contextualGroundingPolicyConfig: GuardrailContextualGroundingPolicyConfigTypeDef = ...,  # (5)
    kmsKeyId: str = ...,
) -> UpdateGuardrailResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: GuardrailTopicPolicyConfigTypeDef](./type_defs.md#guardrailtopicpolicyconfigtypedef) 
2. See [:material-code-braces: GuardrailContentPolicyConfigTypeDef](./type_defs.md#guardrailcontentpolicyconfigtypedef) 
3. See [:material-code-braces: GuardrailWordPolicyConfigTypeDef](./type_defs.md#guardrailwordpolicyconfigtypedef) 
4. See [:material-code-braces: GuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyconfigtypedef) 
5. See [:material-code-braces: GuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#guardrailcontextualgroundingpolicyconfigtypedef) 
6. See [:material-code-braces: UpdateGuardrailResponseTypeDef](./type_defs.md#updateguardrailresponsetypedef) 


```python
# update_guardrail method usage example with argument unpacking

kwargs: UpdateGuardrailRequestTypeDef = {  # (1)
    "guardrailIdentifier": ...,
    "name": ...,
    "blockedInputMessaging": ...,
    "blockedOutputsMessaging": ...,
}

parent.update_guardrail(**kwargs)
```

1. See [:material-code-braces: UpdateGuardrailRequestTypeDef](./type_defs.md#updateguardrailrequesttypedef) 

### update\_marketplace\_model\_endpoint

Updates the configuration of an existing endpoint for a model from Amazon
Bedrock Marketplace.

Type annotations and code completion for `#!python session.create_client("bedrock").update_marketplace_model_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/update_marketplace_model_endpoint.html)

```python
# update_marketplace_model_endpoint method definition

await def update_marketplace_model_endpoint(
    self,
    *,
    endpointArn: str,
    endpointConfig: EndpointConfigUnionTypeDef,  # (1)
    clientRequestToken: str = ...,
) -> UpdateMarketplaceModelEndpointResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EndpointConfigTypeDef](./type_defs.md#endpointconfigtypedef) [:material-code-braces: EndpointConfigOutputTypeDef](./type_defs.md#endpointconfigoutputtypedef) 
2. See [:material-code-braces: UpdateMarketplaceModelEndpointResponseTypeDef](./type_defs.md#updatemarketplacemodelendpointresponsetypedef) 


```python
# update_marketplace_model_endpoint method usage example with argument unpacking

kwargs: UpdateMarketplaceModelEndpointRequestTypeDef = {  # (1)
    "endpointArn": ...,
    "endpointConfig": ...,
}

parent.update_marketplace_model_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateMarketplaceModelEndpointRequestTypeDef](./type_defs.md#updatemarketplacemodelendpointrequesttypedef) 

### update\_provisioned\_model\_throughput

Updates the name or associated model for a Provisioned Throughput.

Type annotations and code completion for `#!python session.create_client("bedrock").update_provisioned_model_throughput` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock/client/update_provisioned_model_throughput.html)

```python
# update_provisioned_model_throughput method definition

await def update_provisioned_model_throughput(
    self,
    *,
    provisionedModelId: str,
    desiredProvisionedModelName: str = ...,
    desiredModelId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_provisioned_model_throughput method usage example with argument unpacking

kwargs: UpdateProvisionedModelThroughputRequestTypeDef = {  # (1)
    "provisionedModelId": ...,
}

parent.update_provisioned_model_throughput(**kwargs)
```

1. See [:material-code-braces: UpdateProvisionedModelThroughputRequestTypeDef](./type_defs.md#updateprovisionedmodelthroughputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("bedrock").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("bedrock").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#Bedrock.Client)

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

Type annotations and code completion for `#!python session.create_client("bedrock").get_paginator` method with overloads.

- `client.get_paginator("list_custom_models")` -> [ListCustomModelsPaginator](./paginators.md#listcustommodelspaginator)
- `client.get_paginator("list_evaluation_jobs")` -> [ListEvaluationJobsPaginator](./paginators.md#listevaluationjobspaginator)
- `client.get_paginator("list_guardrails")` -> [ListGuardrailsPaginator](./paginators.md#listguardrailspaginator)
- `client.get_paginator("list_imported_models")` -> [ListImportedModelsPaginator](./paginators.md#listimportedmodelspaginator)
- `client.get_paginator("list_inference_profiles")` -> [ListInferenceProfilesPaginator](./paginators.md#listinferenceprofilespaginator)
- `client.get_paginator("list_marketplace_model_endpoints")` -> [ListMarketplaceModelEndpointsPaginator](./paginators.md#listmarketplacemodelendpointspaginator)
- `client.get_paginator("list_model_copy_jobs")` -> [ListModelCopyJobsPaginator](./paginators.md#listmodelcopyjobspaginator)
- `client.get_paginator("list_model_customization_jobs")` -> [ListModelCustomizationJobsPaginator](./paginators.md#listmodelcustomizationjobspaginator)
- `client.get_paginator("list_model_import_jobs")` -> [ListModelImportJobsPaginator](./paginators.md#listmodelimportjobspaginator)
- `client.get_paginator("list_model_invocation_jobs")` -> [ListModelInvocationJobsPaginator](./paginators.md#listmodelinvocationjobspaginator)
- `client.get_paginator("list_prompt_routers")` -> [ListPromptRoutersPaginator](./paginators.md#listpromptrouterspaginator)
- `client.get_paginator("list_provisioned_model_throughputs")` -> [ListProvisionedModelThroughputsPaginator](./paginators.md#listprovisionedmodelthroughputspaginator)



