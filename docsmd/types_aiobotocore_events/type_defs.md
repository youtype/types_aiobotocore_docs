# Type definitions

> [Index](../README.md) > [EventBridge](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EventBridge](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
    type annotations stubs module [types-aiobotocore-events](https://pypi.org/project/types-aiobotocore-events/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ActivateEventSourceRequestRequestTypeDef

```python
# ActivateEventSourceRequestRequestTypeDef definition

class ActivateEventSourceRequestRequestTypeDef(TypedDict):
    Name: str,
```

## ApiDestinationTypeDef

```python
# ApiDestinationTypeDef definition

class ApiDestinationTypeDef(TypedDict):
    ApiDestinationArn: NotRequired[str],
    Name: NotRequired[str],
    ApiDestinationState: NotRequired[ApiDestinationStateType],  # (1)
    ConnectionArn: NotRequired[str],
    InvocationEndpoint: NotRequired[str],
    HttpMethod: NotRequired[ApiDestinationHttpMethodType],  # (2)
    InvocationRateLimitPerSecond: NotRequired[int],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ApiDestinationStateType](./literals.md#apidestinationstatetype) 
2. See [:material-code-brackets: ApiDestinationHttpMethodType](./literals.md#apidestinationhttpmethodtype) 
## ArchiveTypeDef

```python
# ArchiveTypeDef definition

class ArchiveTypeDef(TypedDict):
    ArchiveName: NotRequired[str],
    EventSourceArn: NotRequired[str],
    State: NotRequired[ArchiveStateType],  # (1)
    StateReason: NotRequired[str],
    RetentionDays: NotRequired[int],
    SizeBytes: NotRequired[int],
    EventCount: NotRequired[int],
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ArchiveStateType](./literals.md#archivestatetype) 
## AwsVpcConfigurationTypeDef

```python
# AwsVpcConfigurationTypeDef definition

class AwsVpcConfigurationTypeDef(TypedDict):
    Subnets: List[str],
    SecurityGroups: NotRequired[List[str]],
    AssignPublicIp: NotRequired[AssignPublicIpType],  # (1)
```

1. See [:material-code-brackets: AssignPublicIpType](./literals.md#assignpubliciptype) 
## BatchArrayPropertiesTypeDef

```python
# BatchArrayPropertiesTypeDef definition

class BatchArrayPropertiesTypeDef(TypedDict):
    Size: NotRequired[int],
```

## BatchRetryStrategyTypeDef

```python
# BatchRetryStrategyTypeDef definition

class BatchRetryStrategyTypeDef(TypedDict):
    Attempts: NotRequired[int],
```

## CancelReplayRequestRequestTypeDef

```python
# CancelReplayRequestRequestTypeDef definition

class CancelReplayRequestRequestTypeDef(TypedDict):
    ReplayName: str,
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

## CapacityProviderStrategyItemTypeDef

```python
# CapacityProviderStrategyItemTypeDef definition

class CapacityProviderStrategyItemTypeDef(TypedDict):
    capacityProvider: str,
    weight: NotRequired[int],
    base: NotRequired[int],
```

## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    Type: str,
    Key: str,
    Value: str,
```

## ConnectionApiKeyAuthResponseParametersTypeDef

```python
# ConnectionApiKeyAuthResponseParametersTypeDef definition

class ConnectionApiKeyAuthResponseParametersTypeDef(TypedDict):
    ApiKeyName: NotRequired[str],
```

## ConnectionBasicAuthResponseParametersTypeDef

```python
# ConnectionBasicAuthResponseParametersTypeDef definition

class ConnectionBasicAuthResponseParametersTypeDef(TypedDict):
    Username: NotRequired[str],
```

## ConnectionBodyParameterTypeDef

```python
# ConnectionBodyParameterTypeDef definition

class ConnectionBodyParameterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    IsValueSecret: NotRequired[bool],
```

## ConnectionHeaderParameterTypeDef

```python
# ConnectionHeaderParameterTypeDef definition

class ConnectionHeaderParameterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    IsValueSecret: NotRequired[bool],
```

## ConnectionQueryStringParameterTypeDef

```python
# ConnectionQueryStringParameterTypeDef definition

class ConnectionQueryStringParameterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    IsValueSecret: NotRequired[bool],
```

## ConnectionOAuthClientResponseParametersTypeDef

```python
# ConnectionOAuthClientResponseParametersTypeDef definition

class ConnectionOAuthClientResponseParametersTypeDef(TypedDict):
    ClientID: NotRequired[str],
```

## ConnectionTypeDef

```python
# ConnectionTypeDef definition

class ConnectionTypeDef(TypedDict):
    ConnectionArn: NotRequired[str],
    Name: NotRequired[str],
    ConnectionState: NotRequired[ConnectionStateType],  # (1)
    StateReason: NotRequired[str],
    AuthorizationType: NotRequired[ConnectionAuthorizationTypeType],  # (2)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    LastAuthorizedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
2. See [:material-code-brackets: ConnectionAuthorizationTypeType](./literals.md#connectionauthorizationtypetype) 
## CreateApiDestinationRequestRequestTypeDef

```python
# CreateApiDestinationRequestRequestTypeDef definition

class CreateApiDestinationRequestRequestTypeDef(TypedDict):
    Name: str,
    ConnectionArn: str,
    InvocationEndpoint: str,
    HttpMethod: ApiDestinationHttpMethodType,  # (1)
    Description: NotRequired[str],
    InvocationRateLimitPerSecond: NotRequired[int],
```

1. See [:material-code-brackets: ApiDestinationHttpMethodType](./literals.md#apidestinationhttpmethodtype) 
## CreateArchiveRequestRequestTypeDef

```python
# CreateArchiveRequestRequestTypeDef definition

class CreateArchiveRequestRequestTypeDef(TypedDict):
    ArchiveName: str,
    EventSourceArn: str,
    Description: NotRequired[str],
    EventPattern: NotRequired[str],
    RetentionDays: NotRequired[int],
```

## CreateConnectionApiKeyAuthRequestParametersTypeDef

```python
# CreateConnectionApiKeyAuthRequestParametersTypeDef definition

class CreateConnectionApiKeyAuthRequestParametersTypeDef(TypedDict):
    ApiKeyName: str,
    ApiKeyValue: str,
```

## CreateConnectionBasicAuthRequestParametersTypeDef

```python
# CreateConnectionBasicAuthRequestParametersTypeDef definition

class CreateConnectionBasicAuthRequestParametersTypeDef(TypedDict):
    Username: str,
    Password: str,
```

## CreateConnectionOAuthClientRequestParametersTypeDef

```python
# CreateConnectionOAuthClientRequestParametersTypeDef definition

class CreateConnectionOAuthClientRequestParametersTypeDef(TypedDict):
    ClientID: str,
    ClientSecret: str,
```

## EndpointEventBusTypeDef

```python
# EndpointEventBusTypeDef definition

class EndpointEventBusTypeDef(TypedDict):
    EventBusArn: str,
```

## ReplicationConfigTypeDef

```python
# ReplicationConfigTypeDef definition

class ReplicationConfigTypeDef(TypedDict):
    State: NotRequired[ReplicationStateType],  # (1)
```

1. See [:material-code-brackets: ReplicationStateType](./literals.md#replicationstatetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreatePartnerEventSourceRequestRequestTypeDef

```python
# CreatePartnerEventSourceRequestRequestTypeDef definition

class CreatePartnerEventSourceRequestRequestTypeDef(TypedDict):
    Name: str,
    Account: str,
```

## DeactivateEventSourceRequestRequestTypeDef

```python
# DeactivateEventSourceRequestRequestTypeDef definition

class DeactivateEventSourceRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeadLetterConfigTypeDef

```python
# DeadLetterConfigTypeDef definition

class DeadLetterConfigTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## DeauthorizeConnectionRequestRequestTypeDef

```python
# DeauthorizeConnectionRequestRequestTypeDef definition

class DeauthorizeConnectionRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteApiDestinationRequestRequestTypeDef

```python
# DeleteApiDestinationRequestRequestTypeDef definition

class DeleteApiDestinationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteArchiveRequestRequestTypeDef

```python
# DeleteArchiveRequestRequestTypeDef definition

class DeleteArchiveRequestRequestTypeDef(TypedDict):
    ArchiveName: str,
```

## DeleteConnectionRequestRequestTypeDef

```python
# DeleteConnectionRequestRequestTypeDef definition

class DeleteConnectionRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteEndpointRequestRequestTypeDef

```python
# DeleteEndpointRequestRequestTypeDef definition

class DeleteEndpointRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteEventBusRequestRequestTypeDef

```python
# DeleteEventBusRequestRequestTypeDef definition

class DeleteEventBusRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeletePartnerEventSourceRequestRequestTypeDef

```python
# DeletePartnerEventSourceRequestRequestTypeDef definition

class DeletePartnerEventSourceRequestRequestTypeDef(TypedDict):
    Name: str,
    Account: str,
```

## DeleteRuleRequestRequestTypeDef

```python
# DeleteRuleRequestRequestTypeDef definition

class DeleteRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    EventBusName: NotRequired[str],
    Force: NotRequired[bool],
```

## DescribeApiDestinationRequestRequestTypeDef

```python
# DescribeApiDestinationRequestRequestTypeDef definition

class DescribeApiDestinationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeArchiveRequestRequestTypeDef

```python
# DescribeArchiveRequestRequestTypeDef definition

class DescribeArchiveRequestRequestTypeDef(TypedDict):
    ArchiveName: str,
```

## DescribeConnectionRequestRequestTypeDef

```python
# DescribeConnectionRequestRequestTypeDef definition

class DescribeConnectionRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeEndpointRequestRequestTypeDef

```python
# DescribeEndpointRequestRequestTypeDef definition

class DescribeEndpointRequestRequestTypeDef(TypedDict):
    Name: str,
    HomeRegion: NotRequired[str],
```

## DescribeEventBusRequestRequestTypeDef

```python
# DescribeEventBusRequestRequestTypeDef definition

class DescribeEventBusRequestRequestTypeDef(TypedDict):
    Name: NotRequired[str],
```

## DescribeEventSourceRequestRequestTypeDef

```python
# DescribeEventSourceRequestRequestTypeDef definition

class DescribeEventSourceRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribePartnerEventSourceRequestRequestTypeDef

```python
# DescribePartnerEventSourceRequestRequestTypeDef definition

class DescribePartnerEventSourceRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DescribeReplayRequestRequestTypeDef

```python
# DescribeReplayRequestRequestTypeDef definition

class DescribeReplayRequestRequestTypeDef(TypedDict):
    ReplayName: str,
```

## ReplayDestinationTypeDef

```python
# ReplayDestinationTypeDef definition

class ReplayDestinationTypeDef(TypedDict):
    Arn: str,
    FilterArns: NotRequired[List[str]],
```

## DescribeRuleRequestRequestTypeDef

```python
# DescribeRuleRequestRequestTypeDef definition

class DescribeRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    EventBusName: NotRequired[str],
```

## DisableRuleRequestRequestTypeDef

```python
# DisableRuleRequestRequestTypeDef definition

class DisableRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    EventBusName: NotRequired[str],
```

## PlacementConstraintTypeDef

```python
# PlacementConstraintTypeDef definition

class PlacementConstraintTypeDef(TypedDict):
    type: NotRequired[PlacementConstraintTypeType],  # (1)
    expression: NotRequired[str],
```

1. See [:material-code-brackets: PlacementConstraintTypeType](./literals.md#placementconstrainttypetype) 
## PlacementStrategyTypeDef

```python
# PlacementStrategyTypeDef definition

class PlacementStrategyTypeDef(TypedDict):
    type: NotRequired[PlacementStrategyTypeType],  # (1)
    field: NotRequired[str],
```

1. See [:material-code-brackets: PlacementStrategyTypeType](./literals.md#placementstrategytypetype) 
## EnableRuleRequestRequestTypeDef

```python
# EnableRuleRequestRequestTypeDef definition

class EnableRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    EventBusName: NotRequired[str],
```

## EventBusTypeDef

```python
# EventBusTypeDef definition

class EventBusTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Policy: NotRequired[str],
```

## EventSourceTypeDef

```python
# EventSourceTypeDef definition

class EventSourceTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedBy: NotRequired[str],
    CreationTime: NotRequired[datetime],
    ExpirationTime: NotRequired[datetime],
    Name: NotRequired[str],
    State: NotRequired[EventSourceStateType],  # (1)
```

1. See [:material-code-brackets: EventSourceStateType](./literals.md#eventsourcestatetype) 
## PrimaryTypeDef

```python
# PrimaryTypeDef definition

class PrimaryTypeDef(TypedDict):
    HealthCheck: str,
```

## SecondaryTypeDef

```python
# SecondaryTypeDef definition

class SecondaryTypeDef(TypedDict):
    Route: str,
```

## HttpParametersTypeDef

```python
# HttpParametersTypeDef definition

class HttpParametersTypeDef(TypedDict):
    PathParameterValues: NotRequired[List[str]],
    HeaderParameters: NotRequired[Dict[str, str]],
    QueryStringParameters: NotRequired[Dict[str, str]],
```

## InputTransformerTypeDef

```python
# InputTransformerTypeDef definition

class InputTransformerTypeDef(TypedDict):
    InputTemplate: str,
    InputPathsMap: NotRequired[Dict[str, str]],
```

## KinesisParametersTypeDef

```python
# KinesisParametersTypeDef definition

class KinesisParametersTypeDef(TypedDict):
    PartitionKeyPath: str,
```

## ListApiDestinationsRequestRequestTypeDef

```python
# ListApiDestinationsRequestRequestTypeDef definition

class ListApiDestinationsRequestRequestTypeDef(TypedDict):
    NamePrefix: NotRequired[str],
    ConnectionArn: NotRequired[str],
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

## ListArchivesRequestRequestTypeDef

```python
# ListArchivesRequestRequestTypeDef definition

class ListArchivesRequestRequestTypeDef(TypedDict):
    NamePrefix: NotRequired[str],
    EventSourceArn: NotRequired[str],
    State: NotRequired[ArchiveStateType],  # (1)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ArchiveStateType](./literals.md#archivestatetype) 
## ListConnectionsRequestRequestTypeDef

```python
# ListConnectionsRequestRequestTypeDef definition

class ListConnectionsRequestRequestTypeDef(TypedDict):
    NamePrefix: NotRequired[str],
    ConnectionState: NotRequired[ConnectionStateType],  # (1)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
## ListEndpointsRequestRequestTypeDef

```python
# ListEndpointsRequestRequestTypeDef definition

class ListEndpointsRequestRequestTypeDef(TypedDict):
    NamePrefix: NotRequired[str],
    HomeRegion: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListEventBusesRequestRequestTypeDef

```python
# ListEventBusesRequestRequestTypeDef definition

class ListEventBusesRequestRequestTypeDef(TypedDict):
    NamePrefix: NotRequired[str],
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

## ListEventSourcesRequestRequestTypeDef

```python
# ListEventSourcesRequestRequestTypeDef definition

class ListEventSourcesRequestRequestTypeDef(TypedDict):
    NamePrefix: NotRequired[str],
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

## ListPartnerEventSourceAccountsRequestRequestTypeDef

```python
# ListPartnerEventSourceAccountsRequestRequestTypeDef definition

class ListPartnerEventSourceAccountsRequestRequestTypeDef(TypedDict):
    EventSourceName: str,
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

## PartnerEventSourceAccountTypeDef

```python
# PartnerEventSourceAccountTypeDef definition

class PartnerEventSourceAccountTypeDef(TypedDict):
    Account: NotRequired[str],
    CreationTime: NotRequired[datetime],
    ExpirationTime: NotRequired[datetime],
    State: NotRequired[EventSourceStateType],  # (1)
```

1. See [:material-code-brackets: EventSourceStateType](./literals.md#eventsourcestatetype) 
## ListPartnerEventSourcesRequestRequestTypeDef

```python
# ListPartnerEventSourcesRequestRequestTypeDef definition

class ListPartnerEventSourcesRequestRequestTypeDef(TypedDict):
    NamePrefix: str,
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

## PartnerEventSourceTypeDef

```python
# PartnerEventSourceTypeDef definition

class PartnerEventSourceTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
```

## ListReplaysRequestRequestTypeDef

```python
# ListReplaysRequestRequestTypeDef definition

class ListReplaysRequestRequestTypeDef(TypedDict):
    NamePrefix: NotRequired[str],
    State: NotRequired[ReplayStateType],  # (1)
    EventSourceArn: NotRequired[str],
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ReplayStateType](./literals.md#replaystatetype) 
## ReplayTypeDef

```python
# ReplayTypeDef definition

class ReplayTypeDef(TypedDict):
    ReplayName: NotRequired[str],
    EventSourceArn: NotRequired[str],
    State: NotRequired[ReplayStateType],  # (1)
    StateReason: NotRequired[str],
    EventStartTime: NotRequired[datetime],
    EventEndTime: NotRequired[datetime],
    EventLastReplayedTime: NotRequired[datetime],
    ReplayStartTime: NotRequired[datetime],
    ReplayEndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ReplayStateType](./literals.md#replaystatetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListRuleNamesByTargetRequestRequestTypeDef

```python
# ListRuleNamesByTargetRequestRequestTypeDef definition

class ListRuleNamesByTargetRequestRequestTypeDef(TypedDict):
    TargetArn: str,
    EventBusName: NotRequired[str],
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

## ListRulesRequestRequestTypeDef

```python
# ListRulesRequestRequestTypeDef definition

class ListRulesRequestRequestTypeDef(TypedDict):
    NamePrefix: NotRequired[str],
    EventBusName: NotRequired[str],
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    EventPattern: NotRequired[str],
    State: NotRequired[RuleStateType],  # (1)
    Description: NotRequired[str],
    ScheduleExpression: NotRequired[str],
    RoleArn: NotRequired[str],
    ManagedBy: NotRequired[str],
    EventBusName: NotRequired[str],
```

1. See [:material-code-brackets: RuleStateType](./literals.md#rulestatetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## ListTargetsByRuleRequestRequestTypeDef

```python
# ListTargetsByRuleRequestRequestTypeDef definition

class ListTargetsByRuleRequestRequestTypeDef(TypedDict):
    Rule: str,
    EventBusName: NotRequired[str],
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

## PutEventsResultEntryTypeDef

```python
# PutEventsResultEntryTypeDef definition

class PutEventsResultEntryTypeDef(TypedDict):
    EventId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## PutPartnerEventsResultEntryTypeDef

```python
# PutPartnerEventsResultEntryTypeDef definition

class PutPartnerEventsResultEntryTypeDef(TypedDict):
    EventId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## PutTargetsResultEntryTypeDef

```python
# PutTargetsResultEntryTypeDef definition

class PutTargetsResultEntryTypeDef(TypedDict):
    TargetId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## RedshiftDataParametersTypeDef

```python
# RedshiftDataParametersTypeDef definition

class RedshiftDataParametersTypeDef(TypedDict):
    Database: str,
    SecretManagerArn: NotRequired[str],
    DbUser: NotRequired[str],
    Sql: NotRequired[str],
    StatementName: NotRequired[str],
    WithEvent: NotRequired[bool],
    Sqls: NotRequired[List[str]],
```

## RemovePermissionRequestRequestTypeDef

```python
# RemovePermissionRequestRequestTypeDef definition

class RemovePermissionRequestRequestTypeDef(TypedDict):
    StatementId: NotRequired[str],
    RemoveAllPermissions: NotRequired[bool],
    EventBusName: NotRequired[str],
```

## RemoveTargetsRequestRequestTypeDef

```python
# RemoveTargetsRequestRequestTypeDef definition

class RemoveTargetsRequestRequestTypeDef(TypedDict):
    Rule: str,
    Ids: Sequence[str],
    EventBusName: NotRequired[str],
    Force: NotRequired[bool],
```

## RemoveTargetsResultEntryTypeDef

```python
# RemoveTargetsResultEntryTypeDef definition

class RemoveTargetsResultEntryTypeDef(TypedDict):
    TargetId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## RetryPolicyTypeDef

```python
# RetryPolicyTypeDef definition

class RetryPolicyTypeDef(TypedDict):
    MaximumRetryAttempts: NotRequired[int],
    MaximumEventAgeInSeconds: NotRequired[int],
```

## RunCommandTargetTypeDef

```python
# RunCommandTargetTypeDef definition

class RunCommandTargetTypeDef(TypedDict):
    Key: str,
    Values: List[str],
```

## SageMakerPipelineParameterTypeDef

```python
# SageMakerPipelineParameterTypeDef definition

class SageMakerPipelineParameterTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## SqsParametersTypeDef

```python
# SqsParametersTypeDef definition

class SqsParametersTypeDef(TypedDict):
    MessageGroupId: NotRequired[str],
```

## TestEventPatternRequestRequestTypeDef

```python
# TestEventPatternRequestRequestTypeDef definition

class TestEventPatternRequestRequestTypeDef(TypedDict):
    EventPattern: str,
    Event: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateApiDestinationRequestRequestTypeDef

```python
# UpdateApiDestinationRequestRequestTypeDef definition

class UpdateApiDestinationRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    ConnectionArn: NotRequired[str],
    InvocationEndpoint: NotRequired[str],
    HttpMethod: NotRequired[ApiDestinationHttpMethodType],  # (1)
    InvocationRateLimitPerSecond: NotRequired[int],
```

1. See [:material-code-brackets: ApiDestinationHttpMethodType](./literals.md#apidestinationhttpmethodtype) 
## UpdateArchiveRequestRequestTypeDef

```python
# UpdateArchiveRequestRequestTypeDef definition

class UpdateArchiveRequestRequestTypeDef(TypedDict):
    ArchiveName: str,
    Description: NotRequired[str],
    EventPattern: NotRequired[str],
    RetentionDays: NotRequired[int],
```

## UpdateConnectionApiKeyAuthRequestParametersTypeDef

```python
# UpdateConnectionApiKeyAuthRequestParametersTypeDef definition

class UpdateConnectionApiKeyAuthRequestParametersTypeDef(TypedDict):
    ApiKeyName: NotRequired[str],
    ApiKeyValue: NotRequired[str],
```

## UpdateConnectionBasicAuthRequestParametersTypeDef

```python
# UpdateConnectionBasicAuthRequestParametersTypeDef definition

class UpdateConnectionBasicAuthRequestParametersTypeDef(TypedDict):
    Username: NotRequired[str],
    Password: NotRequired[str],
```

## UpdateConnectionOAuthClientRequestParametersTypeDef

```python
# UpdateConnectionOAuthClientRequestParametersTypeDef definition

class UpdateConnectionOAuthClientRequestParametersTypeDef(TypedDict):
    ClientID: NotRequired[str],
    ClientSecret: NotRequired[str],
```

## NetworkConfigurationTypeDef

```python
# NetworkConfigurationTypeDef definition

class NetworkConfigurationTypeDef(TypedDict):
    awsvpcConfiguration: NotRequired[AwsVpcConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: AwsVpcConfigurationTypeDef](./type_defs.md#awsvpcconfigurationtypedef) 
## BatchParametersTypeDef

```python
# BatchParametersTypeDef definition

class BatchParametersTypeDef(TypedDict):
    JobDefinition: str,
    JobName: str,
    ArrayProperties: NotRequired[BatchArrayPropertiesTypeDef],  # (1)
    RetryStrategy: NotRequired[BatchRetryStrategyTypeDef],  # (2)
```

1. See [:material-code-braces: BatchArrayPropertiesTypeDef](./type_defs.md#batcharraypropertiestypedef) 
2. See [:material-code-braces: BatchRetryStrategyTypeDef](./type_defs.md#batchretrystrategytypedef) 
## CancelReplayResponseTypeDef

```python
# CancelReplayResponseTypeDef definition

class CancelReplayResponseTypeDef(TypedDict):
    ReplayArn: str,
    State: ReplayStateType,  # (1)
    StateReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReplayStateType](./literals.md#replaystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApiDestinationResponseTypeDef

```python
# CreateApiDestinationResponseTypeDef definition

class CreateApiDestinationResponseTypeDef(TypedDict):
    ApiDestinationArn: str,
    ApiDestinationState: ApiDestinationStateType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ApiDestinationStateType](./literals.md#apidestinationstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateArchiveResponseTypeDef

```python
# CreateArchiveResponseTypeDef definition

class CreateArchiveResponseTypeDef(TypedDict):
    ArchiveArn: str,
    State: ArchiveStateType,  # (1)
    StateReason: str,
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ArchiveStateType](./literals.md#archivestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConnectionResponseTypeDef

```python
# CreateConnectionResponseTypeDef definition

class CreateConnectionResponseTypeDef(TypedDict):
    ConnectionArn: str,
    ConnectionState: ConnectionStateType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEventBusResponseTypeDef

```python
# CreateEventBusResponseTypeDef definition

class CreateEventBusResponseTypeDef(TypedDict):
    EventBusArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePartnerEventSourceResponseTypeDef

```python
# CreatePartnerEventSourceResponseTypeDef definition

class CreatePartnerEventSourceResponseTypeDef(TypedDict):
    EventSourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeauthorizeConnectionResponseTypeDef

```python
# DeauthorizeConnectionResponseTypeDef definition

class DeauthorizeConnectionResponseTypeDef(TypedDict):
    ConnectionArn: str,
    ConnectionState: ConnectionStateType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    LastAuthorizedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteConnectionResponseTypeDef

```python
# DeleteConnectionResponseTypeDef definition

class DeleteConnectionResponseTypeDef(TypedDict):
    ConnectionArn: str,
    ConnectionState: ConnectionStateType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    LastAuthorizedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApiDestinationResponseTypeDef

```python
# DescribeApiDestinationResponseTypeDef definition

class DescribeApiDestinationResponseTypeDef(TypedDict):
    ApiDestinationArn: str,
    Name: str,
    Description: str,
    ApiDestinationState: ApiDestinationStateType,  # (1)
    ConnectionArn: str,
    InvocationEndpoint: str,
    HttpMethod: ApiDestinationHttpMethodType,  # (2)
    InvocationRateLimitPerSecond: int,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ApiDestinationStateType](./literals.md#apidestinationstatetype) 
2. See [:material-code-brackets: ApiDestinationHttpMethodType](./literals.md#apidestinationhttpmethodtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeArchiveResponseTypeDef

```python
# DescribeArchiveResponseTypeDef definition

class DescribeArchiveResponseTypeDef(TypedDict):
    ArchiveArn: str,
    ArchiveName: str,
    EventSourceArn: str,
    Description: str,
    EventPattern: str,
    State: ArchiveStateType,  # (1)
    StateReason: str,
    RetentionDays: int,
    SizeBytes: int,
    EventCount: int,
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ArchiveStateType](./literals.md#archivestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventBusResponseTypeDef

```python
# DescribeEventBusResponseTypeDef definition

class DescribeEventBusResponseTypeDef(TypedDict):
    Name: str,
    Arn: str,
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEventSourceResponseTypeDef

```python
# DescribeEventSourceResponseTypeDef definition

class DescribeEventSourceResponseTypeDef(TypedDict):
    Arn: str,
    CreatedBy: str,
    CreationTime: datetime,
    ExpirationTime: datetime,
    Name: str,
    State: EventSourceStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EventSourceStateType](./literals.md#eventsourcestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePartnerEventSourceResponseTypeDef

```python
# DescribePartnerEventSourceResponseTypeDef definition

class DescribePartnerEventSourceResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRuleResponseTypeDef

```python
# DescribeRuleResponseTypeDef definition

class DescribeRuleResponseTypeDef(TypedDict):
    Name: str,
    Arn: str,
    EventPattern: str,
    ScheduleExpression: str,
    State: RuleStateType,  # (1)
    Description: str,
    RoleArn: str,
    ManagedBy: str,
    EventBusName: str,
    CreatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RuleStateType](./literals.md#rulestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApiDestinationsResponseTypeDef

```python
# ListApiDestinationsResponseTypeDef definition

class ListApiDestinationsResponseTypeDef(TypedDict):
    ApiDestinations: List[ApiDestinationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApiDestinationTypeDef](./type_defs.md#apidestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListArchivesResponseTypeDef

```python
# ListArchivesResponseTypeDef definition

class ListArchivesResponseTypeDef(TypedDict):
    Archives: List[ArchiveTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ArchiveTypeDef](./type_defs.md#archivetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRuleNamesByTargetResponseTypeDef

```python
# ListRuleNamesByTargetResponseTypeDef definition

class ListRuleNamesByTargetResponseTypeDef(TypedDict):
    RuleNames: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRuleResponseTypeDef

```python
# PutRuleResponseTypeDef definition

class PutRuleResponseTypeDef(TypedDict):
    RuleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartReplayResponseTypeDef

```python
# StartReplayResponseTypeDef definition

class StartReplayResponseTypeDef(TypedDict):
    ReplayArn: str,
    State: ReplayStateType,  # (1)
    StateReason: str,
    ReplayStartTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ReplayStateType](./literals.md#replaystatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestEventPatternResponseTypeDef

```python
# TestEventPatternResponseTypeDef definition

class TestEventPatternResponseTypeDef(TypedDict):
    Result: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApiDestinationResponseTypeDef

```python
# UpdateApiDestinationResponseTypeDef definition

class UpdateApiDestinationResponseTypeDef(TypedDict):
    ApiDestinationArn: str,
    ApiDestinationState: ApiDestinationStateType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ApiDestinationStateType](./literals.md#apidestinationstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateArchiveResponseTypeDef

```python
# UpdateArchiveResponseTypeDef definition

class UpdateArchiveResponseTypeDef(TypedDict):
    ArchiveArn: str,
    State: ArchiveStateType,  # (1)
    StateReason: str,
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ArchiveStateType](./literals.md#archivestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConnectionResponseTypeDef

```python
# UpdateConnectionResponseTypeDef definition

class UpdateConnectionResponseTypeDef(TypedDict):
    ConnectionArn: str,
    ConnectionState: ConnectionStateType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    LastAuthorizedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPermissionRequestRequestTypeDef

```python
# PutPermissionRequestRequestTypeDef definition

class PutPermissionRequestRequestTypeDef(TypedDict):
    EventBusName: NotRequired[str],
    Action: NotRequired[str],
    Principal: NotRequired[str],
    StatementId: NotRequired[str],
    Condition: NotRequired[ConditionTypeDef],  # (1)
    Policy: NotRequired[str],
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
## ConnectionHttpParametersTypeDef

```python
# ConnectionHttpParametersTypeDef definition

class ConnectionHttpParametersTypeDef(TypedDict):
    HeaderParameters: NotRequired[Sequence[ConnectionHeaderParameterTypeDef]],  # (1)
    QueryStringParameters: NotRequired[Sequence[ConnectionQueryStringParameterTypeDef]],  # (2)
    BodyParameters: NotRequired[Sequence[ConnectionBodyParameterTypeDef]],  # (3)
```

1. See [:material-code-braces: ConnectionHeaderParameterTypeDef](./type_defs.md#connectionheaderparametertypedef) 
2. See [:material-code-braces: ConnectionQueryStringParameterTypeDef](./type_defs.md#connectionquerystringparametertypedef) 
3. See [:material-code-braces: ConnectionBodyParameterTypeDef](./type_defs.md#connectionbodyparametertypedef) 
## ListConnectionsResponseTypeDef

```python
# ListConnectionsResponseTypeDef definition

class ListConnectionsResponseTypeDef(TypedDict):
    Connections: List[ConnectionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEventBusRequestRequestTypeDef

```python
# CreateEventBusRequestRequestTypeDef definition

class CreateEventBusRequestRequestTypeDef(TypedDict):
    Name: str,
    EventSourceName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRuleRequestRequestTypeDef

```python
# PutRuleRequestRequestTypeDef definition

class PutRuleRequestRequestTypeDef(TypedDict):
    Name: str,
    ScheduleExpression: NotRequired[str],
    EventPattern: NotRequired[str],
    State: NotRequired[RuleStateType],  # (1)
    Description: NotRequired[str],
    RoleArn: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    EventBusName: NotRequired[str],
```

1. See [:material-code-brackets: RuleStateType](./literals.md#rulestatetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeReplayResponseTypeDef

```python
# DescribeReplayResponseTypeDef definition

class DescribeReplayResponseTypeDef(TypedDict):
    ReplayName: str,
    ReplayArn: str,
    Description: str,
    State: ReplayStateType,  # (1)
    StateReason: str,
    EventSourceArn: str,
    Destination: ReplayDestinationTypeDef,  # (2)
    EventStartTime: datetime,
    EventEndTime: datetime,
    EventLastReplayedTime: datetime,
    ReplayStartTime: datetime,
    ReplayEndTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ReplayStateType](./literals.md#replaystatetype) 
2. See [:material-code-braces: ReplayDestinationTypeDef](./type_defs.md#replaydestinationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventBusesResponseTypeDef

```python
# ListEventBusesResponseTypeDef definition

class ListEventBusesResponseTypeDef(TypedDict):
    EventBuses: List[EventBusTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventBusTypeDef](./type_defs.md#eventbustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventSourcesResponseTypeDef

```python
# ListEventSourcesResponseTypeDef definition

class ListEventSourcesResponseTypeDef(TypedDict):
    EventSources: List[EventSourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventSourceTypeDef](./type_defs.md#eventsourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailoverConfigTypeDef

```python
# FailoverConfigTypeDef definition

class FailoverConfigTypeDef(TypedDict):
    Primary: PrimaryTypeDef,  # (1)
    Secondary: SecondaryTypeDef,  # (2)
```

1. See [:material-code-braces: PrimaryTypeDef](./type_defs.md#primarytypedef) 
2. See [:material-code-braces: SecondaryTypeDef](./type_defs.md#secondarytypedef) 
## ListPartnerEventSourceAccountsResponseTypeDef

```python
# ListPartnerEventSourceAccountsResponseTypeDef definition

class ListPartnerEventSourceAccountsResponseTypeDef(TypedDict):
    PartnerEventSourceAccounts: List[PartnerEventSourceAccountTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartnerEventSourceAccountTypeDef](./type_defs.md#partnereventsourceaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPartnerEventSourcesResponseTypeDef

```python
# ListPartnerEventSourcesResponseTypeDef definition

class ListPartnerEventSourcesResponseTypeDef(TypedDict):
    PartnerEventSources: List[PartnerEventSourceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartnerEventSourceTypeDef](./type_defs.md#partnereventsourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReplaysResponseTypeDef

```python
# ListReplaysResponseTypeDef definition

class ListReplaysResponseTypeDef(TypedDict):
    Replays: List[ReplayTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplayTypeDef](./type_defs.md#replaytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef

```python
# ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef definition

class ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef(TypedDict):
    TargetArn: str,
    EventBusName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesRequestListRulesPaginateTypeDef

```python
# ListRulesRequestListRulesPaginateTypeDef definition

class ListRulesRequestListRulesPaginateTypeDef(TypedDict):
    NamePrefix: NotRequired[str],
    EventBusName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef

```python
# ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef definition

class ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef(TypedDict):
    Rule: str,
    EventBusName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesResponseTypeDef

```python
# ListRulesResponseTypeDef definition

class ListRulesResponseTypeDef(TypedDict):
    Rules: List[RuleTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEventsRequestEntryTypeDef

```python
# PutEventsRequestEntryTypeDef definition

class PutEventsRequestEntryTypeDef(TypedDict):
    Time: NotRequired[Union[datetime, str]],
    Source: NotRequired[str],
    Resources: NotRequired[Sequence[str]],
    DetailType: NotRequired[str],
    Detail: NotRequired[str],
    EventBusName: NotRequired[str],
    TraceHeader: NotRequired[str],
```

## PutPartnerEventsRequestEntryTypeDef

```python
# PutPartnerEventsRequestEntryTypeDef definition

class PutPartnerEventsRequestEntryTypeDef(TypedDict):
    Time: NotRequired[Union[datetime, str]],
    Source: NotRequired[str],
    Resources: NotRequired[Sequence[str]],
    DetailType: NotRequired[str],
    Detail: NotRequired[str],
```

## StartReplayRequestRequestTypeDef

```python
# StartReplayRequestRequestTypeDef definition

class StartReplayRequestRequestTypeDef(TypedDict):
    ReplayName: str,
    EventSourceArn: str,
    EventStartTime: Union[datetime, str],
    EventEndTime: Union[datetime, str],
    Destination: ReplayDestinationTypeDef,  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ReplayDestinationTypeDef](./type_defs.md#replaydestinationtypedef) 
## PutEventsResponseTypeDef

```python
# PutEventsResponseTypeDef definition

class PutEventsResponseTypeDef(TypedDict):
    FailedEntryCount: int,
    Entries: List[PutEventsResultEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PutEventsResultEntryTypeDef](./type_defs.md#puteventsresultentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPartnerEventsResponseTypeDef

```python
# PutPartnerEventsResponseTypeDef definition

class PutPartnerEventsResponseTypeDef(TypedDict):
    FailedEntryCount: int,
    Entries: List[PutPartnerEventsResultEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PutPartnerEventsResultEntryTypeDef](./type_defs.md#putpartnereventsresultentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutTargetsResponseTypeDef

```python
# PutTargetsResponseTypeDef definition

class PutTargetsResponseTypeDef(TypedDict):
    FailedEntryCount: int,
    FailedEntries: List[PutTargetsResultEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PutTargetsResultEntryTypeDef](./type_defs.md#puttargetsresultentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveTargetsResponseTypeDef

```python
# RemoveTargetsResponseTypeDef definition

class RemoveTargetsResponseTypeDef(TypedDict):
    FailedEntryCount: int,
    FailedEntries: List[RemoveTargetsResultEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RemoveTargetsResultEntryTypeDef](./type_defs.md#removetargetsresultentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunCommandParametersTypeDef

```python
# RunCommandParametersTypeDef definition

class RunCommandParametersTypeDef(TypedDict):
    RunCommandTargets: List[RunCommandTargetTypeDef],  # (1)
```

1. See [:material-code-braces: RunCommandTargetTypeDef](./type_defs.md#runcommandtargettypedef) 
## SageMakerPipelineParametersTypeDef

```python
# SageMakerPipelineParametersTypeDef definition

class SageMakerPipelineParametersTypeDef(TypedDict):
    PipelineParameterList: NotRequired[List[SageMakerPipelineParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: SageMakerPipelineParameterTypeDef](./type_defs.md#sagemakerpipelineparametertypedef) 
## EcsParametersTypeDef

```python
# EcsParametersTypeDef definition

class EcsParametersTypeDef(TypedDict):
    TaskDefinitionArn: str,
    TaskCount: NotRequired[int],
    LaunchType: NotRequired[LaunchTypeType],  # (1)
    NetworkConfiguration: NotRequired[NetworkConfigurationTypeDef],  # (2)
    PlatformVersion: NotRequired[str],
    Group: NotRequired[str],
    CapacityProviderStrategy: NotRequired[List[CapacityProviderStrategyItemTypeDef]],  # (3)
    EnableECSManagedTags: NotRequired[bool],
    EnableExecuteCommand: NotRequired[bool],
    PlacementConstraints: NotRequired[List[PlacementConstraintTypeDef]],  # (4)
    PlacementStrategy: NotRequired[List[PlacementStrategyTypeDef]],  # (5)
    PropagateTags: NotRequired[PropagateTagsType],  # (6)
    ReferenceId: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (7)
```

1. See [:material-code-brackets: LaunchTypeType](./literals.md#launchtypetype) 
2. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef) 
3. See [:material-code-braces: CapacityProviderStrategyItemTypeDef](./type_defs.md#capacityproviderstrategyitemtypedef) 
4. See [:material-code-braces: PlacementConstraintTypeDef](./type_defs.md#placementconstrainttypedef) 
5. See [:material-code-braces: PlacementStrategyTypeDef](./type_defs.md#placementstrategytypedef) 
6. See [:material-code-brackets: PropagateTagsType](./literals.md#propagatetagstype) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ConnectionOAuthResponseParametersTypeDef

```python
# ConnectionOAuthResponseParametersTypeDef definition

class ConnectionOAuthResponseParametersTypeDef(TypedDict):
    ClientParameters: NotRequired[ConnectionOAuthClientResponseParametersTypeDef],  # (1)
    AuthorizationEndpoint: NotRequired[str],
    HttpMethod: NotRequired[ConnectionOAuthHttpMethodType],  # (2)
    OAuthHttpParameters: NotRequired[ConnectionHttpParametersTypeDef],  # (3)
```

1. See [:material-code-braces: ConnectionOAuthClientResponseParametersTypeDef](./type_defs.md#connectionoauthclientresponseparameterstypedef) 
2. See [:material-code-brackets: ConnectionOAuthHttpMethodType](./literals.md#connectionoauthhttpmethodtype) 
3. See [:material-code-braces: ConnectionHttpParametersTypeDef](./type_defs.md#connectionhttpparameterstypedef) 
## CreateConnectionOAuthRequestParametersTypeDef

```python
# CreateConnectionOAuthRequestParametersTypeDef definition

class CreateConnectionOAuthRequestParametersTypeDef(TypedDict):
    ClientParameters: CreateConnectionOAuthClientRequestParametersTypeDef,  # (1)
    AuthorizationEndpoint: str,
    HttpMethod: ConnectionOAuthHttpMethodType,  # (2)
    OAuthHttpParameters: NotRequired[ConnectionHttpParametersTypeDef],  # (3)
```

1. See [:material-code-braces: CreateConnectionOAuthClientRequestParametersTypeDef](./type_defs.md#createconnectionoauthclientrequestparameterstypedef) 
2. See [:material-code-brackets: ConnectionOAuthHttpMethodType](./literals.md#connectionoauthhttpmethodtype) 
3. See [:material-code-braces: ConnectionHttpParametersTypeDef](./type_defs.md#connectionhttpparameterstypedef) 
## UpdateConnectionOAuthRequestParametersTypeDef

```python
# UpdateConnectionOAuthRequestParametersTypeDef definition

class UpdateConnectionOAuthRequestParametersTypeDef(TypedDict):
    ClientParameters: NotRequired[UpdateConnectionOAuthClientRequestParametersTypeDef],  # (1)
    AuthorizationEndpoint: NotRequired[str],
    HttpMethod: NotRequired[ConnectionOAuthHttpMethodType],  # (2)
    OAuthHttpParameters: NotRequired[ConnectionHttpParametersTypeDef],  # (3)
```

1. See [:material-code-braces: UpdateConnectionOAuthClientRequestParametersTypeDef](./type_defs.md#updateconnectionoauthclientrequestparameterstypedef) 
2. See [:material-code-brackets: ConnectionOAuthHttpMethodType](./literals.md#connectionoauthhttpmethodtype) 
3. See [:material-code-braces: ConnectionHttpParametersTypeDef](./type_defs.md#connectionhttpparameterstypedef) 
## RoutingConfigTypeDef

```python
# RoutingConfigTypeDef definition

class RoutingConfigTypeDef(TypedDict):
    FailoverConfig: FailoverConfigTypeDef,  # (1)
```

1. See [:material-code-braces: FailoverConfigTypeDef](./type_defs.md#failoverconfigtypedef) 
## PutEventsRequestRequestTypeDef

```python
# PutEventsRequestRequestTypeDef definition

class PutEventsRequestRequestTypeDef(TypedDict):
    Entries: Sequence[PutEventsRequestEntryTypeDef],  # (1)
    EndpointId: NotRequired[str],
```

1. See [:material-code-braces: PutEventsRequestEntryTypeDef](./type_defs.md#puteventsrequestentrytypedef) 
## PutPartnerEventsRequestRequestTypeDef

```python
# PutPartnerEventsRequestRequestTypeDef definition

class PutPartnerEventsRequestRequestTypeDef(TypedDict):
    Entries: Sequence[PutPartnerEventsRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: PutPartnerEventsRequestEntryTypeDef](./type_defs.md#putpartnereventsrequestentrytypedef) 
## TargetTypeDef

```python
# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    Id: str,
    Arn: str,
    RoleArn: NotRequired[str],
    Input: NotRequired[str],
    InputPath: NotRequired[str],
    InputTransformer: NotRequired[InputTransformerTypeDef],  # (1)
    KinesisParameters: NotRequired[KinesisParametersTypeDef],  # (2)
    RunCommandParameters: NotRequired[RunCommandParametersTypeDef],  # (3)
    EcsParameters: NotRequired[EcsParametersTypeDef],  # (4)
    BatchParameters: NotRequired[BatchParametersTypeDef],  # (5)
    SqsParameters: NotRequired[SqsParametersTypeDef],  # (6)
    HttpParameters: NotRequired[HttpParametersTypeDef],  # (7)
    RedshiftDataParameters: NotRequired[RedshiftDataParametersTypeDef],  # (8)
    SageMakerPipelineParameters: NotRequired[SageMakerPipelineParametersTypeDef],  # (9)
    DeadLetterConfig: NotRequired[DeadLetterConfigTypeDef],  # (10)
    RetryPolicy: NotRequired[RetryPolicyTypeDef],  # (11)
```

1. See [:material-code-braces: InputTransformerTypeDef](./type_defs.md#inputtransformertypedef) 
2. See [:material-code-braces: KinesisParametersTypeDef](./type_defs.md#kinesisparameterstypedef) 
3. See [:material-code-braces: RunCommandParametersTypeDef](./type_defs.md#runcommandparameterstypedef) 
4. See [:material-code-braces: EcsParametersTypeDef](./type_defs.md#ecsparameterstypedef) 
5. See [:material-code-braces: BatchParametersTypeDef](./type_defs.md#batchparameterstypedef) 
6. See [:material-code-braces: SqsParametersTypeDef](./type_defs.md#sqsparameterstypedef) 
7. See [:material-code-braces: HttpParametersTypeDef](./type_defs.md#httpparameterstypedef) 
8. See [:material-code-braces: RedshiftDataParametersTypeDef](./type_defs.md#redshiftdataparameterstypedef) 
9. See [:material-code-braces: SageMakerPipelineParametersTypeDef](./type_defs.md#sagemakerpipelineparameterstypedef) 
10. See [:material-code-braces: DeadLetterConfigTypeDef](./type_defs.md#deadletterconfigtypedef) 
11. See [:material-code-braces: RetryPolicyTypeDef](./type_defs.md#retrypolicytypedef) 
## ConnectionAuthResponseParametersTypeDef

```python
# ConnectionAuthResponseParametersTypeDef definition

class ConnectionAuthResponseParametersTypeDef(TypedDict):
    BasicAuthParameters: NotRequired[ConnectionBasicAuthResponseParametersTypeDef],  # (1)
    OAuthParameters: NotRequired[ConnectionOAuthResponseParametersTypeDef],  # (2)
    ApiKeyAuthParameters: NotRequired[ConnectionApiKeyAuthResponseParametersTypeDef],  # (3)
    InvocationHttpParameters: NotRequired[ConnectionHttpParametersTypeDef],  # (4)
```

1. See [:material-code-braces: ConnectionBasicAuthResponseParametersTypeDef](./type_defs.md#connectionbasicauthresponseparameterstypedef) 
2. See [:material-code-braces: ConnectionOAuthResponseParametersTypeDef](./type_defs.md#connectionoauthresponseparameterstypedef) 
3. See [:material-code-braces: ConnectionApiKeyAuthResponseParametersTypeDef](./type_defs.md#connectionapikeyauthresponseparameterstypedef) 
4. See [:material-code-braces: ConnectionHttpParametersTypeDef](./type_defs.md#connectionhttpparameterstypedef) 
## CreateConnectionAuthRequestParametersTypeDef

```python
# CreateConnectionAuthRequestParametersTypeDef definition

class CreateConnectionAuthRequestParametersTypeDef(TypedDict):
    BasicAuthParameters: NotRequired[CreateConnectionBasicAuthRequestParametersTypeDef],  # (1)
    OAuthParameters: NotRequired[CreateConnectionOAuthRequestParametersTypeDef],  # (2)
    ApiKeyAuthParameters: NotRequired[CreateConnectionApiKeyAuthRequestParametersTypeDef],  # (3)
    InvocationHttpParameters: NotRequired[ConnectionHttpParametersTypeDef],  # (4)
```

1. See [:material-code-braces: CreateConnectionBasicAuthRequestParametersTypeDef](./type_defs.md#createconnectionbasicauthrequestparameterstypedef) 
2. See [:material-code-braces: CreateConnectionOAuthRequestParametersTypeDef](./type_defs.md#createconnectionoauthrequestparameterstypedef) 
3. See [:material-code-braces: CreateConnectionApiKeyAuthRequestParametersTypeDef](./type_defs.md#createconnectionapikeyauthrequestparameterstypedef) 
4. See [:material-code-braces: ConnectionHttpParametersTypeDef](./type_defs.md#connectionhttpparameterstypedef) 
## UpdateConnectionAuthRequestParametersTypeDef

```python
# UpdateConnectionAuthRequestParametersTypeDef definition

class UpdateConnectionAuthRequestParametersTypeDef(TypedDict):
    BasicAuthParameters: NotRequired[UpdateConnectionBasicAuthRequestParametersTypeDef],  # (1)
    OAuthParameters: NotRequired[UpdateConnectionOAuthRequestParametersTypeDef],  # (2)
    ApiKeyAuthParameters: NotRequired[UpdateConnectionApiKeyAuthRequestParametersTypeDef],  # (3)
    InvocationHttpParameters: NotRequired[ConnectionHttpParametersTypeDef],  # (4)
```

1. See [:material-code-braces: UpdateConnectionBasicAuthRequestParametersTypeDef](./type_defs.md#updateconnectionbasicauthrequestparameterstypedef) 
2. See [:material-code-braces: UpdateConnectionOAuthRequestParametersTypeDef](./type_defs.md#updateconnectionoauthrequestparameterstypedef) 
3. See [:material-code-braces: UpdateConnectionApiKeyAuthRequestParametersTypeDef](./type_defs.md#updateconnectionapikeyauthrequestparameterstypedef) 
4. See [:material-code-braces: ConnectionHttpParametersTypeDef](./type_defs.md#connectionhttpparameterstypedef) 
## CreateEndpointRequestRequestTypeDef

```python
# CreateEndpointRequestRequestTypeDef definition

class CreateEndpointRequestRequestTypeDef(TypedDict):
    Name: str,
    RoutingConfig: RoutingConfigTypeDef,  # (1)
    EventBuses: Sequence[EndpointEventBusTypeDef],  # (2)
    Description: NotRequired[str],
    ReplicationConfig: NotRequired[ReplicationConfigTypeDef],  # (3)
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: RoutingConfigTypeDef](./type_defs.md#routingconfigtypedef) 
2. See [:material-code-braces: EndpointEventBusTypeDef](./type_defs.md#endpointeventbustypedef) 
3. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
## CreateEndpointResponseTypeDef

```python
# CreateEndpointResponseTypeDef definition

class CreateEndpointResponseTypeDef(TypedDict):
    Name: str,
    Arn: str,
    RoutingConfig: RoutingConfigTypeDef,  # (1)
    ReplicationConfig: ReplicationConfigTypeDef,  # (2)
    EventBuses: List[EndpointEventBusTypeDef],  # (3)
    RoleArn: str,
    State: EndpointStateType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: RoutingConfigTypeDef](./type_defs.md#routingconfigtypedef) 
2. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
3. See [:material-code-braces: EndpointEventBusTypeDef](./type_defs.md#endpointeventbustypedef) 
4. See [:material-code-brackets: EndpointStateType](./literals.md#endpointstatetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointResponseTypeDef

```python
# DescribeEndpointResponseTypeDef definition

class DescribeEndpointResponseTypeDef(TypedDict):
    Name: str,
    Description: str,
    Arn: str,
    RoutingConfig: RoutingConfigTypeDef,  # (1)
    ReplicationConfig: ReplicationConfigTypeDef,  # (2)
    EventBuses: List[EndpointEventBusTypeDef],  # (3)
    RoleArn: str,
    EndpointId: str,
    EndpointUrl: str,
    State: EndpointStateType,  # (4)
    StateReason: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: RoutingConfigTypeDef](./type_defs.md#routingconfigtypedef) 
2. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
3. See [:material-code-braces: EndpointEventBusTypeDef](./type_defs.md#endpointeventbustypedef) 
4. See [:material-code-brackets: EndpointStateType](./literals.md#endpointstatetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    Arn: NotRequired[str],
    RoutingConfig: NotRequired[RoutingConfigTypeDef],  # (1)
    ReplicationConfig: NotRequired[ReplicationConfigTypeDef],  # (2)
    EventBuses: NotRequired[List[EndpointEventBusTypeDef]],  # (3)
    RoleArn: NotRequired[str],
    EndpointId: NotRequired[str],
    EndpointUrl: NotRequired[str],
    State: NotRequired[EndpointStateType],  # (4)
    StateReason: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-braces: RoutingConfigTypeDef](./type_defs.md#routingconfigtypedef) 
2. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
3. See [:material-code-braces: EndpointEventBusTypeDef](./type_defs.md#endpointeventbustypedef) 
4. See [:material-code-brackets: EndpointStateType](./literals.md#endpointstatetype) 
## UpdateEndpointRequestRequestTypeDef

```python
# UpdateEndpointRequestRequestTypeDef definition

class UpdateEndpointRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    RoutingConfig: NotRequired[RoutingConfigTypeDef],  # (1)
    ReplicationConfig: NotRequired[ReplicationConfigTypeDef],  # (2)
    EventBuses: NotRequired[Sequence[EndpointEventBusTypeDef]],  # (3)
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: RoutingConfigTypeDef](./type_defs.md#routingconfigtypedef) 
2. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
3. See [:material-code-braces: EndpointEventBusTypeDef](./type_defs.md#endpointeventbustypedef) 
## UpdateEndpointResponseTypeDef

```python
# UpdateEndpointResponseTypeDef definition

class UpdateEndpointResponseTypeDef(TypedDict):
    Name: str,
    Arn: str,
    RoutingConfig: RoutingConfigTypeDef,  # (1)
    ReplicationConfig: ReplicationConfigTypeDef,  # (2)
    EventBuses: List[EndpointEventBusTypeDef],  # (3)
    RoleArn: str,
    EndpointId: str,
    EndpointUrl: str,
    State: EndpointStateType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: RoutingConfigTypeDef](./type_defs.md#routingconfigtypedef) 
2. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
3. See [:material-code-braces: EndpointEventBusTypeDef](./type_defs.md#endpointeventbustypedef) 
4. See [:material-code-brackets: EndpointStateType](./literals.md#endpointstatetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTargetsByRuleResponseTypeDef

```python
# ListTargetsByRuleResponseTypeDef definition

class ListTargetsByRuleResponseTypeDef(TypedDict):
    Targets: List[TargetTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutTargetsRequestRequestTypeDef

```python
# PutTargetsRequestRequestTypeDef definition

class PutTargetsRequestRequestTypeDef(TypedDict):
    Rule: str,
    Targets: Sequence[TargetTypeDef],  # (1)
    EventBusName: NotRequired[str],
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## DescribeConnectionResponseTypeDef

```python
# DescribeConnectionResponseTypeDef definition

class DescribeConnectionResponseTypeDef(TypedDict):
    ConnectionArn: str,
    Name: str,
    Description: str,
    ConnectionState: ConnectionStateType,  # (1)
    StateReason: str,
    AuthorizationType: ConnectionAuthorizationTypeType,  # (2)
    SecretArn: str,
    AuthParameters: ConnectionAuthResponseParametersTypeDef,  # (3)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    LastAuthorizedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
2. See [:material-code-brackets: ConnectionAuthorizationTypeType](./literals.md#connectionauthorizationtypetype) 
3. See [:material-code-braces: ConnectionAuthResponseParametersTypeDef](./type_defs.md#connectionauthresponseparameterstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConnectionRequestRequestTypeDef

```python
# CreateConnectionRequestRequestTypeDef definition

class CreateConnectionRequestRequestTypeDef(TypedDict):
    Name: str,
    AuthorizationType: ConnectionAuthorizationTypeType,  # (1)
    AuthParameters: CreateConnectionAuthRequestParametersTypeDef,  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ConnectionAuthorizationTypeType](./literals.md#connectionauthorizationtypetype) 
2. See [:material-code-braces: CreateConnectionAuthRequestParametersTypeDef](./type_defs.md#createconnectionauthrequestparameterstypedef) 
## UpdateConnectionRequestRequestTypeDef

```python
# UpdateConnectionRequestRequestTypeDef definition

class UpdateConnectionRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    AuthorizationType: NotRequired[ConnectionAuthorizationTypeType],  # (1)
    AuthParameters: NotRequired[UpdateConnectionAuthRequestParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: ConnectionAuthorizationTypeType](./literals.md#connectionauthorizationtypetype) 
2. See [:material-code-braces: UpdateConnectionAuthRequestParametersTypeDef](./type_defs.md#updateconnectionauthrequestparameterstypedef) 
## ListEndpointsResponseTypeDef

```python
# ListEndpointsResponseTypeDef definition

class ListEndpointsResponseTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
