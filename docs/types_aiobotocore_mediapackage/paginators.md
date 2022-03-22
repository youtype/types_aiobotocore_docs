<a id="paginators-for-aiobotocore-mediapackage-module"></a>

# Paginators for aiobotocore MediaPackage module

> [Index](../README.md) > [MediaPackage](./README.md) > Paginators

Auto-generated documentation for
[MediaPackage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage)
type annotations stubs module
[types-aiobotocore-mediapackage](https://pypi.org/project/types-aiobotocore-mediapackage/).

- [Paginators for aiobotocore MediaPackage module](#paginators-for-aiobotocore-mediapackage-module)
  - [ListChannelsPaginator](#listchannelspaginator)
  - [ListHarvestJobsPaginator](#listharvestjobspaginator)
  - [ListOriginEndpointsPaginator](#listoriginendpointspaginator)

<a id="listchannelspaginator"></a>

## ListChannelsPaginator

Type annotations for
`session.create_client("mediapackage").get_paginator("list_channels")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("mediapackage") as client:
    client: MediaPackageClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
```

Boto3 documentation:
[MediaPackage.Paginator.ListChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListChannels)

Arguments for `ListChannelsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListChannelsPaginator.paginate` returns
`AsyncIterator`\[[ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)\].

<a id="listharvestjobspaginator"></a>

## ListHarvestJobsPaginator

Type annotations for
`session.create_client("mediapackage").get_paginator("list_harvest_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage.paginator import ListHarvestJobsPaginator

session = get_session()
async with session.create_client("mediapackage") as client:
    client: MediaPackageClient
    paginator: ListHarvestJobsPaginator = client.get_paginator("list_harvest_jobs")
```

Boto3 documentation:
[MediaPackage.Paginator.ListHarvestJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListHarvestJobs)

Arguments for `ListHarvestJobsPaginator.paginate` method:

- `IncludeChannelId`: `str`
- `IncludeStatus`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListHarvestJobsPaginator.paginate` returns
`AsyncIterator`\[[ListHarvestJobsResponseTypeDef](./type_defs.md#listharvestjobsresponsetypedef)\].

<a id="listoriginendpointspaginator"></a>

## ListOriginEndpointsPaginator

Type annotations for
`session.create_client("mediapackage").get_paginator("list_origin_endpoints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage.paginator import ListOriginEndpointsPaginator

session = get_session()
async with session.create_client("mediapackage") as client:
    client: MediaPackageClient
    paginator: ListOriginEndpointsPaginator = client.get_paginator("list_origin_endpoints")
```

Boto3 documentation:
[MediaPackage.Paginator.ListOriginEndpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Paginator.ListOriginEndpoints)

Arguments for `ListOriginEndpointsPaginator.paginate` method:

- `ChannelId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOriginEndpointsPaginator.paginate` returns
`AsyncIterator`\[[ListOriginEndpointsResponseTypeDef](./type_defs.md#listoriginendpointsresponsetypedef)\].
