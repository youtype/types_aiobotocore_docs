# Type definitions

> [Index](../README.md) > [finspace](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
    type annotations stubs module [types-aiobotocore-finspace](https://pypi.org/project/types-aiobotocore-finspace/).



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
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
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
    type: KxSavedownStorageTypeType,  # (1)
    size: int,
```

1. See [:material-code-brackets: KxSavedownStorageTypeType](./literals.md#kxsavedownstoragetypetype) 
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

## DeleteKxEnvironmentRequestRequestTypeDef

```python
# DeleteKxEnvironmentRequestRequestTypeDef definition

class DeleteKxEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
```

## DeleteKxUserRequestRequestTypeDef

```python
# DeleteKxUserRequestRequestTypeDef definition

class DeleteKxUserRequestRequestTypeDef(TypedDict):
    userName: str,
    environmentId: str,
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

## GetKxEnvironmentRequestRequestTypeDef

```python
# GetKxEnvironmentRequestRequestTypeDef definition

class GetKxEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
```

## TransitGatewayConfigurationTypeDef

```python
# TransitGatewayConfigurationTypeDef definition

class TransitGatewayConfigurationTypeDef(TypedDict):
    transitGatewayID: str,
    routableCIDRSpace: str,
```

## GetKxUserRequestRequestTypeDef

```python
# GetKxUserRequestRequestTypeDef definition

class GetKxUserRequestRequestTypeDef(TypedDict):
    userName: str,
    environmentId: str,
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
    initializationScript: NotRequired[str],
    executionRole: NotRequired[str],
    azMode: NotRequired[KxAzModeType],  # (3)
    availabilityZoneId: NotRequired[str],
    lastModifiedTimestamp: NotRequired[datetime],
    createdTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: KxClusterStatusType](./literals.md#kxclusterstatustype) 
2. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
3. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
## KxDatabaseCacheConfigurationTypeDef

```python
# KxDatabaseCacheConfigurationTypeDef definition

class KxDatabaseCacheConfigurationTypeDef(TypedDict):
    cacheType: str,
    dbPaths: Sequence[str],
```

## KxDatabaseListEntryTypeDef

```python
# KxDatabaseListEntryTypeDef definition

class KxDatabaseListEntryTypeDef(TypedDict):
    databaseName: NotRequired[str],
    createdTimestamp: NotRequired[datetime],
    lastModifiedTimestamp: NotRequired[datetime],
```

## KxNodeTypeDef

```python
# KxNodeTypeDef definition

class KxNodeTypeDef(TypedDict):
    nodeId: NotRequired[str],
    availabilityZoneId: NotRequired[str],
    launchTime: NotRequired[datetime],
```

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

## ListKxUsersRequestRequestTypeDef

```python
# ListKxUsersRequestRequestTypeDef definition

class ListKxUsersRequestRequestTypeDef(TypedDict):
    environmentId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
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
    federationParameters: NotRequired[FederationParametersTypeDef],  # (3)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: FederationModeType](./literals.md#federationmodetype) 
3. See [:material-code-braces: FederationParametersTypeDef](./type_defs.md#federationparameterstypedef) 
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
## GetKxEnvironmentResponseTypeDef

```python
# GetKxEnvironmentResponseTypeDef definition

class GetKxEnvironmentResponseTypeDef(TypedDict):
    name: str,
    environmentId: str,
    awsAccountId: str,
    status: EnvironmentStatusType,  # (1)
    tgwStatus: tgwStatusType,  # (2)
    dnsStatus: dnsStatusType,  # (3)
    errorMessage: str,
    description: str,
    environmentArn: str,
    kmsKeyId: str,
    dedicatedServiceAccountId: str,
    transitGatewayConfiguration: TransitGatewayConfigurationTypeDef,  # (4)
    customDNSConfiguration: List[CustomDNSServerTypeDef],  # (5)
    creationTimestamp: datetime,
    updateTimestamp: datetime,
    availabilityZoneIds: List[str],
    certificateAuthorityArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: tgwStatusType](./literals.md#tgwstatustype) 
3. See [:material-code-brackets: dnsStatusType](./literals.md#dnsstatustype) 
4. See [:material-code-braces: TransitGatewayConfigurationTypeDef](./type_defs.md#transitgatewayconfigurationtypedef) 
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
    tgwStatus: NotRequired[tgwStatusType],  # (2)
    dnsStatus: NotRequired[dnsStatusType],  # (3)
    errorMessage: NotRequired[str],
    description: NotRequired[str],
    environmentArn: NotRequired[str],
    kmsKeyId: NotRequired[str],
    dedicatedServiceAccountId: NotRequired[str],
    transitGatewayConfiguration: NotRequired[TransitGatewayConfigurationTypeDef],  # (4)
    customDNSConfiguration: NotRequired[List[CustomDNSServerTypeDef]],  # (5)
    creationTimestamp: NotRequired[datetime],
    updateTimestamp: NotRequired[datetime],
    availabilityZoneIds: NotRequired[List[str]],
    certificateAuthorityArn: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: tgwStatusType](./literals.md#tgwstatustype) 
3. See [:material-code-brackets: dnsStatusType](./literals.md#dnsstatustype) 
4. See [:material-code-braces: TransitGatewayConfigurationTypeDef](./type_defs.md#transitgatewayconfigurationtypedef) 
5. See [:material-code-braces: CustomDNSServerTypeDef](./type_defs.md#customdnsservertypedef) 
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
## UpdateKxEnvironmentNetworkResponseTypeDef

```python
# UpdateKxEnvironmentNetworkResponseTypeDef definition

class UpdateKxEnvironmentNetworkResponseTypeDef(TypedDict):
    name: str,
    environmentId: str,
    awsAccountId: str,
    status: EnvironmentStatusType,  # (1)
    tgwStatus: tgwStatusType,  # (2)
    dnsStatus: dnsStatusType,  # (3)
    errorMessage: str,
    description: str,
    environmentArn: str,
    kmsKeyId: str,
    dedicatedServiceAccountId: str,
    transitGatewayConfiguration: TransitGatewayConfigurationTypeDef,  # (4)
    customDNSConfiguration: List[CustomDNSServerTypeDef],  # (5)
    creationTimestamp: datetime,
    updateTimestamp: datetime,
    availabilityZoneIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: tgwStatusType](./literals.md#tgwstatustype) 
3. See [:material-code-brackets: dnsStatusType](./literals.md#dnsstatustype) 
4. See [:material-code-braces: TransitGatewayConfigurationTypeDef](./type_defs.md#transitgatewayconfigurationtypedef) 
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
    tgwStatus: tgwStatusType,  # (2)
    dnsStatus: dnsStatusType,  # (3)
    errorMessage: str,
    description: str,
    environmentArn: str,
    kmsKeyId: str,
    dedicatedServiceAccountId: str,
    transitGatewayConfiguration: TransitGatewayConfigurationTypeDef,  # (4)
    customDNSConfiguration: List[CustomDNSServerTypeDef],  # (5)
    creationTimestamp: datetime,
    updateTimestamp: datetime,
    availabilityZoneIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: tgwStatusType](./literals.md#tgwstatustype) 
3. See [:material-code-brackets: dnsStatusType](./literals.md#dnsstatustype) 
4. See [:material-code-braces: TransitGatewayConfigurationTypeDef](./type_defs.md#transitgatewayconfigurationtypedef) 
5. See [:material-code-braces: CustomDNSServerTypeDef](./type_defs.md#customdnsservertypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKxChangesetsResponseTypeDef

```python
# ListKxChangesetsResponseTypeDef definition

class ListKxChangesetsResponseTypeDef(TypedDict):
    kxChangesets: List[KxChangesetListEntryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KxChangesetListEntryTypeDef](./type_defs.md#kxchangesetlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKxClustersResponseTypeDef

```python
# ListKxClustersResponseTypeDef definition

class ListKxClustersResponseTypeDef(TypedDict):
    kxClusterSummaries: List[KxClusterTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KxClusterTypeDef](./type_defs.md#kxclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KxDatabaseConfigurationTypeDef

```python
# KxDatabaseConfigurationTypeDef definition

class KxDatabaseConfigurationTypeDef(TypedDict):
    databaseName: str,
    cacheConfigurations: NotRequired[Sequence[KxDatabaseCacheConfigurationTypeDef]],  # (1)
    changesetId: NotRequired[str],
```

1. See [:material-code-braces: KxDatabaseCacheConfigurationTypeDef](./type_defs.md#kxdatabasecacheconfigurationtypedef) 
## ListKxDatabasesResponseTypeDef

```python
# ListKxDatabasesResponseTypeDef definition

class ListKxDatabasesResponseTypeDef(TypedDict):
    kxDatabases: List[KxDatabaseListEntryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KxDatabaseListEntryTypeDef](./type_defs.md#kxdatabaselistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKxClusterNodesResponseTypeDef

```python
# ListKxClusterNodesResponseTypeDef definition

class ListKxClusterNodesResponseTypeDef(TypedDict):
    nodes: List[KxNodeTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KxNodeTypeDef](./type_defs.md#kxnodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKxUsersResponseTypeDef

```python
# ListKxUsersResponseTypeDef definition

class ListKxUsersResponseTypeDef(TypedDict):
    users: List[KxUserTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KxUserTypeDef](./type_defs.md#kxusertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef

```python
# ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef definition

class ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
## ListKxEnvironmentsResponseTypeDef

```python
# ListKxEnvironmentsResponseTypeDef definition

class ListKxEnvironmentsResponseTypeDef(TypedDict):
    environments: List[KxEnvironmentTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KxEnvironmentTypeDef](./type_defs.md#kxenvironmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKxClusterRequestRequestTypeDef

```python
# CreateKxClusterRequestRequestTypeDef definition

class CreateKxClusterRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clusterName: str,
    clusterType: KxClusterTypeType,  # (1)
    capacityConfiguration: CapacityConfigurationTypeDef,  # (2)
    releaseLabel: str,
    azMode: KxAzModeType,  # (3)
    clientToken: NotRequired[str],
    databases: NotRequired[Sequence[KxDatabaseConfigurationTypeDef]],  # (4)
    cacheStorageConfigurations: NotRequired[Sequence[KxCacheStorageConfigurationTypeDef]],  # (5)
    autoScalingConfiguration: NotRequired[AutoScalingConfigurationTypeDef],  # (6)
    clusterDescription: NotRequired[str],
    vpcConfiguration: NotRequired[VpcConfigurationTypeDef],  # (7)
    initializationScript: NotRequired[str],
    commandLineArguments: NotRequired[Sequence[KxCommandLineArgumentTypeDef]],  # (8)
    code: NotRequired[CodeConfigurationTypeDef],  # (9)
    executionRole: NotRequired[str],
    savedownStorageConfiguration: NotRequired[KxSavedownStorageConfigurationTypeDef],  # (10)
    availabilityZoneId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
2. See [:material-code-braces: CapacityConfigurationTypeDef](./type_defs.md#capacityconfigurationtypedef) 
3. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
4. See [:material-code-braces: KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef) 
5. See [:material-code-braces: KxCacheStorageConfigurationTypeDef](./type_defs.md#kxcachestorageconfigurationtypedef) 
6. See [:material-code-braces: AutoScalingConfigurationTypeDef](./type_defs.md#autoscalingconfigurationtypedef) 
7. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
8. See [:material-code-braces: KxCommandLineArgumentTypeDef](./type_defs.md#kxcommandlineargumenttypedef) 
9. See [:material-code-braces: CodeConfigurationTypeDef](./type_defs.md#codeconfigurationtypedef) 
10. See [:material-code-braces: KxSavedownStorageConfigurationTypeDef](./type_defs.md#kxsavedownstorageconfigurationtypedef) 
## CreateKxClusterResponseTypeDef

```python
# CreateKxClusterResponseTypeDef definition

class CreateKxClusterResponseTypeDef(TypedDict):
    environmentId: str,
    status: KxClusterStatusType,  # (1)
    statusReason: str,
    clusterName: str,
    clusterType: KxClusterTypeType,  # (2)
    databases: List[KxDatabaseConfigurationTypeDef],  # (3)
    cacheStorageConfigurations: List[KxCacheStorageConfigurationTypeDef],  # (4)
    autoScalingConfiguration: AutoScalingConfigurationTypeDef,  # (5)
    clusterDescription: str,
    capacityConfiguration: CapacityConfigurationTypeDef,  # (6)
    releaseLabel: str,
    vpcConfiguration: VpcConfigurationTypeDef,  # (7)
    initializationScript: str,
    commandLineArguments: List[KxCommandLineArgumentTypeDef],  # (8)
    code: CodeConfigurationTypeDef,  # (9)
    executionRole: str,
    lastModifiedTimestamp: datetime,
    savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef,  # (10)
    azMode: KxAzModeType,  # (11)
    availabilityZoneId: str,
    createdTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (12)
```

1. See [:material-code-brackets: KxClusterStatusType](./literals.md#kxclusterstatustype) 
2. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
3. See [:material-code-braces: KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef) 
4. See [:material-code-braces: KxCacheStorageConfigurationTypeDef](./type_defs.md#kxcachestorageconfigurationtypedef) 
5. See [:material-code-braces: AutoScalingConfigurationTypeDef](./type_defs.md#autoscalingconfigurationtypedef) 
6. See [:material-code-braces: CapacityConfigurationTypeDef](./type_defs.md#capacityconfigurationtypedef) 
7. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
8. See [:material-code-braces: KxCommandLineArgumentTypeDef](./type_defs.md#kxcommandlineargumenttypedef) 
9. See [:material-code-braces: CodeConfigurationTypeDef](./type_defs.md#codeconfigurationtypedef) 
10. See [:material-code-braces: KxSavedownStorageConfigurationTypeDef](./type_defs.md#kxsavedownstorageconfigurationtypedef) 
11. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
12. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKxClusterResponseTypeDef

```python
# GetKxClusterResponseTypeDef definition

class GetKxClusterResponseTypeDef(TypedDict):
    status: KxClusterStatusType,  # (1)
    statusReason: str,
    clusterName: str,
    clusterType: KxClusterTypeType,  # (2)
    databases: List[KxDatabaseConfigurationTypeDef],  # (3)
    cacheStorageConfigurations: List[KxCacheStorageConfigurationTypeDef],  # (4)
    autoScalingConfiguration: AutoScalingConfigurationTypeDef,  # (5)
    clusterDescription: str,
    capacityConfiguration: CapacityConfigurationTypeDef,  # (6)
    releaseLabel: str,
    vpcConfiguration: VpcConfigurationTypeDef,  # (7)
    initializationScript: str,
    commandLineArguments: List[KxCommandLineArgumentTypeDef],  # (8)
    code: CodeConfigurationTypeDef,  # (9)
    executionRole: str,
    lastModifiedTimestamp: datetime,
    savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef,  # (10)
    azMode: KxAzModeType,  # (11)
    availabilityZoneId: str,
    createdTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (12)
```

1. See [:material-code-brackets: KxClusterStatusType](./literals.md#kxclusterstatustype) 
2. See [:material-code-brackets: KxClusterTypeType](./literals.md#kxclustertypetype) 
3. See [:material-code-braces: KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef) 
4. See [:material-code-braces: KxCacheStorageConfigurationTypeDef](./type_defs.md#kxcachestorageconfigurationtypedef) 
5. See [:material-code-braces: AutoScalingConfigurationTypeDef](./type_defs.md#autoscalingconfigurationtypedef) 
6. See [:material-code-braces: CapacityConfigurationTypeDef](./type_defs.md#capacityconfigurationtypedef) 
7. See [:material-code-braces: VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef) 
8. See [:material-code-braces: KxCommandLineArgumentTypeDef](./type_defs.md#kxcommandlineargumenttypedef) 
9. See [:material-code-braces: CodeConfigurationTypeDef](./type_defs.md#codeconfigurationtypedef) 
10. See [:material-code-braces: KxSavedownStorageConfigurationTypeDef](./type_defs.md#kxsavedownstorageconfigurationtypedef) 
11. See [:material-code-brackets: KxAzModeType](./literals.md#kxazmodetype) 
12. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKxClusterDatabasesRequestRequestTypeDef

```python
# UpdateKxClusterDatabasesRequestRequestTypeDef definition

class UpdateKxClusterDatabasesRequestRequestTypeDef(TypedDict):
    environmentId: str,
    clusterName: str,
    databases: Sequence[KxDatabaseConfigurationTypeDef],  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: KxDatabaseConfigurationTypeDef](./type_defs.md#kxdatabaseconfigurationtypedef) 
