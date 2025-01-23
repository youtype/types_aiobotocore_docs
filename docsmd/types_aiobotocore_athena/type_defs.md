# Type definitions

> [Index](../README.md) > [Athena](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Athena](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#athena)
    type annotations stubs module [types-aiobotocore-athena](https://pypi.org/project/types-aiobotocore-athena/).

## CapacityAssignmentUnionTypeDef

```python
# CapacityAssignmentUnionTypeDef definition

CapacityAssignmentUnionTypeDef = Union[
    CapacityAssignmentTypeDef,  # (1)
    CapacityAssignmentOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CapacityAssignmentTypeDef](./type_defs.md#capacityassignmenttypedef) 
2. See [:material-code-braces: CapacityAssignmentOutputTypeDef](./type_defs.md#capacityassignmentoutputtypedef) 



## AclConfigurationTypeDef

```python
# AclConfigurationTypeDef definition

class AclConfigurationTypeDef(TypedDict):
    S3AclOption: S3AclOptionType,  # (1)
```

1. See [:material-code-brackets: S3AclOptionType](./literals.md#s3acloptiontype) 
## ApplicationDPUSizesTypeDef

```python
# ApplicationDPUSizesTypeDef definition

class ApplicationDPUSizesTypeDef(TypedDict):
    ApplicationRuntimeId: NotRequired[str],
    SupportedDPUSizes: NotRequired[List[int]],
```

## AthenaErrorTypeDef

```python
# AthenaErrorTypeDef definition

class AthenaErrorTypeDef(TypedDict):
    ErrorCategory: NotRequired[int],
    ErrorType: NotRequired[int],
    Retryable: NotRequired[bool],
    ErrorMessage: NotRequired[str],
```

## BatchGetNamedQueryInputRequestTypeDef

```python
# BatchGetNamedQueryInputRequestTypeDef definition

class BatchGetNamedQueryInputRequestTypeDef(TypedDict):
    NamedQueryIds: Sequence[str],
```

## NamedQueryTypeDef

```python
# NamedQueryTypeDef definition

class NamedQueryTypeDef(TypedDict):
    Name: str,
    Database: str,
    QueryString: str,
    Description: NotRequired[str],
    NamedQueryId: NotRequired[str],
    WorkGroup: NotRequired[str],
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

## UnprocessedNamedQueryIdTypeDef

```python
# UnprocessedNamedQueryIdTypeDef definition

class UnprocessedNamedQueryIdTypeDef(TypedDict):
    NamedQueryId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchGetPreparedStatementInputRequestTypeDef

```python
# BatchGetPreparedStatementInputRequestTypeDef definition

class BatchGetPreparedStatementInputRequestTypeDef(TypedDict):
    PreparedStatementNames: Sequence[str],
    WorkGroup: str,
```

## PreparedStatementTypeDef

```python
# PreparedStatementTypeDef definition

class PreparedStatementTypeDef(TypedDict):
    StatementName: NotRequired[str],
    QueryStatement: NotRequired[str],
    WorkGroupName: NotRequired[str],
    Description: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
```

## UnprocessedPreparedStatementNameTypeDef

```python
# UnprocessedPreparedStatementNameTypeDef definition

class UnprocessedPreparedStatementNameTypeDef(TypedDict):
    StatementName: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchGetQueryExecutionInputRequestTypeDef

```python
# BatchGetQueryExecutionInputRequestTypeDef definition

class BatchGetQueryExecutionInputRequestTypeDef(TypedDict):
    QueryExecutionIds: Sequence[str],
```

## UnprocessedQueryExecutionIdTypeDef

```python
# UnprocessedQueryExecutionIdTypeDef definition

class UnprocessedQueryExecutionIdTypeDef(TypedDict):
    QueryExecutionId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## CalculationConfigurationTypeDef

```python
# CalculationConfigurationTypeDef definition

class CalculationConfigurationTypeDef(TypedDict):
    CodeBlock: NotRequired[str],
```

## CalculationResultTypeDef

```python
# CalculationResultTypeDef definition

class CalculationResultTypeDef(TypedDict):
    StdOutS3Uri: NotRequired[str],
    StdErrorS3Uri: NotRequired[str],
    ResultS3Uri: NotRequired[str],
    ResultType: NotRequired[str],
```

## CalculationStatisticsTypeDef

```python
# CalculationStatisticsTypeDef definition

class CalculationStatisticsTypeDef(TypedDict):
    DpuExecutionInMillis: NotRequired[int],
    Progress: NotRequired[str],
```

## CalculationStatusTypeDef

```python
# CalculationStatusTypeDef definition

class CalculationStatusTypeDef(TypedDict):
    SubmissionDateTime: NotRequired[datetime],
    CompletionDateTime: NotRequired[datetime],
    State: NotRequired[CalculationExecutionStateType],  # (1)
    StateChangeReason: NotRequired[str],
```

1. See [:material-code-brackets: CalculationExecutionStateType](./literals.md#calculationexecutionstatetype) 
## CancelCapacityReservationInputRequestTypeDef

```python
# CancelCapacityReservationInputRequestTypeDef definition

class CancelCapacityReservationInputRequestTypeDef(TypedDict):
    Name: str,
```

## CapacityAllocationTypeDef

```python
# CapacityAllocationTypeDef definition

class CapacityAllocationTypeDef(TypedDict):
    Status: CapacityAllocationStatusType,  # (1)
    RequestTime: datetime,
    StatusMessage: NotRequired[str],
    RequestCompletionTime: NotRequired[datetime],
```

1. See [:material-code-brackets: CapacityAllocationStatusType](./literals.md#capacityallocationstatustype) 
## CapacityAssignmentOutputTypeDef

```python
# CapacityAssignmentOutputTypeDef definition

class CapacityAssignmentOutputTypeDef(TypedDict):
    WorkGroupNames: NotRequired[List[str]],
```

## CapacityAssignmentTypeDef

```python
# CapacityAssignmentTypeDef definition

class CapacityAssignmentTypeDef(TypedDict):
    WorkGroupNames: NotRequired[Sequence[str]],
```

## ColumnInfoTypeDef

```python
# ColumnInfoTypeDef definition

class ColumnInfoTypeDef(TypedDict):
    Name: str,
    Type: str,
    CatalogName: NotRequired[str],
    SchemaName: NotRequired[str],
    TableName: NotRequired[str],
    Label: NotRequired[str],
    Precision: NotRequired[int],
    Scale: NotRequired[int],
    Nullable: NotRequired[ColumnNullableType],  # (1)
    CaseSensitive: NotRequired[bool],
```

1. See [:material-code-brackets: ColumnNullableType](./literals.md#columnnullabletype) 
## ColumnTypeDef

```python
# ColumnTypeDef definition

class ColumnTypeDef(TypedDict):
    Name: str,
    Type: NotRequired[str],
    Comment: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## DataCatalogTypeDef

```python
# DataCatalogTypeDef definition

class DataCatalogTypeDef(TypedDict):
    Name: str,
    Type: DataCatalogTypeType,  # (1)
    Description: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
    Status: NotRequired[DataCatalogStatusType],  # (2)
    ConnectionType: NotRequired[ConnectionTypeType],  # (3)
    Error: NotRequired[str],
```

1. See [:material-code-brackets: DataCatalogTypeType](./literals.md#datacatalogtypetype) 
2. See [:material-code-brackets: DataCatalogStatusType](./literals.md#datacatalogstatustype) 
3. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
## CreateNamedQueryInputRequestTypeDef

```python
# CreateNamedQueryInputRequestTypeDef definition

class CreateNamedQueryInputRequestTypeDef(TypedDict):
    Name: str,
    Database: str,
    QueryString: str,
    Description: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    WorkGroup: NotRequired[str],
```

## CreateNotebookInputRequestTypeDef

```python
# CreateNotebookInputRequestTypeDef definition

class CreateNotebookInputRequestTypeDef(TypedDict):
    WorkGroup: str,
    Name: str,
    ClientRequestToken: NotRequired[str],
```

## CreatePreparedStatementInputRequestTypeDef

```python
# CreatePreparedStatementInputRequestTypeDef definition

class CreatePreparedStatementInputRequestTypeDef(TypedDict):
    StatementName: str,
    WorkGroup: str,
    QueryStatement: str,
    Description: NotRequired[str],
```

## CreatePresignedNotebookUrlRequestRequestTypeDef

```python
# CreatePresignedNotebookUrlRequestRequestTypeDef definition

class CreatePresignedNotebookUrlRequestRequestTypeDef(TypedDict):
    SessionId: str,
```

## CustomerContentEncryptionConfigurationTypeDef

```python
# CustomerContentEncryptionConfigurationTypeDef definition

class CustomerContentEncryptionConfigurationTypeDef(TypedDict):
    KmsKey: str,
```

## DataCatalogSummaryTypeDef

```python
# DataCatalogSummaryTypeDef definition

class DataCatalogSummaryTypeDef(TypedDict):
    CatalogName: NotRequired[str],
    Type: NotRequired[DataCatalogTypeType],  # (1)
    Status: NotRequired[DataCatalogStatusType],  # (2)
    ConnectionType: NotRequired[ConnectionTypeType],  # (3)
    Error: NotRequired[str],
```

1. See [:material-code-brackets: DataCatalogTypeType](./literals.md#datacatalogtypetype) 
2. See [:material-code-brackets: DataCatalogStatusType](./literals.md#datacatalogstatustype) 
3. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
## DatabaseTypeDef

```python
# DatabaseTypeDef definition

class DatabaseTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
```

## DatumTypeDef

```python
# DatumTypeDef definition

class DatumTypeDef(TypedDict):
    VarCharValue: NotRequired[str],
```

## DeleteCapacityReservationInputRequestTypeDef

```python
# DeleteCapacityReservationInputRequestTypeDef definition

class DeleteCapacityReservationInputRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteDataCatalogInputRequestTypeDef

```python
# DeleteDataCatalogInputRequestTypeDef definition

class DeleteDataCatalogInputRequestTypeDef(TypedDict):
    Name: str,
    DeleteCatalogOnly: NotRequired[bool],
```

## DeleteNamedQueryInputRequestTypeDef

```python
# DeleteNamedQueryInputRequestTypeDef definition

class DeleteNamedQueryInputRequestTypeDef(TypedDict):
    NamedQueryId: str,
```

## DeleteNotebookInputRequestTypeDef

```python
# DeleteNotebookInputRequestTypeDef definition

class DeleteNotebookInputRequestTypeDef(TypedDict):
    NotebookId: str,
```

## DeletePreparedStatementInputRequestTypeDef

```python
# DeletePreparedStatementInputRequestTypeDef definition

class DeletePreparedStatementInputRequestTypeDef(TypedDict):
    StatementName: str,
    WorkGroup: str,
```

## DeleteWorkGroupInputRequestTypeDef

```python
# DeleteWorkGroupInputRequestTypeDef definition

class DeleteWorkGroupInputRequestTypeDef(TypedDict):
    WorkGroup: str,
    RecursiveDeleteOption: NotRequired[bool],
```

## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    EncryptionOption: EncryptionOptionType,  # (1)
    KmsKey: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionOptionType](./literals.md#encryptionoptiontype) 
## EngineConfigurationOutputTypeDef

```python
# EngineConfigurationOutputTypeDef definition

class EngineConfigurationOutputTypeDef(TypedDict):
    MaxConcurrentDpus: int,
    CoordinatorDpuSize: NotRequired[int],
    DefaultExecutorDpuSize: NotRequired[int],
    AdditionalConfigs: NotRequired[Dict[str, str]],
    SparkProperties: NotRequired[Dict[str, str]],
```

## EngineConfigurationTypeDef

```python
# EngineConfigurationTypeDef definition

class EngineConfigurationTypeDef(TypedDict):
    MaxConcurrentDpus: int,
    CoordinatorDpuSize: NotRequired[int],
    DefaultExecutorDpuSize: NotRequired[int],
    AdditionalConfigs: NotRequired[Mapping[str, str]],
    SparkProperties: NotRequired[Mapping[str, str]],
```

## EngineVersionTypeDef

```python
# EngineVersionTypeDef definition

class EngineVersionTypeDef(TypedDict):
    SelectedEngineVersion: NotRequired[str],
    EffectiveEngineVersion: NotRequired[str],
```

## ExecutorsSummaryTypeDef

```python
# ExecutorsSummaryTypeDef definition

class ExecutorsSummaryTypeDef(TypedDict):
    ExecutorId: str,
    ExecutorType: NotRequired[ExecutorTypeType],  # (1)
    StartDateTime: NotRequired[int],
    TerminationDateTime: NotRequired[int],
    ExecutorState: NotRequired[ExecutorStateType],  # (2)
    ExecutorSize: NotRequired[int],
```

1. See [:material-code-brackets: ExecutorTypeType](./literals.md#executortypetype) 
2. See [:material-code-brackets: ExecutorStateType](./literals.md#executorstatetype) 
## ExportNotebookInputRequestTypeDef

```python
# ExportNotebookInputRequestTypeDef definition

class ExportNotebookInputRequestTypeDef(TypedDict):
    NotebookId: str,
```

## NotebookMetadataTypeDef

```python
# NotebookMetadataTypeDef definition

class NotebookMetadataTypeDef(TypedDict):
    NotebookId: NotRequired[str],
    Name: NotRequired[str],
    WorkGroup: NotRequired[str],
    CreationTime: NotRequired[datetime],
    Type: NotRequired[NotebookTypeType],  # (1)
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: NotebookTypeType](./literals.md#notebooktypetype) 
## FilterDefinitionTypeDef

```python
# FilterDefinitionTypeDef definition

class FilterDefinitionTypeDef(TypedDict):
    Name: NotRequired[str],
```

## GetCalculationExecutionCodeRequestRequestTypeDef

```python
# GetCalculationExecutionCodeRequestRequestTypeDef definition

class GetCalculationExecutionCodeRequestRequestTypeDef(TypedDict):
    CalculationExecutionId: str,
```

## GetCalculationExecutionRequestRequestTypeDef

```python
# GetCalculationExecutionRequestRequestTypeDef definition

class GetCalculationExecutionRequestRequestTypeDef(TypedDict):
    CalculationExecutionId: str,
```

## GetCalculationExecutionStatusRequestRequestTypeDef

```python
# GetCalculationExecutionStatusRequestRequestTypeDef definition

class GetCalculationExecutionStatusRequestRequestTypeDef(TypedDict):
    CalculationExecutionId: str,
```

## GetCapacityAssignmentConfigurationInputRequestTypeDef

```python
# GetCapacityAssignmentConfigurationInputRequestTypeDef definition

class GetCapacityAssignmentConfigurationInputRequestTypeDef(TypedDict):
    CapacityReservationName: str,
```

## GetCapacityReservationInputRequestTypeDef

```python
# GetCapacityReservationInputRequestTypeDef definition

class GetCapacityReservationInputRequestTypeDef(TypedDict):
    Name: str,
```

## GetDataCatalogInputRequestTypeDef

```python
# GetDataCatalogInputRequestTypeDef definition

class GetDataCatalogInputRequestTypeDef(TypedDict):
    Name: str,
    WorkGroup: NotRequired[str],
```

## GetDatabaseInputRequestTypeDef

```python
# GetDatabaseInputRequestTypeDef definition

class GetDatabaseInputRequestTypeDef(TypedDict):
    CatalogName: str,
    DatabaseName: str,
    WorkGroup: NotRequired[str],
```

## GetNamedQueryInputRequestTypeDef

```python
# GetNamedQueryInputRequestTypeDef definition

class GetNamedQueryInputRequestTypeDef(TypedDict):
    NamedQueryId: str,
```

## GetNotebookMetadataInputRequestTypeDef

```python
# GetNotebookMetadataInputRequestTypeDef definition

class GetNotebookMetadataInputRequestTypeDef(TypedDict):
    NotebookId: str,
```

## GetPreparedStatementInputRequestTypeDef

```python
# GetPreparedStatementInputRequestTypeDef definition

class GetPreparedStatementInputRequestTypeDef(TypedDict):
    StatementName: str,
    WorkGroup: str,
```

## GetQueryExecutionInputRequestTypeDef

```python
# GetQueryExecutionInputRequestTypeDef definition

class GetQueryExecutionInputRequestTypeDef(TypedDict):
    QueryExecutionId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetQueryResultsInputRequestTypeDef

```python
# GetQueryResultsInputRequestTypeDef definition

class GetQueryResultsInputRequestTypeDef(TypedDict):
    QueryExecutionId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetQueryRuntimeStatisticsInputRequestTypeDef

```python
# GetQueryRuntimeStatisticsInputRequestTypeDef definition

class GetQueryRuntimeStatisticsInputRequestTypeDef(TypedDict):
    QueryExecutionId: str,
```

## GetSessionRequestRequestTypeDef

```python
# GetSessionRequestRequestTypeDef definition

class GetSessionRequestRequestTypeDef(TypedDict):
    SessionId: str,
```

## SessionStatisticsTypeDef

```python
# SessionStatisticsTypeDef definition

class SessionStatisticsTypeDef(TypedDict):
    DpuExecutionInMillis: NotRequired[int],
```

## SessionStatusTypeDef

```python
# SessionStatusTypeDef definition

class SessionStatusTypeDef(TypedDict):
    StartDateTime: NotRequired[datetime],
    LastModifiedDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
    IdleSinceDateTime: NotRequired[datetime],
    State: NotRequired[SessionStateType],  # (1)
    StateChangeReason: NotRequired[str],
```

1. See [:material-code-brackets: SessionStateType](./literals.md#sessionstatetype) 
## GetSessionStatusRequestRequestTypeDef

```python
# GetSessionStatusRequestRequestTypeDef definition

class GetSessionStatusRequestRequestTypeDef(TypedDict):
    SessionId: str,
```

## GetTableMetadataInputRequestTypeDef

```python
# GetTableMetadataInputRequestTypeDef definition

class GetTableMetadataInputRequestTypeDef(TypedDict):
    CatalogName: str,
    DatabaseName: str,
    TableName: str,
    WorkGroup: NotRequired[str],
```

## GetWorkGroupInputRequestTypeDef

```python
# GetWorkGroupInputRequestTypeDef definition

class GetWorkGroupInputRequestTypeDef(TypedDict):
    WorkGroup: str,
```

## IdentityCenterConfigurationTypeDef

```python
# IdentityCenterConfigurationTypeDef definition

class IdentityCenterConfigurationTypeDef(TypedDict):
    EnableIdentityCenter: NotRequired[bool],
    IdentityCenterInstanceArn: NotRequired[str],
```

## ImportNotebookInputRequestTypeDef

```python
# ImportNotebookInputRequestTypeDef definition

class ImportNotebookInputRequestTypeDef(TypedDict):
    WorkGroup: str,
    Name: str,
    Type: NotebookTypeType,  # (1)
    Payload: NotRequired[str],
    NotebookS3LocationUri: NotRequired[str],
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-brackets: NotebookTypeType](./literals.md#notebooktypetype) 
## ListApplicationDPUSizesInputRequestTypeDef

```python
# ListApplicationDPUSizesInputRequestTypeDef definition

class ListApplicationDPUSizesInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCalculationExecutionsRequestRequestTypeDef

```python
# ListCalculationExecutionsRequestRequestTypeDef definition

class ListCalculationExecutionsRequestRequestTypeDef(TypedDict):
    SessionId: str,
    StateFilter: NotRequired[CalculationExecutionStateType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: CalculationExecutionStateType](./literals.md#calculationexecutionstatetype) 
## ListCapacityReservationsInputRequestTypeDef

```python
# ListCapacityReservationsInputRequestTypeDef definition

class ListCapacityReservationsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDataCatalogsInputRequestTypeDef

```python
# ListDataCatalogsInputRequestTypeDef definition

class ListDataCatalogsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    WorkGroup: NotRequired[str],
```

## ListDatabasesInputRequestTypeDef

```python
# ListDatabasesInputRequestTypeDef definition

class ListDatabasesInputRequestTypeDef(TypedDict):
    CatalogName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    WorkGroup: NotRequired[str],
```

## ListEngineVersionsInputRequestTypeDef

```python
# ListEngineVersionsInputRequestTypeDef definition

class ListEngineVersionsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListExecutorsRequestRequestTypeDef

```python
# ListExecutorsRequestRequestTypeDef definition

class ListExecutorsRequestRequestTypeDef(TypedDict):
    SessionId: str,
    ExecutorStateFilter: NotRequired[ExecutorStateType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ExecutorStateType](./literals.md#executorstatetype) 
## ListNamedQueriesInputRequestTypeDef

```python
# ListNamedQueriesInputRequestTypeDef definition

class ListNamedQueriesInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    WorkGroup: NotRequired[str],
```

## ListNotebookSessionsRequestRequestTypeDef

```python
# ListNotebookSessionsRequestRequestTypeDef definition

class ListNotebookSessionsRequestRequestTypeDef(TypedDict):
    NotebookId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## NotebookSessionSummaryTypeDef

```python
# NotebookSessionSummaryTypeDef definition

class NotebookSessionSummaryTypeDef(TypedDict):
    SessionId: NotRequired[str],
    CreationTime: NotRequired[datetime],
```

## ListPreparedStatementsInputRequestTypeDef

```python
# ListPreparedStatementsInputRequestTypeDef definition

class ListPreparedStatementsInputRequestTypeDef(TypedDict):
    WorkGroup: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PreparedStatementSummaryTypeDef

```python
# PreparedStatementSummaryTypeDef definition

class PreparedStatementSummaryTypeDef(TypedDict):
    StatementName: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
```

## ListQueryExecutionsInputRequestTypeDef

```python
# ListQueryExecutionsInputRequestTypeDef definition

class ListQueryExecutionsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    WorkGroup: NotRequired[str],
```

## ListSessionsRequestRequestTypeDef

```python
# ListSessionsRequestRequestTypeDef definition

class ListSessionsRequestRequestTypeDef(TypedDict):
    WorkGroup: str,
    StateFilter: NotRequired[SessionStateType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: SessionStateType](./literals.md#sessionstatetype) 
## ListTableMetadataInputRequestTypeDef

```python
# ListTableMetadataInputRequestTypeDef definition

class ListTableMetadataInputRequestTypeDef(TypedDict):
    CatalogName: str,
    DatabaseName: str,
    Expression: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    WorkGroup: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListWorkGroupsInputRequestTypeDef

```python
# ListWorkGroupsInputRequestTypeDef definition

class ListWorkGroupsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## QueryExecutionContextTypeDef

```python
# QueryExecutionContextTypeDef definition

class QueryExecutionContextTypeDef(TypedDict):
    Database: NotRequired[str],
    Catalog: NotRequired[str],
```

## ResultReuseInformationTypeDef

```python
# ResultReuseInformationTypeDef definition

class ResultReuseInformationTypeDef(TypedDict):
    ReusedPreviousResult: bool,
```

## QueryResultsS3AccessGrantsConfigurationTypeDef

```python
# QueryResultsS3AccessGrantsConfigurationTypeDef definition

class QueryResultsS3AccessGrantsConfigurationTypeDef(TypedDict):
    EnableS3AccessGrants: bool,
    AuthenticationType: AuthenticationTypeType,  # (1)
    CreateUserLevelPrefix: NotRequired[bool],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
## QueryRuntimeStatisticsRowsTypeDef

```python
# QueryRuntimeStatisticsRowsTypeDef definition

class QueryRuntimeStatisticsRowsTypeDef(TypedDict):
    InputRows: NotRequired[int],
    InputBytes: NotRequired[int],
    OutputBytes: NotRequired[int],
    OutputRows: NotRequired[int],
```

## QueryRuntimeStatisticsTimelineTypeDef

```python
# QueryRuntimeStatisticsTimelineTypeDef definition

class QueryRuntimeStatisticsTimelineTypeDef(TypedDict):
    QueryQueueTimeInMillis: NotRequired[int],
    ServicePreProcessingTimeInMillis: NotRequired[int],
    QueryPlanningTimeInMillis: NotRequired[int],
    EngineExecutionTimeInMillis: NotRequired[int],
    ServiceProcessingTimeInMillis: NotRequired[int],
    TotalExecutionTimeInMillis: NotRequired[int],
```

## QueryStagePlanNodeTypeDef

```python
# QueryStagePlanNodeTypeDef definition

class QueryStagePlanNodeTypeDef(TypedDict):
    Name: NotRequired[str],
    Identifier: NotRequired[str],
    Children: NotRequired[List[Dict[str, Any]]],
    RemoteSources: NotRequired[List[str]],
```

## ResultReuseByAgeConfigurationTypeDef

```python
# ResultReuseByAgeConfigurationTypeDef definition

class ResultReuseByAgeConfigurationTypeDef(TypedDict):
    Enabled: bool,
    MaxAgeInMinutes: NotRequired[int],
```

## StopCalculationExecutionRequestRequestTypeDef

```python
# StopCalculationExecutionRequestRequestTypeDef definition

class StopCalculationExecutionRequestRequestTypeDef(TypedDict):
    CalculationExecutionId: str,
```

## StopQueryExecutionInputRequestTypeDef

```python
# StopQueryExecutionInputRequestTypeDef definition

class StopQueryExecutionInputRequestTypeDef(TypedDict):
    QueryExecutionId: str,
```

## TerminateSessionRequestRequestTypeDef

```python
# TerminateSessionRequestRequestTypeDef definition

class TerminateSessionRequestRequestTypeDef(TypedDict):
    SessionId: str,
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateCapacityReservationInputRequestTypeDef

```python
# UpdateCapacityReservationInputRequestTypeDef definition

class UpdateCapacityReservationInputRequestTypeDef(TypedDict):
    TargetDpus: int,
    Name: str,
```

## UpdateDataCatalogInputRequestTypeDef

```python
# UpdateDataCatalogInputRequestTypeDef definition

class UpdateDataCatalogInputRequestTypeDef(TypedDict):
    Name: str,
    Type: DataCatalogTypeType,  # (1)
    Description: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DataCatalogTypeType](./literals.md#datacatalogtypetype) 
## UpdateNamedQueryInputRequestTypeDef

```python
# UpdateNamedQueryInputRequestTypeDef definition

class UpdateNamedQueryInputRequestTypeDef(TypedDict):
    NamedQueryId: str,
    Name: str,
    QueryString: str,
    Description: NotRequired[str],
```

## UpdateNotebookInputRequestTypeDef

```python
# UpdateNotebookInputRequestTypeDef definition

class UpdateNotebookInputRequestTypeDef(TypedDict):
    NotebookId: str,
    Payload: str,
    Type: NotebookTypeType,  # (1)
    SessionId: NotRequired[str],
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-brackets: NotebookTypeType](./literals.md#notebooktypetype) 
## UpdateNotebookMetadataInputRequestTypeDef

```python
# UpdateNotebookMetadataInputRequestTypeDef definition

class UpdateNotebookMetadataInputRequestTypeDef(TypedDict):
    NotebookId: str,
    Name: str,
    ClientRequestToken: NotRequired[str],
```

## UpdatePreparedStatementInputRequestTypeDef

```python
# UpdatePreparedStatementInputRequestTypeDef definition

class UpdatePreparedStatementInputRequestTypeDef(TypedDict):
    StatementName: str,
    WorkGroup: str,
    QueryStatement: str,
    Description: NotRequired[str],
```

## QueryExecutionStatusTypeDef

```python
# QueryExecutionStatusTypeDef definition

class QueryExecutionStatusTypeDef(TypedDict):
    State: NotRequired[QueryExecutionStateType],  # (1)
    StateChangeReason: NotRequired[str],
    SubmissionDateTime: NotRequired[datetime],
    CompletionDateTime: NotRequired[datetime],
    AthenaError: NotRequired[AthenaErrorTypeDef],  # (2)
```

1. See [:material-code-brackets: QueryExecutionStateType](./literals.md#queryexecutionstatetype) 
2. See [:material-code-braces: AthenaErrorTypeDef](./type_defs.md#athenaerrortypedef) 
## CreateNamedQueryOutputTypeDef

```python
# CreateNamedQueryOutputTypeDef definition

class CreateNamedQueryOutputTypeDef(TypedDict):
    NamedQueryId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNotebookOutputTypeDef

```python
# CreateNotebookOutputTypeDef definition

class CreateNotebookOutputTypeDef(TypedDict):
    NotebookId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePresignedNotebookUrlResponseTypeDef

```python
# CreatePresignedNotebookUrlResponseTypeDef definition

class CreatePresignedNotebookUrlResponseTypeDef(TypedDict):
    NotebookUrl: str,
    AuthToken: str,
    AuthTokenExpirationTime: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCalculationExecutionCodeResponseTypeDef

```python
# GetCalculationExecutionCodeResponseTypeDef definition

class GetCalculationExecutionCodeResponseTypeDef(TypedDict):
    CodeBlock: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNamedQueryOutputTypeDef

```python
# GetNamedQueryOutputTypeDef definition

class GetNamedQueryOutputTypeDef(TypedDict):
    NamedQuery: NamedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamedQueryTypeDef](./type_defs.md#namedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportNotebookOutputTypeDef

```python
# ImportNotebookOutputTypeDef definition

class ImportNotebookOutputTypeDef(TypedDict):
    NotebookId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationDPUSizesOutputTypeDef

```python
# ListApplicationDPUSizesOutputTypeDef definition

class ListApplicationDPUSizesOutputTypeDef(TypedDict):
    ApplicationDPUSizes: List[ApplicationDPUSizesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationDPUSizesTypeDef](./type_defs.md#applicationdpusizestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNamedQueriesOutputTypeDef

```python
# ListNamedQueriesOutputTypeDef definition

class ListNamedQueriesOutputTypeDef(TypedDict):
    NamedQueryIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueryExecutionsOutputTypeDef

```python
# ListQueryExecutionsOutputTypeDef definition

class ListQueryExecutionsOutputTypeDef(TypedDict):
    QueryExecutionIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCalculationExecutionResponseTypeDef

```python
# StartCalculationExecutionResponseTypeDef definition

class StartCalculationExecutionResponseTypeDef(TypedDict):
    CalculationExecutionId: str,
    State: CalculationExecutionStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CalculationExecutionStateType](./literals.md#calculationexecutionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartQueryExecutionOutputTypeDef

```python
# StartQueryExecutionOutputTypeDef definition

class StartQueryExecutionOutputTypeDef(TypedDict):
    QueryExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSessionResponseTypeDef

```python
# StartSessionResponseTypeDef definition

class StartSessionResponseTypeDef(TypedDict):
    SessionId: str,
    State: SessionStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SessionStateType](./literals.md#sessionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopCalculationExecutionResponseTypeDef

```python
# StopCalculationExecutionResponseTypeDef definition

class StopCalculationExecutionResponseTypeDef(TypedDict):
    State: CalculationExecutionStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CalculationExecutionStateType](./literals.md#calculationexecutionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TerminateSessionResponseTypeDef

```python
# TerminateSessionResponseTypeDef definition

class TerminateSessionResponseTypeDef(TypedDict):
    State: SessionStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SessionStateType](./literals.md#sessionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetNamedQueryOutputTypeDef

```python
# BatchGetNamedQueryOutputTypeDef definition

class BatchGetNamedQueryOutputTypeDef(TypedDict):
    NamedQueries: List[NamedQueryTypeDef],  # (1)
    UnprocessedNamedQueryIds: List[UnprocessedNamedQueryIdTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: NamedQueryTypeDef](./type_defs.md#namedquerytypedef) 
2. See [:material-code-braces: UnprocessedNamedQueryIdTypeDef](./type_defs.md#unprocessednamedqueryidtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPreparedStatementOutputTypeDef

```python
# GetPreparedStatementOutputTypeDef definition

class GetPreparedStatementOutputTypeDef(TypedDict):
    PreparedStatement: PreparedStatementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PreparedStatementTypeDef](./type_defs.md#preparedstatementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetPreparedStatementOutputTypeDef

```python
# BatchGetPreparedStatementOutputTypeDef definition

class BatchGetPreparedStatementOutputTypeDef(TypedDict):
    PreparedStatements: List[PreparedStatementTypeDef],  # (1)
    UnprocessedPreparedStatementNames: List[UnprocessedPreparedStatementNameTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PreparedStatementTypeDef](./type_defs.md#preparedstatementtypedef) 
2. See [:material-code-braces: UnprocessedPreparedStatementNameTypeDef](./type_defs.md#unprocessedpreparedstatementnametypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartCalculationExecutionRequestRequestTypeDef

```python
# StartCalculationExecutionRequestRequestTypeDef definition

class StartCalculationExecutionRequestRequestTypeDef(TypedDict):
    SessionId: str,
    Description: NotRequired[str],
    CalculationConfiguration: NotRequired[CalculationConfigurationTypeDef],  # (1)
    CodeBlock: NotRequired[str],
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: CalculationConfigurationTypeDef](./type_defs.md#calculationconfigurationtypedef) 
## CalculationSummaryTypeDef

```python
# CalculationSummaryTypeDef definition

class CalculationSummaryTypeDef(TypedDict):
    CalculationExecutionId: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[CalculationStatusTypeDef],  # (1)
```

1. See [:material-code-braces: CalculationStatusTypeDef](./type_defs.md#calculationstatustypedef) 
## GetCalculationExecutionResponseTypeDef

```python
# GetCalculationExecutionResponseTypeDef definition

class GetCalculationExecutionResponseTypeDef(TypedDict):
    CalculationExecutionId: str,
    SessionId: str,
    Description: str,
    WorkingDirectory: str,
    Status: CalculationStatusTypeDef,  # (1)
    Statistics: CalculationStatisticsTypeDef,  # (2)
    Result: CalculationResultTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: CalculationStatusTypeDef](./type_defs.md#calculationstatustypedef) 
2. See [:material-code-braces: CalculationStatisticsTypeDef](./type_defs.md#calculationstatisticstypedef) 
3. See [:material-code-braces: CalculationResultTypeDef](./type_defs.md#calculationresulttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCalculationExecutionStatusResponseTypeDef

```python
# GetCalculationExecutionStatusResponseTypeDef definition

class GetCalculationExecutionStatusResponseTypeDef(TypedDict):
    Status: CalculationStatusTypeDef,  # (1)
    Statistics: CalculationStatisticsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CalculationStatusTypeDef](./type_defs.md#calculationstatustypedef) 
2. See [:material-code-braces: CalculationStatisticsTypeDef](./type_defs.md#calculationstatisticstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CapacityReservationTypeDef

```python
# CapacityReservationTypeDef definition

class CapacityReservationTypeDef(TypedDict):
    Name: str,
    Status: CapacityReservationStatusType,  # (1)
    TargetDpus: int,
    AllocatedDpus: int,
    CreationTime: datetime,
    LastAllocation: NotRequired[CapacityAllocationTypeDef],  # (2)
    LastSuccessfulAllocationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: CapacityReservationStatusType](./literals.md#capacityreservationstatustype) 
2. See [:material-code-braces: CapacityAllocationTypeDef](./type_defs.md#capacityallocationtypedef) 
## CapacityAssignmentConfigurationTypeDef

```python
# CapacityAssignmentConfigurationTypeDef definition

class CapacityAssignmentConfigurationTypeDef(TypedDict):
    CapacityReservationName: NotRequired[str],
    CapacityAssignments: NotRequired[List[CapacityAssignmentOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: CapacityAssignmentOutputTypeDef](./type_defs.md#capacityassignmentoutputtypedef) 
## ResultSetMetadataTypeDef

```python
# ResultSetMetadataTypeDef definition

class ResultSetMetadataTypeDef(TypedDict):
    ColumnInfo: NotRequired[List[ColumnInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
## TableMetadataTypeDef

```python
# TableMetadataTypeDef definition

class TableMetadataTypeDef(TypedDict):
    Name: str,
    CreateTime: NotRequired[datetime],
    LastAccessTime: NotRequired[datetime],
    TableType: NotRequired[str],
    Columns: NotRequired[List[ColumnTypeDef]],  # (1)
    PartitionKeys: NotRequired[List[ColumnTypeDef]],  # (1)
    Parameters: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
2. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
## CreateCapacityReservationInputRequestTypeDef

```python
# CreateCapacityReservationInputRequestTypeDef definition

class CreateCapacityReservationInputRequestTypeDef(TypedDict):
    TargetDpus: int,
    Name: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDataCatalogInputRequestTypeDef

```python
# CreateDataCatalogInputRequestTypeDef definition

class CreateDataCatalogInputRequestTypeDef(TypedDict):
    Name: str,
    Type: DataCatalogTypeType,  # (1)
    Description: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: DataCatalogTypeType](./literals.md#datacatalogtypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateDataCatalogOutputTypeDef

```python
# CreateDataCatalogOutputTypeDef definition

class CreateDataCatalogOutputTypeDef(TypedDict):
    DataCatalog: DataCatalogTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataCatalogTypeDef](./type_defs.md#datacatalogtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataCatalogOutputTypeDef

```python
# DeleteDataCatalogOutputTypeDef definition

class DeleteDataCatalogOutputTypeDef(TypedDict):
    DataCatalog: DataCatalogTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataCatalogTypeDef](./type_defs.md#datacatalogtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataCatalogOutputTypeDef

```python
# GetDataCatalogOutputTypeDef definition

class GetDataCatalogOutputTypeDef(TypedDict):
    DataCatalog: DataCatalogTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataCatalogTypeDef](./type_defs.md#datacatalogtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataCatalogsOutputTypeDef

```python
# ListDataCatalogsOutputTypeDef definition

class ListDataCatalogsOutputTypeDef(TypedDict):
    DataCatalogsSummary: List[DataCatalogSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataCatalogSummaryTypeDef](./type_defs.md#datacatalogsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDatabaseOutputTypeDef

```python
# GetDatabaseOutputTypeDef definition

class GetDatabaseOutputTypeDef(TypedDict):
    Database: DatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatabasesOutputTypeDef

```python
# ListDatabasesOutputTypeDef definition

class ListDatabasesOutputTypeDef(TypedDict):
    DatabaseList: List[DatabaseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RowTypeDef

```python
# RowTypeDef definition

class RowTypeDef(TypedDict):
    Data: NotRequired[List[DatumTypeDef]],  # (1)
```

1. See [:material-code-braces: DatumTypeDef](./type_defs.md#datumtypedef) 
## ResultConfigurationTypeDef

```python
# ResultConfigurationTypeDef definition

class ResultConfigurationTypeDef(TypedDict):
    OutputLocation: NotRequired[str],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (1)
    ExpectedBucketOwner: NotRequired[str],
    AclConfiguration: NotRequired[AclConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
2. See [:material-code-braces: AclConfigurationTypeDef](./type_defs.md#aclconfigurationtypedef) 
## ResultConfigurationUpdatesTypeDef

```python
# ResultConfigurationUpdatesTypeDef definition

class ResultConfigurationUpdatesTypeDef(TypedDict):
    OutputLocation: NotRequired[str],
    RemoveOutputLocation: NotRequired[bool],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (1)
    RemoveEncryptionConfiguration: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
    RemoveExpectedBucketOwner: NotRequired[bool],
    AclConfiguration: NotRequired[AclConfigurationTypeDef],  # (2)
    RemoveAclConfiguration: NotRequired[bool],
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
2. See [:material-code-braces: AclConfigurationTypeDef](./type_defs.md#aclconfigurationtypedef) 
## SessionConfigurationTypeDef

```python
# SessionConfigurationTypeDef definition

class SessionConfigurationTypeDef(TypedDict):
    ExecutionRole: NotRequired[str],
    WorkingDirectory: NotRequired[str],
    IdleTimeoutSeconds: NotRequired[int],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## StartSessionRequestRequestTypeDef

```python
# StartSessionRequestRequestTypeDef definition

class StartSessionRequestRequestTypeDef(TypedDict):
    WorkGroup: str,
    EngineConfiguration: EngineConfigurationTypeDef,  # (1)
    Description: NotRequired[str],
    NotebookVersion: NotRequired[str],
    SessionIdleTimeoutInMinutes: NotRequired[int],
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: EngineConfigurationTypeDef](./type_defs.md#engineconfigurationtypedef) 
## ListEngineVersionsOutputTypeDef

```python
# ListEngineVersionsOutputTypeDef definition

class ListEngineVersionsOutputTypeDef(TypedDict):
    EngineVersions: List[EngineVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkGroupSummaryTypeDef

```python
# WorkGroupSummaryTypeDef definition

class WorkGroupSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    State: NotRequired[WorkGroupStateType],  # (1)
    Description: NotRequired[str],
    CreationTime: NotRequired[datetime],
    EngineVersion: NotRequired[EngineVersionTypeDef],  # (2)
    IdentityCenterApplicationArn: NotRequired[str],
```

1. See [:material-code-brackets: WorkGroupStateType](./literals.md#workgroupstatetype) 
2. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
## ListExecutorsResponseTypeDef

```python
# ListExecutorsResponseTypeDef definition

class ListExecutorsResponseTypeDef(TypedDict):
    SessionId: str,
    ExecutorsSummary: List[ExecutorsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExecutorsSummaryTypeDef](./type_defs.md#executorssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportNotebookOutputTypeDef

```python
# ExportNotebookOutputTypeDef definition

class ExportNotebookOutputTypeDef(TypedDict):
    NotebookMetadata: NotebookMetadataTypeDef,  # (1)
    Payload: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotebookMetadataTypeDef](./type_defs.md#notebookmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNotebookMetadataOutputTypeDef

```python
# GetNotebookMetadataOutputTypeDef definition

class GetNotebookMetadataOutputTypeDef(TypedDict):
    NotebookMetadata: NotebookMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotebookMetadataTypeDef](./type_defs.md#notebookmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNotebookMetadataOutputTypeDef

```python
# ListNotebookMetadataOutputTypeDef definition

class ListNotebookMetadataOutputTypeDef(TypedDict):
    NotebookMetadataList: List[NotebookMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NotebookMetadataTypeDef](./type_defs.md#notebookmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNotebookMetadataInputRequestTypeDef

```python
# ListNotebookMetadataInputRequestTypeDef definition

class ListNotebookMetadataInputRequestTypeDef(TypedDict):
    WorkGroup: str,
    Filters: NotRequired[FilterDefinitionTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterDefinitionTypeDef](./type_defs.md#filterdefinitiontypedef) 
## GetQueryResultsInputPaginateTypeDef

```python
# GetQueryResultsInputPaginateTypeDef definition

class GetQueryResultsInputPaginateTypeDef(TypedDict):
    QueryExecutionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataCatalogsInputPaginateTypeDef

```python
# ListDataCatalogsInputPaginateTypeDef definition

class ListDataCatalogsInputPaginateTypeDef(TypedDict):
    WorkGroup: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatabasesInputPaginateTypeDef

```python
# ListDatabasesInputPaginateTypeDef definition

class ListDatabasesInputPaginateTypeDef(TypedDict):
    CatalogName: str,
    WorkGroup: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNamedQueriesInputPaginateTypeDef

```python
# ListNamedQueriesInputPaginateTypeDef definition

class ListNamedQueriesInputPaginateTypeDef(TypedDict):
    WorkGroup: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueryExecutionsInputPaginateTypeDef

```python
# ListQueryExecutionsInputPaginateTypeDef definition

class ListQueryExecutionsInputPaginateTypeDef(TypedDict):
    WorkGroup: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTableMetadataInputPaginateTypeDef

```python
# ListTableMetadataInputPaginateTypeDef definition

class ListTableMetadataInputPaginateTypeDef(TypedDict):
    CatalogName: str,
    DatabaseName: str,
    Expression: NotRequired[str],
    WorkGroup: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceInputPaginateTypeDef

```python
# ListTagsForResourceInputPaginateTypeDef definition

class ListTagsForResourceInputPaginateTypeDef(TypedDict):
    ResourceARN: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetSessionStatusResponseTypeDef

```python
# GetSessionStatusResponseTypeDef definition

class GetSessionStatusResponseTypeDef(TypedDict):
    SessionId: str,
    Status: SessionStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionStatusTypeDef](./type_defs.md#sessionstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SessionSummaryTypeDef

```python
# SessionSummaryTypeDef definition

class SessionSummaryTypeDef(TypedDict):
    SessionId: NotRequired[str],
    Description: NotRequired[str],
    EngineVersion: NotRequired[EngineVersionTypeDef],  # (1)
    NotebookVersion: NotRequired[str],
    Status: NotRequired[SessionStatusTypeDef],  # (2)
```

1. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
2. See [:material-code-braces: SessionStatusTypeDef](./type_defs.md#sessionstatustypedef) 
## ListNotebookSessionsResponseTypeDef

```python
# ListNotebookSessionsResponseTypeDef definition

class ListNotebookSessionsResponseTypeDef(TypedDict):
    NotebookSessionsList: List[NotebookSessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: NotebookSessionSummaryTypeDef](./type_defs.md#notebooksessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPreparedStatementsOutputTypeDef

```python
# ListPreparedStatementsOutputTypeDef definition

class ListPreparedStatementsOutputTypeDef(TypedDict):
    PreparedStatements: List[PreparedStatementSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PreparedStatementSummaryTypeDef](./type_defs.md#preparedstatementsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryExecutionStatisticsTypeDef

```python
# QueryExecutionStatisticsTypeDef definition

class QueryExecutionStatisticsTypeDef(TypedDict):
    EngineExecutionTimeInMillis: NotRequired[int],
    DataScannedInBytes: NotRequired[int],
    DataManifestLocation: NotRequired[str],
    TotalExecutionTimeInMillis: NotRequired[int],
    QueryQueueTimeInMillis: NotRequired[int],
    ServicePreProcessingTimeInMillis: NotRequired[int],
    QueryPlanningTimeInMillis: NotRequired[int],
    ServiceProcessingTimeInMillis: NotRequired[int],
    ResultReuseInformation: NotRequired[ResultReuseInformationTypeDef],  # (1)
```

1. See [:material-code-braces: ResultReuseInformationTypeDef](./type_defs.md#resultreuseinformationtypedef) 
## QueryStageTypeDef

```python
# QueryStageTypeDef definition

class QueryStageTypeDef(TypedDict):
    StageId: NotRequired[int],
    State: NotRequired[str],
    OutputBytes: NotRequired[int],
    OutputRows: NotRequired[int],
    InputBytes: NotRequired[int],
    InputRows: NotRequired[int],
    ExecutionTime: NotRequired[int],
    QueryStagePlan: NotRequired[QueryStagePlanNodeTypeDef],  # (1)
    SubStages: NotRequired[List[Dict[str, Any]]],
```

1. See [:material-code-braces: QueryStagePlanNodeTypeDef](./type_defs.md#querystageplannodetypedef) 
## ResultReuseConfigurationTypeDef

```python
# ResultReuseConfigurationTypeDef definition

class ResultReuseConfigurationTypeDef(TypedDict):
    ResultReuseByAgeConfiguration: NotRequired[ResultReuseByAgeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ResultReuseByAgeConfigurationTypeDef](./type_defs.md#resultreusebyageconfigurationtypedef) 
## ListCalculationExecutionsResponseTypeDef

```python
# ListCalculationExecutionsResponseTypeDef definition

class ListCalculationExecutionsResponseTypeDef(TypedDict):
    Calculations: List[CalculationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CalculationSummaryTypeDef](./type_defs.md#calculationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCapacityReservationOutputTypeDef

```python
# GetCapacityReservationOutputTypeDef definition

class GetCapacityReservationOutputTypeDef(TypedDict):
    CapacityReservation: CapacityReservationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapacityReservationTypeDef](./type_defs.md#capacityreservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCapacityReservationsOutputTypeDef

```python
# ListCapacityReservationsOutputTypeDef definition

class ListCapacityReservationsOutputTypeDef(TypedDict):
    CapacityReservations: List[CapacityReservationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CapacityReservationTypeDef](./type_defs.md#capacityreservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCapacityAssignmentConfigurationOutputTypeDef

```python
# GetCapacityAssignmentConfigurationOutputTypeDef definition

class GetCapacityAssignmentConfigurationOutputTypeDef(TypedDict):
    CapacityAssignmentConfiguration: CapacityAssignmentConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapacityAssignmentConfigurationTypeDef](./type_defs.md#capacityassignmentconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutCapacityAssignmentConfigurationInputRequestTypeDef

```python
# PutCapacityAssignmentConfigurationInputRequestTypeDef definition

class PutCapacityAssignmentConfigurationInputRequestTypeDef(TypedDict):
    CapacityReservationName: str,
    CapacityAssignments: Sequence[CapacityAssignmentUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CapacityAssignmentTypeDef](./type_defs.md#capacityassignmenttypedef) [:material-code-braces: CapacityAssignmentOutputTypeDef](./type_defs.md#capacityassignmentoutputtypedef) 
## GetTableMetadataOutputTypeDef

```python
# GetTableMetadataOutputTypeDef definition

class GetTableMetadataOutputTypeDef(TypedDict):
    TableMetadata: TableMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableMetadataTypeDef](./type_defs.md#tablemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTableMetadataOutputTypeDef

```python
# ListTableMetadataOutputTypeDef definition

class ListTableMetadataOutputTypeDef(TypedDict):
    TableMetadataList: List[TableMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TableMetadataTypeDef](./type_defs.md#tablemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResultSetTypeDef

```python
# ResultSetTypeDef definition

class ResultSetTypeDef(TypedDict):
    Rows: NotRequired[List[RowTypeDef]],  # (1)
    ResultSetMetadata: NotRequired[ResultSetMetadataTypeDef],  # (2)
```

1. See [:material-code-braces: RowTypeDef](./type_defs.md#rowtypedef) 
2. See [:material-code-braces: ResultSetMetadataTypeDef](./type_defs.md#resultsetmetadatatypedef) 
## WorkGroupConfigurationTypeDef

```python
# WorkGroupConfigurationTypeDef definition

class WorkGroupConfigurationTypeDef(TypedDict):
    ResultConfiguration: NotRequired[ResultConfigurationTypeDef],  # (1)
    EnforceWorkGroupConfiguration: NotRequired[bool],
    PublishCloudWatchMetricsEnabled: NotRequired[bool],
    BytesScannedCutoffPerQuery: NotRequired[int],
    RequesterPaysEnabled: NotRequired[bool],
    EngineVersion: NotRequired[EngineVersionTypeDef],  # (2)
    AdditionalConfiguration: NotRequired[str],
    ExecutionRole: NotRequired[str],
    CustomerContentEncryptionConfiguration: NotRequired[CustomerContentEncryptionConfigurationTypeDef],  # (3)
    EnableMinimumEncryptionConfiguration: NotRequired[bool],
    IdentityCenterConfiguration: NotRequired[IdentityCenterConfigurationTypeDef],  # (4)
    QueryResultsS3AccessGrantsConfiguration: NotRequired[QueryResultsS3AccessGrantsConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: ResultConfigurationTypeDef](./type_defs.md#resultconfigurationtypedef) 
2. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
3. See [:material-code-braces: CustomerContentEncryptionConfigurationTypeDef](./type_defs.md#customercontentencryptionconfigurationtypedef) 
4. See [:material-code-braces: IdentityCenterConfigurationTypeDef](./type_defs.md#identitycenterconfigurationtypedef) 
5. See [:material-code-braces: QueryResultsS3AccessGrantsConfigurationTypeDef](./type_defs.md#queryresultss3accessgrantsconfigurationtypedef) 
## WorkGroupConfigurationUpdatesTypeDef

```python
# WorkGroupConfigurationUpdatesTypeDef definition

class WorkGroupConfigurationUpdatesTypeDef(TypedDict):
    EnforceWorkGroupConfiguration: NotRequired[bool],
    ResultConfigurationUpdates: NotRequired[ResultConfigurationUpdatesTypeDef],  # (1)
    PublishCloudWatchMetricsEnabled: NotRequired[bool],
    BytesScannedCutoffPerQuery: NotRequired[int],
    RemoveBytesScannedCutoffPerQuery: NotRequired[bool],
    RequesterPaysEnabled: NotRequired[bool],
    EngineVersion: NotRequired[EngineVersionTypeDef],  # (2)
    RemoveCustomerContentEncryptionConfiguration: NotRequired[bool],
    AdditionalConfiguration: NotRequired[str],
    ExecutionRole: NotRequired[str],
    CustomerContentEncryptionConfiguration: NotRequired[CustomerContentEncryptionConfigurationTypeDef],  # (3)
    EnableMinimumEncryptionConfiguration: NotRequired[bool],
    QueryResultsS3AccessGrantsConfiguration: NotRequired[QueryResultsS3AccessGrantsConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: ResultConfigurationUpdatesTypeDef](./type_defs.md#resultconfigurationupdatestypedef) 
2. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
3. See [:material-code-braces: CustomerContentEncryptionConfigurationTypeDef](./type_defs.md#customercontentencryptionconfigurationtypedef) 
4. See [:material-code-braces: QueryResultsS3AccessGrantsConfigurationTypeDef](./type_defs.md#queryresultss3accessgrantsconfigurationtypedef) 
## GetSessionResponseTypeDef

```python
# GetSessionResponseTypeDef definition

class GetSessionResponseTypeDef(TypedDict):
    SessionId: str,
    Description: str,
    WorkGroup: str,
    EngineVersion: str,
    EngineConfiguration: EngineConfigurationOutputTypeDef,  # (1)
    NotebookVersion: str,
    SessionConfiguration: SessionConfigurationTypeDef,  # (2)
    Status: SessionStatusTypeDef,  # (3)
    Statistics: SessionStatisticsTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: EngineConfigurationOutputTypeDef](./type_defs.md#engineconfigurationoutputtypedef) 
2. See [:material-code-braces: SessionConfigurationTypeDef](./type_defs.md#sessionconfigurationtypedef) 
3. See [:material-code-braces: SessionStatusTypeDef](./type_defs.md#sessionstatustypedef) 
4. See [:material-code-braces: SessionStatisticsTypeDef](./type_defs.md#sessionstatisticstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkGroupsOutputTypeDef

```python
# ListWorkGroupsOutputTypeDef definition

class ListWorkGroupsOutputTypeDef(TypedDict):
    WorkGroups: List[WorkGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkGroupSummaryTypeDef](./type_defs.md#workgroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSessionsResponseTypeDef

```python
# ListSessionsResponseTypeDef definition

class ListSessionsResponseTypeDef(TypedDict):
    Sessions: List[SessionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionSummaryTypeDef](./type_defs.md#sessionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryRuntimeStatisticsTypeDef

```python
# QueryRuntimeStatisticsTypeDef definition

class QueryRuntimeStatisticsTypeDef(TypedDict):
    Timeline: NotRequired[QueryRuntimeStatisticsTimelineTypeDef],  # (1)
    Rows: NotRequired[QueryRuntimeStatisticsRowsTypeDef],  # (2)
    OutputStage: NotRequired[QueryStageTypeDef],  # (3)
```

1. See [:material-code-braces: QueryRuntimeStatisticsTimelineTypeDef](./type_defs.md#queryruntimestatisticstimelinetypedef) 
2. See [:material-code-braces: QueryRuntimeStatisticsRowsTypeDef](./type_defs.md#queryruntimestatisticsrowstypedef) 
3. See [:material-code-braces: QueryStageTypeDef](./type_defs.md#querystagetypedef) 
## QueryExecutionTypeDef

```python
# QueryExecutionTypeDef definition

class QueryExecutionTypeDef(TypedDict):
    QueryExecutionId: NotRequired[str],
    Query: NotRequired[str],
    StatementType: NotRequired[StatementTypeType],  # (1)
    ResultConfiguration: NotRequired[ResultConfigurationTypeDef],  # (2)
    ResultReuseConfiguration: NotRequired[ResultReuseConfigurationTypeDef],  # (3)
    QueryExecutionContext: NotRequired[QueryExecutionContextTypeDef],  # (4)
    Status: NotRequired[QueryExecutionStatusTypeDef],  # (5)
    Statistics: NotRequired[QueryExecutionStatisticsTypeDef],  # (6)
    WorkGroup: NotRequired[str],
    EngineVersion: NotRequired[EngineVersionTypeDef],  # (7)
    ExecutionParameters: NotRequired[List[str]],
    SubstatementType: NotRequired[str],
    QueryResultsS3AccessGrantsConfiguration: NotRequired[QueryResultsS3AccessGrantsConfigurationTypeDef],  # (8)
```

1. See [:material-code-brackets: StatementTypeType](./literals.md#statementtypetype) 
2. See [:material-code-braces: ResultConfigurationTypeDef](./type_defs.md#resultconfigurationtypedef) 
3. See [:material-code-braces: ResultReuseConfigurationTypeDef](./type_defs.md#resultreuseconfigurationtypedef) 
4. See [:material-code-braces: QueryExecutionContextTypeDef](./type_defs.md#queryexecutioncontexttypedef) 
5. See [:material-code-braces: QueryExecutionStatusTypeDef](./type_defs.md#queryexecutionstatustypedef) 
6. See [:material-code-braces: QueryExecutionStatisticsTypeDef](./type_defs.md#queryexecutionstatisticstypedef) 
7. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
8. See [:material-code-braces: QueryResultsS3AccessGrantsConfigurationTypeDef](./type_defs.md#queryresultss3accessgrantsconfigurationtypedef) 
## StartQueryExecutionInputRequestTypeDef

```python
# StartQueryExecutionInputRequestTypeDef definition

class StartQueryExecutionInputRequestTypeDef(TypedDict):
    QueryString: str,
    ClientRequestToken: NotRequired[str],
    QueryExecutionContext: NotRequired[QueryExecutionContextTypeDef],  # (1)
    ResultConfiguration: NotRequired[ResultConfigurationTypeDef],  # (2)
    WorkGroup: NotRequired[str],
    ExecutionParameters: NotRequired[Sequence[str]],
    ResultReuseConfiguration: NotRequired[ResultReuseConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: QueryExecutionContextTypeDef](./type_defs.md#queryexecutioncontexttypedef) 
2. See [:material-code-braces: ResultConfigurationTypeDef](./type_defs.md#resultconfigurationtypedef) 
3. See [:material-code-braces: ResultReuseConfigurationTypeDef](./type_defs.md#resultreuseconfigurationtypedef) 
## GetQueryResultsOutputTypeDef

```python
# GetQueryResultsOutputTypeDef definition

class GetQueryResultsOutputTypeDef(TypedDict):
    UpdateCount: int,
    ResultSet: ResultSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResultSetTypeDef](./type_defs.md#resultsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkGroupInputRequestTypeDef

```python
# CreateWorkGroupInputRequestTypeDef definition

class CreateWorkGroupInputRequestTypeDef(TypedDict):
    Name: str,
    Configuration: NotRequired[WorkGroupConfigurationTypeDef],  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: WorkGroupConfigurationTypeDef](./type_defs.md#workgroupconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## WorkGroupTypeDef

```python
# WorkGroupTypeDef definition

class WorkGroupTypeDef(TypedDict):
    Name: str,
    State: NotRequired[WorkGroupStateType],  # (1)
    Configuration: NotRequired[WorkGroupConfigurationTypeDef],  # (2)
    Description: NotRequired[str],
    CreationTime: NotRequired[datetime],
    IdentityCenterApplicationArn: NotRequired[str],
```

1. See [:material-code-brackets: WorkGroupStateType](./literals.md#workgroupstatetype) 
2. See [:material-code-braces: WorkGroupConfigurationTypeDef](./type_defs.md#workgroupconfigurationtypedef) 
## UpdateWorkGroupInputRequestTypeDef

```python
# UpdateWorkGroupInputRequestTypeDef definition

class UpdateWorkGroupInputRequestTypeDef(TypedDict):
    WorkGroup: str,
    Description: NotRequired[str],
    ConfigurationUpdates: NotRequired[WorkGroupConfigurationUpdatesTypeDef],  # (1)
    State: NotRequired[WorkGroupStateType],  # (2)
```

1. See [:material-code-braces: WorkGroupConfigurationUpdatesTypeDef](./type_defs.md#workgroupconfigurationupdatestypedef) 
2. See [:material-code-brackets: WorkGroupStateType](./literals.md#workgroupstatetype) 
## GetQueryRuntimeStatisticsOutputTypeDef

```python
# GetQueryRuntimeStatisticsOutputTypeDef definition

class GetQueryRuntimeStatisticsOutputTypeDef(TypedDict):
    QueryRuntimeStatistics: QueryRuntimeStatisticsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueryRuntimeStatisticsTypeDef](./type_defs.md#queryruntimestatisticstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetQueryExecutionOutputTypeDef

```python
# BatchGetQueryExecutionOutputTypeDef definition

class BatchGetQueryExecutionOutputTypeDef(TypedDict):
    QueryExecutions: List[QueryExecutionTypeDef],  # (1)
    UnprocessedQueryExecutionIds: List[UnprocessedQueryExecutionIdTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: QueryExecutionTypeDef](./type_defs.md#queryexecutiontypedef) 
2. See [:material-code-braces: UnprocessedQueryExecutionIdTypeDef](./type_defs.md#unprocessedqueryexecutionidtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueryExecutionOutputTypeDef

```python
# GetQueryExecutionOutputTypeDef definition

class GetQueryExecutionOutputTypeDef(TypedDict):
    QueryExecution: QueryExecutionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueryExecutionTypeDef](./type_defs.md#queryexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkGroupOutputTypeDef

```python
# GetWorkGroupOutputTypeDef definition

class GetWorkGroupOutputTypeDef(TypedDict):
    WorkGroup: WorkGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkGroupTypeDef](./type_defs.md#workgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
