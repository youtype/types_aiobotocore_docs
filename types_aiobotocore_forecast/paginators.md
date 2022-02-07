<a id="paginators-for-aiobotocore-forecastservice-module"></a>

# Paginators for aiobotocore ForecastService module

> [Index](..) > [ForecastService](.) > Paginators

Auto-generated documentation for
[ForecastService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
type annotations stubs module
[types-aiobotocore-forecast](https://pypi.org/project/types-aiobotocore-forecast/).

- [Paginators for aiobotocore ForecastService module](#paginators-for-aiobotocore-forecastservice-module)
  - [ListDatasetGroupsPaginator](#listdatasetgroupspaginator)
  - [ListDatasetImportJobsPaginator](#listdatasetimportjobspaginator)
  - [ListDatasetsPaginator](#listdatasetspaginator)
  - [ListForecastExportJobsPaginator](#listforecastexportjobspaginator)
  - [ListForecastsPaginator](#listforecastspaginator)
  - [ListPredictorBacktestExportJobsPaginator](#listpredictorbacktestexportjobspaginator)
  - [ListPredictorsPaginator](#listpredictorspaginator)

<a id="listdatasetgroupspaginator"></a>

## ListDatasetGroupsPaginator

Type annotations for
`session.create_client("forecast").get_paginator("list_dataset_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListDatasetGroupsPaginator

session = get_session()
async with session.create_client("forecast") as client:
    client: ForecastServiceClient
    paginator: ListDatasetGroupsPaginator = client.get_paginator("list_dataset_groups")
```

Boto3 documentation:
[ForecastService.Paginator.ListDatasetGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups)

Arguments for `ListDatasetGroupsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetGroupsPaginator.paginate` returns
`_PageIterator`\[[ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef)\].

<a id="listdatasetimportjobspaginator"></a>

## ListDatasetImportJobsPaginator

Type annotations for
`session.create_client("forecast").get_paginator("list_dataset_import_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListDatasetImportJobsPaginator

session = get_session()
async with session.create_client("forecast") as client:
    client: ForecastServiceClient
    paginator: ListDatasetImportJobsPaginator = client.get_paginator("list_dataset_import_jobs")
```

Boto3 documentation:
[ForecastService.Paginator.ListDatasetImportJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs)

Arguments for `ListDatasetImportJobsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetImportJobsPaginator.paginate` returns
`_PageIterator`\[[ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef)\].

<a id="listdatasetspaginator"></a>

## ListDatasetsPaginator

Type annotations for
`session.create_client("forecast").get_paginator("list_datasets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("forecast") as client:
    client: ForecastServiceClient
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
```

Boto3 documentation:
[ForecastService.Paginator.ListDatasets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets)

Arguments for `ListDatasetsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetsPaginator.paginate` returns
`_PageIterator`\[[ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)\].

<a id="listforecastexportjobspaginator"></a>

## ListForecastExportJobsPaginator

Type annotations for
`session.create_client("forecast").get_paginator("list_forecast_export_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListForecastExportJobsPaginator

session = get_session()
async with session.create_client("forecast") as client:
    client: ForecastServiceClient
    paginator: ListForecastExportJobsPaginator = client.get_paginator("list_forecast_export_jobs")
```

Boto3 documentation:
[ForecastService.Paginator.ListForecastExportJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs)

Arguments for `ListForecastExportJobsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListForecastExportJobsPaginator.paginate` returns
`_PageIterator`\[[ListForecastExportJobsResponseTypeDef](./type_defs.md#listforecastexportjobsresponsetypedef)\].

<a id="listforecastspaginator"></a>

## ListForecastsPaginator

Type annotations for
`session.create_client("forecast").get_paginator("list_forecasts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListForecastsPaginator

session = get_session()
async with session.create_client("forecast") as client:
    client: ForecastServiceClient
    paginator: ListForecastsPaginator = client.get_paginator("list_forecasts")
```

Boto3 documentation:
[ForecastService.Paginator.ListForecasts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts)

Arguments for `ListForecastsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListForecastsPaginator.paginate` returns
`_PageIterator`\[[ListForecastsResponseTypeDef](./type_defs.md#listforecastsresponsetypedef)\].

<a id="listpredictorbacktestexportjobspaginator"></a>

## ListPredictorBacktestExportJobsPaginator

Type annotations for
`session.create_client("forecast").get_paginator("list_predictor_backtest_export_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListPredictorBacktestExportJobsPaginator

session = get_session()
async with session.create_client("forecast") as client:
    client: ForecastServiceClient
    paginator: ListPredictorBacktestExportJobsPaginator = client.get_paginator("list_predictor_backtest_export_jobs")
```

Boto3 documentation:
[ForecastService.Paginator.ListPredictorBacktestExportJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs)

Arguments for `ListPredictorBacktestExportJobsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPredictorBacktestExportJobsPaginator.paginate` returns
`_PageIterator`\[[ListPredictorBacktestExportJobsResponseTypeDef](./type_defs.md#listpredictorbacktestexportjobsresponsetypedef)\].

<a id="listpredictorspaginator"></a>

## ListPredictorsPaginator

Type annotations for
`session.create_client("forecast").get_paginator("list_predictors")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListPredictorsPaginator

session = get_session()
async with session.create_client("forecast") as client:
    client: ForecastServiceClient
    paginator: ListPredictorsPaginator = client.get_paginator("list_predictors")
```

Boto3 documentation:
[ForecastService.Paginator.ListPredictors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors)

Arguments for `ListPredictorsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPredictorsPaginator.paginate` returns
`_PageIterator`\[[ListPredictorsResponseTypeDef](./type_defs.md#listpredictorsresponsetypedef)\].
