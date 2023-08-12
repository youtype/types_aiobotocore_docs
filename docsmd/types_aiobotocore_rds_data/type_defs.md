# Type definitions

> [Index](../README.md) > [RDSDataService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RDSDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#RDSDataService)
    type annotations stubs module [types-aiobotocore-rds-data](https://pypi.org/project/types-aiobotocore-rds-data/).

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




## ArrayValueTypeDef

```python
# ArrayValueTypeDef definition

class ArrayValueTypeDef(TypedDict):
    booleanValues: NotRequired[Sequence[bool]],
    longValues: NotRequired[Sequence[int]],
    doubleValues: NotRequired[Sequence[float]],
    stringValues: NotRequired[Sequence[str]],
    arrayValues: NotRequired[Sequence[ArrayValueTypeDef]],  # (1)
```

1. See [:material-code-braces: ArrayValueTypeDef](./type_defs.md#arrayvaluetypedef) 
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

## BeginTransactionRequestRequestTypeDef

```python
# BeginTransactionRequestRequestTypeDef definition

class BeginTransactionRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    secretArn: str,
    database: NotRequired[str],
    schema: NotRequired[str],
```

## ColumnMetadataTypeDef

```python
# ColumnMetadataTypeDef definition

class ColumnMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[int],
    typeName: NotRequired[str],
    label: NotRequired[str],
    schemaName: NotRequired[str],
    tableName: NotRequired[str],
    isAutoIncrement: NotRequired[bool],
    isSigned: NotRequired[bool],
    isCurrency: NotRequired[bool],
    isCaseSensitive: NotRequired[bool],
    nullable: NotRequired[int],
    precision: NotRequired[int],
    scale: NotRequired[int],
    arrayBaseColumnType: NotRequired[int],
```

## CommitTransactionRequestRequestTypeDef

```python
# CommitTransactionRequestRequestTypeDef definition

class CommitTransactionRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    secretArn: str,
    transactionId: str,
```

## ExecuteSqlRequestRequestTypeDef

```python
# ExecuteSqlRequestRequestTypeDef definition

class ExecuteSqlRequestRequestTypeDef(TypedDict):
    dbClusterOrInstanceArn: str,
    awsSecretStoreArn: str,
    sqlStatements: str,
    database: NotRequired[str],
    schema: NotRequired[str],
```

## ResultSetOptionsTypeDef

```python
# ResultSetOptionsTypeDef definition

class ResultSetOptionsTypeDef(TypedDict):
    decimalReturnType: NotRequired[DecimalReturnTypeType],  # (1)
    longReturnType: NotRequired[LongReturnTypeType],  # (2)
```

1. See [:material-code-brackets: DecimalReturnTypeType](./literals.md#decimalreturntypetype) 
2. See [:material-code-brackets: LongReturnTypeType](./literals.md#longreturntypetype) 
## RecordTypeDef

```python
# RecordTypeDef definition

class RecordTypeDef(TypedDict):
    values: NotRequired[List[ValueTypeDef]],  # (1)
```

1. See [:material-code-braces: ValueTypeDef](./type_defs.md#valuetypedef) 
## RollbackTransactionRequestRequestTypeDef

```python
# RollbackTransactionRequestRequestTypeDef definition

class RollbackTransactionRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    secretArn: str,
    transactionId: str,
```

## StructValueTypeDef

```python
# StructValueTypeDef definition

class StructValueTypeDef(TypedDict):
    attributes: NotRequired[List[ValueTypeDef]],  # (1)
```

1. See [:material-code-braces: ValueTypeDef](./type_defs.md#valuetypedef) 
## ValueTypeDef

```python
# ValueTypeDef definition

class ValueTypeDef(TypedDict):
    isNull: NotRequired[bool],
    bitValue: NotRequired[bool],
    bigIntValue: NotRequired[int],
    intValue: NotRequired[int],
    doubleValue: NotRequired[float],
    realValue: NotRequired[float],
    stringValue: NotRequired[str],
    blobValue: NotRequired[bytes],
    arrayValues: NotRequired[List[ValueTypeDef]],  # (1)
    structValue: NotRequired[StructValueTypeDef],  # (2)
```

1. See [:material-code-braces: ValueTypeDef](./type_defs.md#valuetypedef) 
2. See [:material-code-braces: StructValueTypeDef](./type_defs.md#structvaluetypedef) 
## BeginTransactionResponseTypeDef

```python
# BeginTransactionResponseTypeDef definition

class BeginTransactionResponseTypeDef(TypedDict):
    transactionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CommitTransactionResponseTypeDef

```python
# CommitTransactionResponseTypeDef definition

class CommitTransactionResponseTypeDef(TypedDict):
    transactionStatus: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RollbackTransactionResponseTypeDef

```python
# RollbackTransactionResponseTypeDef definition

class RollbackTransactionResponseTypeDef(TypedDict):
    transactionStatus: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FieldTypeDef

```python
# FieldTypeDef definition

class FieldTypeDef(TypedDict):
    isNull: NotRequired[bool],
    booleanValue: NotRequired[bool],
    longValue: NotRequired[int],
    doubleValue: NotRequired[float],
    stringValue: NotRequired[str],
    blobValue: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    arrayValue: NotRequired[ArrayValueTypeDef],  # (1)
```

1. See [:material-code-braces: ArrayValueTypeDef](./type_defs.md#arrayvaluetypedef) 
## ResultSetMetadataTypeDef

```python
# ResultSetMetadataTypeDef definition

class ResultSetMetadataTypeDef(TypedDict):
    columnCount: NotRequired[int],
    columnMetadata: NotRequired[List[ColumnMetadataTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef) 
## ExecuteStatementResponseTypeDef

```python
# ExecuteStatementResponseTypeDef definition

class ExecuteStatementResponseTypeDef(TypedDict):
    records: List[List[FieldTypeDef]],  # (1)
    columnMetadata: List[ColumnMetadataTypeDef],  # (2)
    numberOfRecordsUpdated: int,
    generatedFields: List[FieldTypeDef],  # (3)
    formattedRecords: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
2. See [:material-code-braces: ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef) 
3. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SqlParameterTypeDef

```python
# SqlParameterTypeDef definition

class SqlParameterTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[FieldTypeDef],  # (1)
    typeHint: NotRequired[TypeHintType],  # (2)
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
2. See [:material-code-brackets: TypeHintType](./literals.md#typehinttype) 
## UpdateResultTypeDef

```python
# UpdateResultTypeDef definition

class UpdateResultTypeDef(TypedDict):
    generatedFields: NotRequired[List[FieldTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
## ResultFrameTypeDef

```python
# ResultFrameTypeDef definition

class ResultFrameTypeDef(TypedDict):
    resultSetMetadata: NotRequired[ResultSetMetadataTypeDef],  # (1)
    records: NotRequired[List[RecordTypeDef]],  # (2)
```

1. See [:material-code-braces: ResultSetMetadataTypeDef](./type_defs.md#resultsetmetadatatypedef) 
2. See [:material-code-braces: RecordTypeDef](./type_defs.md#recordtypedef) 
## BatchExecuteStatementRequestRequestTypeDef

```python
# BatchExecuteStatementRequestRequestTypeDef definition

class BatchExecuteStatementRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    secretArn: str,
    sql: str,
    database: NotRequired[str],
    schema: NotRequired[str],
    parameterSets: NotRequired[Sequence[Sequence[SqlParameterTypeDef]]],  # (1)
    transactionId: NotRequired[str],
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
## ExecuteStatementRequestRequestTypeDef

```python
# ExecuteStatementRequestRequestTypeDef definition

class ExecuteStatementRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    secretArn: str,
    sql: str,
    database: NotRequired[str],
    schema: NotRequired[str],
    parameters: NotRequired[Sequence[SqlParameterTypeDef]],  # (1)
    transactionId: NotRequired[str],
    includeResultMetadata: NotRequired[bool],
    continueAfterTimeout: NotRequired[bool],
    resultSetOptions: NotRequired[ResultSetOptionsTypeDef],  # (2)
    formatRecordsAs: NotRequired[RecordsFormatTypeType],  # (3)
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
2. See [:material-code-braces: ResultSetOptionsTypeDef](./type_defs.md#resultsetoptionstypedef) 
3. See [:material-code-brackets: RecordsFormatTypeType](./literals.md#recordsformattypetype) 
## BatchExecuteStatementResponseTypeDef

```python
# BatchExecuteStatementResponseTypeDef definition

class BatchExecuteStatementResponseTypeDef(TypedDict):
    updateResults: List[UpdateResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateResultTypeDef](./type_defs.md#updateresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SqlStatementResultTypeDef

```python
# SqlStatementResultTypeDef definition

class SqlStatementResultTypeDef(TypedDict):
    resultFrame: NotRequired[ResultFrameTypeDef],  # (1)
    numberOfRecordsUpdated: NotRequired[int],
```

1. See [:material-code-braces: ResultFrameTypeDef](./type_defs.md#resultframetypedef) 
## ExecuteSqlResponseTypeDef

```python
# ExecuteSqlResponseTypeDef definition

class ExecuteSqlResponseTypeDef(TypedDict):
    sqlStatementResults: List[SqlStatementResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SqlStatementResultTypeDef](./type_defs.md#sqlstatementresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
