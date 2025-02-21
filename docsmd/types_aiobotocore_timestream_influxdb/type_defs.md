# Type definitions

> [Index](../README.md) > [TimestreamInfluxDB](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [TimestreamInfluxDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#timestreaminfluxdb)
    type annotations stubs module [types-aiobotocore-timestream-influxdb](https://pypi.org/project/types-aiobotocore-timestream-influxdb/).



## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DbClusterSummaryTypeDef

```python
# DbClusterSummaryTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import DbClusterSummaryTypeDef


def get_value() -> DbClusterSummaryTypeDef:
    return {
        "id": ...,
    }


# DbClusterSummaryTypeDef definition

class DbClusterSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: NotRequired[ClusterStatusType],  # (1)
    endpoint: NotRequired[str],
    readerEndpoint: NotRequired[str],
    port: NotRequired[int],
    deploymentType: NotRequired[ClusterDeploymentTypeType],  # (2)
    dbInstanceType: NotRequired[DbInstanceTypeType],  # (3)
    networkType: NotRequired[NetworkTypeType],  # (4)
    dbStorageType: NotRequired[DbStorageTypeType],  # (5)
    allocatedStorage: NotRequired[int],
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
2. See [:material-code-brackets: ClusterDeploymentTypeType](./literals.md#clusterdeploymenttypetype) 
3. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
4. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
5. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
## DbInstanceForClusterSummaryTypeDef

```python
# DbInstanceForClusterSummaryTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import DbInstanceForClusterSummaryTypeDef


def get_value() -> DbInstanceForClusterSummaryTypeDef:
    return {
        "id": ...,
    }


# DbInstanceForClusterSummaryTypeDef definition

class DbInstanceForClusterSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: NotRequired[StatusType],  # (1)
    endpoint: NotRequired[str],
    port: NotRequired[int],
    networkType: NotRequired[NetworkTypeType],  # (2)
    dbInstanceType: NotRequired[DbInstanceTypeType],  # (3)
    dbStorageType: NotRequired[DbStorageTypeType],  # (4)
    allocatedStorage: NotRequired[int],
    deploymentType: NotRequired[DeploymentTypeType],  # (5)
    instanceMode: NotRequired[InstanceModeType],  # (6)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
3. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
4. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
5. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
6. See [:material-code-brackets: InstanceModeType](./literals.md#instancemodetype) 
## DbInstanceSummaryTypeDef

```python
# DbInstanceSummaryTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import DbInstanceSummaryTypeDef


def get_value() -> DbInstanceSummaryTypeDef:
    return {
        "id": ...,
    }


# DbInstanceSummaryTypeDef definition

class DbInstanceSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: NotRequired[StatusType],  # (1)
    endpoint: NotRequired[str],
    port: NotRequired[int],
    networkType: NotRequired[NetworkTypeType],  # (2)
    dbInstanceType: NotRequired[DbInstanceTypeType],  # (3)
    dbStorageType: NotRequired[DbStorageTypeType],  # (4)
    allocatedStorage: NotRequired[int],
    deploymentType: NotRequired[DeploymentTypeType],  # (5)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
3. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
4. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
5. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
## DbParameterGroupSummaryTypeDef

```python
# DbParameterGroupSummaryTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import DbParameterGroupSummaryTypeDef


def get_value() -> DbParameterGroupSummaryTypeDef:
    return {
        "id": ...,
    }


# DbParameterGroupSummaryTypeDef definition

class DbParameterGroupSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    description: NotRequired[str],
```

## DeleteDbClusterInputTypeDef

```python
# DeleteDbClusterInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import DeleteDbClusterInputTypeDef


def get_value() -> DeleteDbClusterInputTypeDef:
    return {
        "dbClusterId": ...,
    }


# DeleteDbClusterInputTypeDef definition

class DeleteDbClusterInputTypeDef(TypedDict):
    dbClusterId: str,
```

## DeleteDbInstanceInputTypeDef

```python
# DeleteDbInstanceInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import DeleteDbInstanceInputTypeDef


def get_value() -> DeleteDbInstanceInputTypeDef:
    return {
        "identifier": ...,
    }


# DeleteDbInstanceInputTypeDef definition

class DeleteDbInstanceInputTypeDef(TypedDict):
    identifier: str,
```

## DurationTypeDef

```python
# DurationTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import DurationTypeDef


def get_value() -> DurationTypeDef:
    return {
        "durationType": ...,
    }


# DurationTypeDef definition

class DurationTypeDef(TypedDict):
    durationType: DurationTypeType,  # (1)
    value: int,
```

1. See [:material-code-brackets: DurationTypeType](./literals.md#durationtypetype) 
## GetDbClusterInputTypeDef

```python
# GetDbClusterInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import GetDbClusterInputTypeDef


def get_value() -> GetDbClusterInputTypeDef:
    return {
        "dbClusterId": ...,
    }


# GetDbClusterInputTypeDef definition

class GetDbClusterInputTypeDef(TypedDict):
    dbClusterId: str,
```

## GetDbInstanceInputTypeDef

```python
# GetDbInstanceInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import GetDbInstanceInputTypeDef


def get_value() -> GetDbInstanceInputTypeDef:
    return {
        "identifier": ...,
    }


# GetDbInstanceInputTypeDef definition

class GetDbInstanceInputTypeDef(TypedDict):
    identifier: str,
```

## GetDbParameterGroupInputTypeDef

```python
# GetDbParameterGroupInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import GetDbParameterGroupInputTypeDef


def get_value() -> GetDbParameterGroupInputTypeDef:
    return {
        "identifier": ...,
    }


# GetDbParameterGroupInputTypeDef definition

class GetDbParameterGroupInputTypeDef(TypedDict):
    identifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDbClustersInputTypeDef

```python
# ListDbClustersInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbClustersInputTypeDef


def get_value() -> ListDbClustersInputTypeDef:
    return {
        "nextToken": ...,
    }


# ListDbClustersInputTypeDef definition

class ListDbClustersInputTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDbInstancesForClusterInputTypeDef

```python
# ListDbInstancesForClusterInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbInstancesForClusterInputTypeDef


def get_value() -> ListDbInstancesForClusterInputTypeDef:
    return {
        "dbClusterId": ...,
    }


# ListDbInstancesForClusterInputTypeDef definition

class ListDbInstancesForClusterInputTypeDef(TypedDict):
    dbClusterId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDbInstancesInputTypeDef

```python
# ListDbInstancesInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbInstancesInputTypeDef


def get_value() -> ListDbInstancesInputTypeDef:
    return {
        "nextToken": ...,
    }


# ListDbInstancesInputTypeDef definition

class ListDbInstancesInputTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDbParameterGroupsInputTypeDef

```python
# ListDbParameterGroupsInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbParameterGroupsInputTypeDef


def get_value() -> ListDbParameterGroupsInputTypeDef:
    return {
        "nextToken": ...,
    }


# ListDbParameterGroupsInputTypeDef definition

class ListDbParameterGroupsInputTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## S3ConfigurationTypeDef

```python
# S3ConfigurationTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import S3ConfigurationTypeDef


def get_value() -> S3ConfigurationTypeDef:
    return {
        "bucketName": ...,
    }


# S3ConfigurationTypeDef definition

class S3ConfigurationTypeDef(TypedDict):
    bucketName: str,
    enabled: bool,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## CreateDbClusterOutputTypeDef

```python
# CreateDbClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import CreateDbClusterOutputTypeDef


def get_value() -> CreateDbClusterOutputTypeDef:
    return {
        "dbClusterId": ...,
    }


# CreateDbClusterOutputTypeDef definition

class CreateDbClusterOutputTypeDef(TypedDict):
    dbClusterId: str,
    dbClusterStatus: ClusterStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDbClusterOutputTypeDef

```python
# DeleteDbClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import DeleteDbClusterOutputTypeDef


def get_value() -> DeleteDbClusterOutputTypeDef:
    return {
        "dbClusterStatus": ...,
    }


# DeleteDbClusterOutputTypeDef definition

class DeleteDbClusterOutputTypeDef(TypedDict):
    dbClusterStatus: ClusterStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDbClusterOutputTypeDef

```python
# UpdateDbClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import UpdateDbClusterOutputTypeDef


def get_value() -> UpdateDbClusterOutputTypeDef:
    return {
        "dbClusterStatus": ...,
    }


# UpdateDbClusterOutputTypeDef definition

class UpdateDbClusterOutputTypeDef(TypedDict):
    dbClusterStatus: ClusterStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDbClustersOutputTypeDef

```python
# ListDbClustersOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbClustersOutputTypeDef


def get_value() -> ListDbClustersOutputTypeDef:
    return {
        "items": ...,
    }


# ListDbClustersOutputTypeDef definition

class ListDbClustersOutputTypeDef(TypedDict):
    items: List[DbClusterSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DbClusterSummaryTypeDef](./type_defs.md#dbclustersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDbInstancesForClusterOutputTypeDef

```python
# ListDbInstancesForClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbInstancesForClusterOutputTypeDef


def get_value() -> ListDbInstancesForClusterOutputTypeDef:
    return {
        "items": ...,
    }


# ListDbInstancesForClusterOutputTypeDef definition

class ListDbInstancesForClusterOutputTypeDef(TypedDict):
    items: List[DbInstanceForClusterSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DbInstanceForClusterSummaryTypeDef](./type_defs.md#dbinstanceforclustersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDbInstancesOutputTypeDef

```python
# ListDbInstancesOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbInstancesOutputTypeDef


def get_value() -> ListDbInstancesOutputTypeDef:
    return {
        "items": ...,
    }


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
# ListDbParameterGroupsOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbParameterGroupsOutputTypeDef


def get_value() -> ListDbParameterGroupsOutputTypeDef:
    return {
        "items": ...,
    }


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
# InfluxDBv2ParametersTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import InfluxDBv2ParametersTypeDef


def get_value() -> InfluxDBv2ParametersTypeDef:
    return {
        "fluxLogEnabled": ...,
    }


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
## ListDbClustersInputPaginateTypeDef

```python
# ListDbClustersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbClustersInputPaginateTypeDef


def get_value() -> ListDbClustersInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDbClustersInputPaginateTypeDef definition

class ListDbClustersInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDbInstancesForClusterInputPaginateTypeDef

```python
# ListDbInstancesForClusterInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbInstancesForClusterInputPaginateTypeDef


def get_value() -> ListDbInstancesForClusterInputPaginateTypeDef:
    return {
        "dbClusterId": ...,
    }


# ListDbInstancesForClusterInputPaginateTypeDef definition

class ListDbInstancesForClusterInputPaginateTypeDef(TypedDict):
    dbClusterId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDbInstancesInputPaginateTypeDef

```python
# ListDbInstancesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbInstancesInputPaginateTypeDef


def get_value() -> ListDbInstancesInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDbInstancesInputPaginateTypeDef definition

class ListDbInstancesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDbParameterGroupsInputPaginateTypeDef

```python
# ListDbParameterGroupsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ListDbParameterGroupsInputPaginateTypeDef


def get_value() -> ListDbParameterGroupsInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDbParameterGroupsInputPaginateTypeDef definition

class ListDbParameterGroupsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LogDeliveryConfigurationTypeDef

```python
# LogDeliveryConfigurationTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import LogDeliveryConfigurationTypeDef


def get_value() -> LogDeliveryConfigurationTypeDef:
    return {
        "s3Configuration": ...,
    }


# LogDeliveryConfigurationTypeDef definition

class LogDeliveryConfigurationTypeDef(TypedDict):
    s3Configuration: S3ConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: S3ConfigurationTypeDef](./type_defs.md#s3configurationtypedef) 
## ParametersTypeDef

```python
# ParametersTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import ParametersTypeDef


def get_value() -> ParametersTypeDef:
    return {
        "InfluxDBv2": ...,
    }


# ParametersTypeDef definition

class ParametersTypeDef(TypedDict):
    InfluxDBv2: NotRequired[InfluxDBv2ParametersTypeDef],  # (1)
```

1. See [:material-code-braces: InfluxDBv2ParametersTypeDef](./type_defs.md#influxdbv2parameterstypedef) 
## CreateDbClusterInputTypeDef

```python
# CreateDbClusterInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import CreateDbClusterInputTypeDef


def get_value() -> CreateDbClusterInputTypeDef:
    return {
        "name": ...,
    }


# CreateDbClusterInputTypeDef definition

class CreateDbClusterInputTypeDef(TypedDict):
    name: str,
    password: str,
    dbInstanceType: DbInstanceTypeType,  # (1)
    allocatedStorage: int,
    vpcSubnetIds: Sequence[str],
    vpcSecurityGroupIds: Sequence[str],
    deploymentType: ClusterDeploymentTypeType,  # (2)
    username: NotRequired[str],
    organization: NotRequired[str],
    bucket: NotRequired[str],
    port: NotRequired[int],
    dbParameterGroupIdentifier: NotRequired[str],
    dbStorageType: NotRequired[DbStorageTypeType],  # (3)
    networkType: NotRequired[NetworkTypeType],  # (4)
    publiclyAccessible: NotRequired[bool],
    failoverMode: NotRequired[FailoverModeType],  # (5)
    logDeliveryConfiguration: NotRequired[LogDeliveryConfigurationTypeDef],  # (6)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
2. See [:material-code-brackets: ClusterDeploymentTypeType](./literals.md#clusterdeploymenttypetype) 
3. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
4. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
5. See [:material-code-brackets: FailoverModeType](./literals.md#failovermodetype) 
6. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
## CreateDbInstanceInputTypeDef

```python
# CreateDbInstanceInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import CreateDbInstanceInputTypeDef


def get_value() -> CreateDbInstanceInputTypeDef:
    return {
        "name": ...,
    }


# CreateDbInstanceInputTypeDef definition

class CreateDbInstanceInputTypeDef(TypedDict):
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
    networkType: NotRequired[NetworkTypeType],  # (5)
```

1. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
2. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
3. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
4. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
5. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
## CreateDbInstanceOutputTypeDef

```python
# CreateDbInstanceOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import CreateDbInstanceOutputTypeDef


def get_value() -> CreateDbInstanceOutputTypeDef:
    return {
        "id": ...,
    }


# CreateDbInstanceOutputTypeDef definition

class CreateDbInstanceOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: StatusType,  # (1)
    endpoint: str,
    port: int,
    networkType: NetworkTypeType,  # (2)
    dbInstanceType: DbInstanceTypeType,  # (3)
    dbStorageType: DbStorageTypeType,  # (4)
    allocatedStorage: int,
    deploymentType: DeploymentTypeType,  # (5)
    vpcSubnetIds: List[str],
    publiclyAccessible: bool,
    vpcSecurityGroupIds: List[str],
    dbParameterGroupIdentifier: str,
    availabilityZone: str,
    secondaryAvailabilityZone: str,
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef,  # (6)
    influxAuthParametersSecretArn: str,
    dbClusterId: str,
    instanceMode: InstanceModeType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
3. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
4. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
5. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
6. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
7. See [:material-code-brackets: InstanceModeType](./literals.md#instancemodetype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDbInstanceOutputTypeDef

```python
# DeleteDbInstanceOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import DeleteDbInstanceOutputTypeDef


def get_value() -> DeleteDbInstanceOutputTypeDef:
    return {
        "id": ...,
    }


# DeleteDbInstanceOutputTypeDef definition

class DeleteDbInstanceOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: StatusType,  # (1)
    endpoint: str,
    port: int,
    networkType: NetworkTypeType,  # (2)
    dbInstanceType: DbInstanceTypeType,  # (3)
    dbStorageType: DbStorageTypeType,  # (4)
    allocatedStorage: int,
    deploymentType: DeploymentTypeType,  # (5)
    vpcSubnetIds: List[str],
    publiclyAccessible: bool,
    vpcSecurityGroupIds: List[str],
    dbParameterGroupIdentifier: str,
    availabilityZone: str,
    secondaryAvailabilityZone: str,
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef,  # (6)
    influxAuthParametersSecretArn: str,
    dbClusterId: str,
    instanceMode: InstanceModeType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
3. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
4. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
5. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
6. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
7. See [:material-code-brackets: InstanceModeType](./literals.md#instancemodetype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDbClusterOutputTypeDef

```python
# GetDbClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import GetDbClusterOutputTypeDef


def get_value() -> GetDbClusterOutputTypeDef:
    return {
        "id": ...,
    }


# GetDbClusterOutputTypeDef definition

class GetDbClusterOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: ClusterStatusType,  # (1)
    endpoint: str,
    readerEndpoint: str,
    port: int,
    deploymentType: ClusterDeploymentTypeType,  # (2)
    dbInstanceType: DbInstanceTypeType,  # (3)
    networkType: NetworkTypeType,  # (4)
    dbStorageType: DbStorageTypeType,  # (5)
    allocatedStorage: int,
    publiclyAccessible: bool,
    dbParameterGroupIdentifier: str,
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef,  # (6)
    influxAuthParametersSecretArn: str,
    vpcSubnetIds: List[str],
    vpcSecurityGroupIds: List[str],
    failoverMode: FailoverModeType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
2. See [:material-code-brackets: ClusterDeploymentTypeType](./literals.md#clusterdeploymenttypetype) 
3. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
4. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
5. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
6. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
7. See [:material-code-brackets: FailoverModeType](./literals.md#failovermodetype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDbInstanceOutputTypeDef

```python
# GetDbInstanceOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import GetDbInstanceOutputTypeDef


def get_value() -> GetDbInstanceOutputTypeDef:
    return {
        "id": ...,
    }


# GetDbInstanceOutputTypeDef definition

class GetDbInstanceOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: StatusType,  # (1)
    endpoint: str,
    port: int,
    networkType: NetworkTypeType,  # (2)
    dbInstanceType: DbInstanceTypeType,  # (3)
    dbStorageType: DbStorageTypeType,  # (4)
    allocatedStorage: int,
    deploymentType: DeploymentTypeType,  # (5)
    vpcSubnetIds: List[str],
    publiclyAccessible: bool,
    vpcSecurityGroupIds: List[str],
    dbParameterGroupIdentifier: str,
    availabilityZone: str,
    secondaryAvailabilityZone: str,
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef,  # (6)
    influxAuthParametersSecretArn: str,
    dbClusterId: str,
    instanceMode: InstanceModeType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
3. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
4. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
5. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
6. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
7. See [:material-code-brackets: InstanceModeType](./literals.md#instancemodetype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDbClusterInputTypeDef

```python
# UpdateDbClusterInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import UpdateDbClusterInputTypeDef


def get_value() -> UpdateDbClusterInputTypeDef:
    return {
        "dbClusterId": ...,
    }


# UpdateDbClusterInputTypeDef definition

class UpdateDbClusterInputTypeDef(TypedDict):
    dbClusterId: str,
    logDeliveryConfiguration: NotRequired[LogDeliveryConfigurationTypeDef],  # (1)
    dbParameterGroupIdentifier: NotRequired[str],
    port: NotRequired[int],
    dbInstanceType: NotRequired[DbInstanceTypeType],  # (2)
    failoverMode: NotRequired[FailoverModeType],  # (3)
```

1. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
2. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
3. See [:material-code-brackets: FailoverModeType](./literals.md#failovermodetype) 
## UpdateDbInstanceInputTypeDef

```python
# UpdateDbInstanceInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import UpdateDbInstanceInputTypeDef


def get_value() -> UpdateDbInstanceInputTypeDef:
    return {
        "identifier": ...,
    }


# UpdateDbInstanceInputTypeDef definition

class UpdateDbInstanceInputTypeDef(TypedDict):
    identifier: str,
    logDeliveryConfiguration: NotRequired[LogDeliveryConfigurationTypeDef],  # (1)
    dbParameterGroupIdentifier: NotRequired[str],
    port: NotRequired[int],
    dbInstanceType: NotRequired[DbInstanceTypeType],  # (2)
    deploymentType: NotRequired[DeploymentTypeType],  # (3)
    dbStorageType: NotRequired[DbStorageTypeType],  # (4)
    allocatedStorage: NotRequired[int],
```

1. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
2. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
3. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
4. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
## UpdateDbInstanceOutputTypeDef

```python
# UpdateDbInstanceOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import UpdateDbInstanceOutputTypeDef


def get_value() -> UpdateDbInstanceOutputTypeDef:
    return {
        "id": ...,
    }


# UpdateDbInstanceOutputTypeDef definition

class UpdateDbInstanceOutputTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    status: StatusType,  # (1)
    endpoint: str,
    port: int,
    networkType: NetworkTypeType,  # (2)
    dbInstanceType: DbInstanceTypeType,  # (3)
    dbStorageType: DbStorageTypeType,  # (4)
    allocatedStorage: int,
    deploymentType: DeploymentTypeType,  # (5)
    vpcSubnetIds: List[str],
    publiclyAccessible: bool,
    vpcSecurityGroupIds: List[str],
    dbParameterGroupIdentifier: str,
    availabilityZone: str,
    secondaryAvailabilityZone: str,
    logDeliveryConfiguration: LogDeliveryConfigurationTypeDef,  # (6)
    influxAuthParametersSecretArn: str,
    dbClusterId: str,
    instanceMode: InstanceModeType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: NetworkTypeType](./literals.md#networktypetype) 
3. See [:material-code-brackets: DbInstanceTypeType](./literals.md#dbinstancetypetype) 
4. See [:material-code-brackets: DbStorageTypeType](./literals.md#dbstoragetypetype) 
5. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
6. See [:material-code-braces: LogDeliveryConfigurationTypeDef](./type_defs.md#logdeliveryconfigurationtypedef) 
7. See [:material-code-brackets: InstanceModeType](./literals.md#instancemodetype) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDbParameterGroupInputTypeDef

```python
# CreateDbParameterGroupInputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import CreateDbParameterGroupInputTypeDef


def get_value() -> CreateDbParameterGroupInputTypeDef:
    return {
        "name": ...,
    }


# CreateDbParameterGroupInputTypeDef definition

class CreateDbParameterGroupInputTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    parameters: NotRequired[ParametersTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
## CreateDbParameterGroupOutputTypeDef

```python
# CreateDbParameterGroupOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import CreateDbParameterGroupOutputTypeDef


def get_value() -> CreateDbParameterGroupOutputTypeDef:
    return {
        "id": ...,
    }


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
# GetDbParameterGroupOutputTypeDef TypedDict usage example

from types_aiobotocore_timestream_influxdb.type_defs import GetDbParameterGroupOutputTypeDef


def get_value() -> GetDbParameterGroupOutputTypeDef:
    return {
        "id": ...,
    }


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
