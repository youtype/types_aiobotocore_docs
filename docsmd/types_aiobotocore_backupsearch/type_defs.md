# Type definitions

> [Index](../README.md) > [BackupSearch](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [BackupSearch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupsearch.html#backupsearch)
    type annotations stubs module [types-aiobotocore-backupsearch](https://pypi.org/project/types-aiobotocore-backupsearch/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## BackupCreationTimeFilterUnionTypeDef

```python
# BackupCreationTimeFilterUnionTypeDef definition

BackupCreationTimeFilterUnionTypeDef = Union[
    BackupCreationTimeFilterTypeDef,  # (1)
    BackupCreationTimeFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BackupCreationTimeFilterTypeDef](./type_defs.md#backupcreationtimefiltertypedef) 
2. See [:material-code-braces: BackupCreationTimeFilterOutputTypeDef](./type_defs.md#backupcreationtimefilteroutputtypedef) 

## TimeConditionUnionTypeDef

```python
# TimeConditionUnionTypeDef definition

TimeConditionUnionTypeDef = Union[
    TimeConditionTypeDef,  # (1)
    TimeConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TimeConditionTypeDef](./type_defs.md#timeconditiontypedef) 
2. See [:material-code-braces: TimeConditionOutputTypeDef](./type_defs.md#timeconditionoutputtypedef) 

## S3ItemFilterUnionTypeDef

```python
# S3ItemFilterUnionTypeDef definition

S3ItemFilterUnionTypeDef = Union[
    S3ItemFilterTypeDef,  # (1)
    S3ItemFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3ItemFilterTypeDef](./type_defs.md#s3itemfiltertypedef) 
2. See [:material-code-braces: S3ItemFilterOutputTypeDef](./type_defs.md#s3itemfilteroutputtypedef) 

## EBSItemFilterUnionTypeDef

```python
# EBSItemFilterUnionTypeDef definition

EBSItemFilterUnionTypeDef = Union[
    EBSItemFilterTypeDef,  # (1)
    EBSItemFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EBSItemFilterTypeDef](./type_defs.md#ebsitemfiltertypedef) 
2. See [:material-code-braces: EBSItemFilterOutputTypeDef](./type_defs.md#ebsitemfilteroutputtypedef) 



## BackupCreationTimeFilterOutputTypeDef

```python
# BackupCreationTimeFilterOutputTypeDef definition

class BackupCreationTimeFilterOutputTypeDef(TypedDict):
    CreatedAfter: NotRequired[datetime],
    CreatedBefore: NotRequired[datetime],
```

## CurrentSearchProgressTypeDef

```python
# CurrentSearchProgressTypeDef definition

class CurrentSearchProgressTypeDef(TypedDict):
    RecoveryPointsScannedCount: NotRequired[int],
    ItemsScannedCount: NotRequired[int],
    ItemsMatchedCount: NotRequired[int],
```

## LongConditionTypeDef

```python
# LongConditionTypeDef definition

class LongConditionTypeDef(TypedDict):
    Value: int,
    Operator: NotRequired[LongConditionOperatorType],  # (1)
```

1. See [:material-code-brackets: LongConditionOperatorType](./literals.md#longconditionoperatortype) 
## StringConditionTypeDef

```python
# StringConditionTypeDef definition

class StringConditionTypeDef(TypedDict):
    Value: str,
    Operator: NotRequired[StringConditionOperatorType],  # (1)
```

1. See [:material-code-brackets: StringConditionOperatorType](./literals.md#stringconditionoperatortype) 
## TimeConditionOutputTypeDef

```python
# TimeConditionOutputTypeDef definition

class TimeConditionOutputTypeDef(TypedDict):
    Value: datetime,
    Operator: NotRequired[TimeConditionOperatorType],  # (1)
```

1. See [:material-code-brackets: TimeConditionOperatorType](./literals.md#timeconditionoperatortype) 
## EBSResultItemTypeDef

```python
# EBSResultItemTypeDef definition

class EBSResultItemTypeDef(TypedDict):
    BackupResourceArn: NotRequired[str],
    SourceResourceArn: NotRequired[str],
    BackupVaultName: NotRequired[str],
    FileSystemIdentifier: NotRequired[str],
    FilePath: NotRequired[str],
    FileSize: NotRequired[int],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

## ExportJobSummaryTypeDef

```python
# ExportJobSummaryTypeDef definition

class ExportJobSummaryTypeDef(TypedDict):
    ExportJobIdentifier: str,
    ExportJobArn: NotRequired[str],
    Status: NotRequired[ExportJobStatusType],  # (1)
    CreationTime: NotRequired[datetime],
    CompletionTime: NotRequired[datetime],
    StatusMessage: NotRequired[str],
    SearchJobArn: NotRequired[str],
```

1. See [:material-code-brackets: ExportJobStatusType](./literals.md#exportjobstatustype) 
## S3ExportSpecificationTypeDef

```python
# S3ExportSpecificationTypeDef definition

class S3ExportSpecificationTypeDef(TypedDict):
    DestinationBucket: str,
    DestinationPrefix: NotRequired[str],
```

## GetSearchJobInputRequestTypeDef

```python
# GetSearchJobInputRequestTypeDef definition

class GetSearchJobInputRequestTypeDef(TypedDict):
    SearchJobIdentifier: str,
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

## SearchScopeSummaryTypeDef

```python
# SearchScopeSummaryTypeDef definition

class SearchScopeSummaryTypeDef(TypedDict):
    TotalRecoveryPointsToScanCount: NotRequired[int],
    TotalItemsToScanCount: NotRequired[int],
```

## GetSearchResultExportJobInputRequestTypeDef

```python
# GetSearchResultExportJobInputRequestTypeDef definition

class GetSearchResultExportJobInputRequestTypeDef(TypedDict):
    ExportJobIdentifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListSearchJobBackupsInputRequestTypeDef

```python
# ListSearchJobBackupsInputRequestTypeDef definition

class ListSearchJobBackupsInputRequestTypeDef(TypedDict):
    SearchJobIdentifier: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SearchJobBackupsResultTypeDef

```python
# SearchJobBackupsResultTypeDef definition

class SearchJobBackupsResultTypeDef(TypedDict):
    Status: NotRequired[SearchJobStateType],  # (1)
    StatusMessage: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (2)
    BackupResourceArn: NotRequired[str],
    SourceResourceArn: NotRequired[str],
    IndexCreationTime: NotRequired[datetime],
    BackupCreationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: SearchJobStateType](./literals.md#searchjobstatetype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ListSearchJobResultsInputRequestTypeDef

```python
# ListSearchJobResultsInputRequestTypeDef definition

class ListSearchJobResultsInputRequestTypeDef(TypedDict):
    SearchJobIdentifier: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListSearchJobsInputRequestTypeDef

```python
# ListSearchJobsInputRequestTypeDef definition

class ListSearchJobsInputRequestTypeDef(TypedDict):
    ByStatus: NotRequired[SearchJobStateType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SearchJobStateType](./literals.md#searchjobstatetype) 
## ListSearchResultExportJobsInputRequestTypeDef

```python
# ListSearchResultExportJobsInputRequestTypeDef definition

class ListSearchResultExportJobsInputRequestTypeDef(TypedDict):
    Status: NotRequired[ExportJobStatusType],  # (1)
    SearchJobIdentifier: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ExportJobStatusType](./literals.md#exportjobstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## S3ResultItemTypeDef

```python
# S3ResultItemTypeDef definition

class S3ResultItemTypeDef(TypedDict):
    BackupResourceArn: NotRequired[str],
    SourceResourceArn: NotRequired[str],
    BackupVaultName: NotRequired[str],
    ObjectKey: NotRequired[str],
    ObjectSize: NotRequired[int],
    CreationTime: NotRequired[datetime],
    ETag: NotRequired[str],
    VersionId: NotRequired[str],
```

## StopSearchJobInputRequestTypeDef

```python
# StopSearchJobInputRequestTypeDef definition

class StopSearchJobInputRequestTypeDef(TypedDict):
    SearchJobIdentifier: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## SearchScopeOutputTypeDef

```python
# SearchScopeOutputTypeDef definition

class SearchScopeOutputTypeDef(TypedDict):
    BackupResourceTypes: List[ResourceTypeType],  # (1)
    BackupResourceCreationTime: NotRequired[BackupCreationTimeFilterOutputTypeDef],  # (2)
    SourceResourceArns: NotRequired[List[str]],
    BackupResourceArns: NotRequired[List[str]],
    BackupResourceTags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: BackupCreationTimeFilterOutputTypeDef](./type_defs.md#backupcreationtimefilteroutputtypedef) 
## BackupCreationTimeFilterTypeDef

```python
# BackupCreationTimeFilterTypeDef definition

class BackupCreationTimeFilterTypeDef(TypedDict):
    CreatedAfter: NotRequired[TimestampTypeDef],
    CreatedBefore: NotRequired[TimestampTypeDef],
```

## TimeConditionTypeDef

```python
# TimeConditionTypeDef definition

class TimeConditionTypeDef(TypedDict):
    Value: TimestampTypeDef,
    Operator: NotRequired[TimeConditionOperatorType],  # (1)
```

1. See [:material-code-brackets: TimeConditionOperatorType](./literals.md#timeconditionoperatortype) 
## EBSItemFilterOutputTypeDef

```python
# EBSItemFilterOutputTypeDef definition

class EBSItemFilterOutputTypeDef(TypedDict):
    FilePaths: NotRequired[List[StringConditionTypeDef]],  # (1)
    Sizes: NotRequired[List[LongConditionTypeDef]],  # (2)
    CreationTimes: NotRequired[List[TimeConditionOutputTypeDef]],  # (3)
    LastModificationTimes: NotRequired[List[TimeConditionOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-braces: LongConditionTypeDef](./type_defs.md#longconditiontypedef) 
3. See [:material-code-braces: TimeConditionOutputTypeDef](./type_defs.md#timeconditionoutputtypedef) 
4. See [:material-code-braces: TimeConditionOutputTypeDef](./type_defs.md#timeconditionoutputtypedef) 
## S3ItemFilterOutputTypeDef

```python
# S3ItemFilterOutputTypeDef definition

class S3ItemFilterOutputTypeDef(TypedDict):
    ObjectKeys: NotRequired[List[StringConditionTypeDef]],  # (1)
    Sizes: NotRequired[List[LongConditionTypeDef]],  # (2)
    CreationTimes: NotRequired[List[TimeConditionOutputTypeDef]],  # (3)
    VersionIds: NotRequired[List[StringConditionTypeDef]],  # (1)
    ETags: NotRequired[List[StringConditionTypeDef]],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-braces: LongConditionTypeDef](./type_defs.md#longconditiontypedef) 
3. See [:material-code-braces: TimeConditionOutputTypeDef](./type_defs.md#timeconditionoutputtypedef) 
4. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
5. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## ExportSpecificationTypeDef

```python
# ExportSpecificationTypeDef definition

class ExportSpecificationTypeDef(TypedDict):
    s3ExportSpecification: NotRequired[S3ExportSpecificationTypeDef],  # (1)
```

1. See [:material-code-braces: S3ExportSpecificationTypeDef](./type_defs.md#s3exportspecificationtypedef) 
## ListSearchResultExportJobsOutputTypeDef

```python
# ListSearchResultExportJobsOutputTypeDef definition

class ListSearchResultExportJobsOutputTypeDef(TypedDict):
    ExportJobs: List[ExportJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportJobSummaryTypeDef](./type_defs.md#exportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSearchJobOutputTypeDef

```python
# StartSearchJobOutputTypeDef definition

class StartSearchJobOutputTypeDef(TypedDict):
    SearchJobArn: str,
    CreationTime: datetime,
    SearchJobIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSearchResultExportJobOutputTypeDef

```python
# StartSearchResultExportJobOutputTypeDef definition

class StartSearchResultExportJobOutputTypeDef(TypedDict):
    ExportJobArn: str,
    ExportJobIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchJobSummaryTypeDef

```python
# SearchJobSummaryTypeDef definition

class SearchJobSummaryTypeDef(TypedDict):
    SearchJobIdentifier: NotRequired[str],
    SearchJobArn: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[SearchJobStateType],  # (1)
    CreationTime: NotRequired[datetime],
    CompletionTime: NotRequired[datetime],
    SearchScopeSummary: NotRequired[SearchScopeSummaryTypeDef],  # (2)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: SearchJobStateType](./literals.md#searchjobstatetype) 
2. See [:material-code-braces: SearchScopeSummaryTypeDef](./type_defs.md#searchscopesummarytypedef) 
## ListSearchJobBackupsInputPaginateTypeDef

```python
# ListSearchJobBackupsInputPaginateTypeDef definition

class ListSearchJobBackupsInputPaginateTypeDef(TypedDict):
    SearchJobIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSearchJobResultsInputPaginateTypeDef

```python
# ListSearchJobResultsInputPaginateTypeDef definition

class ListSearchJobResultsInputPaginateTypeDef(TypedDict):
    SearchJobIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSearchJobsInputPaginateTypeDef

```python
# ListSearchJobsInputPaginateTypeDef definition

class ListSearchJobsInputPaginateTypeDef(TypedDict):
    ByStatus: NotRequired[SearchJobStateType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SearchJobStateType](./literals.md#searchjobstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSearchResultExportJobsInputPaginateTypeDef

```python
# ListSearchResultExportJobsInputPaginateTypeDef definition

class ListSearchResultExportJobsInputPaginateTypeDef(TypedDict):
    Status: NotRequired[ExportJobStatusType],  # (1)
    SearchJobIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ExportJobStatusType](./literals.md#exportjobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSearchJobBackupsOutputTypeDef

```python
# ListSearchJobBackupsOutputTypeDef definition

class ListSearchJobBackupsOutputTypeDef(TypedDict):
    Results: List[SearchJobBackupsResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchJobBackupsResultTypeDef](./type_defs.md#searchjobbackupsresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResultItemTypeDef

```python
# ResultItemTypeDef definition

class ResultItemTypeDef(TypedDict):
    S3ResultItem: NotRequired[S3ResultItemTypeDef],  # (1)
    EBSResultItem: NotRequired[EBSResultItemTypeDef],  # (2)
```

1. See [:material-code-braces: S3ResultItemTypeDef](./type_defs.md#s3resultitemtypedef) 
2. See [:material-code-braces: EBSResultItemTypeDef](./type_defs.md#ebsresultitemtypedef) 
## S3ItemFilterTypeDef

```python
# S3ItemFilterTypeDef definition

class S3ItemFilterTypeDef(TypedDict):
    ObjectKeys: NotRequired[Sequence[StringConditionTypeDef]],  # (1)
    Sizes: NotRequired[Sequence[LongConditionTypeDef]],  # (2)
    CreationTimes: NotRequired[Sequence[TimeConditionTypeDef]],  # (3)
    VersionIds: NotRequired[Sequence[StringConditionTypeDef]],  # (1)
    ETags: NotRequired[Sequence[StringConditionTypeDef]],  # (1)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-braces: LongConditionTypeDef](./type_defs.md#longconditiontypedef) 
3. See [:material-code-braces: TimeConditionTypeDef](./type_defs.md#timeconditiontypedef) 
4. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
5. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
## ItemFiltersOutputTypeDef

```python
# ItemFiltersOutputTypeDef definition

class ItemFiltersOutputTypeDef(TypedDict):
    S3ItemFilters: NotRequired[List[S3ItemFilterOutputTypeDef]],  # (1)
    EBSItemFilters: NotRequired[List[EBSItemFilterOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: S3ItemFilterOutputTypeDef](./type_defs.md#s3itemfilteroutputtypedef) 
2. See [:material-code-braces: EBSItemFilterOutputTypeDef](./type_defs.md#ebsitemfilteroutputtypedef) 
## GetSearchResultExportJobOutputTypeDef

```python
# GetSearchResultExportJobOutputTypeDef definition

class GetSearchResultExportJobOutputTypeDef(TypedDict):
    ExportJobIdentifier: str,
    ExportJobArn: str,
    Status: ExportJobStatusType,  # (1)
    CreationTime: datetime,
    CompletionTime: datetime,
    StatusMessage: str,
    ExportSpecification: ExportSpecificationTypeDef,  # (2)
    SearchJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ExportJobStatusType](./literals.md#exportjobstatustype) 
2. See [:material-code-braces: ExportSpecificationTypeDef](./type_defs.md#exportspecificationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSearchResultExportJobInputRequestTypeDef

```python
# StartSearchResultExportJobInputRequestTypeDef definition

class StartSearchResultExportJobInputRequestTypeDef(TypedDict):
    SearchJobIdentifier: str,
    ExportSpecification: ExportSpecificationTypeDef,  # (1)
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: ExportSpecificationTypeDef](./type_defs.md#exportspecificationtypedef) 
## ListSearchJobsOutputTypeDef

```python
# ListSearchJobsOutputTypeDef definition

class ListSearchJobsOutputTypeDef(TypedDict):
    SearchJobs: List[SearchJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchJobSummaryTypeDef](./type_defs.md#searchjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSearchJobResultsOutputTypeDef

```python
# ListSearchJobResultsOutputTypeDef definition

class ListSearchJobResultsOutputTypeDef(TypedDict):
    Results: List[ResultItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResultItemTypeDef](./type_defs.md#resultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchScopeTypeDef

```python
# SearchScopeTypeDef definition

class SearchScopeTypeDef(TypedDict):
    BackupResourceTypes: Sequence[ResourceTypeType],  # (1)
    BackupResourceCreationTime: NotRequired[BackupCreationTimeFilterUnionTypeDef],  # (2)
    SourceResourceArns: NotRequired[Sequence[str]],
    BackupResourceArns: NotRequired[Sequence[str]],
    BackupResourceTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: BackupCreationTimeFilterTypeDef](./type_defs.md#backupcreationtimefiltertypedef) [:material-code-braces: BackupCreationTimeFilterOutputTypeDef](./type_defs.md#backupcreationtimefilteroutputtypedef) 
## EBSItemFilterTypeDef

```python
# EBSItemFilterTypeDef definition

class EBSItemFilterTypeDef(TypedDict):
    FilePaths: NotRequired[Sequence[StringConditionTypeDef]],  # (1)
    Sizes: NotRequired[Sequence[LongConditionTypeDef]],  # (2)
    CreationTimes: NotRequired[Sequence[TimeConditionUnionTypeDef]],  # (3)
    LastModificationTimes: NotRequired[Sequence[TimeConditionTypeDef]],  # (4)
```

1. See [:material-code-braces: StringConditionTypeDef](./type_defs.md#stringconditiontypedef) 
2. See [:material-code-braces: LongConditionTypeDef](./type_defs.md#longconditiontypedef) 
3. See [:material-code-braces: TimeConditionTypeDef](./type_defs.md#timeconditiontypedef) [:material-code-braces: TimeConditionOutputTypeDef](./type_defs.md#timeconditionoutputtypedef) 
4. See [:material-code-braces: TimeConditionTypeDef](./type_defs.md#timeconditiontypedef) 
## GetSearchJobOutputTypeDef

```python
# GetSearchJobOutputTypeDef definition

class GetSearchJobOutputTypeDef(TypedDict):
    Name: str,
    SearchScopeSummary: SearchScopeSummaryTypeDef,  # (1)
    CurrentSearchProgress: CurrentSearchProgressTypeDef,  # (2)
    StatusMessage: str,
    EncryptionKeyArn: str,
    CompletionTime: datetime,
    Status: SearchJobStateType,  # (3)
    SearchScope: SearchScopeOutputTypeDef,  # (4)
    ItemFilters: ItemFiltersOutputTypeDef,  # (5)
    CreationTime: datetime,
    SearchJobIdentifier: str,
    SearchJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: SearchScopeSummaryTypeDef](./type_defs.md#searchscopesummarytypedef) 
2. See [:material-code-braces: CurrentSearchProgressTypeDef](./type_defs.md#currentsearchprogresstypedef) 
3. See [:material-code-brackets: SearchJobStateType](./literals.md#searchjobstatetype) 
4. See [:material-code-braces: SearchScopeOutputTypeDef](./type_defs.md#searchscopeoutputtypedef) 
5. See [:material-code-braces: ItemFiltersOutputTypeDef](./type_defs.md#itemfiltersoutputtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ItemFiltersTypeDef

```python
# ItemFiltersTypeDef definition

class ItemFiltersTypeDef(TypedDict):
    S3ItemFilters: NotRequired[Sequence[S3ItemFilterUnionTypeDef]],  # (1)
    EBSItemFilters: NotRequired[Sequence[EBSItemFilterUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: S3ItemFilterTypeDef](./type_defs.md#s3itemfiltertypedef) [:material-code-braces: S3ItemFilterOutputTypeDef](./type_defs.md#s3itemfilteroutputtypedef) 
2. See [:material-code-braces: EBSItemFilterTypeDef](./type_defs.md#ebsitemfiltertypedef) [:material-code-braces: EBSItemFilterOutputTypeDef](./type_defs.md#ebsitemfilteroutputtypedef) 
## StartSearchJobInputRequestTypeDef

```python
# StartSearchJobInputRequestTypeDef definition

class StartSearchJobInputRequestTypeDef(TypedDict):
    SearchScope: SearchScopeTypeDef,  # (1)
    Tags: NotRequired[Mapping[str, str]],
    Name: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
    ClientToken: NotRequired[str],
    ItemFilters: NotRequired[ItemFiltersTypeDef],  # (2)
```

1. See [:material-code-braces: SearchScopeTypeDef](./type_defs.md#searchscopetypedef) 
2. See [:material-code-braces: ItemFiltersTypeDef](./type_defs.md#itemfilterstypedef) 
