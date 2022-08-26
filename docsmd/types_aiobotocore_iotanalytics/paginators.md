# Paginators

> [Index](../README.md) > [IoTAnalytics](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics)
    type annotations stubs module [types-aiobotocore-iotanalytics](https://pypi.org/project/types-aiobotocore-iotanalytics/).

## ListChannelsPaginator

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator("list_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListChannels)

```python title="Usage example"
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
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChannelsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListChannelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListChannelsRequestListChannelsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestListChannelsPaginateTypeDef](./type_defs.md#listchannelsrequestlistchannelspaginatetypedef) 
## ListDatasetContentsPaginator

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator("list_dataset_contents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasetContents)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDatasetContentsResponseTypeDef](./type_defs.md#listdatasetcontentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetContentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    datasetName: str,
    scheduledOnOrAfter: Union[datetime, str] = ...,
    scheduledBefore: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetContentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetContentsResponseTypeDef](./type_defs.md#listdatasetcontentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetContentsRequestListDatasetContentsPaginateTypeDef = {  # (1)
    "datasetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetContentsRequestListDatasetContentsPaginateTypeDef](./type_defs.md#listdatasetcontentsrequestlistdatasetcontentspaginatetypedef) 
## ListDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatasets)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetsRequestListDatasetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestListDatasetsPaginateTypeDef](./type_defs.md#listdatasetsrequestlistdatasetspaginatetypedef) 
## ListDatastoresPaginator

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator("list_datastores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListDatastores)

```python title="Usage example"
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
3. item: [:material-code-braces: ListDatastoresResponseTypeDef](./type_defs.md#listdatastoresresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatastoresPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatastoresResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatastoresResponseTypeDef](./type_defs.md#listdatastoresresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatastoresRequestListDatastoresPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatastoresRequestListDatastoresPaginateTypeDef](./type_defs.md#listdatastoresrequestlistdatastorespaginatetypedef) 
## ListPipelinesPaginator

Type annotations and code completion for `#!python session.create_client("iotanalytics").get_paginator("list_pipelines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#IoTAnalytics.Paginator.ListPipelines)

```python title="Usage example"
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
3. item: [:material-code-braces: ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPipelinesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPipelinesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPipelinesResponseTypeDef](./type_defs.md#listpipelinesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPipelinesRequestListPipelinesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelinesRequestListPipelinesPaginateTypeDef](./type_defs.md#listpipelinesrequestlistpipelinespaginatetypedef) 
