<a id="paginators-for-aiobotocore-s3-module"></a>

# Paginators for aiobotocore S3 module

> [Index](..) > [S3](.) > Paginators

Auto-generated documentation for
[S3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3)
type annotations stubs module
[types-aiobotocore-s3](https://pypi.org/project/types-aiobotocore-s3/).

- [Paginators for aiobotocore S3 module](#paginators-for-aiobotocore-s3-module)
  - [ListMultipartUploadsPaginator](#listmultipartuploadspaginator)
  - [ListObjectVersionsPaginator](#listobjectversionspaginator)
  - [ListObjectsPaginator](#listobjectspaginator)
  - [ListObjectsV2Paginator](#listobjectsv2paginator)
  - [ListPartsPaginator](#listpartspaginator)

<a id="listmultipartuploadspaginator"></a>

## ListMultipartUploadsPaginator

Type annotations for
`session.create_client("s3").get_paginator("list_multipart_uploads")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListMultipartUploadsPaginator

session = get_session()
async with session.create_client("s3") as client:
    client: S3Client
    paginator: ListMultipartUploadsPaginator = client.get_paginator("list_multipart_uploads")
```

Boto3 documentation:
[S3.Paginator.ListMultipartUploads](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListMultipartUploads)

Arguments for `ListMultipartUploadsPaginator.paginate` method:

- `Bucket`: `str` *(required)*
- `Delimiter`: `str`
- `EncodingType`: `Literal['url']` (see
  [EncodingTypeType](./literals.md#encodingtypetype))
- `Prefix`: `str`
- `ExpectedBucketOwner`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMultipartUploadsPaginator.paginate` returns
`_PageIterator`\[[ListMultipartUploadsOutputTypeDef](./type_defs.md#listmultipartuploadsoutputtypedef)\].

<a id="listobjectversionspaginator"></a>

## ListObjectVersionsPaginator

Type annotations for
`session.create_client("s3").get_paginator("list_object_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListObjectVersionsPaginator

session = get_session()
async with session.create_client("s3") as client:
    client: S3Client
    paginator: ListObjectVersionsPaginator = client.get_paginator("list_object_versions")
```

Boto3 documentation:
[S3.Paginator.ListObjectVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectVersions)

Arguments for `ListObjectVersionsPaginator.paginate` method:

- `Bucket`: `str` *(required)*
- `Delimiter`: `str`
- `EncodingType`: `Literal['url']` (see
  [EncodingTypeType](./literals.md#encodingtypetype))
- `Prefix`: `str`
- `ExpectedBucketOwner`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListObjectVersionsPaginator.paginate` returns
`_PageIterator`\[[ListObjectVersionsOutputTypeDef](./type_defs.md#listobjectversionsoutputtypedef)\].

<a id="listobjectspaginator"></a>

## ListObjectsPaginator

Type annotations for
`session.create_client("s3").get_paginator("list_objects")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListObjectsPaginator

session = get_session()
async with session.create_client("s3") as client:
    client: S3Client
    paginator: ListObjectsPaginator = client.get_paginator("list_objects")
```

Boto3 documentation:
[S3.Paginator.ListObjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjects)

Arguments for `ListObjectsPaginator.paginate` method:

- `Bucket`: `str` *(required)*
- `Delimiter`: `str`
- `EncodingType`: `Literal['url']` (see
  [EncodingTypeType](./literals.md#encodingtypetype))
- `Prefix`: `str`
- `RequestPayer`: `Literal['requester']` (see
  [RequestPayerType](./literals.md#requestpayertype))
- `ExpectedBucketOwner`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListObjectsPaginator.paginate` returns
`_PageIterator`\[[ListObjectsOutputTypeDef](./type_defs.md#listobjectsoutputtypedef)\].

<a id="listobjectsv2paginator"></a>

## ListObjectsV2Paginator

Type annotations for
`session.create_client("s3").get_paginator("list_objects_v2")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListObjectsV2Paginator

session = get_session()
async with session.create_client("s3") as client:
    client: S3Client
    paginator: ListObjectsV2Paginator = client.get_paginator("list_objects_v2")
```

Boto3 documentation:
[S3.Paginator.ListObjectsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListObjectsV2)

Arguments for `ListObjectsV2Paginator.paginate` method:

- `Bucket`: `str` *(required)*
- `Delimiter`: `str`
- `EncodingType`: `Literal['url']` (see
  [EncodingTypeType](./literals.md#encodingtypetype))
- `Prefix`: `str`
- `FetchOwner`: `bool`
- `StartAfter`: `str`
- `RequestPayer`: `Literal['requester']` (see
  [RequestPayerType](./literals.md#requestpayertype))
- `ExpectedBucketOwner`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListObjectsV2Paginator.paginate` returns
`_PageIterator`\[[ListObjectsV2OutputTypeDef](./type_defs.md#listobjectsv2outputtypedef)\].

<a id="listpartspaginator"></a>

## ListPartsPaginator

Type annotations for `session.create_client("s3").get_paginator("list_parts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_s3.paginator import ListPartsPaginator

session = get_session()
async with session.create_client("s3") as client:
    client: S3Client
    paginator: ListPartsPaginator = client.get_paginator("list_parts")
```

Boto3 documentation:
[S3.Paginator.ListParts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Paginator.ListParts)

Arguments for `ListPartsPaginator.paginate` method:

- `Bucket`: `str` *(required)*
- `Key`: `str` *(required)*
- `UploadId`: `str` *(required)*
- `RequestPayer`: `Literal['requester']` (see
  [RequestPayerType](./literals.md#requestpayertype))
- `ExpectedBucketOwner`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPartsPaginator.paginate` returns
`_PageIterator`\[[ListPartsOutputTypeDef](./type_defs.md#listpartsoutputtypedef)\].
