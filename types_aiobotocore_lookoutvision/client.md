<a id="lookoutforvisionclient-for-aiobotocore-lookoutforvision-module"></a>

# LookoutforVisionClient for aiobotocore LookoutforVision module

> [Index](..) > [LookoutforVision](.) > LookoutforVisionClient

Auto-generated documentation for
[LookoutforVision](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision)
type annotations stubs module
[types-aiobotocore-lookoutvision](https://pypi.org/project/types-aiobotocore-lookoutvision/).

- [LookoutforVisionClient for aiobotocore LookoutforVision module](#lookoutforvisionclient-for-aiobotocore-lookoutforvision-module)
  - [LookoutforVisionClient](#lookoutforvisionclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_dataset](#create_dataset)
    - [create_model](#create_model)
    - [create_project](#create_project)
    - [delete_dataset](#delete_dataset)
    - [delete_model](#delete_model)
    - [delete_project](#delete_project)
    - [describe_dataset](#describe_dataset)
    - [describe_model](#describe_model)
    - [describe_model_packaging_job](#describe_model_packaging_job)
    - [describe_project](#describe_project)
    - [detect_anomalies](#detect_anomalies)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_dataset_entries](#list_dataset_entries)
    - [list_model_packaging_jobs](#list_model_packaging_jobs)
    - [list_models](#list_models)
    - [list_projects](#list_projects)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [start_model](#start_model)
    - [start_model_packaging_job](#start_model_packaging_job)
    - [stop_model](#stop_model)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_dataset_entries](#update_dataset_entries)
    - [get_paginator](#get_paginator)

<a id="lookoutforvisionclient"></a>

## LookoutforVisionClient

Type annotations for `aiobotocore.create_client("lookoutvision")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_lookoutvision.client import LookoutforVisionClient

def get_lookoutvision_client() -> LookoutforVisionClient:
    return Session().client("lookoutvision")
```

Boto3 documentation:
[LookoutforVision.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_lookoutvision.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

LookoutforVisionClient exceptions.

Type annotations for `aiobotocore.create_client("lookoutvision").exceptions`
method.

Boto3 documentation:
[LookoutforVision.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("lookoutvision").can_paginate`
method.

Boto3 documentation:
[LookoutforVision.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_dataset"></a>

### create_dataset

Creates a new dataset in an Amazon Lookout for Vision project.

Type annotations for
`aiobotocore.create_client("lookoutvision").create_dataset` method.

Boto3 documentation:
[LookoutforVision.Client.create_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.create_dataset)

Asynchronous method. Use `await create_dataset(...)` for a synchronous call.

Arguments mapping described in
[CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `DatasetType`: `str` *(required)*
- `DatasetSource`: [DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef)
- `ClientToken`: `str`

Returns a `Coroutine` for
[CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef).

<a id="create_model"></a>

### create_model

Creates a new version of a model within an an Amazon Lookout for Vision
project.

Type annotations for `aiobotocore.create_client("lookoutvision").create_model`
method.

Boto3 documentation:
[LookoutforVision.Client.create_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.create_model)

Asynchronous method. Use `await create_model(...)` for a synchronous call.

Arguments mapping described in
[CreateModelRequestRequestTypeDef](./type_defs.md#createmodelrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `OutputConfig`: [OutputConfigTypeDef](./type_defs.md#outputconfigtypedef)
  *(required)*
- `Description`: `str`
- `ClientToken`: `str`
- `KmsKeyId`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateModelResponseTypeDef](./type_defs.md#createmodelresponsetypedef).

<a id="create_project"></a>

### create_project

Creates an empty Amazon Lookout for Vision project.

Type annotations for
`aiobotocore.create_client("lookoutvision").create_project` method.

Boto3 documentation:
[LookoutforVision.Client.create_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.create_project)

Asynchronous method. Use `await create_project(...)` for a synchronous call.

Arguments mapping described in
[CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `ClientToken`: `str`

Returns a `Coroutine` for
[CreateProjectResponseTypeDef](./type_defs.md#createprojectresponsetypedef).

<a id="delete_dataset"></a>

### delete_dataset

Deletes an existing Amazon Lookout for Vision `dataset` .

Type annotations for
`aiobotocore.create_client("lookoutvision").delete_dataset` method.

Boto3 documentation:
[LookoutforVision.Client.delete_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.delete_dataset)

Asynchronous method. Use `await delete_dataset(...)` for a synchronous call.

Arguments mapping described in
[DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `DatasetType`: `str` *(required)*
- `ClientToken`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_model"></a>

### delete_model

Deletes an Amazon Lookout for Vision model.

Type annotations for `aiobotocore.create_client("lookoutvision").delete_model`
method.

Boto3 documentation:
[LookoutforVision.Client.delete_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.delete_model)

Asynchronous method. Use `await delete_model(...)` for a synchronous call.

Arguments mapping described in
[DeleteModelRequestRequestTypeDef](./type_defs.md#deletemodelrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `ModelVersion`: `str` *(required)*
- `ClientToken`: `str`

Returns a `Coroutine` for
[DeleteModelResponseTypeDef](./type_defs.md#deletemodelresponsetypedef).

<a id="delete_project"></a>

### delete_project

Deletes an Amazon Lookout for Vision project.

Type annotations for
`aiobotocore.create_client("lookoutvision").delete_project` method.

Boto3 documentation:
[LookoutforVision.Client.delete_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.delete_project)

Asynchronous method. Use `await delete_project(...)` for a synchronous call.

Arguments mapping described in
[DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `ClientToken`: `str`

Returns a `Coroutine` for
[DeleteProjectResponseTypeDef](./type_defs.md#deleteprojectresponsetypedef).

<a id="describe_dataset"></a>

### describe_dataset

Describe an Amazon Lookout for Vision dataset.

Type annotations for
`aiobotocore.create_client("lookoutvision").describe_dataset` method.

Boto3 documentation:
[LookoutforVision.Client.describe_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.describe_dataset)

Asynchronous method. Use `await describe_dataset(...)` for a synchronous call.

Arguments mapping described in
[DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `DatasetType`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef).

<a id="describe_model"></a>

### describe_model

Describes a version of an Amazon Lookout for Vision model.

Type annotations for
`aiobotocore.create_client("lookoutvision").describe_model` method.

Boto3 documentation:
[LookoutforVision.Client.describe_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.describe_model)

Asynchronous method. Use `await describe_model(...)` for a synchronous call.

Arguments mapping described in
[DescribeModelRequestRequestTypeDef](./type_defs.md#describemodelrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `ModelVersion`: `str` *(required)*

Returns a `Coroutine` for
[DescribeModelResponseTypeDef](./type_defs.md#describemodelresponsetypedef).

<a id="describe_model_packaging_job"></a>

### describe_model_packaging_job

Describes an Amazon Lookout for Vision model packaging job.

Type annotations for
`aiobotocore.create_client("lookoutvision").describe_model_packaging_job`
method.

Boto3 documentation:
[LookoutforVision.Client.describe_model_packaging_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.describe_model_packaging_job)

Asynchronous method. Use `await describe_model_packaging_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeModelPackagingJobRequestRequestTypeDef](./type_defs.md#describemodelpackagingjobrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `JobName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeModelPackagingJobResponseTypeDef](./type_defs.md#describemodelpackagingjobresponsetypedef).

<a id="describe_project"></a>

### describe_project

Describes an Amazon Lookout for Vision project.

Type annotations for
`aiobotocore.create_client("lookoutvision").describe_project` method.

Boto3 documentation:
[LookoutforVision.Client.describe_project](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.describe_project)

Asynchronous method. Use `await describe_project(...)` for a synchronous call.

Arguments mapping described in
[DescribeProjectRequestRequestTypeDef](./type_defs.md#describeprojectrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeProjectResponseTypeDef](./type_defs.md#describeprojectresponsetypedef).

<a id="detect_anomalies"></a>

### detect_anomalies

Detects anomalies in an image that you supply.

Type annotations for
`aiobotocore.create_client("lookoutvision").detect_anomalies` method.

Boto3 documentation:
[LookoutforVision.Client.detect_anomalies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.detect_anomalies)

Asynchronous method. Use `await detect_anomalies(...)` for a synchronous call.

Arguments mapping described in
[DetectAnomaliesRequestRequestTypeDef](./type_defs.md#detectanomaliesrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `ModelVersion`: `str` *(required)*
- `Body`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\] *(required)*
- `ContentType`: `str` *(required)*

Returns a `Coroutine` for
[DetectAnomaliesResponseTypeDef](./type_defs.md#detectanomaliesresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("lookoutvision").generate_presigned_url` method.

Boto3 documentation:
[LookoutforVision.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_dataset_entries"></a>

### list_dataset_entries

Lists the JSON Lines within a dataset.

Type annotations for
`aiobotocore.create_client("lookoutvision").list_dataset_entries` method.

Boto3 documentation:
[LookoutforVision.Client.list_dataset_entries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.list_dataset_entries)

Asynchronous method. Use `await list_dataset_entries(...)` for a synchronous
call.

Arguments mapping described in
[ListDatasetEntriesRequestRequestTypeDef](./type_defs.md#listdatasetentriesrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `DatasetType`: `str` *(required)*
- `Labeled`: `bool`
- `AnomalyClass`: `str`
- `BeforeCreationDate`: `Union`\[`datetime`, `str`\]
- `AfterCreationDate`: `Union`\[`datetime`, `str`\]
- `NextToken`: `str`
- `MaxResults`: `int`
- `SourceRefContains`: `str`

Returns a `Coroutine` for
[ListDatasetEntriesResponseTypeDef](./type_defs.md#listdatasetentriesresponsetypedef).

<a id="list_model_packaging_jobs"></a>

### list_model_packaging_jobs

Lists the model packaging jobs created for an Amazon Lookout for Vision
project.

Type annotations for
`aiobotocore.create_client("lookoutvision").list_model_packaging_jobs` method.

Boto3 documentation:
[LookoutforVision.Client.list_model_packaging_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.list_model_packaging_jobs)

Asynchronous method. Use `await list_model_packaging_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListModelPackagingJobsRequestRequestTypeDef](./type_defs.md#listmodelpackagingjobsrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListModelPackagingJobsResponseTypeDef](./type_defs.md#listmodelpackagingjobsresponsetypedef).

<a id="list_models"></a>

### list_models

Lists the versions of a model in an Amazon Lookout for Vision project.

Type annotations for `aiobotocore.create_client("lookoutvision").list_models`
method.

Boto3 documentation:
[LookoutforVision.Client.list_models](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.list_models)

Asynchronous method. Use `await list_models(...)` for a synchronous call.

Arguments mapping described in
[ListModelsRequestRequestTypeDef](./type_defs.md#listmodelsrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListModelsResponseTypeDef](./type_defs.md#listmodelsresponsetypedef).

<a id="list_projects"></a>

### list_projects

Lists the Amazon Lookout for Vision projects in your AWS account.

Type annotations for `aiobotocore.create_client("lookoutvision").list_projects`
method.

Boto3 documentation:
[LookoutforVision.Client.list_projects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.list_projects)

Asynchronous method. Use `await list_projects(...)` for a synchronous call.

Arguments mapping described in
[ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Returns a list of tags attached to the specified Amazon Lookout for Vision
model.

Type annotations for
`aiobotocore.create_client("lookoutvision").list_tags_for_resource` method.

Boto3 documentation:
[LookoutforVision.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="start_model"></a>

### start_model

Starts the running of the version of an Amazon Lookout for Vision model.

Type annotations for `aiobotocore.create_client("lookoutvision").start_model`
method.

Boto3 documentation:
[LookoutforVision.Client.start_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.start_model)

Asynchronous method. Use `await start_model(...)` for a synchronous call.

Arguments mapping described in
[StartModelRequestRequestTypeDef](./type_defs.md#startmodelrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `ModelVersion`: `str` *(required)*
- `MinInferenceUnits`: `int` *(required)*
- `ClientToken`: `str`

Returns a `Coroutine` for
[StartModelResponseTypeDef](./type_defs.md#startmodelresponsetypedef).

<a id="start_model_packaging_job"></a>

### start_model_packaging_job

Starts an Amazon Lookout for Vision model packaging job.

Type annotations for
`aiobotocore.create_client("lookoutvision").start_model_packaging_job` method.

Boto3 documentation:
[LookoutforVision.Client.start_model_packaging_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.start_model_packaging_job)

Asynchronous method. Use `await start_model_packaging_job(...)` for a
synchronous call.

Arguments mapping described in
[StartModelPackagingJobRequestRequestTypeDef](./type_defs.md#startmodelpackagingjobrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `ModelVersion`: `str` *(required)*
- `Configuration`:
  [ModelPackagingConfigurationTypeDef](./type_defs.md#modelpackagingconfigurationtypedef)
  *(required)*
- `JobName`: `str`
- `Description`: `str`
- `ClientToken`: `str`

Returns a `Coroutine` for
[StartModelPackagingJobResponseTypeDef](./type_defs.md#startmodelpackagingjobresponsetypedef).

<a id="stop_model"></a>

### stop_model

Stops the hosting of a running model.

Type annotations for `aiobotocore.create_client("lookoutvision").stop_model`
method.

Boto3 documentation:
[LookoutforVision.Client.stop_model](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.stop_model)

Asynchronous method. Use `await stop_model(...)` for a synchronous call.

Arguments mapping described in
[StopModelRequestRequestTypeDef](./type_defs.md#stopmodelrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `ModelVersion`: `str` *(required)*
- `ClientToken`: `str`

Returns a `Coroutine` for
[StopModelResponseTypeDef](./type_defs.md#stopmodelresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds one or more key-value tags to an Amazon Lookout for Vision model.

Type annotations for `aiobotocore.create_client("lookoutvision").tag_resource`
method.

Boto3 documentation:
[LookoutforVision.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes one or more tags from an Amazon Lookout for Vision model.

Type annotations for
`aiobotocore.create_client("lookoutvision").untag_resource` method.

Boto3 documentation:
[LookoutforVision.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_dataset_entries"></a>

### update_dataset_entries

Adds or updates one or more JSON Line entries in a dataset.

Type annotations for
`aiobotocore.create_client("lookoutvision").update_dataset_entries` method.

Boto3 documentation:
[LookoutforVision.Client.update_dataset_entries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutvision.html#LookoutforVision.Client.update_dataset_entries)

Asynchronous method. Use `await update_dataset_entries(...)` for a synchronous
call.

Arguments mapping described in
[UpdateDatasetEntriesRequestRequestTypeDef](./type_defs.md#updatedatasetentriesrequestrequesttypedef).

Keyword-only arguments:

- `ProjectName`: `str` *(required)*
- `DatasetType`: `str` *(required)*
- `Changes`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\] *(required)*
- `ClientToken`: `str`

Returns a `Coroutine` for
[UpdateDatasetEntriesResponseTypeDef](./type_defs.md#updatedatasetentriesresponsetypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("lookoutvision").get_paginator`
method with overloads.

- `client.get_paginator("list_dataset_entries")` ->
  [ListDatasetEntriesPaginator](./paginators.md#listdatasetentriespaginator)
- `client.get_paginator("list_model_packaging_jobs")` ->
  [ListModelPackagingJobsPaginator](./paginators.md#listmodelpackagingjobspaginator)
- `client.get_paginator("list_models")` ->
  [ListModelsPaginator](./paginators.md#listmodelspaginator)
- `client.get_paginator("list_projects")` ->
  [ListProjectsPaginator](./paginators.md#listprojectspaginator)
