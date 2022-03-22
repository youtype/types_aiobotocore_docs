<a id="paginators-for-aiobotocore-directoryservice-module"></a>

# Paginators for aiobotocore DirectoryService module

> [Index](../README.md) > [DirectoryService](./README.md) > Paginators

Auto-generated documentation for
[DirectoryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService)
type annotations stubs module
[types-aiobotocore-ds](https://pypi.org/project/types-aiobotocore-ds/).

- [Paginators for aiobotocore DirectoryService module](#paginators-for-aiobotocore-directoryservice-module)
  - [DescribeDirectoriesPaginator](#describedirectoriespaginator)
  - [DescribeDomainControllersPaginator](#describedomaincontrollerspaginator)
  - [DescribeSharedDirectoriesPaginator](#describeshareddirectoriespaginator)
  - [DescribeSnapshotsPaginator](#describesnapshotspaginator)
  - [DescribeTrustsPaginator](#describetrustspaginator)
  - [ListIpRoutesPaginator](#listiproutespaginator)
  - [ListLogSubscriptionsPaginator](#listlogsubscriptionspaginator)
  - [ListSchemaExtensionsPaginator](#listschemaextensionspaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)

<a id="describedirectoriespaginator"></a>

## DescribeDirectoriesPaginator

Type annotations for
`session.create_client("ds").get_paginator("describe_directories")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeDirectoriesPaginator

session = get_session()
async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    paginator: DescribeDirectoriesPaginator = client.get_paginator("describe_directories")
```

Boto3 documentation:
[DirectoryService.Paginator.DescribeDirectories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDirectories)

Arguments for `DescribeDirectoriesPaginator.paginate` method:

- `DirectoryIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDirectoriesPaginator.paginate` returns
`AsyncIterator`\[[DescribeDirectoriesResultTypeDef](./type_defs.md#describedirectoriesresulttypedef)\].

<a id="describedomaincontrollerspaginator"></a>

## DescribeDomainControllersPaginator

Type annotations for
`session.create_client("ds").get_paginator("describe_domain_controllers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeDomainControllersPaginator

session = get_session()
async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    paginator: DescribeDomainControllersPaginator = client.get_paginator("describe_domain_controllers")
```

Boto3 documentation:
[DirectoryService.Paginator.DescribeDomainControllers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeDomainControllers)

Arguments for `DescribeDomainControllersPaginator.paginate` method:

- `DirectoryId`: `str` *(required)*
- `DomainControllerIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDomainControllersPaginator.paginate` returns
`AsyncIterator`\[[DescribeDomainControllersResultTypeDef](./type_defs.md#describedomaincontrollersresulttypedef)\].

<a id="describeshareddirectoriespaginator"></a>

## DescribeSharedDirectoriesPaginator

Type annotations for
`session.create_client("ds").get_paginator("describe_shared_directories")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeSharedDirectoriesPaginator

session = get_session()
async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    paginator: DescribeSharedDirectoriesPaginator = client.get_paginator("describe_shared_directories")
```

Boto3 documentation:
[DirectoryService.Paginator.DescribeSharedDirectories](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSharedDirectories)

Arguments for `DescribeSharedDirectoriesPaginator.paginate` method:

- `OwnerDirectoryId`: `str` *(required)*
- `SharedDirectoryIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeSharedDirectoriesPaginator.paginate` returns
`AsyncIterator`\[[DescribeSharedDirectoriesResultTypeDef](./type_defs.md#describeshareddirectoriesresulttypedef)\].

<a id="describesnapshotspaginator"></a>

## DescribeSnapshotsPaginator

Type annotations for
`session.create_client("ds").get_paginator("describe_snapshots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeSnapshotsPaginator

session = get_session()
async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")
```

Boto3 documentation:
[DirectoryService.Paginator.DescribeSnapshots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeSnapshots)

Arguments for `DescribeSnapshotsPaginator.paginate` method:

- `DirectoryId`: `str`
- `SnapshotIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeSnapshotsPaginator.paginate` returns
`AsyncIterator`\[[DescribeSnapshotsResultTypeDef](./type_defs.md#describesnapshotsresulttypedef)\].

<a id="describetrustspaginator"></a>

## DescribeTrustsPaginator

Type annotations for
`session.create_client("ds").get_paginator("describe_trusts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import DescribeTrustsPaginator

session = get_session()
async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    paginator: DescribeTrustsPaginator = client.get_paginator("describe_trusts")
```

Boto3 documentation:
[DirectoryService.Paginator.DescribeTrusts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.DescribeTrusts)

Arguments for `DescribeTrustsPaginator.paginate` method:

- `DirectoryId`: `str`
- `TrustIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeTrustsPaginator.paginate` returns
`AsyncIterator`\[[DescribeTrustsResultTypeDef](./type_defs.md#describetrustsresulttypedef)\].

<a id="listiproutespaginator"></a>

## ListIpRoutesPaginator

Type annotations for
`session.create_client("ds").get_paginator("list_ip_routes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListIpRoutesPaginator

session = get_session()
async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    paginator: ListIpRoutesPaginator = client.get_paginator("list_ip_routes")
```

Boto3 documentation:
[DirectoryService.Paginator.ListIpRoutes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListIpRoutes)

Arguments for `ListIpRoutesPaginator.paginate` method:

- `DirectoryId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListIpRoutesPaginator.paginate` returns
`AsyncIterator`\[[ListIpRoutesResultTypeDef](./type_defs.md#listiproutesresulttypedef)\].

<a id="listlogsubscriptionspaginator"></a>

## ListLogSubscriptionsPaginator

Type annotations for
`session.create_client("ds").get_paginator("list_log_subscriptions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListLogSubscriptionsPaginator

session = get_session()
async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    paginator: ListLogSubscriptionsPaginator = client.get_paginator("list_log_subscriptions")
```

Boto3 documentation:
[DirectoryService.Paginator.ListLogSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListLogSubscriptions)

Arguments for `ListLogSubscriptionsPaginator.paginate` method:

- `DirectoryId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListLogSubscriptionsPaginator.paginate` returns
`AsyncIterator`\[[ListLogSubscriptionsResultTypeDef](./type_defs.md#listlogsubscriptionsresulttypedef)\].

<a id="listschemaextensionspaginator"></a>

## ListSchemaExtensionsPaginator

Type annotations for
`session.create_client("ds").get_paginator("list_schema_extensions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListSchemaExtensionsPaginator

session = get_session()
async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    paginator: ListSchemaExtensionsPaginator = client.get_paginator("list_schema_extensions")
```

Boto3 documentation:
[DirectoryService.Paginator.ListSchemaExtensions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListSchemaExtensions)

Arguments for `ListSchemaExtensionsPaginator.paginate` method:

- `DirectoryId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSchemaExtensionsPaginator.paginate` returns
`AsyncIterator`\[[ListSchemaExtensionsResultTypeDef](./type_defs.md#listschemaextensionsresulttypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("ds").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ds.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[DirectoryService.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `ResourceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterator`\[[ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)\].
