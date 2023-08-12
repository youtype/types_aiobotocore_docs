# Type definitions

> [Index](../README.md) > [KinesisAnalyticsV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [KinesisAnalyticsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
    type annotations stubs module [types-aiobotocore-kinesisanalyticsv2](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2/).

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


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## CloudWatchLoggingOptionTypeDef

```python
# CloudWatchLoggingOptionTypeDef definition

class CloudWatchLoggingOptionTypeDef(TypedDict):
    LogStreamARN: str,
```

## CloudWatchLoggingOptionDescriptionTypeDef

```python
# CloudWatchLoggingOptionDescriptionTypeDef definition

class CloudWatchLoggingOptionDescriptionTypeDef(TypedDict):
    LogStreamARN: str,
    CloudWatchLoggingOptionId: NotRequired[str],
    RoleARN: NotRequired[str],
```

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

## VpcConfigurationTypeDef

```python
# VpcConfigurationTypeDef definition

class VpcConfigurationTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    SecurityGroupIds: Sequence[str],
```

## VpcConfigurationDescriptionTypeDef

```python
# VpcConfigurationDescriptionTypeDef definition

class VpcConfigurationDescriptionTypeDef(TypedDict):
    VpcConfigurationId: str,
    VpcId: str,
    SubnetIds: List[str],
    SecurityGroupIds: List[str],
```

## ApplicationSnapshotConfigurationDescriptionTypeDef

```python
# ApplicationSnapshotConfigurationDescriptionTypeDef definition

class ApplicationSnapshotConfigurationDescriptionTypeDef(TypedDict):
    SnapshotsEnabled: bool,
```

## ApplicationSnapshotConfigurationTypeDef

```python
# ApplicationSnapshotConfigurationTypeDef definition

class ApplicationSnapshotConfigurationTypeDef(TypedDict):
    SnapshotsEnabled: bool,
```

## ApplicationSnapshotConfigurationUpdateTypeDef

```python
# ApplicationSnapshotConfigurationUpdateTypeDef definition

class ApplicationSnapshotConfigurationUpdateTypeDef(TypedDict):
    SnapshotsEnabledUpdate: bool,
```

## VpcConfigurationUpdateTypeDef

```python
# VpcConfigurationUpdateTypeDef definition

class VpcConfigurationUpdateTypeDef(TypedDict):
    VpcConfigurationId: str,
    SubnetIdUpdates: NotRequired[Sequence[str]],
    SecurityGroupIdUpdates: NotRequired[Sequence[str]],
```

## ApplicationMaintenanceConfigurationDescriptionTypeDef

```python
# ApplicationMaintenanceConfigurationDescriptionTypeDef definition

class ApplicationMaintenanceConfigurationDescriptionTypeDef(TypedDict):
    ApplicationMaintenanceWindowStartTime: str,
    ApplicationMaintenanceWindowEndTime: str,
```

## ApplicationMaintenanceConfigurationUpdateTypeDef

```python
# ApplicationMaintenanceConfigurationUpdateTypeDef definition

class ApplicationMaintenanceConfigurationUpdateTypeDef(TypedDict):
    ApplicationMaintenanceWindowStartTimeUpdate: str,
```

## ApplicationRestoreConfigurationTypeDef

```python
# ApplicationRestoreConfigurationTypeDef definition

class ApplicationRestoreConfigurationTypeDef(TypedDict):
    ApplicationRestoreType: ApplicationRestoreTypeType,  # (1)
    SnapshotName: NotRequired[str],
```

1. See [:material-code-brackets: ApplicationRestoreTypeType](./literals.md#applicationrestoretypetype) 
## ApplicationSummaryTypeDef

```python
# ApplicationSummaryTypeDef definition

class ApplicationSummaryTypeDef(TypedDict):
    ApplicationName: str,
    ApplicationARN: str,
    ApplicationStatus: ApplicationStatusType,  # (1)
    ApplicationVersionId: int,
    RuntimeEnvironment: RuntimeEnvironmentType,  # (2)
    ApplicationMode: NotRequired[ApplicationModeType],  # (3)
```

1. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
2. See [:material-code-brackets: RuntimeEnvironmentType](./literals.md#runtimeenvironmenttype) 
3. See [:material-code-brackets: ApplicationModeType](./literals.md#applicationmodetype) 
## ApplicationVersionSummaryTypeDef

```python
# ApplicationVersionSummaryTypeDef definition

class ApplicationVersionSummaryTypeDef(TypedDict):
    ApplicationVersionId: int,
    ApplicationStatus: ApplicationStatusType,  # (1)
```

1. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
## CSVMappingParametersTypeDef

```python
# CSVMappingParametersTypeDef definition

class CSVMappingParametersTypeDef(TypedDict):
    RecordRowDelimiter: str,
    RecordColumnDelimiter: str,
```

## GlueDataCatalogConfigurationDescriptionTypeDef

```python
# GlueDataCatalogConfigurationDescriptionTypeDef definition

class GlueDataCatalogConfigurationDescriptionTypeDef(TypedDict):
    DatabaseARN: str,
```

## GlueDataCatalogConfigurationTypeDef

```python
# GlueDataCatalogConfigurationTypeDef definition

class GlueDataCatalogConfigurationTypeDef(TypedDict):
    DatabaseARN: str,
```

## GlueDataCatalogConfigurationUpdateTypeDef

```python
# GlueDataCatalogConfigurationUpdateTypeDef definition

class GlueDataCatalogConfigurationUpdateTypeDef(TypedDict):
    DatabaseARNUpdate: str,
```

## CheckpointConfigurationDescriptionTypeDef

```python
# CheckpointConfigurationDescriptionTypeDef definition

class CheckpointConfigurationDescriptionTypeDef(TypedDict):
    ConfigurationType: NotRequired[ConfigurationTypeType],  # (1)
    CheckpointingEnabled: NotRequired[bool],
    CheckpointInterval: NotRequired[int],
    MinPauseBetweenCheckpoints: NotRequired[int],
```

1. See [:material-code-brackets: ConfigurationTypeType](./literals.md#configurationtypetype) 
## CheckpointConfigurationTypeDef

```python
# CheckpointConfigurationTypeDef definition

class CheckpointConfigurationTypeDef(TypedDict):
    ConfigurationType: ConfigurationTypeType,  # (1)
    CheckpointingEnabled: NotRequired[bool],
    CheckpointInterval: NotRequired[int],
    MinPauseBetweenCheckpoints: NotRequired[int],
```

1. See [:material-code-brackets: ConfigurationTypeType](./literals.md#configurationtypetype) 
## CheckpointConfigurationUpdateTypeDef

```python
# CheckpointConfigurationUpdateTypeDef definition

class CheckpointConfigurationUpdateTypeDef(TypedDict):
    ConfigurationTypeUpdate: NotRequired[ConfigurationTypeType],  # (1)
    CheckpointingEnabledUpdate: NotRequired[bool],
    CheckpointIntervalUpdate: NotRequired[int],
    MinPauseBetweenCheckpointsUpdate: NotRequired[int],
```

1. See [:material-code-brackets: ConfigurationTypeType](./literals.md#configurationtypetype) 
## CloudWatchLoggingOptionUpdateTypeDef

```python
# CloudWatchLoggingOptionUpdateTypeDef definition

class CloudWatchLoggingOptionUpdateTypeDef(TypedDict):
    CloudWatchLoggingOptionId: str,
    LogStreamARNUpdate: NotRequired[str],
```

## S3ApplicationCodeLocationDescriptionTypeDef

```python
# S3ApplicationCodeLocationDescriptionTypeDef definition

class S3ApplicationCodeLocationDescriptionTypeDef(TypedDict):
    BucketARN: str,
    FileKey: str,
    ObjectVersion: NotRequired[str],
```

## S3ContentLocationTypeDef

```python
# S3ContentLocationTypeDef definition

class S3ContentLocationTypeDef(TypedDict):
    BucketARN: str,
    FileKey: str,
    ObjectVersion: NotRequired[str],
```

## S3ContentLocationUpdateTypeDef

```python
# S3ContentLocationUpdateTypeDef definition

class S3ContentLocationUpdateTypeDef(TypedDict):
    BucketARNUpdate: NotRequired[str],
    FileKeyUpdate: NotRequired[str],
    ObjectVersionUpdate: NotRequired[str],
```

## CreateApplicationPresignedUrlRequestRequestTypeDef

```python
# CreateApplicationPresignedUrlRequestRequestTypeDef definition

class CreateApplicationPresignedUrlRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    UrlType: UrlTypeType,  # (1)
    SessionExpirationDurationInSeconds: NotRequired[int],
```

1. See [:material-code-brackets: UrlTypeType](./literals.md#urltypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## CreateApplicationSnapshotRequestRequestTypeDef

```python
# CreateApplicationSnapshotRequestRequestTypeDef definition

class CreateApplicationSnapshotRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    SnapshotName: str,
```

## MavenReferenceTypeDef

```python
# MavenReferenceTypeDef definition

class MavenReferenceTypeDef(TypedDict):
    GroupId: str,
    ArtifactId: str,
    Version: str,
```

## DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef

```python
# DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef definition

class DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CloudWatchLoggingOptionId: str,
    CurrentApplicationVersionId: NotRequired[int],
    ConditionalToken: NotRequired[str],
```

## DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef

```python
# DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef definition

class DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CurrentApplicationVersionId: int,
    InputId: str,
```

## DeleteApplicationOutputRequestRequestTypeDef

```python
# DeleteApplicationOutputRequestRequestTypeDef definition

class DeleteApplicationOutputRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CurrentApplicationVersionId: int,
    OutputId: str,
```

## DeleteApplicationReferenceDataSourceRequestRequestTypeDef

```python
# DeleteApplicationReferenceDataSourceRequestRequestTypeDef definition

class DeleteApplicationReferenceDataSourceRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CurrentApplicationVersionId: int,
    ReferenceId: str,
```

## DeleteApplicationVpcConfigurationRequestRequestTypeDef

```python
# DeleteApplicationVpcConfigurationRequestRequestTypeDef definition

class DeleteApplicationVpcConfigurationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    VpcConfigurationId: str,
    CurrentApplicationVersionId: NotRequired[int],
    ConditionalToken: NotRequired[str],
```

## S3ContentBaseLocationDescriptionTypeDef

```python
# S3ContentBaseLocationDescriptionTypeDef definition

class S3ContentBaseLocationDescriptionTypeDef(TypedDict):
    BucketARN: str,
    BasePath: NotRequired[str],
```

## S3ContentBaseLocationTypeDef

```python
# S3ContentBaseLocationTypeDef definition

class S3ContentBaseLocationTypeDef(TypedDict):
    BucketARN: str,
    BasePath: NotRequired[str],
```

## S3ContentBaseLocationUpdateTypeDef

```python
# S3ContentBaseLocationUpdateTypeDef definition

class S3ContentBaseLocationUpdateTypeDef(TypedDict):
    BucketARNUpdate: NotRequired[str],
    BasePathUpdate: NotRequired[str],
```

## DescribeApplicationRequestRequestTypeDef

```python
# DescribeApplicationRequestRequestTypeDef definition

class DescribeApplicationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    IncludeAdditionalDetails: NotRequired[bool],
```

## DescribeApplicationSnapshotRequestRequestTypeDef

```python
# DescribeApplicationSnapshotRequestRequestTypeDef definition

class DescribeApplicationSnapshotRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    SnapshotName: str,
```

## SnapshotDetailsTypeDef

```python
# SnapshotDetailsTypeDef definition

class SnapshotDetailsTypeDef(TypedDict):
    SnapshotName: str,
    SnapshotStatus: SnapshotStatusType,  # (1)
    ApplicationVersionId: int,
    SnapshotCreationTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: SnapshotStatusType](./literals.md#snapshotstatustype) 
## DescribeApplicationVersionRequestRequestTypeDef

```python
# DescribeApplicationVersionRequestRequestTypeDef definition

class DescribeApplicationVersionRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    ApplicationVersionId: int,
```

## DestinationSchemaTypeDef

```python
# DestinationSchemaTypeDef definition

class DestinationSchemaTypeDef(TypedDict):
    RecordFormatType: RecordFormatTypeType,  # (1)
```

1. See [:material-code-brackets: RecordFormatTypeType](./literals.md#recordformattypetype) 
## InputStartingPositionConfigurationTypeDef

```python
# InputStartingPositionConfigurationTypeDef definition

class InputStartingPositionConfigurationTypeDef(TypedDict):
    InputStartingPosition: NotRequired[InputStartingPositionType],  # (1)
```

1. See [:material-code-brackets: InputStartingPositionType](./literals.md#inputstartingpositiontype) 
## S3ConfigurationTypeDef

```python
# S3ConfigurationTypeDef definition

class S3ConfigurationTypeDef(TypedDict):
    BucketARN: str,
    FileKey: str,
```

## PropertyGroupTypeDef

```python
# PropertyGroupTypeDef definition

class PropertyGroupTypeDef(TypedDict):
    PropertyGroupId: str,
    PropertyMap: Mapping[str, str],
```

## MonitoringConfigurationDescriptionTypeDef

```python
# MonitoringConfigurationDescriptionTypeDef definition

class MonitoringConfigurationDescriptionTypeDef(TypedDict):
    ConfigurationType: NotRequired[ConfigurationTypeType],  # (1)
    MetricsLevel: NotRequired[MetricsLevelType],  # (2)
    LogLevel: NotRequired[LogLevelType],  # (3)
```

1. See [:material-code-brackets: ConfigurationTypeType](./literals.md#configurationtypetype) 
2. See [:material-code-brackets: MetricsLevelType](./literals.md#metricsleveltype) 
3. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## ParallelismConfigurationDescriptionTypeDef

```python
# ParallelismConfigurationDescriptionTypeDef definition

class ParallelismConfigurationDescriptionTypeDef(TypedDict):
    ConfigurationType: NotRequired[ConfigurationTypeType],  # (1)
    Parallelism: NotRequired[int],
    ParallelismPerKPU: NotRequired[int],
    CurrentParallelism: NotRequired[int],
    AutoScalingEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: ConfigurationTypeType](./literals.md#configurationtypetype) 
## MonitoringConfigurationTypeDef

```python
# MonitoringConfigurationTypeDef definition

class MonitoringConfigurationTypeDef(TypedDict):
    ConfigurationType: ConfigurationTypeType,  # (1)
    MetricsLevel: NotRequired[MetricsLevelType],  # (2)
    LogLevel: NotRequired[LogLevelType],  # (3)
```

1. See [:material-code-brackets: ConfigurationTypeType](./literals.md#configurationtypetype) 
2. See [:material-code-brackets: MetricsLevelType](./literals.md#metricsleveltype) 
3. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## ParallelismConfigurationTypeDef

```python
# ParallelismConfigurationTypeDef definition

class ParallelismConfigurationTypeDef(TypedDict):
    ConfigurationType: ConfigurationTypeType,  # (1)
    Parallelism: NotRequired[int],
    ParallelismPerKPU: NotRequired[int],
    AutoScalingEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: ConfigurationTypeType](./literals.md#configurationtypetype) 
## MonitoringConfigurationUpdateTypeDef

```python
# MonitoringConfigurationUpdateTypeDef definition

class MonitoringConfigurationUpdateTypeDef(TypedDict):
    ConfigurationTypeUpdate: NotRequired[ConfigurationTypeType],  # (1)
    MetricsLevelUpdate: NotRequired[MetricsLevelType],  # (2)
    LogLevelUpdate: NotRequired[LogLevelType],  # (3)
```

1. See [:material-code-brackets: ConfigurationTypeType](./literals.md#configurationtypetype) 
2. See [:material-code-brackets: MetricsLevelType](./literals.md#metricsleveltype) 
3. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## ParallelismConfigurationUpdateTypeDef

```python
# ParallelismConfigurationUpdateTypeDef definition

class ParallelismConfigurationUpdateTypeDef(TypedDict):
    ConfigurationTypeUpdate: NotRequired[ConfigurationTypeType],  # (1)
    ParallelismUpdate: NotRequired[int],
    ParallelismPerKPUUpdate: NotRequired[int],
    AutoScalingEnabledUpdate: NotRequired[bool],
```

1. See [:material-code-brackets: ConfigurationTypeType](./literals.md#configurationtypetype) 
## FlinkRunConfigurationTypeDef

```python
# FlinkRunConfigurationTypeDef definition

class FlinkRunConfigurationTypeDef(TypedDict):
    AllowNonRestoredState: NotRequired[bool],
```

## InputParallelismTypeDef

```python
# InputParallelismTypeDef definition

class InputParallelismTypeDef(TypedDict):
    Count: NotRequired[int],
```

## KinesisFirehoseInputDescriptionTypeDef

```python
# KinesisFirehoseInputDescriptionTypeDef definition

class KinesisFirehoseInputDescriptionTypeDef(TypedDict):
    ResourceARN: str,
    RoleARN: NotRequired[str],
```

## KinesisStreamsInputDescriptionTypeDef

```python
# KinesisStreamsInputDescriptionTypeDef definition

class KinesisStreamsInputDescriptionTypeDef(TypedDict):
    ResourceARN: str,
    RoleARN: NotRequired[str],
```

## InputLambdaProcessorDescriptionTypeDef

```python
# InputLambdaProcessorDescriptionTypeDef definition

class InputLambdaProcessorDescriptionTypeDef(TypedDict):
    ResourceARN: str,
    RoleARN: NotRequired[str],
```

## InputLambdaProcessorTypeDef

```python
# InputLambdaProcessorTypeDef definition

class InputLambdaProcessorTypeDef(TypedDict):
    ResourceARN: str,
```

## InputLambdaProcessorUpdateTypeDef

```python
# InputLambdaProcessorUpdateTypeDef definition

class InputLambdaProcessorUpdateTypeDef(TypedDict):
    ResourceARNUpdate: str,
```

## InputParallelismUpdateTypeDef

```python
# InputParallelismUpdateTypeDef definition

class InputParallelismUpdateTypeDef(TypedDict):
    CountUpdate: int,
```

## RecordColumnTypeDef

```python
# RecordColumnTypeDef definition

class RecordColumnTypeDef(TypedDict):
    Name: str,
    SqlType: str,
    Mapping: NotRequired[str],
```

## KinesisFirehoseInputTypeDef

```python
# KinesisFirehoseInputTypeDef definition

class KinesisFirehoseInputTypeDef(TypedDict):
    ResourceARN: str,
```

## KinesisStreamsInputTypeDef

```python
# KinesisStreamsInputTypeDef definition

class KinesisStreamsInputTypeDef(TypedDict):
    ResourceARN: str,
```

## KinesisFirehoseInputUpdateTypeDef

```python
# KinesisFirehoseInputUpdateTypeDef definition

class KinesisFirehoseInputUpdateTypeDef(TypedDict):
    ResourceARNUpdate: str,
```

## KinesisStreamsInputUpdateTypeDef

```python
# KinesisStreamsInputUpdateTypeDef definition

class KinesisStreamsInputUpdateTypeDef(TypedDict):
    ResourceARNUpdate: str,
```

## JSONMappingParametersTypeDef

```python
# JSONMappingParametersTypeDef definition

class JSONMappingParametersTypeDef(TypedDict):
    RecordRowPath: str,
```

## KinesisFirehoseOutputDescriptionTypeDef

```python
# KinesisFirehoseOutputDescriptionTypeDef definition

class KinesisFirehoseOutputDescriptionTypeDef(TypedDict):
    ResourceARN: str,
    RoleARN: NotRequired[str],
```

## KinesisFirehoseOutputTypeDef

```python
# KinesisFirehoseOutputTypeDef definition

class KinesisFirehoseOutputTypeDef(TypedDict):
    ResourceARN: str,
```

## KinesisFirehoseOutputUpdateTypeDef

```python
# KinesisFirehoseOutputUpdateTypeDef definition

class KinesisFirehoseOutputUpdateTypeDef(TypedDict):
    ResourceARNUpdate: str,
```

## KinesisStreamsOutputDescriptionTypeDef

```python
# KinesisStreamsOutputDescriptionTypeDef definition

class KinesisStreamsOutputDescriptionTypeDef(TypedDict):
    ResourceARN: str,
    RoleARN: NotRequired[str],
```

## KinesisStreamsOutputTypeDef

```python
# KinesisStreamsOutputTypeDef definition

class KinesisStreamsOutputTypeDef(TypedDict):
    ResourceARN: str,
```

## KinesisStreamsOutputUpdateTypeDef

```python
# KinesisStreamsOutputUpdateTypeDef definition

class KinesisStreamsOutputUpdateTypeDef(TypedDict):
    ResourceARNUpdate: str,
```

## LambdaOutputDescriptionTypeDef

```python
# LambdaOutputDescriptionTypeDef definition

class LambdaOutputDescriptionTypeDef(TypedDict):
    ResourceARN: str,
    RoleARN: NotRequired[str],
```

## LambdaOutputTypeDef

```python
# LambdaOutputTypeDef definition

class LambdaOutputTypeDef(TypedDict):
    ResourceARN: str,
```

## LambdaOutputUpdateTypeDef

```python
# LambdaOutputUpdateTypeDef definition

class LambdaOutputUpdateTypeDef(TypedDict):
    ResourceARNUpdate: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListApplicationSnapshotsRequestRequestTypeDef

```python
# ListApplicationSnapshotsRequestRequestTypeDef definition

class ListApplicationSnapshotsRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListApplicationVersionsRequestRequestTypeDef

```python
# ListApplicationVersionsRequestRequestTypeDef definition

class ListApplicationVersionsRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## S3ReferenceDataSourceDescriptionTypeDef

```python
# S3ReferenceDataSourceDescriptionTypeDef definition

class S3ReferenceDataSourceDescriptionTypeDef(TypedDict):
    BucketARN: str,
    FileKey: str,
    ReferenceRoleARN: NotRequired[str],
```

## S3ReferenceDataSourceTypeDef

```python
# S3ReferenceDataSourceTypeDef definition

class S3ReferenceDataSourceTypeDef(TypedDict):
    BucketARN: NotRequired[str],
    FileKey: NotRequired[str],
```

## S3ReferenceDataSourceUpdateTypeDef

```python
# S3ReferenceDataSourceUpdateTypeDef definition

class S3ReferenceDataSourceUpdateTypeDef(TypedDict):
    BucketARNUpdate: NotRequired[str],
    FileKeyUpdate: NotRequired[str],
```

## RollbackApplicationRequestRequestTypeDef

```python
# RollbackApplicationRequestRequestTypeDef definition

class RollbackApplicationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CurrentApplicationVersionId: int,
```

## StopApplicationRequestRequestTypeDef

```python
# StopApplicationRequestRequestTypeDef definition

class StopApplicationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    Force: NotRequired[bool],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## ZeppelinMonitoringConfigurationDescriptionTypeDef

```python
# ZeppelinMonitoringConfigurationDescriptionTypeDef definition

class ZeppelinMonitoringConfigurationDescriptionTypeDef(TypedDict):
    LogLevel: NotRequired[LogLevelType],  # (1)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## ZeppelinMonitoringConfigurationTypeDef

```python
# ZeppelinMonitoringConfigurationTypeDef definition

class ZeppelinMonitoringConfigurationTypeDef(TypedDict):
    LogLevel: LogLevelType,  # (1)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## ZeppelinMonitoringConfigurationUpdateTypeDef

```python
# ZeppelinMonitoringConfigurationUpdateTypeDef definition

class ZeppelinMonitoringConfigurationUpdateTypeDef(TypedDict):
    LogLevelUpdate: LogLevelType,  # (1)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
## AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef

```python
# AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef definition

class AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CloudWatchLoggingOption: CloudWatchLoggingOptionTypeDef,  # (1)
    CurrentApplicationVersionId: NotRequired[int],
    ConditionalToken: NotRequired[str],
```

1. See [:material-code-braces: CloudWatchLoggingOptionTypeDef](./type_defs.md#cloudwatchloggingoptiontypedef) 
## AddApplicationCloudWatchLoggingOptionResponseTypeDef

```python
# AddApplicationCloudWatchLoggingOptionResponseTypeDef definition

class AddApplicationCloudWatchLoggingOptionResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    CloudWatchLoggingOptionDescriptions: List[CloudWatchLoggingOptionDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudWatchLoggingOptionDescriptionTypeDef](./type_defs.md#cloudwatchloggingoptiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationPresignedUrlResponseTypeDef

```python
# CreateApplicationPresignedUrlResponseTypeDef definition

class CreateApplicationPresignedUrlResponseTypeDef(TypedDict):
    AuthorizedUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApplicationCloudWatchLoggingOptionResponseTypeDef

```python
# DeleteApplicationCloudWatchLoggingOptionResponseTypeDef definition

class DeleteApplicationCloudWatchLoggingOptionResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    CloudWatchLoggingOptionDescriptions: List[CloudWatchLoggingOptionDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudWatchLoggingOptionDescriptionTypeDef](./type_defs.md#cloudwatchloggingoptiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApplicationInputProcessingConfigurationResponseTypeDef

```python
# DeleteApplicationInputProcessingConfigurationResponseTypeDef definition

class DeleteApplicationInputProcessingConfigurationResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApplicationOutputResponseTypeDef

```python
# DeleteApplicationOutputResponseTypeDef definition

class DeleteApplicationOutputResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApplicationReferenceDataSourceResponseTypeDef

```python
# DeleteApplicationReferenceDataSourceResponseTypeDef definition

class DeleteApplicationReferenceDataSourceResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApplicationVpcConfigurationResponseTypeDef

```python
# DeleteApplicationVpcConfigurationResponseTypeDef definition

class DeleteApplicationVpcConfigurationResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddApplicationVpcConfigurationRequestRequestTypeDef

```python
# AddApplicationVpcConfigurationRequestRequestTypeDef definition

class AddApplicationVpcConfigurationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    VpcConfiguration: VpcConfigurationTypeDef,  # (1)
    CurrentApplicationVersionId: NotRequired[int],
    ConditionalToken: NotRequired[str],
```

1. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
## AddApplicationVpcConfigurationResponseTypeDef

```python
# AddApplicationVpcConfigurationResponseTypeDef definition

class AddApplicationVpcConfigurationResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    VpcConfigurationDescription: VpcConfigurationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcConfigurationDescriptionTypeDef](./type_defs.md#vpcconfigurationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationMaintenanceConfigurationResponseTypeDef

```python
# UpdateApplicationMaintenanceConfigurationResponseTypeDef definition

class UpdateApplicationMaintenanceConfigurationResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationMaintenanceConfigurationDescription: ApplicationMaintenanceConfigurationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationMaintenanceConfigurationDescriptionTypeDef](./type_defs.md#applicationmaintenanceconfigurationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef

```python
# UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef definition

class UpdateApplicationMaintenanceConfigurationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    ApplicationMaintenanceConfigurationUpdate: ApplicationMaintenanceConfigurationUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: ApplicationMaintenanceConfigurationUpdateTypeDef](./type_defs.md#applicationmaintenanceconfigurationupdatetypedef) 
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    ApplicationSummaries: List[ApplicationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationVersionsResponseTypeDef

```python
# ListApplicationVersionsResponseTypeDef definition

class ListApplicationVersionsResponseTypeDef(TypedDict):
    ApplicationVersionSummaries: List[ApplicationVersionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationVersionSummaryTypeDef](./type_defs.md#applicationversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CatalogConfigurationDescriptionTypeDef

```python
# CatalogConfigurationDescriptionTypeDef definition

class CatalogConfigurationDescriptionTypeDef(TypedDict):
    GlueDataCatalogConfigurationDescription: GlueDataCatalogConfigurationDescriptionTypeDef,  # (1)
```

1. See [:material-code-braces: GlueDataCatalogConfigurationDescriptionTypeDef](./type_defs.md#gluedatacatalogconfigurationdescriptiontypedef) 
## CatalogConfigurationTypeDef

```python
# CatalogConfigurationTypeDef definition

class CatalogConfigurationTypeDef(TypedDict):
    GlueDataCatalogConfiguration: GlueDataCatalogConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: GlueDataCatalogConfigurationTypeDef](./type_defs.md#gluedatacatalogconfigurationtypedef) 
## CatalogConfigurationUpdateTypeDef

```python
# CatalogConfigurationUpdateTypeDef definition

class CatalogConfigurationUpdateTypeDef(TypedDict):
    GlueDataCatalogConfigurationUpdate: GlueDataCatalogConfigurationUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: GlueDataCatalogConfigurationUpdateTypeDef](./type_defs.md#gluedatacatalogconfigurationupdatetypedef) 
## CodeContentDescriptionTypeDef

```python
# CodeContentDescriptionTypeDef definition

class CodeContentDescriptionTypeDef(TypedDict):
    TextContent: NotRequired[str],
    CodeMD5: NotRequired[str],
    CodeSize: NotRequired[int],
    S3ApplicationCodeLocationDescription: NotRequired[S3ApplicationCodeLocationDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: S3ApplicationCodeLocationDescriptionTypeDef](./type_defs.md#s3applicationcodelocationdescriptiontypedef) 
## CodeContentTypeDef

```python
# CodeContentTypeDef definition

class CodeContentTypeDef(TypedDict):
    TextContent: NotRequired[str],
    ZipFileContent: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    S3ContentLocation: NotRequired[S3ContentLocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3ContentLocationTypeDef](./type_defs.md#s3contentlocationtypedef) 
## CodeContentUpdateTypeDef

```python
# CodeContentUpdateTypeDef definition

class CodeContentUpdateTypeDef(TypedDict):
    TextContentUpdate: NotRequired[str],
    ZipFileContentUpdate: NotRequired[Union[str, bytes, IO[Any], StreamingBody]],
    S3ContentLocationUpdate: NotRequired[S3ContentLocationUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: S3ContentLocationUpdateTypeDef](./type_defs.md#s3contentlocationupdatetypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CustomArtifactConfigurationDescriptionTypeDef

```python
# CustomArtifactConfigurationDescriptionTypeDef definition

class CustomArtifactConfigurationDescriptionTypeDef(TypedDict):
    ArtifactType: NotRequired[ArtifactTypeType],  # (1)
    S3ContentLocationDescription: NotRequired[S3ContentLocationTypeDef],  # (2)
    MavenReferenceDescription: NotRequired[MavenReferenceTypeDef],  # (3)
```

1. See [:material-code-brackets: ArtifactTypeType](./literals.md#artifacttypetype) 
2. See [:material-code-braces: S3ContentLocationTypeDef](./type_defs.md#s3contentlocationtypedef) 
3. See [:material-code-braces: MavenReferenceTypeDef](./type_defs.md#mavenreferencetypedef) 
## CustomArtifactConfigurationTypeDef

```python
# CustomArtifactConfigurationTypeDef definition

class CustomArtifactConfigurationTypeDef(TypedDict):
    ArtifactType: ArtifactTypeType,  # (1)
    S3ContentLocation: NotRequired[S3ContentLocationTypeDef],  # (2)
    MavenReference: NotRequired[MavenReferenceTypeDef],  # (3)
```

1. See [:material-code-brackets: ArtifactTypeType](./literals.md#artifacttypetype) 
2. See [:material-code-braces: S3ContentLocationTypeDef](./type_defs.md#s3contentlocationtypedef) 
3. See [:material-code-braces: MavenReferenceTypeDef](./type_defs.md#mavenreferencetypedef) 
## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CreateTimestamp: Union[datetime, str],
```

## DeleteApplicationSnapshotRequestRequestTypeDef

```python
# DeleteApplicationSnapshotRequestRequestTypeDef definition

class DeleteApplicationSnapshotRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    SnapshotName: str,
    SnapshotCreationTimestamp: Union[datetime, str],
```

## DeployAsApplicationConfigurationDescriptionTypeDef

```python
# DeployAsApplicationConfigurationDescriptionTypeDef definition

class DeployAsApplicationConfigurationDescriptionTypeDef(TypedDict):
    S3ContentLocationDescription: S3ContentBaseLocationDescriptionTypeDef,  # (1)
```

1. See [:material-code-braces: S3ContentBaseLocationDescriptionTypeDef](./type_defs.md#s3contentbaselocationdescriptiontypedef) 
## DeployAsApplicationConfigurationTypeDef

```python
# DeployAsApplicationConfigurationTypeDef definition

class DeployAsApplicationConfigurationTypeDef(TypedDict):
    S3ContentLocation: S3ContentBaseLocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3ContentBaseLocationTypeDef](./type_defs.md#s3contentbaselocationtypedef) 
## DeployAsApplicationConfigurationUpdateTypeDef

```python
# DeployAsApplicationConfigurationUpdateTypeDef definition

class DeployAsApplicationConfigurationUpdateTypeDef(TypedDict):
    S3ContentLocationUpdate: NotRequired[S3ContentBaseLocationUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: S3ContentBaseLocationUpdateTypeDef](./type_defs.md#s3contentbaselocationupdatetypedef) 
## DescribeApplicationSnapshotResponseTypeDef

```python
# DescribeApplicationSnapshotResponseTypeDef definition

class DescribeApplicationSnapshotResponseTypeDef(TypedDict):
    SnapshotDetails: SnapshotDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotDetailsTypeDef](./type_defs.md#snapshotdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationSnapshotsResponseTypeDef

```python
# ListApplicationSnapshotsResponseTypeDef definition

class ListApplicationSnapshotsResponseTypeDef(TypedDict):
    SnapshotSummaries: List[SnapshotDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotDetailsTypeDef](./type_defs.md#snapshotdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SqlRunConfigurationTypeDef

```python
# SqlRunConfigurationTypeDef definition

class SqlRunConfigurationTypeDef(TypedDict):
    InputId: str,
    InputStartingPositionConfiguration: InputStartingPositionConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: InputStartingPositionConfigurationTypeDef](./type_defs.md#inputstartingpositionconfigurationtypedef) 
## EnvironmentPropertiesTypeDef

```python
# EnvironmentPropertiesTypeDef definition

class EnvironmentPropertiesTypeDef(TypedDict):
    PropertyGroups: Sequence[PropertyGroupTypeDef],  # (1)
```

1. See [:material-code-braces: PropertyGroupTypeDef](./type_defs.md#propertygrouptypedef) 
## EnvironmentPropertyDescriptionsTypeDef

```python
# EnvironmentPropertyDescriptionsTypeDef definition

class EnvironmentPropertyDescriptionsTypeDef(TypedDict):
    PropertyGroupDescriptions: NotRequired[List[PropertyGroupTypeDef]],  # (1)
```

1. See [:material-code-braces: PropertyGroupTypeDef](./type_defs.md#propertygrouptypedef) 
## EnvironmentPropertyUpdatesTypeDef

```python
# EnvironmentPropertyUpdatesTypeDef definition

class EnvironmentPropertyUpdatesTypeDef(TypedDict):
    PropertyGroups: Sequence[PropertyGroupTypeDef],  # (1)
```

1. See [:material-code-braces: PropertyGroupTypeDef](./type_defs.md#propertygrouptypedef) 
## FlinkApplicationConfigurationDescriptionTypeDef

```python
# FlinkApplicationConfigurationDescriptionTypeDef definition

class FlinkApplicationConfigurationDescriptionTypeDef(TypedDict):
    CheckpointConfigurationDescription: NotRequired[CheckpointConfigurationDescriptionTypeDef],  # (1)
    MonitoringConfigurationDescription: NotRequired[MonitoringConfigurationDescriptionTypeDef],  # (2)
    ParallelismConfigurationDescription: NotRequired[ParallelismConfigurationDescriptionTypeDef],  # (3)
    JobPlanDescription: NotRequired[str],
```

1. See [:material-code-braces: CheckpointConfigurationDescriptionTypeDef](./type_defs.md#checkpointconfigurationdescriptiontypedef) 
2. See [:material-code-braces: MonitoringConfigurationDescriptionTypeDef](./type_defs.md#monitoringconfigurationdescriptiontypedef) 
3. See [:material-code-braces: ParallelismConfigurationDescriptionTypeDef](./type_defs.md#parallelismconfigurationdescriptiontypedef) 
## FlinkApplicationConfigurationTypeDef

```python
# FlinkApplicationConfigurationTypeDef definition

class FlinkApplicationConfigurationTypeDef(TypedDict):
    CheckpointConfiguration: NotRequired[CheckpointConfigurationTypeDef],  # (1)
    MonitoringConfiguration: NotRequired[MonitoringConfigurationTypeDef],  # (2)
    ParallelismConfiguration: NotRequired[ParallelismConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: CheckpointConfigurationTypeDef](./type_defs.md#checkpointconfigurationtypedef) 
2. See [:material-code-braces: MonitoringConfigurationTypeDef](./type_defs.md#monitoringconfigurationtypedef) 
3. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
## FlinkApplicationConfigurationUpdateTypeDef

```python
# FlinkApplicationConfigurationUpdateTypeDef definition

class FlinkApplicationConfigurationUpdateTypeDef(TypedDict):
    CheckpointConfigurationUpdate: NotRequired[CheckpointConfigurationUpdateTypeDef],  # (1)
    MonitoringConfigurationUpdate: NotRequired[MonitoringConfigurationUpdateTypeDef],  # (2)
    ParallelismConfigurationUpdate: NotRequired[ParallelismConfigurationUpdateTypeDef],  # (3)
```

1. See [:material-code-braces: CheckpointConfigurationUpdateTypeDef](./type_defs.md#checkpointconfigurationupdatetypedef) 
2. See [:material-code-braces: MonitoringConfigurationUpdateTypeDef](./type_defs.md#monitoringconfigurationupdatetypedef) 
3. See [:material-code-braces: ParallelismConfigurationUpdateTypeDef](./type_defs.md#parallelismconfigurationupdatetypedef) 
## RunConfigurationDescriptionTypeDef

```python
# RunConfigurationDescriptionTypeDef definition

class RunConfigurationDescriptionTypeDef(TypedDict):
    ApplicationRestoreConfigurationDescription: NotRequired[ApplicationRestoreConfigurationTypeDef],  # (1)
    FlinkRunConfigurationDescription: NotRequired[FlinkRunConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ApplicationRestoreConfigurationTypeDef](./type_defs.md#applicationrestoreconfigurationtypedef) 
2. See [:material-code-braces: FlinkRunConfigurationTypeDef](./type_defs.md#flinkrunconfigurationtypedef) 
## RunConfigurationUpdateTypeDef

```python
# RunConfigurationUpdateTypeDef definition

class RunConfigurationUpdateTypeDef(TypedDict):
    FlinkRunConfiguration: NotRequired[FlinkRunConfigurationTypeDef],  # (1)
    ApplicationRestoreConfiguration: NotRequired[ApplicationRestoreConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FlinkRunConfigurationTypeDef](./type_defs.md#flinkrunconfigurationtypedef) 
2. See [:material-code-braces: ApplicationRestoreConfigurationTypeDef](./type_defs.md#applicationrestoreconfigurationtypedef) 
## InputProcessingConfigurationDescriptionTypeDef

```python
# InputProcessingConfigurationDescriptionTypeDef definition

class InputProcessingConfigurationDescriptionTypeDef(TypedDict):
    InputLambdaProcessorDescription: NotRequired[InputLambdaProcessorDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: InputLambdaProcessorDescriptionTypeDef](./type_defs.md#inputlambdaprocessordescriptiontypedef) 
## InputProcessingConfigurationTypeDef

```python
# InputProcessingConfigurationTypeDef definition

class InputProcessingConfigurationTypeDef(TypedDict):
    InputLambdaProcessor: InputLambdaProcessorTypeDef,  # (1)
```

1. See [:material-code-braces: InputLambdaProcessorTypeDef](./type_defs.md#inputlambdaprocessortypedef) 
## InputProcessingConfigurationUpdateTypeDef

```python
# InputProcessingConfigurationUpdateTypeDef definition

class InputProcessingConfigurationUpdateTypeDef(TypedDict):
    InputLambdaProcessorUpdate: InputLambdaProcessorUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: InputLambdaProcessorUpdateTypeDef](./type_defs.md#inputlambdaprocessorupdatetypedef) 
## MappingParametersTypeDef

```python
# MappingParametersTypeDef definition

class MappingParametersTypeDef(TypedDict):
    JSONMappingParameters: NotRequired[JSONMappingParametersTypeDef],  # (1)
    CSVMappingParameters: NotRequired[CSVMappingParametersTypeDef],  # (2)
```

1. See [:material-code-braces: JSONMappingParametersTypeDef](./type_defs.md#jsonmappingparameterstypedef) 
2. See [:material-code-braces: CSVMappingParametersTypeDef](./type_defs.md#csvmappingparameterstypedef) 
## OutputDescriptionTypeDef

```python
# OutputDescriptionTypeDef definition

class OutputDescriptionTypeDef(TypedDict):
    OutputId: NotRequired[str],
    Name: NotRequired[str],
    KinesisStreamsOutputDescription: NotRequired[KinesisStreamsOutputDescriptionTypeDef],  # (1)
    KinesisFirehoseOutputDescription: NotRequired[KinesisFirehoseOutputDescriptionTypeDef],  # (2)
    LambdaOutputDescription: NotRequired[LambdaOutputDescriptionTypeDef],  # (3)
    DestinationSchema: NotRequired[DestinationSchemaTypeDef],  # (4)
```

1. See [:material-code-braces: KinesisStreamsOutputDescriptionTypeDef](./type_defs.md#kinesisstreamsoutputdescriptiontypedef) 
2. See [:material-code-braces: KinesisFirehoseOutputDescriptionTypeDef](./type_defs.md#kinesisfirehoseoutputdescriptiontypedef) 
3. See [:material-code-braces: LambdaOutputDescriptionTypeDef](./type_defs.md#lambdaoutputdescriptiontypedef) 
4. See [:material-code-braces: DestinationSchemaTypeDef](./type_defs.md#destinationschematypedef) 
## OutputTypeDef

```python
# OutputTypeDef definition

class OutputTypeDef(TypedDict):
    Name: str,
    DestinationSchema: DestinationSchemaTypeDef,  # (4)
    KinesisStreamsOutput: NotRequired[KinesisStreamsOutputTypeDef],  # (1)
    KinesisFirehoseOutput: NotRequired[KinesisFirehoseOutputTypeDef],  # (2)
    LambdaOutput: NotRequired[LambdaOutputTypeDef],  # (3)
```

1. See [:material-code-braces: KinesisStreamsOutputTypeDef](./type_defs.md#kinesisstreamsoutputtypedef) 
2. See [:material-code-braces: KinesisFirehoseOutputTypeDef](./type_defs.md#kinesisfirehoseoutputtypedef) 
3. See [:material-code-braces: LambdaOutputTypeDef](./type_defs.md#lambdaoutputtypedef) 
4. See [:material-code-braces: DestinationSchemaTypeDef](./type_defs.md#destinationschematypedef) 
## OutputUpdateTypeDef

```python
# OutputUpdateTypeDef definition

class OutputUpdateTypeDef(TypedDict):
    OutputId: str,
    NameUpdate: NotRequired[str],
    KinesisStreamsOutputUpdate: NotRequired[KinesisStreamsOutputUpdateTypeDef],  # (1)
    KinesisFirehoseOutputUpdate: NotRequired[KinesisFirehoseOutputUpdateTypeDef],  # (2)
    LambdaOutputUpdate: NotRequired[LambdaOutputUpdateTypeDef],  # (3)
    DestinationSchemaUpdate: NotRequired[DestinationSchemaTypeDef],  # (4)
```

1. See [:material-code-braces: KinesisStreamsOutputUpdateTypeDef](./type_defs.md#kinesisstreamsoutputupdatetypedef) 
2. See [:material-code-braces: KinesisFirehoseOutputUpdateTypeDef](./type_defs.md#kinesisfirehoseoutputupdatetypedef) 
3. See [:material-code-braces: LambdaOutputUpdateTypeDef](./type_defs.md#lambdaoutputupdatetypedef) 
4. See [:material-code-braces: DestinationSchemaTypeDef](./type_defs.md#destinationschematypedef) 
## ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef

```python
# ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef definition

class ListApplicationSnapshotsRequestListApplicationSnapshotsPaginateTypeDef(TypedDict):
    ApplicationName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationsRequestListApplicationsPaginateTypeDef

```python
# ListApplicationsRequestListApplicationsPaginateTypeDef definition

class ListApplicationsRequestListApplicationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ApplicationCodeConfigurationDescriptionTypeDef

```python
# ApplicationCodeConfigurationDescriptionTypeDef definition

class ApplicationCodeConfigurationDescriptionTypeDef(TypedDict):
    CodeContentType: CodeContentTypeType,  # (1)
    CodeContentDescription: NotRequired[CodeContentDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: CodeContentTypeType](./literals.md#codecontenttypetype) 
2. See [:material-code-braces: CodeContentDescriptionTypeDef](./type_defs.md#codecontentdescriptiontypedef) 
## ApplicationCodeConfigurationTypeDef

```python
# ApplicationCodeConfigurationTypeDef definition

class ApplicationCodeConfigurationTypeDef(TypedDict):
    CodeContentType: CodeContentTypeType,  # (2)
    CodeContent: NotRequired[CodeContentTypeDef],  # (1)
```

1. See [:material-code-braces: CodeContentTypeDef](./type_defs.md#codecontenttypedef) 
2. See [:material-code-brackets: CodeContentTypeType](./literals.md#codecontenttypetype) 
## ApplicationCodeConfigurationUpdateTypeDef

```python
# ApplicationCodeConfigurationUpdateTypeDef definition

class ApplicationCodeConfigurationUpdateTypeDef(TypedDict):
    CodeContentTypeUpdate: NotRequired[CodeContentTypeType],  # (1)
    CodeContentUpdate: NotRequired[CodeContentUpdateTypeDef],  # (2)
```

1. See [:material-code-brackets: CodeContentTypeType](./literals.md#codecontenttypetype) 
2. See [:material-code-braces: CodeContentUpdateTypeDef](./type_defs.md#codecontentupdatetypedef) 
## ZeppelinApplicationConfigurationDescriptionTypeDef

```python
# ZeppelinApplicationConfigurationDescriptionTypeDef definition

class ZeppelinApplicationConfigurationDescriptionTypeDef(TypedDict):
    MonitoringConfigurationDescription: ZeppelinMonitoringConfigurationDescriptionTypeDef,  # (1)
    CatalogConfigurationDescription: NotRequired[CatalogConfigurationDescriptionTypeDef],  # (2)
    DeployAsApplicationConfigurationDescription: NotRequired[DeployAsApplicationConfigurationDescriptionTypeDef],  # (3)
    CustomArtifactsConfigurationDescription: NotRequired[List[CustomArtifactConfigurationDescriptionTypeDef]],  # (4)
```

1. See [:material-code-braces: ZeppelinMonitoringConfigurationDescriptionTypeDef](./type_defs.md#zeppelinmonitoringconfigurationdescriptiontypedef) 
2. See [:material-code-braces: CatalogConfigurationDescriptionTypeDef](./type_defs.md#catalogconfigurationdescriptiontypedef) 
3. See [:material-code-braces: DeployAsApplicationConfigurationDescriptionTypeDef](./type_defs.md#deployasapplicationconfigurationdescriptiontypedef) 
4. See [:material-code-braces: CustomArtifactConfigurationDescriptionTypeDef](./type_defs.md#customartifactconfigurationdescriptiontypedef) 
## ZeppelinApplicationConfigurationTypeDef

```python
# ZeppelinApplicationConfigurationTypeDef definition

class ZeppelinApplicationConfigurationTypeDef(TypedDict):
    MonitoringConfiguration: NotRequired[ZeppelinMonitoringConfigurationTypeDef],  # (1)
    CatalogConfiguration: NotRequired[CatalogConfigurationTypeDef],  # (2)
    DeployAsApplicationConfiguration: NotRequired[DeployAsApplicationConfigurationTypeDef],  # (3)
    CustomArtifactsConfiguration: NotRequired[Sequence[CustomArtifactConfigurationTypeDef]],  # (4)
```

1. See [:material-code-braces: ZeppelinMonitoringConfigurationTypeDef](./type_defs.md#zeppelinmonitoringconfigurationtypedef) 
2. See [:material-code-braces: CatalogConfigurationTypeDef](./type_defs.md#catalogconfigurationtypedef) 
3. See [:material-code-braces: DeployAsApplicationConfigurationTypeDef](./type_defs.md#deployasapplicationconfigurationtypedef) 
4. See [:material-code-braces: CustomArtifactConfigurationTypeDef](./type_defs.md#customartifactconfigurationtypedef) 
## ZeppelinApplicationConfigurationUpdateTypeDef

```python
# ZeppelinApplicationConfigurationUpdateTypeDef definition

class ZeppelinApplicationConfigurationUpdateTypeDef(TypedDict):
    MonitoringConfigurationUpdate: NotRequired[ZeppelinMonitoringConfigurationUpdateTypeDef],  # (1)
    CatalogConfigurationUpdate: NotRequired[CatalogConfigurationUpdateTypeDef],  # (2)
    DeployAsApplicationConfigurationUpdate: NotRequired[DeployAsApplicationConfigurationUpdateTypeDef],  # (3)
    CustomArtifactsConfigurationUpdate: NotRequired[Sequence[CustomArtifactConfigurationTypeDef]],  # (4)
```

1. See [:material-code-braces: ZeppelinMonitoringConfigurationUpdateTypeDef](./type_defs.md#zeppelinmonitoringconfigurationupdatetypedef) 
2. See [:material-code-braces: CatalogConfigurationUpdateTypeDef](./type_defs.md#catalogconfigurationupdatetypedef) 
3. See [:material-code-braces: DeployAsApplicationConfigurationUpdateTypeDef](./type_defs.md#deployasapplicationconfigurationupdatetypedef) 
4. See [:material-code-braces: CustomArtifactConfigurationTypeDef](./type_defs.md#customartifactconfigurationtypedef) 
## RunConfigurationTypeDef

```python
# RunConfigurationTypeDef definition

class RunConfigurationTypeDef(TypedDict):
    FlinkRunConfiguration: NotRequired[FlinkRunConfigurationTypeDef],  # (1)
    SqlRunConfigurations: NotRequired[Sequence[SqlRunConfigurationTypeDef]],  # (2)
    ApplicationRestoreConfiguration: NotRequired[ApplicationRestoreConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: FlinkRunConfigurationTypeDef](./type_defs.md#flinkrunconfigurationtypedef) 
2. See [:material-code-braces: SqlRunConfigurationTypeDef](./type_defs.md#sqlrunconfigurationtypedef) 
3. See [:material-code-braces: ApplicationRestoreConfigurationTypeDef](./type_defs.md#applicationrestoreconfigurationtypedef) 
## AddApplicationInputProcessingConfigurationResponseTypeDef

```python
# AddApplicationInputProcessingConfigurationResponseTypeDef definition

class AddApplicationInputProcessingConfigurationResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    InputId: str,
    InputProcessingConfigurationDescription: InputProcessingConfigurationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputProcessingConfigurationDescriptionTypeDef](./type_defs.md#inputprocessingconfigurationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddApplicationInputProcessingConfigurationRequestRequestTypeDef

```python
# AddApplicationInputProcessingConfigurationRequestRequestTypeDef definition

class AddApplicationInputProcessingConfigurationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CurrentApplicationVersionId: int,
    InputId: str,
    InputProcessingConfiguration: InputProcessingConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: InputProcessingConfigurationTypeDef](./type_defs.md#inputprocessingconfigurationtypedef) 
## DiscoverInputSchemaRequestRequestTypeDef

```python
# DiscoverInputSchemaRequestRequestTypeDef definition

class DiscoverInputSchemaRequestRequestTypeDef(TypedDict):
    ServiceExecutionRole: str,
    ResourceARN: NotRequired[str],
    InputStartingPositionConfiguration: NotRequired[InputStartingPositionConfigurationTypeDef],  # (1)
    S3Configuration: NotRequired[S3ConfigurationTypeDef],  # (2)
    InputProcessingConfiguration: NotRequired[InputProcessingConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: InputStartingPositionConfigurationTypeDef](./type_defs.md#inputstartingpositionconfigurationtypedef) 
2. See [:material-code-braces: S3ConfigurationTypeDef](./type_defs.md#s3configurationtypedef) 
3. See [:material-code-braces: InputProcessingConfigurationTypeDef](./type_defs.md#inputprocessingconfigurationtypedef) 
## RecordFormatTypeDef

```python
# RecordFormatTypeDef definition

class RecordFormatTypeDef(TypedDict):
    RecordFormatType: RecordFormatTypeType,  # (1)
    MappingParameters: NotRequired[MappingParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: RecordFormatTypeType](./literals.md#recordformattypetype) 
2. See [:material-code-braces: MappingParametersTypeDef](./type_defs.md#mappingparameterstypedef) 
## AddApplicationOutputResponseTypeDef

```python
# AddApplicationOutputResponseTypeDef definition

class AddApplicationOutputResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    OutputDescriptions: List[OutputDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutputDescriptionTypeDef](./type_defs.md#outputdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddApplicationOutputRequestRequestTypeDef

```python
# AddApplicationOutputRequestRequestTypeDef definition

class AddApplicationOutputRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CurrentApplicationVersionId: int,
    Output: OutputTypeDef,  # (1)
```

1. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
## StartApplicationRequestRequestTypeDef

```python
# StartApplicationRequestRequestTypeDef definition

class StartApplicationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    RunConfiguration: NotRequired[RunConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: RunConfigurationTypeDef](./type_defs.md#runconfigurationtypedef) 
## InputSchemaUpdateTypeDef

```python
# InputSchemaUpdateTypeDef definition

class InputSchemaUpdateTypeDef(TypedDict):
    RecordFormatUpdate: NotRequired[RecordFormatTypeDef],  # (1)
    RecordEncodingUpdate: NotRequired[str],
    RecordColumnUpdates: NotRequired[Sequence[RecordColumnTypeDef]],  # (2)
```

1. See [:material-code-braces: RecordFormatTypeDef](./type_defs.md#recordformattypedef) 
2. See [:material-code-braces: RecordColumnTypeDef](./type_defs.md#recordcolumntypedef) 
## SourceSchemaTypeDef

```python
# SourceSchemaTypeDef definition

class SourceSchemaTypeDef(TypedDict):
    RecordFormat: RecordFormatTypeDef,  # (1)
    RecordColumns: Sequence[RecordColumnTypeDef],  # (2)
    RecordEncoding: NotRequired[str],
```

1. See [:material-code-braces: RecordFormatTypeDef](./type_defs.md#recordformattypedef) 
2. See [:material-code-braces: RecordColumnTypeDef](./type_defs.md#recordcolumntypedef) 
## InputUpdateTypeDef

```python
# InputUpdateTypeDef definition

class InputUpdateTypeDef(TypedDict):
    InputId: str,
    NamePrefixUpdate: NotRequired[str],
    InputProcessingConfigurationUpdate: NotRequired[InputProcessingConfigurationUpdateTypeDef],  # (1)
    KinesisStreamsInputUpdate: NotRequired[KinesisStreamsInputUpdateTypeDef],  # (2)
    KinesisFirehoseInputUpdate: NotRequired[KinesisFirehoseInputUpdateTypeDef],  # (3)
    InputSchemaUpdate: NotRequired[InputSchemaUpdateTypeDef],  # (4)
    InputParallelismUpdate: NotRequired[InputParallelismUpdateTypeDef],  # (5)
```

1. See [:material-code-braces: InputProcessingConfigurationUpdateTypeDef](./type_defs.md#inputprocessingconfigurationupdatetypedef) 
2. See [:material-code-braces: KinesisStreamsInputUpdateTypeDef](./type_defs.md#kinesisstreamsinputupdatetypedef) 
3. See [:material-code-braces: KinesisFirehoseInputUpdateTypeDef](./type_defs.md#kinesisfirehoseinputupdatetypedef) 
4. See [:material-code-braces: InputSchemaUpdateTypeDef](./type_defs.md#inputschemaupdatetypedef) 
5. See [:material-code-braces: InputParallelismUpdateTypeDef](./type_defs.md#inputparallelismupdatetypedef) 
## DiscoverInputSchemaResponseTypeDef

```python
# DiscoverInputSchemaResponseTypeDef definition

class DiscoverInputSchemaResponseTypeDef(TypedDict):
    InputSchema: SourceSchemaTypeDef,  # (1)
    ParsedInputRecords: List[List[str]],
    ProcessedInputRecords: List[str],
    RawInputRecords: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceSchemaTypeDef](./type_defs.md#sourceschematypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InputDescriptionTypeDef

```python
# InputDescriptionTypeDef definition

class InputDescriptionTypeDef(TypedDict):
    InputId: NotRequired[str],
    NamePrefix: NotRequired[str],
    InAppStreamNames: NotRequired[List[str]],
    InputProcessingConfigurationDescription: NotRequired[InputProcessingConfigurationDescriptionTypeDef],  # (1)
    KinesisStreamsInputDescription: NotRequired[KinesisStreamsInputDescriptionTypeDef],  # (2)
    KinesisFirehoseInputDescription: NotRequired[KinesisFirehoseInputDescriptionTypeDef],  # (3)
    InputSchema: NotRequired[SourceSchemaTypeDef],  # (4)
    InputParallelism: NotRequired[InputParallelismTypeDef],  # (5)
    InputStartingPositionConfiguration: NotRequired[InputStartingPositionConfigurationTypeDef],  # (6)
```

1. See [:material-code-braces: InputProcessingConfigurationDescriptionTypeDef](./type_defs.md#inputprocessingconfigurationdescriptiontypedef) 
2. See [:material-code-braces: KinesisStreamsInputDescriptionTypeDef](./type_defs.md#kinesisstreamsinputdescriptiontypedef) 
3. See [:material-code-braces: KinesisFirehoseInputDescriptionTypeDef](./type_defs.md#kinesisfirehoseinputdescriptiontypedef) 
4. See [:material-code-braces: SourceSchemaTypeDef](./type_defs.md#sourceschematypedef) 
5. See [:material-code-braces: InputParallelismTypeDef](./type_defs.md#inputparallelismtypedef) 
6. See [:material-code-braces: InputStartingPositionConfigurationTypeDef](./type_defs.md#inputstartingpositionconfigurationtypedef) 
## InputTypeDef

```python
# InputTypeDef definition

class InputTypeDef(TypedDict):
    NamePrefix: str,
    InputSchema: SourceSchemaTypeDef,  # (5)
    InputProcessingConfiguration: NotRequired[InputProcessingConfigurationTypeDef],  # (1)
    KinesisStreamsInput: NotRequired[KinesisStreamsInputTypeDef],  # (2)
    KinesisFirehoseInput: NotRequired[KinesisFirehoseInputTypeDef],  # (3)
    InputParallelism: NotRequired[InputParallelismTypeDef],  # (4)
```

1. See [:material-code-braces: InputProcessingConfigurationTypeDef](./type_defs.md#inputprocessingconfigurationtypedef) 
2. See [:material-code-braces: KinesisStreamsInputTypeDef](./type_defs.md#kinesisstreamsinputtypedef) 
3. See [:material-code-braces: KinesisFirehoseInputTypeDef](./type_defs.md#kinesisfirehoseinputtypedef) 
4. See [:material-code-braces: InputParallelismTypeDef](./type_defs.md#inputparallelismtypedef) 
5. See [:material-code-braces: SourceSchemaTypeDef](./type_defs.md#sourceschematypedef) 
## ReferenceDataSourceDescriptionTypeDef

```python
# ReferenceDataSourceDescriptionTypeDef definition

class ReferenceDataSourceDescriptionTypeDef(TypedDict):
    ReferenceId: str,
    TableName: str,
    S3ReferenceDataSourceDescription: S3ReferenceDataSourceDescriptionTypeDef,  # (1)
    ReferenceSchema: NotRequired[SourceSchemaTypeDef],  # (2)
```

1. See [:material-code-braces: S3ReferenceDataSourceDescriptionTypeDef](./type_defs.md#s3referencedatasourcedescriptiontypedef) 
2. See [:material-code-braces: SourceSchemaTypeDef](./type_defs.md#sourceschematypedef) 
## ReferenceDataSourceTypeDef

```python
# ReferenceDataSourceTypeDef definition

class ReferenceDataSourceTypeDef(TypedDict):
    TableName: str,
    ReferenceSchema: SourceSchemaTypeDef,  # (2)
    S3ReferenceDataSource: NotRequired[S3ReferenceDataSourceTypeDef],  # (1)
```

1. See [:material-code-braces: S3ReferenceDataSourceTypeDef](./type_defs.md#s3referencedatasourcetypedef) 
2. See [:material-code-braces: SourceSchemaTypeDef](./type_defs.md#sourceschematypedef) 
## ReferenceDataSourceUpdateTypeDef

```python
# ReferenceDataSourceUpdateTypeDef definition

class ReferenceDataSourceUpdateTypeDef(TypedDict):
    ReferenceId: str,
    TableNameUpdate: NotRequired[str],
    S3ReferenceDataSourceUpdate: NotRequired[S3ReferenceDataSourceUpdateTypeDef],  # (1)
    ReferenceSchemaUpdate: NotRequired[SourceSchemaTypeDef],  # (2)
```

1. See [:material-code-braces: S3ReferenceDataSourceUpdateTypeDef](./type_defs.md#s3referencedatasourceupdatetypedef) 
2. See [:material-code-braces: SourceSchemaTypeDef](./type_defs.md#sourceschematypedef) 
## AddApplicationInputResponseTypeDef

```python
# AddApplicationInputResponseTypeDef definition

class AddApplicationInputResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    InputDescriptions: List[InputDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InputDescriptionTypeDef](./type_defs.md#inputdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddApplicationInputRequestRequestTypeDef

```python
# AddApplicationInputRequestRequestTypeDef definition

class AddApplicationInputRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CurrentApplicationVersionId: int,
    Input: InputTypeDef,  # (1)
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
## AddApplicationReferenceDataSourceResponseTypeDef

```python
# AddApplicationReferenceDataSourceResponseTypeDef definition

class AddApplicationReferenceDataSourceResponseTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationVersionId: int,
    ReferenceDataSourceDescriptions: List[ReferenceDataSourceDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReferenceDataSourceDescriptionTypeDef](./type_defs.md#referencedatasourcedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SqlApplicationConfigurationDescriptionTypeDef

```python
# SqlApplicationConfigurationDescriptionTypeDef definition

class SqlApplicationConfigurationDescriptionTypeDef(TypedDict):
    InputDescriptions: NotRequired[List[InputDescriptionTypeDef]],  # (1)
    OutputDescriptions: NotRequired[List[OutputDescriptionTypeDef]],  # (2)
    ReferenceDataSourceDescriptions: NotRequired[List[ReferenceDataSourceDescriptionTypeDef]],  # (3)
```

1. See [:material-code-braces: InputDescriptionTypeDef](./type_defs.md#inputdescriptiontypedef) 
2. See [:material-code-braces: OutputDescriptionTypeDef](./type_defs.md#outputdescriptiontypedef) 
3. See [:material-code-braces: ReferenceDataSourceDescriptionTypeDef](./type_defs.md#referencedatasourcedescriptiontypedef) 
## AddApplicationReferenceDataSourceRequestRequestTypeDef

```python
# AddApplicationReferenceDataSourceRequestRequestTypeDef definition

class AddApplicationReferenceDataSourceRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CurrentApplicationVersionId: int,
    ReferenceDataSource: ReferenceDataSourceTypeDef,  # (1)
```

1. See [:material-code-braces: ReferenceDataSourceTypeDef](./type_defs.md#referencedatasourcetypedef) 
## SqlApplicationConfigurationTypeDef

```python
# SqlApplicationConfigurationTypeDef definition

class SqlApplicationConfigurationTypeDef(TypedDict):
    Inputs: NotRequired[Sequence[InputTypeDef]],  # (1)
    Outputs: NotRequired[Sequence[OutputTypeDef]],  # (2)
    ReferenceDataSources: NotRequired[Sequence[ReferenceDataSourceTypeDef]],  # (3)
```

1. See [:material-code-braces: InputTypeDef](./type_defs.md#inputtypedef) 
2. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
3. See [:material-code-braces: ReferenceDataSourceTypeDef](./type_defs.md#referencedatasourcetypedef) 
## SqlApplicationConfigurationUpdateTypeDef

```python
# SqlApplicationConfigurationUpdateTypeDef definition

class SqlApplicationConfigurationUpdateTypeDef(TypedDict):
    InputUpdates: NotRequired[Sequence[InputUpdateTypeDef]],  # (1)
    OutputUpdates: NotRequired[Sequence[OutputUpdateTypeDef]],  # (2)
    ReferenceDataSourceUpdates: NotRequired[Sequence[ReferenceDataSourceUpdateTypeDef]],  # (3)
```

1. See [:material-code-braces: InputUpdateTypeDef](./type_defs.md#inputupdatetypedef) 
2. See [:material-code-braces: OutputUpdateTypeDef](./type_defs.md#outputupdatetypedef) 
3. See [:material-code-braces: ReferenceDataSourceUpdateTypeDef](./type_defs.md#referencedatasourceupdatetypedef) 
## ApplicationConfigurationDescriptionTypeDef

```python
# ApplicationConfigurationDescriptionTypeDef definition

class ApplicationConfigurationDescriptionTypeDef(TypedDict):
    SqlApplicationConfigurationDescription: NotRequired[SqlApplicationConfigurationDescriptionTypeDef],  # (1)
    ApplicationCodeConfigurationDescription: NotRequired[ApplicationCodeConfigurationDescriptionTypeDef],  # (2)
    RunConfigurationDescription: NotRequired[RunConfigurationDescriptionTypeDef],  # (3)
    FlinkApplicationConfigurationDescription: NotRequired[FlinkApplicationConfigurationDescriptionTypeDef],  # (4)
    EnvironmentPropertyDescriptions: NotRequired[EnvironmentPropertyDescriptionsTypeDef],  # (5)
    ApplicationSnapshotConfigurationDescription: NotRequired[ApplicationSnapshotConfigurationDescriptionTypeDef],  # (6)
    VpcConfigurationDescriptions: NotRequired[List[VpcConfigurationDescriptionTypeDef]],  # (7)
    ZeppelinApplicationConfigurationDescription: NotRequired[ZeppelinApplicationConfigurationDescriptionTypeDef],  # (8)
```

1. See [:material-code-braces: SqlApplicationConfigurationDescriptionTypeDef](./type_defs.md#sqlapplicationconfigurationdescriptiontypedef) 
2. See [:material-code-braces: ApplicationCodeConfigurationDescriptionTypeDef](./type_defs.md#applicationcodeconfigurationdescriptiontypedef) 
3. See [:material-code-braces: RunConfigurationDescriptionTypeDef](./type_defs.md#runconfigurationdescriptiontypedef) 
4. See [:material-code-braces: FlinkApplicationConfigurationDescriptionTypeDef](./type_defs.md#flinkapplicationconfigurationdescriptiontypedef) 
5. See [:material-code-braces: EnvironmentPropertyDescriptionsTypeDef](./type_defs.md#environmentpropertydescriptionstypedef) 
6. See [:material-code-braces: ApplicationSnapshotConfigurationDescriptionTypeDef](./type_defs.md#applicationsnapshotconfigurationdescriptiontypedef) 
7. See [:material-code-braces: VpcConfigurationDescriptionTypeDef](./type_defs.md#vpcconfigurationdescriptiontypedef) 
8. See [:material-code-braces: ZeppelinApplicationConfigurationDescriptionTypeDef](./type_defs.md#zeppelinapplicationconfigurationdescriptiontypedef) 
## ApplicationConfigurationTypeDef

```python
# ApplicationConfigurationTypeDef definition

class ApplicationConfigurationTypeDef(TypedDict):
    SqlApplicationConfiguration: NotRequired[SqlApplicationConfigurationTypeDef],  # (1)
    FlinkApplicationConfiguration: NotRequired[FlinkApplicationConfigurationTypeDef],  # (2)
    EnvironmentProperties: NotRequired[EnvironmentPropertiesTypeDef],  # (3)
    ApplicationCodeConfiguration: NotRequired[ApplicationCodeConfigurationTypeDef],  # (4)
    ApplicationSnapshotConfiguration: NotRequired[ApplicationSnapshotConfigurationTypeDef],  # (5)
    VpcConfigurations: NotRequired[Sequence[VpcConfigurationTypeDef]],  # (6)
    ZeppelinApplicationConfiguration: NotRequired[ZeppelinApplicationConfigurationTypeDef],  # (7)
```

1. See [:material-code-braces: SqlApplicationConfigurationTypeDef](./type_defs.md#sqlapplicationconfigurationtypedef) 
2. See [:material-code-braces: FlinkApplicationConfigurationTypeDef](./type_defs.md#flinkapplicationconfigurationtypedef) 
3. See [:material-code-braces: EnvironmentPropertiesTypeDef](./type_defs.md#environmentpropertiestypedef) 
4. See [:material-code-braces: ApplicationCodeConfigurationTypeDef](./type_defs.md#applicationcodeconfigurationtypedef) 
5. See [:material-code-braces: ApplicationSnapshotConfigurationTypeDef](./type_defs.md#applicationsnapshotconfigurationtypedef) 
6. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
7. See [:material-code-braces: ZeppelinApplicationConfigurationTypeDef](./type_defs.md#zeppelinapplicationconfigurationtypedef) 
## ApplicationConfigurationUpdateTypeDef

```python
# ApplicationConfigurationUpdateTypeDef definition

class ApplicationConfigurationUpdateTypeDef(TypedDict):
    SqlApplicationConfigurationUpdate: NotRequired[SqlApplicationConfigurationUpdateTypeDef],  # (1)
    ApplicationCodeConfigurationUpdate: NotRequired[ApplicationCodeConfigurationUpdateTypeDef],  # (2)
    FlinkApplicationConfigurationUpdate: NotRequired[FlinkApplicationConfigurationUpdateTypeDef],  # (3)
    EnvironmentPropertyUpdates: NotRequired[EnvironmentPropertyUpdatesTypeDef],  # (4)
    ApplicationSnapshotConfigurationUpdate: NotRequired[ApplicationSnapshotConfigurationUpdateTypeDef],  # (5)
    VpcConfigurationUpdates: NotRequired[Sequence[VpcConfigurationUpdateTypeDef]],  # (6)
    ZeppelinApplicationConfigurationUpdate: NotRequired[ZeppelinApplicationConfigurationUpdateTypeDef],  # (7)
```

1. See [:material-code-braces: SqlApplicationConfigurationUpdateTypeDef](./type_defs.md#sqlapplicationconfigurationupdatetypedef) 
2. See [:material-code-braces: ApplicationCodeConfigurationUpdateTypeDef](./type_defs.md#applicationcodeconfigurationupdatetypedef) 
3. See [:material-code-braces: FlinkApplicationConfigurationUpdateTypeDef](./type_defs.md#flinkapplicationconfigurationupdatetypedef) 
4. See [:material-code-braces: EnvironmentPropertyUpdatesTypeDef](./type_defs.md#environmentpropertyupdatestypedef) 
5. See [:material-code-braces: ApplicationSnapshotConfigurationUpdateTypeDef](./type_defs.md#applicationsnapshotconfigurationupdatetypedef) 
6. See [:material-code-braces: VpcConfigurationUpdateTypeDef](./type_defs.md#vpcconfigurationupdatetypedef) 
7. See [:material-code-braces: ZeppelinApplicationConfigurationUpdateTypeDef](./type_defs.md#zeppelinapplicationconfigurationupdatetypedef) 
## ApplicationDetailTypeDef

```python
# ApplicationDetailTypeDef definition

class ApplicationDetailTypeDef(TypedDict):
    ApplicationARN: str,
    ApplicationName: str,
    RuntimeEnvironment: RuntimeEnvironmentType,  # (1)
    ApplicationStatus: ApplicationStatusType,  # (2)
    ApplicationVersionId: int,
    ApplicationDescription: NotRequired[str],
    ServiceExecutionRole: NotRequired[str],
    CreateTimestamp: NotRequired[datetime],
    LastUpdateTimestamp: NotRequired[datetime],
    ApplicationConfigurationDescription: NotRequired[ApplicationConfigurationDescriptionTypeDef],  # (3)
    CloudWatchLoggingOptionDescriptions: NotRequired[List[CloudWatchLoggingOptionDescriptionTypeDef]],  # (4)
    ApplicationMaintenanceConfigurationDescription: NotRequired[ApplicationMaintenanceConfigurationDescriptionTypeDef],  # (5)
    ApplicationVersionUpdatedFrom: NotRequired[int],
    ApplicationVersionRolledBackFrom: NotRequired[int],
    ConditionalToken: NotRequired[str],
    ApplicationVersionRolledBackTo: NotRequired[int],
    ApplicationMode: NotRequired[ApplicationModeType],  # (6)
```

1. See [:material-code-brackets: RuntimeEnvironmentType](./literals.md#runtimeenvironmenttype) 
2. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
3. See [:material-code-braces: ApplicationConfigurationDescriptionTypeDef](./type_defs.md#applicationconfigurationdescriptiontypedef) 
4. See [:material-code-braces: CloudWatchLoggingOptionDescriptionTypeDef](./type_defs.md#cloudwatchloggingoptiondescriptiontypedef) 
5. See [:material-code-braces: ApplicationMaintenanceConfigurationDescriptionTypeDef](./type_defs.md#applicationmaintenanceconfigurationdescriptiontypedef) 
6. See [:material-code-brackets: ApplicationModeType](./literals.md#applicationmodetype) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    RuntimeEnvironment: RuntimeEnvironmentType,  # (1)
    ServiceExecutionRole: str,
    ApplicationDescription: NotRequired[str],
    ApplicationConfiguration: NotRequired[ApplicationConfigurationTypeDef],  # (2)
    CloudWatchLoggingOptions: NotRequired[Sequence[CloudWatchLoggingOptionTypeDef]],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    ApplicationMode: NotRequired[ApplicationModeType],  # (5)
```

1. See [:material-code-brackets: RuntimeEnvironmentType](./literals.md#runtimeenvironmenttype) 
2. See [:material-code-braces: ApplicationConfigurationTypeDef](./type_defs.md#applicationconfigurationtypedef) 
3. See [:material-code-braces: CloudWatchLoggingOptionTypeDef](./type_defs.md#cloudwatchloggingoptiontypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-brackets: ApplicationModeType](./literals.md#applicationmodetype) 
## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    ApplicationName: str,
    CurrentApplicationVersionId: NotRequired[int],
    ApplicationConfigurationUpdate: NotRequired[ApplicationConfigurationUpdateTypeDef],  # (1)
    ServiceExecutionRoleUpdate: NotRequired[str],
    RunConfigurationUpdate: NotRequired[RunConfigurationUpdateTypeDef],  # (2)
    CloudWatchLoggingOptionUpdates: NotRequired[Sequence[CloudWatchLoggingOptionUpdateTypeDef]],  # (3)
    ConditionalToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationConfigurationUpdateTypeDef](./type_defs.md#applicationconfigurationupdatetypedef) 
2. See [:material-code-braces: RunConfigurationUpdateTypeDef](./type_defs.md#runconfigurationupdatetypedef) 
3. See [:material-code-braces: CloudWatchLoggingOptionUpdateTypeDef](./type_defs.md#cloudwatchloggingoptionupdatetypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    ApplicationDetail: ApplicationDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationDetailTypeDef](./type_defs.md#applicationdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicationResponseTypeDef

```python
# DescribeApplicationResponseTypeDef definition

class DescribeApplicationResponseTypeDef(TypedDict):
    ApplicationDetail: ApplicationDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationDetailTypeDef](./type_defs.md#applicationdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicationVersionResponseTypeDef

```python
# DescribeApplicationVersionResponseTypeDef definition

class DescribeApplicationVersionResponseTypeDef(TypedDict):
    ApplicationVersionDetail: ApplicationDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationDetailTypeDef](./type_defs.md#applicationdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RollbackApplicationResponseTypeDef

```python
# RollbackApplicationResponseTypeDef definition

class RollbackApplicationResponseTypeDef(TypedDict):
    ApplicationDetail: ApplicationDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationDetailTypeDef](./type_defs.md#applicationdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationResponseTypeDef

```python
# UpdateApplicationResponseTypeDef definition

class UpdateApplicationResponseTypeDef(TypedDict):
    ApplicationDetail: ApplicationDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationDetailTypeDef](./type_defs.md#applicationdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
