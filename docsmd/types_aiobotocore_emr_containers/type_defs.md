# Type definitions

> [Index](../README.md) > [EMRContainers](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EMRContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#EMRContainers)
    type annotations stubs module [types-aiobotocore-emr-containers](https://pypi.org/project/types-aiobotocore-emr-containers/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## CancelJobRunRequestRequestTypeDef

```python
# CancelJobRunRequestRequestTypeDef definition

class CancelJobRunRequestRequestTypeDef(TypedDict):
    id: str,
    virtualClusterId: str,
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

## CertificateTypeDef

```python
# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    certificateArn: NotRequired[str],
    certificateData: NotRequired[str],
```

## CloudWatchMonitoringConfigurationTypeDef

```python
# CloudWatchMonitoringConfigurationTypeDef definition

class CloudWatchMonitoringConfigurationTypeDef(TypedDict):
    logGroupName: str,
    logStreamNamePrefix: NotRequired[str],
```

## ConfigurationTypeDef

```python
# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    classification: str,
    properties: NotRequired[Mapping[str, str]],
    configurations: NotRequired[Sequence[ConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
## EksInfoTypeDef

```python
# EksInfoTypeDef definition

class EksInfoTypeDef(TypedDict):
    namespace: NotRequired[str],
```

## ContainerLogRotationConfigurationTypeDef

```python
# ContainerLogRotationConfigurationTypeDef definition

class ContainerLogRotationConfigurationTypeDef(TypedDict):
    rotationSize: str,
    maxFilesToKeep: int,
```

## CredentialsTypeDef

```python
# CredentialsTypeDef definition

class CredentialsTypeDef(TypedDict):
    token: NotRequired[str],
```

## DeleteJobTemplateRequestRequestTypeDef

```python
# DeleteJobTemplateRequestRequestTypeDef definition

class DeleteJobTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteManagedEndpointRequestRequestTypeDef

```python
# DeleteManagedEndpointRequestRequestTypeDef definition

class DeleteManagedEndpointRequestRequestTypeDef(TypedDict):
    id: str,
    virtualClusterId: str,
```

## DeleteVirtualClusterRequestRequestTypeDef

```python
# DeleteVirtualClusterRequestRequestTypeDef definition

class DeleteVirtualClusterRequestRequestTypeDef(TypedDict):
    id: str,
```

## DescribeJobRunRequestRequestTypeDef

```python
# DescribeJobRunRequestRequestTypeDef definition

class DescribeJobRunRequestRequestTypeDef(TypedDict):
    id: str,
    virtualClusterId: str,
```

## DescribeJobTemplateRequestRequestTypeDef

```python
# DescribeJobTemplateRequestRequestTypeDef definition

class DescribeJobTemplateRequestRequestTypeDef(TypedDict):
    id: str,
```

## DescribeManagedEndpointRequestRequestTypeDef

```python
# DescribeManagedEndpointRequestRequestTypeDef definition

class DescribeManagedEndpointRequestRequestTypeDef(TypedDict):
    id: str,
    virtualClusterId: str,
```

## DescribeVirtualClusterRequestRequestTypeDef

```python
# DescribeVirtualClusterRequestRequestTypeDef definition

class DescribeVirtualClusterRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetManagedEndpointSessionCredentialsRequestRequestTypeDef

```python
# GetManagedEndpointSessionCredentialsRequestRequestTypeDef definition

class GetManagedEndpointSessionCredentialsRequestRequestTypeDef(TypedDict):
    endpointIdentifier: str,
    virtualClusterIdentifier: str,
    executionRoleArn: str,
    credentialType: str,
    durationInSeconds: NotRequired[int],
    logContext: NotRequired[str],
    clientToken: NotRequired[str],
```

## SparkSqlJobDriverTypeDef

```python
# SparkSqlJobDriverTypeDef definition

class SparkSqlJobDriverTypeDef(TypedDict):
    entryPoint: NotRequired[str],
    sparkSqlParameters: NotRequired[str],
```

## SparkSubmitJobDriverTypeDef

```python
# SparkSubmitJobDriverTypeDef definition

class SparkSubmitJobDriverTypeDef(TypedDict):
    entryPoint: str,
    entryPointArguments: NotRequired[Sequence[str]],
    sparkSubmitParameters: NotRequired[str],
```

## RetryPolicyConfigurationTypeDef

```python
# RetryPolicyConfigurationTypeDef definition

class RetryPolicyConfigurationTypeDef(TypedDict):
    maxAttempts: int,
```

## RetryPolicyExecutionTypeDef

```python
# RetryPolicyExecutionTypeDef definition

class RetryPolicyExecutionTypeDef(TypedDict):
    currentAttemptCount: int,
```

## TemplateParameterConfigurationTypeDef

```python
# TemplateParameterConfigurationTypeDef definition

class TemplateParameterConfigurationTypeDef(TypedDict):
    type: NotRequired[TemplateParameterDataTypeType],  # (1)
    defaultValue: NotRequired[str],
```

1. See [:material-code-brackets: TemplateParameterDataTypeType](./literals.md#templateparameterdatatypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## S3MonitoringConfigurationTypeDef

```python
# S3MonitoringConfigurationTypeDef definition

class S3MonitoringConfigurationTypeDef(TypedDict):
    logUri: str,
```

## ParametricCloudWatchMonitoringConfigurationTypeDef

```python
# ParametricCloudWatchMonitoringConfigurationTypeDef definition

class ParametricCloudWatchMonitoringConfigurationTypeDef(TypedDict):
    logGroupName: NotRequired[str],
    logStreamNamePrefix: NotRequired[str],
```

## ParametricS3MonitoringConfigurationTypeDef

```python
# ParametricS3MonitoringConfigurationTypeDef definition

class ParametricS3MonitoringConfigurationTypeDef(TypedDict):
    logUri: NotRequired[str],
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

## CancelJobRunResponseTypeDef

```python
# CancelJobRunResponseTypeDef definition

class CancelJobRunResponseTypeDef(TypedDict):
    id: str,
    virtualClusterId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobTemplateResponseTypeDef

```python
# CreateJobTemplateResponseTypeDef definition

class CreateJobTemplateResponseTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateManagedEndpointResponseTypeDef

```python
# CreateManagedEndpointResponseTypeDef definition

class CreateManagedEndpointResponseTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    virtualClusterId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVirtualClusterResponseTypeDef

```python
# CreateVirtualClusterResponseTypeDef definition

class CreateVirtualClusterResponseTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteJobTemplateResponseTypeDef

```python
# DeleteJobTemplateResponseTypeDef definition

class DeleteJobTemplateResponseTypeDef(TypedDict):
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteManagedEndpointResponseTypeDef

```python
# DeleteManagedEndpointResponseTypeDef definition

class DeleteManagedEndpointResponseTypeDef(TypedDict):
    id: str,
    virtualClusterId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVirtualClusterResponseTypeDef

```python
# DeleteVirtualClusterResponseTypeDef definition

class DeleteVirtualClusterResponseTypeDef(TypedDict):
    id: str,
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
## StartJobRunResponseTypeDef

```python
# StartJobRunResponseTypeDef definition

class StartJobRunResponseTypeDef(TypedDict):
    id: str,
    name: str,
    arn: str,
    virtualClusterId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContainerInfoTypeDef

```python
# ContainerInfoTypeDef definition

class ContainerInfoTypeDef(TypedDict):
    eksInfo: NotRequired[EksInfoTypeDef],  # (1)
```

1. See [:material-code-braces: EksInfoTypeDef](./type_defs.md#eksinfotypedef) 
## GetManagedEndpointSessionCredentialsResponseTypeDef

```python
# GetManagedEndpointSessionCredentialsResponseTypeDef definition

class GetManagedEndpointSessionCredentialsResponseTypeDef(TypedDict):
    id: str,
    credentials: CredentialsTypeDef,  # (1)
    expiresAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobDriverTypeDef

```python
# JobDriverTypeDef definition

class JobDriverTypeDef(TypedDict):
    sparkSubmitJobDriver: NotRequired[SparkSubmitJobDriverTypeDef],  # (1)
    sparkSqlJobDriver: NotRequired[SparkSqlJobDriverTypeDef],  # (2)
```

1. See [:material-code-braces: SparkSubmitJobDriverTypeDef](./type_defs.md#sparksubmitjobdrivertypedef) 
2. See [:material-code-braces: SparkSqlJobDriverTypeDef](./type_defs.md#sparksqljobdrivertypedef) 
## ListJobRunsRequestListJobRunsPaginateTypeDef

```python
# ListJobRunsRequestListJobRunsPaginateTypeDef definition

class ListJobRunsRequestListJobRunsPaginateTypeDef(TypedDict):
    virtualClusterId: str,
    createdBefore: NotRequired[Union[datetime, str]],
    createdAfter: NotRequired[Union[datetime, str]],
    name: NotRequired[str],
    states: NotRequired[Sequence[JobRunStateType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobRunsRequestRequestTypeDef

```python
# ListJobRunsRequestRequestTypeDef definition

class ListJobRunsRequestRequestTypeDef(TypedDict):
    virtualClusterId: str,
    createdBefore: NotRequired[Union[datetime, str]],
    createdAfter: NotRequired[Union[datetime, str]],
    name: NotRequired[str],
    states: NotRequired[Sequence[JobRunStateType]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
## ListJobTemplatesRequestListJobTemplatesPaginateTypeDef

```python
# ListJobTemplatesRequestListJobTemplatesPaginateTypeDef definition

class ListJobTemplatesRequestListJobTemplatesPaginateTypeDef(TypedDict):
    createdAfter: NotRequired[Union[datetime, str]],
    createdBefore: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobTemplatesRequestRequestTypeDef

```python
# ListJobTemplatesRequestRequestTypeDef definition

class ListJobTemplatesRequestRequestTypeDef(TypedDict):
    createdAfter: NotRequired[Union[datetime, str]],
    createdBefore: NotRequired[Union[datetime, str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef

```python
# ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef definition

class ListManagedEndpointsRequestListManagedEndpointsPaginateTypeDef(TypedDict):
    virtualClusterId: str,
    createdBefore: NotRequired[Union[datetime, str]],
    createdAfter: NotRequired[Union[datetime, str]],
    types: NotRequired[Sequence[str]],
    states: NotRequired[Sequence[EndpointStateType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EndpointStateType](./literals.md#endpointstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListManagedEndpointsRequestRequestTypeDef

```python
# ListManagedEndpointsRequestRequestTypeDef definition

class ListManagedEndpointsRequestRequestTypeDef(TypedDict):
    virtualClusterId: str,
    createdBefore: NotRequired[Union[datetime, str]],
    createdAfter: NotRequired[Union[datetime, str]],
    types: NotRequired[Sequence[str]],
    states: NotRequired[Sequence[EndpointStateType]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: EndpointStateType](./literals.md#endpointstatetype) 
## ListVirtualClustersRequestListVirtualClustersPaginateTypeDef

```python
# ListVirtualClustersRequestListVirtualClustersPaginateTypeDef definition

class ListVirtualClustersRequestListVirtualClustersPaginateTypeDef(TypedDict):
    containerProviderId: NotRequired[str],
    containerProviderType: NotRequired[ContainerProviderTypeType],  # (1)
    createdAfter: NotRequired[Union[datetime, str]],
    createdBefore: NotRequired[Union[datetime, str]],
    states: NotRequired[Sequence[VirtualClusterStateType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ContainerProviderTypeType](./literals.md#containerprovidertypetype) 
2. See [:material-code-brackets: VirtualClusterStateType](./literals.md#virtualclusterstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVirtualClustersRequestRequestTypeDef

```python
# ListVirtualClustersRequestRequestTypeDef definition

class ListVirtualClustersRequestRequestTypeDef(TypedDict):
    containerProviderId: NotRequired[str],
    containerProviderType: NotRequired[ContainerProviderTypeType],  # (1)
    createdAfter: NotRequired[Union[datetime, str]],
    createdBefore: NotRequired[Union[datetime, str]],
    states: NotRequired[Sequence[VirtualClusterStateType]],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ContainerProviderTypeType](./literals.md#containerprovidertypetype) 
2. See [:material-code-brackets: VirtualClusterStateType](./literals.md#virtualclusterstatetype) 
## MonitoringConfigurationTypeDef

```python
# MonitoringConfigurationTypeDef definition

class MonitoringConfigurationTypeDef(TypedDict):
    persistentAppUI: NotRequired[PersistentAppUIType],  # (1)
    cloudWatchMonitoringConfiguration: NotRequired[CloudWatchMonitoringConfigurationTypeDef],  # (2)
    s3MonitoringConfiguration: NotRequired[S3MonitoringConfigurationTypeDef],  # (3)
    containerLogRotationConfiguration: NotRequired[ContainerLogRotationConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: PersistentAppUIType](./literals.md#persistentappuitype) 
2. See [:material-code-braces: CloudWatchMonitoringConfigurationTypeDef](./type_defs.md#cloudwatchmonitoringconfigurationtypedef) 
3. See [:material-code-braces: S3MonitoringConfigurationTypeDef](./type_defs.md#s3monitoringconfigurationtypedef) 
4. See [:material-code-braces: ContainerLogRotationConfigurationTypeDef](./type_defs.md#containerlogrotationconfigurationtypedef) 
## ParametricMonitoringConfigurationTypeDef

```python
# ParametricMonitoringConfigurationTypeDef definition

class ParametricMonitoringConfigurationTypeDef(TypedDict):
    persistentAppUI: NotRequired[str],
    cloudWatchMonitoringConfiguration: NotRequired[ParametricCloudWatchMonitoringConfigurationTypeDef],  # (1)
    s3MonitoringConfiguration: NotRequired[ParametricS3MonitoringConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ParametricCloudWatchMonitoringConfigurationTypeDef](./type_defs.md#parametriccloudwatchmonitoringconfigurationtypedef) 
2. See [:material-code-braces: ParametricS3MonitoringConfigurationTypeDef](./type_defs.md#parametrics3monitoringconfigurationtypedef) 
## ContainerProviderTypeDef

```python
# ContainerProviderTypeDef definition

class ContainerProviderTypeDef(TypedDict):
    type: ContainerProviderTypeType,  # (1)
    id: str,
    info: NotRequired[ContainerInfoTypeDef],  # (2)
```

1. See [:material-code-brackets: ContainerProviderTypeType](./literals.md#containerprovidertypetype) 
2. See [:material-code-braces: ContainerInfoTypeDef](./type_defs.md#containerinfotypedef) 
## ConfigurationOverridesTypeDef

```python
# ConfigurationOverridesTypeDef definition

class ConfigurationOverridesTypeDef(TypedDict):
    applicationConfiguration: NotRequired[Sequence[ConfigurationTypeDef]],  # (1)
    monitoringConfiguration: NotRequired[MonitoringConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-braces: MonitoringConfigurationTypeDef](./type_defs.md#monitoringconfigurationtypedef) 
## ParametricConfigurationOverridesTypeDef

```python
# ParametricConfigurationOverridesTypeDef definition

class ParametricConfigurationOverridesTypeDef(TypedDict):
    applicationConfiguration: NotRequired[Sequence[ConfigurationTypeDef]],  # (1)
    monitoringConfiguration: NotRequired[ParametricMonitoringConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-braces: ParametricMonitoringConfigurationTypeDef](./type_defs.md#parametricmonitoringconfigurationtypedef) 
## CreateVirtualClusterRequestRequestTypeDef

```python
# CreateVirtualClusterRequestRequestTypeDef definition

class CreateVirtualClusterRequestRequestTypeDef(TypedDict):
    name: str,
    containerProvider: ContainerProviderTypeDef,  # (1)
    clientToken: str,
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ContainerProviderTypeDef](./type_defs.md#containerprovidertypedef) 
## VirtualClusterTypeDef

```python
# VirtualClusterTypeDef definition

class VirtualClusterTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    arn: NotRequired[str],
    state: NotRequired[VirtualClusterStateType],  # (1)
    containerProvider: NotRequired[ContainerProviderTypeDef],  # (2)
    createdAt: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: VirtualClusterStateType](./literals.md#virtualclusterstatetype) 
2. See [:material-code-braces: ContainerProviderTypeDef](./type_defs.md#containerprovidertypedef) 
## CreateManagedEndpointRequestRequestTypeDef

```python
# CreateManagedEndpointRequestRequestTypeDef definition

class CreateManagedEndpointRequestRequestTypeDef(TypedDict):
    name: str,
    virtualClusterId: str,
    type: str,
    releaseLabel: str,
    executionRoleArn: str,
    clientToken: str,
    certificateArn: NotRequired[str],
    configurationOverrides: NotRequired[ConfigurationOverridesTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConfigurationOverridesTypeDef](./type_defs.md#configurationoverridestypedef) 
## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    arn: NotRequired[str],
    virtualClusterId: NotRequired[str],
    type: NotRequired[str],
    state: NotRequired[EndpointStateType],  # (1)
    releaseLabel: NotRequired[str],
    executionRoleArn: NotRequired[str],
    certificateArn: NotRequired[str],
    certificateAuthority: NotRequired[CertificateTypeDef],  # (2)
    configurationOverrides: NotRequired[ConfigurationOverridesTypeDef],  # (3)
    serverUrl: NotRequired[str],
    createdAt: NotRequired[datetime],
    securityGroup: NotRequired[str],
    subnetIds: NotRequired[List[str]],
    stateDetails: NotRequired[str],
    failureReason: NotRequired[FailureReasonType],  # (4)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: EndpointStateType](./literals.md#endpointstatetype) 
2. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
3. See [:material-code-braces: ConfigurationOverridesTypeDef](./type_defs.md#configurationoverridestypedef) 
4. See [:material-code-brackets: FailureReasonType](./literals.md#failurereasontype) 
## JobRunTypeDef

```python
# JobRunTypeDef definition

class JobRunTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    virtualClusterId: NotRequired[str],
    arn: NotRequired[str],
    state: NotRequired[JobRunStateType],  # (1)
    clientToken: NotRequired[str],
    executionRoleArn: NotRequired[str],
    releaseLabel: NotRequired[str],
    configurationOverrides: NotRequired[ConfigurationOverridesTypeDef],  # (2)
    jobDriver: NotRequired[JobDriverTypeDef],  # (3)
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    finishedAt: NotRequired[datetime],
    stateDetails: NotRequired[str],
    failureReason: NotRequired[FailureReasonType],  # (4)
    tags: NotRequired[Dict[str, str]],
    retryPolicyConfiguration: NotRequired[RetryPolicyConfigurationTypeDef],  # (5)
    retryPolicyExecution: NotRequired[RetryPolicyExecutionTypeDef],  # (6)
```

1. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
2. See [:material-code-braces: ConfigurationOverridesTypeDef](./type_defs.md#configurationoverridestypedef) 
3. See [:material-code-braces: JobDriverTypeDef](./type_defs.md#jobdrivertypedef) 
4. See [:material-code-brackets: FailureReasonType](./literals.md#failurereasontype) 
5. See [:material-code-braces: RetryPolicyConfigurationTypeDef](./type_defs.md#retrypolicyconfigurationtypedef) 
6. See [:material-code-braces: RetryPolicyExecutionTypeDef](./type_defs.md#retrypolicyexecutiontypedef) 
## StartJobRunRequestRequestTypeDef

```python
# StartJobRunRequestRequestTypeDef definition

class StartJobRunRequestRequestTypeDef(TypedDict):
    virtualClusterId: str,
    clientToken: str,
    name: NotRequired[str],
    executionRoleArn: NotRequired[str],
    releaseLabel: NotRequired[str],
    jobDriver: NotRequired[JobDriverTypeDef],  # (1)
    configurationOverrides: NotRequired[ConfigurationOverridesTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
    jobTemplateId: NotRequired[str],
    jobTemplateParameters: NotRequired[Mapping[str, str]],
    retryPolicyConfiguration: NotRequired[RetryPolicyConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: JobDriverTypeDef](./type_defs.md#jobdrivertypedef) 
2. See [:material-code-braces: ConfigurationOverridesTypeDef](./type_defs.md#configurationoverridestypedef) 
3. See [:material-code-braces: RetryPolicyConfigurationTypeDef](./type_defs.md#retrypolicyconfigurationtypedef) 
## JobTemplateDataTypeDef

```python
# JobTemplateDataTypeDef definition

class JobTemplateDataTypeDef(TypedDict):
    executionRoleArn: str,
    releaseLabel: str,
    jobDriver: JobDriverTypeDef,  # (2)
    configurationOverrides: NotRequired[ParametricConfigurationOverridesTypeDef],  # (1)
    parameterConfiguration: NotRequired[Mapping[str, TemplateParameterConfigurationTypeDef]],  # (3)
    jobTags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ParametricConfigurationOverridesTypeDef](./type_defs.md#parametricconfigurationoverridestypedef) 
2. See [:material-code-braces: JobDriverTypeDef](./type_defs.md#jobdrivertypedef) 
3. See [:material-code-braces: TemplateParameterConfigurationTypeDef](./type_defs.md#templateparameterconfigurationtypedef) 
## DescribeVirtualClusterResponseTypeDef

```python
# DescribeVirtualClusterResponseTypeDef definition

class DescribeVirtualClusterResponseTypeDef(TypedDict):
    virtualCluster: VirtualClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualClusterTypeDef](./type_defs.md#virtualclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVirtualClustersResponseTypeDef

```python
# ListVirtualClustersResponseTypeDef definition

class ListVirtualClustersResponseTypeDef(TypedDict):
    virtualClusters: List[VirtualClusterTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualClusterTypeDef](./type_defs.md#virtualclustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeManagedEndpointResponseTypeDef

```python
# DescribeManagedEndpointResponseTypeDef definition

class DescribeManagedEndpointResponseTypeDef(TypedDict):
    endpoint: EndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListManagedEndpointsResponseTypeDef

```python
# ListManagedEndpointsResponseTypeDef definition

class ListManagedEndpointsResponseTypeDef(TypedDict):
    endpoints: List[EndpointTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeJobRunResponseTypeDef

```python
# DescribeJobRunResponseTypeDef definition

class DescribeJobRunResponseTypeDef(TypedDict):
    jobRun: JobRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobRunTypeDef](./type_defs.md#jobruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobRunsResponseTypeDef

```python
# ListJobRunsResponseTypeDef definition

class ListJobRunsResponseTypeDef(TypedDict):
    jobRuns: List[JobRunTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobRunTypeDef](./type_defs.md#jobruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobTemplateRequestRequestTypeDef

```python
# CreateJobTemplateRequestRequestTypeDef definition

class CreateJobTemplateRequestRequestTypeDef(TypedDict):
    name: str,
    clientToken: str,
    jobTemplateData: JobTemplateDataTypeDef,  # (1)
    tags: NotRequired[Mapping[str, str]],
    kmsKeyArn: NotRequired[str],
```

1. See [:material-code-braces: JobTemplateDataTypeDef](./type_defs.md#jobtemplatedatatypedef) 
## JobTemplateTypeDef

```python
# JobTemplateTypeDef definition

class JobTemplateTypeDef(TypedDict):
    jobTemplateData: JobTemplateDataTypeDef,  # (1)
    name: NotRequired[str],
    id: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    kmsKeyArn: NotRequired[str],
    decryptionError: NotRequired[str],
```

1. See [:material-code-braces: JobTemplateDataTypeDef](./type_defs.md#jobtemplatedatatypedef) 
## DescribeJobTemplateResponseTypeDef

```python
# DescribeJobTemplateResponseTypeDef definition

class DescribeJobTemplateResponseTypeDef(TypedDict):
    jobTemplate: JobTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobTemplatesResponseTypeDef

```python
# ListJobTemplatesResponseTypeDef definition

class ListJobTemplatesResponseTypeDef(TypedDict):
    templates: List[JobTemplateTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTemplateTypeDef](./type_defs.md#jobtemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
