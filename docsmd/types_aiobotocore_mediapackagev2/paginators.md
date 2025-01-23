# Paginators

> [Index](../README.md) > [Mediapackagev2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Mediapackagev2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2)
    type annotations stubs module [types-aiobotocore-mediapackagev2](https://pypi.org/project/types-aiobotocore-mediapackagev2/).

## ListChannelGroupsPaginator

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_paginator("list_channel_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/paginator/ListChannelGroups.html#Mediapackagev2.Paginator.ListChannelGroups)

```python
# ListChannelGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediapackagev2.paginator import ListChannelGroupsPaginator

session = get_session()
async with session.create_client("mediapackagev2") as client:  # (1)
    paginator: ListChannelGroupsPaginator = client.get_paginator("list_channel_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [Mediapackagev2Client](./client.md)
2. paginator: [ListChannelGroupsPaginator](./paginators.md#listchannelgroupspaginator)
3. item: [:material-code-braces: ListChannelGroupsResponseTypeDef](./type_defs.md#listchannelgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChannelGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListChannelGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChannelGroupsResponseTypeDef](./type_defs.md#listchannelgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChannelGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelGroupsRequestPaginateTypeDef](./type_defs.md#listchannelgroupsrequestpaginatetypedef) 
## ListChannelsPaginator

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_paginator("list_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/paginator/ListChannels.html#Mediapackagev2.Paginator.ListChannels)

```python
# ListChannelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediapackagev2.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("mediapackagev2") as client:  # (1)
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelsResponseTypeDef
        print(item)  # (3)
```

1. client: [Mediapackagev2Client](./client.md)
2. paginator: [ListChannelsPaginator](./paginators.md#listchannelspaginator)
3. item: [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChannelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChannelGroupName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListChannelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChannelsRequestPaginateTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestPaginateTypeDef](./type_defs.md#listchannelsrequestpaginatetypedef) 
## ListHarvestJobsPaginator

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_paginator("list_harvest_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/paginator/ListHarvestJobs.html#Mediapackagev2.Paginator.ListHarvestJobs)

```python
# ListHarvestJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediapackagev2.paginator import ListHarvestJobsPaginator

session = get_session()
async with session.create_client("mediapackagev2") as client:  # (1)
    paginator: ListHarvestJobsPaginator = client.get_paginator("list_harvest_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListHarvestJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [Mediapackagev2Client](./client.md)
2. paginator: [ListHarvestJobsPaginator](./paginators.md#listharvestjobspaginator)
3. item: [:material-code-braces: ListHarvestJobsResponseTypeDef](./type_defs.md#listharvestjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListHarvestJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str = ...,
    OriginEndpointName: str = ...,
    Status: HarvestJobStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListHarvestJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: HarvestJobStatusType](./literals.md#harvestjobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListHarvestJobsResponseTypeDef](./type_defs.md#listharvestjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListHarvestJobsRequestPaginateTypeDef = {  # (1)
    "ChannelGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHarvestJobsRequestPaginateTypeDef](./type_defs.md#listharvestjobsrequestpaginatetypedef) 
## ListOriginEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("mediapackagev2").get_paginator("list_origin_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2/paginator/ListOriginEndpoints.html#Mediapackagev2.Paginator.ListOriginEndpoints)

```python
# ListOriginEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediapackagev2.paginator import ListOriginEndpointsPaginator

session = get_session()
async with session.create_client("mediapackagev2") as client:  # (1)
    paginator: ListOriginEndpointsPaginator = client.get_paginator("list_origin_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListOriginEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [Mediapackagev2Client](./client.md)
2. paginator: [ListOriginEndpointsPaginator](./paginators.md#listoriginendpointspaginator)
3. item: [:material-code-braces: ListOriginEndpointsResponseTypeDef](./type_defs.md#listoriginendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOriginEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ChannelGroupName: str,
    ChannelName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOriginEndpointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOriginEndpointsResponseTypeDef](./type_defs.md#listoriginendpointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOriginEndpointsRequestPaginateTypeDef = {  # (1)
    "ChannelGroupName": ...,
    "ChannelName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOriginEndpointsRequestPaginateTypeDef](./type_defs.md#listoriginendpointsrequestpaginatetypedef) 
