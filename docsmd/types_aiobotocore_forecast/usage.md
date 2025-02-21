# Examples

> [Index](../README.md) > [ForecastService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ForecastService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#forecastservice)
    type annotations stubs module [types-aiobotocore-forecast](https://pypi.org/project/types-aiobotocore-forecast/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[forecast]` package installed.

Write your `ForecastService` code as usual,
type checking and code completion should work out of the box.



```python
# ForecastServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("forecast") as client:  # (1)
    result = await client.create_auto_predictor()  # (2)
```

1. client: [ForecastServiceClient](./client.md)
2. result: [:material-code-braces: CreateAutoPredictorResponseTypeDef](./type_defs.md#createautopredictorresponsetypedef) 



```python
# ListDatasetGroupsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("forecast") as client:  # (1)
    paginator = client.get_paginator("list_dataset_groups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListDatasetGroupsPaginator](./paginators.md#listdatasetgroupspaginator)
3. item: [:material-code-braces: ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[forecast]`
or a standalone `types_aiobotocore_forecast` package, you have to explicitly specify
`client: ForecastServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ForecastServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_forecast.client import ForecastServiceClient
from types_aiobotocore_forecast.type_defs import CreateAutoPredictorResponseTypeDef
from types_aiobotocore_forecast.type_defs import CreateAutoPredictorRequestTypeDef


session = get_session()

async with session.create_client("forecast") as client:
    client: ForecastServiceClient
    kwargs: CreateAutoPredictorRequestTypeDef = {...}
    result: CreateAutoPredictorResponseTypeDef = await client.create_auto_predictor(**kwargs)
```



```python
# ListDatasetGroupsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_forecast.client import ForecastServiceClient
from types_aiobotocore_forecast.paginator import ListDatasetGroupsPaginator
from types_aiobotocore_forecast.type_defs import ListDatasetGroupsResponseTypeDef


session = get_session()

async with session.create_client("forecast") as client:
    client: ForecastServiceClient
    paginator: ListDatasetGroupsPaginator = client.get_paginator("list_dataset_groups")
    async for item in paginator.paginate(...):
        item: ListDatasetGroupsResponseTypeDef
        print(item)
```


