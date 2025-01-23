# Type definitions

> [Index](../README.md) > [MWAA](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MWAA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#mwaa)
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
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## NetworkConfigurationTypeDef

```python
# NetworkConfigurationTypeDef definition

class NetworkConfigurationTypeDef(TypedDict):
    SubnetIds: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
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

## NetworkConfigurationOutputTypeDef

```python
# NetworkConfigurationOutputTypeDef definition

class NetworkConfigurationOutputTypeDef(TypedDict):
    SubnetIds: NotRequired[List[str]],
    SecurityGroupIds: NotRequired[List[str]],
```

## GetEnvironmentInputRequestTypeDef

```python
# GetEnvironmentInputRequestTypeDef definition

class GetEnvironmentInputRequestTypeDef(TypedDict):
    Name: str,
```

## InvokeRestApiRequestRequestTypeDef

```python
# InvokeRestApiRequestRequestTypeDef definition

class InvokeRestApiRequestRequestTypeDef(TypedDict):
    Name: str,
    Path: str,
    Method: RestApiMethodType,  # (1)
    QueryParameters: NotRequired[Mapping[str, Any]],
    Body: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-brackets: RestApiMethodType](./literals.md#restapimethodtype) 
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
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
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
    Enabled: NotRequired[bool],
    LogLevel: NotRequired[LoggingLevelType],  # (1)
    CloudWatchLogGroupArn: NotRequired[str],
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
## StatisticSetTypeDef

```python
# StatisticSetTypeDef definition

class StatisticSetTypeDef(TypedDict):
    SampleCount: NotRequired[int],
    Sum: NotRequired[float],
    Minimum: NotRequired[float],
    Maximum: NotRequired[float],
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
    WebToken: str,
    WebServerHostname: str,
    IamIdentity: str,
    AirflowIdentity: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvokeRestApiResponseTypeDef

```python
# InvokeRestApiResponseTypeDef definition

class InvokeRestApiResponseTypeDef(TypedDict):
    RestApiStatusCode: int,
    RestApiResponse: Dict[str, Any],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentsOutputTypeDef

```python
# ListEnvironmentsOutputTypeDef definition

class ListEnvironmentsOutputTypeDef(TypedDict):
    Environments: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
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
    Status: NotRequired[UpdateStatusType],  # (1)
    CreatedAt: NotRequired[datetime],
    Error: NotRequired[UpdateErrorTypeDef],  # (2)
    Source: NotRequired[str],
```

1. See [:material-code-brackets: UpdateStatusType](./literals.md#updatestatustype) 
2. See [:material-code-braces: UpdateErrorTypeDef](./type_defs.md#updateerrortypedef) 
## ListEnvironmentsInputPaginateTypeDef

```python
# ListEnvironmentsInputPaginateTypeDef definition

class ListEnvironmentsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LoggingConfigurationInputTypeDef

```python
# LoggingConfigurationInputTypeDef definition

class LoggingConfigurationInputTypeDef(TypedDict):
    DagProcessingLogs: NotRequired[ModuleLoggingConfigurationInputTypeDef],  # (1)
    SchedulerLogs: NotRequired[ModuleLoggingConfigurationInputTypeDef],  # (1)
    WebserverLogs: NotRequired[ModuleLoggingConfigurationInputTypeDef],  # (1)
    WorkerLogs: NotRequired[ModuleLoggingConfigurationInputTypeDef],  # (1)
    TaskLogs: NotRequired[ModuleLoggingConfigurationInputTypeDef],  # (1)
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
    WebserverLogs: NotRequired[ModuleLoggingConfigurationTypeDef],  # (1)
    WorkerLogs: NotRequired[ModuleLoggingConfigurationTypeDef],  # (1)
    TaskLogs: NotRequired[ModuleLoggingConfigurationTypeDef],  # (1)
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
    Timestamp: TimestampTypeDef,
    Dimensions: NotRequired[Sequence[DimensionTypeDef]],  # (1)
    Value: NotRequired[float],
    Unit: NotRequired[UnitType],  # (2)
    StatisticValues: NotRequired[StatisticSetTypeDef],  # (3)
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
2. See [:material-code-brackets: UnitType](./literals.md#unittype) 
3. See [:material-code-braces: StatisticSetTypeDef](./type_defs.md#statisticsettypedef) 
## CreateEnvironmentInputRequestTypeDef

```python
# CreateEnvironmentInputRequestTypeDef definition

class CreateEnvironmentInputRequestTypeDef(TypedDict):
    Name: str,
    ExecutionRoleArn: str,
    SourceBucketArn: str,
    DagS3Path: str,
    NetworkConfiguration: NetworkConfigurationTypeDef,  # (1)
    PluginsS3Path: NotRequired[str],
    PluginsS3ObjectVersion: NotRequired[str],
    RequirementsS3Path: NotRequired[str],
    RequirementsS3ObjectVersion: NotRequired[str],
    StartupScriptS3Path: NotRequired[str],
    StartupScriptS3ObjectVersion: NotRequired[str],
    AirflowConfigurationOptions: NotRequired[Mapping[str, str]],
    EnvironmentClass: NotRequired[str],
    MaxWorkers: NotRequired[int],
    KmsKey: NotRequired[str],
    AirflowVersion: NotRequired[str],
    LoggingConfiguration: NotRequired[LoggingConfigurationInputTypeDef],  # (2)
    WeeklyMaintenanceWindowStart: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    WebserverAccessMode: NotRequired[WebserverAccessModeType],  # (3)
    MinWorkers: NotRequired[int],
    Schedulers: NotRequired[int],
    EndpointManagement: NotRequired[EndpointManagementType],  # (4)
    MinWebservers: NotRequired[int],
    MaxWebservers: NotRequired[int],
```

1. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
2. See [:material-code-braces: LoggingConfigurationInputTypeDef](./type_defs.md#loggingconfigurationinputtypedef) 
3. See [:material-code-brackets: WebserverAccessModeType](./literals.md#webserveraccessmodetype) 
4. See [:material-code-brackets: EndpointManagementType](./literals.md#endpointmanagementtype) 
## UpdateEnvironmentInputRequestTypeDef

```python
# UpdateEnvironmentInputRequestTypeDef definition

class UpdateEnvironmentInputRequestTypeDef(TypedDict):
    Name: str,
    ExecutionRoleArn: NotRequired[str],
    AirflowVersion: NotRequired[str],
    SourceBucketArn: NotRequired[str],
    DagS3Path: NotRequired[str],
    PluginsS3Path: NotRequired[str],
    PluginsS3ObjectVersion: NotRequired[str],
    RequirementsS3Path: NotRequired[str],
    RequirementsS3ObjectVersion: NotRequired[str],
    StartupScriptS3Path: NotRequired[str],
    StartupScriptS3ObjectVersion: NotRequired[str],
    AirflowConfigurationOptions: NotRequired[Mapping[str, str]],
    EnvironmentClass: NotRequired[str],
    MaxWorkers: NotRequired[int],
    NetworkConfiguration: NotRequired[UpdateNetworkConfigurationInputTypeDef],  # (1)
    LoggingConfiguration: NotRequired[LoggingConfigurationInputTypeDef],  # (2)
    WeeklyMaintenanceWindowStart: NotRequired[str],
    WebserverAccessMode: NotRequired[WebserverAccessModeType],  # (3)
    MinWorkers: NotRequired[int],
    Schedulers: NotRequired[int],
    MinWebservers: NotRequired[int],
    MaxWebservers: NotRequired[int],
```

1. See [:material-code-braces: UpdateNetworkConfigurationInputTypeDef](./type_defs.md#updatenetworkconfigurationinputtypedef) 
2. See [:material-code-braces: LoggingConfigurationInputTypeDef](./type_defs.md#loggingconfigurationinputtypedef) 
3. See [:material-code-brackets: WebserverAccessModeType](./literals.md#webserveraccessmodetype) 
## EnvironmentTypeDef

```python
# EnvironmentTypeDef definition

class EnvironmentTypeDef(TypedDict):
    Name: NotRequired[str],
    Status: NotRequired[EnvironmentStatusType],  # (1)
    Arn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    WebserverUrl: NotRequired[str],
    ExecutionRoleArn: NotRequired[str],
    ServiceRoleArn: NotRequired[str],
    KmsKey: NotRequired[str],
    AirflowVersion: NotRequired[str],
    SourceBucketArn: NotRequired[str],
    DagS3Path: NotRequired[str],
    PluginsS3Path: NotRequired[str],
    PluginsS3ObjectVersion: NotRequired[str],
    RequirementsS3Path: NotRequired[str],
    RequirementsS3ObjectVersion: NotRequired[str],
    StartupScriptS3Path: NotRequired[str],
    StartupScriptS3ObjectVersion: NotRequired[str],
    AirflowConfigurationOptions: NotRequired[Dict[str, str]],
    EnvironmentClass: NotRequired[str],
    MaxWorkers: NotRequired[int],
    NetworkConfiguration: NotRequired[NetworkConfigurationOutputTypeDef],  # (2)
    LoggingConfiguration: NotRequired[LoggingConfigurationTypeDef],  # (3)
    LastUpdate: NotRequired[LastUpdateTypeDef],  # (4)
    WeeklyMaintenanceWindowStart: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    WebserverAccessMode: NotRequired[WebserverAccessModeType],  # (5)
    MinWorkers: NotRequired[int],
    Schedulers: NotRequired[int],
    WebserverVpcEndpointService: NotRequired[str],
    DatabaseVpcEndpointService: NotRequired[str],
    CeleryExecutorQueue: NotRequired[str],
    EndpointManagement: NotRequired[EndpointManagementType],  # (6)
    MinWebservers: NotRequired[int],
    MaxWebservers: NotRequired[int],
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-braces: NetworkConfigurationOutputTypeDef](./type_defs.md#networkconfigurationoutputtypedef) 
3. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
4. See [:material-code-braces: LastUpdateTypeDef](./type_defs.md#lastupdatetypedef) 
5. See [:material-code-brackets: WebserverAccessModeType](./literals.md#webserveraccessmodetype) 
6. See [:material-code-brackets: EndpointManagementType](./literals.md#endpointmanagementtype) 
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
