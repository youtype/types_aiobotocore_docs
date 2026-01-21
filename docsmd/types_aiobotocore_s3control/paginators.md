# Paginators

> [Index](../README.md) > [S3Control](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [S3Control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#s3control)
    type annotations stubs module [types-aiobotocore-s3control](https://pypi.org/project/types-aiobotocore-s3control/).

## ListAccessPointsForDirectoryBucketsPaginator

Type annotations and code completion for `#!python session.create_client("s3control").get_paginator("list_access_points_for_directory_buckets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control/paginator/ListAccessPointsForDirectoryBuckets.html#S3Control.Paginator.ListAccessPointsForDirectoryBuckets)

```python
# ListAccessPointsForDirectoryBucketsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3control.paginator import ListAccessPointsForDirectoryBucketsPaginator

session = get_session()
async with session.create_client("s3control") as client:  # (1)
    paginator: ListAccessPointsForDirectoryBucketsPaginator = client.get_paginator("list_access_points_for_directory_buckets")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessPointsForDirectoryBucketsResultTypeDef
        print(item)  # (3)
```

1. client: [S3ControlClient](./client.md)
2. paginator: [ListAccessPointsForDirectoryBucketsPaginator](./paginators.md#listaccesspointsfordirectorybucketspaginator)
3. item: `AioPageIterator[ListAccessPointsForDirectoryBucketsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccessPointsForDirectoryBucketsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    DirectoryBucket: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAccessPointsForDirectoryBucketsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAccessPointsForDirectoryBucketsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessPointsForDirectoryBucketsRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessPointsForDirectoryBucketsRequestPaginateTypeDef](./type_defs.md#listaccesspointsfordirectorybucketsrequestpaginatetypedef)
## ListAccessPointsForObjectLambdaPaginator

Type annotations and code completion for `#!python session.create_client("s3control").get_paginator("list_access_points_for_object_lambda")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control/paginator/ListAccessPointsForObjectLambda.html#S3Control.Paginator.ListAccessPointsForObjectLambda)

```python
# ListAccessPointsForObjectLambdaPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3control.paginator import ListAccessPointsForObjectLambdaPaginator

session = get_session()
async with session.create_client("s3control") as client:  # (1)
    paginator: ListAccessPointsForObjectLambdaPaginator = client.get_paginator("list_access_points_for_object_lambda")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessPointsForObjectLambdaResultTypeDef
        print(item)  # (3)
```

1. client: [S3ControlClient](./client.md)
2. paginator: [ListAccessPointsForObjectLambdaPaginator](./paginators.md#listaccesspointsforobjectlambdapaginator)
3. item: `AioPageIterator[ListAccessPointsForObjectLambdaResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccessPointsForObjectLambdaPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAccessPointsForObjectLambdaResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAccessPointsForObjectLambdaResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessPointsForObjectLambdaRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessPointsForObjectLambdaRequestPaginateTypeDef](./type_defs.md#listaccesspointsforobjectlambdarequestpaginatetypedef)
## ListCallerAccessGrantsPaginator

Type annotations and code completion for `#!python session.create_client("s3control").get_paginator("list_caller_access_grants")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control/paginator/ListCallerAccessGrants.html#S3Control.Paginator.ListCallerAccessGrants)

```python
# ListCallerAccessGrantsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3control.paginator import ListCallerAccessGrantsPaginator

session = get_session()
async with session.create_client("s3control") as client:  # (1)
    paginator: ListCallerAccessGrantsPaginator = client.get_paginator("list_caller_access_grants")  # (2)
    async for item in paginator.paginate(...):
        item: ListCallerAccessGrantsResultTypeDef
        print(item)  # (3)
```

1. client: [S3ControlClient](./client.md)
2. paginator: [ListCallerAccessGrantsPaginator](./paginators.md#listcalleraccessgrantspaginator)
3. item: `AioPageIterator[ListCallerAccessGrantsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCallerAccessGrantsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountId: str,
    GrantScope: str = ...,
    AllowedByApplication: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCallerAccessGrantsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCallerAccessGrantsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCallerAccessGrantsRequestPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCallerAccessGrantsRequestPaginateTypeDef](./type_defs.md#listcalleraccessgrantsrequestpaginatetypedef)
