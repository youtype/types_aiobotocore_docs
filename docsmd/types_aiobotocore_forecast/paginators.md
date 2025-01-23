# Paginators

> [Index](../README.md) > [ForecastService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ForecastService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#forecastservice)
    type annotations stubs module [types-aiobotocore-forecast](https://pypi.org/project/types-aiobotocore-forecast/).

## ListDatasetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_dataset_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListDatasetGroups.html#ForecastService.Paginator.ListDatasetGroups)

```python
# ListDatasetGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListDatasetGroupsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListDatasetGroupsPaginator = client.get_paginator("list_dataset_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListDatasetGroupsPaginator](./paginators.md#listdatasetgroupspaginator)
3. item: [:material-code-braces: ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDatasetGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetGroupsResponseTypeDef](./type_defs.md#listdatasetgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetGroupsRequestPaginateTypeDef](./type_defs.md#listdatasetgroupsrequestpaginatetypedef) 
## ListDatasetImportJobsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_dataset_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListDatasetImportJobs.html#ForecastService.Paginator.ListDatasetImportJobs)

```python
# ListDatasetImportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListDatasetImportJobsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListDatasetImportJobsPaginator = client.get_paginator("list_dataset_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListDatasetImportJobsPaginator](./paginators.md#listdatasetimportjobspaginator)
3. item: [:material-code-braces: ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetImportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDatasetImportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDatasetImportJobsResponseTypeDef](./type_defs.md#listdatasetimportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetImportJobsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetImportJobsRequestPaginateTypeDef](./type_defs.md#listdatasetimportjobsrequestpaginatetypedef) 
## ListDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListDatasets.html#ForecastService.Paginator.ListDatasets)

```python
# ListDatasetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef) 
## ListExplainabilitiesPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_explainabilities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListExplainabilities.html#ForecastService.Paginator.ListExplainabilities)

```python
# ListExplainabilitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListExplainabilitiesPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListExplainabilitiesPaginator = client.get_paginator("list_explainabilities")  # (2)
    async for item in paginator.paginate(...):
        item: ListExplainabilitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListExplainabilitiesPaginator](./paginators.md#listexplainabilitiespaginator)
3. item: [:material-code-braces: ListExplainabilitiesResponseTypeDef](./type_defs.md#listexplainabilitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExplainabilitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListExplainabilitiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListExplainabilitiesResponseTypeDef](./type_defs.md#listexplainabilitiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExplainabilitiesRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExplainabilitiesRequestPaginateTypeDef](./type_defs.md#listexplainabilitiesrequestpaginatetypedef) 
## ListExplainabilityExportsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_explainability_exports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListExplainabilityExports.html#ForecastService.Paginator.ListExplainabilityExports)

```python
# ListExplainabilityExportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListExplainabilityExportsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListExplainabilityExportsPaginator = client.get_paginator("list_explainability_exports")  # (2)
    async for item in paginator.paginate(...):
        item: ListExplainabilityExportsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListExplainabilityExportsPaginator](./paginators.md#listexplainabilityexportspaginator)
3. item: [:material-code-braces: ListExplainabilityExportsResponseTypeDef](./type_defs.md#listexplainabilityexportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExplainabilityExportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListExplainabilityExportsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListExplainabilityExportsResponseTypeDef](./type_defs.md#listexplainabilityexportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExplainabilityExportsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExplainabilityExportsRequestPaginateTypeDef](./type_defs.md#listexplainabilityexportsrequestpaginatetypedef) 
## ListForecastExportJobsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_forecast_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListForecastExportJobs.html#ForecastService.Paginator.ListForecastExportJobs)

```python
# ListForecastExportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListForecastExportJobsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListForecastExportJobsPaginator = client.get_paginator("list_forecast_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListForecastExportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListForecastExportJobsPaginator](./paginators.md#listforecastexportjobspaginator)
3. item: [:material-code-braces: ListForecastExportJobsResponseTypeDef](./type_defs.md#listforecastexportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListForecastExportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListForecastExportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListForecastExportJobsResponseTypeDef](./type_defs.md#listforecastexportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListForecastExportJobsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListForecastExportJobsRequestPaginateTypeDef](./type_defs.md#listforecastexportjobsrequestpaginatetypedef) 
## ListForecastsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_forecasts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListForecasts.html#ForecastService.Paginator.ListForecasts)

```python
# ListForecastsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListForecastsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListForecastsPaginator = client.get_paginator("list_forecasts")  # (2)
    async for item in paginator.paginate(...):
        item: ListForecastsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListForecastsPaginator](./paginators.md#listforecastspaginator)
3. item: [:material-code-braces: ListForecastsResponseTypeDef](./type_defs.md#listforecastsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListForecastsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListForecastsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListForecastsResponseTypeDef](./type_defs.md#listforecastsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListForecastsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListForecastsRequestPaginateTypeDef](./type_defs.md#listforecastsrequestpaginatetypedef) 
## ListMonitorEvaluationsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_monitor_evaluations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListMonitorEvaluations.html#ForecastService.Paginator.ListMonitorEvaluations)

```python
# ListMonitorEvaluationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListMonitorEvaluationsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListMonitorEvaluationsPaginator = client.get_paginator("list_monitor_evaluations")  # (2)
    async for item in paginator.paginate(...):
        item: ListMonitorEvaluationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListMonitorEvaluationsPaginator](./paginators.md#listmonitorevaluationspaginator)
3. item: [:material-code-braces: ListMonitorEvaluationsResponseTypeDef](./type_defs.md#listmonitorevaluationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMonitorEvaluationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    MonitorArn: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListMonitorEvaluationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListMonitorEvaluationsResponseTypeDef](./type_defs.md#listmonitorevaluationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMonitorEvaluationsRequestPaginateTypeDef = {  # (1)
    "MonitorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMonitorEvaluationsRequestPaginateTypeDef](./type_defs.md#listmonitorevaluationsrequestpaginatetypedef) 
## ListMonitorsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_monitors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListMonitors.html#ForecastService.Paginator.ListMonitors)

```python
# ListMonitorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListMonitorsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListMonitorsPaginator = client.get_paginator("list_monitors")  # (2)
    async for item in paginator.paginate(...):
        item: ListMonitorsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)
3. item: [:material-code-braces: ListMonitorsResponseTypeDef](./type_defs.md#listmonitorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMonitorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListMonitorsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListMonitorsResponseTypeDef](./type_defs.md#listmonitorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMonitorsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMonitorsRequestPaginateTypeDef](./type_defs.md#listmonitorsrequestpaginatetypedef) 
## ListPredictorBacktestExportJobsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_predictor_backtest_export_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListPredictorBacktestExportJobs.html#ForecastService.Paginator.ListPredictorBacktestExportJobs)

```python
# ListPredictorBacktestExportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListPredictorBacktestExportJobsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListPredictorBacktestExportJobsPaginator = client.get_paginator("list_predictor_backtest_export_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListPredictorBacktestExportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListPredictorBacktestExportJobsPaginator](./paginators.md#listpredictorbacktestexportjobspaginator)
3. item: [:material-code-braces: ListPredictorBacktestExportJobsResponseTypeDef](./type_defs.md#listpredictorbacktestexportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPredictorBacktestExportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListPredictorBacktestExportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPredictorBacktestExportJobsResponseTypeDef](./type_defs.md#listpredictorbacktestexportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPredictorBacktestExportJobsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPredictorBacktestExportJobsRequestPaginateTypeDef](./type_defs.md#listpredictorbacktestexportjobsrequestpaginatetypedef) 
## ListPredictorsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_predictors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListPredictors.html#ForecastService.Paginator.ListPredictors)

```python
# ListPredictorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListPredictorsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListPredictorsPaginator = client.get_paginator("list_predictors")  # (2)
    async for item in paginator.paginate(...):
        item: ListPredictorsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListPredictorsPaginator](./paginators.md#listpredictorspaginator)
3. item: [:material-code-braces: ListPredictorsResponseTypeDef](./type_defs.md#listpredictorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPredictorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListPredictorsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPredictorsResponseTypeDef](./type_defs.md#listpredictorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPredictorsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPredictorsRequestPaginateTypeDef](./type_defs.md#listpredictorsrequestpaginatetypedef) 
## ListWhatIfAnalysesPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_what_if_analyses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListWhatIfAnalyses.html#ForecastService.Paginator.ListWhatIfAnalyses)

```python
# ListWhatIfAnalysesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListWhatIfAnalysesPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListWhatIfAnalysesPaginator = client.get_paginator("list_what_if_analyses")  # (2)
    async for item in paginator.paginate(...):
        item: ListWhatIfAnalysesResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListWhatIfAnalysesPaginator](./paginators.md#listwhatifanalysespaginator)
3. item: [:material-code-braces: ListWhatIfAnalysesResponseTypeDef](./type_defs.md#listwhatifanalysesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWhatIfAnalysesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListWhatIfAnalysesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWhatIfAnalysesResponseTypeDef](./type_defs.md#listwhatifanalysesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWhatIfAnalysesRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWhatIfAnalysesRequestPaginateTypeDef](./type_defs.md#listwhatifanalysesrequestpaginatetypedef) 
## ListWhatIfForecastExportsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_what_if_forecast_exports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListWhatIfForecastExports.html#ForecastService.Paginator.ListWhatIfForecastExports)

```python
# ListWhatIfForecastExportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListWhatIfForecastExportsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListWhatIfForecastExportsPaginator = client.get_paginator("list_what_if_forecast_exports")  # (2)
    async for item in paginator.paginate(...):
        item: ListWhatIfForecastExportsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListWhatIfForecastExportsPaginator](./paginators.md#listwhatifforecastexportspaginator)
3. item: [:material-code-braces: ListWhatIfForecastExportsResponseTypeDef](./type_defs.md#listwhatifforecastexportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWhatIfForecastExportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListWhatIfForecastExportsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWhatIfForecastExportsResponseTypeDef](./type_defs.md#listwhatifforecastexportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWhatIfForecastExportsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWhatIfForecastExportsRequestPaginateTypeDef](./type_defs.md#listwhatifforecastexportsrequestpaginatetypedef) 
## ListWhatIfForecastsPaginator

Type annotations and code completion for `#!python session.create_client("forecast").get_paginator("list_what_if_forecasts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast/paginator/ListWhatIfForecasts.html#ForecastService.Paginator.ListWhatIfForecasts)

```python
# ListWhatIfForecastsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_forecast.paginator import ListWhatIfForecastsPaginator

session = get_session()
async with session.create_client("forecast") as client:  # (1)
    paginator: ListWhatIfForecastsPaginator = client.get_paginator("list_what_if_forecasts")  # (2)
    async for item in paginator.paginate(...):
        item: ListWhatIfForecastsResponseTypeDef
        print(item)  # (3)
```

1. client: [ForecastServiceClient](./client.md)
2. paginator: [ListWhatIfForecastsPaginator](./paginators.md#listwhatifforecastspaginator)
3. item: [:material-code-braces: ListWhatIfForecastsResponseTypeDef](./type_defs.md#listwhatifforecastsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListWhatIfForecastsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListWhatIfForecastsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListWhatIfForecastsResponseTypeDef](./type_defs.md#listwhatifforecastsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListWhatIfForecastsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWhatIfForecastsRequestPaginateTypeDef](./type_defs.md#listwhatifforecastsrequestpaginatetypedef) 
