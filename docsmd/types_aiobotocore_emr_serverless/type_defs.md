# Type definitions

> [Index](../README.md) > [EMRServerless](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EMRServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#emrserverless)
    type annotations stubs module [types-aiobotocore-emr-serverless](https://pypi.org/project/types-aiobotocore-emr-serverless/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## CloudWatchLoggingConfigurationUnionTypeDef

```python
# CloudWatchLoggingConfigurationUnionTypeDef definition

CloudWatchLoggingConfigurationUnionTypeDef = Union[
    CloudWatchLoggingConfigurationTypeDef,  # (1)
    CloudWatchLoggingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CloudWatchLoggingConfigurationTypeDef](./type_defs.md#cloudwatchloggingconfigurationtypedef) 
2. See [:material-code-braces: CloudWatchLoggingConfigurationOutputTypeDef](./type_defs.md#cloudwatchloggingconfigurationoutputtypedef) 

## ConfigurationUnionTypeDef

```python
# ConfigurationUnionTypeDef definition

ConfigurationUnionTypeDef = Union[
    ConfigurationTypeDef,  # (1)
    ConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 

## SparkSubmitUnionTypeDef

```python
# SparkSubmitUnionTypeDef definition

SparkSubmitUnionTypeDef = Union[
    SparkSubmitTypeDef,  # (1)
    SparkSubmitOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SparkSubmitTypeDef](./type_defs.md#sparksubmittypedef) 
2. See [:material-code-braces: SparkSubmitOutputTypeDef](./type_defs.md#sparksubmitoutputtypedef) 

## MonitoringConfigurationUnionTypeDef

```python
# MonitoringConfigurationUnionTypeDef definition

MonitoringConfigurationUnionTypeDef = Union[
    MonitoringConfigurationTypeDef,  # (1)
    MonitoringConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MonitoringConfigurationTypeDef](./type_defs.md#monitoringconfigurationtypedef) 
2. See [:material-code-braces: MonitoringConfigurationOutputTypeDef](./type_defs.md#monitoringconfigurationoutputtypedef) 



## ApplicationSummaryTypeDef

```python
# ApplicationSummaryTypeDef definition

class ApplicationSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    releaseLabel: str,
    type: str,
    state: ApplicationStateType,  # (1)
    createdAt: datetime,
    updatedAt: datetime,
    name: NotRequired[str],
    stateDetails: NotRequired[str],
    architecture: NotRequired[ArchitectureType],  # (2)
```

1. See [:material-code-brackets: ApplicationStateType](./literals.md#applicationstatetype) 
2. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
## AutoStartConfigTypeDef

```python
# AutoStartConfigTypeDef definition

class AutoStartConfigTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## AutoStopConfigTypeDef

```python
# AutoStopConfigTypeDef definition

class AutoStopConfigTypeDef(TypedDict):
    enabled: NotRequired[bool],
    idleTimeoutMinutes: NotRequired[int],
```

## ConfigurationOutputTypeDef

```python
# ConfigurationOutputTypeDef definition

class ConfigurationOutputTypeDef(TypedDict):
    classification: str,
    properties: NotRequired[Dict[str, str]],
    configurations: NotRequired[List[Dict[str, Any]]],
```

## ImageConfigurationTypeDef

```python
# ImageConfigurationTypeDef definition

class ImageConfigurationTypeDef(TypedDict):
    imageUri: str,
    resolvedImageDigest: NotRequired[str],
```

## InteractiveConfigurationTypeDef

```python
# InteractiveConfigurationTypeDef definition

class InteractiveConfigurationTypeDef(TypedDict):
    studioEnabled: NotRequired[bool],
    livyEndpointEnabled: NotRequired[bool],
```

## MaximumAllowedResourcesTypeDef

```python
# MaximumAllowedResourcesTypeDef definition

class MaximumAllowedResourcesTypeDef(TypedDict):
    cpu: str,
    memory: str,
    disk: NotRequired[str],
```

## NetworkConfigurationOutputTypeDef

```python
# NetworkConfigurationOutputTypeDef definition

class NetworkConfigurationOutputTypeDef(TypedDict):
    subnetIds: NotRequired[List[str]],
    securityGroupIds: NotRequired[List[str]],
```

## SchedulerConfigurationTypeDef

```python
# SchedulerConfigurationTypeDef definition

class SchedulerConfigurationTypeDef(TypedDict):
    queueTimeoutMinutes: NotRequired[int],
    maxConcurrentRuns: NotRequired[int],
```

## CancelJobRunRequestRequestTypeDef

```python
# CancelJobRunRequestRequestTypeDef definition

class CancelJobRunRequestRequestTypeDef(TypedDict):
    applicationId: str,
    jobRunId: str,
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

## CloudWatchLoggingConfigurationOutputTypeDef

```python
# CloudWatchLoggingConfigurationOutputTypeDef definition

class CloudWatchLoggingConfigurationOutputTypeDef(TypedDict):
    enabled: bool,
    logGroupName: NotRequired[str],
    logStreamNamePrefix: NotRequired[str],
    encryptionKeyArn: NotRequired[str],
    logTypes: NotRequired[Dict[str, List[str]]],
```

## CloudWatchLoggingConfigurationTypeDef

```python
# CloudWatchLoggingConfigurationTypeDef definition

class CloudWatchLoggingConfigurationTypeDef(TypedDict):
    enabled: bool,
    logGroupName: NotRequired[str],
    logStreamNamePrefix: NotRequired[str],
    encryptionKeyArn: NotRequired[str],
    logTypes: NotRequired[Mapping[str, Sequence[str]]],
```

## ConfigurationTypeDef

```python
# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    classification: str,
    properties: NotRequired[Mapping[str, str]],
    configurations: NotRequired[Sequence[Mapping[str, Any]]],
```

## ImageConfigurationInputTypeDef

```python
# ImageConfigurationInputTypeDef definition

class ImageConfigurationInputTypeDef(TypedDict):
    imageUri: NotRequired[str],
```

## NetworkConfigurationTypeDef

```python
# NetworkConfigurationTypeDef definition

class NetworkConfigurationTypeDef(TypedDict):
    subnetIds: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
```

## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## GetApplicationRequestRequestTypeDef

```python
# GetApplicationRequestRequestTypeDef definition

class GetApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
```

## GetDashboardForJobRunRequestRequestTypeDef

```python
# GetDashboardForJobRunRequestRequestTypeDef definition

class GetDashboardForJobRunRequestRequestTypeDef(TypedDict):
    applicationId: str,
    jobRunId: str,
    attempt: NotRequired[int],
    accessSystemProfileLogs: NotRequired[bool],
```

## GetJobRunRequestRequestTypeDef

```python
# GetJobRunRequestRequestTypeDef definition

class GetJobRunRequestRequestTypeDef(TypedDict):
    applicationId: str,
    jobRunId: str,
    attempt: NotRequired[int],
```

## HiveTypeDef

```python
# HiveTypeDef definition

class HiveTypeDef(TypedDict):
    query: str,
    initQueryFile: NotRequired[str],
    parameters: NotRequired[str],
```

## WorkerResourceConfigTypeDef

```python
# WorkerResourceConfigTypeDef definition

class WorkerResourceConfigTypeDef(TypedDict):
    cpu: str,
    memory: str,
    disk: NotRequired[str],
    diskType: NotRequired[str],
```

## SparkSubmitOutputTypeDef

```python
# SparkSubmitOutputTypeDef definition

class SparkSubmitOutputTypeDef(TypedDict):
    entryPoint: str,
    entryPointArguments: NotRequired[List[str]],
    sparkSubmitParameters: NotRequired[str],
```

## JobRunAttemptSummaryTypeDef

```python
# JobRunAttemptSummaryTypeDef definition

class JobRunAttemptSummaryTypeDef(TypedDict):
    applicationId: str,
    id: str,
    arn: str,
    createdBy: str,
    jobCreatedAt: datetime,
    createdAt: datetime,
    updatedAt: datetime,
    executionRole: str,
    state: JobRunStateType,  # (2)
    stateDetails: str,
    releaseLabel: str,
    name: NotRequired[str],
    mode: NotRequired[JobRunModeType],  # (1)
    type: NotRequired[str],
    attempt: NotRequired[int],
```

1. See [:material-code-brackets: JobRunModeType](./literals.md#jobrunmodetype) 
2. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
## JobRunSummaryTypeDef

```python
# JobRunSummaryTypeDef definition

class JobRunSummaryTypeDef(TypedDict):
    applicationId: str,
    id: str,
    arn: str,
    createdBy: str,
    createdAt: datetime,
    updatedAt: datetime,
    executionRole: str,
    state: JobRunStateType,  # (2)
    stateDetails: str,
    releaseLabel: str,
    name: NotRequired[str],
    mode: NotRequired[JobRunModeType],  # (1)
    type: NotRequired[str],
    attempt: NotRequired[int],
    attemptCreatedAt: NotRequired[datetime],
    attemptUpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: JobRunModeType](./literals.md#jobrunmodetype) 
2. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
## ResourceUtilizationTypeDef

```python
# ResourceUtilizationTypeDef definition

class ResourceUtilizationTypeDef(TypedDict):
    vCPUHour: NotRequired[float],
    memoryGBHour: NotRequired[float],
    storageGBHour: NotRequired[float],
```

## RetryPolicyTypeDef

```python
# RetryPolicyTypeDef definition

class RetryPolicyTypeDef(TypedDict):
    maxAttempts: NotRequired[int],
    maxFailedAttemptsPerHour: NotRequired[int],
```

## TotalResourceUtilizationTypeDef

```python
# TotalResourceUtilizationTypeDef definition

class TotalResourceUtilizationTypeDef(TypedDict):
    vCPUHour: NotRequired[float],
    memoryGBHour: NotRequired[float],
    storageGBHour: NotRequired[float],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    states: NotRequired[Sequence[ApplicationStateType]],  # (1)
```

1. See [:material-code-brackets: ApplicationStateType](./literals.md#applicationstatetype) 
## ListJobRunAttemptsRequestRequestTypeDef

```python
# ListJobRunAttemptsRequestRequestTypeDef definition

class ListJobRunAttemptsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    jobRunId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ManagedPersistenceMonitoringConfigurationTypeDef

```python
# ManagedPersistenceMonitoringConfigurationTypeDef definition

class ManagedPersistenceMonitoringConfigurationTypeDef(TypedDict):
    enabled: NotRequired[bool],
    encryptionKeyArn: NotRequired[str],
```

## PrometheusMonitoringConfigurationTypeDef

```python
# PrometheusMonitoringConfigurationTypeDef definition

class PrometheusMonitoringConfigurationTypeDef(TypedDict):
    remoteWriteUrl: NotRequired[str],
```

## S3MonitoringConfigurationTypeDef

```python
# S3MonitoringConfigurationTypeDef definition

class S3MonitoringConfigurationTypeDef(TypedDict):
    logUri: NotRequired[str],
    encryptionKeyArn: NotRequired[str],
```

## SparkSubmitTypeDef

```python
# SparkSubmitTypeDef definition

class SparkSubmitTypeDef(TypedDict):
    entryPoint: str,
    entryPointArguments: NotRequired[Sequence[str]],
    sparkSubmitParameters: NotRequired[str],
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

## WorkerTypeSpecificationTypeDef

```python
# WorkerTypeSpecificationTypeDef definition

class WorkerTypeSpecificationTypeDef(TypedDict):
    imageConfiguration: NotRequired[ImageConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ImageConfigurationTypeDef](./type_defs.md#imageconfigurationtypedef) 
## CancelJobRunResponseTypeDef

```python
# CancelJobRunResponseTypeDef definition

class CancelJobRunResponseTypeDef(TypedDict):
    applicationId: str,
    jobRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    applicationId: str,
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDashboardForJobRunResponseTypeDef

```python
# GetDashboardForJobRunResponseTypeDef definition

class GetDashboardForJobRunResponseTypeDef(TypedDict):
    url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## StartJobRunResponseTypeDef

```python
# StartJobRunResponseTypeDef definition

class StartJobRunResponseTypeDef(TypedDict):
    applicationId: str,
    jobRunId: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkerTypeSpecificationInputTypeDef

```python
# WorkerTypeSpecificationInputTypeDef definition

class WorkerTypeSpecificationInputTypeDef(TypedDict):
    imageConfiguration: NotRequired[ImageConfigurationInputTypeDef],  # (1)
```

1. See [:material-code-braces: ImageConfigurationInputTypeDef](./type_defs.md#imageconfigurationinputtypedef) 
## InitialCapacityConfigTypeDef

```python
# InitialCapacityConfigTypeDef definition

class InitialCapacityConfigTypeDef(TypedDict):
    workerCount: int,
    workerConfiguration: NotRequired[WorkerResourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WorkerResourceConfigTypeDef](./type_defs.md#workerresourceconfigtypedef) 
## JobDriverOutputTypeDef

```python
# JobDriverOutputTypeDef definition

class JobDriverOutputTypeDef(TypedDict):
    sparkSubmit: NotRequired[SparkSubmitOutputTypeDef],  # (1)
    hive: NotRequired[HiveTypeDef],  # (2)
```

1. See [:material-code-braces: SparkSubmitOutputTypeDef](./type_defs.md#sparksubmitoutputtypedef) 
2. See [:material-code-braces: HiveTypeDef](./type_defs.md#hivetypedef) 
## ListJobRunAttemptsResponseTypeDef

```python
# ListJobRunAttemptsResponseTypeDef definition

class ListJobRunAttemptsResponseTypeDef(TypedDict):
    jobRunAttempts: List[JobRunAttemptSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobRunAttemptSummaryTypeDef](./type_defs.md#jobrunattemptsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobRunsResponseTypeDef

```python
# ListJobRunsResponseTypeDef definition

class ListJobRunsResponseTypeDef(TypedDict):
    jobRuns: List[JobRunSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobRunSummaryTypeDef](./type_defs.md#jobrunsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsRequestPaginateTypeDef

```python
# ListApplicationsRequestPaginateTypeDef definition

class ListApplicationsRequestPaginateTypeDef(TypedDict):
    states: NotRequired[Sequence[ApplicationStateType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ApplicationStateType](./literals.md#applicationstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobRunAttemptsRequestPaginateTypeDef

```python
# ListJobRunAttemptsRequestPaginateTypeDef definition

class ListJobRunAttemptsRequestPaginateTypeDef(TypedDict):
    applicationId: str,
    jobRunId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobRunsRequestPaginateTypeDef

```python
# ListJobRunsRequestPaginateTypeDef definition

class ListJobRunsRequestPaginateTypeDef(TypedDict):
    applicationId: str,
    createdAtAfter: NotRequired[TimestampTypeDef],
    createdAtBefore: NotRequired[TimestampTypeDef],
    states: NotRequired[Sequence[JobRunStateType]],  # (1)
    mode: NotRequired[JobRunModeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
2. See [:material-code-brackets: JobRunModeType](./literals.md#jobrunmodetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobRunsRequestRequestTypeDef

```python
# ListJobRunsRequestRequestTypeDef definition

class ListJobRunsRequestRequestTypeDef(TypedDict):
    applicationId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    createdAtAfter: NotRequired[TimestampTypeDef],
    createdAtBefore: NotRequired[TimestampTypeDef],
    states: NotRequired[Sequence[JobRunStateType]],  # (1)
    mode: NotRequired[JobRunModeType],  # (2)
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
2. See [:material-code-brackets: JobRunModeType](./literals.md#jobrunmodetype) 
## MonitoringConfigurationOutputTypeDef

```python
# MonitoringConfigurationOutputTypeDef definition

class MonitoringConfigurationOutputTypeDef(TypedDict):
    s3MonitoringConfiguration: NotRequired[S3MonitoringConfigurationTypeDef],  # (1)
    managedPersistenceMonitoringConfiguration: NotRequired[ManagedPersistenceMonitoringConfigurationTypeDef],  # (2)
    cloudWatchLoggingConfiguration: NotRequired[CloudWatchLoggingConfigurationOutputTypeDef],  # (3)
    prometheusMonitoringConfiguration: NotRequired[PrometheusMonitoringConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: S3MonitoringConfigurationTypeDef](./type_defs.md#s3monitoringconfigurationtypedef) 
2. See [:material-code-braces: ManagedPersistenceMonitoringConfigurationTypeDef](./type_defs.md#managedpersistencemonitoringconfigurationtypedef) 
3. See [:material-code-braces: CloudWatchLoggingConfigurationOutputTypeDef](./type_defs.md#cloudwatchloggingconfigurationoutputtypedef) 
4. See [:material-code-braces: PrometheusMonitoringConfigurationTypeDef](./type_defs.md#prometheusmonitoringconfigurationtypedef) 
## MonitoringConfigurationTypeDef

```python
# MonitoringConfigurationTypeDef definition

class MonitoringConfigurationTypeDef(TypedDict):
    s3MonitoringConfiguration: NotRequired[S3MonitoringConfigurationTypeDef],  # (1)
    managedPersistenceMonitoringConfiguration: NotRequired[ManagedPersistenceMonitoringConfigurationTypeDef],  # (2)
    cloudWatchLoggingConfiguration: NotRequired[CloudWatchLoggingConfigurationUnionTypeDef],  # (3)
    prometheusMonitoringConfiguration: NotRequired[PrometheusMonitoringConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: S3MonitoringConfigurationTypeDef](./type_defs.md#s3monitoringconfigurationtypedef) 
2. See [:material-code-braces: ManagedPersistenceMonitoringConfigurationTypeDef](./type_defs.md#managedpersistencemonitoringconfigurationtypedef) 
3. See [:material-code-braces: CloudWatchLoggingConfigurationTypeDef](./type_defs.md#cloudwatchloggingconfigurationtypedef) [:material-code-braces: CloudWatchLoggingConfigurationOutputTypeDef](./type_defs.md#cloudwatchloggingconfigurationoutputtypedef) 
4. See [:material-code-braces: PrometheusMonitoringConfigurationTypeDef](./type_defs.md#prometheusmonitoringconfigurationtypedef) 
## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    applicationId: str,
    arn: str,
    releaseLabel: str,
    type: str,
    state: ApplicationStateType,  # (1)
    createdAt: datetime,
    updatedAt: datetime,
    name: NotRequired[str],
    stateDetails: NotRequired[str],
    initialCapacity: NotRequired[Dict[str, InitialCapacityConfigTypeDef]],  # (2)
    maximumCapacity: NotRequired[MaximumAllowedResourcesTypeDef],  # (3)
    tags: NotRequired[Dict[str, str]],
    autoStartConfiguration: NotRequired[AutoStartConfigTypeDef],  # (4)
    autoStopConfiguration: NotRequired[AutoStopConfigTypeDef],  # (5)
    networkConfiguration: NotRequired[NetworkConfigurationOutputTypeDef],  # (6)
    architecture: NotRequired[ArchitectureType],  # (7)
    imageConfiguration: NotRequired[ImageConfigurationTypeDef],  # (8)
    workerTypeSpecifications: NotRequired[Dict[str, WorkerTypeSpecificationTypeDef]],  # (9)
    runtimeConfiguration: NotRequired[List[ConfigurationOutputTypeDef]],  # (10)
    monitoringConfiguration: NotRequired[MonitoringConfigurationOutputTypeDef],  # (11)
    interactiveConfiguration: NotRequired[InteractiveConfigurationTypeDef],  # (12)
    schedulerConfiguration: NotRequired[SchedulerConfigurationTypeDef],  # (13)
```

1. See [:material-code-brackets: ApplicationStateType](./literals.md#applicationstatetype) 
2. See [:material-code-braces: InitialCapacityConfigTypeDef](./type_defs.md#initialcapacityconfigtypedef) 
3. See [:material-code-braces: MaximumAllowedResourcesTypeDef](./type_defs.md#maximumallowedresourcestypedef) 
4. See [:material-code-braces: AutoStartConfigTypeDef](./type_defs.md#autostartconfigtypedef) 
5. See [:material-code-braces: AutoStopConfigTypeDef](./type_defs.md#autostopconfigtypedef) 
6. See [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
7. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
8. See [:material-code-braces: ImageConfigurationTypeDef](./type_defs.md#imageconfigurationtypedef) 
9. See [:material-code-braces: WorkerTypeSpecificationTypeDef](./type_defs.md#workertypespecificationtypedef) 
10. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
11. See [:material-code-braces: MonitoringConfigurationOutputTypeDef](./type_defs.md#monitoringconfigurationoutputtypedef) 
12. See [:material-code-braces: InteractiveConfigurationTypeDef](./type_defs.md#interactiveconfigurationtypedef) 
13. See [:material-code-braces: SchedulerConfigurationTypeDef](./type_defs.md#schedulerconfigurationtypedef) 
## ConfigurationOverridesOutputTypeDef

```python
# ConfigurationOverridesOutputTypeDef definition

class ConfigurationOverridesOutputTypeDef(TypedDict):
    applicationConfiguration: NotRequired[List[ConfigurationOutputTypeDef]],  # (1)
    monitoringConfiguration: NotRequired[MonitoringConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
2. See [:material-code-braces: MonitoringConfigurationOutputTypeDef](./type_defs.md#monitoringconfigurationoutputtypedef) 
## JobDriverTypeDef

```python
# JobDriverTypeDef definition

class JobDriverTypeDef(TypedDict):
    sparkSubmit: NotRequired[SparkSubmitUnionTypeDef],  # (1)
    hive: NotRequired[HiveTypeDef],  # (2)
```

1. See [:material-code-braces: SparkSubmitTypeDef](./type_defs.md#sparksubmittypedef) [:material-code-braces: SparkSubmitOutputTypeDef](./type_defs.md#sparksubmitoutputtypedef) 
2. See [:material-code-braces: HiveTypeDef](./type_defs.md#hivetypedef) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    releaseLabel: str,
    type: str,
    clientToken: str,
    name: NotRequired[str],
    initialCapacity: NotRequired[Mapping[str, InitialCapacityConfigTypeDef]],  # (1)
    maximumCapacity: NotRequired[MaximumAllowedResourcesTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
    autoStartConfiguration: NotRequired[AutoStartConfigTypeDef],  # (3)
    autoStopConfiguration: NotRequired[AutoStopConfigTypeDef],  # (4)
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (5)
    architecture: NotRequired[ArchitectureType],  # (6)
    imageConfiguration: NotRequired[ImageConfigurationInputTypeDef],  # (7)
    workerTypeSpecifications: NotRequired[Mapping[str, WorkerTypeSpecificationInputTypeDef]],  # (8)
    runtimeConfiguration: NotRequired[Sequence[ConfigurationUnionTypeDef]],  # (9)
    monitoringConfiguration: NotRequired[MonitoringConfigurationTypeDef],  # (10)
    interactiveConfiguration: NotRequired[InteractiveConfigurationTypeDef],  # (11)
    schedulerConfiguration: NotRequired[SchedulerConfigurationTypeDef],  # (12)
```

1. See [:material-code-braces: InitialCapacityConfigTypeDef](./type_defs.md#initialcapacityconfigtypedef) 
2. See [:material-code-braces: MaximumAllowedResourcesTypeDef](./type_defs.md#maximumallowedresourcestypedef) 
3. See [:material-code-braces: AutoStartConfigTypeDef](./type_defs.md#autostartconfigtypedef) 
4. See [:material-code-braces: AutoStopConfigTypeDef](./type_defs.md#autostopconfigtypedef) 
5. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
6. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
7. See [:material-code-braces: ImageConfigurationInputTypeDef](./type_defs.md#imageconfigurationinputtypedef) 
8. See [:material-code-braces: WorkerTypeSpecificationInputTypeDef](./type_defs.md#workertypespecificationinputtypedef) 
9. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
10. See [:material-code-braces: MonitoringConfigurationTypeDef](./type_defs.md#monitoringconfigurationtypedef) 
11. See [:material-code-braces: InteractiveConfigurationTypeDef](./type_defs.md#interactiveconfigurationtypedef) 
12. See [:material-code-braces: SchedulerConfigurationTypeDef](./type_defs.md#schedulerconfigurationtypedef) 
## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    applicationId: str,
    clientToken: str,
    initialCapacity: NotRequired[Mapping[str, InitialCapacityConfigTypeDef]],  # (1)
    maximumCapacity: NotRequired[MaximumAllowedResourcesTypeDef],  # (2)
    autoStartConfiguration: NotRequired[AutoStartConfigTypeDef],  # (3)
    autoStopConfiguration: NotRequired[AutoStopConfigTypeDef],  # (4)
    networkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (5)
    architecture: NotRequired[ArchitectureType],  # (6)
    imageConfiguration: NotRequired[ImageConfigurationInputTypeDef],  # (7)
    workerTypeSpecifications: NotRequired[Mapping[str, WorkerTypeSpecificationInputTypeDef]],  # (8)
    interactiveConfiguration: NotRequired[InteractiveConfigurationTypeDef],  # (9)
    releaseLabel: NotRequired[str],
    runtimeConfiguration: NotRequired[Sequence[ConfigurationTypeDef]],  # (10)
    monitoringConfiguration: NotRequired[MonitoringConfigurationTypeDef],  # (11)
    schedulerConfiguration: NotRequired[SchedulerConfigurationTypeDef],  # (12)
```

1. See [:material-code-braces: InitialCapacityConfigTypeDef](./type_defs.md#initialcapacityconfigtypedef) 
2. See [:material-code-braces: MaximumAllowedResourcesTypeDef](./type_defs.md#maximumallowedresourcestypedef) 
3. See [:material-code-braces: AutoStartConfigTypeDef](./type_defs.md#autostartconfigtypedef) 
4. See [:material-code-braces: AutoStopConfigTypeDef](./type_defs.md#autostopconfigtypedef) 
5. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
6. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
7. See [:material-code-braces: ImageConfigurationInputTypeDef](./type_defs.md#imageconfigurationinputtypedef) 
8. See [:material-code-braces: WorkerTypeSpecificationInputTypeDef](./type_defs.md#workertypespecificationinputtypedef) 
9. See [:material-code-braces: InteractiveConfigurationTypeDef](./type_defs.md#interactiveconfigurationtypedef) 
10. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
11. See [:material-code-braces: MonitoringConfigurationTypeDef](./type_defs.md#monitoringconfigurationtypedef) 
12. See [:material-code-braces: SchedulerConfigurationTypeDef](./type_defs.md#schedulerconfigurationtypedef) 
## GetApplicationResponseTypeDef

```python
# GetApplicationResponseTypeDef definition

class GetApplicationResponseTypeDef(TypedDict):
    application: ApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationResponseTypeDef

```python
# UpdateApplicationResponseTypeDef definition

class UpdateApplicationResponseTypeDef(TypedDict):
    application: ApplicationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobRunTypeDef

```python
# JobRunTypeDef definition

class JobRunTypeDef(TypedDict):
    applicationId: str,
    jobRunId: str,
    arn: str,
    createdBy: str,
    createdAt: datetime,
    updatedAt: datetime,
    executionRole: str,
    state: JobRunStateType,  # (1)
    stateDetails: str,
    releaseLabel: str,
    jobDriver: JobDriverOutputTypeDef,  # (3)
    name: NotRequired[str],
    configurationOverrides: NotRequired[ConfigurationOverridesOutputTypeDef],  # (2)
    tags: NotRequired[Dict[str, str]],
    totalResourceUtilization: NotRequired[TotalResourceUtilizationTypeDef],  # (4)
    networkConfiguration: NotRequired[NetworkConfigurationOutputTypeDef],  # (5)
    totalExecutionDurationSeconds: NotRequired[int],
    executionTimeoutMinutes: NotRequired[int],
    billedResourceUtilization: NotRequired[ResourceUtilizationTypeDef],  # (6)
    mode: NotRequired[JobRunModeType],  # (7)
    retryPolicy: NotRequired[RetryPolicyTypeDef],  # (8)
    attempt: NotRequired[int],
    attemptCreatedAt: NotRequired[datetime],
    attemptUpdatedAt: NotRequired[datetime],
    startedAt: NotRequired[datetime],
    endedAt: NotRequired[datetime],
    queuedDurationMilliseconds: NotRequired[int],
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
2. See [:material-code-braces: ConfigurationOverridesOutputTypeDef](./type_defs.md#configurationoverridesoutputtypedef) 
3. See [:material-code-braces: JobDriverOutputTypeDef](./type_defs.md#jobdriveroutputtypedef) 
4. See [:material-code-braces: TotalResourceUtilizationTypeDef](./type_defs.md#totalresourceutilizationtypedef) 
5. See [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
6. See [:material-code-braces: ResourceUtilizationTypeDef](./type_defs.md#resourceutilizationtypedef) 
7. See [:material-code-brackets: JobRunModeType](./literals.md#jobrunmodetype) 
8. See [:material-code-braces: RetryPolicyTypeDef](./type_defs.md#retrypolicytypedef) 
## ConfigurationOverridesTypeDef

```python
# ConfigurationOverridesTypeDef definition

class ConfigurationOverridesTypeDef(TypedDict):
    applicationConfiguration: NotRequired[Sequence[ConfigurationUnionTypeDef]],  # (1)
    monitoringConfiguration: NotRequired[MonitoringConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
2. See [:material-code-braces: MonitoringConfigurationTypeDef](./type_defs.md#monitoringconfigurationtypedef) [:material-code-braces: MonitoringConfigurationOutputTypeDef](./type_defs.md#monitoringconfigurationoutputtypedef) 
## GetJobRunResponseTypeDef

```python
# GetJobRunResponseTypeDef definition

class GetJobRunResponseTypeDef(TypedDict):
    jobRun: JobRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobRunTypeDef](./type_defs.md#jobruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartJobRunRequestRequestTypeDef

```python
# StartJobRunRequestRequestTypeDef definition

class StartJobRunRequestRequestTypeDef(TypedDict):
    applicationId: str,
    clientToken: str,
    executionRoleArn: str,
    jobDriver: NotRequired[JobDriverTypeDef],  # (1)
    configurationOverrides: NotRequired[ConfigurationOverridesTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
    executionTimeoutMinutes: NotRequired[int],
    name: NotRequired[str],
    mode: NotRequired[JobRunModeType],  # (3)
    retryPolicy: NotRequired[RetryPolicyTypeDef],  # (4)
```

1. See [:material-code-braces: JobDriverTypeDef](./type_defs.md#jobdrivertypedef) 
2. See [:material-code-braces: ConfigurationOverridesTypeDef](./type_defs.md#configurationoverridestypedef) 
3. See [:material-code-brackets: JobRunModeType](./literals.md#jobrunmodetype) 
4. See [:material-code-braces: RetryPolicyTypeDef](./type_defs.md#retrypolicytypedef) 
