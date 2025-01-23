# Type definitions

> [Index](../README.md) > [Finspace](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).

## KxDatabaseCacheConfigurationUnionTypeDef

```python
# KxDatabaseCacheConfigurationUnionTypeDef definition

KxDatabaseCacheConfigurationUnionTypeDef = Union[
    KxDatabaseCacheConfigurationTypeDef,  # (1)
    KxDatabaseCacheConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KxDatabaseCacheConfigurationTypeDef](./type_defs.md#kxdatabasecacheconfigurationtypedef) 
2. See [:material-code-braces: KxDatabaseCacheConfigurationOutputTypeDef](./type_defs.md#kxdatabasecacheconfigurationoutputtypedef) 

## KxDataviewSegmentConfigurationUnionTypeDef

```python
# KxDataviewSegmentConfigurationUnionTypeDef definition

KxDataviewSegmentConfigurationUnionTypeDef = Union[
    KxDataviewSegmentConfigurationTypeDef,  # (1)
    KxDataviewSegmentConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KxDataviewSegmentConfigurationTypeDef](./type_defs.md#kxdataviewsegmentconfigurationtypedef) 
2. See [:material-code-braces: KxDataviewSegmentConfigurationOutputTypeDef](./type_defs.md#kxdataviewsegmentconfigurationoutputtypedef) 

## KxDataviewConfigurationUnionTypeDef

```python
# KxDataviewConfigurationUnionTypeDef definition

KxDataviewConfigurationUnionTypeDef = Union[
    KxDataviewConfigurationTypeDef,  # (1)
    KxDataviewConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KxDataviewConfigurationTypeDef](./type_defs.md#kxdataviewconfigurationtypedef) 
2. See [:material-code-braces: KxDataviewConfigurationOutputTypeDef](./type_defs.md#kxdataviewconfigurationoutputtypedef) 

## KxDatabaseConfigurationUnionTypeDef

```python
# KxDatabaseConfigurationUnionTypeDef definition

KxDatabaseConfigurationUnionTypeDef = Union[
    KxDatabaseConfigurationTypeDef,  # (1)
    KxDatabaseConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef) 
2. See [:material-code-braces: KxDatabaseConfigurationOutputTypeDef](./type_defs.md#kxdatabaseconfigurationoutputtypedef) 



## AutoScalingConfigurationTypeDef

```python
# AutoScalingConfigurationTypeDef definition

class AutoScalingConfigurationTypeDef(TypedDict):
    minNodeCount: NotRequired[int],
    maxNodeCount: NotRequired[int],
    autoScalingMetric: NotRequired[AutoScalingMetricType],  # (1)
    metricTarget: NotRequired[float],
    scaleInCooldownSeconds: NotRequired[float],
    scaleOutCooldownSeconds: NotRequired[float],
```

1. See [:material-code-brackets: AutoScalingMetricType](./literals.md#autoscalingmetrictype) 
## CapacityConfigurationTypeDef

```python
# CapacityConfigurationTypeDef definition

class CapacityConfigurationTypeDef(TypedDict):
    nodeType: NotRequired[str],
    nodeCount: NotRequired[int],
```

## ChangeRequestTypeDef

```python
# ChangeRequestTypeDef definition

class ChangeRequestTypeDef(TypedDict):
    changeType: ChangeTypeType,  # (1)
    dbPath: str,
    s3Path: NotRequired[str],
```

1. See [:material-code-brackets: ChangeTypeType](./literals.md#changetypetype) 
## CodeConfigurationTypeDef

```python
# CodeConfigurationTypeDef definition

class CodeConfigurationTypeDef(TypedDict):
    s3Bucket: NotRequired[str],
    s3Key: NotRequired[str],
    s3ObjectVersion: NotRequired[str],
```

## FederationParametersTypeDef

```python
# FederationParametersTypeDef definition

class FederationParametersTypeDef(TypedDict):
    samlMetadataDocument: NotRequired[str],
    samlMetadataURL: NotRequired[str],
    applicationCallBackURL: NotRequired[str],
    federationURN: NotRequired[str],
    federationProviderName: NotRequired[str],
    attributeMap: NotRequired[Mapping[str, str]],
```

## SuperuserParametersTypeDef

```python
# SuperuserParametersTypeDef definition

class SuperuserParametersTypeDef(TypedDict):
    emailAddress: str,
    firstName: str,
    lastName: str,
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

## ErrorInfoTypeDef

```python
# ErrorInfoTypeDef definition

class ErrorInfoTypeDef(TypedDict):
    errorMessage: NotRequired[str],
    errorType: NotRequired[ErrorDetailsType],  # (1)
```

1. See [:material-code-brackets: ErrorDetailsType](./literals.md#errordetailstype) 
## KxCacheStorageConfigurationTypeDef

```python
# KxCacheStorageConfigurationTypeDef definition

class KxCacheStorageConfigurationTypeDef(TypedDict):
    type: str,
    size: int,
```

## KxCommandLineArgumentTypeDef

```python
# KxCommandLineArgumentTypeDef definition

class KxCommandLineArgumentTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## KxSavedownStorageConfigurationTypeDef

```python
# KxSavedownStorageConfigurationTypeDef definition

class KxSavedownStorageConfigurationTypeDef(TypedDict):
    type: NotRequired[KxSavedownStorageTypeType],  # (1)
    size: NotRequired[int],
    volumeName: NotRequired[str],
```

1. See [:material-code-brackets: KxSavedownStorageTypeType](./literals.md#kxsavedownstoragetypetype) 
## KxScalingGroupConfigurationTypeDef

```python
# KxScalingGroupConfigurationTypeDef definition

class KxScalingGroupConfigurationTypeDef(TypedDict):
    scalingGroupName: str,
    memoryReservation: int,
    nodeCount: int,
    memoryLimit: NotRequired[int],
    cpu: NotRequired[float],
```

## TickerplantLogConfigurationTypeDef

```python
# TickerplantLogConfigurationTypeDef definition

class TickerplantLogConfigurationTypeDef(TypedDict):
    tickerplantLogVolumes: NotRequired[Sequence[str]],
```

## VpcConfigurationTypeDef

```python
# VpcConfigurationTypeDef definition

class VpcConfigurationTypeDef(TypedDict):
    vpcId: NotRequired[str],
    securityGroupIds: NotRequired[Sequence[str]],
    subnetIds: NotRequired[Sequence[str]],
    ipAddressType: NotRequired[IPAddressTypeType],  # (1)
```

1. See [:material-code-brackets: IPAddressTypeType](./literals.md#ipaddresstypetype) 
## TickerplantLogConfigurationOutputTypeDef

```python
# TickerplantLogConfigurationOutputTypeDef definition

class TickerplantLogConfigurationOutputTypeDef(TypedDict):
    tickerplantLogVolumes: NotRequired[List[str]],
```

## VolumeTypeDef

```python
# VolumeTypeDef definition

class VolumeTypeDef(TypedDict):
    volumeName: NotRequired[str],
    volumeType: NotRequired[VolumeTypeType],  # (1)
```

1. See [:material-code-brackets: VolumeTypeType](./literals.md#volumetypetype) 
## VpcConfigurationOutputTypeDef

```python
# VpcConfigurationOutputTypeDef definition

class VpcConfigurationOutputTypeDef(TypedDict):
    vpcId: NotRequired[str],
    securityGroupIds: NotRequired[List[str]],
    subnetIds: NotRequired[List[str]],
    ipAddressType: NotRequired[IPAddressTypeType],  # (1)
```

1. See [:material-code-brackets: IPAddressTypeType](./literals.md#ipaddresstypetype) 
## CreateKxDatabaseRequestRequestTypeDef

```python
# CreateKxDatabaseRequestRequestTypeDef definition

class CreateKxDatabaseRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    clientToken: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## KxDataviewSegmentConfigurationOutputTypeDef

```python
# KxDataviewSegmentConfigurationOutputTypeDef definition

class KxDataviewSegmentConfigurationOutputTypeDef(TypedDict):
    dbPaths: List[str],
    volumeName: str,
    onDemand: NotRequired[bool],
```

## CreateKxEnvironmentRequestRequestTypeDef

```python
# CreateKxEnvironmentRequestRequestTypeDef definition

class CreateKxEnvironmentRequestRequestTypeDef(TypedDict):
    name: str,
    kmsKeyId: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
```

## CreateKxScalingGroupRequestRequestTypeDef

```python
# CreateKxScalingGroupRequestRequestTypeDef definition

class CreateKxScalingGroupRequestRequestTypeDef(TypedDict):
    clientToken: str,
    environmentId: str,
    scalingGroupName: str,
    hostType: str,
    availabilityZoneId: str,
    tags: NotRequired[Mapping[str, str]],
```

## CreateKxUserRequestRequestTypeDef

```python
# CreateKxUserRequestRequestTypeDef definition

class CreateKxUserRequestRequestTypeDef(TypedDict):
    environmentId: str,
    userName: str,
    iamRole: str,
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
```

## KxNAS1ConfigurationTypeDef

```python
# KxNAS1ConfigurationTypeDef definition

class KxNAS1ConfigurationTypeDef(TypedDict):
    type: NotRequired[KxNAS1TypeType],  # (1)
    size: NotRequired[int],
```

1. See [:material-code-brackets: KxNAS1TypeType](./literals.md#kxnas1typetype) 
## CustomDNSServerTypeDef

```python
# CustomDNSServerTypeDef definition

class CustomDNSServerTypeDef(TypedDict):
    customDNSServerName: str,
    customDNSServerIP: str,
```

## DeleteEnvironmentRequestRequestTypeDef

```python
# DeleteEnvironmentRequestRequestTypeDef definition

class DeleteEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
```

## DeleteKxClusterNodeRequestRequestTypeDef

```python
# DeleteKxClusterNodeRequestRequestTypeDef definition

class DeleteKxClusterNodeRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clusterName: str,
    nodeId: str,
```

## DeleteKxClusterRequestRequestTypeDef

```python
# DeleteKxClusterRequestRequestTypeDef definition

class DeleteKxClusterRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clusterName: str,
    clientToken: NotRequired[str],
```

## DeleteKxDatabaseRequestRequestTypeDef

```python
# DeleteKxDatabaseRequestRequestTypeDef definition

class DeleteKxDatabaseRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    clientToken: str,
```

## DeleteKxDataviewRequestRequestTypeDef

```python
# DeleteKxDataviewRequestRequestTypeDef definition

class DeleteKxDataviewRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    dataviewName: str,
    clientToken: str,
```

## DeleteKxEnvironmentRequestRequestTypeDef

```python
# DeleteKxEnvironmentRequestRequestTypeDef definition

class DeleteKxEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clientToken: NotRequired[str],
```

## DeleteKxScalingGroupRequestRequestTypeDef

```python
# DeleteKxScalingGroupRequestRequestTypeDef definition

class DeleteKxScalingGroupRequestRequestTypeDef(TypedDict):
    environmentId: str,
    scalingGroupName: str,
    clientToken: NotRequired[str],
```

## DeleteKxUserRequestRequestTypeDef

```python
# DeleteKxUserRequestRequestTypeDef definition

class DeleteKxUserRequestRequestTypeDef(TypedDict):
    userName: str,
    environmentId: str,
    clientToken: NotRequired[str],
```

## DeleteKxVolumeRequestRequestTypeDef

```python
# DeleteKxVolumeRequestRequestTypeDef definition

class DeleteKxVolumeRequestRequestTypeDef(TypedDict):
    environmentId: str,
    volumeName: str,
    clientToken: NotRequired[str],
```

## FederationParametersOutputTypeDef

```python
# FederationParametersOutputTypeDef definition

class FederationParametersOutputTypeDef(TypedDict):
    samlMetadataDocument: NotRequired[str],
    samlMetadataURL: NotRequired[str],
    applicationCallBackURL: NotRequired[str],
    federationURN: NotRequired[str],
    federationProviderName: NotRequired[str],
    attributeMap: NotRequired[Dict[str, str]],
```

## GetEnvironmentRequestRequestTypeDef

```python
# GetEnvironmentRequestRequestTypeDef definition

class GetEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
```

## GetKxChangesetRequestRequestTypeDef

```python
# GetKxChangesetRequestRequestTypeDef definition

class GetKxChangesetRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    changesetId: str,
```

## GetKxClusterRequestRequestTypeDef

```python
# GetKxClusterRequestRequestTypeDef definition

class GetKxClusterRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clusterName: str,
```

## GetKxConnectionStringRequestRequestTypeDef

```python
# GetKxConnectionStringRequestRequestTypeDef definition

class GetKxConnectionStringRequestRequestTypeDef(TypedDict):
    userArn: str,
    environmentId: str,
    clusterName: str,
```

## GetKxDatabaseRequestRequestTypeDef

```python
# GetKxDatabaseRequestRequestTypeDef definition

class GetKxDatabaseRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
```

## GetKxDataviewRequestRequestTypeDef

```python
# GetKxDataviewRequestRequestTypeDef definition

class GetKxDataviewRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    dataviewName: str,
```

## GetKxEnvironmentRequestRequestTypeDef

```python
# GetKxEnvironmentRequestRequestTypeDef definition

class GetKxEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
```

## GetKxScalingGroupRequestRequestTypeDef

```python
# GetKxScalingGroupRequestRequestTypeDef definition

class GetKxScalingGroupRequestRequestTypeDef(TypedDict):
    environmentId: str,
    scalingGroupName: str,
```

## GetKxUserRequestRequestTypeDef

```python
# GetKxUserRequestRequestTypeDef definition

class GetKxUserRequestRequestTypeDef(TypedDict):
    userName: str,
    environmentId: str,
```

## GetKxVolumeRequestRequestTypeDef

```python
# GetKxVolumeRequestRequestTypeDef definition

class GetKxVolumeRequestRequestTypeDef(TypedDict):
    environmentId: str,
    volumeName: str,
```

## KxAttachedClusterTypeDef

```python
# KxAttachedClusterTypeDef definition

class KxAttachedClusterTypeDef(TypedDict):
    clusterName: NotRequired[str],
    clusterType: NotRequired[KxClusterTypeType],  # (1)
    clusterStatus: NotRequired[KxClusterStatusType],  # (2)
```

1. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
2. See [:material-code-brackets: KxClusterStatusType](./literals.md#kxclusterstatustype) 
## IcmpTypeCodeTypeDef

```python
# IcmpTypeCodeTypeDef definition

class IcmpTypeCodeTypeDef(TypedDict):
    type: int,
    code: int,
```

## KxChangesetListEntryTypeDef

```python
# KxChangesetListEntryTypeDef definition

class KxChangesetListEntryTypeDef(TypedDict):
    changesetId: NotRequired[str],
    createdTimestamp: NotRequired[datetime],
    activeFromTimestamp: NotRequired[datetime],
    lastModifiedTimestamp: NotRequired[datetime],
    status: NotRequired[ChangesetStatusType],  # (1)
```

1. See [:material-code-brackets: ChangesetStatusType](./literals.md#changesetstatustype) 
## KxClusterCodeDeploymentConfigurationTypeDef

```python
# KxClusterCodeDeploymentConfigurationTypeDef definition

class KxClusterCodeDeploymentConfigurationTypeDef(TypedDict):
    deploymentStrategy: KxClusterCodeDeploymentStrategyType,  # (1)
```

1. See [:material-code-brackets: KxClusterCodeDeploymentStrategyType](./literals.md#kxclustercodedeploymentstrategytype) 
## KxDatabaseCacheConfigurationOutputTypeDef

```python
# KxDatabaseCacheConfigurationOutputTypeDef definition

class KxDatabaseCacheConfigurationOutputTypeDef(TypedDict):
    cacheType: str,
    dbPaths: List[str],
    dataviewName: NotRequired[str],
```

## KxDatabaseCacheConfigurationTypeDef

```python
# KxDatabaseCacheConfigurationTypeDef definition

class KxDatabaseCacheConfigurationTypeDef(TypedDict):
    cacheType: str,
    dbPaths: Sequence[str],
    dataviewName: NotRequired[str],
```

## KxDatabaseListEntryTypeDef

```python
# KxDatabaseListEntryTypeDef definition

class KxDatabaseListEntryTypeDef(TypedDict):
    databaseName: NotRequired[str],
    createdTimestamp: NotRequired[datetime],
    lastModifiedTimestamp: NotRequired[datetime],
```

## KxDataviewSegmentConfigurationTypeDef

```python
# KxDataviewSegmentConfigurationTypeDef definition

class KxDataviewSegmentConfigurationTypeDef(TypedDict):
    dbPaths: Sequence[str],
    volumeName: str,
    onDemand: NotRequired[bool],
```

## KxDeploymentConfigurationTypeDef

```python
# KxDeploymentConfigurationTypeDef definition

class KxDeploymentConfigurationTypeDef(TypedDict):
    deploymentStrategy: KxDeploymentStrategyType,  # (1)
```

1. See [:material-code-brackets: KxDeploymentStrategyType](./literals.md#kxdeploymentstrategytype) 
## KxNodeTypeDef

```python
# KxNodeTypeDef definition

class KxNodeTypeDef(TypedDict):
    nodeId: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    launchTime: NotRequired[datetime],
    status: NotRequired[KxNodeStatusType],  # (1)
```

1. See [:material-code-brackets: KxNodeStatusType](./literals.md#kxnodestatustype) 
## KxScalingGroupTypeDef

```python
# KxScalingGroupTypeDef definition

class KxScalingGroupTypeDef(TypedDict):
    scalingGroupName: NotRequired[str],
    hostType: NotRequired[str],
    clusters: NotRequired[List[str]],
    availabilityZoneId: NotRequired[str],
    status: NotRequired[KxScalingGroupStatusType],  # (1)
    statusReason: NotRequired[str],
    lastModifiedTimestamp: NotRequired[datetime],
    createdTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: KxScalingGroupStatusType](./literals.md#kxscalinggroupstatustype) 
## KxUserTypeDef

```python
# KxUserTypeDef definition

class KxUserTypeDef(TypedDict):
    userArn: NotRequired[str],
    userName: NotRequired[str],
    iamRole: NotRequired[str],
    createTimestamp: NotRequired[datetime],
    updateTimestamp: NotRequired[datetime],
```

## KxVolumeTypeDef

```python
# KxVolumeTypeDef definition

class KxVolumeTypeDef(TypedDict):
    volumeName: NotRequired[str],
    volumeType: NotRequired[KxVolumeTypeType],  # (1)
    status: NotRequired[KxVolumeStatusType],  # (2)
    description: NotRequired[str],
    statusReason: NotRequired[str],
    azMode: NotRequired[KxAzModeType],  # (3)
    availabilityZoneIds: NotRequired[List[str]],
    createdTimestamp: NotRequired[datetime],
    lastModifiedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: KxVolumeTypeType](./literals.md#kxvolumetypetype) 
2. See [:material-code-brackets: KxVolumeStatusType](./literals.md#kxvolumestatustype) 
3. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
## ListEnvironmentsRequestRequestTypeDef

```python
# ListEnvironmentsRequestRequestTypeDef definition

class ListEnvironmentsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListKxChangesetsRequestRequestTypeDef

```python
# ListKxChangesetsRequestRequestTypeDef definition

class ListKxChangesetsRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListKxClusterNodesRequestRequestTypeDef

```python
# ListKxClusterNodesRequestRequestTypeDef definition

class ListKxClusterNodesRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clusterName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListKxClustersRequestRequestTypeDef

```python
# ListKxClustersRequestRequestTypeDef definition

class ListKxClustersRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clusterType: NotRequired[KxClusterTypeType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
## ListKxDatabasesRequestRequestTypeDef

```python
# ListKxDatabasesRequestRequestTypeDef definition

class ListKxDatabasesRequestRequestTypeDef(TypedDict):
    environmentId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListKxDataviewsRequestRequestTypeDef

```python
# ListKxDataviewsRequestRequestTypeDef definition

class ListKxDataviewsRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListKxEnvironmentsRequestRequestTypeDef

```python
# ListKxEnvironmentsRequestRequestTypeDef definition

class ListKxEnvironmentsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListKxScalingGroupsRequestRequestTypeDef

```python
# ListKxScalingGroupsRequestRequestTypeDef definition

class ListKxScalingGroupsRequestRequestTypeDef(TypedDict):
    environmentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListKxUsersRequestRequestTypeDef

```python
# ListKxUsersRequestRequestTypeDef definition

class ListKxUsersRequestRequestTypeDef(TypedDict):
    environmentId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListKxVolumesRequestRequestTypeDef

```python
# ListKxVolumesRequestRequestTypeDef definition

class ListKxVolumesRequestRequestTypeDef(TypedDict):
    environmentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    volumeType: NotRequired[KxVolumeTypeType],  # (1)
```

1. See [:material-code-brackets: KxVolumeTypeType](./literals.md#kxvolumetypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## PortRangeTypeDef

```python
# PortRangeTypeDef definition

class PortRangeTypeDef(TypedDict):
    from: int,
    to: int,
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

## UpdateKxDatabaseRequestRequestTypeDef

```python
# UpdateKxDatabaseRequestRequestTypeDef definition

class UpdateKxDatabaseRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    clientToken: str,
    description: NotRequired[str],
```

## UpdateKxEnvironmentRequestRequestTypeDef

```python
# UpdateKxEnvironmentRequestRequestTypeDef definition

class UpdateKxEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
    name: NotRequired[str],
    description: NotRequired[str],
    clientToken: NotRequired[str],
```

## UpdateKxUserRequestRequestTypeDef

```python
# UpdateKxUserRequestRequestTypeDef definition

class UpdateKxUserRequestRequestTypeDef(TypedDict):
    environmentId: str,
    userName: str,
    iamRole: str,
    clientToken: NotRequired[str],
```

## CreateKxChangesetRequestRequestTypeDef

```python
# CreateKxChangesetRequestRequestTypeDef definition

class CreateKxChangesetRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    changeRequests: Sequence[ChangeRequestTypeDef],  # (1)
    clientToken: str,
```

1. See [:material-code-braces: ChangeRequestTypeDef](./type_defs.md#changerequesttypedef) 
## UpdateEnvironmentRequestRequestTypeDef

```python
# UpdateEnvironmentRequestRequestTypeDef definition

class UpdateEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
    name: NotRequired[str],
    description: NotRequired[str],
    federationMode: NotRequired[FederationModeType],  # (1)
    federationParameters: NotRequired[FederationParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: FederationModeType](./literals.md#federationmodetype) 
2. See [:material-code-braces: FederationParametersTypeDef](./type_defs.md#federationparameterstypedef) 
## CreateEnvironmentRequestRequestTypeDef

```python
# CreateEnvironmentRequestRequestTypeDef definition

class CreateEnvironmentRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    kmsKeyId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    federationMode: NotRequired[FederationModeType],  # (1)
    federationParameters: NotRequired[FederationParametersTypeDef],  # (2)
    superuserParameters: NotRequired[SuperuserParametersTypeDef],  # (3)
    dataBundles: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: FederationModeType](./literals.md#federationmodetype) 
2. See [:material-code-braces: FederationParametersTypeDef](./type_defs.md#federationparameterstypedef) 
3. See [:material-code-braces: SuperuserParametersTypeDef](./type_defs.md#superuserparameterstypedef) 
## CreateEnvironmentResponseTypeDef

```python
# CreateEnvironmentResponseTypeDef definition

class CreateEnvironmentResponseTypeDef(TypedDict):
    environmentId: str,
    environmentArn: str,
    environmentUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKxDatabaseResponseTypeDef

```python
# CreateKxDatabaseResponseTypeDef definition

class CreateKxDatabaseResponseTypeDef(TypedDict):
    databaseName: str,
    databaseArn: str,
    environmentId: str,
    description: str,
    createdTimestamp: datetime,
    lastModifiedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKxEnvironmentResponseTypeDef

```python
# CreateKxEnvironmentResponseTypeDef definition

class CreateKxEnvironmentResponseTypeDef(TypedDict):
    name: str,
    status: EnvironmentStatusType,  # (1)
    environmentId: str,
    description: str,
    environmentArn: str,
    kmsKeyId: str,
    creationTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKxScalingGroupResponseTypeDef

```python
# CreateKxScalingGroupResponseTypeDef definition

class CreateKxScalingGroupResponseTypeDef(TypedDict):
    environmentId: str,
    scalingGroupName: str,
    hostType: str,
    availabilityZoneId: str,
    status: KxScalingGroupStatusType,  # (1)
    lastModifiedTimestamp: datetime,
    createdTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: KxScalingGroupStatusType](./literals.md#kxscalinggroupstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKxUserResponseTypeDef

```python
# CreateKxUserResponseTypeDef definition

class CreateKxUserResponseTypeDef(TypedDict):
    userName: str,
    userArn: str,
    environmentId: str,
    iamRole: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKxConnectionStringResponseTypeDef

```python
# GetKxConnectionStringResponseTypeDef definition

class GetKxConnectionStringResponseTypeDef(TypedDict):
    signedConnectionString: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKxDatabaseResponseTypeDef

```python
# GetKxDatabaseResponseTypeDef definition

class GetKxDatabaseResponseTypeDef(TypedDict):
    databaseName: str,
    databaseArn: str,
    environmentId: str,
    description: str,
    createdTimestamp: datetime,
    lastModifiedTimestamp: datetime,
    lastCompletedChangesetId: str,
    numBytes: int,
    numChangesets: int,
    numFiles: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKxScalingGroupResponseTypeDef

```python
# GetKxScalingGroupResponseTypeDef definition

class GetKxScalingGroupResponseTypeDef(TypedDict):
    scalingGroupName: str,
    scalingGroupArn: str,
    hostType: str,
    clusters: List[str],
    availabilityZoneId: str,
    status: KxScalingGroupStatusType,  # (1)
    statusReason: str,
    lastModifiedTimestamp: datetime,
    createdTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: KxScalingGroupStatusType](./literals.md#kxscalinggroupstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKxUserResponseTypeDef

```python
# GetKxUserResponseTypeDef definition

class GetKxUserResponseTypeDef(TypedDict):
    userName: str,
    userArn: str,
    environmentId: str,
    iamRole: str,
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
## UpdateKxDatabaseResponseTypeDef

```python
# UpdateKxDatabaseResponseTypeDef definition

class UpdateKxDatabaseResponseTypeDef(TypedDict):
    databaseName: str,
    environmentId: str,
    description: str,
    lastModifiedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKxUserResponseTypeDef

```python
# UpdateKxUserResponseTypeDef definition

class UpdateKxUserResponseTypeDef(TypedDict):
    userName: str,
    userArn: str,
    environmentId: str,
    iamRole: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKxChangesetResponseTypeDef

```python
# CreateKxChangesetResponseTypeDef definition

class CreateKxChangesetResponseTypeDef(TypedDict):
    changesetId: str,
    databaseName: str,
    environmentId: str,
    changeRequests: List[ChangeRequestTypeDef],  # (1)
    createdTimestamp: datetime,
    lastModifiedTimestamp: datetime,
    status: ChangesetStatusType,  # (2)
    errorInfo: ErrorInfoTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ChangeRequestTypeDef](./type_defs.md#changerequesttypedef) 
2. See [:material-code-brackets: ChangesetStatusType](./literals.md#changesetstatustype) 
3. See [:material-code-braces: ErrorInfoTypeDef](./type_defs.md#errorinfotypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKxChangesetResponseTypeDef

```python
# GetKxChangesetResponseTypeDef definition

class GetKxChangesetResponseTypeDef(TypedDict):
    changesetId: str,
    databaseName: str,
    environmentId: str,
    changeRequests: List[ChangeRequestTypeDef],  # (1)
    createdTimestamp: datetime,
    activeFromTimestamp: datetime,
    lastModifiedTimestamp: datetime,
    status: ChangesetStatusType,  # (2)
    errorInfo: ErrorInfoTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ChangeRequestTypeDef](./type_defs.md#changerequesttypedef) 
2. See [:material-code-brackets: ChangesetStatusType](./literals.md#changesetstatustype) 
3. See [:material-code-braces: ErrorInfoTypeDef](./type_defs.md#errorinfotypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KxClusterTypeDef

```python
# KxClusterTypeDef definition

class KxClusterTypeDef(TypedDict):
    status: NotRequired[KxClusterStatusType],  # (1)
    statusReason: NotRequired[str],
    clusterName: NotRequired[str],
    clusterType: NotRequired[KxClusterTypeType],  # (2)
    clusterDescription: NotRequired[str],
    releaseLabel: NotRequired[str],
    volumes: NotRequired[List[VolumeTypeDef]],  # (3)
    initializationScript: NotRequired[str],
    executionRole: NotRequired[str],
    azMode: NotRequired[KxAzModeType],  # (4)
    availabilityZoneId: NotRequired[str],
    lastModifiedTimestamp: NotRequired[datetime],
    createdTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: KxClusterStatusType](./literals.md#kxclusterstatustype) 
2. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
3. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
4. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
## CreateKxDataviewResponseTypeDef

```python
# CreateKxDataviewResponseTypeDef definition

class CreateKxDataviewResponseTypeDef(TypedDict):
    dataviewName: str,
    databaseName: str,
    environmentId: str,
    azMode: KxAzModeType,  # (1)
    availabilityZoneId: str,
    changesetId: str,
    segmentConfigurations: List[KxDataviewSegmentConfigurationOutputTypeDef],  # (2)
    description: str,
    autoUpdate: bool,
    readWrite: bool,
    createdTimestamp: datetime,
    lastModifiedTimestamp: datetime,
    status: KxDataviewStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
2. See [:material-code-braces: KxDataviewSegmentConfigurationOutputTypeDef](./type_defs.md#kxdataviewsegmentconfigurationoutputtypedef) 
3. See [:material-code-brackets: KxDataviewStatusType](./literals.md#kxdataviewstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KxDataviewActiveVersionTypeDef

```python
# KxDataviewActiveVersionTypeDef definition

class KxDataviewActiveVersionTypeDef(TypedDict):
    changesetId: NotRequired[str],
    segmentConfigurations: NotRequired[List[KxDataviewSegmentConfigurationOutputTypeDef]],  # (1)
    attachedClusters: NotRequired[List[str]],
    createdTimestamp: NotRequired[datetime],
    versionId: NotRequired[str],
```

1. See [:material-code-braces: KxDataviewSegmentConfigurationOutputTypeDef](./type_defs.md#kxdataviewsegmentconfigurationoutputtypedef) 
## KxDataviewConfigurationOutputTypeDef

```python
# KxDataviewConfigurationOutputTypeDef definition

class KxDataviewConfigurationOutputTypeDef(TypedDict):
    dataviewName: NotRequired[str],
    dataviewVersionId: NotRequired[str],
    changesetId: NotRequired[str],
    segmentConfigurations: NotRequired[List[KxDataviewSegmentConfigurationOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: KxDataviewSegmentConfigurationOutputTypeDef](./type_defs.md#kxdataviewsegmentconfigurationoutputtypedef) 
## CreateKxVolumeRequestRequestTypeDef

```python
# CreateKxVolumeRequestRequestTypeDef definition

class CreateKxVolumeRequestRequestTypeDef(TypedDict):
    environmentId: str,
    volumeType: KxVolumeTypeType,  # (1)
    volumeName: str,
    azMode: KxAzModeType,  # (2)
    availabilityZoneIds: Sequence[str],
    clientToken: NotRequired[str],
    description: NotRequired[str],
    nas1Configuration: NotRequired[KxNAS1ConfigurationTypeDef],  # (3)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: KxVolumeTypeType](./literals.md#kxvolumetypetype) 
2. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
3. See [:material-code-braces: KxNAS1ConfigurationTypeDef](./type_defs.md#kxnas1configurationtypedef) 
## CreateKxVolumeResponseTypeDef

```python
# CreateKxVolumeResponseTypeDef definition

class CreateKxVolumeResponseTypeDef(TypedDict):
    environmentId: str,
    volumeName: str,
    volumeType: KxVolumeTypeType,  # (1)
    volumeArn: str,
    nas1Configuration: KxNAS1ConfigurationTypeDef,  # (2)
    status: KxVolumeStatusType,  # (3)
    statusReason: str,
    azMode: KxAzModeType,  # (4)
    description: str,
    availabilityZoneIds: List[str],
    createdTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: KxVolumeTypeType](./literals.md#kxvolumetypetype) 
2. See [:material-code-braces: KxNAS1ConfigurationTypeDef](./type_defs.md#kxnas1configurationtypedef) 
3. See [:material-code-brackets: KxVolumeStatusType](./literals.md#kxvolumestatustype) 
4. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKxVolumeRequestRequestTypeDef

```python
# UpdateKxVolumeRequestRequestTypeDef definition

class UpdateKxVolumeRequestRequestTypeDef(TypedDict):
    environmentId: str,
    volumeName: str,
    description: NotRequired[str],
    clientToken: NotRequired[str],
    nas1Configuration: NotRequired[KxNAS1ConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: KxNAS1ConfigurationTypeDef](./type_defs.md#kxnas1configurationtypedef) 
## EnvironmentTypeDef

```python
# EnvironmentTypeDef definition

class EnvironmentTypeDef(TypedDict):
    name: NotRequired[str],
    environmentId: NotRequired[str],
    awsAccountId: NotRequired[str],
    status: NotRequired[EnvironmentStatusType],  # (1)
    environmentUrl: NotRequired[str],
    description: NotRequired[str],
    environmentArn: NotRequired[str],
    sageMakerStudioDomainUrl: NotRequired[str],
    kmsKeyId: NotRequired[str],
    dedicatedServiceAccountId: NotRequired[str],
    federationMode: NotRequired[FederationModeType],  # (2)
    federationParameters: NotRequired[FederationParametersOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: FederationModeType](./literals.md#federationmodetype) 
3. See [:material-code-braces: FederationParametersOutputTypeDef](./type_defs.md#federationparametersoutputtypedef) 
## GetKxVolumeResponseTypeDef

```python
# GetKxVolumeResponseTypeDef definition

class GetKxVolumeResponseTypeDef(TypedDict):
    environmentId: str,
    volumeName: str,
    volumeType: KxVolumeTypeType,  # (1)
    volumeArn: str,
    nas1Configuration: KxNAS1ConfigurationTypeDef,  # (2)
    status: KxVolumeStatusType,  # (3)
    statusReason: str,
    createdTimestamp: datetime,
    description: str,
    azMode: KxAzModeType,  # (4)
    availabilityZoneIds: List[str],
    lastModifiedTimestamp: datetime,
    attachedClusters: List[KxAttachedClusterTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: KxVolumeTypeType](./literals.md#kxvolumetypetype) 
2. See [:material-code-braces: KxNAS1ConfigurationTypeDef](./type_defs.md#kxnas1configurationtypedef) 
3. See [:material-code-brackets: KxVolumeStatusType](./literals.md#kxvolumestatustype) 
4. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
5. See [:material-code-braces: KxAttachedClusterTypeDef](./type_defs.md#kxattachedclustertypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKxVolumeResponseTypeDef

```python
# UpdateKxVolumeResponseTypeDef definition

class UpdateKxVolumeResponseTypeDef(TypedDict):
    environmentId: str,
    volumeName: str,
    volumeType: KxVolumeTypeType,  # (1)
    volumeArn: str,
    nas1Configuration: KxNAS1ConfigurationTypeDef,  # (2)
    status: KxVolumeStatusType,  # (3)
    description: str,
    statusReason: str,
    createdTimestamp: datetime,
    azMode: KxAzModeType,  # (4)
    availabilityZoneIds: List[str],
    lastModifiedTimestamp: datetime,
    attachedClusters: List[KxAttachedClusterTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: KxVolumeTypeType](./literals.md#kxvolumetypetype) 
2. See [:material-code-braces: KxNAS1ConfigurationTypeDef](./type_defs.md#kxnas1configurationtypedef) 
3. See [:material-code-brackets: KxVolumeStatusType](./literals.md#kxvolumestatustype) 
4. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
5. See [:material-code-braces: KxAttachedClusterTypeDef](./type_defs.md#kxattachedclustertypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKxChangesetsResponseTypeDef

```python
# ListKxChangesetsResponseTypeDef definition

class ListKxChangesetsResponseTypeDef(TypedDict):
    kxChangesets: List[KxChangesetListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KxChangesetListEntryTypeDef](./type_defs.md#kxchangesetlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKxClusterCodeConfigurationRequestRequestTypeDef

```python
# UpdateKxClusterCodeConfigurationRequestRequestTypeDef definition

class UpdateKxClusterCodeConfigurationRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clusterName: str,
    code: CodeConfigurationTypeDef,  # (1)
    clientToken: NotRequired[str],
    initializationScript: NotRequired[str],
    commandLineArguments: NotRequired[Sequence[KxCommandLineArgumentTypeDef]],  # (2)
    deploymentConfiguration: NotRequired[KxClusterCodeDeploymentConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: CodeConfigurationTypeDef](./type_defs.md#codeconfigurationtypedef) 
2. See [:material-code-braces: KxCommandLineArgumentTypeDef](./type_defs.md#kxcommandlineargumenttypedef) 
3. See [:material-code-braces: KxClusterCodeDeploymentConfigurationTypeDef](./type_defs.md#kxclustercodedeploymentconfigurationtypedef) 
## ListKxDatabasesResponseTypeDef

```python
# ListKxDatabasesResponseTypeDef definition

class ListKxDatabasesResponseTypeDef(TypedDict):
    kxDatabases: List[KxDatabaseListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KxDatabaseListEntryTypeDef](./type_defs.md#kxdatabaselistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKxDataviewRequestRequestTypeDef

```python
# UpdateKxDataviewRequestRequestTypeDef definition

class UpdateKxDataviewRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    dataviewName: str,
    clientToken: str,
    description: NotRequired[str],
    changesetId: NotRequired[str],
    segmentConfigurations: NotRequired[Sequence[KxDataviewSegmentConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: KxDataviewSegmentConfigurationTypeDef](./type_defs.md#kxdataviewsegmentconfigurationtypedef) 
## ListKxClusterNodesResponseTypeDef

```python
# ListKxClusterNodesResponseTypeDef definition

class ListKxClusterNodesResponseTypeDef(TypedDict):
    nodes: List[KxNodeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KxNodeTypeDef](./type_defs.md#kxnodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKxScalingGroupsResponseTypeDef

```python
# ListKxScalingGroupsResponseTypeDef definition

class ListKxScalingGroupsResponseTypeDef(TypedDict):
    scalingGroups: List[KxScalingGroupTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KxScalingGroupTypeDef](./type_defs.md#kxscalinggrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKxUsersResponseTypeDef

```python
# ListKxUsersResponseTypeDef definition

class ListKxUsersResponseTypeDef(TypedDict):
    users: List[KxUserTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KxUserTypeDef](./type_defs.md#kxusertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKxVolumesResponseTypeDef

```python
# ListKxVolumesResponseTypeDef definition

class ListKxVolumesResponseTypeDef(TypedDict):
    kxVolumeSummaries: List[KxVolumeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KxVolumeTypeDef](./type_defs.md#kxvolumetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKxEnvironmentsRequestPaginateTypeDef

```python
# ListKxEnvironmentsRequestPaginateTypeDef definition

class ListKxEnvironmentsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## NetworkACLEntryTypeDef

```python
# NetworkACLEntryTypeDef definition

class NetworkACLEntryTypeDef(TypedDict):
    ruleNumber: int,
    protocol: str,
    ruleAction: RuleActionType,  # (1)
    cidrBlock: str,
    portRange: NotRequired[PortRangeTypeDef],  # (2)
    icmpTypeCode: NotRequired[IcmpTypeCodeTypeDef],  # (3)
```

1. See [:material-code-brackets: RuleActionType](./literals.md#ruleactiontype) 
2. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
3. See [:material-code-braces: IcmpTypeCodeTypeDef](./type_defs.md#icmptypecodetypedef) 
## ListKxClustersResponseTypeDef

```python
# ListKxClustersResponseTypeDef definition

class ListKxClustersResponseTypeDef(TypedDict):
    kxClusterSummaries: List[KxClusterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KxClusterTypeDef](./type_defs.md#kxclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKxDataviewResponseTypeDef

```python
# GetKxDataviewResponseTypeDef definition

class GetKxDataviewResponseTypeDef(TypedDict):
    databaseName: str,
    dataviewName: str,
    azMode: KxAzModeType,  # (1)
    availabilityZoneId: str,
    changesetId: str,
    segmentConfigurations: List[KxDataviewSegmentConfigurationOutputTypeDef],  # (2)
    activeVersions: List[KxDataviewActiveVersionTypeDef],  # (3)
    description: str,
    autoUpdate: bool,
    readWrite: bool,
    environmentId: str,
    createdTimestamp: datetime,
    lastModifiedTimestamp: datetime,
    status: KxDataviewStatusType,  # (4)
    statusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
2. See [:material-code-braces: KxDataviewSegmentConfigurationOutputTypeDef](./type_defs.md#kxdataviewsegmentconfigurationoutputtypedef) 
3. See [:material-code-braces: KxDataviewActiveVersionTypeDef](./type_defs.md#kxdataviewactiveversiontypedef) 
4. See [:material-code-brackets: KxDataviewStatusType](./literals.md#kxdataviewstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KxDataviewListEntryTypeDef

```python
# KxDataviewListEntryTypeDef definition

class KxDataviewListEntryTypeDef(TypedDict):
    environmentId: NotRequired[str],
    databaseName: NotRequired[str],
    dataviewName: NotRequired[str],
    azMode: NotRequired[KxAzModeType],  # (1)
    availabilityZoneId: NotRequired[str],
    changesetId: NotRequired[str],
    segmentConfigurations: NotRequired[List[KxDataviewSegmentConfigurationOutputTypeDef]],  # (2)
    activeVersions: NotRequired[List[KxDataviewActiveVersionTypeDef]],  # (3)
    status: NotRequired[KxDataviewStatusType],  # (4)
    description: NotRequired[str],
    autoUpdate: NotRequired[bool],
    readWrite: NotRequired[bool],
    createdTimestamp: NotRequired[datetime],
    lastModifiedTimestamp: NotRequired[datetime],
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
2. See [:material-code-braces: KxDataviewSegmentConfigurationOutputTypeDef](./type_defs.md#kxdataviewsegmentconfigurationoutputtypedef) 
3. See [:material-code-braces: KxDataviewActiveVersionTypeDef](./type_defs.md#kxdataviewactiveversiontypedef) 
4. See [:material-code-brackets: KxDataviewStatusType](./literals.md#kxdataviewstatustype) 
## UpdateKxDataviewResponseTypeDef

```python
# UpdateKxDataviewResponseTypeDef definition

class UpdateKxDataviewResponseTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    dataviewName: str,
    azMode: KxAzModeType,  # (1)
    availabilityZoneId: str,
    changesetId: str,
    segmentConfigurations: List[KxDataviewSegmentConfigurationOutputTypeDef],  # (2)
    activeVersions: List[KxDataviewActiveVersionTypeDef],  # (3)
    status: KxDataviewStatusType,  # (4)
    autoUpdate: bool,
    readWrite: bool,
    description: str,
    createdTimestamp: datetime,
    lastModifiedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
2. See [:material-code-braces: KxDataviewSegmentConfigurationOutputTypeDef](./type_defs.md#kxdataviewsegmentconfigurationoutputtypedef) 
3. See [:material-code-braces: KxDataviewActiveVersionTypeDef](./type_defs.md#kxdataviewactiveversiontypedef) 
4. See [:material-code-brackets: KxDataviewStatusType](./literals.md#kxdataviewstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KxDatabaseConfigurationOutputTypeDef

```python
# KxDatabaseConfigurationOutputTypeDef definition

class KxDatabaseConfigurationOutputTypeDef(TypedDict):
    databaseName: str,
    cacheConfigurations: NotRequired[List[KxDatabaseCacheConfigurationOutputTypeDef]],  # (1)
    changesetId: NotRequired[str],
    dataviewName: NotRequired[str],
    dataviewConfiguration: NotRequired[KxDataviewConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: KxDatabaseCacheConfigurationOutputTypeDef](./type_defs.md#kxdatabasecacheconfigurationoutputtypedef) 
2. See [:material-code-braces: KxDataviewConfigurationOutputTypeDef](./type_defs.md#kxdataviewconfigurationoutputtypedef) 
## GetEnvironmentResponseTypeDef

```python
# GetEnvironmentResponseTypeDef definition

class GetEnvironmentResponseTypeDef(TypedDict):
    environment: EnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentsResponseTypeDef

```python
# ListEnvironmentsResponseTypeDef definition

class ListEnvironmentsResponseTypeDef(TypedDict):
    environments: List[EnvironmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentResponseTypeDef

```python
# UpdateEnvironmentResponseTypeDef definition

class UpdateEnvironmentResponseTypeDef(TypedDict):
    environment: EnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKxDataviewRequestRequestTypeDef

```python
# CreateKxDataviewRequestRequestTypeDef definition

class CreateKxDataviewRequestRequestTypeDef(TypedDict):
    environmentId: str,
    databaseName: str,
    dataviewName: str,
    azMode: KxAzModeType,  # (1)
    clientToken: str,
    availabilityZoneId: NotRequired[str],
    changesetId: NotRequired[str],
    segmentConfigurations: NotRequired[Sequence[KxDataviewSegmentConfigurationUnionTypeDef]],  # (2)
    autoUpdate: NotRequired[bool],
    readWrite: NotRequired[bool],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
2. See [:material-code-braces: KxDataviewSegmentConfigurationTypeDef](./type_defs.md#kxdataviewsegmentconfigurationtypedef) [:material-code-braces: KxDataviewSegmentConfigurationOutputTypeDef](./type_defs.md#kxdataviewsegmentconfigurationoutputtypedef) 
## KxDataviewConfigurationTypeDef

```python
# KxDataviewConfigurationTypeDef definition

class KxDataviewConfigurationTypeDef(TypedDict):
    dataviewName: NotRequired[str],
    dataviewVersionId: NotRequired[str],
    changesetId: NotRequired[str],
    segmentConfigurations: NotRequired[Sequence[KxDataviewSegmentConfigurationUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: KxDataviewSegmentConfigurationTypeDef](./type_defs.md#kxdataviewsegmentconfigurationtypedef) [:material-code-braces: KxDataviewSegmentConfigurationOutputTypeDef](./type_defs.md#kxdataviewsegmentconfigurationoutputtypedef) 
## TransitGatewayConfigurationOutputTypeDef

```python
# TransitGatewayConfigurationOutputTypeDef definition

class TransitGatewayConfigurationOutputTypeDef(TypedDict):
    transitGatewayID: str,
    routableCIDRSpace: str,
    attachmentNetworkAclConfiguration: NotRequired[List[NetworkACLEntryTypeDef]],  # (1)
```

1. See [:material-code-braces: NetworkACLEntryTypeDef](./type_defs.md#networkaclentrytypedef) 
## TransitGatewayConfigurationTypeDef

```python
# TransitGatewayConfigurationTypeDef definition

class TransitGatewayConfigurationTypeDef(TypedDict):
    transitGatewayID: str,
    routableCIDRSpace: str,
    attachmentNetworkAclConfiguration: NotRequired[Sequence[NetworkACLEntryTypeDef]],  # (1)
```

1. See [:material-code-braces: NetworkACLEntryTypeDef](./type_defs.md#networkaclentrytypedef) 
## ListKxDataviewsResponseTypeDef

```python
# ListKxDataviewsResponseTypeDef definition

class ListKxDataviewsResponseTypeDef(TypedDict):
    kxDataviews: List[KxDataviewListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KxDataviewListEntryTypeDef](./type_defs.md#kxdataviewlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKxClusterResponseTypeDef

```python
# CreateKxClusterResponseTypeDef definition

class CreateKxClusterResponseTypeDef(TypedDict):
    environmentId: str,
    status: KxClusterStatusType,  # (1)
    statusReason: str,
    clusterName: str,
    clusterType: KxClusterTypeType,  # (2)
    tickerplantLogConfiguration: TickerplantLogConfigurationOutputTypeDef,  # (3)
    volumes: List[VolumeTypeDef],  # (4)
    databases: List[KxDatabaseConfigurationOutputTypeDef],  # (5)
    cacheStorageConfigurations: List[KxCacheStorageConfigurationTypeDef],  # (6)
    autoScalingConfiguration: AutoScalingConfigurationTypeDef,  # (7)
    clusterDescription: str,
    capacityConfiguration: CapacityConfigurationTypeDef,  # (8)
    releaseLabel: str,
    vpcConfiguration: VpcConfigurationOutputTypeDef,  # (9)
    initializationScript: str,
    commandLineArguments: List[KxCommandLineArgumentTypeDef],  # (10)
    code: CodeConfigurationTypeDef,  # (11)
    executionRole: str,
    lastModifiedTimestamp: datetime,
    savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef,  # (12)
    azMode: KxAzModeType,  # (13)
    availabilityZoneId: str,
    createdTimestamp: datetime,
    scalingGroupConfiguration: KxScalingGroupConfigurationTypeDef,  # (14)
    ResponseMetadata: ResponseMetadataTypeDef,  # (15)
```

1. See [:material-code-brackets: KxClusterStatusType](./literals.md#kxclusterstatustype) 
2. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
3. See [:material-code-braces: TickerplantLogConfigurationOutputTypeDef](./type_defs.md#tickerplantlogconfigurationoutputtypedef) 
4. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
5. See [:material-code-braces: KxDatabaseConfigurationOutputTypeDef](./type_defs.md#kxdatabaseconfigurationoutputtypedef) 
6. See [:material-code-braces: KxCacheStorageConfigurationTypeDef](./type_defs.md#kxcachestorageconfigurationtypedef) 
7. See [:material-code-braces: AutoScalingConfigurationTypeDef](./type_defs.md#autoscalingconfigurationtypedef) 
8. See [:material-code-braces: CapacityConfigurationTypeDef](./type_defs.md#capacityconfigurationtypedef) 
9. See [:material-code-braces: VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef) 
10. See [:material-code-braces: KxCommandLineArgumentTypeDef](./type_defs.md#kxcommandlineargumenttypedef) 
11. See [:material-code-braces: CodeConfigurationTypeDef](./type_defs.md#codeconfigurationtypedef) 
12. See [:material-code-braces: KxSavedownStorageConfigurationTypeDef](./type_defs.md#kxsavedownstorageconfigurationtypedef) 
13. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
14. See [:material-code-braces: KxScalingGroupConfigurationTypeDef](./type_defs.md#kxscalinggroupconfigurationtypedef) 
15. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKxClusterResponseTypeDef

```python
# GetKxClusterResponseTypeDef definition

class GetKxClusterResponseTypeDef(TypedDict):
    status: KxClusterStatusType,  # (1)
    statusReason: str,
    clusterName: str,
    clusterType: KxClusterTypeType,  # (2)
    tickerplantLogConfiguration: TickerplantLogConfigurationOutputTypeDef,  # (3)
    volumes: List[VolumeTypeDef],  # (4)
    databases: List[KxDatabaseConfigurationOutputTypeDef],  # (5)
    cacheStorageConfigurations: List[KxCacheStorageConfigurationTypeDef],  # (6)
    autoScalingConfiguration: AutoScalingConfigurationTypeDef,  # (7)
    clusterDescription: str,
    capacityConfiguration: CapacityConfigurationTypeDef,  # (8)
    releaseLabel: str,
    vpcConfiguration: VpcConfigurationOutputTypeDef,  # (9)
    initializationScript: str,
    commandLineArguments: List[KxCommandLineArgumentTypeDef],  # (10)
    code: CodeConfigurationTypeDef,  # (11)
    executionRole: str,
    lastModifiedTimestamp: datetime,
    savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef,  # (12)
    azMode: KxAzModeType,  # (13)
    availabilityZoneId: str,
    createdTimestamp: datetime,
    scalingGroupConfiguration: KxScalingGroupConfigurationTypeDef,  # (14)
    ResponseMetadata: ResponseMetadataTypeDef,  # (15)
```

1. See [:material-code-brackets: KxClusterStatusType](./literals.md#kxclusterstatustype) 
2. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
3. See [:material-code-braces: TickerplantLogConfigurationOutputTypeDef](./type_defs.md#tickerplantlogconfigurationoutputtypedef) 
4. See [:material-code-braces: VolumeTypeDef](./type_defs.md#volumetypedef) 
5. See [:material-code-braces: KxDatabaseConfigurationOutputTypeDef](./type_defs.md#kxdatabaseconfigurationoutputtypedef) 
6. See [:material-code-braces: KxCacheStorageConfigurationTypeDef](./type_defs.md#kxcachestorageconfigurationtypedef) 
7. See [:material-code-braces: AutoScalingConfigurationTypeDef](./type_defs.md#autoscalingconfigurationtypedef) 
8. See [:material-code-braces: CapacityConfigurationTypeDef](./type_defs.md#capacityconfigurationtypedef) 
9. See [:material-code-braces: VpcConfigurationOutputTypeDef](./type_defs.md#vpcconfigurationoutputtypedef) 
10. See [:material-code-braces: KxCommandLineArgumentTypeDef](./type_defs.md#kxcommandlineargumenttypedef) 
11. See [:material-code-braces: CodeConfigurationTypeDef](./type_defs.md#codeconfigurationtypedef) 
12. See [:material-code-braces: KxSavedownStorageConfigurationTypeDef](./type_defs.md#kxsavedownstorageconfigurationtypedef) 
13. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
14. See [:material-code-braces: KxScalingGroupConfigurationTypeDef](./type_defs.md#kxscalinggroupconfigurationtypedef) 
15. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKxEnvironmentResponseTypeDef

```python
# GetKxEnvironmentResponseTypeDef definition

class GetKxEnvironmentResponseTypeDef(TypedDict):
    name: str,
    environmentId: str,
    awsAccountId: str,
    status: EnvironmentStatusType,  # (1)
    tgwStatus: TgwStatusType,  # (2)
    dnsStatus: DnsStatusType,  # (3)
    errorMessage: str,
    description: str,
    environmentArn: str,
    kmsKeyId: str,
    dedicatedServiceAccountId: str,
    transitGatewayConfiguration: TransitGatewayConfigurationOutputTypeDef,  # (4)
    customDNSConfiguration: List[CustomDNSServerTypeDef],  # (5)
    creationTimestamp: datetime,
    updateTimestamp: datetime,
    availabilityZoneIds: List[str],
    certificateAuthorityArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: TgwStatusType](./literals.md#tgwstatustype) 
3. See [:material-code-brackets: DnsStatusType](./literals.md#dnsstatustype) 
4. See [:material-code-braces: TransitGatewayConfigurationOutputTypeDef](./type_defs.md#transitgatewayconfigurationoutputtypedef) 
5. See [:material-code-braces: CustomDNSServerTypeDef](./type_defs.md#customdnsservertypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KxEnvironmentTypeDef

```python
# KxEnvironmentTypeDef definition

class KxEnvironmentTypeDef(TypedDict):
    name: NotRequired[str],
    environmentId: NotRequired[str],
    awsAccountId: NotRequired[str],
    status: NotRequired[EnvironmentStatusType],  # (1)
    tgwStatus: NotRequired[TgwStatusType],  # (2)
    dnsStatus: NotRequired[DnsStatusType],  # (3)
    errorMessage: NotRequired[str],
    description: NotRequired[str],
    environmentArn: NotRequired[str],
    kmsKeyId: NotRequired[str],
    dedicatedServiceAccountId: NotRequired[str],
    transitGatewayConfiguration: NotRequired[TransitGatewayConfigurationOutputTypeDef],  # (4)
    customDNSConfiguration: NotRequired[List[CustomDNSServerTypeDef]],  # (5)
    creationTimestamp: NotRequired[datetime],
    updateTimestamp: NotRequired[datetime],
    availabilityZoneIds: NotRequired[List[str]],
    certificateAuthorityArn: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: TgwStatusType](./literals.md#tgwstatustype) 
3. See [:material-code-brackets: DnsStatusType](./literals.md#dnsstatustype) 
4. See [:material-code-braces: TransitGatewayConfigurationOutputTypeDef](./type_defs.md#transitgatewayconfigurationoutputtypedef) 
5. See [:material-code-braces: CustomDNSServerTypeDef](./type_defs.md#customdnsservertypedef) 
## UpdateKxEnvironmentNetworkResponseTypeDef

```python
# UpdateKxEnvironmentNetworkResponseTypeDef definition

class UpdateKxEnvironmentNetworkResponseTypeDef(TypedDict):
    name: str,
    environmentId: str,
    awsAccountId: str,
    status: EnvironmentStatusType,  # (1)
    tgwStatus: TgwStatusType,  # (2)
    dnsStatus: DnsStatusType,  # (3)
    errorMessage: str,
    description: str,
    environmentArn: str,
    kmsKeyId: str,
    dedicatedServiceAccountId: str,
    transitGatewayConfiguration: TransitGatewayConfigurationOutputTypeDef,  # (4)
    customDNSConfiguration: List[CustomDNSServerTypeDef],  # (5)
    creationTimestamp: datetime,
    updateTimestamp: datetime,
    availabilityZoneIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: TgwStatusType](./literals.md#tgwstatustype) 
3. See [:material-code-brackets: DnsStatusType](./literals.md#dnsstatustype) 
4. See [:material-code-braces: TransitGatewayConfigurationOutputTypeDef](./type_defs.md#transitgatewayconfigurationoutputtypedef) 
5. See [:material-code-braces: CustomDNSServerTypeDef](./type_defs.md#customdnsservertypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKxEnvironmentResponseTypeDef

```python
# UpdateKxEnvironmentResponseTypeDef definition

class UpdateKxEnvironmentResponseTypeDef(TypedDict):
    name: str,
    environmentId: str,
    awsAccountId: str,
    status: EnvironmentStatusType,  # (1)
    tgwStatus: TgwStatusType,  # (2)
    dnsStatus: DnsStatusType,  # (3)
    errorMessage: str,
    description: str,
    environmentArn: str,
    kmsKeyId: str,
    dedicatedServiceAccountId: str,
    transitGatewayConfiguration: TransitGatewayConfigurationOutputTypeDef,  # (4)
    customDNSConfiguration: List[CustomDNSServerTypeDef],  # (5)
    creationTimestamp: datetime,
    updateTimestamp: datetime,
    availabilityZoneIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: TgwStatusType](./literals.md#tgwstatustype) 
3. See [:material-code-brackets: DnsStatusType](./literals.md#dnsstatustype) 
4. See [:material-code-braces: TransitGatewayConfigurationOutputTypeDef](./type_defs.md#transitgatewayconfigurationoutputtypedef) 
5. See [:material-code-braces: CustomDNSServerTypeDef](./type_defs.md#customdnsservertypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKxEnvironmentNetworkRequestRequestTypeDef

```python
# UpdateKxEnvironmentNetworkRequestRequestTypeDef definition

class UpdateKxEnvironmentNetworkRequestRequestTypeDef(TypedDict):
    environmentId: str,
    transitGatewayConfiguration: NotRequired[TransitGatewayConfigurationTypeDef],  # (1)
    customDNSConfiguration: NotRequired[Sequence[CustomDNSServerTypeDef]],  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: TransitGatewayConfigurationTypeDef](./type_defs.md#transitgatewayconfigurationtypedef) 
2. See [:material-code-braces: CustomDNSServerTypeDef](./type_defs.md#customdnsservertypedef) 
## KxDatabaseConfigurationTypeDef

```python
# KxDatabaseConfigurationTypeDef definition

class KxDatabaseConfigurationTypeDef(TypedDict):
    databaseName: str,
    cacheConfigurations: NotRequired[Sequence[KxDatabaseCacheConfigurationUnionTypeDef]],  # (1)
    changesetId: NotRequired[str],
    dataviewName: NotRequired[str],
    dataviewConfiguration: NotRequired[KxDataviewConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: KxDatabaseCacheConfigurationTypeDef](./type_defs.md#kxdatabasecacheconfigurationtypedef) [:material-code-braces: KxDatabaseCacheConfigurationOutputTypeDef](./type_defs.md#kxdatabasecacheconfigurationoutputtypedef) 
2. See [:material-code-braces: KxDataviewConfigurationTypeDef](./type_defs.md#kxdataviewconfigurationtypedef) [:material-code-braces: KxDataviewConfigurationOutputTypeDef](./type_defs.md#kxdataviewconfigurationoutputtypedef) 
## ListKxEnvironmentsResponseTypeDef

```python
# ListKxEnvironmentsResponseTypeDef definition

class ListKxEnvironmentsResponseTypeDef(TypedDict):
    environments: List[KxEnvironmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KxEnvironmentTypeDef](./type_defs.md#kxenvironmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKxClusterDatabasesRequestRequestTypeDef

```python
# UpdateKxClusterDatabasesRequestRequestTypeDef definition

class UpdateKxClusterDatabasesRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clusterName: str,
    databases: Sequence[KxDatabaseConfigurationTypeDef],  # (1)
    clientToken: NotRequired[str],
    deploymentConfiguration: NotRequired[KxDeploymentConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef) 
2. See [:material-code-braces: KxDeploymentConfigurationTypeDef](./type_defs.md#kxdeploymentconfigurationtypedef) 
## CreateKxClusterRequestRequestTypeDef

```python
# CreateKxClusterRequestRequestTypeDef definition

class CreateKxClusterRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clusterName: str,
    clusterType: KxClusterTypeType,  # (1)
    releaseLabel: str,
    vpcConfiguration: VpcConfigurationTypeDef,  # (2)
    azMode: KxAzModeType,  # (3)
    clientToken: NotRequired[str],
    tickerplantLogConfiguration: NotRequired[TickerplantLogConfigurationTypeDef],  # (4)
    databases: NotRequired[Sequence[KxDatabaseConfigurationUnionTypeDef]],  # (5)
    cacheStorageConfigurations: NotRequired[Sequence[KxCacheStorageConfigurationTypeDef]],  # (6)
    autoScalingConfiguration: NotRequired[AutoScalingConfigurationTypeDef],  # (7)
    clusterDescription: NotRequired[str],
    capacityConfiguration: NotRequired[CapacityConfigurationTypeDef],  # (8)
    initializationScript: NotRequired[str],
    commandLineArguments: NotRequired[Sequence[KxCommandLineArgumentTypeDef]],  # (9)
    code: NotRequired[CodeConfigurationTypeDef],  # (10)
    executionRole: NotRequired[str],
    savedownStorageConfiguration: NotRequired[KxSavedownStorageConfigurationTypeDef],  # (11)
    availabilityZoneId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    scalingGroupConfiguration: NotRequired[KxScalingGroupConfigurationTypeDef],  # (12)
```

1. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
2. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
3. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
4. See [:material-code-braces: TickerplantLogConfigurationTypeDef](./type_defs.md#tickerplantlogconfigurationtypedef) 
5. See [:material-code-braces: KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef) [:material-code-braces: KxDatabaseConfigurationOutputTypeDef](./type_defs.md#kxdatabaseconfigurationoutputtypedef) 
6. See [:material-code-braces: KxCacheStorageConfigurationTypeDef](./type_defs.md#kxcachestorageconfigurationtypedef) 
7. See [:material-code-braces: AutoScalingConfigurationTypeDef](./type_defs.md#autoscalingconfigurationtypedef) 
8. See [:material-code-braces: CapacityConfigurationTypeDef](./type_defs.md#capacityconfigurationtypedef) 
9. See [:material-code-braces: KxCommandLineArgumentTypeDef](./type_defs.md#kxcommandlineargumenttypedef) 
10. See [:material-code-braces: CodeConfigurationTypeDef](./type_defs.md#codeconfigurationtypedef) 
11. See [:material-code-braces: KxSavedownStorageConfigurationTypeDef](./type_defs.md#kxsavedownstorageconfigurationtypedef) 
12. See [:material-code-braces: KxScalingGroupConfigurationTypeDef](./type_defs.md#kxscalinggroupconfigurationtypedef) 
