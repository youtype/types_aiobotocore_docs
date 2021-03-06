# Paginators

> [Index](../README.md) > [S3Outposts](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
    type annotations stubs module [types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

## ListEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("s3outposts").get_paginator("list_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_s3outposts.paginator import ListEndpointsPaginator

session = get_session()
async with session.create_client("s3outposts") as client:
    client: S3OutpostsClient
    paginator: ListEndpointsPaginator = client.get_paginator("list_endpoints")
```


### paginate

Type annotations and code completion for `#!python ListEndpointsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEndpointsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListEndpointsRequestListEndpointsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEndpointsRequestListEndpointsPaginateTypeDef](./type_defs.md#listendpointsrequestlistendpointspaginatetypedef) 
## ListSharedEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("s3outposts").get_paginator("list_shared_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_s3outposts.paginator import ListSharedEndpointsPaginator

session = get_session()
async with session.create_client("s3outposts") as client:
    client: S3OutpostsClient
    paginator: ListSharedEndpointsPaginator = client.get_paginator("list_shared_endpoints")
```


### paginate

Type annotations and code completion for `#!python ListSharedEndpointsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    OutpostId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSharedEndpointsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSharedEndpointsResultTypeDef](./type_defs.md#listsharedendpointsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = {  # (1)
    "OutpostId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef](./type_defs.md#listsharedendpointsrequestlistsharedendpointspaginatetypedef) 
