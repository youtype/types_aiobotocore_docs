# Paginators

> [Index](../README.md) > [IoTAnalytics](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#iotanalytics)
    type annotations stubs module [types-aiobotocore-iotanalytics](https://pypi.org/project/types-aiobotocore-iotanalytics/).

## ListChannelsPaginator

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator("list_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/paginator/ListChannels.html#IoTAnalytics.Paginator.ListChannels)

```python
# ListChannelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("iotanalytics") as client:  # (1)
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTAnalyticsClient](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: `AioPageIterator[ListChannelsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListChannelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListChannelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListChannelsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListChannelsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestPaginateTypeDef](./type_defs.md#listchannelsrequestpaginatetypedef)
## ListDatasetContentsPaginator

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator("list_dataset_contents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/paginator/ListDatasetContents.html#IoTAnalytics.Paginator.ListDatasetContents)

```python
# ListDatasetContentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.paginator import ListDatasetContentsPaginator

session = get_session()
async with session.create_client("iotanalytics") as client:  # (1)
    paginator: ListDatasetContentsPaginator = client.get_paginator("list_dataset_contents")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetContentsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTAnalyticsClient](./client.md)
2. paginator: [ListDatasetContentsPaginator](./paginators.md#listdatasetcontentspaginator)
3. item: `AioPageIterator[ListDatasetContentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDatasetContentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datasetName: str,
    scheduledOnOrAfter: TimestampTypeDef = ...,
    scheduledBefore: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDatasetContentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDatasetContentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetContentsRequestPaginateTypeDef = {  # (1)
    "datasetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetContentsRequestPaginateTypeDef](./type_defs.md#listdatasetcontentsrequestpaginatetypedef)
## ListDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/paginator/ListDatasets.html#IoTAnalytics.Paginator.ListDatasets)

```python
# ListDatasetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("iotanalytics") as client:  # (1)
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTAnalyticsClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: `AioPageIterator[ListDatasetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDatasetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef)
## ListDatastoresPaginator

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator("list_datastores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/paginator/ListDatastores.html#IoTAnalytics.Paginator.ListDatastores)

```python
# ListDatastoresPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.paginator import ListDatastoresPaginator

session = get_session()
async with session.create_client("iotanalytics") as client:  # (1)
    paginator: ListDatastoresPaginator = client.get_paginator("list_datastores")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatastoresResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTAnalyticsClient](./client.md)
2. paginator: [ListDatastoresPaginator](./paginators.md#listdatastorespaginator)
3. item: `AioPageIterator[ListDatastoresResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDatastoresPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDatastoresResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDatastoresResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDatastoresRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatastoresRequestPaginateTypeDef](./type_defs.md#listdatastoresrequestpaginatetypedef)
## ListPipelinesPaginator

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator("list_pipelines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics/paginator/ListPipelines.html#IoTAnalytics.Paginator.ListPipelines)

```python
# ListPipelinesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotanalytics.paginator import ListPipelinesPaginator

session = get_session()
async with session.create_client("iotanalytics") as client:  # (1)
    paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")  # (2)
    async for item in paginator.paginate(...):
        item: ListPipelinesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTAnalyticsClient](./client.md)
2. paginator: [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
3. item: `AioPageIterator[ListPipelinesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPipelinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPipelinesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPipelinesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPipelinesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelinesRequestPaginateTypeDef](./type_defs.md#listpipelinesrequestpaginatetypedef)
