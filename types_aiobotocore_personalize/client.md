<a id="personalizeclient-for-aiobotocore-personalize-module"></a>

# PersonalizeClient for aiobotocore Personalize module

> [Index](..) > [Personalize](.) > PersonalizeClient

Auto-generated documentation for
[Personalize](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
type annotations stubs module
[types-aiobotocore-personalize](https://pypi.org/project/types-aiobotocore-personalize/).

- [PersonalizeClient for aiobotocore Personalize module](#personalizeclient-for-aiobotocore-personalize-module)
  - [PersonalizeClient](#personalizeclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_batch_inference_job](#create_batch_inference_job)
    - [create_batch_segment_job](#create_batch_segment_job)
    - [create_campaign](#create_campaign)
    - [create_dataset](#create_dataset)
    - [create_dataset_export_job](#create_dataset_export_job)
    - [create_dataset_group](#create_dataset_group)
    - [create_dataset_import_job](#create_dataset_import_job)
    - [create_event_tracker](#create_event_tracker)
    - [create_filter](#create_filter)
    - [create_recommender](#create_recommender)
    - [create_schema](#create_schema)
    - [create_solution](#create_solution)
    - [create_solution_version](#create_solution_version)
    - [delete_campaign](#delete_campaign)
    - [delete_dataset](#delete_dataset)
    - [delete_dataset_group](#delete_dataset_group)
    - [delete_event_tracker](#delete_event_tracker)
    - [delete_filter](#delete_filter)
    - [delete_recommender](#delete_recommender)
    - [delete_schema](#delete_schema)
    - [delete_solution](#delete_solution)
    - [describe_algorithm](#describe_algorithm)
    - [describe_batch_inference_job](#describe_batch_inference_job)
    - [describe_batch_segment_job](#describe_batch_segment_job)
    - [describe_campaign](#describe_campaign)
    - [describe_dataset](#describe_dataset)
    - [describe_dataset_export_job](#describe_dataset_export_job)
    - [describe_dataset_group](#describe_dataset_group)
    - [describe_dataset_import_job](#describe_dataset_import_job)
    - [describe_event_tracker](#describe_event_tracker)
    - [describe_feature_transformation](#describe_feature_transformation)
    - [describe_filter](#describe_filter)
    - [describe_recipe](#describe_recipe)
    - [describe_recommender](#describe_recommender)
    - [describe_schema](#describe_schema)
    - [describe_solution](#describe_solution)
    - [describe_solution_version](#describe_solution_version)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_solution_metrics](#get_solution_metrics)
    - [list_batch_inference_jobs](#list_batch_inference_jobs)
    - [list_batch_segment_jobs](#list_batch_segment_jobs)
    - [list_campaigns](#list_campaigns)
    - [list_dataset_export_jobs](#list_dataset_export_jobs)
    - [list_dataset_groups](#list_dataset_groups)
    - [list_dataset_import_jobs](#list_dataset_import_jobs)
    - [list_datasets](#list_datasets)
    - [list_event_trackers](#list_event_trackers)
    - [list_filters](#list_filters)
    - [list_recipes](#list_recipes)
    - [list_recommenders](#list_recommenders)
    - [list_schemas](#list_schemas)
    - [list_solution_versions](#list_solution_versions)
    - [list_solutions](#list_solutions)
    - [stop_solution_version_creation](#stop_solution_version_creation)
    - [update_campaign](#update_campaign)
    - [update_recommender](#update_recommender)
    - [get_paginator](#get_paginator)

<a id="personalizeclient"></a>

## PersonalizeClient

Type annotations for `aiobotocore.create_client("personalize")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_personalize.client import PersonalizeClient

def get_personalize_client() -> PersonalizeClient:
    return Session().client("personalize")
```

Boto3 documentation:
[Personalize.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_personalize.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InvalidInputException`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceAlreadyExistsException`
- `Exceptions.ResourceInUseException`
- `Exceptions.ResourceNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

PersonalizeClient exceptions.

Type annotations for `aiobotocore.create_client("personalize").exceptions`
method.

Boto3 documentation:
[Personalize.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("personalize").can_paginate`
method.

Boto3 documentation:
[Personalize.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_batch_inference_job"></a>

### create_batch_inference_job

Creates a batch inference job.

Type annotations for
`aiobotocore.create_client("personalize").create_batch_inference_job` method.

Boto3 documentation:
[Personalize.Client.create_batch_inference_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_inference_job)

Asynchronous method. Use `await create_batch_inference_job(...)` for a
synchronous call.

Arguments mapping described in
[CreateBatchInferenceJobRequestRequestTypeDef](./type_defs.md#createbatchinferencejobrequestrequesttypedef).

Keyword-only arguments:

- `jobName`: `str` *(required)*
- `solutionVersionArn`: `str` *(required)*
- `jobInput`:
  [BatchInferenceJobInputTypeDef](./type_defs.md#batchinferencejobinputtypedef)
  *(required)*
- `jobOutput`:
  [BatchInferenceJobOutputTypeDef](./type_defs.md#batchinferencejoboutputtypedef)
  *(required)*
- `roleArn`: `str` *(required)*
- `filterArn`: `str`
- `numResults`: `int`
- `batchInferenceJobConfig`:
  [BatchInferenceJobConfigTypeDef](./type_defs.md#batchinferencejobconfigtypedef)

Returns a `Coroutine` for
[CreateBatchInferenceJobResponseTypeDef](./type_defs.md#createbatchinferencejobresponsetypedef).

<a id="create_batch_segment_job"></a>

### create_batch_segment_job

Creates a batch segment job.

Type annotations for
`aiobotocore.create_client("personalize").create_batch_segment_job` method.

Boto3 documentation:
[Personalize.Client.create_batch_segment_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_segment_job)

Asynchronous method. Use `await create_batch_segment_job(...)` for a
synchronous call.

Arguments mapping described in
[CreateBatchSegmentJobRequestRequestTypeDef](./type_defs.md#createbatchsegmentjobrequestrequesttypedef).

Keyword-only arguments:

- `jobName`: `str` *(required)*
- `solutionVersionArn`: `str` *(required)*
- `jobInput`:
  [BatchSegmentJobInputTypeDef](./type_defs.md#batchsegmentjobinputtypedef)
  *(required)*
- `jobOutput`:
  [BatchSegmentJobOutputTypeDef](./type_defs.md#batchsegmentjoboutputtypedef)
  *(required)*
- `roleArn`: `str` *(required)*
- `filterArn`: `str`
- `numResults`: `int`

Returns a `Coroutine` for
[CreateBatchSegmentJobResponseTypeDef](./type_defs.md#createbatchsegmentjobresponsetypedef).

<a id="create_campaign"></a>

### create_campaign

Creates a campaign that deploys a solution version.

Type annotations for `aiobotocore.create_client("personalize").create_campaign`
method.

Boto3 documentation:
[Personalize.Client.create_campaign](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)

Asynchronous method. Use `await create_campaign(...)` for a synchronous call.

Arguments mapping described in
[CreateCampaignRequestRequestTypeDef](./type_defs.md#createcampaignrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `solutionVersionArn`: `str` *(required)*
- `minProvisionedTPS`: `int`
- `campaignConfig`:
  [CampaignConfigTypeDef](./type_defs.md#campaignconfigtypedef)

Returns a `Coroutine` for
[CreateCampaignResponseTypeDef](./type_defs.md#createcampaignresponsetypedef).

<a id="create_dataset"></a>

### create_dataset

Creates an empty dataset and adds it to the specified dataset group.

Type annotations for `aiobotocore.create_client("personalize").create_dataset`
method.

Boto3 documentation:
[Personalize.Client.create_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset)

Asynchronous method. Use `await create_dataset(...)` for a synchronous call.

Arguments mapping described in
[CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `schemaArn`: `str` *(required)*
- `datasetGroupArn`: `str` *(required)*
- `datasetType`: `str` *(required)*

Returns a `Coroutine` for
[CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef).

<a id="create_dataset_export_job"></a>

### create_dataset_export_job

Creates a job that exports data from your dataset to an Amazon S3 bucket.

Type annotations for
`aiobotocore.create_client("personalize").create_dataset_export_job` method.

Boto3 documentation:
[Personalize.Client.create_dataset_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_export_job)

Asynchronous method. Use `await create_dataset_export_job(...)` for a
synchronous call.

Arguments mapping described in
[CreateDatasetExportJobRequestRequestTypeDef](./type_defs.md#createdatasetexportjobrequestrequesttypedef).

Keyword-only arguments:

- `jobName`: `str` *(required)*
- `datasetArn`: `str` *(required)*
- `roleArn`: `str` *(required)*
- `jobOutput`:
  [DatasetExportJobOutputTypeDef](./type_defs.md#datasetexportjoboutputtypedef)
  *(required)*
- `ingestionMode`: [IngestionModeType](./literals.md#ingestionmodetype)

Returns a `Coroutine` for
[CreateDatasetExportJobResponseTypeDef](./type_defs.md#createdatasetexportjobresponsetypedef).

<a id="create_dataset_group"></a>

### create_dataset_group

Creates an empty dataset group.

Type annotations for
`aiobotocore.create_client("personalize").create_dataset_group` method.

Boto3 documentation:
[Personalize.Client.create_dataset_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_group)

Asynchronous method. Use `await create_dataset_group(...)` for a synchronous
call.

Arguments mapping described in
[CreateDatasetGroupRequestRequestTypeDef](./type_defs.md#createdatasetgrouprequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `roleArn`: `str`
- `kmsKeyArn`: `str`
- `domain`: [DomainType](./literals.md#domaintype)

Returns a `Coroutine` for
[CreateDatasetGroupResponseTypeDef](./type_defs.md#createdatasetgroupresponsetypedef).

<a id="create_dataset_import_job"></a>

### create_dataset_import_job

Creates a job that imports training data from your data source (an Amazon S3
bucket) to an Amazon Personalize dataset.

Type annotations for
`aiobotocore.create_client("personalize").create_dataset_import_job` method.

Boto3 documentation:
[Personalize.Client.create_dataset_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_import_job)

Asynchronous method. Use `await create_dataset_import_job(...)` for a
synchronous call.

Arguments mapping described in
[CreateDatasetImportJobRequestRequestTypeDef](./type_defs.md#createdatasetimportjobrequestrequesttypedef).

Keyword-only arguments:

- `jobName`: `str` *(required)*
- `datasetArn`: `str` *(required)*
- `dataSource`: [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
  *(required)*
- `roleArn`: `str` *(required)*

Returns a `Coroutine` for
[CreateDatasetImportJobResponseTypeDef](./type_defs.md#createdatasetimportjobresponsetypedef).

<a id="create_event_tracker"></a>

### create_event_tracker

Creates an event tracker that you use when adding event data to a specified
dataset group using the
[PutEvents](https://docs.aws.amazon.com/personalize/latest/dg/API_UBS_PutEvents.html)\_
API.

Type annotations for
`aiobotocore.create_client("personalize").create_event_tracker` method.

Boto3 documentation:
[Personalize.Client.create_event_tracker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_event_tracker)

Asynchronous method. Use `await create_event_tracker(...)` for a synchronous
call.

Arguments mapping described in
[CreateEventTrackerRequestRequestTypeDef](./type_defs.md#createeventtrackerrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `datasetGroupArn`: `str` *(required)*

Returns a `Coroutine` for
[CreateEventTrackerResponseTypeDef](./type_defs.md#createeventtrackerresponsetypedef).

<a id="create_filter"></a>

### create_filter

Creates a recommendation filter.

Type annotations for `aiobotocore.create_client("personalize").create_filter`
method.

Boto3 documentation:
[Personalize.Client.create_filter](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_filter)

Asynchronous method. Use `await create_filter(...)` for a synchronous call.

Arguments mapping described in
[CreateFilterRequestRequestTypeDef](./type_defs.md#createfilterrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `datasetGroupArn`: `str` *(required)*
- `filterExpression`: `str` *(required)*

Returns a `Coroutine` for
[CreateFilterResponseTypeDef](./type_defs.md#createfilterresponsetypedef).

<a id="create_recommender"></a>

### create_recommender

Creates a recommender with the recipe (a Domain dataset group use case) you
specify.

Type annotations for
`aiobotocore.create_client("personalize").create_recommender` method.

Boto3 documentation:
[Personalize.Client.create_recommender](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)

Asynchronous method. Use `await create_recommender(...)` for a synchronous
call.

Arguments mapping described in
[CreateRecommenderRequestRequestTypeDef](./type_defs.md#createrecommenderrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `datasetGroupArn`: `str` *(required)*
- `recipeArn`: `str` *(required)*
- `recommenderConfig`:
  [RecommenderConfigTypeDef](./type_defs.md#recommenderconfigtypedef)

Returns a `Coroutine` for
[CreateRecommenderResponseTypeDef](./type_defs.md#createrecommenderresponsetypedef).

<a id="create_schema"></a>

### create_schema

Creates an Amazon Personalize schema from the specified schema string.

Type annotations for `aiobotocore.create_client("personalize").create_schema`
method.

Boto3 documentation:
[Personalize.Client.create_schema](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_schema)

Asynchronous method. Use `await create_schema(...)` for a synchronous call.

Arguments mapping described in
[CreateSchemaRequestRequestTypeDef](./type_defs.md#createschemarequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `schema`: `str` *(required)*
- `domain`: [DomainType](./literals.md#domaintype)

Returns a `Coroutine` for
[CreateSchemaResponseTypeDef](./type_defs.md#createschemaresponsetypedef).

<a id="create_solution"></a>

### create_solution

Creates the configuration for training a model.

Type annotations for `aiobotocore.create_client("personalize").create_solution`
method.

Boto3 documentation:
[Personalize.Client.create_solution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)

Asynchronous method. Use `await create_solution(...)` for a synchronous call.

Arguments mapping described in
[CreateSolutionRequestRequestTypeDef](./type_defs.md#createsolutionrequestrequesttypedef).

Keyword-only arguments:

- `name`: `str` *(required)*
- `datasetGroupArn`: `str` *(required)*
- `performHPO`: `bool`
- `performAutoML`: `bool`
- `recipeArn`: `str`
- `eventType`: `str`
- `solutionConfig`:
  [SolutionConfigTypeDef](./type_defs.md#solutionconfigtypedef)

Returns a `Coroutine` for
[CreateSolutionResponseTypeDef](./type_defs.md#createsolutionresponsetypedef).

<a id="create_solution_version"></a>

### create_solution_version

Trains or retrains an active solution in a Custom dataset group.

Type annotations for
`aiobotocore.create_client("personalize").create_solution_version` method.

Boto3 documentation:
[Personalize.Client.create_solution_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution_version)

Asynchronous method. Use `await create_solution_version(...)` for a synchronous
call.

Arguments mapping described in
[CreateSolutionVersionRequestRequestTypeDef](./type_defs.md#createsolutionversionrequestrequesttypedef).

Keyword-only arguments:

- `solutionArn`: `str` *(required)*
- `trainingMode`: [TrainingModeType](./literals.md#trainingmodetype)

Returns a `Coroutine` for
[CreateSolutionVersionResponseTypeDef](./type_defs.md#createsolutionversionresponsetypedef).

<a id="delete_campaign"></a>

### delete_campaign

Removes a campaign by deleting the solution deployment.

Type annotations for `aiobotocore.create_client("personalize").delete_campaign`
method.

Boto3 documentation:
[Personalize.Client.delete_campaign](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_campaign)

Asynchronous method. Use `await delete_campaign(...)` for a synchronous call.

Arguments mapping described in
[DeleteCampaignRequestRequestTypeDef](./type_defs.md#deletecampaignrequestrequesttypedef).

Keyword-only arguments:

- `campaignArn`: `str` *(required)*

<a id="delete_dataset"></a>

### delete_dataset

Deletes a dataset.

Type annotations for `aiobotocore.create_client("personalize").delete_dataset`
method.

Boto3 documentation:
[Personalize.Client.delete_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_dataset)

Asynchronous method. Use `await delete_dataset(...)` for a synchronous call.

Arguments mapping described in
[DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef).

Keyword-only arguments:

- `datasetArn`: `str` *(required)*

<a id="delete_dataset_group"></a>

### delete_dataset_group

Deletes a dataset group.

Type annotations for
`aiobotocore.create_client("personalize").delete_dataset_group` method.

Boto3 documentation:
[Personalize.Client.delete_dataset_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_dataset_group)

Asynchronous method. Use `await delete_dataset_group(...)` for a synchronous
call.

Arguments mapping described in
[DeleteDatasetGroupRequestRequestTypeDef](./type_defs.md#deletedatasetgrouprequestrequesttypedef).

Keyword-only arguments:

- `datasetGroupArn`: `str` *(required)*

<a id="delete_event_tracker"></a>

### delete_event_tracker

Deletes the event tracker.

Type annotations for
`aiobotocore.create_client("personalize").delete_event_tracker` method.

Boto3 documentation:
[Personalize.Client.delete_event_tracker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_event_tracker)

Asynchronous method. Use `await delete_event_tracker(...)` for a synchronous
call.

Arguments mapping described in
[DeleteEventTrackerRequestRequestTypeDef](./type_defs.md#deleteeventtrackerrequestrequesttypedef).

Keyword-only arguments:

- `eventTrackerArn`: `str` *(required)*

<a id="delete_filter"></a>

### delete_filter

Deletes a filter.

Type annotations for `aiobotocore.create_client("personalize").delete_filter`
method.

Boto3 documentation:
[Personalize.Client.delete_filter](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_filter)

Asynchronous method. Use `await delete_filter(...)` for a synchronous call.

Arguments mapping described in
[DeleteFilterRequestRequestTypeDef](./type_defs.md#deletefilterrequestrequesttypedef).

Keyword-only arguments:

- `filterArn`: `str` *(required)*

<a id="delete_recommender"></a>

### delete_recommender

Deactivates and removes a recommender.

Type annotations for
`aiobotocore.create_client("personalize").delete_recommender` method.

Boto3 documentation:
[Personalize.Client.delete_recommender](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_recommender)

Asynchronous method. Use `await delete_recommender(...)` for a synchronous
call.

Arguments mapping described in
[DeleteRecommenderRequestRequestTypeDef](./type_defs.md#deleterecommenderrequestrequesttypedef).

Keyword-only arguments:

- `recommenderArn`: `str` *(required)*

<a id="delete_schema"></a>

### delete_schema

Deletes a schema.

Type annotations for `aiobotocore.create_client("personalize").delete_schema`
method.

Boto3 documentation:
[Personalize.Client.delete_schema](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_schema)

Asynchronous method. Use `await delete_schema(...)` for a synchronous call.

Arguments mapping described in
[DeleteSchemaRequestRequestTypeDef](./type_defs.md#deleteschemarequestrequesttypedef).

Keyword-only arguments:

- `schemaArn`: `str` *(required)*

<a id="delete_solution"></a>

### delete_solution

Deletes all versions of a solution and the `Solution` object itself.

Type annotations for `aiobotocore.create_client("personalize").delete_solution`
method.

Boto3 documentation:
[Personalize.Client.delete_solution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.delete_solution)

Asynchronous method. Use `await delete_solution(...)` for a synchronous call.

Arguments mapping described in
[DeleteSolutionRequestRequestTypeDef](./type_defs.md#deletesolutionrequestrequesttypedef).

Keyword-only arguments:

- `solutionArn`: `str` *(required)*

<a id="describe_algorithm"></a>

### describe_algorithm

Describes the given algorithm.

Type annotations for
`aiobotocore.create_client("personalize").describe_algorithm` method.

Boto3 documentation:
[Personalize.Client.describe_algorithm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_algorithm)

Asynchronous method. Use `await describe_algorithm(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAlgorithmRequestRequestTypeDef](./type_defs.md#describealgorithmrequestrequesttypedef).

Keyword-only arguments:

- `algorithmArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAlgorithmResponseTypeDef](./type_defs.md#describealgorithmresponsetypedef).

<a id="describe_batch_inference_job"></a>

### describe_batch_inference_job

Gets the properties of a batch inference job including name, Amazon Resource
Name (ARN), status, input and output configurations, and the ARN of the
solution version used to generate the recommendations.

Type annotations for
`aiobotocore.create_client("personalize").describe_batch_inference_job` method.

Boto3 documentation:
[Personalize.Client.describe_batch_inference_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_inference_job)

Asynchronous method. Use `await describe_batch_inference_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeBatchInferenceJobRequestRequestTypeDef](./type_defs.md#describebatchinferencejobrequestrequesttypedef).

Keyword-only arguments:

- `batchInferenceJobArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBatchInferenceJobResponseTypeDef](./type_defs.md#describebatchinferencejobresponsetypedef).

<a id="describe_batch_segment_job"></a>

### describe_batch_segment_job

Gets the properties of a batch segment job including name, Amazon Resource Name
(ARN), status, input and output configurations, and the ARN of the solution
version used to generate segments.

Type annotations for
`aiobotocore.create_client("personalize").describe_batch_segment_job` method.

Boto3 documentation:
[Personalize.Client.describe_batch_segment_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_batch_segment_job)

Asynchronous method. Use `await describe_batch_segment_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeBatchSegmentJobRequestRequestTypeDef](./type_defs.md#describebatchsegmentjobrequestrequesttypedef).

Keyword-only arguments:

- `batchSegmentJobArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeBatchSegmentJobResponseTypeDef](./type_defs.md#describebatchsegmentjobresponsetypedef).

<a id="describe_campaign"></a>

### describe_campaign

Describes the given campaign, including its status.

Type annotations for
`aiobotocore.create_client("personalize").describe_campaign` method.

Boto3 documentation:
[Personalize.Client.describe_campaign](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_campaign)

Asynchronous method. Use `await describe_campaign(...)` for a synchronous call.

Arguments mapping described in
[DescribeCampaignRequestRequestTypeDef](./type_defs.md#describecampaignrequestrequesttypedef).

Keyword-only arguments:

- `campaignArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeCampaignResponseTypeDef](./type_defs.md#describecampaignresponsetypedef).

<a id="describe_dataset"></a>

### describe_dataset

Describes the given dataset.

Type annotations for
`aiobotocore.create_client("personalize").describe_dataset` method.

Boto3 documentation:
[Personalize.Client.describe_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset)

Asynchronous method. Use `await describe_dataset(...)` for a synchronous call.

Arguments mapping described in
[DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef).

Keyword-only arguments:

- `datasetArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef).

<a id="describe_dataset_export_job"></a>

### describe_dataset_export_job

Describes the dataset export job created by CreateDatasetExportJob , including
the export job status.

Type annotations for
`aiobotocore.create_client("personalize").describe_dataset_export_job` method.

Boto3 documentation:
[Personalize.Client.describe_dataset_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_export_job)

Asynchronous method. Use `await describe_dataset_export_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeDatasetExportJobRequestRequestTypeDef](./type_defs.md#describedatasetexportjobrequestrequesttypedef).

Keyword-only arguments:

- `datasetExportJobArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDatasetExportJobResponseTypeDef](./type_defs.md#describedatasetexportjobresponsetypedef).

<a id="describe_dataset_group"></a>

### describe_dataset_group

Describes the given dataset group.

Type annotations for
`aiobotocore.create_client("personalize").describe_dataset_group` method.

Boto3 documentation:
[Personalize.Client.describe_dataset_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_group)

Asynchronous method. Use `await describe_dataset_group(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDatasetGroupRequestRequestTypeDef](./type_defs.md#describedatasetgrouprequestrequesttypedef).

Keyword-only arguments:

- `datasetGroupArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDatasetGroupResponseTypeDef](./type_defs.md#describedatasetgroupresponsetypedef).

<a id="describe_dataset_import_job"></a>

### describe_dataset_import_job

Describes the dataset import job created by CreateDatasetImportJob , including
the import job status.

Type annotations for
`aiobotocore.create_client("personalize").describe_dataset_import_job` method.

Boto3 documentation:
[Personalize.Client.describe_dataset_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_dataset_import_job)

Asynchronous method. Use `await describe_dataset_import_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeDatasetImportJobRequestRequestTypeDef](./type_defs.md#describedatasetimportjobrequestrequesttypedef).

Keyword-only arguments:

- `datasetImportJobArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDatasetImportJobResponseTypeDef](./type_defs.md#describedatasetimportjobresponsetypedef).

<a id="describe_event_tracker"></a>

### describe_event_tracker

Describes an event tracker.

Type annotations for
`aiobotocore.create_client("personalize").describe_event_tracker` method.

Boto3 documentation:
[Personalize.Client.describe_event_tracker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_event_tracker)

Asynchronous method. Use `await describe_event_tracker(...)` for a synchronous
call.

Arguments mapping described in
[DescribeEventTrackerRequestRequestTypeDef](./type_defs.md#describeeventtrackerrequestrequesttypedef).

Keyword-only arguments:

- `eventTrackerArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeEventTrackerResponseTypeDef](./type_defs.md#describeeventtrackerresponsetypedef).

<a id="describe_feature_transformation"></a>

### describe_feature_transformation

Describes the given feature transformation.

Type annotations for
`aiobotocore.create_client("personalize").describe_feature_transformation`
method.

Boto3 documentation:
[Personalize.Client.describe_feature_transformation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_feature_transformation)

Asynchronous method. Use `await describe_feature_transformation(...)` for a
synchronous call.

Arguments mapping described in
[DescribeFeatureTransformationRequestRequestTypeDef](./type_defs.md#describefeaturetransformationrequestrequesttypedef).

Keyword-only arguments:

- `featureTransformationArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeFeatureTransformationResponseTypeDef](./type_defs.md#describefeaturetransformationresponsetypedef).

<a id="describe_filter"></a>

### describe_filter

Describes a filter's properties.

Type annotations for `aiobotocore.create_client("personalize").describe_filter`
method.

Boto3 documentation:
[Personalize.Client.describe_filter](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_filter)

Asynchronous method. Use `await describe_filter(...)` for a synchronous call.

Arguments mapping described in
[DescribeFilterRequestRequestTypeDef](./type_defs.md#describefilterrequestrequesttypedef).

Keyword-only arguments:

- `filterArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeFilterResponseTypeDef](./type_defs.md#describefilterresponsetypedef).

<a id="describe_recipe"></a>

### describe_recipe

Describes a recipe.

Type annotations for `aiobotocore.create_client("personalize").describe_recipe`
method.

Boto3 documentation:
[Personalize.Client.describe_recipe](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recipe)

Asynchronous method. Use `await describe_recipe(...)` for a synchronous call.

Arguments mapping described in
[DescribeRecipeRequestRequestTypeDef](./type_defs.md#describereciperequestrequesttypedef).

Keyword-only arguments:

- `recipeArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeRecipeResponseTypeDef](./type_defs.md#describereciperesponsetypedef).

<a id="describe_recommender"></a>

### describe_recommender

Describes the given recommender, including its status.

Type annotations for
`aiobotocore.create_client("personalize").describe_recommender` method.

Boto3 documentation:
[Personalize.Client.describe_recommender](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_recommender)

Asynchronous method. Use `await describe_recommender(...)` for a synchronous
call.

Arguments mapping described in
[DescribeRecommenderRequestRequestTypeDef](./type_defs.md#describerecommenderrequestrequesttypedef).

Keyword-only arguments:

- `recommenderArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeRecommenderResponseTypeDef](./type_defs.md#describerecommenderresponsetypedef).

<a id="describe_schema"></a>

### describe_schema

Describes a schema.

Type annotations for `aiobotocore.create_client("personalize").describe_schema`
method.

Boto3 documentation:
[Personalize.Client.describe_schema](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_schema)

Asynchronous method. Use `await describe_schema(...)` for a synchronous call.

Arguments mapping described in
[DescribeSchemaRequestRequestTypeDef](./type_defs.md#describeschemarequestrequesttypedef).

Keyword-only arguments:

- `schemaArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSchemaResponseTypeDef](./type_defs.md#describeschemaresponsetypedef).

<a id="describe_solution"></a>

### describe_solution

Describes a solution.

Type annotations for
`aiobotocore.create_client("personalize").describe_solution` method.

Boto3 documentation:
[Personalize.Client.describe_solution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution)

Asynchronous method. Use `await describe_solution(...)` for a synchronous call.

Arguments mapping described in
[DescribeSolutionRequestRequestTypeDef](./type_defs.md#describesolutionrequestrequesttypedef).

Keyword-only arguments:

- `solutionArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSolutionResponseTypeDef](./type_defs.md#describesolutionresponsetypedef).

<a id="describe_solution_version"></a>

### describe_solution_version

Describes a specific version of a solution.

Type annotations for
`aiobotocore.create_client("personalize").describe_solution_version` method.

Boto3 documentation:
[Personalize.Client.describe_solution_version](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.describe_solution_version)

Asynchronous method. Use `await describe_solution_version(...)` for a
synchronous call.

Arguments mapping described in
[DescribeSolutionVersionRequestRequestTypeDef](./type_defs.md#describesolutionversionrequestrequesttypedef).

Keyword-only arguments:

- `solutionVersionArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeSolutionVersionResponseTypeDef](./type_defs.md#describesolutionversionresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("personalize").generate_presigned_url` method.

Boto3 documentation:
[Personalize.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_solution_metrics"></a>

### get_solution_metrics

Gets the metrics for the specified solution version.

Type annotations for
`aiobotocore.create_client("personalize").get_solution_metrics` method.

Boto3 documentation:
[Personalize.Client.get_solution_metrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.get_solution_metrics)

Asynchronous method. Use `await get_solution_metrics(...)` for a synchronous
call.

Arguments mapping described in
[GetSolutionMetricsRequestRequestTypeDef](./type_defs.md#getsolutionmetricsrequestrequesttypedef).

Keyword-only arguments:

- `solutionVersionArn`: `str` *(required)*

Returns a `Coroutine` for
[GetSolutionMetricsResponseTypeDef](./type_defs.md#getsolutionmetricsresponsetypedef).

<a id="list_batch_inference_jobs"></a>

### list_batch_inference_jobs

Gets a list of the batch inference jobs that have been performed off of a
solution version.

Type annotations for
`aiobotocore.create_client("personalize").list_batch_inference_jobs` method.

Boto3 documentation:
[Personalize.Client.list_batch_inference_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_inference_jobs)

Asynchronous method. Use `await list_batch_inference_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListBatchInferenceJobsRequestRequestTypeDef](./type_defs.md#listbatchinferencejobsrequestrequesttypedef).

Keyword-only arguments:

- `solutionVersionArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListBatchInferenceJobsResponseTypeDef](./type_defs.md#listbatchinferencejobsresponsetypedef).

<a id="list_batch_segment_jobs"></a>

### list_batch_segment_jobs

Gets a list of the batch segment jobs that have been performed off of a
solution version that you specify.

Type annotations for
`aiobotocore.create_client("personalize").list_batch_segment_jobs` method.

Boto3 documentation:
[Personalize.Client.list_batch_segment_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_batch_segment_jobs)

Asynchronous method. Use `await list_batch_segment_jobs(...)` for a synchronous
call.

Arguments mapping described in
[ListBatchSegmentJobsRequestRequestTypeDef](./type_defs.md#listbatchsegmentjobsrequestrequesttypedef).

Keyword-only arguments:

- `solutionVersionArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListBatchSegmentJobsResponseTypeDef](./type_defs.md#listbatchsegmentjobsresponsetypedef).

<a id="list_campaigns"></a>

### list_campaigns

Returns a list of campaigns that use the given solution.

Type annotations for `aiobotocore.create_client("personalize").list_campaigns`
method.

Boto3 documentation:
[Personalize.Client.list_campaigns](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_campaigns)

Asynchronous method. Use `await list_campaigns(...)` for a synchronous call.

Arguments mapping described in
[ListCampaignsRequestRequestTypeDef](./type_defs.md#listcampaignsrequestrequesttypedef).

Keyword-only arguments:

- `solutionArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef).

<a id="list_dataset_export_jobs"></a>

### list_dataset_export_jobs

Returns a list of dataset export jobs that use the given dataset.

Type annotations for
`aiobotocore.create_client("personalize").list_dataset_export_jobs` method.

Boto3 documentation:
[Personalize.Client.list_dataset_export_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_export_jobs)

Asynchronous method. Use `await list_dataset_export_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListDatasetExportJobsRequestRequestTypeDef](./type_defs.md#listdatasetexportjobsrequestrequesttypedef).

Keyword-only arguments:

- `datasetArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListDatasetExportJobsResponseTypeDef](./type_defs.md#listdatasetexportjobsresponsetypedef).

<a id="list_dataset_groups"></a>

### list_dataset_groups

Returns a list of dataset groups.

Type annotations for
`aiobotocore.create_client("personalize").list_dataset_groups` method.

Boto3 documentation:
[Personalize.Client.list_dataset_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_groups)

Asynchronous method. Use `await list_dataset_groups(...)` for a synchronous
call.

Arguments mapping described in
[ListDatasetGroupsRequestRequestTypeDef](./type_defs.md#listdatasetgroupsrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef).

<a id="list_dataset_import_jobs"></a>

### list_dataset_import_jobs

Returns a list of dataset import jobs that use the given dataset.

Type annotations for
`aiobotocore.create_client("personalize").list_dataset_import_jobs` method.

Boto3 documentation:
[Personalize.Client.list_dataset_import_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_dataset_import_jobs)

Asynchronous method. Use `await list_dataset_import_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListDatasetImportJobsRequestRequestTypeDef](./type_defs.md#listdatasetimportjobsrequestrequesttypedef).

Keyword-only arguments:

- `datasetArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef).

<a id="list_datasets"></a>

### list_datasets

Returns the list of datasets contained in the given dataset group.

Type annotations for `aiobotocore.create_client("personalize").list_datasets`
method.

Boto3 documentation:
[Personalize.Client.list_datasets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_datasets)

Asynchronous method. Use `await list_datasets(...)` for a synchronous call.

Arguments mapping described in
[ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef).

Keyword-only arguments:

- `datasetGroupArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef).

<a id="list_event_trackers"></a>

### list_event_trackers

Returns the list of event trackers associated with the account.

Type annotations for
`aiobotocore.create_client("personalize").list_event_trackers` method.

Boto3 documentation:
[Personalize.Client.list_event_trackers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_event_trackers)

Asynchronous method. Use `await list_event_trackers(...)` for a synchronous
call.

Arguments mapping described in
[ListEventTrackersRequestRequestTypeDef](./type_defs.md#listeventtrackersrequestrequesttypedef).

Keyword-only arguments:

- `datasetGroupArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListEventTrackersResponseTypeDef](./type_defs.md#listeventtrackersresponsetypedef).

<a id="list_filters"></a>

### list_filters

Lists all filters that belong to a given dataset group.

Type annotations for `aiobotocore.create_client("personalize").list_filters`
method.

Boto3 documentation:
[Personalize.Client.list_filters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_filters)

Asynchronous method. Use `await list_filters(...)` for a synchronous call.

Arguments mapping described in
[ListFiltersRequestRequestTypeDef](./type_defs.md#listfiltersrequestrequesttypedef).

Keyword-only arguments:

- `datasetGroupArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef).

<a id="list_recipes"></a>

### list_recipes

Returns a list of available recipes.

Type annotations for `aiobotocore.create_client("personalize").list_recipes`
method.

Boto3 documentation:
[Personalize.Client.list_recipes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recipes)

Asynchronous method. Use `await list_recipes(...)` for a synchronous call.

Arguments mapping described in
[ListRecipesRequestRequestTypeDef](./type_defs.md#listrecipesrequestrequesttypedef).

Keyword-only arguments:

- `recipeProvider`: `Literal['SERVICE']` (see
  [RecipeProviderType](./literals.md#recipeprovidertype))
- `nextToken`: `str`
- `maxResults`: `int`
- `domain`: [DomainType](./literals.md#domaintype)

Returns a `Coroutine` for
[ListRecipesResponseTypeDef](./type_defs.md#listrecipesresponsetypedef).

<a id="list_recommenders"></a>

### list_recommenders

Returns a list of recommenders in a given Domain dataset group.

Type annotations for
`aiobotocore.create_client("personalize").list_recommenders` method.

Boto3 documentation:
[Personalize.Client.list_recommenders](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recommenders)

Asynchronous method. Use `await list_recommenders(...)` for a synchronous call.

Arguments mapping described in
[ListRecommendersRequestRequestTypeDef](./type_defs.md#listrecommendersrequestrequesttypedef).

Keyword-only arguments:

- `datasetGroupArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListRecommendersResponseTypeDef](./type_defs.md#listrecommendersresponsetypedef).

<a id="list_schemas"></a>

### list_schemas

Returns the list of schemas associated with the account.

Type annotations for `aiobotocore.create_client("personalize").list_schemas`
method.

Boto3 documentation:
[Personalize.Client.list_schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_schemas)

Asynchronous method. Use `await list_schemas(...)` for a synchronous call.

Arguments mapping described in
[ListSchemasRequestRequestTypeDef](./type_defs.md#listschemasrequestrequesttypedef).

Keyword-only arguments:

- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListSchemasResponseTypeDef](./type_defs.md#listschemasresponsetypedef).

<a id="list_solution_versions"></a>

### list_solution_versions

Returns a list of solution versions for the given solution.

Type annotations for
`aiobotocore.create_client("personalize").list_solution_versions` method.

Boto3 documentation:
[Personalize.Client.list_solution_versions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solution_versions)

Asynchronous method. Use `await list_solution_versions(...)` for a synchronous
call.

Arguments mapping described in
[ListSolutionVersionsRequestRequestTypeDef](./type_defs.md#listsolutionversionsrequestrequesttypedef).

Keyword-only arguments:

- `solutionArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListSolutionVersionsResponseTypeDef](./type_defs.md#listsolutionversionsresponsetypedef).

<a id="list_solutions"></a>

### list_solutions

Returns a list of solutions that use the given dataset group.

Type annotations for `aiobotocore.create_client("personalize").list_solutions`
method.

Boto3 documentation:
[Personalize.Client.list_solutions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_solutions)

Asynchronous method. Use `await list_solutions(...)` for a synchronous call.

Arguments mapping described in
[ListSolutionsRequestRequestTypeDef](./type_defs.md#listsolutionsrequestrequesttypedef).

Keyword-only arguments:

- `datasetGroupArn`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef).

<a id="stop_solution_version_creation"></a>

### stop_solution_version_creation

Stops creating a solution version that is in a state of CREATE_PENDING or
CREATE IN_PROGRESS.

Type annotations for
`aiobotocore.create_client("personalize").stop_solution_version_creation`
method.

Boto3 documentation:
[Personalize.Client.stop_solution_version_creation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.stop_solution_version_creation)

Asynchronous method. Use `await stop_solution_version_creation(...)` for a
synchronous call.

Arguments mapping described in
[StopSolutionVersionCreationRequestRequestTypeDef](./type_defs.md#stopsolutionversioncreationrequestrequesttypedef).

Keyword-only arguments:

- `solutionVersionArn`: `str` *(required)*

<a id="update_campaign"></a>

### update_campaign

Updates a campaign by either deploying a new solution or changing the value of
the campaign's `minProvisionedTPS` parameter.

Type annotations for `aiobotocore.create_client("personalize").update_campaign`
method.

Boto3 documentation:
[Personalize.Client.update_campaign](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_campaign)

Asynchronous method. Use `await update_campaign(...)` for a synchronous call.

Arguments mapping described in
[UpdateCampaignRequestRequestTypeDef](./type_defs.md#updatecampaignrequestrequesttypedef).

Keyword-only arguments:

- `campaignArn`: `str` *(required)*
- `solutionVersionArn`: `str`
- `minProvisionedTPS`: `int`
- `campaignConfig`:
  [CampaignConfigTypeDef](./type_defs.md#campaignconfigtypedef)

Returns a `Coroutine` for
[UpdateCampaignResponseTypeDef](./type_defs.md#updatecampaignresponsetypedef).

<a id="update_recommender"></a>

### update_recommender

Updates the recommender to modify the recommender configuration.

Type annotations for
`aiobotocore.create_client("personalize").update_recommender` method.

Boto3 documentation:
[Personalize.Client.update_recommender](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_recommender)

Asynchronous method. Use `await update_recommender(...)` for a synchronous
call.

Arguments mapping described in
[UpdateRecommenderRequestRequestTypeDef](./type_defs.md#updaterecommenderrequestrequesttypedef).

Keyword-only arguments:

- `recommenderArn`: `str` *(required)*
- `recommenderConfig`:
  [RecommenderConfigTypeDef](./type_defs.md#recommenderconfigtypedef)
  *(required)*

Returns a `Coroutine` for
[UpdateRecommenderResponseTypeDef](./type_defs.md#updaterecommenderresponsetypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("personalize").get_paginator`
method with overloads.

- `client.get_paginator("list_batch_inference_jobs")` ->
  [ListBatchInferenceJobsPaginator](./paginators.md#listbatchinferencejobspaginator)
- `client.get_paginator("list_batch_segment_jobs")` ->
  [ListBatchSegmentJobsPaginator](./paginators.md#listbatchsegmentjobspaginator)
- `client.get_paginator("list_campaigns")` ->
  [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
- `client.get_paginator("list_dataset_export_jobs")` ->
  [ListDatasetExportJobsPaginator](./paginators.md#listdatasetexportjobspaginator)
- `client.get_paginator("list_dataset_groups")` ->
  [ListDatasetGroupsPaginator](./paginators.md#listdatasetgroupspaginator)
- `client.get_paginator("list_dataset_import_jobs")` ->
  [ListDatasetImportJobsPaginator](./paginators.md#listdatasetimportjobspaginator)
- `client.get_paginator("list_datasets")` ->
  [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- `client.get_paginator("list_event_trackers")` ->
  [ListEventTrackersPaginator](./paginators.md#listeventtrackerspaginator)
- `client.get_paginator("list_filters")` ->
  [ListFiltersPaginator](./paginators.md#listfilterspaginator)
- `client.get_paginator("list_recipes")` ->
  [ListRecipesPaginator](./paginators.md#listrecipespaginator)
- `client.get_paginator("list_recommenders")` ->
  [ListRecommendersPaginator](./paginators.md#listrecommenderspaginator)
- `client.get_paginator("list_schemas")` ->
  [ListSchemasPaginator](./paginators.md#listschemaspaginator)
- `client.get_paginator("list_solution_versions")` ->
  [ListSolutionVersionsPaginator](./paginators.md#listsolutionversionspaginator)
- `client.get_paginator("list_solutions")` ->
  [ListSolutionsPaginator](./paginators.md#listsolutionspaginator)
