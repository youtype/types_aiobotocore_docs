<a id="typed-dictionaries-for-aiobotocore-redshiftdataapiservice-module"></a>

# Typed dictionaries for aiobotocore RedshiftDataAPIService module

> [Index](..) > [RedshiftDataAPIService](.) > Typed dictionaries

Auto-generated documentation for
[RedshiftDataAPIService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
type annotations stubs module
[types-aiobotocore-redshift-data](https://pypi.org/project/types-aiobotocore-redshift-data/).

- [Typed dictionaries for aiobotocore RedshiftDataAPIService module](#typed-dictionaries-for-aiobotocore-redshiftdataapiservice-module)
  - [BatchExecuteStatementInputRequestTypeDef](#batchexecutestatementinputrequesttypedef)
  - [BatchExecuteStatementOutputTypeDef](#batchexecutestatementoutputtypedef)
  - [CancelStatementRequestRequestTypeDef](#cancelstatementrequestrequesttypedef)
  - [CancelStatementResponseTypeDef](#cancelstatementresponsetypedef)
  - [ColumnMetadataTypeDef](#columnmetadatatypedef)
  - [DescribeStatementRequestRequestTypeDef](#describestatementrequestrequesttypedef)
  - [DescribeStatementResponseTypeDef](#describestatementresponsetypedef)
  - [DescribeTableRequestRequestTypeDef](#describetablerequestrequesttypedef)
  - [DescribeTableResponseTypeDef](#describetableresponsetypedef)
  - [ExecuteStatementInputRequestTypeDef](#executestatementinputrequesttypedef)
  - [ExecuteStatementOutputTypeDef](#executestatementoutputtypedef)
  - [FieldTypeDef](#fieldtypedef)
  - [GetStatementResultRequestRequestTypeDef](#getstatementresultrequestrequesttypedef)
  - [GetStatementResultResponseTypeDef](#getstatementresultresponsetypedef)
  - [ListDatabasesRequestRequestTypeDef](#listdatabasesrequestrequesttypedef)
  - [ListDatabasesResponseTypeDef](#listdatabasesresponsetypedef)
  - [ListSchemasRequestRequestTypeDef](#listschemasrequestrequesttypedef)
  - [ListSchemasResponseTypeDef](#listschemasresponsetypedef)
  - [ListStatementsRequestRequestTypeDef](#liststatementsrequestrequesttypedef)
  - [ListStatementsResponseTypeDef](#liststatementsresponsetypedef)
  - [ListTablesRequestRequestTypeDef](#listtablesrequestrequesttypedef)
  - [ListTablesResponseTypeDef](#listtablesresponsetypedef)
  - [PaginatorConfigTypeDef](#paginatorconfigtypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [SqlParameterTypeDef](#sqlparametertypedef)
  - [StatementDataTypeDef](#statementdatatypedef)
  - [SubStatementDataTypeDef](#substatementdatatypedef)
  - [TableMemberTypeDef](#tablemembertypedef)

<a id="batchexecutestatementinputrequesttypedef"></a>

## BatchExecuteStatementInputRequestTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementInputRequestTypeDef
```

Required fields:

- `Database`: `str`
- `Sqls`: `Sequence`\[`str`\]

Optional fields:

- `ClusterIdentifier`: `str`
- `DbUser`: `str`
- `SecretArn`: `str`
- `StatementName`: `str`
- `WithEvent`: `bool`

<a id="batchexecutestatementoutputtypedef"></a>

## BatchExecuteStatementOutputTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementOutputTypeDef
```

Required fields:

- `ClusterIdentifier`: `str`
- `CreatedAt`: `datetime`
- `Database`: `str`
- `DbUser`: `str`
- `Id`: `str`
- `SecretArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="cancelstatementrequestrequesttypedef"></a>

## CancelStatementRequestRequestTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import CancelStatementRequestRequestTypeDef
```

Required fields:

- `Id`: `str`

<a id="cancelstatementresponsetypedef"></a>

## CancelStatementResponseTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import CancelStatementResponseTypeDef
```

Required fields:

- `Status`: `bool`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="columnmetadatatypedef"></a>

## ColumnMetadataTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ColumnMetadataTypeDef
```

Optional fields:

- `columnDefault`: `str`
- `isCaseSensitive`: `bool`
- `isCurrency`: `bool`
- `isSigned`: `bool`
- `label`: `str`
- `length`: `int`
- `name`: `str`
- `nullable`: `int`
- `precision`: `int`
- `scale`: `int`
- `schemaName`: `str`
- `tableName`: `str`
- `typeName`: `str`

<a id="describestatementrequestrequesttypedef"></a>

## DescribeStatementRequestRequestTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import DescribeStatementRequestRequestTypeDef
```

Required fields:

- `Id`: `str`

<a id="describestatementresponsetypedef"></a>

## DescribeStatementResponseTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import DescribeStatementResponseTypeDef
```

Required fields:

- `ClusterIdentifier`: `str`
- `CreatedAt`: `datetime`
- `Database`: `str`
- `DbUser`: `str`
- `Duration`: `int`
- `Error`: `str`
- `HasResultSet`: `bool`
- `Id`: `str`
- `QueryParameters`:
  `List`\[[SqlParameterTypeDef](./type_defs.md#sqlparametertypedef)\]
- `QueryString`: `str`
- `RedshiftPid`: `int`
- `RedshiftQueryId`: `int`
- `ResultRows`: `int`
- `ResultSize`: `int`
- `SecretArn`: `str`
- `Status`: [StatusStringType](./literals.md#statusstringtype)
- `SubStatements`:
  `List`\[[SubStatementDataTypeDef](./type_defs.md#substatementdatatypedef)\]
- `UpdatedAt`: `datetime`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describetablerequestrequesttypedef"></a>

## DescribeTableRequestRequestTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import DescribeTableRequestRequestTypeDef
```

Required fields:

- `Database`: `str`

Optional fields:

- `ClusterIdentifier`: `str`
- `ConnectedDatabase`: `str`
- `DbUser`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`
- `Schema`: `str`
- `SecretArn`: `str`
- `Table`: `str`

<a id="describetableresponsetypedef"></a>

## DescribeTableResponseTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import DescribeTableResponseTypeDef
```

Required fields:

- `ColumnList`:
  `List`\[[ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef)\]
- `NextToken`: `str`
- `TableName`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="executestatementinputrequesttypedef"></a>

## ExecuteStatementInputRequestTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ExecuteStatementInputRequestTypeDef
```

Required fields:

- `Database`: `str`
- `Sql`: `str`

Optional fields:

- `ClusterIdentifier`: `str`
- `DbUser`: `str`
- `Parameters`:
  `Sequence`\[[SqlParameterTypeDef](./type_defs.md#sqlparametertypedef)\]
- `SecretArn`: `str`
- `StatementName`: `str`
- `WithEvent`: `bool`

<a id="executestatementoutputtypedef"></a>

## ExecuteStatementOutputTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ExecuteStatementOutputTypeDef
```

Required fields:

- `ClusterIdentifier`: `str`
- `CreatedAt`: `datetime`
- `Database`: `str`
- `DbUser`: `str`
- `Id`: `str`
- `SecretArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="fieldtypedef"></a>

## FieldTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import FieldTypeDef
```

Optional fields:

- `blobValue`: `bytes`
- `booleanValue`: `bool`
- `doubleValue`: `float`
- `isNull`: `bool`
- `longValue`: `int`
- `stringValue`: `str`

<a id="getstatementresultrequestrequesttypedef"></a>

## GetStatementResultRequestRequestTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import GetStatementResultRequestRequestTypeDef
```

Required fields:

- `Id`: `str`

Optional fields:

- `NextToken`: `str`

<a id="getstatementresultresponsetypedef"></a>

## GetStatementResultResponseTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import GetStatementResultResponseTypeDef
```

Required fields:

- `ColumnMetadata`:
  `List`\[[ColumnMetadataTypeDef](./type_defs.md#columnmetadatatypedef)\]
- `NextToken`: `str`
- `Records`: `List`\[`List`\[[FieldTypeDef](./type_defs.md#fieldtypedef)\]\]
- `TotalNumRows`: `int`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listdatabasesrequestrequesttypedef"></a>

## ListDatabasesRequestRequestTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ListDatabasesRequestRequestTypeDef
```

Required fields:

- `Database`: `str`

Optional fields:

- `ClusterIdentifier`: `str`
- `DbUser`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`
- `SecretArn`: `str`

<a id="listdatabasesresponsetypedef"></a>

## ListDatabasesResponseTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ListDatabasesResponseTypeDef
```

Required fields:

- `Databases`: `List`\[`str`\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listschemasrequestrequesttypedef"></a>

## ListSchemasRequestRequestTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ListSchemasRequestRequestTypeDef
```

Required fields:

- `Database`: `str`

Optional fields:

- `ClusterIdentifier`: `str`
- `ConnectedDatabase`: `str`
- `DbUser`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`
- `SchemaPattern`: `str`
- `SecretArn`: `str`

<a id="listschemasresponsetypedef"></a>

## ListSchemasResponseTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ListSchemasResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Schemas`: `List`\[`str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="liststatementsrequestrequesttypedef"></a>

## ListStatementsRequestRequestTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ListStatementsRequestRequestTypeDef
```

Optional fields:

- `MaxResults`: `int`
- `NextToken`: `str`
- `RoleLevel`: `bool`
- `StatementName`: `str`
- `Status`: [StatusStringType](./literals.md#statusstringtype)

<a id="liststatementsresponsetypedef"></a>

## ListStatementsResponseTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ListStatementsResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Statements`:
  `List`\[[StatementDataTypeDef](./type_defs.md#statementdatatypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtablesrequestrequesttypedef"></a>

## ListTablesRequestRequestTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ListTablesRequestRequestTypeDef
```

Required fields:

- `Database`: `str`

Optional fields:

- `ClusterIdentifier`: `str`
- `ConnectedDatabase`: `str`
- `DbUser`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`
- `SchemaPattern`: `str`
- `SecretArn`: `str`
- `TablePattern`: `str`

<a id="listtablesresponsetypedef"></a>

## ListTablesResponseTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ListTablesResponseTypeDef
```

Required fields:

- `NextToken`: `str`
- `Tables`: `List`\[[TableMemberTypeDef](./type_defs.md#tablemembertypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="paginatorconfigtypedef"></a>

## PaginatorConfigTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import PaginatorConfigTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `PageSize`: `int`
- `StartingToken`: `str`

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="sqlparametertypedef"></a>

## SqlParameterTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import SqlParameterTypeDef
```

Required fields:

- `name`: `str`
- `value`: `str`

<a id="statementdatatypedef"></a>

## StatementDataTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import StatementDataTypeDef
```

Required fields:

- `Id`: `str`

Optional fields:

- `CreatedAt`: `datetime`
- `IsBatchStatement`: `bool`
- `QueryParameters`:
  `List`\[[SqlParameterTypeDef](./type_defs.md#sqlparametertypedef)\]
- `QueryString`: `str`
- `QueryStrings`: `List`\[`str`\]
- `SecretArn`: `str`
- `StatementName`: `str`
- `Status`: [StatusStringType](./literals.md#statusstringtype)
- `UpdatedAt`: `datetime`

<a id="substatementdatatypedef"></a>

## SubStatementDataTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import SubStatementDataTypeDef
```

Required fields:

- `Id`: `str`

Optional fields:

- `CreatedAt`: `datetime`
- `Duration`: `int`
- `Error`: `str`
- `HasResultSet`: `bool`
- `QueryString`: `str`
- `RedshiftQueryId`: `int`
- `ResultRows`: `int`
- `ResultSize`: `int`
- `Status`:
  [StatementStatusStringType](./literals.md#statementstatusstringtype)
- `UpdatedAt`: `datetime`

<a id="tablemembertypedef"></a>

## TableMemberTypeDef

```python
from types_aiobotocore_redshift_data.type_defs import TableMemberTypeDef
```

Optional fields:

- `name`: `str`
- `schema`: `str`
- `type`: `str`
