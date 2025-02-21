# Paginators

> [Index](../README.md) > [S3](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [S3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#s3)
    type annotations stubs module [types-aiobotocore-s3](https://pypi.org/project/types-aiobotocore-s3/).

## ListBucketsPaginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_buckets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/paginator/ListBuckets.html#S3.Paginator.ListBuckets)

```python
# ListBucketsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListBucketsPaginator

session = get_session()
async with session.create_client("s3") as client:  # (1)
    paginator: ListBucketsPaginator = client.get_paginator("list_buckets")  # (2)
    async for item in paginator.paginate(...):
        item: ListBucketsOutputTypeDef
        print(item)  # (3)
```

1. client: [S3Client](./client.md)
2. paginator: [ListBucketsPaginator](./paginators.md#listbucketspaginator)
3. item: [:material-code-braces: ListBucketsOutputTypeDef](./type_defs.md#listbucketsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBucketsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Prefix: str = ...,
    BucketRegion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBucketsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBucketsOutputTypeDef](./type_defs.md#listbucketsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBucketsRequestPaginateTypeDef = {  # (1)
    "Prefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBucketsRequestPaginateTypeDef](./type_defs.md#listbucketsrequestpaginatetypedef) 
## ListDirectoryBucketsPaginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_directory_buckets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/paginator/ListDirectoryBuckets.html#S3.Paginator.ListDirectoryBuckets)

```python
# ListDirectoryBucketsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListDirectoryBucketsPaginator

session = get_session()
async with session.create_client("s3") as client:  # (1)
    paginator: ListDirectoryBucketsPaginator = client.get_paginator("list_directory_buckets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDirectoryBucketsOutputTypeDef
        print(item)  # (3)
```

1. client: [S3Client](./client.md)
2. paginator: [ListDirectoryBucketsPaginator](./paginators.md#listdirectorybucketspaginator)
3. item: [:material-code-braces: ListDirectoryBucketsOutputTypeDef](./type_defs.md#listdirectorybucketsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListDirectoryBucketsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDirectoryBucketsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDirectoryBucketsOutputTypeDef](./type_defs.md#listdirectorybucketsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDirectoryBucketsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDirectoryBucketsRequestPaginateTypeDef](./type_defs.md#listdirectorybucketsrequestpaginatetypedef) 
## ListMultipartUploadsPaginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_multipart_uploads")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/paginator/ListMultipartUploads.html#S3.Paginator.ListMultipartUploads)

```python
# ListMultipartUploadsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListMultipartUploadsPaginator

session = get_session()
async with session.create_client("s3") as client:  # (1)
    paginator: ListMultipartUploadsPaginator = client.get_paginator("list_multipart_uploads")  # (2)
    async for item in paginator.paginate(...):
        item: ListMultipartUploadsOutputTypeDef
        print(item)  # (3)
```

1. client: [S3Client](./client.md)
2. paginator: [ListMultipartUploadsPaginator](./paginators.md#listmultipartuploadspaginator)
3. item: [:material-code-braces: ListMultipartUploadsOutputTypeDef](./type_defs.md#listmultipartuploadsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListMultipartUploadsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Bucket: str,
    Delimiter: str = ...,
    EncodingType: EncodingTypeType = ...,  # (1)
    Prefix: str = ...,
    ExpectedBucketOwner: str = ...,
    RequestPayer: RequestPayerType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListMultipartUploadsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListMultipartUploadsOutputTypeDef](./type_defs.md#listmultipartuploadsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMultipartUploadsRequestPaginateTypeDef = {  # (1)
    "Bucket": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMultipartUploadsRequestPaginateTypeDef](./type_defs.md#listmultipartuploadsrequestpaginatetypedef) 
## ListObjectVersionsPaginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_object_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/paginator/ListObjectVersions.html#S3.Paginator.ListObjectVersions)

```python
# ListObjectVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListObjectVersionsPaginator

session = get_session()
async with session.create_client("s3") as client:  # (1)
    paginator: ListObjectVersionsPaginator = client.get_paginator("list_object_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListObjectVersionsOutputTypeDef
        print(item)  # (3)
```

1. client: [S3Client](./client.md)
2. paginator: [ListObjectVersionsPaginator](./paginators.md#listobjectversionspaginator)
3. item: [:material-code-braces: ListObjectVersionsOutputTypeDef](./type_defs.md#listobjectversionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListObjectVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Bucket: str,
    Delimiter: str = ...,
    EncodingType: EncodingTypeType = ...,  # (1)
    Prefix: str = ...,
    ExpectedBucketOwner: str = ...,
    RequestPayer: RequestPayerType = ...,  # (2)
    OptionalObjectAttributes: Sequence[OptionalObjectAttributesType] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListObjectVersionsOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: OptionalObjectAttributesType](./literals.md#optionalobjectattributestype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListObjectVersionsOutputTypeDef](./type_defs.md#listobjectversionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListObjectVersionsRequestPaginateTypeDef = {  # (1)
    "Bucket": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectVersionsRequestPaginateTypeDef](./type_defs.md#listobjectversionsrequestpaginatetypedef) 
## ListObjectsPaginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_objects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/paginator/ListObjects.html#S3.Paginator.ListObjects)

```python
# ListObjectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListObjectsPaginator

session = get_session()
async with session.create_client("s3") as client:  # (1)
    paginator: ListObjectsPaginator = client.get_paginator("list_objects")  # (2)
    async for item in paginator.paginate(...):
        item: ListObjectsOutputTypeDef
        print(item)  # (3)
```

1. client: [S3Client](./client.md)
2. paginator: [ListObjectsPaginator](./paginators.md#listobjectspaginator)
3. item: [:material-code-braces: ListObjectsOutputTypeDef](./type_defs.md#listobjectsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListObjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Bucket: str,
    Delimiter: str = ...,
    EncodingType: EncodingTypeType = ...,  # (1)
    Prefix: str = ...,
    RequestPayer: RequestPayerType = ...,  # (2)
    ExpectedBucketOwner: str = ...,
    OptionalObjectAttributes: Sequence[OptionalObjectAttributesType] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListObjectsOutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: OptionalObjectAttributesType](./literals.md#optionalobjectattributestype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListObjectsOutputTypeDef](./type_defs.md#listobjectsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListObjectsRequestPaginateTypeDef = {  # (1)
    "Bucket": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectsRequestPaginateTypeDef](./type_defs.md#listobjectsrequestpaginatetypedef) 
## ListObjectsV2Paginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_objects_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/paginator/ListObjectsV2.html#S3.Paginator.ListObjectsV2)

```python
# ListObjectsV2Paginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListObjectsV2Paginator

session = get_session()
async with session.create_client("s3") as client:  # (1)
    paginator: ListObjectsV2Paginator = client.get_paginator("list_objects_v2")  # (2)
    async for item in paginator.paginate(...):
        item: ListObjectsV2OutputTypeDef
        print(item)  # (3)
```

1. client: [S3Client](./client.md)
2. paginator: [ListObjectsV2Paginator](./paginators.md#listobjectsv2paginator)
3. item: [:material-code-braces: ListObjectsV2OutputTypeDef](./type_defs.md#listobjectsv2outputtypedef) 


### paginate

Type annotations and code completion for `#!python ListObjectsV2Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Bucket: str,
    Delimiter: str = ...,
    EncodingType: EncodingTypeType = ...,  # (1)
    Prefix: str = ...,
    FetchOwner: bool = ...,
    StartAfter: str = ...,
    RequestPayer: RequestPayerType = ...,  # (2)
    ExpectedBucketOwner: str = ...,
    OptionalObjectAttributes: Sequence[OptionalObjectAttributesType] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListObjectsV2OutputTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-brackets: OptionalObjectAttributesType](./literals.md#optionalobjectattributestype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListObjectsV2OutputTypeDef](./type_defs.md#listobjectsv2outputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListObjectsV2RequestPaginateTypeDef = {  # (1)
    "Bucket": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectsV2RequestPaginateTypeDef](./type_defs.md#listobjectsv2requestpaginatetypedef) 
## ListPartsPaginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_parts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/paginator/ListParts.html#S3.Paginator.ListParts)

```python
# ListPartsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListPartsPaginator

session = get_session()
async with session.create_client("s3") as client:  # (1)
    paginator: ListPartsPaginator = client.get_paginator("list_parts")  # (2)
    async for item in paginator.paginate(...):
        item: ListPartsOutputTypeDef
        print(item)  # (3)
```

1. client: [S3Client](./client.md)
2. paginator: [ListPartsPaginator](./paginators.md#listpartspaginator)
3. item: [:material-code-braces: ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPartsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Bucket: str,
    Key: str,
    UploadId: str,
    RequestPayer: RequestPayerType = ...,  # (1)
    ExpectedBucketOwner: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: Union[str, bytes] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListPartsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPartsRequestPaginateTypeDef = {  # (1)
    "Bucket": ...,
    "Key": ...,
    "UploadId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPartsRequestPaginateTypeDef](./type_defs.md#listpartsrequestpaginatetypedef) 
