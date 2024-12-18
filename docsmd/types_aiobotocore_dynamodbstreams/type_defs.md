# Type definitions

> [Index](../README.md) > [DynamoDBStreams](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DynamoDBStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#dynamodbstreams)
    type annotations stubs module [types-aiobotocore-dynamodbstreams](https://pypi.org/project/types-aiobotocore-dynamodbstreams/).



## AttributeValueTypeDef

```python
# AttributeValueTypeDef definition

class AttributeValueTypeDef(TypedDict):
    S: NotRequired[str],
    N: NotRequired[str],
    B: NotRequired[bytes],
    SS: NotRequired[List[str]],
    NS: NotRequired[List[str]],
    BS: NotRequired[List[bytes]],
    M: NotRequired[Dict[str, Dict[str, Any]]],
    L: NotRequired[List[Dict[str, Any]]],
    NULL: NotRequired[bool],
    BOOL: NotRequired[bool],
```

## DescribeStreamInputRequestTypeDef

```python
# DescribeStreamInputRequestTypeDef definition

class DescribeStreamInputRequestTypeDef(TypedDict):
    StreamArn: str,
    Limit: NotRequired[int],
    ExclusiveStartShardId: NotRequired[str],
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

## GetRecordsInputRequestTypeDef

```python
# GetRecordsInputRequestTypeDef definition

class GetRecordsInputRequestTypeDef(TypedDict):
    ShardIterator: str,
    Limit: NotRequired[int],
```

## GetShardIteratorInputRequestTypeDef

```python
# GetShardIteratorInputRequestTypeDef definition

class GetShardIteratorInputRequestTypeDef(TypedDict):
    StreamArn: str,
    ShardId: str,
    ShardIteratorType: ShardIteratorTypeType,  # (1)
    SequenceNumber: NotRequired[str],
```

1. See [:material-code-brackets: ShardIteratorTypeType](./literals.md#sharditeratortypetype) 
## IdentityTypeDef

```python
# IdentityTypeDef definition

class IdentityTypeDef(TypedDict):
    PrincipalId: NotRequired[str],
    Type: NotRequired[str],
```

## KeySchemaElementTypeDef

```python
# KeySchemaElementTypeDef definition

class KeySchemaElementTypeDef(TypedDict):
    AttributeName: str,
    KeyType: KeyTypeType,  # (1)
```

1. See [:material-code-brackets: KeyTypeType](./literals.md#keytypetype) 
## ListStreamsInputRequestTypeDef

```python
# ListStreamsInputRequestTypeDef definition

class ListStreamsInputRequestTypeDef(TypedDict):
    TableName: NotRequired[str],
    Limit: NotRequired[int],
    ExclusiveStartStreamArn: NotRequired[str],
```

## StreamTypeDef

```python
# StreamTypeDef definition

class StreamTypeDef(TypedDict):
    StreamArn: NotRequired[str],
    TableName: NotRequired[str],
    StreamLabel: NotRequired[str],
```

## SequenceNumberRangeTypeDef

```python
# SequenceNumberRangeTypeDef definition

class SequenceNumberRangeTypeDef(TypedDict):
    StartingSequenceNumber: NotRequired[str],
    EndingSequenceNumber: NotRequired[str],
```

## StreamRecordTypeDef

```python
# StreamRecordTypeDef definition

class StreamRecordTypeDef(TypedDict):
    ApproximateCreationDateTime: NotRequired[datetime],
    Keys: NotRequired[Dict[str, AttributeValueTypeDef]],  # (1)
    NewImage: NotRequired[Dict[str, AttributeValueTypeDef]],  # (1)
    OldImage: NotRequired[Dict[str, AttributeValueTypeDef]],  # (1)
    SequenceNumber: NotRequired[str],
    SizeBytes: NotRequired[int],
    StreamViewType: NotRequired[StreamViewTypeType],  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
4. See [:material-code-brackets: StreamViewTypeType](./literals.md#streamviewtypetype) 
## GetShardIteratorOutputTypeDef

```python
# GetShardIteratorOutputTypeDef definition

class GetShardIteratorOutputTypeDef(TypedDict):
    ShardIterator: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStreamsOutputTypeDef

```python
# ListStreamsOutputTypeDef definition

class ListStreamsOutputTypeDef(TypedDict):
    Streams: List[StreamTypeDef],  # (1)
    LastEvaluatedStreamArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamTypeDef](./type_defs.md#streamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ShardTypeDef

```python
# ShardTypeDef definition

class ShardTypeDef(TypedDict):
    ShardId: NotRequired[str],
    SequenceNumberRange: NotRequired[SequenceNumberRangeTypeDef],  # (1)
    ParentShardId: NotRequired[str],
```

1. See [:material-code-braces: SequenceNumberRangeTypeDef](./type_defs.md#sequencenumberrangetypedef) 
## RecordTypeDef

```python
# RecordTypeDef definition

class RecordTypeDef(TypedDict):
    eventID: NotRequired[str],
    eventName: NotRequired[OperationTypeType],  # (1)
    eventVersion: NotRequired[str],
    eventSource: NotRequired[str],
    awsRegion: NotRequired[str],
    dynamodb: NotRequired[StreamRecordTypeDef],  # (2)
    userIdentity: NotRequired[IdentityTypeDef],  # (3)
```

1. See [:material-code-brackets: OperationTypeType](./literals.md#operationtypetype) 
2. See [:material-code-braces: StreamRecordTypeDef](./type_defs.md#streamrecordtypedef) 
3. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
## StreamDescriptionTypeDef

```python
# StreamDescriptionTypeDef definition

class StreamDescriptionTypeDef(TypedDict):
    StreamArn: NotRequired[str],
    StreamLabel: NotRequired[str],
    StreamStatus: NotRequired[StreamStatusType],  # (1)
    StreamViewType: NotRequired[StreamViewTypeType],  # (2)
    CreationRequestDateTime: NotRequired[datetime],
    TableName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (3)
    Shards: NotRequired[List[ShardTypeDef]],  # (4)
    LastEvaluatedShardId: NotRequired[str],
```

1. See [:material-code-brackets: StreamStatusType](./literals.md#streamstatustype) 
2. See [:material-code-brackets: StreamViewTypeType](./literals.md#streamviewtypetype) 
3. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
4. See [:material-code-braces: ShardTypeDef](./type_defs.md#shardtypedef) 
## GetRecordsOutputTypeDef

```python
# GetRecordsOutputTypeDef definition

class GetRecordsOutputTypeDef(TypedDict):
    Records: List[RecordTypeDef],  # (1)
    NextShardIterator: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStreamOutputTypeDef

```python
# DescribeStreamOutputTypeDef definition

class DescribeStreamOutputTypeDef(TypedDict):
    StreamDescription: StreamDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StreamDescriptionTypeDef](./type_defs.md#streamdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
