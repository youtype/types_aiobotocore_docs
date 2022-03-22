<a id="forecastserviceclient-for-aiobotocore-forecastservice-module"></a>

# ForecastServiceClient for aiobotocore ForecastService module

> [Index](../README.md) > [ForecastService](./README.md) >
> ForecastServiceClient

Auto-generated documentation for
[ForecastService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
type annotations stubs module
[types-aiobotocore-forecast](https://pypi.org/project/types-aiobotocore-forecast/).

- [ForecastServiceClient for aiobotocore ForecastService module](#forecastserviceclient-for-aiobotocore-forecastservice-module)
  - [ForecastServiceClient](#forecastserviceclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_auto_predictor](#create_auto_predictor)
    - [create_dataset](#create_dataset)
    - [create_dataset_group](#create_dataset_group)
    - [create_dataset_import_job](#create_dataset_import_job)
    - [create_explainability](#create_explainability)
    - [create_explainability_export](#create_explainability_export)
    - [create_forecast](#create_forecast)
    - [create_forecast_export_job](#create_forecast_export_job)
    - [create_predictor](#create_predictor)
    - [create_predictor_backtest_export_job](#create_predictor_backtest_export_job)
    - [delete_dataset](#delete_dataset)
    - [delete_dataset_group](#delete_dataset_group)
    - [delete_dataset_import_job](#delete_dataset_import_job)
    - [delete_explainability](#delete_explainability)
    - [delete_explainability_export](#delete_explainability_export)
    - [delete_forecast](#delete_forecast)
    - [delete_forecast_export_job](#delete_forecast_export_job)
    - [delete_predictor](#delete_predictor)
    - [delete_predictor_backtest_export_job](#delete_predictor_backtest_export_job)
    - [delete_resource_tree](#delete_resource_tree)
    - [describe_auto_predictor](#describe_auto_predictor)
    - [describe_dataset](#describe_dataset)
    - [describe_dataset_group](#describe_dataset_group)
    - [describe_dataset_import_job](#describe_dataset_import_job)
    - [describe_explainability](#describe_explainability)
    - [describe_explainability_export](#describe_explainability_export)
    - [describe_forecast](#describe_forecast)
    - [describe_forecast_export_job](#describe_forecast_export_job)
    - [describe_predictor](#describe_predictor)
    - [describe_predictor_backtest_export_job](#describe_predictor_backtest_export_job)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_accuracy_metrics](#get_accuracy_metrics)
    - [list_dataset_groups](#list_dataset_groups)
    - [list_dataset_import_jobs](#list_dataset_import_jobs)
    - [list_datasets](#list_datasets)
    - [list_explainabilities](#list_explainabilities)
    - [list_explainability_exports](#list_explainability_exports)
    - [list_forecast_export_jobs](#list_forecast_export_jobs)
    - [list_forecasts](#list_forecasts)
    - [list_predictor_backtest_export_jobs](#list_predictor_backtest_export_jobs)
    - [list_predictors](#list_predictors)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [stop_resource](#stop_resource)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_dataset_group](#update_dataset_group)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="forecastserviceclient"></a>

## ForecastServiceClient

Type annotations for `session.create_client("forecast")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_forecast.client import ForecastServiceClient

session = get_session()
async with session.create_client("forecast") as client:
    client: ForecastServiceClient
```

Boto3 documentation:
[ForecastService.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_forecast.client import Exceptions

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

ForecastServiceClient exceptions.

Type annotations for `session.create_client("forecast").exceptions` method.

Boto3 documentation:
[ForecastService.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("forecast").can_paginate` method.

Boto3 documentation:
[ForecastService.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_auto\_predictor"></a>

### create_auto_predictor

Creates an Amazon Forecast predictor.

Type annotations for `session.create_client("forecast").create_auto_predictor`
method.

Boto3 documentation:
[ForecastService.Client.create_auto_predictor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_auto_predictor)

Asynchronous method. Use `await create_auto_predictor(...)` for a synchronous
call.

Arguments mapping described in
[CreateAutoPredictorRequestRequestTypeDef](./type_defs.md#createautopredictorrequestrequesttypedef).

Keyword-only arguments:

- `PredictorName`: `str` *(required)*
- `ForecastHorizon`: `int`
- `ForecastTypes`: `Sequence`\[`str`\]
- `ForecastDimensions`: `Sequence`\[`str`\]
- `ForecastFrequency`: `str`
- `DataConfig`: [DataConfigTypeDef](./type_defs.md#dataconfigtypedef)
- `EncryptionConfig`:
  [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- `ReferencePredictorArn`: `str`
- `OptimizationMetric`:
  [OptimizationMetricType](./literals.md#optimizationmetrictype)
- `ExplainPredictor`: `bool`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateAutoPredictorResponseTypeDef](./type_defs.md#createautopredictorresponsetypedef).

<a id="create\_dataset"></a>

### create_dataset

Creates an Amazon Forecast dataset.

Type annotations for `session.create_client("forecast").create_dataset` method.

Boto3 documentation:
[ForecastService.Client.create_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_dataset)

Asynchronous method. Use `await create_dataset(...)` for a synchronous call.

Arguments mapping described in
[CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef).

Keyword-only arguments:

- `DatasetName`: `str` *(required)*
- `Domain`: [DomainType](./literals.md#domaintype) *(required)*
- `DatasetType`: [DatasetTypeType](./literals.md#datasettypetype) *(required)*
- `Schema`: [SchemaTypeDef](./type_defs.md#schematypedef) *(required)*
- `DataFrequency`: `str`
- `EncryptionConfig`:
  [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef).

<a id="create\_dataset\_group"></a>

### create_dataset_group

Creates a dataset group, which holds a collection of related datasets.

Type annotations for `session.create_client("forecast").create_dataset_group`
method.

Boto3 documentation:
[ForecastService.Client.create_dataset_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_dataset_group)

Asynchronous method. Use `await create_dataset_group(...)` for a synchronous
call.

Arguments mapping described in
[CreateDatasetGroupRequestRequestTypeDef](./type_defs.md#createdatasetgrouprequestrequesttypedef).

Keyword-only arguments:

- `DatasetGroupName`: `str` *(required)*
- `Domain`: [DomainType](./literals.md#domaintype) *(required)*
- `DatasetArns`: `Sequence`\[`str`\]
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateDatasetGroupResponseTypeDef](./type_defs.md#createdatasetgroupresponsetypedef).

<a id="create\_dataset\_import\_job"></a>

### create_dataset_import_job

Imports your training data to an Amazon Forecast dataset.

Type annotations for
`session.create_client("forecast").create_dataset_import_job` method.

Boto3 documentation:
[ForecastService.Client.create_dataset_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_dataset_import_job)

Asynchronous method. Use `await create_dataset_import_job(...)` for a
synchronous call.

Arguments mapping described in
[CreateDatasetImportJobRequestRequestTypeDef](./type_defs.md#createdatasetimportjobrequestrequesttypedef).

Keyword-only arguments:

- `DatasetImportJobName`: `str` *(required)*
- `DatasetArn`: `str` *(required)*
- `DataSource`: [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
  *(required)*
- `TimestampFormat`: `str`
- `TimeZone`: `str`
- `UseGeolocationForTimeZone`: `bool`
- `GeolocationFormat`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateDatasetImportJobResponseTypeDef](./type_defs.md#createdatasetimportjobresponsetypedef).

<a id="create\_explainability"></a>

### create_explainability

.

Type annotations for `session.create_client("forecast").create_explainability`
method.

Boto3 documentation:
[ForecastService.Client.create_explainability](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_explainability)

Asynchronous method. Use `await create_explainability(...)` for a synchronous
call.

Arguments mapping described in
[CreateExplainabilityRequestRequestTypeDef](./type_defs.md#createexplainabilityrequestrequesttypedef).

Keyword-only arguments:

- `ExplainabilityName`: `str` *(required)*
- `ResourceArn`: `str` *(required)*
- `ExplainabilityConfig`:
  [ExplainabilityConfigTypeDef](./type_defs.md#explainabilityconfigtypedef)
  *(required)*
- `DataSource`: [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- `Schema`: [SchemaTypeDef](./type_defs.md#schematypedef)
- `EnableVisualization`: `bool`
- `StartDateTime`: `str`
- `EndDateTime`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateExplainabilityResponseTypeDef](./type_defs.md#createexplainabilityresponsetypedef).

<a id="create\_explainability\_export"></a>

### create_explainability_export

Exports an Explainability resource created by the CreateExplainability
operation.

Type annotations for
`session.create_client("forecast").create_explainability_export` method.

Boto3 documentation:
[ForecastService.Client.create_explainability_export](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_explainability_export)

Asynchronous method. Use `await create_explainability_export(...)` for a
synchronous call.

Arguments mapping described in
[CreateExplainabilityExportRequestRequestTypeDef](./type_defs.md#createexplainabilityexportrequestrequesttypedef).

Keyword-only arguments:

- `ExplainabilityExportName`: `str` *(required)*
- `ExplainabilityArn`: `str` *(required)*
- `Destination`:
  [DataDestinationTypeDef](./type_defs.md#datadestinationtypedef) *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateExplainabilityExportResponseTypeDef](./type_defs.md#createexplainabilityexportresponsetypedef).

<a id="create\_forecast"></a>

### create_forecast

Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
used to train the predictor.

Type annotations for `session.create_client("forecast").create_forecast`
method.

Boto3 documentation:
[ForecastService.Client.create_forecast](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)

Asynchronous method. Use `await create_forecast(...)` for a synchronous call.

Arguments mapping described in
[CreateForecastRequestRequestTypeDef](./type_defs.md#createforecastrequestrequesttypedef).

Keyword-only arguments:

- `ForecastName`: `str` *(required)*
- `PredictorArn`: `str` *(required)*
- `ForecastTypes`: `Sequence`\[`str`\]
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateForecastResponseTypeDef](./type_defs.md#createforecastresponsetypedef).

<a id="create\_forecast\_export\_job"></a>

### create_forecast_export_job

Exports a forecast created by the CreateForecast operation to your Amazon
Simple Storage Service (Amazon S3) bucket.

Type annotations for
`session.create_client("forecast").create_forecast_export_job` method.

Boto3 documentation:
[ForecastService.Client.create_forecast_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast_export_job)

Asynchronous method. Use `await create_forecast_export_job(...)` for a
synchronous call.

Arguments mapping described in
[CreateForecastExportJobRequestRequestTypeDef](./type_defs.md#createforecastexportjobrequestrequesttypedef).

Keyword-only arguments:

- `ForecastExportJobName`: `str` *(required)*
- `ForecastArn`: `str` *(required)*
- `Destination`:
  [DataDestinationTypeDef](./type_defs.md#datadestinationtypedef) *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateForecastExportJobResponseTypeDef](./type_defs.md#createforecastexportjobresponsetypedef).

<a id="create\_predictor"></a>

### create_predictor

.

Type annotations for `session.create_client("forecast").create_predictor`
method.

Boto3 documentation:
[ForecastService.Client.create_predictor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_predictor)

Asynchronous method. Use `await create_predictor(...)` for a synchronous call.

Arguments mapping described in
[CreatePredictorRequestRequestTypeDef](./type_defs.md#createpredictorrequestrequesttypedef).

Keyword-only arguments:

- `PredictorName`: `str` *(required)*
- `ForecastHorizon`: `int` *(required)*
- `InputDataConfig`:
  [InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) *(required)*
- `FeaturizationConfig`:
  [FeaturizationConfigTypeDef](./type_defs.md#featurizationconfigtypedef)
  *(required)*
- `AlgorithmArn`: `str`
- `ForecastTypes`: `Sequence`\[`str`\]
- `PerformAutoML`: `bool`
- `AutoMLOverrideStrategy`:
  [AutoMLOverrideStrategyType](./literals.md#automloverridestrategytype)
- `PerformHPO`: `bool`
- `TrainingParameters`: `Mapping`\[`str`, `str`\]
- `EvaluationParameters`:
  [EvaluationParametersTypeDef](./type_defs.md#evaluationparameterstypedef)
- `HPOConfig`:
  [HyperParameterTuningJobConfigTypeDef](./type_defs.md#hyperparametertuningjobconfigtypedef)
- `EncryptionConfig`:
  [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `OptimizationMetric`:
  [OptimizationMetricType](./literals.md#optimizationmetrictype)

Returns a `Coroutine` for
[CreatePredictorResponseTypeDef](./type_defs.md#createpredictorresponsetypedef).

<a id="create\_predictor\_backtest\_export\_job"></a>

### create_predictor_backtest_export_job

Exports backtest forecasts and accuracy metrics generated by the
CreateAutoPredictor or CreatePredictor operations.

Type annotations for
`session.create_client("forecast").create_predictor_backtest_export_job`
method.

Boto3 documentation:
[ForecastService.Client.create_predictor_backtest_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_predictor_backtest_export_job)

Asynchronous method. Use `await create_predictor_backtest_export_job(...)` for
a synchronous call.

Arguments mapping described in
[CreatePredictorBacktestExportJobRequestRequestTypeDef](./type_defs.md#createpredictorbacktestexportjobrequestrequesttypedef).

Keyword-only arguments:

- `PredictorBacktestExportJobName`: `str` *(required)*
- `PredictorArn`: `str` *(required)*
- `Destination`:
  [DataDestinationTypeDef](./type_defs.md#datadestinationtypedef) *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreatePredictorBacktestExportJobResponseTypeDef](./type_defs.md#createpredictorbacktestexportjobresponsetypedef).

<a id="delete\_dataset"></a>

### delete_dataset

Deletes an Amazon Forecast dataset that was created using the CreateDataset
operation.

Type annotations for `session.create_client("forecast").delete_dataset` method.

Boto3 documentation:
[ForecastService.Client.delete_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.delete_dataset)

Asynchronous method. Use `await delete_dataset(...)` for a synchronous call.

Arguments mapping described in
[DeleteDatasetRequestRequestTypeDef](./type_defs.md#deletedatasetrequestrequesttypedef).

Keyword-only arguments:

- `DatasetArn`: `str` *(required)*

<a id="delete\_dataset\_group"></a>

### delete_dataset_group

Deletes a dataset group created using the CreateDatasetGroup operation.

Type annotations for `session.create_client("forecast").delete_dataset_group`
method.

Boto3 documentation:
[ForecastService.Client.delete_dataset_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.delete_dataset_group)

Asynchronous method. Use `await delete_dataset_group(...)` for a synchronous
call.

Arguments mapping described in
[DeleteDatasetGroupRequestRequestTypeDef](./type_defs.md#deletedatasetgrouprequestrequesttypedef).

Keyword-only arguments:

- `DatasetGroupArn`: `str` *(required)*

<a id="delete\_dataset\_import\_job"></a>

### delete_dataset_import_job

Deletes a dataset import job created using the CreateDatasetImportJob
operation.

Type annotations for
`session.create_client("forecast").delete_dataset_import_job` method.

Boto3 documentation:
[ForecastService.Client.delete_dataset_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.delete_dataset_import_job)

Asynchronous method. Use `await delete_dataset_import_job(...)` for a
synchronous call.

Arguments mapping described in
[DeleteDatasetImportJobRequestRequestTypeDef](./type_defs.md#deletedatasetimportjobrequestrequesttypedef).

Keyword-only arguments:

- `DatasetImportJobArn`: `str` *(required)*

<a id="delete\_explainability"></a>

### delete_explainability

Deletes an Explainability resource.

Type annotations for `session.create_client("forecast").delete_explainability`
method.

Boto3 documentation:
[ForecastService.Client.delete_explainability](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.delete_explainability)

Asynchronous method. Use `await delete_explainability(...)` for a synchronous
call.

Arguments mapping described in
[DeleteExplainabilityRequestRequestTypeDef](./type_defs.md#deleteexplainabilityrequestrequesttypedef).

Keyword-only arguments:

- `ExplainabilityArn`: `str` *(required)*

<a id="delete\_explainability\_export"></a>

### delete_explainability_export

Deletes an Explainability export.

Type annotations for
`session.create_client("forecast").delete_explainability_export` method.

Boto3 documentation:
[ForecastService.Client.delete_explainability_export](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.delete_explainability_export)

Asynchronous method. Use `await delete_explainability_export(...)` for a
synchronous call.

Arguments mapping described in
[DeleteExplainabilityExportRequestRequestTypeDef](./type_defs.md#deleteexplainabilityexportrequestrequesttypedef).

Keyword-only arguments:

- `ExplainabilityExportArn`: `str` *(required)*

<a id="delete\_forecast"></a>

### delete_forecast

Deletes a forecast created using the CreateForecast operation.

Type annotations for `session.create_client("forecast").delete_forecast`
method.

Boto3 documentation:
[ForecastService.Client.delete_forecast](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.delete_forecast)

Asynchronous method. Use `await delete_forecast(...)` for a synchronous call.

Arguments mapping described in
[DeleteForecastRequestRequestTypeDef](./type_defs.md#deleteforecastrequestrequesttypedef).

Keyword-only arguments:

- `ForecastArn`: `str` *(required)*

<a id="delete\_forecast\_export\_job"></a>

### delete_forecast_export_job

Deletes a forecast export job created using the CreateForecastExportJob
operation.

Type annotations for
`session.create_client("forecast").delete_forecast_export_job` method.

Boto3 documentation:
[ForecastService.Client.delete_forecast_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.delete_forecast_export_job)

Asynchronous method. Use `await delete_forecast_export_job(...)` for a
synchronous call.

Arguments mapping described in
[DeleteForecastExportJobRequestRequestTypeDef](./type_defs.md#deleteforecastexportjobrequestrequesttypedef).

Keyword-only arguments:

- `ForecastExportJobArn`: `str` *(required)*

<a id="delete\_predictor"></a>

### delete_predictor

Deletes a predictor created using the DescribePredictor or CreatePredictor
operations.

Type annotations for `session.create_client("forecast").delete_predictor`
method.

Boto3 documentation:
[ForecastService.Client.delete_predictor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.delete_predictor)

Asynchronous method. Use `await delete_predictor(...)` for a synchronous call.

Arguments mapping described in
[DeletePredictorRequestRequestTypeDef](./type_defs.md#deletepredictorrequestrequesttypedef).

Keyword-only arguments:

- `PredictorArn`: `str` *(required)*

<a id="delete\_predictor\_backtest\_export\_job"></a>

### delete_predictor_backtest_export_job

Deletes a predictor backtest export job.

Type annotations for
`session.create_client("forecast").delete_predictor_backtest_export_job`
method.

Boto3 documentation:
[ForecastService.Client.delete_predictor_backtest_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.delete_predictor_backtest_export_job)

Asynchronous method. Use `await delete_predictor_backtest_export_job(...)` for
a synchronous call.

Arguments mapping described in
[DeletePredictorBacktestExportJobRequestRequestTypeDef](./type_defs.md#deletepredictorbacktestexportjobrequestrequesttypedef).

Keyword-only arguments:

- `PredictorBacktestExportJobArn`: `str` *(required)*

<a id="delete\_resource\_tree"></a>

### delete_resource_tree

Deletes an entire resource tree.

Type annotations for `session.create_client("forecast").delete_resource_tree`
method.

Boto3 documentation:
[ForecastService.Client.delete_resource_tree](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.delete_resource_tree)

Asynchronous method. Use `await delete_resource_tree(...)` for a synchronous
call.

Arguments mapping described in
[DeleteResourceTreeRequestRequestTypeDef](./type_defs.md#deleteresourcetreerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

<a id="describe\_auto\_predictor"></a>

### describe_auto_predictor

Describes a predictor created using the CreateAutoPredictor operation.

Type annotations for
`session.create_client("forecast").describe_auto_predictor` method.

Boto3 documentation:
[ForecastService.Client.describe_auto_predictor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.describe_auto_predictor)

Asynchronous method. Use `await describe_auto_predictor(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAutoPredictorRequestRequestTypeDef](./type_defs.md#describeautopredictorrequestrequesttypedef).

Keyword-only arguments:

- `PredictorArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAutoPredictorResponseTypeDef](./type_defs.md#describeautopredictorresponsetypedef).

<a id="describe\_dataset"></a>

### describe_dataset

Describes an Amazon Forecast dataset created using the CreateDataset operation.

Type annotations for `session.create_client("forecast").describe_dataset`
method.

Boto3 documentation:
[ForecastService.Client.describe_dataset](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.describe_dataset)

Asynchronous method. Use `await describe_dataset(...)` for a synchronous call.

Arguments mapping described in
[DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef).

Keyword-only arguments:

- `DatasetArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef).

<a id="describe\_dataset\_group"></a>

### describe_dataset_group

Describes a dataset group created using the CreateDatasetGroup operation.

Type annotations for `session.create_client("forecast").describe_dataset_group`
method.

Boto3 documentation:
[ForecastService.Client.describe_dataset_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.describe_dataset_group)

Asynchronous method. Use `await describe_dataset_group(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDatasetGroupRequestRequestTypeDef](./type_defs.md#describedatasetgrouprequestrequesttypedef).

Keyword-only arguments:

- `DatasetGroupArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDatasetGroupResponseTypeDef](./type_defs.md#describedatasetgroupresponsetypedef).

<a id="describe\_dataset\_import\_job"></a>

### describe_dataset_import_job

Describes a dataset import job created using the CreateDatasetImportJob
operation.

Type annotations for
`session.create_client("forecast").describe_dataset_import_job` method.

Boto3 documentation:
[ForecastService.Client.describe_dataset_import_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.describe_dataset_import_job)

Asynchronous method. Use `await describe_dataset_import_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeDatasetImportJobRequestRequestTypeDef](./type_defs.md#describedatasetimportjobrequestrequesttypedef).

Keyword-only arguments:

- `DatasetImportJobArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeDatasetImportJobResponseTypeDef](./type_defs.md#describedatasetimportjobresponsetypedef).

<a id="describe\_explainability"></a>

### describe_explainability

Describes an Explainability resource created using the CreateExplainability
operation.

Type annotations for
`session.create_client("forecast").describe_explainability` method.

Boto3 documentation:
[ForecastService.Client.describe_explainability](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.describe_explainability)

Asynchronous method. Use `await describe_explainability(...)` for a synchronous
call.

Arguments mapping described in
[DescribeExplainabilityRequestRequestTypeDef](./type_defs.md#describeexplainabilityrequestrequesttypedef).

Keyword-only arguments:

- `ExplainabilityArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeExplainabilityResponseTypeDef](./type_defs.md#describeexplainabilityresponsetypedef).

<a id="describe\_explainability\_export"></a>

### describe_explainability_export

Describes an Explainability export created using the CreateExplainabilityExport
operation.

Type annotations for
`session.create_client("forecast").describe_explainability_export` method.

Boto3 documentation:
[ForecastService.Client.describe_explainability_export](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.describe_explainability_export)

Asynchronous method. Use `await describe_explainability_export(...)` for a
synchronous call.

Arguments mapping described in
[DescribeExplainabilityExportRequestRequestTypeDef](./type_defs.md#describeexplainabilityexportrequestrequesttypedef).

Keyword-only arguments:

- `ExplainabilityExportArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeExplainabilityExportResponseTypeDef](./type_defs.md#describeexplainabilityexportresponsetypedef).

<a id="describe\_forecast"></a>

### describe_forecast

Describes a forecast created using the CreateForecast operation.

Type annotations for `session.create_client("forecast").describe_forecast`
method.

Boto3 documentation:
[ForecastService.Client.describe_forecast](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.describe_forecast)

Asynchronous method. Use `await describe_forecast(...)` for a synchronous call.

Arguments mapping described in
[DescribeForecastRequestRequestTypeDef](./type_defs.md#describeforecastrequestrequesttypedef).

Keyword-only arguments:

- `ForecastArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeForecastResponseTypeDef](./type_defs.md#describeforecastresponsetypedef).

<a id="describe\_forecast\_export\_job"></a>

### describe_forecast_export_job

Describes a forecast export job created using the CreateForecastExportJob
operation.

Type annotations for
`session.create_client("forecast").describe_forecast_export_job` method.

Boto3 documentation:
[ForecastService.Client.describe_forecast_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.describe_forecast_export_job)

Asynchronous method. Use `await describe_forecast_export_job(...)` for a
synchronous call.

Arguments mapping described in
[DescribeForecastExportJobRequestRequestTypeDef](./type_defs.md#describeforecastexportjobrequestrequesttypedef).

Keyword-only arguments:

- `ForecastExportJobArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeForecastExportJobResponseTypeDef](./type_defs.md#describeforecastexportjobresponsetypedef).

<a id="describe\_predictor"></a>

### describe_predictor

.

Type annotations for `session.create_client("forecast").describe_predictor`
method.

Boto3 documentation:
[ForecastService.Client.describe_predictor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.describe_predictor)

Asynchronous method. Use `await describe_predictor(...)` for a synchronous
call.

Arguments mapping described in
[DescribePredictorRequestRequestTypeDef](./type_defs.md#describepredictorrequestrequesttypedef).

Keyword-only arguments:

- `PredictorArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribePredictorResponseTypeDef](./type_defs.md#describepredictorresponsetypedef).

<a id="describe\_predictor\_backtest\_export\_job"></a>

### describe_predictor_backtest_export_job

Describes a predictor backtest export job created using the
CreatePredictorBacktestExportJob operation.

Type annotations for
`session.create_client("forecast").describe_predictor_backtest_export_job`
method.

Boto3 documentation:
[ForecastService.Client.describe_predictor_backtest_export_job](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.describe_predictor_backtest_export_job)

Asynchronous method. Use `await describe_predictor_backtest_export_job(...)`
for a synchronous call.

Arguments mapping described in
[DescribePredictorBacktestExportJobRequestRequestTypeDef](./type_defs.md#describepredictorbacktestexportjobrequestrequesttypedef).

Keyword-only arguments:

- `PredictorBacktestExportJobArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribePredictorBacktestExportJobResponseTypeDef](./type_defs.md#describepredictorbacktestexportjobresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("forecast").generate_presigned_url`
method.

Boto3 documentation:
[ForecastService.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_accuracy\_metrics"></a>

### get_accuracy_metrics

Provides metrics on the accuracy of the models that were trained by the
CreatePredictor operation.

Type annotations for `session.create_client("forecast").get_accuracy_metrics`
method.

Boto3 documentation:
[ForecastService.Client.get_accuracy_metrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.get_accuracy_metrics)

Asynchronous method. Use `await get_accuracy_metrics(...)` for a synchronous
call.

Arguments mapping described in
[GetAccuracyMetricsRequestRequestTypeDef](./type_defs.md#getaccuracymetricsrequestrequesttypedef).

Keyword-only arguments:

- `PredictorArn`: `str` *(required)*

Returns a `Coroutine` for
[GetAccuracyMetricsResponseTypeDef](./type_defs.md#getaccuracymetricsresponsetypedef).

<a id="list\_dataset\_groups"></a>

### list_dataset_groups

Returns a list of dataset groups created using the CreateDatasetGroup
operation.

Type annotations for `session.create_client("forecast").list_dataset_groups`
method.

Boto3 documentation:
[ForecastService.Client.list_dataset_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_dataset_groups)

Asynchronous method. Use `await list_dataset_groups(...)` for a synchronous
call.

Arguments mapping described in
[ListDatasetGroupsRequestRequestTypeDef](./type_defs.md#listdatasetgroupsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef).

<a id="list\_dataset\_import\_jobs"></a>

### list_dataset_import_jobs

Returns a list of dataset import jobs created using the CreateDatasetImportJob
operation.

Type annotations for
`session.create_client("forecast").list_dataset_import_jobs` method.

Boto3 documentation:
[ForecastService.Client.list_dataset_import_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_dataset_import_jobs)

Asynchronous method. Use `await list_dataset_import_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListDatasetImportJobsRequestRequestTypeDef](./type_defs.md#listdatasetimportjobsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef).

<a id="list\_datasets"></a>

### list_datasets

Returns a list of datasets created using the CreateDataset operation.

Type annotations for `session.create_client("forecast").list_datasets` method.

Boto3 documentation:
[ForecastService.Client.list_datasets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_datasets)

Asynchronous method. Use `await list_datasets(...)` for a synchronous call.

Arguments mapping described in
[ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef).

<a id="list\_explainabilities"></a>

### list_explainabilities

Returns a list of Explainability resources created using the
CreateExplainability operation.

Type annotations for `session.create_client("forecast").list_explainabilities`
method.

Boto3 documentation:
[ForecastService.Client.list_explainabilities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_explainabilities)

Asynchronous method. Use `await list_explainabilities(...)` for a synchronous
call.

Arguments mapping described in
[ListExplainabilitiesRequestRequestTypeDef](./type_defs.md#listexplainabilitiesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListExplainabilitiesResponseTypeDef](./type_defs.md#listexplainabilitiesresponsetypedef).

<a id="list\_explainability\_exports"></a>

### list_explainability_exports

Returns a list of Explainability exports created using the
CreateExplainabilityExport operation.

Type annotations for
`session.create_client("forecast").list_explainability_exports` method.

Boto3 documentation:
[ForecastService.Client.list_explainability_exports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_explainability_exports)

Asynchronous method. Use `await list_explainability_exports(...)` for a
synchronous call.

Arguments mapping described in
[ListExplainabilityExportsRequestRequestTypeDef](./type_defs.md#listexplainabilityexportsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListExplainabilityExportsResponseTypeDef](./type_defs.md#listexplainabilityexportsresponsetypedef).

<a id="list\_forecast\_export\_jobs"></a>

### list_forecast_export_jobs

Returns a list of forecast export jobs created using the
CreateForecastExportJob operation.

Type annotations for
`session.create_client("forecast").list_forecast_export_jobs` method.

Boto3 documentation:
[ForecastService.Client.list_forecast_export_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_forecast_export_jobs)

Asynchronous method. Use `await list_forecast_export_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListForecastExportJobsRequestRequestTypeDef](./type_defs.md#listforecastexportjobsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListForecastExportJobsResponseTypeDef](./type_defs.md#listforecastexportjobsresponsetypedef).

<a id="list\_forecasts"></a>

### list_forecasts

Returns a list of forecasts created using the CreateForecast operation.

Type annotations for `session.create_client("forecast").list_forecasts` method.

Boto3 documentation:
[ForecastService.Client.list_forecasts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_forecasts)

Asynchronous method. Use `await list_forecasts(...)` for a synchronous call.

Arguments mapping described in
[ListForecastsRequestRequestTypeDef](./type_defs.md#listforecastsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListForecastsResponseTypeDef](./type_defs.md#listforecastsresponsetypedef).

<a id="list\_predictor\_backtest\_export\_jobs"></a>

### list_predictor_backtest_export_jobs

Returns a list of predictor backtest export jobs created using the
CreatePredictorBacktestExportJob operation.

Type annotations for
`session.create_client("forecast").list_predictor_backtest_export_jobs` method.

Boto3 documentation:
[ForecastService.Client.list_predictor_backtest_export_jobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_predictor_backtest_export_jobs)

Asynchronous method. Use `await list_predictor_backtest_export_jobs(...)` for a
synchronous call.

Arguments mapping described in
[ListPredictorBacktestExportJobsRequestRequestTypeDef](./type_defs.md#listpredictorbacktestexportjobsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListPredictorBacktestExportJobsResponseTypeDef](./type_defs.md#listpredictorbacktestexportjobsresponsetypedef).

<a id="list\_predictors"></a>

### list_predictors

Returns a list of predictors created using the CreateAutoPredictor or
CreatePredictor operations.

Type annotations for `session.create_client("forecast").list_predictors`
method.

Boto3 documentation:
[ForecastService.Client.list_predictors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_predictors)

Asynchronous method. Use `await list_predictors(...)` for a synchronous call.

Arguments mapping described in
[ListPredictorsRequestRequestTypeDef](./type_defs.md#listpredictorsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`
- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]

Returns a `Coroutine` for
[ListPredictorsResponseTypeDef](./type_defs.md#listpredictorsresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists the tags for an Amazon Forecast resource.

Type annotations for `session.create_client("forecast").list_tags_for_resource`
method.

Boto3 documentation:
[ForecastService.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="stop\_resource"></a>

### stop_resource

Stops a resource.

Type annotations for `session.create_client("forecast").stop_resource` method.

Boto3 documentation:
[ForecastService.Client.stop_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.stop_resource)

Asynchronous method. Use `await stop_resource(...)` for a synchronous call.

Arguments mapping described in
[StopResourceRequestRequestTypeDef](./type_defs.md#stopresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

<a id="tag\_resource"></a>

### tag_resource

Associates the specified tags to a resource with the specified `resourceArn`.

Type annotations for `session.create_client("forecast").tag_resource` method.

Boto3 documentation:
[ForecastService.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Deletes the specified tags from a resource.

Type annotations for `session.create_client("forecast").untag_resource` method.

Boto3 documentation:
[ForecastService.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_dataset\_group"></a>

### update_dataset_group

Replaces the datasets in a dataset group with the specified datasets.

Type annotations for `session.create_client("forecast").update_dataset_group`
method.

Boto3 documentation:
[ForecastService.Client.update_dataset_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.update_dataset_group)

Asynchronous method. Use `await update_dataset_group(...)` for a synchronous
call.

Arguments mapping described in
[UpdateDatasetGroupRequestRequestTypeDef](./type_defs.md#updatedatasetgrouprequestrequesttypedef).

Keyword-only arguments:

- `DatasetGroupArn`: `str` *(required)*
- `DatasetArns`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("forecast").__aenter__` method.

Boto3 documentation:
[ForecastService.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [ForecastServiceClient](#forecastserviceclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("forecast").__aexit__` method.

Boto3 documentation:
[ForecastService.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("forecast").get_paginator` method
with overloads.

- `client.get_paginator("list_dataset_groups")` ->
  [ListDatasetGroupsPaginator](./paginators.md#listdatasetgroupspaginator)
- `client.get_paginator("list_dataset_import_jobs")` ->
  [ListDatasetImportJobsPaginator](./paginators.md#listdatasetimportjobspaginator)
- `client.get_paginator("list_datasets")` ->
  [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
- `client.get_paginator("list_forecast_export_jobs")` ->
  [ListForecastExportJobsPaginator](./paginators.md#listforecastexportjobspaginator)
- `client.get_paginator("list_forecasts")` ->
  [ListForecastsPaginator](./paginators.md#listforecastspaginator)
- `client.get_paginator("list_predictor_backtest_export_jobs")` ->
  [ListPredictorBacktestExportJobsPaginator](./paginators.md#listpredictorbacktestexportjobspaginator)
- `client.get_paginator("list_predictors")` ->
  [ListPredictorsPaginator](./paginators.md#listpredictorspaginator)
