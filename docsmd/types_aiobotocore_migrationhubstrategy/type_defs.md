# Type definitions

> [Index](../README.md) > [MigrationHubStrategyRecommendations](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MigrationHubStrategyRecommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#migrationhubstrategyrecommendations)
    type annotations stubs module [types-aiobotocore-migrationhubstrategy](https://pypi.org/project/types-aiobotocore-migrationhubstrategy/).

## AssessmentTargetUnionTypeDef

```python
# AssessmentTargetUnionTypeDef definition

AssessmentTargetUnionTypeDef = Union[
    AssessmentTargetTypeDef,  # (1)
    AssessmentTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AssessmentTargetTypeDef](./type_defs.md#assessmenttargettypedef) 
2. See [:material-code-braces: AssessmentTargetOutputTypeDef](./type_defs.md#assessmenttargetoutputtypedef) 

## AwsManagedResourcesUnionTypeDef

```python
# AwsManagedResourcesUnionTypeDef definition

AwsManagedResourcesUnionTypeDef = Union[
    AwsManagedResourcesTypeDef,  # (1)
    AwsManagedResourcesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AwsManagedResourcesTypeDef](./type_defs.md#awsmanagedresourcestypedef) 
2. See [:material-code-braces: AwsManagedResourcesOutputTypeDef](./type_defs.md#awsmanagedresourcesoutputtypedef) 

## HeterogeneousUnionTypeDef

```python
# HeterogeneousUnionTypeDef definition

HeterogeneousUnionTypeDef = Union[
    HeterogeneousTypeDef,  # (1)
    HeterogeneousOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HeterogeneousTypeDef](./type_defs.md#heterogeneoustypedef) 
2. See [:material-code-braces: HeterogeneousOutputTypeDef](./type_defs.md#heterogeneousoutputtypedef) 

## HomogeneousUnionTypeDef

```python
# HomogeneousUnionTypeDef definition

HomogeneousUnionTypeDef = Union[
    HomogeneousTypeDef,  # (1)
    HomogeneousOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HomogeneousTypeDef](./type_defs.md#homogeneoustypedef) 
2. See [:material-code-braces: HomogeneousOutputTypeDef](./type_defs.md#homogeneousoutputtypedef) 

## NoDatabaseMigrationPreferenceUnionTypeDef

```python
# NoDatabaseMigrationPreferenceUnionTypeDef definition

NoDatabaseMigrationPreferenceUnionTypeDef = Union[
    NoDatabaseMigrationPreferenceTypeDef,  # (1)
    NoDatabaseMigrationPreferenceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NoDatabaseMigrationPreferenceTypeDef](./type_defs.md#nodatabasemigrationpreferencetypedef) 
2. See [:material-code-braces: NoDatabaseMigrationPreferenceOutputTypeDef](./type_defs.md#nodatabasemigrationpreferenceoutputtypedef) 

## NoManagementPreferenceUnionTypeDef

```python
# NoManagementPreferenceUnionTypeDef definition

NoManagementPreferenceUnionTypeDef = Union[
    NoManagementPreferenceTypeDef,  # (1)
    NoManagementPreferenceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NoManagementPreferenceTypeDef](./type_defs.md#nomanagementpreferencetypedef) 
2. See [:material-code-braces: NoManagementPreferenceOutputTypeDef](./type_defs.md#nomanagementpreferenceoutputtypedef) 

## SelfManageResourcesUnionTypeDef

```python
# SelfManageResourcesUnionTypeDef definition

SelfManageResourcesUnionTypeDef = Union[
    SelfManageResourcesTypeDef,  # (1)
    SelfManageResourcesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SelfManageResourcesTypeDef](./type_defs.md#selfmanageresourcestypedef) 
2. See [:material-code-braces: SelfManageResourcesOutputTypeDef](./type_defs.md#selfmanageresourcesoutputtypedef) 

## DatabaseMigrationPreferenceUnionTypeDef

```python
# DatabaseMigrationPreferenceUnionTypeDef definition

DatabaseMigrationPreferenceUnionTypeDef = Union[
    DatabaseMigrationPreferenceTypeDef,  # (1)
    DatabaseMigrationPreferenceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DatabaseMigrationPreferenceTypeDef](./type_defs.md#databasemigrationpreferencetypedef) 
2. See [:material-code-braces: DatabaseMigrationPreferenceOutputTypeDef](./type_defs.md#databasemigrationpreferenceoutputtypedef) 

## ManagementPreferenceUnionTypeDef

```python
# ManagementPreferenceUnionTypeDef definition

ManagementPreferenceUnionTypeDef = Union[
    ManagementPreferenceTypeDef,  # (1)
    ManagementPreferenceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ManagementPreferenceTypeDef](./type_defs.md#managementpreferencetypedef) 
2. See [:material-code-braces: ManagementPreferenceOutputTypeDef](./type_defs.md#managementpreferenceoutputtypedef) 



## AnalysisStatusUnionTypeDef

```python
# AnalysisStatusUnionTypeDef definition

class AnalysisStatusUnionTypeDef(TypedDict):
    runtimeAnalysisStatus: NotRequired[RuntimeAnalysisStatusType],  # (1)
    srcCodeOrDbAnalysisStatus: NotRequired[SrcCodeOrDbAnalysisStatusType],  # (2)
```

1. See [:material-code-brackets: RuntimeAnalysisStatusType](./literals.md#runtimeanalysisstatustype) 
2. See [:material-code-brackets: SrcCodeOrDbAnalysisStatusType](./literals.md#srccodeordbanalysisstatustype) 
## AnalyzableServerSummaryTypeDef

```python
# AnalyzableServerSummaryTypeDef definition

class AnalyzableServerSummaryTypeDef(TypedDict):
    hostname: NotRequired[str],
    ipAddress: NotRequired[str],
    source: NotRequired[str],
    vmId: NotRequired[str],
```

## AnalyzerNameUnionTypeDef

```python
# AnalyzerNameUnionTypeDef definition

class AnalyzerNameUnionTypeDef(TypedDict):
    binaryAnalyzerName: NotRequired[BinaryAnalyzerNameType],  # (1)
    runTimeAnalyzerName: NotRequired[RunTimeAnalyzerNameType],  # (2)
    sourceCodeAnalyzerName: NotRequired[SourceCodeAnalyzerNameType],  # (3)
```

1. See [:material-code-brackets: BinaryAnalyzerNameType](./literals.md#binaryanalyzernametype) 
2. See [:material-code-brackets: RunTimeAnalyzerNameType](./literals.md#runtimeanalyzernametype) 
3. See [:material-code-brackets: SourceCodeAnalyzerNameType](./literals.md#sourcecodeanalyzernametype) 
## S3ObjectTypeDef

```python
# S3ObjectTypeDef definition

class S3ObjectTypeDef(TypedDict):
    s3Bucket: NotRequired[str],
    s3key: NotRequired[str],
```

## AntipatternSeveritySummaryTypeDef

```python
# AntipatternSeveritySummaryTypeDef definition

class AntipatternSeveritySummaryTypeDef(TypedDict):
    count: NotRequired[int],
    severity: NotRequired[SeverityType],  # (1)
```

1. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
## AppUnitErrorTypeDef

```python
# AppUnitErrorTypeDef definition

class AppUnitErrorTypeDef(TypedDict):
    appUnitErrorCategory: NotRequired[AppUnitErrorCategoryType],  # (1)
```

1. See [:material-code-brackets: AppUnitErrorCategoryType](./literals.md#appuniterrorcategorytype) 
## DatabaseConfigDetailTypeDef

```python
# DatabaseConfigDetailTypeDef definition

class DatabaseConfigDetailTypeDef(TypedDict):
    secretName: NotRequired[str],
```

## SourceCodeRepositoryTypeDef

```python
# SourceCodeRepositoryTypeDef definition

class SourceCodeRepositoryTypeDef(TypedDict):
    branch: NotRequired[str],
    projectName: NotRequired[str],
    repository: NotRequired[str],
    versionControlType: NotRequired[str],
```

## ApplicationComponentStatusSummaryTypeDef

```python
# ApplicationComponentStatusSummaryTypeDef definition

class ApplicationComponentStatusSummaryTypeDef(TypedDict):
    count: NotRequired[int],
    srcCodeOrDbAnalysisStatus: NotRequired[SrcCodeOrDbAnalysisStatusType],  # (1)
```

1. See [:material-code-brackets: SrcCodeOrDbAnalysisStatusType](./literals.md#srccodeordbanalysisstatustype) 
## ApplicationComponentSummaryTypeDef

```python
# ApplicationComponentSummaryTypeDef definition

class ApplicationComponentSummaryTypeDef(TypedDict):
    appType: NotRequired[AppTypeType],  # (1)
    count: NotRequired[int],
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
## ServerStatusSummaryTypeDef

```python
# ServerStatusSummaryTypeDef definition

class ServerStatusSummaryTypeDef(TypedDict):
    count: NotRequired[int],
    runTimeAssessmentStatus: NotRequired[RunTimeAssessmentStatusType],  # (1)
```

1. See [:material-code-brackets: RunTimeAssessmentStatusType](./literals.md#runtimeassessmentstatustype) 
## ServerSummaryTypeDef

```python
# ServerSummaryTypeDef definition

class ServerSummaryTypeDef(TypedDict):
    ServerOsType: NotRequired[ServerOsTypeType],  # (1)
    count: NotRequired[int],
```

1. See [:material-code-brackets: ServerOsTypeType](./literals.md#serverostypetype) 
## StrategySummaryTypeDef

```python
# StrategySummaryTypeDef definition

class StrategySummaryTypeDef(TypedDict):
    count: NotRequired[int],
    strategy: NotRequired[StrategyType],  # (1)
```

1. See [:material-code-brackets: StrategyType](./literals.md#strategytype) 
## AssessmentTargetOutputTypeDef

```python
# AssessmentTargetOutputTypeDef definition

class AssessmentTargetOutputTypeDef(TypedDict):
    condition: ConditionType,  # (1)
    name: str,
    values: List[str],
```

1. See [:material-code-brackets: ConditionType](./literals.md#conditiontype) 
## AssessmentTargetTypeDef

```python
# AssessmentTargetTypeDef definition

class AssessmentTargetTypeDef(TypedDict):
    condition: ConditionType,  # (1)
    name: str,
    values: Sequence[str],
```

1. See [:material-code-brackets: ConditionType](./literals.md#conditiontype) 
## AssociatedApplicationTypeDef

```python
# AssociatedApplicationTypeDef definition

class AssociatedApplicationTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## AwsManagedResourcesOutputTypeDef

```python
# AwsManagedResourcesOutputTypeDef definition

class AwsManagedResourcesOutputTypeDef(TypedDict):
    targetDestination: List[AwsManagedTargetDestinationType],  # (1)
```

1. See [:material-code-brackets: AwsManagedTargetDestinationType](./literals.md#awsmanagedtargetdestinationtype) 
## AwsManagedResourcesTypeDef

```python
# AwsManagedResourcesTypeDef definition

class AwsManagedResourcesTypeDef(TypedDict):
    targetDestination: Sequence[AwsManagedTargetDestinationType],  # (1)
```

1. See [:material-code-brackets: AwsManagedTargetDestinationType](./literals.md#awsmanagedtargetdestinationtype) 
## BusinessGoalsTypeDef

```python
# BusinessGoalsTypeDef definition

class BusinessGoalsTypeDef(TypedDict):
    licenseCostReduction: NotRequired[int],
    modernizeInfrastructureWithCloudNativeTechnologies: NotRequired[int],
    reduceOperationalOverheadWithManagedServices: NotRequired[int],
    speedOfMigration: NotRequired[int],
```

## IPAddressBasedRemoteInfoTypeDef

```python
# IPAddressBasedRemoteInfoTypeDef definition

class IPAddressBasedRemoteInfoTypeDef(TypedDict):
    authType: NotRequired[AuthTypeType],  # (1)
    ipAddressConfigurationTimeStamp: NotRequired[str],
    osType: NotRequired[OSTypeType],  # (2)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-brackets: OSTypeType](./literals.md#ostypetype) 
## PipelineInfoTypeDef

```python
# PipelineInfoTypeDef definition

class PipelineInfoTypeDef(TypedDict):
    pipelineConfigurationTimeStamp: NotRequired[str],
    pipelineType: NotRequired[PipelineTypeType],  # (1)
```

1. See [:material-code-brackets: PipelineTypeType](./literals.md#pipelinetypetype) 
## RemoteSourceCodeAnalysisServerInfoTypeDef

```python
# RemoteSourceCodeAnalysisServerInfoTypeDef definition

class RemoteSourceCodeAnalysisServerInfoTypeDef(TypedDict):
    remoteSourceCodeAnalysisServerConfigurationTimestamp: NotRequired[str],
```

## VcenterBasedRemoteInfoTypeDef

```python
# VcenterBasedRemoteInfoTypeDef definition

class VcenterBasedRemoteInfoTypeDef(TypedDict):
    osType: NotRequired[OSTypeType],  # (1)
    vcenterConfigurationTimeStamp: NotRequired[str],
```

1. See [:material-code-brackets: OSTypeType](./literals.md#ostypetype) 
## VersionControlInfoTypeDef

```python
# VersionControlInfoTypeDef definition

class VersionControlInfoTypeDef(TypedDict):
    versionControlConfigurationTimeStamp: NotRequired[str],
    versionControlType: NotRequired[VersionControlTypeType],  # (1)
```

1. See [:material-code-brackets: VersionControlTypeType](./literals.md#versioncontroltypetype) 
## DataCollectionDetailsTypeDef

```python
# DataCollectionDetailsTypeDef definition

class DataCollectionDetailsTypeDef(TypedDict):
    completionTime: NotRequired[datetime],
    failed: NotRequired[int],
    inProgress: NotRequired[int],
    servers: NotRequired[int],
    startTime: NotRequired[datetime],
    status: NotRequired[AssessmentStatusType],  # (1)
    statusMessage: NotRequired[str],
    success: NotRequired[int],
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
## HeterogeneousOutputTypeDef

```python
# HeterogeneousOutputTypeDef definition

class HeterogeneousOutputTypeDef(TypedDict):
    targetDatabaseEngine: List[HeterogeneousTargetDatabaseEngineType],  # (1)
```

1. See [:material-code-brackets: HeterogeneousTargetDatabaseEngineType](./literals.md#heterogeneoustargetdatabaseenginetype) 
## HomogeneousOutputTypeDef

```python
# HomogeneousOutputTypeDef definition

class HomogeneousOutputTypeDef(TypedDict):
    targetDatabaseEngine: NotRequired[List[HomogeneousTargetDatabaseEngineType]],  # (1)
```

1. See [:material-code-brackets: HomogeneousTargetDatabaseEngineType](./literals.md#homogeneoustargetdatabaseenginetype) 
## NoDatabaseMigrationPreferenceOutputTypeDef

```python
# NoDatabaseMigrationPreferenceOutputTypeDef definition

class NoDatabaseMigrationPreferenceOutputTypeDef(TypedDict):
    targetDatabaseEngine: List[TargetDatabaseEngineType],  # (1)
```

1. See [:material-code-brackets: TargetDatabaseEngineType](./literals.md#targetdatabaseenginetype) 
## GetApplicationComponentDetailsRequestRequestTypeDef

```python
# GetApplicationComponentDetailsRequestRequestTypeDef definition

class GetApplicationComponentDetailsRequestRequestTypeDef(TypedDict):
    applicationComponentId: str,
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

## GetApplicationComponentStrategiesRequestRequestTypeDef

```python
# GetApplicationComponentStrategiesRequestRequestTypeDef definition

class GetApplicationComponentStrategiesRequestRequestTypeDef(TypedDict):
    applicationComponentId: str,
```

## GetAssessmentRequestRequestTypeDef

```python
# GetAssessmentRequestRequestTypeDef definition

class GetAssessmentRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetImportFileTaskRequestRequestTypeDef

```python
# GetImportFileTaskRequestRequestTypeDef definition

class GetImportFileTaskRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetRecommendationReportDetailsRequestRequestTypeDef

```python
# GetRecommendationReportDetailsRequestRequestTypeDef definition

class GetRecommendationReportDetailsRequestRequestTypeDef(TypedDict):
    id: str,
```

## RecommendationReportDetailsTypeDef

```python
# RecommendationReportDetailsTypeDef definition

class RecommendationReportDetailsTypeDef(TypedDict):
    completionTime: NotRequired[datetime],
    s3Bucket: NotRequired[str],
    s3Keys: NotRequired[List[str]],
    startTime: NotRequired[datetime],
    status: NotRequired[RecommendationReportStatusType],  # (1)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: RecommendationReportStatusType](./literals.md#recommendationreportstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetServerDetailsRequestRequestTypeDef

```python
# GetServerDetailsRequestRequestTypeDef definition

class GetServerDetailsRequestRequestTypeDef(TypedDict):
    serverId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetServerStrategiesRequestRequestTypeDef

```python
# GetServerStrategiesRequestRequestTypeDef definition

class GetServerStrategiesRequestRequestTypeDef(TypedDict):
    serverId: str,
```

## GroupTypeDef

```python
# GroupTypeDef definition

class GroupTypeDef(TypedDict):
    name: NotRequired[GroupNameType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: GroupNameType](./literals.md#groupnametype) 
## HeterogeneousTypeDef

```python
# HeterogeneousTypeDef definition

class HeterogeneousTypeDef(TypedDict):
    targetDatabaseEngine: Sequence[HeterogeneousTargetDatabaseEngineType],  # (1)
```

1. See [:material-code-brackets: HeterogeneousTargetDatabaseEngineType](./literals.md#heterogeneoustargetdatabaseenginetype) 
## HomogeneousTypeDef

```python
# HomogeneousTypeDef definition

class HomogeneousTypeDef(TypedDict):
    targetDatabaseEngine: NotRequired[Sequence[HomogeneousTargetDatabaseEngineType]],  # (1)
```

1. See [:material-code-brackets: HomogeneousTargetDatabaseEngineType](./literals.md#homogeneoustargetdatabaseenginetype) 
## ImportFileTaskInformationTypeDef

```python
# ImportFileTaskInformationTypeDef definition

class ImportFileTaskInformationTypeDef(TypedDict):
    completionTime: NotRequired[datetime],
    id: NotRequired[str],
    importName: NotRequired[str],
    inputS3Bucket: NotRequired[str],
    inputS3Key: NotRequired[str],
    numberOfRecordsFailed: NotRequired[int],
    numberOfRecordsSuccess: NotRequired[int],
    startTime: NotRequired[datetime],
    status: NotRequired[ImportFileTaskStatusType],  # (1)
    statusReportS3Bucket: NotRequired[str],
    statusReportS3Key: NotRequired[str],
```

1. See [:material-code-brackets: ImportFileTaskStatusType](./literals.md#importfiletaskstatustype) 
## ListAnalyzableServersRequestRequestTypeDef

```python
# ListAnalyzableServersRequestRequestTypeDef definition

class ListAnalyzableServersRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sort: NotRequired[SortOrderType],  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListCollectorsRequestRequestTypeDef

```python
# ListCollectorsRequestRequestTypeDef definition

class ListCollectorsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListImportFileTaskRequestRequestTypeDef

```python
# ListImportFileTaskRequestRequestTypeDef definition

class ListImportFileTaskRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## NoManagementPreferenceOutputTypeDef

```python
# NoManagementPreferenceOutputTypeDef definition

class NoManagementPreferenceOutputTypeDef(TypedDict):
    targetDestination: List[NoPreferenceTargetDestinationType],  # (1)
```

1. See [:material-code-brackets: NoPreferenceTargetDestinationType](./literals.md#nopreferencetargetdestinationtype) 
## SelfManageResourcesOutputTypeDef

```python
# SelfManageResourcesOutputTypeDef definition

class SelfManageResourcesOutputTypeDef(TypedDict):
    targetDestination: List[SelfManageTargetDestinationType],  # (1)
```

1. See [:material-code-brackets: SelfManageTargetDestinationType](./literals.md#selfmanagetargetdestinationtype) 
## NetworkInfoTypeDef

```python
# NetworkInfoTypeDef definition

class NetworkInfoTypeDef(TypedDict):
    interfaceName: str,
    ipAddress: str,
    macAddress: str,
    netMask: str,
```

## NoDatabaseMigrationPreferenceTypeDef

```python
# NoDatabaseMigrationPreferenceTypeDef definition

class NoDatabaseMigrationPreferenceTypeDef(TypedDict):
    targetDatabaseEngine: Sequence[TargetDatabaseEngineType],  # (1)
```

1. See [:material-code-brackets: TargetDatabaseEngineType](./literals.md#targetdatabaseenginetype) 
## NoManagementPreferenceTypeDef

```python
# NoManagementPreferenceTypeDef definition

class NoManagementPreferenceTypeDef(TypedDict):
    targetDestination: Sequence[NoPreferenceTargetDestinationType],  # (1)
```

1. See [:material-code-brackets: NoPreferenceTargetDestinationType](./literals.md#nopreferencetargetdestinationtype) 
## OSInfoTypeDef

```python
# OSInfoTypeDef definition

class OSInfoTypeDef(TypedDict):
    type: NotRequired[OSTypeType],  # (1)
    version: NotRequired[str],
```

1. See [:material-code-brackets: OSTypeType](./literals.md#ostypetype) 
## TransformationToolTypeDef

```python
# TransformationToolTypeDef definition

class TransformationToolTypeDef(TypedDict):
    description: NotRequired[str],
    name: NotRequired[TransformationToolNameType],  # (1)
    tranformationToolInstallationLink: NotRequired[str],
```

1. See [:material-code-brackets: TransformationToolNameType](./literals.md#transformationtoolnametype) 
## SelfManageResourcesTypeDef

```python
# SelfManageResourcesTypeDef definition

class SelfManageResourcesTypeDef(TypedDict):
    targetDestination: Sequence[SelfManageTargetDestinationType],  # (1)
```

1. See [:material-code-brackets: SelfManageTargetDestinationType](./literals.md#selfmanagetargetdestinationtype) 
## ServerErrorTypeDef

```python
# ServerErrorTypeDef definition

class ServerErrorTypeDef(TypedDict):
    serverErrorCategory: NotRequired[ServerErrorCategoryType],  # (1)
```

1. See [:material-code-brackets: ServerErrorCategoryType](./literals.md#servererrorcategorytype) 
## SourceCodeTypeDef

```python
# SourceCodeTypeDef definition

class SourceCodeTypeDef(TypedDict):
    location: NotRequired[str],
    projectName: NotRequired[str],
    sourceVersion: NotRequired[str],
    versionControl: NotRequired[VersionControlType],  # (1)
```

1. See [:material-code-brackets: VersionControlType](./literals.md#versioncontroltype) 
## StopAssessmentRequestRequestTypeDef

```python
# StopAssessmentRequestRequestTypeDef definition

class StopAssessmentRequestRequestTypeDef(TypedDict):
    assessmentId: str,
```

## StrategyOptionTypeDef

```python
# StrategyOptionTypeDef definition

class StrategyOptionTypeDef(TypedDict):
    isPreferred: NotRequired[bool],
    strategy: NotRequired[StrategyType],  # (1)
    targetDestination: NotRequired[TargetDestinationType],  # (2)
    toolName: NotRequired[TransformationToolNameType],  # (3)
```

1. See [:material-code-brackets: StrategyType](./literals.md#strategytype) 
2. See [:material-code-brackets: TargetDestinationType](./literals.md#targetdestinationtype) 
3. See [:material-code-brackets: TransformationToolNameType](./literals.md#transformationtoolnametype) 
## AntipatternReportResultTypeDef

```python
# AntipatternReportResultTypeDef definition

class AntipatternReportResultTypeDef(TypedDict):
    analyzerName: NotRequired[AnalyzerNameUnionTypeDef],  # (1)
    antiPatternReportS3Object: NotRequired[S3ObjectTypeDef],  # (2)
    antipatternReportStatus: NotRequired[AntipatternReportStatusType],  # (3)
    antipatternReportStatusMessage: NotRequired[str],
```

1. See [:material-code-braces: AnalyzerNameUnionTypeDef](./type_defs.md#analyzernameuniontypedef) 
2. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
3. See [:material-code-brackets: AntipatternReportStatusType](./literals.md#antipatternreportstatustype) 
## AssessmentSummaryTypeDef

```python
# AssessmentSummaryTypeDef definition

class AssessmentSummaryTypeDef(TypedDict):
    antipatternReportS3Object: NotRequired[S3ObjectTypeDef],  # (1)
    antipatternReportStatus: NotRequired[AntipatternReportStatusType],  # (2)
    antipatternReportStatusMessage: NotRequired[str],
    lastAnalyzedTimestamp: NotRequired[datetime],
    listAntipatternSeveritySummary: NotRequired[List[AntipatternSeveritySummaryTypeDef]],  # (3)
    listApplicationComponentStatusSummary: NotRequired[List[ApplicationComponentStatusSummaryTypeDef]],  # (4)
    listApplicationComponentStrategySummary: NotRequired[List[StrategySummaryTypeDef]],  # (5)
    listApplicationComponentSummary: NotRequired[List[ApplicationComponentSummaryTypeDef]],  # (6)
    listServerStatusSummary: NotRequired[List[ServerStatusSummaryTypeDef]],  # (7)
    listServerStrategySummary: NotRequired[List[StrategySummaryTypeDef]],  # (5)
    listServerSummary: NotRequired[List[ServerSummaryTypeDef]],  # (9)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
2. See [:material-code-brackets: AntipatternReportStatusType](./literals.md#antipatternreportstatustype) 
3. See [:material-code-braces: AntipatternSeveritySummaryTypeDef](./type_defs.md#antipatternseveritysummarytypedef) 
4. See [:material-code-braces: ApplicationComponentStatusSummaryTypeDef](./type_defs.md#applicationcomponentstatussummarytypedef) 
5. See [:material-code-braces: StrategySummaryTypeDef](./type_defs.md#strategysummarytypedef) 
6. See [:material-code-braces: ApplicationComponentSummaryTypeDef](./type_defs.md#applicationcomponentsummarytypedef) 
7. See [:material-code-braces: ServerStatusSummaryTypeDef](./type_defs.md#serverstatussummarytypedef) 
8. See [:material-code-braces: StrategySummaryTypeDef](./type_defs.md#strategysummarytypedef) 
9. See [:material-code-braces: ServerSummaryTypeDef](./type_defs.md#serversummarytypedef) 
## PrioritizeBusinessGoalsTypeDef

```python
# PrioritizeBusinessGoalsTypeDef definition

class PrioritizeBusinessGoalsTypeDef(TypedDict):
    businessGoals: NotRequired[BusinessGoalsTypeDef],  # (1)
```

1. See [:material-code-braces: BusinessGoalsTypeDef](./type_defs.md#businessgoalstypedef) 
## ConfigurationSummaryTypeDef

```python
# ConfigurationSummaryTypeDef definition

class ConfigurationSummaryTypeDef(TypedDict):
    ipAddressBasedRemoteInfoList: NotRequired[List[IPAddressBasedRemoteInfoTypeDef]],  # (1)
    pipelineInfoList: NotRequired[List[PipelineInfoTypeDef]],  # (2)
    remoteSourceCodeAnalysisServerInfo: NotRequired[RemoteSourceCodeAnalysisServerInfoTypeDef],  # (3)
    vcenterBasedRemoteInfoList: NotRequired[List[VcenterBasedRemoteInfoTypeDef]],  # (4)
    versionControlInfoList: NotRequired[List[VersionControlInfoTypeDef]],  # (5)
```

1. See [:material-code-braces: IPAddressBasedRemoteInfoTypeDef](./type_defs.md#ipaddressbasedremoteinfotypedef) 
2. See [:material-code-braces: PipelineInfoTypeDef](./type_defs.md#pipelineinfotypedef) 
3. See [:material-code-braces: RemoteSourceCodeAnalysisServerInfoTypeDef](./type_defs.md#remotesourcecodeanalysisserverinfotypedef) 
4. See [:material-code-braces: VcenterBasedRemoteInfoTypeDef](./type_defs.md#vcenterbasedremoteinfotypedef) 
5. See [:material-code-braces: VersionControlInfoTypeDef](./type_defs.md#versioncontrolinfotypedef) 
## DatabaseMigrationPreferenceOutputTypeDef

```python
# DatabaseMigrationPreferenceOutputTypeDef definition

class DatabaseMigrationPreferenceOutputTypeDef(TypedDict):
    heterogeneous: NotRequired[HeterogeneousOutputTypeDef],  # (1)
    homogeneous: NotRequired[HomogeneousOutputTypeDef],  # (2)
    noPreference: NotRequired[NoDatabaseMigrationPreferenceOutputTypeDef],  # (3)
```

1. See [:material-code-braces: HeterogeneousOutputTypeDef](./type_defs.md#heterogeneousoutputtypedef) 
2. See [:material-code-braces: HomogeneousOutputTypeDef](./type_defs.md#homogeneousoutputtypedef) 
3. See [:material-code-braces: NoDatabaseMigrationPreferenceOutputTypeDef](./type_defs.md#nodatabasemigrationpreferenceoutputtypedef) 
## GetAssessmentResponseTypeDef

```python
# GetAssessmentResponseTypeDef definition

class GetAssessmentResponseTypeDef(TypedDict):
    assessmentTargets: List[AssessmentTargetOutputTypeDef],  # (1)
    dataCollectionDetails: DataCollectionDetailsTypeDef,  # (2)
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssessmentTargetOutputTypeDef](./type_defs.md#assessmenttargetoutputtypedef) 
2. See [:material-code-braces: DataCollectionDetailsTypeDef](./type_defs.md#datacollectiondetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImportFileTaskResponseTypeDef

```python
# GetImportFileTaskResponseTypeDef definition

class GetImportFileTaskResponseTypeDef(TypedDict):
    completionTime: datetime,
    id: str,
    importName: str,
    inputS3Bucket: str,
    inputS3Key: str,
    numberOfRecordsFailed: int,
    numberOfRecordsSuccess: int,
    startTime: datetime,
    status: ImportFileTaskStatusType,  # (1)
    statusReportS3Bucket: str,
    statusReportS3Key: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ImportFileTaskStatusType](./literals.md#importfiletaskstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLatestAssessmentIdResponseTypeDef

```python
# GetLatestAssessmentIdResponseTypeDef definition

class GetLatestAssessmentIdResponseTypeDef(TypedDict):
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAnalyzableServersResponseTypeDef

```python
# ListAnalyzableServersResponseTypeDef definition

class ListAnalyzableServersResponseTypeDef(TypedDict):
    analyzableServers: List[AnalyzableServerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnalyzableServerSummaryTypeDef](./type_defs.md#analyzableserversummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAssessmentResponseTypeDef

```python
# StartAssessmentResponseTypeDef definition

class StartAssessmentResponseTypeDef(TypedDict):
    assessmentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImportFileTaskResponseTypeDef

```python
# StartImportFileTaskResponseTypeDef definition

class StartImportFileTaskResponseTypeDef(TypedDict):
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartRecommendationReportGenerationResponseTypeDef

```python
# StartRecommendationReportGenerationResponseTypeDef definition

class StartRecommendationReportGenerationResponseTypeDef(TypedDict):
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecommendationReportDetailsResponseTypeDef

```python
# GetRecommendationReportDetailsResponseTypeDef definition

class GetRecommendationReportDetailsResponseTypeDef(TypedDict):
    id: str,
    recommendationReportDetails: RecommendationReportDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendationReportDetailsTypeDef](./type_defs.md#recommendationreportdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServerDetailsRequestPaginateTypeDef

```python
# GetServerDetailsRequestPaginateTypeDef definition

class GetServerDetailsRequestPaginateTypeDef(TypedDict):
    serverId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAnalyzableServersRequestPaginateTypeDef

```python
# ListAnalyzableServersRequestPaginateTypeDef definition

class ListAnalyzableServersRequestPaginateTypeDef(TypedDict):
    sort: NotRequired[SortOrderType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollectorsRequestPaginateTypeDef

```python
# ListCollectorsRequestPaginateTypeDef definition

class ListCollectorsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImportFileTaskRequestPaginateTypeDef

```python
# ListImportFileTaskRequestPaginateTypeDef definition

class ListImportFileTaskRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationComponentsRequestPaginateTypeDef

```python
# ListApplicationComponentsRequestPaginateTypeDef definition

class ListApplicationComponentsRequestPaginateTypeDef(TypedDict):
    applicationComponentCriteria: NotRequired[ApplicationComponentCriteriaType],  # (1)
    filterValue: NotRequired[str],
    groupIdFilter: NotRequired[Sequence[GroupTypeDef]],  # (2)
    sort: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ApplicationComponentCriteriaType](./literals.md#applicationcomponentcriteriatype) 
2. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationComponentsRequestRequestTypeDef

```python
# ListApplicationComponentsRequestRequestTypeDef definition

class ListApplicationComponentsRequestRequestTypeDef(TypedDict):
    applicationComponentCriteria: NotRequired[ApplicationComponentCriteriaType],  # (1)
    filterValue: NotRequired[str],
    groupIdFilter: NotRequired[Sequence[GroupTypeDef]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sort: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: ApplicationComponentCriteriaType](./literals.md#applicationcomponentcriteriatype) 
2. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListServersRequestPaginateTypeDef

```python
# ListServersRequestPaginateTypeDef definition

class ListServersRequestPaginateTypeDef(TypedDict):
    filterValue: NotRequired[str],
    groupIdFilter: NotRequired[Sequence[GroupTypeDef]],  # (1)
    serverCriteria: NotRequired[ServerCriteriaType],  # (2)
    sort: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-brackets: ServerCriteriaType](./literals.md#servercriteriatype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServersRequestRequestTypeDef

```python
# ListServersRequestRequestTypeDef definition

class ListServersRequestRequestTypeDef(TypedDict):
    filterValue: NotRequired[str],
    groupIdFilter: NotRequired[Sequence[GroupTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    serverCriteria: NotRequired[ServerCriteriaType],  # (2)
    sort: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-brackets: ServerCriteriaType](./literals.md#servercriteriatype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## StartImportFileTaskRequestRequestTypeDef

```python
# StartImportFileTaskRequestRequestTypeDef definition

class StartImportFileTaskRequestRequestTypeDef(TypedDict):
    S3Bucket: str,
    name: str,
    s3key: str,
    dataSourceType: NotRequired[DataSourceTypeType],  # (1)
    groupId: NotRequired[Sequence[GroupTypeDef]],  # (2)
    s3bucketForReportData: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
## StartRecommendationReportGenerationRequestRequestTypeDef

```python
# StartRecommendationReportGenerationRequestRequestTypeDef definition

class StartRecommendationReportGenerationRequestRequestTypeDef(TypedDict):
    groupIdFilter: NotRequired[Sequence[GroupTypeDef]],  # (1)
    outputFormat: NotRequired[OutputFormatType],  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
## ListImportFileTaskResponseTypeDef

```python
# ListImportFileTaskResponseTypeDef definition

class ListImportFileTaskResponseTypeDef(TypedDict):
    taskInfos: List[ImportFileTaskInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportFileTaskInformationTypeDef](./type_defs.md#importfiletaskinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ManagementPreferenceOutputTypeDef

```python
# ManagementPreferenceOutputTypeDef definition

class ManagementPreferenceOutputTypeDef(TypedDict):
    awsManagedResources: NotRequired[AwsManagedResourcesOutputTypeDef],  # (1)
    noPreference: NotRequired[NoManagementPreferenceOutputTypeDef],  # (2)
    selfManageResources: NotRequired[SelfManageResourcesOutputTypeDef],  # (3)
```

1. See [:material-code-braces: AwsManagedResourcesOutputTypeDef](./type_defs.md#awsmanagedresourcesoutputtypedef) 
2. See [:material-code-braces: NoManagementPreferenceOutputTypeDef](./type_defs.md#nomanagementpreferenceoutputtypedef) 
3. See [:material-code-braces: SelfManageResourcesOutputTypeDef](./type_defs.md#selfmanageresourcesoutputtypedef) 
## SystemInfoTypeDef

```python
# SystemInfoTypeDef definition

class SystemInfoTypeDef(TypedDict):
    cpuArchitecture: NotRequired[str],
    fileSystemType: NotRequired[str],
    networkInfoList: NotRequired[List[NetworkInfoTypeDef]],  # (1)
    osInfo: NotRequired[OSInfoTypeDef],  # (2)
```

1. See [:material-code-braces: NetworkInfoTypeDef](./type_defs.md#networkinfotypedef) 
2. See [:material-code-braces: OSInfoTypeDef](./type_defs.md#osinfotypedef) 
## RecommendationSetTypeDef

```python
# RecommendationSetTypeDef definition

class RecommendationSetTypeDef(TypedDict):
    strategy: NotRequired[StrategyType],  # (1)
    targetDestination: NotRequired[TargetDestinationType],  # (2)
    transformationTool: NotRequired[TransformationToolTypeDef],  # (3)
```

1. See [:material-code-brackets: StrategyType](./literals.md#strategytype) 
2. See [:material-code-brackets: TargetDestinationType](./literals.md#targetdestinationtype) 
3. See [:material-code-braces: TransformationToolTypeDef](./type_defs.md#transformationtooltypedef) 
## UpdateApplicationComponentConfigRequestRequestTypeDef

```python
# UpdateApplicationComponentConfigRequestRequestTypeDef definition

class UpdateApplicationComponentConfigRequestRequestTypeDef(TypedDict):
    applicationComponentId: str,
    appType: NotRequired[AppTypeType],  # (1)
    configureOnly: NotRequired[bool],
    inclusionStatus: NotRequired[InclusionStatusType],  # (2)
    secretsManagerKey: NotRequired[str],
    sourceCodeList: NotRequired[Sequence[SourceCodeTypeDef]],  # (3)
    strategyOption: NotRequired[StrategyOptionTypeDef],  # (4)
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
2. See [:material-code-brackets: InclusionStatusType](./literals.md#inclusionstatustype) 
3. See [:material-code-braces: SourceCodeTypeDef](./type_defs.md#sourcecodetypedef) 
4. See [:material-code-braces: StrategyOptionTypeDef](./type_defs.md#strategyoptiontypedef) 
## UpdateServerConfigRequestRequestTypeDef

```python
# UpdateServerConfigRequestRequestTypeDef definition

class UpdateServerConfigRequestRequestTypeDef(TypedDict):
    serverId: str,
    strategyOption: NotRequired[StrategyOptionTypeDef],  # (1)
```

1. See [:material-code-braces: StrategyOptionTypeDef](./type_defs.md#strategyoptiontypedef) 
## ResultTypeDef

```python
# ResultTypeDef definition

class ResultTypeDef(TypedDict):
    analysisStatus: NotRequired[AnalysisStatusUnionTypeDef],  # (1)
    analysisType: NotRequired[AnalysisTypeType],  # (2)
    antipatternReportResultList: NotRequired[List[AntipatternReportResultTypeDef]],  # (3)
    statusMessage: NotRequired[str],
```

1. See [:material-code-braces: AnalysisStatusUnionTypeDef](./type_defs.md#analysisstatusuniontypedef) 
2. See [:material-code-brackets: AnalysisTypeType](./literals.md#analysistypetype) 
3. See [:material-code-braces: AntipatternReportResultTypeDef](./type_defs.md#antipatternreportresulttypedef) 
## GetPortfolioSummaryResponseTypeDef

```python
# GetPortfolioSummaryResponseTypeDef definition

class GetPortfolioSummaryResponseTypeDef(TypedDict):
    assessmentSummary: AssessmentSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentSummaryTypeDef](./type_defs.md#assessmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAssessmentRequestRequestTypeDef

```python
# StartAssessmentRequestRequestTypeDef definition

class StartAssessmentRequestRequestTypeDef(TypedDict):
    assessmentDataSourceType: NotRequired[AssessmentDataSourceTypeType],  # (1)
    assessmentTargets: NotRequired[Sequence[AssessmentTargetUnionTypeDef]],  # (2)
    s3bucketForAnalysisData: NotRequired[str],
    s3bucketForReportData: NotRequired[str],
```

1. See [:material-code-brackets: AssessmentDataSourceTypeType](./literals.md#assessmentdatasourcetypetype) 
2. See [:material-code-braces: AssessmentTargetTypeDef](./type_defs.md#assessmenttargettypedef) [:material-code-braces: AssessmentTargetOutputTypeDef](./type_defs.md#assessmenttargetoutputtypedef) 
## CollectorTypeDef

```python
# CollectorTypeDef definition

class CollectorTypeDef(TypedDict):
    collectorHealth: NotRequired[CollectorHealthType],  # (1)
    collectorId: NotRequired[str],
    collectorVersion: NotRequired[str],
    configurationSummary: NotRequired[ConfigurationSummaryTypeDef],  # (2)
    hostName: NotRequired[str],
    ipAddress: NotRequired[str],
    lastActivityTimeStamp: NotRequired[str],
    registeredTimeStamp: NotRequired[str],
```

1. See [:material-code-brackets: CollectorHealthType](./literals.md#collectorhealthtype) 
2. See [:material-code-braces: ConfigurationSummaryTypeDef](./type_defs.md#configurationsummarytypedef) 
## DatabasePreferencesOutputTypeDef

```python
# DatabasePreferencesOutputTypeDef definition

class DatabasePreferencesOutputTypeDef(TypedDict):
    databaseManagementPreference: NotRequired[DatabaseManagementPreferenceType],  # (1)
    databaseMigrationPreference: NotRequired[DatabaseMigrationPreferenceOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: DatabaseManagementPreferenceType](./literals.md#databasemanagementpreferencetype) 
2. See [:material-code-braces: DatabaseMigrationPreferenceOutputTypeDef](./type_defs.md#databasemigrationpreferenceoutputtypedef) 
## ApplicationPreferencesOutputTypeDef

```python
# ApplicationPreferencesOutputTypeDef definition

class ApplicationPreferencesOutputTypeDef(TypedDict):
    managementPreference: NotRequired[ManagementPreferenceOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ManagementPreferenceOutputTypeDef](./type_defs.md#managementpreferenceoutputtypedef) 
## DatabaseMigrationPreferenceTypeDef

```python
# DatabaseMigrationPreferenceTypeDef definition

class DatabaseMigrationPreferenceTypeDef(TypedDict):
    heterogeneous: NotRequired[HeterogeneousUnionTypeDef],  # (1)
    homogeneous: NotRequired[HomogeneousUnionTypeDef],  # (2)
    noPreference: NotRequired[NoDatabaseMigrationPreferenceUnionTypeDef],  # (3)
```

1. See [:material-code-braces: HeterogeneousTypeDef](./type_defs.md#heterogeneoustypedef) [:material-code-braces: HeterogeneousOutputTypeDef](./type_defs.md#heterogeneousoutputtypedef) 
2. See [:material-code-braces: HomogeneousTypeDef](./type_defs.md#homogeneoustypedef) [:material-code-braces: HomogeneousOutputTypeDef](./type_defs.md#homogeneousoutputtypedef) 
3. See [:material-code-braces: NoDatabaseMigrationPreferenceTypeDef](./type_defs.md#nodatabasemigrationpreferencetypedef) [:material-code-braces: NoDatabaseMigrationPreferenceOutputTypeDef](./type_defs.md#nodatabasemigrationpreferenceoutputtypedef) 
## ApplicationComponentStrategyTypeDef

```python
# ApplicationComponentStrategyTypeDef definition

class ApplicationComponentStrategyTypeDef(TypedDict):
    isPreferred: NotRequired[bool],
    recommendation: NotRequired[RecommendationSetTypeDef],  # (1)
    status: NotRequired[StrategyRecommendationType],  # (2)
```

1. See [:material-code-braces: RecommendationSetTypeDef](./type_defs.md#recommendationsettypedef) 
2. See [:material-code-brackets: StrategyRecommendationType](./literals.md#strategyrecommendationtype) 
## ServerDetailTypeDef

```python
# ServerDetailTypeDef definition

class ServerDetailTypeDef(TypedDict):
    antipatternReportS3Object: NotRequired[S3ObjectTypeDef],  # (1)
    antipatternReportStatus: NotRequired[AntipatternReportStatusType],  # (2)
    antipatternReportStatusMessage: NotRequired[str],
    applicationComponentStrategySummary: NotRequired[List[StrategySummaryTypeDef]],  # (3)
    dataCollectionStatus: NotRequired[RunTimeAssessmentStatusType],  # (4)
    id: NotRequired[str],
    lastAnalyzedTimestamp: NotRequired[datetime],
    listAntipatternSeveritySummary: NotRequired[List[AntipatternSeveritySummaryTypeDef]],  # (5)
    name: NotRequired[str],
    recommendationSet: NotRequired[RecommendationSetTypeDef],  # (6)
    serverError: NotRequired[ServerErrorTypeDef],  # (7)
    serverType: NotRequired[str],
    statusMessage: NotRequired[str],
    systemInfo: NotRequired[SystemInfoTypeDef],  # (8)
```

1. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
2. See [:material-code-brackets: AntipatternReportStatusType](./literals.md#antipatternreportstatustype) 
3. See [:material-code-braces: StrategySummaryTypeDef](./type_defs.md#strategysummarytypedef) 
4. See [:material-code-brackets: RunTimeAssessmentStatusType](./literals.md#runtimeassessmentstatustype) 
5. See [:material-code-braces: AntipatternSeveritySummaryTypeDef](./type_defs.md#antipatternseveritysummarytypedef) 
6. See [:material-code-braces: RecommendationSetTypeDef](./type_defs.md#recommendationsettypedef) 
7. See [:material-code-braces: ServerErrorTypeDef](./type_defs.md#servererrortypedef) 
8. See [:material-code-braces: SystemInfoTypeDef](./type_defs.md#systeminfotypedef) 
## ServerStrategyTypeDef

```python
# ServerStrategyTypeDef definition

class ServerStrategyTypeDef(TypedDict):
    isPreferred: NotRequired[bool],
    numberOfApplicationComponents: NotRequired[int],
    recommendation: NotRequired[RecommendationSetTypeDef],  # (1)
    status: NotRequired[StrategyRecommendationType],  # (2)
```

1. See [:material-code-braces: RecommendationSetTypeDef](./type_defs.md#recommendationsettypedef) 
2. See [:material-code-brackets: StrategyRecommendationType](./literals.md#strategyrecommendationtype) 
## ManagementPreferenceTypeDef

```python
# ManagementPreferenceTypeDef definition

class ManagementPreferenceTypeDef(TypedDict):
    awsManagedResources: NotRequired[AwsManagedResourcesUnionTypeDef],  # (1)
    noPreference: NotRequired[NoManagementPreferenceUnionTypeDef],  # (2)
    selfManageResources: NotRequired[SelfManageResourcesUnionTypeDef],  # (3)
```

1. See [:material-code-braces: AwsManagedResourcesTypeDef](./type_defs.md#awsmanagedresourcestypedef) [:material-code-braces: AwsManagedResourcesOutputTypeDef](./type_defs.md#awsmanagedresourcesoutputtypedef) 
2. See [:material-code-braces: NoManagementPreferenceTypeDef](./type_defs.md#nomanagementpreferencetypedef) [:material-code-braces: NoManagementPreferenceOutputTypeDef](./type_defs.md#nomanagementpreferenceoutputtypedef) 
3. See [:material-code-braces: SelfManageResourcesTypeDef](./type_defs.md#selfmanageresourcestypedef) [:material-code-braces: SelfManageResourcesOutputTypeDef](./type_defs.md#selfmanageresourcesoutputtypedef) 
## ApplicationComponentDetailTypeDef

```python
# ApplicationComponentDetailTypeDef definition

class ApplicationComponentDetailTypeDef(TypedDict):
    analysisStatus: NotRequired[SrcCodeOrDbAnalysisStatusType],  # (1)
    antipatternReportS3Object: NotRequired[S3ObjectTypeDef],  # (2)
    antipatternReportStatus: NotRequired[AntipatternReportStatusType],  # (3)
    antipatternReportStatusMessage: NotRequired[str],
    appType: NotRequired[AppTypeType],  # (4)
    appUnitError: NotRequired[AppUnitErrorTypeDef],  # (5)
    associatedServerId: NotRequired[str],
    databaseConfigDetail: NotRequired[DatabaseConfigDetailTypeDef],  # (6)
    id: NotRequired[str],
    inclusionStatus: NotRequired[InclusionStatusType],  # (7)
    lastAnalyzedTimestamp: NotRequired[datetime],
    listAntipatternSeveritySummary: NotRequired[List[AntipatternSeveritySummaryTypeDef]],  # (8)
    moreServerAssociationExists: NotRequired[bool],
    name: NotRequired[str],
    osDriver: NotRequired[str],
    osVersion: NotRequired[str],
    recommendationSet: NotRequired[RecommendationSetTypeDef],  # (9)
    resourceSubType: NotRequired[ResourceSubTypeType],  # (10)
    resultList: NotRequired[List[ResultTypeDef]],  # (11)
    runtimeStatus: NotRequired[RuntimeAnalysisStatusType],  # (12)
    runtimeStatusMessage: NotRequired[str],
    sourceCodeRepositories: NotRequired[List[SourceCodeRepositoryTypeDef]],  # (13)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: SrcCodeOrDbAnalysisStatusType](./literals.md#srccodeordbanalysisstatustype) 
2. See [:material-code-braces: S3ObjectTypeDef](./type_defs.md#s3objecttypedef) 
3. See [:material-code-brackets: AntipatternReportStatusType](./literals.md#antipatternreportstatustype) 
4. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
5. See [:material-code-braces: AppUnitErrorTypeDef](./type_defs.md#appuniterrortypedef) 
6. See [:material-code-braces: DatabaseConfigDetailTypeDef](./type_defs.md#databaseconfigdetailtypedef) 
7. See [:material-code-brackets: InclusionStatusType](./literals.md#inclusionstatustype) 
8. See [:material-code-braces: AntipatternSeveritySummaryTypeDef](./type_defs.md#antipatternseveritysummarytypedef) 
9. See [:material-code-braces: RecommendationSetTypeDef](./type_defs.md#recommendationsettypedef) 
10. See [:material-code-brackets: ResourceSubTypeType](./literals.md#resourcesubtypetype) 
11. See [:material-code-braces: ResultTypeDef](./type_defs.md#resulttypedef) 
12. See [:material-code-brackets: RuntimeAnalysisStatusType](./literals.md#runtimeanalysisstatustype) 
13. See [:material-code-braces: SourceCodeRepositoryTypeDef](./type_defs.md#sourcecoderepositorytypedef) 
## ListCollectorsResponseTypeDef

```python
# ListCollectorsResponseTypeDef definition

class ListCollectorsResponseTypeDef(TypedDict):
    Collectors: List[CollectorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollectorTypeDef](./type_defs.md#collectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPortfolioPreferencesResponseTypeDef

```python
# GetPortfolioPreferencesResponseTypeDef definition

class GetPortfolioPreferencesResponseTypeDef(TypedDict):
    applicationMode: ApplicationModeType,  # (1)
    applicationPreferences: ApplicationPreferencesOutputTypeDef,  # (2)
    databasePreferences: DatabasePreferencesOutputTypeDef,  # (3)
    prioritizeBusinessGoals: PrioritizeBusinessGoalsTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ApplicationModeType](./literals.md#applicationmodetype) 
2. See [:material-code-braces: ApplicationPreferencesOutputTypeDef](./type_defs.md#applicationpreferencesoutputtypedef) 
3. See [:material-code-braces: DatabasePreferencesOutputTypeDef](./type_defs.md#databasepreferencesoutputtypedef) 
4. See [:material-code-braces: PrioritizeBusinessGoalsTypeDef](./type_defs.md#prioritizebusinessgoalstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationComponentStrategiesResponseTypeDef

```python
# GetApplicationComponentStrategiesResponseTypeDef definition

class GetApplicationComponentStrategiesResponseTypeDef(TypedDict):
    applicationComponentStrategies: List[ApplicationComponentStrategyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationComponentStrategyTypeDef](./type_defs.md#applicationcomponentstrategytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServerDetailsResponseTypeDef

```python
# GetServerDetailsResponseTypeDef definition

class GetServerDetailsResponseTypeDef(TypedDict):
    associatedApplications: List[AssociatedApplicationTypeDef],  # (1)
    serverDetail: ServerDetailTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociatedApplicationTypeDef](./type_defs.md#associatedapplicationtypedef) 
2. See [:material-code-braces: ServerDetailTypeDef](./type_defs.md#serverdetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServersResponseTypeDef

```python
# ListServersResponseTypeDef definition

class ListServersResponseTypeDef(TypedDict):
    serverInfos: List[ServerDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ServerDetailTypeDef](./type_defs.md#serverdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServerStrategiesResponseTypeDef

```python
# GetServerStrategiesResponseTypeDef definition

class GetServerStrategiesResponseTypeDef(TypedDict):
    serverStrategies: List[ServerStrategyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerStrategyTypeDef](./type_defs.md#serverstrategytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationComponentDetailsResponseTypeDef

```python
# GetApplicationComponentDetailsResponseTypeDef definition

class GetApplicationComponentDetailsResponseTypeDef(TypedDict):
    applicationComponentDetail: ApplicationComponentDetailTypeDef,  # (1)
    associatedApplications: List[AssociatedApplicationTypeDef],  # (2)
    associatedServerIds: List[str],
    moreApplicationResource: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ApplicationComponentDetailTypeDef](./type_defs.md#applicationcomponentdetailtypedef) 
2. See [:material-code-braces: AssociatedApplicationTypeDef](./type_defs.md#associatedapplicationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationComponentsResponseTypeDef

```python
# ListApplicationComponentsResponseTypeDef definition

class ListApplicationComponentsResponseTypeDef(TypedDict):
    applicationComponentInfos: List[ApplicationComponentDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationComponentDetailTypeDef](./type_defs.md#applicationcomponentdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatabasePreferencesTypeDef

```python
# DatabasePreferencesTypeDef definition

class DatabasePreferencesTypeDef(TypedDict):
    databaseManagementPreference: NotRequired[DatabaseManagementPreferenceType],  # (1)
    databaseMigrationPreference: NotRequired[DatabaseMigrationPreferenceUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: DatabaseManagementPreferenceType](./literals.md#databasemanagementpreferencetype) 
2. See [:material-code-braces: DatabaseMigrationPreferenceTypeDef](./type_defs.md#databasemigrationpreferencetypedef) [:material-code-braces: DatabaseMigrationPreferenceOutputTypeDef](./type_defs.md#databasemigrationpreferenceoutputtypedef) 
## ApplicationPreferencesTypeDef

```python
# ApplicationPreferencesTypeDef definition

class ApplicationPreferencesTypeDef(TypedDict):
    managementPreference: NotRequired[ManagementPreferenceUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ManagementPreferenceTypeDef](./type_defs.md#managementpreferencetypedef) [:material-code-braces: ManagementPreferenceOutputTypeDef](./type_defs.md#managementpreferenceoutputtypedef) 
## PutPortfolioPreferencesRequestRequestTypeDef

```python
# PutPortfolioPreferencesRequestRequestTypeDef definition

class PutPortfolioPreferencesRequestRequestTypeDef(TypedDict):
    applicationMode: NotRequired[ApplicationModeType],  # (1)
    applicationPreferences: NotRequired[ApplicationPreferencesTypeDef],  # (2)
    databasePreferences: NotRequired[DatabasePreferencesTypeDef],  # (3)
    prioritizeBusinessGoals: NotRequired[PrioritizeBusinessGoalsTypeDef],  # (4)
```

1. See [:material-code-brackets: ApplicationModeType](./literals.md#applicationmodetype) 
2. See [:material-code-braces: ApplicationPreferencesTypeDef](./type_defs.md#applicationpreferencestypedef) 
3. See [:material-code-braces: DatabasePreferencesTypeDef](./type_defs.md#databasepreferencestypedef) 
4. See [:material-code-braces: PrioritizeBusinessGoalsTypeDef](./type_defs.md#prioritizebusinessgoalstypedef) 
