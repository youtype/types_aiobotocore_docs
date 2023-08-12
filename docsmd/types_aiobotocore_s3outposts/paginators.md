# Paginators

> [Index](../README.md) > [S3Outposts](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts)
    type annotations stubs module [types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).

## ListEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("s3outposts").get_paginator("list_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListEndpoints)

```python
# ListEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3outposts.paginator import ListEndpointsPaginator

session = get_session()
async with session.create_client("s3outposts") as client:  # (1)
    paginator: ListEndpointsPaginator = client.get_paginator("list_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListEndpointsResultTypeDef
        print(item)  # (3)
```

1. client: [S3OutpostsClient](./client.md)
2. paginator: [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
3. item: [:material-code-braces: ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEndpointsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEndpointsResultTypeDef](./type_defs.md#listendpointsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEndpointsRequestListEndpointsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEndpointsRequestListEndpointsPaginateTypeDef](./type_defs.md#listendpointsrequestlistendpointspaginatetypedef) 
## ListOutpostsWithS3Paginator

Type annotations and code completion for `#!python session.create_client("s3outposts").get_paginator("list_outposts_with_s3")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListOutpostsWithS3)

```python
# ListOutpostsWithS3Paginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3outposts.paginator import ListOutpostsWithS3Paginator

session = get_session()
async with session.create_client("s3outposts") as client:  # (1)
    paginator: ListOutpostsWithS3Paginator = client.get_paginator("list_outposts_with_s3")  # (2)
    async for item in paginator.paginate(...):
        item: ListOutpostsWithS3ResultTypeDef
        print(item)  # (3)
```

1. client: [S3OutpostsClient](./client.md)
2. paginator: [ListOutpostsWithS3Paginator](./paginators.md#listoutpostswiths3paginator)
3. item: [:material-code-braces: ListOutpostsWithS3ResultTypeDef](./type_defs.md#listoutpostswiths3resulttypedef) 


### paginate

Type annotations and code completion for `#!python ListOutpostsWithS3Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOutpostsWithS3ResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOutpostsWithS3ResultTypeDef](./type_defs.md#listoutpostswiths3resulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOutpostsWithS3RequestListOutpostsWithS3PaginateTypeDef](./type_defs.md#listoutpostswiths3requestlistoutpostswiths3paginatetypedef) 
## ListSharedEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("s3outposts").get_paginator("list_shared_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#S3Outposts.Paginator.ListSharedEndpoints)

```python
# ListSharedEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3outposts.paginator import ListSharedEndpointsPaginator

session = get_session()
async with session.create_client("s3outposts") as client:  # (1)
    paginator: ListSharedEndpointsPaginator = client.get_paginator("list_shared_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListSharedEndpointsResultTypeDef
        print(item)  # (3)
```

1. client: [S3OutpostsClient](./client.md)
2. paginator: [ListSharedEndpointsPaginator](./paginators.md#listsharedendpointspaginator)
3. item: [:material-code-braces: ListSharedEndpointsResultTypeDef](./type_defs.md#listsharedendpointsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListSharedEndpointsPaginator.paginate` method.

```python
# paginate method definition

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


```python
# paginate method usage example with argument unpacking

kwargs: ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef = {  # (1)
    "OutpostId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSharedEndpointsRequestListSharedEndpointsPaginateTypeDef](./type_defs.md#listsharedendpointsrequestlistsharedendpointspaginatetypedef) 
