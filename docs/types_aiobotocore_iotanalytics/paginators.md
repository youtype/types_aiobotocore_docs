<a id="paginators-for-aiobotocore-iotanalytics-module"></a>

# Paginators for aiobotocore IoTAnalytics module

> [Index](../README.md) > [IoTAnalytics](./README.md) > Paginators

Auto-generated documentation for
[IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
type annotations stubs module
[types-aiobotocore-iotanalytics](https://pypi.org/project/types-aiobotocore-iotanalytics/).

- [Paginators for aiobotocore IoTAnalytics module](#paginators-for-aiobotocore-iotanalytics-module)
  - [ListChannelsPaginator](#listchannelspaginator)
  - [ListDatasetContentsPaginator](#listdatasetcontentspaginator)
  - [ListDatasetsPaginator](#listdatasetspaginator)
  - [ListDatastoresPaginator](#listdatastorespaginator)
  - [ListPipelinesPaginator](#listpipelinespaginator)

<a id="listchannelspaginator"></a>

## ListChannelsPaginator

Type annotations for
`session.create_client("iotanalytics").get_paginator("list_channels")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("iotanalytics") as client:
    client: IoTAnalyticsClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
```

Boto3 documentation:
[IoTAnalytics.Paginator.ListChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels)

Arguments for `ListChannelsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListChannelsPaginator.paginate` returns
`AsyncIterator`\[[ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)\].

<a id="listdatasetcontentspaginator"></a>

## ListDatasetContentsPaginator

Type annotations for
`session.create_client("iotanalytics").get_paginator("list_dataset_contents")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.paginator import ListDatasetContentsPaginator

session = get_session()
async with session.create_client("iotanalytics") as client:
    client: IoTAnalyticsClient
    paginator: ListDatasetContentsPaginator = client.get_paginator("list_dataset_contents")
```

Boto3 documentation:
[IoTAnalytics.Paginator.ListDatasetContents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents)

Arguments for `ListDatasetContentsPaginator.paginate` method:

- `datasetName`: `str` *(required)*
- `scheduledOnOrAfter`: `Union`\[`datetime`, `str`\]
- `scheduledBefore`: `Union`\[`datetime`, `str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetContentsPaginator.paginate` returns
`AsyncIterator`\[[ListDatasetContentsResponseTypeDef](./type_defs.md#listdatasetcontentsresponsetypedef)\].

<a id="listdatasetspaginator"></a>

## ListDatasetsPaginator

Type annotations for
`session.create_client("iotanalytics").get_paginator("list_datasets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("iotanalytics") as client:
    client: IoTAnalyticsClient
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")
```

Boto3 documentation:
[IoTAnalytics.Paginator.ListDatasets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets)

Arguments for `ListDatasetsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatasetsPaginator.paginate` returns
`AsyncIterator`\[[ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef)\].

<a id="listdatastorespaginator"></a>

## ListDatastoresPaginator

Type annotations for
`session.create_client("iotanalytics").get_paginator("list_datastores")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.paginator import ListDatastoresPaginator

session = get_session()
async with session.create_client("iotanalytics") as client:
    client: IoTAnalyticsClient
    paginator: ListDatastoresPaginator = client.get_paginator("list_datastores")
```

Boto3 documentation:
[IoTAnalytics.Paginator.ListDatastores](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores)

Arguments for `ListDatastoresPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDatastoresPaginator.paginate` returns
`AsyncIterator`\[[ListDatastoresResponseTypeDef](./type_defs.md#listdatastoresresponsetypedef)\].

<a id="listpipelinespaginator"></a>

## ListPipelinesPaginator

Type annotations for
`session.create_client("iotanalytics").get_paginator("list_pipelines")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.paginator import ListPipelinesPaginator

session = get_session()
async with session.create_client("iotanalytics") as client:
    client: IoTAnalyticsClient
    paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")
```

Boto3 documentation:
[IoTAnalytics.Paginator.ListPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines)

Arguments for `ListPipelinesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPipelinesPaginator.paginate` returns
`AsyncIterator`\[[ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef)\].