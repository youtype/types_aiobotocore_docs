<a id="paginators-for-aiobotocore-mediapackagevod-module"></a>

# Paginators for aiobotocore MediaPackageVod module

> [Index](..) > [MediaPackageVod](.) > Paginators

Auto-generated documentation for
[MediaPackageVod](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
type annotations stubs module
[types-aiobotocore-mediapackage-vod](https://pypi.org/project/types-aiobotocore-mediapackage-vod/).

- [Paginators for aiobotocore MediaPackageVod module](#paginators-for-aiobotocore-mediapackagevod-module)
  - [ListAssetsPaginator](#listassetspaginator)
  - [ListPackagingConfigurationsPaginator](#listpackagingconfigurationspaginator)
  - [ListPackagingGroupsPaginator](#listpackaginggroupspaginator)

<a id="listassetspaginator"></a>

## ListAssetsPaginator

Type annotations for
`session.create_client("mediapackage-vod").get_paginator("list_assets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage_vod.paginator import ListAssetsPaginator

session = get_session()
async with session.create_client("mediapackage-vod") as client:
    client: MediaPackageVodClient
    paginator: ListAssetsPaginator = client.get_paginator("list_assets")
```

Boto3 documentation:
[MediaPackageVod.Paginator.ListAssets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListAssets)

Arguments for `ListAssetsPaginator.paginate` method:

- `PackagingGroupId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAssetsPaginator.paginate` returns
`AsyncIterable`\[[ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef)\].

<a id="listpackagingconfigurationspaginator"></a>

## ListPackagingConfigurationsPaginator

Type annotations for
`session.create_client("mediapackage-vod").get_paginator("list_packaging_configurations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage_vod.paginator import ListPackagingConfigurationsPaginator

session = get_session()
async with session.create_client("mediapackage-vod") as client:
    client: MediaPackageVodClient
    paginator: ListPackagingConfigurationsPaginator = client.get_paginator("list_packaging_configurations")
```

Boto3 documentation:
[MediaPackageVod.Paginator.ListPackagingConfigurations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingConfigurations)

Arguments for `ListPackagingConfigurationsPaginator.paginate` method:

- `PackagingGroupId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPackagingConfigurationsPaginator.paginate` returns
`AsyncIterable`\[[ListPackagingConfigurationsResponseTypeDef](./type_defs.md#listpackagingconfigurationsresponsetypedef)\].

<a id="listpackaginggroupspaginator"></a>

## ListPackagingGroupsPaginator

Type annotations for
`session.create_client("mediapackage-vod").get_paginator("list_packaging_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage_vod.paginator import ListPackagingGroupsPaginator

session = get_session()
async with session.create_client("mediapackage-vod") as client:
    client: MediaPackageVodClient
    paginator: ListPackagingGroupsPaginator = client.get_paginator("list_packaging_groups")
```

Boto3 documentation:
[MediaPackageVod.Paginator.ListPackagingGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingGroups)

Arguments for `ListPackagingGroupsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPackagingGroupsPaginator.paginate` returns
`AsyncIterable`\[[ListPackagingGroupsResponseTypeDef](./type_defs.md#listpackaginggroupsresponsetypedef)\].
