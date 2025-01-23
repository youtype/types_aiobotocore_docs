# Paginators

> [Index](../README.md) > [MachineLearning](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MachineLearning](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#machinelearning)
    type annotations stubs module [types-aiobotocore-machinelearning](https://pypi.org/project/types-aiobotocore-machinelearning/).

## DescribeBatchPredictionsPaginator

Type annotations and code completion for `#!python session.create_client("machinelearning").get_paginator("describe_batch_predictions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning/paginator/DescribeBatchPredictions.html#MachineLearning.Paginator.DescribeBatchPredictions)

```python
# DescribeBatchPredictionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeBatchPredictionsPaginator

session = get_session()
async with session.create_client("machinelearning") as client:  # (1)
    paginator: DescribeBatchPredictionsPaginator = client.get_paginator("describe_batch_predictions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBatchPredictionsOutputTypeDef
        print(item)  # (3)
```

1. client: [MachineLearningClient](./client.md)
2. paginator: [DescribeBatchPredictionsPaginator](./paginators.md#describebatchpredictionspaginator)
3. item: [:material-code-braces: DescribeBatchPredictionsOutputTypeDef](./type_defs.md#describebatchpredictionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeBatchPredictionsPaginator.paginate` method.

```python
# paginate method definition

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
) -> AioPageIterator[DescribeBatchPredictionsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: BatchPredictionFilterVariableType](./literals.md#batchpredictionfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeBatchPredictionsOutputTypeDef](./type_defs.md#describebatchpredictionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBatchPredictionsInputPaginateTypeDef = {  # (1)
    "FilterVariable": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBatchPredictionsInputPaginateTypeDef](./type_defs.md#describebatchpredictionsinputpaginatetypedef) 
## DescribeDataSourcesPaginator

Type annotations and code completion for `#!python session.create_client("machinelearning").get_paginator("describe_data_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning/paginator/DescribeDataSources.html#MachineLearning.Paginator.DescribeDataSources)

```python
# DescribeDataSourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeDataSourcesPaginator

session = get_session()
async with session.create_client("machinelearning") as client:  # (1)
    paginator: DescribeDataSourcesPaginator = client.get_paginator("describe_data_sources")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDataSourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [MachineLearningClient](./client.md)
2. paginator: [DescribeDataSourcesPaginator](./paginators.md#describedatasourcespaginator)
3. item: [:material-code-braces: DescribeDataSourcesOutputTypeDef](./type_defs.md#describedatasourcesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDataSourcesPaginator.paginate` method.

```python
# paginate method definition

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
) -> AioPageIterator[DescribeDataSourcesOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: DataSourceFilterVariableType](./literals.md#datasourcefiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeDataSourcesOutputTypeDef](./type_defs.md#describedatasourcesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDataSourcesInputPaginateTypeDef = {  # (1)
    "FilterVariable": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDataSourcesInputPaginateTypeDef](./type_defs.md#describedatasourcesinputpaginatetypedef) 
## DescribeEvaluationsPaginator

Type annotations and code completion for `#!python session.create_client("machinelearning").get_paginator("describe_evaluations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning/paginator/DescribeEvaluations.html#MachineLearning.Paginator.DescribeEvaluations)

```python
# DescribeEvaluationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeEvaluationsPaginator

session = get_session()
async with session.create_client("machinelearning") as client:  # (1)
    paginator: DescribeEvaluationsPaginator = client.get_paginator("describe_evaluations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEvaluationsOutputTypeDef
        print(item)  # (3)
```

1. client: [MachineLearningClient](./client.md)
2. paginator: [DescribeEvaluationsPaginator](./paginators.md#describeevaluationspaginator)
3. item: [:material-code-braces: DescribeEvaluationsOutputTypeDef](./type_defs.md#describeevaluationsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEvaluationsPaginator.paginate` method.

```python
# paginate method definition

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
) -> AioPageIterator[DescribeEvaluationsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: EvaluationFilterVariableType](./literals.md#evaluationfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeEvaluationsOutputTypeDef](./type_defs.md#describeevaluationsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEvaluationsInputPaginateTypeDef = {  # (1)
    "FilterVariable": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEvaluationsInputPaginateTypeDef](./type_defs.md#describeevaluationsinputpaginatetypedef) 
## DescribeMLModelsPaginator

Type annotations and code completion for `#!python session.create_client("machinelearning").get_paginator("describe_ml_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning/paginator/DescribeMLModels.html#MachineLearning.Paginator.DescribeMLModels)

```python
# DescribeMLModelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_machinelearning.paginator import DescribeMLModelsPaginator

session = get_session()
async with session.create_client("machinelearning") as client:  # (1)
    paginator: DescribeMLModelsPaginator = client.get_paginator("describe_ml_models")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMLModelsOutputTypeDef
        print(item)  # (3)
```

1. client: [MachineLearningClient](./client.md)
2. paginator: [DescribeMLModelsPaginator](./paginators.md#describemlmodelspaginator)
3. item: [:material-code-braces: DescribeMLModelsOutputTypeDef](./type_defs.md#describemlmodelsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeMLModelsPaginator.paginate` method.

```python
# paginate method definition

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
) -> AioPageIterator[DescribeMLModelsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: MLModelFilterVariableType](./literals.md#mlmodelfiltervariabletype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeMLModelsOutputTypeDef](./type_defs.md#describemlmodelsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeMLModelsInputPaginateTypeDef = {  # (1)
    "FilterVariable": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMLModelsInputPaginateTypeDef](./type_defs.md#describemlmodelsinputpaginatetypedef) 
