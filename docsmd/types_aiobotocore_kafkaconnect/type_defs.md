# Type definitions

> [Index](../README.md) > [KafkaConnect](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [KafkaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#KafkaConnect)
    type annotations stubs module [types-aiobotocore-kafkaconnect](https://pypi.org/project/types-aiobotocore-kafkaconnect/).



## VpcDescriptionTypeDef

```python
# VpcDescriptionTypeDef definition

class VpcDescriptionTypeDef(TypedDict):
    securityGroups: NotRequired[List[str]],
    subnets: NotRequired[List[str]],
```

## VpcTypeDef

```python
# VpcTypeDef definition

class VpcTypeDef(TypedDict):
    subnets: Sequence[str],
    securityGroups: NotRequired[Sequence[str]],
```

## ScaleInPolicyDescriptionTypeDef

```python
# ScaleInPolicyDescriptionTypeDef definition

class ScaleInPolicyDescriptionTypeDef(TypedDict):
    cpuUtilizationPercentage: NotRequired[int],
```

## ScaleOutPolicyDescriptionTypeDef

```python
# ScaleOutPolicyDescriptionTypeDef definition

class ScaleOutPolicyDescriptionTypeDef(TypedDict):
    cpuUtilizationPercentage: NotRequired[int],
```

## ScaleInPolicyTypeDef

```python
# ScaleInPolicyTypeDef definition

class ScaleInPolicyTypeDef(TypedDict):
    cpuUtilizationPercentage: int,
```

## ScaleOutPolicyTypeDef

```python
# ScaleOutPolicyTypeDef definition

class ScaleOutPolicyTypeDef(TypedDict):
    cpuUtilizationPercentage: int,
```

## ScaleInPolicyUpdateTypeDef

```python
# ScaleInPolicyUpdateTypeDef definition

class ScaleInPolicyUpdateTypeDef(TypedDict):
    cpuUtilizationPercentage: int,
```

## ScaleOutPolicyUpdateTypeDef

```python
# ScaleOutPolicyUpdateTypeDef definition

class ScaleOutPolicyUpdateTypeDef(TypedDict):
    cpuUtilizationPercentage: int,
```

## ProvisionedCapacityDescriptionTypeDef

```python
# ProvisionedCapacityDescriptionTypeDef definition

class ProvisionedCapacityDescriptionTypeDef(TypedDict):
    mcuCount: NotRequired[int],
    workerCount: NotRequired[int],
```

## ProvisionedCapacityTypeDef

```python
# ProvisionedCapacityTypeDef definition

class ProvisionedCapacityTypeDef(TypedDict):
    mcuCount: int,
    workerCount: int,
```

## ProvisionedCapacityUpdateTypeDef

```python
# ProvisionedCapacityUpdateTypeDef definition

class ProvisionedCapacityUpdateTypeDef(TypedDict):
    mcuCount: int,
    workerCount: int,
```

## CloudWatchLogsLogDeliveryDescriptionTypeDef

```python
# CloudWatchLogsLogDeliveryDescriptionTypeDef definition

class CloudWatchLogsLogDeliveryDescriptionTypeDef(TypedDict):
    enabled: NotRequired[bool],
    logGroup: NotRequired[str],
```

## CloudWatchLogsLogDeliveryTypeDef

```python
# CloudWatchLogsLogDeliveryTypeDef definition

class CloudWatchLogsLogDeliveryTypeDef(TypedDict):
    enabled: bool,
    logGroup: NotRequired[str],
```

## KafkaClusterClientAuthenticationDescriptionTypeDef

```python
# KafkaClusterClientAuthenticationDescriptionTypeDef definition

class KafkaClusterClientAuthenticationDescriptionTypeDef(TypedDict):
    authenticationType: NotRequired[KafkaClusterClientAuthenticationTypeType],  # (1)
```

1. See [:material-code-brackets: KafkaClusterClientAuthenticationTypeType](./literals.md#kafkaclusterclientauthenticationtypetype) 
## KafkaClusterEncryptionInTransitDescriptionTypeDef

```python
# KafkaClusterEncryptionInTransitDescriptionTypeDef definition

class KafkaClusterEncryptionInTransitDescriptionTypeDef(TypedDict):
    encryptionType: NotRequired[KafkaClusterEncryptionInTransitTypeType],  # (1)
```

1. See [:material-code-brackets: KafkaClusterEncryptionInTransitTypeType](./literals.md#kafkaclusterencryptionintransittypetype) 
## WorkerConfigurationDescriptionTypeDef

```python
# WorkerConfigurationDescriptionTypeDef definition

class WorkerConfigurationDescriptionTypeDef(TypedDict):
    revision: NotRequired[int],
    workerConfigurationArn: NotRequired[str],
```

## KafkaClusterClientAuthenticationTypeDef

```python
# KafkaClusterClientAuthenticationTypeDef definition

class KafkaClusterClientAuthenticationTypeDef(TypedDict):
    authenticationType: KafkaClusterClientAuthenticationTypeType,  # (1)
```

1. See [:material-code-brackets: KafkaClusterClientAuthenticationTypeType](./literals.md#kafkaclusterclientauthenticationtypetype) 
## KafkaClusterEncryptionInTransitTypeDef

```python
# KafkaClusterEncryptionInTransitTypeDef definition

class KafkaClusterEncryptionInTransitTypeDef(TypedDict):
    encryptionType: KafkaClusterEncryptionInTransitTypeType,  # (1)
```

1. See [:material-code-brackets: KafkaClusterEncryptionInTransitTypeType](./literals.md#kafkaclusterencryptionintransittypetype) 
## WorkerConfigurationTypeDef

```python
# WorkerConfigurationTypeDef definition

class WorkerConfigurationTypeDef(TypedDict):
    revision: int,
    workerConfigurationArn: str,
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

## CreateWorkerConfigurationRequestRequestTypeDef

```python
# CreateWorkerConfigurationRequestRequestTypeDef definition

class CreateWorkerConfigurationRequestRequestTypeDef(TypedDict):
    name: str,
    propertiesFileContent: str,
    description: NotRequired[str],
```

## WorkerConfigurationRevisionSummaryTypeDef

```python
# WorkerConfigurationRevisionSummaryTypeDef definition

class WorkerConfigurationRevisionSummaryTypeDef(TypedDict):
    creationTime: NotRequired[datetime],
    description: NotRequired[str],
    revision: NotRequired[int],
```

## CustomPluginDescriptionTypeDef

```python
# CustomPluginDescriptionTypeDef definition

class CustomPluginDescriptionTypeDef(TypedDict):
    customPluginArn: NotRequired[str],
    revision: NotRequired[int],
```

## CustomPluginFileDescriptionTypeDef

```python
# CustomPluginFileDescriptionTypeDef definition

class CustomPluginFileDescriptionTypeDef(TypedDict):
    fileMd5: NotRequired[str],
    fileSize: NotRequired[int],
```

## S3LocationDescriptionTypeDef

```python
# S3LocationDescriptionTypeDef definition

class S3LocationDescriptionTypeDef(TypedDict):
    bucketArn: NotRequired[str],
    fileKey: NotRequired[str],
    objectVersion: NotRequired[str],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucketArn: str,
    fileKey: str,
    objectVersion: NotRequired[str],
```

## CustomPluginTypeDef

```python
# CustomPluginTypeDef definition

class CustomPluginTypeDef(TypedDict):
    customPluginArn: str,
    revision: int,
```

## DeleteConnectorRequestRequestTypeDef

```python
# DeleteConnectorRequestRequestTypeDef definition

class DeleteConnectorRequestRequestTypeDef(TypedDict):
    connectorArn: str,
    currentVersion: NotRequired[str],
```

## DeleteCustomPluginRequestRequestTypeDef

```python
# DeleteCustomPluginRequestRequestTypeDef definition

class DeleteCustomPluginRequestRequestTypeDef(TypedDict):
    customPluginArn: str,
```

## DescribeConnectorRequestRequestTypeDef

```python
# DescribeConnectorRequestRequestTypeDef definition

class DescribeConnectorRequestRequestTypeDef(TypedDict):
    connectorArn: str,
```

## StateDescriptionTypeDef

```python
# StateDescriptionTypeDef definition

class StateDescriptionTypeDef(TypedDict):
    code: NotRequired[str],
    message: NotRequired[str],
```

## DescribeCustomPluginRequestRequestTypeDef

```python
# DescribeCustomPluginRequestRequestTypeDef definition

class DescribeCustomPluginRequestRequestTypeDef(TypedDict):
    customPluginArn: str,
```

## DescribeWorkerConfigurationRequestRequestTypeDef

```python
# DescribeWorkerConfigurationRequestRequestTypeDef definition

class DescribeWorkerConfigurationRequestRequestTypeDef(TypedDict):
    workerConfigurationArn: str,
```

## WorkerConfigurationRevisionDescriptionTypeDef

```python
# WorkerConfigurationRevisionDescriptionTypeDef definition

class WorkerConfigurationRevisionDescriptionTypeDef(TypedDict):
    creationTime: NotRequired[datetime],
    description: NotRequired[str],
    propertiesFileContent: NotRequired[str],
    revision: NotRequired[int],
```

## FirehoseLogDeliveryDescriptionTypeDef

```python
# FirehoseLogDeliveryDescriptionTypeDef definition

class FirehoseLogDeliveryDescriptionTypeDef(TypedDict):
    deliveryStream: NotRequired[str],
    enabled: NotRequired[bool],
```

## FirehoseLogDeliveryTypeDef

```python
# FirehoseLogDeliveryTypeDef definition

class FirehoseLogDeliveryTypeDef(TypedDict):
    enabled: bool,
    deliveryStream: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListConnectorsRequestRequestTypeDef

```python
# ListConnectorsRequestRequestTypeDef definition

class ListConnectorsRequestRequestTypeDef(TypedDict):
    connectorNamePrefix: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListCustomPluginsRequestRequestTypeDef

```python
# ListCustomPluginsRequestRequestTypeDef definition

class ListCustomPluginsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListWorkerConfigurationsRequestRequestTypeDef

```python
# ListWorkerConfigurationsRequestRequestTypeDef definition

class ListWorkerConfigurationsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## S3LogDeliveryDescriptionTypeDef

```python
# S3LogDeliveryDescriptionTypeDef definition

class S3LogDeliveryDescriptionTypeDef(TypedDict):
    bucket: NotRequired[str],
    enabled: NotRequired[bool],
    prefix: NotRequired[str],
```

## S3LogDeliveryTypeDef

```python
# S3LogDeliveryTypeDef definition

class S3LogDeliveryTypeDef(TypedDict):
    enabled: bool,
    bucket: NotRequired[str],
    prefix: NotRequired[str],
```

## ApacheKafkaClusterDescriptionTypeDef

```python
# ApacheKafkaClusterDescriptionTypeDef definition

class ApacheKafkaClusterDescriptionTypeDef(TypedDict):
    bootstrapServers: NotRequired[str],
    vpc: NotRequired[VpcDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: VpcDescriptionTypeDef](./type_defs.md#vpcdescriptiontypedef) 
## ApacheKafkaClusterTypeDef

```python
# ApacheKafkaClusterTypeDef definition

class ApacheKafkaClusterTypeDef(TypedDict):
    bootstrapServers: str,
    vpc: VpcTypeDef,  # (1)
```

1. See [:material-code-braces: VpcTypeDef](./type_defs.md#vpctypedef) 
## AutoScalingDescriptionTypeDef

```python
# AutoScalingDescriptionTypeDef definition

class AutoScalingDescriptionTypeDef(TypedDict):
    maxWorkerCount: NotRequired[int],
    mcuCount: NotRequired[int],
    minWorkerCount: NotRequired[int],
    scaleInPolicy: NotRequired[ScaleInPolicyDescriptionTypeDef],  # (1)
    scaleOutPolicy: NotRequired[ScaleOutPolicyDescriptionTypeDef],  # (2)
```

1. See [:material-code-braces: ScaleInPolicyDescriptionTypeDef](./type_defs.md#scaleinpolicydescriptiontypedef) 
2. See [:material-code-braces: ScaleOutPolicyDescriptionTypeDef](./type_defs.md#scaleoutpolicydescriptiontypedef) 
## AutoScalingTypeDef

```python
# AutoScalingTypeDef definition

class AutoScalingTypeDef(TypedDict):
    maxWorkerCount: int,
    mcuCount: int,
    minWorkerCount: int,
    scaleInPolicy: NotRequired[ScaleInPolicyTypeDef],  # (1)
    scaleOutPolicy: NotRequired[ScaleOutPolicyTypeDef],  # (2)
```

1. See [:material-code-braces: ScaleInPolicyTypeDef](./type_defs.md#scaleinpolicytypedef) 
2. See [:material-code-braces: ScaleOutPolicyTypeDef](./type_defs.md#scaleoutpolicytypedef) 
## AutoScalingUpdateTypeDef

```python
# AutoScalingUpdateTypeDef definition

class AutoScalingUpdateTypeDef(TypedDict):
    maxWorkerCount: int,
    mcuCount: int,
    minWorkerCount: int,
    scaleInPolicy: ScaleInPolicyUpdateTypeDef,  # (1)
    scaleOutPolicy: ScaleOutPolicyUpdateTypeDef,  # (2)
```

1. See [:material-code-braces: ScaleInPolicyUpdateTypeDef](./type_defs.md#scaleinpolicyupdatetypedef) 
2. See [:material-code-braces: ScaleOutPolicyUpdateTypeDef](./type_defs.md#scaleoutpolicyupdatetypedef) 
## CreateConnectorResponseTypeDef

```python
# CreateConnectorResponseTypeDef definition

class CreateConnectorResponseTypeDef(TypedDict):
    connectorArn: str,
    connectorName: str,
    connectorState: ConnectorStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectorStateType](./literals.md#connectorstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomPluginResponseTypeDef

```python
# CreateCustomPluginResponseTypeDef definition

class CreateCustomPluginResponseTypeDef(TypedDict):
    customPluginArn: str,
    customPluginState: CustomPluginStateType,  # (1)
    name: str,
    revision: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CustomPluginStateType](./literals.md#custompluginstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteConnectorResponseTypeDef

```python
# DeleteConnectorResponseTypeDef definition

class DeleteConnectorResponseTypeDef(TypedDict):
    connectorArn: str,
    connectorState: ConnectorStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectorStateType](./literals.md#connectorstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCustomPluginResponseTypeDef

```python
# DeleteCustomPluginResponseTypeDef definition

class DeleteCustomPluginResponseTypeDef(TypedDict):
    customPluginArn: str,
    customPluginState: CustomPluginStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CustomPluginStateType](./literals.md#custompluginstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConnectorResponseTypeDef

```python
# UpdateConnectorResponseTypeDef definition

class UpdateConnectorResponseTypeDef(TypedDict):
    connectorArn: str,
    connectorState: ConnectorStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectorStateType](./literals.md#connectorstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkerConfigurationResponseTypeDef

```python
# CreateWorkerConfigurationResponseTypeDef definition

class CreateWorkerConfigurationResponseTypeDef(TypedDict):
    creationTime: datetime,
    latestRevision: WorkerConfigurationRevisionSummaryTypeDef,  # (1)
    name: str,
    workerConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkerConfigurationRevisionSummaryTypeDef](./type_defs.md#workerconfigurationrevisionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkerConfigurationSummaryTypeDef

```python
# WorkerConfigurationSummaryTypeDef definition

class WorkerConfigurationSummaryTypeDef(TypedDict):
    creationTime: NotRequired[datetime],
    description: NotRequired[str],
    latestRevision: NotRequired[WorkerConfigurationRevisionSummaryTypeDef],  # (1)
    name: NotRequired[str],
    workerConfigurationArn: NotRequired[str],
```

1. See [:material-code-braces: WorkerConfigurationRevisionSummaryTypeDef](./type_defs.md#workerconfigurationrevisionsummarytypedef) 
## PluginDescriptionTypeDef

```python
# PluginDescriptionTypeDef definition

class PluginDescriptionTypeDef(TypedDict):
    customPlugin: NotRequired[CustomPluginDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: CustomPluginDescriptionTypeDef](./type_defs.md#customplugindescriptiontypedef) 
## CustomPluginLocationDescriptionTypeDef

```python
# CustomPluginLocationDescriptionTypeDef definition

class CustomPluginLocationDescriptionTypeDef(TypedDict):
    s3Location: NotRequired[S3LocationDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationDescriptionTypeDef](./type_defs.md#s3locationdescriptiontypedef) 
## CustomPluginLocationTypeDef

```python
# CustomPluginLocationTypeDef definition

class CustomPluginLocationTypeDef(TypedDict):
    s3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## PluginTypeDef

```python
# PluginTypeDef definition

class PluginTypeDef(TypedDict):
    customPlugin: CustomPluginTypeDef,  # (1)
```

1. See [:material-code-braces: CustomPluginTypeDef](./type_defs.md#customplugintypedef) 
## DescribeWorkerConfigurationResponseTypeDef

```python
# DescribeWorkerConfigurationResponseTypeDef definition

class DescribeWorkerConfigurationResponseTypeDef(TypedDict):
    creationTime: datetime,
    description: str,
    latestRevision: WorkerConfigurationRevisionDescriptionTypeDef,  # (1)
    name: str,
    workerConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkerConfigurationRevisionDescriptionTypeDef](./type_defs.md#workerconfigurationrevisiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConnectorsRequestListConnectorsPaginateTypeDef

```python
# ListConnectorsRequestListConnectorsPaginateTypeDef definition

class ListConnectorsRequestListConnectorsPaginateTypeDef(TypedDict):
    connectorNamePrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomPluginsRequestListCustomPluginsPaginateTypeDef

```python
# ListCustomPluginsRequestListCustomPluginsPaginateTypeDef definition

class ListCustomPluginsRequestListCustomPluginsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef

```python
# ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef definition

class ListWorkerConfigurationsRequestListWorkerConfigurationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## WorkerLogDeliveryDescriptionTypeDef

```python
# WorkerLogDeliveryDescriptionTypeDef definition

class WorkerLogDeliveryDescriptionTypeDef(TypedDict):
    cloudWatchLogs: NotRequired[CloudWatchLogsLogDeliveryDescriptionTypeDef],  # (1)
    firehose: NotRequired[FirehoseLogDeliveryDescriptionTypeDef],  # (2)
    s3: NotRequired[S3LogDeliveryDescriptionTypeDef],  # (3)
```

1. See [:material-code-braces: CloudWatchLogsLogDeliveryDescriptionTypeDef](./type_defs.md#cloudwatchlogslogdeliverydescriptiontypedef) 
2. See [:material-code-braces: FirehoseLogDeliveryDescriptionTypeDef](./type_defs.md#firehoselogdeliverydescriptiontypedef) 
3. See [:material-code-braces: S3LogDeliveryDescriptionTypeDef](./type_defs.md#s3logdeliverydescriptiontypedef) 
## WorkerLogDeliveryTypeDef

```python
# WorkerLogDeliveryTypeDef definition

class WorkerLogDeliveryTypeDef(TypedDict):
    cloudWatchLogs: NotRequired[CloudWatchLogsLogDeliveryTypeDef],  # (1)
    firehose: NotRequired[FirehoseLogDeliveryTypeDef],  # (2)
    s3: NotRequired[S3LogDeliveryTypeDef],  # (3)
```

1. See [:material-code-braces: CloudWatchLogsLogDeliveryTypeDef](./type_defs.md#cloudwatchlogslogdeliverytypedef) 
2. See [:material-code-braces: FirehoseLogDeliveryTypeDef](./type_defs.md#firehoselogdeliverytypedef) 
3. See [:material-code-braces: S3LogDeliveryTypeDef](./type_defs.md#s3logdeliverytypedef) 
## KafkaClusterDescriptionTypeDef

```python
# KafkaClusterDescriptionTypeDef definition

class KafkaClusterDescriptionTypeDef(TypedDict):
    apacheKafkaCluster: NotRequired[ApacheKafkaClusterDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: ApacheKafkaClusterDescriptionTypeDef](./type_defs.md#apachekafkaclusterdescriptiontypedef) 
## KafkaClusterTypeDef

```python
# KafkaClusterTypeDef definition

class KafkaClusterTypeDef(TypedDict):
    apacheKafkaCluster: ApacheKafkaClusterTypeDef,  # (1)
```

1. See [:material-code-braces: ApacheKafkaClusterTypeDef](./type_defs.md#apachekafkaclustertypedef) 
## CapacityDescriptionTypeDef

```python
# CapacityDescriptionTypeDef definition

class CapacityDescriptionTypeDef(TypedDict):
    autoScaling: NotRequired[AutoScalingDescriptionTypeDef],  # (1)
    provisionedCapacity: NotRequired[ProvisionedCapacityDescriptionTypeDef],  # (2)
```

1. See [:material-code-braces: AutoScalingDescriptionTypeDef](./type_defs.md#autoscalingdescriptiontypedef) 
2. See [:material-code-braces: ProvisionedCapacityDescriptionTypeDef](./type_defs.md#provisionedcapacitydescriptiontypedef) 
## CapacityTypeDef

```python
# CapacityTypeDef definition

class CapacityTypeDef(TypedDict):
    autoScaling: NotRequired[AutoScalingTypeDef],  # (1)
    provisionedCapacity: NotRequired[ProvisionedCapacityTypeDef],  # (2)
```

1. See [:material-code-braces: AutoScalingTypeDef](./type_defs.md#autoscalingtypedef) 
2. See [:material-code-braces: ProvisionedCapacityTypeDef](./type_defs.md#provisionedcapacitytypedef) 
## CapacityUpdateTypeDef

```python
# CapacityUpdateTypeDef definition

class CapacityUpdateTypeDef(TypedDict):
    autoScaling: NotRequired[AutoScalingUpdateTypeDef],  # (1)
    provisionedCapacity: NotRequired[ProvisionedCapacityUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: AutoScalingUpdateTypeDef](./type_defs.md#autoscalingupdatetypedef) 
2. See [:material-code-braces: ProvisionedCapacityUpdateTypeDef](./type_defs.md#provisionedcapacityupdatetypedef) 
## ListWorkerConfigurationsResponseTypeDef

```python
# ListWorkerConfigurationsResponseTypeDef definition

class ListWorkerConfigurationsResponseTypeDef(TypedDict):
    nextToken: str,
    workerConfigurations: List[WorkerConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkerConfigurationSummaryTypeDef](./type_defs.md#workerconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomPluginRevisionSummaryTypeDef

```python
# CustomPluginRevisionSummaryTypeDef definition

class CustomPluginRevisionSummaryTypeDef(TypedDict):
    contentType: NotRequired[CustomPluginContentTypeType],  # (1)
    creationTime: NotRequired[datetime],
    description: NotRequired[str],
    fileDescription: NotRequired[CustomPluginFileDescriptionTypeDef],  # (2)
    location: NotRequired[CustomPluginLocationDescriptionTypeDef],  # (3)
    revision: NotRequired[int],
```

1. See [:material-code-brackets: CustomPluginContentTypeType](./literals.md#customplugincontenttypetype) 
2. See [:material-code-braces: CustomPluginFileDescriptionTypeDef](./type_defs.md#custompluginfiledescriptiontypedef) 
3. See [:material-code-braces: CustomPluginLocationDescriptionTypeDef](./type_defs.md#custompluginlocationdescriptiontypedef) 
## CreateCustomPluginRequestRequestTypeDef

```python
# CreateCustomPluginRequestRequestTypeDef definition

class CreateCustomPluginRequestRequestTypeDef(TypedDict):
    contentType: CustomPluginContentTypeType,  # (1)
    location: CustomPluginLocationTypeDef,  # (2)
    name: str,
    description: NotRequired[str],
```

1. See [:material-code-brackets: CustomPluginContentTypeType](./literals.md#customplugincontenttypetype) 
2. See [:material-code-braces: CustomPluginLocationTypeDef](./type_defs.md#custompluginlocationtypedef) 
## LogDeliveryDescriptionTypeDef

```python
# LogDeliveryDescriptionTypeDef definition

class LogDeliveryDescriptionTypeDef(TypedDict):
    workerLogDelivery: NotRequired[WorkerLogDeliveryDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: WorkerLogDeliveryDescriptionTypeDef](./type_defs.md#workerlogdeliverydescriptiontypedef) 
## LogDeliveryTypeDef

```python
# LogDeliveryTypeDef definition

class LogDeliveryTypeDef(TypedDict):
    workerLogDelivery: WorkerLogDeliveryTypeDef,  # (1)
```

1. See [:material-code-braces: WorkerLogDeliveryTypeDef](./type_defs.md#workerlogdeliverytypedef) 
## UpdateConnectorRequestRequestTypeDef

```python
# UpdateConnectorRequestRequestTypeDef definition

class UpdateConnectorRequestRequestTypeDef(TypedDict):
    capacity: CapacityUpdateTypeDef,  # (1)
    connectorArn: str,
    currentVersion: str,
```

1. See [:material-code-braces: CapacityUpdateTypeDef](./type_defs.md#capacityupdatetypedef) 
## CustomPluginSummaryTypeDef

```python
# CustomPluginSummaryTypeDef definition

class CustomPluginSummaryTypeDef(TypedDict):
    creationTime: NotRequired[datetime],
    customPluginArn: NotRequired[str],
    customPluginState: NotRequired[CustomPluginStateType],  # (1)
    description: NotRequired[str],
    latestRevision: NotRequired[CustomPluginRevisionSummaryTypeDef],  # (2)
    name: NotRequired[str],
```

1. See [:material-code-brackets: CustomPluginStateType](./literals.md#custompluginstatetype) 
2. See [:material-code-braces: CustomPluginRevisionSummaryTypeDef](./type_defs.md#custompluginrevisionsummarytypedef) 
## DescribeCustomPluginResponseTypeDef

```python
# DescribeCustomPluginResponseTypeDef definition

class DescribeCustomPluginResponseTypeDef(TypedDict):
    creationTime: datetime,
    customPluginArn: str,
    customPluginState: CustomPluginStateType,  # (1)
    description: str,
    latestRevision: CustomPluginRevisionSummaryTypeDef,  # (2)
    name: str,
    stateDescription: StateDescriptionTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: CustomPluginStateType](./literals.md#custompluginstatetype) 
2. See [:material-code-braces: CustomPluginRevisionSummaryTypeDef](./type_defs.md#custompluginrevisionsummarytypedef) 
3. See [:material-code-braces: StateDescriptionTypeDef](./type_defs.md#statedescriptiontypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectorSummaryTypeDef

```python
# ConnectorSummaryTypeDef definition

class ConnectorSummaryTypeDef(TypedDict):
    capacity: NotRequired[CapacityDescriptionTypeDef],  # (1)
    connectorArn: NotRequired[str],
    connectorDescription: NotRequired[str],
    connectorName: NotRequired[str],
    connectorState: NotRequired[ConnectorStateType],  # (2)
    creationTime: NotRequired[datetime],
    currentVersion: NotRequired[str],
    kafkaCluster: NotRequired[KafkaClusterDescriptionTypeDef],  # (3)
    kafkaClusterClientAuthentication: NotRequired[KafkaClusterClientAuthenticationDescriptionTypeDef],  # (4)
    kafkaClusterEncryptionInTransit: NotRequired[KafkaClusterEncryptionInTransitDescriptionTypeDef],  # (5)
    kafkaConnectVersion: NotRequired[str],
    logDelivery: NotRequired[LogDeliveryDescriptionTypeDef],  # (6)
    plugins: NotRequired[List[PluginDescriptionTypeDef]],  # (7)
    serviceExecutionRoleArn: NotRequired[str],
    workerConfiguration: NotRequired[WorkerConfigurationDescriptionTypeDef],  # (8)
```

1. See [:material-code-braces: CapacityDescriptionTypeDef](./type_defs.md#capacitydescriptiontypedef) 
2. See [:material-code-brackets: ConnectorStateType](./literals.md#connectorstatetype) 
3. See [:material-code-braces: KafkaClusterDescriptionTypeDef](./type_defs.md#kafkaclusterdescriptiontypedef) 
4. See [:material-code-braces: KafkaClusterClientAuthenticationDescriptionTypeDef](./type_defs.md#kafkaclusterclientauthenticationdescriptiontypedef) 
5. See [:material-code-braces: KafkaClusterEncryptionInTransitDescriptionTypeDef](./type_defs.md#kafkaclusterencryptionintransitdescriptiontypedef) 
6. See [:material-code-braces: LogDeliveryDescriptionTypeDef](./type_defs.md#logdeliverydescriptiontypedef) 
7. See [:material-code-braces: PluginDescriptionTypeDef](./type_defs.md#plugindescriptiontypedef) 
8. See [:material-code-braces: WorkerConfigurationDescriptionTypeDef](./type_defs.md#workerconfigurationdescriptiontypedef) 
## DescribeConnectorResponseTypeDef

```python
# DescribeConnectorResponseTypeDef definition

class DescribeConnectorResponseTypeDef(TypedDict):
    capacity: CapacityDescriptionTypeDef,  # (1)
    connectorArn: str,
    connectorConfiguration: Dict[str, str],
    connectorDescription: str,
    connectorName: str,
    connectorState: ConnectorStateType,  # (2)
    creationTime: datetime,
    currentVersion: str,
    kafkaCluster: KafkaClusterDescriptionTypeDef,  # (3)
    kafkaClusterClientAuthentication: KafkaClusterClientAuthenticationDescriptionTypeDef,  # (4)
    kafkaClusterEncryptionInTransit: KafkaClusterEncryptionInTransitDescriptionTypeDef,  # (5)
    kafkaConnectVersion: str,
    logDelivery: LogDeliveryDescriptionTypeDef,  # (6)
    plugins: List[PluginDescriptionTypeDef],  # (7)
    serviceExecutionRoleArn: str,
    stateDescription: StateDescriptionTypeDef,  # (8)
    workerConfiguration: WorkerConfigurationDescriptionTypeDef,  # (9)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-braces: CapacityDescriptionTypeDef](./type_defs.md#capacitydescriptiontypedef) 
2. See [:material-code-brackets: ConnectorStateType](./literals.md#connectorstatetype) 
3. See [:material-code-braces: KafkaClusterDescriptionTypeDef](./type_defs.md#kafkaclusterdescriptiontypedef) 
4. See [:material-code-braces: KafkaClusterClientAuthenticationDescriptionTypeDef](./type_defs.md#kafkaclusterclientauthenticationdescriptiontypedef) 
5. See [:material-code-braces: KafkaClusterEncryptionInTransitDescriptionTypeDef](./type_defs.md#kafkaclusterencryptionintransitdescriptiontypedef) 
6. See [:material-code-braces: LogDeliveryDescriptionTypeDef](./type_defs.md#logdeliverydescriptiontypedef) 
7. See [:material-code-braces: PluginDescriptionTypeDef](./type_defs.md#plugindescriptiontypedef) 
8. See [:material-code-braces: StateDescriptionTypeDef](./type_defs.md#statedescriptiontypedef) 
9. See [:material-code-braces: WorkerConfigurationDescriptionTypeDef](./type_defs.md#workerconfigurationdescriptiontypedef) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConnectorRequestRequestTypeDef

```python
# CreateConnectorRequestRequestTypeDef definition

class CreateConnectorRequestRequestTypeDef(TypedDict):
    capacity: CapacityTypeDef,  # (1)
    connectorConfiguration: Mapping[str, str],
    connectorName: str,
    kafkaCluster: KafkaClusterTypeDef,  # (2)
    kafkaClusterClientAuthentication: KafkaClusterClientAuthenticationTypeDef,  # (3)
    kafkaClusterEncryptionInTransit: KafkaClusterEncryptionInTransitTypeDef,  # (4)
    kafkaConnectVersion: str,
    plugins: Sequence[PluginTypeDef],  # (5)
    serviceExecutionRoleArn: str,
    connectorDescription: NotRequired[str],
    logDelivery: NotRequired[LogDeliveryTypeDef],  # (6)
    workerConfiguration: NotRequired[WorkerConfigurationTypeDef],  # (7)
```

1. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
2. See [:material-code-braces: KafkaClusterTypeDef](./type_defs.md#kafkaclustertypedef) 
3. See [:material-code-braces: KafkaClusterClientAuthenticationTypeDef](./type_defs.md#kafkaclusterclientauthenticationtypedef) 
4. See [:material-code-braces: KafkaClusterEncryptionInTransitTypeDef](./type_defs.md#kafkaclusterencryptionintransittypedef) 
5. See [:material-code-braces: PluginTypeDef](./type_defs.md#plugintypedef) 
6. See [:material-code-braces: LogDeliveryTypeDef](./type_defs.md#logdeliverytypedef) 
7. See [:material-code-braces: WorkerConfigurationTypeDef](./type_defs.md#workerconfigurationtypedef) 
## ListCustomPluginsResponseTypeDef

```python
# ListCustomPluginsResponseTypeDef definition

class ListCustomPluginsResponseTypeDef(TypedDict):
    customPlugins: List[CustomPluginSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomPluginSummaryTypeDef](./type_defs.md#custompluginsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConnectorsResponseTypeDef

```python
# ListConnectorsResponseTypeDef definition

class ListConnectorsResponseTypeDef(TypedDict):
    connectors: List[ConnectorSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectorSummaryTypeDef](./type_defs.md#connectorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
