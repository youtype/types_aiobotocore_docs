<a id="paginators-for-aiobotocore-machinelearning-module"></a>

# Paginators for aiobotocore MachineLearning module

> [Index](../README.md) > [MachineLearning](./README.md) > Paginators

Auto-generated documentation for
[MachineLearning](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
type annotations stubs module
[types-aiobotocore-machinelearning](https://pypi.org/project/types-aiobotocore-machinelearning/).

- [Paginators for aiobotocore MachineLearning module](#paginators-for-aiobotocore-machinelearning-module)
  - [DescribeBatchPredictionsPaginator](#describebatchpredictionspaginator)
  - [DescribeDataSourcesPaginator](#describedatasourcespaginator)
  - [DescribeEvaluationsPaginator](#describeevaluationspaginator)
  - [DescribeMLModelsPaginator](#describemlmodelspaginator)

<a id="describebatchpredictionspaginator"></a>

## DescribeBatchPredictionsPaginator

Type annotations for
`session.create_client("machinelearning").get_paginator("describe_batch_predictions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeBatchPredictionsPaginator

session = get_session()
async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    paginator: DescribeBatchPredictionsPaginator = client.get_paginator("describe_batch_predictions")
```

Boto3 documentation:
[MachineLearning.Paginator.DescribeBatchPredictions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeBatchPredictions)

Arguments for `DescribeBatchPredictionsPaginator.paginate` method:

- `FilterVariable`:
  [BatchPredictionFilterVariableType](./literals.md#batchpredictionfiltervariabletype)
- `EQ`: `str`
- `GT`: `str`
- `LT`: `str`
- `GE`: `str`
- `LE`: `str`
- `NE`: `str`
- `Prefix`: `str`
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeBatchPredictionsPaginator.paginate` returns
`AsyncIterator`\[[DescribeBatchPredictionsOutputTypeDef](./type_defs.md#describebatchpredictionsoutputtypedef)\].

<a id="describedatasourcespaginator"></a>

## DescribeDataSourcesPaginator

Type annotations for
`session.create_client("machinelearning").get_paginator("describe_data_sources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeDataSourcesPaginator

session = get_session()
async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    paginator: DescribeDataSourcesPaginator = client.get_paginator("describe_data_sources")
```

Boto3 documentation:
[MachineLearning.Paginator.DescribeDataSources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeDataSources)

Arguments for `DescribeDataSourcesPaginator.paginate` method:

- `FilterVariable`:
  [DataSourceFilterVariableType](./literals.md#datasourcefiltervariabletype)
- `EQ`: `str`
- `GT`: `str`
- `LT`: `str`
- `GE`: `str`
- `LE`: `str`
- `NE`: `str`
- `Prefix`: `str`
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDataSourcesPaginator.paginate` returns
`AsyncIterator`\[[DescribeDataSourcesOutputTypeDef](./type_defs.md#describedatasourcesoutputtypedef)\].

<a id="describeevaluationspaginator"></a>

## DescribeEvaluationsPaginator

Type annotations for
`session.create_client("machinelearning").get_paginator("describe_evaluations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeEvaluationsPaginator

session = get_session()
async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    paginator: DescribeEvaluationsPaginator = client.get_paginator("describe_evaluations")
```

Boto3 documentation:
[MachineLearning.Paginator.DescribeEvaluations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeEvaluations)

Arguments for `DescribeEvaluationsPaginator.paginate` method:

- `FilterVariable`:
  [EvaluationFilterVariableType](./literals.md#evaluationfiltervariabletype)
- `EQ`: `str`
- `GT`: `str`
- `LT`: `str`
- `GE`: `str`
- `LE`: `str`
- `NE`: `str`
- `Prefix`: `str`
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEvaluationsPaginator.paginate` returns
`AsyncIterator`\[[DescribeEvaluationsOutputTypeDef](./type_defs.md#describeevaluationsoutputtypedef)\].

<a id="describemlmodelspaginator"></a>

## DescribeMLModelsPaginator

Type annotations for
`session.create_client("machinelearning").get_paginator("describe_ml_models")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeMLModelsPaginator

session = get_session()
async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    paginator: DescribeMLModelsPaginator = client.get_paginator("describe_ml_models")
```

Boto3 documentation:
[MachineLearning.Paginator.DescribeMLModels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeMLModels)

Arguments for `DescribeMLModelsPaginator.paginate` method:

- `FilterVariable`:
  [MLModelFilterVariableType](./literals.md#mlmodelfiltervariabletype)
- `EQ`: `str`
- `GT`: `str`
- `LT`: `str`
- `GE`: `str`
- `LE`: `str`
- `NE`: `str`
- `Prefix`: `str`
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeMLModelsPaginator.paginate` returns
`AsyncIterator`\[[DescribeMLModelsOutputTypeDef](./type_defs.md#describemlmodelsoutputtypedef)\].
