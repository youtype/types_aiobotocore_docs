# Type definitions

> [Index](../README.md) > [EBS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EBS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
    type annotations stubs module [types-aiobotocore-ebs](https://pypi.org/project/types-aiobotocore-ebs/).

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




## BlockTypeDef

```python
# BlockTypeDef definition

class BlockTypeDef(TypedDict):
    BlockIndex: NotRequired[int],
    BlockToken: NotRequired[str],
```

## ChangedBlockTypeDef

```python
# ChangedBlockTypeDef definition

class ChangedBlockTypeDef(TypedDict):
    BlockIndex: NotRequired[int],
    FirstBlockToken: NotRequired[str],
    SecondBlockToken: NotRequired[str],
```

## CompleteSnapshotRequestRequestTypeDef

```python
# CompleteSnapshotRequestRequestTypeDef definition

class CompleteSnapshotRequestRequestTypeDef(TypedDict):
    SnapshotId: str,
    ChangedBlocksCount: int,
    Checksum: NotRequired[str],
    ChecksumAlgorithm: NotRequired[ChecksumAlgorithmType],  # (1)
    ChecksumAggregationMethod: NotRequired[ChecksumAggregationMethodType],  # (2)
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-brackets: ChecksumAggregationMethodType](./literals.md#checksumaggregationmethodtype) 
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

## GetSnapshotBlockRequestRequestTypeDef

```python
# GetSnapshotBlockRequestRequestTypeDef definition

class GetSnapshotBlockRequestRequestTypeDef(TypedDict):
    SnapshotId: str,
    BlockIndex: int,
    BlockToken: str,
```

## ListChangedBlocksRequestRequestTypeDef

```python
# ListChangedBlocksRequestRequestTypeDef definition

class ListChangedBlocksRequestRequestTypeDef(TypedDict):
    SecondSnapshotId: str,
    FirstSnapshotId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    StartingBlockIndex: NotRequired[int],
```

## ListSnapshotBlocksRequestRequestTypeDef

```python
# ListSnapshotBlocksRequestRequestTypeDef definition

class ListSnapshotBlocksRequestRequestTypeDef(TypedDict):
    SnapshotId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    StartingBlockIndex: NotRequired[int],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## PutSnapshotBlockRequestRequestTypeDef

```python
# PutSnapshotBlockRequestRequestTypeDef definition

class PutSnapshotBlockRequestRequestTypeDef(TypedDict):
    SnapshotId: str,
    BlockIndex: int,
    BlockData: Union[str, bytes, IO[Any], StreamingBody],
    DataLength: int,
    Checksum: str,
    ChecksumAlgorithm: ChecksumAlgorithmType,  # (1)
    Progress: NotRequired[int],
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
## CompleteSnapshotResponseTypeDef

```python
# CompleteSnapshotResponseTypeDef definition

class CompleteSnapshotResponseTypeDef(TypedDict):
    Status: StatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSnapshotBlockResponseTypeDef

```python
# GetSnapshotBlockResponseTypeDef definition

class GetSnapshotBlockResponseTypeDef(TypedDict):
    DataLength: int,
    BlockData: StreamingBody,
    Checksum: str,
    ChecksumAlgorithm: ChecksumAlgorithmType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChangedBlocksResponseTypeDef

```python
# ListChangedBlocksResponseTypeDef definition

class ListChangedBlocksResponseTypeDef(TypedDict):
    ChangedBlocks: List[ChangedBlockTypeDef],  # (1)
    ExpiryTime: datetime,
    VolumeSize: int,
    BlockSize: int,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangedBlockTypeDef](./type_defs.md#changedblocktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSnapshotBlocksResponseTypeDef

```python
# ListSnapshotBlocksResponseTypeDef definition

class ListSnapshotBlocksResponseTypeDef(TypedDict):
    Blocks: List[BlockTypeDef],  # (1)
    ExpiryTime: datetime,
    VolumeSize: int,
    BlockSize: int,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlockTypeDef](./type_defs.md#blocktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSnapshotBlockResponseTypeDef

```python
# PutSnapshotBlockResponseTypeDef definition

class PutSnapshotBlockResponseTypeDef(TypedDict):
    Checksum: str,
    ChecksumAlgorithm: ChecksumAlgorithmType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ChecksumAlgorithmType](./literals.md#checksumalgorithmtype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSnapshotRequestRequestTypeDef

```python
# StartSnapshotRequestRequestTypeDef definition

class StartSnapshotRequestRequestTypeDef(TypedDict):
    VolumeSize: int,
    ParentSnapshotId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    Encrypted: NotRequired[bool],
    KmsKeyArn: NotRequired[str],
    Timeout: NotRequired[int],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StartSnapshotResponseTypeDef

```python
# StartSnapshotResponseTypeDef definition

class StartSnapshotResponseTypeDef(TypedDict):
    Description: str,
    SnapshotId: str,
    OwnerId: str,
    Status: StatusType,  # (1)
    StartTime: datetime,
    VolumeSize: int,
    BlockSize: int,
    Tags: List[TagTypeDef],  # (2)
    ParentSnapshotId: str,
    KmsKeyArn: str,
    SseType: SSETypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: SSETypeType](./literals.md#ssetypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
