<a id="paginators-for-aiobotocore-s3outposts-module"></a>

# Paginators for aiobotocore S3Outposts module

> [Index](..) > [S3Outposts](.) > Paginators

Auto-generated documentation for
[S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
type annotations stubs module
[types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

- [Paginators for aiobotocore S3Outposts module](#paginators-for-aiobotocore-s3outposts-module)
  - [ListEndpointsPaginator](#listendpointspaginator)

<a id="listendpointspaginator"></a>

## ListEndpointsPaginator

Type annotations for
`aiobotocore.create_client("s3outposts").get_paginator("list_endpoints")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_s3outposts.paginator import ListEndpointsPaginator

def get_list_endpoints_paginator() -> ListEndpointsPaginator:
    return Session().create_client("s3outposts").get_paginator("list_endpoints")
```

Boto3 documentation:
[S3Outposts.Paginator.ListEndpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints)

Arguments for `ListEndpointsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEndpointsPaginator.paginate` returns
`_PageIterator`\[[ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef)\].
