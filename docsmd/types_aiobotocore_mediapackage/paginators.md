# Paginators

> [Index](../README.md) > [MediaPackage](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaPackage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
    type annotations stubs module [types-aiobotocore-mediapackage](https://pypi.org/project/types-aiobotocore-mediapackage/).

## ListChannelsPaginator

Type annotations and code completion for `#!python session.create_client("mediapackage").get_paginator("list_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListChannels)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("mediapackage") as client:  # (1)
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaPackageClient](./client.md)
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
## ListHarvestJobsPaginator

Type annotations and code completion for `#!python session.create_client("mediapackage").get_paginator("list_harvest_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListHarvestJobs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage.paginator import ListHarvestJobsPaginator

session = get_session()
async with session.create_client("mediapackage") as client:  # (1)
    paginator: ListHarvestJobsPaginator = client.get_paginator("list_harvest_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListHarvestJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaPackageClient](./client.md)
2. paginator: [ListHarvestJobsPaginator](./paginators.md#listharvestjobspaginator)
3. item: [:material-code-braces: ListHarvestJobsResponseTypeDef](./type_defs.md#listharvestjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHarvestJobsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    IncludeChannelId: str = ...,
    IncludeStatus: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListHarvestJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHarvestJobsResponseTypeDef](./type_defs.md#listharvestjobsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHarvestJobsRequestListHarvestJobsPaginateTypeDef = {  # (1)
    "IncludeChannelId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHarvestJobsRequestListHarvestJobsPaginateTypeDef](./type_defs.md#listharvestjobsrequestlistharvestjobspaginatetypedef) 
## ListOriginEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("mediapackage").get_paginator("list_origin_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListOriginEndpoints)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage.paginator import ListOriginEndpointsPaginator

session = get_session()
async with session.create_client("mediapackage") as client:  # (1)
    paginator: ListOriginEndpointsPaginator = client.get_paginator("list_origin_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListOriginEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaPackageClient](./client.md)
2. paginator: [ListOriginEndpointsPaginator](./paginators.md#listoriginendpointspaginator)
3. item: [:material-code-braces: ListOriginEndpointsResponseTypeDef](./type_defs.md#listoriginendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOriginEndpointsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ChannelId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOriginEndpointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOriginEndpointsResponseTypeDef](./type_defs.md#listoriginendpointsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOriginEndpointsRequestListOriginEndpointsPaginateTypeDef](./type_defs.md#listoriginendpointsrequestlistoriginendpointspaginatetypedef) 
