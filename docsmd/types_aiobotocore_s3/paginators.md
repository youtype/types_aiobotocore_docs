# Paginators

> [Index](../README.md) > [S3](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [S3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
    type annotations stubs module [types-aiobotocore-s3](https://pypi.org/project/types-aiobotocore-s3/).

## ListMultipartUploadsPaginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_multipart_uploads")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    Bucket: str,
    Delimiter: str = ...,
    EncodingType: EncodingTypeType = ...,  # (1)
    Prefix: str = ...,
    ExpectedBucketOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListMultipartUploadsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListMultipartUploadsOutputTypeDef](./type_defs.md#listmultipartuploadsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef = {  # (1)
    "Bucket": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMultipartUploadsRequestListMultipartUploadsPaginateTypeDef](./type_defs.md#listmultipartuploadsrequestlistmultipartuploadspaginatetypedef) 
## ListObjectVersionsPaginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_object_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    Bucket: str,
    Delimiter: str = ...,
    EncodingType: EncodingTypeType = ...,  # (1)
    Prefix: str = ...,
    ExpectedBucketOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListObjectVersionsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListObjectVersionsOutputTypeDef](./type_defs.md#listobjectversionsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListObjectVersionsRequestListObjectVersionsPaginateTypeDef = {  # (1)
    "Bucket": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectVersionsRequestListObjectVersionsPaginateTypeDef](./type_defs.md#listobjectversionsrequestlistobjectversionspaginatetypedef) 
## ListObjectsPaginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_objects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    Bucket: str,
    Delimiter: str = ...,
    EncodingType: EncodingTypeType = ...,  # (1)
    Prefix: str = ...,
    RequestPayer: RequestPayerType = ...,  # (2)
    ExpectedBucketOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListObjectsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListObjectsOutputTypeDef](./type_defs.md#listobjectsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListObjectsRequestListObjectsPaginateTypeDef = {  # (1)
    "Bucket": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectsRequestListObjectsPaginateTypeDef](./type_defs.md#listobjectsrequestlistobjectspaginatetypedef) 
## ListObjectsV2Paginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_objects_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2)

```python title="Usage example"
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

```python title="Method definition"
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
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListObjectsV2OutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: EncodingTypeType](./literals.md#encodingtypetype) 
2. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListObjectsV2OutputTypeDef](./type_defs.md#listobjectsv2outputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListObjectsV2RequestListObjectsV2PaginateTypeDef = {  # (1)
    "Bucket": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectsV2RequestListObjectsV2PaginateTypeDef](./type_defs.md#listobjectsv2requestlistobjectsv2paginatetypedef) 
## ListPartsPaginator

Type annotations and code completion for `#!python session.create_client("s3").get_paginator("list_parts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    Bucket: str,
    Key: str,
    UploadId: str,
    RequestPayer: RequestPayerType = ...,  # (1)
    ExpectedBucketOwner: str = ...,
    SSECustomerAlgorithm: str = ...,
    SSECustomerKey: str = ...,
    SSECustomerKeyMD5: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPartsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: RequestPayerType](./literals.md#requestpayertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListPartsRequestListPartsPaginateTypeDef = {  # (1)
    "Bucket": ...,
    "Key": ...,
    "UploadId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPartsRequestListPartsPaginateTypeDef](./type_defs.md#listpartsrequestlistpartspaginatetypedef) 
