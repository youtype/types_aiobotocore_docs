# CleanRoomsMLClient

> [Index](../README.md) > [CleanRoomsML](./README.md) > CleanRoomsMLClient

!!! note ""

    Auto-generated documentation for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML)
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

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_audience\_model

Defines the information necessary to create an audience model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").create_audience_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_audience_model)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_configured_audience_model)

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

### create\_training\_dataset

Defines the information necessary to create a training dataset.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").create_training_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.create_training_dataset)

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
with the
job.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_audience_generation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.delete_audience_generation_job)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.delete_audience_model)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.delete_configured_audience_model)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.delete_configured_audience_model_policy)

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

### delete\_training\_dataset

Specifies a training dataset that you want to delete.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").delete_training_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.delete_training_dataset)

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

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.generate_presigned_url)

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


### get\_audience\_generation\_job

Returns information about an audience generation job.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_audience_generation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.get_audience_generation_job)

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

Returns information about an audience model See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/cleanroomsml-2023-09-06/GetAudienceModel).

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_audience_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.get_audience_model)

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

### get\_configured\_audience\_model

Returns information about a specified configured audience model.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_configured_audience_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.get_configured_audience_model)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.get_configured_audience_model_policy)

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

### get\_training\_dataset

Returns information about a training dataset.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_training_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.get_training_dataset)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.list_audience_export_jobs)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.list_audience_generation_jobs)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.list_audience_models)

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

### list\_configured\_audience\_models

Returns a list of the configured audience models.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_configured_audience_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.list_configured_audience_models)

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

### list\_tags\_for\_resource

Returns a list of tags for a provided resource.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.list_tags_for_resource)

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

### list\_training\_datasets

Returns a list of training datasets.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").list_training_datasets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.list_training_datasets)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.put_configured_audience_model_policy)

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

### start\_audience\_export\_job

Export an audience of a specified size after you have generated an audience.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").start_audience_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.start_audience_export_job)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.start_audience_generation_job)

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

### tag\_resource

Adds metadata tags to a specified resource.

Type annotations and code completion for `#!python session.create_client("cleanroomsml").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.tag_resource)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.untag_resource)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.update_configured_audience_model)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CleanRoomsMLClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cleanroomsml").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#CleanRoomsML.Client.__aexit__)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("cleanroomsml").get_paginator` method with overloads.

- `client.get_paginator("list_audience_export_jobs")` -> [ListAudienceExportJobsPaginator](./paginators.md#listaudienceexportjobspaginator)
- `client.get_paginator("list_audience_generation_jobs")` -> [ListAudienceGenerationJobsPaginator](./paginators.md#listaudiencegenerationjobspaginator)
- `client.get_paginator("list_audience_models")` -> [ListAudienceModelsPaginator](./paginators.md#listaudiencemodelspaginator)
- `client.get_paginator("list_configured_audience_models")` -> [ListConfiguredAudienceModelsPaginator](./paginators.md#listconfiguredaudiencemodelspaginator)
- `client.get_paginator("list_training_datasets")` -> [ListTrainingDatasetsPaginator](./paginators.md#listtrainingdatasetspaginator)



