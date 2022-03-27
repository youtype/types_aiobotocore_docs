# Paginators

> [Index](../README.md) > [MachineLearning](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MachineLearning](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
    type annotations stubs module [types-aiobotocore-machinelearning](https://pypi.org/project/types-aiobotocore-machinelearning/).

## DescribeBatchPredictionsPaginator

Type annotations and code completion for `#!python session.create_client("machinelearning").get_paginator("describe_batch_predictions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeBatchPredictions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeBatchPredictionsPaginator

session = get_session()
async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    paginator: DescribeBatchPredictionsPaginator = client.get_paginator("describe_batch_predictions")
```


### paginate

Type annotations and code completion for `#!python DescribeBatchPredictionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    FilterVariable: BatchPredictionFilterVariableType = ...,  # (1)
    EQ: str = ...,
    GT: str = ...,
    LT: str = ...,
    GE: str = ...,
    LE: str = ...,
    NE: str = ...,
    Prefix: str = ...,
    SortOrder: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeBatchPredictionsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: BatchPredictionFilterVariableType](./literals.md#batchpredictionfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeBatchPredictionsOutputTypeDef](./type_defs.md#describebatchpredictionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = {  # (1)
    "FilterVariable": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef](./type_defs.md#describebatchpredictionsinputdescribebatchpredictionspaginatetypedef) 
## DescribeDataSourcesPaginator

Type annotations and code completion for `#!python session.create_client("machinelearning").get_paginator("describe_data_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeDataSources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeDataSourcesPaginator

session = get_session()
async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    paginator: DescribeDataSourcesPaginator = client.get_paginator("describe_data_sources")
```


### paginate

Type annotations and code completion for `#!python DescribeDataSourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    FilterVariable: DataSourceFilterVariableType = ...,  # (1)
    EQ: str = ...,
    GT: str = ...,
    LT: str = ...,
    GE: str = ...,
    LE: str = ...,
    NE: str = ...,
    Prefix: str = ...,
    SortOrder: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeDataSourcesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: DataSourceFilterVariableType](./literals.md#datasourcefiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeDataSourcesOutputTypeDef](./type_defs.md#describedatasourcesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = {  # (1)
    "FilterVariable": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef](./type_defs.md#describedatasourcesinputdescribedatasourcespaginatetypedef) 
## DescribeEvaluationsPaginator

Type annotations and code completion for `#!python session.create_client("machinelearning").get_paginator("describe_evaluations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeEvaluations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeEvaluationsPaginator

session = get_session()
async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    paginator: DescribeEvaluationsPaginator = client.get_paginator("describe_evaluations")
```


### paginate

Type annotations and code completion for `#!python DescribeEvaluationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    FilterVariable: EvaluationFilterVariableType = ...,  # (1)
    EQ: str = ...,
    GT: str = ...,
    LT: str = ...,
    GE: str = ...,
    LE: str = ...,
    NE: str = ...,
    Prefix: str = ...,
    SortOrder: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeEvaluationsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: EvaluationFilterVariableType](./literals.md#evaluationfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeEvaluationsOutputTypeDef](./type_defs.md#describeevaluationsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = {  # (1)
    "FilterVariable": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef](./type_defs.md#describeevaluationsinputdescribeevaluationspaginatetypedef) 
## DescribeMLModelsPaginator

Type annotations and code completion for `#!python session.create_client("machinelearning").get_paginator("describe_ml_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeMLModels)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeMLModelsPaginator

session = get_session()
async with session.create_client("machinelearning") as client:
    client: MachineLearningClient
    paginator: DescribeMLModelsPaginator = client.get_paginator("describe_ml_models")
```


### paginate

Type annotations and code completion for `#!python DescribeMLModelsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    FilterVariable: MLModelFilterVariableType = ...,  # (1)
    EQ: str = ...,
    GT: str = ...,
    LT: str = ...,
    GE: str = ...,
    LE: str = ...,
    NE: str = ...,
    Prefix: str = ...,
    SortOrder: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeMLModelsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: MLModelFilterVariableType](./literals.md#mlmodelfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeMLModelsOutputTypeDef](./type_defs.md#describemlmodelsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = {  # (1)
    "FilterVariable": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMLModelsInputDescribeMLModelsPaginateTypeDef](./type_defs.md#describemlmodelsinputdescribemlmodelspaginatetypedef) 
