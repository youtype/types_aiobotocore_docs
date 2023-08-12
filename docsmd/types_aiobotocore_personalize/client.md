# PersonalizeClient

> [Index](../README.md) > [Personalize](./README.md) > PersonalizeClient

!!! note ""

    Auto-generated documentation for [Personalize](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
    type annotations stubs module [types-aiobotocore-personalize](https://pypi.org/project/types-aiobotocore-personalize/).

## PersonalizeClient

Type annotations and code completion for `#!python session.create_client("personalize")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client)

```python
PersonalizeClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_personalize.client import PersonalizeClient

session = get_session()
async with session.create_client("personalize") as client:
    client: PersonalizeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("personalize").exceptions` structure.

```python
PersonalizeClient.exceptions usage example

async with session.create_client("personalize") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InvalidInputException,
        client.InvalidNextTokenException,
        client.LimitExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
        client.TooManyTagKeysException,
        client.TooManyTagsException,
    ) as e:
        print(e)
```

```python
PersonalizeClient usage type checking example

from types_aiobotocore_personalize.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("personalize").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("personalize").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_batch\_inference\_job

Creates a batch inference job.

Type annotations and code completion for `#!python session.create_client("personalize").create_batch_inference_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_inference_job)

```python
# create_batch_inference_job method definition

await def create_batch_inference_job(
    self,
    *,
    jobName: str,
    solutionVersionArn: str,
    jobInput: BatchInferenceJobInputTypeDef,  # (1)
    jobOutput: BatchInferenceJobOutputTypeDef,  # (2)
    roleArn: str,
    filterArn: str = ...,
    numResults: int = ...,
    batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,  # (3)
    tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateBatchInferenceJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: BatchInferenceJobInputTypeDef](./type_defs.md#batchinferencejobinputtypedef) 
2. See [:material-code-braces: BatchInferenceJobOutputTypeDef](./type_defs.md#batchinferencejoboutputtypedef) 
3. See [:material-code-braces: BatchInferenceJobConfigTypeDef](./type_defs.md#batchinferencejobconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateBatchInferenceJobResponseTypeDef](./type_defs.md#createbatchinferencejobresponsetypedef) 


```python
# create_batch_inference_job method usage example with argument unpacking

kwargs: CreateBatchInferenceJobRequestRequestTypeDef = {  # (1)
    "jobName": ...,
    "solutionVersionArn": ...,
    "jobInput": ...,
    "jobOutput": ...,
    "roleArn": ...,
}

parent.create_batch_inference_job(**kwargs)
```

1. See [:material-code-braces: CreateBatchInferenceJobRequestRequestTypeDef](./type_defs.md#createbatchinferencejobrequestrequesttypedef) 

### create\_batch\_segment\_job

Creates a batch segment job.

Type annotations and code completion for `#!python session.create_client("personalize").create_batch_segment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_segment_job)

```python
# create_batch_segment_job method definition

await def create_batch_segment_job(
    self,
    *,
    jobName: str,
    solutionVersionArn: str,
    jobInput: BatchSegmentJobInputTypeDef,  # (1)
    jobOutput: BatchSegmentJobOutputTypeDef,  # (2)
    roleArn: str,
    filterArn: str = ...,
    numResults: int = ...,
    tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateBatchSegmentJobResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: BatchSegmentJobInputTypeDef](./type_defs.md#batchsegmentjobinputtypedef) 
2. See [:material-code-braces: BatchSegmentJobOutputTypeDef](./type_defs.md#batchsegmentjoboutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateBatchSegmentJobResponseTypeDef](./type_defs.md#createbatchsegmentjobresponsetypedef) 


```python
# create_batch_segment_job method usage example with argument unpacking

kwargs: CreateBatchSegmentJobRequestRequestTypeDef = {  # (1)
    "jobName": ...,
    "solutionVersionArn": ...,
    "jobInput": ...,
    "jobOutput": ...,
    "roleArn": ...,
}

parent.create_batch_segment_job(**kwargs)
```

1. See [:material-code-braces: CreateBatchSegmentJobRequestRequestTypeDef](./type_defs.md#createbatchsegmentjobrequestrequesttypedef) 

### create\_campaign

Creates a campaign that deploys a solution version.

Type annotations and code completion for `#!python session.create_client("personalize").create_campaign` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)

```python
# create_campaign method definition

await def create_campaign(
    self,
    *,
    name: str,
    solutionVersionArn: str,
    minProvisionedTPS: int = ...,
    campaignConfig: CampaignConfigTypeDef = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateCampaignResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CampaignConfigTypeDef](./type_defs.md#campaignconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateCampaignResponseTypeDef](./type_defs.md#createcampaignresponsetypedef) 


```python
# create_campaign method usage example with argument unpacking

kwargs: CreateCampaignRequestRequestTypeDef = {  # (1)
    "name": ...,
    "solutionVersionArn": ...,
}

parent.create_campaign(**kwargs)
```

1. See [:material-code-braces: CreateCampaignRequestRequestTypeDef](./type_defs.md#createcampaignrequestrequesttypedef) 

### create\_dataset

Creates an empty dataset and adds it to the specified dataset group.

Type annotations and code completion for `#!python session.create_client("personalize").create_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset)

```python
# create_dataset method definition

await def create_dataset(
    self,
    *,
    name: str,
    schemaArn: str,
    datasetGroupArn: str,
    datasetType: str,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateDatasetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef) 


```python
# create_dataset method usage example with argument unpacking

kwargs: CreateDatasetRequestRequestTypeDef = {  # (1)
    "name": ...,
    "schemaArn": ...,
    "datasetGroupArn": ...,
    "datasetType": ...,
}

parent.create_dataset(**kwargs)
```

1. See [:material-code-braces: CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef) 

### create\_dataset\_export\_job

Creates a job that exports data from your dataset to an Amazon S3 bucket.

Type annotations and code completion for `#!python session.create_client("personalize").create_dataset_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_export_job)

```python
# create_dataset_export_job method definition

await def create_dataset_export_job(
    self,
    *,
    jobName: str,
    datasetArn: str,
    roleArn: str,
    jobOutput: DatasetExportJobOutputTypeDef,  # (1)
    ingestionMode: IngestionModeType = ...,  # (2)
    tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateDatasetExportJobResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DatasetExportJobOutputTypeDef](./type_defs.md#datasetexportjoboutputtypedef) 
2. See [:material-code-brackets: IngestionModeType](./literals.md#ingestionmodetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateDatasetExportJobResponseTypeDef](./type_defs.md#createdatasetexportjobresponsetypedef) 


```python
# create_dataset_export_job method usage example with argument unpacking

kwargs: CreateDatasetExportJobRequestRequestTypeDef = {  # (1)
    "jobName": ...,
    "datasetArn": ...,
    "roleArn": ...,
    "jobOutput": ...,
}

parent.create_dataset_export_job(**kwargs)
```

1. See [:material-code-braces: CreateDatasetExportJobRequestRequestTypeDef](./type_defs.md#createdatasetexportjobrequestrequesttypedef) 

### create\_dataset\_group

Creates an empty dataset group.

Type annotations and code completion for `#!python session.create_client("personalize").create_dataset_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_group)

```python
# create_dataset_group method definition

await def create_dataset_group(
    self,
    *,
    name: str,
    roleArn: str = ...,
    kmsKeyArn: str = ...,
    domain: DomainType = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateDatasetGroupResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DomainType](./literals.md#domaintype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDatasetGroupResponseTypeDef](./type_defs.md#createdatasetgroupresponsetypedef) 


```python
# create_dataset_group method usage example with argument unpacking

kwargs: CreateDatasetGroupRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_dataset_group(**kwargs)
```

1. See [:material-code-braces: CreateDatasetGroupRequestRequestTypeDef](./type_defs.md#createdatasetgrouprequestrequesttypedef) 

### create\_dataset\_import\_job

Creates a job that imports training data from your data source (an Amazon S3
bucket) to an Amazon Personalize dataset.

Type annotations and code completion for `#!python session.create_client("personalize").create_dataset_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_import_job)

```python
# create_dataset_import_job method definition

await def create_dataset_import_job(
    self,
    *,
    jobName: str,
    datasetArn: str,
    dataSource: DataSourceTypeDef,  # (1)
    roleArn: str,
    tags: Sequence[TagTypeDef] = ...,  # (2)
    importMode: ImportModeType = ...,  # (3)
    publishAttributionMetricsToS3: bool = ...,
) -> CreateDatasetImportJobResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: ImportModeType](./literals.md#importmodetype) 
4. See [:material-code-braces: CreateDatasetImportJobResponseTypeDef](./type_defs.md#createdatasetimportjobresponsetypedef) 


```python
# create_dataset_import_job method usage example with argument unpacking

kwargs: CreateDatasetImportJobRequestRequestTypeDef = {  # (1)
    "jobName": ...,
    "datasetArn": ...,
    "dataSource": ...,
    "roleArn": ...,
}

parent.create_dataset_import_job(**kwargs)
```

1. See [:material-code-braces: CreateDatasetImportJobRequestRequestTypeDef](./type_defs.md#createdatasetimportjobrequestrequesttypedef) 

### create\_event\_tracker

Creates an event tracker that you use when adding event data to a specified
dataset group using the
[PutEvents](https://docs.aws.amazon.com/personalize/latest/dg/API_UBS_PutEvents.html)_
API.

Type annotations and code completion for `#!python session.create_client("personalize").create_event_tracker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_event_tracker)

```python
# create_event_tracker method definition

await def create_event_tracker(
    self,
    *,
    name: str,
    datasetGroupArn: str,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateEventTrackerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateEventTrackerResponseTypeDef](./type_defs.md#createeventtrackerresponsetypedef) 


```python
# create_event_tracker method usage example with argument unpacking

kwargs: CreateEventTrackerRequestRequestTypeDef = {  # (1)
    "name": ...,
    "datasetGroupArn": ...,
}

parent.create_event_tracker(**kwargs)
```

1. See [:material-code-braces: CreateEventTrackerRequestRequestTypeDef](./type_defs.md#createeventtrackerrequestrequesttypedef) 

### create\_filter

Creates a recommendation filter.

Type annotations and code completion for `#!python session.create_client("personalize").create_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_filter)

```python
# create_filter method definition

await def create_filter(
    self,
    *,
    name: str,
    datasetGroupArn: str,
    filterExpression: str,
    tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateFilterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateFilterResponseTypeDef](./type_defs.md#createfilterresponsetypedef) 


```python
# create_filter method usage example with argument unpacking

kwargs: CreateFilterRequestRequestTypeDef = {  # (1)
    "name": ...,
    "datasetGroupArn": ...,
    "filterExpression": ...,
}

parent.create_filter(**kwargs)
```

1. See [:material-code-braces: CreateFilterRequestRequestTypeDef](./type_defs.md#createfilterrequestrequesttypedef) 

### create\_metric\_attribution

Creates a metric attribution.

Type annotations and code completion for `#!python session.create_client("personalize").create_metric_attribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_metric_attribution)

```python
# create_metric_attribution method definition

await def create_metric_attribution(
    self,
    *,
    name: str,
    datasetGroupArn: str,
    metrics: Sequence[MetricAttributeTypeDef],  # (1)
    metricsOutputConfig: MetricAttributionOutputTypeDef,  # (2)
) -> CreateMetricAttributionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MetricAttributeTypeDef](./type_defs.md#metricattributetypedef) 
2. See [:material-code-braces: MetricAttributionOutputTypeDef](./type_defs.md#metricattributionoutputtypedef) 
3. See [:material-code-braces: CreateMetricAttributionResponseTypeDef](./type_defs.md#createmetricattributionresponsetypedef) 


```python
# create_metric_attribution method usage example with argument unpacking

kwargs: CreateMetricAttributionRequestRequestTypeDef = {  # (1)
    "name": ...,
    "datasetGroupArn": ...,
    "metrics": ...,
    "metricsOutputConfig": ...,
}

parent.create_metric_attribution(**kwargs)
```

1. See [:material-code-braces: CreateMetricAttributionRequestRequestTypeDef](./type_defs.md#createmetricattributionrequestrequesttypedef) 

### create\_recommender

Creates a recommender with the recipe (a Domain dataset group use case) you
specify.

Type annotations and code completion for `#!python session.create_client("personalize").create_recommender` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)

```python
# create_recommender method definition

await def create_recommender(
    self,
    *,
    name: str,
    datasetGroupArn: str,
    recipeArn: str,
    recommenderConfig: RecommenderConfigTypeDef = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateRecommenderResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RecommenderConfigTypeDef](./type_defs.md#recommenderconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateRecommenderResponseTypeDef](./type_defs.md#createrecommenderresponsetypedef) 


```python
# create_recommender method usage example with argument unpacking

kwargs: CreateRecommenderRequestRequestTypeDef = {  # (1)
    "name": ...,
    "datasetGroupArn": ...,
    "recipeArn": ...,
}

parent.create_recommender(**kwargs)
```

1. See [:material-code-braces: CreateRecommenderRequestRequestTypeDef](./type_defs.md#createrecommenderrequestrequesttypedef) 

### create\_schema

Creates an Amazon Personalize schema from the specified schema string.

Type annotations and code completion for `#!python session.create_client("personalize").create_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_schema)

```python
# create_schema method definition

await def create_schema(
    self,
    *,
    name: str,
    schema: str,
    domain: DomainType = ...,  # (1)
) -> CreateSchemaResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DomainType](./literals.md#domaintype) 
2. See [:material-code-braces: CreateSchemaResponseTypeDef](./type_defs.md#createschemaresponsetypedef) 


```python
# create_schema method usage example with argument unpacking

kwargs: CreateSchemaRequestRequestTypeDef = {  # (1)
    "name": ...,
    "schema": ...,
}

parent.create_schema(**kwargs)
```

1. See [:material-code-braces: CreateSchemaRequestRequestTypeDef](./type_defs.md#createschemarequestrequesttypedef) 

### create\_solution

Creates the configuration for training a model.

Type annotations and code completion for `#!python session.create_client("personalize").create_solution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)

```python
# create_solution method definition

await def create_solution(
    self,
    *,
    name: str,
    datasetGroupArn: str,
    performHPO: bool = ...,
    performAutoML: bool = ...,
    recipeArn: str = ...,
    eventType: str = ...,
    solutionConfig: SolutionConfigTypeDef = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateSolutionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SolutionConfigTypeDef](./type_defs.md#solutionconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateSolutionResponseTypeDef](./type_defs.md#createsolutionresponsetypedef) 


```python
# create_solution method usage example with argument unpacking

kwargs: CreateSolutionRequestRequestTypeDef = {  # (1)
    "name": ...,
    "datasetGroupArn": ...,
}

parent.create_solution(**kwargs)
```

1. See [:material-code-braces: CreateSolutionRequestRequestTypeDef](./type_defs.md#createsolutionrequestrequesttypedef) 

### create\_solution\_version

Trains or retrains an active solution in a Custom dataset group.

Type annotations and code completion for `#!python session.create_client("personalize").create_solution_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution_version)

```python
# create_solution_version method definition

await def create_solution_version(
    self,
    *,
    solutionArn: str,
    name: str = ...,
    trainingMode: TrainingModeType = ...,  # (1)
    tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateSolutionVersionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TrainingModeType](./literals.md#trainingmodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateSolutionVersionResponseTypeDef](./type_defs.md#createsolutionversionresponsetypedef) 


```python
# create_solution_version method usage example with argument unpacking

kwargs: CreateSolutionVersionRequestRequestTypeDef = {  # (1)
    "solutionArn": ...,
}

parent.create_solution_version(**kwargs)
```

1. See [:material-code-braces: CreateSolutionVersionRequestRequestTypeDef](./type_defs.md#createsolutionversionrequestrequesttypedef) 

### delete\_campaign

Removes a campaign by deleting the solution deployment.

Type annotations and code completion for `#!python session.create_client("personalize").delete_campaign` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_campaign)

```python
# delete_campaign method definition

await def delete_campaign(
    self,
    *,
    campaignArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_campaign method usage example with argument unpacking

kwargs: DeleteCampaignRequestRequestTypeDef = {  # (1)
    "campaignArn": ...,
}

parent.delete_campaign(**kwargs)
```

1. See [:material-code-braces: DeleteCampaignRequestRequestTypeDef](./type_defs.md#deletecampaignrequestrequesttypedef) 

### delete\_dataset

Deletes a dataset.

Type annotations and code completion for `#!python session.create_client("personalize").delete_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_dataset)

```python
# delete_dataset method definition

await def delete_dataset(
    self,
    *,
    datasetArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_dataset method usage example with argument unpacking

kwargs: DeleteDatasetRequestRequestTypeDef = {  # (1)
    "datasetArn": ...,
}

parent.delete_dataset(**kwargs)
```

1. See [:material-code-braces: DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef) 

### delete\_dataset\_group

Deletes a dataset group.

Type annotations and code completion for `#!python session.create_client("personalize").delete_dataset_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_dataset_group)

```python
# delete_dataset_group method definition

await def delete_dataset_group(
    self,
    *,
    datasetGroupArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_dataset_group method usage example with argument unpacking

kwargs: DeleteDatasetGroupRequestRequestTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.delete_dataset_group(**kwargs)
```

1. See [:material-code-braces: DeleteDatasetGroupRequestRequestTypeDef](./type_defs.md#deletedatasetgrouprequestrequesttypedef) 

### delete\_event\_tracker

Deletes the event tracker.

Type annotations and code completion for `#!python session.create_client("personalize").delete_event_tracker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_event_tracker)

```python
# delete_event_tracker method definition

await def delete_event_tracker(
    self,
    *,
    eventTrackerArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_event_tracker method usage example with argument unpacking

kwargs: DeleteEventTrackerRequestRequestTypeDef = {  # (1)
    "eventTrackerArn": ...,
}

parent.delete_event_tracker(**kwargs)
```

1. See [:material-code-braces: DeleteEventTrackerRequestRequestTypeDef](./type_defs.md#deleteeventtrackerrequestrequesttypedef) 

### delete\_filter

Deletes a filter.

Type annotations and code completion for `#!python session.create_client("personalize").delete_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_filter)

```python
# delete_filter method definition

await def delete_filter(
    self,
    *,
    filterArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_filter method usage example with argument unpacking

kwargs: DeleteFilterRequestRequestTypeDef = {  # (1)
    "filterArn": ...,
}

parent.delete_filter(**kwargs)
```

1. See [:material-code-braces: DeleteFilterRequestRequestTypeDef](./type_defs.md#deletefilterrequestrequesttypedef) 

### delete\_metric\_attribution

Deletes a metric attribution.

Type annotations and code completion for `#!python session.create_client("personalize").delete_metric_attribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_metric_attribution)

```python
# delete_metric_attribution method definition

await def delete_metric_attribution(
    self,
    *,
    metricAttributionArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_metric_attribution method usage example with argument unpacking

kwargs: DeleteMetricAttributionRequestRequestTypeDef = {  # (1)
    "metricAttributionArn": ...,
}

parent.delete_metric_attribution(**kwargs)
```

1. See [:material-code-braces: DeleteMetricAttributionRequestRequestTypeDef](./type_defs.md#deletemetricattributionrequestrequesttypedef) 

### delete\_recommender

Deactivates and removes a recommender.

Type annotations and code completion for `#!python session.create_client("personalize").delete_recommender` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_recommender)

```python
# delete_recommender method definition

await def delete_recommender(
    self,
    *,
    recommenderArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_recommender method usage example with argument unpacking

kwargs: DeleteRecommenderRequestRequestTypeDef = {  # (1)
    "recommenderArn": ...,
}

parent.delete_recommender(**kwargs)
```

1. See [:material-code-braces: DeleteRecommenderRequestRequestTypeDef](./type_defs.md#deleterecommenderrequestrequesttypedef) 

### delete\_schema

Deletes a schema.

Type annotations and code completion for `#!python session.create_client("personalize").delete_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_schema)

```python
# delete_schema method definition

await def delete_schema(
    self,
    *,
    schemaArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_schema method usage example with argument unpacking

kwargs: DeleteSchemaRequestRequestTypeDef = {  # (1)
    "schemaArn": ...,
}

parent.delete_schema(**kwargs)
```

1. See [:material-code-braces: DeleteSchemaRequestRequestTypeDef](./type_defs.md#deleteschemarequestrequesttypedef) 

### delete\_solution

Deletes all versions of a solution and the `Solution` object itself.

Type annotations and code completion for `#!python session.create_client("personalize").delete_solution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_solution)

```python
# delete_solution method definition

await def delete_solution(
    self,
    *,
    solutionArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_solution method usage example with argument unpacking

kwargs: DeleteSolutionRequestRequestTypeDef = {  # (1)
    "solutionArn": ...,
}

parent.delete_solution(**kwargs)
```

1. See [:material-code-braces: DeleteSolutionRequestRequestTypeDef](./type_defs.md#deletesolutionrequestrequesttypedef) 

### describe\_algorithm

Describes the given algorithm.

Type annotations and code completion for `#!python session.create_client("personalize").describe_algorithm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_algorithm)

```python
# describe_algorithm method definition

await def describe_algorithm(
    self,
    *,
    algorithmArn: str,
) -> DescribeAlgorithmResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAlgorithmResponseTypeDef](./type_defs.md#describealgorithmresponsetypedef) 


```python
# describe_algorithm method usage example with argument unpacking

kwargs: DescribeAlgorithmRequestRequestTypeDef = {  # (1)
    "algorithmArn": ...,
}

parent.describe_algorithm(**kwargs)
```

1. See [:material-code-braces: DescribeAlgorithmRequestRequestTypeDef](./type_defs.md#describealgorithmrequestrequesttypedef) 

### describe\_batch\_inference\_job

Gets the properties of a batch inference job including name, Amazon Resource
Name (ARN), status, input and output configurations, and the ARN of the solution
version used to generate the recommendations.

Type annotations and code completion for `#!python session.create_client("personalize").describe_batch_inference_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_inference_job)

```python
# describe_batch_inference_job method definition

await def describe_batch_inference_job(
    self,
    *,
    batchInferenceJobArn: str,
) -> DescribeBatchInferenceJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBatchInferenceJobResponseTypeDef](./type_defs.md#describebatchinferencejobresponsetypedef) 


```python
# describe_batch_inference_job method usage example with argument unpacking

kwargs: DescribeBatchInferenceJobRequestRequestTypeDef = {  # (1)
    "batchInferenceJobArn": ...,
}

parent.describe_batch_inference_job(**kwargs)
```

1. See [:material-code-braces: DescribeBatchInferenceJobRequestRequestTypeDef](./type_defs.md#describebatchinferencejobrequestrequesttypedef) 

### describe\_batch\_segment\_job

Gets the properties of a batch segment job including name, Amazon Resource Name
(ARN), status, input and output configurations, and the ARN of the solution
version used to generate segments.

Type annotations and code completion for `#!python session.create_client("personalize").describe_batch_segment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_segment_job)

```python
# describe_batch_segment_job method definition

await def describe_batch_segment_job(
    self,
    *,
    batchSegmentJobArn: str,
) -> DescribeBatchSegmentJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBatchSegmentJobResponseTypeDef](./type_defs.md#describebatchsegmentjobresponsetypedef) 


```python
# describe_batch_segment_job method usage example with argument unpacking

kwargs: DescribeBatchSegmentJobRequestRequestTypeDef = {  # (1)
    "batchSegmentJobArn": ...,
}

parent.describe_batch_segment_job(**kwargs)
```

1. See [:material-code-braces: DescribeBatchSegmentJobRequestRequestTypeDef](./type_defs.md#describebatchsegmentjobrequestrequesttypedef) 

### describe\_campaign

Describes the given campaign, including its status.

Type annotations and code completion for `#!python session.create_client("personalize").describe_campaign` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_campaign)

```python
# describe_campaign method definition

await def describe_campaign(
    self,
    *,
    campaignArn: str,
) -> DescribeCampaignResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCampaignResponseTypeDef](./type_defs.md#describecampaignresponsetypedef) 


```python
# describe_campaign method usage example with argument unpacking

kwargs: DescribeCampaignRequestRequestTypeDef = {  # (1)
    "campaignArn": ...,
}

parent.describe_campaign(**kwargs)
```

1. See [:material-code-braces: DescribeCampaignRequestRequestTypeDef](./type_defs.md#describecampaignrequestrequesttypedef) 

### describe\_dataset

Describes the given dataset.

Type annotations and code completion for `#!python session.create_client("personalize").describe_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset)

```python
# describe_dataset method definition

await def describe_dataset(
    self,
    *,
    datasetArn: str,
) -> DescribeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef) 


```python
# describe_dataset method usage example with argument unpacking

kwargs: DescribeDatasetRequestRequestTypeDef = {  # (1)
    "datasetArn": ...,
}

parent.describe_dataset(**kwargs)
```

1. See [:material-code-braces: DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef) 

### describe\_dataset\_export\_job

Describes the dataset export job created by
[CreateDatasetExportJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDatasetExportJob.html)_,
including the export job status.

Type annotations and code completion for `#!python session.create_client("personalize").describe_dataset_export_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_export_job)

```python
# describe_dataset_export_job method definition

await def describe_dataset_export_job(
    self,
    *,
    datasetExportJobArn: str,
) -> DescribeDatasetExportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatasetExportJobResponseTypeDef](./type_defs.md#describedatasetexportjobresponsetypedef) 


```python
# describe_dataset_export_job method usage example with argument unpacking

kwargs: DescribeDatasetExportJobRequestRequestTypeDef = {  # (1)
    "datasetExportJobArn": ...,
}

parent.describe_dataset_export_job(**kwargs)
```

1. See [:material-code-braces: DescribeDatasetExportJobRequestRequestTypeDef](./type_defs.md#describedatasetexportjobrequestrequesttypedef) 

### describe\_dataset\_group

Describes the given dataset group.

Type annotations and code completion for `#!python session.create_client("personalize").describe_dataset_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_group)

```python
# describe_dataset_group method definition

await def describe_dataset_group(
    self,
    *,
    datasetGroupArn: str,
) -> DescribeDatasetGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatasetGroupResponseTypeDef](./type_defs.md#describedatasetgroupresponsetypedef) 


```python
# describe_dataset_group method usage example with argument unpacking

kwargs: DescribeDatasetGroupRequestRequestTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.describe_dataset_group(**kwargs)
```

1. See [:material-code-braces: DescribeDatasetGroupRequestRequestTypeDef](./type_defs.md#describedatasetgrouprequestrequesttypedef) 

### describe\_dataset\_import\_job

Describes the dataset import job created by
[CreateDatasetImportJob](https://docs.aws.amazon.com/personalize/latest/dg/API_CreateDatasetImportJob.html)_,
including the import job status.

Type annotations and code completion for `#!python session.create_client("personalize").describe_dataset_import_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_import_job)

```python
# describe_dataset_import_job method definition

await def describe_dataset_import_job(
    self,
    *,
    datasetImportJobArn: str,
) -> DescribeDatasetImportJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatasetImportJobResponseTypeDef](./type_defs.md#describedatasetimportjobresponsetypedef) 


```python
# describe_dataset_import_job method usage example with argument unpacking

kwargs: DescribeDatasetImportJobRequestRequestTypeDef = {  # (1)
    "datasetImportJobArn": ...,
}

parent.describe_dataset_import_job(**kwargs)
```

1. See [:material-code-braces: DescribeDatasetImportJobRequestRequestTypeDef](./type_defs.md#describedatasetimportjobrequestrequesttypedef) 

### describe\_event\_tracker

Describes an event tracker.

Type annotations and code completion for `#!python session.create_client("personalize").describe_event_tracker` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_event_tracker)

```python
# describe_event_tracker method definition

await def describe_event_tracker(
    self,
    *,
    eventTrackerArn: str,
) -> DescribeEventTrackerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEventTrackerResponseTypeDef](./type_defs.md#describeeventtrackerresponsetypedef) 


```python
# describe_event_tracker method usage example with argument unpacking

kwargs: DescribeEventTrackerRequestRequestTypeDef = {  # (1)
    "eventTrackerArn": ...,
}

parent.describe_event_tracker(**kwargs)
```

1. See [:material-code-braces: DescribeEventTrackerRequestRequestTypeDef](./type_defs.md#describeeventtrackerrequestrequesttypedef) 

### describe\_feature\_transformation

Describes the given feature transformation.

Type annotations and code completion for `#!python session.create_client("personalize").describe_feature_transformation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_feature_transformation)

```python
# describe_feature_transformation method definition

await def describe_feature_transformation(
    self,
    *,
    featureTransformationArn: str,
) -> DescribeFeatureTransformationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFeatureTransformationResponseTypeDef](./type_defs.md#describefeaturetransformationresponsetypedef) 


```python
# describe_feature_transformation method usage example with argument unpacking

kwargs: DescribeFeatureTransformationRequestRequestTypeDef = {  # (1)
    "featureTransformationArn": ...,
}

parent.describe_feature_transformation(**kwargs)
```

1. See [:material-code-braces: DescribeFeatureTransformationRequestRequestTypeDef](./type_defs.md#describefeaturetransformationrequestrequesttypedef) 

### describe\_filter

Describes a filter's properties.

Type annotations and code completion for `#!python session.create_client("personalize").describe_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_filter)

```python
# describe_filter method definition

await def describe_filter(
    self,
    *,
    filterArn: str,
) -> DescribeFilterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFilterResponseTypeDef](./type_defs.md#describefilterresponsetypedef) 


```python
# describe_filter method usage example with argument unpacking

kwargs: DescribeFilterRequestRequestTypeDef = {  # (1)
    "filterArn": ...,
}

parent.describe_filter(**kwargs)
```

1. See [:material-code-braces: DescribeFilterRequestRequestTypeDef](./type_defs.md#describefilterrequestrequesttypedef) 

### describe\_metric\_attribution

Describes a metric attribution.

Type annotations and code completion for `#!python session.create_client("personalize").describe_metric_attribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_metric_attribution)

```python
# describe_metric_attribution method definition

await def describe_metric_attribution(
    self,
    *,
    metricAttributionArn: str,
) -> DescribeMetricAttributionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMetricAttributionResponseTypeDef](./type_defs.md#describemetricattributionresponsetypedef) 


```python
# describe_metric_attribution method usage example with argument unpacking

kwargs: DescribeMetricAttributionRequestRequestTypeDef = {  # (1)
    "metricAttributionArn": ...,
}

parent.describe_metric_attribution(**kwargs)
```

1. See [:material-code-braces: DescribeMetricAttributionRequestRequestTypeDef](./type_defs.md#describemetricattributionrequestrequesttypedef) 

### describe\_recipe

Describes a recipe.

Type annotations and code completion for `#!python session.create_client("personalize").describe_recipe` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recipe)

```python
# describe_recipe method definition

await def describe_recipe(
    self,
    *,
    recipeArn: str,
) -> DescribeRecipeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRecipeResponseTypeDef](./type_defs.md#describereciperesponsetypedef) 


```python
# describe_recipe method usage example with argument unpacking

kwargs: DescribeRecipeRequestRequestTypeDef = {  # (1)
    "recipeArn": ...,
}

parent.describe_recipe(**kwargs)
```

1. See [:material-code-braces: DescribeRecipeRequestRequestTypeDef](./type_defs.md#describereciperequestrequesttypedef) 

### describe\_recommender

Describes the given recommender, including its status.

Type annotations and code completion for `#!python session.create_client("personalize").describe_recommender` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recommender)

```python
# describe_recommender method definition

await def describe_recommender(
    self,
    *,
    recommenderArn: str,
) -> DescribeRecommenderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRecommenderResponseTypeDef](./type_defs.md#describerecommenderresponsetypedef) 


```python
# describe_recommender method usage example with argument unpacking

kwargs: DescribeRecommenderRequestRequestTypeDef = {  # (1)
    "recommenderArn": ...,
}

parent.describe_recommender(**kwargs)
```

1. See [:material-code-braces: DescribeRecommenderRequestRequestTypeDef](./type_defs.md#describerecommenderrequestrequesttypedef) 

### describe\_schema

Describes a schema.

Type annotations and code completion for `#!python session.create_client("personalize").describe_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_schema)

```python
# describe_schema method definition

await def describe_schema(
    self,
    *,
    schemaArn: str,
) -> DescribeSchemaResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSchemaResponseTypeDef](./type_defs.md#describeschemaresponsetypedef) 


```python
# describe_schema method usage example with argument unpacking

kwargs: DescribeSchemaRequestRequestTypeDef = {  # (1)
    "schemaArn": ...,
}

parent.describe_schema(**kwargs)
```

1. See [:material-code-braces: DescribeSchemaRequestRequestTypeDef](./type_defs.md#describeschemarequestrequesttypedef) 

### describe\_solution

Describes a solution.

Type annotations and code completion for `#!python session.create_client("personalize").describe_solution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution)

```python
# describe_solution method definition

await def describe_solution(
    self,
    *,
    solutionArn: str,
) -> DescribeSolutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSolutionResponseTypeDef](./type_defs.md#describesolutionresponsetypedef) 


```python
# describe_solution method usage example with argument unpacking

kwargs: DescribeSolutionRequestRequestTypeDef = {  # (1)
    "solutionArn": ...,
}

parent.describe_solution(**kwargs)
```

1. See [:material-code-braces: DescribeSolutionRequestRequestTypeDef](./type_defs.md#describesolutionrequestrequesttypedef) 

### describe\_solution\_version

Describes a specific version of a solution.

Type annotations and code completion for `#!python session.create_client("personalize").describe_solution_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution_version)

```python
# describe_solution_version method definition

await def describe_solution_version(
    self,
    *,
    solutionVersionArn: str,
) -> DescribeSolutionVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSolutionVersionResponseTypeDef](./type_defs.md#describesolutionversionresponsetypedef) 


```python
# describe_solution_version method usage example with argument unpacking

kwargs: DescribeSolutionVersionRequestRequestTypeDef = {  # (1)
    "solutionVersionArn": ...,
}

parent.describe_solution_version(**kwargs)
```

1. See [:material-code-braces: DescribeSolutionVersionRequestRequestTypeDef](./type_defs.md#describesolutionversionrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("personalize").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.generate_presigned_url)

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


### get\_solution\_metrics

Gets the metrics for the specified solution version.

Type annotations and code completion for `#!python session.create_client("personalize").get_solution_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.get_solution_metrics)

```python
# get_solution_metrics method definition

await def get_solution_metrics(
    self,
    *,
    solutionVersionArn: str,
) -> GetSolutionMetricsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSolutionMetricsResponseTypeDef](./type_defs.md#getsolutionmetricsresponsetypedef) 


```python
# get_solution_metrics method usage example with argument unpacking

kwargs: GetSolutionMetricsRequestRequestTypeDef = {  # (1)
    "solutionVersionArn": ...,
}

parent.get_solution_metrics(**kwargs)
```

1. See [:material-code-braces: GetSolutionMetricsRequestRequestTypeDef](./type_defs.md#getsolutionmetricsrequestrequesttypedef) 

### list\_batch\_inference\_jobs

Gets a list of the batch inference jobs that have been performed off of a
solution version.

Type annotations and code completion for `#!python session.create_client("personalize").list_batch_inference_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_inference_jobs)

```python
# list_batch_inference_jobs method definition

await def list_batch_inference_jobs(
    self,
    *,
    solutionVersionArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListBatchInferenceJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBatchInferenceJobsResponseTypeDef](./type_defs.md#listbatchinferencejobsresponsetypedef) 


```python
# list_batch_inference_jobs method usage example with argument unpacking

kwargs: ListBatchInferenceJobsRequestRequestTypeDef = {  # (1)
    "solutionVersionArn": ...,
}

parent.list_batch_inference_jobs(**kwargs)
```

1. See [:material-code-braces: ListBatchInferenceJobsRequestRequestTypeDef](./type_defs.md#listbatchinferencejobsrequestrequesttypedef) 

### list\_batch\_segment\_jobs

Gets a list of the batch segment jobs that have been performed off of a solution
version that you specify.

Type annotations and code completion for `#!python session.create_client("personalize").list_batch_segment_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_segment_jobs)

```python
# list_batch_segment_jobs method definition

await def list_batch_segment_jobs(
    self,
    *,
    solutionVersionArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListBatchSegmentJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListBatchSegmentJobsResponseTypeDef](./type_defs.md#listbatchsegmentjobsresponsetypedef) 


```python
# list_batch_segment_jobs method usage example with argument unpacking

kwargs: ListBatchSegmentJobsRequestRequestTypeDef = {  # (1)
    "solutionVersionArn": ...,
}

parent.list_batch_segment_jobs(**kwargs)
```

1. See [:material-code-braces: ListBatchSegmentJobsRequestRequestTypeDef](./type_defs.md#listbatchsegmentjobsrequestrequesttypedef) 

### list\_campaigns

Returns a list of campaigns that use the given solution.

Type annotations and code completion for `#!python session.create_client("personalize").list_campaigns` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_campaigns)

```python
# list_campaigns method definition

await def list_campaigns(
    self,
    *,
    solutionArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListCampaignsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef) 


```python
# list_campaigns method usage example with argument unpacking

kwargs: ListCampaignsRequestRequestTypeDef = {  # (1)
    "solutionArn": ...,
}

parent.list_campaigns(**kwargs)
```

1. See [:material-code-braces: ListCampaignsRequestRequestTypeDef](./type_defs.md#listcampaignsrequestrequesttypedef) 

### list\_dataset\_export\_jobs

Returns a list of dataset export jobs that use the given dataset.

Type annotations and code completion for `#!python session.create_client("personalize").list_dataset_export_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_export_jobs)

```python
# list_dataset_export_jobs method definition

await def list_dataset_export_jobs(
    self,
    *,
    datasetArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDatasetExportJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatasetExportJobsResponseTypeDef](./type_defs.md#listdatasetexportjobsresponsetypedef) 


```python
# list_dataset_export_jobs method usage example with argument unpacking

kwargs: ListDatasetExportJobsRequestRequestTypeDef = {  # (1)
    "datasetArn": ...,
}

parent.list_dataset_export_jobs(**kwargs)
```

1. See [:material-code-braces: ListDatasetExportJobsRequestRequestTypeDef](./type_defs.md#listdatasetexportjobsrequestrequesttypedef) 

### list\_dataset\_groups

Returns a list of dataset groups.

Type annotations and code completion for `#!python session.create_client("personalize").list_dataset_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_groups)

```python
# list_dataset_groups method definition

await def list_dataset_groups(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDatasetGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef) 


```python
# list_dataset_groups method usage example with argument unpacking

kwargs: ListDatasetGroupsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_dataset_groups(**kwargs)
```

1. See [:material-code-braces: ListDatasetGroupsRequestRequestTypeDef](./type_defs.md#listdatasetgroupsrequestrequesttypedef) 

### list\_dataset\_import\_jobs

Returns a list of dataset import jobs that use the given dataset.

Type annotations and code completion for `#!python session.create_client("personalize").list_dataset_import_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_import_jobs)

```python
# list_dataset_import_jobs method definition

await def list_dataset_import_jobs(
    self,
    *,
    datasetArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDatasetImportJobsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef) 


```python
# list_dataset_import_jobs method usage example with argument unpacking

kwargs: ListDatasetImportJobsRequestRequestTypeDef = {  # (1)
    "datasetArn": ...,
}

parent.list_dataset_import_jobs(**kwargs)
```

1. See [:material-code-braces: ListDatasetImportJobsRequestRequestTypeDef](./type_defs.md#listdatasetimportjobsrequestrequesttypedef) 

### list\_datasets

Returns the list of datasets contained in the given dataset group.

Type annotations and code completion for `#!python session.create_client("personalize").list_datasets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_datasets)

```python
# list_datasets method definition

await def list_datasets(
    self,
    *,
    datasetGroupArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDatasetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# list_datasets method usage example with argument unpacking

kwargs: ListDatasetsRequestRequestTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.list_datasets(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef) 

### list\_event\_trackers

Returns the list of event trackers associated with the account.

Type annotations and code completion for `#!python session.create_client("personalize").list_event_trackers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_event_trackers)

```python
# list_event_trackers method definition

await def list_event_trackers(
    self,
    *,
    datasetGroupArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListEventTrackersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventTrackersResponseTypeDef](./type_defs.md#listeventtrackersresponsetypedef) 


```python
# list_event_trackers method usage example with argument unpacking

kwargs: ListEventTrackersRequestRequestTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.list_event_trackers(**kwargs)
```

1. See [:material-code-braces: ListEventTrackersRequestRequestTypeDef](./type_defs.md#listeventtrackersrequestrequesttypedef) 

### list\_filters

Lists all filters that belong to a given dataset group.

Type annotations and code completion for `#!python session.create_client("personalize").list_filters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_filters)

```python
# list_filters method definition

await def list_filters(
    self,
    *,
    datasetGroupArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListFiltersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef) 


```python
# list_filters method usage example with argument unpacking

kwargs: ListFiltersRequestRequestTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.list_filters(**kwargs)
```

1. See [:material-code-braces: ListFiltersRequestRequestTypeDef](./type_defs.md#listfiltersrequestrequesttypedef) 

### list\_metric\_attribution\_metrics

Lists the metrics for the metric attribution.

Type annotations and code completion for `#!python session.create_client("personalize").list_metric_attribution_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_metric_attribution_metrics)

```python
# list_metric_attribution_metrics method definition

await def list_metric_attribution_metrics(
    self,
    *,
    metricAttributionArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListMetricAttributionMetricsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMetricAttributionMetricsResponseTypeDef](./type_defs.md#listmetricattributionmetricsresponsetypedef) 


```python
# list_metric_attribution_metrics method usage example with argument unpacking

kwargs: ListMetricAttributionMetricsRequestRequestTypeDef = {  # (1)
    "metricAttributionArn": ...,
}

parent.list_metric_attribution_metrics(**kwargs)
```

1. See [:material-code-braces: ListMetricAttributionMetricsRequestRequestTypeDef](./type_defs.md#listmetricattributionmetricsrequestrequesttypedef) 

### list\_metric\_attributions

Lists metric attributions.

Type annotations and code completion for `#!python session.create_client("personalize").list_metric_attributions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_metric_attributions)

```python
# list_metric_attributions method definition

await def list_metric_attributions(
    self,
    *,
    datasetGroupArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListMetricAttributionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMetricAttributionsResponseTypeDef](./type_defs.md#listmetricattributionsresponsetypedef) 


```python
# list_metric_attributions method usage example with argument unpacking

kwargs: ListMetricAttributionsRequestRequestTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.list_metric_attributions(**kwargs)
```

1. See [:material-code-braces: ListMetricAttributionsRequestRequestTypeDef](./type_defs.md#listmetricattributionsrequestrequesttypedef) 

### list\_recipes

Returns a list of available recipes.

Type annotations and code completion for `#!python session.create_client("personalize").list_recipes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recipes)

```python
# list_recipes method definition

await def list_recipes(
    self,
    *,
    recipeProvider: RecipeProviderType = ...,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
    domain: DomainType = ...,  # (2)
) -> ListRecipesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RecipeProviderType](./literals.md#recipeprovidertype) 
2. See [:material-code-brackets: DomainType](./literals.md#domaintype) 
3. See [:material-code-braces: ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef) 


```python
# list_recipes method usage example with argument unpacking

kwargs: ListRecipesRequestRequestTypeDef = {  # (1)
    "recipeProvider": ...,
}

parent.list_recipes(**kwargs)
```

1. See [:material-code-braces: ListRecipesRequestRequestTypeDef](./type_defs.md#listrecipesrequestrequesttypedef) 

### list\_recommenders

Returns a list of recommenders in a given Domain dataset group.

Type annotations and code completion for `#!python session.create_client("personalize").list_recommenders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recommenders)

```python
# list_recommenders method definition

await def list_recommenders(
    self,
    *,
    datasetGroupArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListRecommendersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRecommendersResponseTypeDef](./type_defs.md#listrecommendersresponsetypedef) 


```python
# list_recommenders method usage example with argument unpacking

kwargs: ListRecommendersRequestRequestTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.list_recommenders(**kwargs)
```

1. See [:material-code-braces: ListRecommendersRequestRequestTypeDef](./type_defs.md#listrecommendersrequestrequesttypedef) 

### list\_schemas

Returns the list of schemas associated with the account.

Type annotations and code completion for `#!python session.create_client("personalize").list_schemas` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_schemas)

```python
# list_schemas method definition

await def list_schemas(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListSchemasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef) 


```python
# list_schemas method usage example with argument unpacking

kwargs: ListSchemasRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_schemas(**kwargs)
```

1. See [:material-code-braces: ListSchemasRequestRequestTypeDef](./type_defs.md#listschemasrequestrequesttypedef) 

### list\_solution\_versions

Returns a list of solution versions for the given solution.

Type annotations and code completion for `#!python session.create_client("personalize").list_solution_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solution_versions)

```python
# list_solution_versions method definition

await def list_solution_versions(
    self,
    *,
    solutionArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListSolutionVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSolutionVersionsResponseTypeDef](./type_defs.md#listsolutionversionsresponsetypedef) 


```python
# list_solution_versions method usage example with argument unpacking

kwargs: ListSolutionVersionsRequestRequestTypeDef = {  # (1)
    "solutionArn": ...,
}

parent.list_solution_versions(**kwargs)
```

1. See [:material-code-braces: ListSolutionVersionsRequestRequestTypeDef](./type_defs.md#listsolutionversionsrequestrequesttypedef) 

### list\_solutions

Returns a list of solutions that use the given dataset group.

Type annotations and code completion for `#!python session.create_client("personalize").list_solutions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solutions)

```python
# list_solutions method definition

await def list_solutions(
    self,
    *,
    datasetGroupArn: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListSolutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef) 


```python
# list_solutions method usage example with argument unpacking

kwargs: ListSolutionsRequestRequestTypeDef = {  # (1)
    "datasetGroupArn": ...,
}

parent.list_solutions(**kwargs)
```

1. See [:material-code-braces: ListSolutionsRequestRequestTypeDef](./type_defs.md#listsolutionsrequestrequesttypedef) 

### list\_tags\_for\_resource

Get a list of [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-
resources.html)_ attached to a resource.

Type annotations and code completion for `#!python session.create_client("personalize").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_tags_for_resource)

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

### start\_recommender

Starts a recommender that is INACTIVE.

Type annotations and code completion for `#!python session.create_client("personalize").start_recommender` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.start_recommender)

```python
# start_recommender method definition

await def start_recommender(
    self,
    *,
    recommenderArn: str,
) -> StartRecommenderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartRecommenderResponseTypeDef](./type_defs.md#startrecommenderresponsetypedef) 


```python
# start_recommender method usage example with argument unpacking

kwargs: StartRecommenderRequestRequestTypeDef = {  # (1)
    "recommenderArn": ...,
}

parent.start_recommender(**kwargs)
```

1. See [:material-code-braces: StartRecommenderRequestRequestTypeDef](./type_defs.md#startrecommenderrequestrequesttypedef) 

### stop\_recommender

Stops a recommender that is ACTIVE.

Type annotations and code completion for `#!python session.create_client("personalize").stop_recommender` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.stop_recommender)

```python
# stop_recommender method definition

await def stop_recommender(
    self,
    *,
    recommenderArn: str,
) -> StopRecommenderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopRecommenderResponseTypeDef](./type_defs.md#stoprecommenderresponsetypedef) 


```python
# stop_recommender method usage example with argument unpacking

kwargs: StopRecommenderRequestRequestTypeDef = {  # (1)
    "recommenderArn": ...,
}

parent.stop_recommender(**kwargs)
```

1. See [:material-code-braces: StopRecommenderRequestRequestTypeDef](./type_defs.md#stoprecommenderrequestrequesttypedef) 

### stop\_solution\_version\_creation

Stops creating a solution version that is in a state of CREATE_PENDING or CREATE
IN_PROGRESS.

Type annotations and code completion for `#!python session.create_client("personalize").stop_solution_version_creation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.stop_solution_version_creation)

```python
# stop_solution_version_creation method definition

await def stop_solution_version_creation(
    self,
    *,
    solutionVersionArn: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_solution_version_creation method usage example with argument unpacking

kwargs: StopSolutionVersionCreationRequestRequestTypeDef = {  # (1)
    "solutionVersionArn": ...,
}

parent.stop_solution_version_creation(**kwargs)
```

1. See [:material-code-braces: StopSolutionVersionCreationRequestRequestTypeDef](./type_defs.md#stopsolutionversioncreationrequestrequesttypedef) 

### tag\_resource

Add a list of tags to a resource.

Type annotations and code completion for `#!python session.create_client("personalize").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


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

Remove [tags](https://docs.aws.amazon.com/personalize/latest/dg/tagging-
resources.html)_ that are attached to a resource.

Type annotations and code completion for `#!python session.create_client("personalize").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.untag_resource)

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

### update\_campaign

Updates a campaign by either deploying a new solution or changing the value of
the campaign's `minProvisionedTPS` parameter.

Type annotations and code completion for `#!python session.create_client("personalize").update_campaign` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)

```python
# update_campaign method definition

await def update_campaign(
    self,
    *,
    campaignArn: str,
    solutionVersionArn: str = ...,
    minProvisionedTPS: int = ...,
    campaignConfig: CampaignConfigTypeDef = ...,  # (1)
) -> UpdateCampaignResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CampaignConfigTypeDef](./type_defs.md#campaignconfigtypedef) 
2. See [:material-code-braces: UpdateCampaignResponseTypeDef](./type_defs.md#updatecampaignresponsetypedef) 


```python
# update_campaign method usage example with argument unpacking

kwargs: UpdateCampaignRequestRequestTypeDef = {  # (1)
    "campaignArn": ...,
}

parent.update_campaign(**kwargs)
```

1. See [:material-code-braces: UpdateCampaignRequestRequestTypeDef](./type_defs.md#updatecampaignrequestrequesttypedef) 

### update\_dataset

Update a dataset to replace its schema with a new or existing one.

Type annotations and code completion for `#!python session.create_client("personalize").update_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_dataset)

```python
# update_dataset method definition

await def update_dataset(
    self,
    *,
    datasetArn: str,
    schemaArn: str,
) -> UpdateDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDatasetResponseTypeDef](./type_defs.md#updatedatasetresponsetypedef) 


```python
# update_dataset method usage example with argument unpacking

kwargs: UpdateDatasetRequestRequestTypeDef = {  # (1)
    "datasetArn": ...,
    "schemaArn": ...,
}

parent.update_dataset(**kwargs)
```

1. See [:material-code-braces: UpdateDatasetRequestRequestTypeDef](./type_defs.md#updatedatasetrequestrequesttypedef) 

### update\_metric\_attribution

Updates a metric attribution.

Type annotations and code completion for `#!python session.create_client("personalize").update_metric_attribution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)

```python
# update_metric_attribution method definition

await def update_metric_attribution(
    self,
    *,
    addMetrics: Sequence[MetricAttributeTypeDef] = ...,  # (1)
    removeMetrics: Sequence[str] = ...,
    metricsOutputConfig: MetricAttributionOutputTypeDef = ...,  # (2)
    metricAttributionArn: str = ...,
) -> UpdateMetricAttributionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MetricAttributeTypeDef](./type_defs.md#metricattributetypedef) 
2. See [:material-code-braces: MetricAttributionOutputTypeDef](./type_defs.md#metricattributionoutputtypedef) 
3. See [:material-code-braces: UpdateMetricAttributionResponseTypeDef](./type_defs.md#updatemetricattributionresponsetypedef) 


```python
# update_metric_attribution method usage example with argument unpacking

kwargs: UpdateMetricAttributionRequestRequestTypeDef = {  # (1)
    "addMetrics": ...,
}

parent.update_metric_attribution(**kwargs)
```

1. See [:material-code-braces: UpdateMetricAttributionRequestRequestTypeDef](./type_defs.md#updatemetricattributionrequestrequesttypedef) 

### update\_recommender

Updates the recommender to modify the recommender configuration.

Type annotations and code completion for `#!python session.create_client("personalize").update_recommender` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_recommender)

```python
# update_recommender method definition

await def update_recommender(
    self,
    *,
    recommenderArn: str,
    recommenderConfig: RecommenderConfigTypeDef,  # (1)
) -> UpdateRecommenderResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RecommenderConfigTypeDef](./type_defs.md#recommenderconfigtypedef) 
2. See [:material-code-braces: UpdateRecommenderResponseTypeDef](./type_defs.md#updaterecommenderresponsetypedef) 


```python
# update_recommender method usage example with argument unpacking

kwargs: UpdateRecommenderRequestRequestTypeDef = {  # (1)
    "recommenderArn": ...,
    "recommenderConfig": ...,
}

parent.update_recommender(**kwargs)
```

1. See [:material-code-braces: UpdateRecommenderRequestRequestTypeDef](./type_defs.md#updaterecommenderrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("personalize").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> PersonalizeClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("personalize").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("personalize").get_paginator` method with overloads.

- `client.get_paginator("list_batch_inference_jobs")` -> [ListBatchInferenceJobsPaginator](./paginators.md#listbatchinferencejobspaginator)
- `client.get_paginator("list_batch_segment_jobs")` -> [ListBatchSegmentJobsPaginator](./paginators.md#listbatchsegmentjobspaginator)
- `client.get_paginator("list_campaigns")` -> [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
- `client.get_paginator("list_dataset_export_jobs")` -> [ListDatasetExportJobsPaginator](./paginators.md#listdatasetexportjobspaginator)
- `client.get_paginator("list_dataset_groups")` -> [ListDatasetGroupsPaginator](./paginators.md#listdatasetgroupspaginator)
- `client.get_paginator("list_dataset_import_jobs")` -> [ListDatasetImportJobsPaginator](./paginators.md#listdatasetimportjobspaginator)
- `client.get_paginator("list_datasets")` -> [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- `client.get_paginator("list_event_trackers")` -> [ListEventTrackersPaginator](./paginators.md#listeventtrackerspaginator)
- `client.get_paginator("list_filters")` -> [ListFiltersPaginator](./paginators.md#listfilterspaginator)
- `client.get_paginator("list_metric_attribution_metrics")` -> [ListMetricAttributionMetricsPaginator](./paginators.md#listmetricattributionmetricspaginator)
- `client.get_paginator("list_metric_attributions")` -> [ListMetricAttributionsPaginator](./paginators.md#listmetricattributionspaginator)
- `client.get_paginator("list_recipes")` -> [ListRecipesPaginator](./paginators.md#listrecipespaginator)
- `client.get_paginator("list_recommenders")` -> [ListRecommendersPaginator](./paginators.md#listrecommenderspaginator)
- `client.get_paginator("list_schemas")` -> [ListSchemasPaginator](./paginators.md#listschemaspaginator)
- `client.get_paginator("list_solution_versions")` -> [ListSolutionVersionsPaginator](./paginators.md#listsolutionversionspaginator)
- `client.get_paginator("list_solutions")` -> [ListSolutionsPaginator](./paginators.md#listsolutionspaginator)



