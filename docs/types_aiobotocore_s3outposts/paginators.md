<a id="paginators-for-aiobotocore-s3outposts-module"></a>

# Paginators for aiobotocore S3Outposts module

> [Index](../README.md) > [S3Outposts](./README.md) > Paginators

Auto-generated documentation for
[S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
type annotations stubs module
[types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

- [Paginators for aiobotocore S3Outposts module](#paginators-for-aiobotocore-s3outposts-module)
  - [ListEndpointsPaginator](#listendpointspaginator)
  - [ListSharedEndpointsPaginator](#listsharedendpointspaginator)

<a id="listendpointspaginator"></a>

## ListEndpointsPaginator

Type annotations for
`session.create_client("s3outposts").get_paginator("list_endpoints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_s3outposts.paginator import ListEndpointsPaginator

session = get_session()
async with session.create_client("s3outposts") as client:
    client: S3OutpostsClient
    paginator: ListEndpointsPaginator = client.get_paginator("list_endpoints")
```

Boto3 documentation:
[S3Outposts.Paginator.ListEndpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints)

Arguments for `ListEndpointsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEndpointsPaginator.paginate` returns
`AsyncIterator`\[[ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef)\].

<a id="listsharedendpointspaginator"></a>

## ListSharedEndpointsPaginator

Type annotations for
`session.create_client("s3outposts").get_paginator("list_shared_endpoints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_s3outposts.paginator import ListSharedEndpointsPaginator

session = get_session()
async with session.create_client("s3outposts") as client:
    client: S3OutpostsClient
    paginator: ListSharedEndpointsPaginator = client.get_paginator("list_shared_endpoints")
```

Boto3 documentation:
[S3Outposts.Paginator.ListSharedEndpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints)

Arguments for `ListSharedEndpointsPaginator.paginate` method:

- `OutpostId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSharedEndpointsPaginator.paginate` returns
`AsyncIterator`\[[ListSharedEndpointsResultTypeDef](./type_defs.md#listsharedendpointsresulttypedef)\].
