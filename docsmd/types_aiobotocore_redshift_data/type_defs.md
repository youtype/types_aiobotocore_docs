# Type definitions

> [Index](../README.md) > [RedshiftDataAPIService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RedshiftDataAPIService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#redshiftdataapiservice)
    type annotations stubs module [types-aiobotocore-redshift-data](https://pypi.org/project/types-aiobotocore-redshift-data/).



## BatchExecuteStatementInputRequestTypeDef

```python
# BatchExecuteStatementInputRequestTypeDef definition

class BatchExecuteStatementInputRequestTypeDef(TypedDict):
    Sqls: Sequence[str],
    ClientToken: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    Database: NotRequired[str],
    DbUser: NotRequired[str],
    ResultFormat: NotRequired[ResultFormatStringType],  # (1)
    SecretArn: NotRequired[str],
    SessionId: NotRequired[str],
    SessionKeepAliveSeconds: NotRequired[int],
    StatementName: NotRequired[str],
    WithEvent: NotRequired[bool],
    WorkgroupName: NotRequired[str],
```

1. See [:material-code-brackets: ResultFormatStringType](./literals.md#resultformatstringtype) 
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

## CancelStatementRequestRequestTypeDef

```python
# CancelStatementRequestRequestTypeDef definition

class CancelStatementRequestRequestTypeDef(TypedDict):
    Id: str,
```

## ColumnMetadataTypeDef

```python
# ColumnMetadataTypeDef definition

class ColumnMetadataTypeDef(TypedDict):
    columnDefault: NotRequired[str],
    isCaseSensitive: NotRequired[bool],
    isCurrency: NotRequired[bool],
    isSigned: NotRequired[bool],
    label: NotRequired[str],
    length: NotRequired[int],
    name: NotRequired[str],
    nullable: NotRequired[int],
    precision: NotRequired[int],
    scale: NotRequired[int],
    schemaName: NotRequired[str],
    tableName: NotRequired[str],
    typeName: NotRequired[str],
```

## DescribeStatementRequestRequestTypeDef

```python
# DescribeStatementRequestRequestTypeDef definition

class DescribeStatementRequestRequestTypeDef(TypedDict):
    Id: str,
```

## SqlParameterTypeDef

```python
# SqlParameterTypeDef definition

class SqlParameterTypeDef(TypedDict):
    name: str,
    value: str,
```

## SubStatementDataTypeDef

```python
# SubStatementDataTypeDef definition

class SubStatementDataTypeDef(TypedDict):
    Id: str,
    CreatedAt: NotRequired[datetime],
    Duration: NotRequired[int],
    Error: NotRequired[str],
    HasResultSet: NotRequired[bool],
    QueryString: NotRequired[str],
    RedshiftQueryId: NotRequired[int],
    ResultRows: NotRequired[int],
    ResultSize: NotRequired[int],
    Status: NotRequired[StatementStatusStringType],  # (1)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: StatementStatusStringType](./literals.md#statementstatusstringtype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeTableRequestRequestTypeDef

```python
# DescribeTableRequestRequestTypeDef definition

class DescribeTableRequestRequestTypeDef(TypedDict):
    Database: str,
    ClusterIdentifier: NotRequired[str],
    ConnectedDatabase: NotRequired[str],
    DbUser: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Schema: NotRequired[str],
    SecretArn: NotRequired[str],
    Table: NotRequired[str],
    WorkgroupName: NotRequired[str],
```

## FieldTypeDef

```python
# FieldTypeDef definition

class FieldTypeDef(TypedDict):
    blobValue: NotRequired[bytes],
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    isNull: NotRequired[bool],
    longValue: NotRequired[int],
    stringValue: NotRequired[str],
```

## GetStatementResultRequestRequestTypeDef

```python
# GetStatementResultRequestRequestTypeDef definition

class GetStatementResultRequestRequestTypeDef(TypedDict):
    Id: str,
    NextToken: NotRequired[str],
```

## GetStatementResultV2RequestRequestTypeDef

```python
# GetStatementResultV2RequestRequestTypeDef definition

class GetStatementResultV2RequestRequestTypeDef(TypedDict):
    Id: str,
    NextToken: NotRequired[str],
```

## QueryRecordsTypeDef

```python
# QueryRecordsTypeDef definition

class QueryRecordsTypeDef(TypedDict):
    CSVRecords: NotRequired[str],
```

## ListDatabasesRequestRequestTypeDef

```python
# ListDatabasesRequestRequestTypeDef definition

class ListDatabasesRequestRequestTypeDef(TypedDict):
    Database: str,
    ClusterIdentifier: NotRequired[str],
    DbUser: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SecretArn: NotRequired[str],
    WorkgroupName: NotRequired[str],
```

## ListSchemasRequestRequestTypeDef

```python
# ListSchemasRequestRequestTypeDef definition

class ListSchemasRequestRequestTypeDef(TypedDict):
    Database: str,
    ClusterIdentifier: NotRequired[str],
    ConnectedDatabase: NotRequired[str],
    DbUser: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SchemaPattern: NotRequired[str],
    SecretArn: NotRequired[str],
    WorkgroupName: NotRequired[str],
```

## ListStatementsRequestRequestTypeDef

```python
# ListStatementsRequestRequestTypeDef definition

class ListStatementsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    RoleLevel: NotRequired[bool],
    StatementName: NotRequired[str],
    Status: NotRequired[StatusStringType],  # (1)
```

1. See [:material-code-brackets: StatusStringType](./literals.md#statusstringtype) 
## ListTablesRequestRequestTypeDef

```python
# ListTablesRequestRequestTypeDef definition

class ListTablesRequestRequestTypeDef(TypedDict):
    Database: str,
    ClusterIdentifier: NotRequired[str],
    ConnectedDatabase: NotRequired[str],
    DbUser: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SchemaPattern: NotRequired[str],
    SecretArn: NotRequired[str],
    TablePattern: NotRequired[str],
    WorkgroupName: NotRequired[str],
```

## TableMemberTypeDef

```python
# TableMemberTypeDef definition

class TableMemberTypeDef(TypedDict):
    name: NotRequired[str],
    schema: NotRequired[str],
    type: NotRequired[str],
```

## BatchExecuteStatementOutputTypeDef

```python
# BatchExecuteStatementOutputTypeDef definition

class BatchExecuteStatementOutputTypeDef(TypedDict):
    ClusterIdentifier: str,
    CreatedAt: datetime,
    Database: str,
    DbGroups: List[str],
    DbUser: str,
    Id: str,
    SecretArn: str,
    SessionId: str,
    WorkgroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelStatementResponseTypeDef

```python
# CancelStatementResponseTypeDef definition

class CancelStatementResponseTypeDef(TypedDict):
    Status: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteStatementOutputTypeDef

```python
# ExecuteStatementOutputTypeDef definition

class ExecuteStatementOutputTypeDef(TypedDict):
    ClusterIdentifier: str,
    CreatedAt: datetime,
    Database: str,
    DbGroups: List[str],
    DbUser: str,
    Id: str,
    SecretArn: str,
    SessionId: str,
    WorkgroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatabasesResponseTypeDef

```python
# ListDatabasesResponseTypeDef definition

class ListDatabasesResponseTypeDef(TypedDict):
    Databases: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemasResponseTypeDef

```python
# ListSchemasResponseTypeDef definition

class ListSchemasResponseTypeDef(TypedDict):
    Schemas: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableResponseTypeDef

```python
# DescribeTableResponseTypeDef definition

class DescribeTableResponseTypeDef(TypedDict):
    ColumnList: List[ColumnMetadataTypeDef],  # (1)
    TableName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteStatementInputRequestTypeDef

```python
# ExecuteStatementInputRequestTypeDef definition

class ExecuteStatementInputRequestTypeDef(TypedDict):
    Sql: str,
    ClientToken: NotRequired[str],
    ClusterIdentifier: NotRequired[str],
    Database: NotRequired[str],
    DbUser: NotRequired[str],
    Parameters: NotRequired[Sequence[SqlParameterTypeDef]],  # (1)
    ResultFormat: NotRequired[ResultFormatStringType],  # (2)
    SecretArn: NotRequired[str],
    SessionId: NotRequired[str],
    SessionKeepAliveSeconds: NotRequired[int],
    StatementName: NotRequired[str],
    WithEvent: NotRequired[bool],
    WorkgroupName: NotRequired[str],
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
2. See [:material-code-brackets: ResultFormatStringType](./literals.md#resultformatstringtype) 
## StatementDataTypeDef

```python
# StatementDataTypeDef definition

class StatementDataTypeDef(TypedDict):
    Id: str,
    CreatedAt: NotRequired[datetime],
    IsBatchStatement: NotRequired[bool],
    QueryParameters: NotRequired[List[SqlParameterTypeDef]],  # (1)
    QueryString: NotRequired[str],
    QueryStrings: NotRequired[List[str]],
    ResultFormat: NotRequired[ResultFormatStringType],  # (2)
    SecretArn: NotRequired[str],
    SessionId: NotRequired[str],
    StatementName: NotRequired[str],
    Status: NotRequired[StatusStringType],  # (3)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
2. See [:material-code-brackets: ResultFormatStringType](./literals.md#resultformatstringtype) 
3. See [:material-code-brackets: StatusStringType](./literals.md#statusstringtype) 
## DescribeStatementResponseTypeDef

```python
# DescribeStatementResponseTypeDef definition

class DescribeStatementResponseTypeDef(TypedDict):
    ClusterIdentifier: str,
    CreatedAt: datetime,
    Database: str,
    DbUser: str,
    Duration: int,
    Error: str,
    HasResultSet: bool,
    Id: str,
    QueryParameters: List[SqlParameterTypeDef],  # (1)
    QueryString: str,
    RedshiftPid: int,
    RedshiftQueryId: int,
    ResultFormat: ResultFormatStringType,  # (2)
    ResultRows: int,
    ResultSize: int,
    SecretArn: str,
    SessionId: str,
    Status: StatusStringType,  # (3)
    SubStatements: List[SubStatementDataTypeDef],  # (4)
    UpdatedAt: datetime,
    WorkgroupName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SqlParameterTypeDef](./type_defs.md#sqlparametertypedef) 
2. See [:material-code-brackets: ResultFormatStringType](./literals.md#resultformatstringtype) 
3. See [:material-code-brackets: StatusStringType](./literals.md#statusstringtype) 
4. See [:material-code-braces: SubStatementDataTypeDef](./type_defs.md#substatementdatatypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableRequestPaginateTypeDef

```python
# DescribeTableRequestPaginateTypeDef definition

class DescribeTableRequestPaginateTypeDef(TypedDict):
    Database: str,
    ClusterIdentifier: NotRequired[str],
    ConnectedDatabase: NotRequired[str],
    DbUser: NotRequired[str],
    Schema: NotRequired[str],
    SecretArn: NotRequired[str],
    Table: NotRequired[str],
    WorkgroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetStatementResultRequestPaginateTypeDef

```python
# GetStatementResultRequestPaginateTypeDef definition

class GetStatementResultRequestPaginateTypeDef(TypedDict):
    Id: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetStatementResultV2RequestPaginateTypeDef

```python
# GetStatementResultV2RequestPaginateTypeDef definition

class GetStatementResultV2RequestPaginateTypeDef(TypedDict):
    Id: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatabasesRequestPaginateTypeDef

```python
# ListDatabasesRequestPaginateTypeDef definition

class ListDatabasesRequestPaginateTypeDef(TypedDict):
    Database: str,
    ClusterIdentifier: NotRequired[str],
    DbUser: NotRequired[str],
    SecretArn: NotRequired[str],
    WorkgroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemasRequestPaginateTypeDef

```python
# ListSchemasRequestPaginateTypeDef definition

class ListSchemasRequestPaginateTypeDef(TypedDict):
    Database: str,
    ClusterIdentifier: NotRequired[str],
    ConnectedDatabase: NotRequired[str],
    DbUser: NotRequired[str],
    SchemaPattern: NotRequired[str],
    SecretArn: NotRequired[str],
    WorkgroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStatementsRequestPaginateTypeDef

```python
# ListStatementsRequestPaginateTypeDef definition

class ListStatementsRequestPaginateTypeDef(TypedDict):
    RoleLevel: NotRequired[bool],
    StatementName: NotRequired[str],
    Status: NotRequired[StatusStringType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: StatusStringType](./literals.md#statusstringtype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesRequestPaginateTypeDef

```python
# ListTablesRequestPaginateTypeDef definition

class ListTablesRequestPaginateTypeDef(TypedDict):
    Database: str,
    ClusterIdentifier: NotRequired[str],
    ConnectedDatabase: NotRequired[str],
    DbUser: NotRequired[str],
    SchemaPattern: NotRequired[str],
    SecretArn: NotRequired[str],
    TablePattern: NotRequired[str],
    WorkgroupName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetStatementResultResponseTypeDef

```python
# GetStatementResultResponseTypeDef definition

class GetStatementResultResponseTypeDef(TypedDict):
    ColumnMetadata: List[ColumnMetadataTypeDef],  # (1)
    Records: List[List[FieldTypeDef]],  # (2)
    TotalNumRows: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef) 
2. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStatementResultV2ResponseTypeDef

```python
# GetStatementResultV2ResponseTypeDef definition

class GetStatementResultV2ResponseTypeDef(TypedDict):
    ColumnMetadata: List[ColumnMetadataTypeDef],  # (1)
    Records: List[QueryRecordsTypeDef],  # (2)
    ResultFormat: ResultFormatStringType,  # (3)
    TotalNumRows: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef) 
2. See [:material-code-braces: QueryRecordsTypeDef](./type_defs.md#queryrecordstypedef) 
3. See [:material-code-brackets: ResultFormatStringType](./literals.md#resultformatstringtype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTablesResponseTypeDef

```python
# ListTablesResponseTypeDef definition

class ListTablesResponseTypeDef(TypedDict):
    Tables: List[TableMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TableMemberTypeDef](./type_defs.md#tablemembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStatementsResponseTypeDef

```python
# ListStatementsResponseTypeDef definition

class ListStatementsResponseTypeDef(TypedDict):
    Statements: List[StatementDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StatementDataTypeDef](./type_defs.md#statementdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
