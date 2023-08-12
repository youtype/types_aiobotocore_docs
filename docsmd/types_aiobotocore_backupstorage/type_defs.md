# Type definitions

> [Index](../README.md) > [BackupStorage](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BackupStorage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
    type annotations stubs module [types-aiobotocore-backupstorage](https://pypi.org/project/types-aiobotocore-backupstorage/).

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


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## BackupObjectTypeDef

```python
# BackupObjectTypeDef definition

class BackupObjectTypeDef(TypedDict):
    Name: str,
    ObjectChecksum: str,
    ObjectChecksumAlgorithm: SummaryChecksumAlgorithmType,  # (1)
    ObjectToken: str,
    ChunksCount: NotRequired[int],
    MetadataString: NotRequired[str],
```

1. See [:material-code-brackets: SummaryChecksumAlgorithmType](./literals.md#summarychecksumalgorithmtype) 
## ChunkTypeDef

```python
# ChunkTypeDef definition

class ChunkTypeDef(TypedDict):
    Index: int,
    Length: int,
    Checksum: str,
    ChecksumAlgorithm: DataChecksumAlgorithmType,  # (1)
    ChunkToken: str,
```

1. See [:material-code-brackets: DataChecksumAlgorithmType](./literals.md#datachecksumalgorithmtype) 
## DeleteObjectInputRequestTypeDef

```python
# DeleteObjectInputRequestTypeDef definition

class DeleteObjectInputRequestTypeDef(TypedDict):
    BackupJobId: str,
    ObjectName: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## GetChunkInputRequestTypeDef

```python
# GetChunkInputRequestTypeDef definition

class GetChunkInputRequestTypeDef(TypedDict):
    StorageJobId: str,
    ChunkToken: str,
```

## GetObjectMetadataInputRequestTypeDef

```python
# GetObjectMetadataInputRequestTypeDef definition

class GetObjectMetadataInputRequestTypeDef(TypedDict):
    StorageJobId: str,
    ObjectToken: str,
```

## ListChunksInputRequestTypeDef

```python
# ListChunksInputRequestTypeDef definition

class ListChunksInputRequestTypeDef(TypedDict):
    StorageJobId: str,
    ObjectToken: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## StartObjectInputRequestTypeDef

```python
# StartObjectInputRequestTypeDef definition

class StartObjectInputRequestTypeDef(TypedDict):
    BackupJobId: str,
    ObjectName: str,
    ThrowOnDuplicate: NotRequired[bool],
```

## NotifyObjectCompleteInputRequestTypeDef

```python
# NotifyObjectCompleteInputRequestTypeDef definition

class NotifyObjectCompleteInputRequestTypeDef(TypedDict):
    BackupJobId: str,
    UploadId: str,
    ObjectChecksum: str,
    ObjectChecksumAlgorithm: SummaryChecksumAlgorithmType,  # (1)
    MetadataString: NotRequired[str],
    MetadataBlob: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    MetadataBlobLength: NotRequired[int],
    MetadataBlobChecksum: NotRequired[str],
    MetadataBlobChecksumAlgorithm: NotRequired[DataChecksumAlgorithmType],  # (2)
```

1. See [:material-code-brackets: SummaryChecksumAlgorithmType](./literals.md#summarychecksumalgorithmtype) 
2. See [:material-code-brackets: DataChecksumAlgorithmType](./literals.md#datachecksumalgorithmtype) 
## PutChunkInputRequestTypeDef

```python
# PutChunkInputRequestTypeDef definition

class PutChunkInputRequestTypeDef(TypedDict):
    BackupJobId: str,
    UploadId: str,
    ChunkIndex: int,
    Data: Union[str, bytes, IO[Any], StreamingBody],
    Length: int,
    Checksum: str,
    ChecksumAlgorithm: DataChecksumAlgorithmType,  # (1)
```

1. See [:material-code-brackets: DataChecksumAlgorithmType](./literals.md#datachecksumalgorithmtype) 
## PutObjectInputRequestTypeDef

```python
# PutObjectInputRequestTypeDef definition

class PutObjectInputRequestTypeDef(TypedDict):
    BackupJobId: str,
    ObjectName: str,
    MetadataString: NotRequired[str],
    InlineChunk: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    InlineChunkLength: NotRequired[int],
    InlineChunkChecksum: NotRequired[str],
    InlineChunkChecksumAlgorithm: NotRequired[str],
    ObjectChecksum: NotRequired[str],
    ObjectChecksumAlgorithm: NotRequired[SummaryChecksumAlgorithmType],  # (1)
    ThrowOnDuplicate: NotRequired[bool],
```

1. See [:material-code-brackets: SummaryChecksumAlgorithmType](./literals.md#summarychecksumalgorithmtype) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChunkOutputTypeDef

```python
# GetChunkOutputTypeDef definition

class GetChunkOutputTypeDef(TypedDict):
    Data: StreamingBody,
    Length: int,
    Checksum: str,
    ChecksumAlgorithm: DataChecksumAlgorithmType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataChecksumAlgorithmType](./literals.md#datachecksumalgorithmtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetObjectMetadataOutputTypeDef

```python
# GetObjectMetadataOutputTypeDef definition

class GetObjectMetadataOutputTypeDef(TypedDict):
    MetadataString: str,
    MetadataBlob: StreamingBody,
    MetadataBlobLength: int,
    MetadataBlobChecksum: str,
    MetadataBlobChecksumAlgorithm: DataChecksumAlgorithmType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataChecksumAlgorithmType](./literals.md#datachecksumalgorithmtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChunksOutputTypeDef

```python
# ListChunksOutputTypeDef definition

class ListChunksOutputTypeDef(TypedDict):
    ChunkList: List[ChunkTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChunkTypeDef](./type_defs.md#chunktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListObjectsOutputTypeDef

```python
# ListObjectsOutputTypeDef definition

class ListObjectsOutputTypeDef(TypedDict):
    ObjectList: List[BackupObjectTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupObjectTypeDef](./type_defs.md#backupobjecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotifyObjectCompleteOutputTypeDef

```python
# NotifyObjectCompleteOutputTypeDef definition

class NotifyObjectCompleteOutputTypeDef(TypedDict):
    ObjectChecksum: str,
    ObjectChecksumAlgorithm: SummaryChecksumAlgorithmType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SummaryChecksumAlgorithmType](./literals.md#summarychecksumalgorithmtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutChunkOutputTypeDef

```python
# PutChunkOutputTypeDef definition

class PutChunkOutputTypeDef(TypedDict):
    ChunkChecksum: str,
    ChunkChecksumAlgorithm: DataChecksumAlgorithmType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataChecksumAlgorithmType](./literals.md#datachecksumalgorithmtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutObjectOutputTypeDef

```python
# PutObjectOutputTypeDef definition

class PutObjectOutputTypeDef(TypedDict):
    InlineChunkChecksum: str,
    InlineChunkChecksumAlgorithm: DataChecksumAlgorithmType,  # (1)
    ObjectChecksum: str,
    ObjectChecksumAlgorithm: SummaryChecksumAlgorithmType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DataChecksumAlgorithmType](./literals.md#datachecksumalgorithmtype) 
2. See [:material-code-brackets: SummaryChecksumAlgorithmType](./literals.md#summarychecksumalgorithmtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartObjectOutputTypeDef

```python
# StartObjectOutputTypeDef definition

class StartObjectOutputTypeDef(TypedDict):
    UploadId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListObjectsInputRequestTypeDef

```python
# ListObjectsInputRequestTypeDef definition

class ListObjectsInputRequestTypeDef(TypedDict):
    StorageJobId: str,
    StartingObjectName: NotRequired[str],
    StartingObjectPrefix: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    CreatedBefore: NotRequired[Union[datetime, str]],
    CreatedAfter: NotRequired[Union[datetime, str]],
```

