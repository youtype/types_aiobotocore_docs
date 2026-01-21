# Paginators

> [Index](../README.md) > [S3Vectors](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [S3Vectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors.html#s3vectors)
    type annotations stubs module [types-aiobotocore-s3vectors](https://pypi.org/project/types-aiobotocore-s3vectors/).

## ListIndexesPaginator

Type annotations and code completion for `#!python session.create_client("s3vectors").get_paginator("list_indexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/paginator/ListIndexes.html#S3Vectors.Paginator.ListIndexes)

```python
# ListIndexesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3vectors.paginator import ListIndexesPaginator

session = get_session()
async with session.create_client("s3vectors") as client:  # (1)
    paginator: ListIndexesPaginator = client.get_paginator("list_indexes")  # (2)
    async for item in paginator.paginate(...):
        item: ListIndexesOutputTypeDef
        print(item)  # (3)
```

1. client: [S3VectorsClient](./client.md)
2. paginator: [ListIndexesPaginator](./paginators.md#listindexespaginator)
3. item: `AioPageIterator[ListIndexesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIndexesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    vectorBucketName: str = ...,
    vectorBucketArn: str = ...,
    prefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIndexesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIndexesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIndexesInputPaginateTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIndexesInputPaginateTypeDef](./type_defs.md#listindexesinputpaginatetypedef)
## ListVectorBucketsPaginator

Type annotations and code completion for `#!python session.create_client("s3vectors").get_paginator("list_vector_buckets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/paginator/ListVectorBuckets.html#S3Vectors.Paginator.ListVectorBuckets)

```python
# ListVectorBucketsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3vectors.paginator import ListVectorBucketsPaginator

session = get_session()
async with session.create_client("s3vectors") as client:  # (1)
    paginator: ListVectorBucketsPaginator = client.get_paginator("list_vector_buckets")  # (2)
    async for item in paginator.paginate(...):
        item: ListVectorBucketsOutputTypeDef
        print(item)  # (3)
```

1. client: [S3VectorsClient](./client.md)
2. paginator: [ListVectorBucketsPaginator](./paginators.md#listvectorbucketspaginator)
3. item: `AioPageIterator[ListVectorBucketsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListVectorBucketsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    prefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListVectorBucketsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListVectorBucketsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListVectorBucketsInputPaginateTypeDef = {  # (1)
    "prefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVectorBucketsInputPaginateTypeDef](./type_defs.md#listvectorbucketsinputpaginatetypedef)
## ListVectorsPaginator

Type annotations and code completion for `#!python session.create_client("s3vectors").get_paginator("list_vectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors/paginator/ListVectors.html#S3Vectors.Paginator.ListVectors)

```python
# ListVectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3vectors.paginator import ListVectorsPaginator

session = get_session()
async with session.create_client("s3vectors") as client:  # (1)
    paginator: ListVectorsPaginator = client.get_paginator("list_vectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListVectorsOutputTypeDef
        print(item)  # (3)
```

1. client: [S3VectorsClient](./client.md)
2. paginator: [ListVectorsPaginator](./paginators.md#listvectorspaginator)
3. item: `AioPageIterator[ListVectorsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListVectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    vectorBucketName: str = ...,
    indexName: str = ...,
    indexArn: str = ...,
    segmentCount: int = ...,
    segmentIndex: int = ...,
    returnData: bool = ...,
    returnMetadata: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListVectorsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListVectorsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListVectorsInputPaginateTypeDef = {  # (1)
    "vectorBucketName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVectorsInputPaginateTypeDef](./type_defs.md#listvectorsinputpaginatetypedef)
