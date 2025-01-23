# Type definitions

> [Index](../README.md) > [MediaStoreData](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MediaStoreData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#mediastoredata)
    type annotations stubs module [types-aiobotocore-mediastore-data](https://pypi.org/project/types-aiobotocore-mediastore-data/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## DeleteObjectRequestRequestTypeDef

```python
# DeleteObjectRequestRequestTypeDef definition

class DeleteObjectRequestRequestTypeDef(TypedDict):
    Path: str,
```

## DescribeObjectRequestRequestTypeDef

```python
# DescribeObjectRequestRequestTypeDef definition

class DescribeObjectRequestRequestTypeDef(TypedDict):
    Path: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## GetObjectRequestRequestTypeDef

```python
# GetObjectRequestRequestTypeDef definition

class GetObjectRequestRequestTypeDef(TypedDict):
    Path: str,
    Range: NotRequired[str],
```

## ItemTypeDef

```python
# ItemTypeDef definition

class ItemTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[ItemTypeType],  # (1)
    ETag: NotRequired[str],
    LastModified: NotRequired[datetime],
    ContentType: NotRequired[str],
    ContentLength: NotRequired[int],
```

1. See [:material-code-brackets: ItemTypeType](./literals.md#itemtypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListItemsRequestRequestTypeDef

```python
# ListItemsRequestRequestTypeDef definition

class ListItemsRequestRequestTypeDef(TypedDict):
    Path: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## PutObjectRequestRequestTypeDef

```python
# PutObjectRequestRequestTypeDef definition

class PutObjectRequestRequestTypeDef(TypedDict):
    Body: BlobTypeDef,
    Path: str,
    ContentType: NotRequired[str],
    CacheControl: NotRequired[str],
    StorageClass: NotRequired[StorageClassType],  # (1)
    UploadAvailability: NotRequired[UploadAvailabilityType],  # (2)
```

1. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
2. See [:material-code-brackets: UploadAvailabilityType](./literals.md#uploadavailabilitytype) 
## DescribeObjectResponseTypeDef

```python
# DescribeObjectResponseTypeDef definition

class DescribeObjectResponseTypeDef(TypedDict):
    ETag: str,
    ContentType: str,
    ContentLength: int,
    CacheControl: str,
    LastModified: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetObjectResponseTypeDef

```python
# GetObjectResponseTypeDef definition

class GetObjectResponseTypeDef(TypedDict):
    Body: StreamingBody,
    CacheControl: str,
    ContentRange: str,
    ContentLength: int,
    ContentType: str,
    ETag: str,
    LastModified: datetime,
    StatusCode: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectResponseTypeDef

```python
# PutObjectResponseTypeDef definition

class PutObjectResponseTypeDef(TypedDict):
    ContentSHA256: str,
    ETag: str,
    StorageClass: StorageClassType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StorageClassType](./literals.md#storageclasstype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListItemsResponseTypeDef

```python
# ListItemsResponseTypeDef definition

class ListItemsResponseTypeDef(TypedDict):
    Items: List[ItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ItemTypeDef](./type_defs.md#itemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListItemsRequestPaginateTypeDef

```python
# ListItemsRequestPaginateTypeDef definition

class ListItemsRequestPaginateTypeDef(TypedDict):
    Path: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
