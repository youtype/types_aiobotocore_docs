# Type definitions

> [Index](../README.md) > [MainframeModernization](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MainframeModernization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#mainframemodernization)
    type annotations stubs module [types-aiobotocore-m2](https://pypi.org/project/types-aiobotocore-m2/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AlternateKeyTypeDef

```python
# AlternateKeyTypeDef definition

class AlternateKeyTypeDef(TypedDict):
    length: int,
    offset: int,
    allowDuplicates: NotRequired[bool],
    name: NotRequired[str],
```

## ApplicationSummaryTypeDef

```python
# ApplicationSummaryTypeDef definition

class ApplicationSummaryTypeDef(TypedDict):
    applicationArn: str,
    applicationId: str,
    applicationVersion: int,
    creationTime: datetime,
    engineType: EngineTypeType,  # (2)
    name: str,
    status: ApplicationLifecycleType,  # (3)
    deploymentStatus: NotRequired[ApplicationDeploymentLifecycleType],  # (1)
    description: NotRequired[str],
    environmentId: NotRequired[str],
    lastStartTime: NotRequired[datetime],
    roleArn: NotRequired[str],
    versionStatus: NotRequired[ApplicationVersionLifecycleType],  # (4)
```

1. See [:material-code-brackets: ApplicationDeploymentLifecycleType](./literals.md#applicationdeploymentlifecycletype) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-brackets: ApplicationLifecycleType](./literals.md#applicationlifecycletype) 
4. See [:material-code-brackets: ApplicationVersionLifecycleType](./literals.md#applicationversionlifecycletype) 
## ApplicationVersionSummaryTypeDef

```python
# ApplicationVersionSummaryTypeDef definition

class ApplicationVersionSummaryTypeDef(TypedDict):
    applicationVersion: int,
    creationTime: datetime,
    status: ApplicationVersionLifecycleType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: ApplicationVersionLifecycleType](./literals.md#applicationversionlifecycletype) 
## FileBatchJobDefinitionTypeDef

```python
# FileBatchJobDefinitionTypeDef definition

class FileBatchJobDefinitionTypeDef(TypedDict):
    fileName: str,
    folderPath: NotRequired[str],
```

## ScriptBatchJobDefinitionTypeDef

```python
# ScriptBatchJobDefinitionTypeDef definition

class ScriptBatchJobDefinitionTypeDef(TypedDict):
    scriptName: str,
```

## FileBatchJobIdentifierTypeDef

```python
# FileBatchJobIdentifierTypeDef definition

class FileBatchJobIdentifierTypeDef(TypedDict):
    fileName: str,
    folderPath: NotRequired[str],
```

## ScriptBatchJobIdentifierTypeDef

```python
# ScriptBatchJobIdentifierTypeDef definition

class ScriptBatchJobIdentifierTypeDef(TypedDict):
    scriptName: str,
```

## CancelBatchJobExecutionRequestRequestTypeDef

```python
# CancelBatchJobExecutionRequestRequestTypeDef definition

class CancelBatchJobExecutionRequestRequestTypeDef(TypedDict):
    applicationId: str,
    executionId: str,
    authSecretsManagerArn: NotRequired[str],
```

## DefinitionTypeDef

```python
# DefinitionTypeDef definition

class DefinitionTypeDef(TypedDict):
    content: NotRequired[str],
    s3Location: NotRequired[str],
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

## CreateDeploymentRequestRequestTypeDef

```python
# CreateDeploymentRequestRequestTypeDef definition

class CreateDeploymentRequestRequestTypeDef(TypedDict):
    applicationId: str,
    applicationVersion: int,
    environmentId: str,
    clientToken: NotRequired[str],
```

## HighAvailabilityConfigTypeDef

```python
# HighAvailabilityConfigTypeDef definition

class HighAvailabilityConfigTypeDef(TypedDict):
    desiredCapacity: int,
```

## ExternalLocationTypeDef

```python
# ExternalLocationTypeDef definition

class ExternalLocationTypeDef(TypedDict):
    s3Location: NotRequired[str],
```

## DataSetImportSummaryTypeDef

```python
# DataSetImportSummaryTypeDef definition

class DataSetImportSummaryTypeDef(TypedDict):
    failed: int,
    inProgress: int,
    pending: int,
    succeeded: int,
    total: int,
```

## DataSetSummaryTypeDef

```python
# DataSetSummaryTypeDef definition

class DataSetSummaryTypeDef(TypedDict):
    dataSetName: str,
    creationTime: NotRequired[datetime],
    dataSetOrg: NotRequired[str],
    format: NotRequired[str],
    lastReferencedTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
```

## RecordLengthTypeDef

```python
# RecordLengthTypeDef definition

class RecordLengthTypeDef(TypedDict):
    max: int,
    min: int,
```

## GdgDetailAttributesTypeDef

```python
# GdgDetailAttributesTypeDef definition

class GdgDetailAttributesTypeDef(TypedDict):
    limit: NotRequired[int],
    rollDisposition: NotRequired[str],
```

## PoDetailAttributesTypeDef

```python
# PoDetailAttributesTypeDef definition

class PoDetailAttributesTypeDef(TypedDict):
    encoding: str,
    format: str,
```

## PsDetailAttributesTypeDef

```python
# PsDetailAttributesTypeDef definition

class PsDetailAttributesTypeDef(TypedDict):
    encoding: str,
    format: str,
```

## GdgAttributesTypeDef

```python
# GdgAttributesTypeDef definition

class GdgAttributesTypeDef(TypedDict):
    limit: NotRequired[int],
    rollDisposition: NotRequired[str],
```

## PoAttributesTypeDef

```python
# PoAttributesTypeDef definition

class PoAttributesTypeDef(TypedDict):
    format: str,
    memberFileExtensions: Sequence[str],
    encoding: NotRequired[str],
```

## PsAttributesTypeDef

```python
# PsAttributesTypeDef definition

class PsAttributesTypeDef(TypedDict):
    format: str,
    encoding: NotRequired[str],
```

## DeleteApplicationFromEnvironmentRequestRequestTypeDef

```python
# DeleteApplicationFromEnvironmentRequestRequestTypeDef definition

class DeleteApplicationFromEnvironmentRequestRequestTypeDef(TypedDict):
    applicationId: str,
    environmentId: str,
```

## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## DeleteEnvironmentRequestRequestTypeDef

```python
# DeleteEnvironmentRequestRequestTypeDef definition

class DeleteEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
```

## DeployedVersionSummaryTypeDef

```python
# DeployedVersionSummaryTypeDef definition

class DeployedVersionSummaryTypeDef(TypedDict):
    applicationVersion: int,
    status: DeploymentLifecycleType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentLifecycleType](./literals.md#deploymentlifecycletype) 
## DeploymentSummaryTypeDef

```python
# DeploymentSummaryTypeDef definition

class DeploymentSummaryTypeDef(TypedDict):
    applicationId: str,
    applicationVersion: int,
    creationTime: datetime,
    deploymentId: str,
    environmentId: str,
    status: DeploymentLifecycleType,  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentLifecycleType](./literals.md#deploymentlifecycletype) 
## EfsStorageConfigurationTypeDef

```python
# EfsStorageConfigurationTypeDef definition

class EfsStorageConfigurationTypeDef(TypedDict):
    fileSystemId: str,
    mountPoint: str,
```

## EngineVersionsSummaryTypeDef

```python
# EngineVersionsSummaryTypeDef definition

class EngineVersionsSummaryTypeDef(TypedDict):
    engineType: str,
    engineVersion: str,
```

## EnvironmentSummaryTypeDef

```python
# EnvironmentSummaryTypeDef definition

class EnvironmentSummaryTypeDef(TypedDict):
    creationTime: datetime,
    engineType: EngineTypeType,  # (1)
    engineVersion: str,
    environmentArn: str,
    environmentId: str,
    instanceType: str,
    name: str,
    status: EnvironmentLifecycleType,  # (3)
    networkType: NotRequired[NetworkTypeType],  # (2)
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
3. See [:material-code-brackets: EnvironmentLifecycleType](./literals.md#environmentlifecycletype) 
## FsxStorageConfigurationTypeDef

```python
# FsxStorageConfigurationTypeDef definition

class FsxStorageConfigurationTypeDef(TypedDict):
    fileSystemId: str,
    mountPoint: str,
```

## GetApplicationRequestRequestTypeDef

```python
# GetApplicationRequestRequestTypeDef definition

class GetApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## LogGroupSummaryTypeDef

```python
# LogGroupSummaryTypeDef definition

class LogGroupSummaryTypeDef(TypedDict):
    logGroupName: str,
    logType: str,
```

## GetApplicationVersionRequestRequestTypeDef

```python
# GetApplicationVersionRequestRequestTypeDef definition

class GetApplicationVersionRequestRequestTypeDef(TypedDict):
    applicationId: str,
    applicationVersion: int,
```

## GetBatchJobExecutionRequestRequestTypeDef

```python
# GetBatchJobExecutionRequestRequestTypeDef definition

class GetBatchJobExecutionRequestRequestTypeDef(TypedDict):
    applicationId: str,
    executionId: str,
```

## JobStepRestartMarkerTypeDef

```python
# JobStepRestartMarkerTypeDef definition

class JobStepRestartMarkerTypeDef(TypedDict):
    fromStep: str,
    fromProcStep: NotRequired[str],
    toProcStep: NotRequired[str],
    toStep: NotRequired[str],
```

## GetDataSetDetailsRequestRequestTypeDef

```python
# GetDataSetDetailsRequestRequestTypeDef definition

class GetDataSetDetailsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    dataSetName: str,
```

## GetDataSetImportTaskRequestRequestTypeDef

```python
# GetDataSetImportTaskRequestRequestTypeDef definition

class GetDataSetImportTaskRequestRequestTypeDef(TypedDict):
    applicationId: str,
    taskId: str,
```

## GetDeploymentRequestRequestTypeDef

```python
# GetDeploymentRequestRequestTypeDef definition

class GetDeploymentRequestRequestTypeDef(TypedDict):
    applicationId: str,
    deploymentId: str,
```

## GetEnvironmentRequestRequestTypeDef

```python
# GetEnvironmentRequestRequestTypeDef definition

class GetEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
```

## JobIdentifierTypeDef

```python
# JobIdentifierTypeDef definition

class JobIdentifierTypeDef(TypedDict):
    fileName: NotRequired[str],
    scriptName: NotRequired[str],
```

## JobStepTypeDef

```python
# JobStepTypeDef definition

class JobStepTypeDef(TypedDict):
    procStepName: NotRequired[str],
    procStepNumber: NotRequired[int],
    stepCondCode: NotRequired[str],
    stepName: NotRequired[str],
    stepNumber: NotRequired[int],
    stepRestartable: NotRequired[bool],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListApplicationVersionsRequestRequestTypeDef

```python
# ListApplicationVersionsRequestRequestTypeDef definition

class ListApplicationVersionsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    environmentId: NotRequired[str],
    maxResults: NotRequired[int],
    names: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
```

## ListBatchJobDefinitionsRequestRequestTypeDef

```python
# ListBatchJobDefinitionsRequestRequestTypeDef definition

class ListBatchJobDefinitionsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    prefix: NotRequired[str],
```

## ListBatchJobRestartPointsRequestRequestTypeDef

```python
# ListBatchJobRestartPointsRequestRequestTypeDef definition

class ListBatchJobRestartPointsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    executionId: str,
    authSecretsManagerArn: NotRequired[str],
```

## ListDataSetImportHistoryRequestRequestTypeDef

```python
# ListDataSetImportHistoryRequestRequestTypeDef definition

class ListDataSetImportHistoryRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDataSetsRequestRequestTypeDef

```python
# ListDataSetsRequestRequestTypeDef definition

class ListDataSetsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nameFilter: NotRequired[str],
    nextToken: NotRequired[str],
    prefix: NotRequired[str],
```

## ListDeploymentsRequestRequestTypeDef

```python
# ListDeploymentsRequestRequestTypeDef definition

class ListDeploymentsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListEngineVersionsRequestRequestTypeDef

```python
# ListEngineVersionsRequestRequestTypeDef definition

class ListEngineVersionsRequestRequestTypeDef(TypedDict):
    engineType: NotRequired[EngineTypeType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
## ListEnvironmentsRequestRequestTypeDef

```python
# ListEnvironmentsRequestRequestTypeDef definition

class ListEnvironmentsRequestRequestTypeDef(TypedDict):
    engineType: NotRequired[EngineTypeType],  # (1)
    maxResults: NotRequired[int],
    names: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## MaintenanceScheduleTypeDef

```python
# MaintenanceScheduleTypeDef definition

class MaintenanceScheduleTypeDef(TypedDict):
    endTime: NotRequired[datetime],
    startTime: NotRequired[datetime],
```

## PrimaryKeyTypeDef

```python
# PrimaryKeyTypeDef definition

class PrimaryKeyTypeDef(TypedDict):
    length: int,
    offset: int,
    name: NotRequired[str],
```

## StartApplicationRequestRequestTypeDef

```python
# StartApplicationRequestRequestTypeDef definition

class StartApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## StopApplicationRequestRequestTypeDef

```python
# StopApplicationRequestRequestTypeDef definition

class StopApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
    forceStop: NotRequired[bool],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateEnvironmentRequestRequestTypeDef

```python
# UpdateEnvironmentRequestRequestTypeDef definition

class UpdateEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
    applyDuringMaintenanceWindow: NotRequired[bool],
    desiredCapacity: NotRequired[int],
    engineVersion: NotRequired[str],
    forceUpdate: NotRequired[bool],
    instanceType: NotRequired[str],
    preferredMaintenanceWindow: NotRequired[str],
```

## BatchJobDefinitionTypeDef

```python
# BatchJobDefinitionTypeDef definition

class BatchJobDefinitionTypeDef(TypedDict):
    fileBatchJobDefinition: NotRequired[FileBatchJobDefinitionTypeDef],  # (1)
    scriptBatchJobDefinition: NotRequired[ScriptBatchJobDefinitionTypeDef],  # (2)
```

1. See [:material-code-braces: FileBatchJobDefinitionTypeDef](./type_defs.md#filebatchjobdefinitiontypedef) 
2. See [:material-code-braces: ScriptBatchJobDefinitionTypeDef](./type_defs.md#scriptbatchjobdefinitiontypedef) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    definition: DefinitionTypeDef,  # (1)
    engineType: EngineTypeType,  # (2)
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    kmsKeyId: NotRequired[str],
    roleArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DefinitionTypeDef](./type_defs.md#definitiontypedef) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
    currentApplicationVersion: int,
    definition: NotRequired[DefinitionTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: DefinitionTypeDef](./type_defs.md#definitiontypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    applicationArn: str,
    applicationId: str,
    applicationVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSetImportTaskResponseTypeDef

```python
# CreateDataSetImportTaskResponseTypeDef definition

class CreateDataSetImportTaskResponseTypeDef(TypedDict):
    taskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentResponseTypeDef

```python
# CreateDeploymentResponseTypeDef definition

class CreateDeploymentResponseTypeDef(TypedDict):
    deploymentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentResponseTypeDef

```python
# CreateEnvironmentResponseTypeDef definition

class CreateEnvironmentResponseTypeDef(TypedDict):
    environmentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationVersionResponseTypeDef

```python
# GetApplicationVersionResponseTypeDef definition

class GetApplicationVersionResponseTypeDef(TypedDict):
    applicationVersion: int,
    creationTime: datetime,
    definitionContent: str,
    description: str,
    name: str,
    status: ApplicationVersionLifecycleType,  # (1)
    statusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ApplicationVersionLifecycleType](./literals.md#applicationversionlifecycletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeploymentResponseTypeDef

```python
# GetDeploymentResponseTypeDef definition

class GetDeploymentResponseTypeDef(TypedDict):
    applicationId: str,
    applicationVersion: int,
    creationTime: datetime,
    deploymentId: str,
    environmentId: str,
    status: DeploymentLifecycleType,  # (1)
    statusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DeploymentLifecycleType](./literals.md#deploymentlifecycletype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSignedBluinsightsUrlResponseTypeDef

```python
# GetSignedBluinsightsUrlResponseTypeDef definition

class GetSignedBluinsightsUrlResponseTypeDef(TypedDict):
    signedBiUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationVersionsResponseTypeDef

```python
# ListApplicationVersionsResponseTypeDef definition

class ListApplicationVersionsResponseTypeDef(TypedDict):
    applicationVersions: List[ApplicationVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationVersionSummaryTypeDef](./type_defs.md#applicationversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    applications: List[ApplicationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBatchJobResponseTypeDef

```python
# StartBatchJobResponseTypeDef definition

class StartBatchJobResponseTypeDef(TypedDict):
    executionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationResponseTypeDef

```python
# UpdateApplicationResponseTypeDef definition

class UpdateApplicationResponseTypeDef(TypedDict):
    applicationVersion: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentResponseTypeDef

```python
# UpdateEnvironmentResponseTypeDef definition

class UpdateEnvironmentResponseTypeDef(TypedDict):
    environmentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSetImportTaskTypeDef

```python
# DataSetImportTaskTypeDef definition

class DataSetImportTaskTypeDef(TypedDict):
    status: DataSetTaskLifecycleType,  # (1)
    summary: DataSetImportSummaryTypeDef,  # (2)
    taskId: str,
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: DataSetTaskLifecycleType](./literals.md#datasettasklifecycletype) 
2. See [:material-code-braces: DataSetImportSummaryTypeDef](./type_defs.md#datasetimportsummarytypedef) 
## GetDataSetImportTaskResponseTypeDef

```python
# GetDataSetImportTaskResponseTypeDef definition

class GetDataSetImportTaskResponseTypeDef(TypedDict):
    status: DataSetTaskLifecycleType,  # (1)
    summary: DataSetImportSummaryTypeDef,  # (2)
    taskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DataSetTaskLifecycleType](./literals.md#datasettasklifecycletype) 
2. See [:material-code-braces: DataSetImportSummaryTypeDef](./type_defs.md#datasetimportsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataSetsResponseTypeDef

```python
# ListDataSetsResponseTypeDef definition

class ListDataSetsResponseTypeDef(TypedDict):
    dataSets: List[DataSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSetSummaryTypeDef](./type_defs.md#datasetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentsResponseTypeDef

```python
# ListDeploymentsResponseTypeDef definition

class ListDeploymentsResponseTypeDef(TypedDict):
    deployments: List[DeploymentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentSummaryTypeDef](./type_defs.md#deploymentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEngineVersionsResponseTypeDef

```python
# ListEngineVersionsResponseTypeDef definition

class ListEngineVersionsResponseTypeDef(TypedDict):
    engineVersions: List[EngineVersionsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EngineVersionsSummaryTypeDef](./type_defs.md#engineversionssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentsResponseTypeDef

```python
# ListEnvironmentsResponseTypeDef definition

class ListEnvironmentsResponseTypeDef(TypedDict):
    environments: List[EnvironmentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentSummaryTypeDef](./type_defs.md#environmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StorageConfigurationTypeDef

```python
# StorageConfigurationTypeDef definition

class StorageConfigurationTypeDef(TypedDict):
    efs: NotRequired[EfsStorageConfigurationTypeDef],  # (1)
    fsx: NotRequired[FsxStorageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: EfsStorageConfigurationTypeDef](./type_defs.md#efsstorageconfigurationtypedef) 
2. See [:material-code-braces: FsxStorageConfigurationTypeDef](./type_defs.md#fsxstorageconfigurationtypedef) 
## GetApplicationResponseTypeDef

```python
# GetApplicationResponseTypeDef definition

class GetApplicationResponseTypeDef(TypedDict):
    applicationArn: str,
    applicationId: str,
    creationTime: datetime,
    deployedVersion: DeployedVersionSummaryTypeDef,  # (1)
    description: str,
    engineType: EngineTypeType,  # (2)
    environmentId: str,
    kmsKeyId: str,
    lastStartTime: datetime,
    latestVersion: ApplicationVersionSummaryTypeDef,  # (3)
    listenerArns: List[str],
    listenerPorts: List[int],
    loadBalancerDnsName: str,
    logGroups: List[LogGroupSummaryTypeDef],  # (4)
    name: str,
    roleArn: str,
    status: ApplicationLifecycleType,  # (5)
    statusReason: str,
    tags: Dict[str, str],
    targetGroupArns: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: DeployedVersionSummaryTypeDef](./type_defs.md#deployedversionsummarytypedef) 
2. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
3. See [:material-code-braces: ApplicationVersionSummaryTypeDef](./type_defs.md#applicationversionsummarytypedef) 
4. See [:material-code-braces: LogGroupSummaryTypeDef](./type_defs.md#loggroupsummarytypedef) 
5. See [:material-code-brackets: ApplicationLifecycleType](./literals.md#applicationlifecycletype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestartBatchJobIdentifierTypeDef

```python
# RestartBatchJobIdentifierTypeDef definition

class RestartBatchJobIdentifierTypeDef(TypedDict):
    executionId: str,
    jobStepRestartMarker: JobStepRestartMarkerTypeDef,  # (1)
```

1. See [:material-code-braces: JobStepRestartMarkerTypeDef](./type_defs.md#jobsteprestartmarkertypedef) 
## S3BatchJobIdentifierTypeDef

```python
# S3BatchJobIdentifierTypeDef definition

class S3BatchJobIdentifierTypeDef(TypedDict):
    bucket: str,
    identifier: JobIdentifierTypeDef,  # (1)
    keyPrefix: NotRequired[str],
```

1. See [:material-code-braces: JobIdentifierTypeDef](./type_defs.md#jobidentifiertypedef) 
## ListBatchJobRestartPointsResponseTypeDef

```python
# ListBatchJobRestartPointsResponseTypeDef definition

class ListBatchJobRestartPointsResponseTypeDef(TypedDict):
    batchJobSteps: List[JobStepTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobStepTypeDef](./type_defs.md#jobsteptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationVersionsRequestPaginateTypeDef

```python
# ListApplicationVersionsRequestPaginateTypeDef definition

class ListApplicationVersionsRequestPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationsRequestPaginateTypeDef

```python
# ListApplicationsRequestPaginateTypeDef definition

class ListApplicationsRequestPaginateTypeDef(TypedDict):
    environmentId: NotRequired[str],
    names: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBatchJobDefinitionsRequestPaginateTypeDef

```python
# ListBatchJobDefinitionsRequestPaginateTypeDef definition

class ListBatchJobDefinitionsRequestPaginateTypeDef(TypedDict):
    applicationId: str,
    prefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSetImportHistoryRequestPaginateTypeDef

```python
# ListDataSetImportHistoryRequestPaginateTypeDef definition

class ListDataSetImportHistoryRequestPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSetsRequestPaginateTypeDef

```python
# ListDataSetsRequestPaginateTypeDef definition

class ListDataSetsRequestPaginateTypeDef(TypedDict):
    applicationId: str,
    nameFilter: NotRequired[str],
    prefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentsRequestPaginateTypeDef

```python
# ListDeploymentsRequestPaginateTypeDef definition

class ListDeploymentsRequestPaginateTypeDef(TypedDict):
    applicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEngineVersionsRequestPaginateTypeDef

```python
# ListEngineVersionsRequestPaginateTypeDef definition

class ListEngineVersionsRequestPaginateTypeDef(TypedDict):
    engineType: NotRequired[EngineTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentsRequestPaginateTypeDef

```python
# ListEnvironmentsRequestPaginateTypeDef definition

class ListEnvironmentsRequestPaginateTypeDef(TypedDict):
    engineType: NotRequired[EngineTypeType],  # (1)
    names: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBatchJobExecutionsRequestPaginateTypeDef

```python
# ListBatchJobExecutionsRequestPaginateTypeDef definition

class ListBatchJobExecutionsRequestPaginateTypeDef(TypedDict):
    applicationId: str,
    executionIds: NotRequired[Sequence[str]],
    jobName: NotRequired[str],
    startedAfter: NotRequired[TimestampTypeDef],
    startedBefore: NotRequired[TimestampTypeDef],
    status: NotRequired[BatchJobExecutionStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: BatchJobExecutionStatusType](./literals.md#batchjobexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBatchJobExecutionsRequestRequestTypeDef

```python
# ListBatchJobExecutionsRequestRequestTypeDef definition

class ListBatchJobExecutionsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    executionIds: NotRequired[Sequence[str]],
    jobName: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    startedAfter: NotRequired[TimestampTypeDef],
    startedBefore: NotRequired[TimestampTypeDef],
    status: NotRequired[BatchJobExecutionStatusType],  # (1)
```

1. See [:material-code-brackets: BatchJobExecutionStatusType](./literals.md#batchjobexecutionstatustype) 
## PendingMaintenanceTypeDef

```python
# PendingMaintenanceTypeDef definition

class PendingMaintenanceTypeDef(TypedDict):
    engineVersion: NotRequired[str],
    schedule: NotRequired[MaintenanceScheduleTypeDef],  # (1)
```

1. See [:material-code-braces: MaintenanceScheduleTypeDef](./type_defs.md#maintenancescheduletypedef) 
## VsamAttributesTypeDef

```python
# VsamAttributesTypeDef definition

class VsamAttributesTypeDef(TypedDict):
    format: str,
    alternateKeys: NotRequired[Sequence[AlternateKeyTypeDef]],  # (1)
    compressed: NotRequired[bool],
    encoding: NotRequired[str],
    primaryKey: NotRequired[PrimaryKeyTypeDef],  # (2)
```

1. See [:material-code-braces: AlternateKeyTypeDef](./type_defs.md#alternatekeytypedef) 
2. See [:material-code-braces: PrimaryKeyTypeDef](./type_defs.md#primarykeytypedef) 
## VsamDetailAttributesTypeDef

```python
# VsamDetailAttributesTypeDef definition

class VsamDetailAttributesTypeDef(TypedDict):
    alternateKeys: NotRequired[List[AlternateKeyTypeDef]],  # (1)
    cacheAtStartup: NotRequired[bool],
    compressed: NotRequired[bool],
    encoding: NotRequired[str],
    primaryKey: NotRequired[PrimaryKeyTypeDef],  # (2)
    recordFormat: NotRequired[str],
```

1. See [:material-code-braces: AlternateKeyTypeDef](./type_defs.md#alternatekeytypedef) 
2. See [:material-code-braces: PrimaryKeyTypeDef](./type_defs.md#primarykeytypedef) 
## ListBatchJobDefinitionsResponseTypeDef

```python
# ListBatchJobDefinitionsResponseTypeDef definition

class ListBatchJobDefinitionsResponseTypeDef(TypedDict):
    batchJobDefinitions: List[BatchJobDefinitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BatchJobDefinitionTypeDef](./type_defs.md#batchjobdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataSetImportHistoryResponseTypeDef

```python
# ListDataSetImportHistoryResponseTypeDef definition

class ListDataSetImportHistoryResponseTypeDef(TypedDict):
    dataSetImportTasks: List[DataSetImportTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSetImportTaskTypeDef](./type_defs.md#datasetimporttasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentRequestRequestTypeDef

```python
# CreateEnvironmentRequestRequestTypeDef definition

class CreateEnvironmentRequestRequestTypeDef(TypedDict):
    engineType: EngineTypeType,  # (1)
    instanceType: str,
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    engineVersion: NotRequired[str],
    highAvailabilityConfig: NotRequired[HighAvailabilityConfigTypeDef],  # (2)
    kmsKeyId: NotRequired[str],
    networkType: NotRequired[NetworkTypeType],  # (3)
    preferredMaintenanceWindow: NotRequired[str],
    publiclyAccessible: NotRequired[bool],
    securityGroupIds: NotRequired[Sequence[str]],
    storageConfigurations: NotRequired[Sequence[StorageConfigurationTypeDef]],  # (4)
    subnetIds: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: HighAvailabilityConfigTypeDef](./type_defs.md#highavailabilityconfigtypedef) 
3. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
4. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
## BatchJobIdentifierTypeDef

```python
# BatchJobIdentifierTypeDef definition

class BatchJobIdentifierTypeDef(TypedDict):
    fileBatchJobIdentifier: NotRequired[FileBatchJobIdentifierTypeDef],  # (1)
    restartBatchJobIdentifier: NotRequired[RestartBatchJobIdentifierTypeDef],  # (2)
    s3BatchJobIdentifier: NotRequired[S3BatchJobIdentifierTypeDef],  # (3)
    scriptBatchJobIdentifier: NotRequired[ScriptBatchJobIdentifierTypeDef],  # (4)
```

1. See [:material-code-braces: FileBatchJobIdentifierTypeDef](./type_defs.md#filebatchjobidentifiertypedef) 
2. See [:material-code-braces: RestartBatchJobIdentifierTypeDef](./type_defs.md#restartbatchjobidentifiertypedef) 
3. See [:material-code-braces: S3BatchJobIdentifierTypeDef](./type_defs.md#s3batchjobidentifiertypedef) 
4. See [:material-code-braces: ScriptBatchJobIdentifierTypeDef](./type_defs.md#scriptbatchjobidentifiertypedef) 
## GetEnvironmentResponseTypeDef

```python
# GetEnvironmentResponseTypeDef definition

class GetEnvironmentResponseTypeDef(TypedDict):
    actualCapacity: int,
    creationTime: datetime,
    description: str,
    engineType: EngineTypeType,  # (1)
    engineVersion: str,
    environmentArn: str,
    environmentId: str,
    highAvailabilityConfig: HighAvailabilityConfigTypeDef,  # (2)
    instanceType: str,
    kmsKeyId: str,
    loadBalancerArn: str,
    name: str,
    networkType: NetworkTypeType,  # (3)
    pendingMaintenance: PendingMaintenanceTypeDef,  # (4)
    preferredMaintenanceWindow: str,
    publiclyAccessible: bool,
    securityGroupIds: List[str],
    status: EnvironmentLifecycleType,  # (5)
    statusReason: str,
    storageConfigurations: List[StorageConfigurationTypeDef],  # (6)
    subnetIds: List[str],
    tags: Dict[str, str],
    vpcId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: HighAvailabilityConfigTypeDef](./type_defs.md#highavailabilityconfigtypedef) 
3. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
4. See [:material-code-braces: PendingMaintenanceTypeDef](./type_defs.md#pendingmaintenancetypedef) 
5. See [:material-code-brackets: EnvironmentLifecycleType](./literals.md#environmentlifecycletype) 
6. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetOrgAttributesTypeDef

```python
# DatasetOrgAttributesTypeDef definition

class DatasetOrgAttributesTypeDef(TypedDict):
    gdg: NotRequired[GdgAttributesTypeDef],  # (1)
    po: NotRequired[PoAttributesTypeDef],  # (2)
    ps: NotRequired[PsAttributesTypeDef],  # (3)
    vsam: NotRequired[VsamAttributesTypeDef],  # (4)
```

1. See [:material-code-braces: GdgAttributesTypeDef](./type_defs.md#gdgattributestypedef) 
2. See [:material-code-braces: PoAttributesTypeDef](./type_defs.md#poattributestypedef) 
3. See [:material-code-braces: PsAttributesTypeDef](./type_defs.md#psattributestypedef) 
4. See [:material-code-braces: VsamAttributesTypeDef](./type_defs.md#vsamattributestypedef) 
## DatasetDetailOrgAttributesTypeDef

```python
# DatasetDetailOrgAttributesTypeDef definition

class DatasetDetailOrgAttributesTypeDef(TypedDict):
    gdg: NotRequired[GdgDetailAttributesTypeDef],  # (1)
    po: NotRequired[PoDetailAttributesTypeDef],  # (2)
    ps: NotRequired[PsDetailAttributesTypeDef],  # (3)
    vsam: NotRequired[VsamDetailAttributesTypeDef],  # (4)
```

1. See [:material-code-braces: GdgDetailAttributesTypeDef](./type_defs.md#gdgdetailattributestypedef) 
2. See [:material-code-braces: PoDetailAttributesTypeDef](./type_defs.md#podetailattributestypedef) 
3. See [:material-code-braces: PsDetailAttributesTypeDef](./type_defs.md#psdetailattributestypedef) 
4. See [:material-code-braces: VsamDetailAttributesTypeDef](./type_defs.md#vsamdetailattributestypedef) 
## BatchJobExecutionSummaryTypeDef

```python
# BatchJobExecutionSummaryTypeDef definition

class BatchJobExecutionSummaryTypeDef(TypedDict):
    applicationId: str,
    executionId: str,
    startTime: datetime,
    status: BatchJobExecutionStatusType,  # (3)
    batchJobIdentifier: NotRequired[BatchJobIdentifierTypeDef],  # (1)
    endTime: NotRequired[datetime],
    jobId: NotRequired[str],
    jobName: NotRequired[str],
    jobType: NotRequired[BatchJobTypeType],  # (2)
    returnCode: NotRequired[str],
```

1. See [:material-code-braces: BatchJobIdentifierTypeDef](./type_defs.md#batchjobidentifiertypedef) 
2. See [:material-code-brackets: BatchJobTypeType](./literals.md#batchjobtypetype) 
3. See [:material-code-brackets: BatchJobExecutionStatusType](./literals.md#batchjobexecutionstatustype) 
## GetBatchJobExecutionResponseTypeDef

```python
# GetBatchJobExecutionResponseTypeDef definition

class GetBatchJobExecutionResponseTypeDef(TypedDict):
    applicationId: str,
    batchJobIdentifier: BatchJobIdentifierTypeDef,  # (1)
    endTime: datetime,
    executionId: str,
    jobId: str,
    jobName: str,
    jobStepRestartMarker: JobStepRestartMarkerTypeDef,  # (2)
    jobType: BatchJobTypeType,  # (3)
    jobUser: str,
    returnCode: str,
    startTime: datetime,
    status: BatchJobExecutionStatusType,  # (4)
    statusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: BatchJobIdentifierTypeDef](./type_defs.md#batchjobidentifiertypedef) 
2. See [:material-code-braces: JobStepRestartMarkerTypeDef](./type_defs.md#jobsteprestartmarkertypedef) 
3. See [:material-code-brackets: BatchJobTypeType](./literals.md#batchjobtypetype) 
4. See [:material-code-brackets: BatchJobExecutionStatusType](./literals.md#batchjobexecutionstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBatchJobRequestRequestTypeDef

```python
# StartBatchJobRequestRequestTypeDef definition

class StartBatchJobRequestRequestTypeDef(TypedDict):
    applicationId: str,
    batchJobIdentifier: BatchJobIdentifierTypeDef,  # (1)
    authSecretsManagerArn: NotRequired[str],
    jobParams: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: BatchJobIdentifierTypeDef](./type_defs.md#batchjobidentifiertypedef) 
## DataSetTypeDef

```python
# DataSetTypeDef definition

class DataSetTypeDef(TypedDict):
    datasetName: str,
    datasetOrg: DatasetOrgAttributesTypeDef,  # (1)
    recordLength: RecordLengthTypeDef,  # (2)
    relativePath: NotRequired[str],
    storageType: NotRequired[str],
```

1. See [:material-code-braces: DatasetOrgAttributesTypeDef](./type_defs.md#datasetorgattributestypedef) 
2. See [:material-code-braces: RecordLengthTypeDef](./type_defs.md#recordlengthtypedef) 
## GetDataSetDetailsResponseTypeDef

```python
# GetDataSetDetailsResponseTypeDef definition

class GetDataSetDetailsResponseTypeDef(TypedDict):
    blocksize: int,
    creationTime: datetime,
    dataSetName: str,
    dataSetOrg: DatasetDetailOrgAttributesTypeDef,  # (1)
    fileSize: int,
    lastReferencedTime: datetime,
    lastUpdatedTime: datetime,
    location: str,
    recordLength: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetDetailOrgAttributesTypeDef](./type_defs.md#datasetdetailorgattributestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBatchJobExecutionsResponseTypeDef

```python
# ListBatchJobExecutionsResponseTypeDef definition

class ListBatchJobExecutionsResponseTypeDef(TypedDict):
    batchJobExecutions: List[BatchJobExecutionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BatchJobExecutionSummaryTypeDef](./type_defs.md#batchjobexecutionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSetImportItemTypeDef

```python
# DataSetImportItemTypeDef definition

class DataSetImportItemTypeDef(TypedDict):
    dataSet: DataSetTypeDef,  # (1)
    externalLocation: ExternalLocationTypeDef,  # (2)
```

1. See [:material-code-braces: DataSetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: ExternalLocationTypeDef](./type_defs.md#externallocationtypedef) 
## DataSetImportConfigTypeDef

```python
# DataSetImportConfigTypeDef definition

class DataSetImportConfigTypeDef(TypedDict):
    dataSets: NotRequired[Sequence[DataSetImportItemTypeDef]],  # (1)
    s3Location: NotRequired[str],
```

1. See [:material-code-braces: DataSetImportItemTypeDef](./type_defs.md#datasetimportitemtypedef) 
## CreateDataSetImportTaskRequestRequestTypeDef

```python
# CreateDataSetImportTaskRequestRequestTypeDef definition

class CreateDataSetImportTaskRequestRequestTypeDef(TypedDict):
    applicationId: str,
    importConfig: DataSetImportConfigTypeDef,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: DataSetImportConfigTypeDef](./type_defs.md#datasetimportconfigtypedef) 
