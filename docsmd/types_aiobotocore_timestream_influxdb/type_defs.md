# Type definitions

> [Index](../README.md) > [TimestreamInfluxDB](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [TimestreamInfluxDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#TimestreamInfluxDB)
    type annotations stubs module [types-aiobotocore-timestream-influxdb](https://pypi.org/project/types-aiobotocore-timestream-influxdb/).



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

## DbInstanceSummaryTypeDef

```python
# DbInstanceSummaryTypeDef definition

class DbInstanceSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: NotRequired[StatusType],  # (1)
    endpoint: NotRequired[str],
    port: NotRequired[int],
    dbInstanceType: NotRequired[DbInstanceTypeType],  # (2)
    dbStorageType: NotRequired[DbStorageTypeType],  # (3)
    allocatedStorage: NotRequired[int],
    deploymentType: NotRequired[DeploymentTypeType],  # (4)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
3. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
4. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
## DbParameterGroupSummaryTypeDef

```python
# DbParameterGroupSummaryTypeDef definition

class DbParameterGroupSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    description: NotRequired[str],
```

## DeleteDbInstanceInputRequestTypeDef

```python
# DeleteDbInstanceInputRequestTypeDef definition

class DeleteDbInstanceInputRequestTypeDef(TypedDict):
    identifier: str,
```

## DurationTypeDef

```python
# DurationTypeDef definition

class DurationTypeDef(TypedDict):
    durationType: DurationTypeType,  # (1)
    value: int,
```

1. See [:material-code-brackets: DurationTypeType](./literals.md#durationtypetype) 
## GetDbInstanceInputRequestTypeDef

```python
# GetDbInstanceInputRequestTypeDef definition

class GetDbInstanceInputRequestTypeDef(TypedDict):
    identifier: str,
```

## GetDbParameterGroupInputRequestTypeDef

```python
# GetDbParameterGroupInputRequestTypeDef definition

class GetDbParameterGroupInputRequestTypeDef(TypedDict):
    identifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDbInstancesInputRequestTypeDef

```python
# ListDbInstancesInputRequestTypeDef definition

class ListDbInstancesInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDbParameterGroupsInputRequestTypeDef

```python
# ListDbParameterGroupsInputRequestTypeDef definition

class ListDbParameterGroupsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## S3ConfigurationTypeDef

```python
# S3ConfigurationTypeDef definition

class S3ConfigurationTypeDef(TypedDict):
    bucketName: str,
    enabled: bool,
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

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDbInstancesOutputTypeDef

```python
# ListDbInstancesOutputTypeDef definition

class ListDbInstancesOutputTypeDef(TypedDict):
    items: List[DbInstanceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DbInstanceSummaryTypeDef](./type_defs.md#dbinstancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDbParameterGroupsOutputTypeDef

```python
# ListDbParameterGroupsOutputTypeDef definition

class ListDbParameterGroupsOutputTypeDef(TypedDict):
    items: List[DbParameterGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DbParameterGroupSummaryTypeDef](./type_defs.md#dbparametergroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InfluxDBv2ParametersTypeDef

```python
# InfluxDBv2ParametersTypeDef definition

class InfluxDBv2ParametersTypeDef(TypedDict):
    fluxLogEnabled: NotRequired[bool],
    logLevel: NotRequired[LogLevelType],  # (1)
    noTasks: NotRequired[bool],
    queryConcurrency: NotRequired[int],
    queryQueueSize: NotRequired[int],
    tracingType: NotRequired[TracingTypeType],  # (2)
    metricsDisabled: NotRequired[bool],
    httpIdleTimeout: NotRequired[DurationTypeDef],  # (3)
    httpReadHeaderTimeout: NotRequired[DurationTypeDef],  # (3)
    httpReadTimeout: NotRequired[DurationTypeDef],  # (3)
    httpWriteTimeout: NotRequired[DurationTypeDef],  # (3)
    influxqlMaxSelectBuckets: NotRequired[int],
    influxqlMaxSelectPoint: NotRequired[int],
    influxqlMaxSelectSeries: NotRequired[int],
    pprofDisabled: NotRequired[bool],
    queryInitialMemoryBytes: NotRequired[int],
    queryMaxMemoryBytes: NotRequired[int],
    queryMemoryBytes: NotRequired[int],
    sessionLength: NotRequired[int],
    sessionRenewDisabled: NotRequired[bool],
    storageCacheMaxMemorySize: NotRequired[int],
    storageCacheSnapshotMemorySize: NotRequired[int],
    storageCacheSnapshotWriteColdDuration: NotRequired[DurationTypeDef],  # (3)
    storageCompactFullWriteColdDuration: NotRequired[DurationTypeDef],  # (3)
    storageCompactThroughputBurst: NotRequired[int],
    storageMaxConcurrentCompactions: NotRequired[int],
    storageMaxIndexLogFileSize: NotRequired[int],
    storageNoValidateFieldSize: NotRequired[bool],
    storageRetentionCheckInterval: NotRequired[DurationTypeDef],  # (3)
    storageSeriesFileMaxConcurrentSnapshotCompactions: NotRequired[int],
    storageSeriesIdSetCacheSize: NotRequired[int],
    storageWalMaxConcurrentWrites: NotRequired[int],
    storageWalMaxWriteDelay: NotRequired[DurationTypeDef],  # (3)
    uiDisabled: NotRequired[bool],
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-brackets: TracingTypeType](./literals.md#tracingtypetype) 
3. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
4. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
5. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
6. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
7. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
8. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
9. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
10. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
## ListDbInstancesInputListDbInstancesPaginateTypeDef

```python
# ListDbInstancesInputListDbInstancesPaginateTypeDef definition

class ListDbInstancesInputListDbInstancesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDbParameterGroupsInputListDbParameterGroupsPaginateTypeDef

```python
# ListDbParameterGroupsInputListDbParameterGroupsPaginateTypeDef definition

class ListDbParameterGroupsInputListDbParameterGroupsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LogDeliveryConfigurationTypeDef

```python
# LogDeliveryConfigurationTypeDef definition

class LogDeliveryConfigurationTypeDef(TypedDict):
    s3Configuration: S3ConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: S3ConfigurationTypeDef](./type_defs.md#s3configurationtypedef) 
## ParametersTypeDef

```python
# ParametersTypeDef definition

class ParametersTypeDef(TypedDict):
    InfluxDBv2: NotRequired[InfluxDBv2ParametersTypeDef],  # (1)
```

1. See [:material-code-braces: InfluxDBv2ParametersTypeDef](./type_defs.md#influxdbv2parameterstypedef) 
## CreateDbInstanceInputRequestTypeDef

```python
# CreateDbInstanceInputRequestTypeDef definition

class CreateDbInstanceInputRequestTypeDef(TypedDict):
    name: str,
    password: str,
    dbInstanceType: DbInstanceTypeType,  # (1)
    vpcSubnetIds: Sequence[str],
    vpcSecurityGroupIds: Sequence[str],
    allocatedStorage: int,
    username: NotRequired[str],
    organization: NotRequired[str],
    bucket: NotRequired[str],
    publiclyAccessible: NotRequired[bool],
    dbStorageType: NotRequired[DbStorageTypeType],  # (2)
    dbParameterGroupIdentifier: NotRequired[str],
    deploymentType: NotRequired[DeploymentTypeType],  # (3)
    logDeliveryConfiguration: NotRequired[LogDeliveryConfigurationTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
    port: NotRequired[int],
```

1. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
2. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
3. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
4. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
## CreateDbInstanceOutputTypeDef

```python
# CreateDbInstanceOutputTypeDef definition

class CreateDbInstanceOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: StatusType,  # (1)
    endpoint: str,
    port: int,
    dbInstanceType: DbInstanceTypeType,  # (2)
    dbStorageType: DbStorageTypeType,  # (3)
    allocatedStorage: int,
    deploymentType: DeploymentTypeType,  # (4)
    vpcSubnetIds: List[str],
    publiclyAccessible: bool,
    vpcSecurityGroupIds: List[str],
    dbParameterGroupIdentifier: str,
    availabilityZone: str,
    secondaryAvailabilityZone: str,
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef,  # (5)
    influxAuthParametersSecretArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
3. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
4. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
5. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDbInstanceOutputTypeDef

```python
# DeleteDbInstanceOutputTypeDef definition

class DeleteDbInstanceOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: StatusType,  # (1)
    endpoint: str,
    port: int,
    dbInstanceType: DbInstanceTypeType,  # (2)
    dbStorageType: DbStorageTypeType,  # (3)
    allocatedStorage: int,
    deploymentType: DeploymentTypeType,  # (4)
    vpcSubnetIds: List[str],
    publiclyAccessible: bool,
    vpcSecurityGroupIds: List[str],
    dbParameterGroupIdentifier: str,
    availabilityZone: str,
    secondaryAvailabilityZone: str,
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef,  # (5)
    influxAuthParametersSecretArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
3. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
4. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
5. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDbInstanceOutputTypeDef

```python
# GetDbInstanceOutputTypeDef definition

class GetDbInstanceOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: StatusType,  # (1)
    endpoint: str,
    port: int,
    dbInstanceType: DbInstanceTypeType,  # (2)
    dbStorageType: DbStorageTypeType,  # (3)
    allocatedStorage: int,
    deploymentType: DeploymentTypeType,  # (4)
    vpcSubnetIds: List[str],
    publiclyAccessible: bool,
    vpcSecurityGroupIds: List[str],
    dbParameterGroupIdentifier: str,
    availabilityZone: str,
    secondaryAvailabilityZone: str,
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef,  # (5)
    influxAuthParametersSecretArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
3. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
4. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
5. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDbInstanceInputRequestTypeDef

```python
# UpdateDbInstanceInputRequestTypeDef definition

class UpdateDbInstanceInputRequestTypeDef(TypedDict):
    identifier: str,
    logDeliveryConfiguration: NotRequired[LogDeliveryConfigurationTypeDef],  # (1)
    dbParameterGroupIdentifier: NotRequired[str],
    port: NotRequired[int],
    dbInstanceType: NotRequired[DbInstanceTypeType],  # (2)
    deploymentType: NotRequired[DeploymentTypeType],  # (3)
```

1. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
2. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
3. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
## UpdateDbInstanceOutputTypeDef

```python
# UpdateDbInstanceOutputTypeDef definition

class UpdateDbInstanceOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: StatusType,  # (1)
    endpoint: str,
    port: int,
    dbInstanceType: DbInstanceTypeType,  # (2)
    dbStorageType: DbStorageTypeType,  # (3)
    allocatedStorage: int,
    deploymentType: DeploymentTypeType,  # (4)
    vpcSubnetIds: List[str],
    publiclyAccessible: bool,
    vpcSecurityGroupIds: List[str],
    dbParameterGroupIdentifier: str,
    availabilityZone: str,
    secondaryAvailabilityZone: str,
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef,  # (5)
    influxAuthParametersSecretArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
3. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
4. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
5. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDbParameterGroupInputRequestTypeDef

```python
# CreateDbParameterGroupInputRequestTypeDef definition

class CreateDbParameterGroupInputRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    parameters: NotRequired[ParametersTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
## CreateDbParameterGroupOutputTypeDef

```python
# CreateDbParameterGroupOutputTypeDef definition

class CreateDbParameterGroupOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    description: str,
    parameters: ParametersTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDbParameterGroupOutputTypeDef

```python
# GetDbParameterGroupOutputTypeDef definition

class GetDbParameterGroupOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    description: str,
    parameters: ParametersTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
