# Type definitions

> [Index](../README.md) > [MWAA](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MWAA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
    type annotations stubs module [types-aiobotocore-mwaa](https://pypi.org/project/types-aiobotocore-mwaa/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## CreateCliTokenRequestRequestTypeDef

```python
# CreateCliTokenRequestRequestTypeDef definition

class CreateCliTokenRequestRequestTypeDef(TypedDict):
    Name: str,
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

## NetworkConfigurationTypeDef

```python
# NetworkConfigurationTypeDef definition

class NetworkConfigurationTypeDef(TypedDict):
    SecurityGroupIds: NotRequired[Sequence[str]],
    SubnetIds: NotRequired[Sequence[str]],
```

## CreateWebLoginTokenRequestRequestTypeDef

```python
# CreateWebLoginTokenRequestRequestTypeDef definition

class CreateWebLoginTokenRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteEnvironmentInputRequestTypeDef

```python
# DeleteEnvironmentInputRequestTypeDef definition

class DeleteEnvironmentInputRequestTypeDef(TypedDict):
    Name: str,
```

## DimensionTypeDef

```python
# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## GetEnvironmentInputRequestTypeDef

```python
# GetEnvironmentInputRequestTypeDef definition

class GetEnvironmentInputRequestTypeDef(TypedDict):
    Name: str,
```

## UpdateErrorTypeDef

```python
# UpdateErrorTypeDef definition

class UpdateErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEnvironmentsInputRequestTypeDef

```python
# ListEnvironmentsInputRequestTypeDef definition

class ListEnvironmentsInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ModuleLoggingConfigurationInputTypeDef

```python
# ModuleLoggingConfigurationInputTypeDef definition

class ModuleLoggingConfigurationInputTypeDef(TypedDict):
    Enabled: bool,
    LogLevel: LoggingLevelType,  # (1)
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
## ModuleLoggingConfigurationTypeDef

```python
# ModuleLoggingConfigurationTypeDef definition

class ModuleLoggingConfigurationTypeDef(TypedDict):
    CloudWatchLogGroupArn: NotRequired[str],
    Enabled: NotRequired[bool],
    LogLevel: NotRequired[LoggingLevelType],  # (1)
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
## StatisticSetTypeDef

```python
# StatisticSetTypeDef definition

class StatisticSetTypeDef(TypedDict):
    Maximum: NotRequired[float],
    Minimum: NotRequired[float],
    SampleCount: NotRequired[int],
    Sum: NotRequired[float],
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateNetworkConfigurationInputTypeDef

```python
# UpdateNetworkConfigurationInputTypeDef definition

class UpdateNetworkConfigurationInputTypeDef(TypedDict):
    SecurityGroupIds: Sequence[str],
```

## CreateCliTokenResponseTypeDef

```python
# CreateCliTokenResponseTypeDef definition

class CreateCliTokenResponseTypeDef(TypedDict):
    CliToken: str,
    WebServerHostname: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentOutputTypeDef

```python
# CreateEnvironmentOutputTypeDef definition

class CreateEnvironmentOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWebLoginTokenResponseTypeDef

```python
# CreateWebLoginTokenResponseTypeDef definition

class CreateWebLoginTokenResponseTypeDef(TypedDict):
    WebServerHostname: str,
    WebToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentsOutputTypeDef

```python
# ListEnvironmentsOutputTypeDef definition

class ListEnvironmentsOutputTypeDef(TypedDict):
    Environments: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentOutputTypeDef

```python
# UpdateEnvironmentOutputTypeDef definition

class UpdateEnvironmentOutputTypeDef(TypedDict):
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LastUpdateTypeDef

```python
# LastUpdateTypeDef definition

class LastUpdateTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    Error: NotRequired[UpdateErrorTypeDef],  # (1)
    Source: NotRequired[str],
    Status: NotRequired[UpdateStatusType],  # (2)
```

1. See [:material-code-braces: UpdateErrorTypeDef](./type_defs.md#updateerrortypedef) 
2. See [:material-code-brackets: UpdateStatusType](./literals.md#updatestatustype) 
## ListEnvironmentsInputListEnvironmentsPaginateTypeDef

```python
# ListEnvironmentsInputListEnvironmentsPaginateTypeDef definition

class ListEnvironmentsInputListEnvironmentsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LoggingConfigurationInputTypeDef

```python
# LoggingConfigurationInputTypeDef definition

class LoggingConfigurationInputTypeDef(TypedDict):
    DagProcessingLogs: NotRequired[ModuleLoggingConfigurationInputTypeDef],  # (1)
    SchedulerLogs: NotRequired[ModuleLoggingConfigurationInputTypeDef],  # (1)
    TaskLogs: NotRequired[ModuleLoggingConfigurationInputTypeDef],  # (1)
    WebserverLogs: NotRequired[ModuleLoggingConfigurationInputTypeDef],  # (1)
    WorkerLogs: NotRequired[ModuleLoggingConfigurationInputTypeDef],  # (1)
```

1. See [:material-code-braces: ModuleLoggingConfigurationInputTypeDef](./type_defs.md#moduleloggingconfigurationinputtypedef) 
2. See [:material-code-braces: ModuleLoggingConfigurationInputTypeDef](./type_defs.md#moduleloggingconfigurationinputtypedef) 
3. See [:material-code-braces: ModuleLoggingConfigurationInputTypeDef](./type_defs.md#moduleloggingconfigurationinputtypedef) 
4. See [:material-code-braces: ModuleLoggingConfigurationInputTypeDef](./type_defs.md#moduleloggingconfigurationinputtypedef) 
5. See [:material-code-braces: ModuleLoggingConfigurationInputTypeDef](./type_defs.md#moduleloggingconfigurationinputtypedef) 
## LoggingConfigurationTypeDef

```python
# LoggingConfigurationTypeDef definition

class LoggingConfigurationTypeDef(TypedDict):
    DagProcessingLogs: NotRequired[ModuleLoggingConfigurationTypeDef],  # (1)
    SchedulerLogs: NotRequired[ModuleLoggingConfigurationTypeDef],  # (1)
    TaskLogs: NotRequired[ModuleLoggingConfigurationTypeDef],  # (1)
    WebserverLogs: NotRequired[ModuleLoggingConfigurationTypeDef],  # (1)
    WorkerLogs: NotRequired[ModuleLoggingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ModuleLoggingConfigurationTypeDef](./type_defs.md#moduleloggingconfigurationtypedef) 
2. See [:material-code-braces: ModuleLoggingConfigurationTypeDef](./type_defs.md#moduleloggingconfigurationtypedef) 
3. See [:material-code-braces: ModuleLoggingConfigurationTypeDef](./type_defs.md#moduleloggingconfigurationtypedef) 
4. See [:material-code-braces: ModuleLoggingConfigurationTypeDef](./type_defs.md#moduleloggingconfigurationtypedef) 
5. See [:material-code-braces: ModuleLoggingConfigurationTypeDef](./type_defs.md#moduleloggingconfigurationtypedef) 
## MetricDatumTypeDef

```python
# MetricDatumTypeDef definition

class MetricDatumTypeDef(TypedDict):
    MetricName: str,
    Timestamp: Union[datetime, str],
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    StatisticValues: NotRequired[StatisticSetTypeDef],  # (2)
    Unit: NotRequired[UnitType],  # (3)
    Value: NotRequired[float],
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-braces: StatisticSetTypeDef](./type_defs.md#statisticsettypedef) 
3. See [:material-code-brackets: UnitType](./literals.md#unittype) 
## CreateEnvironmentInputRequestTypeDef

```python
# CreateEnvironmentInputRequestTypeDef definition

class CreateEnvironmentInputRequestTypeDef(TypedDict):
    DagS3Path: str,
    ExecutionRoleArn: str,
    Name: str,
    NetworkConfiguration: NetworkConfigurationTypeDef,  # (1)
    SourceBucketArn: str,
    AirflowConfigurationOptions: NotRequired[Mapping[str, str]],
    AirflowVersion: NotRequired[str],
    EnvironmentClass: NotRequired[str],
    KmsKey: NotRequired[str],
    LoggingConfiguration: NotRequired[LoggingConfigurationInputTypeDef],  # (2)
    MaxWorkers: NotRequired[int],
    MinWorkers: NotRequired[int],
    PluginsS3ObjectVersion: NotRequired[str],
    PluginsS3Path: NotRequired[str],
    RequirementsS3ObjectVersion: NotRequired[str],
    RequirementsS3Path: NotRequired[str],
    Schedulers: NotRequired[int],
    StartupScriptS3ObjectVersion: NotRequired[str],
    StartupScriptS3Path: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    WebserverAccessMode: NotRequired[WebserverAccessModeType],  # (3)
    WeeklyMaintenanceWindowStart: NotRequired[str],
```

1. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
2. See [:material-code-braces: LoggingConfigurationInputTypeDef](./type_defs.md#loggingconfigurationinputtypedef) 
3. See [:material-code-brackets: WebserverAccessModeType](./literals.md#webserveraccessmodetype) 
## UpdateEnvironmentInputRequestTypeDef

```python
# UpdateEnvironmentInputRequestTypeDef definition

class UpdateEnvironmentInputRequestTypeDef(TypedDict):
    Name: str,
    AirflowConfigurationOptions: NotRequired[Mapping[str, str]],
    AirflowVersion: NotRequired[str],
    DagS3Path: NotRequired[str],
    EnvironmentClass: NotRequired[str],
    ExecutionRoleArn: NotRequired[str],
    LoggingConfiguration: NotRequired[LoggingConfigurationInputTypeDef],  # (1)
    MaxWorkers: NotRequired[int],
    MinWorkers: NotRequired[int],
    NetworkConfiguration: NotRequired[UpdateNetworkConfigurationInputTypeDef],  # (2)
    PluginsS3ObjectVersion: NotRequired[str],
    PluginsS3Path: NotRequired[str],
    RequirementsS3ObjectVersion: NotRequired[str],
    RequirementsS3Path: NotRequired[str],
    Schedulers: NotRequired[int],
    SourceBucketArn: NotRequired[str],
    StartupScriptS3ObjectVersion: NotRequired[str],
    StartupScriptS3Path: NotRequired[str],
    WebserverAccessMode: NotRequired[WebserverAccessModeType],  # (3)
    WeeklyMaintenanceWindowStart: NotRequired[str],
```

1. See [:material-code-braces: LoggingConfigurationInputTypeDef](./type_defs.md#loggingconfigurationinputtypedef) 
2. See [:material-code-braces: UpdateNetworkConfigurationInputTypeDef](./type_defs.md#updatenetworkconfigurationinputtypedef) 
3. See [:material-code-brackets: WebserverAccessModeType](./literals.md#webserveraccessmodetype) 
## EnvironmentTypeDef

```python
# EnvironmentTypeDef definition

class EnvironmentTypeDef(TypedDict):
    AirflowConfigurationOptions: NotRequired[Dict[str, str]],
    AirflowVersion: NotRequired[str],
    Arn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    DagS3Path: NotRequired[str],
    EnvironmentClass: NotRequired[str],
    ExecutionRoleArn: NotRequired[str],
    KmsKey: NotRequired[str],
    LastUpdate: NotRequired[LastUpdateTypeDef],  # (1)
    LoggingConfiguration: NotRequired[LoggingConfigurationTypeDef],  # (2)
    MaxWorkers: NotRequired[int],
    MinWorkers: NotRequired[int],
    Name: NotRequired[str],
    NetworkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (3)
    PluginsS3ObjectVersion: NotRequired[str],
    PluginsS3Path: NotRequired[str],
    RequirementsS3ObjectVersion: NotRequired[str],
    RequirementsS3Path: NotRequired[str],
    Schedulers: NotRequired[int],
    ServiceRoleArn: NotRequired[str],
    SourceBucketArn: NotRequired[str],
    StartupScriptS3ObjectVersion: NotRequired[str],
    StartupScriptS3Path: NotRequired[str],
    Status: NotRequired[EnvironmentStatusType],  # (4)
    Tags: NotRequired[Dict[str, str]],
    WebserverAccessMode: NotRequired[WebserverAccessModeType],  # (5)
    WebserverUrl: NotRequired[str],
    WeeklyMaintenanceWindowStart: NotRequired[str],
```

1. See [:material-code-braces: LastUpdateTypeDef](./type_defs.md#lastupdatetypedef) 
2. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
3. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
4. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
5. See [:material-code-brackets: WebserverAccessModeType](./literals.md#webserveraccessmodetype) 
## PublishMetricsInputRequestTypeDef

```python
# PublishMetricsInputRequestTypeDef definition

class PublishMetricsInputRequestTypeDef(TypedDict):
    EnvironmentName: str,
    MetricData: Sequence[MetricDatumTypeDef],  # (1)
```

1. See [:material-code-braces: MetricDatumTypeDef](./type_defs.md#metricdatumtypedef) 
## GetEnvironmentOutputTypeDef

```python
# GetEnvironmentOutputTypeDef definition

class GetEnvironmentOutputTypeDef(TypedDict):
    Environment: EnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
