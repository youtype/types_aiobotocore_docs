# Paginators

> [Index](../README.md) > [MediaPackageVod](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaPackageVod](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod)
    type annotations stubs module [types-aiobotocore-mediapackage-vod](https://pypi.org/project/types-aiobotocore-mediapackage-vod/).

## ListAssetsPaginator

Type annotations and code completion for `#!python session.create_client("mediapackage-vod").get_paginator("list_assets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListAssets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage_vod.paginator import ListAssetsPaginator

session = get_session()
async with session.create_client("mediapackage-vod") as client:  # (1)
    paginator: ListAssetsPaginator = client.get_paginator("list_assets")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaPackageVodClient](./client.md)
2. paginator: [ListAssetsPaginator](./paginators.md#listassetspaginator)
3. item: [:material-code-braces: ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PackagingGroupId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAssetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAssetsRequestListAssetsPaginateTypeDef = {  # (1)
    "PackagingGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetsRequestListAssetsPaginateTypeDef](./type_defs.md#listassetsrequestlistassetspaginatetypedef) 
## ListPackagingConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("mediapackage-vod").get_paginator("list_packaging_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingConfigurations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage_vod.paginator import ListPackagingConfigurationsPaginator

session = get_session()
async with session.create_client("mediapackage-vod") as client:  # (1)
    paginator: ListPackagingConfigurationsPaginator = client.get_paginator("list_packaging_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListPackagingConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaPackageVodClient](./client.md)
2. paginator: [ListPackagingConfigurationsPaginator](./paginators.md#listpackagingconfigurationspaginator)
3. item: [:material-code-braces: ListPackagingConfigurationsResponseTypeDef](./type_defs.md#listpackagingconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPackagingConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PackagingGroupId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPackagingConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPackagingConfigurationsResponseTypeDef](./type_defs.md#listpackagingconfigurationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef = {  # (1)
    "PackagingGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPackagingConfigurationsRequestListPackagingConfigurationsPaginateTypeDef](./type_defs.md#listpackagingconfigurationsrequestlistpackagingconfigurationspaginatetypedef) 
## ListPackagingGroupsPaginator

Type annotations and code completion for `#!python session.create_client("mediapackage-vod").get_paginator("list_packaging_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Paginator.ListPackagingGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediapackage_vod.paginator import ListPackagingGroupsPaginator

session = get_session()
async with session.create_client("mediapackage-vod") as client:  # (1)
    paginator: ListPackagingGroupsPaginator = client.get_paginator("list_packaging_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListPackagingGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaPackageVodClient](./client.md)
2. paginator: [ListPackagingGroupsPaginator](./paginators.md#listpackaginggroupspaginator)
3. item: [:material-code-braces: ListPackagingGroupsResponseTypeDef](./type_defs.md#listpackaginggroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPackagingGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPackagingGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPackagingGroupsResponseTypeDef](./type_defs.md#listpackaginggroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPackagingGroupsRequestListPackagingGroupsPaginateTypeDef](./type_defs.md#listpackaginggroupsrequestlistpackaginggroupspaginatetypedef) 
