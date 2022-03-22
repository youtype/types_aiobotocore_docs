<a id="waiters-for-aiobotocore-machinelearning-module"></a>

# Waiters for aiobotocore MachineLearning module

> [Index](../README.md) > [MachineLearning](./README.md) > Waiters

Auto-generated documentation for
[MachineLearning](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
type annotations stubs module
[types-aiobotocore-machinelearning](https://pypi.org/project/types-aiobotocore-machinelearning/).

- [Waiters for aiobotocore MachineLearning module](#waiters-for-aiobotocore-machinelearning-module)
  - [BatchPredictionAvailableWaiter](#batchpredictionavailablewaiter)
  - [DataSourceAvailableWaiter](#datasourceavailablewaiter)
  - [EvaluationAvailableWaiter](#evaluationavailablewaiter)
  - [MLModelAvailableWaiter](#mlmodelavailablewaiter)

<a id="batchpredictionavailablewaiter"></a>

## BatchPredictionAvailableWaiter

Type annotations for
`session.create_client("machinelearning").get_waiter("batch_prediction_available")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_machinelearning.waiter import BatchPredictionAvailableWaiter

def get_batch_prediction_available_waiter() -> BatchPredictionAvailableWaiter:
    return Session().client("machinelearning").get_waiter("batch_prediction_available")
```

Boto3 documentation:
[MachineLearning.Waiter.batch_prediction_available](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.BatchPredictionAvailable)

Arguments for `BatchPredictionAvailableWaiter.wait` method:

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
- `NextToken`: `str`
- `Limit`: `int`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="datasourceavailablewaiter"></a>

## DataSourceAvailableWaiter

Type annotations for
`session.create_client("machinelearning").get_waiter("data_source_available")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_machinelearning.waiter import DataSourceAvailableWaiter

def get_data_source_available_waiter() -> DataSourceAvailableWaiter:
    return Session().client("machinelearning").get_waiter("data_source_available")
```

Boto3 documentation:
[MachineLearning.Waiter.data_source_available](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.DataSourceAvailable)

Arguments for `DataSourceAvailableWaiter.wait` method:

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
- `NextToken`: `str`
- `Limit`: `int`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="evaluationavailablewaiter"></a>

## EvaluationAvailableWaiter

Type annotations for
`session.create_client("machinelearning").get_waiter("evaluation_available")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_machinelearning.waiter import EvaluationAvailableWaiter

def get_evaluation_available_waiter() -> EvaluationAvailableWaiter:
    return Session().client("machinelearning").get_waiter("evaluation_available")
```

Boto3 documentation:
[MachineLearning.Waiter.evaluation_available](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.EvaluationAvailable)

Arguments for `EvaluationAvailableWaiter.wait` method:

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
- `NextToken`: `str`
- `Limit`: `int`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="mlmodelavailablewaiter"></a>

## MLModelAvailableWaiter

Type annotations for
`session.create_client("machinelearning").get_waiter("ml_model_available")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_machinelearning.waiter import MLModelAvailableWaiter

def get_ml_model_available_waiter() -> MLModelAvailableWaiter:
    return Session().client("machinelearning").get_waiter("ml_model_available")
```

Boto3 documentation:
[MachineLearning.Waiter.ml_model_available](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.MLModelAvailable)

Arguments for `MLModelAvailableWaiter.wait` method:

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
- `NextToken`: `str`
- `Limit`: `int`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
