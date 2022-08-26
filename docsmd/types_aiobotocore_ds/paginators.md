# Paginators

> [Index](../README.md) > [DirectoryService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DirectoryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
    type annotations stubs module [types-aiobotocore-ds](https://pypi.org/project/types-aiobotocore-ds/).

## DescribeDirectoriesPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_directories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDirectories)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeDirectoriesPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeDirectoriesPaginator = client.get_paginator("describe_directories")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDirectoriesResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeDirectoriesPaginator](./paginators.md#describedirectoriespaginator)
3. item: [:material-code-braces: DescribeDirectoriesResultTypeDef](./type_defs.md#describedirectoriesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDirectoriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DirectoryIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeDirectoriesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDirectoriesResultTypeDef](./type_defs.md#describedirectoriesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef = {  # (1)
    "DirectoryIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDirectoriesRequestDescribeDirectoriesPaginateTypeDef](./type_defs.md#describedirectoriesrequestdescribedirectoriespaginatetypedef) 
## DescribeDomainControllersPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_domain_controllers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDomainControllers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeDomainControllersPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeDomainControllersPaginator = client.get_paginator("describe_domain_controllers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDomainControllersResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeDomainControllersPaginator](./paginators.md#describedomaincontrollerspaginator)
3. item: [:material-code-braces: DescribeDomainControllersResultTypeDef](./type_defs.md#describedomaincontrollersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDomainControllersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DirectoryId: str,
    DomainControllerIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeDomainControllersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDomainControllersResultTypeDef](./type_defs.md#describedomaincontrollersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDomainControllersRequestDescribeDomainControllersPaginateTypeDef](./type_defs.md#describedomaincontrollersrequestdescribedomaincontrollerspaginatetypedef) 
## DescribeSharedDirectoriesPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_shared_directories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSharedDirectories)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeSharedDirectoriesPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeSharedDirectoriesPaginator = client.get_paginator("describe_shared_directories")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSharedDirectoriesResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeSharedDirectoriesPaginator](./paginators.md#describeshareddirectoriespaginator)
3. item: [:material-code-braces: DescribeSharedDirectoriesResultTypeDef](./type_defs.md#describeshareddirectoriesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSharedDirectoriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OwnerDirectoryId: str,
    SharedDirectoryIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSharedDirectoriesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSharedDirectoriesResultTypeDef](./type_defs.md#describeshareddirectoriesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef = {  # (1)
    "OwnerDirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSharedDirectoriesRequestDescribeSharedDirectoriesPaginateTypeDef](./type_defs.md#describeshareddirectoriesrequestdescribeshareddirectoriespaginatetypedef) 
## DescribeSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSnapshots)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeSnapshotsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSnapshotsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeSnapshotsPaginator](./paginators.md#describesnapshotspaginator)
3. item: [:material-code-braces: DescribeSnapshotsResultTypeDef](./type_defs.md#describesnapshotsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSnapshotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DirectoryId: str = ...,
    SnapshotIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSnapshotsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSnapshotsResultTypeDef](./type_defs.md#describesnapshotsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef](./type_defs.md#describesnapshotsrequestdescribesnapshotspaginatetypedef) 
## DescribeTrustsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("describe_trusts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeTrusts)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeTrustsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: DescribeTrustsPaginator = client.get_paginator("describe_trusts")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTrustsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeTrustsPaginator](./paginators.md#describetrustspaginator)
3. item: [:material-code-braces: DescribeTrustsResultTypeDef](./type_defs.md#describetrustsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTrustsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DirectoryId: str = ...,
    TrustIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeTrustsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeTrustsResultTypeDef](./type_defs.md#describetrustsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTrustsRequestDescribeTrustsPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTrustsRequestDescribeTrustsPaginateTypeDef](./type_defs.md#describetrustsrequestdescribetrustspaginatetypedef) 
## ListIpRoutesPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("list_ip_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListIpRoutes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListIpRoutesPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: ListIpRoutesPaginator = client.get_paginator("list_ip_routes")  # (2)
    async for item in paginator.paginate(...):
        item: ListIpRoutesResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [ListIpRoutesPaginator](./paginators.md#listiproutespaginator)
3. item: [:material-code-braces: ListIpRoutesResultTypeDef](./type_defs.md#listiproutesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListIpRoutesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DirectoryId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIpRoutesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIpRoutesResultTypeDef](./type_defs.md#listiproutesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListIpRoutesRequestListIpRoutesPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIpRoutesRequestListIpRoutesPaginateTypeDef](./type_defs.md#listiproutesrequestlistiproutespaginatetypedef) 
## ListLogSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("list_log_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListLogSubscriptions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListLogSubscriptionsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: ListLogSubscriptionsPaginator = client.get_paginator("list_log_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: ListLogSubscriptionsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [ListLogSubscriptionsPaginator](./paginators.md#listlogsubscriptionspaginator)
3. item: [:material-code-braces: ListLogSubscriptionsResultTypeDef](./type_defs.md#listlogsubscriptionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListLogSubscriptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DirectoryId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListLogSubscriptionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLogSubscriptionsResultTypeDef](./type_defs.md#listlogsubscriptionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLogSubscriptionsRequestListLogSubscriptionsPaginateTypeDef](./type_defs.md#listlogsubscriptionsrequestlistlogsubscriptionspaginatetypedef) 
## ListSchemaExtensionsPaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("list_schema_extensions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListSchemaExtensions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListSchemaExtensionsPaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: ListSchemaExtensionsPaginator = client.get_paginator("list_schema_extensions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemaExtensionsResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [ListSchemaExtensionsPaginator](./paginators.md#listschemaextensionspaginator)
3. item: [:material-code-braces: ListSchemaExtensionsResultTypeDef](./type_defs.md#listschemaextensionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListSchemaExtensionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DirectoryId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSchemaExtensionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSchemaExtensionsResultTypeDef](./type_defs.md#listschemaextensionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef = {  # (1)
    "DirectoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemaExtensionsRequestListSchemaExtensionsPaginateTypeDef](./type_defs.md#listschemaextensionsrequestlistschemaextensionspaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("ds").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListTagsForResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("ds") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResultTypeDef
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef) 
