# Type definitions

> [Index](../README.md) > [EventBridgePipes](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EventBridgePipes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#EventBridgePipes)
    type annotations stubs module [types-aiobotocore-pipes](https://pypi.org/project/types-aiobotocore-pipes/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AwsVpcConfigurationTypeDef

```python
# AwsVpcConfigurationTypeDef definition

class AwsVpcConfigurationTypeDef(TypedDict):
    Subnets: Sequence[str],
    AssignPublicIp: NotRequired[AssignPublicIpType],  # (1)
    SecurityGroups: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AssignPublicIpType](./literals.md#assignpubliciptype) 
## BatchArrayPropertiesTypeDef

```python
# BatchArrayPropertiesTypeDef definition

class BatchArrayPropertiesTypeDef(TypedDict):
    Size: NotRequired[int],
```

## BatchEnvironmentVariableTypeDef

```python
# BatchEnvironmentVariableTypeDef definition

class BatchEnvironmentVariableTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## BatchResourceRequirementTypeDef

```python
# BatchResourceRequirementTypeDef definition

class BatchResourceRequirementTypeDef(TypedDict):
    Type: BatchResourceRequirementTypeType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: BatchResourceRequirementTypeType](./literals.md#batchresourcerequirementtypetype) 
## BatchJobDependencyTypeDef

```python
# BatchJobDependencyTypeDef definition

class BatchJobDependencyTypeDef(TypedDict):
    JobId: NotRequired[str],
    Type: NotRequired[BatchJobDependencyTypeType],  # (1)
```

1. See [:material-code-brackets: BatchJobDependencyTypeType](./literals.md#batchjobdependencytypetype) 
## BatchRetryStrategyTypeDef

```python
# BatchRetryStrategyTypeDef definition

class BatchRetryStrategyTypeDef(TypedDict):
    Attempts: NotRequired[int],
```

## CapacityProviderStrategyItemTypeDef

```python
# CapacityProviderStrategyItemTypeDef definition

class CapacityProviderStrategyItemTypeDef(TypedDict):
    capacityProvider: str,
    base: NotRequired[int],
    weight: NotRequired[int],
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

## DeadLetterConfigTypeDef

```python
# DeadLetterConfigTypeDef definition

class DeadLetterConfigTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## DeletePipeRequestRequestTypeDef

```python
# DeletePipeRequestRequestTypeDef definition

class DeletePipeRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribePipeRequestRequestTypeDef

```python
# DescribePipeRequestRequestTypeDef definition

class DescribePipeRequestRequestTypeDef(TypedDict):
    Name: str,
```

## EcsEnvironmentFileTypeDef

```python
# EcsEnvironmentFileTypeDef definition

class EcsEnvironmentFileTypeDef(TypedDict):
    type: EcsEnvironmentFileTypeType,  # (1)
    value: str,
```

1. See [:material-code-brackets: EcsEnvironmentFileTypeType](./literals.md#ecsenvironmentfiletypetype) 
## EcsEnvironmentVariableTypeDef

```python
# EcsEnvironmentVariableTypeDef definition

class EcsEnvironmentVariableTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```

## EcsResourceRequirementTypeDef

```python
# EcsResourceRequirementTypeDef definition

class EcsResourceRequirementTypeDef(TypedDict):
    type: EcsResourceRequirementTypeType,  # (1)
    value: str,
```

1. See [:material-code-brackets: EcsResourceRequirementTypeType](./literals.md#ecsresourcerequirementtypetype) 
## EcsEphemeralStorageTypeDef

```python
# EcsEphemeralStorageTypeDef definition

class EcsEphemeralStorageTypeDef(TypedDict):
    sizeInGiB: int,
```

## EcsInferenceAcceleratorOverrideTypeDef

```python
# EcsInferenceAcceleratorOverrideTypeDef definition

class EcsInferenceAcceleratorOverrideTypeDef(TypedDict):
    deviceName: NotRequired[str],
    deviceType: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Pattern: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListPipesRequestRequestTypeDef

```python
# ListPipesRequestRequestTypeDef definition

class ListPipesRequestRequestTypeDef(TypedDict):
    CurrentState: NotRequired[PipeStateType],  # (1)
    DesiredState: NotRequired[RequestedPipeStateType],  # (2)
    Limit: NotRequired[int],
    NamePrefix: NotRequired[str],
    NextToken: NotRequired[str],
    SourcePrefix: NotRequired[str],
    TargetPrefix: NotRequired[str],
```

1. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
2. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
## PipeTypeDef

```python
# PipeTypeDef definition

class PipeTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreationTime: NotRequired[datetime],
    CurrentState: NotRequired[PipeStateType],  # (1)
    DesiredState: NotRequired[RequestedPipeStateType],  # (2)
    Enrichment: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
    Name: NotRequired[str],
    Source: NotRequired[str],
    StateReason: NotRequired[str],
    Target: NotRequired[str],
```

1. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
2. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## MQBrokerAccessCredentialsTypeDef

```python
# MQBrokerAccessCredentialsTypeDef definition

class MQBrokerAccessCredentialsTypeDef(TypedDict):
    BasicAuth: NotRequired[str],
```

## MSKAccessCredentialsTypeDef

```python
# MSKAccessCredentialsTypeDef definition

class MSKAccessCredentialsTypeDef(TypedDict):
    ClientCertificateTlsAuth: NotRequired[str],
    SaslScram512Auth: NotRequired[str],
```

## PipeEnrichmentHttpParametersTypeDef

```python
# PipeEnrichmentHttpParametersTypeDef definition

class PipeEnrichmentHttpParametersTypeDef(TypedDict):
    HeaderParameters: NotRequired[Mapping[str, str]],
    PathParameterValues: NotRequired[Sequence[str]],
    QueryStringParameters: NotRequired[Mapping[str, str]],
```

## PipeSourceSqsQueueParametersTypeDef

```python
# PipeSourceSqsQueueParametersTypeDef definition

class PipeSourceSqsQueueParametersTypeDef(TypedDict):
    BatchSize: NotRequired[int],
    MaximumBatchingWindowInSeconds: NotRequired[int],
```

## SelfManagedKafkaAccessConfigurationCredentialsTypeDef

```python
# SelfManagedKafkaAccessConfigurationCredentialsTypeDef definition

class SelfManagedKafkaAccessConfigurationCredentialsTypeDef(TypedDict):
    BasicAuth: NotRequired[str],
    ClientCertificateTlsAuth: NotRequired[str],
    SaslScram256Auth: NotRequired[str],
    SaslScram512Auth: NotRequired[str],
```

## SelfManagedKafkaAccessConfigurationVpcTypeDef

```python
# SelfManagedKafkaAccessConfigurationVpcTypeDef definition

class SelfManagedKafkaAccessConfigurationVpcTypeDef(TypedDict):
    SecurityGroup: NotRequired[Sequence[str]],
    Subnets: NotRequired[Sequence[str]],
```

## PipeTargetCloudWatchLogsParametersTypeDef

```python
# PipeTargetCloudWatchLogsParametersTypeDef definition

class PipeTargetCloudWatchLogsParametersTypeDef(TypedDict):
    LogStreamName: NotRequired[str],
    Timestamp: NotRequired[str],
```

## PlacementConstraintTypeDef

```python
# PlacementConstraintTypeDef definition

class PlacementConstraintTypeDef(TypedDict):
    expression: NotRequired[str],
    type: NotRequired[PlacementConstraintTypeType],  # (1)
```

1. See [:material-code-brackets: PlacementConstraintTypeType](./literals.md#placementconstrainttypetype) 
## PlacementStrategyTypeDef

```python
# PlacementStrategyTypeDef definition

class PlacementStrategyTypeDef(TypedDict):
    field: NotRequired[str],
    type: NotRequired[PlacementStrategyTypeType],  # (1)
```

1. See [:material-code-brackets: PlacementStrategyTypeType](./literals.md#placementstrategytypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## PipeTargetEventBridgeEventBusParametersTypeDef

```python
# PipeTargetEventBridgeEventBusParametersTypeDef definition

class PipeTargetEventBridgeEventBusParametersTypeDef(TypedDict):
    DetailType: NotRequired[str],
    EndpointId: NotRequired[str],
    Resources: NotRequired[Sequence[str]],
    Source: NotRequired[str],
    Time: NotRequired[str],
```

## PipeTargetHttpParametersTypeDef

```python
# PipeTargetHttpParametersTypeDef definition

class PipeTargetHttpParametersTypeDef(TypedDict):
    HeaderParameters: NotRequired[Mapping[str, str]],
    PathParameterValues: NotRequired[Sequence[str]],
    QueryStringParameters: NotRequired[Mapping[str, str]],
```

## PipeTargetKinesisStreamParametersTypeDef

```python
# PipeTargetKinesisStreamParametersTypeDef definition

class PipeTargetKinesisStreamParametersTypeDef(TypedDict):
    PartitionKey: str,
```

## PipeTargetLambdaFunctionParametersTypeDef

```python
# PipeTargetLambdaFunctionParametersTypeDef definition

class PipeTargetLambdaFunctionParametersTypeDef(TypedDict):
    InvocationType: NotRequired[PipeTargetInvocationTypeType],  # (1)
```

1. See [:material-code-brackets: PipeTargetInvocationTypeType](./literals.md#pipetargetinvocationtypetype) 
## PipeTargetRedshiftDataParametersTypeDef

```python
# PipeTargetRedshiftDataParametersTypeDef definition

class PipeTargetRedshiftDataParametersTypeDef(TypedDict):
    Database: str,
    Sqls: Sequence[str],
    DbUser: NotRequired[str],
    SecretManagerArn: NotRequired[str],
    StatementName: NotRequired[str],
    WithEvent: NotRequired[bool],
```

## PipeTargetSqsQueueParametersTypeDef

```python
# PipeTargetSqsQueueParametersTypeDef definition

class PipeTargetSqsQueueParametersTypeDef(TypedDict):
    MessageDeduplicationId: NotRequired[str],
    MessageGroupId: NotRequired[str],
```

## PipeTargetStateMachineParametersTypeDef

```python
# PipeTargetStateMachineParametersTypeDef definition

class PipeTargetStateMachineParametersTypeDef(TypedDict):
    InvocationType: NotRequired[PipeTargetInvocationTypeType],  # (1)
```

1. See [:material-code-brackets: PipeTargetInvocationTypeType](./literals.md#pipetargetinvocationtypetype) 
## SageMakerPipelineParameterTypeDef

```python
# SageMakerPipelineParameterTypeDef definition

class SageMakerPipelineParameterTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## StartPipeRequestRequestTypeDef

```python
# StartPipeRequestRequestTypeDef definition

class StartPipeRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StopPipeRequestRequestTypeDef

```python
# StopPipeRequestRequestTypeDef definition

class StopPipeRequestRequestTypeDef(TypedDict):
    Name: str,
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

## UpdatePipeSourceSqsQueueParametersTypeDef

```python
# UpdatePipeSourceSqsQueueParametersTypeDef definition

class UpdatePipeSourceSqsQueueParametersTypeDef(TypedDict):
    BatchSize: NotRequired[int],
    MaximumBatchingWindowInSeconds: NotRequired[int],
```

## NetworkConfigurationTypeDef

```python
# NetworkConfigurationTypeDef definition

class NetworkConfigurationTypeDef(TypedDict):
    awsvpcConfiguration: NotRequired[AwsVpcConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AwsVpcConfigurationTypeDef](./type_defs.md#awsvpcconfigurationtypedef) 
## BatchContainerOverridesTypeDef

```python
# BatchContainerOverridesTypeDef definition

class BatchContainerOverridesTypeDef(TypedDict):
    Command: NotRequired[Sequence[str]],
    Environment: NotRequired[Sequence[BatchEnvironmentVariableTypeDef]],  # (1)
    InstanceType: NotRequired[str],
    ResourceRequirements: NotRequired[Sequence[BatchResourceRequirementTypeDef]],  # (2)
```

1. See [:material-code-braces: BatchEnvironmentVariableTypeDef](./type_defs.md#batchenvironmentvariabletypedef) 
2. See [:material-code-braces: BatchResourceRequirementTypeDef](./type_defs.md#batchresourcerequirementtypedef) 
## CreatePipeResponseTypeDef

```python
# CreatePipeResponseTypeDef definition

class CreatePipeResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    CurrentState: PipeStateType,  # (1)
    DesiredState: RequestedPipeStateType,  # (2)
    LastModifiedTime: datetime,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
2. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePipeResponseTypeDef

```python
# DeletePipeResponseTypeDef definition

class DeletePipeResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    CurrentState: PipeStateType,  # (1)
    DesiredState: RequestedPipeStateDescribeResponseType,  # (2)
    LastModifiedTime: datetime,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
2. See [:material-code-brackets: RequestedPipeStateDescribeResponseType](./literals.md#requestedpipestatedescriberesponsetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPipeResponseTypeDef

```python
# StartPipeResponseTypeDef definition

class StartPipeResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    CurrentState: PipeStateType,  # (1)
    DesiredState: RequestedPipeStateType,  # (2)
    LastModifiedTime: datetime,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
2. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopPipeResponseTypeDef

```python
# StopPipeResponseTypeDef definition

class StopPipeResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    CurrentState: PipeStateType,  # (1)
    DesiredState: RequestedPipeStateType,  # (2)
    LastModifiedTime: datetime,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
2. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipeResponseTypeDef

```python
# UpdatePipeResponseTypeDef definition

class UpdatePipeResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    CurrentState: PipeStateType,  # (1)
    DesiredState: RequestedPipeStateType,  # (2)
    LastModifiedTime: datetime,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
2. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PipeSourceDynamoDBStreamParametersTypeDef

```python
# PipeSourceDynamoDBStreamParametersTypeDef definition

class PipeSourceDynamoDBStreamParametersTypeDef(TypedDict):
    StartingPosition: DynamoDBStreamStartPositionType,  # (3)
    BatchSize: NotRequired[int],
    DeadLetterConfig: NotRequired[DeadLetterConfigTypeDef],  # (1)
    MaximumBatchingWindowInSeconds: NotRequired[int],
    MaximumRecordAgeInSeconds: NotRequired[int],
    MaximumRetryAttempts: NotRequired[int],
    OnPartialBatchItemFailure: NotRequired[OnPartialBatchItemFailureStreamsType],  # (2)
    ParallelizationFactor: NotRequired[int],
```

1. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
2. See [:material-code-brackets: OnPartialBatchItemFailureStreamsType](./literals.md#onpartialbatchitemfailurestreamstype) 
3. See [:material-code-brackets: DynamoDBStreamStartPositionType](./literals.md#dynamodbstreamstartpositiontype) 
## UpdatePipeSourceDynamoDBStreamParametersTypeDef

```python
# UpdatePipeSourceDynamoDBStreamParametersTypeDef definition

class UpdatePipeSourceDynamoDBStreamParametersTypeDef(TypedDict):
    BatchSize: NotRequired[int],
    DeadLetterConfig: NotRequired[DeadLetterConfigTypeDef],  # (1)
    MaximumBatchingWindowInSeconds: NotRequired[int],
    MaximumRecordAgeInSeconds: NotRequired[int],
    MaximumRetryAttempts: NotRequired[int],
    OnPartialBatchItemFailure: NotRequired[OnPartialBatchItemFailureStreamsType],  # (2)
    ParallelizationFactor: NotRequired[int],
```

1. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
2. See [:material-code-brackets: OnPartialBatchItemFailureStreamsType](./literals.md#onpartialbatchitemfailurestreamstype) 
## UpdatePipeSourceKinesisStreamParametersTypeDef

```python
# UpdatePipeSourceKinesisStreamParametersTypeDef definition

class UpdatePipeSourceKinesisStreamParametersTypeDef(TypedDict):
    BatchSize: NotRequired[int],
    DeadLetterConfig: NotRequired[DeadLetterConfigTypeDef],  # (1)
    MaximumBatchingWindowInSeconds: NotRequired[int],
    MaximumRecordAgeInSeconds: NotRequired[int],
    MaximumRetryAttempts: NotRequired[int],
    OnPartialBatchItemFailure: NotRequired[OnPartialBatchItemFailureStreamsType],  # (2)
    ParallelizationFactor: NotRequired[int],
```

1. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
2. See [:material-code-brackets: OnPartialBatchItemFailureStreamsType](./literals.md#onpartialbatchitemfailurestreamstype) 
## EcsContainerOverrideTypeDef

```python
# EcsContainerOverrideTypeDef definition

class EcsContainerOverrideTypeDef(TypedDict):
    Command: NotRequired[Sequence[str]],
    Cpu: NotRequired[int],
    Environment: NotRequired[Sequence[EcsEnvironmentVariableTypeDef]],  # (1)
    EnvironmentFiles: NotRequired[Sequence[EcsEnvironmentFileTypeDef]],  # (2)
    Memory: NotRequired[int],
    MemoryReservation: NotRequired[int],
    Name: NotRequired[str],
    ResourceRequirements: NotRequired[Sequence[EcsResourceRequirementTypeDef]],  # (3)
```

1. See [:material-code-braces: EcsEnvironmentVariableTypeDef](./type_defs.md#ecsenvironmentvariabletypedef) 
2. See [:material-code-braces: EcsEnvironmentFileTypeDef](./type_defs.md#ecsenvironmentfiletypedef) 
3. See [:material-code-braces: EcsResourceRequirementTypeDef](./type_defs.md#ecsresourcerequirementtypedef) 
## FilterCriteriaTypeDef

```python
# FilterCriteriaTypeDef definition

class FilterCriteriaTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListPipesRequestListPipesPaginateTypeDef

```python
# ListPipesRequestListPipesPaginateTypeDef definition

class ListPipesRequestListPipesPaginateTypeDef(TypedDict):
    CurrentState: NotRequired[PipeStateType],  # (1)
    DesiredState: NotRequired[RequestedPipeStateType],  # (2)
    NamePrefix: NotRequired[str],
    SourcePrefix: NotRequired[str],
    TargetPrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
2. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipesResponseTypeDef

```python
# ListPipesResponseTypeDef definition

class ListPipesResponseTypeDef(TypedDict):
    NextToken: str,
    Pipes: List[PipeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipeTypeDef](./type_defs.md#pipetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PipeSourceActiveMQBrokerParametersTypeDef

```python
# PipeSourceActiveMQBrokerParametersTypeDef definition

class PipeSourceActiveMQBrokerParametersTypeDef(TypedDict):
    Credentials: MQBrokerAccessCredentialsTypeDef,  # (1)
    QueueName: str,
    BatchSize: NotRequired[int],
    MaximumBatchingWindowInSeconds: NotRequired[int],
```

1. See [:material-code-braces: MQBrokerAccessCredentialsTypeDef](./type_defs.md#mqbrokeraccesscredentialstypedef) 
## PipeSourceRabbitMQBrokerParametersTypeDef

```python
# PipeSourceRabbitMQBrokerParametersTypeDef definition

class PipeSourceRabbitMQBrokerParametersTypeDef(TypedDict):
    Credentials: MQBrokerAccessCredentialsTypeDef,  # (1)
    QueueName: str,
    BatchSize: NotRequired[int],
    MaximumBatchingWindowInSeconds: NotRequired[int],
    VirtualHost: NotRequired[str],
```

1. See [:material-code-braces: MQBrokerAccessCredentialsTypeDef](./type_defs.md#mqbrokeraccesscredentialstypedef) 
## UpdatePipeSourceActiveMQBrokerParametersTypeDef

```python
# UpdatePipeSourceActiveMQBrokerParametersTypeDef definition

class UpdatePipeSourceActiveMQBrokerParametersTypeDef(TypedDict):
    Credentials: MQBrokerAccessCredentialsTypeDef,  # (1)
    BatchSize: NotRequired[int],
    MaximumBatchingWindowInSeconds: NotRequired[int],
```

1. See [:material-code-braces: MQBrokerAccessCredentialsTypeDef](./type_defs.md#mqbrokeraccesscredentialstypedef) 
## UpdatePipeSourceRabbitMQBrokerParametersTypeDef

```python
# UpdatePipeSourceRabbitMQBrokerParametersTypeDef definition

class UpdatePipeSourceRabbitMQBrokerParametersTypeDef(TypedDict):
    Credentials: MQBrokerAccessCredentialsTypeDef,  # (1)
    BatchSize: NotRequired[int],
    MaximumBatchingWindowInSeconds: NotRequired[int],
```

1. See [:material-code-braces: MQBrokerAccessCredentialsTypeDef](./type_defs.md#mqbrokeraccesscredentialstypedef) 
## PipeSourceManagedStreamingKafkaParametersTypeDef

```python
# PipeSourceManagedStreamingKafkaParametersTypeDef definition

class PipeSourceManagedStreamingKafkaParametersTypeDef(TypedDict):
    TopicName: str,
    BatchSize: NotRequired[int],
    ConsumerGroupID: NotRequired[str],
    Credentials: NotRequired[MSKAccessCredentialsTypeDef],  # (1)
    MaximumBatchingWindowInSeconds: NotRequired[int],
    StartingPosition: NotRequired[MSKStartPositionType],  # (2)
```

1. See [:material-code-braces: MSKAccessCredentialsTypeDef](./type_defs.md#mskaccesscredentialstypedef) 
2. See [:material-code-brackets: MSKStartPositionType](./literals.md#mskstartpositiontype) 
## UpdatePipeSourceManagedStreamingKafkaParametersTypeDef

```python
# UpdatePipeSourceManagedStreamingKafkaParametersTypeDef definition

class UpdatePipeSourceManagedStreamingKafkaParametersTypeDef(TypedDict):
    BatchSize: NotRequired[int],
    Credentials: NotRequired[MSKAccessCredentialsTypeDef],  # (1)
    MaximumBatchingWindowInSeconds: NotRequired[int],
```

1. See [:material-code-braces: MSKAccessCredentialsTypeDef](./type_defs.md#mskaccesscredentialstypedef) 
## PipeEnrichmentParametersTypeDef

```python
# PipeEnrichmentParametersTypeDef definition

class PipeEnrichmentParametersTypeDef(TypedDict):
    HttpParameters: NotRequired[PipeEnrichmentHttpParametersTypeDef],  # (1)
    InputTemplate: NotRequired[str],
```

1. See [:material-code-braces: PipeEnrichmentHttpParametersTypeDef](./type_defs.md#pipeenrichmenthttpparameterstypedef) 
## PipeSourceKinesisStreamParametersTypeDef

```python
# PipeSourceKinesisStreamParametersTypeDef definition

class PipeSourceKinesisStreamParametersTypeDef(TypedDict):
    StartingPosition: KinesisStreamStartPositionType,  # (3)
    BatchSize: NotRequired[int],
    DeadLetterConfig: NotRequired[DeadLetterConfigTypeDef],  # (1)
    MaximumBatchingWindowInSeconds: NotRequired[int],
    MaximumRecordAgeInSeconds: NotRequired[int],
    MaximumRetryAttempts: NotRequired[int],
    OnPartialBatchItemFailure: NotRequired[OnPartialBatchItemFailureStreamsType],  # (2)
    ParallelizationFactor: NotRequired[int],
    StartingPositionTimestamp: NotRequired[Union[datetime, str]],
```

1. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
2. See [:material-code-brackets: OnPartialBatchItemFailureStreamsType](./literals.md#onpartialbatchitemfailurestreamstype) 
3. See [:material-code-brackets: KinesisStreamStartPositionType](./literals.md#kinesisstreamstartpositiontype) 
## PipeSourceSelfManagedKafkaParametersTypeDef

```python
# PipeSourceSelfManagedKafkaParametersTypeDef definition

class PipeSourceSelfManagedKafkaParametersTypeDef(TypedDict):
    TopicName: str,
    AdditionalBootstrapServers: NotRequired[Sequence[str]],
    BatchSize: NotRequired[int],
    ConsumerGroupID: NotRequired[str],
    Credentials: NotRequired[SelfManagedKafkaAccessConfigurationCredentialsTypeDef],  # (1)
    MaximumBatchingWindowInSeconds: NotRequired[int],
    ServerRootCaCertificate: NotRequired[str],
    StartingPosition: NotRequired[SelfManagedKafkaStartPositionType],  # (2)
    Vpc: NotRequired[SelfManagedKafkaAccessConfigurationVpcTypeDef],  # (3)
```

1. See [:material-code-braces: SelfManagedKafkaAccessConfigurationCredentialsTypeDef](./type_defs.md#selfmanagedkafkaaccessconfigurationcredentialstypedef) 
2. See [:material-code-brackets: SelfManagedKafkaStartPositionType](./literals.md#selfmanagedkafkastartpositiontype) 
3. See [:material-code-braces: SelfManagedKafkaAccessConfigurationVpcTypeDef](./type_defs.md#selfmanagedkafkaaccessconfigurationvpctypedef) 
## UpdatePipeSourceSelfManagedKafkaParametersTypeDef

```python
# UpdatePipeSourceSelfManagedKafkaParametersTypeDef definition

class UpdatePipeSourceSelfManagedKafkaParametersTypeDef(TypedDict):
    BatchSize: NotRequired[int],
    Credentials: NotRequired[SelfManagedKafkaAccessConfigurationCredentialsTypeDef],  # (1)
    MaximumBatchingWindowInSeconds: NotRequired[int],
    ServerRootCaCertificate: NotRequired[str],
    Vpc: NotRequired[SelfManagedKafkaAccessConfigurationVpcTypeDef],  # (2)
```

1. See [:material-code-braces: SelfManagedKafkaAccessConfigurationCredentialsTypeDef](./type_defs.md#selfmanagedkafkaaccessconfigurationcredentialstypedef) 
2. See [:material-code-braces: SelfManagedKafkaAccessConfigurationVpcTypeDef](./type_defs.md#selfmanagedkafkaaccessconfigurationvpctypedef) 
## PipeTargetSageMakerPipelineParametersTypeDef

```python
# PipeTargetSageMakerPipelineParametersTypeDef definition

class PipeTargetSageMakerPipelineParametersTypeDef(TypedDict):
    PipelineParameterList: NotRequired[Sequence[SageMakerPipelineParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: SageMakerPipelineParameterTypeDef](./type_defs.md#sagemakerpipelineparametertypedef) 
## PipeTargetBatchJobParametersTypeDef

```python
# PipeTargetBatchJobParametersTypeDef definition

class PipeTargetBatchJobParametersTypeDef(TypedDict):
    JobDefinition: str,
    JobName: str,
    ArrayProperties: NotRequired[BatchArrayPropertiesTypeDef],  # (1)
    ContainerOverrides: NotRequired[BatchContainerOverridesTypeDef],  # (2)
    DependsOn: NotRequired[Sequence[BatchJobDependencyTypeDef]],  # (3)
    Parameters: NotRequired[Mapping[str, str]],
    RetryStrategy: NotRequired[BatchRetryStrategyTypeDef],  # (4)
```

1. See [:material-code-braces: BatchArrayPropertiesTypeDef](./type_defs.md#batcharraypropertiestypedef) 
2. See [:material-code-braces: BatchContainerOverridesTypeDef](./type_defs.md#batchcontaineroverridestypedef) 
3. See [:material-code-braces: BatchJobDependencyTypeDef](./type_defs.md#batchjobdependencytypedef) 
4. See [:material-code-braces: BatchRetryStrategyTypeDef](./type_defs.md#batchretrystrategytypedef) 
## EcsTaskOverrideTypeDef

```python
# EcsTaskOverrideTypeDef definition

class EcsTaskOverrideTypeDef(TypedDict):
    ContainerOverrides: NotRequired[Sequence[EcsContainerOverrideTypeDef]],  # (1)
    Cpu: NotRequired[str],
    EphemeralStorage: NotRequired[EcsEphemeralStorageTypeDef],  # (2)
    ExecutionRoleArn: NotRequired[str],
    InferenceAcceleratorOverrides: NotRequired[Sequence[EcsInferenceAcceleratorOverrideTypeDef]],  # (3)
    Memory: NotRequired[str],
    TaskRoleArn: NotRequired[str],
```

1. See [:material-code-braces: EcsContainerOverrideTypeDef](./type_defs.md#ecscontaineroverridetypedef) 
2. See [:material-code-braces: EcsEphemeralStorageTypeDef](./type_defs.md#ecsephemeralstoragetypedef) 
3. See [:material-code-braces: EcsInferenceAcceleratorOverrideTypeDef](./type_defs.md#ecsinferenceacceleratoroverridetypedef) 
## PipeSourceParametersTypeDef

```python
# PipeSourceParametersTypeDef definition

class PipeSourceParametersTypeDef(TypedDict):
    ActiveMQBrokerParameters: NotRequired[PipeSourceActiveMQBrokerParametersTypeDef],  # (1)
    DynamoDBStreamParameters: NotRequired[PipeSourceDynamoDBStreamParametersTypeDef],  # (2)
    FilterCriteria: NotRequired[FilterCriteriaTypeDef],  # (3)
    KinesisStreamParameters: NotRequired[PipeSourceKinesisStreamParametersTypeDef],  # (4)
    ManagedStreamingKafkaParameters: NotRequired[PipeSourceManagedStreamingKafkaParametersTypeDef],  # (5)
    RabbitMQBrokerParameters: NotRequired[PipeSourceRabbitMQBrokerParametersTypeDef],  # (6)
    SelfManagedKafkaParameters: NotRequired[PipeSourceSelfManagedKafkaParametersTypeDef],  # (7)
    SqsQueueParameters: NotRequired[PipeSourceSqsQueueParametersTypeDef],  # (8)
```

1. See [:material-code-braces: PipeSourceActiveMQBrokerParametersTypeDef](./type_defs.md#pipesourceactivemqbrokerparameterstypedef) 
2. See [:material-code-braces: PipeSourceDynamoDBStreamParametersTypeDef](./type_defs.md#pipesourcedynamodbstreamparameterstypedef) 
3. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
4. See [:material-code-braces: PipeSourceKinesisStreamParametersTypeDef](./type_defs.md#pipesourcekinesisstreamparameterstypedef) 
5. See [:material-code-braces: PipeSourceManagedStreamingKafkaParametersTypeDef](./type_defs.md#pipesourcemanagedstreamingkafkaparameterstypedef) 
6. See [:material-code-braces: PipeSourceRabbitMQBrokerParametersTypeDef](./type_defs.md#pipesourcerabbitmqbrokerparameterstypedef) 
7. See [:material-code-braces: PipeSourceSelfManagedKafkaParametersTypeDef](./type_defs.md#pipesourceselfmanagedkafkaparameterstypedef) 
8. See [:material-code-braces: PipeSourceSqsQueueParametersTypeDef](./type_defs.md#pipesourcesqsqueueparameterstypedef) 
## UpdatePipeSourceParametersTypeDef

```python
# UpdatePipeSourceParametersTypeDef definition

class UpdatePipeSourceParametersTypeDef(TypedDict):
    ActiveMQBrokerParameters: NotRequired[UpdatePipeSourceActiveMQBrokerParametersTypeDef],  # (1)
    DynamoDBStreamParameters: NotRequired[UpdatePipeSourceDynamoDBStreamParametersTypeDef],  # (2)
    FilterCriteria: NotRequired[FilterCriteriaTypeDef],  # (3)
    KinesisStreamParameters: NotRequired[UpdatePipeSourceKinesisStreamParametersTypeDef],  # (4)
    ManagedStreamingKafkaParameters: NotRequired[UpdatePipeSourceManagedStreamingKafkaParametersTypeDef],  # (5)
    RabbitMQBrokerParameters: NotRequired[UpdatePipeSourceRabbitMQBrokerParametersTypeDef],  # (6)
    SelfManagedKafkaParameters: NotRequired[UpdatePipeSourceSelfManagedKafkaParametersTypeDef],  # (7)
    SqsQueueParameters: NotRequired[UpdatePipeSourceSqsQueueParametersTypeDef],  # (8)
```

1. See [:material-code-braces: UpdatePipeSourceActiveMQBrokerParametersTypeDef](./type_defs.md#updatepipesourceactivemqbrokerparameterstypedef) 
2. See [:material-code-braces: UpdatePipeSourceDynamoDBStreamParametersTypeDef](./type_defs.md#updatepipesourcedynamodbstreamparameterstypedef) 
3. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
4. See [:material-code-braces: UpdatePipeSourceKinesisStreamParametersTypeDef](./type_defs.md#updatepipesourcekinesisstreamparameterstypedef) 
5. See [:material-code-braces: UpdatePipeSourceManagedStreamingKafkaParametersTypeDef](./type_defs.md#updatepipesourcemanagedstreamingkafkaparameterstypedef) 
6. See [:material-code-braces: UpdatePipeSourceRabbitMQBrokerParametersTypeDef](./type_defs.md#updatepipesourcerabbitmqbrokerparameterstypedef) 
7. See [:material-code-braces: UpdatePipeSourceSelfManagedKafkaParametersTypeDef](./type_defs.md#updatepipesourceselfmanagedkafkaparameterstypedef) 
8. See [:material-code-braces: UpdatePipeSourceSqsQueueParametersTypeDef](./type_defs.md#updatepipesourcesqsqueueparameterstypedef) 
## PipeTargetEcsTaskParametersTypeDef

```python
# PipeTargetEcsTaskParametersTypeDef definition

class PipeTargetEcsTaskParametersTypeDef(TypedDict):
    TaskDefinitionArn: str,
    CapacityProviderStrategy: NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],  # (1)
    EnableECSManagedTags: NotRequired[bool],
    EnableExecuteCommand: NotRequired[bool],
    Group: NotRequired[str],
    LaunchType: NotRequired[LaunchTypeType],  # (2)
    NetworkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (3)
    Overrides: NotRequired[EcsTaskOverrideTypeDef],  # (4)
    PlacementConstraints: NotRequired[Sequence[PlacementConstraintTypeDef]],  # (5)
    PlacementStrategy: NotRequired[Sequence[PlacementStrategyTypeDef]],  # (6)
    PlatformVersion: NotRequired[str],
    PropagateTags: NotRequired[PropagateTagsType],  # (7)
    ReferenceId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (8)
    TaskCount: NotRequired[int],
```

1. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
2. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
3. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
4. See [:material-code-braces: EcsTaskOverrideTypeDef](./type_defs.md#ecstaskoverridetypedef) 
5. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
6. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
7. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PipeTargetParametersTypeDef

```python
# PipeTargetParametersTypeDef definition

class PipeTargetParametersTypeDef(TypedDict):
    BatchJobParameters: NotRequired[PipeTargetBatchJobParametersTypeDef],  # (1)
    CloudWatchLogsParameters: NotRequired[PipeTargetCloudWatchLogsParametersTypeDef],  # (2)
    EcsTaskParameters: NotRequired[PipeTargetEcsTaskParametersTypeDef],  # (3)
    EventBridgeEventBusParameters: NotRequired[PipeTargetEventBridgeEventBusParametersTypeDef],  # (4)
    HttpParameters: NotRequired[PipeTargetHttpParametersTypeDef],  # (5)
    InputTemplate: NotRequired[str],
    KinesisStreamParameters: NotRequired[PipeTargetKinesisStreamParametersTypeDef],  # (6)
    LambdaFunctionParameters: NotRequired[PipeTargetLambdaFunctionParametersTypeDef],  # (7)
    RedshiftDataParameters: NotRequired[PipeTargetRedshiftDataParametersTypeDef],  # (8)
    SageMakerPipelineParameters: NotRequired[PipeTargetSageMakerPipelineParametersTypeDef],  # (9)
    SqsQueueParameters: NotRequired[PipeTargetSqsQueueParametersTypeDef],  # (10)
    StepFunctionStateMachineParameters: NotRequired[PipeTargetStateMachineParametersTypeDef],  # (11)
```

1. See [:material-code-braces: PipeTargetBatchJobParametersTypeDef](./type_defs.md#pipetargetbatchjobparameterstypedef) 
2. See [:material-code-braces: PipeTargetCloudWatchLogsParametersTypeDef](./type_defs.md#pipetargetcloudwatchlogsparameterstypedef) 
3. See [:material-code-braces: PipeTargetEcsTaskParametersTypeDef](./type_defs.md#pipetargetecstaskparameterstypedef) 
4. See [:material-code-braces: PipeTargetEventBridgeEventBusParametersTypeDef](./type_defs.md#pipetargeteventbridgeeventbusparameterstypedef) 
5. See [:material-code-braces: PipeTargetHttpParametersTypeDef](./type_defs.md#pipetargethttpparameterstypedef) 
6. See [:material-code-braces: PipeTargetKinesisStreamParametersTypeDef](./type_defs.md#pipetargetkinesisstreamparameterstypedef) 
7. See [:material-code-braces: PipeTargetLambdaFunctionParametersTypeDef](./type_defs.md#pipetargetlambdafunctionparameterstypedef) 
8. See [:material-code-braces: PipeTargetRedshiftDataParametersTypeDef](./type_defs.md#pipetargetredshiftdataparameterstypedef) 
9. See [:material-code-braces: PipeTargetSageMakerPipelineParametersTypeDef](./type_defs.md#pipetargetsagemakerpipelineparameterstypedef) 
10. See [:material-code-braces: PipeTargetSqsQueueParametersTypeDef](./type_defs.md#pipetargetsqsqueueparameterstypedef) 
11. See [:material-code-braces: PipeTargetStateMachineParametersTypeDef](./type_defs.md#pipetargetstatemachineparameterstypedef) 
## CreatePipeRequestRequestTypeDef

```python
# CreatePipeRequestRequestTypeDef definition

class CreatePipeRequestRequestTypeDef(TypedDict):
    Name: str,
    RoleArn: str,
    Source: str,
    Target: str,
    Description: NotRequired[str],
    DesiredState: NotRequired[RequestedPipeStateType],  # (1)
    Enrichment: NotRequired[str],
    EnrichmentParameters: NotRequired[PipeEnrichmentParametersTypeDef],  # (2)
    SourceParameters: NotRequired[PipeSourceParametersTypeDef],  # (3)
    Tags: NotRequired[Mapping[str, str]],
    TargetParameters: NotRequired[PipeTargetParametersTypeDef],  # (4)
```

1. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
2. See [:material-code-braces: PipeEnrichmentParametersTypeDef](./type_defs.md#pipeenrichmentparameterstypedef) 
3. See [:material-code-braces: PipeSourceParametersTypeDef](./type_defs.md#pipesourceparameterstypedef) 
4. See [:material-code-braces: PipeTargetParametersTypeDef](./type_defs.md#pipetargetparameterstypedef) 
## DescribePipeResponseTypeDef

```python
# DescribePipeResponseTypeDef definition

class DescribePipeResponseTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    CurrentState: PipeStateType,  # (1)
    Description: str,
    DesiredState: RequestedPipeStateDescribeResponseType,  # (2)
    Enrichment: str,
    EnrichmentParameters: PipeEnrichmentParametersTypeDef,  # (3)
    LastModifiedTime: datetime,
    Name: str,
    RoleArn: str,
    Source: str,
    SourceParameters: PipeSourceParametersTypeDef,  # (4)
    StateReason: str,
    Tags: Dict[str, str],
    Target: str,
    TargetParameters: PipeTargetParametersTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: PipeStateType](./literals.md#pipestatetype) 
2. See [:material-code-brackets: RequestedPipeStateDescribeResponseType](./literals.md#requestedpipestatedescriberesponsetype) 
3. See [:material-code-braces: PipeEnrichmentParametersTypeDef](./type_defs.md#pipeenrichmentparameterstypedef) 
4. See [:material-code-braces: PipeSourceParametersTypeDef](./type_defs.md#pipesourceparameterstypedef) 
5. See [:material-code-braces: PipeTargetParametersTypeDef](./type_defs.md#pipetargetparameterstypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipeRequestRequestTypeDef

```python
# UpdatePipeRequestRequestTypeDef definition

class UpdatePipeRequestRequestTypeDef(TypedDict):
    Name: str,
    RoleArn: str,
    Description: NotRequired[str],
    DesiredState: NotRequired[RequestedPipeStateType],  # (1)
    Enrichment: NotRequired[str],
    EnrichmentParameters: NotRequired[PipeEnrichmentParametersTypeDef],  # (2)
    SourceParameters: NotRequired[UpdatePipeSourceParametersTypeDef],  # (3)
    Target: NotRequired[str],
    TargetParameters: NotRequired[PipeTargetParametersTypeDef],  # (4)
```

1. See [:material-code-brackets: RequestedPipeStateType](./literals.md#requestedpipestatetype) 
2. See [:material-code-braces: PipeEnrichmentParametersTypeDef](./type_defs.md#pipeenrichmentparameterstypedef) 
3. See [:material-code-braces: UpdatePipeSourceParametersTypeDef](./type_defs.md#updatepipesourceparameterstypedef) 
4. See [:material-code-braces: PipeTargetParametersTypeDef](./type_defs.md#pipetargetparameterstypedef) 
