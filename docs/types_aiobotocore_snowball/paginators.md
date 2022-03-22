<a id="paginators-for-aiobotocore-snowball-module"></a>

# Paginators for aiobotocore Snowball module

> [Index](../README.md) > [Snowball](./README.md) > Paginators

Auto-generated documentation for
[Snowball](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
type annotations stubs module
[types-aiobotocore-snowball](https://pypi.org/project/types-aiobotocore-snowball/).

- [Paginators for aiobotocore Snowball module](#paginators-for-aiobotocore-snowball-module)
  - [DescribeAddressesPaginator](#describeaddressespaginator)
  - [ListClusterJobsPaginator](#listclusterjobspaginator)
  - [ListClustersPaginator](#listclusterspaginator)
  - [ListCompatibleImagesPaginator](#listcompatibleimagespaginator)
  - [ListJobsPaginator](#listjobspaginator)

<a id="describeaddressespaginator"></a>

## DescribeAddressesPaginator

Type annotations for
`session.create_client("snowball").get_paginator("describe_addresses")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import DescribeAddressesPaginator

session = get_session()
async with session.create_client("snowball") as client:
    client: SnowballClient
    paginator: DescribeAddressesPaginator = client.get_paginator("describe_addresses")
```

Boto3 documentation:
[Snowball.Paginator.DescribeAddresses](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses)

Arguments for `DescribeAddressesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeAddressesPaginator.paginate` returns
`AsyncIterator`\[[DescribeAddressesResultTypeDef](./type_defs.md#describeaddressesresulttypedef)\].

<a id="listclusterjobspaginator"></a>

## ListClusterJobsPaginator

Type annotations for
`session.create_client("snowball").get_paginator("list_cluster_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import ListClusterJobsPaginator

session = get_session()
async with session.create_client("snowball") as client:
    client: SnowballClient
    paginator: ListClusterJobsPaginator = client.get_paginator("list_cluster_jobs")
```

Boto3 documentation:
[Snowball.Paginator.ListClusterJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs)

Arguments for `ListClusterJobsPaginator.paginate` method:

- `ClusterId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListClusterJobsPaginator.paginate` returns
`AsyncIterator`\[[ListClusterJobsResultTypeDef](./type_defs.md#listclusterjobsresulttypedef)\].

<a id="listclusterspaginator"></a>

## ListClustersPaginator

Type annotations for
`session.create_client("snowball").get_paginator("list_clusters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("snowball") as client:
    client: SnowballClient
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")
```

Boto3 documentation:
[Snowball.Paginator.ListClusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters)

Arguments for `ListClustersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListClustersPaginator.paginate` returns
`AsyncIterator`\[[ListClustersResultTypeDef](./type_defs.md#listclustersresulttypedef)\].

<a id="listcompatibleimagespaginator"></a>

## ListCompatibleImagesPaginator

Type annotations for
`session.create_client("snowball").get_paginator("list_compatible_images")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import ListCompatibleImagesPaginator

session = get_session()
async with session.create_client("snowball") as client:
    client: SnowballClient
    paginator: ListCompatibleImagesPaginator = client.get_paginator("list_compatible_images")
```

Boto3 documentation:
[Snowball.Paginator.ListCompatibleImages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages)

Arguments for `ListCompatibleImagesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCompatibleImagesPaginator.paginate` returns
`AsyncIterator`\[[ListCompatibleImagesResultTypeDef](./type_defs.md#listcompatibleimagesresulttypedef)\].

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for
`session.create_client("snowball").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("snowball") as client:
    client: SnowballClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```

Boto3 documentation:
[Snowball.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`AsyncIterator`\[[ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef)\].
