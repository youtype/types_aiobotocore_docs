# Type definitions

> [Index](../README.md) > [RedshiftDataAPIService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RedshiftDataAPIService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#redshiftdataapiservice)
    type annotations stubs module [types-aiobotocore-redshift-data](https://pypi.org/project/types-aiobotocore-redshift-data/).



## BatchExecuteStatementInputTypeDef

```python
# BatchExecuteStatementInputTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementInputTypeDef


def get_value() -> BatchExecuteStatementInputTypeDef:
    return {
        "Sqls": ...,
    }


# BatchExecuteStatementInputTypeDef definition

class BatchExecuteStatementInputTypeDef(TypedDict):
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
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## CancelStatementRequestTypeDef

```python
# CancelStatementRequestTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import CancelStatementRequestTypeDef


def get_value() -> CancelStatementRequestTypeDef:
    return {
        "Id": ...,
    }


# CancelStatementRequestTypeDef definition

class CancelStatementRequestTypeDef(TypedDict):
    Id: str,
```

## ColumnMetadataTypeDef

```python
# ColumnMetadataTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ColumnMetadataTypeDef


def get_value() -> ColumnMetadataTypeDef:
    return {
        "columnDefault": ...,
    }


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

## DescribeStatementRequestTypeDef

```python
# DescribeStatementRequestTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import DescribeStatementRequestTypeDef


def get_value() -> DescribeStatementRequestTypeDef:
    return {
        "Id": ...,
    }


# DescribeStatementRequestTypeDef definition

class DescribeStatementRequestTypeDef(TypedDict):
    Id: str,
```

## SqlParameterTypeDef

```python
# SqlParameterTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import SqlParameterTypeDef


def get_value() -> SqlParameterTypeDef:
    return {
        "name": ...,
    }


# SqlParameterTypeDef definition

class SqlParameterTypeDef(TypedDict):
    name: str,
    value: str,
```

## SubStatementDataTypeDef

```python
# SubStatementDataTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import SubStatementDataTypeDef


def get_value() -> SubStatementDataTypeDef:
    return {
        "CreatedAt": ...,
    }


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
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeTableRequestTypeDef

```python
# DescribeTableRequestTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import DescribeTableRequestTypeDef


def get_value() -> DescribeTableRequestTypeDef:
    return {
        "Database": ...,
    }


# DescribeTableRequestTypeDef definition

class DescribeTableRequestTypeDef(TypedDict):
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
# FieldTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import FieldTypeDef


def get_value() -> FieldTypeDef:
    return {
        "blobValue": ...,
    }


# FieldTypeDef definition

class FieldTypeDef(TypedDict):
    blobValue: NotRequired[bytes],
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    isNull: NotRequired[bool],
    longValue: NotRequired[int],
    stringValue: NotRequired[str],
```

## GetStatementResultRequestTypeDef

```python
# GetStatementResultRequestTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import GetStatementResultRequestTypeDef


def get_value() -> GetStatementResultRequestTypeDef:
    return {
        "Id": ...,
    }


# GetStatementResultRequestTypeDef definition

class GetStatementResultRequestTypeDef(TypedDict):
    Id: str,
    NextToken: NotRequired[str],
```

## GetStatementResultV2RequestTypeDef

```python
# GetStatementResultV2RequestTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import GetStatementResultV2RequestTypeDef


def get_value() -> GetStatementResultV2RequestTypeDef:
    return {
        "Id": ...,
    }


# GetStatementResultV2RequestTypeDef definition

class GetStatementResultV2RequestTypeDef(TypedDict):
    Id: str,
    NextToken: NotRequired[str],
```

## QueryRecordsTypeDef

```python
# QueryRecordsTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import QueryRecordsTypeDef


def get_value() -> QueryRecordsTypeDef:
    return {
        "CSVRecords": ...,
    }


# QueryRecordsTypeDef definition

class QueryRecordsTypeDef(TypedDict):
    CSVRecords: NotRequired[str],
```

## ListDatabasesRequestTypeDef

```python
# ListDatabasesRequestTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListDatabasesRequestTypeDef


def get_value() -> ListDatabasesRequestTypeDef:
    return {
        "Database": ...,
    }


# ListDatabasesRequestTypeDef definition

class ListDatabasesRequestTypeDef(TypedDict):
    Database: str,
    ClusterIdentifier: NotRequired[str],
    DbUser: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SecretArn: NotRequired[str],
    WorkgroupName: NotRequired[str],
```

## ListSchemasRequestTypeDef

```python
# ListSchemasRequestTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListSchemasRequestTypeDef


def get_value() -> ListSchemasRequestTypeDef:
    return {
        "Database": ...,
    }


# ListSchemasRequestTypeDef definition

class ListSchemasRequestTypeDef(TypedDict):
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

## ListStatementsRequestTypeDef

```python
# ListStatementsRequestTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListStatementsRequestTypeDef


def get_value() -> ListStatementsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListStatementsRequestTypeDef definition

class ListStatementsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    RoleLevel: NotRequired[bool],
    StatementName: NotRequired[str],
    Status: NotRequired[StatusStringType],  # (1)
```

1. See [:material-code-brackets: StatusStringType](./literals.md#statusstringtype) 
## ListTablesRequestTypeDef

```python
# ListTablesRequestTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListTablesRequestTypeDef


def get_value() -> ListTablesRequestTypeDef:
    return {
        "Database": ...,
    }


# ListTablesRequestTypeDef definition

class ListTablesRequestTypeDef(TypedDict):
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
# TableMemberTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import TableMemberTypeDef


def get_value() -> TableMemberTypeDef:
    return {
        "name": ...,
    }


# TableMemberTypeDef definition

class TableMemberTypeDef(TypedDict):
    name: NotRequired[str],
    schema: NotRequired[str],
    type: NotRequired[str],
```

## BatchExecuteStatementOutputTypeDef

```python
# BatchExecuteStatementOutputTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementOutputTypeDef


def get_value() -> BatchExecuteStatementOutputTypeDef:
    return {
        "ClusterIdentifier": ...,
    }


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
# CancelStatementResponseTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import CancelStatementResponseTypeDef


def get_value() -> CancelStatementResponseTypeDef:
    return {
        "Status": ...,
    }


# CancelStatementResponseTypeDef definition

class CancelStatementResponseTypeDef(TypedDict):
    Status: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteStatementOutputTypeDef

```python
# ExecuteStatementOutputTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ExecuteStatementOutputTypeDef


def get_value() -> ExecuteStatementOutputTypeDef:
    return {
        "ClusterIdentifier": ...,
    }


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
# ListDatabasesResponseTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListDatabasesResponseTypeDef


def get_value() -> ListDatabasesResponseTypeDef:
    return {
        "Databases": ...,
    }


# ListDatabasesResponseTypeDef definition

class ListDatabasesResponseTypeDef(TypedDict):
    Databases: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemasResponseTypeDef

```python
# ListSchemasResponseTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListSchemasResponseTypeDef


def get_value() -> ListSchemasResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListSchemasResponseTypeDef definition

class ListSchemasResponseTypeDef(TypedDict):
    Schemas: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableResponseTypeDef

```python
# DescribeTableResponseTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import DescribeTableResponseTypeDef


def get_value() -> DescribeTableResponseTypeDef:
    return {
        "ColumnList": ...,
    }


# DescribeTableResponseTypeDef definition

class DescribeTableResponseTypeDef(TypedDict):
    ColumnList: List[ColumnMetadataTypeDef],  # (1)
    TableName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteStatementInputTypeDef

```python
# ExecuteStatementInputTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ExecuteStatementInputTypeDef


def get_value() -> ExecuteStatementInputTypeDef:
    return {
        "Sql": ...,
    }


# ExecuteStatementInputTypeDef definition

class ExecuteStatementInputTypeDef(TypedDict):
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
# StatementDataTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import StatementDataTypeDef


def get_value() -> StatementDataTypeDef:
    return {
        "CreatedAt": ...,
    }


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
# DescribeStatementResponseTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import DescribeStatementResponseTypeDef


def get_value() -> DescribeStatementResponseTypeDef:
    return {
        "ClusterIdentifier": ...,
    }


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
# DescribeTableRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import DescribeTableRequestPaginateTypeDef


def get_value() -> DescribeTableRequestPaginateTypeDef:
    return {
        "Database": ...,
    }


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
# GetStatementResultRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import GetStatementResultRequestPaginateTypeDef


def get_value() -> GetStatementResultRequestPaginateTypeDef:
    return {
        "Id": ...,
    }


# GetStatementResultRequestPaginateTypeDef definition

class GetStatementResultRequestPaginateTypeDef(TypedDict):
    Id: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetStatementResultV2RequestPaginateTypeDef

```python
# GetStatementResultV2RequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import GetStatementResultV2RequestPaginateTypeDef


def get_value() -> GetStatementResultV2RequestPaginateTypeDef:
    return {
        "Id": ...,
    }


# GetStatementResultV2RequestPaginateTypeDef definition

class GetStatementResultV2RequestPaginateTypeDef(TypedDict):
    Id: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatabasesRequestPaginateTypeDef

```python
# ListDatabasesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListDatabasesRequestPaginateTypeDef


def get_value() -> ListDatabasesRequestPaginateTypeDef:
    return {
        "Database": ...,
    }


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
# ListSchemasRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListSchemasRequestPaginateTypeDef


def get_value() -> ListSchemasRequestPaginateTypeDef:
    return {
        "Database": ...,
    }


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
# ListStatementsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListStatementsRequestPaginateTypeDef


def get_value() -> ListStatementsRequestPaginateTypeDef:
    return {
        "RoleLevel": ...,
    }


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
# ListTablesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListTablesRequestPaginateTypeDef


def get_value() -> ListTablesRequestPaginateTypeDef:
    return {
        "Database": ...,
    }


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
# GetStatementResultResponseTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import GetStatementResultResponseTypeDef


def get_value() -> GetStatementResultResponseTypeDef:
    return {
        "ColumnMetadata": ...,
    }


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
# GetStatementResultV2ResponseTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import GetStatementResultV2ResponseTypeDef


def get_value() -> GetStatementResultV2ResponseTypeDef:
    return {
        "ColumnMetadata": ...,
    }


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
# ListTablesResponseTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListTablesResponseTypeDef


def get_value() -> ListTablesResponseTypeDef:
    return {
        "NextToken": ...,
    }


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
# ListStatementsResponseTypeDef TypedDict usage example

from types_aiobotocore_redshift_data.type_defs import ListStatementsResponseTypeDef


def get_value() -> ListStatementsResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListStatementsResponseTypeDef definition

class ListStatementsResponseTypeDef(TypedDict):
    Statements: List[StatementDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StatementDataTypeDef](./type_defs.md#statementdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
